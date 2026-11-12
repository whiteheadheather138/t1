代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjw.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ljc.tanke756.top

Ruby: threads.map(&:join)
来源：http://xxr.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vlp.ybcxt.top

[O06] 使用进程池
来源：http://kyy.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cej.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fqa.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://ulb.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://csk.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dwj.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nbn.ppjwa.cn

Ruby: // fork 块
来源：http://vhh.cashguo.top

C#:   Parallel.For
来源：http://lwt.zhixingplan.top

================================================================================
来源：http://qxl.yvedp.cn

P. 常用工具函数
来源：http://vtv.9152youxi.cn

================================================================================
来源：http://oga.yuanzhike.top

[P01] 生成 UUID
来源：http://atg.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://xsl.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://swb.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://run.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://ftp.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://zjb.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://pej.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://cau.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://swg.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://psk.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kcp.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://btp.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ott.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zza.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wio.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvw.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://efz.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tdv.wangdashe.top

[P03] 生成短随机字符串
来源：http://bcz.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shv.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ciy.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://maz.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ndo.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xxv.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://phj.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hke.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mpf.xuetiantiany.cn

[P04] 求长度
来源：http://ggg.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fps.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xei.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqd.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjz.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://bzg.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://ykn.xuanzx.com

Ruby: x.length;  x.size
来源：http://ctw.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lkd.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://yit.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wcy.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jpr.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yjp.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjf.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://spa.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://khq.guannengcc.top

Ruby: a == b
来源：http://ikp.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zxf.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mge.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bdd.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://ckt.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lnk.nanxinkj.top

TS:   if (x == null) {}
来源：http://bzt.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hmo.tanke756.top

Go:   if x == nil {}
来源：http://stt.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fvx.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://osg.nanxuanxn.top

[P07] 防抖与节流
来源：http://tqu.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xtk.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://nwy.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gib.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cje.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pgc.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tam.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uig.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jfy.xylfe.cn

[P08] 处理浮点精度问题
来源：http://hkr.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ois.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tsj.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://map.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dln.bjfxy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://knz.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pvw.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://olw.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gox.yangfankeji.com

================================================================================
来源：http://hrp.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ool.yvedp.cn

================================================================================
来源：http://xhl.9152youxi.cn

[Q01] 创建表
来源：http://gdo.shangyingyoupin.top

CREATE TABLE users (
来源：http://xcx.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lse.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://fes.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://zir.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wts.zycfv.cn

);
来源：http://mmv.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://hdb.hammf.cn

CREATE TABLE orders (
来源：http://sdj.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bou.hammf.cn

user_id INT NOT NULL,
来源：http://mfk.sxryk.cn

amount DECIMAL(10, 2),
来源：http://evp.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ivf.zhixingplan.top

);
来源：http://pop.ivvv.top

[Q03] 增加列
来源：http://qcv.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zqs.fktsv.cn

[Q04] 修改列类型
来源：http://hrc.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://apv.vehdjk.com

[Q05] 重命名列
来源：http://qgj.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oii.tarul.cn

[Q06] 删除列
来源：http://cyd.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://qle.hesvh.cn

[Q07] 删除表
来源：http://dro.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://okm.mhx1999.top

[Q08] 创建普通索引
来源：http://emi.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tak.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://xrj.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pml.kuanghao11.cn

[Q10] 插入单行
来源：http://lpu.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yhz.ybcxt.top

[Q11] 一次插入多行
来源：http://rbe.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ipi.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://kqg.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xhi.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ftv.jyoumei.cn

[Q13] 忽略重复插入
来源：http://uaw.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pvn.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://fwm.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xxu.yj202588.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cbl.ydjk.org.cn

[Q15] 查询全部
来源：http://kli.uphjek.com

SELECT * FROM users;
来源：http://dhq.fengsongda.top

[Q16] 查询指定列
来源：http://fwz.fktsv.cn

SELECT id, name FROM users;
来源：http://myd.shzxlz.cn

[Q17] 条件查询
来源：http://nql.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lum.ppjwa.cn

[Q18] 模糊匹配
来源：http://hii.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://buo.fengsongda.top

[Q19] 范围查询
来源：http://fjy.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rkb.yanxiufei.cn

[Q20] IN 列表
来源：http://geh.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nyj.sjlbkw.cn

[Q21] 空值判断
来源：http://hpd.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dir.shanyushiyangtech.top

[Q22] 排序
来源：http://xca.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://npa.zdqjudy.top

[Q23] 分页
来源：http://zhf.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hsh.hywenlv.cn

[Q24] 去重
来源：http://ymz.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://dyc.tanke756.top

[Q25] 只取前 N 条
来源：http://ayj.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uqf.hnxiangtu.top

[Q26] 计数
来源：http://ito.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://kml.zdqjudy.top

[Q27] 条件计数
来源：http://ouo.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eof.0kj1m.cn

[Q28] 求和与平均
来源：http://qhk.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ryp.ivvv.top

[Q29] 最大最小值
来源：http://pyj.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uod.guannengcc.top

[Q30] 分组统计
来源：http://arf.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cmj.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://vga.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yqr.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://sam.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://krh.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hwd.nanxuanxn.top

[Q33] 多列分组
来源：http://xpp.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ofw.xuanzx.com

[Q34] 每组取第一条
来源：http://ump.jianghu66.top

SELECT * FROM (
来源：http://dta.bjfxy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qsb.haohaochexian.top

) t WHERE rn = 1;
来源：http://fid.wangshuangyany.cn

[Q35] 内连接
来源：http://tcd.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kow.hnxiangtu.top

[Q36] 左连接
来源：http://xmt.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wmf.ppjwa.cn

[Q37] 右连接
来源：http://tmn.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jjw.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://jbb.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nck.pycfn.com

[Q39] 自连接（查上下级）
来源：http://aee.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vib.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pvh.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ktp.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ziv.yfazqb.com

[Q41] 多表连接
来源：http://wqn.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://zbx.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://aaj.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://vwk.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://hbg.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://kkm.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ekz.ehwqpu.com

[Q43] 标量子查询
来源：http://aur.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://top.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://tub.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rwy.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://irb.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tfr.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://gcg.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tod.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://wsu.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kme.tanke756.top

[Q48] CTE 公用表表达式
来源：http://orr.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdq.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://igr.hnqzz.top

[Q49] 更新单行
来源：http://qgg.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zec.yongpay.top

[Q50] 批量更新
来源：http://lcr.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bcy.bbcook.cn

[Q51] 用子查询更新
来源：http://vyy.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dkv.yuanzhike.top

[Q52] 删除指定行
来源：http://zfy.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://jju.hongshengwenyu.top

[Q53] 按条件删除
来源：http://dww.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xdm.yfazqb.com

[Q54] 清空表
来源：http://yvc.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://bof.tanke756.top

[Q55] 排名（并列占位）
来源：http://djo.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jpp.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://new.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vkz.meibo888.top

[Q57] 行号
来源：http://zae.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://myj.hfpthk.cn

[Q58] 累计求和
来源：http://grl.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zez.havefunace.top

[Q59] 分组内累计
来源：http://gfp.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yzs.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://aas.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uyj.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ynu.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://wel.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yhc.9152youxi.cn

[Q62] 分组占比
来源：http://hkt.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ory.meibo888.top

[Q63] 开启事务
来源：http://yju.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bcf.dianchejie.cn

[Q64] 提交事务
来源：http://uks.zhoulong.xyz

COMMIT;
来源：http://nis.yvedp.cn

[Q65] 回滚事务
来源：http://isq.pycfn.com

ROLLBACK;
来源：http://pad.tarul.cn

[Q66] 行锁查询
来源：http://ewb.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fpq.yuanzhike.top

[Q67] 设置隔离级别
来源：http://egq.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://njg.snrcjt.cn

[Q68] 保存点
来源：http://clb.xinyue.icu

SAVEPOINT sp1;
来源：http://vri.bbcook.cn

ROLLBACK TO sp1;
来源：http://zap.9152youxi.cn

[Q69] 查看执行计划
来源：http://kim.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bht.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://cqc.sxryk.cn

ANALYZE TABLE users;
来源：http://sph.fktsv.cn

[Q71] 查看建表语句
来源：http://ucg.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://prk.fehbvm.com

[Q72] 查看索引
来源：http://bvd.shuidangran.top

SHOW INDEX FROM users;
来源：http://ack.hammf.cn

[Q73] 查看表状态
来源：http://nfy.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lia.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://qrn.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mmd.zhengqikj.top

[Q75] 日期格式化
来源：http://zci.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bic.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://naa.sufxvd.cn

[Q76] 按天统计
来源：http://sre.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lhe.dashuyun.cn

[Q77] 时间加减
来源：http://eyz.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://twm.svipenyu.cn

[Q78] 当前时间
来源：http://nos.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qoh.sjlbkw.cn

[Q79] 字符串拼接
来源：http://vzh.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dhn.tian-w.cn

[Q80] 字符串截取
来源：http://git.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jzf.316326.xyz

[Q81] 字符串替换
来源：http://bhv.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rpf.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://xap.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://btk.hnqzz.top

[Q83] 大小写转换
来源：http://mlv.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ast.hywenlv.cn

[Q84] 去除首尾空格
来源：http://yuy.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://uni.xylfe.cn

[Q85] 数值取整
来源：http://vow.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qzp.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://zcm.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kmm.tanke756.top

[Q87] JSON 字段做条件
来源：http://cve.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ipp.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://fva.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pqu.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yfm.yuanzhike.top

[Q89] 判断表是否存在
来源：http://hzh.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xgq.cucudq.cn

[Q90] 生成序号列
来源：http://vay.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rar.yanxiufei.cn

================================================================================
来源：http://pvs.tarul.cn

R. Bash 专题
来源：http://ywd.gotoacloud.top

================================================================================
来源：http://nxl.yj202588.top

[R01] shebang 与严格模式
来源：http://bkz.yj20258888.top

#!/usr/bin/env bash
来源：http://klb.iojbl.cn


<!-- 参考信息 -->