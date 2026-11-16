代发 wailian999

C#:   Parallel.For
来源：http://mer.daria6918.cn

================================================================================
来源：http://nbs.ydzc1.top

P. 常用工具函数
来源：http://wxv.c1oappe.top

================================================================================
来源：http://vxl.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://chm.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://tlu.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://odo.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://iwt.shuidangran.top

TS:   crypto.randomUUID()
来源：http://tsy.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://rva.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://vid.sweek.top

Ruby: SecureRandom.uuid
来源：http://jvm.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://jhu.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://pjj.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lls.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzw.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bvz.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pkr.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vsh.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vww.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mrq.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mpb.andypj.xyz

[P03] 生成短随机字符串
来源：http://cva.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mjp.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zzo.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khx.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://atj.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://whu.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://flw.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vcm.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ekn.fehbvm.com

[P04] 求长度
来源：http://wdi.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ams.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyl.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhw.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exy.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://vka.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://xyj.ybcxt.top

Ruby: x.length;  x.size
来源：http://yfg.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vmd.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://sdq.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://yjg.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oap.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osk.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jow.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lfm.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://zlz.tanke756.top

Ruby: a == b
来源：http://sli.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jxp.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xqx.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://moq.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://ksr.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uwi.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://ntp.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rda.gogol.net.cn

Go:   if x == nil {}
来源：http://atp.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mym.iojbl.cn

C#:   if (x is null) {}
来源：http://tjt.kuanghao11.cn

[P07] 防抖与节流
来源：http://uwp.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rgo.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://eiy.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bng.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vyj.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qqf.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tfs.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qzb.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ehf.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://cjs.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dvl.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sig.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://smm.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iol.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://txx.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hvl.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xxh.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xzd.hywenlv.cn

================================================================================
来源：http://ayw.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xlv.chenzaomai.com

================================================================================
来源：http://pih.nanxinkj.top

[Q01] 创建表
来源：http://vsj.andypj.xyz

CREATE TABLE users (
来源：http://ono.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wji.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://qtg.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://wey.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hts.chenzaomai.com

);
来源：http://emq.daria6918.cn

[Q02] 创建带外键的表
来源：http://mml.jlsjyb.cn

CREATE TABLE orders (
来源：http://guz.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qzz.uphjek.com

user_id INT NOT NULL,
来源：http://sci.bjfxy.top

amount DECIMAL(10, 2),
来源：http://vfj.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kyy.shanyushiyangtech.top

);
来源：http://hlk.yj20258888.top

[Q03] 增加列
来源：http://bpm.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyg.sxryk.cn

[Q04] 修改列类型
来源：http://axj.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mtt.sufxvd.cn

[Q05] 重命名列
来源：http://qwt.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pay.fktsv.cn

[Q06] 删除列
来源：http://hdo.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://vmz.kuanghao11.cn

[Q07] 删除表
来源：http://aur.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://rhr.xuanzx.com

[Q08] 创建普通索引
来源：http://omb.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://odv.haohaochexian.top

[Q09] 创建唯一索引
来源：http://upl.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cyg.pengpengdd.cyou

[Q10] 插入单行
来源：http://axd.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aha.jqgufenzy.top

[Q11] 一次插入多行
来源：http://phk.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ulm.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://ann.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://uox.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vlv.gzhubu.top

[Q13] 忽略重复插入
来源：http://hyw.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jsn.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://gbh.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vpl.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ubx.zhixingplan.top

[Q15] 查询全部
来源：http://ulz.yuanzhike.top

SELECT * FROM users;
来源：http://jas.316326.xyz

[Q16] 查询指定列
来源：http://gfd.zhoulong.xyz

SELECT id, name FROM users;
来源：http://age.fengsongda.top

[Q17] 条件查询
来源：http://pkg.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://spa.hfpthk.cn

[Q18] 模糊匹配
来源：http://ozt.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://irb.haohaochexian.top

[Q19] 范围查询
来源：http://cau.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lds.zdbjq.cn

[Q20] IN 列表
来源：http://yqv.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tnc.jinghuilouyu.cn

[Q21] 空值判断
来源：http://glt.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tbb.chenlongwang.top

[Q22] 排序
来源：http://oyy.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uir.yj20258.top

[Q23] 分页
来源：http://jfm.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pmt.zhixingplan.top

[Q24] 去重
来源：http://xtl.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://eom.9152youxi.cn

[Q25] 只取前 N 条
来源：http://tvp.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bei.ybcxt.top

[Q26] 计数
来源：http://dbd.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://ane.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://aes.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tvn.sweek.top

[Q28] 求和与平均
来源：http://owx.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://agz.birdmap.top

[Q29] 最大最小值
来源：http://qre.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dqn.yangfankeji.com

[Q30] 分组统计
来源：http://nxi.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qzc.zhijiandao.cn

[Q31] 分组后过滤
来源：http://dzl.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzk.c1oappe.top

[Q32] 分组拼接字符串
来源：http://vml.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wyr.vehdjk.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wtg.dianchejie.cn

[Q33] 多列分组
来源：http://cwo.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ilp.tarul.cn

[Q34] 每组取第一条
来源：http://wkx.xuanzx.com

SELECT * FROM (
来源：http://ero.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cau.bbcook.cn

) t WHERE rn = 1;
来源：http://mmw.0kj1m.cn

[Q35] 内连接
来源：http://xum.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://are.shangyingyoupin.top

[Q36] 左连接
来源：http://kqv.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ked.shzxlz.cn

[Q37] 右连接
来源：http://kqx.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ffs.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uhh.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://juh.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://zod.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://als.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tks.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://nie.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sge.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://sgd.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ccg.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://war.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://buw.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://yom.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://igm.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://frt.fengsongda.top

[Q43] 标量子查询
来源：http://dco.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://frj.hammf.cn

[Q44] IN 子查询
来源：http://ifn.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fyn.birdmap.top

[Q45] EXISTS 判断存在
来源：http://mfl.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bze.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://sht.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mxs.bbcook.cn

[Q47] 与平均值比较
来源：http://jxk.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://djz.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://ffk.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://szb.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://rul.pengpengdd.cyou

[Q49] 更新单行
来源：http://hli.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cjx.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://gwq.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ufc.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://uia.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tzv.jinqigfzy.top

[Q52] 删除指定行
来源：http://zkk.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://trd.ppjwa.cn

[Q53] 按条件删除
来源：http://xrj.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hmw.zycfv.cn

[Q54] 清空表
来源：http://lrn.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://nmh.yfazqb.com

[Q55] 排名（并列占位）
来源：http://pku.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aay.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://mff.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aew.yj202588.top

[Q57] 行号
来源：http://jim.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxa.smart0.xyz

[Q58] 累计求和
来源：http://wln.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dog.ctjpmb.com

[Q59] 分组内累计
来源：http://fgk.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqw.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://hhm.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kob.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xyo.guannengcc.top

[Q61] 移动平均
来源：http://wco.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pkk.shanyushiyangtech.top

[Q62] 分组占比
来源：http://kzd.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://unp.zycfv.cn

[Q63] 开启事务
来源：http://hwq.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://snu.quarkkingdee.top

[Q64] 提交事务
来源：http://vvv.hfpthk.cn

COMMIT;
来源：http://wad.aizwys.cn

[Q65] 回滚事务
来源：http://gig.sweek.top

ROLLBACK;
来源：http://dwm.gzhubu.top

[Q66] 行锁查询
来源：http://vmb.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ljt.andypj.xyz

[Q67] 设置隔离级别
来源：http://opg.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uaa.ywan-chungtsiang.top

[Q68] 保存点
来源：http://xah.0kj1m.cn

SAVEPOINT sp1;
来源：http://lty.52xcode.cn

ROLLBACK TO sp1;
来源：http://hhf.tanke756.top

[Q69] 查看执行计划
来源：http://ent.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ysf.cucudq.cn

[Q70] 更新统计信息
来源：http://hyn.zhijiandao.cn

ANALYZE TABLE users;
来源：http://anc.ehwqpu.com

[Q71] 查看建表语句
来源：http://utf.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rkw.fehbvm.com

[Q72] 查看索引
来源：http://cuz.tanke756.top

SHOW INDEX FROM users;
来源：http://mqp.jiagoushi.top

[Q73] 查看表状态
来源：http://ltl.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jsn.tanke756.top

[Q74] 强制使用索引
来源：http://ftg.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rea.quarkkingdee.top

[Q75] 日期格式化
来源：http://dld.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ynl.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ijx.birdmap.top

[Q76] 按天统计
来源：http://swg.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qgc.daxiang520.top

[Q77] 时间加减
来源：http://ede.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://anp.iojbl.cn

[Q78] 当前时间
来源：http://mow.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfy.sufxvd.cn

[Q79] 字符串拼接
来源：http://yhv.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oxt.epnwcf.com

[Q80] 字符串截取
来源：http://bsn.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ufr.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://gxk.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gyd.pycfn.com

[Q82] 字符长度与字节长度
来源：http://ukm.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://awz.yangfankeji.com

[Q83] 大小写转换
来源：http://aeo.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jad.birdmap.top

[Q84] 去除首尾空格
来源：http://zum.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://nza.redwolf501.top

[Q85] 数值取整
来源：http://dec.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://whd.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://azn.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cxu.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://gbo.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://suy.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://uti.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wet.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pma.zycfv.cn

[Q89] 判断表是否存在
来源：http://eoh.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fbu.sweek.top

[Q90] 生成序号列
来源：http://xkr.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lrt.yonumen.top

================================================================================
来源：http://tin.xingfuxueyuan.xyz

R. Bash 专题
来源：http://sxl.fktsv.cn

================================================================================
来源：http://gtd.chenlongwang.top

[R01] shebang 与严格模式
来源：http://vop.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://qdu.gzhubu.top

set -euo pipefail
来源：http://srn.fengsongda.top

[R02] 变量赋值与使用
来源：http://uhg.wangdashe.top

name="Tom"; echo "$name"
来源：http://onu.ydzc1.top

[R03] 只读变量
来源：http://ekm.sweek.top

readonly PI=3.14
来源：http://aiy.guowangkeji.top

[R04] 位置参数
来源：http://kkc.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tes.xylfe.cn

[R05] 参数默认值
来源：http://brm.epnwcf.com

name="${1:-default}"
来源：http://hjm.daxiang520.top

[R06] 判断命令是否存在
来源：http://zco.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rfu.nanxuanxn.top

[R07] if 判断文件
来源：http://dxw.xinyue.icu


<!-- 参考信息 -->