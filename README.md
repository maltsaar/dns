# DNS with octodns

## Setup

### .env

```
# Very important this is an "Account API Token" not any other type of API key or token
export CLOUDFLARE_TOKEN=token_goes_here
```

### Create and activate venv

```
chmod +x create-venv.sh
./create-venv.sh
source venv/bin/activate
source .env
```

## Usage

### Validate

```
octodns-validate --config config.yaml
```

### Dry run

```
octodns-sync --config config.yaml
```

### Run

```
octodns-sync --config config.yaml --doit
```
