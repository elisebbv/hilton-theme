---
title: Blog
description: Hilton blog features productivity, tips, inspiration and strategies for massive profits. Find out how to set up a successful blog or how to make yours even better!
---

          <div>
            {{ if .Site.Params.mailchimp.enable }}
            <div class="hero__subscribe" style="margin-left: auto; margin-right: auto;" >
              <form class="subscribe-form validate"
                action="{{ if .Site.Params.mailchimp.mailchimp__identifier }}//{{.Site.Params.mailchimp.mailchimp__identifier}}{{ else }}#{{ end }}" method="POST"
                id="membedded-subscribe-form" name="membedded-subscribe-form" target="_blank" novalidate>
                <label class="screen-reader-text" for="mce-EMAIL">Email address</label>
                <input class="subscribe-email required email" id="mce-EMAIL" type="text" name="EMAIL"
                  placeholder="{{ if .Site.Params.mailchimp.mailchimp__input__text }}{{ .Site.Params.mailchimp.mailchimp__input__text }}{{ else }}Email address{{ end }}">
                <button class="button button--primary button--small subscribe-button" id="membedded-subscribe" type="submit" name="subscribe">{{ .Site.Params.mailchimp.mailchimp__button__text }}</button>
              </form>
            </div>
            {{ end }}
          </div>