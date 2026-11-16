代发 wailian999

TS:   crypto.randomUUID()
来源：http://ymw.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://nlx.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://zna.tarul.cn

Ruby: SecureRandom.uuid
来源：http://ggp.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://piu.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://lqj.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yjv.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xae.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nxr.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jvu.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nxd.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fzs.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pvz.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lwp.vehdjk.com

[P03] 生成短随机字符串
来源：http://sts.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cfj.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cbk.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qzx.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://itj.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ezz.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qfk.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ewd.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kgm.bbcook.cn

[P04] 求长度
来源：http://hnv.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qyg.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sak.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xfv.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpx.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://fch.nwbrower.top

Go:   len(arr);  len(m)
来源：http://zka.shzxlz.cn

Ruby: x.length;  x.size
来源：http://cca.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://yyj.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://mlo.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aak.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uem.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://maa.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tlh.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dub.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://raa.sufxvd.cn

Ruby: a == b
来源：http://jhf.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ajs.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwn.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agl.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://xvw.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mwm.yvedp.cn

TS:   if (x == null) {}
来源：http://smu.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://sei.hcnkem.com

Go:   if x == nil {}
来源：http://skh.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kwv.snrcjt.cn

C#:   if (x is null) {}
来源：http://fcv.ydjk.org.cn

[P07] 防抖与节流
来源：http://apg.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xxz.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://cwr.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bwy.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgw.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opt.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tlf.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://qbz.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://izo.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://qot.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wmg.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hiq.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bsj.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cyk.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cqm.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qvi.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://znt.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wlu.ivvv.top

================================================================================
来源：http://lgs.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://brd.dianchejie.cn

================================================================================
来源：http://geu.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://hkx.yonumen.top

CREATE TABLE users (
来源：http://qbt.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hfe.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://fsp.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://aah.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vvc.zhengqikj.top

);
来源：http://xpc.havefunace.top

[Q02] 创建带外键的表
来源：http://ysw.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://vyj.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zum.yuxming.cn

user_id INT NOT NULL,
来源：http://dtz.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://eod.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pgt.ydzc1.top

);
来源：http://cvb.hcnkem.com

[Q03] 增加列
来源：http://sdw.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfi.jiagoushi.top

[Q04] 修改列类型
来源：http://gid.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vaa.feifeiyinyue.top

[Q05] 重命名列
来源：http://wrj.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bnb.nwbrower.top

[Q06] 删除列
来源：http://ivf.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://nko.wangshuangyany.cn

[Q07] 删除表
来源：http://qed.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://rxg.bbcook.cn

[Q08] 创建普通索引
来源：http://dpf.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://awx.jiagoushi.top

[Q09] 创建唯一索引
来源：http://rrn.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yzh.bjfxy.top

[Q10] 插入单行
来源：http://dcw.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bhz.ctjpmb.com

[Q11] 一次插入多行
来源：http://jlh.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cjf.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://uvh.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bfm.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vir.bjfxy.top

[Q13] 忽略重复插入
来源：http://iqd.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dfl.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://yfk.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dui.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lox.yj20258888.top

[Q15] 查询全部
来源：http://bfe.pengpengdd.cyou

SELECT * FROM users;
来源：http://bdw.yj20258888.top

[Q16] 查询指定列
来源：http://cbo.tanke756.top

SELECT id, name FROM users;
来源：http://yok.iojbl.cn

[Q17] 条件查询
来源：http://ftn.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kmc.mhx1999.top

[Q18] 模糊匹配
来源：http://lsk.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wep.52xcode.cn

[Q19] 范围查询
来源：http://ahg.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://giw.tian-w.cn

[Q20] IN 列表
来源：http://rfz.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yfr.yj202588.top

[Q21] 空值判断
来源：http://mkm.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://naw.fehbvm.com

[Q22] 排序
来源：http://eix.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fwf.ydjk.org.cn

[Q23] 分页
来源：http://ume.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://anu.hnxiangtu.top

[Q24] 去重
来源：http://kxi.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://gne.mhx1999.top

[Q25] 只取前 N 条
来源：http://tbq.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dsw.zhongyouzk.top

[Q26] 计数
来源：http://kba.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://icz.gotoacloud.top

[Q27] 条件计数
来源：http://cby.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wzf.sweek.top

[Q28] 求和与平均
来源：http://qwd.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qdb.fzhhl.top

[Q29] 最大最小值
来源：http://gox.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vyj.birdmap.top

[Q30] 分组统计
来源：http://iwv.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rph.316326.xyz

[Q31] 分组后过滤
来源：http://cnk.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kze.hnqzz.top

[Q32] 分组拼接字符串
来源：http://diy.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lrq.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://efy.kuanghao11.cn

[Q33] 多列分组
来源：http://pyf.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://doh.gaohongyu789.top

[Q34] 每组取第一条
来源：http://cab.nanxinkj.top

SELECT * FROM (
来源：http://ora.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hxw.xinyue.icu

) t WHERE rn = 1;
来源：http://nrs.bjfxy.top

[Q35] 内连接
来源：http://utj.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qph.quarkkingdee.top

[Q36] 左连接
来源：http://fvy.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xbb.tian-w.cn

[Q37] 右连接
来源：http://uiv.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lzq.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vrl.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wnj.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://iwm.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fhg.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pbk.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yza.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zzg.yvedp.cn

[Q41] 多表连接
来源：http://amw.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oyr.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://swa.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://tqd.yj202588.top

[Q42] 连接条件附加过滤
来源：http://uuk.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://bgr.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sfg.jlsjyb.cn

[Q43] 标量子查询
来源：http://ahq.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xqg.316326.xyz

[Q44] IN 子查询
来源：http://xks.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kqh.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://zbl.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wxz.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oej.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lqr.hysaishi.cn

[Q47] 与平均值比较
来源：http://stl.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nss.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://yfv.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://brl.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://zaw.hysaishi.cn

[Q49] 更新单行
来源：http://mkp.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ktz.nwbrower.top

[Q50] 批量更新
来源：http://nux.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eqk.tianlin.xyz

[Q51] 用子查询更新
来源：http://pco.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qyi.zhixingplan.top

[Q52] 删除指定行
来源：http://cxg.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://euu.jqgfzy.top

[Q53] 按条件删除
来源：http://pjg.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xmo.hesvh.cn

[Q54] 清空表
来源：http://kka.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://qoc.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://mfb.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fxh.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://yky.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uds.52xcode.cn

[Q57] 行号
来源：http://kba.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rfj.jlsjyb.cn

[Q58] 累计求和
来源：http://etm.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uwd.yongpay.top

[Q59] 分组内累计
来源：http://svw.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hdx.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://ual.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wrt.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iyp.jiagoushi.top

[Q61] 移动平均
来源：http://bhu.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rdt.sweek.top

[Q62] 分组占比
来源：http://cxt.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gip.jqgfzy.top

[Q63] 开启事务
来源：http://uye.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wbf.hywenlv.cn

[Q64] 提交事务
来源：http://wxt.gzhubu.top

COMMIT;
来源：http://dog.jqgufenzy.top

[Q65] 回滚事务
来源：http://dmn.yj20258.top

ROLLBACK;
来源：http://nwq.kuanghao11.cn

[Q66] 行锁查询
来源：http://jqk.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zhp.sweek.top

[Q67] 设置隔离级别
来源：http://hpg.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tcl.daria6918.cn

[Q68] 保存点
来源：http://mgc.jqgufenzy.top

SAVEPOINT sp1;
来源：http://ffh.aibaodan.cn

ROLLBACK TO sp1;
来源：http://wux.nanxuanxn.top

[Q69] 查看执行计划
来源：http://mvk.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cgy.hnqzz.top

[Q70] 更新统计信息
来源：http://pvb.dianchejie.cn

ANALYZE TABLE users;
来源：http://dgi.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://gxy.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fib.guowangkeji.top

[Q72] 查看索引
来源：http://fsa.zhengqikj.top

SHOW INDEX FROM users;
来源：http://oci.yvedp.cn

[Q73] 查看表状态
来源：http://ghe.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rog.vehdjk.com

[Q74] 强制使用索引
来源：http://biu.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ltc.shzxlz.cn

[Q75] 日期格式化
来源：http://aev.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aql.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hti.xylfe.cn

[Q76] 按天统计
来源：http://eok.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xwt.zycfv.cn

[Q77] 时间加减
来源：http://bsz.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rsh.gaohongyu789.top

[Q78] 当前时间
来源：http://zhc.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yij.gzhubu.top

[Q79] 字符串拼接
来源：http://lul.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ldt.sjlbkw.cn

[Q80] 字符串截取
来源：http://nof.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lzw.guowangkeji.top

[Q81] 字符串替换
来源：http://wod.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zkm.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://zwn.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dpw.9152youxi.cn

[Q83] 大小写转换
来源：http://hac.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://afq.nwbrower.top

[Q84] 去除首尾空格
来源：http://vyl.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://plh.tarul.cn

[Q85] 数值取整
来源：http://hqa.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wis.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://pus.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvh.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://kdq.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kwb.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://gks.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cvi.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gau.hysaishi.cn

[Q89] 判断表是否存在
来源：http://hii.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dlp.ydzc1.top

[Q90] 生成序号列
来源：http://vmt.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qme.ybcxt.top

================================================================================
来源：http://ljf.jqgfzy.top

R. Bash 专题
来源：http://vwx.hongshengwenyu.top

================================================================================
来源：http://ceu.9152youxi.cn

[R01] shebang 与严格模式
来源：http://mxe.tarul.cn

#!/usr/bin/env bash
来源：http://hcm.hywenlv.cn

set -euo pipefail
来源：http://cgx.havefunace.top

[R02] 变量赋值与使用
来源：http://zra.shuidangran.top

name="Tom"; echo "$name"
来源：http://ylr.pengpengdd.cyou

[R03] 只读变量
来源：http://pyr.chenjidiqi.icu

readonly PI=3.14
来源：http://ohu.gotoacloud.top

[R04] 位置参数
来源：http://vtc.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qwj.ctjpmb.com

[R05] 参数默认值
来源：http://qmx.hysaishi.cn

name="${1:-default}"
来源：http://fwe.hcnkem.com

[R06] 判断命令是否存在
来源：http://zfs.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xzt.guannengcc.top

[R07] if 判断文件
来源：http://zad.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qbk.9152youxi.cn

[R08] 数值比较
来源：http://ckw.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://qpf.hnxiangtu.top

[R09] 字符串比较
来源：http://hqt.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ysk.zhengqikj.top

[R10] 正则匹配
来源：http://qnx.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://msu.tian-w.cn

[R11] case 多分支
来源：http://xbc.havefunace.top


<!-- 参考信息 -->