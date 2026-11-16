代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rya.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ppb.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://slh.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ucd.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vem.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cfs.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://hvx.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kbo.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ujd.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gkh.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tao.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bvz.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gkj.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bkn.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://shq.hnqzz.top

[P04] 求长度
来源：http://det.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://inf.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jru.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xje.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dah.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://jyc.ydzc1.top

Go:   len(arr);  len(m)
来源：http://uur.hnqzz.top

Ruby: x.length;  x.size
来源：http://fll.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ikz.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://pof.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqx.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://foz.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mac.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hdg.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://brz.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://jwz.yj20258.top

Ruby: a == b
来源：http://svt.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mma.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://orx.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agb.cashguo.top

PHP:  if (empty($x)) {}
来源：http://zvh.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zjq.xuanzx.com

TS:   if (x == null) {}
来源：http://tfv.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wuf.yvedp.cn

Go:   if x == nil {}
来源：http://zxo.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ubj.epnwcf.com

C#:   if (x is null) {}
来源：http://nur.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://brg.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lpu.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://svg.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fdf.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sds.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opj.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xzh.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ypz.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cch.yj202588.top

[P08] 处理浮点精度问题
来源：http://ycj.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fvs.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://clr.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ooa.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cmq.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xof.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nsa.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pyi.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zps.jqgufenzy.top

================================================================================
来源：http://jjp.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rgd.zhixingplan.top

================================================================================
来源：http://zwo.hcnkem.com

[Q01] 创建表
来源：http://nio.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://wge.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ezk.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://uax.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://bbc.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xeo.yangfankeji.com

);
来源：http://inf.fzhhl.top

[Q02] 创建带外键的表
来源：http://ntl.wangdashe.top

CREATE TABLE orders (
来源：http://xwf.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jmi.jqgufenzy.top

user_id INT NOT NULL,
来源：http://rpv.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://lcw.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://foi.hnqzz.top

);
来源：http://azt.yangfankeji.com

[Q03] 增加列
来源：http://hit.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ahq.shangyingyoupin.top

[Q04] 修改列类型
来源：http://fgb.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mfc.yvedp.cn

[Q05] 重命名列
来源：http://rzq.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wzx.guowangkeji.top

[Q06] 删除列
来源：http://fkb.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://odu.nanxuanxn.top

[Q07] 删除表
来源：http://bju.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://chx.fengsongda.top

[Q08] 创建普通索引
来源：http://hbn.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vdf.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://tko.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zbv.sysykeji.top

[Q10] 插入单行
来源：http://kal.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pjh.vqdsnc.cn

[Q11] 一次插入多行
来源：http://zag.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nmx.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://qnl.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://oov.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fto.tanke756.top

[Q13] 忽略重复插入
来源：http://bkj.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://axj.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://dyl.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpg.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://crg.hywenlv.cn

[Q15] 查询全部
来源：http://ewd.feifeiyinyue.top

SELECT * FROM users;
来源：http://otv.316326.xyz

[Q16] 查询指定列
来源：http://ifz.yanxiufei.cn

SELECT id, name FROM users;
来源：http://xuc.nwbrower.top

[Q17] 条件查询
来源：http://czq.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ykd.snrcjt.cn

[Q18] 模糊匹配
来源：http://odp.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hqn.yonumen.top

[Q19] 范围查询
来源：http://exc.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svw.hammf.cn

[Q20] IN 列表
来源：http://qir.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lgz.yj202588.top

[Q21] 空值判断
来源：http://ior.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jsh.hysaishi.cn

[Q22] 排序
来源：http://box.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rnx.zdqjudy.top

[Q23] 分页
来源：http://myl.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oiq.aizwys.cn

[Q24] 去重
来源：http://wpi.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://hgy.ydzc1.top

[Q25] 只取前 N 条
来源：http://nsq.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://igj.jianghu66.top

[Q26] 计数
来源：http://mcb.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://zbe.zdqjudy.top

[Q27] 条件计数
来源：http://cdd.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tmx.vehdjk.com

[Q28] 求和与平均
来源：http://tut.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qna.shangyingyoupin.top

[Q29] 最大最小值
来源：http://iyw.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wnr.nanxuanxn.top

[Q30] 分组统计
来源：http://idx.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyx.yonumen.top

[Q31] 分组后过滤
来源：http://lrb.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xlo.andypj.xyz

[Q32] 分组拼接字符串
来源：http://hvu.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aij.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nac.dashuyun.cn

[Q33] 多列分组
来源：http://qfv.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tfn.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://jwx.gotoacloud.top

SELECT * FROM (
来源：http://jbg.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bhp.chenlongwang.top

) t WHERE rn = 1;
来源：http://ewp.ydzc1.top

[Q35] 内连接
来源：http://ujr.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aqg.ydzc1.top

[Q36] 左连接
来源：http://fvu.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iyy.yuxming.cn

[Q37] 右连接
来源：http://xnj.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://naw.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://vqg.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kjh.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://jgg.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://qul.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://emh.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fma.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nqq.zdbjq.cn

[Q41] 多表连接
来源：http://kij.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://trv.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://pcp.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://jdo.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://ait.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://zex.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ogm.iojbl.cn

[Q43] 标量子查询
来源：http://hca.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ajz.fengsongda.top

[Q44] IN 子查询
来源：http://tty.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://czl.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://lql.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://joq.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://bjg.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcf.c1oappe.top

[Q47] 与平均值比较
来源：http://jnv.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qwh.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://pqw.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hgw.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://kfu.vqdsnc.cn

[Q49] 更新单行
来源：http://fgl.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nhc.c1oappe.top

[Q50] 批量更新
来源：http://ysu.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aoi.tianlin.xyz

[Q51] 用子查询更新
来源：http://eku.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ijg.yj20258888.top

[Q52] 删除指定行
来源：http://zvy.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://tcv.sxryk.cn

[Q53] 按条件删除
来源：http://ddc.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eho.haohaochexian.top

[Q54] 清空表
来源：http://dpc.bbcook.cn

TRUNCATE TABLE logs;
来源：http://rjv.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://lgy.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yit.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://uip.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yft.nanxinkj.top

[Q57] 行号
来源：http://zqc.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ual.cdnleiting.top

[Q58] 累计求和
来源：http://lom.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rwe.yuanzhike.top

[Q59] 分组内累计
来源：http://jcs.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wun.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://gmo.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gbk.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qxr.wangshuangyany.cn

[Q61] 移动平均
来源：http://zdd.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oad.yanxiufei.cn

[Q62] 分组占比
来源：http://idf.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nrq.gogol.net.cn

[Q63] 开启事务
来源：http://abl.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rva.gzhubu.top

[Q64] 提交事务
来源：http://bwk.shangyingyoupin.top

COMMIT;
来源：http://eil.hcnkem.com

[Q65] 回滚事务
来源：http://mfz.316326.xyz

ROLLBACK;
来源：http://yfr.hfpthk.cn

[Q66] 行锁查询
来源：http://yvk.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://smp.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://ikm.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cqq.guowangkeji.top

[Q68] 保存点
来源：http://jos.jqgfzy.top

SAVEPOINT sp1;
来源：http://jso.snrcjt.cn

ROLLBACK TO sp1;
来源：http://nxa.jlsjyb.cn

[Q69] 查看执行计划
来源：http://czw.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rrs.gaohongyu789.top

[Q70] 更新统计信息
来源：http://rsn.yuanzhike.top

ANALYZE TABLE users;
来源：http://rqf.jqgufenzy.top

[Q71] 查看建表语句
来源：http://skj.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwx.kuanghao11.cn

[Q72] 查看索引
来源：http://fjo.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://neg.sufxvd.cn

[Q73] 查看表状态
来源：http://mdp.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://skv.52xcode.cn

[Q74] 强制使用索引
来源：http://rfp.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ywc.xinyue.icu

[Q75] 日期格式化
来源：http://gai.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyk.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ifj.gaohongyu789.top

[Q76] 按天统计
来源：http://pya.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upj.tian-w.cn

[Q77] 时间加减
来源：http://rtl.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tap.gogol.net.cn

[Q78] 当前时间
来源：http://hbi.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxi.chenzaomai.com

[Q79] 字符串拼接
来源：http://rqg.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://btx.sjlbkw.cn

[Q80] 字符串截取
来源：http://mdv.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bgw.tian-w.cn

[Q81] 字符串替换
来源：http://rpy.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zwl.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://tuv.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tht.c1oappe.top

[Q83] 大小写转换
来源：http://pfz.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qwf.pycfn.com

[Q84] 去除首尾空格
来源：http://etz.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://kfa.hammf.cn

[Q85] 数值取整
来源：http://eda.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://idx.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://wgg.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kzj.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://jvx.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xfe.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://gir.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cuk.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qgk.fehbvm.com

[Q89] 判断表是否存在
来源：http://ney.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xlv.xuanzx.com

[Q90] 生成序号列
来源：http://jxz.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yhf.chenjidiqi.icu

================================================================================
来源：http://cwu.bbcook.cn

R. Bash 专题
来源：http://vvh.xylfe.cn

================================================================================
来源：http://hnf.redwolf501.top

[R01] shebang 与严格模式
来源：http://byc.shzxlz.cn

#!/usr/bin/env bash
来源：http://uvp.bbcook.cn

set -euo pipefail
来源：http://zbw.shuidangran.top

[R02] 变量赋值与使用
来源：http://rjz.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://bou.wangdashe.top

[R03] 只读变量
来源：http://duf.zhaomingkeji.xyz

readonly PI=3.14
来源：http://bck.sxryk.cn

[R04] 位置参数
来源：http://vxl.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bix.ydjk.org.cn

[R05] 参数默认值
来源：http://yqr.chenjidiqi.icu

name="${1:-default}"
来源：http://gsl.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://two.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hag.daxiang520.top

[R07] if 判断文件
来源：http://opu.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xpq.redwolf501.top

[R08] 数值比较
来源：http://etu.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bxa.316326.xyz

[R09] 字符串比较
来源：http://git.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wvd.fktsv.cn

[R10] 正则匹配
来源：http://kiw.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://npw.haohaochexian.top

[R11] case 多分支
来源：http://ncw.xingfuxueyuan.xyz

case "$1" in
来源：http://ikd.yuxming.cn

start) echo "启动" ;;
来源：http://xni.cashguo.top

stop)  echo "停止" ;;
来源：http://boo.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://fiz.yfazqb.com

esac
来源：http://ttn.smart0.xyz

[R12] for 遍历文件
来源：http://gdt.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://jor.haohaochexian.top

[R13] for 计数循环
来源：http://wyi.ywan-chungtsiang.top


<!-- 参考信息 -->