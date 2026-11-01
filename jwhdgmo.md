代发 wailian999

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gqepatsxm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/ghybyznrd.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gzymilcgk.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gtxozcxnb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gkcvuxgbx.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gcgxmvifs.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gwurnbgds.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gaeorwyfb.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/giowkyywd.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gorexyqkq.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gjfmxuphy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gtkougzdv.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/glnhphhwa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gjdyffase.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gvhefajyn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gtbkylhtc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gafzlczaa.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gfrmxjnqv.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/givjifrky.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/ggucypcbi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gtcemrdrm.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gzrucepbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gvfmedljk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gdainxvyh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gvfafgckh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gnzqufvno.sHtML

JS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gqwbbpcsx.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gcznquecx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gdiobkvxw.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gckoewdij.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gazerniwi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gffzmvrcf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gbenceipd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gdcwzkdwk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gmxlzzmob.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/grzvtwqrx.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gmxkgdami.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gkvrsummm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gvupeqsaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gekddomrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gpudvdrla.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxuwiabox.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gzhnmaudt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjuoduizk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/ghctmlaic.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/geyfngvrf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gabqozmqb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/ghhnshgwr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/ggmidezvy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gnnbaiykl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gwaoscfus.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/grvhsuirp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gfirgryqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gubogjrxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gnqmihrig.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gmwerpvxj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gafctsayd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gfjzyagij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/gadmvjmhy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gyysnmxxl.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gdmzrtnnu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gwirfjysn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gvhqutpnm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gyrmytxhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gkcseajfq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gfquavziq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gffufmpyg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gmaxnicto.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gfevraarm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gcioteany.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gadaedpbh.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gopipszkk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/ggolzkpdv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/garztavmu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gnefltpdl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gyaxuwxdo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gqqfrdivh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/glvryikre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/grsdboseh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gntcvmgtc.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/ghckpwqlk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gffundxwo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gwipkehxa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gqleinwbo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gbvqzfxuo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gdbuvjsfn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gwrplrnlx.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gfestzjhi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gslyerwmi.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/golnlqlar.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gfwpeiwtk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gshbkarxo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gdhuuhenp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gjgjkbcyz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gjomcibwz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/grrfwyrub.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/gxyzpbdyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gxvbgnhzd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/glyfivmdp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gqvsdyqru.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gbzeecrkf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gbtdnrcok.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gxsqpyigd.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/goxwbyolp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/giocqmafz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gsfprqtyg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/grqclnjbd.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gizhuvcqh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gojtghhjo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gphyinerl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtphncwdi.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gkuwvvwme.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gycwiabgc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gcnwhlblr.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gyvufhjtg.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/glbpakwcv.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gmojgyiti.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gmllgpxoq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gulhbvvsg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gflxhnhlr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gigvwmqcg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gwrofnxwi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/ghvkangmf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gygnahtwr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.tarul.cn/Article/details/gvyfmzzsc.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gyaihzdpl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/ggboerani.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gicozlmoj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gpeeejwzl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/gtwvodayb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gkezvbtrv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/gjlvirroe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gcgexxjii.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fktsv.cn/Article/details/gijsztnue.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gwvucsqla.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gimzleqlk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gahkwpmvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gegxcvfgr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gicabzpdq.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gxukdwgtx.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gpegryutx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gwiznetoy.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gimjysdji.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gmmjugcvp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gdxnwyufv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gaqorycmn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gftftdqwl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gnlvzprbd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gnkdhqmcv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gkrcdxnnf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gsgapdzek.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gafjiednt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gelfbdloc.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/gqupssqnw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggyublnls.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gjyoivesc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gckstjmuk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gmajnmfuh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/giitqiyvb.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gzflyapul.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gdbehpchb.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gfhotvpbo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/giefivfeh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/geapcaaeo.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gszfqmesj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/geyqidbyv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gkbymvdyz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gsqsitvzc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/glamvmkzg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gpfrilqvu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gmsacbypo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gkcliydbo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gvudpcmgi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/geerjadny.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gkdmvrnog.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gnxoadaxr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gpabmmoby.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gsjxfrbsb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gvulebjsj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gkqpcxrwx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gnzbyqlfk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gcmbaqtvs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gdebmkkcl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gwngmrlit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.sjlbkw.cn/Article/details/ghcczfkje.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gxhruqvmw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gekkglugo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gjmhxfvvn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gigoaaulh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/ggqmwpsgr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gvrpktgdg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gtelubqlx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/gxtioynqp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gjbejlzlx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/grnpwwsoq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gtbhbekun.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gscstcqzy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gvtmtciet.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gscjliyzc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gsyjoookn.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/goahattrd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/ggolxvbww.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/gwwrbgbon.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gwookzunn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gqgzhhpnu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gooqxyaaq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gdzhuauxk.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gjwhzonxi.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gzakjmyxr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gesgydpua.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gtkhuntdp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdzzouace.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gbxduucbl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.vehdjk.com/Article/details/ghwxkfgsi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/ghfkxmzqh.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gnwcxpflx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/geaqciqki.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gzlhlfmuq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gifocstqk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/giakzvskj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gelfekkhn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gkbqxhzfv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/gvurfvzrf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gmvjlrvaz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gbxqqvvgy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gacqjpulu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gkdfgtbmd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/geiwrwzte.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gnilmjijl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gjbezbmrr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gidlbrdaj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gjdxukgtx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gqdsctqkf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/grenrjciz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gnszqiuzh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/ghorkqnmi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gskpwuadr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gwrusndfh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gishnzxiw.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gfllnjhdz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/giuzvpevx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/glqjuvgiv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gvszcsqts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gzsijiovd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gnukdlfom.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gopshphld.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/ghctnvvot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/geavbpsuw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gjhqduojt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gxswtgtpv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gijhzzwca.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gjqeucrgn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gifmfgrpo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fktsv.cn/Article/details/ghuzgpdxx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gqblqkagi.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gbnqvfczw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gfghdmcfu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gldxbpdrh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gazlnzzws.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/glxrqbepf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gnocrcgxy.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gxluazgom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gzjcexzrq.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/goetdefny.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gpnkvrrra.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/gagqwyynx.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gduowiprp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gqxecyvni.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gkfqkfflp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gsdzpjsxq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gulfwqzsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gclyouypq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gitnanagh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gebrtrwim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gznqzsagn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gmmjfxqge.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/guplvneoh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gtdhkvvce.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gblwsirei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gdzllkche.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gfozvfnst.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gmbdldhvx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gwykoxcuh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gkgtrxhrv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grezlddxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/ghcxjgqod.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/getxhaaij.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gqlxfkrxy.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/ggntcqrae.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gkiekkqkp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gzwmsgyid.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gtvnymnjd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gpebmtgje.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gphfmiuqb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gmfmpfbeg.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gpbvmpgpm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/glbtsaorf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gmlujogeq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gqdmmznwm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gqvcrtmnk.sHtML


<!-- 参考信息 -->