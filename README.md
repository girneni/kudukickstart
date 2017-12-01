# kudukickstart
Gives an overview of KUDU and the starting point to create KUDU tables and Integration with Spark 
Kudu Basics: Basic Kudu Installation, API Usage, and SQL Integration

Before running these examples, I recommend installing git and maven. See the boostrap.sh script or run the following:

sudo yum -y install git
wget -P /tmp/ http://apache.cs.utah.edu/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz
sudo tar xzf /tmp/apache-maven-3.3.9-bin.tar.gz -C /usr/local
cat <<'EOF'>> maven.sh
export M2_HOME=/usr/local/apache-maven-3.3.9
export PATH=${M2_HOME}/bin:${PATH}
EOF
sudo mv maven.sh /etc/profile.d/maven.sh
source /etc/profile
You'll also want to download some sample data:

wget -P /tmp https://raw.githubusercontent.com/girneni/user_ratings.txt
