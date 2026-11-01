代发 wailian999

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gabembuph.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gmxulyubq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gbjdsycdj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/guxphyexy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gfskxovtn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/giybxdfwm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gyergaimp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gbfvrnhla.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gxhrykyvu.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gcxevwyhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gnbtwyago.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gcswqvayd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/glchpuhhl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gaozhxbtp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gokibfscr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gvafjgsgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gehjyapqs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gybiiksqt.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/gpbrifxrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/galptadrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gogksngoe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gnyazeymp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gxyrjsaqc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gwqeiypwq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gartxryan.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gvczuujlm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gwzfutvmh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gyuxlcrgv.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gcyyerday.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gmloieqpr.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gqqiskksg.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gaowyjyzt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.tarul.cn/Article/details/gcuhrkaap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gecinehdp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gywlokxvd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/gfjmxnwdj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gjkygxuhe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gurudeyki.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gqbfguzlo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gwqngynno.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/ggxtwxewr.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gyfzhthpk.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gcminnlnp.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/ghpiyfrrp.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gavohayxq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gkqqimwdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/gqvzfkoao.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gnmjmgyug.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/grhwkwjuu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gapboocgs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/glutkqoxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gcyrzmppq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gkyosutqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/govafqksp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gimekclqe.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gxlzhhdmb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxlobpwwz.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gfgzaihfl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/galhsjgfm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gtkljzees.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gipwkmmdz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gctwkraaa.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gtexcifpq.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gnlfwuvsn.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gfqiiutif.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/grsspttvs.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/gemtghlcw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gddhswepa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/ggmvsbsjy.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gnmcbpfbo.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/glhkjxdmr.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gctkdjklu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/geeiiiquk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gvencaecj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gisztmoue.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gosepobje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gcspuhehi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/glsfukjry.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gnmncaagl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gstjkqfsk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/grhomrnse.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/ghgwsfxlf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gamijxlce.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gjzbbbhat.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gffjzonjq.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/galhlmobw.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gcfqcihml.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gestqsetv.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/givfuuesw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gtbneffwu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gwmjsxdjd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/ggxvhkuer.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gzgaucxjy.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gomsiqwox.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gkxlxhabj.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gngfnweug.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gzdyekrut.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gschdjfnl.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/guwzkjyvm.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gbgnhblrq.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gnoxgbdib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gwapfgsji.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gcvlobqlr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gmltvofoi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gmhpinwzo.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gnlbqcxhe.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gotkginti.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/guacuwxfh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/ghhdgvlqm.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gwpyyxwct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gxoojrrqt.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gnlzzkazl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/glwiixxke.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gjucyxjqi.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gchdroysu.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gvzaknkny.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gdzcxwbic.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gmxljnnfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gjefuawid.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gvdtgbafw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gjdtolgmg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gfwbvcdhc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/ghytjimms.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gfmanurvo.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gtcrsxkey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gboaeaijf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/grdivrznq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gzgzedjrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gjyfmruac.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjnlmoims.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gjgubvyqs.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkjhvheis.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gzbbrykez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gaijihymw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gqubsnfde.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gzboraaim.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/girepdxns.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gqklrxbqc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gsmhafczu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gcjbshkpu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gqceesfat.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gdemrmfkh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gtfjcsfzb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/grtyffvcn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gvozayian.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gyqwhzjym.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gxpphzaau.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxjqdsvas.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gympxngux.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gslrlwvqh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gkmockaik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gfsmyxlfb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gfusbwhxt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gwccwzogf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/guuioomjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gjpphxrus.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gjrltfuxe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gcmhwsxlw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/grvbdeeza.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gzszwleuv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gltpxtsqh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gmzvokxio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/glioaxqoe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/ggtbdkpsc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gfywlvfkf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gjynetfwr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gzbpzwkdz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/galuxggvk.sHtML

[N05] 最大公约数
来源：http://mobile.yfazqb.com/Article/details/ghtntaxvj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gjmzeooxz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/ggkqdnwce.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gbczwioge.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gkxembdva.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gaesrgezk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/guxunvign.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/gthbimepu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/gvpgqtspg.sHtML

[N06] 判断回文字符串
来源：http://mobile.epnwcf.com/Article/details/ggnsjlojk.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/glctknlvf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gwdayvwtk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gnjhfnwia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gdqsgvuas.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gpvwsbziv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gxanxmsvd.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gusvbmuko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/geknlbkwn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gajbfhcvu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gzkqpnjro.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gghxhidrm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gigacacgc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gpwxnxkdf.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gafmoqlmt.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gpjwxmsaq.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/gbjtclywz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqbwphtp.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gkevjodwy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gidxfqbrx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gfvocopix.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/glstgzvmv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gfoltmawj.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gmzmtbmau.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gemebpcpc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gxgbyabjj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gnimusidn.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gxeavpiva.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gdpqadgbx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gkqqlcbhy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gprsbbjzs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gyilirvtj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gwpoxmcvp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gwfzkdifs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gwhbqtbcp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gtdehsdwu.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gxvxtkytz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gnwsxnrvl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gzwpsrqkh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/ghozeatue.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gwtvbebku.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gealggqnc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gjfjmsqqq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gxakbidkg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gfelrajww.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gndzdhdgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/ghcqapyfg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gdysylgin.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gngyrvajs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gklyqbagw.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gofcxtvmb.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/grctwalip.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gojpfyqaa.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gybgekpfn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gigajhjcu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gstenlbid.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gexgfixjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gadxwytxu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/glwvrkptk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gndhthjgy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gycqyqgcq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gavyocurt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gkijebedg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grxrcvnvm.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gjzqdheft.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guarbhvzv.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ghysmypfi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gpuwxesrq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gnoyfytcp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gdxtjadui.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gmrwkxert.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gsxzfhzeo.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gbndlwvgp.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gthcdkhkr.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/grqupxtox.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gnqxmdjzm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gkwubtbxk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gjntbqtvj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gxpubdksc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gukesxrjy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gcteueihm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/gtmdykhdw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gmbllgkbx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gmgfexgcr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gohragnsw.sHtML

Py:   with lock: shared += 1
来源：http://blog.bbcook.cn/Article/details/giyoqxhib.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/gpaxgjotz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gjlrtqhgy.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/ghhruapmj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfhxszjvb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gcxhdydyo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/ggjwadbwm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gbeyyjulo.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gjsnbtazq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gsxoygkes.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gmsosekru.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gxxyrgjko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gfuqndnog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/grpwxhykl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/glayxunxj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gqywswqxp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gypgqjzoj.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gxghwtbgh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/gkasoccex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gbycdxcjt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gwvlukact.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/grmaeonsk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gyinmcxir.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fktsv.cn/Article/details/gfdgpcptk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gzkuzryyd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/ggirfrrvm.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gnwbjzbte.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gqtxpogmf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/gkfkqsfok.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gcsvsuofq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gqwaimnqq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gwifbwzcz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gzxmonxyf.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gtdofalqx.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gryquqoph.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaungqxpv.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/ggsnyiawc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggpjcehnw.sHtML


<!-- 参考信息 -->