# Cosmos-Chains-Sync
## Example for change the addrbook

sudo systemctl stop strided
rm $HOME/.stride/config/addrbook.json
wget -O $HOME/.stride/config/addrbook.json "https://raw.githubusercontent.com/BadaBing01/Cosmos-Chains-Sync/main/Stride/addrbook.json"
sudo systemctl restart strided && journalctl -u strided -f -o cat
