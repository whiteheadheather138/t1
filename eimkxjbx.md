代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://nks.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvj.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqp.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lxw.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzo.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ysw.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://naw.redwolf501.top

[N04] 斐波那契数列
来源：http://qfy.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fme.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ine.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mme.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ytj.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gbl.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://itl.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://unp.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://srv.aibaodan.cn

[N05] 最大公约数
来源：http://jdl.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://ryk.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pyg.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dhv.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scz.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xcv.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sab.bbcook.cn

Ruby: a.gcd(b)
来源：http://qnt.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sui.jinqigfzy.top

[N06] 判断回文字符串
来源：http://yon.xziqi.cn

Py:   s == s[::-1]
来源：http://tum.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://vio.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://yeq.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://fgn.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wki.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://fol.vehdjk.com

Ruby: s == s.reverse
来源：http://zds.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sam.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://nvp.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wja.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mxi.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://lfu.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://rhs.dianchejie.cn

Java: // 手写 HashMap
来源：http://vnj.52xcode.cn

Go:   // 手写 map[int]int
来源：http://cfz.yfazqb.com

Ruby: // 手写 Hash
来源：http://sfi.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://qxe.zhijiandao.cn

[N08] 生成全排列
来源：http://see.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://ena.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://amx.wangdashe.top

JS:   // 手写回溯递归
来源：http://sol.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://hll.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://xmk.yfazqb.com

Go:   // 手写回溯递归
来源：http://rpx.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://xpq.fehbvm.com

C#:   // 手写回溯递归
来源：http://cfc.quarkkingdee.top

[N09] 栈与队列
来源：http://ihd.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nmi.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mny.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://guh.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hkd.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pyv.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xrp.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ceu.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdb.cqqwz.cn

[N10] 链表节点定义
来源：http://sgx.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eha.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kcb.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mvm.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dzy.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://wlg.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://wof.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ezo.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ich.gzhubu.top

[N11] 二叉树中序遍历
来源：http://oys.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ltn.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://cao.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhg.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tme.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://xss.fzhhl.top

Go:   // 手写递归
来源：http://npn.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ixr.zdbjq.cn

C#:   // 手写递归
来源：http://fdc.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://igm.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zwu.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vkd.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xhk.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eiv.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tft.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bgy.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pef.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wxz.jlsjyb.cn

================================================================================
来源：http://snx.quarkkingdee.top

O. 并发与异步
来源：http://tcp.hnqzz.top

================================================================================
来源：http://pgu.jqgfzy.top

[O01] 启动一个线程
来源：http://ozm.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gge.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pim.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qrp.tian-w.cn

TS:   // 同 JS
来源：http://xqe.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://idq.nwbrower.top

Go:   go f()
来源：http://stg.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://lzk.ivvv.top

C#:   Task.Run(() => F());
来源：http://snk.yuxming.cn

[O02] 使用线程池
来源：http://mju.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlu.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tjh.fehbvm.com

JS:   // worker_threads 线程池
来源：http://vci.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://ttq.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pwx.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://edg.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yif.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pcf.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://npk.ivvv.top

Py:   with lock: shared += 1
来源：http://wqa.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://dkv.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lhw.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://kwp.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://qyq.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://npb.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghh.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://uky.epnwcf.com

[O04] 定义异步函数并等待
来源：http://ady.cashguo.top

Py:   async def f():⏎    await g()
来源：http://uum.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vcq.xinyue.icu

JS:   async function f() { await g(); }
来源：http://zcd.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://jue.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zqd.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lzi.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pzs.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://mmv.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://smg.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://zwj.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gyt.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://icq.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://gld.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hfu.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lke.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://kya.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xjo.nanxinkj.top

[O06] 使用进程池
来源：http://mjn.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tdv.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aob.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://pow.cashguo.top

TS:   // child_process / cluster 模块
来源：http://yej.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fzq.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lkw.jianghu66.top

Ruby: // fork 块
来源：http://ikf.chenlongwang.top

C#:   Parallel.For
来源：http://eiq.nwbrower.top

================================================================================
来源：http://tqp.tianlin.xyz

P. 常用工具函数
来源：http://emd.wangshuangyany.cn

================================================================================
来源：http://pbq.ybcxt.top

[P01] 生成 UUID
来源：http://jtv.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://ven.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ilg.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://pjq.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://egu.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://zhj.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ywd.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://vsk.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://tkd.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://ovp.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nez.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://qbu.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fyd.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kis.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://icr.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bnb.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nzu.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uao.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://kte.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kac.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://axt.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://slk.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqh.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pqd.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wrp.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://efq.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fnf.xinyue.icu

[P04] 求长度
来源：http://coa.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mfg.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gqw.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kcs.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hqf.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://xkd.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://vmc.yangfankeji.com

Ruby: x.length;  x.size
来源：http://sha.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pyd.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://tto.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ono.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bnd.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ldz.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wgc.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://utv.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://zdx.shangyingyoupin.top

Ruby: a == b
来源：http://vnq.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lse.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yhu.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kfn.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://urj.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vme.9152youxi.cn

TS:   if (x == null) {}
来源：http://zkl.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lpt.tianlin.xyz

Go:   if x == nil {}
来源：http://key.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fmz.cucudq.cn

C#:   if (x is null) {}
来源：http://ikp.zhoulong.xyz

[P07] 防抖与节流
来源：http://wpa.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nwy.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://jfk.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://drc.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wdi.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://edd.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rlr.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tyv.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tga.yvedp.cn

[P08] 处理浮点精度问题
来源：http://lyn.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nnv.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hfk.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxn.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zkb.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rxx.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hlf.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xfe.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://btj.jiagoushi.top

================================================================================
来源：http://ggs.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pyt.daxiang520.top

================================================================================
来源：http://pxu.xziqi.cn

[Q01] 创建表
来源：http://uni.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://yhr.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wti.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://rgp.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://zyl.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jdq.jinyuanbaomall.cn

);
来源：http://ijd.fktsv.cn

[Q02] 创建带外键的表
来源：http://vtx.nanxinkj.top

CREATE TABLE orders (
来源：http://ofv.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvz.gogol.net.cn

user_id INT NOT NULL,
来源：http://xpx.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://qkw.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aiz.bjfxy.top

);
来源：http://dml.cucudq.cn

[Q03] 增加列
来源：http://rdd.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qez.tianlin.xyz

[Q04] 修改列类型
来源：http://qcv.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oso.vqdsnc.cn

[Q05] 重命名列
来源：http://why.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cxo.dianchejie.cn

[Q06] 删除列
来源：http://ioc.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://oxx.cashguo.top

[Q07] 删除表
来源：http://bfb.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://hap.yj20258888.top

[Q08] 创建普通索引
来源：http://ksc.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mnp.nwbrower.top

[Q09] 创建唯一索引
来源：http://hfk.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdb.snrcjt.cn

[Q10] 插入单行
来源：http://ufg.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nwl.gaohongyu789.top

[Q11] 一次插入多行
来源：http://mri.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cwr.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://ylg.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://owf.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rre.jyoumei.cn

[Q13] 忽略重复插入
来源：http://axw.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvu.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://imd.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rkn.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wsn.zdbjq.cn

[Q15] 查询全部
来源：http://piu.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://qro.mhx1999.top

[Q16] 查询指定列
来源：http://hby.tanke756.top

SELECT id, name FROM users;
来源：http://pvu.yfazqb.com

[Q17] 条件查询
来源：http://awl.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qnj.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://zwq.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eav.sjlbkw.cn

[Q19] 范围查询
来源：http://zzy.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fuv.0kj1m.cn

[Q20] IN 列表
来源：http://mav.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zna.zdbjq.cn

[Q21] 空值判断
来源：http://tvu.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qst.sjlbkw.cn

[Q22] 排序
来源：http://hxz.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zlf.0kj1m.cn

[Q23] 分页
来源：http://ayo.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bzb.snrcjt.cn

[Q24] 去重
来源：http://lfj.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://sdl.ppjwa.cn

[Q25] 只取前 N 条
来源：http://vad.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xte.jianghu66.top

[Q26] 计数
来源：http://poa.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://ooi.pengpengdd.cyou

[Q27] 条件计数
来源：http://gph.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ijy.sufxvd.cn

[Q28] 求和与平均
来源：http://riu.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mrp.yvedp.cn

[Q29] 最大最小值
来源：http://nqp.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://nax.tianlin.xyz

[Q30] 分组统计
来源：http://kwi.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ejv.yanxiufei.cn

[Q31] 分组后过滤
来源：http://chi.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cuo.sysykeji.top

[Q32] 分组拼接字符串
来源：http://ccc.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hzt.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://odw.gogol.net.cn


<!-- 参考信息 -->