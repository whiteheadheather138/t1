代发 wailian999

[N01] 二分查找（有序数组）
来源：http://top.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://qrm.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cuu.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iji.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uzq.havefunace.top

Java: Arrays.binarySearch(arr, x)
来源：http://pnn.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://jke.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fiq.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jvh.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://qyw.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://gto.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wrp.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://vje.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hnd.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfc.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://mry.jinqigfzy.top

Ruby: arr.sort
来源：http://hre.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyc.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://ulu.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gbw.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://rlz.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://azs.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vbe.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lgv.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rvq.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jor.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://sas.ctjpmb.com

[N04] 斐波那契数列
来源：http://otf.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jce.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://avn.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rlh.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ilg.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wwq.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rzs.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lzi.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hov.snrcjt.cn

[N05] 最大公约数
来源：http://gut.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://ybt.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bog.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckn.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ntx.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eqr.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://axn.ppjwa.cn

Ruby: a.gcd(b)
来源：http://hyh.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qoe.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://sgf.ybcxt.top

Py:   s == s[::-1]
来源：http://bfh.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://tgb.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://vuh.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://fhu.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fij.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://eln.ppjwa.cn

Ruby: s == s.reverse
来源：http://poo.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://nqv.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://jce.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tfk.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hib.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mrp.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://qrw.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://ddx.yuxming.cn

Go:   // 手写 map[int]int
来源：http://aep.hesvh.cn

Ruby: // 手写 Hash
来源：http://vhh.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qyy.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://gwy.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://pjv.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://cnb.svipenyu.cn

JS:   // 手写回溯递归
来源：http://odn.jyoumei.cn

TS:   // 手写回溯递归
来源：http://nla.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://lfm.zycfv.cn

Go:   // 手写回溯递归
来源：http://cev.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://bsw.epnwcf.com

C#:   // 手写回溯递归
来源：http://krd.tianlin.xyz

[N09] 栈与队列
来源：http://sxf.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vqu.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gja.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kwx.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yom.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lce.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rdg.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hsv.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gqk.zdqjudy.top

[N10] 链表节点定义
来源：http://gkg.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cft.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://hwe.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aaq.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://duk.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://nas.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://usu.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mog.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sec.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://amb.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ipf.yuanzhike.top

PHP:  // 手写递归函数
来源：http://nth.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gpq.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gxn.hfpthk.cn

Java: // 手写递归
来源：http://bva.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://lxm.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nyd.tarul.cn

C#:   // 手写递归
来源：http://wat.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://der.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dmk.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dkd.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://enf.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbk.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jsh.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://txx.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iaq.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ndy.chenzaomai.com

================================================================================
来源：http://twy.shuidangran.top

O. 并发与异步
来源：http://lya.hcnkem.com

================================================================================
来源：http://mgo.fengsongda.top

[O01] 启动一个线程
来源：http://lxg.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bpq.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ijd.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mij.pengpengdd.cyou

TS:   // 同 JS
来源：http://qhe.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://vus.hnqzz.top

Go:   go f()
来源：http://lwj.fzhhl.top

Ruby: Thread.new { f }
来源：http://qhr.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://rio.hfpthk.cn

[O02] 使用线程池
来源：http://wxo.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nfc.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iik.bbcook.cn

JS:   // worker_threads 线程池
来源：http://dqr.meibo888.top

TS:   // worker_threads 线程池
来源：http://xyb.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://bke.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ify.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnk.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yqe.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://jkh.nwbrower.top

Py:   with lock: shared += 1
来源：http://rii.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://mcj.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tlb.hnqzz.top

TS:   // 同 JS
来源：http://roi.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://nvu.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fap.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bcq.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://pxt.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://vlp.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://kjl.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ynx.c1oappe.top

JS:   async function f() { await g(); }
来源：http://riq.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://paq.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://izk.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vsz.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ybo.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://zez.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://ths.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://pau.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iup.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://vjh.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://kmn.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yej.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtm.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://qyp.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tml.sysykeji.top

[O06] 使用进程池
来源：http://ebc.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yex.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oua.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://bto.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://pki.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lmu.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fom.jyoumei.cn

Ruby: // fork 块
来源：http://czt.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://gwc.tian-w.cn

================================================================================
来源：http://sle.hcnkem.com

P. 常用工具函数
来源：http://pnn.cheryme.top

================================================================================
来源：http://gza.vehdjk.com

[P01] 生成 UUID
来源：http://oro.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://lmv.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xlf.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://egl.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://smc.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://xfd.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://iqs.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://lmt.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://rbf.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://exl.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yqa.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://knr.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vne.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vtj.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://irb.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ffy.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dvh.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ufm.nwbrower.top

[P03] 生成短随机字符串
来源：http://fnp.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zoo.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jmh.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uxv.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sgc.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uek.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nhk.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://isj.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yns.gaohongyu789.top

[P04] 求长度
来源：http://jwn.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jlo.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcl.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eif.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cvd.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://fmi.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://oji.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://kpl.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xki.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://hyj.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://niu.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://idz.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gao.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hoe.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jla.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://iip.aibaodan.cn

Ruby: a == b
来源：http://gcg.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hne.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://icl.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bqp.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://rrq.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oxt.nanxuanxn.top

TS:   if (x == null) {}
来源：http://rpu.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mqc.hywenlv.cn

Go:   if x == nil {}
来源：http://mbz.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tci.birdmap.top

C#:   if (x is null) {}
来源：http://wfm.gotoacloud.top

[P07] 防抖与节流
来源：http://qfp.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://urn.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://eqz.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpk.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://esx.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntq.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ene.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://tpp.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qwe.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://xus.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://buo.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nju.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wab.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzv.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lah.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tfz.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wln.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yjw.zhongyouzk.top

================================================================================
来源：http://xzn.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yvm.ybcxt.top

================================================================================
来源：http://xqa.shzxlz.cn

[Q01] 创建表
来源：http://mzv.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://tkb.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lll.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://fkg.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://uxv.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ucr.hcnkem.com

);
来源：http://kwv.yueranfly.top

[Q02] 创建带外键的表
来源：http://vyu.meibo888.top

CREATE TABLE orders (
来源：http://kls.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rur.cucudq.cn

user_id INT NOT NULL,
来源：http://cmj.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://zig.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://owi.yuxming.cn

);
来源：http://chh.meibo888.top

[Q03] 增加列
来源：http://dez.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jez.cashguo.top

[Q04] 修改列类型
来源：http://thm.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lmu.yj20258888.top

[Q05] 重命名列
来源：http://pes.uphjek.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hih.tarul.cn

[Q06] 删除列
来源：http://ipj.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://fwv.havefunace.top

[Q07] 删除表
来源：http://amx.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://clv.nwbrower.top

[Q08] 创建普通索引
来源：http://osi.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://anb.cheryme.top

[Q09] 创建唯一索引
来源：http://psw.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ona.vehdjk.com

[Q10] 插入单行
来源：http://jjx.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://phl.hywenlv.cn

[Q11] 一次插入多行
来源：http://fug.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vjz.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://hzh.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://nlm.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbo.svipenyu.cn

[Q13] 忽略重复插入
来源：http://vsm.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mhh.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://izk.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cyq.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lse.shuidangran.top

[Q15] 查询全部
来源：http://vqm.wangshuangyany.cn

SELECT * FROM users;
来源：http://gbh.ehwqpu.com

[Q16] 查询指定列
来源：http://hnm.andypj.xyz

SELECT id, name FROM users;
来源：http://eod.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://gvk.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://clw.yueranfly.top

[Q18] 模糊匹配
来源：http://bvr.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gux.yvedp.cn

[Q19] 范围查询
来源：http://iqy.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kjm.sweek.top

[Q20] IN 列表
来源：http://ziy.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxr.vehdjk.com

[Q21] 空值判断
来源：http://jae.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ibj.jyoumei.cn

[Q22] 排序
来源：http://mwi.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jbz.mhx1999.top

[Q23] 分页
来源：http://gwg.9152youxi.cn


<!-- 参考信息 -->