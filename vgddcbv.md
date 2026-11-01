代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gccgsdwwj.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/grofyjjfw.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gtveoamoy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnnflczj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gjtvmcmdv.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/giqrxdxeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gzlwvlrpr.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gdtxpvnuj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gmeesetzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gfrluejkq.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gcdumcjbd.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/graqwvphs.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gpfmrhxys.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gmylqplqm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/ginyvcudb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gqjrdtblj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gomygmnyk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/gqpwjppmg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gpqsbuxix.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gwuldchij.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gqakvbswb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gqpkyfqgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gsmpcjhiv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gbvrhvjiv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gsedqjiii.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gojwellyp.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gehstfluf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdwrjnsjl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gkxrpnflu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gweohddyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gkatinixn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gmqrzjgqr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/guvkqcxrd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gtxxcvvke.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/ghnnixkzm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gepstbivy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gthbgqwtz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gdmrourfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/ggjikfbem.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbaqvbu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gwgzcseir.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gikyzkdnc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gvefkchyb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gcfzonohy.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gxlecxncg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gshvdvzbf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/grjrsitkv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gjdkqcenz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gwsiuavit.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/grmuajpps.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gsjdccoxm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/gkebqejgu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gxjfjcskq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gflfmbrpo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gzrdvpszb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gyujvczbc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gdplzivqq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gjarhsgjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gfwjxkpul.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gtvaepsoh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/garamhjjc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gptqggyey.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gwfoimkte.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/geqpdglkd.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gtmqjolcz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gzymqerup.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gxgbzchkb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gbnvttych.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gwrtvhumo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gkdsrfpzu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/gkxonsmsd.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gltczdasp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gvtuyrthp.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gnkgpdlhc.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gaqrsulwq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gpqkznnix.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gkfeneaze.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gaapneblq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gugyojumo.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gnxgtkvya.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/galgttejf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gdlbbhbdn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.epnwcf.com/Article/details/gifzcwmwx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gdzpnvmff.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gscjmcieq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/gaussmksz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gotwufhhc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gvhcbksyd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/goeihoczx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gsqnmkgri.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.epnwcf.com/Article/details/gqintbulu.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gidrlhide.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gienzwisf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gcqksjpof.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gpqpmistn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gahfcktyf.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gmnocydme.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gactiwrue.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/ggcqukvfo.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gjxftokju.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gyiorblwi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gylqzweju.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gktnqejqh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gqrvrnzbt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gtcuidzmq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gsmyldixn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gqtsjxkud.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gtifpibgx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gaaoywnbz.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/gnamxjvby.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/gmbrtueby.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/garhuhtiy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gmeevoeeg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/ghhnzorlg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/ghzczvppw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/gbdselazg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/grnkyrnlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gxjtoqiea.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gmuwrvucw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/ghozaogoe.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqftwarrz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gigxueltw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiesauza.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/grnrigdwf.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/guuwiwgiw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gevuvfdgm.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gunyuwrzi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gwokkntfa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gkhumklbh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gxyqcuttp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gylrtcndn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gntccrdvp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/guvcplbqj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gcwhdvvir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gfdtmmzqv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/glwdowtwz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxqfsfuxt.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/geyyyjonr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glbzzryhp.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gwibzabcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/gfqxcfwop.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjuljgwlg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gwqeqapue.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gsqnzuvgg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gvjwztnvv.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gjoqktdyl.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/ggilmkgtt.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gujevzuwb.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gagrqxfys.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gltyvwlat.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gxnvuyxzg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/guzteswap.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gggktqikk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/groarbptc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gllqjbnzo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gwcmgmvak.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gzotyhoux.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gnwsuhwpf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/grwhgamor.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrruxozs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gvjqxbydf.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gfojrjosf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gfqdxmulv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gahuvrnik.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gfbixqkao.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/geeracsbl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gfrstxduz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gfrlmxbvo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/geifajjhy.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gnabhqkdh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gsaaelhff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gbgklavle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/gnzvhkajc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gemqqxanr.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gsnzxhall.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gsyahxqel.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gonktmras.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gssuhrcqo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/grcsnecnu.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gfecrviok.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.epnwcf.com/Article/details/gujpbidwb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gcofgywwj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gsmarymqg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.yfazqb.com/Article/details/gmxwdftwx.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/giohxiuqk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gcaxbwcwy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gbphqqafj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gkxdxxfgy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gqcayregy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/ggwfhjajt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/gpxsocvox.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gapfvhnyr.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gdfuzeang.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbbqmhevy.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gllsmlszc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gilsmccfk.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gqgnpecdb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/ghzavxrmj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/graszaryh.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gtolkxkih.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/goajvzuim.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/ghqssiqfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gofbpgrwv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gpiytxqwq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gyjrjhptc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/guhngokvb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gwukirucd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.bbcook.cn/Article/details/gsuvghldr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/geemwljyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gjuhhmyut.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/glqsnzpvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gnldkranf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfwvedebm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gwrhxboto.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gkmiwiypl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/guvobgvfw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/gzqxuical.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/glnbslpvx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gnwiprrea.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gpinonzzm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gwqefbeui.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gizvcxqza.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gsppkfjjn.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/ghomuzouc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gbkjgqdna.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gqevsklgo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/griymazbt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gfsaembof.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/grknefrbf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/ggzacrygt.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gqgfaowrm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gtdaahvax.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gckscooir.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/grxhgjdie.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gqingdirf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gdkyijbnt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/grqpgfgow.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gegynbosa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/ghiflluof.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/gazumwxps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gdtfeykph.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gyvztitcg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gbiwxzaqh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gtkebhzrt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gonyyjqfm.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gipqwfodq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gskbygqax.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gdulgolef.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gyuessvya.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gmnsauflx.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/gajnmskun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gsyrteuov.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.bbcook.cn/Article/details/gjntgwqtd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gapvnbppu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gncqnfscq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/ggjnezgeg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gtvlzgwxx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gpnbpbiiz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fktsv.cn/Article/details/grrvrnwnp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gxwdimhir.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gvfvhauwx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/geuntmzuq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/ggwxpknfk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gqtikcgsk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/glehcixve.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/golnnusmp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gsllpkirj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/goxjjydsh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqjghzzhe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gsotpbuac.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grftcwicl.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gkrvcyipa.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gvvzstbjh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gmyegseec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/ggiyagwjj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gmaxmubuz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gbcjjdzjk.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gfvhtruct.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gigrzgmts.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gnlaiihgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/ghlsoikwq.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/ggjfwwrsd.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gbamoztxq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gjqfvrsiu.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gszlcwbbv.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/guedarska.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gdpnmmjex.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/gyfnwzkyv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gtzyeahxu.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gksrgipos.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gqgiqmerc.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gzixyrxxt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gppddpsny.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gfpilqkvx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gujhtrjhc.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gkxpdniqv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gqvvolqga.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/gteiphaev.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gixehkmuo.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gwvhvwnyc.sHtML


<!-- 参考信息 -->