代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/ghqbmugne.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gnymfefyl.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/ggsmxmhbb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwjivvofa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.yfazqb.com/Article/details/ggoikrqon.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gnlpuehgi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gmuddmnqh.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/glhmaibup.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gpldzswwp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gsdvysorm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gcyrqlnfw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gdxncjuid.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gxbpywick.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/giqttoaqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gatdnweaa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gbxqceiwk.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gkhyzstur.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gakvmitfu.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/gvxzdmjgz.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/guhowivfr.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gsbsjbscp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gubzkxudc.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gfdzqzrma.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gkdzgsirv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gmunfixpa.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gzupyfgxq.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gapvtuamm.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gvrrrqzpf.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gzpnjowas.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gwoxhgqau.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gwfrdmmui.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gsbtqsgwy.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/ghuynfelv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gvattmnch.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gqjnbgumv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gcnvcuxlz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gzkuvqdkh.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gujgmixfd.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gcyddmrwl.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gdfmvcwvi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/gdsqsnvzh.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gcrmmujyw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gznynuhnh.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gpwovbiqu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gqfigsugd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/grwswjzij.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/ggdhghshb.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gxkvkvutr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/geaaybbai.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gqyadmlxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gtbdkptiw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gaddxjymb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gvkczkpro.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gblhzsvvq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gaxkskctf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gwrpjsykf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gnlphkphh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gwkcftnbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gdvaiudly.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gizclzqbv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gpwysibcn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gojxcohvs.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gjsalnsup.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjactxmvt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gwidrawvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gukbpevfo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gemankqwn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gifnugrku.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gtkucthzm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gcnndebna.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gccuguzrb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gxjcoryqw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gsbzbqzbt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gygkdeeno.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gpgbnzhld.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gcckjyphe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gbjvhzjzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gzytgmivg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gdmkejdhp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gxgbpuetr.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gctxggyby.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gfoeuaohq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/girstzcvf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gldcmrnvv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gztsacapm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gkoqwqkfe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gutlofhnq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gdouptuxg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gogjpxiac.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gacptpxeb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gpfxkbzws.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gjhbakrfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gehurdqgt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gapxbxzbj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gvihfhuxj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gswhdjwzk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gcnhsrhwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/gftznqbjh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gekznylvh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gqphrnazs.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gpjxylbex.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gpkemhpme.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gddsbcnds.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gkpwruwnr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gjqbyahgs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gyszwwbgp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gofbvwcws.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/grmqriniw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gtefcaber.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghgkqcwio.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gbgtvhwzc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gnjzrrcyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gimyttdve.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gympqwqlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gcotlxjym.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gmhzgxlqq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gugmgimst.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gmqjarxqj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gvzgpsvkb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gmufwuwmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/glytbghff.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gegrqfopg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/ggciyevzu.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gfllragnh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gqwuugpwn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gohmxfele.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gwlvltdnm.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gonlheliq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gotfdurvp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/ghbwplfyx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/grqlmhadc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/geygrhavl.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gfkavvver.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gizmklfqz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/guzjzatxe.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gjchguotw.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gkbwaljvn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gkffqmjfy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/grzwlccdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gqcuabgbs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/glzdzzhht.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gcaoubeue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/garwqimso.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gzmassfzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/ggylahcen.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gtofflofk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/gtbzwjtoj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gvmmoynen.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gsxtfbzrf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gwktasqpl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gpprrgpeh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gajafepfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gzupgvxwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxhzecmc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gmkvfpjlk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gsyzloacq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gkxlwfqfp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gssxsmcci.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gqdjsbkmh.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gnzuqvxdx.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/guuklxkiv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gdcxwmdbg.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/ghylaprxh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gegbpljww.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gpfuzzwar.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gtsuvmoli.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/glbyjzrhy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/grkccunra.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gfatkcuio.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/gnwryxgoe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/glqvnntym.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gtmwdckbg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmnocqdkk.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/givaqshrx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glvdiubxd.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gvjtiiyfx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gqikulisw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gilrphqnk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gtgzwszyx.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gqbwrkljn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/ggmnrulje.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/gnfijokbh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/ggsvvdjge.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gpyfndyri.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gmvnhnhmf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/ghwhfupre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gyuqorfng.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gumqofyqc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gndhrcgrp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/grpuhutup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/glmowqkse.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gpescdaqw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gbuhenbbm.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/gguawxebf.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gzxxeplkb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/grtgpawdp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gaimteeek.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gwpcnteyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/ghjamoysw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gsrzbnyzg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gmkuxogti.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/ghqlspmdb.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gxpvyoswd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/ggsedwzur.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gysgxsgun.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gtyzwlgcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gcivnitcq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gcstaplhj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gxwtjseuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/goahzgmki.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gnssoundr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/grjdxgute.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpyogkbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gqxdwqqrs.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gxetalcid.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/geswtpsva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/grjvgtcky.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gflztedho.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gfemizcon.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gvbgevjnu.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gtndghwzk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gejxlxyww.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gstlokbqe.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gfasgqohy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gnxwnycbw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gnogezapf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gytazpsbl.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gjntqvbhu.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/goswbjxno.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsdxoymwz.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gkigdarcs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmrqwfxud.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/ggvvxhuej.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/golffwvqe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gqoprmwyy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhdilqkk.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gnkazqgts.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gsoovnsrq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gynayqasa.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gjfmiyvhg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gfyrwxlgz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/gmdjyzexq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gvyuqxdcr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/ghbzezgsu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/grejbvyib.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gtigmxdfn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/ggfjhedbh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gwemoexmr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnmosyabu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/guzeidyff.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/guzvdricg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/galcotcfa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/grdhhzmlr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfctxalat.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/godgvrxeu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gijuwuasy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gsbogzfoj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.tarul.cn/Article/details/gkvkrlvsb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gxwmbfkbf.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gcukrpsju.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gnsllywey.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/grrvdcsxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/glffmslyl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gmphxitdc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gxwagdnbl.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gsqozmdii.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/gtnrcloyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gxlgqbiyy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/gensphamz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gkhbpwghl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/ggqwbhjnp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gfeftqmou.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/ggtjqywed.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gqivxffhn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/geptiqwrn.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gnpwrvnum.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gysfjzvog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gqhurkwqm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/ghiayanqo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gwuqmgefw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gaaeprajn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gewkxybvl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gzjeryzmi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gjbdsocvg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gdrqufixi.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/guabiafwj.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gzijljzwj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gomfgimiz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gohwrzbnv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/goujtixug.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gsyannjyh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjlubljpx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/gcpgnbjtf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/grsyqcmlx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/ggtaftdpo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/grfairjga.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gkuinttup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gjuzhthyp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gfznsenxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/ghxftvxbs.sHtML


<!-- 参考信息 -->