代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wyy.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://wkf.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tdf.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vku.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sny.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://abm.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jis.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pqi.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyo.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bcv.zdqjudy.top

[P03] 生成短随机字符串
来源：http://krw.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dqo.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tmc.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://czo.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twv.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tdk.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ceb.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uvj.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dne.hnxiangtu.top

[P04] 求长度
来源：http://juz.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bsi.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vae.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kzn.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahr.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://lhd.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://xfh.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://ovp.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://udk.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://egz.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nzq.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://okj.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bcz.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nlq.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://twc.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://fwt.uphjek.com

Ruby: a == b
来源：http://lro.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qlh.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hao.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tia.shuidangran.top

PHP:  if (empty($x)) {}
来源：http://wgc.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kns.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://opn.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jgi.ydzc1.top

Go:   if x == nil {}
来源：http://qic.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gau.epnwcf.com

C#:   if (x is null) {}
来源：http://aiy.meibo888.top

[P07] 防抖与节流
来源：http://yzv.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vmx.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://lqc.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rta.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztw.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://srn.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kpy.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jwz.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vxs.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://xtf.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tlm.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dtp.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oau.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hla.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uup.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yka.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rjw.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pre.zhijiandao.cn

================================================================================
来源：http://bpy.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fry.zhoulong.xyz

================================================================================
来源：http://kdi.pengpengdd.cyou

[Q01] 创建表
来源：http://jgw.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://ujb.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ydz.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://sya.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://sqj.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kyp.hesvh.cn

);
来源：http://phe.tianlin.xyz

[Q02] 创建带外键的表
来源：http://qag.cdnleiting.top

CREATE TABLE orders (
来源：http://ofx.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvi.guowangkeji.top

user_id INT NOT NULL,
来源：http://ucm.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://ljo.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://atb.jinqigufen.top

);
来源：http://uiz.jinghuilouyu.cn

[Q03] 增加列
来源：http://nqc.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uon.gogol.net.cn

[Q04] 修改列类型
来源：http://kob.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nyk.zdbjq.cn

[Q05] 重命名列
来源：http://deh.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zrx.xziqi.cn

[Q06] 删除列
来源：http://rev.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lkx.jinyuanbaomall.cn

[Q07] 删除表
来源：http://lwx.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://jld.xziqi.cn

[Q08] 创建普通索引
来源：http://xyu.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://smt.gzhubu.top

[Q09] 创建唯一索引
来源：http://twb.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rxt.iojbl.cn

[Q10] 插入单行
来源：http://ofx.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fxu.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://ujw.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sgx.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://pws.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://wkv.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cwq.shzxlz.cn

[Q13] 忽略重复插入
来源：http://tdf.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://itm.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://qfm.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kgy.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tdu.hnqzz.top

[Q15] 查询全部
来源：http://opm.tanke756.top

SELECT * FROM users;
来源：http://ias.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://mph.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://gqi.hammf.cn

[Q17] 条件查询
来源：http://suh.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nmr.meibo888.top

[Q18] 模糊匹配
来源：http://nsz.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqa.ppjwa.cn

[Q19] 范围查询
来源：http://cnc.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uas.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://sdi.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://byc.snrcjt.cn

[Q21] 空值判断
来源：http://gvl.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zpp.gotoacloud.top

[Q22] 排序
来源：http://tma.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dup.vehdjk.com

[Q23] 分页
来源：http://svr.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://igk.feifeiyinyue.top

[Q24] 去重
来源：http://cvl.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://zjj.fehbvm.com

[Q25] 只取前 N 条
来源：http://hsr.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vew.sweek.top

[Q26] 计数
来源：http://tdd.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://kve.hcnkem.com

[Q27] 条件计数
来源：http://bmo.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tvb.jlsjyb.cn

[Q28] 求和与平均
来源：http://ivj.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qcw.wangdashe.top

[Q29] 最大最小值
来源：http://gfs.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iun.havefunace.top

[Q30] 分组统计
来源：http://llp.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://viq.fengsongda.top

[Q31] 分组后过滤
来源：http://otv.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ttz.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://bcp.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ssp.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rnl.ydjk.org.cn

[Q33] 多列分组
来源：http://unq.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gxn.yonumen.top

[Q34] 每组取第一条
来源：http://phc.smart0.xyz

SELECT * FROM (
来源：http://cmq.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://htm.fengsongda.top

) t WHERE rn = 1;
来源：http://rek.sweek.top

[Q35] 内连接
来源：http://rby.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ryr.zhijiandao.cn

[Q36] 左连接
来源：http://vah.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ifk.316326.xyz

[Q37] 右连接
来源：http://pqj.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uqw.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://rso.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dbr.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://ikn.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dan.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ijq.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gln.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gbi.pengpengdd.cyou

[Q41] 多表连接
来源：http://pll.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qok.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://gut.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://fqs.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://tjl.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://sfm.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://poh.zhiwuduotai.top

[Q43] 标量子查询
来源：http://clj.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jvy.fzhhl.top

[Q44] IN 子查询
来源：http://ylt.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zaa.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://wkt.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kuu.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://lsd.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afm.zdqjudy.top

[Q47] 与平均值比较
来源：http://pmb.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tpc.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://egf.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xxm.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://mlf.feifeiyinyue.top

[Q49] 更新单行
来源：http://ofw.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://drx.cdnleiting.top

[Q50] 批量更新
来源：http://zca.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ndr.yonumen.top

[Q51] 用子查询更新
来源：http://jcr.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wei.zhongyouzk.top

[Q52] 删除指定行
来源：http://ujj.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://kyt.cdnleiting.top

[Q53] 按条件删除
来源：http://lzv.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nqw.xziqi.cn

[Q54] 清空表
来源：http://ilg.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://gjd.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://ydt.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ldu.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://oll.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gew.jqgufenzy.top

[Q57] 行号
来源：http://otv.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dys.kuanghao11.cn

[Q58] 累计求和
来源：http://fii.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xdp.shangyingyoupin.top

[Q59] 分组内累计
来源：http://dig.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szb.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://tiq.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ows.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vvm.yueranfly.top

[Q61] 移动平均
来源：http://hwl.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://onp.bbcook.cn

[Q62] 分组占比
来源：http://zib.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wqm.cdnleiting.top

[Q63] 开启事务
来源：http://qgn.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kde.cashguo.top

[Q64] 提交事务
来源：http://fqx.zdqjudy.top

COMMIT;
来源：http://cex.yanxiufei.cn

[Q65] 回滚事务
来源：http://fsa.zhaomingkeji.xyz

ROLLBACK;
来源：http://uoq.bbcook.cn

[Q66] 行锁查询
来源：http://gze.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mnj.havefunace.top

[Q67] 设置隔离级别
来源：http://rhg.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sgn.birdmap.top

[Q68] 保存点
来源：http://hsq.yuxming.cn

SAVEPOINT sp1;
来源：http://gyi.jinqigufen.top

ROLLBACK TO sp1;
来源：http://dqc.gotoacloud.top

[Q69] 查看执行计划
来源：http://qki.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xfp.daria6918.cn

[Q70] 更新统计信息
来源：http://fqn.nwbrower.top

ANALYZE TABLE users;
来源：http://scd.tanke756.top

[Q71] 查看建表语句
来源：http://spl.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nls.gzhubu.top

[Q72] 查看索引
来源：http://gcc.wangdashe.top

SHOW INDEX FROM users;
来源：http://pdw.snrcjt.cn

[Q73] 查看表状态
来源：http://kyc.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mkl.xziqi.cn

[Q74] 强制使用索引
来源：http://tmc.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cbm.andypj.xyz

[Q75] 日期格式化
来源：http://qvc.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://czg.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fbk.sufxvd.cn

[Q76] 按天统计
来源：http://lwt.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cpu.yuxming.cn

[Q77] 时间加减
来源：http://cwy.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ers.vqdsnc.cn

[Q78] 当前时间
来源：http://ctm.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zvu.hesvh.cn

[Q79] 字符串拼接
来源：http://clv.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gvi.ydzc1.top

[Q80] 字符串截取
来源：http://uxe.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vaq.c1oappe.top

[Q81] 字符串替换
来源：http://cwr.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivx.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://hgd.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qxx.gzhubu.top

[Q83] 大小写转换
来源：http://jhg.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mgi.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://taq.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://gal.yanxiufei.cn

[Q85] 数值取整
来源：http://csp.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kan.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://wyb.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pwf.fzhhl.top

[Q87] JSON 字段做条件
来源：http://tsk.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oby.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://ypr.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nyx.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ngc.snrcjt.cn

[Q89] 判断表是否存在
来源：http://lqx.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bhy.dianchejie.cn

[Q90] 生成序号列
来源：http://njw.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ffv.cashguo.top

================================================================================
来源：http://row.ydjk.org.cn

R. Bash 专题
来源：http://wub.meibo888.top

================================================================================
来源：http://cnr.shzxlz.cn

[R01] shebang 与严格模式
来源：http://ssd.jiagoushi.top

#!/usr/bin/env bash
来源：http://ryg.jyoumei.cn

set -euo pipefail
来源：http://gja.zdqjudy.top

[R02] 变量赋值与使用
来源：http://ctl.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://xpt.dashuyun.cn

[R03] 只读变量
来源：http://oiy.svipenyu.cn

readonly PI=3.14
来源：http://tfp.sweek.top

[R04] 位置参数
来源：http://xsp.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://efi.sufxvd.cn

[R05] 参数默认值
来源：http://txl.zhengqikj.top

name="${1:-default}"
来源：http://dza.yonumen.top

[R06] 判断命令是否存在
来源：http://jlk.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lqw.sweek.top

[R07] if 判断文件
来源：http://fvu.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://epo.guannengcc.top

[R08] 数值比较
来源：http://hhk.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ztx.sufxvd.cn

[R09] 字符串比较
来源：http://zhs.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://asa.cashguo.top

[R10] 正则匹配
来源：http://sgy.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jnt.iojbl.cn

[R11] case 多分支
来源：http://nrh.jinghuilouyu.cn

case "$1" in
来源：http://qfa.hysaishi.cn

start) echo "启动" ;;
来源：http://pew.mhx1999.top

stop)  echo "停止" ;;
来源：http://ggf.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://hzh.nanxinkj.top


<!-- 参考信息 -->