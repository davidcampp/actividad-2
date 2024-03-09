from flask import Flask, jsonify

app = Flask(__name__)

@app.route("/")
def index():
    
    listaDePersonas =[
    { 'N_identificacion': 2245672133, 'nombre': "david campo palma", 'telefono':3245679843},
    { 'N_identificacion': 1003452354,'nombre': "alberto marmol campo", 'telefono':3025462762},
    { 'N_identificacion': 1024672312, 'nombre': "yair campo palma", 'telefono':3004574523},
    { 'N_identificacion': 1024675673, 'nombre': "diana palma meza", 'telefono':3042342668},
    { 'N_identificacion': 22456785, 'nombre': "yair campo araque", 'telefono':3013452685}
    ]
    return jsonify(listaDePersonas)

if __name__ == "__main__":
    app.run(debug=True)
