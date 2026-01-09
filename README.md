# @charliekmc/fishbone-chart

> A fishbone (Ishikawa) diagram React component for root cause analysis

[![NPM](https://img.shields.io/npm/v/@charliekmc/fishbone-chart.svg)](https://www.npmjs.com/package/@charliekmc/fishbone-chart) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a>

![fishbonechart](https://user-images.githubusercontent.com/43149895/54030834-a40bb100-418b-11e9-8c41-2706b4ea0307.gif)

## Attribution

This package is a fork of [fishbone-chart](https://github.com/thiagoferrax/fishbone-chart) originally created by [Thiago Ferraz](https://github.com/thiagoferrax) ([@thiagoferrax](https://github.com/thiagoferrax)).

This fork has been updated to support React 19 and modernised dependencies.

Original work © Thiago Ferraz, licensed under the MIT Licence.

## Install

\`\`\`bash
npm install --save @charliekmc/fishbone-chart
\`\`\`

## Usage

\`\`\`jsx
import FishboneChart from '@charliekmc/fishbone-chart'

function Example() {
  const data = {
    'Bad coffee': {
      'Procedures': ['Too much water', 'Too many grounds', 'Lack of training'],
      'Equipment': ['Dirty cups', 'Coffee not hot enough', 'Dirty basket'],
      'Material': ['Bad sugar', 'Lids do not fit cup', 'Bad cream'],
      'People': ['Wrong fee', 'No training', 'Rude'],
      'Machine': ['Not working', 'Deregulated', 'Dirty']
    },
    'Scrum not working': {
      'Principles': ['Functional software (SW) is not released'],
      'Product Owner (PO)': ['No authority to prioritise', 'Poor interaction with the team'],
      'Sprint': ['SW not released for validation', 'Sprint speed is not measured', 'Team is controlled from outside'],
      'Planning': ['PO does not explain the backlog'],
      'Development Team': ['Members dedicated to specific roles', 'Does not deliver what was promised'],
    },
    'Security Incident': {
      'Technology': ['Weak encryption', 'No technology for remote data destruction'],
      'Process': ['No process for reporting incident'],
      'People': ['Worker lost laptop', 'Distraction was a factor'],
      'Controls': ['Weak password policy', 'No audit trail of the laptop information'],
      'Procedure': ['No procedure for securing laptop at public locations'],
      'Environment': ['No place to secure laptop overnight at workplace']
    }
  }

  return (
    <FishboneChart data={data} />
  )
}
\`\`\`

## Licence

MIT © [Charlie McMahon](https://github.com/charliekmc)

Original work MIT © [Thiago Ferraz](https://github.com/thiagoferrax)
