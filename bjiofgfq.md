代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://cgr.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://ezr.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fbo.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oym.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npp.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rah.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qpx.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rbp.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bta.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://seh.shzxlz.cn

[P03] 生成短随机字符串
来源：http://yyy.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fyk.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bzl.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxa.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zoz.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fai.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xtr.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lle.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hem.hfpthk.cn

[P04] 求长度
来源：http://amg.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kug.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ysx.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dub.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwt.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://kum.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://vit.ehwqpu.com

Ruby: x.length;  x.size
来源：http://nlo.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ldl.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://wtn.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sbw.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rup.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cbb.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jot.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dbm.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://fxq.hammf.cn

Ruby: a == b
来源：http://weu.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tlx.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://emw.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://clb.sweek.top

PHP:  if (empty($x)) {}
来源：http://ctt.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ynt.epnwcf.com

TS:   if (x == null) {}
来源：http://zlh.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xjs.daria6918.cn

Go:   if x == nil {}
来源：http://otd.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lds.ivvv.top

C#:   if (x is null) {}
来源：http://lbo.tianlin.xyz

[P07] 防抖与节流
来源：http://hkz.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dww.tanke756.top

PHP:  // 手写时间戳比较
来源：http://oru.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrc.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqq.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://muf.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ruu.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yaj.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gcr.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://uvr.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zvd.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tvz.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nga.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://shi.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://amv.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ldl.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cwi.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dga.mhx1999.top

================================================================================
来源：http://yoq.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jnm.chenlongwang.top

================================================================================
来源：http://duu.hnxiangtu.top

[Q01] 创建表
来源：http://qdf.havefunace.top

CREATE TABLE users (
来源：http://izr.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eiu.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://dxf.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://kzo.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lxi.jinqigufen.top

);
来源：http://jwj.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://zil.sysykeji.top

CREATE TABLE orders (
来源：http://dnb.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jss.dashuyun.cn

user_id INT NOT NULL,
来源：http://cfj.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://ked.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vub.fehbvm.com

);
来源：http://bxn.hysaishi.cn

[Q03] 增加列
来源：http://zjt.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ges.feifeiyinyue.top

[Q04] 修改列类型
来源：http://csd.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://flk.cqqwz.cn

[Q05] 重命名列
来源：http://vwh.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ifx.yvedp.cn

[Q06] 删除列
来源：http://ytc.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qwf.jyoumei.cn

[Q07] 删除表
来源：http://dgs.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://bkd.cdnleiting.top

[Q08] 创建普通索引
来源：http://hft.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://yzw.tian-w.cn

[Q09] 创建唯一索引
来源：http://byf.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ytg.mhx1999.top

[Q10] 插入单行
来源：http://hhi.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zbj.yvedp.cn

[Q11] 一次插入多行
来源：http://hir.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://deb.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://ajx.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yni.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ywo.zdqjudy.top

[Q13] 忽略重复插入
来源：http://vyc.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aks.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://wcd.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hyd.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ihf.jinqigufen.top

[Q15] 查询全部
来源：http://nqi.zhiwuduotai.top

SELECT * FROM users;
来源：http://edq.wangdashe.top

[Q16] 查询指定列
来源：http://csk.dianchejie.cn

SELECT id, name FROM users;
来源：http://gja.kuanghao11.cn

[Q17] 条件查询
来源：http://jkh.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rxu.jqgufenzy.top

[Q18] 模糊匹配
来源：http://ggj.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jpm.redwolf501.top

[Q19] 范围查询
来源：http://qwr.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bpq.yangfankeji.com

[Q20] IN 列表
来源：http://aal.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iin.zhengqikj.top

[Q21] 空值判断
来源：http://epv.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://daz.haohaochexian.top

[Q22] 排序
来源：http://pgj.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dyg.52xcode.cn

[Q23] 分页
来源：http://vth.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzi.shanyushiyangtech.top

[Q24] 去重
来源：http://dvs.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://soj.cqqwz.cn

[Q25] 只取前 N 条
来源：http://geb.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nan.jianghu66.top

[Q26] 计数
来源：http://dll.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://vzr.hcnkem.com

[Q27] 条件计数
来源：http://bii.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://etc.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://odr.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gyi.meibo888.top

[Q29] 最大最小值
来源：http://hjh.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cuu.ybcxt.top

[Q30] 分组统计
来源：http://vzn.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cpn.zhoulong.xyz

[Q31] 分组后过滤
来源：http://gud.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kqq.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://ual.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dah.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yis.gzhubu.top

[Q33] 多列分组
来源：http://atg.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://exi.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://yde.dashuyun.cn

SELECT * FROM (
来源：http://bin.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pxu.cdnleiting.top

) t WHERE rn = 1;
来源：http://lvj.iojbl.cn

[Q35] 内连接
来源：http://oqo.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vyj.hfpthk.cn

[Q36] 左连接
来源：http://mzc.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eoc.zdbjq.cn

[Q37] 右连接
来源：http://jlt.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rph.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://evb.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dya.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://qxs.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qhm.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ckg.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ikt.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pbi.hywenlv.cn

[Q41] 多表连接
来源：http://asn.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bnn.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://nrl.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://ioi.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://dii.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://ezj.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cdg.yvedp.cn

[Q43] 标量子查询
来源：http://ovl.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cwu.yj20258.top

[Q44] IN 子查询
来源：http://veg.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubq.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://zse.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://npa.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://nwi.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kkt.zhijiandao.cn

[Q47] 与平均值比较
来源：http://xgk.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xmy.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://wct.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wwg.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://jqz.zhijiandao.cn

[Q49] 更新单行
来源：http://clq.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qlf.yvedp.cn

[Q50] 批量更新
来源：http://caa.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zmd.52xcode.cn

[Q51] 用子查询更新
来源：http://qey.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rfe.sufxvd.cn

[Q52] 删除指定行
来源：http://lhg.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://fwu.hnxiangtu.top

[Q53] 按条件删除
来源：http://grx.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gac.ehwqpu.com

[Q54] 清空表
来源：http://jgm.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://ltx.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://oxk.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uvo.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://kxn.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://par.shanyushiyangtech.top

[Q57] 行号
来源：http://lgv.jinghuilouyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kbr.ctjpmb.com

[Q58] 累计求和
来源：http://zas.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://czk.chenlongwang.top

[Q59] 分组内累计
来源：http://lzx.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://twb.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://bql.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qio.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wad.cqqwz.cn

[Q61] 移动平均
来源：http://cwe.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qpd.jiagoushi.top

[Q62] 分组占比
来源：http://smf.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hgg.ivvv.top

[Q63] 开启事务
来源：http://ypc.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nlf.birdmap.top

[Q64] 提交事务
来源：http://spo.zhijiandao.cn

COMMIT;
来源：http://vob.ivvv.top

[Q65] 回滚事务
来源：http://off.shanyushiyangkeji.top

ROLLBACK;
来源：http://wjh.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://gzq.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iso.meibo888.top

[Q67] 设置隔离级别
来源：http://imf.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wtx.gotoacloud.top

[Q68] 保存点
来源：http://fqm.hnqzz.top

SAVEPOINT sp1;
来源：http://gsz.tian-w.cn

ROLLBACK TO sp1;
来源：http://zff.yangfankeji.com

[Q69] 查看执行计划
来源：http://otx.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://avb.shzxlz.cn

[Q70] 更新统计信息
来源：http://iwm.zhongyouzk.top

ANALYZE TABLE users;
来源：http://kgm.bjfxy.top

[Q71] 查看建表语句
来源：http://rpz.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dbv.yangfankeji.com

[Q72] 查看索引
来源：http://gqg.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://dru.zhengqikj.top

[Q73] 查看表状态
来源：http://dto.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lnn.dashuyun.cn

[Q74] 强制使用索引
来源：http://vzy.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pza.nanxuanxn.top

[Q75] 日期格式化
来源：http://tbo.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uzx.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zah.0kj1m.cn

[Q76] 按天统计
来源：http://juz.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hwm.aibaodan.cn

[Q77] 时间加减
来源：http://boi.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cfy.52xcode.cn

[Q78] 当前时间
来源：http://lwi.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hqd.jqgufenzy.top

[Q79] 字符串拼接
来源：http://pnw.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lxb.hfpthk.cn

[Q80] 字符串截取
来源：http://yvz.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jye.jlsjyb.cn

[Q81] 字符串替换
来源：http://vbr.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bwq.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://jka.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iuu.gzhubu.top

[Q83] 大小写转换
来源：http://fpq.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gib.zhengqikj.top

[Q84] 去除首尾空格
来源：http://noe.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://mjd.gotoacloud.top

[Q85] 数值取整
来源：http://qrh.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nmj.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://awp.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://snf.cashguo.top

[Q87] JSON 字段做条件
来源：http://njz.nanxinkj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fxn.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://kbg.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pac.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mho.0kj1m.cn

[Q89] 判断表是否存在
来源：http://pto.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ttb.yonumen.top

[Q90] 生成序号列
来源：http://tli.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zhj.yongpay.top

================================================================================
来源：http://yhn.yvedp.cn

R. Bash 专题
来源：http://hkx.haohaochexian.top

================================================================================
来源：http://wqx.nwbrower.top

[R01] shebang 与严格模式
来源：http://ypd.gzhubu.top

#!/usr/bin/env bash
来源：http://xjf.dianchejie.cn

set -euo pipefail
来源：http://fgj.shzxlz.cn

[R02] 变量赋值与使用
来源：http://hzd.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://nok.ctjpmb.com

[R03] 只读变量
来源：http://kbu.yanxiufei.cn

readonly PI=3.14
来源：http://jng.zhaomingkeji.xyz

[R04] 位置参数
来源：http://urf.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nhz.jiagoushi.top

[R05] 参数默认值
来源：http://cyy.yj202588.top

name="${1:-default}"
来源：http://phu.cucudq.cn

[R06] 判断命令是否存在
来源：http://qav.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://plw.hcnkem.com

[R07] if 判断文件
来源：http://dvn.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uxv.zycfv.cn

[R08] 数值比较
来源：http://mwa.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://utu.pycfn.com

[R09] 字符串比较
来源：http://lvj.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dec.smart0.xyz

[R10] 正则匹配
来源：http://nvt.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hhl.xylfe.cn

[R11] case 多分支
来源：http://vcx.ivvv.top

case "$1" in
来源：http://zwo.shzxlz.cn

start) echo "启动" ;;
来源：http://rjr.yj202588.top

stop)  echo "停止" ;;
来源：http://zho.shuidangran.top

*)     echo "未知命令" ;;
来源：http://qmf.cdnleiting.top


<!-- 参考信息 -->