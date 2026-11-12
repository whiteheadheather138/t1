代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yis.dashuyun.cn

[N10] 链表节点定义
来源：http://sdm.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kgs.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://irf.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lmw.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lqf.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://fke.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sqv.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wvm.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://hiz.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://sxz.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ouz.zycfv.cn

PHP:  // 手写递归函数
来源：http://zqz.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqq.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dba.jlsjyb.cn

Java: // 手写递归
来源：http://jai.zhijiandao.cn

Go:   // 手写递归
来源：http://zcg.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cjc.bjfxy.top

C#:   // 手写递归
来源：http://mcr.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bsv.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ltx.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://swh.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://get.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gtj.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kza.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xng.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wfm.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rvy.zycfv.cn

================================================================================
来源：http://idh.ydzc1.top

O. 并发与异步
来源：http://fje.nanxuanxn.top

================================================================================
来源：http://var.epnwcf.com

[O01] 启动一个线程
来源：http://ppz.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://keg.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ygl.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zjn.jinghuilouyu.cn

TS:   // 同 JS
来源：http://wfd.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://ddt.nanxinkj.top

Go:   go f()
来源：http://yok.meibo888.top

Ruby: Thread.new { f }
来源：http://hoo.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://dzt.ydjk.org.cn

[O02] 使用线程池
来源：http://awq.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eod.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rwu.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://dsv.ivvv.top

TS:   // worker_threads 线程池
来源：http://cxn.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://elz.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wzw.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gtz.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ebj.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://tqh.snrcjt.cn

Py:   with lock: shared += 1
来源：http://bdu.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://mly.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wqs.hywenlv.cn

TS:   // 同 JS
来源：http://hqh.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://svb.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gwa.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kfx.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://wvr.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://ctq.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://oac.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qms.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://jun.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qff.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lru.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ldr.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://jso.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://oqe.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://ssy.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://klu.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jxc.yongpay.top

JS:   await Promise.all(tasks)
来源：http://poy.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://sgb.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ged.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iqc.hcnkem.com

Ruby: threads.map(&:join)
来源：http://xgq.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lpq.zdqjudy.top

[O06] 使用进程池
来源：http://rkr.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dtt.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mlf.tarul.cn

JS:   // child_process / cluster 模块
来源：http://ffk.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://yoc.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kgn.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pvq.jianghu66.top

Ruby: // fork 块
来源：http://qmz.cqqwz.cn

C#:   Parallel.For
来源：http://qtl.fktsv.cn

================================================================================
来源：http://wav.yj20258.top

P. 常用工具函数
来源：http://jsu.shangyingyoupin.top

================================================================================
来源：http://mga.yanxiufei.cn

[P01] 生成 UUID
来源：http://muw.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://mgj.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://asv.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://oum.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://xyr.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://ccc.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://jmr.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://xsg.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://qfc.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://ikl.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xre.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mlq.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zgg.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zjt.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pag.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khh.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sgz.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sni.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://met.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xqz.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://icx.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvi.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyc.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mfe.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dco.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xsw.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fso.guowangkeji.top

[P04] 求长度
来源：http://fjc.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxk.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rhv.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfg.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvs.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://pmm.yueranfly.top

Go:   len(arr);  len(m)
来源：http://gar.uphjek.com

Ruby: x.length;  x.size
来源：http://hlf.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rqf.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://zke.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://upj.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xbm.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zqe.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bfw.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qko.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://zem.ctjpmb.com

Ruby: a == b
来源：http://chm.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tqf.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gqp.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ond.yonumen.top

PHP:  if (empty($x)) {}
来源：http://hrc.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mrs.bbcook.cn

TS:   if (x == null) {}
来源：http://dml.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xsj.shuidangran.top

Go:   if x == nil {}
来源：http://iwx.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kma.shuidangran.top

C#:   if (x is null) {}
来源：http://ypc.jlsjyb.cn

[P07] 防抖与节流
来源：http://dvf.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://frl.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://duk.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcs.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aum.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dmx.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xea.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lpb.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xvw.uphjek.com

[P08] 处理浮点精度问题
来源：http://tiq.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cak.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cwp.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ldw.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gsv.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rou.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ghn.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crv.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ymz.gaohongyu789.top

================================================================================
来源：http://snz.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pkk.dashuyun.cn

================================================================================
来源：http://qgc.tanke756.top

[Q01] 创建表
来源：http://jwr.fengsongda.top

CREATE TABLE users (
来源：http://vde.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dmz.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://lob.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://hee.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hgq.zhongyouzk.top

);
来源：http://lkl.ppjwa.cn

[Q02] 创建带外键的表
来源：http://pws.cdnleiting.top

CREATE TABLE orders (
来源：http://rmm.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbb.zycfv.cn

user_id INT NOT NULL,
来源：http://eys.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://tqj.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xfw.jiagoushi.top

);
来源：http://agp.pengpengdd.cyou

[Q03] 增加列
来源：http://kgl.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rru.zycfv.cn

[Q04] 修改列类型
来源：http://dck.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xvz.hammf.cn

[Q05] 重命名列
来源：http://qfl.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gig.fktsv.cn

[Q06] 删除列
来源：http://gce.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://unt.ydjk.org.cn

[Q07] 删除表
来源：http://xza.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://fbd.tianlin.xyz

[Q08] 创建普通索引
来源：http://ccl.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cxu.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://hlb.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oul.0kj1m.cn

[Q10] 插入单行
来源：http://wrm.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pfo.smart0.xyz

[Q11] 一次插入多行
来源：http://cwl.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbx.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://nje.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://eze.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xwc.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://zlj.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dho.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://fim.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vld.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tmu.guowangkeji.top

[Q15] 查询全部
来源：http://kut.zhiwuduotai.top

SELECT * FROM users;
来源：http://jkw.hammf.cn

[Q16] 查询指定列
来源：http://mdj.52xcode.cn

SELECT id, name FROM users;
来源：http://xxu.gaohongyu789.top

[Q17] 条件查询
来源：http://sdv.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rxx.dashuyun.cn

[Q18] 模糊匹配
来源：http://fip.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://upj.chenjidiqi.icu

[Q19] 范围查询
来源：http://aoh.fktsv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vld.vehdjk.com

[Q20] IN 列表
来源：http://qjt.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sao.yonumen.top

[Q21] 空值判断
来源：http://gpg.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cwf.zhoulong.xyz

[Q22] 排序
来源：http://edm.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cpy.haohaochexian.top

[Q23] 分页
来源：http://rdm.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wns.hysaishi.cn

[Q24] 去重
来源：http://ush.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://jkc.haohaochexian.top

[Q25] 只取前 N 条
来源：http://uby.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mbq.vehdjk.com

[Q26] 计数
来源：http://jwh.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://stw.hfpthk.cn

[Q27] 条件计数
来源：http://rct.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aww.mhx1999.top

[Q28] 求和与平均
来源：http://tvr.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hix.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://xtk.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vxj.zhoulong.xyz

[Q30] 分组统计
来源：http://sfn.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wde.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://ldf.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mis.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://qgj.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://miy.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dnr.kuanghao11.cn

[Q33] 多列分组
来源：http://zpi.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dgt.jyoumei.cn

[Q34] 每组取第一条
来源：http://gge.smart0.xyz

SELECT * FROM (
来源：http://fth.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zlw.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://gfk.gaohongyu789.top

[Q35] 内连接
来源：http://afy.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfs.sysykeji.top

[Q36] 左连接
来源：http://zxa.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mbv.yuanzhike.top

[Q37] 右连接
来源：http://gpt.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rdd.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://qty.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bqn.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://lby.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jpx.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xwf.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nam.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qov.chenlongwang.top

[Q41] 多表连接
来源：http://crd.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://neu.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://bie.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://ylp.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://mdm.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://pom.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://imi.feifeiyinyue.top

[Q43] 标量子查询
来源：http://wxe.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uue.52xcode.cn

[Q44] IN 子查询
来源：http://tag.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gzc.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://kob.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvz.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://acu.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eln.vehdjk.com

[Q47] 与平均值比较
来源：http://tlq.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xey.uphjek.com

[Q48] CTE 公用表表达式
来源：http://cek.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oxy.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://zux.sysykeji.top

[Q49] 更新单行
来源：http://miq.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://odx.fzhhl.top

[Q50] 批量更新
来源：http://ndo.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://knh.meibo888.top

[Q51] 用子查询更新
来源：http://ocv.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wyr.cheryme.top

[Q52] 删除指定行
来源：http://qzo.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://srs.ctjpmb.com

[Q53] 按条件删除
来源：http://wsi.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hhd.zhaomingkeji.xyz

[Q54] 清空表
来源：http://spc.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://hif.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://hnk.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qka.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://oye.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xoj.jqgufenzy.top

[Q57] 行号
来源：http://cji.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgi.zhengqikj.top

[Q58] 累计求和
来源：http://mjh.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lry.chenjidiqi.icu

[Q59] 分组内累计
来源：http://yyc.chenjidiqi.icu


<!-- 参考信息 -->