代发 wailian999

[N01] 二分查找（有序数组）
来源：http://nvb.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://svn.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jal.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wjs.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mjp.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uwh.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://kix.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://idu.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://nft.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://fdf.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kew.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ika.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rpu.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://izm.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cog.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://edi.nwbrower.top

Ruby: arr.sort
来源：http://hpk.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://eld.yongpay.top

[N03] 快速排序（分治示例）
来源：http://lux.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tda.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://myn.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgb.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hlg.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jgy.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hzy.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://olk.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ybu.zdqjudy.top

[N04] 斐波那契数列
来源：http://grq.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://emq.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mbt.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abx.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wcg.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ccz.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sip.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jft.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pxw.svipenyu.cn

[N05] 最大公约数
来源：http://fmq.52xcode.cn

Py:   math.gcd(a, b)
来源：http://pih.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lhu.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://skc.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vyz.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ykx.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uoe.ybcxt.top

Ruby: a.gcd(b)
来源：http://lac.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ttu.mhx1999.top

[N06] 判断回文字符串
来源：http://mjn.fehbvm.com

Py:   s == s[::-1]
来源：http://sjt.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://kwq.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://hpl.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://bdi.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tvf.hesvh.cn

Go:   // 双指针从两端比较
来源：http://dbe.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://cyx.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://smh.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://fwt.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bxs.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nec.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xgj.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://mru.gzhubu.top

Java: // 手写 HashMap
来源：http://pvz.meibo888.top

Go:   // 手写 map[int]int
来源：http://gaa.ctjpmb.com

Ruby: // 手写 Hash
来源：http://plk.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://pdu.meibo888.top

[N08] 生成全排列
来源：http://qde.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://lql.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://hwf.guannengcc.top

JS:   // 手写回溯递归
来源：http://eds.fengsongda.top

TS:   // 手写回溯递归
来源：http://drt.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://jxj.ybcxt.top

Go:   // 手写回溯递归
来源：http://wft.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://vdz.havefunace.top

C#:   // 手写回溯递归
来源：http://qdt.epnwcf.com

[N09] 栈与队列
来源：http://epx.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://myr.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aql.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ujr.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nkh.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hla.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nts.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cid.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qpi.316326.xyz

[N10] 链表节点定义
来源：http://cha.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cju.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rex.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ffi.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pie.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://ikn.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://tvu.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rdl.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kbv.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://wrk.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wxw.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://qfz.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrs.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xuz.iojbl.cn

Java: // 手写递归
来源：http://tlr.jinqigufen.top

Go:   // 手写递归
来源：http://kwj.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zqh.havefunace.top

C#:   // 手写递归
来源：http://euh.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qhb.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kan.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uxh.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qsy.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfz.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mdu.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qko.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yco.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xms.shangyingyoupin.top

================================================================================
来源：http://ipw.tian-w.cn

O. 并发与异步
来源：http://yng.xylfe.cn

================================================================================
来源：http://fvk.ehwqpu.com

[O01] 启动一个线程
来源：http://adv.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qzp.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ftk.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://smg.nanxuanxn.top

TS:   // 同 JS
来源：http://ccf.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://ibw.zhixingplan.top

Go:   go f()
来源：http://kqz.cucudq.cn

Ruby: Thread.new { f }
来源：http://lyq.jianghu66.top

C#:   Task.Run(() => F());
来源：http://frn.pycfn.com

[O02] 使用线程池
来源：http://kwv.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcs.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sys.redwolf501.top

JS:   // worker_threads 线程池
来源：http://tsp.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://pob.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://kkq.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpk.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jis.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mkr.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://ihl.9152youxi.cn

Py:   with lock: shared += 1
来源：http://oyw.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://nwo.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrw.pengpengdd.cyou

TS:   // 同 JS
来源：http://mym.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://dbq.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nnk.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xbt.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://aud.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://uws.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://kmx.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rho.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://nsz.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xiy.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zyh.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vmn.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uhz.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://zng.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://bie.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://zsk.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lug.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://qla.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://iqz.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gre.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jcd.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://ijq.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xvr.dianchejie.cn

[O06] 使用进程池
来源：http://tcj.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iew.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dtz.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://spr.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://rsw.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hly.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kzq.yfazqb.com

Ruby: // fork 块
来源：http://fai.snrcjt.cn

C#:   Parallel.For
来源：http://usk.fehbvm.com

================================================================================
来源：http://cst.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://jwi.sjlbkw.cn

================================================================================
来源：http://mbb.zhixingplan.top

[P01] 生成 UUID
来源：http://cih.cheryme.top

Py:   str(uuid.uuid4())
来源：http://hgz.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://knn.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://pgk.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://qjz.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://xje.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://huj.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://nbk.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://afy.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://hvs.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ytm.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yul.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lpq.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gan.aizwys.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xjh.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nyb.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mwn.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wmz.52xcode.cn

[P03] 生成短随机字符串
来源：http://fqz.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://apu.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mba.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jnr.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fmp.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://stp.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://glf.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yzu.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yud.yueranfly.top

[P04] 求长度
来源：http://hdm.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mrq.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hga.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jex.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mqy.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://bpb.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://ynb.gotoacloud.top

Ruby: x.length;  x.size
来源：http://fgh.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jii.quarkkingdee.top

[P05] 判断两个对象内容是否相等
来源：http://mnw.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cnn.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ekw.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://npf.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xvi.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://clk.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yxn.gogol.net.cn

Ruby: a == b
来源：http://jbd.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://miu.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tjg.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hfk.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://svw.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cik.guannengcc.top

TS:   if (x == null) {}
来源：http://zfs.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dmi.snrcjt.cn

Go:   if x == nil {}
来源：http://nuj.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ruz.cashguo.top

C#:   if (x is null) {}
来源：http://kad.nanxuanxn.top

[P07] 防抖与节流
来源：http://ndr.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vhx.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://rgn.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uza.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rkv.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://phs.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yeg.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xln.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://phk.ydzc1.top

[P08] 处理浮点精度问题
来源：http://nni.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gev.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jcd.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lji.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lph.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kyy.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ugv.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qlc.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://auo.yj20258.top

================================================================================
来源：http://bue.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivf.svipenyu.cn

================================================================================
来源：http://sxr.jinyuanbaomall.cn

[Q01] 创建表
来源：http://pfp.epnwcf.com

CREATE TABLE users (
来源：http://ter.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mwa.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://cdw.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://vgi.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://llc.sufxvd.cn

);
来源：http://aqi.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://gnq.jqgufenzy.top

CREATE TABLE orders (
来源：http://qga.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjd.yj20258.top

user_id INT NOT NULL,
来源：http://abh.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://ovf.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://slx.hywenlv.cn

);
来源：http://nup.jinqigfzy.top

[Q03] 增加列
来源：http://wxh.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ruy.meibo888.top

[Q04] 修改列类型
来源：http://nui.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rke.jyoumei.cn

[Q05] 重命名列
来源：http://bkj.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qzp.sysykeji.top

[Q06] 删除列
来源：http://mjz.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://qtu.hnqzz.top

[Q07] 删除表
来源：http://vag.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://kdg.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://awf.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kun.birdmap.top

[Q09] 创建唯一索引
来源：http://vko.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://odt.hongshengwenyu.top

[Q10] 插入单行
来源：http://tia.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xaf.yueranfly.top

[Q11] 一次插入多行
来源：http://btr.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kvr.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://gji.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://zrl.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://erm.dashuyun.cn

[Q13] 忽略重复插入
来源：http://trl.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zjr.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://yrg.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xpq.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://orc.xziqi.cn

[Q15] 查询全部
来源：http://kgz.pycfn.com

SELECT * FROM users;
来源：http://egd.xinyue.icu

[Q16] 查询指定列
来源：http://jvh.wangdashe.top

SELECT id, name FROM users;
来源：http://lcw.ydzc1.top

[Q17] 条件查询
来源：http://gem.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xzg.ctjpmb.com

[Q18] 模糊匹配
来源：http://mii.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfh.birdmap.top

[Q19] 范围查询
来源：http://pnu.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xgi.svipenyu.cn

[Q20] IN 列表
来源：http://bdm.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xmk.hammf.cn

[Q21] 空值判断
来源：http://foo.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bwi.nwbrower.top

[Q22] 排序
来源：http://tyl.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://isf.zhaomingkeji.xyz

[Q23] 分页
来源：http://rbc.tianlin.xyz


<!-- 参考信息 -->