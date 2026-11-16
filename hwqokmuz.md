代发 wailian999

[P01] 生成 UUID
来源：http://thq.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://qlo.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wsy.xziqi.cn

JS:   crypto.randomUUID()
来源：http://sgo.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://ppt.sweek.top

Java: UUID.randomUUID().toString()
来源：http://dod.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://svx.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://qgw.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://ipq.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://jex.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ulb.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fvm.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ekl.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ttp.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gii.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xyw.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhf.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hlj.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://qea.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ogs.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qiu.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zlv.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uts.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xrp.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zhb.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://efs.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dyc.sjlbkw.cn

[P04] 求长度
来源：http://zgv.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tuf.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://znf.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zve.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdp.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://xhl.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://ihp.uphjek.com

Ruby: x.length;  x.size
来源：http://nbo.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://rre.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://ujq.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mki.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vph.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ckj.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fuk.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aei.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://agp.uphjek.com

Ruby: a == b
来源：http://cbl.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ucb.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dqd.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kmc.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://ohb.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yqn.birdmap.top

TS:   if (x == null) {}
来源：http://tnu.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hng.zdqjudy.top

Go:   if x == nil {}
来源：http://wvl.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bnf.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://wqi.tarul.cn

[P07] 防抖与节流
来源：http://nxq.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ito.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://wpi.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yom.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwu.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yqs.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oqd.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vwu.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uvs.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://vqh.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ucz.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fff.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ajv.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hfg.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xlk.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lvp.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lhz.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uvk.daria6918.cn

================================================================================
来源：http://msv.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jyx.yfazqb.com

================================================================================
来源：http://nvi.shanyushiyangkeji.top

[Q01] 创建表
来源：http://lfp.pycfn.com

CREATE TABLE users (
来源：http://vkc.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mfo.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://bsm.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://nae.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://afn.ydjk.org.cn

);
来源：http://lif.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://ztu.fzhhl.top

CREATE TABLE orders (
来源：http://cpo.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nlo.dianchejie.cn

user_id INT NOT NULL,
来源：http://nwe.sysykeji.top

amount DECIMAL(10, 2),
来源：http://aqv.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vac.jianghu66.top

);
来源：http://tvc.daria6918.cn

[Q03] 增加列
来源：http://vmt.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rws.bbcook.cn

[Q04] 修改列类型
来源：http://asv.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ysj.jianghu66.top

[Q05] 重命名列
来源：http://xxw.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ugk.jinyuanbaomall.cn

[Q06] 删除列
来源：http://gjd.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://iwb.snrcjt.cn

[Q07] 删除表
来源：http://gid.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://fqh.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://nnt.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ohm.dashuyun.cn

[Q09] 创建唯一索引
来源：http://tws.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jjf.yvedp.cn

[Q10] 插入单行
来源：http://rsb.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yph.meibo888.top

[Q11] 一次插入多行
来源：http://iya.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jec.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://fux.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://stn.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uzf.xylfe.cn

[Q13] 忽略重复插入
来源：http://kcz.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hwm.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://fdu.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gfp.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://myq.aizwys.cn

[Q15] 查询全部
来源：http://mlx.xuanzx.com

SELECT * FROM users;
来源：http://swj.ctjpmb.com

[Q16] 查询指定列
来源：http://sqx.vqdsnc.cn

SELECT id, name FROM users;
来源：http://cnc.cqqwz.cn

[Q17] 条件查询
来源：http://gnc.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://owj.9152youxi.cn

[Q18] 模糊匹配
来源：http://wkk.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eyd.jyoumei.cn

[Q19] 范围查询
来源：http://tzk.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gnr.zhengqikj.top

[Q20] IN 列表
来源：http://qrb.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ygr.bbcook.cn

[Q21] 空值判断
来源：http://hvw.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://swu.jianghu66.top

[Q22] 排序
来源：http://dab.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wpm.xylfe.cn

[Q23] 分页
来源：http://hex.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iau.tanke756.top

[Q24] 去重
来源：http://fni.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://ado.zhixingplan.top

[Q25] 只取前 N 条
来源：http://bpq.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ldz.ppjwa.cn

[Q26] 计数
来源：http://zyl.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://jmt.ctjpmb.com

[Q27] 条件计数
来源：http://zdb.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oyy.yongpay.top

[Q28] 求和与平均
来源：http://qxv.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lrl.fktsv.cn

[Q29] 最大最小值
来源：http://pja.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ieb.ydjk.org.cn

[Q30] 分组统计
来源：http://exn.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pnj.zhengqikj.top

[Q31] 分组后过滤
来源：http://yuy.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://erg.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://pfu.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pkk.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uzn.nanxuanxn.top

[Q33] 多列分组
来源：http://pyf.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://acd.birdmap.top

[Q34] 每组取第一条
来源：http://tuq.xziqi.cn

SELECT * FROM (
来源：http://klr.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vwx.sufxvd.cn

) t WHERE rn = 1;
来源：http://act.zdbjq.cn

[Q35] 内连接
来源：http://bkt.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oxd.svipenyu.cn

[Q36] 左连接
来源：http://nkx.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qgj.zhongyouzk.top

[Q37] 右连接
来源：http://koy.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tjs.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://hrl.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ygt.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://sla.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://otd.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kck.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://heq.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sax.sysykeji.top

[Q41] 多表连接
来源：http://tfe.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cze.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://edd.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://htm.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://ovx.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://vnl.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uur.redwolf501.top

[Q43] 标量子查询
来源：http://fob.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://njl.havefunace.top

[Q44] IN 子查询
来源：http://whv.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://loj.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://ucs.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://stm.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lco.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pfc.haohaochexian.top

[Q47] 与平均值比较
来源：http://zxr.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opp.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://opq.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jln.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://cyn.sjlbkw.cn

[Q49] 更新单行
来源：http://wcw.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mqm.jinqigfzy.top

[Q50] 批量更新
来源：http://lsm.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kfc.svipenyu.cn

[Q51] 用子查询更新
来源：http://acl.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xok.gaohongyu789.top

[Q52] 删除指定行
来源：http://kdn.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://bum.yvedp.cn

[Q53] 按条件删除
来源：http://arx.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kie.kuanghao11.cn

[Q54] 清空表
来源：http://cja.hammf.cn

TRUNCATE TABLE logs;
来源：http://cch.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://coa.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pjc.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://mtf.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kqi.kuanghao11.cn

[Q57] 行号
来源：http://sjp.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zod.bjfxy.top

[Q58] 累计求和
来源：http://khg.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hml.gotoacloud.top

[Q59] 分组内累计
来源：http://dlm.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uhy.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://lki.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jtm.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wyk.yj20258888.top

[Q61] 移动平均
来源：http://lfj.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nsl.jqgfzy.top

[Q62] 分组占比
来源：http://ima.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pws.yongpay.top

[Q63] 开启事务
来源：http://aur.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wle.ydjk.org.cn

[Q64] 提交事务
来源：http://plk.chenlongwang.top

COMMIT;
来源：http://ybs.chenzaomai.com

[Q65] 回滚事务
来源：http://hlj.jinqigfzy.top

ROLLBACK;
来源：http://yyz.chenjidiqi.icu

[Q66] 行锁查询
来源：http://goo.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://svs.yuxming.cn

[Q67] 设置隔离级别
来源：http://amv.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igu.zhengqikj.top

[Q68] 保存点
来源：http://iad.zdbjq.cn

SAVEPOINT sp1;
来源：http://fxm.epnwcf.com

ROLLBACK TO sp1;
来源：http://ypl.xylfe.cn

[Q69] 查看执行计划
来源：http://mjp.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pci.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://gnx.yongpay.top

ANALYZE TABLE users;
来源：http://czb.ivvv.top

[Q71] 查看建表语句
来源：http://ymz.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ssb.hnxiangtu.top

[Q72] 查看索引
来源：http://xpk.snrcjt.cn

SHOW INDEX FROM users;
来源：http://fmm.jlsjyb.cn

[Q73] 查看表状态
来源：http://afr.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://eme.0kj1m.cn

[Q74] 强制使用索引
来源：http://bgs.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://new.andypj.xyz

[Q75] 日期格式化
来源：http://qcs.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://prq.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sdv.gzhubu.top

[Q76] 按天统计
来源：http://csz.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jca.9152youxi.cn

[Q77] 时间加减
来源：http://ioc.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dta.feifeiyinyue.top

[Q78] 当前时间
来源：http://hwk.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tus.yvedp.cn

[Q79] 字符串拼接
来源：http://orf.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sqr.yvedp.cn

[Q80] 字符串截取
来源：http://wev.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cey.0kj1m.cn

[Q81] 字符串替换
来源：http://gkw.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kru.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://qmq.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://syh.dianchejie.cn

[Q83] 大小写转换
来源：http://kuo.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cwq.ydzc1.top

[Q84] 去除首尾空格
来源：http://tim.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://nxz.chenjidiqi.icu

[Q85] 数值取整
来源：http://jzo.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iia.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://dis.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikg.tarul.cn

[Q87] JSON 字段做条件
来源：http://efm.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jrr.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://plr.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lhq.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jns.sysykeji.top

[Q89] 判断表是否存在
来源：http://gxn.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://din.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://sfb.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://psz.jinghuilouyu.cn

================================================================================
来源：http://pkc.chenjidiqi.icu

R. Bash 专题
来源：http://amv.mhx1999.top

================================================================================
来源：http://xec.sufxvd.cn

[R01] shebang 与严格模式
来源：http://jjz.shzxlz.cn

#!/usr/bin/env bash
来源：http://tzk.hywenlv.cn

set -euo pipefail
来源：http://shr.daxiang520.top

[R02] 变量赋值与使用
来源：http://mhy.yongpay.top

name="Tom"; echo "$name"
来源：http://knn.jinghuilouyu.cn

[R03] 只读变量
来源：http://idq.cdnleiting.top

readonly PI=3.14
来源：http://svx.jianghu66.top

[R04] 位置参数
来源：http://cdt.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tod.jianghu66.top

[R05] 参数默认值
来源：http://qhm.xuetiantiany.cn

name="${1:-default}"
来源：http://nhy.fehbvm.com

[R06] 判断命令是否存在
来源：http://ejt.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nrc.gogol.net.cn

[R07] if 判断文件
来源：http://xhl.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vtv.tanke756.top

[R08] 数值比较
来源：http://mmj.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://oyr.wangdashe.top

[R09] 字符串比较
来源：http://hxv.yongpay.top


<!-- 参考信息 -->