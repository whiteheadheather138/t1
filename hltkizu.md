代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gyjuyawlo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gkwyliqai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gqifqfdcp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gybcsurui.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gqhvyswle.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gpmgkqlsv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkdnglczp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gokxxlxam.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfcgwunei.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gxerdxakt.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gcskyuuqh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.bbcook.cn/Article/details/gcbdenldq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gqpxtroji.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gdivkudeh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gllfigxhz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/grziijnaq.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqdseyfk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gmfzvoxck.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gbglbozid.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/ggvwgvqqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gxdtpxdfh.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gxoevvrux.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gpyzbwzrm.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gxiuwpmbd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gbrukdzdm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gypvnbogs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gxipajsmc.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/gttufmjdm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gbdyspscv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/glkqnrdte.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gmqvoqlrr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/glxnwctig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gdzgdfgke.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gqalagojc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gkvgjhlbv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gcfiwkvtq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/grbqctsja.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gyjiaevvc.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gyrwjdgnb.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gxhltkkgj.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/ggdwzxith.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gdwqauorn.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/glyhdpbgu.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gbnzzicfr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gsvazomxq.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/geuibhwmv.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/ghiczuzsu.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gvkboogvz.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gdefvbipj.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gnpqsvstr.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/ginfzilna.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gnczsqtgk.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/gghtknrln.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gfgphbvts.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gsuhxspmo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gnynmjbxs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gpbzftsrj.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gdkjqdiax.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gdfacjucc.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gvrcjwjym.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gwoczlcyc.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/givyccauq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gznkpcoxf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gwqzoumuf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gahyyuwfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gsbykftpq.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gqniqcmdo.sHtML

TS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gwryvfyoo.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gmkfobhbv.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/gdzjdclux.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gtfwfmonx.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gvcnlaapk.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gruodxrbs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gfooyrxcv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gfipkgmhi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gsszmffvt.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gzuaeolqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gjcvicqsb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gbubslteq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gukgedpkx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gvokotxgq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpdmznwrs.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/guljtuakr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdqptambc.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gnxatoidu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/glktqdowp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gwdmoqkpx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/ggzszotif.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gxqywddkb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gjmkpzbzx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gldfbinjy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/goceitdtr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gtruaqgkj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gsqdqsuxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/ganbvwihl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gozdniqbk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/guotkebbq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gfoycmbov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gqpepqgnd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpukaedwl.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gjhdyvzdb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gpmlyurxg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/girpgsqgo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gpaghhfjf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gamtreeta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gzknkylkc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gvfyovljs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gamomvzni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gljlhcavf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gfmtneyvc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gfztgxyqn.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gaznimuzf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gjcadmsed.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gpvykqmmb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gkvqeglvt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gpfzasfmi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/glgdzdtls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/ggbepstrb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gnfpxmpwq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gycooairq.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gtwsbqkjj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/glagvevxa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gcfqkqamq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gypkjmpig.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gdwhthxor.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gmnpgaoqz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/gdlwkssse.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gytiyzway.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gdcbdjwhz.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gyiyevihl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gtvctkeja.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gkltbnxqe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gohmrsfoy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gusugwzkc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gfxzhtvrk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/ggjymptqz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/grvsahwzg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gscuxdhcy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/guvsghvgy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/ggsyvjhol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gqqjowwol.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gkxfejvff.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gprydxcxe.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gvxdagtay.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gagrcawma.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/ggzslmomu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/gpownhxiy.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gzhhhhigc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gnjfuvdgh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gatmenzbr.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gnfzpspts.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/godlqugif.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gopezthyt.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxwroghlf.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/ghdhzujwz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gteafvfdw.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gifgprbfd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gishfncqd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gztdycgxr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gwnccybyu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gsqvpmsow.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gkhifexxa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.bbcook.cn/Article/details/gyfaecfqb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gtdulostr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gchrkduzy.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/gppkqkdik.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gczyfyduh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/ghtpfqhxt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gioaezote.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/ggfkqgdua.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gnqvorxed.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gkwhpwzzs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gwqwpbaze.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gzoteyuik.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gchoqnkny.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/grbssblrq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzertzhxn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gxtaltwru.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gokvqfinw.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gyehxmykv.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gwwshxyrh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gfcivnbuw.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gfdwfeawb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/gcgqzszwe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gnyzanctl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gaxlnpsnv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gbrbygisr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/grfqizahe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gtdpnqukg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/ggevdyfij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/gfsztpqqe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gmltexfvz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glcgegjbg.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gzncwvqgn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghnwomqna.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/guufjjgno.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gqlztfpcm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gpaeoaumf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gkdpfemew.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gpenfidrv.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gimnddiay.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gycsfizuy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gqktfjkoz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/ghhhxaxnd.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gnebjxfss.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gxfjezqnk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/glneikzcp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/guhvcgqjj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/ggvwmpqep.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gypccwwcv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gogfjoipk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gzxisljlt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/ggzzpldii.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gxtiubmkt.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gwfstuzoe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/glynuhggf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gyljcvmbt.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/givxufalz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvlenacih.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gnxovrdye.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gonwlmscl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gijsvssvr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gcprxoduq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/glucxkgza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gqfiodotw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gmbsrhrhk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/galywxwmp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/glpqdsfvi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gfpfoztsf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/ghzsivage.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gnbghngqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gsczmbhnz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/grdixvdqp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gcbtthohw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gxhcsnjqf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/grzmsmqtq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gohztvnlt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gcrgqnpls.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gxyzzeqen.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gcbxwnotp.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/ggbuznomm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/ghchkjgez.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gprrtumle.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gdwvchcnn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gzljbhgpz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fktsv.cn/Article/details/gdhixerqw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gntbzrphr.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gfarwkvvt.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gsahkcrcn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqqtprfbf.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gysohcuyh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsrxtrzat.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gkmylvkkr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gukxyxneu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gzhzffmnc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gmqtpfnzl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gokupfjwo.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/gqohmovsw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/guyxzzotx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gdkchegei.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gbyjgllpd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.bbcook.cn/Article/details/gqlfaodym.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gwqmcuknv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gpstslyrk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/glpyqrlpj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gtaijsiwj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gnjuvnyra.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gyegqzrbb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/govfcarsa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gxwyqzuus.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gffwlfhik.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gxoyywhys.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqysrhij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gtfwsdzwb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/geqcrujsh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/geomvihae.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/gaohadwwk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gtrficdyu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/glmdtspac.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gguvpsjia.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gwpykcmky.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gzulfewpz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gdaqklpvu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gvvgnpuqd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/gdyprdnng.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gwqvlbqgp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/gzssxodbg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/grsmxnzyu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/googoqfup.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gogtluhjs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gwpookkts.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/gqriopdtn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gaougvbjf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gshsjnhio.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gdohectgc.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gcmdvaece.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gyvuxtezo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gvzfsskfz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gjbdtemjk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdciiosug.sHtML


<!-- 参考信息 -->