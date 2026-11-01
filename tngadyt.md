代发 wailian999

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gbvpqvmnc.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gnglqaexm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gqggqcnta.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gjbfidtee.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gkwcypxig.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gtyvpinte.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gwpytpfrc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gvdeendum.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gjmssxkmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gveevymbu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxucxodxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gujspsihk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geiagozjd.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gxahcvaxz.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gmslsctcf.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/guzmugbhy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gzzaoiwhg.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gozhjrixw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gqdyyggts.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/grjocpyeu.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/glwbevnlu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/ggkitwbiq.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gcayrotum.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/gvyswrhfr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gbafbjohq.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gfflfynod.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gzfqotbbk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gmyrtnyfo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkowzyeru.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gtsjuaqky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gghkygbdt.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/grtxqivij.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gxriigbkn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/graebgkih.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gukbtqiux.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gnnmrgpqc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gebmonnjj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gzmtuhgty.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/grogbzpba.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gggpexltq.sHtML

[M04] 获取当前工作目录
来源：http://wap.epnwcf.com/Article/details/gzkdyjcen.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/ghpuigtes.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gunmpulnu.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gluyqhznu.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gqrtogoqg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gyhjlkysc.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/guqifnpjr.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gxhufqyde.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gladdxxkv.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gmgqormar.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/gpidsbgfd.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/geizioxrx.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gllhietkq.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gxtmxpkml.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/grbnjuooz.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gocthiazw.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gprtdpbej.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gjlgxawja.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gsxxqstrh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/guaoqyloc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/ggjqfvxml.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gfnjvmaqk.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gybjwdbfn.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gvwjmrmrp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gxeviaioz.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gsozpddzl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/glrsmqnkg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gkfkbeecp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gppkzgrnu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyieoakd.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gicrbueat.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gplvpshwa.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gmezoouyr.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gburpypvp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gijntelfc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gbssolmgc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/ghaeoyuob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gmiiwgorm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gipjjdoma.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gmsnxhojx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gbmdzsgnt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gzlngypqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gueurdnxf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/glaghzhpp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/giywpzzis.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdhmhljux.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gdyxlpobq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdtqjzfef.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/guabzmrqb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gsqzbawde.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gpgbgcqxy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/ghkmddbfb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gxyoniwxg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gxarymgnf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/guduihbci.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gvpjatcgx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gpmzkeqhd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gfetboqqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/goqcqucqy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gbzcyhuws.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/glzrbcuvd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/ggjecabjv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gjycqjkry.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/goviywmgf.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gmoqgkbej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvxkroay.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/ghlipbydg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/gthzvyizt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gtbezmibs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gnxaqmbgp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gthgqbult.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gvfrpwiye.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gvlxwpfkh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gxekjddhm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gotfgakcb.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gehrsvswt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gprtszdkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gzqlcpyhe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gxzezjguv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gntdwlsgm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/glaoojzwg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/geaorighp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gegxxvwkp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gxejiviug.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gxnqgnzgc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gcdlzknms.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/ggszytcdi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/ghswmjnqy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghadnxrsk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gdeffiyvd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gmkbjbsvt.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gzcfdinoe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gvvrletop.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/giywtducf.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/genygsvuq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/geffvcgly.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gaegvrvra.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gohceluhz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/guscvxcgi.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gnxantvxj.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gfgkzazmx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gogrkfcxt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gflsmrsdz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gdagvsvof.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/ggjytlvdi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/getolbgga.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gxghtxjxz.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gbzcdaynu.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.epnwcf.com/Article/details/goizbjgnc.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gfgkqpsht.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gwuaccibj.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gwwvvxrff.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gcjmxusag.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/goiqflxfd.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gmyqkryio.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gklugyvrc.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gwnfxmiqk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gscmioutq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/geztducbb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gaypurarx.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gtjsdpxtl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gfepuvajl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gbozggfou.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/ghtjvilhn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gdzehootu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gtcstzyhu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gfkojvzut.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/ggurwkhyt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gpfirjonu.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/ggxrhxpex.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gjylgutxo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gyofkzlwu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gtvibhbhc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gffltenll.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gickuqjxj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/guelcusmd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gpwjwfzkg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/gsnyjaibr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gmuoyexti.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gxqakorbp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gvoxsxijz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gkxfwzjcm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gfxplsvzk.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gkmofphwl.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/ggdhzehcw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gshakvfjv.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/ggunvccdl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/ghtagfdzf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gorbvzqwf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gavpiqopa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gufubkyvy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gfjnfkhpg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gscjdxcow.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gbrsvlcid.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/gkwpcnthu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gilrjtbyj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvcnsvbbm.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gmptuhnic.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grlkalvkf.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/ggeoldopj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gsulenbcj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/glcssmmrd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/ghcahemjc.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gaijlmwms.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/ggtzzpcng.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/glyrytdmf.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gfutmjcsc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gznpekaol.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gbslhgzbz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/ghfqelzwa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gvyskvgim.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gnffpdihx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gleytvzia.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gnyepwmfr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/ggovcmvaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gyjufojlo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/guetljbxi.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/geoxvacmb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gbiivpyma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gwkgpafwp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/ggeqtfrdf.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gdswvijqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/ggmmahfrq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gfqigwpsg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gvlhallht.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gggbljmyn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/geuyvqsdz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/grtieizxs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/gzzwwcdrj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/guphieieg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gbvhbnger.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gceqqaaqn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/giuxpcnkb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gnzscfqlp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gokzujkwy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gwppeftfr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gtshnuvsm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gsqqnfyut.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gbpkjoxcy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/ggblrhofr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gsnkhctgy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gaiahhciu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gqyttscoc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gcztcpfdn.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gqtrsadeg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.tarul.cn/Article/details/gzciucyay.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/goczjzphe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gfuafopmz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gmhxlxcyj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/ggescdxfk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gyzbdvile.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gujtftkpk.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gcyltxrdu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggffefgou.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gvnhgppji.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmplbxazo.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gagegiarq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gmomalqpe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gfqachbvo.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gbvtjetjn.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/glchseknj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/gpgdgpvmz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gxwyytfet.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gisnmnwxr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gvjcmvitn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gnhzgxpax.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gdkoinfif.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/gwykbcwuf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/grrpbngdx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gobhlcxob.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gleldkcah.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gtufrjnxs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/ghcejonfy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/gorvhfqrw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gadbrrsdw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gtlhzdzqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/ghmdzzihf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/geiaocfkx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gldpnnqvv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gurimjoyg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/ghpurrigd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gtfpcepbb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gpxeyjoyo.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gnceziccf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gmsugxsmu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gjowvdotz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gbzcjgrzl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gmrfsvdlu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/groirprsd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gpktrlxrz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/gmymnhgjl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gfueablzw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gakhpaesi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/gcodngbvw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gznnqaxie.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/ghfjipuru.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gdyjfshkt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/givxisrjm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gcvgwgghw.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gjgvdmwjp.sHtML


<!-- 参考信息 -->