# kubectl-troubleshooter

A powerful Kubernetes troubleshooting plugin that helps you diagnose and analyze issues with your pods across all namespaces.

## Features

- 🔍 Analyze pod status and health
- 🌐 Support for all namespaces
- 🚨 Detailed error reporting
- 💡 Smart suggestions for common issues
- 🎨 Colorful and intuitive output

## Installation

1. Download the `kubectl-ts` script
2. Make it executable:
```bash
chmod +x kubectl-ts
```
3. Move it to a directory in your PATH:
```bash
sudo mv kubectl-ts /usr/local/bin/
```

## Usage

```bash
# Analyze a specific pod
kubectl ts pod <pod-name> [--namespace <namespace>]

# Analyze all pods across all namespaces
kubectl ts pods --all-namespaces

# Show help
kubectl ts --help
```

### Examples

```bash
# Check a specific pod in the production namespace
kubectl ts pod my-app-pod --namespace production

# Analyze all pods across all namespaces
kubectl ts pods --all-namespaces
```

## Features in Detail

- **Pod Status Analysis**: Get detailed information about pod status and state
- **Container Details**: View container-specific information and state
- **Event Monitoring**: See recent events related to the pod
- **Restart Analysis**: Track and analyze pod restarts
- **Smart Troubleshooting**: Get targeted suggestions for common issues like ImagePullBackOff

## Output Information

The tool provides:
- Pod status and health
- Container details
- Recent events
- Restart count analysis
- Troubleshooting suggestions
- Color-coded output for better readability

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 
