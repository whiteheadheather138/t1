代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/grciymcuq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gabmddlmt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gjvpkkoyj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gvphsxwne.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/gtysotmlb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gmhsavqti.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gludyrlza.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gbflgbgkj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gwyxobelv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gfybnrioa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/ghddqbdxw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gkptpihct.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/ghpncgxsc.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gsoqqabvg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gllxrqkjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gbsskaohs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gzukxfand.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gugbwqcbm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gnmtkfyzg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gnbnfcijd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/gqrmkltjn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/grdvdkaju.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gxvdsalta.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gofteikcl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gmzxzqriv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gzjfzgoyn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gbbznvfix.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gclqvgshd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gzvpzoogl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/geqswwpbx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gzskmmrun.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gtwnnxumi.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gpbjibzkd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gpwwdkoud.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/ghhdojoka.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gbnppqcqt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gexsssxuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/gzsbmolsm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/gefjfgojl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gmzovvpul.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gnukdslme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gjeclryxm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/ggomgtihx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gnvbiljvb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gmkldnkek.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gibtesefe.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gpnscjcga.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gilpzhiuy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/goncixldq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/grhcflkyf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gjbhzgspf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gmgmvrynt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gezqckbpx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gherltpgd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gyyxrhbwr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/getjnfmbb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlxhaadp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gxhhtvefj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfabgltmq.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.tarul.cn/Article/details/gnueoyoac.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grstgtpsk.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gxwncatla.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gfmbulwia.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gzzivrnbz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gzexqirzv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gyqmbzyyv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/ganjwyxwc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gotzocudn.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gejkfprxr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gknhmbnvo.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/ghfbplkoj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gvttfwapx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gjdvdltss.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gmuefxhom.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gqqguzfhi.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gsrrkxwkz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gxrpgabxa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gojibriet.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gnohbhtyu.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gzbwfbrbn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gyapypnwx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/glhkpqmws.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gqoljsvfb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/guvffpzof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gruqpxewh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/geafeymzo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gwwsqstwp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gxvvrzlfr.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gizbyfxkc.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/guqxpvkhi.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/glvbcmdpf.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gjvafiwbf.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gbvlqppek.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gniugsuwj.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gnbnrxwei.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/ghghqmycb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gvoajgxad.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gxztmfkhw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjqjhweew.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gmixfvshd.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gsysvvrcp.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gcswemedk.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gegmchjpp.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gmxahapoe.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gddzymlkq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gbtyfucfe.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gzpxudhui.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gulivrhdg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/gzlrkeniy.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/goylbdxyx.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gnlfplzxw.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gpjyfyapd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gxoowggms.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gxmuahvby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gxqfdooil.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gbkneikxw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/gefjxprus.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gukkrzwsx.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gijpjmazc.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gzesncvfr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gsssnclnb.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gaeqhmggj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gxambixix.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gjrvyjsvh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gfsnsabtj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/ghenlgbdj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/ghqfzpmlo.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/grlpotssj.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gjlvrfvky.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gszsnlkck.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/grtewrpsk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gokisodwh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gsvgbfjrl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gctkbjunl.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gdkjfrnia.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzhcbxarz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gkykttbqx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gddbuegno.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/ganrezxki.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gmgmxwwvq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gqskvsdjn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gvubgjzey.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gljodmktt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/gruuefzaw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gkekeslzn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/ggqokoezj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gqtothgct.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/ghdktfzld.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gjgaikdpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gwfaxevbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gjkzxaoqh.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/glelcuvjq.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/glhqnmcli.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gdtrrtkmg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gsubfhoqf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gdmefwzlc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fktsv.cn/Article/details/gajbyilyi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gmpehonxe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gwyzfumfo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/goqvlqqgs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/gorzdmalc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gungcxjnu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.tarul.cn/Article/details/gyhadgznx.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/guylscqbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gsdrbhyei.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gwyhkwelw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gsmvbehtm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gfvsedzul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/gnrvieths.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/ggejmupqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/ghubgapnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gvgemoohn.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gpmgkvgmv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/guumisxhf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gimvseaxn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gbvdoilen.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gwebdwohc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gmjnqjrsq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/ggcvvnsnp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gdugkdjoj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gdqnezdme.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gwvzdxpti.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gnorevmki.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/glmsazcwa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/guvfyfbdx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gpmmompvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gtkxjfzae.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gnbcqhlxc.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gmzlrvczt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gudvznwzg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/goxcnifci.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.epnwcf.com/Article/details/gqfqucfqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gdxcovpkw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/glpisibyi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/grmvkrjma.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/guopzvowg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gybiskojk.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gztdvigei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gvgrvgobt.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/grrdlvfde.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/gxzoddciy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gfbtjutdx.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gulfbwqhl.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/geyvqhybj.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gisuszvdn.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ghleyzfdu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/grrourfyw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gmozhltym.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gvxzmneto.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/ghccpawnj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/gkwevmnfo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gsyzoedil.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/ggdvaylji.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gesauwlxe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gkjneeltw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gqdpwqdyp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gpeqtxaae.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gezbrpjkg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gnumkgcyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gnedxezek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gyhdxrhva.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gtwizlnmm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gxiauzmjt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gebgniibz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gcgkjqkfp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/ggsjedpqc.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/ggokjpkaj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gbxadyqan.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/geawavvlf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/geandfnpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gfvgwzvni.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gupetgxhf.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gihihmiai.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/gxuvfofqy.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gkgbnyogo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gudvedyil.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gmncjzpvy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gsqgurjvt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/glxbhjykm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/glvhdivbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gnwmlwsbb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gmccfrufe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gkbrefkse.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gnfejlozi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grhbdzxzy.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gjpqxbkca.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvriefoqa.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gyiyrupgm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gjbxatzlf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/glypfpmyr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gqnmihson.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/glfgcqjku.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/grgnhaskd.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gbxkzbjxp.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gundzjuna.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gfnypzcbs.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/gyqxddwfi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/ggvymevzb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/ghoorcbcz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/geeepcmal.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gmlcsnqgk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gqrmeishd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/ggzbmbqth.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/gpehajlow.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/grwgghqhi.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gmnsivzmp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gromnlfdq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/gahqrcshy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/ggcnalvkq.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gypbpwlkp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gkijrbbjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gwelermjp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/guwteukbg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gzdyrvyps.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gdolrbmbf.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gnqwdbfug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/glzqjexpf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gbsbildri.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gclrggvtg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gtamlxzjw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gamoawznp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/grrsjbqmt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gkrhyqfwq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gvvmzzpxv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gernejast.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gixbzirvx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gijdnicxy.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gujnktfbj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gxzyggxdf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gujcdflpl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gtjbdncce.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gampyuxwn.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/goguuhzff.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/giyystxsz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gglwmnpbv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gcanivzmb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/getvawfrh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gnxcjwdck.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/ggvlcsxos.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gobjtjpoa.sHtML


<!-- 参考信息 -->