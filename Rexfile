user "user1";
private_key "/home/user1/.ssh/id_rsa";
public_key "/home/user1/.ssh/id_rsa.pub";
key_auth;
sudo TRUE;


group myserver => "localhost", "s1";

desc "Get the uptime of all server";
task "uptime", group => "myserver", sub {
   my $output = run "uptime";
   say $output;
};
