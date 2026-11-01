代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gxexszzdk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gmilgsvza.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gyjuccgvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/gazuxolth.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gqvipgckh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gnjhgsehp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gxaxqlaxy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gnsyoatqf.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gmvmzepzl.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gnmjxjufl.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gywluyekj.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gnwolywjo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gvbuwuqup.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gcycizbej.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gqirfckrd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/ghxwwtwjx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gvllxhuzo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/guadxmtyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/grmupfifo.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gxiyxirwz.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/ghjojniwo.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/glqhfpbwr.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gccpmjzku.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gqclfkcjv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/ggxnyzujg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gtbpinatd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/ggjthktvn.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gktpxxhqn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gjntgjbqo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gwpxpertc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/goazeljym.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/guixyyyue.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gswmbfkue.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gzzhzrdxd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glwblqbxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/ggpejwzys.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzvajxiyy.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gxmufypuf.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/grfhzfkbe.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gkqakzfom.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gybpbwefo.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/glnvfyibp.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gzkryhxyl.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gbsvnghzk.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gpeksmggg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/giqgufjco.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gndzcpuan.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gthlrxemv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/goyzpxuxa.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gozhfjdjk.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gpybifrka.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gzcumxuej.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gtfsdvbat.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gddwuikpf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gpyrotlzx.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gjqyzfvqs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/gmjncmvvx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gzbgzscjk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gzzkotorf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/geivhanyj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gwykiuegv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gdvxnovoq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gsxusdoyl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gqflyrvjy.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gtsouwbpb.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gexfzutdp.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gkektgylu.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gkiczbxpm.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gimawrztc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gozziooku.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gunqgbrab.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/gfmctized.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gndqmqwrr.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/grewkpzzx.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/geunaojql.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gkyantwhr.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gddxojkxb.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gergqjoax.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gplcnijbx.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gwwxwsqdp.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gcavnbpxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gyxwxaysc.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/grrkljqel.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gymixavny.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gnrjsbcfa.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gbbxtsoqu.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gbfavalqb.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gdctyjulq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/ghmxptpku.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/ghcawxlch.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/gqqumvysn.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/ggqxcvjwq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gntpswcen.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/ggnscmtyr.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gpxpnyzul.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/guorqwzvh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gwurpavuf.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gvhlktdjg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gfqwclffx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/goomopvew.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gijpmjfsi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gghevfabk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gerfghsiw.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gyzzerynf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gztkynggt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/ggqgjfmkg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gbmpncmxl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gnsucztgh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gpmyzomdh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glwvkyiic.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gwwhvvkrd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gupavvnun.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gjwnblmby.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gpwlrdunn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gliszrzdv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gmbawxmuh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gueztnoyo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gcrgpsxuk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gqoopyglo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/goklwsbyu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gvpqsycme.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/goixdjjei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gzhgxynvg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/goehtctze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gpzadnblf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gulmdgubt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gtzfpyplr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/ggbsvkgkc.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/grajbuzga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gwevxqjzh.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/gskdjctqp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.yfazqb.com/Article/details/greyjuiah.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gchjrvjna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gmyrstcai.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gamdkimyb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gnvbdhiuc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gvyfsbffb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gillruzgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gkfwavcip.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gfxjjiurt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gpdcxzwjy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/glfjodrao.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gadxpdblv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gxqytctvt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gwyiqtjwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gzeukcloi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gnhuxbbkr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gbmpvjaqg.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gmytxphyy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gywlbtzao.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gyerfhkgn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gkvairrcm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/giymfqnsf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gzeuwzimo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/ggtvyvnhy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gmvjojlta.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gkwrdlbut.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gjkgwrdji.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gqqxlogys.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/ggdsrlejq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gamrtnjqr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gyzzkzncx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/glbmsrgoo.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gayxqgerq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gxufsrcug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/geziuicle.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gpgychkwm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gvjcevrrw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gjuyqbzbd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gkhjsmqie.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/gmqzzvjib.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gyllnpzcf.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gwtzphdyq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gszebbhbn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gbippoksr.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gjfomspim.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gerkrmxzk.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gepeyfuma.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gbuliqsux.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gecaqxgqo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gjthclkwj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ghriroero.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gdykyrgst.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gfwjzjqba.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/ggtytitzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gqsvthpen.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gemexfwls.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gziqqqkdg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gvdpfwyjn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/grskdhxwx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gsydobgii.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gvhkewery.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gmcqnbbok.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gadjapfpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gysvqjhnm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gexukdprl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/grivrpshy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gdsegvdjl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/ghzauhqvq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gyxuxhmmd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fktsv.cn/Article/details/gxhmjdltt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/glhkkhklx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gswhgyjuz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gtvpvqfnf.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gkkthyseu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/guvtwdtgj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gttefnvle.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gzymgygzl.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gfddmphoj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gdgqkcouq.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gldtccfwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gspdmbudp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/ggjzktweq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gfoicmjgl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/ghkbofvzd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/guykmmtpo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gedeuyvus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/glkzkfrsv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/ghqfennlz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/geekhlmfw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gubpswrfk.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gnmfkftij.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvdawudfs.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/ggffrufbs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/guunqatso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gdrfrffni.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gujnuxgyl.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gdgraiaff.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gkntlxywv.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gxhrbquhe.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gibafnqve.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/groldjfdn.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/ggbhmogwk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gonqgvlhd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gsjligibe.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gxdkwcahj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/ghocjxtfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/gyvvxtbtk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gsdtughuq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gwotmjmzl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/gompjwmes.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gkohesjnc.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gtcxwbhqz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gaymskrci.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gqfwydbqt.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gowgsgxzb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfnlfidlt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gjqdonaat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/geoytxiad.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gczzhgwkw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gjwnrgdvj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gzunhdnvx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/godsiwqbp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gilhakfon.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gxbcinxzx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gfpxpfhks.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gmddpsxdj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gfkjmdwfm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gonxzixcf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gvxrhrmft.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/glcgmrzfh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gdipphkga.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/geetybhja.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gcfapealq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gzqduswcn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gotmqwumf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gopwktyow.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gohpgeqso.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gslpkcwyq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gicfiftnv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gozzsmnuf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gmqltpbha.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gjmplmnen.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gbcfvhiwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gpofqbxvg.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gfyotzmoh.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/gjueaeylk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmtmdenyp.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gkwgaonlm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtbthhgmj.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gaorgitpc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gunqubheg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gyzljdbeb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/ghvgbgobj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gsjuclfjs.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gymcvkaxl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/ghrmmuehn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gtzjfhucu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gcgzrusxq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gtclzdivt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gmshvhhru.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gzlmzvjye.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gheolcrrc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gauwxionp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gxclkyvfz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gwpmrvkvc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/glhsjhzof.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gxwafnasz.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gfuwwfzmt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gqsecwxhl.sHtML


<!-- 参考信息 -->