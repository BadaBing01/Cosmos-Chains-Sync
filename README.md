# Cosmos-Chains-Sync
## Example for change the addrbook

sudo systemctl stop strided <br>
rm $HOME/.stride/config/addrbook.json <br>
wget -O $HOME/.stride/config/addrbook.json "https://raw.githubusercontent.com/BadaBing01/Cosmos-Chains-Sync/main/Stride/addrbook.json" <br>
sudo systemctl restart strided && journalctl -u strided -f -o cat <br>
