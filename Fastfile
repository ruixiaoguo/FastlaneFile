
default_platform(:ios)

platform :ios do
  desc "正式版"
  lane :ApStore do
    gym(
        scheme:"PupeyReach",
        export_method:"app-store",
        output_directory:"./build",
        configuration:"Release",
        output_name:"KMHealth",
        clean:"true",
        include_bitcode: true,
        workspace: "PupeyReach.xcworkspace",
    )

    #firim(firim_api_token: "xxxx")
    #pgyer(api_key: "", user_key: "", update_description: "")
  end


  desc "内测版"
  lane :AdHoc do
    gym(
        scheme:"PupeyReach",
        export_method:"ad-hoc",
        output_directory:"./build",
        configuration:"Release",
        output_name:"KMHealth-AdHoc",
        clean:"true",
        include_bitcode: true,
        workspace: "PupeyReach.xcworkspace",’
        #自动管理证书的时候，Xcode 9及以上没有权限获取钥匙串里面的证书，必须加上这个才能打包成功
        #export_xcargs: "-allowProvisioningUpdates"
    )

    #firim(firim_api_token: "xxxx")
    #pgyer(api_key: "", user_key: "", update_description: "")
  end

  desc "开发版"
  lane :Development do
    gym(
        scheme:"PupeyReach",
        export_method:"development",
        output_directory:"./build",
        configuration:"Debug",
        output_name:"KMHealth-Del",
        clean:"true",
        include_bitcode: true,
        workspace: "PupeyReach.xcworkspace",
    )

    #firim(firim_api_token: "xxxx")
    #pgyer(api_key: "", user_key: "", update_description: "")
   end

  desc "企业版"
  lane :Enterprise do
    gym(
        scheme:"PupeyReach",
        export_method:"enterprise",
        output_directory:"./build",
        configuration:"Release",
        output_name:"KMHealth-Enter",
        clean:"true",
        include_bitcode: true,
        workspace: "PupeyReach.xcworkspace",
    )

    #firim(firim_api_token: "xxxx")
    #pgyer(api_key: "", user_key: "", update_description: "")
  end



end
