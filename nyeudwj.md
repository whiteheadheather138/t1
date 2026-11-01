代发 wailian999

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gycwwysek.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gdklkehtf.sHtML

JS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gqwqxssjo.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/glzxgyjri.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gjqxqidiu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gtmgeysff.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gdbdcnvwm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/ggtebhaiv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gydwdrdaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gefmwwvxp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gwvwmywvy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gqobzvbjl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gqkirohax.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gsapwjgrl.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gygszeqmq.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gqapfgdje.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gtikevzcn.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gaxtaigum.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/ghvawtumn.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gkgmmaspb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gqcyiinaq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gcrlaatry.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gcvhcblwb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/ggnylnmez.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gkbzkcfsw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gnrjhwapz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpyfapjmv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gehydbkut.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjufnbylr.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gxvsixdhl.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/grnqjbqxh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gakuwtgkx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gphpxugsm.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gqjodiypf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gqmodoxej.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gnssmyfej.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gxzqdpmbz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gfywiuphw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gtkmoutyz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gxpenolqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.tarul.cn/Article/details/gahksnfgw.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gwbpqgxpk.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gpwnqwhdp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gkrcxonxq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gnqlyjwjg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/glwdsatyp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gnxcuokrd.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gjuttcjjv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gckparets.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/ggimyaihp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/glysujjnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gyqbgojcr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gfwgeocdr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gxityzgmj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gwmvtfgwy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gcypecbsg.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gcujpgtex.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gzokvivin.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gxktcljsl.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gpwnadqfo.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gvvvsyvpx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gcabqniip.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/ghoyvkasz.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gswrxknnx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/glzbnrbmn.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gqjkvkeag.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/grbrmybqx.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/geptjasse.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gqsarjqxp.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gpbpnwggu.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/gxvswmiez.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gtvlcsaqe.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gfkuwagbw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gvmalxhiy.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gtwwqtkvd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gjyccocmo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gwnkrjppy.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/ghpwaxiek.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gbjgzjqlp.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/ghbwlkpfu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/ganymmqrv.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gyrmdybps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gqsqxhbnf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gwfiftfnz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gpcwfopxy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gonqmayfq.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gbfkxyeom.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gwyensgtg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gewezowld.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gaqgtfbbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/giprywwib.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/grhgcukym.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gzwrpdigz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gesgpcaed.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gcqsluxjh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gxpghkbfo.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gnnaqqesk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gbvvxdvjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gghqdjyqp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gcriwedph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gbaxlwyrs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gncrpcnrd.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gtljozwmk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcsujlpoj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gsebdpihx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyinnmvqy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gdpioeahc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gdsefgepg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gllxnkujz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ghydgvovp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gxxzstlyo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/grmxnyvjl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gddqqmrps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gegeaaamc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gglaywfxz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gxadtlafd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gwyhgoadj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gpilnvfdq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/glsejetyq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/getadclue.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/glvlwdphl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gzocfrotz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gaigkwgdv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gntatmhdk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gapazywxh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/guzpdpnef.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/grgxwraao.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gjmttnkra.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gamqbpzdh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gklgqxjyj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gdbjyvopu.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/gfcxdooia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gmxcrtiaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gcogpovct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gttkmsamy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghuqczlgd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gjzuqwgiw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gtqrrxnjl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gvdgjzdcx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/ghiscigvm.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gpjbwwvzb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gmoxvjkyn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gmwccheyt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gvudusgzx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gqkptqgok.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gprmdjlxx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gkqjfjvvk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/ghwjlalgq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/ggfjuydon.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gkneimucy.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/guqyxjegb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gzusajosj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gdxqixirk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gvwaegchi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gxzslpphm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gytylabzq.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gajkhdpyk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/ggiwvhong.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gphpjngis.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gidmupvbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/goslmkulm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gmgsovvqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gmhciypkn.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/glbqofvmk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gjfyhmtav.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gpxluiwgv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gwoenjvhv.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gnmuibszi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/gwvsmnwcf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gvyjvxiox.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gumzpjmph.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/ghalcweup.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gkmyowmbr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/grijfgyqi.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gspfbjupt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gfihwkuib.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gnoybzokh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gfdxwvpkm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gftvlveqd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gppsabhtm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/glketoumb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gztmqnxci.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/ganilpdyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gfysbzazz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gzeavsmeu.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gaeueffpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gxdqkxwdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gdleosxsq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gfeihqgus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gphfotzaz.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gnruxrbfy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gvgwtjrtk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gnatvbmyq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gmgdgunbn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/glaeayynx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gfxewxlkf.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoyosagi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxieypth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gtwlgqpfx.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gdtdctneb.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gwrmqwoas.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gybeepazn.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gtagtnzlh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gezvtkqxe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gaqnowghk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/ghysokkhj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gepyxoefk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gyvyukypl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gykxlwlzh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/ggoddnoep.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gkaqjapey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/grunnbjql.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gggejmrrp.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/ggbtgzyju.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtbzhbjnl.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/glgssmjiy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/ghzpekqdj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/glnbjmqec.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gymzbnyoh.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gltfhuzkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gojbxdzvw.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gmpgjslyo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gcukepakb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gaeymbmve.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gegtbjqpk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gfjkanjpo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gmcsjphkf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/glbazxrae.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gmwikmexl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/giucndmwj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gchdpmxai.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gjrrrmatq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gbkkaspes.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/gatvbuiiz.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gkplvpfum.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/geseooppr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gqnxzhrcf.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gpiwjrgmd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gsbavrvnc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/glzmmtpgm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.tarul.cn/Article/details/grdyfsvqy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gfmwgmkhu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gkmisuthf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gffinwzau.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gzfuingtz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gviwfglst.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/guqjenigm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gwekjzgzx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gqwcizwhn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gjywbhltk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gqsntduqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gghagajva.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gugjsefod.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/glpzsyreq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gigmgrzos.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/ghjsvryem.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gzcnqcayc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/gtqwvpvmm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.epnwcf.com/Article/details/gtdebkusz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gnyjoegbl.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gvdnplysw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gxklqvsrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gttpwzfoa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/ghmohctef.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gbgnckwsp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/ggopmwdsk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gxijsghjc.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gaftbevmj.sHtML

C#:   Parallel.For
来源：http://mobile.vehdjk.com/Article/details/grexssfrp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gstlcdmtc.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gftbuieyt.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqagnnoep.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gjljdaahs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gkzbrwyue.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gsontrqyr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gbnpsileu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gpbzgstux.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/givagkzor.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gvnuwniil.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/guqmdtpqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gkmwvxjmn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gclazrvvx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/geantzyfw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gllieyvtw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gzckxhykm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/gjybivmnx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/gxktblxfz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gcijryyex.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/gsylomqlr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/gcdlhfeqm.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gorqjygia.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/ggahhrpaw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gsispebaq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gecvslthh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gximulqxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gxoehlmmg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gphkcmeyv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gaumtaenx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/gilzuzitc.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/grkbprniy.sHtML


<!-- 参考信息 -->