[![Build Status](https://travis-ci.org/AnaTofuZ/p5-webservice-YDMM.svg?branch=master)](https://travis-ci.org/AnaTofuZ/p5-webservice-YDMM) [![MetaCPAN Release](https://badge.fury.io/pl/WebService-YDMM.svg)](https://metacpan.org/release/WebService-YDMM)
# NAME

WebService::YDMM - It's yet another DMM sdk.

# SYNOPSIS

    use WebService::YDMM;

    my $dmm = WebService::YDMM->new(
        affiliate_id => ${affiliate_id},
        api_id       => ${api_id},
    );

    my $items = $dmm->item("DMM.com",+{ keyword => "魔法少女まどか☆マギカ"});

    # or 

    my $items = $dmm->item(+{ site => "DMM.R18" , keyword => "魔法少女まどか☆マギカ"});

# DESCRIPTION

WebService::YDMM is another DMM webservice module.
[DMM](http://www.dmm.com) is Japanese shopping site.

This module supported by [DMM.API](https://affiliate.dmm.com/api/).

# METHODS

## new(%params)

Create instance of WebService::Reactio.

_%params_ must have following parameter:

- api\_id

    API ID of DMM.com web service
    You can get API key on project application for DMM affiliate service.

- affiliate\_id

    Affiliate ID of DMM.com web service
    You can get API key on project application for DMM affiliate service.
    This affiliate\_id validate of 990 ~ 999 number.

## item(\[$site\],\\%params)

# LICENSE

Copyright (C) AnaTofuZ.

DMM API Copyright 
Powered by [DMM.com Webサービス](https://affiliate.dmm.com/api/)

Powered by [DMM.R18 Webサービス](https://affiliate.dmm.com/api/)

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# AUTHOR

AnaTofuZ <anatofuz@gmail.com>
