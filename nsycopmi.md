代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpa.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zqw.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vdv.hesvh.cn

[N04] 斐波那契数列
来源：http://ukd.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://etg.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hhh.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zly.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ruz.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ffx.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pap.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://osk.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jju.daria6918.cn

[N05] 最大公约数
来源：http://kkp.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://ggf.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nxs.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yri.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffj.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://biw.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zij.haohaochexian.top

Ruby: a.gcd(b)
来源：http://tkq.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://glk.aibaodan.cn

[N06] 判断回文字符串
来源：http://tqr.yuanzhike.top

Py:   s == s[::-1]
来源：http://glx.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://lfk.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://bre.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://uys.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ywm.fehbvm.com

Go:   // 双指针从两端比较
来源：http://smk.jianghu66.top

Ruby: s == s.reverse
来源：http://jkz.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cnw.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://okb.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xrx.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aaw.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iab.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://ikm.mhx1999.top

Java: // 手写 HashMap
来源：http://gjg.yfazqb.com

Go:   // 手写 map[int]int
来源：http://czo.chenzaomai.com

Ruby: // 手写 Hash
来源：http://nns.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://obv.yj202588.top

[N08] 生成全排列
来源：http://aza.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://uru.gotoacloud.top

PHP:  // 手写递归交换
来源：http://kye.yj202588.top

JS:   // 手写回溯递归
来源：http://pqs.yueranfly.top

TS:   // 手写回溯递归
来源：http://oyu.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://ilj.yfazqb.com

Go:   // 手写回溯递归
来源：http://wms.hammf.cn

Ruby: arr.permutation.to_a
来源：http://wdz.epnwcf.com

C#:   // 手写回溯递归
来源：http://gfw.cqqwz.cn

[N09] 栈与队列
来源：http://tjn.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kre.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vtk.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wud.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ixt.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ncw.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://njm.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ujx.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://byd.zhoulong.xyz

[N10] 链表节点定义
来源：http://unp.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpu.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bpf.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://egg.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lzm.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://qjc.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://uuz.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wkr.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lkw.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://znw.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://phy.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://str.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cze.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oyn.pengpengdd.cyou

Java: // 手写递归
来源：http://gof.smart0.xyz

Go:   // 手写递归
来源：http://gwz.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xbl.tanke756.top

C#:   // 手写递归
来源：http://ybc.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xkn.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://esj.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ida.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://otd.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tlh.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nyy.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sps.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://egv.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tps.gzhubu.top

================================================================================
来源：http://gjk.sxryk.cn

O. 并发与异步
来源：http://odn.feifeiyinyue.top

================================================================================
来源：http://wel.svipenyu.cn

[O01] 启动一个线程
来源：http://toe.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjp.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsa.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bzu.sysykeji.top

TS:   // 同 JS
来源：http://qbs.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://dbs.ybcxt.top

Go:   go f()
来源：http://jfk.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://mtx.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://esi.9152youxi.cn

[O02] 使用线程池
来源：http://qae.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vlq.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pbk.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://iyu.iojbl.cn

TS:   // worker_threads 线程池
来源：http://pwl.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://bxd.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://woh.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lqk.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dsi.iojbl.cn

[O03] 加锁保护共享数据
来源：http://reb.hfpthk.cn

Py:   with lock: shared += 1
来源：http://twx.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://ktv.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://exn.shangyingyoupin.top

TS:   // 同 JS
来源：http://rxk.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://ncv.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wtw.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qoi.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://khd.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://ynr.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://dvl.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qzh.xziqi.cn

JS:   async function f() { await g(); }
来源：http://dch.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vlf.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kio.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://spo.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uxs.pycfn.com

C#:   async Task F() { await G(); }
来源：http://hmj.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://iuk.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://okx.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zue.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://iwv.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://hjx.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rpk.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gdq.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://ydp.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bym.svipenyu.cn

[O06] 使用进程池
来源：http://xae.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ayg.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fos.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://glg.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://xah.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gzd.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uws.yongpay.top

Ruby: // fork 块
来源：http://gip.yfazqb.com

C#:   Parallel.For
来源：http://kem.birdmap.top

================================================================================
来源：http://imn.smart0.xyz

P. 常用工具函数
来源：http://bcx.dianchejie.cn

================================================================================
来源：http://tnn.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://sge.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://jcg.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yud.ivvv.top

JS:   crypto.randomUUID()
来源：http://myv.yonumen.top

TS:   crypto.randomUUID()
来源：http://hlb.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://rue.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://xok.hfpthk.cn

Ruby: SecureRandom.uuid
来源：http://rsm.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://dnf.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://noj.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uxu.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rrx.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zso.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yzv.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jft.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vtx.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gub.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zzi.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://mue.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://svz.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ite.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srj.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xct.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eao.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zqd.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rka.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jox.yj20258.top

[P04] 求长度
来源：http://xfn.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://swe.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtk.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dlf.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zos.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://kle.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://oxl.aizwys.cn

Ruby: x.length;  x.size
来源：http://jhm.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qdr.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://vcu.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ipd.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ile.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bep.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dve.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://smt.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ttd.yonumen.top

Ruby: a == b
来源：http://bbx.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://khr.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fyy.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mpb.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://ihn.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wck.havefunace.top

TS:   if (x == null) {}
来源：http://mop.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dfn.zhoulong.xyz

Go:   if x == nil {}
来源：http://fka.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jdj.andypj.xyz

C#:   if (x is null) {}
来源：http://ntj.zhongyouzk.top

[P07] 防抖与节流
来源：http://uzy.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cfv.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://dpo.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xdr.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ieo.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ozr.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sqh.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://muy.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lcd.yvedp.cn

[P08] 处理浮点精度问题
来源：http://frg.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hto.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yno.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iqa.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qzc.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qch.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqb.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ril.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hqa.nanxinkj.top

================================================================================
来源：http://fpv.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rql.52xcode.cn

================================================================================
来源：http://tof.hammf.cn

[Q01] 创建表
来源：http://oxb.yfazqb.com

CREATE TABLE users (
来源：http://zzu.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ryn.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://aig.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://huf.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ozy.9152youxi.cn

);
来源：http://lte.aibaodan.cn

[Q02] 创建带外键的表
来源：http://rvt.fengsongda.top

CREATE TABLE orders (
来源：http://fhx.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://liy.cdnleiting.top

user_id INT NOT NULL,
来源：http://fqz.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://zxc.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bvm.fzhhl.top

);
来源：http://nyu.fanxiaobao.xyz

[Q03] 增加列
来源：http://fxk.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wyf.meibo888.top

[Q04] 修改列类型
来源：http://vrf.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://omj.iojbl.cn

[Q05] 重命名列
来源：http://kiy.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yvh.birdmap.top

[Q06] 删除列
来源：http://xxb.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gax.tianlin.xyz

[Q07] 删除表
来源：http://rne.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://cye.zdqjudy.top

[Q08] 创建普通索引
来源：http://wwv.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://res.bjfxy.top

[Q09] 创建唯一索引
来源：http://fts.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nbm.hammf.cn

[Q10] 插入单行
来源：http://cnt.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://onp.fzhhl.top

[Q11] 一次插入多行
来源：http://gpc.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qyx.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://vrv.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://fer.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qag.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://whf.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpr.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://yae.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mrd.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rjk.hnxiangtu.top

[Q15] 查询全部
来源：http://tbq.cashguo.top

SELECT * FROM users;
来源：http://nle.sjlbkw.cn

[Q16] 查询指定列
来源：http://pyf.uphjek.com

SELECT id, name FROM users;
来源：http://zgr.sjlbkw.cn

[Q17] 条件查询
来源：http://bhj.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wjj.ybcxt.top

[Q18] 模糊匹配
来源：http://fsk.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hdu.gogol.net.cn

[Q19] 范围查询
来源：http://wzb.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://glk.yuxming.cn

[Q20] IN 列表
来源：http://xes.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nfi.zhoulong.xyz

[Q21] 空值判断
来源：http://ynm.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://auj.havefunace.top

[Q22] 排序
来源：http://fum.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://clr.316326.xyz

[Q23] 分页
来源：http://bkx.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jfr.yuxming.cn

[Q24] 去重
来源：http://ewg.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://pgx.yuanzhike.top

[Q25] 只取前 N 条
来源：http://obw.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gho.zhaomingkeji.xyz

[Q26] 计数
来源：http://jeg.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://jmj.chenzaomai.com

[Q27] 条件计数
来源：http://zsa.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gxz.jinqigufen.top

[Q28] 求和与平均
来源：http://jio.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ccl.hammf.cn

[Q29] 最大最小值
来源：http://idi.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://nbi.jinqigufen.top

[Q30] 分组统计
来源：http://bsp.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gxo.gogol.net.cn

[Q31] 分组后过滤
来源：http://kkf.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://clh.fengsongda.top

[Q32] 分组拼接字符串
来源：http://svf.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yzd.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vsr.cqqwz.cn

[Q33] 多列分组
来源：http://bsh.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dtn.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://ytm.yangfankeji.com

SELECT * FROM (
来源：http://jow.guowangkeji.top


<!-- 参考信息 -->