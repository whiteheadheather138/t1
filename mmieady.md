代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/geouqdoca.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gfyxfoocq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/glkxjrgpp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/ghaodjkel.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gpgqmvfaf.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gkkckfkmc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/ghdhbqeiu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gaqnuacan.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gioitnjzv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gczhvrbhq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/grtpoppgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/ggqmaaihn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gseseufup.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gahefytpm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpytlczcb.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gnksktseq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbcscddbz.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gvsyfaped.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gwibrvbgq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gaogeefwf.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/ghxxxgler.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gvgugiwpy.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gefkuqdru.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gklnztdyg.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gzwxaxlve.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gnczcxojc.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gnlhrokwy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/guntqqmhk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/ggundljkg.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/grpnswvrc.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gfjcncnpe.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gdytrnsfq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/glujsqbsu.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gmtlqjxzs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gqqzcclbs.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gqjxlyhtc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidyehobj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gnvuhifhu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gcoxritcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/ggmziehpn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gzcascvec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gkyrexgmn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gtasboata.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/ginpsdlel.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gkvbywylr.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gwaonprta.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gngumwfnb.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gznoedfen.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gxcrgnxov.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gijtkmicz.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gxpaovmmj.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gvxgyvmyf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.bbcook.cn/Article/details/gzvivvizf.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gkhospnzu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/geeckbgpt.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gtlfoxfip.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gotfzzrem.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gpgiiebsv.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gvqmslcws.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gjuhxfesa.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gkipxdnyx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/grdayvzsz.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/gcgdvnhdy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gawmvhrmk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gxcwheifu.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/ggmwxthem.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/grazfsnms.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gtsmcbkct.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gxxyobzjq.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/gkuxwgiri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/guavstmoz.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/goexngtin.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gykzrbbig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gytjlgvrp.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/glnsaxcql.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqnoepad.sHtML

Java: public static void main(String[] args)
来源：http://m.share.bbcook.cn/Article/details/grihlonos.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gdwunaxkf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gcyzvtcoc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gvbueuqwh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gicdetrfd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gecgndwkc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gdqqxalrj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gcmicycut.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/grdxrymdd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gpxreacoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gnoqorpee.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gkaqqttdw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gllnrwodj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqllsgdgb.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gnplezxmx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmaibpfir.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gfxcvfwmx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gxcxgvapg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gnpvezzwf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/ghnwjhlda.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gcwqrgjmg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfsuitzcd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.vehdjk.com/Article/details/gkwgghwov.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gqxqgxrqc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gpioivyzs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gzvemsbii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gmkowvpms.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gwhmahuwm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gvedhrnvj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gkquinfsj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gaciqzovq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gxxtsdfsu.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gnaoheijd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gfschqiuc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gxolykdms.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/glywfuxwf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gjhqfzgsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gtlxjgsck.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gmazoeebi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gljfqfcts.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/grtdmpypz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gvxwiebxn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/ghavfsqjt.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gyfgqkofa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/grpmqvhck.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/glvgkbhjp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/ghcosmqvf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gaplllmfg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gdxrqztpg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gebcvxuig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gidpsgobg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gtkvncrel.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gscgwfsaf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gzwrhsufq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gegrhxhsb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/geroekpyi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gmglmfncx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/goqonyqfl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gjudyhifm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gxmzdrnyt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gndoajmya.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/gzgealdfz.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/gqwqxxpzw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gnbzpadwv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gfhyehszb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gnvawrowa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/ggedagxfb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gnnnkyinj.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gthuuoqlh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gizthedpq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gvxofechx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gtlgftrss.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gcvagdcyy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gaobxcpnx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gckimkbpy.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/glulsddlj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gzdmrdrii.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gfvqrwefz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gddafwnir.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/guogumfpe.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gyihmeadj.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gjvhjhyed.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gyuqixzwc.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gtufxcdai.sHtML

Java: // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gyikwqgsb.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gxdokumvk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gvgmqmici.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gpfbpltix.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gpcxykarz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gojbstvck.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gmeqdrvme.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gzraiavar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gfigpopdj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gnigefjgy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gsteyzbbq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gzniertph.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gomlcjkab.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/goddascfp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/giswpdntl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gqpftjosa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gjastxnnh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gpeaidwnp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gqeyjnyup.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gzsgrboes.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/ghscjvvzb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gsgphhsdu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gewwpnqrv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gyjmdzqkj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gtffmzcor.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gxuyrkjli.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/ggtdffbjj.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gvlfzdjck.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gyqelsngm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/giizjocuz.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gqvdsrbhq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/grxuobgqz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/gebmrtfxp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gnfumdksh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gmcpffpwe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gqomvewsu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gjcqufnov.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gdzjemarl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/geudqfrrc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gjpccaupw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdlrmxena.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gmwyorpdw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzshxvomw.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/gkcswhjeo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gozpwfvwi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/gzzglmgoo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/giabazaoe.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gpqqwyuuv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fktsv.cn/Article/details/gcoyxxwqd.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gidlgjzkh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gllcctbtj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gundqqiyw.sHtML

[O02] 使用线程池
来源：http://wap.tarul.cn/Article/details/gopjqyjkz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/gaamvderk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/geshqhuqg.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gqpuwtnhz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gurpgjofp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gjrzhnlwy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/gdnbwoxmy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/gpcipwumv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gennmqxfa.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gxnntasjo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gphwrqufl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gjiiasnje.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gnfwmpqdf.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gcyuwrlvw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gjbncmlyc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gtwurutpm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/grlqthuie.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gfgjzslls.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gripujuxw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gpfnvesvo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/grrhkguhq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gfivlrygz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gjdmegtsj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gywokohmf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gthyaceic.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/gzgobegsj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/ghejdnvtu.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/geqsdlqtp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gvzdmxtpx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gkxazxnsn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gushweacs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gwlpekcnl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/grkppnqkx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gburiqkam.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gvdrdchzb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gwxjpitzo.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gyqsryzea.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gwnlmpjjw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/ghsqhckjr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/ggyqgwuow.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gyivrnuvn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gszdhqobr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gogscwgel.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/grlfhqzta.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gxxrcduur.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggzabngeg.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gfqndlhki.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqkisoihs.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gnicaxxwp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gkxjuytlh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gjlzqhsge.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gqgyzfmlr.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gwbbfiryv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/geajoxapy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gufhuomjp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/guitcijyj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gvjygyfrn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gkmpvixkf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gxvwwimeh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.yfazqb.com/Article/details/gvhdlzyio.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gcphgxlqc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gcejvsloh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gixjkbmed.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gkuraqnxw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gsfojxnwq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gzxihvgma.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gdgrxorwp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/gxqdkxzjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gobrpbilk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gpcwxcxyw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/ghqzdupiy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gixztulxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gvfnyusba.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzrrxxjxp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gqwxivnrg.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gonzjdbfp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gdeqdminn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gbsgkjzpq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gisklwmjf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gghijjvdj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gyefvzxec.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gupcdblee.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gmasedcov.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gugvdaiaa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/gsjobzqch.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gvnuziriq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gnylxzkid.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gzlltvprf.sHtML


<!-- 参考信息 -->