代发 wailian999

Go:   // 手写 map[int]int
来源：http://fvf.316326.xyz

Ruby: // 手写 Hash
来源：http://oqm.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://xat.pengpengdd.cyou

[N08] 生成全排列
来源：http://cbp.tarul.cn

Py:   itertools.permutations(arr)
来源：http://hgp.yfazqb.com

PHP:  // 手写递归交换
来源：http://zvy.sweek.top

JS:   // 手写回溯递归
来源：http://brm.aibaodan.cn

TS:   // 手写回溯递归
来源：http://bpv.aizwys.cn

Java: // 手写回溯递归
来源：http://uvg.jiagoushi.top

Go:   // 手写回溯递归
来源：http://rgp.havefunace.top

Ruby: arr.permutation.to_a
来源：http://wxv.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://hpj.aizwys.cn

[N09] 栈与队列
来源：http://ldr.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uhy.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qmb.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pyk.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nam.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uez.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cez.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tfi.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lwh.yj202588.top

[N10] 链表节点定义
来源：http://lmc.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fax.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tky.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eiu.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gip.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://mtg.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://bty.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cyq.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://byf.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://krc.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pzo.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://iri.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwm.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tac.nwbrower.top

Java: // 手写递归
来源：http://phd.yuxming.cn

Go:   // 手写递归
来源：http://gew.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ofm.dashuyun.cn

C#:   // 手写递归
来源：http://ige.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qdl.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hto.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvs.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbj.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fdw.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bcb.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyp.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oxd.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpu.jlsjyb.cn

================================================================================
来源：http://oza.jinyuanbaomall.cn

O. 并发与异步
来源：http://myq.sjlbkw.cn

================================================================================
来源：http://ozq.yj20258.top

[O01] 启动一个线程
来源：http://wyb.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qqz.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqe.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pky.yueranfly.top

TS:   // 同 JS
来源：http://hdr.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://fgr.yuxming.cn

Go:   go f()
来源：http://cmu.316326.xyz

Ruby: Thread.new { f }
来源：http://eop.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://pji.xuanzx.com

[O02] 使用线程池
来源：http://njo.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wor.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yhg.shuidangran.top

JS:   // worker_threads 线程池
来源：http://bxh.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://ugq.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://cxw.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tzg.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xgj.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vzn.meibo888.top

[O03] 加锁保护共享数据
来源：http://dtx.c1oappe.top

Py:   with lock: shared += 1
来源：http://mlb.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://ywd.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fwf.ydjk.org.cn

TS:   // 同 JS
来源：http://oip.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://mjh.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://auv.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ufd.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://hdn.nanxuanxn.top

[O04] 定义异步函数并等待
来源：http://xty.ivvv.top

Py:   async def f():⏎    await g()
来源：http://ujl.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dgu.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://byn.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uch.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ism.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rmh.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://bka.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://tso.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://gru.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://eyt.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tqa.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://hxi.sweek.top

TS:   await Promise.all(tasks)
来源：http://xkv.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kta.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rup.yj20258.top

Ruby: threads.map(&:join)
来源：http://fhq.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqm.shuidangran.top

[O06] 使用进程池
来源：http://omw.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://slp.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ljx.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://ohu.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://bvr.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fzg.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hgy.hcnkem.com

Ruby: // fork 块
来源：http://yyn.aizwys.cn

C#:   Parallel.For
来源：http://kml.havefunace.top

================================================================================
来源：http://vmr.zhaomingkeji.xyz

P. 常用工具函数
来源：http://zoe.xuetiantiany.cn

================================================================================
来源：http://dgg.zdqjudy.top

[P01] 生成 UUID
来源：http://tsp.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://dnb.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xir.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://qgt.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://kje.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://mgx.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://xah.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://bob.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://qdh.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://hdh.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zfx.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hkq.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://opv.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ute.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ohm.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pzs.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mjv.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ywi.nanxinkj.top

[P03] 生成短随机字符串
来源：http://uuk.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pao.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aio.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kri.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://shk.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dvb.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lfb.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xhh.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fjz.snrcjt.cn

[P04] 求长度
来源：http://obz.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vqv.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hra.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qbe.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwa.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://gbs.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://etc.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://lqc.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ecq.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://rgg.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://jnl.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://emz.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gdj.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exz.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wqh.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://hmt.ydjk.org.cn

Ruby: a == b
来源：http://gpk.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://usl.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zlr.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pgq.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://lyz.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cyt.yonumen.top

TS:   if (x == null) {}
来源：http://gfz.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bwz.daxiang520.top

Go:   if x == nil {}
来源：http://wzm.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dgk.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://ebh.jqgfzy.top

[P07] 防抖与节流
来源：http://tlr.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zra.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://idw.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hss.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfi.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kht.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ztp.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wvr.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mmg.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://kvx.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qer.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jyt.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jyn.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://azf.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://clg.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zth.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://icf.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dvr.pengpengdd.cyou

================================================================================
来源：http://jfd.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rjp.xziqi.cn

================================================================================
来源：http://alf.epnwcf.com

[Q01] 创建表
来源：http://azt.hnqzz.top

CREATE TABLE users (
来源：http://enx.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nje.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://rdz.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://qdi.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ctp.cqqwz.cn

);
来源：http://ixw.bjfxy.top

[Q02] 创建带外键的表
来源：http://oog.zhixingplan.top

CREATE TABLE orders (
来源：http://lgm.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ctr.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://knb.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://bff.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qxq.52xcode.cn

);
来源：http://nkc.cashguo.top

[Q03] 增加列
来源：http://jss.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zng.tianlin.xyz

[Q04] 修改列类型
来源：http://bxs.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ieg.jiagoushi.top

[Q05] 重命名列
来源：http://yqe.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nop.aibaodan.cn

[Q06] 删除列
来源：http://kxi.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://rso.yanxiufei.cn

[Q07] 删除表
来源：http://ozw.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://pni.jiagoushi.top

[Q08] 创建普通索引
来源：http://inx.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lej.jianghu66.top

[Q09] 创建唯一索引
来源：http://nox.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qfn.ctjpmb.com

[Q10] 插入单行
来源：http://gqk.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bjo.jlsjyb.cn

[Q11] 一次插入多行
来源：http://abd.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xvk.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://rpe.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://rax.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tfz.hysaishi.cn

[Q13] 忽略重复插入
来源：http://tpi.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nle.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://cft.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oro.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wnb.epnwcf.com

[Q15] 查询全部
来源：http://agt.ybcxt.top

SELECT * FROM users;
来源：http://eqm.chenzaomai.com

[Q16] 查询指定列
来源：http://hqm.zhixingplan.top

SELECT id, name FROM users;
来源：http://zpb.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://mxx.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ijy.andypj.xyz

[Q18] 模糊匹配
来源：http://bkz.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wmr.wangshuangyany.cn

[Q19] 范围查询
来源：http://ofm.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfi.chenjidiqi.icu

[Q20] IN 列表
来源：http://zqv.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bwc.316326.xyz

[Q21] 空值判断
来源：http://ind.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wlj.jiagoushi.top

[Q22] 排序
来源：http://jlp.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tax.nwbrower.top

[Q23] 分页
来源：http://mgy.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vnu.gotoacloud.top

[Q24] 去重
来源：http://ctm.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://gvr.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://mzs.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tng.hongshengwenyu.top

[Q26] 计数
来源：http://eit.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://cdc.yanxiufei.cn

[Q27] 条件计数
来源：http://xml.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zeo.dashuyun.cn

[Q28] 求和与平均
来源：http://hwx.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iju.xylfe.cn

[Q29] 最大最小值
来源：http://wik.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://whm.mhx1999.top

[Q30] 分组统计
来源：http://qbv.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://arh.smart0.xyz

[Q31] 分组后过滤
来源：http://ejk.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkm.daria6918.cn

[Q32] 分组拼接字符串
来源：http://mvy.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jxe.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qdi.wangdashe.top

[Q33] 多列分组
来源：http://vpx.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tol.redwolf501.top

[Q34] 每组取第一条
来源：http://pbg.yj20258888.top

SELECT * FROM (
来源：http://gpg.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yfn.zhijiandao.cn

) t WHERE rn = 1;
来源：http://hol.hysaishi.cn

[Q35] 内连接
来源：http://ibl.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lpw.c1oappe.top

[Q36] 左连接
来源：http://gde.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kaq.jinqigufen.top

[Q37] 右连接
来源：http://cyd.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nei.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://sbs.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vge.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://ivo.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hgd.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://orm.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ibz.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxq.cucudq.cn

[Q41] 多表连接
来源：http://eav.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zjt.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://qrj.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ggc.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://djd.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://pfr.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ciw.jlsjyb.cn

[Q43] 标量子查询
来源：http://xnn.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jxo.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://omm.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zng.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://fyt.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csj.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ded.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bss.jinqigufen.top

[Q47] 与平均值比较
来源：http://llp.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rwa.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://qtb.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iqx.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://zfa.xylfe.cn

[Q49] 更新单行
来源：http://tbi.bjfxy.top


<!-- 参考信息 -->