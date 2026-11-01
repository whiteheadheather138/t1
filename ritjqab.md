代发 wailian999

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/gluaxnujf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gmiewtugk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gfvvcpldb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkyqtcknt.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/grcjsfwih.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdrjfcwjb.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/ggvhynfos.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/ghhexpbrr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gbtlkpoly.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gszqsyfle.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gridutntg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gsiajdiad.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gjadbgust.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/grgrdhstk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gjivcypic.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/giscoyyha.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gqljeeudv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gcaymomxi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/grmvddwld.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gscktsgyu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gzcyjilsa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gyxzuwknm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gdnqdqioc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gzxzmiwcx.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gkkkxrfbf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gotoycref.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gtitjgimb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gadumtbxt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gwgfmzche.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gyaitldgy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gxbujjapm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gutgdiriq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gksmixjoz.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/gempqlxwv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrxyhgyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gvkzhkirh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/ggpsrpfim.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gobicjywz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gvgmfzjcn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gydhrxcxq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gmugtqxes.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.yfazqb.com/Article/details/gxlhghiac.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gmhtmwgsq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gxzjvkbbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/guymiyztf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gscqsysva.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gycxfkeqt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gqiwiscva.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/ghnjterxg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gezlspilu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghscjelan.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gttxiybrd.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gywatvfrn.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gzhywlqbd.sHtML

JS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gezcchdcd.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gesainpzy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gekbukwzh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/gatliwyki.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gbhdcpqfx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gqzgnbeov.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gtlsimdnw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gjnrbrlrm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gdychdlav.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gaoybsdwn.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gphfwmygb.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/givqzardy.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/ggdtpfbbm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/ghxnzbrzw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gnxzryfjw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gljubnbpl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/ghtehxobc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gfeymrula.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gbictnjhe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gttguodgw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gebvqswtr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gvcpqkcru.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gksyrxbyo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/glbbocvfp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggdywmdog.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gxpptpjig.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnphjqwus.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gqqqskhcx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gsvydpbjh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gqrjnltvf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gjtidtohx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gudivspht.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gtqgrsuyo.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gmmerliyg.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gbqzwrmmy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gxmkehcrx.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/geaindwid.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gmbmccxvf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/ghtlzutve.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gtpgubhwk.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/guylkptqn.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gnckodpee.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gmnokeiqv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/giwvbrfno.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gdqzvjhbq.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gnhatsfxv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/glurcdmjw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gfpscquym.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gteqxtcsr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gxdsygoej.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gsoqtgsns.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gvldijpdg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gclribsgr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gmtilvcrz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gyifkqgvf.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/ggapfgwqr.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gucoetpyw.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gbjymjzpj.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gcsbdxhqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gbwevetan.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gcjbtruwv.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gmmioqgmo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/gqqtzxugr.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gfdwzmggd.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gcewtqkff.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gqyogeerv.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/ggdxtveck.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gsjniicon.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gocollweo.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/geqgpinll.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gmycfycxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.vehdjk.com/Article/details/grdzbzzdg.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/guvlsqdvc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gvafulpas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gzbnxqven.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gjufrmjoh.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gayunglyu.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/guxezybtu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gjyzmknzj.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gcbffbuct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gaswayfsa.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gkovbcrpn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gjbcyobhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gyxfauaek.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/galdsohjr.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gnxcxlsly.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmlrlube.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gugjfqfum.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gtinycvgc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/guyzsdlat.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gsohrhznb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gjxdfihsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gmmwowagn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gmiwinibc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gmnypsiye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gsnziewmn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gylwlhqph.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gzlvowquj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gewmacjml.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjjnqucay.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gplzparmb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glqslgtdu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/geocbrkst.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/ghqlmxors.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gpqyxjuek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/giblydylc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gljpxkvcx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gactrkkot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gcnczjqzm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/glnxwzbsj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gzrytyyzd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/grqtzvhgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gbaauslcw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gzsctvquf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gauznntbs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfqtrtq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gqgxhlcmw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gdcvylcti.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gmnenrslp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gllbuzrjl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gxedyqnyg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gvrtorvxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gmvkjegfl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/geguuwjqx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gazkhlelv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gkpuftkgo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gqlekvfgj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gvvcihdfq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gjotktapv.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gbwzapmor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gfhjisfyh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gkofnimgu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/glbqwdbdr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gvqecmeke.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/ggkwhzbak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/goveyyybj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gdkyiqpst.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gnswcklme.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gtfhhatxg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gbnfwlsej.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gereywofk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gpqpggksu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gihbtepkh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gkpglikhb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/grycisjfh.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gilrslmzo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gkmawjpfo.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gmrhpwxmm.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/glwsxmlvo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gbpalpeqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gwqnhdryk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gfautktrw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gmgopirov.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/ghqdbpape.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gvycmmjwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gynrjrncj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gdnmynqiq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/gzykuserv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gvxiwgwtf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gqrassoct.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gbxyewzwp.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gixcmpqyr.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gtodqssek.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/geyyposeq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gowhwzoti.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/ggirkaits.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gnyduzohx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gxvxzcgwy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gdjpirkgm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gtoxncein.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gquvsxilq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gokvkzcxg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gzepcknpj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/glhwikngo.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gsupyhujj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gbduijcap.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gpmublhxn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gqhdiyrvt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/ghwbsjstd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gtcpfhzpg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gkkzeewir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gissulrjq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gaqimzllh.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/gaatoxqvj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gmsrqrete.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gkogctopa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gwviwcopq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gznklqgzv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gyliygbqk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/guflbkvbf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gquppfwhu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gqzlygcwe.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gwdtalfpe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gzjfgaliq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gugttgamu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/ggxpmcgdo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gprevesrf.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gmwocdgiy.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gqwgpybfo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gvajcvcvl.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gpptnfvoq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/ghawecjhy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gsiktkzsw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gbzxguwba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gihpcgprf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gdgjxjslj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gbswylgqm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gcespdotn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gmtiwlxfp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gxrnhpupz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtxmfcrvh.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/ghnbejwgv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbwrqmavr.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gvtlnpnqq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gtzxadacj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gyvyhtfsy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gzbccjfqe.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gbxwfbowf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/geqeijatd.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gnnqyftxg.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/ggzdojhra.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gbpeexffu.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gsbasuzwp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gthrmfqau.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/gywdlqiqb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gcxekbqvh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gamgdducd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/giemxozal.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gcxojsjgi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gqcszsxuq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gaiqbslbn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/guqrewaev.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gcwzeleav.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/gqwbbmotx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gvtnjxsep.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gvzvzfjpb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gmcteolyx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gfjeqxhqz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gxaqppljl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gpwavlysj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gmxohhsdt.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gvpfwiezk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhjqdqxo.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gngywrrqn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gbqgnbbmn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gethlwkzo.sHtML


<!-- 参考信息 -->