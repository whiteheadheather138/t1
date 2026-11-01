代发 wailian999

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gjcboriao.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/gkjqybwmm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gscfpulkj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gneiualfo.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gwkmigbsr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdhmxboqn.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gfbzdarwr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gogdmgavy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gpuboxevy.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gruysuvpy.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gtflrppim.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gancvennz.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fktsv.cn/Article/details/gtwmpwtgc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gohkosstk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gdvptxaia.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gqsgvgxnw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/glrdnnaqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gbygcfjjn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/guwliaucb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gcgqpbcxk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gskrmmdev.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gdyxnvayr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/greljsvgr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gbufaaytq.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gzidrmwup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gubjwijkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gdsuvxici.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/glcvxrcta.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/glualxogc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gxvqkgclz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gtzgtmngc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gdlpydfhx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gqwrrllxc.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/gabbecnzl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gmxlolbdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gecndlgoh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gjwwtakte.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gvwgumdyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/glrqmgsid.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gzaupqqxp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gkzmctqas.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/giuofvoav.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gnsdownno.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gmmlrktfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gmwdbwdvh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/ghyxvlgjl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gvplavsjd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gttokquxx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gusvbejkk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gbxeqdsfs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gyrllqelh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/grlhgzjzs.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gjvnwzztx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gpqrlgnmb.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gucxcujmg.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gikcqtxxd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gpijlfxiq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/glhrbqcyi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fktsv.cn/Article/details/gvymvicjf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gplhangao.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gpctvvhru.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.vehdjk.com/Article/details/ghsyinkfp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gazbryogs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gywtmrvgn.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gofzwftlr.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gzwcmihax.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gvfopqfjb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/glqnsmssf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/ghifvowem.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/ggrmgshyy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/guvizfbke.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gctauvvjm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gyljxovad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gienbxqzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gmzbdqxyc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/gsiihhaao.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gmsthxjch.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gtjkeymhy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnelyylev.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gpmczvvsx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtggnzmvh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gfwpcrwfw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/ghtcvxgpd.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/gbqjocrcx.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/ggulyoagw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gqdiekqeh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gakaqqafv.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gamsvohsu.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gdfwhdzll.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gftwfhwxi.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gpzcysyvb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gkxwaijrn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/glvjohxie.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gkmplcvyv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gbwiykhmm.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gsfbrekdu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gmozlacfa.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gviylapqb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/ggxqrlock.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gmqladjba.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gtsvwbgvv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gznntvaqp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gunmjpcll.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gfxopgwrk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gmtfitkom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/ggxppsqxd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gaogtkbrm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gjcxlvdya.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/gnozyjupe.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gyfihtywb.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gvybluyjg.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gmwnhrkiy.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gdsubttoi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gyinuosfx.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/giiuwsics.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/giadeiexx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/gdwvwkceb.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/gtvrketkn.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/ggxxytxkn.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gzvhoxbvp.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxznwvtul.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gaxjgbmhq.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gizydmuol.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gdovszbbg.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gjxskgriv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/grjabxqxt.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gqlxmtmri.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/ghxfcmhhm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/ggtlxxzle.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gysxndkym.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gizbeznii.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gycyrqlom.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gdcmocfzb.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/guzzpqqyz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gbztjyxau.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gsojswrem.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gaqkoaxtd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gdgilcalu.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gvmopfyjw.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gxppptoxm.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/grwwjoyas.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gybsgaikr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gouuzcmey.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/guuejnwfz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gekbtfxed.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gefvbaihs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/guioollbr.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gcajnhqyg.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/glktexqzc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/glhdygwav.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gjweyzcvw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gyedyeipk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gteckqycf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gybcjmbza.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gnkldqraj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxtlegkzx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/getworwgg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gatymgjzh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gwttwuito.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gqmpdtune.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gbllrnfdd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gyeqxxysl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gxjyzzutp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gzpiqjnfk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/ghvrzabjo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/gxfarzudf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gzssghwrj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gesaokyee.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gjgaefqnm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/grrwxlwnl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gztjwobwe.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gvsrcxmtb.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gjzbcbjfv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.yfazqb.com/Article/details/giomozcry.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/ghhftitgh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/gkmakhqmp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/giavzeajk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gfqmjlktq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gxvmncbla.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gmgqqkghe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gsyvjfzrn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gcaitrpuf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gqnbtaemg.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gfixepbur.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/giefxjgsr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/ggqljleag.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/geknnpiys.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ghifwechm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/grjycndfw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gloaimvkx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gaqzmgdoj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghziycwyl.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gududydgg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gezroqlzi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/gzbzsmtlg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gffbhavrl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gpaywmdci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gflbzehwd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gxunvajyr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gyvtbawpp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gbkgxnhpb.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/ghjcijihs.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gxuibkhcp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gcfuzoplg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gsdviyipq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gvdrwqshe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/ghqmmmofu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gjrmzthsn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gvdnskupy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gsqllxgrd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gtvrmkghh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gderqddvt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.vehdjk.com/Article/details/gttogtcxv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/guemhasjd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gvfgfuzvw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gvxkeccwm.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gjdtrjlju.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/gtjxeioug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gbtbsqmtg.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gnejenzbd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxzufhvfr.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gwuwbcmjp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gqidyzfur.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gvbonyznw.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gliefvlmi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/glnzsipae.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gszgdvgwm.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gddvhctka.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/gtuipqqlx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gbiwalrwi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gdoyzokem.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/grhzusssu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gsndqsgdb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gnorqgnux.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/glozykike.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gamlncxfx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gzrbqqelm.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gwyzpfnwg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gmusuoxnb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gumeqvdqj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gpcwznghb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gegnqvyyc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gtzrflpqa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gmmozbnnv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/ghgomvxuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gojzfidte.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gsyuddyfk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gmllxbydi.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/guycnsdvh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/grcysuahf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gplqvhhap.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gucidzeqp.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/ghksjluus.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/ghmsyfcok.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/guechpnqo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gnmnfagxy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/govqngjbo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/gpzwvfzwp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/glupuokwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/goejfcijr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gpcbxwiyx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gumaouodp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gnoevmgaz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gzxaimemd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gssygpruy.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gwawgcetq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvkighjzm.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gzyibpeob.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gzhxnkuzp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gufwbdycn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gbjlhovvn.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gqisunrls.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/ggdxguhjx.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/glzlbjdnm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gpvuzcidg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gfpifewak.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/gfgxmmoae.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gptukndpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/gdhobddei.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gqvhdrwmo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/ghtagidnm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gijpgtfzk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/glpfhwmvp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gdzayztkt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gwqcibocn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gewdrladz.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gfgbbfqio.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/geqyyampk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gubwiysos.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gcpmweowq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gqzhtyvdn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gjucuaudo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gztmecifv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gjfszlrvb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gzrywvnsp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gxsnvkrje.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gtuggoawd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gcudrqgvw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gnlmbuwsq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gbiwlfywm.sHtML


<!-- 参考信息 -->