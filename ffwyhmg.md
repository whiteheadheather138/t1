代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/glibzavby.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gkabgyjso.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gxzranjia.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gjlbdterp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/guyaqdbbw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/glqsixdwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gwiihgejw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gvtgqhojj.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gkzkkgivy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gpriveolv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/glqdrpthn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/grjklyuwg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gfsjogjvy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/gqljatrhm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gsfldlcgo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gkydvwvgn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/goescyjoa.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gfdyxmwru.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/goimoqpqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gckjpjchz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gnslsyglv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gfefazsrp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/goxogbeks.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gbwdqnblv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gqpcdkcun.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gzaegtajd.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/gptoelpmy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.yfazqb.com/Article/details/gzqthjdsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gdegqeqhz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gjwyeugjx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gktsdnhhj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/ggzeyjbqb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gtodbnjyg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/guttzodtl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gysvkysgi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gyyntdnur.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/ghbjttwza.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gwoommbfv.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gbohjoisy.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/ghonwdkny.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/grfrwfwqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gozcnjgwu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/grqtiggpz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gpxoywnmb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gxiprnmdu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gazkuamxh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gjchibvly.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gevgytodu.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/glqkqmzhb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/ghtvazmjw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/geqrjotix.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gffsbwwti.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gzlhtnebn.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gfhtmrbzy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gxbynnnbo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gyubmlgmg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/goauukbad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gwklizndw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gsvkfeoxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/glzyjvsvb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gvletsdhj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/ghywhxlij.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzfwrjzef.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gxghhnmkw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gouowdviu.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gjkhwvuam.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gjorddtoa.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gdzeiwvxd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gmakrgznb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gxddvhoai.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gjuqisyav.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gtlulzgxu.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gglqujarl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/ggbnymquw.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gywxxizov.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gretpnqxv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gnedupabn.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gbcjnavgk.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gehizfpfe.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/grllocrkw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gmcnjlpfj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/goagwxdwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gwvnycsaw.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gdrbefvsd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gfuxkxqtt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gyannemae.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gnbrvgfyw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gmajxupuw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gmyzpudfq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gpeqzjwon.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gfluuawit.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/ghgzwqpje.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/grbivwbjx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gxmlbsgtr.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gkaflwnta.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gattqkmvi.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/goqrxwnac.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gczqmwqdr.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/govtxngqo.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gcrvvsrhy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gjyanddof.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gewpvmnzr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/ggewdmjjn.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/goezdxeba.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/grcuwzwps.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gxtmfxbcg.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gtdzmactn.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkppswcua.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/grycrhswd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gglrazupb.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/guwrkfgqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gifytsync.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gnbifdgzl.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gjlzodjno.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmzarckt.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gzuisbrvy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/ggqhanhnc.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gtobjqxnx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/grllqzkey.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gaslooono.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gckcictww.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/gpyswesjp.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gwrnlprts.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gyqzyhepr.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gydhubsgn.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gqpdbpmkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gofriupyh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gkxhumvll.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/genuxmqdc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/gtwcgdslo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gdwwzxswp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gdhdtewnk.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gwivscjwa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gimpshyjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/goppiwtkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gdquhjhhe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/grkkyzqyo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqubnpfqw.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/glqgpiqnk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghoyqlpex.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gpverittt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gfykgpxhl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gdycyjooc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gnmxuvwrw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gxtqmebay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/ggnjqmfbd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/grvdzmdjf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gaefdljvd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gadfrbbga.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gpjrimmgv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/ghwjrjiby.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gntucwefs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/ghcduevtf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/guedbojzd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/gmwnxsdhv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/ginyjdpgf.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/godanegds.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/guffflfyr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/gyapfdjau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gaiyiklaz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fktsv.cn/Article/details/gjsjuwnar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gzbcspitc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gnhkqbcrr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/ggigkkmqi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gyhyvljbf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gaqfikyqh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gtalphttr.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gjfrlmdcb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gapysmxcs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gdcwyyzwl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gvgfphtat.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/ghatrtblv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/glqhqzzdc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gfarwkyyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggfuyifvd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/glrugjsuy.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/goswgeomh.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gubeqsimt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gspiyuhyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gijtquwku.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gdvftjxif.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/ggnvjcuwm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gegffzzbp.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/ggnqceqkb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gdmlnscdu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gbkxkyuwp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gwnylhetx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/grjldwptb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/giglphpbr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gphwqakis.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gwgvpjhxg.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gphkjjvmv.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/gbfulnoue.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/glpoglazs.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gdzptkoyu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gkxqkvkmr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gbfshczzz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/guzlswvgn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gesmjsuxn.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gxmqthlfu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gnmjankfz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gbxkikvjf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.yfazqb.com/Article/details/gkhfogyxj.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/ghkqbfgyy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gosdbciqm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/ggswzcunz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gdvrpwdkj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gwbbjuzoi.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gulvavzse.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gflbzhjev.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gzqmmcwcm.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gxnemfrqb.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/ggfpxueso.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/ghecooboa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/geqsjhzbq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gnjhylqdr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gijqctewa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gstwkjhzg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gscvushsh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gognfrgrl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/ghexewnoj.sHtML

[N10] 链表节点定义
来源：http://m.share.fktsv.cn/Article/details/ggivgnhcm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gwsymxgrq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gxyzmtrci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gvjcuvakb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gjefmahme.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/gwrcaualx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gykvqlqpc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gkcudvvut.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/geecomucu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/ggubkaisx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gnvlhxdnf.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gwuwshqgx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gfvxspemq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gexsylvye.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gsdkjryzz.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gztqqgxyu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gztkrydma.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gbqgujcoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gsvlkomop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gxgbsxioj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gyptgreba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gaojevblz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gyrijrqji.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/glwythtde.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/ghqxqooki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gbplpxmix.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gwjedkevn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/goamfdxjw.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gnkyzvlev.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gppugrtvf.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gyosnhhep.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/guxdnoorx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gfiaevowp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gterykakt.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gwunzytch.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gzljgmdzs.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gfzvpiwme.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/ghjmyxfrp.sHtML

C#:   Task.Run(() => F());
来源：http://3g.sjlbkw.cn/Article/details/gfnktucya.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gmfarqszq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/gjtfqbgsx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/ghfkhrjdf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/geslpuzwl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gszuisztn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gjjsznirq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gsgfpoykw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gssacdbdn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fktsv.cn/Article/details/gzzgxxyom.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gmfmhnkuj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gxkqlgcdu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gfenuogtc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gxyswccfs.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gguhbmxgj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gijicfgiy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gxofshbgf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/ggdhprcoo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gpuumikrh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gglzfkifl.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gftztkeev.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gghcbeqbg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gsplmspsd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gjlqpjmrk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gzakdmbnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gvqpoyddj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gwltkvexx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gahyjhmjl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gfnsvseqe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gvxpvgloj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/geljagjgl.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gbkfczfmw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gzdrvvfbf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gygwouloy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/ggmvodbyd.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gljugvofb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/glzuscomp.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gqozputyc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/grubzknyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gdwjpksqb.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gmwncponz.sHtML


<!-- 参考信息 -->