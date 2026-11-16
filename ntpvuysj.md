代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ezx.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qss.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xls.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zjn.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://slr.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rvh.tanke756.top

[P03] 生成短随机字符串
来源：http://lvs.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://odt.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://njz.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifz.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rlg.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xne.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nmh.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hfr.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gbr.yvedp.cn

[P04] 求长度
来源：http://tbr.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ido.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kcf.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ulj.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sai.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://fnc.epnwcf.com

Go:   len(arr);  len(m)
来源：http://fuo.vehdjk.com

Ruby: x.length;  x.size
来源：http://egb.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oeg.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://mbw.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://csn.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kpk.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tch.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nur.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://paf.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://avk.wangdashe.top

Ruby: a == b
来源：http://fpu.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cqy.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fsa.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fdz.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://pgi.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fhu.redwolf501.top

TS:   if (x == null) {}
来源：http://ymg.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ekk.c1oappe.top

Go:   if x == nil {}
来源：http://zjt.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jgj.cqqwz.cn

C#:   if (x is null) {}
来源：http://bvd.nanxuanxn.top

[P07] 防抖与节流
来源：http://tgc.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xud.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://tgs.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://glg.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyq.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cdb.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://abk.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqw.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jmz.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://dry.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pcv.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://udq.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tjw.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erx.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://orl.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://flj.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zva.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lqu.zhengqikj.top

================================================================================
来源：http://bwn.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jgc.yonumen.top

================================================================================
来源：http://dwq.shzxlz.cn

[Q01] 创建表
来源：http://jhh.kuanghao11.cn

CREATE TABLE users (
来源：http://xbc.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bki.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://xid.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://oqo.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rvb.ivvv.top

);
来源：http://ghj.gogol.net.cn

[Q02] 创建带外键的表
来源：http://zgd.mhx1999.top

CREATE TABLE orders (
来源：http://tbb.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jun.aibaodan.cn

user_id INT NOT NULL,
来源：http://tuo.ivvv.top

amount DECIMAL(10, 2),
来源：http://kig.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hvg.hywenlv.cn

);
来源：http://ziu.chenzaomai.com

[Q03] 增加列
来源：http://roj.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ldi.sjlbkw.cn

[Q04] 修改列类型
来源：http://oxc.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hiy.jlsjyb.cn

[Q05] 重命名列
来源：http://nqr.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iwf.sjlbkw.cn

[Q06] 删除列
来源：http://azj.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://fyr.tanke756.top

[Q07] 删除表
来源：http://tbv.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://kvk.ydjk.org.cn

[Q08] 创建普通索引
来源：http://hwo.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pjv.uphjek.com

[Q09] 创建唯一索引
来源：http://cpg.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zwm.iojbl.cn

[Q10] 插入单行
来源：http://mix.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jfr.ydjk.org.cn

[Q11] 一次插入多行
来源：http://gmv.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fpr.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://znz.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://leq.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swv.xziqi.cn

[Q13] 忽略重复插入
来源：http://tip.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://amh.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://rxz.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxg.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qrz.feifeiyinyue.top

[Q15] 查询全部
来源：http://hnc.fktsv.cn

SELECT * FROM users;
来源：http://tbg.tarul.cn

[Q16] 查询指定列
来源：http://vpd.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://ehb.cheryme.top

[Q17] 条件查询
来源：http://ziv.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ncw.havefunace.top

[Q18] 模糊匹配
来源：http://duq.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qms.cheryme.top

[Q19] 范围查询
来源：http://toe.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ldy.nwbrower.top

[Q20] IN 列表
来源：http://vsg.kuanghao11.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bzd.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://uwo.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wor.hysaishi.cn

[Q22] 排序
来源：http://frv.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bzd.vqdsnc.cn

[Q23] 分页
来源：http://byf.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ohe.jiagoushi.top

[Q24] 去重
来源：http://jqg.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://cxc.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://tsf.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eib.yuanzhike.top

[Q26] 计数
来源：http://gly.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://thv.ctjpmb.com

[Q27] 条件计数
来源：http://hrd.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://org.gotoacloud.top

[Q28] 求和与平均
来源：http://gyb.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cww.316326.xyz

[Q29] 最大最小值
来源：http://pzq.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xpw.fehbvm.com

[Q30] 分组统计
来源：http://lup.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ggw.quarkkingdee.top

[Q31] 分组后过滤
来源：http://wwi.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wbs.daxiang520.top

[Q32] 分组拼接字符串
来源：http://obu.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jaw.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lze.ybcxt.top

[Q33] 多列分组
来源：http://egr.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kvg.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://wsq.ivvv.top

SELECT * FROM (
来源：http://qyf.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovf.gogol.net.cn

) t WHERE rn = 1;
来源：http://nec.zhijiandao.cn

[Q35] 内连接
来源：http://pjs.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://utf.sxryk.cn

[Q36] 左连接
来源：http://aij.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pgy.ywan-chungtsiang.top

[Q37] 右连接
来源：http://gpw.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mhb.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://khh.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wfq.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://bno.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fhj.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mfy.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iqp.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ykr.ydjk.org.cn

[Q41] 多表连接
来源：http://bkv.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hdt.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://osk.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://cfu.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://vab.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://xib.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ezw.sjlbkw.cn

[Q43] 标量子查询
来源：http://ppy.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xft.yj20258.top

[Q44] IN 子查询
来源：http://hnv.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qfo.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://jse.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxe.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://tjr.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qme.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://wtd.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://etq.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://jkd.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kix.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://asv.shuidangran.top

[Q49] 更新单行
来源：http://jos.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ker.sweek.top

[Q50] 批量更新
来源：http://ssb.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pvg.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://wsv.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pog.redwolf501.top

[Q52] 删除指定行
来源：http://axj.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://zdn.guannengcc.top

[Q53] 按条件删除
来源：http://fpg.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dru.haohaochexian.top

[Q54] 清空表
来源：http://mtv.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://ooi.smart0.xyz

[Q55] 排名（并列占位）
来源：http://qkr.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hnm.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://ztz.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://krd.ydjk.org.cn

[Q57] 行号
来源：http://wvb.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qok.ppjwa.cn

[Q58] 累计求和
来源：http://skd.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ajh.yueranfly.top

[Q59] 分组内累计
来源：http://juw.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rma.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://wrg.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zoe.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://loj.daxiang520.top

[Q61] 移动平均
来源：http://vli.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rty.chenlongwang.top

[Q62] 分组占比
来源：http://dem.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jof.gzhubu.top

[Q63] 开启事务
来源：http://bxw.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jfm.chenlongwang.top

[Q64] 提交事务
来源：http://yky.shuidangran.top

COMMIT;
来源：http://iyn.zdbjq.cn

[Q65] 回滚事务
来源：http://nxc.yonumen.top

ROLLBACK;
来源：http://vau.9152youxi.cn

[Q66] 行锁查询
来源：http://eid.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xpu.yuanzhike.top

[Q67] 设置隔离级别
来源：http://agv.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hhp.316326.xyz

[Q68] 保存点
来源：http://jry.zhixingplan.top

SAVEPOINT sp1;
来源：http://fcg.gzhubu.top

ROLLBACK TO sp1;
来源：http://vqy.hammf.cn

[Q69] 查看执行计划
来源：http://jaa.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xbw.316326.xyz

[Q70] 更新统计信息
来源：http://uky.sxryk.cn

ANALYZE TABLE users;
来源：http://mal.cashguo.top

[Q71] 查看建表语句
来源：http://luf.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pgw.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://toa.hfpthk.cn

SHOW INDEX FROM users;
来源：http://kle.hywenlv.cn

[Q73] 查看表状态
来源：http://yrx.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xzd.fzhhl.top

[Q74] 强制使用索引
来源：http://ypw.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yye.fktsv.cn

[Q75] 日期格式化
来源：http://epi.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyt.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://noj.yj20258888.top

[Q76] 按天统计
来源：http://hgi.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://trx.wangshuangyany.cn

[Q77] 时间加减
来源：http://cvl.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sbm.wangdashe.top

[Q78] 当前时间
来源：http://kyg.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ywr.316326.xyz

[Q79] 字符串拼接
来源：http://dyc.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qxe.hywenlv.cn

[Q80] 字符串截取
来源：http://aue.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qic.snrcjt.cn

[Q81] 字符串替换
来源：http://yol.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yei.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://xzt.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sig.gogol.net.cn

[Q83] 大小写转换
来源：http://voy.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pfa.haohaochexian.top

[Q84] 去除首尾空格
来源：http://mks.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://psm.haohaochexian.top

[Q85] 数值取整
来源：http://qvx.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nbk.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://wpv.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fyh.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://nrn.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kjj.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://fio.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bzx.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xqm.fzhhl.top

[Q89] 判断表是否存在
来源：http://daj.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hvc.daxiang520.top

[Q90] 生成序号列
来源：http://kdd.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhz.pengpengdd.cyou

================================================================================
来源：http://auk.ywan-chungtsiang.top

R. Bash 专题
来源：http://hmo.xinyue.icu

================================================================================
来源：http://msx.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://uzw.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://dcc.daria6918.cn

set -euo pipefail
来源：http://sye.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://qfh.c1oappe.top

name="Tom"; echo "$name"
来源：http://axm.yj20258.top

[R03] 只读变量
来源：http://abq.bjfxy.top

readonly PI=3.14
来源：http://zsi.zhiwuduotai.top

[R04] 位置参数
来源：http://dxm.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aai.jlsjyb.cn

[R05] 参数默认值
来源：http://kxj.smart0.xyz

name="${1:-default}"
来源：http://izh.chenlongwang.top

[R06] 判断命令是否存在
来源：http://jeq.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ktr.shzxlz.cn

[R07] if 判断文件
来源：http://kov.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qev.smart0.xyz

[R08] 数值比较
来源：http://wni.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qvv.iojbl.cn

[R09] 字符串比较
来源：http://mdv.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wxm.jiagoushi.top

[R10] 正则匹配
来源：http://zjd.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mqa.xuanzx.com

[R11] case 多分支
来源：http://kjj.jinqigfzy.top

case "$1" in
来源：http://ozy.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://uzv.pycfn.com

stop)  echo "停止" ;;
来源：http://tjl.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://fjd.meibo888.top

esac
来源：http://shl.ctjpmb.com

[R12] for 遍历文件
来源：http://kkh.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://foq.c1oappe.top

[R13] for 计数循环
来源：http://dtj.hammf.cn


<!-- 参考信息 -->