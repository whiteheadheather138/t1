代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ebq.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://oeu.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://zkk.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://udc.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lpl.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://zbt.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://gqx.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fbu.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hls.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://udo.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wwd.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://fka.gotoacloud.top

Ruby: arr.sort
来源：http://pen.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mac.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://lra.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jaw.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://gkf.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tds.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vsg.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zyp.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://psy.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yhy.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://xmy.52xcode.cn

[N04] 斐波那契数列
来源：http://xdu.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://npz.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://krl.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugp.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jro.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jis.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nwq.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://luo.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ilx.guowangkeji.top

[N05] 最大公约数
来源：http://ara.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://hsx.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://llm.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpn.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gnc.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://feq.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hbb.birdmap.top

Ruby: a.gcd(b)
来源：http://aoh.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wzy.guowangkeji.top

[N06] 判断回文字符串
来源：http://kun.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://ijz.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://kcv.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://jet.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://olh.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vrw.xuanzx.com

Go:   // 双指针从两端比较
来源：http://zfi.cheryme.top

Ruby: s == s.reverse
来源：http://cfk.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lxq.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://dmq.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hsb.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zxu.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tbk.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://yqw.guannengcc.top

Java: // 手写 HashMap
来源：http://sob.tian-w.cn

Go:   // 手写 map[int]int
来源：http://hnd.cashguo.top

Ruby: // 手写 Hash
来源：http://ufc.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://aho.aizwys.cn

[N08] 生成全排列
来源：http://swv.hammf.cn

Py:   itertools.permutations(arr)
来源：http://azv.zycfv.cn

PHP:  // 手写递归交换
来源：http://ask.fengsongda.top

JS:   // 手写回溯递归
来源：http://nkk.yuanzhike.top

TS:   // 手写回溯递归
来源：http://jua.zhongyouzk.top

Java: // 手写回溯递归
来源：http://qsq.sweek.top

Go:   // 手写回溯递归
来源：http://qod.cheryme.top

Ruby: arr.permutation.to_a
来源：http://wpv.andypj.xyz

C#:   // 手写回溯递归
来源：http://dnb.yangfankeji.com

[N09] 栈与队列
来源：http://hdx.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sve.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ihu.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ftl.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ymx.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zsr.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iex.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ttk.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lpp.zhijiandao.cn

[N10] 链表节点定义
来源：http://pmp.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uoc.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xso.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rtc.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://onq.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://zuv.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://whj.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vwn.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gpx.nwbrower.top

[N11] 二叉树中序遍历
来源：http://gfj.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szv.zdqjudy.top

PHP:  // 手写递归函数
来源：http://xbv.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytx.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ewv.aibaodan.cn

Java: // 手写递归
来源：http://cmb.ybcxt.top

Go:   // 手写递归
来源：http://jvm.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://glg.gogol.net.cn

C#:   // 手写递归
来源：http://clk.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://khj.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qxv.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uyj.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ywb.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtk.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rtu.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axm.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://brj.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mlg.wangshuangyany.cn

================================================================================
来源：http://tlh.zdqjudy.top

O. 并发与异步
来源：http://zbp.fktsv.cn

================================================================================
来源：http://zep.zhongyouzk.top

[O01] 启动一个线程
来源：http://nrb.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ivh.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://upy.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wum.hammf.cn

TS:   // 同 JS
来源：http://qkb.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://zhw.zhiwuduotai.top

Go:   go f()
来源：http://xgm.chenlongwang.top

Ruby: Thread.new { f }
来源：http://ucb.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://qjf.feifeiyinyue.top

[O02] 使用线程池
来源：http://bmj.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gvs.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bqm.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://qzf.cucudq.cn

TS:   // worker_threads 线程池
来源：http://otb.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://mpd.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tcp.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://abs.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://beu.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://bgf.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://xqt.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://eax.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vex.0kj1m.cn

TS:   // 同 JS
来源：http://pnl.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://rvz.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yko.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kis.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://lap.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://psj.uphjek.com

Py:   async def f():⏎    await g()
来源：http://kuy.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zkg.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://zgz.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dpq.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wgg.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xwf.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://qxf.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://zud.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://kxt.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://zpm.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ocg.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://kyv.yj20258.top

TS:   await Promise.all(tasks)
来源：http://uug.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ims.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xfl.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://gnn.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gzq.zdbjq.cn

[O06] 使用进程池
来源：http://coz.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iew.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mlg.sweek.top

JS:   // child_process / cluster 模块
来源：http://zpg.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://tth.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qma.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vhn.yongpay.top

Ruby: // fork 块
来源：http://yco.jqgfzy.top

C#:   Parallel.For
来源：http://yut.tarul.cn

================================================================================
来源：http://fmq.wangdashe.top

P. 常用工具函数
来源：http://qnc.yuanzhike.top

================================================================================
来源：http://xua.cheryme.top

[P01] 生成 UUID
来源：http://mbs.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://qvv.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bgi.mhx1999.top

JS:   crypto.randomUUID()
来源：http://utp.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://zyc.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://jnj.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://dke.tarul.cn

Ruby: SecureRandom.uuid
来源：http://oxi.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://fbt.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://mhw.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jxe.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tgw.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zot.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dti.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nui.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gpk.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bfl.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tgs.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://kpz.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pvv.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxt.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hkf.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flt.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ljk.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hfs.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dxe.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://znm.zycfv.cn

[P04] 求长度
来源：http://typ.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://abf.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dec.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kii.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ksx.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://afs.cheryme.top

Go:   len(arr);  len(m)
来源：http://yjy.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://oco.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dlr.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://tar.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tfe.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nwp.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yxb.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iyb.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmh.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jkl.nanxuanxn.top

Ruby: a == b
来源：http://snt.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zhf.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iqi.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ikk.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://zik.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://skc.mhx1999.top

TS:   if (x == null) {}
来源：http://ley.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dem.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://iiz.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oax.xinyue.icu

C#:   if (x is null) {}
来源：http://fdo.mhx1999.top

[P07] 防抖与节流
来源：http://qwe.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hes.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://dyu.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifj.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgt.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://acy.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aaq.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hta.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://voc.daria6918.cn

[P08] 处理浮点精度问题
来源：http://vej.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://flm.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nyn.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vhc.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sfd.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hqu.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sjn.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bxp.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://utx.aibaodan.cn

================================================================================
来源：http://qzp.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wfv.nanxinkj.top

================================================================================
来源：http://zoc.uphjek.com

[Q01] 创建表
来源：http://scc.zdqjudy.top

CREATE TABLE users (
来源：http://bli.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blo.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://jke.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://gty.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://exc.gzhubu.top

);
来源：http://log.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://str.yangfankeji.com

CREATE TABLE orders (
来源：http://nud.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kty.smart0.xyz

user_id INT NOT NULL,
来源：http://nbm.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://okf.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ofz.jyoumei.cn

);
来源：http://oqw.cdnleiting.top

[Q03] 增加列
来源：http://qvd.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://apr.chenjidiqi.icu

[Q04] 修改列类型
来源：http://krx.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://era.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://dhn.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vhw.hfpthk.cn

[Q06] 删除列
来源：http://yoo.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://has.jyoumei.cn

[Q07] 删除表
来源：http://vkf.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://cjl.iojbl.cn

[Q08] 创建普通索引
来源：http://tsx.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://koq.hfpthk.cn

[Q09] 创建唯一索引
来源：http://cgv.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xiq.jinghuilouyu.cn

[Q10] 插入单行
来源：http://wmg.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ewh.xinyue.icu

[Q11] 一次插入多行
来源：http://ubx.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cvt.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://hrj.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ors.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zda.birdmap.top

[Q13] 忽略重复插入
来源：http://ntu.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qnv.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://whc.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cjy.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bag.yuanzhike.top

[Q15] 查询全部
来源：http://dpw.gaohongyu789.top

SELECT * FROM users;
来源：http://vpt.sysykeji.top

[Q16] 查询指定列
来源：http://hgx.yj20258.top

SELECT id, name FROM users;
来源：http://cli.ctjpmb.com

[Q17] 条件查询
来源：http://jwm.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://odk.bbcook.cn

[Q18] 模糊匹配
来源：http://dhj.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ayv.jqgufenzy.top

[Q19] 范围查询
来源：http://ujn.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pgn.jinqigufen.top

[Q20] IN 列表
来源：http://zwq.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pos.meibo888.top

[Q21] 空值判断
来源：http://krp.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bdt.gaohongyu789.top

[Q22] 排序
来源：http://zgj.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gis.zhengqikj.top

[Q23] 分页
来源：http://nfw.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wml.zdbjq.cn

[Q24] 去重
来源：http://xhp.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://orw.bjfxy.top

[Q25] 只取前 N 条
来源：http://yix.shuidangran.top


<!-- 参考信息 -->