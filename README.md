# Milight v6 PHP
Use PHP to send commands to Milight v6

### Usage

  1. Set the IP address of your Milight v6 Wifi Bridge in [milight.php](https://github.com/colincwc/Milight-v6-PHP/blob/master/milight.php) (The port should remain as 5987)
  
  ```
      $server = 'XXX.XXX.XXX.XXX';
  ```
  
  2. Pass GET parameter/value pairs for "cmd" and "zone" to [milight.php](https://github.com/colincwc/Milight-v6-PHP/blob/master/milight.php) (See [milight.php](https://github.com/colincwc/Milight-v6-PHP/blob/master/milight.php) for available commands)
  
  ```
      <form action="milight.php" method="GET">
         <input type="text" name="cmd" value="blue"> <!-- Defaults to "on" command if a command isn't sent -->
         <input type="text" name="zone" value="1"> <!-- Defaults to "0" (ALL zones) if a zone isn't set -->
         <input type="submit" name="submit" value="Send Command">
      </form>
      
      Or
      
      <a href='milight.php">Turn on lights in All Zones</a>
      <a href='milight.php?cmd=off'>Turn off lights All Zones</a>
      <a href='milight.php?cmd=blue&zone=1'>Turn lights blue in Zone 1</a>
      
  ```
