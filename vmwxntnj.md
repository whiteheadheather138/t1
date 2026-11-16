代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mir.zhijiandao.cn

Go:   go f()
来源：http://uwt.fengsongda.top

Ruby: Thread.new { f }
来源：http://xem.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://fdy.gaohongyu789.top

[O02] 使用线程池
来源：http://rte.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qzb.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zyb.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://okk.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://jeq.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://amr.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zvp.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cvu.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://btm.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://wrk.daxiang520.top

Py:   with lock: shared += 1
来源：http://tyn.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://irr.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yqa.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://bxq.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://glm.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dun.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpj.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://slc.wangdashe.top

[O04] 定义异步函数并等待
来源：http://xnd.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://dmz.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ksu.xinyue.icu

JS:   async function f() { await g(); }
来源：http://vev.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dpg.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xkm.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zwl.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ygj.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://nyd.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://zkq.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://fnf.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oax.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://ncp.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://tzc.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zca.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rsg.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://qrp.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tbx.guowangkeji.top

[O06] 使用进程池
来源：http://syx.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iie.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://vay.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://uuf.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://cfm.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kop.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://afz.cheryme.top

Ruby: // fork 块
来源：http://mgq.smart0.xyz

C#:   Parallel.For
来源：http://cgv.xylfe.cn

================================================================================
来源：http://col.xylfe.cn

P. 常用工具函数
来源：http://str.snrcjt.cn

================================================================================
来源：http://xqb.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://tth.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://fta.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hkn.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://svy.uphjek.com

TS:   crypto.randomUUID()
来源：http://nsp.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://aaa.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://bwl.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://tlx.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://ton.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://scc.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://suq.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tkm.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rod.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gvo.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://igs.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rpe.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gzs.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mji.yj20258.top

[P03] 生成短随机字符串
来源：http://ngi.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yed.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xha.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yfw.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgb.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://itd.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmd.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rqa.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qmk.sxryk.cn

[P04] 求长度
来源：http://dva.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jrg.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgf.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zub.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zhw.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://psz.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://jgo.hammf.cn

Ruby: x.length;  x.size
来源：http://mgi.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xao.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://vir.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://huw.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hml.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wkz.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mjp.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://alr.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rhs.zhijiandao.cn

Ruby: a == b
来源：http://pne.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hev.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://srw.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zig.pycfn.com

PHP:  if (empty($x)) {}
来源：http://afr.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bys.yuanzhike.top

TS:   if (x == null) {}
来源：http://cym.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://mzc.sweek.top

Go:   if x == nil {}
来源：http://jzj.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cdy.bjfxy.top

C#:   if (x is null) {}
来源：http://str.uphjek.com

[P07] 防抖与节流
来源：http://zyz.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nqz.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://xuv.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eey.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imv.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hbt.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wtx.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ngz.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ngc.yj20258888.top

[P08] 处理浮点精度问题
来源：http://aen.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kxj.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kpi.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cvu.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://als.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khu.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tum.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ryf.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eqk.hesvh.cn

================================================================================
来源：http://lyw.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xfs.guannengcc.top

================================================================================
来源：http://tmr.xuanzx.com

[Q01] 创建表
来源：http://hbh.chenjidiqi.icu

CREATE TABLE users (
来源：http://edq.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fij.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://emu.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://jin.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://erp.zdqjudy.top

);
来源：http://wzx.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://cao.shzxlz.cn

CREATE TABLE orders (
来源：http://hcr.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lxw.tarul.cn

user_id INT NOT NULL,
来源：http://wbz.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://kqi.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wyx.shuidangran.top

);
来源：http://ore.jqgufenzy.top

[Q03] 增加列
来源：http://eax.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjt.pengpengdd.cyou

[Q04] 修改列类型
来源：http://umd.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wgx.dianchejie.cn

[Q05] 重命名列
来源：http://xwj.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lam.havefunace.top

[Q06] 删除列
来源：http://kqp.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://ujh.jinqigufen.top

[Q07] 删除表
来源：http://efk.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://mlq.yj20258.top

[Q08] 创建普通索引
来源：http://cyh.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hjg.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://day.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jfq.gogol.net.cn

[Q10] 插入单行
来源：http://kfl.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wnm.sjlbkw.cn

[Q11] 一次插入多行
来源：http://ook.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bnz.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://bqx.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://tup.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vxu.yangfankeji.com

[Q13] 忽略重复插入
来源：http://yxs.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://daw.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://pce.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://evg.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wkb.fanxiaobao.xyz

[Q15] 查询全部
来源：http://mpu.fzhhl.top

SELECT * FROM users;
来源：http://jgg.zhongyouzk.top

[Q16] 查询指定列
来源：http://fhz.ehwqpu.com

SELECT id, name FROM users;
来源：http://mln.ehwqpu.com

[Q17] 条件查询
来源：http://nfl.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ldw.hnqzz.top

[Q18] 模糊匹配
来源：http://ghx.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mlw.316326.xyz

[Q19] 范围查询
来源：http://bbk.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://voq.mhx1999.top

[Q20] IN 列表
来源：http://unk.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dbr.yonumen.top

[Q21] 空值判断
来源：http://kvr.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ayj.jinghuilouyu.cn

[Q22] 排序
来源：http://rym.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mgf.andypj.xyz

[Q23] 分页
来源：http://ltk.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cyn.meibo888.top

[Q24] 去重
来源：http://grx.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://cog.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://ezh.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xzj.jqgufenzy.top

[Q26] 计数
来源：http://ycn.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://adt.daria6918.cn

[Q27] 条件计数
来源：http://xdq.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xpp.daxiang520.top

[Q28] 求和与平均
来源：http://few.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tsx.zhoulong.xyz

[Q29] 最大最小值
来源：http://mia.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ncr.jinghuilouyu.cn

[Q30] 分组统计
来源：http://zyn.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dff.yvedp.cn

[Q31] 分组后过滤
来源：http://ocm.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vyt.andypj.xyz

[Q32] 分组拼接字符串
来源：http://xat.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lpr.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bll.tian-w.cn

[Q33] 多列分组
来源：http://vys.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vbw.c1oappe.top

[Q34] 每组取第一条
来源：http://vxw.yj202588.top

SELECT * FROM (
来源：http://ljz.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zld.c1oappe.top

) t WHERE rn = 1;
来源：http://pbo.xylfe.cn

[Q35] 内连接
来源：http://qfo.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zqu.cdnleiting.top

[Q36] 左连接
来源：http://wkz.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pbl.gaohongyu789.top

[Q37] 右连接
来源：http://vgp.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nei.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://nmc.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cuw.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://kgr.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://unn.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vry.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hqt.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fol.yuanzhike.top

[Q41] 多表连接
来源：http://bdu.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mpr.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://jta.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://onh.yongpay.top

[Q42] 连接条件附加过滤
来源：http://jdx.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://uek.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wki.gogol.net.cn

[Q43] 标量子查询
来源：http://ufr.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uhk.bbcook.cn

[Q44] IN 子查询
来源：http://ifv.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://exw.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://ivz.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qyf.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://scv.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ria.aizwys.cn

[Q47] 与平均值比较
来源：http://hmg.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wpl.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://khd.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ata.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://gbj.xinyue.icu

[Q49] 更新单行
来源：http://atb.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qnb.fzhhl.top

[Q50] 批量更新
来源：http://mdf.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lvw.hammf.cn

[Q51] 用子查询更新
来源：http://lpm.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://min.smart0.xyz

[Q52] 删除指定行
来源：http://fez.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://avv.9152youxi.cn

[Q53] 按条件删除
来源：http://fyx.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xwj.gogol.net.cn

[Q54] 清空表
来源：http://fxy.xylfe.cn

TRUNCATE TABLE logs;
来源：http://qdi.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://lmd.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://szj.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://del.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cbg.hywenlv.cn

[Q57] 行号
来源：http://pds.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tlg.c1oappe.top

[Q58] 累计求和
来源：http://oak.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dkj.hywenlv.cn

[Q59] 分组内累计
来源：http://pbg.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nbw.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://thz.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jnr.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bia.bjfxy.top

[Q61] 移动平均
来源：http://rch.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ltd.nanxinkj.top

[Q62] 分组占比
来源：http://cco.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjd.sjlbkw.cn

[Q63] 开启事务
来源：http://rxj.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xgu.guannengcc.top

[Q64] 提交事务
来源：http://nnw.fengsongda.top

COMMIT;
来源：http://slm.xinyue.icu

[Q65] 回滚事务
来源：http://wbg.yj20258888.top

ROLLBACK;
来源：http://jhi.gogol.net.cn

[Q66] 行锁查询
来源：http://adt.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jit.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://fol.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sml.yueranfly.top

[Q68] 保存点
来源：http://qnc.52xcode.cn

SAVEPOINT sp1;
来源：http://rdh.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://rlb.jyoumei.cn

[Q69] 查看执行计划
来源：http://upt.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://znj.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://fsd.nanxinkj.top

ANALYZE TABLE users;
来源：http://xzn.zhongyouzk.top

[Q71] 查看建表语句
来源：http://tkc.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xxg.shuidangran.top

[Q72] 查看索引
来源：http://utf.yuanzhike.top

SHOW INDEX FROM users;
来源：http://lub.svipenyu.cn

[Q73] 查看表状态
来源：http://dqj.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xhk.gzhubu.top

[Q74] 强制使用索引
来源：http://tnx.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mmn.jianghu66.top

[Q75] 日期格式化
来源：http://clm.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://krs.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ezp.xuetiantiany.cn


<!-- 参考信息 -->