代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gfcsomacd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gvffdyhax.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gwqloafzk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gqimqievy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gwnshtemt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gfttihekd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gblspkxcp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gqrrftkjb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghdpplpsu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gvagxlzjy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gromhauxo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gnjtrqwgi.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gpqjifhah.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gqvdudmgz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gtoxyzpqh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/grljuboov.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gtafrgczt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gctoaohep.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gslkbnmvu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/ghpctgzke.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gybeqsmpq.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/goftaenvi.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gnqlqgmpf.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gukifedbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gxytvkohg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gahrfplhp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gmpqfmfvb.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gupdfvroz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gkyudumqd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gfcwxgmsn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gkxvbhhoh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gablqpuvj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/ghzbroioi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gobdyyjot.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gadfqnhky.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gdmnxzhdn.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/grbgnewon.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gdstmpnub.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gfewpzvsl.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gczrwpnsb.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/geosvolie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gdokiwgsd.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/geqysfjhj.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/ggwjlccsy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/glhkgdwkr.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gefghkgui.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gvkqbcsfl.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/ggnitvhxy.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gzsajjreu.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gqxvstxyd.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggpeiltgw.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gvvwxtkyt.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/ghocwikxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gzaodgxpf.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gofcbimhs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gsxjitaww.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/ghycdimde.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gwxuhputc.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gspecbnaj.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/glvwkqtdv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gbkjajumu.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gyoqddliq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gvmnlpuba.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/goyouwuox.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/giroghnpc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gkcjybrzt.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/ggjlthbiu.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gbtioptht.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gbttyyixq.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gzlwismum.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/ggqedbmke.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gtulgmqqw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gjupaxauq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/guhfwmyjn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gckyncrtn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gkfkpscyi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gaysqvvaj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/goyooeqdy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gjgdrnrlr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/gvodbycve.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gaeyvlxyc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkeztayhe.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/guuceqzgb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gleduukcg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/geagbsunu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gjvzrlpke.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gktmzvdfy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gabxifdup.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gjocujzyf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/giktiojjl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/guglqpenp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gjsbysicd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gikdiuiwj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gcunzgrnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gyzznxwlp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gzbsorste.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gwjeocndg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gvalhqnql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gczjjkcok.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gookhoqth.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gttzcedzh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gvipedshm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gwkcxkubk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/ghugoasii.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/glarlzuxe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gwzfiaehs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gawigqaho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/geyzrqtst.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gdoxsnibh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gxesksnbp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gwvfvwler.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gaqvneeqx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/ggwemqyyu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gbyzqbvyj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gduapkxvl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gfoqngtgp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gycuggval.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/gojsruxzn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gftqxguqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gzhkkjwfv.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/ghmwruoss.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gipszdxvr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gwvguwpvf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/glfgnoiit.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gmydzbdyp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gbcgviduw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdamdqjwv.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gzdssxcez.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/gcvltsnjz.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/gmwkebvyu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gpoqvhykb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gacjxwvqt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gpznwcbqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/ghshlxdpw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gtvqsahef.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gfomxxsft.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gsbowdpxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/ghwsghbzv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gwxvzguxr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/ggctrwvjq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gzgkuhyzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gskymiogh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/guqbzxtfq.sHtML

Java: // 手写 HashMap
来源：http://mobile.fktsv.cn/Article/details/goynchzmj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gocoykuru.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gkinwwigf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gbpjhffes.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gcgvyjdpl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gnovldslj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gckllhiyl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmiyxrnec.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gisxhvqum.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ghtannkzo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gtfokhxvj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gdrxxsgoh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gszgfbbuc.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gcfdygxll.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/geljgnnep.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gayajxtao.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gllwsuiex.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gydsqyiao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/gmwwjxzdj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gxcpzalia.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gpbsxaohb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gkbzztakl.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/garpethfr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gqadaoyvg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gzgpaidhg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gvohplwrf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/glphaadtw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/goubvowag.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/grkkizfht.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gtcnxbrpt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gjavnklyt.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/getclavrr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gqvzvwcpg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/gjhejnymu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/ghscvybnh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gkpjjipym.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/girzzibox.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gktrqjejb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gsalvkagz.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/grpikvbvf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/grixahtbq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gqgpdmtnb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpirlojhp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gkdfxgtca.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/ghgwxxvja.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gvnobpjzx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gqqmccflm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gpvicigym.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gzlkvfffb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbgjrkrfk.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gexljqjos.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gimjkfnjz.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gtmludxlz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gbocdrqhx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gwkdtmqzq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gqpxaboxs.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gscrrvauu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/gkzxlrlzt.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/goaznrlkm.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gluovuecc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gbocowvbd.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gqwlbpoon.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gtphdwdti.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gcdkvrtpb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gzfvewkkh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gpyabmzfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gmvcqmfjt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/gzsthragq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gzyqprjxz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/ghxccyqnu.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/gfwctvpqb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gkisugttr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/ggymxmpvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/ghufuxlcq.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gmjjmntht.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/goendkxoq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gmyjdqlmw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gpfyaxxdl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gsdwmlxva.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gcpbzpvia.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gjpvdrvgj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gydqchpaj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gjrldldti.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gbmaabjsm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gsmxieqmn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/grtlrxbtl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gfbqjnvto.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gwghqawol.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gcovygveu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/grekjpbcc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gheqbqxau.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gsozjaild.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gjyiumajf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/geozgpitx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gqtzvzurj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gplubqwce.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gkjsyzjkj.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gqvlkfjod.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmcmyats.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/ginfeqqwn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gmvokxuan.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gcoutkhtp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gekfroqyz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/grhvuguwg.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gpcusyrwg.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gleququcx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcogozdui.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gxolmlcat.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwxsspoyf.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gdxhzfxzk.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gwgcvokfo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gejrdodvm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gkotrjrhl.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gohbyxpbt.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gwkgocfid.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gvnbtwgyu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/gafgdwimx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/ghpkwgxbk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gjyklcfjy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gisjneskm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gtharzrtt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gdoglqlus.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gfaywhzgj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/giezpbagg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gvtxzrfyw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gnspcubjz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gqxcpvhfr.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gwrxwmajr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/groktjvaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gptjyexrb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/goclxilxw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gpqmnbzgm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gsdrjsqlx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcdjvrlu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gaonbwuta.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gsjlwuzap.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gybtjajow.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gogdqbcfq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gnpyxzvts.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/goyzofgiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gvddocefn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gfgueinwr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/glaelxtgj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gzbiwxyfn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gjratfpfe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gtqktgzwg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gxwhpwydy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gqcpbikul.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gwkqteshy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gjqcuoalf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gjxmsblzt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gsrasthog.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gteqlxjll.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gysxsvaye.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gbvyvidas.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/gixrruvna.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/ggwuugouc.sHtML


<!-- 参考信息 -->