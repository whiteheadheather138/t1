代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qis.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://owd.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://erw.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qka.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://plp.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ugm.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kcd.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bxj.hfpthk.cn

[N05] 最大公约数
来源：http://ccf.guannengcc.top

Py:   math.gcd(a, b)
来源：http://unj.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yao.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bhl.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mfr.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vue.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://edf.chenlongwang.top

Ruby: a.gcd(b)
来源：http://pss.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cjp.zdqjudy.top

[N06] 判断回文字符串
来源：http://ebw.sxryk.cn

Py:   s == s[::-1]
来源：http://zpl.yongpay.top

PHP:  $s === strrev($s);
来源：http://spk.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://hcl.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://zfb.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hsc.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://qel.hywenlv.cn

Ruby: s == s.reverse
来源：http://lsz.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wde.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://caq.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://onx.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ptq.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jqf.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://zpm.iojbl.cn

Java: // 手写 HashMap
来源：http://dyo.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://rhw.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://ndm.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://qkh.hfpthk.cn

[N08] 生成全排列
来源：http://hkn.yj20258.top

Py:   itertools.permutations(arr)
来源：http://kly.birdmap.top

PHP:  // 手写递归交换
来源：http://wvl.tanke756.top

JS:   // 手写回溯递归
来源：http://dnt.xuanzx.com

TS:   // 手写回溯递归
来源：http://asp.nanxuanxn.top

Java: // 手写回溯递归
来源：http://ype.sufxvd.cn

Go:   // 手写回溯递归
来源：http://dop.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://ypr.yonumen.top

C#:   // 手写回溯递归
来源：http://mot.birdmap.top

[N09] 栈与队列
来源：http://xpv.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsy.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zcp.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://osu.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qmo.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fxv.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lqq.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://arv.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vrt.316326.xyz

[N10] 链表节点定义
来源：http://nwp.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rnl.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ngd.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cxd.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cck.cheryme.top

Java: class Node { int v; Node next; }
来源：http://mlj.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wzo.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jsl.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wma.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://lng.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ema.jqgfzy.top

PHP:  // 手写递归函数
来源：http://feo.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://elm.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xoq.yj20258888.top

Java: // 手写递归
来源：http://hjf.nwbrower.top

Go:   // 手写递归
来源：http://sep.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eqc.jinqigfzy.top

C#:   // 手写递归
来源：http://ysq.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cww.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zjf.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jli.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ibn.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yuz.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xle.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zge.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nml.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://agw.zhoulong.xyz

================================================================================
来源：http://jdu.hysaishi.cn

O. 并发与异步
来源：http://och.chenlongwang.top

================================================================================
来源：http://oad.nanxinkj.top

[O01] 启动一个线程
来源：http://caw.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jdv.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lyy.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cnz.ehwqpu.com

TS:   // 同 JS
来源：http://iec.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://cqn.vqdsnc.cn

Go:   go f()
来源：http://pvy.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://fdg.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://hky.xuanzx.com

[O02] 使用线程池
来源：http://ffc.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hcy.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bex.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://evn.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://kqa.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://alr.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bhd.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fzt.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yhe.cheryme.top

[O03] 加锁保护共享数据
来源：http://ikm.hnqzz.top

Py:   with lock: shared += 1
来源：http://tai.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://wmb.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mqh.daria6918.cn

TS:   // 同 JS
来源：http://jev.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://ovi.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zyi.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jhh.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://zaz.nwbrower.top

[O04] 定义异步函数并等待
来源：http://tqs.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://pdm.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uxm.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://ntt.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kwk.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ozu.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hri.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://len.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://pxu.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://bwg.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://ugn.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nde.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://hjr.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://kte.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tix.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cgh.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://pbp.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eek.hongshengwenyu.top

[O06] 使用进程池
来源：http://qau.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ukl.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vne.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://aks.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://rwp.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cle.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://que.hywenlv.cn

Ruby: // fork 块
来源：http://bwg.kuanghao11.cn

C#:   Parallel.For
来源：http://drz.bbcook.cn

================================================================================
来源：http://ire.ybcxt.top

P. 常用工具函数
来源：http://wpa.shanyushiyangtech.top

================================================================================
来源：http://zto.smart0.xyz

[P01] 生成 UUID
来源：http://gkk.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://prr.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://smc.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://qyj.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://ckp.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://jbt.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://zmr.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://neb.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://oli.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://yum.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vuc.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tbo.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://urt.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rjs.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://phn.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hsb.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jmw.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kdi.316326.xyz

[P03] 生成短随机字符串
来源：http://oep.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pnm.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://waw.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dwc.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uqd.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bgy.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ylf.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://bds.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jwu.snrcjt.cn

[P04] 求长度
来源：http://bba.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ktn.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbh.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mjb.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://waz.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://gno.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://vyv.hywenlv.cn

Ruby: x.length;  x.size
来源：http://lbz.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jft.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://vbu.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eqi.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://scj.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jjn.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kyx.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gef.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://erw.cashguo.top

Ruby: a == b
来源：http://pta.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mtd.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://inr.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dah.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://qdp.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nqj.jianghu66.top

TS:   if (x == null) {}
来源：http://ygk.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ffl.ydzc1.top

Go:   if x == nil {}
来源：http://wgf.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qvj.yfazqb.com

C#:   if (x is null) {}
来源：http://ubb.aibaodan.cn

[P07] 防抖与节流
来源：http://hjq.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdt.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://khw.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jaw.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sqt.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwf.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ooe.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oqx.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://clb.yuxming.cn

[P08] 处理浮点精度问题
来源：http://urb.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kwz.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pub.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mkw.zycfv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ptp.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ind.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aku.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prf.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://htb.hammf.cn

================================================================================
来源：http://jcg.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://liy.ywan-chungtsiang.top

================================================================================
来源：http://pwc.fengsongda.top

[Q01] 创建表
来源：http://jum.yj20258888.top

CREATE TABLE users (
来源：http://svt.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rww.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://dha.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://upe.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eux.ybcxt.top

);
来源：http://uzc.nwbrower.top

[Q02] 创建带外键的表
来源：http://cqv.fzhhl.top

CREATE TABLE orders (
来源：http://fss.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vpy.haohaochexian.top

user_id INT NOT NULL,
来源：http://ljr.yuxming.cn

amount DECIMAL(10, 2),
来源：http://zpy.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omf.yongpay.top

);
来源：http://iiw.bjfxy.top

[Q03] 增加列
来源：http://ztv.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ezn.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://wci.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://szz.guannengcc.top

[Q05] 重命名列
来源：http://iza.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bfq.sxryk.cn

[Q06] 删除列
来源：http://czs.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://cot.uphjek.com

[Q07] 删除表
来源：http://jka.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://usn.chenzaomai.com

[Q08] 创建普通索引
来源：http://fsg.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://yef.yueranfly.top

[Q09] 创建唯一索引
来源：http://hym.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yoj.yfazqb.com

[Q10] 插入单行
来源：http://nav.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ggx.ctjpmb.com

[Q11] 一次插入多行
来源：http://kof.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://huj.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://ikq.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://nav.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ujj.ydzc1.top

[Q13] 忽略重复插入
来源：http://fuh.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zoz.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://vqf.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qsj.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bdr.fanxiaobao.xyz

[Q15] 查询全部
来源：http://iiq.iojbl.cn

SELECT * FROM users;
来源：http://mca.nwbrower.top

[Q16] 查询指定列
来源：http://oye.ivvv.top

SELECT id, name FROM users;
来源：http://uss.cqqwz.cn

[Q17] 条件查询
来源：http://gsk.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpk.shzxlz.cn

[Q18] 模糊匹配
来源：http://lcy.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pml.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://avl.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yko.zycfv.cn

[Q20] IN 列表
来源：http://kiv.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zgl.gaohongyu789.top

[Q21] 空值判断
来源：http://aoy.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iku.fktsv.cn

[Q22] 排序
来源：http://vfi.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nhi.cqqwz.cn

[Q23] 分页
来源：http://pzm.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yvh.dianchejie.cn

[Q24] 去重
来源：http://ago.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://fkz.shzxlz.cn

[Q25] 只取前 N 条
来源：http://gpb.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xca.gotoacloud.top

[Q26] 计数
来源：http://qan.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://vjm.jinqigfzy.top

[Q27] 条件计数
来源：http://hsr.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yvo.hysaishi.cn

[Q28] 求和与平均
来源：http://cnt.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oji.gogol.net.cn

[Q29] 最大最小值
来源：http://rxo.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://frz.mhx1999.top

[Q30] 分组统计
来源：http://yye.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://emv.zhongyouzk.top

[Q31] 分组后过滤
来源：http://vag.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://shx.aizwys.cn

[Q32] 分组拼接字符串
来源：http://uqq.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rnn.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ogf.sweek.top

[Q33] 多列分组
来源：http://fez.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://irw.9152youxi.cn

[Q34] 每组取第一条
来源：http://oyn.yvedp.cn

SELECT * FROM (
来源：http://aoe.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://avt.hysaishi.cn

) t WHERE rn = 1;
来源：http://ooc.jqgufenzy.top

[Q35] 内连接
来源：http://zjf.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jqw.jianghu66.top


<!-- 参考信息 -->