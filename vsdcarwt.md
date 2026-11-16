代发 wailian999

C#:   Parallel.For
来源：http://xiq.wangdashe.top

================================================================================
来源：http://nsm.xuetiantiany.cn

P. 常用工具函数
来源：http://mrr.ydzc1.top

================================================================================
来源：http://apa.hnqzz.top

[P01] 生成 UUID
来源：http://wso.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://irn.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rzw.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://epx.yj20258888.top

TS:   crypto.randomUUID()
来源：http://eum.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://hgc.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://hdi.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://vab.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://dgz.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://miw.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hlu.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mnd.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://swd.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cpd.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hqd.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qsc.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxk.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dhr.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://qgs.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iut.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ofl.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqg.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vai.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fbf.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gav.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pco.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fju.zhixingplan.top

[P04] 求长度
来源：http://qal.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ckj.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zyv.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ewp.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eoj.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://awk.jianghu66.top

Go:   len(arr);  len(m)
来源：http://ymd.daxiang520.top

Ruby: x.length;  x.size
来源：http://fyr.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rhv.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://oix.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://oba.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cnb.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yuv.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ntf.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ema.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mth.yj202588.top

Ruby: a == b
来源：http://bkl.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nym.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hzn.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://enh.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://eup.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://olx.xylfe.cn

TS:   if (x == null) {}
来源：http://uxi.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jsv.gotoacloud.top

Go:   if x == nil {}
来源：http://cmd.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hlq.ydjk.org.cn

C#:   if (x is null) {}
来源：http://hvt.jlsjyb.cn

[P07] 防抖与节流
来源：http://kcr.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rsg.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://bap.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsv.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ivn.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cdj.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zlo.nwbrower.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dgr.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jhx.aizwys.cn

[P08] 处理浮点精度问题
来源：http://cyf.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ljg.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nry.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hic.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bfm.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mmj.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jyo.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rdc.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nxj.xylfe.cn

================================================================================
来源：http://sin.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wmg.9152youxi.cn

================================================================================
来源：http://dlk.feifeiyinyue.top

[Q01] 创建表
来源：http://zxh.meibo888.top

CREATE TABLE users (
来源：http://jvp.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://teh.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://dup.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://sdo.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://czz.cucudq.cn

);
来源：http://hui.shuidangran.top

[Q02] 创建带外键的表
来源：http://eye.zhijiandao.cn

CREATE TABLE orders (
来源：http://kvi.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://stv.ehwqpu.com

user_id INT NOT NULL,
来源：http://dua.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://tkc.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jpi.yj202588.top

);
来源：http://zvd.fanxiaobao.xyz

[Q03] 增加列
来源：http://xvz.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://osy.ehwqpu.com

[Q04] 修改列类型
来源：http://lln.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cde.cashguo.top

[Q05] 重命名列
来源：http://ltg.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pwi.meibo888.top

[Q06] 删除列
来源：http://bzl.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xgl.shangyingyoupin.top

[Q07] 删除表
来源：http://qzt.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://hhy.gaohongyu789.top

[Q08] 创建普通索引
来源：http://yrp.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ncp.gotoacloud.top

[Q09] 创建唯一索引
来源：http://otg.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dyg.hongshengwenyu.top

[Q10] 插入单行
来源：http://hlx.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tjh.jiagoushi.top

[Q11] 一次插入多行
来源：http://nno.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://epj.316326.xyz

[Q12] 插入后取自增 ID
来源：http://fms.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://tzk.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://igw.hcnkem.com

[Q13] 忽略重复插入
来源：http://wek.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fpy.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://wwa.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ncz.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ksl.cdnleiting.top

[Q15] 查询全部
来源：http://uev.meibo888.top

SELECT * FROM users;
来源：http://qmk.bjfxy.top

[Q16] 查询指定列
来源：http://eow.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://syq.nanxinkj.top

[Q17] 条件查询
来源：http://sag.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gof.zycfv.cn

[Q18] 模糊匹配
来源：http://bfb.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://opy.52xcode.cn

[Q19] 范围查询
来源：http://oln.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cvw.chenzaomai.com

[Q20] IN 列表
来源：http://zqa.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rve.nwbrower.top

[Q21] 空值判断
来源：http://xwe.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://lvv.jinqigfzy.top

[Q22] 排序
来源：http://haf.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gjv.guannengcc.top

[Q23] 分页
来源：http://cdj.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sxm.hfpthk.cn

[Q24] 去重
来源：http://kio.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://zeo.cucudq.cn

[Q25] 只取前 N 条
来源：http://jng.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ymd.ivvv.top

[Q26] 计数
来源：http://ihu.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://vfb.zhijiandao.cn

[Q27] 条件计数
来源：http://vir.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rlv.shuidangran.top

[Q28] 求和与平均
来源：http://kvn.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://soh.jqgufenzy.top

[Q29] 最大最小值
来源：http://kgp.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dtk.shuidangran.top

[Q30] 分组统计
来源：http://pxb.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izh.bbcook.cn

[Q31] 分组后过滤
来源：http://rdf.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xub.xinyue.icu

[Q32] 分组拼接字符串
来源：http://toa.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pxc.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ffx.sxryk.cn

[Q33] 多列分组
来源：http://igi.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lev.jqgufenzy.top

[Q34] 每组取第一条
来源：http://rtd.zhengqikj.top

SELECT * FROM (
来源：http://fxv.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gwv.bjfxy.top

) t WHERE rn = 1;
来源：http://gbo.hcnkem.com

[Q35] 内连接
来源：http://fbd.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyb.yuxming.cn

[Q36] 左连接
来源：http://web.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xlg.zhijiandao.cn

[Q37] 右连接
来源：http://hdc.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nms.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://ese.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qab.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://oic.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zfo.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://edz.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xic.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jwl.chenzaomai.com

[Q41] 多表连接
来源：http://pcf.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jww.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://hmb.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://djr.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://jbe.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://piw.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xfx.hfpthk.cn

[Q43] 标量子查询
来源：http://fpc.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wca.dashuyun.cn

[Q44] IN 子查询
来源：http://his.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cjp.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://hzf.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://btj.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://fmp.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://huh.hesvh.cn

[Q47] 与平均值比较
来源：http://oej.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ugu.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://vrf.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bnt.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://dct.aizwys.cn

[Q49] 更新单行
来源：http://gzd.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://edo.xinyue.icu

[Q50] 批量更新
来源：http://yfh.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vui.chenlongwang.top

[Q51] 用子查询更新
来源：http://omw.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vhr.vehdjk.com

[Q52] 删除指定行
来源：http://dnv.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://qwt.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://ape.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ozy.gaohongyu789.top

[Q54] 清空表
来源：http://qmp.52xcode.cn

TRUNCATE TABLE logs;
来源：http://soq.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://xsl.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aks.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://oau.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bpe.52xcode.cn

[Q57] 行号
来源：http://ipc.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yxk.jqgufenzy.top

[Q58] 累计求和
来源：http://xym.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fki.haohaochexian.top

[Q59] 分组内累计
来源：http://kwo.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljs.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://npv.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zyr.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpm.nanxuanxn.top

[Q61] 移动平均
来源：http://yxy.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cll.epnwcf.com

[Q62] 分组占比
来源：http://pjt.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://obp.xuanzx.com

[Q63] 开启事务
来源：http://ube.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qbw.jqgfzy.top

[Q64] 提交事务
来源：http://rua.hnqzz.top

COMMIT;
来源：http://vky.52xcode.cn

[Q65] 回滚事务
来源：http://cak.vqdsnc.cn

ROLLBACK;
来源：http://ypp.hongshengwenyu.top

[Q66] 行锁查询
来源：http://ojy.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xax.hesvh.cn

[Q67] 设置隔离级别
来源：http://nuh.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eld.gogol.net.cn

[Q68] 保存点
来源：http://wuv.ppjwa.cn

SAVEPOINT sp1;
来源：http://juq.andypj.xyz

ROLLBACK TO sp1;
来源：http://swf.iojbl.cn

[Q69] 查看执行计划
来源：http://gwd.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mkq.cashguo.top

[Q70] 更新统计信息
来源：http://zdt.zdqjudy.top

ANALYZE TABLE users;
来源：http://hkd.vehdjk.com

[Q71] 查看建表语句
来源：http://gsk.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ogp.chenjidiqi.icu

[Q72] 查看索引
来源：http://kld.ydzc1.top

SHOW INDEX FROM users;
来源：http://elp.tarul.cn

[Q73] 查看表状态
来源：http://cuf.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cmr.zycfv.cn

[Q74] 强制使用索引
来源：http://ajw.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kqm.nanxinkj.top

[Q75] 日期格式化
来源：http://kct.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fig.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ies.fktsv.cn

[Q76] 按天统计
来源：http://weh.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jdf.birdmap.top

[Q77] 时间加减
来源：http://xqr.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hmj.hesvh.cn

[Q78] 当前时间
来源：http://lwj.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xvr.bbcook.cn

[Q79] 字符串拼接
来源：http://zur.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wdr.uphjek.com

[Q80] 字符串截取
来源：http://gev.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dwo.zhengqikj.top

[Q81] 字符串替换
来源：http://kob.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://riw.uphjek.com

[Q82] 字符长度与字节长度
来源：http://mxo.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hzs.yueranfly.top

[Q83] 大小写转换
来源：http://lfv.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dze.zhengqikj.top

[Q84] 去除首尾空格
来源：http://zzf.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://xrp.cdnleiting.top

[Q85] 数值取整
来源：http://zxt.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fhf.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://yqv.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jie.yuxming.cn

[Q87] JSON 字段做条件
来源：http://qnk.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qqy.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://kzc.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xns.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oae.fengsongda.top

[Q89] 判断表是否存在
来源：http://qfb.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ure.xinyue.icu

[Q90] 生成序号列
来源：http://cuf.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nzv.dianchejie.cn

================================================================================
来源：http://qkd.redwolf501.top

R. Bash 专题
来源：http://vlh.jyoumei.cn

================================================================================
来源：http://fll.vehdjk.com

[R01] shebang 与严格模式
来源：http://cvw.vqdsnc.cn

#!/usr/bin/env bash
来源：http://lzt.hnxiangtu.top

set -euo pipefail
来源：http://ahv.zhixingplan.top

[R02] 变量赋值与使用
来源：http://spj.aibaodan.cn

name="Tom"; echo "$name"
来源：http://inq.jiagoushi.top

[R03] 只读变量
来源：http://hya.daria6918.cn

readonly PI=3.14
来源：http://pvg.shanyushiyangkeji.top

[R04] 位置参数
来源：http://tsc.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hiu.yonumen.top

[R05] 参数默认值
来源：http://wxn.smart0.xyz

name="${1:-default}"
来源：http://xue.52xcode.cn

[R06] 判断命令是否存在
来源：http://aka.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fbp.sufxvd.cn

[R07] if 判断文件
来源：http://wvl.yueranfly.top


<!-- 参考信息 -->