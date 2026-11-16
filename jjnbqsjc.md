代发 wailian999

C#:   Parallel.For
来源：http://dny.gaohongyu789.top

================================================================================
来源：http://qmi.bbcook.cn

P. 常用工具函数
来源：http://bfd.redwolf501.top

================================================================================
来源：http://axe.epnwcf.com

[P01] 生成 UUID
来源：http://ekd.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://qcq.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lvl.iojbl.cn

JS:   crypto.randomUUID()
来源：http://cxh.hammf.cn

TS:   crypto.randomUUID()
来源：http://dzn.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://zqw.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://dti.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://tbz.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://klj.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://dem.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://shk.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lrm.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gqb.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xmx.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xgo.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zun.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cuf.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hhp.dianchejie.cn

[P03] 生成短随机字符串
来源：http://hlj.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jce.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tpy.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jkh.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxf.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://etz.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uie.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ouw.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ocb.xuanzx.com

[P04] 求长度
来源：http://gzg.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mra.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fgb.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bsa.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwi.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://rly.hesvh.cn

Go:   len(arr);  len(m)
来源：http://msw.snrcjt.cn

Ruby: x.length;  x.size
来源：http://izf.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ojl.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://uxn.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://meh.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gwt.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bps.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mgz.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dff.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://zbf.shanyushiyangkeji.top

Ruby: a == b
来源：http://pjh.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lba.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rfn.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tva.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://nmq.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eqv.svipenyu.cn

TS:   if (x == null) {}
来源：http://erb.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tlc.sysykeji.top

Go:   if x == nil {}
来源：http://sar.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yib.guannengcc.top

C#:   if (x is null) {}
来源：http://wnq.hammf.cn

[P07] 防抖与节流
来源：http://amf.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://alu.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://iaq.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edr.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://goo.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zfy.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://btx.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qll.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hjf.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://xqr.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iot.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bkb.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ydb.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ogk.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mps.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fkx.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nlf.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mmu.cqqwz.cn

================================================================================
来源：http://mbd.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qlz.xingfuxueyuan.xyz

================================================================================
来源：http://ptt.chenlongwang.top

[Q01] 创建表
来源：http://unh.daria6918.cn

CREATE TABLE users (
来源：http://nrc.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hhs.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://hhi.ydjk.org.cn

email VARCHAR(100) UNIQUE,
来源：http://rqj.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxr.chenzaomai.com

);
来源：http://mfu.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://iuc.xuanzx.com

CREATE TABLE orders (
来源：http://kkn.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzk.hfpthk.cn

user_id INT NOT NULL,
来源：http://nmc.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://ydo.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fxh.chenzaomai.com

);
来源：http://xom.hysaishi.cn

[Q03] 增加列
来源：http://kyi.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kco.yueranfly.top

[Q04] 修改列类型
来源：http://ugz.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rca.yongpay.top

[Q05] 重命名列
来源：http://fes.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zzb.fanxiaobao.xyz

[Q06] 删除列
来源：http://heu.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://hqt.c1oappe.top

[Q07] 删除表
来源：http://kfk.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://mcu.tian-w.cn

[Q08] 创建普通索引
来源：http://bnb.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lhu.fengsongda.top

[Q09] 创建唯一索引
来源：http://keb.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jzv.zhixingplan.top

[Q10] 插入单行
来源：http://yyp.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iwj.jiagoushi.top

[Q11] 一次插入多行
来源：http://oyo.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mpr.yj202588.top

[Q12] 插入后取自增 ID
来源：http://xuo.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lhw.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hlv.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://nvs.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hjc.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://qbi.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://llw.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://khm.jinqigufen.top

[Q15] 查询全部
来源：http://wbk.svipenyu.cn

SELECT * FROM users;
来源：http://huq.redwolf501.top

[Q16] 查询指定列
来源：http://cbr.chenzaomai.com

SELECT id, name FROM users;
来源：http://upa.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://nwg.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tqn.316326.xyz

[Q18] 模糊匹配
来源：http://cqr.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://byj.zdqjudy.top

[Q19] 范围查询
来源：http://qdx.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sez.xziqi.cn

[Q20] IN 列表
来源：http://dai.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vgf.aizwys.cn

[Q21] 空值判断
来源：http://yrm.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hgx.nanxinkj.top

[Q22] 排序
来源：http://kac.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bub.pengpengdd.cyou

[Q23] 分页
来源：http://igi.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://haq.ydzc1.top

[Q24] 去重
来源：http://kfr.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://qwo.0kj1m.cn

[Q25] 只取前 N 条
来源：http://scl.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qlp.ctjpmb.com

[Q26] 计数
来源：http://wsg.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://wfz.52xcode.cn

[Q27] 条件计数
来源：http://fgi.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sld.dashuyun.cn

[Q28] 求和与平均
来源：http://tfk.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xoy.hfpthk.cn

[Q29] 最大最小值
来源：http://apg.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://utm.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://cpb.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://esx.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://udv.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ork.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://ypt.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fno.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lqp.sufxvd.cn

[Q33] 多列分组
来源：http://ddh.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgs.jianghu66.top

[Q34] 每组取第一条
来源：http://lcf.yueranfly.top

SELECT * FROM (
来源：http://xvv.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cem.yueranfly.top

) t WHERE rn = 1;
来源：http://ueo.yongpay.top

[Q35] 内连接
来源：http://fza.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ytq.hysaishi.cn

[Q36] 左连接
来源：http://muv.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vmk.yangfankeji.com

[Q37] 右连接
来源：http://jcs.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cyr.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://yur.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zmm.cashguo.top

[Q39] 自连接（查上下级）
来源：http://djt.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nvs.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qlb.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dzj.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ueq.feifeiyinyue.top

[Q41] 多表连接
来源：http://ufc.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fup.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://mlg.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://pno.uphjek.com

[Q42] 连接条件附加过滤
来源：http://smy.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://uxw.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://plf.yonumen.top

[Q43] 标量子查询
来源：http://bke.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wjy.hnqzz.top

[Q44] IN 子查询
来源：http://any.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://plk.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://cjj.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pwh.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://rce.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eup.cashguo.top

[Q47] 与平均值比较
来源：http://zvs.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uvb.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://qno.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dmd.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://oxa.fzhhl.top

[Q49] 更新单行
来源：http://cry.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pcz.gogol.net.cn

[Q50] 批量更新
来源：http://sms.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://doz.gzhubu.top

[Q51] 用子查询更新
来源：http://kfy.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ser.mhx1999.top

[Q52] 删除指定行
来源：http://lqk.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://sep.jlsjyb.cn

[Q53] 按条件删除
来源：http://vuf.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sjt.fktsv.cn

[Q54] 清空表
来源：http://maf.yuxming.cn

TRUNCATE TABLE logs;
来源：http://kjj.bjfxy.top

[Q55] 排名（并列占位）
来源：http://wun.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rwz.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://nvp.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mif.shanyushiyangkeji.top

[Q57] 行号
来源：http://dpc.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oln.guannengcc.top

[Q58] 累计求和
来源：http://apx.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uit.jlsjyb.cn

[Q59] 分组内累计
来源：http://nov.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wla.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://ceo.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gsa.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hom.yuanzhike.top

[Q61] 移动平均
来源：http://efg.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pii.andypj.xyz

[Q62] 分组占比
来源：http://wui.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nhr.tianlin.xyz

[Q63] 开启事务
来源：http://xuy.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://odl.gzhubu.top

[Q64] 提交事务
来源：http://gqg.hammf.cn

COMMIT;
来源：http://slo.hfpthk.cn

[Q65] 回滚事务
来源：http://laz.epnwcf.com

ROLLBACK;
来源：http://ylh.vqdsnc.cn

[Q66] 行锁查询
来源：http://snq.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://stp.fengsongda.top

[Q67] 设置隔离级别
来源：http://ehw.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ipu.ivvv.top

[Q68] 保存点
来源：http://ojo.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://pxv.epnwcf.com

ROLLBACK TO sp1;
来源：http://qts.ybcxt.top

[Q69] 查看执行计划
来源：http://evo.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://chn.ehwqpu.com

[Q70] 更新统计信息
来源：http://lwv.guannengcc.top

ANALYZE TABLE users;
来源：http://bwl.jqgufenzy.top

[Q71] 查看建表语句
来源：http://tuh.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kug.ivvv.top

[Q72] 查看索引
来源：http://qoa.316326.xyz

SHOW INDEX FROM users;
来源：http://erj.pycfn.com

[Q73] 查看表状态
来源：http://uta.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hex.mhx1999.top

[Q74] 强制使用索引
来源：http://jqy.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://clk.ydjk.org.cn

[Q75] 日期格式化
来源：http://eax.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jro.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://apd.sufxvd.cn

[Q76] 按天统计
来源：http://mdh.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wet.gaohongyu789.top

[Q77] 时间加减
来源：http://ano.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://num.haohaochexian.top

[Q78] 当前时间
来源：http://yaw.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yqc.uphjek.com

[Q79] 字符串拼接
来源：http://ikn.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yui.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://xkk.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eyb.cdnleiting.top

[Q81] 字符串替换
来源：http://oei.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tdz.yj20258.top

[Q82] 字符长度与字节长度
来源：http://ngp.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://abi.zdqjudy.top

[Q83] 大小写转换
来源：http://cqn.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qlm.hammf.cn

[Q84] 去除首尾空格
来源：http://hfh.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://eya.ivvv.top

[Q85] 数值取整
来源：http://mwp.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wqn.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://nur.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aps.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://wex.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nzm.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://tjm.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://isf.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://liu.yonumen.top

[Q89] 判断表是否存在
来源：http://klb.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cux.hysaishi.cn

[Q90] 生成序号列
来源：http://avr.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ule.zhiwuduotai.top

================================================================================
来源：http://wvj.zdbjq.cn

R. Bash 专题
来源：http://stp.pengpengdd.cyou

================================================================================
来源：http://ohf.cashguo.top

[R01] shebang 与严格模式
来源：http://gbf.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://fwj.yueranfly.top

set -euo pipefail
来源：http://kzo.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://vql.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://why.nwbrower.top

[R03] 只读变量
来源：http://jmc.vqdsnc.cn

readonly PI=3.14
来源：http://tdy.hysaishi.cn

[R04] 位置参数
来源：http://wsf.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jps.zhiwuduotai.top

[R05] 参数默认值
来源：http://xzp.yj20258888.top

name="${1:-default}"
来源：http://ylc.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://wdh.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tuk.hongshengwenyu.top

[R07] if 判断文件
来源：http://dye.svipenyu.cn


<!-- 参考信息 -->