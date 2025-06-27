# Virginia Hospital Mortality Intelligence Dashboard

A comprehensive healthcare analytics dashboard for risk-adjusted mortality analysis and quality benchmarking, built for hospital quality teams and healthcare data analysts.



## Project Overview

This dashboard addresses critical healthcare quality challenges by providing:
- **CMS Compliance**: 30-day mortality reporting for Medicare Star Ratings
- **Leapfrog Analysis**: A-F safety grade tracking and benchmarking
- **Competitive Intelligence**: Multi-hospital performance comparisons
- **Business Impact**: Revenue risk assessment ($2M+ at stake from poor ratings)


## Key Features

### Business Intelligence
- **CMS Star Ratings Impact**: Direct revenue implications tracking
- **Leapfrog Grade Distribution**: Patient safety score analysis  
- **US News Rankings**: National reputation monitoring
- **Vizient Benchmarking**: Peer hospital comparisons

### Analytics Capabilities
- Risk-adjusted mortality rates for 6 key conditions
- Volume-outcome relationship analysis
- Monthly trend tracking (Virginia vs National)
- Hospital performance rankings
- Real-time data upload and processing

### Medical Conditions Tracked
- Heart Attack (AMI)
- Heart Failure  
- Pneumonia
- Stroke
- Hip Fracture
- GI Hemorrhage

## Technical Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Visualization**: Chart.js 3.9.1
- **Data Processing**: PapaParse for CSV handling
- **Design**: Modern glassmorphism UI with gradient backgrounds
- **Responsive**: Mobile-first design approach


## Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/virginia-hospital-mortality-dashboard.git
   cd virginia-hospital-mortality-dashboard
   ```

2. **Open in browser**
   ```bash
   open index.html
   # or serve with a local server
   python -m http.server 8000
   ```

3. **Load sample data**
   - Click "Load Virginia Sample Data" for demo
   - Or upload your own CSV with hospital mortality data

## Data Format

The dashboard accepts CSV files with the following structure:

| Column | Description | Example |
|--------|-------------|---------|
| hospital | Hospital name | "Carilion Roanoke Memorial Hospital" |
| condition | Medical condition | "Heart Attack (AMI)" |
| mortalityRate | Risk-adjusted rate (%) | "6.45" |
| grade | Leapfrog grade | "A" |
| cases | Annual volume | "324" |
| deaths | Total deaths | "21" |
| benchmark | Performance vs national | "Better than National" |

## Healthcare Context

### Why This Matters
- **Patient Safety**: Direct impact on clinical outcomes
- **Financial**: Medicare reimbursements tied to quality scores
- **Reputation**: Public reporting affects patient choice
- **Regulatory**: CMS and Joint Commission requirements

### Target Users
- Hospital Quality Directors
- Chief Medical Officers  
- Healthcare Data Analysts
- Population Health Teams
- Hospital Administrators

## Customization

### Adding New Conditions
```javascript
const conditions = [
    'Heart Attack (AMI)', 
    'Heart Failure', 
    'Pneumonia',
    'Your New Condition'  // Add here
];
```

### Modifying Grade Thresholds
```javascript
// Adjust mortality rate thresholds for grades
if (mortalityRate < 5) grade = 'A';
else if (mortalityRate < 7) grade = 'B';
// Customize thresholds as needed
```

## Sample Insights

The dashboard reveals patterns like:
- **Volume-Outcome Relationships**: Higher volume hospitals often show lower mortality
- **Condition Variability**: Stroke mortality rates vary more than heart attack rates
- **Seasonal Trends**: Winter months typically show higher mortality rates
- **Competitive Positioning**: Identify improvement opportunities vs peers

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-analysis`)
3. Commit changes (`git commit -am 'Add volume prediction model'`)
4. Push to branch (`git push origin feature/new-analysis`)
5. Create a Pull Request

## License

MIT License - see [LICENSE.md](LICENSE.md) for details

## Acknowledgments

- **Healthcare Domain Knowledge**: Based on real CMS quality measures
- **Design Inspiration**: Modern healthcare dashboard UX patterns
- **Data Sources**: Simulated Virginia hospital performance data


Project Link: [https://github.com/yourusername/virginia-hospital-mortality-dashboard](https://github.com/yourusername/virginia-hospital-mortality-dashboard)

---

*Built for healthcare professionals who need actionable mortality intelligence* 
