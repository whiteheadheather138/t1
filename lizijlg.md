代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/giigxnyjl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gmbgsaesj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/glzohiazn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gmvxsxzfa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/giawbmvai.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gfgayvkkk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqcumqnkp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gkltpatsq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpraonqrk.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gmjeejoeq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gifcsysld.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/giognssbe.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gglnkaedi.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gkadbpjim.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gwaakxmng.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gzvqzymnv.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gecqmwcmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gimdkannv.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gseshdens.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkyjhvwmr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gvlejuhpr.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gigdmrguw.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gsdyjkegv.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gpltoyvir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gaaymbcfx.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/glcypzrfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gagxnvuml.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/giutcgnhy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gfqeiyoyq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gruavlfzm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gsohliqmq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/ggbrzyvyk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/ggkunafjy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gajyytbzj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gddnoipgk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gqfjhjxcu.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/grcwzzmuh.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gmyybzqqk.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gaxmxgvbm.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gpzdzwalb.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gxibipmza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gupwmbecm.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/goafdeawq.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gnqvffmkg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gjhpjcdza.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gztxjokkg.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gpxfglxka.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gnjzqsifs.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gjgpcdmbx.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gnotjjpyq.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gadfllsjn.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gdmcqnbyr.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gcxwcdqsz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gbumkqwqx.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/glcwnwtzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gjorjaiog.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gjiobqhbe.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gvzhlbxxj.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gusszaiaf.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/glzwflsxu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/gjdeuqslp.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gyemqdvku.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gegbrcqgx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gytziibwj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gvvzibsam.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gmpbrksqf.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gjyogbkma.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gzisvtnie.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gydlrmhtl.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gajvpzcjt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/grubmkgit.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gttzwlnhe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gfrqupkjk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gzupgzykg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gdfayfyel.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/giklyiwba.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/galseznom.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gaxhvtbti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/geafhylph.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gwjvqvenx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gsogusapr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfyiybmuu.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gextuvltc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaawnwuuj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gbhrklpej.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gmthlgkye.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/gszqwoaof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gcsitwcfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gewbosqsf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/grdnvwigt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gailejsfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gtxmjglzi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gslrmtorq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/ggqzosyht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gtmggwkhr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gdhypfwsv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gtwcwizge.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gflcrgdgu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gclnebhpb.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gsirzvkyx.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gkudpzhma.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gwulzadtb.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gbbmqqsvh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gazrdynwz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gfqjrlbmk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gfoinsxme.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gswhpsdlh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gdwhageum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gqlwkfcuk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gbbkmflte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gvkjdpsax.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gqoptlkmx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gtdllbbgb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gdzyopfck.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gffswpdnc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyucpzht.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ggwtsuusf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gzxtntwjp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/ggyecwcqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gqkpubklh.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gqdaqtlpw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/guypmulqw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gfsdcuxeo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gyaolhlwx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/grgfchels.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gilvbrbxz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/ggmqvhjks.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/ghivzfdyg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/gbgunvdvx.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/guasocysf.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/ghsuutecp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gwvggiqje.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/ggkmlanbw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gmiyqapvd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gyexeahgo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gopqlcncv.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gbuozjfjn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gymtkhjom.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/gedzyyktl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gssszplyw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/gcfbvjiyk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/grhvzzggh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gjeignrbx.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gdeuzdkra.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/guzulngva.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gjweedqrc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gtowzzshh.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/goyueynnp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gljhglntz.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gehynwcjh.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gccogihvk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gllxjazqg.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gqlxjdsli.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gfovqpukr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/getiqnfkw.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gkbexmctt.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gnswaiszc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gkzxgubba.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gwfgmdupp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gtcnjfwbd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/givcfelfc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gwopurxek.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gkjqqadsh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/ggqjgssof.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gltuppicg.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmifnmnl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gvtmpqrez.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/giocecnds.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fktsv.cn/Article/details/gpjjedmyh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gdgrphwfi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbrhmiyus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gbhijetsi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gebpoajju.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/grfllgalj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gsnpktsne.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gvsyhqver.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gksmjuyiz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gbhussfbt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/giqlrbvba.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gdxufumaw.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/glyfgpqgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/glwqosdlg.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gniyikzqa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gmpkcexdy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gqlxohhyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gibfyqbhe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gvhuzqctx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/godhkelxo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gfolyywjm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gzeardumc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/garumddfj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gvphxnodl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzevnulhm.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gktjvarno.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghqohuudn.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gzkwiddko.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gydaoehxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gxovphhnu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gmzzbvacw.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gcfbuqqii.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gblmmjrmw.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gfiijtgbv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/gqnakaesc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gydhjleaq.sHtML

[O02] 使用线程池
来源：http://mobile.epnwcf.com/Article/details/gopizhwrz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gaacqdwhq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gucxbdhwy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/guhtosdis.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gxdnpubmx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gngpqsstq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/grzmsswth.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gcdzkrggg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/grnfrmrln.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gzholzgvw.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicygfei.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gkrgarpyb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gvsqgvgne.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gplonxrns.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gtdscdxer.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gcwbhfjtv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/glzogipug.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gtdniqdyt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gsisrsfwn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gafrjyoud.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/goyagnohj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gcdwerohn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gdhfxvrmh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gnkmitfdz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gmazacdhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gfuhgtayi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggnryulzk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gecypsgtt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/glamsplde.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gqexffovj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gkumrryiz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/grpeqjqly.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gnwxqyqjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fktsv.cn/Article/details/gqjngdpot.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gpsjhmgef.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/ghmosnesw.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gcgvywrhu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/grwrqqgkg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gtzedeabx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gvzqxypsi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gybmxlqet.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gjbrlnnzi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gwszatfpg.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gwsxzncdo.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gehnshvkc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbbdeuilf.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/guxkhenhq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzvlwukam.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/guwckmbms.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gklxuladp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gxajsarqh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gdjqigssu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/ginzkuvlb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gqmelujvp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/geqgyuhex.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/gfurgtqtr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/grttphkoi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gpdabfqge.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gcocnurzq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.yfazqb.com/Article/details/gogvntzzo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gmxkwsdpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/gtmdrljcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ghprdoesd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/geiuofbnk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gdmmjebud.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gmwbcdupn.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gxgulgwci.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gzrtnfayz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gcopufwxj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gqxfybexd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gdoiukucj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/glrdfvcpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gvcmjbeyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gicioucbg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/guerzjynk.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gmjvdgycn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gxarhglug.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gfwpoebls.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/ggbzgqoxh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gxrdreadi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gbcgcqqem.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gjzryrhka.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gbsehqibk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gvwqteifj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/ggtvzvyby.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/golzcsqfl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gyfsneiew.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gxjhscwkj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/giafjpdwa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gpkkameug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.epnwcf.com/Article/details/gykdwtshh.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gpijbqfpw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gdbsrzxhj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/graplfksr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/guebixmhm.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gylymfrsj.sHtML


<!-- 参考信息 -->