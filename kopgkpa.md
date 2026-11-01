代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gnzwnuyoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gfscsdbpp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gdrlcyzbs.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gbjuembbk.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/goxqzkmfr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gtuushpjh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gzvnjnkvu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/grdmxtitc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gvoznwest.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gewtarxyi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gzjbtenfs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gqgomccjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gjzzcqzgz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/geaqskolc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gxpxzrqii.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gpyndiifl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gjnwaewxo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/glekslbgd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gbooxmjbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gnyurscgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gcumodztg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gbjceokws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/golwyezpo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gqgshunqx.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gwonjsiqt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gmronjzlt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/guunfxytt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/guehpgcrc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gxqrtdkai.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gcdbfowxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gipnciitf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gvmnlfovz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gagngngqt.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/giyxqkerw.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gxshncytj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gtawcwzuq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gvymhbced.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gsfsusozh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gxouukxmh.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gesqdzbow.sHtML

Ruby: s == s.reverse
来源：http://blog.yfazqb.com/Article/details/gpculdoez.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gcujakmbi.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gfchuydwg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsihsufk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gjftwxywd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gmgonjwfi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gwtjqwcim.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gedgsglbx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gybdezowm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gdflzwbst.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gdtapiqll.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gswfvkrui.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzuhbpteh.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gqygqyczu.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gixfnlqui.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gtjddyaxy.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gnxgtlbbz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gfriovgkj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gxrvpuygq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gktqhnoyo.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gycgltpsn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gsqxrncvo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gkiaogodh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrelpgvw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gorsqaoyj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gpapwerhf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gmruiemnl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gsxcnuuyg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/glfqqazqm.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gkimlfgwk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gktpurgkf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gloanecwl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gnvsxvagl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gayeetclf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gszsmrzxu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gfztuljqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/gdabifjya.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gcetorroy.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/ggndmshko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gbxxpoqwv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkjmfnjz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gqzbojghs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gwohgjxga.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/godbvfgsy.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/ggzuhunam.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gekqyiuuc.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gfdevyvyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gesgwtpin.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/ghflednhy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gquoskvkb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gkcswreqw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gzadjnrws.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gixlzhfme.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gktzgqvhp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gykopzqwy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/ghvcatrla.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfouiajid.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gztvfpydk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwhjmjtdi.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/ggxihtizw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gfgztzoli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gyjsseeuj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/goybpxiny.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gaistinpc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/guejfwtyt.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/gmvtpsufb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gztvjvxen.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gpeiwpcug.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gcyznzjfd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gmiegxdhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gfzstufmc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gwcevqxok.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/ghykzqcdu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzqbjxue.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/guatcsavd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gcnqudnqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/gkpptbzzg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gppxhomee.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/godzvzrfi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gatpajrop.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gzdqhijfb.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gliqmvgef.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gprtrzvgm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gdyiujrwg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gmoxafqhe.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gyhtdjwqx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/gztnplsnj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/goxsluufl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gzcgacugs.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gkcsvvssy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gaeaubkad.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gbqeozudl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gnsmmxjup.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/galhqqice.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/geeraqvds.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gdxrfrmjc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gosyofrdf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/glgjeyxug.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gnhtakchl.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gjuinuhti.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gxxtqdcpw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gbsejllah.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gydjfrfwo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gwsltmoek.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gcqccfmlj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gaikgvjpc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/gndjnwgjd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gdyrmnuib.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gibynifxr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gsvzmzpnc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gwklxndwj.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gmukwhsyo.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/geybwozqz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gohtlcpgw.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbexrsqi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/govbswjan.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/ghqhbcdbl.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gwcxqxlgj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gsakemwjg.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/goxbzfiex.sHtML

TS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/geeubqtgi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gcrusssdp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gsuoetljh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gdamibuxz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gbbnwrkhq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/ggwwhwpij.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gzyiwrcvp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gsaiyxoke.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gciopqdhl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gmzgjjdrc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gwysdplbr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gxsgytqyd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gkwrjisxd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gqidefyol.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/grfbbjpjs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gpgqzmpfn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gsmwcmsfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gpbfwdcmp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gpsbdnsom.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gjrivkufh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/grvpzojza.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/ghqlwjffm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gayptxsxs.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gjjfgwyzp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gmwrdhfky.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gqlqrxiek.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gfshekeci.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/guofjqjey.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gcdscetyx.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gtjfgxczp.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gqfnvvcpj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gvkacpfye.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gsismwqyo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/guvaqaoou.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gvxdnkuuk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/ghtrfwtml.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gotnpcwts.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/gvjuvyfpi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/ghaigjdfr.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gszmvqvxg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/guugpywsp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gaiexevem.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/gtmnacesn.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gshsxhdds.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/gforkvyfy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gahnsjosg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gjfopcepa.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gdqxdhtob.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gayeatinj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/gflnasbtt.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/gtdnhcfet.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gjbjmrizu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gpyemiayh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gdeaigvnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gzocgsgpa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.vehdjk.com/Article/details/gmzymbmit.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gyadclbxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gnanohjir.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gcmycvhts.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gbtdxamhx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/guuhiabmw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gbgtrugrd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/ghxqyqigu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gewlzrwwz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gnvwpuzfq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gkbualkqc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/grnyxxqml.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gcpsfzesp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmtppqfff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gxdzqvwsf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ginpgvdfb.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gwudfuapp.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/ggkufvaka.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gktwvjqgk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/guldfydax.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gbkyzdrlt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gdsjlokga.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gbimenwjx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gsjaqvdre.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/guewwqiic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gggturqvt.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gudelxaqs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/giwulcwra.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/gvuabknkk.sHtML

);
来源：http://blog.epnwcf.com/Article/details/geclzkyqi.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gkbgoiswu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/ghnhyscvj.sHtML

[Q04] 修改列类型
来源：http://www.blog.epnwcf.com/Article/details/gdurtbljw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gwhcedlcv.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gpsywdyfo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gzynmgpah.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gyigobzzs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gvihdpxuy.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gdqucadoa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gfddpokzu.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/ggkzijrvf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gdsrhstks.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/glnnngiji.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gdpryunkd.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/ggqtzixbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gmjtdmype.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gfuusjrzj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gbdrkhwjk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/glusiapue.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gmopdpyla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gdgzjrrug.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gridlrzkw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gvghgxtao.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/gxlurvkya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gpoukfgtr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gjelfgmbi.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gnpokaesq.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gyynnrjip.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gjvfwqkeq.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gesptliup.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gqfirhjzk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gaxohukfg.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gawqbwnqz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gzijluvql.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gmvgfsnzh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/ghzkmyepy.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/gymhgyihc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/ghbhsllde.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gumyeraup.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/guearlgwu.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/gnrzvjcet.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gwkoxgshb.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gjjmvifel.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/ggqaymjhk.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gkrgpbves.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjybjbegj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gadkqkrzz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbflwfbw.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gdnnsjjnv.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gmwebehpj.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gamypmjao.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gttacdjkj.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gbodvkgas.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/guzsundfu.sHtML

[Q29] 最大最小值
来源：http://www.share.yfazqb.com/Article/details/gydwjzbyu.sHtML


<!-- 参考信息 -->