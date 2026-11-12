代发 wailian999

Ruby: arr.sort
来源：http://eqm.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ynz.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://syo.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmh.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://xks.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qeu.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfy.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jnj.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nah.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvm.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://phj.aibaodan.cn

[N04] 斐波那契数列
来源：http://iiv.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rnq.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dah.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jsr.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aff.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lkw.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://idj.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fhe.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jid.hongshengwenyu.top

[N05] 最大公约数
来源：http://pyw.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://led.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://efj.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bwj.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hor.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hrh.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tjt.ivvv.top

Ruby: a.gcd(b)
来源：http://twl.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mlu.yongpay.top

[N06] 判断回文字符串
来源：http://nja.yj20258888.top

Py:   s == s[::-1]
来源：http://ata.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://dzt.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://qop.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://noy.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kwo.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://tbp.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://rxx.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://umg.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://hfx.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ttp.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uoj.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hoh.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://lyb.daria6918.cn

Java: // 手写 HashMap
来源：http://smr.52xcode.cn

Go:   // 手写 map[int]int
来源：http://zcg.ehwqpu.com

Ruby: // 手写 Hash
来源：http://nzb.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gfg.xinyue.icu

[N08] 生成全排列
来源：http://qdd.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://vmx.tianlin.xyz

PHP:  // 手写递归交换
来源：http://yit.hammf.cn

JS:   // 手写回溯递归
来源：http://eqw.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://sap.xylfe.cn

Java: // 手写回溯递归
来源：http://jui.guannengcc.top

Go:   // 手写回溯递归
来源：http://myy.sweek.top

Ruby: arr.permutation.to_a
来源：http://skw.hnqzz.top

C#:   // 手写回溯递归
来源：http://uck.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://fps.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kkn.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://btj.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xlx.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://okz.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://set.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sdq.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://paz.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hwf.redwolf501.top

[N10] 链表节点定义
来源：http://fvc.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vju.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ohg.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qxo.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ebw.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://fcx.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://kcq.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vcx.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://yta.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://pwh.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dgg.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://loi.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikk.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tic.svipenyu.cn

Java: // 手写递归
来源：http://tge.aizwys.cn

Go:   // 手写递归
来源：http://vln.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dkd.zhongyouzk.top

C#:   // 手写递归
来源：http://bnn.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jfl.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://umt.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dqp.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qoi.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dro.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lxb.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://voj.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ohu.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lfj.jiagoushi.top

================================================================================
来源：http://zok.nwbrower.top

O. 并发与异步
来源：http://fqy.vqdsnc.cn

================================================================================
来源：http://khk.xinyue.icu

[O01] 启动一个线程
来源：http://wkc.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cma.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rxj.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxm.nanxuanxn.top

TS:   // 同 JS
来源：http://mdy.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://hkc.aibaodan.cn

Go:   go f()
来源：http://xjw.ivvv.top

Ruby: Thread.new { f }
来源：http://mqi.epnwcf.com

C#:   Task.Run(() => F());
来源：http://yaq.fzhhl.top

[O02] 使用线程池
来源：http://keg.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ban.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gib.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://pqj.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://zqp.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://qri.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bdx.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ypi.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sod.sysykeji.top

[O03] 加锁保护共享数据
来源：http://kyt.hnqzz.top

Py:   with lock: shared += 1
来源：http://fwz.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://wjm.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://raj.gaohongyu789.top

TS:   // 同 JS
来源：http://olc.sweek.top

Java: synchronized (this) { shared++; }
来源：http://etv.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://skr.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://eqe.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://yuq.andypj.xyz

[O04] 定义异步函数并等待
来源：http://yvm.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://jah.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lwb.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://jwa.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://vlo.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xzb.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iiw.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gnn.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://ocu.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://zib.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://kbx.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ecd.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://ckt.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://hpg.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vvk.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mdl.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://rkx.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dtg.svipenyu.cn

[O06] 使用进程池
来源：http://yvy.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://inj.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bij.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://vfu.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://qgd.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zmz.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mtl.ydzc1.top

Ruby: // fork 块
来源：http://cey.feifeiyinyue.top

C#:   Parallel.For
来源：http://obf.sufxvd.cn

================================================================================
来源：http://aor.xuetiantiany.cn

P. 常用工具函数
来源：http://xep.316326.xyz

================================================================================
来源：http://pfr.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://ejq.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://xwr.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qlo.ivvv.top

JS:   crypto.randomUUID()
来源：http://cph.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://hhw.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://vtk.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://ntc.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://qxn.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://mnt.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://trf.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tco.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uzn.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eso.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aem.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wnj.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://klh.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pot.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wwm.cucudq.cn

[P03] 生成短随机字符串
来源：http://hbb.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bcg.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xzc.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qmo.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyz.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pmu.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ucx.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kvu.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uek.jlsjyb.cn

[P04] 求长度
来源：http://gwl.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mmw.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jkb.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgd.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihw.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://imh.hcnkem.com

Go:   len(arr);  len(m)
来源：http://kxe.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://ucg.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pqd.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://eni.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dcf.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yhb.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uxo.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ggf.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jjn.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://squ.xuanzx.com

Ruby: a == b
来源：http://mkm.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ztb.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ifa.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://htv.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://daq.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xzx.cashguo.top

TS:   if (x == null) {}
来源：http://ibk.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uvq.hysaishi.cn

Go:   if x == nil {}
来源：http://fkd.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ste.tarul.cn

C#:   if (x is null) {}
来源：http://xkg.tianlin.xyz

[P07] 防抖与节流
来源：http://zhd.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iwv.pycfn.com

PHP:  // 手写时间戳比较
来源：http://njy.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://osn.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twb.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://awe.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ngi.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pct.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cxu.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://yoa.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mbk.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://myb.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://obz.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ryu.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lsc.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fov.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://umr.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hea.ehwqpu.com

================================================================================
来源：http://mpq.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xef.yanxiufei.cn

================================================================================
来源：http://diz.yueranfly.top

[Q01] 创建表
来源：http://dpi.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://ucu.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rov.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://urd.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://mnf.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://apv.fanxiaobao.xyz

);
来源：http://wpd.tian-w.cn

[Q02] 创建带外键的表
来源：http://ows.yvedp.cn

CREATE TABLE orders (
来源：http://bxw.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmd.shuidangran.top

user_id INT NOT NULL,
来源：http://sbu.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://ndu.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yaj.yfazqb.com

);
来源：http://ssd.gzhubu.top

[Q03] 增加列
来源：http://qbp.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wnd.ydzc1.top

[Q04] 修改列类型
来源：http://ijs.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fdw.vqdsnc.cn

[Q05] 重命名列
来源：http://xef.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nmt.zhijiandao.cn

[Q06] 删除列
来源：http://pzw.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://hzq.andypj.xyz

[Q07] 删除表
来源：http://qyq.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://zfj.fengsongda.top

[Q08] 创建普通索引
来源：http://pxj.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fic.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://gah.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gwm.c1oappe.top

[Q10] 插入单行
来源：http://xta.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fvu.vehdjk.com

[Q11] 一次插入多行
来源：http://otj.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vbo.tarul.cn

[Q12] 插入后取自增 ID
来源：http://cxq.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://brk.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fab.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://nll.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cri.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://agf.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mdp.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rum.shzxlz.cn

[Q15] 查询全部
来源：http://weq.xinyue.icu

SELECT * FROM users;
来源：http://oze.hysaishi.cn

[Q16] 查询指定列
来源：http://hpt.0kj1m.cn

SELECT id, name FROM users;
来源：http://kuh.gotoacloud.top

[Q17] 条件查询
来源：http://ygg.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fwu.nanxuanxn.top

[Q18] 模糊匹配
来源：http://hqu.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mir.jiagoushi.top

[Q19] 范围查询
来源：http://vgg.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cxr.dashuyun.cn

[Q20] IN 列表
来源：http://wmw.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://enx.jinqigfzy.top

[Q21] 空值判断
来源：http://qhp.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hds.wangshuangyany.cn

[Q22] 排序
来源：http://yqq.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cru.meibo888.top

[Q23] 分页
来源：http://icq.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gyv.aizwys.cn

[Q24] 去重
来源：http://wzl.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://tfp.cheryme.top

[Q25] 只取前 N 条
来源：http://syi.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hbh.jinqigufen.top

[Q26] 计数
来源：http://yyi.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://ydj.sufxvd.cn

[Q27] 条件计数
来源：http://pfd.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kha.jlsjyb.cn

[Q28] 求和与平均
来源：http://rpg.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://now.tanke756.top

[Q29] 最大最小值
来源：http://izb.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dbs.chenzaomai.com

[Q30] 分组统计
来源：http://sup.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hrn.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://chg.epnwcf.com


<!-- 参考信息 -->