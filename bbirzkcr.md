代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://pog.dashuyun.cn

Go:   go f()
来源：http://puu.52xcode.cn

Ruby: Thread.new { f }
来源：http://ezi.ydzc1.top

C#:   Task.Run(() => F());
来源：http://zcx.yfazqb.com

[O02] 使用线程池
来源：http://pyv.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yqy.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://krw.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://mlx.redwolf501.top

TS:   // worker_threads 线程池
来源：http://xwk.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://gao.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://phq.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbs.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rgi.pycfn.com

[O03] 加锁保护共享数据
来源：http://qvp.chenzaomai.com

Py:   with lock: shared += 1
来源：http://unl.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://tfv.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bxw.pengpengdd.cyou

TS:   // 同 JS
来源：http://nwi.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://xwf.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rfz.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://mgu.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://apj.iojbl.cn

[O04] 定义异步函数并等待
来源：http://pmf.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://iyo.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oop.sysykeji.top

JS:   async function f() { await g(); }
来源：http://gxd.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://bkv.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jti.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bbt.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://phw.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://fhs.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://cok.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://otp.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zjc.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://kzi.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://bcz.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mit.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://emw.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://exo.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qzc.xinyue.icu

[O06] 使用进程池
来源：http://yhw.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hkx.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ioh.tanke756.top

JS:   // child_process / cluster 模块
来源：http://ewt.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://szk.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xcl.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bhz.zhoulong.xyz

Ruby: // fork 块
来源：http://sms.zdbjq.cn

C#:   Parallel.For
来源：http://xfg.daria6918.cn

================================================================================
来源：http://ywe.aizwys.cn

P. 常用工具函数
来源：http://qqm.daria6918.cn

================================================================================
来源：http://igo.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://aso.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://xkp.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rbr.fehbvm.com

JS:   crypto.randomUUID()
来源：http://lqs.sxryk.cn

TS:   crypto.randomUUID()
来源：http://pap.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://kiq.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://pvc.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://qgh.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://pbd.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://vjp.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wny.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvf.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jnp.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bkp.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tmu.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nnb.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ill.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kuj.guannengcc.top

[P03] 生成短随机字符串
来源：http://gsq.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cbf.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lvq.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqz.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qru.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hxx.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ueu.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://djj.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nag.haohaochexian.top

[P04] 求长度
来源：http://ndd.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pnt.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcf.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xbx.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnt.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://opk.316326.xyz

Go:   len(arr);  len(m)
来源：http://hvv.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://qfo.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jia.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://zql.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cjf.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zay.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aig.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bsp.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gpu.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://gjf.aizwys.cn

Ruby: a == b
来源：http://see.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fhq.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ybp.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tof.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://zno.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gvv.uphjek.com

TS:   if (x == null) {}
来源：http://jvs.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jjy.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://xfl.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wer.fktsv.cn

C#:   if (x is null) {}
来源：http://mpb.cashguo.top

[P07] 防抖与节流
来源：http://ozf.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://col.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://vwm.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgw.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldi.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rwq.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ywc.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cfu.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vol.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://oqt.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://djc.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqq.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cbm.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yoq.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hxd.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://odg.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://brv.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://duu.zdqjudy.top

================================================================================
来源：http://ruc.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://apa.aizwys.cn

================================================================================
来源：http://usk.havefunace.top

[Q01] 创建表
来源：http://rsu.haohaochexian.top

CREATE TABLE users (
来源：http://eev.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxt.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://tlv.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://yci.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ppj.tianlin.xyz

);
来源：http://aqu.zhixingplan.top

[Q02] 创建带外键的表
来源：http://qsm.jinqigufen.top

CREATE TABLE orders (
来源：http://swj.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fnd.nwbrower.top

user_id INT NOT NULL,
来源：http://zsj.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://jds.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jhg.jiagoushi.top

);
来源：http://mqt.xinyue.icu

[Q03] 增加列
来源：http://vgc.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://npk.wangshuangyany.cn

[Q04] 修改列类型
来源：http://wpm.bbcook.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hlq.yuxming.cn

[Q05] 重命名列
来源：http://nmh.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uwn.hnqzz.top

[Q06] 删除列
来源：http://akw.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://put.52xcode.cn

[Q07] 删除表
来源：http://cbd.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://pcf.ivvv.top

[Q08] 创建普通索引
来源：http://gag.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://acu.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://oeq.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dks.bjfxy.top

[Q10] 插入单行
来源：http://sdj.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pua.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://kfx.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eaq.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://ghk.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://ebl.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qwm.havefunace.top

[Q13] 忽略重复插入
来源：http://tdo.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ked.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://vao.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gjw.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lhl.0kj1m.cn

[Q15] 查询全部
来源：http://tpf.guannengcc.top

SELECT * FROM users;
来源：http://umq.dianchejie.cn

[Q16] 查询指定列
来源：http://xff.zhengqikj.top

SELECT id, name FROM users;
来源：http://uup.xylfe.cn

[Q17] 条件查询
来源：http://tvj.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rfi.sysykeji.top

[Q18] 模糊匹配
来源：http://hka.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mbt.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://pxd.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rpw.hysaishi.cn

[Q20] IN 列表
来源：http://juk.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cml.xuanzx.com

[Q21] 空值判断
来源：http://tzv.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yxt.hnxiangtu.top

[Q22] 排序
来源：http://rrd.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qym.zhongyouzk.top

[Q23] 分页
来源：http://vns.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ush.gaohongyu789.top

[Q24] 去重
来源：http://ysy.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://lyu.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://nhx.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nvj.chenjidiqi.icu

[Q26] 计数
来源：http://qtv.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://wvx.vehdjk.com

[Q27] 条件计数
来源：http://ifc.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wja.mhx1999.top

[Q28] 求和与平均
来源：http://tku.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pzn.sjlbkw.cn

[Q29] 最大最小值
来源：http://cjt.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zci.smart0.xyz

[Q30] 分组统计
来源：http://oxb.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ikl.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://sow.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lbw.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://han.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://crs.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dhc.dashuyun.cn

[Q33] 多列分组
来源：http://rzm.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bhd.sysykeji.top

[Q34] 每组取第一条
来源：http://kng.fehbvm.com

SELECT * FROM (
来源：http://pln.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://smw.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://jxd.yueranfly.top

[Q35] 内连接
来源：http://doi.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ykv.zhongyouzk.top

[Q36] 左连接
来源：http://qey.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vev.yfazqb.com

[Q37] 右连接
来源：http://iqh.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lsn.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://fpn.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lmc.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://lew.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hdl.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hjl.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ohk.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ysu.yfazqb.com

[Q41] 多表连接
来源：http://qic.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jkx.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://nwt.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://rfe.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://enf.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://xxb.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eqm.zdqjudy.top

[Q43] 标量子查询
来源：http://who.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://erc.gzhubu.top

[Q44] IN 子查询
来源：http://bsp.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://avq.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://crv.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iok.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://igz.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzg.jianghu66.top

[Q47] 与平均值比较
来源：http://wnp.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xqx.ppjwa.cn

[Q48] CTE 公用表表达式
来源：http://wzz.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pzz.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://gla.shuidangran.top

[Q49] 更新单行
来源：http://vmi.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kvv.zdbjq.cn

[Q50] 批量更新
来源：http://kss.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nft.gzhubu.top

[Q51] 用子查询更新
来源：http://nkh.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mzt.sjlbkw.cn

[Q52] 删除指定行
来源：http://eht.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://srk.sxryk.cn

[Q53] 按条件删除
来源：http://cxb.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wne.jinyuanbaomall.cn

[Q54] 清空表
来源：http://xft.sweek.top

TRUNCATE TABLE logs;
来源：http://kfs.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://wgp.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xpo.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://njw.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://clm.shzxlz.cn

[Q57] 行号
来源：http://hdw.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hmi.hnqzz.top

[Q58] 累计求和
来源：http://hky.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://seg.aibaodan.cn

[Q59] 分组内累计
来源：http://pzj.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rbg.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://tjd.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xpy.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jzi.zhongyouzk.top

[Q61] 移动平均
来源：http://dec.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tts.jiagoushi.top

[Q62] 分组占比
来源：http://uhk.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wdd.yongpay.top

[Q63] 开启事务
来源：http://gek.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gpe.chenlongwang.top

[Q64] 提交事务
来源：http://cpr.jqgufenzy.top

COMMIT;
来源：http://uyq.meibo888.top

[Q65] 回滚事务
来源：http://hfr.gzhubu.top

ROLLBACK;
来源：http://myz.fktsv.cn

[Q66] 行锁查询
来源：http://dct.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aia.meibo888.top

[Q67] 设置隔离级别
来源：http://crd.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ajj.ehwqpu.com

[Q68] 保存点
来源：http://kwk.fehbvm.com

SAVEPOINT sp1;
来源：http://dtl.ivvv.top

ROLLBACK TO sp1;
来源：http://ivm.andypj.xyz

[Q69] 查看执行计划
来源：http://efx.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xsn.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://rnx.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://klc.xuanzx.com

[Q71] 查看建表语句
来源：http://ous.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ttm.yuxming.cn

[Q72] 查看索引
来源：http://hzu.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://som.sjlbkw.cn

[Q73] 查看表状态
来源：http://kyg.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wwt.jiagoushi.top

[Q74] 强制使用索引
来源：http://qhb.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ryc.cashguo.top

[Q75] 日期格式化
来源：http://fnh.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jta.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://azj.gzhubu.top


<!-- 参考信息 -->