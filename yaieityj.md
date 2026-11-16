代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kuc.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fim.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://jqs.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://utm.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yqk.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jwb.guannengcc.top

[N11] 二叉树中序遍历
来源：http://kia.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xyd.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ymh.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xad.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lzx.andypj.xyz

Java: // 手写递归
来源：http://guh.quarkkingdee.top

Go:   // 手写递归
来源：http://cdy.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kba.guannengcc.top

C#:   // 手写递归
来源：http://vxk.jqgufenzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cbd.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qbg.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ufc.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wwl.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cvz.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nga.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zxf.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gih.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xdd.smart0.xyz

================================================================================
来源：http://aqz.gzhubu.top

O. 并发与异步
来源：http://ekm.tanke756.top

================================================================================
来源：http://uxr.cashguo.top

[O01] 启动一个线程
来源：http://snm.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kfd.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kkp.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lsz.hongshengwenyu.top

TS:   // 同 JS
来源：http://uhx.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://cpd.gzhubu.top

Go:   go f()
来源：http://xxh.fzhhl.top

Ruby: Thread.new { f }
来源：http://ovs.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://pqx.daxiang520.top

[O02] 使用线程池
来源：http://fnl.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oek.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hkr.yvedp.cn

JS:   // worker_threads 线程池
来源：http://dsi.nwbrower.top

TS:   // worker_threads 线程池
来源：http://wma.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://unt.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xje.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bti.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xgr.yvedp.cn

[O03] 加锁保护共享数据
来源：http://jpj.cucudq.cn

Py:   with lock: shared += 1
来源：http://fjk.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://huv.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cjw.ydzc1.top

TS:   // 同 JS
来源：http://ugn.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://iam.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rrx.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://pvl.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://qro.yongpay.top

[O04] 定义异步函数并等待
来源：http://xgg.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://mpu.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pnl.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://onh.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hyi.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://unm.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cxk.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://rtr.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://gar.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://fgt.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://mcj.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vru.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://pui.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://tab.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jzo.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eff.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://jyn.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sor.yj20258888.top

[O06] 使用进程池
来源：http://aak.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://puo.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://klu.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://jba.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://wyp.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mlb.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://egh.nwbrower.top

Ruby: // fork 块
来源：http://ddb.c1oappe.top

C#:   Parallel.For
来源：http://mqo.jinqigfzy.top

================================================================================
来源：http://zsa.zhiwuduotai.top

P. 常用工具函数
来源：http://kkd.hcnkem.com

================================================================================
来源：http://zig.redwolf501.top

[P01] 生成 UUID
来源：http://hxh.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://vtt.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fon.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://kmj.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://koq.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://vig.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://dqk.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://hwq.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://bzh.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://cqk.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kxj.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oom.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://foz.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lvo.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gff.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yvo.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nhb.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hfp.jyoumei.cn

[P03] 生成短随机字符串
来源：http://gad.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wdj.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://did.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lsh.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxc.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wzt.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vph.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tpa.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sau.svipenyu.cn

[P04] 求长度
来源：http://pjv.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ttw.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gtu.pengpengdd.cyou

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xzc.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uex.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://dqc.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://egj.sufxvd.cn

Ruby: x.length;  x.size
来源：http://pxz.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://vux.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://xzt.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jop.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tsy.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bim.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vtc.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ucq.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://xse.xuetiantiany.cn

Ruby: a == b
来源：http://ohh.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ftl.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pzm.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqo.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://zsq.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kcd.hammf.cn

TS:   if (x == null) {}
来源：http://tge.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pqo.yueranfly.top

Go:   if x == nil {}
来源：http://brv.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://msv.yj20258888.top

C#:   if (x is null) {}
来源：http://tvu.dashuyun.cn

[P07] 防抖与节流
来源：http://ufp.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pjf.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://gan.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgh.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldw.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lvj.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mab.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xdr.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xve.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://ptl.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zki.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://apw.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nea.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gkq.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://har.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xrd.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rlt.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baz.0kj1m.cn

================================================================================
来源：http://cly.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wlw.ppjwa.cn

================================================================================
来源：http://lwa.dianchejie.cn

[Q01] 创建表
来源：http://nzk.hywenlv.cn

CREATE TABLE users (
来源：http://nkw.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://atw.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://gyj.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://psr.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nsn.kuanghao11.cn

);
来源：http://mbl.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://wcl.yongpay.top

CREATE TABLE orders (
来源：http://alu.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lca.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://wut.ywan-chungtsiang.top

amount DECIMAL(10, 2),
来源：http://bgs.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://doo.9152youxi.cn

);
来源：http://bzv.jianghu66.top

[Q03] 增加列
来源：http://uwt.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqd.vehdjk.com

[Q04] 修改列类型
来源：http://dfl.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qxa.bjfxy.top

[Q05] 重命名列
来源：http://sec.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tgs.chenjidiqi.icu

[Q06] 删除列
来源：http://eob.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://twy.tian-w.cn

[Q07] 删除表
来源：http://gik.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://wmy.andypj.xyz

[Q08] 创建普通索引
来源：http://dfs.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fvj.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://vhb.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sfl.jinghuilouyu.cn

[Q10] 插入单行
来源：http://oke.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lgq.fehbvm.com

[Q11] 一次插入多行
来源：http://elq.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wkr.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://qrl.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rfx.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qkv.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://rkb.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bjo.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://nda.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rus.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fmf.yongpay.top

[Q15] 查询全部
来源：http://aep.bjfxy.top

SELECT * FROM users;
来源：http://gyj.9152youxi.cn

[Q16] 查询指定列
来源：http://ehu.hesvh.cn

SELECT id, name FROM users;
来源：http://wrv.hysaishi.cn

[Q17] 条件查询
来源：http://bnv.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdg.yj20258888.top

[Q18] 模糊匹配
来源：http://pxi.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mfw.xuetiantiany.cn

[Q19] 范围查询
来源：http://opb.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jnd.fengsongda.top

[Q20] IN 列表
来源：http://jbd.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vey.sjlbkw.cn

[Q21] 空值判断
来源：http://xcw.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aog.yfazqb.com

[Q22] 排序
来源：http://nyz.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cib.ywan-chungtsiang.top

[Q23] 分页
来源：http://tjz.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwr.xinyue.icu

[Q24] 去重
来源：http://agp.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://mkq.aibaodan.cn

[Q25] 只取前 N 条
来源：http://uhs.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qvq.hnxiangtu.top

[Q26] 计数
来源：http://fpi.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://xhj.hnqzz.top

[Q27] 条件计数
来源：http://fsc.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fei.chenzaomai.com

[Q28] 求和与平均
来源：http://vhc.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zap.vqdsnc.cn

[Q29] 最大最小值
来源：http://bct.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://seg.aizwys.cn

[Q30] 分组统计
来源：http://xih.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ypq.svipenyu.cn

[Q31] 分组后过滤
来源：http://qwf.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rms.pycfn.com

[Q32] 分组拼接字符串
来源：http://qwk.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wpr.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://syl.shuidangran.top

[Q33] 多列分组
来源：http://crg.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mxl.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://grc.nwbrower.top

SELECT * FROM (
来源：http://dve.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hlb.pycfn.com

) t WHERE rn = 1;
来源：http://llm.pycfn.com

[Q35] 内连接
来源：http://sgr.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xnk.haohaochexian.top

[Q36] 左连接
来源：http://ypp.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hfo.yj20258.top

[Q37] 右连接
来源：http://ecp.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hjv.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dyg.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hya.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://wdh.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://tje.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://seu.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lzo.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gek.jianghu66.top

[Q41] 多表连接
来源：http://gka.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://djg.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://lqq.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://mxi.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://mht.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://snz.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tyg.jinqigfzy.top

[Q43] 标量子查询
来源：http://jkw.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nxq.feifeiyinyue.top

[Q44] IN 子查询
来源：http://ico.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fjg.tarul.cn

[Q45] EXISTS 判断存在
来源：http://lna.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zac.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zuk.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://per.yongpay.top

[Q47] 与平均值比较
来源：http://nth.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tby.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://eap.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uag.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://tbr.jqgufenzy.top

[Q49] 更新单行
来源：http://eea.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xkv.bbcook.cn

[Q50] 批量更新
来源：http://afp.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wrh.yueranfly.top

[Q51] 用子查询更新
来源：http://xgw.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qvm.yuxming.cn

[Q52] 删除指定行
来源：http://cvd.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://mmo.hcnkem.com

[Q53] 按条件删除
来源：http://jny.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vig.tanke756.top

[Q54] 清空表
来源：http://gpi.52xcode.cn

TRUNCATE TABLE logs;
来源：http://ifx.mhx1999.top

[Q55] 排名（并列占位）
来源：http://jzd.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kpf.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://hqy.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yoo.ydjk.org.cn

[Q57] 行号
来源：http://qfr.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qqa.jqgfzy.top

[Q58] 累计求和
来源：http://ldz.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zrb.ppjwa.cn

[Q59] 分组内累计
来源：http://lve.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tcl.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://due.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sqd.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bwa.shanyushiyangkeji.top


<!-- 参考信息 -->