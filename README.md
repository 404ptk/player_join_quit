Player join:
    package p.jaro.firstplugin.Listeners;

    import org.bukkit.Bukkit;
    import org.bukkit.ChatColor;
    import org.bukkit.event.EventHandler;
    import org.bukkit.event.Listener;
    import org.bukkit.event.player.PlayerJoinEvent;

    public class PlayerJoinListener implements Listener {
        @EventHandler
        public void onPlayerJoin(PlayerJoinEvent event){
            event.setJoinMessage(null);
            Bukkit.broadcastMessage(ChatColor.translateAlternateColorCodes('&',"&2+ &8"+event.getPlayer().getName()));
        }
    }
Player quit:
    package p.jaro.firstplugin.Listeners;

    import org.bukkit.Bukkit;
    import org.bukkit.ChatColor;
    import org.bukkit.event.EventHandler;
    import org.bukkit.event.Listener;
    import org.bukkit.event.player.PlayerQuitEvent;

    public class PlayerQuitListener implements Listener {
        @EventHandler
        public void onPlayerLeave(PlayerQuitEvent event){
            event.setQuitMessage(null);
            Bukkit.broadcastMessage(ChatColor.translateAlternateColorCodes('&',"&c- &8"+event.getPlayer().getName()));
        }
    }
