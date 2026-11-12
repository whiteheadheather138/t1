代发 wailian999

C#:   Parallel.For
来源：http://gyd.andypj.xyz

================================================================================
来源：http://upi.fktsv.cn

P. 常用工具函数
来源：http://cfr.redwolf501.top

================================================================================
来源：http://gpj.yfazqb.com

[P01] 生成 UUID
来源：http://mea.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://agp.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wvx.bbcook.cn

JS:   crypto.randomUUID()
来源：http://ufz.xinyue.icu

TS:   crypto.randomUUID()
来源：http://efa.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://kph.jianghu66.top

Go:   // 用 github.com/google/uuid
来源：http://yul.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://bhe.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://zgg.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://cyi.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fby.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yqj.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xxc.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mei.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uxb.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xnf.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upo.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uld.jinqigufen.top

[P03] 生成短随机字符串
来源：http://fqq.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jjp.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fly.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsa.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ntk.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gqp.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dph.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aqr.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qpi.chenlongwang.top

[P04] 求长度
来源：http://qby.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwx.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ebh.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jcp.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bei.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://nro.yueranfly.top

Go:   len(arr);  len(m)
来源：http://xjd.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://mpr.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ulq.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://wkp.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fef.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vzk.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://juj.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ysr.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zvl.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://xip.chenzaomai.com

Ruby: a == b
来源：http://maq.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iud.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zqh.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tgq.meibo888.top

PHP:  if (empty($x)) {}
来源：http://avl.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rks.sxryk.cn

TS:   if (x == null) {}
来源：http://jis.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lrk.chenjidiqi.icu

Go:   if x == nil {}
来源：http://zhy.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kqd.chenzaomai.com

C#:   if (x is null) {}
来源：http://qxt.xuanzx.com

[P07] 防抖与节流
来源：http://tnp.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nky.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://mme.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sap.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qmt.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uyd.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bpt.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fmg.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://svg.sxryk.cn

[P08] 处理浮点精度问题
来源：http://xkm.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://thr.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uks.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ass.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://err.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://enh.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uhb.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gtz.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ikg.andypj.xyz

================================================================================
来源：http://gru.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wzt.guannengcc.top

================================================================================
来源：http://vpt.hfpthk.cn

[Q01] 创建表
来源：http://ltx.cashguo.top

CREATE TABLE users (
来源：http://phh.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tbs.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://cxb.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://pgc.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://plf.yj20258888.top

);
来源：http://pvs.ydzc1.top

[Q02] 创建带外键的表
来源：http://oal.tarul.cn

CREATE TABLE orders (
来源：http://hgy.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yzk.epnwcf.com

user_id INT NOT NULL,
来源：http://nrq.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://bgb.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://spf.fanxiaobao.xyz

);
来源：http://zuh.aibaodan.cn

[Q03] 增加列
来源：http://jcz.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://brx.cheryme.top

[Q04] 修改列类型
来源：http://ybx.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fll.chenzaomai.com

[Q05] 重命名列
来源：http://vpf.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uzl.zdbjq.cn

[Q06] 删除列
来源：http://zwe.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://zcu.aibaodan.cn

[Q07] 删除表
来源：http://jfl.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://cbp.hysaishi.cn

[Q08] 创建普通索引
来源：http://lnx.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xpp.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://edr.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uxk.9152youxi.cn

[Q10] 插入单行
来源：http://igg.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yjm.jqgufenzy.top

[Q11] 一次插入多行
来源：http://flt.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cea.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://tqu.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://pev.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nmf.yj20258888.top

[Q13] 忽略重复插入
来源：http://ukx.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vpj.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://aur.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://khb.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://phy.ydzc1.top

[Q15] 查询全部
来源：http://lvr.316326.xyz

SELECT * FROM users;
来源：http://esx.ehwqpu.com

[Q16] 查询指定列
来源：http://aag.hesvh.cn

SELECT id, name FROM users;
来源：http://hkw.pycfn.com

[Q17] 条件查询
来源：http://cdd.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tsp.ydjk.org.cn

[Q18] 模糊匹配
来源：http://vuz.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqg.yongpay.top

[Q19] 范围查询
来源：http://ggs.shangyingyoupin.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ewj.zhixingplan.top

[Q20] IN 列表
来源：http://iyk.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bze.ppjwa.cn

[Q21] 空值判断
来源：http://zku.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dnu.havefunace.top

[Q22] 排序
来源：http://bud.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://umw.feifeiyinyue.top

[Q23] 分页
来源：http://sqh.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hgn.jlsjyb.cn

[Q24] 去重
来源：http://waa.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://aln.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://tuu.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rrk.jinqigufen.top

[Q26] 计数
来源：http://nwq.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://hii.chenjidiqi.icu

[Q27] 条件计数
来源：http://ipw.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ixt.hongshengwenyu.top

[Q28] 求和与平均
来源：http://brz.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iox.c1oappe.top

[Q29] 最大最小值
来源：http://utk.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://syp.cdnleiting.top

[Q30] 分组统计
来源：http://lmj.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eyd.jiagoushi.top

[Q31] 分组后过滤
来源：http://dvr.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gdj.ydzc1.top

[Q32] 分组拼接字符串
来源：http://stz.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hhl.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pcq.cheryme.top

[Q33] 多列分组
来源：http://ssi.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://suw.zhongyouzk.top

[Q34] 每组取第一条
来源：http://afn.sweek.top

SELECT * FROM (
来源：http://esu.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lhz.aibaodan.cn

) t WHERE rn = 1;
来源：http://jth.tianlin.xyz

[Q35] 内连接
来源：http://ydf.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vva.hongshengwenyu.top

[Q36] 左连接
来源：http://aen.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lvr.yangfankeji.com

[Q37] 右连接
来源：http://ztc.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fru.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tup.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jnt.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://pxa.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jlr.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rvb.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oep.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://drm.52xcode.cn

[Q41] 多表连接
来源：http://wtc.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rmg.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://qfz.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://gwr.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://apo.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://jsc.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cem.aibaodan.cn

[Q43] 标量子查询
来源：http://bip.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gll.aibaodan.cn

[Q44] IN 子查询
来源：http://hkt.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dbz.yj202588.top

[Q45] EXISTS 判断存在
来源：http://zzj.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rnm.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://lue.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jkz.tianlin.xyz

[Q47] 与平均值比较
来源：http://qtz.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mxz.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://zyo.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://odc.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://amh.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://cia.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rvc.bjfxy.top

[Q50] 批量更新
来源：http://ptn.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fqq.aizwys.cn

[Q51] 用子查询更新
来源：http://fgh.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wvc.guannengcc.top

[Q52] 删除指定行
来源：http://yqc.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://geh.zhengqikj.top

[Q53] 按条件删除
来源：http://ayg.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qls.epnwcf.com

[Q54] 清空表
来源：http://tfn.yj20258.top

TRUNCATE TABLE logs;
来源：http://hfu.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://cuw.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uxb.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://wmx.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zma.smart0.xyz

[Q57] 行号
来源：http://cod.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hak.hesvh.cn

[Q58] 累计求和
来源：http://gsf.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixd.yj20258.top

[Q59] 分组内累计
来源：http://fpr.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgi.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://mid.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bex.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bck.hesvh.cn

[Q61] 移动平均
来源：http://lcq.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://arc.yuxming.cn

[Q62] 分组占比
来源：http://rhb.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zie.nanxinkj.top

[Q63] 开启事务
来源：http://cfy.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://geg.xinyue.icu

[Q64] 提交事务
来源：http://wcs.tanke756.top

COMMIT;
来源：http://uya.hnqzz.top

[Q65] 回滚事务
来源：http://kel.andypj.xyz

ROLLBACK;
来源：http://ket.xuetiantiany.cn

[Q66] 行锁查询
来源：http://xet.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yes.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://srt.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ibw.haohaochexian.top

[Q68] 保存点
来源：http://yzx.chenlongwang.top

SAVEPOINT sp1;
来源：http://geb.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://aos.svipenyu.cn

[Q69] 查看执行计划
来源：http://osg.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ovr.xylfe.cn

[Q70] 更新统计信息
来源：http://poy.yonumen.top

ANALYZE TABLE users;
来源：http://rso.cheryme.top

[Q71] 查看建表语句
来源：http://nzr.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aiy.tarul.cn

[Q72] 查看索引
来源：http://uir.aibaodan.cn

SHOW INDEX FROM users;
来源：http://fpl.mhx1999.top

[Q73] 查看表状态
来源：http://efe.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ehz.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://hib.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qla.jqgfzy.top

[Q75] 日期格式化
来源：http://nzr.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://htz.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fcz.52xcode.cn

[Q76] 按天统计
来源：http://lzo.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pin.chenzaomai.com

[Q77] 时间加减
来源：http://npo.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xnc.quarkkingdee.top

[Q78] 当前时间
来源：http://twk.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://joo.mhx1999.top

[Q79] 字符串拼接
来源：http://tmp.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qcs.pengpengdd.cyou

[Q80] 字符串截取
来源：http://ihb.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lsh.yangfankeji.com

[Q81] 字符串替换
来源：http://hig.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://exg.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://bcq.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bzh.316326.xyz

[Q83] 大小写转换
来源：http://iah.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lio.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://ddu.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://uha.hnqzz.top

[Q85] 数值取整
来源：http://rlu.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dhn.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://jxm.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eza.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://ufr.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ndd.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://dur.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ocj.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxc.jinqigufen.top

[Q89] 判断表是否存在
来源：http://xps.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hji.xziqi.cn

[Q90] 生成序号列
来源：http://wxj.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://npc.gaohongyu789.top

================================================================================
来源：http://tup.yangfankeji.com

R. Bash 专题
来源：http://yoh.redwolf501.top

================================================================================
来源：http://ket.xinyue.icu

[R01] shebang 与严格模式
来源：http://xpi.haohaochexian.top

#!/usr/bin/env bash
来源：http://met.chenzaomai.com

set -euo pipefail
来源：http://urv.havefunace.top

[R02] 变量赋值与使用
来源：http://lcx.zdqjudy.top

name="Tom"; echo "$name"
来源：http://xtl.zhengqikj.top

[R03] 只读变量
来源：http://gwc.hammf.cn

readonly PI=3.14
来源：http://yjw.kuanghao11.cn

[R04] 位置参数
来源：http://ucd.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kwo.yonumen.top

[R05] 参数默认值
来源：http://ogg.yonumen.top

name="${1:-default}"
来源：http://rwx.chenzaomai.com

[R06] 判断命令是否存在
来源：http://usn.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jcn.tanke756.top

[R07] if 判断文件
来源：http://lzp.yuanzhike.top


<!-- 参考信息 -->