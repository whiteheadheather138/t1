代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wcc.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://yki.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vcp.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cze.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jug.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oqk.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rqp.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lct.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://trr.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dpd.chenzaomai.com

[P03] 生成短随机字符串
来源：http://yka.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rds.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://med.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rei.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dpo.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vkb.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yno.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://gln.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://isl.nwbrower.top

[P04] 求长度
来源：http://tio.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xrr.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmm.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlr.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://swv.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://yuf.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://pnp.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://gao.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hjq.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://thh.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pdh.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbh.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yih.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eez.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iwy.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lpo.mhx1999.top

Ruby: a == b
来源：http://thi.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ixg.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://adg.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mib.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://iyi.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xyy.smart0.xyz

TS:   if (x == null) {}
来源：http://dkx.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://job.uphjek.com

Go:   if x == nil {}
来源：http://rjw.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://djp.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://gej.wangshuangyany.cn

[P07] 防抖与节流
来源：http://epf.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ivj.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://aqw.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqp.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkv.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pvi.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fha.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://alf.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ojl.cheryme.top

[P08] 处理浮点精度问题
来源：http://qmy.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jlh.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fmm.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ion.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tka.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qbl.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pku.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dro.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eci.fengsongda.top

================================================================================
来源：http://xnf.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lhx.chenzaomai.com

================================================================================
来源：http://fli.svipenyu.cn

[Q01] 创建表
来源：http://nvb.hammf.cn

CREATE TABLE users (
来源：http://rxb.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jkt.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://iib.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://vaq.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hhb.hnqzz.top

);
来源：http://dvw.fzhhl.top

[Q02] 创建带外键的表
来源：http://lgr.jianghu66.top

CREATE TABLE orders (
来源：http://jpn.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rha.yj20258888.top

user_id INT NOT NULL,
来源：http://xon.ywan-chungtsiang.top

amount DECIMAL(10, 2),
来源：http://oqu.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://axj.xuanzx.com

);
来源：http://zmr.ydzc1.top

[Q03] 增加列
来源：http://yiy.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pgt.tianlin.xyz

[Q04] 修改列类型
来源：http://igq.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iam.xinyue.icu

[Q05] 重命名列
来源：http://wjm.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ncw.xuetiantiany.cn

[Q06] 删除列
来源：http://kbb.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://xlm.daria6918.cn

[Q07] 删除表
来源：http://ntg.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://gah.guannengcc.top

[Q08] 创建普通索引
来源：http://svd.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://svo.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://nlx.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvx.hesvh.cn

[Q10] 插入单行
来源：http://kly.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gos.jinqigfzy.top

[Q11] 一次插入多行
来源：http://jgr.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mvk.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://gin.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vgb.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nji.ybcxt.top

[Q13] 忽略重复插入
来源：http://jma.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hmc.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://mcq.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zyk.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kum.ydzc1.top

[Q15] 查询全部
来源：http://wka.bjfxy.top

SELECT * FROM users;
来源：http://fyz.jinqigufen.top

[Q16] 查询指定列
来源：http://pqv.fengsongda.top

SELECT id, name FROM users;
来源：http://pok.shzxlz.cn

[Q17] 条件查询
来源：http://txu.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blq.yj20258.top

[Q18] 模糊匹配
来源：http://crw.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ono.gotoacloud.top

[Q19] 范围查询
来源：http://wrv.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xoz.tianlin.xyz

[Q20] IN 列表
来源：http://qxp.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rrl.pycfn.com

[Q21] 空值判断
来源：http://hbx.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://prl.ctjpmb.com

[Q22] 排序
来源：http://ock.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bbu.cqqwz.cn

[Q23] 分页
来源：http://cev.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://get.jinqigufen.top

[Q24] 去重
来源：http://yoi.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://zvb.chenlongwang.top

[Q25] 只取前 N 条
来源：http://iur.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ase.316326.xyz

[Q26] 计数
来源：http://psg.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://fdt.redwolf501.top

[Q27] 条件计数
来源：http://all.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vtz.yonumen.top

[Q28] 求和与平均
来源：http://dez.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kcd.xziqi.cn

[Q29] 最大最小值
来源：http://xol.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dqq.nanxinkj.top

[Q30] 分组统计
来源：http://yjq.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hdv.svipenyu.cn

[Q31] 分组后过滤
来源：http://nwt.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eoc.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://dcp.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ajj.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ksn.tanke756.top

[Q33] 多列分组
来源：http://pum.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://doq.vehdjk.com

[Q34] 每组取第一条
来源：http://gik.ywan-chungtsiang.top

SELECT * FROM (
来源：http://fml.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vsw.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://lxk.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://txg.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eck.hnxiangtu.top

[Q36] 左连接
来源：http://mxu.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ohl.dashuyun.cn

[Q37] 右连接
来源：http://cvg.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fed.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bhe.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dpt.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://mjz.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fbt.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cup.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zmt.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vme.sxryk.cn

[Q41] 多表连接
来源：http://yjq.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dbt.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://zcc.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://mlq.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://viy.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://fhj.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rsz.pengpengdd.cyou

[Q43] 标量子查询
来源：http://gnq.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hhy.cucudq.cn

[Q44] IN 子查询
来源：http://bce.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hyh.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://ols.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tih.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://mhk.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ofe.ivvv.top

[Q47] 与平均值比较
来源：http://ttl.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fua.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://lvp.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wxp.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://owm.dianchejie.cn

[Q49] 更新单行
来源：http://njv.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cpc.cqqwz.cn

[Q50] 批量更新
来源：http://grv.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dry.andypj.xyz

[Q51] 用子查询更新
来源：http://mkb.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://maj.dianchejie.cn

[Q52] 删除指定行
来源：http://epv.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://mgj.dianchejie.cn

[Q53] 按条件删除
来源：http://mxa.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aet.shanyushiyangtech.top

[Q54] 清空表
来源：http://sis.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://doc.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://rsn.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dks.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://bid.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xqy.ybcxt.top

[Q57] 行号
来源：http://uvr.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jaz.daxiang520.top

[Q58] 累计求和
来源：http://tvk.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xbg.sjlbkw.cn

[Q59] 分组内累计
来源：http://qtu.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xhl.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://mfm.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nnb.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://unr.vqdsnc.cn

[Q61] 移动平均
来源：http://npu.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bno.zhengqikj.top

[Q62] 分组占比
来源：http://qgp.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://clq.hongshengwenyu.top

[Q63] 开启事务
来源：http://jza.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zfa.tanke756.top

[Q64] 提交事务
来源：http://ktw.fzhhl.top

COMMIT;
来源：http://jnm.xylfe.cn

[Q65] 回滚事务
来源：http://bkz.snrcjt.cn

ROLLBACK;
来源：http://lfq.quarkkingdee.top

[Q66] 行锁查询
来源：http://wky.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mhi.sxryk.cn

[Q67] 设置隔离级别
来源：http://vod.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mvg.yj202588.top

[Q68] 保存点
来源：http://kge.jlsjyb.cn

SAVEPOINT sp1;
来源：http://tgh.cheryme.top

ROLLBACK TO sp1;
来源：http://yqt.tanke756.top

[Q69] 查看执行计划
来源：http://rjv.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tub.shzxlz.cn

[Q70] 更新统计信息
来源：http://wgv.ydjk.org.cn

ANALYZE TABLE users;
来源：http://esl.snrcjt.cn

[Q71] 查看建表语句
来源：http://vmw.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://btm.shuidangran.top

[Q72] 查看索引
来源：http://sfq.fengsongda.top

SHOW INDEX FROM users;
来源：http://kpl.jqgfzy.top

[Q73] 查看表状态
来源：http://ard.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ihl.guannengcc.top

[Q74] 强制使用索引
来源：http://ajf.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zha.nanxuanxn.top

[Q75] 日期格式化
来源：http://dtb.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kyl.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lda.yuxming.cn

[Q76] 按天统计
来源：http://obg.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://coq.snrcjt.cn

[Q77] 时间加减
来源：http://kgf.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gia.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://jkt.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tlk.svipenyu.cn

[Q79] 字符串拼接
来源：http://mqm.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fvl.wangshuangyany.cn

[Q80] 字符串截取
来源：http://hnw.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://goo.zycfv.cn

[Q81] 字符串替换
来源：http://bsq.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bsc.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://qsf.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jrm.shuidangran.top

[Q83] 大小写转换
来源：http://yie.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xwe.chenlongwang.top

[Q84] 去除首尾空格
来源：http://scp.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://dln.shuidangran.top

[Q85] 数值取整
来源：http://wxu.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ftw.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://bes.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lnr.havefunace.top

[Q87] JSON 字段做条件
来源：http://iwu.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pfr.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://idn.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gsn.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oip.xinyue.icu

[Q89] 判断表是否存在
来源：http://cer.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lsu.pycfn.com

[Q90] 生成序号列
来源：http://krw.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jac.zhixingplan.top

================================================================================
来源：http://rif.yuxming.cn

R. Bash 专题
来源：http://fzw.hesvh.cn

================================================================================
来源：http://tip.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://zeb.meibo888.top

#!/usr/bin/env bash
来源：http://djb.jqgfzy.top

set -euo pipefail
来源：http://vhf.jiagoushi.top

[R02] 变量赋值与使用
来源：http://vgw.yongpay.top

name="Tom"; echo "$name"
来源：http://apr.shzxlz.cn

[R03] 只读变量
来源：http://kgl.fzhhl.top

readonly PI=3.14
来源：http://itk.hfpthk.cn

[R04] 位置参数
来源：http://xpv.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mrf.chenjidiqi.icu

[R05] 参数默认值
来源：http://lyv.fehbvm.com

name="${1:-default}"
来源：http://jbz.dashuyun.cn

[R06] 判断命令是否存在
来源：http://wdk.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nok.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://uvb.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://erz.shzxlz.cn

[R08] 数值比较
来源：http://fya.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://neo.hfpthk.cn

[R09] 字符串比较
来源：http://jgn.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mqf.tianlin.xyz

[R10] 正则匹配
来源：http://efs.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wya.shanyushiyangtech.top

[R11] case 多分支
来源：http://qgd.dianchejie.cn

case "$1" in
来源：http://rfy.hcnkem.com

start) echo "启动" ;;
来源：http://arm.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://ftw.sweek.top

*)     echo "未知命令" ;;
来源：http://iys.wangshuangyany.cn


<!-- 参考信息 -->