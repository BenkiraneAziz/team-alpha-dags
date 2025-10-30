# Team Alpha DAG Configurations

This repository contains Apache Airflow DAG configurations for Team Alpha data processing workflows.

## Files

- `team_alpha_workflows.yml` - Main DAG configurations including ETL pipeline and data quality checks

## DAGs Included

### team_alpha_etl_pipeline
- **Schedule**: Daily (`@daily`)
- **Description**: Daily ETL pipeline for Team Alpha data processing
- **Tasks**: Extract → Validate → Transform → Load → Notify

### team_alpha_data_quality_check  
- **Schedule**: Every 6 hours (`0 */6 * * *`)
- **Description**: Data quality monitoring for Team Alpha datasets
- **Tasks**: Freshness Check → Volume Check → Schema Check → Generate Report

## Usage

These YAML files are automatically synchronized with the Airflow DAG Factory system. Any changes pushed to this repository will be reflected in the Airflow environment within 15 minutes.

## Team Contact

- **Team**: team-alpha@company.com
- **Owner**: Team Alpha Data Engineering

## Contributing

1. Make changes to the YAML files
2. Test configurations locally if possible
3. Commit and push changes
4. Changes will be automatically deployed to Airflow