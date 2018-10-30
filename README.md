Running this playbook on the included [inventory](hosts) produces the
following output:

    PLAY [localhost] ******************************************************************************

    TASK [set_fact] *******************************************************************************
    ok: [localhost]

    TASK [debug] **********************************************************************************
    ok: [localhost] => (item=[u'codec1', u'web1', u'db1']) => {
        "msg": [
            "codec1", 
            "web1", 
            "db1"
        ]
    }
    ok: [localhost] => (item=[u'codec2', u'web2', u'db2']) => {
        "msg": [
            "codec2", 
            "web2", 
            "db2"
        ]
    }
    ok: [localhost] => (item=[u'codec3', u'web3', u'db3']) => {
        "msg": [
            "codec3", 
            "web3", 
            "db3"
        ]
    }

    PLAY RECAP ************************************************************************************
    localhost                  : ok=2    changed=0    unreachable=0    failed=0    skipped=0   

