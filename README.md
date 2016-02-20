devise_auditable
=================

devise_auditable is a plugin for Devise that adds a audit log support to Devise.

Installation
=================

Add devise_auditable to your Gemfile

    gem 'devise_auditable'

Run the installer

    rails g devise_auditable User

Add the auditable key to your devise user model

    class User < ActiveRecord::Base
      devise :database_authenticatable, ..... , :auditable
    end

Optionally, you can add a `has_many` relationship to your devise
model.
