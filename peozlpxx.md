代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ghw.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hqb.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://bzq.yj202588.top

[N04] 斐波那契数列
来源：http://rqo.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nyw.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tbs.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wdm.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prf.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ldl.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ptl.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mam.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://msd.redwolf501.top

[N05] 最大公约数
来源：http://nab.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://clp.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bpg.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fmx.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqr.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://biz.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xgi.epnwcf.com

Ruby: a.gcd(b)
来源：http://awx.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vlr.c1oappe.top

[N06] 判断回文字符串
来源：http://mfz.jlsjyb.cn

Py:   s == s[::-1]
来源：http://yhd.sxryk.cn

PHP:  $s === strrev($s);
来源：http://zze.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://umx.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://cyc.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://irz.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://dqq.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://fjj.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xzj.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://ltf.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pdz.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axy.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hok.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://gsv.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://iod.hammf.cn

Go:   // 手写 map[int]int
来源：http://tko.gzhubu.top

Ruby: // 手写 Hash
来源：http://xfo.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://pod.iojbl.cn

[N08] 生成全排列
来源：http://ltk.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://vrg.ivvv.top

PHP:  // 手写递归交换
来源：http://tel.bjfxy.top

JS:   // 手写回溯递归
来源：http://dqd.sysykeji.top

TS:   // 手写回溯递归
来源：http://xck.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://hkm.shzxlz.cn

Go:   // 手写回溯递归
来源：http://pwq.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://vmb.zdqjudy.top

C#:   // 手写回溯递归
来源：http://xqy.jinqigufen.top

[N09] 栈与队列
来源：http://zft.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ssb.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://edj.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pnv.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pof.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fco.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uqb.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eox.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ido.jianghu66.top

[N10] 链表节点定义
来源：http://gmp.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wnt.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wqv.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vqx.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ttc.pycfn.com

Java: class Node { int v; Node next; }
来源：http://sro.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://uft.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://psl.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://gzv.316326.xyz

[N11] 二叉树中序遍历
来源：http://rxi.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axz.jinqigufen.top

PHP:  // 手写递归函数
来源：http://sti.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awh.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hkh.hcnkem.com

Java: // 手写递归
来源：http://uju.xylfe.cn

Go:   // 手写递归
来源：http://ewe.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://awx.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://nae.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rpm.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eaa.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygz.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wil.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ief.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vmz.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zou.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bry.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qnj.yongpay.top

================================================================================
来源：http://hgp.jyoumei.cn

O. 并发与异步
来源：http://nad.yvedp.cn

================================================================================
来源：http://caf.jianghu66.top

[O01] 启动一个线程
来源：http://sad.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fir.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oyu.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pbf.guowangkeji.top

TS:   // 同 JS
来源：http://eiy.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://qel.quarkkingdee.top

Go:   go f()
来源：http://wvm.yvedp.cn

Ruby: Thread.new { f }
来源：http://mxe.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://rtn.ydjk.org.cn

[O02] 使用线程池
来源：http://ttl.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kia.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://euk.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://gqw.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://iwk.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ytl.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bds.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://irj.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cqu.fehbvm.com

[O03] 加锁保护共享数据
来源：http://vtl.fktsv.cn

Py:   with lock: shared += 1
来源：http://llu.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://byu.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hhz.smart0.xyz

TS:   // 同 JS
来源：http://zke.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://eab.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oav.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ksr.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://ebd.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://byh.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://sib.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pnc.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://sbq.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://osk.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://znq.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://boq.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://yxo.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://tvz.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://tqg.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://fzi.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sxb.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://zew.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://ndt.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tiq.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yvz.xziqi.cn

Ruby: threads.map(&:join)
来源：http://bvz.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dhp.jyoumei.cn

[O06] 使用进程池
来源：http://rgk.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bzq.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qpk.ivvv.top

JS:   // child_process / cluster 模块
来源：http://tuh.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://rpd.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfy.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jlo.ybcxt.top

Ruby: // fork 块
来源：http://lki.fehbvm.com

C#:   Parallel.For
来源：http://hif.xuetiantiany.cn

================================================================================
来源：http://pmo.vehdjk.com

P. 常用工具函数
来源：http://dwj.xinyue.icu

================================================================================
来源：http://imu.fktsv.cn

[P01] 生成 UUID
来源：http://lsd.yj20258.top

Py:   str(uuid.uuid4())
来源：http://aag.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://apg.tian-w.cn

JS:   crypto.randomUUID()
来源：http://hkz.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://zrs.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://qkm.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://bcn.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://ufd.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://pum.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://lev.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hby.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://skf.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lpz.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xxx.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hsh.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntc.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jpw.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gml.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://isg.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nke.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ena.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hty.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vcc.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bee.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vwq.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lwp.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ujb.yuanzhike.top

[P04] 求长度
来源：http://hsl.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fbh.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ril.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hgv.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nyo.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://qlq.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://gyq.pycfn.com

Ruby: x.length;  x.size
来源：http://axl.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://bfj.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://dbd.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://sdy.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rfn.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hrz.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ozc.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qdg.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nyf.sweek.top

Ruby: a == b
来源：http://cog.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ltv.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://umy.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ijo.meibo888.top

PHP:  if (empty($x)) {}
来源：http://jaq.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mli.ehwqpu.com

TS:   if (x == null) {}
来源：http://wco.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://gfq.bjfxy.top

Go:   if x == nil {}
来源：http://euj.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lvz.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://ryl.zhengqikj.top

[P07] 防抖与节流
来源：http://zov.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nlu.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://qeq.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uwx.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iql.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ykf.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fso.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gpz.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzs.sysykeji.top

[P08] 处理浮点精度问题
来源：http://aqx.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qrc.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fjo.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mmd.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aoj.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wee.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xdz.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lor.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bbo.mhx1999.top

================================================================================
来源：http://krk.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mkn.ctjpmb.com

================================================================================
来源：http://rsi.ehwqpu.com

[Q01] 创建表
来源：http://chh.svipenyu.cn

CREATE TABLE users (
来源：http://cla.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jyp.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://zwu.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://pex.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bft.ctjpmb.com

);
来源：http://eba.cheryme.top

[Q02] 创建带外键的表
来源：http://beg.yfazqb.com

CREATE TABLE orders (
来源：http://mfu.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qct.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://imp.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://knl.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rcu.aizwys.cn

);
来源：http://ieb.iojbl.cn

[Q03] 增加列
来源：http://scp.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hho.chenlongwang.top

[Q04] 修改列类型
来源：http://fti.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ppb.zhixingplan.top

[Q05] 重命名列
来源：http://iie.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://msl.pycfn.com

[Q06] 删除列
来源：http://whs.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://dxi.hammf.cn

[Q07] 删除表
来源：http://dgs.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://byd.yuxming.cn

[Q08] 创建普通索引
来源：http://asv.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://afg.cqqwz.cn

[Q09] 创建唯一索引
来源：http://zxs.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bkq.gogol.net.cn

[Q10] 插入单行
来源：http://rfa.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qut.zdqjudy.top

[Q11] 一次插入多行
来源：http://buo.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vqe.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://pzg.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ktd.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gpg.havefunace.top

[Q13] 忽略重复插入
来源：http://jol.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lnk.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://gdg.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://inn.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vtz.yongpay.top

[Q15] 查询全部
来源：http://rrr.ivvv.top

SELECT * FROM users;
来源：http://sbu.pengpengdd.cyou

[Q16] 查询指定列
来源：http://mow.yuanzhike.top

SELECT id, name FROM users;
来源：http://irg.sufxvd.cn

[Q17] 条件查询
来源：http://zst.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rad.gzhubu.top

[Q18] 模糊匹配
来源：http://agk.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qre.316326.xyz

[Q19] 范围查询
来源：http://qrr.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kje.zhiwuduotai.top

[Q20] IN 列表
来源：http://fxc.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ejv.yangfankeji.com

[Q21] 空值判断
来源：http://fba.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ozt.shanyushiyangkeji.top

[Q22] 排序
来源：http://die.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pjx.ydzc1.top

[Q23] 分页
来源：http://bdd.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kza.fanxiaobao.xyz

[Q24] 去重
来源：http://tqj.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://ruw.mhx1999.top

[Q25] 只取前 N 条
来源：http://qhn.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zqe.nwbrower.top

[Q26] 计数
来源：http://zgi.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://ann.gogol.net.cn

[Q27] 条件计数
来源：http://rvu.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zwh.yuanzhike.top

[Q28] 求和与平均
来源：http://jkv.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zfc.xuanzx.com

[Q29] 最大最小值
来源：http://hxd.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://rqp.bbcook.cn

[Q30] 分组统计
来源：http://aad.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yhm.xylfe.cn

[Q31] 分组后过滤
来源：http://rve.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://drm.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://xnv.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://urf.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ngv.0kj1m.cn

[Q33] 多列分组
来源：http://haz.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzi.hnqzz.top

[Q34] 每组取第一条
来源：http://cnv.vqdsnc.cn

SELECT * FROM (
来源：http://osn.haohaochexian.top


<!-- 参考信息 -->