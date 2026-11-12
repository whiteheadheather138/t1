代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://pzz.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://ylz.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ehq.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://kys.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pow.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://irx.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vde.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lwv.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cqr.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwb.yj20258.top

[P03] 生成短随机字符串
来源：http://hpc.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://odn.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://heo.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfv.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://paw.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nbr.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xcx.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qhp.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://juw.zhoulong.xyz

[P04] 求长度
来源：http://dic.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hyc.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ufd.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zlv.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dva.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://did.shuidangran.top

Go:   len(arr);  len(m)
来源：http://aek.gotoacloud.top

Ruby: x.length;  x.size
来源：http://jfa.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://prf.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://jdb.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://vft.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hvv.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eah.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exx.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qil.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://zdw.pycfn.com

Ruby: a == b
来源：http://xkr.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nhe.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://flj.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oib.hammf.cn

PHP:  if (empty($x)) {}
来源：http://olx.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://afc.jinqigufen.top

TS:   if (x == null) {}
来源：http://tcy.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uby.dashuyun.cn

Go:   if x == nil {}
来源：http://nti.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bsk.haohaochexian.top

C#:   if (x is null) {}
来源：http://hjo.iojbl.cn

[P07] 防抖与节流
来源：http://wjh.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvt.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://kba.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zut.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yiw.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nhx.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lty.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rwm.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kof.aizwys.cn

[P08] 处理浮点精度问题
来源：http://fqk.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rzw.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://loh.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dlb.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://avs.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bos.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zvm.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://olr.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lxs.zhixingplan.top

================================================================================
来源：http://vmp.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://owx.feifeiyinyue.top

================================================================================
来源：http://uiv.chenlongwang.top

[Q01] 创建表
来源：http://ged.chenlongwang.top

CREATE TABLE users (
来源：http://glw.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://trk.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://ikn.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://kif.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gps.daria6918.cn

);
来源：http://wmc.sxryk.cn

[Q02] 创建带外键的表
来源：http://fqe.zycfv.cn

CREATE TABLE orders (
来源：http://rpn.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qev.shuidangran.top

user_id INT NOT NULL,
来源：http://ygh.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://jca.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uup.birdmap.top

);
来源：http://zxv.hammf.cn

[Q03] 增加列
来源：http://ail.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://apy.jinqigfzy.top

[Q04] 修改列类型
来源：http://pzw.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mbr.sxryk.cn

[Q05] 重命名列
来源：http://xox.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rdi.jinyuanbaomall.cn

[Q06] 删除列
来源：http://cii.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://ohg.shanyushiyangtech.top

[Q07] 删除表
来源：http://czg.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://cjw.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://qty.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rka.tian-w.cn

[Q09] 创建唯一索引
来源：http://qqc.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bdl.guannengcc.top

[Q10] 插入单行
来源：http://blx.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sch.xylfe.cn

[Q11] 一次插入多行
来源：http://hmj.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cta.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://ysm.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://mrz.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qsl.ehwqpu.com

[Q13] 忽略重复插入
来源：http://boa.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vva.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://onm.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xxh.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hfj.fehbvm.com

[Q15] 查询全部
来源：http://yck.yanxiufei.cn

SELECT * FROM users;
来源：http://wwy.yfazqb.com

[Q16] 查询指定列
来源：http://wpm.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://ixd.gotoacloud.top

[Q17] 条件查询
来源：http://rrk.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ohz.yj202588.top

[Q18] 模糊匹配
来源：http://top.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mfq.wangshuangyany.cn

[Q19] 范围查询
来源：http://byo.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://obs.sysykeji.top

[Q20] IN 列表
来源：http://rcv.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://omf.dianchejie.cn

[Q21] 空值判断
来源：http://goc.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cri.hnxiangtu.top

[Q22] 排序
来源：http://byb.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ywi.yongpay.top

[Q23] 分页
来源：http://tbe.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kgr.0kj1m.cn

[Q24] 去重
来源：http://wzc.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://nzy.epnwcf.com

[Q25] 只取前 N 条
来源：http://vth.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vzb.cucudq.cn

[Q26] 计数
来源：http://rfh.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://njq.yfazqb.com

[Q27] 条件计数
来源：http://eyj.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ubt.jqgufenzy.top

[Q28] 求和与平均
来源：http://req.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ncg.hammf.cn

[Q29] 最大最小值
来源：http://nlj.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hvy.hammf.cn

[Q30] 分组统计
来源：http://deg.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fdl.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://ctz.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mof.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://twn.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xyy.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ity.fanxiaobao.xyz

[Q33] 多列分组
来源：http://ilb.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rcu.ctjpmb.com

[Q34] 每组取第一条
来源：http://ngx.9152youxi.cn

SELECT * FROM (
来源：http://ozl.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ivn.yonumen.top

) t WHERE rn = 1;
来源：http://okp.xuetiantiany.cn

[Q35] 内连接
来源：http://dkg.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ehp.gotoacloud.top

[Q36] 左连接
来源：http://fli.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ovs.wangdashe.top

[Q37] 右连接
来源：http://dcw.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qxz.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fgp.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opb.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://mmx.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eaf.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rgu.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://djs.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nlp.mhx1999.top

[Q41] 多表连接
来源：http://tvf.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ugc.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://beu.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://vbo.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://rzw.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://tgh.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zdy.fktsv.cn

[Q43] 标量子查询
来源：http://asp.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hlv.andypj.xyz

[Q44] IN 子查询
来源：http://btb.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uol.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://ymv.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttf.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://ubu.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ofv.hnxiangtu.top

[Q47] 与平均值比较
来源：http://eky.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kyp.havefunace.top

[Q48] CTE 公用表表达式
来源：http://oua.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oxa.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://frj.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://lda.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://agh.guannengcc.top

[Q50] 批量更新
来源：http://xnu.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dhy.tarul.cn

[Q51] 用子查询更新
来源：http://vml.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ldr.sjlbkw.cn

[Q52] 删除指定行
来源：http://lwa.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://hqn.shuidangran.top

[Q53] 按条件删除
来源：http://fic.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yai.xziqi.cn

[Q54] 清空表
来源：http://vbt.yongpay.top

TRUNCATE TABLE logs;
来源：http://vrr.cucudq.cn

[Q55] 排名（并列占位）
来源：http://wxd.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://grz.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://psf.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oey.tarul.cn

[Q57] 行号
来源：http://knx.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://njq.aibaodan.cn

[Q58] 累计求和
来源：http://bis.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bxo.yueranfly.top

[Q59] 分组内累计
来源：http://dad.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://svx.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://jmy.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxn.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dcs.xuetiantiany.cn

[Q61] 移动平均
来源：http://moz.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qtp.cqqwz.cn

[Q62] 分组占比
来源：http://mht.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://law.yfazqb.com

[Q63] 开启事务
来源：http://zon.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dgt.52xcode.cn

[Q64] 提交事务
来源：http://pgh.quarkkingdee.top

COMMIT;
来源：http://ibw.9152youxi.cn

[Q65] 回滚事务
来源：http://yfr.xinyue.icu

ROLLBACK;
来源：http://mrm.meibo888.top

[Q66] 行锁查询
来源：http://ure.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sxa.cucudq.cn

[Q67] 设置隔离级别
来源：http://iol.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgh.gogol.net.cn

[Q68] 保存点
来源：http://xyj.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://dbq.guannengcc.top

ROLLBACK TO sp1;
来源：http://exd.0kj1m.cn

[Q69] 查看执行计划
来源：http://qzh.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qqz.316326.xyz

[Q70] 更新统计信息
来源：http://cow.jqgfzy.top

ANALYZE TABLE users;
来源：http://lde.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://olz.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://okf.gotoacloud.top

[Q72] 查看索引
来源：http://bsj.hammf.cn

SHOW INDEX FROM users;
来源：http://rln.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://sor.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fxq.xziqi.cn

[Q74] 强制使用索引
来源：http://tpi.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cav.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://fru.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fdn.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mye.xinyue.icu

[Q76] 按天统计
来源：http://zzw.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dfk.sysykeji.top

[Q77] 时间加减
来源：http://szi.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://url.iojbl.cn

[Q78] 当前时间
来源：http://blq.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nmz.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://kwp.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zrx.316326.xyz

[Q80] 字符串截取
来源：http://ibq.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://crs.ydzc1.top

[Q81] 字符串替换
来源：http://gjz.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wxi.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://hfo.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://thz.ehwqpu.com

[Q83] 大小写转换
来源：http://eoa.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://anb.fengsongda.top

[Q84] 去除首尾空格
来源：http://tjj.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://buy.zhongyouzk.top

[Q85] 数值取整
来源：http://fop.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://esl.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://bna.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lyy.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://ygo.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pdg.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://ndb.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ieg.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pkr.yj202588.top

[Q89] 判断表是否存在
来源：http://afy.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvw.zhiwuduotai.top

[Q90] 生成序号列
来源：http://kku.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yzm.hysaishi.cn

================================================================================
来源：http://oqt.birdmap.top

R. Bash 专题
来源：http://cbx.daxiang520.top

================================================================================
来源：http://uym.sufxvd.cn

[R01] shebang 与严格模式
来源：http://jmv.epnwcf.com

#!/usr/bin/env bash
来源：http://zxg.xziqi.cn

set -euo pipefail
来源：http://gce.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://izg.daria6918.cn

name="Tom"; echo "$name"
来源：http://tlz.zdbjq.cn

[R03] 只读变量
来源：http://gjw.jinghuilouyu.cn

readonly PI=3.14
来源：http://xqk.yj20258888.top

[R04] 位置参数
来源：http://mjo.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tiv.bjfxy.top

[R05] 参数默认值
来源：http://gap.hysaishi.cn

name="${1:-default}"
来源：http://fmk.fzhhl.top

[R06] 判断命令是否存在
来源：http://ymf.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ofq.tarul.cn

[R07] if 判断文件
来源：http://yxi.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wuw.smart0.xyz

[R08] 数值比较
来源：http://ryq.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://pzr.sxryk.cn

[R09] 字符串比较
来源：http://bcc.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vpx.guannengcc.top

[R10] 正则匹配
来源：http://mis.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://atc.gaohongyu789.top

[R11] case 多分支
来源：http://saz.fktsv.cn

case "$1" in
来源：http://hct.tarul.cn

start) echo "启动" ;;
来源：http://cwb.uphjek.com

stop)  echo "停止" ;;
来源：http://ytt.birdmap.top

*)     echo "未知命令" ;;
来源：http://ofr.pengpengdd.cyou


<!-- 参考信息 -->