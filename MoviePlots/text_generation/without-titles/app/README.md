#### Usage

- Mount Google Drive on your computer
- Create `Colab Notebooks` directory and clone the textai repo there

In Google Colab,
- Run the [Data Preparation notebook](https://nbviewer.jupyter.org/github/polakowo/textai/blob/master/MoviePlots/DataPreparation.ipynb)
- Run one of the training notebooks

Then locally,
- Copy the generated `output` directory to the `app/app` directory
- Run the following commands in terminal
```
docker build -t text-generation .
docker run -p 5000:5000 text-generation
open http://localhost:5000
```

![Web app screenshot](app.png)
