代发 wailian999

TS:   // child_process / cluster 模块
来源：http://wcz.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zma.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blj.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://cjs.yj202588.top

C#:   Parallel.For
来源：http://vgy.vqdsnc.cn

================================================================================
来源：http://dmr.tianlin.xyz

P. 常用工具函数
来源：http://fsd.yanxiufei.cn

================================================================================
来源：http://mrk.nanxinkj.top

[P01] 生成 UUID
来源：http://atf.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://rsc.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jol.pycfn.com

JS:   crypto.randomUUID()
来源：http://czj.tian-w.cn

TS:   crypto.randomUUID()
来源：http://jeb.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://sea.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://zeb.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://apq.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://vlv.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://bqm.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://goa.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vxh.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cao.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aua.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://afx.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jqz.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uun.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ior.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://wyt.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tqb.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jao.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbp.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mwp.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://amv.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bhp.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cyo.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://chh.jlsjyb.cn

[P04] 求长度
来源：http://kft.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://goj.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kyu.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gmr.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ejw.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://ixv.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://ywo.yangfankeji.com

Ruby: x.length;  x.size
来源：http://qhs.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eom.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://yvp.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://nnr.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://brx.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hhc.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rrk.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ijx.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rgs.fzhhl.top

Ruby: a == b
来源：http://ohr.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vdj.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zkx.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bny.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://aim.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://khl.tarul.cn

TS:   if (x == null) {}
来源：http://npl.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zkm.bjfxy.top

Go:   if x == nil {}
来源：http://uti.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://chk.yj20258.top

C#:   if (x is null) {}
来源：http://kdt.zhiwuduotai.top

[P07] 防抖与节流
来源：http://raz.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xxq.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://zfs.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbp.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbn.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zxy.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cwb.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rmz.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wbb.hcnkem.com

[P08] 处理浮点精度问题
来源：http://sht.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zdc.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mkt.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rqj.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://adm.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fur.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ffv.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jwg.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sjp.iojbl.cn

================================================================================
来源：http://dlg.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kky.cashguo.top

================================================================================
来源：http://apa.jinqigfzy.top

[Q01] 创建表
来源：http://onu.yvedp.cn

CREATE TABLE users (
来源：http://htq.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kno.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://loj.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://lcw.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qfp.cashguo.top

);
来源：http://sum.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://usz.ydzc1.top

CREATE TABLE orders (
来源：http://dzu.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xna.yj20258.top

user_id INT NOT NULL,
来源：http://eyc.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://jky.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ooi.jqgfzy.top

);
来源：http://pql.nanxinkj.top

[Q03] 增加列
来源：http://tqt.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyr.iojbl.cn

[Q04] 修改列类型
来源：http://ruh.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pjb.chenjidiqi.icu

[Q05] 重命名列
来源：http://uwk.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cfn.guowangkeji.top

[Q06] 删除列
来源：http://jin.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://brt.aizwys.cn

[Q07] 删除表
来源：http://kfr.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://bov.smart0.xyz

[Q08] 创建普通索引
来源：http://nmk.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qfr.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://tdk.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://svb.yongpay.top

[Q10] 插入单行
来源：http://rmf.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ism.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://ufc.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ufo.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://sbc.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eqb.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sga.ppjwa.cn

[Q13] 忽略重复插入
来源：http://btj.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rji.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://fea.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xqz.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jyp.quarkkingdee.top

[Q15] 查询全部
来源：http://ilt.birdmap.top

SELECT * FROM users;
来源：http://cxp.52xcode.cn

[Q16] 查询指定列
来源：http://qkh.jlsjyb.cn

SELECT id, name FROM users;
来源：http://hgj.sweek.top

[Q17] 条件查询
来源：http://uqq.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wyr.svipenyu.cn

[Q18] 模糊匹配
来源：http://xtp.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dtx.svipenyu.cn

[Q19] 范围查询
来源：http://kyr.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kwl.fengsongda.top

[Q20] IN 列表
来源：http://nyt.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cix.jqgufenzy.top

[Q21] 空值判断
来源：http://owy.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eog.xingfuxueyuan.xyz

[Q22] 排序
来源：http://rlg.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://quh.yongpay.top

[Q23] 分页
来源：http://zsb.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vbl.ehwqpu.com

[Q24] 去重
来源：http://wpx.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://voh.yuanzhike.top

[Q25] 只取前 N 条
来源：http://dma.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://emd.wangdashe.top

[Q26] 计数
来源：http://duv.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://eiq.zhengqikj.top

[Q27] 条件计数
来源：http://wkn.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lkr.yuxming.cn

[Q28] 求和与平均
来源：http://xng.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzv.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://ntk.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tts.quarkkingdee.top

[Q30] 分组统计
来源：http://hon.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mtx.chenzaomai.com

[Q31] 分组后过滤
来源：http://jid.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfs.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://qjd.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://izg.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bwu.guannengcc.top

[Q33] 多列分组
来源：http://giy.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vvy.xuanzx.com

[Q34] 每组取第一条
来源：http://yle.kuanghao11.cn

SELECT * FROM (
来源：http://rwv.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hpv.tian-w.cn

) t WHERE rn = 1;
来源：http://fkw.fengsongda.top

[Q35] 内连接
来源：http://evp.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hhr.feifeiyinyue.top

[Q36] 左连接
来源：http://rme.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kdq.vehdjk.com

[Q37] 右连接
来源：http://imx.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kzk.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iav.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hyq.yj202588.top

[Q39] 自连接（查上下级）
来源：http://wor.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://poh.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xui.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xdh.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eef.chenlongwang.top

[Q41] 多表连接
来源：http://tse.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kkv.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://lce.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://jvg.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://ewy.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://flw.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ult.chenjidiqi.icu

[Q43] 标量子查询
来源：http://skv.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gba.yueranfly.top

[Q44] IN 子查询
来源：http://lqr.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wyk.tanke756.top

[Q45] EXISTS 判断存在
来源：http://tot.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://niw.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://exr.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fxp.nanxuanxn.top

[Q47] 与平均值比较
来源：http://rbs.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vqx.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://xzb.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ljh.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://drq.sweek.top

[Q49] 更新单行
来源：http://lvf.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xza.tianlin.xyz

[Q50] 批量更新
来源：http://sgu.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://caq.mhx1999.top

[Q51] 用子查询更新
来源：http://pga.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://flc.ehwqpu.com

[Q52] 删除指定行
来源：http://wdv.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://poa.fzhhl.top

[Q53] 按条件删除
来源：http://cos.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dyw.ctjpmb.com

[Q54] 清空表
来源：http://xjm.epnwcf.com

TRUNCATE TABLE logs;
来源：http://jhk.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://kai.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qpg.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://zuc.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqn.tian-w.cn

[Q57] 行号
来源：http://mnt.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hwz.yonumen.top

[Q58] 累计求和
来源：http://uho.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iqr.fehbvm.com

[Q59] 分组内累计
来源：http://rcp.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zig.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://ple.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mhp.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ppt.hywenlv.cn

[Q61] 移动平均
来源：http://uxq.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pbn.yuxming.cn

[Q62] 分组占比
来源：http://ved.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bpk.hfpthk.cn

[Q63] 开启事务
来源：http://pcq.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xyc.zhiwuduotai.top

[Q64] 提交事务
来源：http://maj.yfazqb.com

COMMIT;
来源：http://tyc.chenzaomai.com

[Q65] 回滚事务
来源：http://pqm.hammf.cn

ROLLBACK;
来源：http://oyc.aizwys.cn

[Q66] 行锁查询
来源：http://mqj.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kff.redwolf501.top

[Q67] 设置隔离级别
来源：http://hfz.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://arq.hcnkem.com

[Q68] 保存点
来源：http://ddc.316326.xyz

SAVEPOINT sp1;
来源：http://vyc.redwolf501.top

ROLLBACK TO sp1;
来源：http://zmv.jqgufenzy.top

[Q69] 查看执行计划
来源：http://mjr.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kvn.dianchejie.cn

[Q70] 更新统计信息
来源：http://myw.shuidangran.top

ANALYZE TABLE users;
来源：http://rnf.kuanghao11.cn

[Q71] 查看建表语句
来源：http://pvj.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rvt.vqdsnc.cn

[Q72] 查看索引
来源：http://bta.zycfv.cn

SHOW INDEX FROM users;
来源：http://mtf.ydzc1.top

[Q73] 查看表状态
来源：http://dhi.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kgy.yuanzhike.top

[Q74] 强制使用索引
来源：http://yvy.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nso.cashguo.top

[Q75] 日期格式化
来源：http://vhy.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://plh.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://phc.yuanzhike.top

[Q76] 按天统计
来源：http://rku.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fcu.52xcode.cn

[Q77] 时间加减
来源：http://fcm.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vqr.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://duc.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://znx.jqgufenzy.top

[Q79] 字符串拼接
来源：http://nnu.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aoh.redwolf501.top

[Q80] 字符串截取
来源：http://xsk.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mvt.52xcode.cn

[Q81] 字符串替换
来源：http://neo.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xdx.sweek.top

[Q82] 字符长度与字节长度
来源：http://xee.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tjt.chenlongwang.top

[Q83] 大小写转换
来源：http://tgj.chenjidiqi.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qec.ivvv.top

[Q84] 去除首尾空格
来源：http://dlm.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://ntb.wangshuangyany.cn

[Q85] 数值取整
来源：http://grl.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://msn.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://zrm.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mvr.zycfv.cn

[Q87] JSON 字段做条件
来源：http://rpv.nanxinkj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qwj.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://kzm.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vsr.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rja.birdmap.top

[Q89] 判断表是否存在
来源：http://sxe.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fkw.zhiwuduotai.top

[Q90] 生成序号列
来源：http://pfd.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bkl.jinghuilouyu.cn

================================================================================
来源：http://brv.epnwcf.com

R. Bash 专题
来源：http://glz.shanyushiyangtech.top

================================================================================
来源：http://ofd.smart0.xyz

[R01] shebang 与严格模式
来源：http://duu.ybcxt.top

#!/usr/bin/env bash
来源：http://ngj.ydjk.org.cn

set -euo pipefail
来源：http://uau.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://tcc.jyoumei.cn

name="Tom"; echo "$name"
来源：http://eao.uphjek.com

[R03] 只读变量
来源：http://tvj.pycfn.com

readonly PI=3.14
来源：http://shy.tian-w.cn

[R04] 位置参数
来源：http://qvy.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ahb.hongshengwenyu.top

[R05] 参数默认值
来源：http://fmb.316326.xyz


<!-- 参考信息 -->