# Troubleshooting

| Symptoms | Recommendation |
| -- | -- |
| Orienteer is running slow on every page  | It seems that you are running Orienteer in Standalone mode and didn't provide enough memory for the application. Please make sure that minimal [system requirements](system_requirements.md) are met. |
| Schema manipulations are slow | Congratulations with big amount of RAM on your computer! Unfortunatly, OrientDB has bug in version 2.1.x which leads to this behavior: database is syncing full memory with hard-drive and for big sizes of RAM that might be  problem. Should be fixed after switching to OrientDB 2.2.|
