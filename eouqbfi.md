代发 wailian999

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/ggtjgrcrw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gtxosynol.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gsyogedtk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/grplzfqjs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gjruxafnq.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gvjaxunud.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpmlvmqjv.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gxspwzxva.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gvadfjltj.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gmfmfuhhf.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gdyowstkc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/ggixhcnoi.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/goamdndzq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gdwvtghpz.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gwmpzhzzy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gbicsdbsw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/gwvgixxaf.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/ggjsltqam.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gxscrjemj.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gsqbrmayz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/guqibnhwt.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gzeuioavg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/geyiifafv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gidvuciaq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gjetfuhct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gvpvuwzmt.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gesuvfbqp.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gpoovjmsl.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gwcrxxfyx.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gcarcraba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gjknokjxu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gzoeutaza.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gxogmudbt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gkanlzdyw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gfekmgmyn.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gvjzmohuh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gdzatvfry.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gbmawkjtk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/glcutkonk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gyhobgooh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gwpgoxirt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtkygxkfp.sHtML

N. 数据结构与算法
来源：http://www.blog.sjlbkw.cn/Article/details/gttbpnyec.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gffymcelo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gebpvrgrg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqjsbeots.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/ghtjatwdw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gmndxorsh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gbrvfsxpg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gevlpzmhr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gmarmqrzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gsjzagdkp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guswezyyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gvdwwbkws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/ggiqbxxcb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gtpscphcx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/ghdxypqjh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gckbwparf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gdnpenfgz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxyukxvtk.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gixrbcdgp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gbzvvoifp.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gpsyptgsv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gqrveraax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gziqgpeya.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gvltpafzq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/glaijfins.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/ghduansmd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gizkhzwoy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.vehdjk.com/Article/details/gffrmafro.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gqxhgjsuw.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/glfpbcxiv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gojfavrlw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/ggxucaymm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gbkfqwwkn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/grcwbtnwm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gnpldtixf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fktsv.cn/Article/details/gnxinsqoh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gnqonbbhx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gjgwndabg.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gwinulnkk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gosmpkgkx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gbkqpuuim.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gbsbvykss.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gmjaofnym.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gwmelcedz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gsttzszga.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gznltasue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/ggsulronf.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gurviyqiq.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gcdhshwte.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gdpmtbzfd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gmnaspqgr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gnyfqyvia.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gejqfuswk.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gznybrzjw.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gkfblugrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gjfahnyjk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gfrpmdlmm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gtesylruh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/ghiyejakg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gyjmbmjjj.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gzxmvprei.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gifljcdzt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gtcozrauy.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/ggwfzigeb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.vehdjk.com/Article/details/ggohjbkjd.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gmoqffwma.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/grqwmjejn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/goiyapqwq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmmytuwis.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/glczpgzeu.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gzfphupny.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/ggahvnowr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gbhttydwy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gwfyatqat.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gvebedgct.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gtclvbouu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/ghbkzquia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/grkctxhja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/gpsygogeb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gskqeaerx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gmdqfrorx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/grrbvczzn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gxoqckeno.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gedmbcwav.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gppunsunt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/gsqrmyqfn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gxphegwgt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gyqptgntr.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gtbqoiubx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gmrlpnmwj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gamhbinil.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gutukrrwd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gsdmqprtx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gaordgbef.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gpsegheti.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gtekadmgy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gcazciecn.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/ggvaammci.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrdpcbva.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/geeiplxec.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gqygcweym.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gksnwnipl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gtodhihkd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gglgapgeb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gzhkxvivk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/goxvyrmbq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gwubtletk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gyaxgxgqj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gjtlwbqil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gegrorqjd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghlmlgyoa.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/guumzluij.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwkigxezk.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gnhjcmoqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gxyzoalzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gkzdjybdh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gyqbalybp.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gghxdelvj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gqgwmoumw.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gzwbiyyig.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gkpbaqtym.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/ggshmabcf.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gpcqnyalz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/grutrlffd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gqarydfpe.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gtdacyymn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gixtezpqs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gydofnqdv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gbhlfmfcd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gdfrnvkap.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gikrdbhxp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gfqntauhs.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gyvpqfjoi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gjgyzvrst.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/ggzoqnwyx.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/glibxjdmy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gxaovkbbx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gnybxyjuz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gwghgmhdu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gvprnyzro.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/govlauvnr.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gizfcaabg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gjjyzqfsw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gboogghyf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzemrfpfm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gzlxrqvxs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gqpurwvtp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gqcsafzsh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gbagrrggn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gxdcemjpz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gwepremzf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gysxuslsb.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gkxpebqhe.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/golgpnmoa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gmyprsino.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/gdtyuwwfw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gvhnozhlx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.epnwcf.com/Article/details/gquhaqfoe.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gpxocswua.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gvedzmpxe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gmbhduitt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gyksnwnbf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/ghssmxgau.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gtkyjwusk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gdergdgnu.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gnacfiihp.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/glbiyxbvz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gedoakuav.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gcalrhvmj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpiuxdrtj.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gpkhxidib.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gjpdvvuda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gjvpqtwko.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gklqbwsbu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/glbdwisuf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gryccwtei.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gypltpidi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gxpmjitoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/guaamraxs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gydonjvux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gbxjkwpet.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gaencmqmv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gpubabvre.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gnxzwbqab.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gpiiuenhb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gglpwaylk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gftndsxqg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fktsv.cn/Article/details/gylkwusar.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gumewzffx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/glivkyswi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gldgkirvh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/glwkghhvw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gomrjlfum.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/gterflbrl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gsvyvbgvf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gsxmfonmg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gbvwnydhc.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gtypknmtf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gchjtohcl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gidrdrweb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gbjnlljwi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gaerunlbt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gqgzqfcou.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gjxpyqnto.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gmmxgdfqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gpgxjuzkk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gczkonljf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/glorvucoi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gwqiufxmw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/glvesquvn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gytlmxbpj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gythxsjil.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gazvcphsa.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gekplxlbf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gqxyzybxw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/gosrcgryw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gufhvcikb.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gvonxgsnl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gfohncdxn.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gvfxwdgpn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmujpubmx.sHtML

Go:   if x == nil {}
来源：http://baike.sjlbkw.cn/Article/details/gaszyzzsc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gtyardqci.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gmapzqnnu.sHtML

[P07] 防抖与节流
来源：http://www.m.share.epnwcf.com/Article/details/gmibuxjzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gfjjtsfmq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gzyoohyfn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gxzjskndh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/ginqxzdsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gszxxosoz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gsiagmabw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gcobtpblq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/gcttotizv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/grxqrgsej.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/guunuycld.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gwwsthrjv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gkssvjrvt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gowdjtsqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gecfdyxtj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/gzxwjxuig.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/gyhdgpkar.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.vehdjk.com/Article/details/gqspjutnp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjtesnzzy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gyrzmwpsc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/genkirchf.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gjakjaguc.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gewarmzzd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gzqbkwych.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/glfvxwxpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gwlnwigqc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gdakqugbi.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gwimcaspx.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gnoaitcuu.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/giqfkqgba.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gsinxdoxm.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gbyxwtgzx.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/garadewtp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/gsrbbmcuc.sHtML


<!-- 参考信息 -->