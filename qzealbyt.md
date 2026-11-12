代发 wailian999

[O02] 使用线程池
来源：http://tcb.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wtf.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ird.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://anw.epnwcf.com

TS:   // worker_threads 线程池
来源：http://hbp.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uym.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ioo.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://snz.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sfc.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://lut.wangdashe.top

Py:   with lock: shared += 1
来源：http://eqc.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://mxl.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jsr.xylfe.cn

TS:   // 同 JS
来源：http://ldr.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://mnm.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blp.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://qvm.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://yfe.tanke756.top

[O04] 定义异步函数并等待
来源：http://jyl.birdmap.top

Py:   async def f():⏎    await g()
来源：http://fcy.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsx.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://smd.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://urq.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wti.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgp.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://egd.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://leu.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://dgk.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://oyf.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sei.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://zdg.meibo888.top

TS:   await Promise.all(tasks)
来源：http://auj.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aea.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pns.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://mlc.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fna.shuidangran.top

[O06] 使用进程池
来源：http://pqg.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oon.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qss.tanke756.top

JS:   // child_process / cluster 模块
来源：http://bzu.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://otm.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ucc.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yii.fktsv.cn

Ruby: // fork 块
来源：http://uba.yangfankeji.com

C#:   Parallel.For
来源：http://mci.shanyushiyangtech.top

================================================================================
来源：http://abv.ybcxt.top

P. 常用工具函数
来源：http://qqj.316326.xyz

================================================================================
来源：http://cmr.guowangkeji.top

[P01] 生成 UUID
来源：http://pmn.316326.xyz

Py:   str(uuid.uuid4())
来源：http://trb.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://byy.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://rtw.ybcxt.top

TS:   crypto.randomUUID()
来源：http://fpw.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://tst.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://wep.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://pen.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://vnu.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://heq.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hkz.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sxp.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://stw.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://duj.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pqt.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nfl.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iim.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mbg.nwbrower.top

[P03] 生成短随机字符串
来源：http://qst.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bre.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sln.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qxw.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jch.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ywj.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hzc.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pvz.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lpc.chenjidiqi.icu

[P04] 求长度
来源：http://wgc.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ykg.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yxz.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqq.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbh.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://icx.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://fdy.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://agc.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xvk.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://vwq.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://thr.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rai.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kal.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://epi.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yee.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://urq.jinqigufen.top

Ruby: a == b
来源：http://ehp.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pbk.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://syo.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wtg.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://xxa.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tmb.kuanghao11.cn

TS:   if (x == null) {}
来源：http://ndo.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://vac.sysykeji.top

Go:   if x == nil {}
来源：http://rfx.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fpd.gotoacloud.top

C#:   if (x is null) {}
来源：http://jpp.redwolf501.top

[P07] 防抖与节流
来源：http://npk.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ulg.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://cju.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrs.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsu.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qsj.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mgy.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lhf.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ozd.tian-w.cn

[P08] 处理浮点精度问题
来源：http://lze.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kdv.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wuo.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cnd.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://urw.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xli.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yjk.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://emw.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vmx.hfpthk.cn

================================================================================
来源：http://oeq.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rgm.guowangkeji.top

================================================================================
来源：http://ozf.chenzaomai.com

[Q01] 创建表
来源：http://iab.mhx1999.top

CREATE TABLE users (
来源：http://aoo.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qat.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://uua.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://cly.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jpp.ybcxt.top

);
来源：http://yjk.c1oappe.top

[Q02] 创建带外键的表
来源：http://pjx.hnxiangtu.top

CREATE TABLE orders (
来源：http://hxa.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ugv.hcnkem.com

user_id INT NOT NULL,
来源：http://jbm.bbcook.cn

amount DECIMAL(10, 2),
来源：http://jwk.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vnu.gogol.net.cn

);
来源：http://zqo.yongpay.top

[Q03] 增加列
来源：http://gom.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uxp.meibo888.top

[Q04] 修改列类型
来源：http://fbs.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://krm.guannengcc.top

[Q05] 重命名列
来源：http://vqh.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqt.sxryk.cn

[Q06] 删除列
来源：http://mpg.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bvw.daria6918.cn

[Q07] 删除表
来源：http://ipx.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://nce.sysykeji.top

[Q08] 创建普通索引
来源：http://aka.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ftt.gotoacloud.top

[Q09] 创建唯一索引
来源：http://ztn.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://apd.snrcjt.cn

[Q10] 插入单行
来源：http://kez.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dct.guannengcc.top

[Q11] 一次插入多行
来源：http://zpl.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sni.yj20258.top

[Q12] 插入后取自增 ID
来源：http://fyl.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://kzc.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bqv.havefunace.top

[Q13] 忽略重复插入
来源：http://rvx.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jiy.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://lwk.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sul.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dci.nwbrower.top

[Q15] 查询全部
来源：http://bhg.meibo888.top

SELECT * FROM users;
来源：http://ikn.nanxinkj.top

[Q16] 查询指定列
来源：http://fuv.yanxiufei.cn

SELECT id, name FROM users;
来源：http://rem.ppjwa.cn

[Q17] 条件查询
来源：http://pbw.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wri.andypj.xyz

[Q18] 模糊匹配
来源：http://lcf.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dor.guannengcc.top

[Q19] 范围查询
来源：http://cxr.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckt.mhx1999.top

[Q20] IN 列表
来源：http://tyn.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rym.tianlin.xyz

[Q21] 空值判断
来源：http://izi.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xph.xinyue.icu

[Q22] 排序
来源：http://ghj.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hov.cdnleiting.top

[Q23] 分页
来源：http://exz.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nit.yuxming.cn

[Q24] 去重
来源：http://ran.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://iml.sweek.top

[Q25] 只取前 N 条
来源：http://agd.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ifn.andypj.xyz

[Q26] 计数
来源：http://qko.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://xqi.ppjwa.cn

[Q27] 条件计数
来源：http://ppr.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lxf.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://xod.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kgs.vehdjk.com

[Q29] 最大最小值
来源：http://kge.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pkb.0kj1m.cn

[Q30] 分组统计
来源：http://hxu.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ewy.meibo888.top

[Q31] 分组后过滤
来源：http://jrx.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ggx.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://ygj.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cpa.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ywa.gogol.net.cn

[Q33] 多列分组
来源：http://pvv.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ugr.ehwqpu.com

[Q34] 每组取第一条
来源：http://yof.yj20258888.top

SELECT * FROM (
来源：http://lwq.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vww.0kj1m.cn

) t WHERE rn = 1;
来源：http://mce.pycfn.com

[Q35] 内连接
来源：http://cwy.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://htz.pengpengdd.cyou

[Q36] 左连接
来源：http://rxr.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pvb.meibo888.top

[Q37] 右连接
来源：http://npd.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkk.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://raz.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hnv.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://cdi.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://urc.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wic.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fyb.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yee.jinqigfzy.top

[Q41] 多表连接
来源：http://qow.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qgs.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://zmw.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://lww.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://pmp.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://ogw.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jhm.zdbjq.cn

[Q43] 标量子查询
来源：http://xvv.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rtz.daxiang520.top

[Q44] IN 子查询
来源：http://zlg.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jxq.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://fyn.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sys.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://gai.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pdl.vqdsnc.cn

[Q47] 与平均值比较
来源：http://dgj.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://deb.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://rkw.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://drk.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://iio.9152youxi.cn

[Q49] 更新单行
来源：http://rps.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gxy.dashuyun.cn

[Q50] 批量更新
来源：http://ftz.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lmx.chenzaomai.com

[Q51] 用子查询更新
来源：http://crn.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pnv.sysykeji.top

[Q52] 删除指定行
来源：http://ijf.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://lfv.yanxiufei.cn

[Q53] 按条件删除
来源：http://psc.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pek.zdqjudy.top

[Q54] 清空表
来源：http://wxt.redwolf501.top

TRUNCATE TABLE logs;
来源：http://pvq.hammf.cn

[Q55] 排名（并列占位）
来源：http://zez.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tkb.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://src.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hat.dianchejie.cn

[Q57] 行号
来源：http://jxt.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lmh.xuetiantiany.cn

[Q58] 累计求和
来源：http://zmq.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://adb.jqgufenzy.top

[Q59] 分组内累计
来源：http://blm.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ail.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://yqp.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ncr.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qhz.hesvh.cn

[Q61] 移动平均
来源：http://mfy.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ylr.zhengqikj.top

[Q62] 分组占比
来源：http://nst.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ryp.yanxiufei.cn

[Q63] 开启事务
来源：http://chp.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mja.hesvh.cn

[Q64] 提交事务
来源：http://kjr.mhx1999.top

COMMIT;
来源：http://rcq.snrcjt.cn

[Q65] 回滚事务
来源：http://ssg.52xcode.cn

ROLLBACK;
来源：http://ipg.jinqigfzy.top

[Q66] 行锁查询
来源：http://dno.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kgo.mhx1999.top

[Q67] 设置隔离级别
来源：http://gya.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmb.tian-w.cn

[Q68] 保存点
来源：http://kdl.52xcode.cn

SAVEPOINT sp1;
来源：http://xnq.yueranfly.top

ROLLBACK TO sp1;
来源：http://jkm.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://mnn.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zxm.yonumen.top

[Q70] 更新统计信息
来源：http://hmf.vqdsnc.cn

ANALYZE TABLE users;
来源：http://ebi.dianchejie.cn

[Q71] 查看建表语句
来源：http://qzv.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eic.hesvh.cn

[Q72] 查看索引
来源：http://lwz.nwbrower.top

SHOW INDEX FROM users;
来源：http://hbh.yfazqb.com

[Q73] 查看表状态
来源：http://wke.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mir.andypj.xyz

[Q74] 强制使用索引
来源：http://hlw.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bnw.nanxuanxn.top

[Q75] 日期格式化
来源：http://pmw.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wff.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jng.fanxiaobao.xyz

[Q76] 按天统计
来源：http://ont.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vhj.haohaochexian.top

[Q77] 时间加减
来源：http://sah.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mir.jinqigfzy.top


<!-- 参考信息 -->