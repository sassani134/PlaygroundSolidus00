rails new PlaygroundSolidius00
bundle add solidus
bin/rails g solidus:install

nigaz@nigaz-82JQ:~/RailsWorks/PlaygroundSolidius00$ bin/rails g solidus:install
    question  Which frontend would you like to use?
              - [starter] Generate all necessary controllers and views directly in your Rails app (default).
              - [none] Skip installing a frontend.
      answer: Starter
       using  starter
    question  Which payment method would you like to use?
              - [paypal] Install `solidus_paypal_commerce_platform` (default).
              - [stripe] Install `solidus_stripe`.
              - [braintree] Install `solidus_braintree`.
              - [none] Skip installing a payment method.
      answer: stripe
       using  stripe
  installing  solidus routes
    question  Where would you like to mount Solidus? (E.g. "/store" or "/shop") (default: "/").
      answer: 
       using  / (default)
      create  config/initializers/spree.rb
      assets  Active Storage
        rake  active_storage:install
Copied migration 20240602203842_create_active_storage_tables.active_storage.rb from active_storage
       exist  app/assets/images
      create  vendor/assets/javascripts/spree/backend
      create  vendor/assets/stylesheets/spree/backend
      create  vendor/assets/images/spree/backend
      create  vendor/assets/javascripts/spree/backend/all.js
      create  vendor/assets/stylesheets/spree/backend/all.css
      create  app/overrides
      append  db/seeds.rb
     copying  migrations
        rake  railties:install:migrations
Copied migration 20240602203844_create_action_mailbox_tables.action_mailbox.rb from action_mailbox
Copied migration 20240602203845_create_action_text_tables.action_text.rb from action_text
Copied migration 20240602203846_solidus_one_four.spree.rb from spree
Copied migration 20240602203847_create_spree_wallet_payment_sources.spree.rb from spree
Copied migration 20240602203848_migrate_credit_cards_to_wallet_payment_sources.spree.rb from spree
Copied migration 20240602203849_remove_is_default_from_prices.spree.rb from spree
Copied migration 20240602203850_remove_currency_from_line_items.spree.rb from spree
Copied migration 20240602203851_add_available_to_columns_and_remove_display_on_from_payment_methods.spree.rb from spree
Copied migration 20240602203852_create_spree_promotion_code_batch.spree.rb from spree
Copied migration 20240602203853_add_available_to_users_and_remove_display_on_from_shipping_methods.spree.rb from spree
Copied migration 20240602203854_add_index_to_spree_payments_number.spree.rb from spree
Copied migration 20240602203855_remove_spree_store_credits_column.spree.rb from spree
Copied migration 20240602203856_add_lft_and_rgt_indexes_to_taxons.spree.rb from spree
Copied migration 20240602203857_remove_order_id_from_inventory_units.spree.rb from spree
Copied migration 20240602203858_transform_tax_rate_category_relation.spree.rb from spree
Copied migration 20240602203859_add_roles_unique_constraints.spree.rb from spree
Copied migration 20240602203860_add_time_range_to_tax_rate.spree.rb from spree
Copied migration 20240602203861_rename_bogus_gateways.spree.rb from spree
Copied migration 20240602203862_remove_default_tax_from_spree_zones.spree.rb from spree
Copied migration 20240602203863_create_promotion_rule_stores.spree.rb from spree
Copied migration 20240602203864_create_store_shipping_methods.spree.rb from spree
Copied migration 20240602203865_add_available_locales_to_stores.spree.rb from spree
Copied migration 20240602203866_add_amount_remaining_to_store_credit_events.spree.rb from spree
Copied migration 20240602203867_add_join_characters_to_promotion_code_batch.spree.rb from spree
Copied migration 20240602203868_add_apply_to_all_to_variant_property_rule.spree.rb from spree
Copied migration 20240602203869_create_spree_store_credit_reasons_table.spree.rb from spree
Copied migration 20240602203870_remove_code_from_spree_promotions.spree.rb from spree
Copied migration 20240602203871_drop_spree_store_credit_update_reasons.spree.rb from spree
Copied migration 20240602203872_add_default_billng_flag_to_user_addresses.spree.rb from spree
Copied migration 20240602203873_add_bcc_email_to_spree_stores.spree.rb from spree
Copied migration 20240602203874_add_discontinue_on_to_spree_products.spree.rb from spree
Copied migration 20240602203875_add_type_before_removal_to_spree_payment_methods.spree.rb from spree
Copied migration 20240602203876_add_name_to_spree_addresses.spree.rb from spree
Copied migration 20240602203877_change_column_null_on_prices.spree.rb from spree
Copied migration 20240602203878_add_unique_index_to_option_values_variants.spree.rb from spree
Copied migration 20240602203879_set_promotions_with_any_policy_to_all_if_possible.spree.rb from spree
Copied migration 20240602203880_add_level_to_spree_tax_rates.spree.rb from spree
Copied migration 20240602203881_add_shipping_category_to_spree_variants.spree.rb from spree
Copied migration 20240602203882_change_column_null_option_values_option_type_id.spree.rb from spree
Copied migration 20240602203883_remove_match_policy_from_spree_promotion.spree.rb from spree
Copied migration 20240602203884_remove_unused_columns_from_promotion_rules.spree.rb from spree
Copied migration 20240602203885_drop_unused_promo_action_line_items.spree.rb from spree
Copied migration 20240602203886_remove_taxon_position.spree.rb from spree
Copied migration 20240602203887_drop_deprecated_address_id_from_shipments.spree.rb from spree
Copied migration 20240602203888_add_order_promotions_foreign_key.spree.rb from spree
Copied migration 20240602203889_add_promotion_order_promotion_foreign_key.spree.rb from spree
Copied migration 20240602203890_add_api_key_to_spree_users.spree_api.rb from spree_api
Copied migration 20240602203891_resize_api_key_field.spree_api.rb from spree_api
Copied migration 20240602203892_rename_api_key_to_spree_api_key.spree_api.rb from spree_api
Copied migration 20240602203893_add_index_to_user_spree_api_key.spree_api.rb from spree_api
    creating  database
        rake  db:create
     running  migrations
        rake  db:migrate
  installing  [authentication] devise
       apply  /mnt/e644da04-91ef-4746-8f4c-8890d86663ff/.asdf/installs/ruby/3.2.2/lib/ruby/gems/3.2.0/gems/solidus_core-4.3.5/lib/generators/solidus/install/app_templates/authentication/devise.rb
         run    bundle add solidus_auth_devise
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
Fetching solidus_support 0.10.2
Installing solidus_support 0.10.2
    generate    solidus:auth:install 
       rails    generate solidus:auth:install  
      create  config/initializers/devise.rb
        rake  railties:install:migrations FROM=solidus_auth 
Copied migration 20240602203894_create_users.solidus_auth.rb from solidus_auth
Copied migration 20240602203895_rename_columns_for_devise.solidus_auth.rb from solidus_auth
Copied migration 20240602203896_convert_user_remember_field.solidus_auth.rb from solidus_auth
Copied migration 20240602203897_add_reset_password_sent_at_to_spree_users.solidus_auth.rb from solidus_auth
Copied migration 20240602203898_make_users_email_index_unique.solidus_auth.rb from solidus_auth
Copied migration 20240602203899_add_deleted_at_to_users.solidus_auth.rb from solidus_auth
Copied migration 20240602203900_add_confirmable_to_users.solidus_auth.rb from solidus_auth
Copied migration 20240602203901_add_reset_password_token_index_to_spree_users.solidus_auth.rb from solidus_auth
Copied migration 20240602203902_add_unconfirmed_email_to_spree_users.solidus_auth.rb from solidus_auth
        rake  db:migrate
      append    db/seeds.rb
  installing  [frontend] starter
       apply  /mnt/e644da04-91ef-4746-8f4c-8890d86663ff/.asdf/installs/ruby/3.2.2/lib/ruby/gems/3.2.0/gems/solidus_core-4.3.5/lib/generators/solidus/install/app_templates/frontend/starter.rb
       apply    https://github.com/solidusio/solidus_starter_frontend/raw/v4.3/template.rb
  installing      [solidus_starter_frontend] checking versions
  installing      [solidus_starter_frontend] fetching remote templates
         run      git clone --quiet --depth 1 --branch v4.3 https://github.com/solidusio/solidus_starter_frontend.git /mnt/e644da04-91ef-4746-8f4c-8890d86663ff/RailsWorks/PlaygroundSolidius00/tmp/solidus_starter_frontend-3ee667248b633c436e3d9a3103281af4 from "."
  installing      [solidus_starter_frontend] installing gems
     gemfile      responders
     gemfile      canonical-rails
     gemfile      solidus_support
     gemfile      truncate_html
     gemfile      view_component (~> 3.0)
     gemfile      tailwindcss-rails
     gemfile      group :test
        gsub      Gemfile
     gemfile      capybara-screenshot (~> 1.0)
     gemfile      database_cleaner (~> 2.0)
        gsub      Gemfile
     gemfile      group :development, :test
        gsub      Gemfile
     gemfile      rspec-rails
     gemfile      rails-controller-testing (~> 1.0.5)
     gemfile      rspec-activemodel-mocks (~> 1.1.0)
     gemfile      factory_bot (>= 4.8)
     gemfile      factory_bot_rails
     gemfile      ffaker (~> 2.13)
     gemfile      rubocop (~> 1.0)
     gemfile      rubocop-performance (~> 1.5)
     gemfile      rubocop-rails (~> 2.3)
     gemfile      rubocop-rspec (~> 2.0)
        gsub      Gemfile
         run      bundle install
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
Fetching json 2.7.2
Fetching rspec-mocks 3.13.1
Fetching parser 3.3.2.0
Fetching view_component 3.12.1
Fetching launchy 3.0.1
Installing json 2.7.2 with native extensions
Installing rspec-mocks 3.13.1
Fetching rspec-rails 6.1.2
Installing parser 3.3.2.0
Installing launchy 3.0.1
Installing view_component 3.12.1
Installing rspec-rails 6.1.2
Fetching rubocop-ast 1.31.3
Installing rubocop-ast 1.31.3
Fetching rubocop 1.64.1
Installing rubocop 1.64.1
Fetching rubocop-rails 2.25.0
Fetching rubocop-performance 1.21.0
Fetching rubocop-rspec_rails 2.28.3
Installing rubocop-rails 2.25.0
Installing rubocop-performance 1.21.0
Installing rubocop-rspec_rails 2.28.3
Fetching rubocop-rspec 2.29.2
Installing rubocop-rspec 2.29.2
Bundle complete! 34 Gemfile dependencies, 162 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
  installing      [solidus_starter_frontend] installing files
       exist      public
      create      public/storefront_favicon.ico
      create      public/storefront_favicon.svg
      create      config/initializers/solidus_auth_devise_unauthorized_redirect.rb
      create      config/initializers/canonical_rails.rb
      create      config/routes/storefront.rb
      create      config/tailwind.config.js
      create      app/assets/builds/tailwind.css
        rake      tailwindcss:install
Add Tailwindcss include tags and container element in application layout
      insert  app/views/layouts/application.html.erb
      insert  app/views/layouts/application.html.erb
      insert  app/views/layouts/application.html.erb
Build into app/assets/builds
       exist  app/assets/builds
      create  app/assets/builds/.keep
      append  app/assets/config/manifest.js
      append  .gitignore
Add default Procfile.dev
      create  Procfile.dev
Ensure foreman is installed
         run  gem install foreman from "."
Successfully installed foreman-0.88.1
Parsing documentation for foreman-0.88.1
Done installing documentation for foreman after 0 seconds
1 gem installed

A new release of RubyGems is available: 3.5.6 → 3.5.11!
Run `gem update --system 3.5.11` to update your installation.

Add bin/dev to start foreman
      create  bin/dev
Compile initial Tailwind build
         run  rails tailwindcss:build from "."
Browserslist: caniuse-lite is outdated. Please run:
  npx update-browserslist-db@latest
  Why you should do it regularly: https://github.com/browserslist/update-db#readme

Rebuilding...

Done in 892ms.
      insert      config/environments/test.rb
      append      config/initializers/devise.rb
  installing      [solidus_starter_frontend] installing routes
      append      public/robots.txt
  installing      [solidus_starter_frontend] patching asset files
      append      config/initializers/assets.rb
      append      config/initializers/assets.rb
        gsub      app/assets/stylesheets/application.css
  installing      [solidus_starter_frontend] setting up rspec
    generate      rspec:install
       rails      generate rspec:install 
      create  .rspec
       exist  spec
      create  spec/spec_helper.rb
      create  spec/rails_helper.rb
  installing      [solidus_starter_frontend] security advisory
 RECOMMENDED      To receive security announcements concerning Solidus Starter Frontend, please subscribe to the Solidus Security mailing list (https://groups.google.com/forum/#!forum/solidus-security). The mailing list is very low traffic, and it receives the public notifications the moment the vulnerability is published. For more information, please check out https://solidus.io/security. 
  installing  [payment_method] stripe
       apply  /mnt/e644da04-91ef-4746-8f4c-8890d86663ff/.asdf/installs/ruby/3.2.2/lib/ruby/gems/3.2.0/gems/solidus_core-4.3.5/lib/generators/solidus/install/app_templates/payment_method/stripe.rb
         run    bundle add solidus_stripe --version '~> 5.a'
Fetching gem metadata from https://rubygems.org/........
Resolving dependencies...
Fetching gem metadata from https://rubygems.org/........
Fetching solidus_stripe 5.0.2
Installing solidus_stripe 5.0.2
    generate    solidus_stripe:install
       rails    generate solidus_stripe:install 
     install  [solidus_stripe] migrations
        rake    railties:install:migrations FROM=solidus_stripe
Copied migration 20240602203937_create_solidus_stripe_payment_sources.solidus_stripe.rb from solidus_stripe
Copied migration 20240602203938_create_solidus_stripe_payment_intents.solidus_stripe.rb from solidus_stripe
Copied migration 20240602203939_create_solidus_stripe_slug_entries.solidus_stripe.rb from solidus_stripe
Copied migration 20240602203940_create_solidus_stripe_customers.solidus_stripe.rb from solidus_stripe
         run    bin/rails db:migrate from "."
     install  [solidus_stripe] solidus_core
       exist    config/initializers
      create    config/initializers/solidus_stripe.rb
       route    mount SolidusStripe::Engine, at: '/solidus_stripe'
     install  [solidus_stripe] solidus_backend
      append    vendor/assets/javascripts/spree/backend/all.js
      insert    vendor/assets/stylesheets/spree/backend/all.css
     install  [solidus_stripe] solidus_starter_frontend
       exist    app
      create    app/assets/stylesheets/spree/frontend/solidus_stripe.css
      create    app/javascript/controllers/solidus_stripe_confirm_controller.js
      create    app/javascript/controllers/solidus_stripe_payment_controller.js
      create    app/views/checkouts/existing_payment/_stripe.html.erb
      create    app/views/checkouts/existing_payment/stripe/_card.html.erb
      create    app/views/checkouts/existing_payment/stripe/_default.html.erb
      create    app/views/checkouts/payment/_stripe.html.erb
      create    app/views/orders/payment_info/_stripe.html.erb
      insert    app/assets/stylesheets/solidus_starter_frontend.css
      create    spec/solidus_stripe_spec_helper.rb
      create    spec/system/frontend
      create    spec/system/frontend/.keep
      create    spec/system/frontend/solidus_stripe/checkout_spec.rb
       exist    spec/support
      create    spec/support/solidus_stripe/backend_test_helper.rb
      create    spec/support/solidus_stripe/checkout_test_helper.rb
      create    spec/support/solidus_stripe/factories.rb
      create    spec/support/solidus_stripe/webhook/data_fixtures.rb
      create    spec/support/solidus_stripe/webhook/event_with_context_factory.rb
      create    spec/support/solidus_stripe/webhook/request_helper.rb
         run    bin/importmap pin @stripe/stripe-js from "."
Pinning "@stripe/stripe-js" to vendor/javascript/@stripe/stripe-js.js via download from https://ga.jspm.io/npm:@stripe/stripe-js@3.4.1/lib/index.mjs
        load  seed data
      append  db/seeds.rb
Creating refund reason for Stripe refunds
  installing  SolidusAdmin
         run  bundle add solidus_admin -v ">= 0.2"
Fetching gem metadata from https://rubygems.org/........
Resolving dependencies...
    generate  solidus_admin:install --tailwind
       rails  generate solidus_admin:install --tailwind 
       route  mount SolidusAdmin::Engine, at: '/admin', constraints: ->(req) {
                req.cookies['solidus_admin'] != 'false' &&
                req.params['solidus_admin'] != 'false'
              }
      create  config/initializers/solidus_admin.rb
      append  .gitignore
        rake  solidus_admin:tailwindcss:install
         run  bundle show tailwindcss-rails
/mnt/e644da04-91ef-4746-8f4c-8890d86663ff/.asdf/installs/ruby/3.2.2/lib/ruby/gems/3.2.0/gems/tailwindcss-rails-2.6.0-x86_64-linux
      create  app/assets/stylesheets/solidus_admin/application.tailwind.css
      create  config/solidus_admin/tailwind.config.js
      create  lib/tasks/solidus_admin/tailwind.rake
   unchanged  .gitignore
      append  Procfile.dev
     loading  seed data
        rake  db:seed 
        seed  stores
        seed  store_credit
        seed  countries
        seed  return_reasons
        seed  states
        seed  stock_locations
        seed  zones
        seed  refund_reasons
        seed  roles
        seed  shipping_categories
Creating admin user with:
  - email: admin@example.com
  - password: test123
(please use the ADMIN_EMAIL and ADMIN_PASSWORD environment variables to control how the default admin user is created)
Creating refund reason for Stripe refunds
     loading  sample data
        rake  spree_sample:load
      sample  Payment Methods
      sample  Tax Categories
      sample  Tax Rates
      sample  Shipping Categories
      sample  Shipping Methods
      sample  Products
      sample  Taxons
      sample  Taxonomies
      sample  Option Values
      sample  Option Types
      sample  Product Option Types
      sample  Product Properties
      sample  Variants
      sample  Stock
      sample  Assets
      sample  images for Solidus Water Bottle
      sample  images for Solidus tote
      sample  images for Solidus hoodie
      sample  images for Solidus winter hat
      sample  images for Solidus circle sticker
      sample  images for Solidus mug set
      sample  images for Solidus notebook
      sample  images for Solidus t-shirt
      sample  images for Solidus long sleeve tee
      sample  images for Solidus dark tee
      sample  images for Solidus canvas tote bag
      sample  images for Solidus cap
      sample  Orders
      sample  Addresses
      sample  Stores
      sample  Payments
      sample  Reimbursements
    complete  Solidus has been installed successfully. Enjoy!
