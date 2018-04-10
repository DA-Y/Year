# Year : General Domain Adaptation Python library

Year is auto experiment library for domain adaptation in deep learning. 

## Getting started

```python
from year.util import ExperimentAll

ExperimentAll(source_data, target_data, [model], output='report') # experiment all DA models
```

experiment on single model
```python
from year.models import fine_tune, dann

fine_tune(source_data, target_data, model, freeze_layer=['fc','layer2'], output='report')
dann(source_data, target_data, output='report')
```

## Year Framwork
### Year = Interface + Models
Interface
- data distance metrics
- data loader
- record experiments
- etc

Models
- domain adaptation model

## Contributing
Add experiment model
- write on model code & (optinal) saved weight
- desribe used model (paper link & pytorch description), dataset, parameters (source-target, epoc, ...)
