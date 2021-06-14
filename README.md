### Ruby API Wrapper - Cloudways
     
Early Release. Only token auth working.
  
Easily connect to your Cloudways account through their API.

* Secure OAuth Cloudways API Authentication

#### Step 1 - Add to your application
  
    gem 'ruby_api_pack_cloudways'
    bundle install
    
#### Controller Example
    
    # Load Gems & Files
    require "ruby_api_pack_cloudways"

    def index
        @server_index_connection_index = RubyApiPackCloudways::Api::CwLists.cw_server_list
    end


#### Example on Index File

    <% @server_index_connection_index.each do |continent| %>
    
    <%= continent["id"] %>
    
    <% end %>

  
#### Variables

    PHCDEV_API_CLOUDWAYS_EMAIL = Your Cloudways Email Login
    PHCDEV_API_CLOUDWAYS_KEY = API Key Provided by Cloudways
