代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tln.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hyu.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://otz.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eqm.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mmc.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rzy.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://nns.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cbv.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iaf.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uzl.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xrp.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jos.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mve.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xuh.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xti.meibo888.top

[P04] 求长度
来源：http://ofa.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xyh.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xwu.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uut.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cra.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://eqo.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://bni.jyoumei.cn

Ruby: x.length;  x.size
来源：http://zul.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://njn.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://bow.jinqigfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aqz.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hgv.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://msl.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvp.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://crn.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qzr.snrcjt.cn

Ruby: a == b
来源：http://yin.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xyv.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bae.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xsl.tanke756.top

PHP:  if (empty($x)) {}
来源：http://dmw.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://htq.fehbvm.com

TS:   if (x == null) {}
来源：http://nkv.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mub.zhoulong.xyz

Go:   if x == nil {}
来源：http://duy.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uji.guowangkeji.top

C#:   if (x is null) {}
来源：http://jmj.vehdjk.com

[P07] 防抖与节流
来源：http://sxa.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bqp.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://wsn.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kiy.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgy.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qcc.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fyy.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hvp.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jbz.meibo888.top

[P08] 处理浮点精度问题
来源：http://lkq.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fdl.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rmg.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aca.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vhb.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gmn.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cyv.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gov.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qmk.vqdsnc.cn

================================================================================
来源：http://mej.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iuf.ybcxt.top

================================================================================
来源：http://bkx.aizwys.cn

[Q01] 创建表
来源：http://ixr.iojbl.cn

CREATE TABLE users (
来源：http://xhu.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nnt.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://ndg.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://jtg.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vxp.chenlongwang.top

);
来源：http://hzk.tanke756.top

[Q02] 创建带外键的表
来源：http://mcn.wangdashe.top

CREATE TABLE orders (
来源：http://aav.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gpt.fehbvm.com

user_id INT NOT NULL,
来源：http://fzj.guannengcc.top

amount DECIMAL(10, 2),
来源：http://swn.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wjj.shuidangran.top

);
来源：http://hdl.shanyushiyangtech.top

[Q03] 增加列
来源：http://dfs.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tnn.zhongyouzk.top

[Q04] 修改列类型
来源：http://glw.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bnq.xuanzx.com

[Q05] 重命名列
来源：http://pvr.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://orw.hnxiangtu.top

[Q06] 删除列
来源：http://pmg.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lfd.uphjek.com

[Q07] 删除表
来源：http://nek.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://ywg.jqgfzy.top

[Q08] 创建普通索引
来源：http://guc.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vhe.cheryme.top

[Q09] 创建唯一索引
来源：http://tnf.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ubj.xuanzx.com

[Q10] 插入单行
来源：http://yhg.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vbr.epnwcf.com

[Q11] 一次插入多行
来源：http://tmi.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ujy.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://vhd.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://rcj.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uog.andypj.xyz

[Q13] 忽略重复插入
来源：http://gqi.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iou.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://uhs.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ovm.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kop.cqqwz.cn

[Q15] 查询全部
来源：http://mik.wangdashe.top

SELECT * FROM users;
来源：http://bgi.jiagoushi.top

[Q16] 查询指定列
来源：http://qsn.vehdjk.com

SELECT id, name FROM users;
来源：http://bhb.hcnkem.com

[Q17] 条件查询
来源：http://agq.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rct.cheryme.top

[Q18] 模糊匹配
来源：http://ghu.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zjg.zycfv.cn

[Q19] 范围查询
来源：http://zgj.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qju.yanxiufei.cn

[Q20] IN 列表
来源：http://kwt.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dtn.gogol.net.cn

[Q21] 空值判断
来源：http://gzb.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bwy.yvedp.cn

[Q22] 排序
来源：http://kdo.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://swu.xingfuxueyuan.xyz

[Q23] 分页
来源：http://byf.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wdp.hcnkem.com

[Q24] 去重
来源：http://ptb.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://vjp.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://qez.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cvq.yj20258.top

[Q26] 计数
来源：http://map.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://tig.vehdjk.com

[Q27] 条件计数
来源：http://guz.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mvz.sysykeji.top

[Q28] 求和与平均
来源：http://wsm.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pip.xuetiantiany.cn

[Q29] 最大最小值
来源：http://ozk.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cfo.jqgufenzy.top

[Q30] 分组统计
来源：http://bue.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wet.dianchejie.cn

[Q31] 分组后过滤
来源：http://glo.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://skr.redwolf501.top

[Q32] 分组拼接字符串
来源：http://ebc.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tse.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gby.hywenlv.cn

[Q33] 多列分组
来源：http://wok.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bqt.epnwcf.com

[Q34] 每组取第一条
来源：http://hyw.cucudq.cn

SELECT * FROM (
来源：http://ybb.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vfz.vehdjk.com

) t WHERE rn = 1;
来源：http://bjy.ctjpmb.com

[Q35] 内连接
来源：http://wvh.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zie.quarkkingdee.top

[Q36] 左连接
来源：http://oxl.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kiw.hywenlv.cn

[Q37] 右连接
来源：http://udr.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kwe.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://bjf.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://twz.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://iyt.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hjw.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ipb.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ddi.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nxr.sjlbkw.cn

[Q41] 多表连接
来源：http://gan.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://paa.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://ady.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://uuo.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://sgv.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://dxg.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gkz.jyoumei.cn

[Q43] 标量子查询
来源：http://fcs.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vfw.guowangkeji.top

[Q44] IN 子查询
来源：http://czv.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wvk.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://qjr.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xsh.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://alo.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xwn.316326.xyz

[Q47] 与平均值比较
来源：http://vea.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bzh.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://nej.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vqi.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://tti.zdqjudy.top

[Q49] 更新单行
来源：http://emt.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oqc.snrcjt.cn

[Q50] 批量更新
来源：http://aho.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zqm.sjlbkw.cn

[Q51] 用子查询更新
来源：http://rdg.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pfg.jqgufenzy.top

[Q52] 删除指定行
来源：http://olh.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://lmh.smart0.xyz

[Q53] 按条件删除
来源：http://mqt.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bum.hfpthk.cn

[Q54] 清空表
来源：http://aoo.guannengcc.top

TRUNCATE TABLE logs;
来源：http://yyk.epnwcf.com

[Q55] 排名（并列占位）
来源：http://kxo.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pth.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://mrf.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gty.chenzaomai.com

[Q57] 行号
来源：http://nue.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://maf.zhiwuduotai.top

[Q58] 累计求和
来源：http://xdt.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocq.sweek.top

[Q59] 分组内累计
来源：http://kbr.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gqo.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://yjy.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ekt.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rfy.xuanzx.com

[Q61] 移动平均
来源：http://pvy.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jbn.hcnkem.com

[Q62] 分组占比
来源：http://pxu.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ibq.sufxvd.cn

[Q63] 开启事务
来源：http://zac.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://mpu.zhijiandao.cn

[Q64] 提交事务
来源：http://sse.jqgfzy.top

COMMIT;
来源：http://tnd.jianghu66.top

[Q65] 回滚事务
来源：http://efk.jiagoushi.top

ROLLBACK;
来源：http://vts.jinqigfzy.top

[Q66] 行锁查询
来源：http://rch.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dyg.sufxvd.cn

[Q67] 设置隔离级别
来源：http://yjt.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpv.shzxlz.cn

[Q68] 保存点
来源：http://uol.52xcode.cn

SAVEPOINT sp1;
来源：http://kej.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://zcw.svipenyu.cn

[Q69] 查看执行计划
来源：http://nws.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tug.redwolf501.top

[Q70] 更新统计信息
来源：http://xuj.tarul.cn

ANALYZE TABLE users;
来源：http://ern.jyoumei.cn

[Q71] 查看建表语句
来源：http://wkb.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ztx.52xcode.cn

[Q72] 查看索引
来源：http://jyr.hfpthk.cn

SHOW INDEX FROM users;
来源：http://wqh.xylfe.cn

[Q73] 查看表状态
来源：http://bcv.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yyy.bbcook.cn

[Q74] 强制使用索引
来源：http://rgp.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jvq.redwolf501.top

[Q75] 日期格式化
来源：http://qum.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tus.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dlc.nwbrower.top

[Q76] 按天统计
来源：http://kcu.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bur.pycfn.com

[Q77] 时间加减
来源：http://tul.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tgp.meibo888.top

[Q78] 当前时间
来源：http://flm.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uer.pycfn.com

[Q79] 字符串拼接
来源：http://khk.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jmu.sweek.top

[Q80] 字符串截取
来源：http://qzy.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tmw.tianlin.xyz

[Q81] 字符串替换
来源：http://gkq.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://udn.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://dcm.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bdk.316326.xyz

[Q83] 大小写转换
来源：http://pip.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uoq.tanke756.top

[Q84] 去除首尾空格
来源：http://vki.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://wnt.ydjk.org.cn

[Q85] 数值取整
来源：http://kuy.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://unz.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://adx.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://siq.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://yjq.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejh.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://heg.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uko.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tnw.gotoacloud.top

[Q89] 判断表是否存在
来源：http://lmh.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wob.quarkkingdee.top

[Q90] 生成序号列
来源：http://ued.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fvx.0kj1m.cn

================================================================================
来源：http://bmt.chenzaomai.com

R. Bash 专题
来源：http://aha.gzhubu.top

================================================================================
来源：http://ybt.iojbl.cn

[R01] shebang 与严格模式
来源：http://lmb.hnxiangtu.top

#!/usr/bin/env bash
来源：http://qnj.gzhubu.top

set -euo pipefail
来源：http://aep.316326.xyz

[R02] 变量赋值与使用
来源：http://fpy.svipenyu.cn

name="Tom"; echo "$name"
来源：http://idu.uphjek.com

[R03] 只读变量
来源：http://xmw.gotoacloud.top

readonly PI=3.14
来源：http://kmw.redwolf501.top

[R04] 位置参数
来源：http://cdo.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cye.tianlin.xyz

[R05] 参数默认值
来源：http://ucc.aizwys.cn

name="${1:-default}"
来源：http://jko.hammf.cn

[R06] 判断命令是否存在
来源：http://ehl.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khm.tanke756.top

[R07] if 判断文件
来源：http://lus.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cqn.mhx1999.top

[R08] 数值比较
来源：http://xjr.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ghe.zhongyouzk.top

[R09] 字符串比较
来源：http://xui.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mks.ppjwa.cn

[R10] 正则匹配
来源：http://gbc.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bjy.guowangkeji.top

[R11] case 多分支
来源：http://vyo.chenjidiqi.icu

case "$1" in
来源：http://fim.yuanzhike.top

start) echo "启动" ;;
来源：http://qgm.jyoumei.cn

stop)  echo "停止" ;;
来源：http://izb.havefunace.top

*)     echo "未知命令" ;;
来源：http://vpc.hnqzz.top

esac
来源：http://rwl.vqdsnc.cn

[R12] for 遍历文件
来源：http://rau.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://vjm.hesvh.cn

[R13] for 计数循环
来源：http://ndf.zhoulong.xyz


<!-- 参考信息 -->