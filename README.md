# Network Intrusion Detection System (NIDS)

A full-stack application for detecting network intrusions using binary classification.

## Features

### Front-end
- User-friendly interface for uploading and analyzing PCAP files
- Real-time network traffic monitoring
- Visualization of detection results
- Dashboard with traffic statistics and alerts

### Back-end
- Binary classification model for detecting malicious network traffic
- Feature extraction from PCAP files
- API for receiving and analyzing network traffic
- Database for storing traffic data and detection results

## Technologies Used

### Front-end
- Next.js
- React
- Tailwind CSS
- Chart.js

### Back-end
- Flask
- scikit-learn
- Scapy
- SQLite

## Getting Started

### Prerequisites
- Docker and Docker Compose
- Node.js (for local development)
- Python 3.10+ (for local development)

### Installation

1. Clone the repository:
\`\`\`bash
git clone https://github.com/yourusername/nids-system.git
cd nids-system
\`\`\`

2. Start the application using Docker Compose:
\`\`\`bash
docker-compose up
\`\`\`

3. Access the application:
   - Front-end: http://localhost:3000
   - Back-end API: http://localhost:5000/api

### Local Development

#### Front-end
\`\`\`bash
cd frontend
npm install
npm run dev
\`\`\`

#### Back-end
\`\`\`bash
cd backend
pip install -r requirements.txt
python app.py
\`\`\`

## Usage

### Uploading PCAP Files
1. Navigate to the "Upload PCAP" tab
2. Drag and drop or select a PCAP file
3. Click "Analyze Traffic" to process the file
4. View the analysis results

### Live Monitoring
1. Navigate to the "Live Monitoring" tab
2. Click "Start Monitoring" to begin real-time analysis
3. View traffic events and statistics in real-time

### Dashboard
- View overall traffic statistics
- Monitor detected threats
- Analyze traffic patterns over time

## Model Training

To train a new model:

\`\`\`bash
cd backend
python train_model.py
\`\`\`

## Security Considerations

- The application implements authentication and authorization
- All API endpoints are secured
- Input validation is performed on all user inputs
- HTTPS is recommended for production deployments

## Scalability

- The application can be scaled horizontally by deploying multiple instances
- Database can be migrated to a more robust solution like PostgreSQL
- Kubernetes can be used for orchestration in production environments

## License

This project is licensed under the MIT License - see the LICENSE file for details.
