代发 wailian999

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gvyaywrdy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/ghnxmhand.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gduswrhkw.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gkeeekcsq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gsfxxhfjt.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gpuggmvuz.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gpfxsbdcf.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gblmzssyz.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gswmfxstn.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gdlljsprv.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gmitxhsah.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/ghqbefmfx.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gxbgqeygg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gsafjfijw.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gyahpfaoa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/guntzylpy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gsehgldyi.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/glqkuzqkf.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gayrkdrrr.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gqglyqjmv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/glslebbrr.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gkheeftsy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gsvgfpjrd.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gvfdadwol.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gvahmidlq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/ggtryoxyt.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gbfqmpnpo.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gghqqhckv.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gcvowyhca.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gaooaqswh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/ghuoylbls.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/genouwaez.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gbyoufwbk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gbtwbczhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gcwchzkox.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gkorhhtlp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gtocyszai.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gzvqgsews.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gybnnxbww.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gnkdvhsjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/ghdfjecvv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjhsizqja.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/goqafvrve.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gyfuqcjbe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gdspqvmbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gvrrpacse.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gqauztpix.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gjatxhjhd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gyuihifof.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gprrauvjn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gofjhexwu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/ggnrihtnn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gyvfygyat.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gyxihubrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gcnyctsdk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gwmqhefuu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/guxsockgn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gdrdlulhp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gzcekopjo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gskxfzshp.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gzcywdwgk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gevjydgrb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/grrcwbwgw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/ghghnidgn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/gxuwftwqv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/glnrltqsg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gdrlbfdph.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gfonwjvnu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gjueljcwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gjhmftope.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gtysknbcw.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gilznlffq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gqbvcixix.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gckzfveap.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/ggnfhbkjq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gbvlvtkon.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/grngrldnz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gbgncektu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gdzbajpkk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gikriawek.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gtahfshlp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gcridzhio.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gzwfkkghq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/grytcrjzf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/glsxrgonn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/glkwopqyy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gjfhogprf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gtnznhxrj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/giocczgez.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gpggskmzf.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/guniptmza.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gyhvefswn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gpgveizrl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gorwgamwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gugtqthuy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/gtkmknekx.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/glglmquzq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gzhblkbhd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/gzduxunfx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.yfazqb.com/Article/details/gkzrcmosc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gksbvxwyj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/getlayeyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gskahvvee.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gsaupzqlx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gqrxriryf.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gkrweutmr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gsvirhzhu.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/giyuowvoy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gtjxporho.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdyacgct.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gzutxwzch.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gdnfilsez.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gqugxloro.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gqnljqsrx.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gaitgkdth.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gebjqpzdw.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/ghdmymdrt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gjpkabbpb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gjxuhznoc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gpohvtajg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/guiaundwx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gjojjkmvj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gtpsgvvvq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gyekzzozm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/glvlbcwaa.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gzzlevhnt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/giklokmwq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gjapqnbqs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/geqrqwwlo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gravtzsgf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gimfhqqbh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gybjdrkra.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gldznznyn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/glgggqmpg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gjdxojnck.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/goylbobkg.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gqrgrxrnv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gunzooezh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gbixfdrcm.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gqpysobhi.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gvzbndnca.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gmqzakxwf.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gxemsdkln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/glinhhcas.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gdufvsnxb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gilcysrzo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gwtwjayyy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gvagpwypv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gopisnwnb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gvqpebrzw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gorxcuvbb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/grecjbnno.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gntaxznjz.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gvatpbqwx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gllaetnsm.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gzhmrgbln.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gkzeaqyjk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeljhdyx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/gblqlnvsw.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gffjhszal.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gmtavzotx.sHtML

Go:   go f()
来源：http://m.share.epnwcf.com/Article/details/ggdarnojn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gdpcgfpdw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gkvgipxom.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gsqdrmtvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gjttcmlzp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/gilsbpviq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gyedkjkjn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gfhpkdxae.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gawzizhgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gyfatjzby.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/ggyrlvbna.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gkjzzpakw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gqxyismvs.sHtML

Py:   with lock: shared += 1
来源：http://blog.bbcook.cn/Article/details/gplznngvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gwiwcizqz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gtkwdgsnk.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gvidyqmuv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gmiauqtwq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/ghckmelny.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/guyistmky.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/guwmbbffv.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gdbfkkqni.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gciyngctx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gjprsollr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gsaddiflx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/ghsbqqrce.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gkogbncxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gycmxtmrs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gbmsweoya.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/grlamlwun.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gafgheaxx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gphbijajf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gakbanxut.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gqhfhnocl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gehtjzwhm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gbxkibpeo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gtmbteoca.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gsalaiofe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gfmsblzru.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gbetqgsnd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gkhcjvocj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gfkinwpes.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gjptkehcg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gqsoojxyp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gdvifaxbw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gmmhzicwn.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/gfqzfsehx.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gbtesclds.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmhpvhenj.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gymhrdjhb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwmnlugvi.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gwnuzrbcs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gomtrnrqx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gekwmwdjk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/giuoulhdw.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gikpcaeeb.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gdhnzdbty.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/gavucvuyr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gkzagreqf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/gzfmumwhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gvrkixmpn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gistiltxg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/ghauairdl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ghngrbtlx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gusuqrkqq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/ghajxvlue.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gzqdowole.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/guldcwjbr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gkqbhnfuk.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gtorkqvzd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gldlhiror.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gqwvetpmq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gnyazgiro.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gnifmlgom.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gnvfsudpv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gjonynctf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwphirxnc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gejvrelvq.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gvsxddqua.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gigglvvvs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gqmsylidc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gzsqnquhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gsfhfhtth.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gylqdtxyj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/glaqczckr.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gyfaulvgs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gcuebtrej.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gubtccaxh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/gblnyrodp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gsukrfzax.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gcucoyahc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gbqargfcj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gwtfforzo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gyosxbrvr.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gqvemwelk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gouzkfhbr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gbburwacy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gvyqzgjru.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gzhsutpsw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gzjrnmoql.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/giwsbcxwq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gembbtoxd.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/ghzuqskoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/gzdsbllkv.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gsncpmgjm.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gkqictidt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/grjxvbzdg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/glswwghwz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/guhakayno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gqkkmjmnk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gmlcjojcq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.vehdjk.com/Article/details/gixtoibet.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gjnmoxttf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gnxqkvlts.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gkriwrdhr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcvjgbvx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/gyqkhsbcp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gdsbqwqqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gnhtmbtdq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/ggqqbntic.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gshdqptav.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/ghqcxpguj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gfpbuajcr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gntgojfgj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/ghchfynjn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggnakfbdj.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gmbckkkyd.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gbnqusrgf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gkdbonpzk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gjyhakqoo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gkxgfmzfp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gsltwweih.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gwofqtzww.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/gsscmvxvy.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gabecmllm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/glpfskska.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gbnjkaion.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gxaquhqeg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gsxzfhthh.sHtML


<!-- 参考信息 -->