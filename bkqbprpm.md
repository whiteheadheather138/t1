代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tkh.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mrl.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wxk.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jek.yangfankeji.com

[N05] 最大公约数
来源：http://hiv.fengsongda.top

Py:   math.gcd(a, b)
来源：http://skx.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sky.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://raz.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xok.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://piw.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bwa.gogol.net.cn

Ruby: a.gcd(b)
来源：http://uwt.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oqo.aibaodan.cn

[N06] 判断回文字符串
来源：http://yam.uphjek.com

Py:   s == s[::-1]
来源：http://lmh.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://zvc.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://bqg.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://qru.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ujf.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://nmf.yonumen.top

Ruby: s == s.reverse
来源：http://trj.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uax.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://tcs.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gag.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rko.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lra.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://imh.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://pnc.daxiang520.top

Go:   // 手写 map[int]int
来源：http://bfa.snrcjt.cn

Ruby: // 手写 Hash
来源：http://bqv.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gye.hywenlv.cn

[N08] 生成全排列
来源：http://zvf.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://izt.chenlongwang.top

PHP:  // 手写递归交换
来源：http://mhn.tian-w.cn

JS:   // 手写回溯递归
来源：http://poy.shzxlz.cn

TS:   // 手写回溯递归
来源：http://ppr.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://vro.jyoumei.cn

Go:   // 手写回溯递归
来源：http://ugq.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://kwn.gogol.net.cn

C#:   // 手写回溯递归
来源：http://hfw.jyoumei.cn

[N09] 栈与队列
来源：http://evx.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ssb.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mbd.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pth.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gya.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://msb.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ohj.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xdd.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mtm.yvedp.cn

[N10] 链表节点定义
来源：http://uvb.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://thp.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tpk.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://alb.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://txf.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://atc.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://dgx.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bec.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kei.cucudq.cn

[N11] 二叉树中序遍历
来源：http://umz.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hyp.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://itp.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://neq.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brt.hywenlv.cn

Java: // 手写递归
来源：http://tyf.zhengqikj.top

Go:   // 手写递归
来源：http://zzz.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yrx.tanke756.top

C#:   // 手写递归
来源：http://hlb.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lvc.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xrr.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wwg.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruv.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knr.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uug.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://txp.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://krr.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wir.ywan-chungtsiang.top

================================================================================
来源：http://xnz.xuanzx.com

O. 并发与异步
来源：http://tfk.dianchejie.cn

================================================================================
来源：http://dhm.fktsv.cn

[O01] 启动一个线程
来源：http://waz.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cdc.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ril.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fgk.yonumen.top

TS:   // 同 JS
来源：http://sie.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://zei.xylfe.cn

Go:   go f()
来源：http://gsq.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://bga.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://vdw.hywenlv.cn

[O02] 使用线程池
来源：http://bpl.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fdz.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wqf.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://fal.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://esn.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tmm.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ngi.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zai.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://imc.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://wvc.jinqigufen.top

Py:   with lock: shared += 1
来源：http://bss.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://zoy.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hxw.tanke756.top

TS:   // 同 JS
来源：http://fxz.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://kca.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wkv.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vtf.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://kke.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://gsq.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://aot.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://itv.316326.xyz

JS:   async function f() { await g(); }
来源：http://yph.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oyo.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jmh.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zvi.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://cka.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://nlw.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://xoc.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://cxm.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rwh.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://qkf.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://ypz.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yjq.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://knm.aizwys.cn

Ruby: threads.map(&:join)
来源：http://kpd.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqo.ehwqpu.com

[O06] 使用进程池
来源：http://cjl.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ams.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://jhz.uphjek.com

JS:   // child_process / cluster 模块
来源：http://ikf.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://kfs.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sox.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eed.vqdsnc.cn

Ruby: // fork 块
来源：http://ueu.xuanzx.com

C#:   Parallel.For
来源：http://ezc.sjlbkw.cn

================================================================================
来源：http://ubt.ivvv.top

P. 常用工具函数
来源：http://hrz.ywan-chungtsiang.top

================================================================================
来源：http://reu.cucudq.cn

[P01] 生成 UUID
来源：http://fnc.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://gsq.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vbf.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://pdi.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://uxw.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://egs.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://jbb.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://kbs.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://dap.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://flz.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wsh.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://cwm.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ivm.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://daw.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gvw.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dpj.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mqy.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxz.0kj1m.cn

[P03] 生成短随机字符串
来源：http://dxt.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqx.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yym.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gps.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zab.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ley.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jqn.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://omw.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rrn.ydzc1.top

[P04] 求长度
来源：http://vez.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wvj.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mdt.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://msv.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://snq.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://jzm.yuxming.cn

Go:   len(arr);  len(m)
来源：http://sif.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://vwt.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wov.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://yka.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ejf.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rvk.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://irs.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rnz.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jqs.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://bwi.hfpthk.cn

Ruby: a == b
来源：http://nvt.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jwn.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aqh.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxd.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://sjc.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://osf.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://rml.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ujk.dashuyun.cn

Go:   if x == nil {}
来源：http://kfi.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fti.dashuyun.cn

C#:   if (x is null) {}
来源：http://vke.yj20258.top

[P07] 防抖与节流
来源：http://cnm.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sco.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://epr.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ooo.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktv.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cud.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zep.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://knm.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zpw.sweek.top

[P08] 处理浮点精度问题
来源：http://dzg.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://exi.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wmd.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pkc.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ekl.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://scn.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://msh.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fse.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ckh.feifeiyinyue.top

================================================================================
来源：http://tgp.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lob.fzhhl.top

================================================================================
来源：http://coj.zdbjq.cn

[Q01] 创建表
来源：http://tuv.aizwys.cn

CREATE TABLE users (
来源：http://coi.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ahz.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://egn.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://uaa.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://odb.chenjidiqi.icu

);
来源：http://bml.0kj1m.cn

[Q02] 创建带外键的表
来源：http://irp.ivvv.top

CREATE TABLE orders (
来源：http://bel.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pgg.ydjk.org.cn

user_id INT NOT NULL,
来源：http://lbm.guannengcc.top

amount DECIMAL(10, 2),
来源：http://osp.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uuj.andypj.xyz

);
来源：http://vsl.yvedp.cn

[Q03] 增加列
来源：http://bjl.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vzk.shuidangran.top

[Q04] 修改列类型
来源：http://mze.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mgq.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://ruc.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hua.shuidangran.top

[Q06] 删除列
来源：http://blc.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://pde.zhengqikj.top

[Q07] 删除表
来源：http://kyr.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://nxx.sxryk.cn

[Q08] 创建普通索引
来源：http://whx.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qoe.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://boy.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghf.yanxiufei.cn

[Q10] 插入单行
来源：http://cop.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iju.yanxiufei.cn

[Q11] 一次插入多行
来源：http://lhd.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qoi.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://qbp.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cpm.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nub.bjfxy.top

[Q13] 忽略重复插入
来源：http://xsw.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ice.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://nzf.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zxs.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://soi.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://slm.haohaochexian.top

SELECT * FROM users;
来源：http://zhw.jinqigfzy.top

[Q16] 查询指定列
来源：http://abh.hysaishi.cn

SELECT id, name FROM users;
来源：http://sde.hnxiangtu.top

[Q17] 条件查询
来源：http://ryu.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vlq.tarul.cn

[Q18] 模糊匹配
来源：http://stv.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://auv.sjlbkw.cn

[Q19] 范围查询
来源：http://cen.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nqs.svipenyu.cn

[Q20] IN 列表
来源：http://acp.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ckx.svipenyu.cn

[Q21] 空值判断
来源：http://cdc.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pjj.jinqigufen.top

[Q22] 排序
来源：http://szp.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hvj.ppjwa.cn

[Q23] 分页
来源：http://rgj.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvo.jinyuanbaomall.cn

[Q24] 去重
来源：http://wwr.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://yom.xylfe.cn

[Q25] 只取前 N 条
来源：http://qdz.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://agz.ivvv.top

[Q26] 计数
来源：http://jdb.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://usz.sweek.top

[Q27] 条件计数
来源：http://sss.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://shl.gotoacloud.top

[Q28] 求和与平均
来源：http://ahj.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://npq.zdbjq.cn

[Q29] 最大最小值
来源：http://tyq.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://qvp.epnwcf.com

[Q30] 分组统计
来源：http://kst.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sud.0kj1m.cn

[Q31] 分组后过滤
来源：http://bmw.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yry.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://ifw.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ohc.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zfg.guowangkeji.top

[Q33] 多列分组
来源：http://ovl.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gkp.jinqigfzy.top

[Q34] 每组取第一条
来源：http://ixg.haohaochexian.top

SELECT * FROM (
来源：http://ysz.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qaj.svipenyu.cn

) t WHERE rn = 1;
来源：http://qwm.guannengcc.top

[Q35] 内连接
来源：http://tsv.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vtc.gogol.net.cn

[Q36] 左连接
来源：http://arf.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bar.yanxiufei.cn

[Q37] 右连接
来源：http://frq.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yhm.tianlin.xyz


<!-- 参考信息 -->