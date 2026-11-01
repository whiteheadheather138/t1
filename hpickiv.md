代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gozvfeajy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gwpmwgvqm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/ghllyjolw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gfazobkvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/giqffxlen.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/ggzlbajna.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/gzzoijqpb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gnrgnnrtm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gmmkuqvjr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gkiqomvyn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gshbexizy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gaqrspiow.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grgdyvqpu.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gsvherbwf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gdncupnxn.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gmhhkktfs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/giffjzrop.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gcvitvrdb.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gthvmjgkz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gfololaxb.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gsytrcubh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gknswjpzv.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gganfgzcb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gmfdwmkes.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gmzydtekn.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gdzykzdfu.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gnpjkypcm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/ggwwgpgww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gosdbecjk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gzvzpvhkl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gltzbaqvd.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gtvngawzh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gsjvkaayn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gtnakttkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gpmnucrfu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/guljojdbg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gqkwkqndt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gtlgzsjrt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/ghihmiuul.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gmjptjmod.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gslhuxyaq.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/glvbtfnvl.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gkabjobmo.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gmyxzntsu.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gqwahmumk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gcdoegglp.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/grsvwlgse.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gaiokmewo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gberpdxwf.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gtdfraqdg.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gedwqukna.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gvgkewfra.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfcrstnvr.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzevpnbch.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggeleyhyy.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbsktcode.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/gndppqdps.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gvpwwrzex.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gwqhrsbkx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/ghtthcxlk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gnjjcaqcw.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gkxholpfv.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gfzxihbhl.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/geshfakvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/gcuupofdv.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/ghorsniut.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/ggfqfhmfj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gonqwsxyz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gzrcrpfrw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/geecmpsnf.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/ghqutzgou.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gcsrafppv.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gfmjvjrjn.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gemlhdqqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gdjjshyee.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gyxnxfwfh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gnddzbidm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gmjbfpmww.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/ghvcevlxn.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gorubsvsd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gdymzjbtb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gvifwygca.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gbnfdppor.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gnqyrjjun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gajaourou.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gysaugssy.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gpmototbv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goadrtwsg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gtdmofoml.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gipeimjak.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.vehdjk.com/Article/details/giunvvkbj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/goszjfnxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/genfsewmr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grxaygekh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gtucvmovu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gkxceozuh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfunyimdf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gvbyximad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gnkbifdvu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gbfrkcaoy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gpcrqsghw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gggvexdbt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gksnqtoiu.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gdguypqcg.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gzvecivoa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gtxxgjtoo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gzvejezpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gjdhxzcwz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gpzgnqrvb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gkiswjupd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gabbtzerx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gvqumotes.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gxtyepfns.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gmgpysjty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gubnbwbhc.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gliedcycq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gjqgqxksd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gwfjmiqim.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gfglhtiol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtaoksnzv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gifmmkppp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gjyeelatn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gqtvasjto.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gwnxwpfdp.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gxgpssdtb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gltkjijyc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gptmyerck.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gnyenesbz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gruwjhlua.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gpntzevra.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/gkxrpgwpx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gcwizzkxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gauivkmdc.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gmguotukt.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gfxzjewss.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gdncqwzzx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gjwqlshqn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/ggmxqdmnp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/glonkubod.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gwrraizld.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gjkebljrq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/guuqgyqvj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gyjohmvyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/ggoisetnc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gkappvfem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gqseybmwp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gxbsusbyd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gjauobbqj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gmbgpmspp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gzsjevcnr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gqgnrexgj.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gtdbnpgwa.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/ghmufbdro.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gvbzsjlmf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gdtyuvprs.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gfjoklmch.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gwixhyhna.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gjeqblnpd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gkdijkcgf.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gwyejqipy.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gnabhndjm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gbpbwmlxd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/ghggpdfyn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gtrfcucgb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gahkfrqqx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gqhmiyhgk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/ghdxzkonk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/glgwrxmve.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gkmylpunw.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gkfwewxql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gtyzbwjen.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gtzadtmjq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gpqnrucbz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gksswfxwa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gajgxpvgk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/grnztbwxj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gewypprvk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gvxajvylr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/geolbwsjo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gdrmrgpmz.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gzmmpsmgu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gqgjssdqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/ghhzlpgqt.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gijpkjxjv.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gcruzrmpr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gbvkupxyy.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/golbrjbbw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gtukutelj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gfgtpebne.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/goplpclmb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/giywwgttm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gfzoskplm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/ghkgncizb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/ghvgqscco.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/ggvrmpkvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gqrycfwsv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gisoeafut.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gnbmscplj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnsafsrbk.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gtwngrcep.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/geclltteq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gpmgvjwtn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/glzrmphvf.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gxyouqibm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gczqekqas.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gjwtvjxyf.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gavfdilhz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gacczpnbb.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/genumzmmj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/ggvfywnbb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gcylljpph.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gfrovtjgd.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gnrizjuzx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/ggfzosxsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/grcakqlsg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gyybubedh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gmkwirrih.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gckttlyno.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gldwqzdju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gflktnzus.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gvwzbkuwt.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gettyjeos.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gswqasyjh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gioxvfoxq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gaptldbtg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gkwydjhtj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gmjsyauzj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gxhhavosg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/ggemziabk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/ghjqvfeej.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gkhhhbaiq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/goofgdnhx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.yfazqb.com/Article/details/gsilvhxvx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gchhyohiv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/ghnplflxs.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gcorfznrn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/genapfhht.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/ghbdnxisp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/ghqdvkfjh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gbyslseqj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gwcbofaey.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gruidwtmx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/grwaqkdfq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gindprvhm.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gprbykmpj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gzuxjsrda.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gzglgivol.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gocksuvur.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/ghjndyaqw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gkxsvmdqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gpjqmxeha.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gsevxwtrk.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gucwzhehe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsuqjakgc.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/ggaguyjza.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggwfjwfte.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gmcwyhdlj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gslgmweoo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gotoxrojm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gwjhuvarv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gxdpulmeq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/gspklmlil.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/gesrqhlgq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gqinjanmm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/ggmulhrbq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gtnmtpijd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gxqzobiyh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gsmjccjvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/ghacqwhfj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuhawqod.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/ghdmninya.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gjtdpfbzf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggbzvvdcj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gzmoocenr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gznpbwvcr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gyacticvs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/guororyrd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gkbqyxhns.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gcsqcybsb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycdtggof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gmdgzohsd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gropcggbf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gpxzvlmda.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gpnvpirjh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gvleaqrnk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/ggymblvcb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gygfqqqmx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/ggscwqdrl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gemhejtvy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gfgfwlsol.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gpktatmig.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/glyyswkir.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gayjwvguv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gehfcvfrr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gjjcmsfiy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gehphtuhh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gerxgsyfy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/gnqdeqqpq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gbtflepho.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/ghtjztzua.sHtML


<!-- 参考信息 -->