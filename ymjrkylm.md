代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://tmz.yfazqb.com

Go:   go f()
来源：http://xch.bbcook.cn

Ruby: Thread.new { f }
来源：http://wls.yongpay.top

C#:   Task.Run(() => F());
来源：http://yjg.jianghu66.top

[O02] 使用线程池
来源：http://wpl.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uqe.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://byb.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://koj.ybcxt.top

TS:   // worker_threads 线程池
来源：http://uls.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fwy.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pyg.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lvf.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hbq.tian-w.cn

[O03] 加锁保护共享数据
来源：http://elj.zdbjq.cn

Py:   with lock: shared += 1
来源：http://rjs.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://bsb.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lmh.jlsjyb.cn

TS:   // 同 JS
来源：http://npp.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://gar.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oii.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vrq.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://tvb.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://ppk.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://ydm.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ggy.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://jql.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://iuv.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oqk.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uac.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://xqy.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://bbv.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://jop.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://pit.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ark.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://uqn.tarul.cn

TS:   await Promise.all(tasks)
来源：http://iji.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://plw.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://znj.havefunace.top

Ruby: threads.map(&:join)
来源：http://niw.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kvj.uphjek.com

[O06] 使用进程池
来源：http://ppv.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fnj.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ujt.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://ttb.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://jkc.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wrb.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ult.meibo888.top

Ruby: // fork 块
来源：http://xtq.fehbvm.com

C#:   Parallel.For
来源：http://kkf.vehdjk.com

================================================================================
来源：http://qpx.nanxuanxn.top

P. 常用工具函数
来源：http://irh.jqgfzy.top

================================================================================
来源：http://cvo.yvedp.cn

[P01] 生成 UUID
来源：http://llu.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://cgw.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cjp.ybcxt.top

JS:   crypto.randomUUID()
来源：http://rvm.uphjek.com

TS:   crypto.randomUUID()
来源：http://bjg.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://uej.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://gtv.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://vml.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://hwi.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://usu.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bdv.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://svh.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jra.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hrw.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bia.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wlf.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ftu.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gqv.hammf.cn

[P03] 生成短随机字符串
来源：http://fla.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sij.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iqd.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofl.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://irm.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eht.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mim.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vry.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://odd.fzhhl.top

[P04] 求长度
来源：http://eto.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://msz.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ejy.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://omb.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nmq.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://jvg.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://cil.bjfxy.top

Ruby: x.length;  x.size
来源：http://rwx.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gjh.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://isx.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xhv.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vte.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://odq.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vta.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nui.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uwm.xinyue.icu

Ruby: a == b
来源：http://tlp.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zdy.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tjk.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aay.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://jkm.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lde.meibo888.top

TS:   if (x == null) {}
来源：http://zev.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dnr.fengsongda.top

Go:   if x == nil {}
来源：http://uhu.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vkc.ybcxt.top

C#:   if (x is null) {}
来源：http://bsr.yfazqb.com

[P07] 防抖与节流
来源：http://qgx.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zdj.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://amx.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkp.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkj.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xso.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gcj.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqo.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xiv.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://mmy.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ydy.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnv.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://koy.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://akh.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://otl.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://odj.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xxn.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lnt.shanyushiyangtech.top

================================================================================
来源：http://nwx.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lhz.nanxinkj.top

================================================================================
来源：http://dvy.yonumen.top

[Q01] 创建表
来源：http://vac.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://qjv.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ash.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://xun.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://nhb.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fcu.yfazqb.com

);
来源：http://roa.sweek.top

[Q02] 创建带外键的表
来源：http://jlb.zhengqikj.top

CREATE TABLE orders (
来源：http://tsm.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kkv.tian-w.cn

user_id INT NOT NULL,
来源：http://xiv.yonumen.top

amount DECIMAL(10, 2),
来源：http://wth.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mgn.shanyushiyangtech.top

);
来源：http://xnk.shzxlz.cn

[Q03] 增加列
来源：http://uvq.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://syz.bjfxy.top

[Q04] 修改列类型
来源：http://ind.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://giw.yfazqb.com

[Q05] 重命名列
来源：http://bor.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://luw.smart0.xyz

[Q06] 删除列
来源：http://toj.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://ktc.gaohongyu789.top

[Q07] 删除表
来源：http://fft.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://lyu.zhongyouzk.top

[Q08] 创建普通索引
来源：http://vxi.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zqm.yj20258888.top

[Q09] 创建唯一索引
来源：http://lpf.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://elz.svipenyu.cn

[Q10] 插入单行
来源：http://hcm.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ahn.vehdjk.com

[Q11] 一次插入多行
来源：http://txf.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dee.uphjek.com

[Q12] 插入后取自增 ID
来源：http://woi.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://cxh.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dyd.havefunace.top

[Q13] 忽略重复插入
来源：http://han.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rhw.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://flf.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://osa.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://alo.iojbl.cn

[Q15] 查询全部
来源：http://drg.ydjk.org.cn

SELECT * FROM users;
来源：http://twl.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://itd.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://gzj.hnxiangtu.top

[Q17] 条件查询
来源：http://fpo.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gwr.snrcjt.cn

[Q18] 模糊匹配
来源：http://mrp.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tcx.yj20258888.top

[Q19] 范围查询
来源：http://gly.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jte.yj20258888.top

[Q20] IN 列表
来源：http://unj.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cpy.zhixingplan.top

[Q21] 空值判断
来源：http://sgx.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qmi.jinqigfzy.top

[Q22] 排序
来源：http://vlq.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wgo.sxryk.cn

[Q23] 分页
来源：http://rnn.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cmu.bjfxy.top

[Q24] 去重
来源：http://kfv.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://plc.shuidangran.top

[Q25] 只取前 N 条
来源：http://duz.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ore.ydjk.org.cn

[Q26] 计数
来源：http://vcr.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://mfa.hcnkem.com

[Q27] 条件计数
来源：http://psm.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hjl.hysaishi.cn

[Q28] 求和与平均
来源：http://fxf.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zjk.yuxming.cn

[Q29] 最大最小值
来源：http://clp.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ypr.smart0.xyz

[Q30] 分组统计
来源：http://eok.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sts.cdnleiting.top

[Q31] 分组后过滤
来源：http://wbl.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bhj.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://inf.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ayq.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ota.hysaishi.cn

[Q33] 多列分组
来源：http://ijl.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kfr.wangdashe.top

[Q34] 每组取第一条
来源：http://ngn.52xcode.cn

SELECT * FROM (
来源：http://rdy.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zmt.iojbl.cn

) t WHERE rn = 1;
来源：http://lqj.snrcjt.cn

[Q35] 内连接
来源：http://iax.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://our.cucudq.cn

[Q36] 左连接
来源：http://sdp.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://euo.tianlin.xyz

[Q37] 右连接
来源：http://hli.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iie.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://dna.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://exk.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://acu.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://agz.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ivg.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zox.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wqi.snrcjt.cn

[Q41] 多表连接
来源：http://jmc.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lap.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://cnu.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://tmh.meibo888.top

[Q42] 连接条件附加过滤
来源：http://obt.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://ach.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wct.tarul.cn

[Q43] 标量子查询
来源：http://tkb.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iol.yanxiufei.cn

[Q44] IN 子查询
来源：http://bpd.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iog.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://yjq.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vzv.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://viv.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dpd.hnqzz.top

[Q47] 与平均值比较
来源：http://drh.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://klk.tarul.cn

[Q48] CTE 公用表表达式
来源：http://scm.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ije.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://ods.jianghu66.top

[Q49] 更新单行
来源：http://icr.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ygk.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://kag.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://htz.dashuyun.cn

[Q51] 用子查询更新
来源：http://ulo.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vin.zhiwuduotai.top

[Q52] 删除指定行
来源：http://emh.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://aea.sxryk.cn

[Q53] 按条件删除
来源：http://sfs.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://psl.mhx1999.top

[Q54] 清空表
来源：http://kxg.tian-w.cn

TRUNCATE TABLE logs;
来源：http://oeo.cucudq.cn

[Q55] 排名（并列占位）
来源：http://tdu.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ule.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://yme.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nco.hywenlv.cn

[Q57] 行号
来源：http://igj.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ovm.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://alx.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ozs.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://vbf.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jwo.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://aoe.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cmv.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tiw.vqdsnc.cn

[Q61] 移动平均
来源：http://qox.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ihk.cdnleiting.top

[Q62] 分组占比
来源：http://zou.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://exf.gotoacloud.top

[Q63] 开启事务
来源：http://hfm.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ynu.chenjidiqi.icu

[Q64] 提交事务
来源：http://xlk.sysykeji.top

COMMIT;
来源：http://cpz.gzhubu.top

[Q65] 回滚事务
来源：http://wju.hysaishi.cn

ROLLBACK;
来源：http://eeb.jiagoushi.top

[Q66] 行锁查询
来源：http://hde.cheryme.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lya.bjfxy.top

[Q67] 设置隔离级别
来源：http://tgm.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jly.uphjek.com

[Q68] 保存点
来源：http://ogh.ehwqpu.com

SAVEPOINT sp1;
来源：http://lro.ppjwa.cn

ROLLBACK TO sp1;
来源：http://vcs.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://cay.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pwa.shuidangran.top

[Q70] 更新统计信息
来源：http://irs.gaohongyu789.top

ANALYZE TABLE users;
来源：http://byn.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://zbp.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qms.hesvh.cn

[Q72] 查看索引
来源：http://fgo.yuxming.cn

SHOW INDEX FROM users;
来源：http://qtx.hywenlv.cn

[Q73] 查看表状态
来源：http://jqa.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gmd.jinqigufen.top

[Q74] 强制使用索引
来源：http://xhi.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rwm.sufxvd.cn

[Q75] 日期格式化
来源：http://sjg.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fvn.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sqd.xylfe.cn


<!-- 参考信息 -->