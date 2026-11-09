# UTW-RG-AdaFedResidual source notebook

This repository contains the Google Colab notebook for the **UTW-RG-AdaFedResidual** study of multi-horizon alum and chlorine dose forecasting across four Baghdad drinking-water treatment plants. It includes the chronological data preparation, model comparisons, proposed federated method, and supporting evaluations.

The published notebook retains the supplied research code, except for syntax and indentation corrections in the result-export cell. Saved outputs, execution counts, and Colab widget state were removed for a smaller, safer source-code release. No datasets or cloud-control credentials are included.

## Data required

1. Download the ten primary Excel files (four station records and six supporting files) from the [Baghdad dataset on Zenodo](https://doi.org/10.5281/zenodo.22817262).
2. The external-generalization cells additionally expect prepared Austin, Tongji, Hannan, and Kirkuk Excel workbooks, and the [Digital Twin workbook](https://doi.org/10.5281/zenodo.24024238). The external source datasets are cited in the paper. The prepared external workbooks are not included in this code repository.

## Run in Google Colab

1. Open `UTW-RG-AdaFedResidual.ipynb` in Google Colab.
2. Run the first code cell and upload the ten primary Excel files when prompted.
3. Run the subsequent cells in order. Before the external-generalization cells, upload the prepared external workbooks and Digital Twin workbook to `/content`.

The notebook was designed for Google Colab. Some later cells use `/content` paths, so local Jupyter execution requires adapting those paths. The paper reports the computational environment used for its published measurements; this repository does not pin every library version.

## Related resources

- [Primary data and dosing reference tables](https://doi.org/10.5281/zenodo.22817262)
- [Digital Twin dataset](https://doi.org/10.5281/zenodo.24024238)
- [Four Wokwi station simulations and dashboard link](https://doi.org/10.5281/zenodo.24026085)

The Wokwi simulation is a complementary demonstration. Model training and evaluation use the historical datasets.
