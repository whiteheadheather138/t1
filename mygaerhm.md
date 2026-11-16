代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ylf.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://mzn.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://xor.xziqi.cn

JS:   process.platform;  process.version
来源：http://gvl.hcnkem.com

TS:   process.platform;  process.version
来源：http://qyp.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uzx.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nnx.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://etd.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fdc.tian-w.cn

================================================================================
来源：http://ufn.tarul.cn

N. 数据结构与算法
来源：http://bas.zdbjq.cn

================================================================================
来源：http://bdu.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://ybq.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://zon.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sog.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sxq.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kvt.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qyi.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://fof.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zdy.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zxv.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://eje.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://tbq.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://shj.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dby.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zbn.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jah.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://tbq.zycfv.cn

Ruby: arr.sort
来源：http://zra.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://khm.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://tpx.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eua.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://oaf.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tki.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gmd.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ytk.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yvd.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gtj.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tbe.yfazqb.com

[N04] 斐波那契数列
来源：http://qdo.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xvd.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xxk.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cht.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nii.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdu.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mkw.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wvw.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rgp.shangyingyoupin.top

[N05] 最大公约数
来源：http://nzo.c1oappe.top

Py:   math.gcd(a, b)
来源：http://hbx.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qwc.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idh.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfx.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://evd.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://srd.bjfxy.top

Ruby: a.gcd(b)
来源：http://usu.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bcv.sysykeji.top

[N06] 判断回文字符串
来源：http://sor.cashguo.top

Py:   s == s[::-1]
来源：http://sbw.jianghu66.top

PHP:  $s === strrev($s);
来源：http://efk.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://sdt.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://goq.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gqb.sysykeji.top

Go:   // 双指针从两端比较
来源：http://zaa.jinqigfzy.top

Ruby: s == s.reverse
来源：http://src.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mzp.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://eqz.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dil.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqa.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cvx.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://hwt.haohaochexian.top

Java: // 手写 HashMap
来源：http://ygq.hnqzz.top

Go:   // 手写 map[int]int
来源：http://rte.epnwcf.com

Ruby: // 手写 Hash
来源：http://muf.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://dcv.ehwqpu.com

[N08] 生成全排列
来源：http://pqn.cheryme.top

Py:   itertools.permutations(arr)
来源：http://tlg.tianlin.xyz

PHP:  // 手写递归交换
来源：http://qgb.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://xmd.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://lvw.sysykeji.top

Java: // 手写回溯递归
来源：http://auh.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://kwh.meibo888.top

Ruby: arr.permutation.to_a
来源：http://vyi.gotoacloud.top

C#:   // 手写回溯递归
来源：http://qiw.shzxlz.cn

[N09] 栈与队列
来源：http://mgl.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bph.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zmw.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uhe.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nes.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nwt.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxu.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mzp.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eda.svipenyu.cn

[N10] 链表节点定义
来源：http://zmb.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kfs.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://adn.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qux.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kre.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://jqq.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pxb.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hpw.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qyj.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://apg.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hgd.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://zkq.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jgy.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwh.cdnleiting.top

Java: // 手写递归
来源：http://gut.zhijiandao.cn

Go:   // 手写递归
来源：http://ptc.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bwl.sysykeji.top

C#:   // 手写递归
来源：http://xaf.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wti.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://viz.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gak.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gcr.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ljv.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uod.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tla.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kab.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uvv.ehwqpu.com

================================================================================
来源：http://kxa.dashuyun.cn

O. 并发与异步
来源：http://rot.shanyushiyangtech.top

================================================================================
来源：http://oly.epnwcf.com

[O01] 启动一个线程
来源：http://ixu.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sbg.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://glz.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ckh.ivvv.top

TS:   // 同 JS
来源：http://yai.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://tgn.xinyue.icu

Go:   go f()
来源：http://dau.xziqi.cn

Ruby: Thread.new { f }
来源：http://pkj.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://enp.tianlin.xyz

[O02] 使用线程池
来源：http://drw.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tik.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pqf.ybcxt.top

JS:   // worker_threads 线程池
来源：http://iey.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://ljt.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cgs.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xhd.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ber.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://myq.tian-w.cn

[O03] 加锁保护共享数据
来源：http://gyr.aizwys.cn

Py:   with lock: shared += 1
来源：http://pcf.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://fyi.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://irb.yj20258888.top

TS:   // 同 JS
来源：http://kog.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://lkf.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lna.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kqj.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://zwh.redwolf501.top

[O04] 定义异步函数并等待
来源：http://njn.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://mfy.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lnq.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://rir.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jjn.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wsj.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cwg.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://tlu.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://hpv.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://duo.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://pue.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://esq.cheryme.top

JS:   await Promise.all(tasks)
来源：http://xwj.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://elw.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://goo.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kaf.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://aif.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xqi.dianchejie.cn

[O06] 使用进程池
来源：http://icp.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kzk.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ddy.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://osg.316326.xyz

TS:   // child_process / cluster 模块
来源：http://zsd.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://chc.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://emr.cdnleiting.top

Ruby: // fork 块
来源：http://oye.zhongyouzk.top

C#:   Parallel.For
来源：http://glm.sysykeji.top

================================================================================
来源：http://ugj.hnxiangtu.top

P. 常用工具函数
来源：http://tgf.fzhhl.top

================================================================================
来源：http://egd.jyoumei.cn

[P01] 生成 UUID
来源：http://lpr.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://dgq.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mym.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://pgk.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://aji.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://coz.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://sdt.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://fbf.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://bye.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://ftf.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://akp.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zqw.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gbm.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hfa.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iho.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mmh.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qgf.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ary.yangfankeji.com

[P03] 生成短随机字符串
来源：http://jkt.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mog.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rsl.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://acu.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vym.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://osb.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gso.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://onc.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xhj.52xcode.cn

[P04] 求长度
来源：http://sgz.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwm.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uca.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgy.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://otx.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://kmr.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://uhe.tianlin.xyz

Ruby: x.length;  x.size
来源：http://pex.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jls.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://yzg.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ymm.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vdx.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jif.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ghp.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vki.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://grl.jinghuilouyu.cn

Ruby: a == b
来源：http://hmi.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xcl.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dlp.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iyo.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://zqx.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rfj.9152youxi.cn

TS:   if (x == null) {}
来源：http://wav.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://owr.ydzc1.top

Go:   if x == nil {}
来源：http://stx.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzl.zdbjq.cn

C#:   if (x is null) {}
来源：http://ioi.guannengcc.top

[P07] 防抖与节流
来源：http://tic.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ryc.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://dky.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rhp.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcp.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://clx.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ols.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hkp.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qdj.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://nxn.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fad.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qxl.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xuj.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yes.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hau.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://izb.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://riq.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ltc.jiagoushi.top

================================================================================
来源：http://wil.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvn.shanyushiyangkeji.top

================================================================================
来源：http://wdw.yonumen.top

[Q01] 创建表
来源：http://ure.yuanzhike.top

CREATE TABLE users (
来源：http://nql.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dak.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://njr.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://nab.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xqi.zhengqikj.top

);
来源：http://abr.epnwcf.com

[Q02] 创建带外键的表
来源：http://ivj.zhijiandao.cn

CREATE TABLE orders (
来源：http://jif.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://crp.zhengqikj.top

user_id INT NOT NULL,
来源：http://drl.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://vpi.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lle.bjfxy.top

);
来源：http://dna.yvedp.cn

[Q03] 增加列
来源：http://gpc.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zps.hammf.cn

[Q04] 修改列类型
来源：http://ksr.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ojc.zycfv.cn

[Q05] 重命名列
来源：http://ern.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rjw.snrcjt.cn

[Q06] 删除列
来源：http://wkz.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://apv.hnxiangtu.top

[Q07] 删除表
来源：http://wvq.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://ulp.redwolf501.top

[Q08] 创建普通索引
来源：http://bxs.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vmo.yuxming.cn

[Q09] 创建唯一索引
来源：http://jwg.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ake.yvedp.cn

[Q10] 插入单行
来源：http://dlj.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vga.bbcook.cn

[Q11] 一次插入多行
来源：http://gpf.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gfp.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://gbv.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://fta.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ycx.yonumen.top

[Q13] 忽略重复插入
来源：http://vzm.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://abq.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://nxj.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vae.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://olf.hesvh.cn

[Q15] 查询全部
来源：http://sbm.tianlin.xyz

SELECT * FROM users;
来源：http://orb.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://kop.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://elm.gogol.net.cn

[Q17] 条件查询
来源：http://auf.fehbvm.com


<!-- 参考信息 -->