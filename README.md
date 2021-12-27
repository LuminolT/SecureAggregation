# Secure Aggregation

This is an unofficial implementation of Secure Aggregation Protocol. The details of the protocol can be found in the original paper: [(CCS '17) Practical Secure Aggregation for Privacy-Preserving Machine Learning](https://dl.acm.org/doi/abs/10.1145/3133956.3133982).

Based on Secure Aggregation Protocol, a verifiable secure aggregation protocol for cross-device federated learning is proposed. The details of the protocol can be found in the original paper: [(TDSC 2021) VERSA: Verifiable Secure Aggregation for Cross-Device Federated Learning](https://ieeexplore.ieee.org/abstract/document/9609695).

These protocols are currently implemented through socket programming and multithreaded programming. In the future, docker-compose will be used for standalone simulation.

## Usage

```
git clone https://github.com/chen-junbao/secureaggregation.git
pip install -r requirements.txt
pip install git+https://github.com/blockstack/secret-sharing

python main.py -h
```

Simulate 100 users and set the waiting time to 300 seconds:
```
python main.py -u 100 -t 300
```

VERSA:
```
git checkout versa
python main.py -u 100 -t 300
```
