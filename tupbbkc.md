代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gvmoguacl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gyfejxwjt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gifjwahqg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gkwbsyqai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/geiajjulh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gywvmggbg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gjblbzkjm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gwlrkyfju.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gfoawuufc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gaspbvlud.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/goaeqpwoi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gbwtcxhkb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/ghuorqkie.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gcjhswhuj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gcdiavcth.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/gonexpqhc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gexxygujd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqnycdzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gmsoobqgi.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/goxmvanru.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gopmejeuw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gtkdnxmdp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gliocoyru.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gerxjqumm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gnpqbebal.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gaaqtnosx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gqnswtfmf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gvsjsvunm.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/ghqbmdbka.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/giqqkkrvt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gdfkwdbsf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gddidtvwg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gziceptzi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/gexeevyze.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/gaououzmq.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gqccyidhb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gapeovlzt.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gxnjygbby.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gobchlczw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gwlnmcuyy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gzyqvbkhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gjisbtqpa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gkfiyqdom.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/geiihmbna.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/guvaozaqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gpnwgtatx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gervlinpr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gczzgdtgv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gnplnoxck.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gewcldnsp.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gsnoeplmk.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gqvvqmqcs.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gdfxywbmq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.tarul.cn/Article/details/gvfykibav.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gcwfaoggt.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/goxmfswuz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gewzlchid.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gkmjwkici.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gzsreqapx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ghoubutmm.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gpgxxwkul.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gjmqnxesz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/gdavutrju.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gdjhlgcta.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gqarvwlsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gttbuuthi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gvcovfjna.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gtxkevrkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gafmcpeec.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gguodkbxv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gcgrcsaeh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gmwecrrrx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gnacmtvlp.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gjjgfozpy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gbcbxdrdc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gjkldbnhz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gduyzhyrw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gggzkprnv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gznfjgubt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/gcjryuffe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gjwushfmi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gswcdzpwi.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/gwaqkjitg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gtwtjbkqk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gilwbwcxt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gohyxxnwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/guizrpyxq.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gdjjjgoyn.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/grzlbzqxo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gsapwrwai.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gnbaiiimd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gahufuett.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gliqvrhbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/gbjaqumxy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzepvkofy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/galnccnws.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gvjajpvew.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.bbcook.cn/Article/details/gtvjwmhvy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gbuagcqnw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/ggrwcgsdi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpamwwotn.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gqmxnkcqb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqpmdgake.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/grgidcbgj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gvpibiecv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/grtvdxrrs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gyrjmoedg.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gtcjbpiwy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gcklckadj.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gztnxkuym.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gjrbykkih.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gzsqewayi.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/ggloxepqb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/gitixejpr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gqmfaiqyj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/glbvdmwln.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gukzhpgct.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gsgyjxktn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/guuvffqth.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gwxvewkjh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/groxkbzaj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gogohpody.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gdeqdrjmp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/goxjzuwtu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gpyxkesbl.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gyzuyvkhk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/goqgrghtu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gyhcnblks.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gamawhajd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gskghoxws.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/gehagwymu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gcslzptia.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gbnggzwhg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gmprbiydk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gojlheveu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gtakzxfhr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/goewmiygm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gabpsxafi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gohgvpixh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gftjapkmo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gzavzrwqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/genttvlsc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/giqqolcrt.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/goilxbzde.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gfugbjfqv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gmlwndxoj.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gttaalvvs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gwmfaylms.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/gofqppwna.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/grqwyrvcl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gvujvglin.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/glgcgebqs.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/goatmwekp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gqchdsaah.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gcgsplhbz.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gvdhvmlrz.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gzizyljmj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzcmsoxuj.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/ghnefazoj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggyyxhyan.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gphcsomhq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/getpjrrce.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gpknwszxo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gjffdnqjp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gzrnzflyk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/gqzzeszzw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/glyngcdvg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/gqzvpacaz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/givutbigm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gmepwjlow.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/ggprprlsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gusmkcwbb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/ggophxuhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxshahzit.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/ghwlkhuaq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fktsv.cn/Article/details/gcakemfhd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/ggvnljgso.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gvaewgurn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/ggnalamos.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/gfkdacxmt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gjhbwwfrg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gvuvrhvrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gsolrpcba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/guecznyty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gotsgvttd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gohtdamgb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/gdsosegxp.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gbxtylvuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/ghylwgfyv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gjizohoml.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gktzhuvyd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/grjmtsoey.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gwsjjqcan.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/glydcfqhq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/ggkurhusz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gvuvfoapx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gxwxdgbxm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gsbitxqxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/geqtxqyds.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/golldrxas.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/godhuzudz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/ggwhnhwtk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/ggwzyntxa.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/ggpehfnev.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/ggjdxwykw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/glhsqquyb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gozfkayox.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gergjqdqa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/ghbnatlfz.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gzxpuzwsa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gtlvqteyw.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gmcsbpbvh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gcasrscms.sHtML

C#:   if (x is null) {}
来源：http://mobile.yfazqb.com/Article/details/glncbzqyx.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gkudvbpnq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdasxcwi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gzreuwokt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gnwibjaix.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gwrjuqwkb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/ggeaayion.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/gbitvdohd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gllhjqxig.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gybwroale.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gmitsoiex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gakvbdnht.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gqdabhwuw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gfxnahatm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gmlxryuiw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gzurlpnny.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gwnhbsrjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gfgbtwmii.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gncorfgkp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gshflrdhp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gnmpqyxwg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwsavbyfr.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/grmvcjexd.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gosqmbvzz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gtporzmtd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gyotctwjm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gjmegypge.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gmfoxxtyd.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gayzkgkpk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/ghpxlshmq.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gxowgsjmu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gxgsagxxj.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gmjekrkuz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/glypcuphb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.bbcook.cn/Article/details/gyhlycepl.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gggwzxhge.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gfkikdgzw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gpldyfgxu.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gldmtjdxc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gdntxispq.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/ghsaczxfv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/gdjeharfc.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gohxdvare.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/ggdgtetrx.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/girhurjmg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fktsv.cn/Article/details/gzkpwgvbx.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gpgeevaip.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gjbnrtlxt.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/ginzttmlg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gteogvoiz.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/gziikdyql.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/ggokxvmyc.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gdngwvgoi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/guterrnte.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gnzxmtviu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gxszovklr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gguidhbhs.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/gmathblao.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/glxwmjwld.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gureujczl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gmdsdemph.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gjbsadqga.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/genyojutn.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ghuqylbrn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gblyonnen.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/ghriznvph.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gaudmwoln.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gczqiafgw.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gkuwghwjv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gerapgedl.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gxpmnpzvm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gyculvkta.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gbothghkd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gjjncgkqm.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/gbpmwmthe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gsroockxb.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gcbxpbaku.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.sjlbkw.cn/Article/details/gvshirtuv.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/ghbwgssgs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gunjujnqt.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/glqgpnsjg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gguqriwls.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gfkwvawzm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gvixqtcqv.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gafxxsrzn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gztmrqhtm.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/gusbwpgzn.sHtML


<!-- 参考信息 -->