cc_library(
    name = "influxdb-cxx",
    includes = [
        "include",
    ],
    hdrs = [
        "include/InfluxDB.h",
        "include/InfluxDBFactory.h",
        "include/Point.h",
        "include/Transport.h",
    ],
    srcs = [
        "src/InfluxDB.cxx",
        "src/Point.cxx",
        "src/InfluxDBFactory.cxx",
        "src/UDP.cxx",
        "src/UnixSocket.cxx",
        "src/HTTP.cxx",
        "src/HTTP.h",
        "src/UDP.h",
        "src/UnixSocket.h",
        "src/UriParser.h",
    ],
    copts = ["-std=c++17"],
    linkopts = ["-lcurl"],
    visibility = ["//visibility:public"],
    deps = ["@boost//:asio"],
)
