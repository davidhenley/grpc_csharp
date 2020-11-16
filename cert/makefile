cacert:
	cfssl gencert -initca ca-csr.json | cfssljson -bare ca

servicecert:
	cfssl gencert -ca=ca.pem -ca-key=ca-key.pem -config=ca-config.json -profile=service  service-csr.json | cfssljson -bare service
