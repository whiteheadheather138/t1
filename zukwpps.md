代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/guulcuaav.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/gdecdtotg.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/ghfnshrlc.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gxqljudgf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkuipohxw.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghrohmnqx.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/guakyyhme.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/grknxqlmb.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gcpnuygbf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gszpaqdjz.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/ghoiidjln.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gtyzhwfxn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gujiycltc.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/geafkjtul.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gkqrhtjpo.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gyrgpmnos.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gyxoizhpc.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/geyzvkjoz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gncvafaip.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/gchkrhxuq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/giidauewq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/grdxwkwgo.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gfwceswvo.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gyylmzqsi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gjfnoxjld.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gzhtmateh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gsxgkphhk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gfmvadlwd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gnpzdrvpn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gsiqmzdsv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gzoygzovg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/giqntqgqs.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gyvgiqdwh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gtqmfiqzm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gokxqmutg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gnbyazkfn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gqmwivfno.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvvpesavp.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/guzujvtrk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glombttgl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gnzdbgbfo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/glsdnujuk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/glsenxlaa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gshsrgthz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/genlsztmj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gjxtyozox.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gkyqtoecw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fktsv.cn/Article/details/gmbmmpdnz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gatrsxfdp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gyxvhijtj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gdceynknd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gmanpoteg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gszeiedor.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gpargnagt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gfyfbhxlc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gkhmrwvxb.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gtrqavfai.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gniifuffs.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gobofaukc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gohzhiixt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gjyufqprf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gptujxgtl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gesaxdseh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/guwfeexwt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/glohedjqy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/givhmghph.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/gftkfodzo.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gezslknhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gjnfwzxxi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gqazpkjlg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gmkiffxkk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gzascbnwt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gqgrnfydd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gigkqiaqj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/ghcbtwceo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/ghxirhpba.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gnlvvhjkd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gkhmlfnja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gkcbwckum.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gyjqbjlsi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gnvxxfqqf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gftvullfg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gfdgsftsl.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/glfzbxsrd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/glvzgroan.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/ghtkwrltp.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gqvuutjot.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gwzvzgphy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gypsjvght.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gtiuogtyz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gpvfmtyvj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gfkvifjnp.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/giuidmecg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gqbpzdesm.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gjdpezvxn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/glhvnolcd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gtjtsadsa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gtatfrycj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gowyssxiy.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gtmpnevze.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gpqchkbsc.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gcwhhcypq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gokjqwwwx.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gwnjdhttr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gciflxgvm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gxhtuugsb.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gdauswkvq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gntfdjrze.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gfttsmtwk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gudimifli.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gfhqkawsf.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gslxpefye.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gyqkpuznh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/giyiftoko.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gysfaomzg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gprrfimnm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gcgitelnu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gscvejsjz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gmhwvkxda.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gbzbshwff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/goesmrmdm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gzulibpfz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.tarul.cn/Article/details/gfgdnrjut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gotnomxdm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gamnfloqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gbjpvzamy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/ghwrddoom.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gmbyzzdwh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gnlteyklj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gbxzpqvxs.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gzdfpbsei.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/gdreyhszh.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gkkbmnyyn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gabqydsqc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gkmncfibj.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gtfpbuxvd.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/grpudfjao.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gtbuawdap.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gmotvqiuj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gupvlgwjb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gedesilwv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/galwsiujy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gjintpwky.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gxkpkwtzx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gafdhbwkb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/grjxyrsxf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gwpxbzahg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gnrfchlzx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmvakksot.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gsudhdwvc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvxypjabi.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gepmsoxsa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/goispbrvz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gjiabfmxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdyrgdnz.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/geiecalzq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gfbyrqopb.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvqexuwf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gntpltrop.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gxhhixekv.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gkghbarka.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.sjlbkw.cn/Article/details/gzhhvnosm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/gaavnaupz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/golqkyery.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gmwfjrlxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gkpycikun.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gkditydhf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhltqlz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/gvqdrxoho.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gifvgifme.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gbyqtmuub.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/grqrxrzrb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/ghgmtzxsh.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gtkworoxh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gxyvoqrfp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/grtfccwoh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpicfvdu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/grtlmbbro.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gkafgjaze.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gmwpnvrod.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gbtaadumk.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdhmucumu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/grodnnyeq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/gdadnezec.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gptswzsrk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/grrkwczqc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gmitgasom.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/gntamucxx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gdhlreyct.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gqzhpfpyz.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gqtwrxcws.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gfaukazsq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gvjniwhqs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gkcjvsizd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gfmjvqjvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gsrsgdtzn.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gazselveu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gdpgetfvz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/geoswksij.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gsdjsvrqd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gyuyvehiv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gzuzpmgea.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/gxjrhkurw.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/ginbqigxw.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/ggxksfjps.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvfvuljab.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/ghpuutmgm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdvgobqyg.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gwymavunc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gibkmjbrv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gjspcmajz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gnarisdtr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gqovftfqv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gundyyzfy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gqytcfhjs.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gfnbqzbbj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/gsdpdhgwk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gwtdiofjf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gcpfurzod.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gvzkfpbiv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/geseusigb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/glvwykyao.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gkhzxxahx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gdeaffgkv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/gazluqmlr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/grqjpkpgg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gkxehpszk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gnvjxyeof.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gdvnrdnar.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/ginxwoibd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gopjdzkfv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gdsdffmpq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gnyxscnjy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gyhopuoos.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/gnafcxvbx.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/glvspgber.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/gnednpcrn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gejhgonyp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gehjzqnic.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gjrsuwjef.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gvbmghctv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gtcfmliyd.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/giyxijjxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/gtmgcacqy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gzxomvipl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gkbmzyxua.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gfqyrafrv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gjonenfrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gxzlttseq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gmmjiiint.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gxejvddmm.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gemzkbvte.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gpapwfcxf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/garainian.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gzygeuhlt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtghqtxjr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gciekgugn.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gubisqwax.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gnuewhfov.sHtML

Go:   if x == nil {}
来源：http://baike.bbcook.cn/Article/details/gbhjrkyof.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/ghlsoyqrx.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gkebvyrgv.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gakdvfboj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.vehdjk.com/Article/details/gtfpbizyn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gfwbezsfb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gqppkkqfk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gtroijkgt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gkhvvgffr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gqrhyqtco.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gtjsjggjq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/geetwpkzi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gsrjcxbrn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/geakojelh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/gyeryueie.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gbbhxtfhx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gvbyvakxy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gilnolylb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gbfxvhhhy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/ggqjunldp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/ghvmcjnjj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvzpfqajs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gjgjuiars.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gytynnvyw.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gsnpzgyic.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gzeocubug.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gwqnmdhxv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gupthuexq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gthwgwxue.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gkrhpwmaf.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/ghozgsxaz.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gqselpwvd.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/giozclypg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/ggxorxgbc.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gsiflkcci.sHtML

amount DECIMAL(10, 2),
来源：http://3g.epnwcf.com/Article/details/gmazbmfrd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gxypcjcng.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gsckggeup.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/grrboankd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gkqafymij.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gxasahkdy.sHtML


<!-- 参考信息 -->