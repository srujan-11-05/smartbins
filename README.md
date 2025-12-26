# Smart Bins Waste Management System

A web-based intelligent waste management system with real-time monitoring, threshold alerts, and SMS notifications for waste collection.

## Features

- **Real-time Waste Monitoring**: Track waste levels in multiple bins
- **Automatic SMS Alerts**: Send alerts when waste exceeds 150L threshold
- **Interactive Dashboard**: Beautiful responsive interface with live statistics
- **Multi-bin Management**: Monitor multiple bins with different waste types
- **Fill Level Tracking**: Visual progress indicators for each bin
- **Collection Status**: Track bin status (Low, Medium, Full)
- **Pure HTML/CSS/JS**: No backend required - runs entirely in the browser

## How It Works

1. **Input Waste Data**: Enter bin ID, waste amount (in liters), waste type, and collector phone number
2. **Automatic Threshold Monitoring**: System checks if waste >= 150L
3. **SMS Alert**: When threshold is reached, an SMS notification modal appears
4. **Live Dashboard**: Real-time updates showing:
   - Total waste collected
   - Number of active bins
   - Bins needing collection
   - SMS alerts sent

## Getting Started

1. Open `index.html` in any web browser
2. Fill in the waste data form:
   - **Bin ID**: Unique identifier (e.g., BIN_001)
   - **Total Waste**: Amount in liters (e.g., 150)
   - **Waste Type**: Select from General, Recyclable, Organic, or Hazardous
   - **Collector Phone**: Phone number to receive SMS
3. Click "Add Waste"
4. System automatically checks threshold and shows SMS alert if needed

## Project Structure

```
smart-bins/
├── index.html                 # Main HTML application
├── README.md                  # This file
└── requirements.txt           # Empty (no Python dependencies)
```

## Features Breakdown

### Dashboard Cards
- **Total Waste**: Cumulative waste from all bins
- **Active Bins**: Number of bins being monitored
- **Full Bins**: Bins exceeding 150L threshold
- **SMS Alerts**: Count of alerts sent

### Bin Status Visualization
- **Green (✅)**: Waste < 100L - Low fill level
- **Orange (🟡)**: Waste 100-149L - Medium fill level
- **Red (🔴)**: Waste ≥ 150L - Full, needs collection

### Collection Status Table
- Detailed view of each bin
- Fill percentage
- Status indicator
- Manual "Empty" button for collection tracking

## SMS Alert Details

When a bin reaches 150L threshold:
1. Modal popup appears with SMS details
2. Shows recipient, waste level, bin ID
3. Message includes waste amount and urgent collection request
4. SMS count increments on dashboard

## Usage Example

```
1. Bin ID: BIN_001
2. Waste: 150L
3. Type: General
4. Phone: +1234567890
↓
System triggers SMS Alert:
"Alert! Bin BIN_001 has reached 150L. Please empty it soon."
```

## Technologies Used

- HTML5
- CSS3 (with gradients and animations)
- Vanilla JavaScript (no frameworks)
- Responsive Design

## Browser Compatibility

Works in all modern browsers:
- Chrome/Chromium
- Firefox
- Safari
- Edge

## Key Features

- ✅ Real-time waste tracking
- ✅ Automatic SMS alerts at 150L threshold
- ✅ Beautiful responsive dashboard
- ✅ Multiple bin management
- ✅ Waste type classification
- ✅ Fill level visualization
- ✅ Collection status tracking
- ✅ Manual empty bin controls

## Notes

- SMS alerts show as popup notifications (modal)
- All data is stored in browser memory (refreshing page clears data)
- Threshold is set to 150L but can be modified in code
- Maximum bin capacity is 200L (configurable)

## License

MIT License
