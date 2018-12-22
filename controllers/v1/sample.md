# Sample

```JS
module.export = {
  getSamples: async (req, res) => {
    try {
      const samples = await sampleService.getSamples();
      res.status(200).json(samples);
    } catch (err) {
      res.status(400).josn({message: err.message});
    }
  }
}
```
