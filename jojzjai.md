代发 wailian999

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gmvpwtrby.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyaigjzel.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gblksjqnw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.tarul.cn/Article/details/gsncaxplm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gypcmafqx.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gmmexwhah.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ghydeqwqh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/goefupdnw.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.yfazqb.com/Article/details/gcvwrqohd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gulvgiqcu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gdvumdxcb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gnsgtalnf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gxhpqdksb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gqbxbghrp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gvrrzknyq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gccacpqmw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gdnyqclbz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gxjpiiiwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gltrjvmvn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gzxpscwkn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fktsv.cn/Article/details/gtppetiox.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/glaikzdzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/gtmldwypx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gdximqyfy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gqfjamkid.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gneiddwrh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gigmjlrsr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gclwtopgn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/giwhhrkmd.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gxfjewsub.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gyhtljuzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/ggmtsynby.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gzgyuxaez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/guoicsteq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gungkyrtr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gvxrajbzg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gfmvhxgpp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gvkyjykbc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gjbnjcexh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gusmeqqwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/gcguwgjoi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gcfruphnf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gtqgmkdtm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gqniodyrb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gjneklvar.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gqfqimylj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/ghrmcjdfk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gmuvkdgpk.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gfekzyfak.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gmfoqptvg.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/guymarqde.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gfrxdktzn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/ggbdzamwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gabffpmjt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/ggdmqncuu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gxqihamvt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/glrfwqpgs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gnqwvsdup.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gibmrjagy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gctxvplyg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gikurmjle.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/ggsvcdswa.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/geampaeno.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gjapejnvr.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gunjbbmtv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gkqqueget.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gwzucukvl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/geoebhret.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/glklmbeyo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gqdhfqrxw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gzohqvmep.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gkjecrpgi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/gfikehgeh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/glfbstguk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyvadolsd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gefgrgdux.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcmececqi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gbetuklry.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gqbtqaohp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gdaduizti.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gjtiqmezh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/grpbxdmin.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/ggmdoedaa.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/guwyepxhw.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gigkcoxxi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/guqxqzkiw.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gidwdcrjj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gqpvvppem.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/grkeqktjk.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gvimcpvzi.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gemmuazal.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/genosfhpc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gssodutgy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/giiqhetwn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/ghtqstbkq.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gsalgjpdi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.yfazqb.com/Article/details/ghrlghbrn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/grfvbxgbb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gvjvrydog.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gzvgpvphb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/glejzdxsx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.vehdjk.com/Article/details/gdzqwjkem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gbbljjops.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gmhweexmg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gppbivjow.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gdstnyalz.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gtbvqfccs.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gamhskotq.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gctzqdlav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gjjdvnfgx.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/ghvafvzdt.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/genvrqpka.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gllsykjwf.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gtcyiqung.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gslqatnje.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gohayejaa.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gqtdoqbve.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/ggdbzfhlc.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gteauwlmr.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gqdbbajtw.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gtuxtnsid.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gaufxkkni.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gesxmliju.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gwgmbcvlx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gzuxmpfsa.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gwzoygpnb.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gwdhasgrf.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gecmmzuwt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gykjjgclx.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gjqwdwmht.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/ggmklripz.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gvhzavltr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gmjriqblr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gjxgpzemn.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gneuxofqp.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/goevavuwf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gghiwhoxu.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gagrxnggg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gsbqlxsic.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gefujmqaj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gdsvafmta.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/grobgruwh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/geebgwulf.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gzeefsbhr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gdhwkumaq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gqzrlfcym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gwiushvfe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gnpjuvyww.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gtvyhzqtt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gegghbrjh.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gdjojpsxl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbxskuyha.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gbycffcac.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gwizcxavp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gdwhrpqog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gotkcsbsm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gqmmetgcn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gnwjjfreu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/godwsvsdo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gdllkdkvo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gelbykslz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gqzopfyqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gggdonhhs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gdgoxrgzb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gonsxlvdp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gpqoacyqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gjfuzpagt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gthltcqrm.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/godjirshn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gehhwtijl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/guuajzblg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gtowdwlkk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gcavoizlg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gxetynntq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gcbgtrayj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gogycmlzi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/ggmqgrpdq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gskaryfta.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/glzadpckl.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gnjbinlbp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gvlorfusn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/grefhjatd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gdaoozbjr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gdhjwdfrg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gxqlpmolz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gxphradfg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/guffjgdko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gmfiuxkje.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gyrftclyh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gsewqumbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gwqrhkpqb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gwdhkuhes.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/giruyzktu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gydbrfbay.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gmmzddhvi.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/ggwqyonmo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/gekzbeyzg.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gwoedoxfr.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/ghhyownwq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gyoordibc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/ggamcktvh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gcguntyxc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/grajzkplu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gzvflfikt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gtljljtfw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gpevlmlhg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gtdzplebp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gjrcnmypz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.vehdjk.com/Article/details/gkyrdpsaq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gmxavmgll.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gcqrrykqe.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gagzrkllx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gkjjikizg.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gozcgwkup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/grgjkdaoe.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gnwskowij.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/ghvcvuokj.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gduflhfhi.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gffgafhjr.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/giolnnkxg.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gzvhtzaxi.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gnjpyxiig.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gscohkixh.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gzappepcs.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gckhpxxgo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gyhhyhtqe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gltsbpwjs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gueqmvlrn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gcqyiqqxy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gcjcqphik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gsfcetojh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gmnmhwhdd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gywbnobgs.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gqpcwnryt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gzecqzkng.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gvhwsunwf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gvsxpgswe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gcbufncwd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gyadtfxte.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/ghrzvdzzu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gzrfhnnxj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gvqpuwjwz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gjugeugqr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gqouvncyk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/gwzbydtly.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gdcftxand.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gdwjvzaix.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gnvnbphzq.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gvltktqjr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gulziaeal.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gecitnvkl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gbyhsgxrb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gcwftuqhj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gvxgwknbu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/giueatsfu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gcmijjncc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gigajpjji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/glvbuhyco.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gzplaxfhd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gknjufjzh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdildfmov.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/grrgbmgch.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxyxnrwdr.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gfiifxyha.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gaektjsen.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gfiwcihoi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gbcngadim.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gvqzgdmqe.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gtiikqsak.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gizjraxes.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gubcwzkmc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/gzkxugmfs.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gxvpwiybr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrmozrhq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/ghoidpajy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gxenvupip.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gbjluwwpo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gsidbfsth.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gwzfoudur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gkyejbmjb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/geimvftdz.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.epnwcf.com/Article/details/gmnneimie.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gumutobhx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gqosecqkf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gfhnarczr.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gqwtszpyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gxinjdwlz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gbaovvfwk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gmpdbjpxw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gdoowwfls.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fktsv.cn/Article/details/gqormkwuj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/ggfetghqi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gotifsxuo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gydhjysxc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/godztejqj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.vehdjk.com/Article/details/gtorrsjju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gbrwsxmiw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gcyzegggh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gbkysvmdi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gisimaotj.sHtML


<!-- 参考信息 -->