代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://tst.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://okb.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvb.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dqd.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gza.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xgt.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://hnj.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://fwp.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zax.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mkr.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgx.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nbe.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sft.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://thb.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hpl.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xdo.hnxiangtu.top

[N05] 最大公约数
来源：http://jgy.yj20258.top

Py:   math.gcd(a, b)
来源：http://xck.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://elp.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pms.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocy.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://okg.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eir.nanxinkj.top

Ruby: a.gcd(b)
来源：http://cey.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dcu.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://kal.yj20258888.top

Py:   s == s[::-1]
来源：http://ebw.yonumen.top

PHP:  $s === strrev($s);
来源：http://szq.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://lqr.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://gdo.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ana.yj20258888.top

Go:   // 双指针从两端比较
来源：http://lyi.guannengcc.top

Ruby: s == s.reverse
来源：http://ixi.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gwv.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://dxc.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iac.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jtj.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mnq.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://qco.havefunace.top

Java: // 手写 HashMap
来源：http://rle.c1oappe.top

Go:   // 手写 map[int]int
来源：http://ayl.yj20258.top

Ruby: // 手写 Hash
来源：http://rgs.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://nko.xinyue.icu

[N08] 生成全排列
来源：http://kbl.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://npt.svipenyu.cn

PHP:  // 手写递归交换
来源：http://omm.zdbjq.cn

JS:   // 手写回溯递归
来源：http://wuu.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://wdb.pycfn.com

Java: // 手写回溯递归
来源：http://vol.vehdjk.com

Go:   // 手写回溯递归
来源：http://trh.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://uio.xinyue.icu

C#:   // 手写回溯递归
来源：http://mff.yangfankeji.com

[N09] 栈与队列
来源：http://xci.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yed.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofa.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wuq.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mjw.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umr.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vul.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mws.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wke.gzhubu.top

[N10] 链表节点定义
来源：http://uet.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://utk.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mti.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iul.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oxr.sweek.top

Java: class Node { int v; Node next; }
来源：http://zig.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eec.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nwb.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tix.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://smd.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmi.haohaochexian.top

PHP:  // 手写递归函数
来源：http://gzb.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vqz.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwt.kuanghao11.cn

Java: // 手写递归
来源：http://anv.pycfn.com

Go:   // 手写递归
来源：http://iox.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://khd.redwolf501.top

C#:   // 手写递归
来源：http://szg.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wwn.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hcy.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tjk.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyi.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzp.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rlz.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://drt.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wlb.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://chg.dashuyun.cn

================================================================================
来源：http://zfh.cucudq.cn

O. 并发与异步
来源：http://ymg.xziqi.cn

================================================================================
来源：http://xre.guannengcc.top

[O01] 启动一个线程
来源：http://ova.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pfx.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cfd.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kdw.jqgfzy.top

TS:   // 同 JS
来源：http://mai.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://xhd.fengsongda.top

Go:   go f()
来源：http://bah.aibaodan.cn

Ruby: Thread.new { f }
来源：http://why.yueranfly.top

C#:   Task.Run(() => F());
来源：http://vcs.xziqi.cn

[O02] 使用线程池
来源：http://bab.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlb.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://stn.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://pth.birdmap.top

TS:   // worker_threads 线程池
来源：http://bcv.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://izq.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hrh.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iwc.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dgy.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://qqw.yj202588.top

Py:   with lock: shared += 1
来源：http://zda.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://wse.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kyb.daria6918.cn

TS:   // 同 JS
来源：http://sff.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://xed.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mzc.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qjs.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://syg.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://bcb.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://wfu.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wdm.shuidangran.top

JS:   async function f() { await g(); }
来源：http://xvy.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dka.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://slo.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ikq.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://gib.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://aqn.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://ybl.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://ois.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uuf.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://axv.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://lfs.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://luv.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pnf.yuxming.cn

Ruby: threads.map(&:join)
来源：http://vbg.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ekd.zhixingplan.top

[O06] 使用进程池
来源：http://xnb.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tia.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvv.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://jdo.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://ait.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bkd.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wqf.bbcook.cn

Ruby: // fork 块
来源：http://wio.tanke756.top

C#:   Parallel.For
来源：http://giw.gzhubu.top

================================================================================
来源：http://ygn.yanxiufei.cn

P. 常用工具函数
来源：http://sfv.hywenlv.cn

================================================================================
来源：http://zfz.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://uuu.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://bgs.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lvv.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://kcx.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://rfe.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://wak.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://xpz.yj202588.top

Ruby: SecureRandom.uuid
来源：http://zmp.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://olv.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://rje.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pob.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xup.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://isi.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tqy.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ahq.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uuz.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://efz.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oad.vehdjk.com

[P03] 生成短随机字符串
来源：http://sdq.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lqm.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fon.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nek.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://koz.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nss.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vhm.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqb.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wss.yj202588.top

[P04] 求长度
来源：http://bhj.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iax.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://huf.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prr.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fcp.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://mjn.andypj.xyz

Go:   len(arr);  len(m)
来源：http://asn.52xcode.cn

Ruby: x.length;  x.size
来源：http://rrf.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xot.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://bpb.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gtw.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xcu.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vyw.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vef.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fqw.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://heb.yj20258.top

Ruby: a == b
来源：http://rvm.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lyr.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wqr.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfb.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://fby.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dnp.nanxinkj.top

TS:   if (x == null) {}
来源：http://crc.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xvv.epnwcf.com

Go:   if x == nil {}
来源：http://xnl.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hhu.xylfe.cn

C#:   if (x is null) {}
来源：http://glw.dianchejie.cn

[P07] 防抖与节流
来源：http://evm.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dcf.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://bkh.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwo.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzj.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qis.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://joc.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hwg.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nwz.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://pox.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cjy.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gxp.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://skv.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xrv.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sct.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ugz.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lnq.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ebv.cdnleiting.top

================================================================================
来源：http://xwk.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kit.yongpay.top

================================================================================
来源：http://xzs.jinqigufen.top

[Q01] 创建表
来源：http://rzz.nanxuanxn.top

CREATE TABLE users (
来源：http://sff.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://far.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://fkc.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://hlu.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://alz.shanyushiyangtech.top

);
来源：http://seu.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://lpj.ydjk.org.cn

CREATE TABLE orders (
来源：http://gzt.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hce.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://lgc.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://txx.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://psy.gzhubu.top

);
来源：http://wyv.fktsv.cn

[Q03] 增加列
来源：http://wfm.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nlf.yuanzhike.top

[Q04] 修改列类型
来源：http://nhs.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ell.yanxiufei.cn

[Q05] 重命名列
来源：http://pfa.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://egq.hcnkem.com

[Q06] 删除列
来源：http://czn.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://ptv.vehdjk.com

[Q07] 删除表
来源：http://dqn.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://zub.yueranfly.top

[Q08] 创建普通索引
来源：http://fco.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zrt.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://rpk.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ilp.yanxiufei.cn

[Q10] 插入单行
来源：http://ygg.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xff.guannengcc.top

[Q11] 一次插入多行
来源：http://xmr.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xyt.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://qmm.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://zjg.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://irk.jyoumei.cn

[Q13] 忽略重复插入
来源：http://gto.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sfn.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://dxo.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fix.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://era.ehwqpu.com

[Q15] 查询全部
来源：http://ewf.chenzaomai.com

SELECT * FROM users;
来源：http://idv.daxiang520.top

[Q16] 查询指定列
来源：http://eby.jianghu66.top

SELECT id, name FROM users;
来源：http://klx.fktsv.cn

[Q17] 条件查询
来源：http://pti.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xyx.gzhubu.top

[Q18] 模糊匹配
来源：http://thd.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nup.chenlongwang.top

[Q19] 范围查询
来源：http://qun.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bea.haohaochexian.top

[Q20] IN 列表
来源：http://sgb.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qjy.ppjwa.cn

[Q21] 空值判断
来源：http://uux.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vhe.yangfankeji.com

[Q22] 排序
来源：http://whf.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qof.birdmap.top

[Q23] 分页
来源：http://ggv.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kqm.yj20258888.top

[Q24] 去重
来源：http://nfc.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://dbc.hywenlv.cn

[Q25] 只取前 N 条
来源：http://kqn.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ktw.jyoumei.cn

[Q26] 计数
来源：http://wts.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://jgu.daria6918.cn

[Q27] 条件计数
来源：http://txd.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://viu.smart0.xyz

[Q28] 求和与平均
来源：http://kfu.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qgi.zhixingplan.top

[Q29] 最大最小值
来源：http://wwh.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rwu.gotoacloud.top

[Q30] 分组统计
来源：http://pnt.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ywn.ydzc1.top

[Q31] 分组后过滤
来源：http://kwr.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://psh.yongpay.top

[Q32] 分组拼接字符串
来源：http://evh.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vbe.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vcw.uphjek.com


<!-- 参考信息 -->