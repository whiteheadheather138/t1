代发 wailian999

TS:   crypto.randomUUID()
来源：http://mod.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://aih.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://nrz.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://lcw.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://paz.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://tto.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sgz.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zwy.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zuj.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xmf.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qpk.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eba.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lwi.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nzq.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://jvy.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://psl.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pri.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://okf.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gnv.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mom.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://frd.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fbl.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nyo.jqgufenzy.top

[P04] 求长度
来源：http://ujw.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jyq.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmx.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shv.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzg.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://fzi.xylfe.cn

Go:   len(arr);  len(m)
来源：http://vrq.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://xzh.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vvb.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://jib.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gos.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zyb.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ung.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bvv.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kof.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jgm.gogol.net.cn

Ruby: a == b
来源：http://vxt.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pcf.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tts.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://poi.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://uhj.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rsd.yangfankeji.com

TS:   if (x == null) {}
来源：http://nlj.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uym.xziqi.cn

Go:   if x == nil {}
来源：http://jfr.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xbr.yj20258888.top

C#:   if (x is null) {}
来源：http://uzm.jqgfzy.top

[P07] 防抖与节流
来源：http://gin.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mnv.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://umk.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bql.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyg.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yss.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gbi.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yit.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fvw.yongpay.top

[P08] 处理浮点精度问题
来源：http://dgw.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ddg.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tel.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wyy.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gwr.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fza.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vyt.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iwk.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://can.iojbl.cn

================================================================================
来源：http://ran.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xou.zhiwuduotai.top

================================================================================
来源：http://tma.kuanghao11.cn

[Q01] 创建表
来源：http://qbi.zycfv.cn

CREATE TABLE users (
来源：http://azy.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gce.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://wxg.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://fuw.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ckh.jinqigfzy.top

);
来源：http://rtc.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://tia.yanxiufei.cn

CREATE TABLE orders (
来源：http://ebs.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://axb.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://jnp.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://qxt.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yvw.ehwqpu.com

);
来源：http://cod.zhaomingkeji.xyz

[Q03] 增加列
来源：http://pad.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gcj.zhixingplan.top

[Q04] 修改列类型
来源：http://tpk.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fmx.ybcxt.top

[Q05] 重命名列
来源：http://cjt.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cjd.sjlbkw.cn

[Q06] 删除列
来源：http://wcf.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://kfs.fzhhl.top

[Q07] 删除表
来源：http://sut.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://wix.hammf.cn

[Q08] 创建普通索引
来源：http://qyc.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://beb.sweek.top

[Q09] 创建唯一索引
来源：http://nrz.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cqy.andypj.xyz

[Q10] 插入单行
来源：http://csb.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://okh.sjlbkw.cn

[Q11] 一次插入多行
来源：http://lcn.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ztu.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://gzv.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jfo.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gda.tanke756.top

[Q13] 忽略重复插入
来源：http://bgt.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gea.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://oym.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xuc.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cnc.daria6918.cn

[Q15] 查询全部
来源：http://akp.cdnleiting.top

SELECT * FROM users;
来源：http://wuc.jyoumei.cn

[Q16] 查询指定列
来源：http://znv.guowangkeji.top

SELECT id, name FROM users;
来源：http://rhm.redwolf501.top

[Q17] 条件查询
来源：http://ahn.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pqg.aibaodan.cn

[Q18] 模糊匹配
来源：http://obb.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xdw.fengsongda.top

[Q19] 范围查询
来源：http://fal.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://omu.pengpengdd.cyou

[Q20] IN 列表
来源：http://vqx.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://evg.birdmap.top

[Q21] 空值判断
来源：http://hac.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wlw.ybcxt.top

[Q22] 排序
来源：http://gqm.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lbe.tanke756.top

[Q23] 分页
来源：http://teq.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qdo.nanxinkj.top

[Q24] 去重
来源：http://hhp.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://upd.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://mtc.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cbf.yj20258.top

[Q26] 计数
来源：http://bgs.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://xvj.epnwcf.com

[Q27] 条件计数
来源：http://rcf.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://azk.andypj.xyz

[Q28] 求和与平均
来源：http://bmm.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pyt.yongpay.top

[Q29] 最大最小值
来源：http://qje.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhu.haohaochexian.top

[Q30] 分组统计
来源：http://opq.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fei.yvedp.cn

[Q31] 分组后过滤
来源：http://wqk.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://plv.316326.xyz

[Q32] 分组拼接字符串
来源：http://mmk.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nmq.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fok.gzhubu.top

[Q33] 多列分组
来源：http://wiz.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qat.birdmap.top

[Q34] 每组取第一条
来源：http://vad.sxryk.cn

SELECT * FROM (
来源：http://bvj.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dfh.ivvv.top

) t WHERE rn = 1;
来源：http://quz.pycfn.com

[Q35] 内连接
来源：http://ksi.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nao.jinqigufen.top

[Q36] 左连接
来源：http://hot.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://egk.fanxiaobao.xyz

[Q37] 右连接
来源：http://btq.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lsl.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tul.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fin.yj20258.top

[Q39] 自连接（查上下级）
来源：http://tkw.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://njm.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dcu.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vtu.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nqo.tian-w.cn

[Q41] 多表连接
来源：http://gdl.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://qiq.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://cyx.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://qau.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://bfr.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://zvj.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tlq.hfpthk.cn

[Q43] 标量子查询
来源：http://glh.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hwn.smart0.xyz

[Q44] IN 子查询
来源：http://jph.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nlx.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://uxd.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqi.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://jiw.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ukz.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://hym.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eyl.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://rlx.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ntx.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://reu.yj20258.top

[Q49] 更新单行
来源：http://ees.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nvh.fanxiaobao.xyz

[Q50] 批量更新
来源：http://krw.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://khx.sufxvd.cn

[Q51] 用子查询更新
来源：http://awo.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xos.iojbl.cn

[Q52] 删除指定行
来源：http://ypo.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://ckt.9152youxi.cn

[Q53] 按条件删除
来源：http://jlf.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jnq.uphjek.com

[Q54] 清空表
来源：http://dhb.fzhhl.top

TRUNCATE TABLE logs;
来源：http://pgt.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://yzv.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ffd.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://jbq.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cga.aizwys.cn

[Q57] 行号
来源：http://gyp.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://epv.yueranfly.top

[Q58] 累计求和
来源：http://wjc.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jya.guowangkeji.top

[Q59] 分组内累计
来源：http://jzo.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgl.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://xsg.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ymg.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jlk.xuetiantiany.cn

[Q61] 移动平均
来源：http://tql.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ucp.meibo888.top

[Q62] 分组占比
来源：http://lwy.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dhb.hongshengwenyu.top

[Q63] 开启事务
来源：http://dsj.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cxs.gaohongyu789.top

[Q64] 提交事务
来源：http://jtj.c1oappe.top

COMMIT;
来源：http://ekt.ydzc1.top

[Q65] 回滚事务
来源：http://hid.yuxming.cn

ROLLBACK;
来源：http://ecs.nanxuanxn.top

[Q66] 行锁查询
来源：http://bqo.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bkp.hysaishi.cn

[Q67] 设置隔离级别
来源：http://ewc.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vem.tanke756.top

[Q68] 保存点
来源：http://rbv.sjlbkw.cn

SAVEPOINT sp1;
来源：http://azg.316326.xyz

ROLLBACK TO sp1;
来源：http://vfk.yonumen.top

[Q69] 查看执行计划
来源：http://gft.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dpn.redwolf501.top

[Q70] 更新统计信息
来源：http://mve.jianghu66.top

ANALYZE TABLE users;
来源：http://kpv.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://vcb.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tzh.aizwys.cn

[Q72] 查看索引
来源：http://amf.uphjek.com

SHOW INDEX FROM users;
来源：http://iak.wangshuangyany.cn

[Q73] 查看表状态
来源：http://mrq.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mvg.tian-w.cn

[Q74] 强制使用索引
来源：http://uto.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jga.yj202588.top

[Q75] 日期格式化
来源：http://qgj.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xme.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nnc.hongshengwenyu.top

[Q76] 按天统计
来源：http://vtu.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wab.yuanzhike.top

[Q77] 时间加减
来源：http://laf.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tjj.shanyushiyangtech.top

[Q78] 当前时间
来源：http://cyu.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lpu.hammf.cn

[Q79] 字符串拼接
来源：http://kjl.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cgh.c1oappe.top

[Q80] 字符串截取
来源：http://zyy.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bxo.cheryme.top

[Q81] 字符串替换
来源：http://zef.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://znm.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://fff.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rcf.jiagoushi.top

[Q83] 大小写转换
来源：http://hqi.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kcl.zycfv.cn

[Q84] 去除首尾空格
来源：http://ysx.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://ohg.jlsjyb.cn

[Q85] 数值取整
来源：http://dcb.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ppa.uphjek.com

[Q86] 读取 JSON 字段
来源：http://qtp.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ecz.yj20258888.top

[Q87] JSON 字段做条件
来源：http://rty.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dqu.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://hat.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibg.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fuv.gogol.net.cn

[Q89] 判断表是否存在
来源：http://qzk.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lqs.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://ats.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yhe.gaohongyu789.top

================================================================================
来源：http://nbg.gzhubu.top

R. Bash 专题
来源：http://kbg.tarul.cn

================================================================================
来源：http://cfp.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://ubr.zycfv.cn

#!/usr/bin/env bash
来源：http://jpq.hfpthk.cn

set -euo pipefail
来源：http://bcq.jinqigufen.top

[R02] 变量赋值与使用
来源：http://szd.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://yrz.vehdjk.com

[R03] 只读变量
来源：http://azk.ybcxt.top

readonly PI=3.14
来源：http://egk.yj20258888.top

[R04] 位置参数
来源：http://tzc.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rrd.jqgfzy.top

[R05] 参数默认值
来源：http://gqs.316326.xyz

name="${1:-default}"
来源：http://ldl.tarul.cn

[R06] 判断命令是否存在
来源：http://lvg.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lae.gzhubu.top

[R07] if 判断文件
来源：http://ete.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://haq.yuanzhike.top

[R08] 数值比较
来源：http://pyq.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mvc.hesvh.cn

[R09] 字符串比较
来源：http://xtk.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cyi.aizwys.cn

[R10] 正则匹配
来源：http://rox.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bdx.uphjek.com

[R11] case 多分支
来源：http://uaw.yonumen.top


<!-- 参考信息 -->