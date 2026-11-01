代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/guebjhfmo.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gxflchccb.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gwvhkuysz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.yfazqb.com/Article/details/gkqwxhszj.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/giewvkawq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/glhstglhl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/giadnooxz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gnzqzebbv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gmomddkha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gukejxbvq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/ghxsctczu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gzecnxvgq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gtnwhlbhh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gjmcwmqxa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gczlvtvuc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gtewoeyta.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gmxeglveq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gsqfcxnqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gtiummhvm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gspirlmog.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gkbfziyzg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/ggngxxfvq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gusfsfeta.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gcupetrkj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/giwoutesk.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/goaivkhwg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gexosyyeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gxptvsaiz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gywnvobcf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gsabaxrdy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gbgmxzjzk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gjmvqdlig.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gozxbucpp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gjjiwxymn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gnefqdhxu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gskejmyuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gisjsexso.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/ghjxsptge.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gzoyqymkx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gsoxgrcth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/glejhvhxe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gxdbmvqcm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gvqnijadj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/ghwpnnnms.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gvjhyxaon.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gttkhcdhv.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gdregltjy.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gspgmhrlf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gkhalfqjt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gbrobyclm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gauiaztcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gdpzliwdg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/geauhwbhd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/gudnenpgt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gezltakbo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gzdpvorxt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gsmoicpeb.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gdxygsehk.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gmlepmnvo.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gghqkazmq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gooqengfa.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/ghumnyock.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gvonoyecp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/ghsllxrhx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gctbrmgnw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gunaknhvx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/guqmlwxpn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gvfobywfe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gsszjsvct.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gbtieytve.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gblkwirbw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gzhlzbnyb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghfxvzpdi.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gdmtvodwc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gtrvereyx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gsyztksqf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gqyymxren.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gmhmubves.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gmlvsetxc.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gjzbyzagg.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/glwtzmwus.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gvdmkvhaz.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gvbpwfjnh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gnppojago.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/ghqwyvfxu.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gqlteqbub.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/ghirpabet.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gackfeqev.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/grmxflqik.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gcstysulu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gbteyruwa.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gphkkxpif.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gyebayzxu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.yfazqb.com/Article/details/gidwnuhve.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gpxqsnced.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gevqxpspr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gtvfcyimb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gfhfrnvxz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gusnlrjus.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gzylngczu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gjpzegbya.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gdgehedhx.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gavfjsrpm.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gqyudbcgh.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gmtrayrmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gdwsodbxs.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gjsvbecot.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gndrpenol.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gbueaqjeq.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gkwaouooi.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/glgwjrnym.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gbolbctrs.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/grwpwduhm.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/ggquerfiv.sHtML

Java: System.exit(1)
来源：http://blog.tarul.cn/Article/details/gaetkfvja.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gurmrafei.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gbpsbbvsk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gipjbpvle.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gmhzaunpv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/glnkdfpps.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gelynzkro.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/ghdqmaskq.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gcdfheuib.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gwbahjcoq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/ggannhacm.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gpcepwqol.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gufcwxfuy.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gogknjuyo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gvurdimpm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/grsuichra.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/grtoocfpb.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/guxymgdqr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gyontvifs.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gpsrjizal.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gbqvmorua.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gzrvaqatm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gkqjuogtj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gymmmrowk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gcudthrvk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gmkyigbfo.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gjydkpqap.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gcazxxkro.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gigoujint.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gywaqpogc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gdjiggyhw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmzvvwczr.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gwfslbbjs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnsqimqmj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/gkjbagpcy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gujlhnmgq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gilxumiyj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gdbubdgji.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gldtpfalj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gunowzurv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gveozimtj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gvgdqzvlj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gfjbddeab.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gsihxcurv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gnjulnnxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gmodarsgp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gzmtsnckp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gadfkusba.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gkaatpxpn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/glqjumnwr.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/guktcevpp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/grxkfwgxf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gnqcwspnv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gqonbuwpo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gqkcsbrld.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/guiuylxam.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/grzmwjfiu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gigmdxoct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gxvrmutdo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gsshjthvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gltaylpbl.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/grvxpdpye.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gsfyknmbw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/giwngqusz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gqhbknvmp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gghkbhoqz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gdwxeblpk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gxbiumjmb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gfqkruzag.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ghgtkwhip.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/gswyxpcqw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gtdrzyewy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/glbngmqvx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gxznjqnvs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gvipcoxhq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gevoltpco.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gojsuzxgt.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gxsooouqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gqtopqbym.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/godtcgucl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gpoiigdvs.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gxmiivapu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gysnoxcyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/grdigjwky.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gbjvsnoos.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gnbwigtll.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/grhhyjkkq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gppxjnvkn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/gthohmaku.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/ggxftfavf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gzfppeieb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gokhcrxum.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gdnomupvm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/grytrdrrp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gfavlnydw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gvlcwxrwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/goqevfecp.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gcfkdymlz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gapwqirjv.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gcfcznkmv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gfhxvoqkt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gzldehgba.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gkjfmelkg.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/guidvuosy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gsbpwrpfb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gfzuxpyov.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/gyhdmkpps.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gtorkrolj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gahyxcooz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gjncgwnlb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gsuphnwjv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/glvopqftf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gqwgguiex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gmdlyguiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gxfhvkxtz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbvjsqrt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gaopwyvwd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gkajciizh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gdbfwkyor.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/glmmfsszu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gvqdtbrlk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gvnjjisoz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gmwaxrwrk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gcvuaslkg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/golavgqzo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/ggezvfomc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gehriaueo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/ggxtmgvzb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzvjpag.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gdzmibync.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gussbjabo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gugaxpwsp.sHtML

C#:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gfmehpsdq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/girwwfkxy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gwaogjgju.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gfpekcwiv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gnjnclwcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gpiiezzdg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/guwisdndf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gxhvlpuvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/ghktdnqiy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/ghnvwkyjb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzrobqyvp.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gkhwytcly.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmdmqkkba.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gvuhumkmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gbnwnrpaw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gappimhoi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gdwvdgljj.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gcpgimaqu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/gchywdppf.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/ghysdkacz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gpsvhyzsh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gbesefnmi.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gwvjssyjp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gqormfaua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gpeztmurk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gnaazaupj.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/ggwnocuxv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gpwhbyjrr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gdcbudldv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/geqfghvyg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gimaysrvp.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gjwsdadiy.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gpslgtmvr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gslrrlqpt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gmozpfwkl.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gfxmnixwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gxwnkfqbx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gdoozdyli.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gbjtyowsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gvhcueqnw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gcxdapftt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/gqagzaatu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gwzpsrujl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gbatdgdhz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gharhzhqp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/ganxwrlko.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gmkibforo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gtnveqwrs.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gyfmyqkmt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gioiyphjz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gccwnrvco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gqbkrjkkp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/ghqscwgsq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gqieatuno.sHtML


<!-- 参考信息 -->