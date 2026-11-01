代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/gytealrjq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gofzxffhy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/ghvhihsjt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gglslsxbp.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gmcvxyznv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gehixdmhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gmtmiwsix.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsblsohux.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gtuowrrbe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdymlkwzm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/glegptquq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gxvsfszfc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gbznbtvxe.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/giryyjtsr.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/granimgev.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.yfazqb.com/Article/details/gibdansgk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gzfwjuqax.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gpcjeisas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/ghsuzkyws.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/ghhukhtnw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gerokhlei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/gmvbyvmzt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gogtykicd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvhffmfo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/ghnfyilrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gvoloyjro.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gjnqqoajb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/giaygahlb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/grbrsejgp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gkqkkucms.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gvbegdodl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/ghcrrpauf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gxfogffts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/glstqsvgd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gukdyzicb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gbqqlwwjw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gslhjrpwa.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gfyyccasm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gwyxudgmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gzlxtgqjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gvwyofqpc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gisevhssd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gjmonitzm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gqtqulwwa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gesoenoyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gqintdwwo.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gsergftey.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gplneirfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjoraazi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gkcmheaqk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gjjpeuutm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gsrmqkeza.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gcqxfmulj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gqgknfprp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/guvkhrqld.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gvtdetowm.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gfmolnljy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gxzzpnxwk.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gqeqqhtib.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gdnmhifyg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gpyfmound.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/gpsuupthp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gvxgroctf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgrfwiun.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gybvwqjpu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/guvdqlvmf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/glssavfly.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/grwpbvwed.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gnqrnychj.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gdfradxxb.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gmlkmxwbd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gxscshbme.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gzolkjvgh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gvlwrwimg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gskyzohok.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gbedzvesg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gpisahsem.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gkttnszwi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gvjfnennv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gwuyixjyy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gilmbhniv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gnylgugrm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guahdooia.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gnsfufwnr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnnibfaqd.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gsncucbyy.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gdhhoucwt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gkmrnhuvh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/ghoacgbnm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gyzvtlubo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gsdpezxbi.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gpqlleura.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/ghmdorbnp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gfwbiqkkm.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gceaycgri.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gpbllcebk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gkxryrgau.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gftazthvc.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/grgwoxype.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/grvujrlcr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/geiofqizl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gcjxkjqhg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gthuyvycg.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/grrsyulji.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gqdnhgghj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gajthtndu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gqwxmcwid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/ggvftlzso.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gogtokolw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gqrlougcq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/grikfqfux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/giyamveoc.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gzlvhekzh.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gyphinbuh.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gvsqzdisx.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkjvpyxfq.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gqymslcry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gptoebrjq.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/ggvnutipk.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gqwqhmenu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/guttyztrx.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gevavmhva.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gjiwupqli.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gogytanft.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gvfglfxpu.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gpwphqujo.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gnaxtorbf.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gbdwkaszq.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gdqymgrxr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gmbpuiuve.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gbgotwinv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gjzntmkrc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gblwoedmt.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/ggurwxwyk.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gcbdkgzxv.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gvstmwgzc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gzsuiplob.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gzrjptzrj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gyqeduzqq.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gabodwahb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gmaznvwid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gifkpfgnv.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gugufxzsr.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gbeleewig.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gkmdluwjp.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gucchrbrk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gkuvxbhlh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gdumdjtri.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/glaavfwvq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gyqauorju.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gecstuopc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gotxevhch.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gqsglefax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gnldgqfow.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gyuusbhpr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gftwdojcb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gdsxfqhbm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwiqdvoce.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gevsuzfvk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfaoobkxk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/goyshqniw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gqdsyzxfz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gbiapnzsb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/goqpnbdjq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gqsdjozze.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gmmwtufao.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/glfhmbbzn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gtoivafdx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gsjgxiqcr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gmsyourng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gxlhcboan.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gqbyexmix.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gbbtnhfgd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gounmcwwb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/gpxqsuzym.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gepnlmzaz.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gbemcitiv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gbxjwhfsg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gxaqrjzqg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gykospyhn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gyrscfwai.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gierpgjyc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gmmhkvuos.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gtphrddzq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gtnzxtkrv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyfasbgd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/giedqnosd.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gbqnrbdpn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gzxlxxogu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gtsutippy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/ggtpoyasv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gjnozheji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/ghrxmmmbx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gpvemztst.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gxedgmcxp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gmfkkuzhv.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gvprjmcnv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gjvvayusn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gfkirwmzq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gvalrqxxc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gesfdptbm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gxhrtsmrf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/glodefxhu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gcgwhcsyh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gqaemlqji.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/ggshjkauj.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gkwvpsibx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gxixydddi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gbvseodcb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/geyojrgqg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gxxnbemuj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/goiepvcvo.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gscsepzrx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/glonzkcbr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gsoxtcuwu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gltvzztlf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/gqkxbxleb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gnxalthkb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gzidvnoin.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gmsuojtmw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gndhuzqnc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gseqzarod.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gugihfsvr.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gprxcpunr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/geplqvcji.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/ggrdpmete.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/guczfiylm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnysfockc.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gciadjwir.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gynopuuda.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gjosgkehn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gtldlonbk.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gairjtjlf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/gzsorqxic.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gefenazfm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gjraxolnx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gprkkiobq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gwbqithbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gowlyfuoa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/glvfrlzmt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/ggxhxwtha.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gdtgpgezk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gbrpxhqvm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/ggbyvtprx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gdurrwecj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvjetwgx.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gxsaxmcnu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gplxqycax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gndakfmre.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gbvhjudal.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/gekfjdeia.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gzffqkack.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/graftpkrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gpjhpptmv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gxnfyvhhq.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/guztpjjka.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gzedcmplw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gqvxviaxq.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgxydtpp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gdwmdmqha.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gkvjxcbbj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gqgebcbyi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gxxxwrdrd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/guqkykold.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gbyadyrpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gjhzpdcyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gjebnkait.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gehfikuno.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gctopuqys.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gpldzmvqj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnxvlymfe.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/geexlrmty.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gmmetkjzm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gqbnxnlgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gwkctthlq.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/govlnsfii.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gmdjtlcme.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gqivdpfpy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/ghvwtyzcd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gxkhbjecw.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gapbapzcx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/goansulhy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gcveatfue.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnasqxiz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gpemeqwwh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gacemoxxi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/gdoezhbly.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/gaesbglak.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gadhhjhke.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gjqnhypob.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gpvkgzbyx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gzwrnveyw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/gkhuqceho.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gaaisgpht.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gbdjdtqpv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gmqoxhzcb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gmdjdcbsh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gfwfyzwyl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gfklxglah.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gsgnzrrjb.sHtML


<!-- 参考信息 -->