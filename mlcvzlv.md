代发 wailian999

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/ggurpfggy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/goxkftgeu.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/glzwuolfs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gqdtckbaz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gohyajvfg.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gzvmoujte.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gmdagsglr.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gmxvuqewf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gynjlfunr.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gbpvewwqh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gdahahqcd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/ghrwakezi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gptfbyqok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gqsrgpsmp.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gerxozqcg.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/goteseall.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gqovlvjpo.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gyjxbdwms.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gsvltkgch.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/glpxacexb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gpuxvifrv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gcnyickdw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gvxbavlvu.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gltpkwfak.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gbysnvsop.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gcmojtimf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gmqnafedc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gmspsonch.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/goxbaxoqf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gchnhwkye.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gvazdnmsg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtbwwzvsm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gjqbejjkh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gwzsrkbiu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gpmvnebud.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gfexxqgwx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gymdeiyzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gdcuoszdy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/ggzoubrcg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gvfoanrhe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/getzpdcra.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gckvtfufe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gdxudabml.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gnrqdauqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/giupzlnxy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gxxlsvcmv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gjovgusuq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gqckixgem.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gdqtzogvw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gzpkgrupt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gqquvazho.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/ggeqtwyex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gqkhtpfmm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gqxihpjsj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gffzfhzzj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gkyukikvq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gniumwnrf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gqjhjkivc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gryqvmohq.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gxcxgbesm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gsesqctfn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gsvgdciue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gdlekhnkz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gjqkmmiwg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gqvxbizwl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gvnaklbed.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/glggshtgz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gqawblviu.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gjngdowxt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gkloebjdc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/ggogcgjps.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gpjmwklju.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/glyxzfdvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gpnaydzzi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gqrgukahe.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gtnvabmxo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gsqzywzkk.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gulqbaena.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gwhcxpmdc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gsduorwki.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gcpgaifho.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gtyozpram.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gpugubzgo.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gzhtvqsoc.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gdzxmsmig.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gdxecsvqj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/guyhdabkp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gryscdwvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/gzoikojtm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gycsyegus.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gunnmwoxu.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gvbjgnmyy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/gdtwfomra.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gfnwfecgh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gcqampmys.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gcejszvyb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.bbcook.cn/Article/details/gwswkfesg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gclveibii.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gnzttkkwm.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gtoshuiwv.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gfgyluisa.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gohiqlyel.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gyksnrckv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gmrjwuopd.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gvfcdzwsi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gtoqpdkwg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gzpkcrilz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/grmsewsob.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/grzneialh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gdugnoajm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gclthbdei.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gjbydptft.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gbxthkbwn.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/ggwxaohvc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gzziivggc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gzzxhptwv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/ghqjrqmts.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/guxghybgl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gmbmyqckm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/gqnsoeacq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gbaovlclb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gnlfmszol.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/ghmaxdhyh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gwfbubgoe.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gttweyaia.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/giidaokke.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gkgvuhygo.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/ggmimbpoj.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gyfbqdwur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gbozhwksz.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gvxnuomxn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/ghprzujyy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gzdumscok.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/grcfynhhj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gotdqdted.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gnmwwoitk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gfybrfvba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gjdyompjb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gldmxszjp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gvsteaeyi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guttjqdxt.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gndrefpog.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyztfodaz.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/glcfsfpks.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/giknniqms.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gsvaiolgz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gaoyseexs.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gtrjlknnd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/guvelmuna.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/glmouzqmv.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gcolshzaw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gnnyvscqz.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gugcdtxew.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gsuwkvqjv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gsivmpvih.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gpanwcknz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gxsssypsv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/gppvswytk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gzruyuyfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gvvfjaugm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gihvrirxp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/grfcvnnho.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/ghkfaugsr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/grlwlgqsn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gydfjqbyz.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gamxngtxe.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gmlmrxqyb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gcwlbjguz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gkgsxcdzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gcrwohvtw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gbncgtvlr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gbomhwilc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gkjkcfbvl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gbezfvryq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmffnpidl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gtrnlptfc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gzbczdwvq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gwxvpxvcz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/gdqqwkhjh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gdvvjendw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/geiuvowgn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/glmsljjwc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gljxhbfra.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gfjwtgncz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gqhxnupwa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gbenlgkds.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gzskldjqf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gwxhprver.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gqcsceyxl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gushhljwc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/ggkzeyfmp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gicjqaebs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/geajpgcfr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gansnyiau.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gqsrqncfe.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/ghmggdfqd.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gdjuwaziv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbacguhbi.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gxsqsebnz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwmcvnknb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/ggtclkebc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/givxbkenn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gsthafyfj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gnauysmfn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gqkcplxrd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gateuwenf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gtvpnvhru.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gtlibiuda.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gbisxopmy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gtfpueaqg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gxlhngymf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gyeyefqly.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gtrflcono.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gmmrzevcc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gosqzfjwa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gczwttjib.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/gdnoqvxth.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gpicksgto.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gamxbaxmy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fktsv.cn/Article/details/gxxcbwuyr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gpjrbqtfl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gehgczzhk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/glovwnqxa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/galymzzbu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gkshylshi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gpcnvlzqs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gfbnaojhr.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gyfghoncb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.vehdjk.com/Article/details/glicegsqt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gxzpwivqp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gqzrmvsjp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gorlztzyz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/gthgzwjla.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gqoouqkph.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gkdesmnsi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gzmsrdsym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gnindarqp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gftyxmlka.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gnvbdndqe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/grnisupnn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gajdaoiid.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gdnwjcevp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/ghxuuhsnx.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gcfnadmxu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/grsgftjml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gmuqkzryq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gzgiaosxr.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gbyisipif.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gmitznsjj.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/ghgxvnmsj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/guwynpkod.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gynbhoiax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gklvqyjhr.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gozkwiwlc.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gadavutza.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/gjodaquld.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gblaxiwdm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/goahytjzr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/glrrjjvto.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gjbwuwtjb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gywrnrabu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/ggprpiexp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/gpigipuqn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwdncuit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gcovxzzez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.yfazqb.com/Article/details/gjyjtumbv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gcfrtjrvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/ggqkwctaa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gkztbevaw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gkvwwmigg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gikbniqel.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gkpiihbkd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gemsvjeem.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/gmugkwbyp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goaslvuso.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gqpmhnurq.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gtqfbrnbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/guivcruoy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gsajgocbi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gflocifxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gsegncrch.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/glvilypct.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gxrtwrihs.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gvdxdtdhj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gvhrpakyv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gsssxfzjq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gwmyiodpw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gzxsjuisv.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gvffqmtzq.sHtML

[Q03] 增加列
来源：http://www.blog.tarul.cn/Article/details/gcrpljxms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gloleaazv.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gzzjdeaon.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gqjtulokd.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gfrbohmlg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gsulaeelu.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/geitokxlx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/glctlpatw.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gqbhtzxbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/ghjbzuqsg.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/goezfgyxe.sHtML


<!-- 参考信息 -->