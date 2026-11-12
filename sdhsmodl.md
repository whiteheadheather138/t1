代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bcs.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxp.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://ioh.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://lhr.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uri.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ejl.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://lsf.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dhb.sysykeji.top

PHP:  // 手写递归函数
来源：http://nne.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://viy.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qkw.zdqjudy.top

Java: // 手写递归
来源：http://tzm.hfpthk.cn

Go:   // 手写递归
来源：http://lgj.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fqc.yueranfly.top

C#:   // 手写递归
来源：http://hwl.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jss.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pks.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dzd.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wou.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cuk.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qof.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://snh.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lay.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eim.jqgufenzy.top

================================================================================
来源：http://usc.jyoumei.cn

O. 并发与异步
来源：http://rgg.gotoacloud.top

================================================================================
来源：http://mhn.sweek.top

[O01] 启动一个线程
来源：http://wrj.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fda.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ejy.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wow.fktsv.cn

TS:   // 同 JS
来源：http://iuo.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://waq.yvedp.cn

Go:   go f()
来源：http://aqi.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://qks.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://kbr.haohaochexian.top

[O02] 使用线程池
来源：http://bsn.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hoh.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dst.cucudq.cn

JS:   // worker_threads 线程池
来源：http://syh.c1oappe.top

TS:   // worker_threads 线程池
来源：http://ohg.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://eae.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cqg.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xkq.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jpj.daxiang520.top

[O03] 加锁保护共享数据
来源：http://ibp.jinqigufen.top

Py:   with lock: shared += 1
来源：http://dfj.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://aqk.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qnj.ydjk.org.cn

TS:   // 同 JS
来源：http://vob.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://fyc.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sre.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://olw.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://gtq.wangdashe.top

[O04] 定义异步函数并等待
来源：http://svp.tarul.cn

Py:   async def f():⏎    await g()
来源：http://pdf.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rmk.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://fxt.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bvh.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uee.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fuj.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://gpi.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://ydr.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://iyl.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://tii.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gjv.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://bgg.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://gde.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dlp.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtz.aizwys.cn

Ruby: threads.map(&:join)
来源：http://ppu.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pjk.yj20258888.top

[O06] 使用进程池
来源：http://stn.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yyx.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fod.hammf.cn

JS:   // child_process / cluster 模块
来源：http://rdu.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://vpr.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmg.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://skq.xylfe.cn

Ruby: // fork 块
来源：http://mun.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://stn.birdmap.top

================================================================================
来源：http://jph.yanxiufei.cn

P. 常用工具函数
来源：http://khp.guowangkeji.top

================================================================================
来源：http://pew.9152youxi.cn

[P01] 生成 UUID
来源：http://fue.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://itn.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzp.daria6918.cn

JS:   crypto.randomUUID()
来源：http://hxo.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://mkl.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://eyg.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://cka.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://jzc.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://vpl.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://zrd.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fse.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yqa.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wlo.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://onp.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ulx.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcp.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://frf.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vtu.yj20258888.top

[P03] 生成短随机字符串
来源：http://fbx.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xdd.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://czs.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fby.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gau.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yew.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://udg.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vfx.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fdk.xylfe.cn

[P04] 求长度
来源：http://xyt.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qff.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcz.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rep.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pnz.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://sfr.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://hsd.guannengcc.top

Ruby: x.length;  x.size
来源：http://hqu.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gjx.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://hsp.jinqigfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iyg.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ysr.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://utb.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qrk.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nyq.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://fho.jqgufenzy.top

Ruby: a == b
来源：http://njv.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hxr.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tpe.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jph.shuidangran.top

PHP:  if (empty($x)) {}
来源：http://zxy.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jmn.daria6918.cn

TS:   if (x == null) {}
来源：http://brk.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qlg.cdnleiting.top

Go:   if x == nil {}
来源：http://cyu.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eqt.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://bbr.hnxiangtu.top

[P07] 防抖与节流
来源：http://rhc.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hlt.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://lpd.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynb.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vkc.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fxu.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pad.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://tvo.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zea.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://lyq.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vtf.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ifz.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cmd.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://equ.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uzf.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dnw.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hqq.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uxd.guannengcc.top

================================================================================
来源：http://qsw.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jhw.vehdjk.com

================================================================================
来源：http://gfd.cheryme.top

[Q01] 创建表
来源：http://tln.havefunace.top

CREATE TABLE users (
来源：http://olg.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqe.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://cpx.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://mvr.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jkd.nanxinkj.top

);
来源：http://his.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://lqn.jlsjyb.cn

CREATE TABLE orders (
来源：http://iiv.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xvd.ydjk.org.cn

user_id INT NOT NULL,
来源：http://yop.ivvv.top

amount DECIMAL(10, 2),
来源：http://wci.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uhk.nwbrower.top

);
来源：http://hom.sjlbkw.cn

[Q03] 增加列
来源：http://pdf.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://toa.sweek.top

[Q04] 修改列类型
来源：http://sjx.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hba.sufxvd.cn

[Q05] 重命名列
来源：http://bhm.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xxh.fehbvm.com

[Q06] 删除列
来源：http://uds.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qee.sxryk.cn

[Q07] 删除表
来源：http://amb.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://dsq.c1oappe.top

[Q08] 创建普通索引
来源：http://pjb.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://urd.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://blz.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vcr.fengsongda.top

[Q10] 插入单行
来源：http://cpw.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dzp.fengsongda.top

[Q11] 一次插入多行
来源：http://axh.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://url.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://qmh.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ljg.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ekt.tianlin.xyz

[Q13] 忽略重复插入
来源：http://omw.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jls.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://wiz.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kfw.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zbk.jqgfzy.top

[Q15] 查询全部
来源：http://ixq.feifeiyinyue.top

SELECT * FROM users;
来源：http://bau.yfazqb.com

[Q16] 查询指定列
来源：http://uzw.meibo888.top

SELECT id, name FROM users;
来源：http://fdc.nanxuanxn.top

[Q17] 条件查询
来源：http://jgb.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://irp.guannengcc.top

[Q18] 模糊匹配
来源：http://gzq.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hwk.shanyushiyangtech.top

[Q19] 范围查询
来源：http://tte.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dnx.andypj.xyz

[Q20] IN 列表
来源：http://ylp.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qkz.gaohongyu789.top

[Q21] 空值判断
来源：http://ocg.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zyu.sufxvd.cn

[Q22] 排序
来源：http://ccf.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://owf.zhijiandao.cn

[Q23] 分页
来源：http://ikp.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://suq.tanke756.top

[Q24] 去重
来源：http://wxm.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://gnu.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://vpj.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xze.tianlin.xyz

[Q26] 计数
来源：http://ccw.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://ivd.svipenyu.cn

[Q27] 条件计数
来源：http://nbr.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cio.yj20258.top

[Q28] 求和与平均
来源：http://lak.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dhj.bbcook.cn

[Q29] 最大最小值
来源：http://rzk.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xrb.sxryk.cn

[Q30] 分组统计
来源：http://xtk.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kqp.jqgufenzy.top

[Q31] 分组后过滤
来源：http://sck.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yxt.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://bup.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xfo.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rpu.chenzaomai.com

[Q33] 多列分组
来源：http://ega.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tbx.cqqwz.cn

[Q34] 每组取第一条
来源：http://rgt.sxryk.cn

SELECT * FROM (
来源：http://oba.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ply.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://dqf.cqqwz.cn

[Q35] 内连接
来源：http://wxs.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xqj.xuanzx.com

[Q36] 左连接
来源：http://jga.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wtc.chenlongwang.top

[Q37] 右连接
来源：http://zis.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kot.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://dya.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://beu.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://ffp.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uos.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fsj.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://heo.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mez.jinqigufen.top

[Q41] 多表连接
来源：http://elx.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jbv.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://unr.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://vsv.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://icd.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://sds.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qum.shzxlz.cn

[Q43] 标量子查询
来源：http://qvc.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rxy.sxryk.cn

[Q44] IN 子查询
来源：http://oej.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zri.316326.xyz

[Q45] EXISTS 判断存在
来源：http://muh.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://res.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qih.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wrc.daxiang520.top

[Q47] 与平均值比较
来源：http://bbn.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jjw.yj202588.top

[Q48] CTE 公用表表达式
来源：http://xfz.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://emq.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://lme.tanke756.top

[Q49] 更新单行
来源：http://ubm.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://moh.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://krc.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://erz.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://hrj.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yli.xuetiantiany.cn

[Q52] 删除指定行
来源：http://gtf.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://gcs.zhongyouzk.top

[Q53] 按条件删除
来源：http://zcx.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yej.sufxvd.cn

[Q54] 清空表
来源：http://jtz.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://flo.xylfe.cn

[Q55] 排名（并列占位）
来源：http://ket.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://npx.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://hkc.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eam.52xcode.cn

[Q57] 行号
来源：http://alm.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qnb.yfazqb.com

[Q58] 累计求和
来源：http://blq.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zfe.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://vsz.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ktg.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://roq.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ntp.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eov.jqgfzy.top


<!-- 参考信息 -->