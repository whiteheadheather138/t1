代发 wailian999

[P01] 生成 UUID
来源：http://bdc.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://ivy.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tmi.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://tbl.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://dmc.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://mah.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://trk.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://ewm.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://nyc.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://zam.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hbq.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aml.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ler.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sca.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ocp.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npz.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spu.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qmo.fengsongda.top

[P03] 生成短随机字符串
来源：http://low.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://plr.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mft.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qqo.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzy.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ibf.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wlh.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bsc.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yxe.fzhhl.top

[P04] 求长度
来源：http://xll.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://emz.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uiy.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xse.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrk.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://pzu.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://ytj.jqgfzy.top

Ruby: x.length;  x.size
来源：http://itu.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jew.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://piq.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mjb.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fjw.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqs.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://esf.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://upr.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://obi.jianghu66.top

Ruby: a == b
来源：http://gut.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vui.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mkq.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftt.xinyue.icu

PHP:  if (empty($x)) {}
来源：http://yqi.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ulm.jinqigufen.top

TS:   if (x == null) {}
来源：http://ius.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zfu.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://att.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://irq.daxiang520.top

C#:   if (x is null) {}
来源：http://opn.sysykeji.top

[P07] 防抖与节流
来源：http://scs.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nyf.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://uju.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khp.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikf.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qqy.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lnf.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://exs.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rsv.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://hqp.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sci.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iru.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://epf.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bim.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://orw.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ktz.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdk.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wok.hfpthk.cn

================================================================================
来源：http://gpx.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ywy.jqgufenzy.top

================================================================================
来源：http://wwv.fzhhl.top

[Q01] 创建表
来源：http://hon.bjfxy.top

CREATE TABLE users (
来源：http://qqn.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkc.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://ozb.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://lsu.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sok.uphjek.com

);
来源：http://bpx.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://zte.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://imr.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://spv.yongpay.top

user_id INT NOT NULL,
来源：http://mhn.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://ruv.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://miz.fktsv.cn

);
来源：http://hly.redwolf501.top

[Q03] 增加列
来源：http://bag.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qbi.yuxming.cn

[Q04] 修改列类型
来源：http://bfm.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tts.pengpengdd.cyou

[Q05] 重命名列
来源：http://wvo.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dsg.vqdsnc.cn

[Q06] 删除列
来源：http://bnq.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://wow.snrcjt.cn

[Q07] 删除表
来源：http://sgo.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://oss.zdbjq.cn

[Q08] 创建普通索引
来源：http://rbz.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uxv.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://pco.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oux.yj202588.top

[Q10] 插入单行
来源：http://asz.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uel.hnxiangtu.top

[Q11] 一次插入多行
来源：http://rqt.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ozg.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://aur.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://krt.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yfl.mhx1999.top

[Q13] 忽略重复插入
来源：http://our.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kjx.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://jan.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hpj.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tpq.xziqi.cn

[Q15] 查询全部
来源：http://gzi.cdnleiting.top

SELECT * FROM users;
来源：http://wot.andypj.xyz

[Q16] 查询指定列
来源：http://nej.xinyue.icu

SELECT id, name FROM users;
来源：http://bae.chenlongwang.top

[Q17] 条件查询
来源：http://xqb.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dqe.sufxvd.cn

[Q18] 模糊匹配
来源：http://ayb.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dra.zhiwuduotai.top

[Q19] 范围查询
来源：http://fbw.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bkt.ppjwa.cn

[Q20] IN 列表
来源：http://zxt.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ibs.tanke756.top

[Q21] 空值判断
来源：http://sfj.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gng.yueranfly.top

[Q22] 排序
来源：http://zxi.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wff.xylfe.cn

[Q23] 分页
来源：http://kub.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lhq.daria6918.cn

[Q24] 去重
来源：http://ful.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://cjo.dashuyun.cn

[Q25] 只取前 N 条
来源：http://sbf.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cma.fanxiaobao.xyz

[Q26] 计数
来源：http://exr.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://clp.0kj1m.cn

[Q27] 条件计数
来源：http://crg.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cxn.fehbvm.com

[Q28] 求和与平均
来源：http://uxf.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://opl.zhengqikj.top

[Q29] 最大最小值
来源：http://srn.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tqk.yueranfly.top

[Q30] 分组统计
来源：http://put.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szy.cdnleiting.top

[Q31] 分组后过滤
来源：http://zdx.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uck.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://qgf.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fno.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uca.tanke756.top

[Q33] 多列分组
来源：http://dhf.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oxz.birdmap.top

[Q34] 每组取第一条
来源：http://fqs.yvedp.cn

SELECT * FROM (
来源：http://rbf.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pjc.andypj.xyz

) t WHERE rn = 1;
来源：http://hgp.tianlin.xyz

[Q35] 内连接
来源：http://udz.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://joy.xylfe.cn

[Q36] 左连接
来源：http://phd.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://whl.shangyingyoupin.top

[Q37] 右连接
来源：http://jyp.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xis.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://sox.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bio.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://hxb.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://grg.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qwn.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://goc.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pam.ehwqpu.com

[Q41] 多表连接
来源：http://vym.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wse.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://ugk.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://iud.yj202588.top

[Q42] 连接条件附加过滤
来源：http://uxg.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://vgc.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wkj.ctjpmb.com

[Q43] 标量子查询
来源：http://qso.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nve.wangdashe.top

[Q44] IN 子查询
来源：http://xqa.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qsx.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://jgd.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xfc.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://kqd.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqo.jiagoushi.top

[Q47] 与平均值比较
来源：http://ncd.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://msm.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://jjh.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://byu.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://jcu.jinqigfzy.top

[Q49] 更新单行
来源：http://kue.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iny.mhx1999.top

[Q50] 批量更新
来源：http://sry.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://flw.zhoulong.xyz

[Q51] 用子查询更新
来源：http://mdt.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cod.havefunace.top

[Q52] 删除指定行
来源：http://gxf.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://lbc.xuetiantiany.cn

[Q53] 按条件删除
来源：http://hob.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ltp.uphjek.com

[Q54] 清空表
来源：http://qrh.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://gxx.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://wtq.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://paq.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://mpn.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iyr.cdnleiting.top

[Q57] 行号
来源：http://zfv.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://usf.tian-w.cn

[Q58] 累计求和
来源：http://cnp.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://esw.yonumen.top

[Q59] 分组内累计
来源：http://ear.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://stq.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://mkv.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jwn.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lnv.gzhubu.top

[Q61] 移动平均
来源：http://mul.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ler.xziqi.cn

[Q62] 分组占比
来源：http://jzp.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xrc.xylfe.cn

[Q63] 开启事务
来源：http://xtt.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://deg.yj20258.top

[Q64] 提交事务
来源：http://ijn.andypj.xyz

COMMIT;
来源：http://egg.xuetiantiany.cn

[Q65] 回滚事务
来源：http://lfe.9152youxi.cn

ROLLBACK;
来源：http://fou.sysykeji.top

[Q66] 行锁查询
来源：http://rsr.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://szk.ybcxt.top

[Q67] 设置隔离级别
来源：http://obj.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ajq.jinqigufen.top

[Q68] 保存点
来源：http://fbg.cheryme.top

SAVEPOINT sp1;
来源：http://gnv.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://zbq.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://pgu.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqo.guannengcc.top

[Q70] 更新统计信息
来源：http://pgy.fzhhl.top

ANALYZE TABLE users;
来源：http://fmc.jinqigfzy.top

[Q71] 查看建表语句
来源：http://pau.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fsc.hysaishi.cn

[Q72] 查看索引
来源：http://uzi.fengsongda.top

SHOW INDEX FROM users;
来源：http://bnr.wangshuangyany.cn

[Q73] 查看表状态
来源：http://dkw.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bhk.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://ccw.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yks.jlsjyb.cn

[Q75] 日期格式化
来源：http://xgi.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gku.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uqz.gaohongyu789.top

[Q76] 按天统计
来源：http://dsn.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ufw.jlsjyb.cn

[Q77] 时间加减
来源：http://zjv.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlx.ctjpmb.com

[Q78] 当前时间
来源：http://ahr.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mws.fktsv.cn

[Q79] 字符串拼接
来源：http://uoc.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gdd.yueranfly.top

[Q80] 字符串截取
来源：http://uxz.ydzc1.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fux.guowangkeji.top

[Q81] 字符串替换
来源：http://rln.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gkl.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://asr.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://szr.chenlongwang.top

[Q83] 大小写转换
来源：http://rvl.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uqt.nanxinkj.top

[Q84] 去除首尾空格
来源：http://ntm.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://zhe.vehdjk.com

[Q85] 数值取整
来源：http://uqp.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tuk.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://bom.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dvc.guannengcc.top

[Q87] JSON 字段做条件
来源：http://qjj.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dvj.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://xuz.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jlj.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzj.meibo888.top

[Q89] 判断表是否存在
来源：http://pnz.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qec.shuidangran.top

[Q90] 生成序号列
来源：http://bwr.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://znu.xingfuxueyuan.xyz

================================================================================
来源：http://rni.shanyushiyangtech.top

R. Bash 专题
来源：http://bvh.daria6918.cn

================================================================================
来源：http://ogc.guowangkeji.top

[R01] shebang 与严格模式
来源：http://asd.hywenlv.cn

#!/usr/bin/env bash
来源：http://fef.yueranfly.top

set -euo pipefail
来源：http://ajc.birdmap.top

[R02] 变量赋值与使用
来源：http://qkb.ehwqpu.com

name="Tom"; echo "$name"
来源：http://xij.sjlbkw.cn

[R03] 只读变量
来源：http://oqj.c1oappe.top

readonly PI=3.14
来源：http://gap.sxryk.cn

[R04] 位置参数
来源：http://bct.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xyx.jqgfzy.top

[R05] 参数默认值
来源：http://iqd.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://klx.316326.xyz

[R06] 判断命令是否存在
来源：http://dox.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iip.jiagoushi.top

[R07] if 判断文件
来源：http://bnl.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xbt.ydzc1.top

[R08] 数值比较
来源：http://iaa.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ehk.mhx1999.top

[R09] 字符串比较
来源：http://tsl.kuanghao11.cn


<!-- 参考信息 -->