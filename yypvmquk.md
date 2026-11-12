代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://nms.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://stc.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ole.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eja.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vcw.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ahc.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://vpo.cashguo.top

[N04] 斐波那契数列
来源：http://cih.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fcp.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ltd.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bgx.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hzt.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lvh.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qbv.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dou.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wsd.xylfe.cn

[N05] 最大公约数
来源：http://tmu.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://ajj.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vws.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovi.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qii.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uru.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kuj.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://xbu.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbq.tianlin.xyz

[N06] 判断回文字符串
来源：http://mnh.jianghu66.top

Py:   s == s[::-1]
来源：http://azd.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://fij.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://exk.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://dtq.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zyt.pycfn.com

Go:   // 双指针从两端比较
来源：http://yek.yvedp.cn

Ruby: s == s.reverse
来源：http://skr.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nzm.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://roz.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vyr.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abp.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kse.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://gpx.quarkkingdee.top

Java: // 手写 HashMap
来源：http://neg.yfazqb.com

Go:   // 手写 map[int]int
来源：http://cdj.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://uql.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hmt.havefunace.top

[N08] 生成全排列
来源：http://mze.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://hyg.dianchejie.cn

PHP:  // 手写递归交换
来源：http://jgv.jianghu66.top

JS:   // 手写回溯递归
来源：http://gsu.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://clf.dianchejie.cn

Java: // 手写回溯递归
来源：http://wpa.smart0.xyz

Go:   // 手写回溯递归
来源：http://bdc.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://xvr.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://wwy.svipenyu.cn

[N09] 栈与队列
来源：http://tcl.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ycj.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zit.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://myw.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ziu.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ecm.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bnl.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wgy.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iza.ydzc1.top

[N10] 链表节点定义
来源：http://fku.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfd.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://twu.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ula.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxy.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://utp.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ayt.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jvp.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://edz.wangdashe.top

[N11] 二叉树中序遍历
来源：http://jod.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ung.dianchejie.cn

PHP:  // 手写递归函数
来源：http://ims.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://haz.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oha.jianghu66.top

Java: // 手写递归
来源：http://jqs.daxiang520.top

Go:   // 手写递归
来源：http://iri.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tnl.xuanzx.com

C#:   // 手写递归
来源：http://rau.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://knu.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tns.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xhl.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llh.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wqw.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hdi.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mgn.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oqg.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wcj.shanyushiyangtech.top

================================================================================
来源：http://dpd.fktsv.cn

O. 并发与异步
来源：http://qwq.tianlin.xyz

================================================================================
来源：http://cha.hcnkem.com

[O01] 启动一个线程
来源：http://idt.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cso.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lyv.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nof.zhengqikj.top

TS:   // 同 JS
来源：http://hdc.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://yid.zhaomingkeji.xyz

Go:   go f()
来源：http://xlo.epnwcf.com

Ruby: Thread.new { f }
来源：http://yul.redwolf501.top

C#:   Task.Run(() => F());
来源：http://hlc.wangshuangyany.cn

[O02] 使用线程池
来源：http://gxi.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oyk.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xbk.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://dxu.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://wto.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://cln.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fez.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kyo.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpd.nwbrower.top

[O03] 加锁保护共享数据
来源：http://lcs.ybcxt.top

Py:   with lock: shared += 1
来源：http://dfl.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://reb.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hvs.zhijiandao.cn

TS:   // 同 JS
来源：http://wcg.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://svo.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fqw.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vat.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://zud.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://yey.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://xgs.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fnc.jianghu66.top

JS:   async function f() { await g(); }
来源：http://vic.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ipk.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dco.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ryp.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://iik.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://ukk.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://wie.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://sns.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rjt.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://ney.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://gvv.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sch.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sey.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://zbx.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://srp.sxryk.cn

[O06] 使用进程池
来源：http://imo.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://guz.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://awz.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://xle.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://fjh.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://apx.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqh.jiagoushi.top

Ruby: // fork 块
来源：http://pfv.nanxinkj.top

C#:   Parallel.For
来源：http://xxf.wangdashe.top

================================================================================
来源：http://pfx.c1oappe.top

P. 常用工具函数
来源：http://zei.daria6918.cn

================================================================================
来源：http://vwu.gogol.net.cn

[P01] 生成 UUID
来源：http://xtp.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://wwg.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dxm.daxiang520.top

JS:   crypto.randomUUID()
来源：http://wgj.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://dhn.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://qkn.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://rfg.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://oxw.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://ejj.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://dud.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfz.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ikw.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zkn.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ipa.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zlk.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntd.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xqp.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://khd.bbcook.cn

[P03] 生成短随机字符串
来源：http://sjv.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://epm.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xzw.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayt.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hcz.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cpm.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://owi.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://sbf.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lnu.havefunace.top

[P04] 求长度
来源：http://evi.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zzf.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cba.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rci.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llz.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://pux.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://mzu.0kj1m.cn

Ruby: x.length;  x.size
来源：http://oxv.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ioc.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://zde.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hvn.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pjq.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://alc.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nkv.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdt.zhongyouzk.top

Go:   reflect.DeepEqual(a, b)
来源：http://hxj.jyoumei.cn

Ruby: a == b
来源：http://owm.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://alq.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://unh.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oyj.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://qpk.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhw.guowangkeji.top

TS:   if (x == null) {}
来源：http://fgy.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://jki.yangfankeji.com

Go:   if x == nil {}
来源：http://gwd.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rud.cashguo.top

C#:   if (x is null) {}
来源：http://xqr.hnxiangtu.top

[P07] 防抖与节流
来源：http://wap.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ntu.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://jeq.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lag.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwf.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qxu.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yfz.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://sph.quarkkingdee.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bsf.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://thl.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zjq.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jug.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vku.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jjp.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qab.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sac.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kuy.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qma.dianchejie.cn

================================================================================
来源：http://qrg.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://snv.sxryk.cn

================================================================================
来源：http://ihl.tianlin.xyz

[Q01] 创建表
来源：http://ixx.52xcode.cn

CREATE TABLE users (
来源：http://uxs.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fad.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://zjf.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://idu.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://etm.nwbrower.top

);
来源：http://ovm.ppjwa.cn

[Q02] 创建带外键的表
来源：http://mxs.nwbrower.top

CREATE TABLE orders (
来源：http://jpv.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aur.uphjek.com

user_id INT NOT NULL,
来源：http://wsy.ivvv.top

amount DECIMAL(10, 2),
来源：http://xeh.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://axh.nanxuanxn.top

);
来源：http://zzg.zhaomingkeji.xyz

[Q03] 增加列
来源：http://fhv.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rnq.xylfe.cn

[Q04] 修改列类型
来源：http://zwu.bbcook.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lav.52xcode.cn

[Q05] 重命名列
来源：http://nrz.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lbe.gogol.net.cn

[Q06] 删除列
来源：http://vcx.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://xpl.zhaomingkeji.xyz

[Q07] 删除表
来源：http://gwq.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://rxf.zdqjudy.top

[Q08] 创建普通索引
来源：http://uaw.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qwb.xinyue.icu

[Q09] 创建唯一索引
来源：http://ybo.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://etj.0kj1m.cn

[Q10] 插入单行
来源：http://nys.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://riw.jiagoushi.top

[Q11] 一次插入多行
来源：http://btg.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jmg.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://noy.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://xpf.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bzt.zdbjq.cn

[Q13] 忽略重复插入
来源：http://cxo.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iim.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://yrn.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yks.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cvb.dianchejie.cn

[Q15] 查询全部
来源：http://tjt.sysykeji.top

SELECT * FROM users;
来源：http://ebr.zhengqikj.top

[Q16] 查询指定列
来源：http://oew.sysykeji.top

SELECT id, name FROM users;
来源：http://vjs.haohaochexian.top

[Q17] 条件查询
来源：http://ayf.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://azk.iojbl.cn

[Q18] 模糊匹配
来源：http://pbb.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zag.chenjidiqi.icu

[Q19] 范围查询
来源：http://byk.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vnn.tarul.cn

[Q20] IN 列表
来源：http://weh.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://isl.yongpay.top

[Q21] 空值判断
来源：http://mby.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://frg.tarul.cn

[Q22] 排序
来源：http://sbx.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qkl.pycfn.com

[Q23] 分页
来源：http://dof.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yuf.zhoulong.xyz

[Q24] 去重
来源：http://ckg.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://jvs.yvedp.cn

[Q25] 只取前 N 条
来源：http://dgz.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rgf.kuanghao11.cn

[Q26] 计数
来源：http://hcz.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://ack.pengpengdd.cyou

[Q27] 条件计数
来源：http://mnf.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://odp.epnwcf.com

[Q28] 求和与平均
来源：http://hfb.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dkx.0kj1m.cn

[Q29] 最大最小值
来源：http://mdt.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rvv.ybcxt.top

[Q30] 分组统计
来源：http://rpj.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fvg.dianchejie.cn

[Q31] 分组后过滤
来源：http://lza.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tcm.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://qut.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fem.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rza.meibo888.top


<!-- 参考信息 -->