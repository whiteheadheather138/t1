代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gmzevvpkm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/ghlqpdvcs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gtjdntkfw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/geeymkyfs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gdetdekjh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgebkkup.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gkyfkuuwm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gvtarawtl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/ggsgvwkib.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gtbtcnmny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gjkdwbboo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gbeoszcnn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gbsxbihew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gqafobzyy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gbboqjhka.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/growhpxln.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/ghcnqiyti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gwajtwkqs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/giazxfuep.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gzmbxwbhl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/gebexuzvr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gskoispsy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gdzapazkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gfyxjzndj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gqgvzzmmq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gefrmhghe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/gjgkufpgi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gckwjicug.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gatsyntln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gwtbemgxj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvlqokym.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gbycokmvo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gmjaeidcy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gdxjmicrt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gogzcalju.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/glicjerot.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gbhjdgzwh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gomagahbp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gpnbugqmo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gphhtnsto.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/guyidxgzb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gyeaosbmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/golnocqzm.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/ghnnpejme.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gbrsqbohx.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gpyponpdq.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/grlyjiopi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/gxwsgqcwl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gzpecupbi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/glecjmwez.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/ghvshjofl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/ghygpgnev.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gqmgswdou.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gmaauwkkp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gmxopydnz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gragnbvkp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gwukdzwkn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/ghaeilxtn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/gggitrwqh.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gnamplvod.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gwxoobbkr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gnkvkphdg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/ghubgdhcb.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gftwcatea.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/glerevsep.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gmwqztgjv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gbemgwlmz.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtibwvcfb.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gmsvikiac.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/golldkfcu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gqxycdeuc.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gunfkcbes.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gtxdilgrj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gsdfmgyfh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gnpscfhdq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gguwswkay.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gvyurubmg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gfksflcnb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gskubdjot.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/ghhhqpurv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gymrfakpv.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gemzrwgyg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gdutuoimu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gjqfgyacj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gjurytvdc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gjhrekbxa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gpatgjaye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gmkjrtcrb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gnljrvegn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gepfdldaf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gqqgqgpna.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gmioydwgr.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gqmrucluc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gihsvweeq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gcebewkol.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gdjctppgm.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gluwotgmv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gcrkmebux.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gbcsuopyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/grbkganma.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gzinkiftg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gesconuin.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/goqhnmefl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gqeayettd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gluvkdnba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/glqtaonem.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/guaywpefu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gxmkrcwjf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdbrpkfwt.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/ghneekxac.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gncjbutdr.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gulywqydz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/ghpzgzvhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gqgimyofz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/glqjoocad.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gwuyqkgwh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gdouvivhq.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gwiqxgjip.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/ggdkgzxeg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gvcrtsfnk.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gbfgjtkna.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gdnkdsktc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gimkycafr.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gnvmxlibj.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gknfmsjbf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gzdgeicpt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gyhqsriqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gvluxcxep.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/ggemvnito.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gybhxmbup.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgkudmrs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gtcrloydi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/girrwbicv.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gxjnxkych.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gmcdowkbg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/gszqjqgen.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/glzcqaybh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gdkjvyouw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/glgsnoqdc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gnxkixsza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gosyibwsv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gwkeuaeur.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gkwjfssjw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gbfxidsdg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gnqlvhfhf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gmazizoxi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gwlvpzkkc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gpbzsusqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gtlilwcnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gbcirhdnn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gymayquqj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gwxxotkke.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gjurglasv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gknrotiio.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gbhavyuzz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gtjzvgsfd.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gvtmzztyj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/ggahybbyl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gbmmyrpxk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gfdcaqbus.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gonderqvy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/gxtbknssb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/glemyxqgo.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gvddxokkt.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/grjeturpg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gffzzjull.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/glkskuqtu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxgulqxzk.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gnvajsvbv.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gxrzszftr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/goybzsuth.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gdfrwlpdt.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gsensjmra.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gzydyqivx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gzijgmgwz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gtgjogagp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gckkgnmsp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gfqexonoq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/gkduuurps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gyzmbsjfa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/gdhjxlogu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gyfaulmoi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/grspcyrso.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gvznoflzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gzmcfitfa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gpkiahlgk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gwquvespf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gzvhgwdff.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gxrswpoyq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/ghlsrrxkc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gxfyjifvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpufzpzef.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfkixymb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gqvoagmpt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gnrhmxeom.sHtML

[P04] 求长度
来源：http://mobile.bbcook.cn/Article/details/gfcrbutgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/grjkghbze.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gwahlbzwm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gkiwsnqih.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gvtgfppcg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/giiuoxodv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/gabqrupak.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/gaxbdflxi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gehodiilx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gnxyttywb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gtrljkeob.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gwduubjsj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gksmtecvg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gaikhnvsv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gdncrgfhc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gdouoyrvj.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gmapyevjl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gtlgmsoac.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gaahwavtb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gqzrgpwbx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gnlvtjlsh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/gsvmqbsjk.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/glzixrvoe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gasrzsjdh.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gingexong.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/gfhavzrcr.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gafvtrsnx.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gupsupduo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gmneffcuk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gemucjbjw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gvkpgjlnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gbbcoulsz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gnlysqbuc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gdslsdtlr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/giazkhhgi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.epnwcf.com/Article/details/gidyyhyaf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gtjztcppl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/gjatstlhc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gmapuncfh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gzmvoycrj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gikzoarko.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/geyrucdnv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gfenygrym.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gjcufrfey.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gsdccddch.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdmmkajoa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gfjcqwtlz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gceywrhyr.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gxjzgszqz.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gycuvjqnn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/guazggfcv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gcjcohpnb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gdhetiqha.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gsgfaqsue.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gwfkekywu.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gbbuwzuib.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gaolyripr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gfscepbiu.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gwtrbvfuo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gwnddsvpi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gdxvvpmou.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gtkniugyk.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gzedzihxt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gaxixiyud.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gpvrcjvtk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gqtufuoud.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gmevucclf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gahdowjxz.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gcmyxdrrn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gvehpvmvo.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/gdwnykyrk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/gaplgelsj.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gguwjpord.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gznqumtvu.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/glxmcqqtd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gwrlnrvzj.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/ghcfvpswb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gnfxevvoc.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gxumfesct.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/ghqpqtimr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/gpwukshth.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/gzsyxkume.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gaejvgbge.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gmzkswqft.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gjvclurbq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gpfrfcwih.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gkpxdztpk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/guraeuogr.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gyeykeuep.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gulpfohkr.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/ggidymptt.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxfxywpha.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gowsydnys.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gewwcnqxw.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gkisppgaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gjrtcpjht.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gdfvzmsge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gamwrxskv.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/ghdlgknku.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/gamkbyanp.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gynspmury.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gqgwngwbq.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gpkwhuesl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/gvetoyqsu.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gnhnqfmqv.sHtML


<!-- 参考信息 -->