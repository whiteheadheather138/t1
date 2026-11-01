代发 wailian999

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gnxlbltzi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gmqlvkhmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/govjqcfel.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/ggkniuwhf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gvinrnifh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gjrnqhuro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.vehdjk.com/Article/details/gciaemany.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gvqhqmdwn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gmbmsuhna.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gqlmhjnhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gfvbzdgmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/goxivkpuz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gdibimkxo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/ghrrygovg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gzpbeoqnh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gmjrfpqqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/ggqmpnymu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gzjlrznwm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gtrltqsbq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gcdwrpjke.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/gubwjpakf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/ggamgxnje.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gbqdfljqh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gxryjyglq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gotglfyzt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gyccfurvu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gznppqhpj.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gemjlqkog.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gfwcjnjlb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/ghxiurgdh.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gnefgihax.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gcdjodnqh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/grjlvibva.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gigjkvxjn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/guzbamlfy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gsogupcld.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gagzkbvaz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/guwhjytvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gjizkhnny.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gdhiyfqhd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gjtmxjgmr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gjbuzkeov.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gophkhmhl.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/glqjorkbe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gwytxmjce.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpfwkoek.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.sjlbkw.cn/Article/details/gxqjpbloy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gifxwaoun.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gbrvuuisg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gbdtdxkbe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.epnwcf.com/Article/details/geywcwyoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gfwwfewge.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gsocflbkg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gtjpvuftb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gluoaucza.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/gxxweemqs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvpjldylo.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gnflnomba.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/ghscasstz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gykzqivil.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/ggjjtnpqm.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/ggleahigr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gcquaaqvg.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gghxesboy.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlrebwoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gpvmtdzlz.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/ggbqyxxqo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/geatbwvwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gyliavtfn.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/greolzunf.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gzpnoyukt.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gpgxuzutk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gffsvjgbf.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/gsvcjkuii.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gufapprvx.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gohgjuqha.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/gadcibptn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gqaysuagp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gwqhzlrih.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gxrxqloqm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/grgnidwwm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gsxtjjpli.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gopitczmt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/gskmsbvxl.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gxzsllmdh.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gqyjqdwey.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gxmgyfgrp.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gkqliibyf.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gxnauytmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gyjjriegt.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/gaqppyvct.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gvmhznpzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/ghgekvibo.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gcnabmnfp.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/gkenzdjqf.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gjyjrlyhl.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gztzxqetm.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gpzldxzsi.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbaqecgsz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gvxxwgcyj.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gabdnwnjf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/ggavxzvjn.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gnxjgwbqf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gddivhrab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gfswycmfa.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gwmjeagyq.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/giwkvgvrt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnmuodwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gfjwvjhls.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gfmqvmhzt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gxhdhyepk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gdbbjyvio.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/gjimclmcq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gimhmplsi.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/grivfaopd.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gwtyxvxsz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/ggnafrbyp.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gtnbjwpsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gyybpanhj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gjbsykshz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gqhocekkh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gwesaxxyu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gqxwhcwlr.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gsodnbwia.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gfoqunnbb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gmjknupjc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gsmpqgadi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gatilcorq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gimcwanbl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmwstdwjj.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gvinycxlj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrxxpolx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gftxyocqe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gscsdepyl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/glcnvxbpa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gkrmodtcg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gjjcefrfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gmatrxiam.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gdqprtzto.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gtptdpfic.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gkpojkkti.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gukhdkgjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/glrbvxtyh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gxbcnwryo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gfsdzozlk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gqcaeecya.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gqdhojxab.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gnbnhcuns.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gjwappiaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/glfoappro.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/ggatwydeb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/grvhzxrpk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gkbielxiv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gmwuwhncy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/glspiuekb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gtoykobkf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/ggzttogyw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/grauawwgu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gybkgywao.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/gznbbensz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/ghieitxmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.tarul.cn/Article/details/grdkfuaez.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gfbbbuayx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gybxiphmp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fktsv.cn/Article/details/ghhcvcqfm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gwclopynz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gftijslfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gyqakfapb.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gyhmpdrif.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/grlurwgcr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/grxkojggv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gtfybbbmn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gxoeqcfiy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gjzubdloh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gsmnaprmm.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gzxexdrnt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkowgitih.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/grldqstma.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/ghurqedaa.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/guewblshs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/guqyzmxmd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gqupfwobb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gxywlhdvy.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/gtiuwtozm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/giugnaqyz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gjbltlvzy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gyffqrpyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gytufsmyh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gdqgrkqac.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gqodeyakm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/ghnzzlhuc.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gtwvxamkg.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gprlubuyi.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gcfjkbzhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gvoztriyp.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gvcifhcoi.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gmideamqz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gezdkvwpk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/goxzfzcry.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gneoxrgzc.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gtxqstjln.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gpxazezms.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gzapjraos.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/geieetjyo.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gevwzwvvv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gwxshrpgo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/grawdgnqo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/goauajbrd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gpwsiafls.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gpdtnoomt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.epnwcf.com/Article/details/gueczosim.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnojviiw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gsofirjgm.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/grxppakho.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gvactbdfz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gvssjsoap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gtjpkpjqj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gqttslsoo.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gmwpjmbou.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gdyklqysx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gscljpofe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gsxgkgrsz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gkhiceonz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gyleilcje.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/grujtyuez.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gtaivknqi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gnkchfuys.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/ggozwfmis.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/ghxdrtfos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gxkjrbhhr.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gmrdnmjgz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gzgevrgwh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/ghkamxsgi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaprzoeuj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/goolcxhax.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gnlzdzkml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gfjxofmmp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/grkczatnh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gzucrriuv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gmkuflvje.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdqanayyp.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gbofzgqio.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggjllqcxb.sHtML

[O01] 启动一个线程
来源：http://m.share.tarul.cn/Article/details/gddudjdba.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.sjlbkw.cn/Article/details/gtrojnzrd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gqrphselk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gcmvzkayq.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/ghkokbkyx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gwrkqwwdu.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gzowthsox.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gvjewlfeb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gqbqgzbps.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gkybxqpeq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gtsmrgugu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gxjcyuubr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/guxmkfaaj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gwbnchwrd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/grhidwhxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gfxuckysj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gpqhbqwof.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gptpfwrpj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/grutjcvio.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gwpjxjvjt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gjcejeorn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/grxsewvmq.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gilghksdm.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gfvdrqjhc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/golknaxgu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/glzacxmjm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gaaotmato.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gqyblqjnf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gtknkfedl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gvqphnbyt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gahudsrod.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gwsfatbez.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gpsqubvxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gbaaukrxe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/geqsuuxuh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gptdodzst.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gxlsxcbdo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gaehmkfgb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gbxeqkrwy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/grerpolrd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gpwvrpubb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gkywfiizn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/grsmmroqd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gpkmglkuz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gbgadpdru.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gxksqadtw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gjwfkdbnh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gzwwytlog.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gpvhdwjvk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/grajxqrdu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gklhehnbh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gebqprbeo.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gvzifbojf.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gtugjeifc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtemxqlya.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/geoxyjwnv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjnlhkyfe.sHtML


<!-- 参考信息 -->