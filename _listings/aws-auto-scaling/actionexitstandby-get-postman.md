{
  "info": {
    "name": "AWS Auto Scaling API Exit Standby",
    "_postman_id": "919fe7da-b339-4d59-9e8a-acf2e5f846ba",
    "description": "Moves the specified instances out of Standby mode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Server Instance",
      "item": [
        {
          "id": "61f79d71-7b10-487e-8cad-dd9b041013e5",
          "name": "attachInstances",
          "request": {
            "url": "http://example.com/api/?Action=AttachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more EC2 instances to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc6689ec-751d-4443-8746-fae2d7437e03"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "8f153a13-12d0-48bb-a52f-7b6fc1c17eca",
          "name": "attachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more Classic load balancers to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7010da3c-db8b-49ad-8631-c4c146d3c60a"
            }
          ]
        },
        {
          "id": "bd0792e7-cc58-4c4c-83ba-bfdde5271dad",
          "name": "attachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more target groups to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a00c09c5-a540-4ae7-8ae0-dbcb385ca8c1"
            }
          ]
        },
        {
          "id": "a3a897e8-d943-49d7-9d69-b88b3894f56a",
          "name": "describeLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the load balancers for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1347a4a5-cfdd-4e28-93f6-5aa163bd5be6"
            }
          ]
        },
        {
          "id": "a6d9e23d-d5ff-4367-bb52-24e22e997dca",
          "name": "describeLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the target groups for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04da6a83-e204-43a5-a973-d2df0079aad3"
            }
          ]
        },
        {
          "id": "5584f9dc-4488-461a-8ff3-fd16a5a9d843",
          "name": "detachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more Classic load balancers from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65802af3-7cc9-4be0-b135-026b5ded4e0d"
            }
          ]
        },
        {
          "id": "1d0f5a1a-9ee2-4df0-a143-64ef5319f26f",
          "name": "detachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more target groups from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec5741b2-cb15-45c5-b898-0f4217c64d1f"
            }
          ]
        }
      ]
    },
    {
      "name": "Life Cycle",
      "item": [
        {
          "id": "e590691c-43fd-42ec-900c-84c3ce23e1e9",
          "name": "completeLifecycleAction",
          "request": {
            "url": "http://example.com/api/?Action=CompleteLifecycleAction?AutoScalingGroupName=AutoScalingGroupName&InstanceId=InstanceId&LifecycleActionResult=LifecycleActionResult&LifecycleActionToken=LifecycleActionToken&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Completes the lifecycle action for the specified token or instance with the specified result."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd09ed39-f153-47fc-8f5f-4b5152d31a5e"
            }
          ]
        },
        {
          "id": "5062b8f9-4674-4502-bc6a-1f9c3e39fb6c",
          "name": "deleteLifecycleHook",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLifecycleHook?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified lifecycle hook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c12bca56-21db-48aa-88a3-2ab71de82010"
            }
          ]
        },
        {
          "id": "c4588924-dc6f-447a-ac95-1ab81251d31d",
          "name": "describeLifecycleHooks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHooks?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookNames.member.N=LifecycleHookNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the lifecycle hooks for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe9d6e9b-5bfa-4b95-bb4c-39d094fbf81e"
            }
          ]
        },
        {
          "id": "7171846a-9c3f-4a14-981f-84a25b46370e",
          "name": "describeLifecycleHookTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHookTypes?LifecycleHookTypes.member.N=LifecycleHookTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available types of lifecycle hooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedd6752-5f28-4e58-b215-88aeb6220da2"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Groups",
      "item": [
        {
          "id": "b021b457-69d7-4f87-9122-b2b13cd9d68c",
          "name": "createAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&AvailabilityZones.member.N=AvailabilityZones.member.N&DefaultCooldown=DefaultCooldown&DesiredCapacity=DesiredCapacity&HealthCheckGracePeriod=HealthCheckGracePeriod&HealthCheckType=HealthCheckType&InstanceId=InstanceId&LaunchConfigurationName=LaunchConfigurationName&LoadBalancerNames.member.N=LoadBalancerNames.member.N&MaxSize=MaxSize&MinSize=MinSize&NewInstancesProtectedFromScaleIn=NewInstancesProtectedFromScaleIn&PlacementGroup=PlacementGroup&Tags.member.N=Tags.member.N&TargetGroupARNs.member.N=TargetGroupARNs.member.N&TerminationPolicies.member.N=TerminationPolicies.member.N&VPCZoneIdentifier=VPCZoneIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Auto Scaling group with the specified name and attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "030e6650-07b6-453e-96c9-48c2cfbe34df"
            }
          ]
        },
        {
          "id": "6e23f8f4-6737-411f-add6-f5a2b1728635",
          "name": "deleteAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&ForceDelete=ForceDelete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "205e2c35-be4b-4cf3-bdd5-e2af0e29d9e6"
            }
          ]
        },
        {
          "id": "2524e49f-685c-4739-aefc-4f7f06082c5c",
          "name": "describeAutoScalingGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingGroups?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f40515a-03c5-4af5-b623-41b5fd618a25"
            }
          ]
        }
      ]
    },
    {
      "name": "Launch",
      "item": [
        {
          "id": "ce00bda2-a201-404e-8756-20b594f43b02",
          "name": "createLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateLaunchConfiguration?AssociatePublicIpAddress=AssociatePublicIpAddress&BlockDeviceMappings.member.N=BlockDeviceMappings.member.N&ClassicLinkVPCId=ClassicLinkVPCId&ClassicLinkVPCSecurityGroups.member.N=ClassicLinkVPCSecurityGroups.member.N&EbsOptimized=EbsOptimized&IamInstanceProfile=IamInstanceProfile&ImageId=ImageId&InstanceId=InstanceId&InstanceMonitoring=InstanceMonitoring&InstanceType=InstanceType&KernelId=KernelId&KeyName=KeyName&LaunchConfigurationName=LaunchConfigurationName&PlacementTenancy=PlacementTenancy&RamdiskId=RamdiskId&SecurityGroups.member.N=SecurityGroups.member.N&SpotPrice=SpotPrice&UserData=UserData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61f9915e-5d5b-4319-ad2b-6a1672b2668f"
            }
          ]
        },
        {
          "id": "f0e35378-f272-4bb8-8d2e-5dfd68ac8b26",
          "name": "deleteLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLaunchConfiguration?LaunchConfigurationName=LaunchConfigurationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "933c645e-7e21-4976-99e6-149239146795"
            }
          ]
        },
        {
          "id": "698609a3-7123-4af1-93e7-200a82fc684e",
          "name": "describeLaunchConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLaunchConfigurations?LaunchConfigurationNames.member.N=LaunchConfigurationNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more launch configurations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d93303-39b6-43b6-98eb-ebf20ed4d4fd"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "37c9596b-1e5d-4333-954c-823a7ce66312",
          "name": "createOrUpdateTags",
          "request": {
            "url": "http://example.com/api/?Action=CreateOrUpdateTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates tags for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2439a60-3623-4ae9-856a-b1402973121c"
            }
          ]
        },
        {
          "id": "6977a73e-fb4c-41a7-a3f8-3373c5d23a5c",
          "name": "deleteTags",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b23ac29-9071-4d48-b1fe-dffe742f360b"
            }
          ]
        },
        {
          "id": "ceec8c2a-be7e-4c22-8171-ba96ae9e9313",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?Filters.member.N=Filters.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f846be3-71f7-4ce1-9f69-a2f88a22372c"
            }
          ]
        }
      ]
    },
    {
      "name": "Notifications",
      "item": [
        {
          "id": "f9b130ac-bbdf-4afa-a5e6-712452605b25",
          "name": "deleteNotificationConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteNotificationConfiguration?AutoScalingGroupName=AutoScalingGroupName&TopicARN=TopicARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified notification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad39e3a8-e3c3-4067-868a-6240b869ce0c"
            }
          ]
        },
        {
          "id": "e1bb2578-60c5-464d-a265-154260d9e5ea",
          "name": "describeNotificationConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeNotificationConfigurations?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification actions associated with the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49f4b913-9638-4800-b793-6571a9a95f88"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "582fc679-e690-4d87-8282-037c567e7621",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?AutoScalingGroupName=AutoScalingGroupName&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc278e21-5220-4289-b6ba-dea26983a3c2"
            }
          ]
        },
        {
          "id": "a2881aa9-4203-4c8b-8ee0-96adabba544e",
          "name": "describePolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribePolicies?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken&PolicyNames.member.N=PolicyNames.member.N&PolicyTypes.member.N=PolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policies for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b2349bc-9ae9-4ef7-ace8-8ff3c699c4fd"
            }
          ]
        },
        {
          "id": "2837eb69-6ac0-441e-94df-5d52c8e22a43",
          "name": "executePolicy",
          "request": {
            "url": "http://example.com/api/?Action=ExecutePolicy?AutoScalingGroupName=AutoScalingGroupName&BreachThreshold=BreachThreshold&HonorCooldown=HonorCooldown&MetricValue=MetricValue&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddbbfdf7-2f52-4f79-a0b0-94c3226614bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Action",
      "item": [
        {
          "id": "cb954394-2aa2-4923-aa2a-8ced52d5eb6f",
          "name": "deleteScheduledAction",
          "request": {
            "url": "http://example.com/api/?Action=DeleteScheduledAction?AutoScalingGroupName=AutoScalingGroupName&ScheduledActionName=ScheduledActionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified scheduled action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "917afda1-6457-48fb-99b6-b14049198337"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "e76192a9-3e6a-4307-9f7f-12a21bd5292d",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?MaxNumberOfAutoScalingGroups=MaxNumberOfAutoScalingGroups&MaxNumberOfLaunchConfigurations=MaxNumberOfLaunchConfigurations&NumberOfAutoScalingGroups=NumberOfAutoScalingGroups&NumberOfLaunchConfigurations=NumberOfLaunchConfigurations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the current Auto Scaling resource limits for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e80b8b4e-a591-44c8-a821-91bd94a046db"
            }
          ]
        }
      ]
    },
    {
      "name": "Adjustment Types",
      "item": [
        {
          "id": "0fddd105-757e-42ab-8c7e-ed292b6eb8de",
          "name": "describeAdjustmentTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAdjustmentTypes?AdjustmentTypes.member.N=AdjustmentTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policy adjustment types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcdf28ff-905b-4d9d-895a-63f4431faaf7"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Instances",
      "item": [
        {
          "id": "3ced4f52-1346-476c-b533-da96eac5d677",
          "name": "describeAutoScalingInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingInstances?InstanceIds.member.N=InstanceIds.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "427f0101-55bd-40fe-8faa-89329579e047"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Notifications",
      "item": [
        {
          "id": "99121923-8c64-4848-ac1e-e32ae2bef395",
          "name": "describeAutoScalingNotificationTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingNotificationTypes?AutoScalingNotificationTypes.member.N=AutoScalingNotificationTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification types that are supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92a618dc-0972-4c78-b51c-18de18602b5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Metric Collection",
      "item": [
        {
          "id": "7f2ab72f-0907-4e1a-a180-55b8cfcd0426",
          "name": "describeMetricCollectionTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMetricCollectionTypes?Granularities.member.N=Granularities.member.N&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available CloudWatch metrics for Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e95f6907-9098-4d2e-832c-88701b1dbc2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Activities",
      "item": [
        {
          "id": "6f543a6e-f733-44b7-b6f5-f4c50abfeb26",
          "name": "describeScalingActivities",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingActivities?ActivityIds.member.N=ActivityIds.member.N&AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more scaling activities for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59e094a0-ab10-41c2-8e3a-130f9d5546ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Process",
      "item": [
        {
          "id": "0c186c90-f352-41c1-b0b1-0b3edfd9c453",
          "name": "describeScalingProcessTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingProcessTypes?Processes.member.N=Processes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the scaling process types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50cdcac3-f695-4c8b-b809-f481cc5e3206"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Actions",
      "item": [
        {
          "id": "e4700edc-0430-48b7-a311-c8bebd77c4c1",
          "name": "describeScheduledActions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScheduledActions?AutoScalingGroupName=AutoScalingGroupName&EndTime=EndTime&MaxRecords=MaxRecords&NextToken=NextToken&ScheduledActionNames.member.N=ScheduledActionNames.member.N&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the actions scheduled for your Auto Scaling group that haven't run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4541d2a1-66a5-404c-8c6f-5d0bbd607039"
            }
          ]
        }
      ]
    },
    {
      "name": "Termination Policies",
      "item": [
        {
          "id": "879c9925-9267-49e4-be4e-4a7cdd449947",
          "name": "describeTerminationPolicyTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTerminationPolicyTypes?TerminationPolicyTypes.member.N=TerminationPolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the termination policies supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "421265e1-b94f-45c9-a5ac-fd076a0bfb06"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Instances",
      "item": [
        {
          "id": "4cd20018-3b17-4256-b2a7-79f06d5e78a8",
          "name": "detachInstances",
          "request": {
            "url": "http://example.com/api/?Action=DetachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes one or more instances from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a93e4bc4-cb5a-4b9c-b3f6-769be488ced1"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics Collection",
      "item": [
        {
          "id": "30a2fbff-d9e3-4574-9f6a-b51c7ac44280",
          "name": "disableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=DisableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b272e989-16b5-488a-a3a9-ff31f6ec3657"
            }
          ]
        },
        {
          "id": "30701a68-4437-47f6-ba1b-2b8a81bb6c63",
          "name": "enableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=EnableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Granularity=Granularity&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6f599e-821e-40b0-913b-26d07535732c"
            }
          ]
        }
      ]
    },
    {
      "name": "Stand By",
      "item": [
        {
          "id": "2981f51a-1afb-470c-bedf-adb1dd178b94",
          "name": "enterStandby",
          "request": {
            "url": "http://example.com/api/?Action=EnterStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances into Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af8e6071-6f61-4dc9-9a1c-5052e04efb7b"
            }
          ]
        },
        {
          "id": "5de1eca6-9422-4434-a274-b787ce26ac8b",
          "name": "exitStandby",
          "request": {
            "url": "http://example.com/api/?Action=ExitStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances out of Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68394b9c-39b3-4a7f-bf9b-b87a13392777"
            }
          ]
        }
      ]
    }
  ]
}