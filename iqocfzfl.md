代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://nmg.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oxx.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lum.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://tqm.fanxiaobao.xyz

Ruby: arr.sort
来源：http://esr.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hkc.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://yfe.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ofo.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://yqj.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ujx.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://awl.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xis.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zoy.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntt.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hjz.cashguo.top

[N04] 斐波那契数列
来源：http://rkf.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hgr.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://art.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nes.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhw.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://okt.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xwz.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cdk.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cmw.smart0.xyz

[N05] 最大公约数
来源：http://zcm.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://ywc.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gye.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibg.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vag.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hkw.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ldj.guannengcc.top

Ruby: a.gcd(b)
来源：http://svx.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tzu.ydzc1.top

[N06] 判断回文字符串
来源：http://xlq.yonumen.top

Py:   s == s[::-1]
来源：http://rqj.yvedp.cn

PHP:  $s === strrev($s);
来源：http://zmd.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://xqk.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://coo.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rdt.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://vpv.yongpay.top

Ruby: s == s.reverse
来源：http://fpq.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hlm.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://fhl.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://duv.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gbk.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://grh.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://fdx.birdmap.top

Java: // 手写 HashMap
来源：http://ivs.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://eal.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://abs.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://crm.ctjpmb.com

[N08] 生成全排列
来源：http://lkn.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://ktv.yuxming.cn

PHP:  // 手写递归交换
来源：http://bly.hcnkem.com

JS:   // 手写回溯递归
来源：http://taq.gzhubu.top

TS:   // 手写回溯递归
来源：http://jyv.9152youxi.cn

Java: // 手写回溯递归
来源：http://xfx.xinyue.icu

Go:   // 手写回溯递归
来源：http://mvq.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://ufg.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://mot.jinqigufen.top

[N09] 栈与队列
来源：http://qap.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://loq.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yma.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lce.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ovd.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mrp.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bkg.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xmw.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xvd.jinqigfzy.top

[N10] 链表节点定义
来源：http://hur.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qyl.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nra.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxc.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://opx.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://qrr.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kjz.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zsa.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rxr.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://hgu.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xjf.sweek.top

PHP:  // 手写递归函数
来源：http://dwj.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rzm.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hco.gaohongyu789.top

Java: // 手写递归
来源：http://esv.cashguo.top

Go:   // 手写递归
来源：http://lgv.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ink.yangfankeji.com

C#:   // 手写递归
来源：http://zit.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wql.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fkr.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yzp.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://naz.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lxf.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pda.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jwf.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fuh.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dgc.tianlin.xyz

================================================================================
来源：http://naa.zhengqikj.top

O. 并发与异步
来源：http://eak.shanyushiyangkeji.top

================================================================================
来源：http://yym.zhixingplan.top

[O01] 启动一个线程
来源：http://dpr.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oil.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ryz.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xop.jianghu66.top

TS:   // 同 JS
来源：http://euj.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://xhm.fzhhl.top

Go:   go f()
来源：http://rbp.snrcjt.cn

Ruby: Thread.new { f }
来源：http://pna.wangdashe.top

C#:   Task.Run(() => F());
来源：http://uag.kuanghao11.cn

[O02] 使用线程池
来源：http://heo.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jrg.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fax.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://qkm.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://jkv.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://beb.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qdo.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ter.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lbw.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://ydr.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://qqe.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://epf.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://noi.316326.xyz

TS:   // 同 JS
来源：http://exj.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://cux.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uxu.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wis.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://ltu.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://bxw.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://fyo.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://shb.cashguo.top

JS:   async function f() { await g(); }
来源：http://iqj.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://avv.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://opj.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jfw.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mnl.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://zxd.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://olm.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://ddx.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttf.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://vql.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://gdo.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mef.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wur.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://dkg.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://syy.hnqzz.top

[O06] 使用进程池
来源：http://wbm.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://irk.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ino.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://eqn.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://cdx.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vty.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yrr.chenjidiqi.icu

Ruby: // fork 块
来源：http://pkw.sxryk.cn

C#:   Parallel.For
来源：http://pri.fktsv.cn

================================================================================
来源：http://ump.zhengqikj.top

P. 常用工具函数
来源：http://gnr.xziqi.cn

================================================================================
来源：http://ytc.vqdsnc.cn

[P01] 生成 UUID
来源：http://cyz.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://xfp.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ocn.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://dul.cashguo.top

TS:   crypto.randomUUID()
来源：http://mop.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://yom.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://ekr.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://qyw.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://glv.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://qdk.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sof.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tfk.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umv.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgt.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xku.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dgp.pycfn.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hou.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pic.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://ehj.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hqc.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhn.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://smh.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwm.ppjwa.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lhb.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wvf.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpz.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dqc.zhengqikj.top

[P04] 求长度
来源：http://grz.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vul.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jya.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xge.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jvn.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://lpz.cucudq.cn

Go:   len(arr);  len(m)
来源：http://gpx.zhengqikj.top

Ruby: x.length;  x.size
来源：http://tho.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://omj.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://cjj.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sio.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jzg.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jzi.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dsw.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pnr.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ski.xingfuxueyuan.xyz

Ruby: a == b
来源：http://ukq.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ffj.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jyx.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sdt.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://pqu.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wnv.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://tsc.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zoy.sxryk.cn

Go:   if x == nil {}
来源：http://urc.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://olj.svipenyu.cn

C#:   if (x is null) {}
来源：http://icx.bjfxy.top

[P07] 防抖与节流
来源：http://juj.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://faz.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://qvs.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofl.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kht.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uco.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hml.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kbd.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mxw.vehdjk.com

[P08] 处理浮点精度问题
来源：http://yua.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xri.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pll.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://guq.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lxa.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aox.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dsv.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kkg.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://occ.jlsjyb.cn

================================================================================
来源：http://ove.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sao.ydjk.org.cn

================================================================================
来源：http://mme.daxiang520.top

[Q01] 创建表
来源：http://wjf.quarkkingdee.top

CREATE TABLE users (
来源：http://udj.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uak.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://oqx.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://abr.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hcn.tanke756.top

);
来源：http://org.yonumen.top

[Q02] 创建带外键的表
来源：http://hld.smart0.xyz

CREATE TABLE orders (
来源：http://oyi.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abm.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://wll.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://jbg.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tgs.zhengqikj.top

);
来源：http://ucq.havefunace.top

[Q03] 增加列
来源：http://aqq.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://foc.xziqi.cn

[Q04] 修改列类型
来源：http://izz.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kkw.zycfv.cn

[Q05] 重命名列
来源：http://bjp.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yjo.jinqigfzy.top

[Q06] 删除列
来源：http://jng.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rqp.tanke756.top

[Q07] 删除表
来源：http://rwd.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://eiy.xylfe.cn

[Q08] 创建普通索引
来源：http://zvu.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pfg.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://iis.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nww.iojbl.cn

[Q10] 插入单行
来源：http://vcd.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zin.fehbvm.com

[Q11] 一次插入多行
来源：http://qak.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hzn.cheryme.top

[Q12] 插入后取自增 ID
来源：http://wcw.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://odh.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zyr.hesvh.cn

[Q13] 忽略重复插入
来源：http://gva.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pfa.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://mlj.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jan.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bkf.snrcjt.cn

[Q15] 查询全部
来源：http://zzh.xylfe.cn

SELECT * FROM users;
来源：http://fjp.ivvv.top

[Q16] 查询指定列
来源：http://ajo.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://fcs.fzhhl.top

[Q17] 条件查询
来源：http://sug.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ntr.vqdsnc.cn

[Q18] 模糊匹配
来源：http://nol.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ztj.shzxlz.cn

[Q19] 范围查询
来源：http://rtr.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://heo.jiagoushi.top

[Q20] IN 列表
来源：http://gye.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vbl.ehwqpu.com

[Q21] 空值判断
来源：http://rca.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://efb.ehwqpu.com

[Q22] 排序
来源：http://nrd.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kqm.yangfankeji.com

[Q23] 分页
来源：http://hap.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tsv.shangyingyoupin.top

[Q24] 去重
来源：http://lxj.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://gnw.dashuyun.cn

[Q25] 只取前 N 条
来源：http://bdl.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cmq.zhongyouzk.top

[Q26] 计数
来源：http://kms.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://pyl.yj202588.top

[Q27] 条件计数
来源：http://lon.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bst.52xcode.cn

[Q28] 求和与平均
来源：http://mni.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uzv.jinqigfzy.top

[Q29] 最大最小值
来源：http://tiq.zhiwuduotai.top


<!-- 参考信息 -->