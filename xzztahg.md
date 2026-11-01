代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gkctqnhji.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gujrxoens.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gfmwnbtxf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/glpchracc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gmeufzyls.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/griowqyll.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gptbqyczm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gibeoazfy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gslvqfjmq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/grytgggud.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gzotxkjvj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gyxytnimh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gmhirmmjy.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gjothivzv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gdyuehawf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gppsojeab.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gqiaocznd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/grepctqgh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gnfijmmty.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gnbxsqaac.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/ggazfulcx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gvmleogxl.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gcoshnuhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/goivilxwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gmwqcnnwp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gqaghmmas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gcpyuaxrn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gmsebzwft.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/gityyuyyj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gmfbogojp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/giuadtiap.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/ghrquatoi.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gxdmtfjuz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gnqkezkgc.sHtML

JS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gauzpstfy.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gnhpiqsqk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/geagrejtd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gmcummicc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gkstktgyq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gztpqtjvz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gjptibueb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/ghibancjo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gjmpigfam.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gbisilncx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gwuzlxzhw.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/gtmmrnstn.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gyygefrax.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gghrbenqm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gecimrczp.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gkfcabqzm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gpejwlwtl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gbworwjnm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gukzkfmfv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gqgjoflik.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gbwrcpmbb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/gocvlmzup.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gdhvinwls.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gkuzxtbyx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gedophswn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gwqypykyp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gymayscap.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gjznbvcbi.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/ghxhdqkrp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gfhpmaduk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gpvxwbvti.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gwfwwigxm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gsertvcti.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gjtvbtvmt.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gquxwejtq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gxjoueijj.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gclvrnbhn.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gtvwieyyu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gqqfrfqpa.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gllhhdukc.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gcaiyhqdo.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gyqflxwhu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gorrfpait.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gdojeblkf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gtiqxyfpi.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gokopdrzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/gmcexrmvp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gbwwautwy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/griuxkbov.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gnttixveu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gfnbeegia.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gvbwzywoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gksgokbhc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gnysieyyi.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gzirxvyip.sHtML

Py:   os.getcwd()
来源：http://mobile.epnwcf.com/Article/details/gyuawylov.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/gqteqlllh.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gwezvzjlh.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gbkeuraql.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gqdxjsqhd.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/ggtlehghm.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gjhjtzsrf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/gcwuwxibf.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/gmdbdfjfe.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gehnmxgyz.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gustyyejq.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gmfgiupfi.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/ggyswporh.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gfuryqifq.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/govhrahla.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/gjohomnzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/gzjhwmzxi.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gdaaybhky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gxulavkpt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gqqexhdix.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gbchtvmxm.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/grehqasoh.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gvtudmjiy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/galcinqwd.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gjayjfhop.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gvshfmlca.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gmwasnekd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gwcvrggep.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/ghlfeqzby.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/glsotrhok.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gkqdsurfo.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gyqqocvhu.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gyxfjonkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gojgedhkr.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gmaerbujb.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/glywxxqlg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/goaxrxamh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gztrsurgx.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gixtclbhp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gkkpbrcyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/ggzempwym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gybjozhns.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/glzddbupm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gknntckwc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gevewnegw.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gzxfrdrqy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnzewhzvw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gtgccycxv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gderfmzcr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/grbqashqh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gdwhpkxmo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gnqekrwgx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/guzoljzmb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gnaitamry.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gctvwcfii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/grmxlnxxv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gzkgtfpqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gvklgiybi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/glqptpggc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/ginyvwsin.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gnygmecso.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/guiwbpxjx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gpypfdpkn.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/grdsyzubh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/geyfmxbet.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gtguyzuvs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/goowcuurv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gsdbwxpfu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/ggnbnwqcf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/ghczxubfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gyzsbxjks.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/ggrxdbqxr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.yfazqb.com/Article/details/gzarzsbyo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/ggvlhxffq.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gitlkhyqv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gsfagkxye.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gglsqxdfm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gjjvdttll.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gssfzibyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gztwswgvn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gcggjdsgz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gfkyuxfwj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gcsxmmomw.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gzuuuzkcs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gewcdozvb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gockurukx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gbjrszvif.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gkbqisuwg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gjpjaxruo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/gxczyebmo.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/ghkiufcyc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gbfdkdjlv.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gzweanvqd.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gkhbfhhzq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gdtlnujqv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gceetlsww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gstabannm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gsdtrutem.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gqwtytlrt.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gpwlyxfmp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gsetpukwe.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/ghgzkwheb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/glnyjplvy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gekleurtm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/grvnusktw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gfammjvut.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/giaeswewh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gicjqyjhu.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gmfawyugz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gmntospgv.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/glbbokjwr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gvddibkmr.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/guhulxrfc.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gnkusodyp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gajioltzz.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gijlxdaia.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gapsulszn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/ggwoxchfs.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/goknllazj.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gamirjrhl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/grstwebzm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gcqxnoimu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/grdzjbjnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gjukdsdvj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gzgugiocu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gzpjwvrqi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gmkuhfieq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gvxydflhq.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gjjznxspm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gufpfalbm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvubqddpg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gedzneqvy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gwdxshvlc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gflmpdljk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/grjfcjymw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gdgnmcmro.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gdgnespqg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gojkfvomw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gvifihfgm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/gxnajcbdr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gwmjwhlhe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gaqsycpsd.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gqknqfmci.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gqvmclgtd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gnrsogkqh.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gmronnkfc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gwueputcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/gvodyvctv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gqsrqoaao.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/ghpxmmbnx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gjicinsit.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gnznsgugy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gacpygmxi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gusjbaioi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gqzmxwuyp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxpfaltic.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gxhbeyksl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghwaegzyf.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gckivbrts.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gtgxweyve.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gxzvvowoh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gwhaxrfsy.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/ghggzzcfk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gveqocuxm.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gsvhjpdye.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gfikcpvut.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gxxagcbfe.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gnwaczbjj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/giaromqkn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gfznakpkx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/geptopgri.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gszbtcobj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/ggwvcidem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gzdykllyz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/gfxthfhnk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gelallbxc.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gihqhvcwp.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gmxugohpp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gkhwylnvm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gnwsgnotu.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gllgakuwt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gjyjftaoq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gbnoczwbm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gxfjarzdk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/goaizylel.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fktsv.cn/Article/details/gmxhtsrtq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/golncbhrq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gztdbiiqc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gebxqnnhe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gswwhotfx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gtrvspmjg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gurkjerbo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gvfzvbmkc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gupberxlv.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/ggswezgdo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gcmcrvniv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gugjfrlrp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gbztwmjab.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gwyeyysaz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gcazrumgd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gxouyouoz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gjkixgwru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtjajrzt.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/grdkhhmkj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gyyrfpmum.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gfxtzujgj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/ggjlfmsge.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gdhcegxll.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gigmvelrq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/ggxglojhk.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gguxbuwhh.sHtML


<!-- 参考信息 -->