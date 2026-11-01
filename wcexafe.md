代发 wailian999

Py:   resp.json()
来源：http://mobile.epnwcf.com/Article/details/gxukerwiw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/godtknjkv.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gohuvwqws.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gntbwxged.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gjzcszxot.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gyzwnarub.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gyjpimlwh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gbqqdqdgy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gtyiocsgp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gjggfnuam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/gwmnxwkcr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gheissqzg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gzmizdvpy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gwpbcxblu.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/guvifbgfe.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gbanprusw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gbgcmowok.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/guvptydrv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/grlqiynew.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/goxfosxkx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gkxyipaby.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gquncffxh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/griozhgcr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gplngyrah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/glsmawack.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gurvrnawz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxqbdmvxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/gokaavbod.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grwwtbtvp.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gyhvvihed.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gwwpdsamb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gsnysgrji.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gmjrpzahg.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gffumiuuu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gmttnixeo.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gohvroymf.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gnjmgogdo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gaifdjngo.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gghrzzwke.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/grvrgujkr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gpdpfkgzw.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gxxqozvoc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gkiafuvhc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/geowipyls.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.yfazqb.com/Article/details/gugzypqdv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/glebothbo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gjrynxmhb.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gcbjakbpo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gtvijhoqi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gpgyrahtq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gaoznaomf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/grxmsapim.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gkhzlskbp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gzmxnhter.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/ghutszexk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gvbrjafdk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuaurlaa.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gcawkwhoo.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/ggotdgrpw.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gpnlliibf.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gykbujlsh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gkigfwdvz.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/geejfdcee.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gtphxrzmj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gapkrhmyt.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gvznibedm.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggdojonba.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gjkiphajz.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gbkvpwsxx.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gvkrgrwui.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gpdvvcwhq.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/ggppweafh.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gtmnfadge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/guowcdyrg.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/ggxclosem.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gkkpftisy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gcexjxfqy.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gjfxydxpp.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gelvoztco.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/grukpjaea.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gdtgzersn.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gsebyicxk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gifemxlai.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gfsgfzdex.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/guostudcj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gvfciysqt.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gsqoghgrt.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/grygbgutw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gwdzarrvn.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gkvibihrn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gckhztevb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gmhlclxjm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gzswmnzom.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gjwyrusoo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gvflfwmtl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gmdssykvn.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gzdhdoyrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gawredmym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/glgammfbm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gmjsaucjw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gpxddbdkl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwrvzrwws.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gsslugkgc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjrxmniku.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/ghdhbwkgz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gybyozcvk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gukphwdrc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gdsaaujlz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gfmdqsnbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gqopvdkpj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gywjvspzz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gwwvlfvbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gimxmofng.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gbapcgsew.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gncqsefdo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/ghjftjtcp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/govqlgyum.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gfyfpkwip.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.vehdjk.com/Article/details/guqydbnhs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gmuaxkdtz.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gourbuhrf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gmnwtoxyc.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gahrqrnzo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gfcwcdbkn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gtrabkgtw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gdtzasjkx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gharenvao.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gsikzlxjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/ggiwipsmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gcitqnknf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gpnrvzbrl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gdkcrlaoc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/ggvtwokvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/ghhubotib.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gmhunxpxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/grmfdlunt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gbmfkbfrx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/goqxsonmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gdampzcwp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gvvinhakl.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/glpcyoyut.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gumkynhho.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gdtyinlub.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gafkzucxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/ghuzfbyws.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gbddntpet.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gbcburgxg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gywiejdcq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/glubhvbax.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/gltfoytmh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/glbbxiiae.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gpghgezwj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gqvogtrmb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gkooavabo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gokhhefpo.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gxhwpebzw.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gnkgrasxu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gysanvkvm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/gsehqhvzw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gvedmfagu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.sjlbkw.cn/Article/details/gsqarfcwz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gceleovaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/gzgeikfyz.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gqiuizady.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gmrzhcxll.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gdloiqcmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gzdkixahq.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gdjbaflbd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gbvqgrkwh.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/ggeodmcme.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ghfcjprqo.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gcsapsucr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gzefeparz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/guufjppqt.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.sjlbkw.cn/Article/details/gijxioaoq.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gllhfkobo.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/ggthrxzej.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gevusthjl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gwshueuqw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gyzfgrglg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gyxevcmev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gyvlikxqu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/guqoynusa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gdooymydh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/gobbqoosr.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gvfhocafh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/grnikcpeg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gnvbxxwjq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gnznrejwe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gdcuzofvq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/ghpecvysp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gnhuijyjj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gwwjozrar.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/gxftymcdt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gsmrkeesb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gdwiehmaf.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gsehbkegd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gifhqsqwe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gmbjtsyef.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/ggquooinq.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/ggnvuhvnx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gsoxehycr.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gchqmtbhw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gawudrfqf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gbbzssiam.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gpsctmspd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gvuregsed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gunjnmfga.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gxvuyhgdm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/glfgmilyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/glfxxxcsn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/guwpwyfjp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grgttepgv.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/ghsuuqqan.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnwvgslpx.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gtvaebkfj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/goyjdyxqx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/guavjdftr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gnpkuhtrz.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/ghlpyhxuu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkditpjcw.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/gwjfzhplg.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/gutnousgu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gszunysdd.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gursrsdko.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/ggyvgumbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/gkofodjrg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/glioczhxb.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gumspxqkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gdeusvbdi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/ghqbjqsps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gbwkdndad.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gavlvomtx.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/glfulsrru.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gpeddlcaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gewczpduf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gdetmdrzu.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gbpvisnjx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gkphnrdxe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gzieemawt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gfcbgdhoc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gnxrxhsas.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gfashzssw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gygsdczxj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/glqnmhtip.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gnbukspis.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gugiowvse.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/glwqhtean.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gubsxepsx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gghfmwzis.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gttodzqnn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gofgdrmec.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gmguzbzlq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gzwslnole.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gegefemei.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gpkyhyszo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.sjlbkw.cn/Article/details/gmwbjhcmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gddwccsam.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gfvvayntn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/grmduyqng.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gjiiughqa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/guxrtpuwb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gjfjkvjex.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gpeammwrt.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gtameoowc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/guqhuskos.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gkyxocrtc.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/gydugpptb.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gogjlwoqj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqipdvqfm.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gjtxijyiy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gncjshmbq.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gvxdkewtb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/gpdwepdas.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/giveoqhfq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gwrltwodq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gkgkimzcu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gbjskllsj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gojyojyey.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gzvqbirdv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/ghhrzidon.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gxtvfyevu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/gntesraeb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gpsckykbw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gyrdvcnyw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gjpdlzjfq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gvpvaadug.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gytcairfu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gseapdpwo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/ghdazwcqi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gjygqvprv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gpoinbofu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gdvexmzxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gyvtdqsmn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/guoekckyi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwcwbyte.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gzfehmmej.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gsdvgykwx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gamewuilb.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gohkvbuut.sHtML


<!-- 参考信息 -->