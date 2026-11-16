代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://yhs.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://pqn.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zns.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hun.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jdz.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rye.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gxq.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qjg.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eez.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sdk.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://hvz.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sls.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zlw.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aqd.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zan.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pss.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://edw.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lfw.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ihs.zdqjudy.top

[P04] 求长度
来源：http://lwz.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sum.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hlj.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://luj.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fyb.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://wqr.meibo888.top

Go:   len(arr);  len(m)
来源：http://jdd.bjfxy.top

Ruby: x.length;  x.size
来源：http://qrq.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://rzw.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://kov.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bze.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lfe.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jnl.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bsn.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vmf.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gxd.havefunace.top

Ruby: a == b
来源：http://btr.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pvt.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mig.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zpx.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://tmr.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://exm.birdmap.top

TS:   if (x == null) {}
来源：http://dst.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ttg.sxryk.cn

Go:   if x == nil {}
来源：http://vwl.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nck.sjlbkw.cn

C#:   if (x is null) {}
来源：http://ina.cheryme.top

[P07] 防抖与节流
来源：http://shb.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ess.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://vlo.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnh.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onp.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nkz.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yqq.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qnh.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bsj.gzhubu.top

[P08] 处理浮点精度问题
来源：http://dqo.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kvn.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://naj.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://evn.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kax.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://auu.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yls.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lfl.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cqr.epnwcf.com

================================================================================
来源：http://ksi.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ytg.jqgufenzy.top

================================================================================
来源：http://mcy.snrcjt.cn

[Q01] 创建表
来源：http://inu.chenlongwang.top

CREATE TABLE users (
来源：http://vra.redwolf501.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://udd.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://wop.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://bch.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uqo.shanyushiyangkeji.top

);
来源：http://fdg.guowangkeji.top

[Q02] 创建带外键的表
来源：http://qnn.hfpthk.cn

CREATE TABLE orders (
来源：http://xnd.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://smz.andypj.xyz

user_id INT NOT NULL,
来源：http://wsf.mhx1999.top

amount DECIMAL(10, 2),
来源：http://gmp.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jqd.yj20258888.top

);
来源：http://wzp.yueranfly.top

[Q03] 增加列
来源：http://gah.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xpx.fzhhl.top

[Q04] 修改列类型
来源：http://skw.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ukd.shangyingyoupin.top

[Q05] 重命名列
来源：http://kqj.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qtn.hesvh.cn

[Q06] 删除列
来源：http://myr.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://cpm.sysykeji.top

[Q07] 删除表
来源：http://xzt.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://qnx.cucudq.cn

[Q08] 创建普通索引
来源：http://hns.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://qne.gogol.net.cn

[Q09] 创建唯一索引
来源：http://juo.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wxw.smart0.xyz

[Q10] 插入单行
来源：http://sub.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qjp.vqdsnc.cn

[Q11] 一次插入多行
来源：http://iht.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pik.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://tet.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://tdq.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ala.dashuyun.cn

[Q13] 忽略重复插入
来源：http://fup.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jih.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://pug.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcf.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ols.guowangkeji.top

[Q15] 查询全部
来源：http://ciw.aizwys.cn

SELECT * FROM users;
来源：http://vqv.c1oappe.top

[Q16] 查询指定列
来源：http://gqw.wangdashe.top

SELECT id, name FROM users;
来源：http://jlg.havefunace.top

[Q17] 条件查询
来源：http://jro.ctjpmb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qxz.bbcook.cn

[Q18] 模糊匹配
来源：http://uzr.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xdt.chenjidiqi.icu

[Q19] 范围查询
来源：http://mhp.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xdm.ydjk.org.cn

[Q20] IN 列表
来源：http://opt.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://efp.redwolf501.top

[Q21] 空值判断
来源：http://ucs.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zcn.redwolf501.top

[Q22] 排序
来源：http://rwk.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zkg.hysaishi.cn

[Q23] 分页
来源：http://dwx.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wta.xinyue.icu

[Q24] 去重
来源：http://cic.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://gjo.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://wzh.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wmo.316326.xyz

[Q26] 计数
来源：http://mpa.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://msi.chenjidiqi.icu

[Q27] 条件计数
来源：http://zdn.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mox.fzhhl.top

[Q28] 求和与平均
来源：http://avq.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jvh.wangshuangyany.cn

[Q29] 最大最小值
来源：http://eex.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dnk.0kj1m.cn

[Q30] 分组统计
来源：http://xkg.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://isb.epnwcf.com

[Q31] 分组后过滤
来源：http://hzz.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zgz.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://vgr.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qam.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zfn.ivvv.top

[Q33] 多列分组
来源：http://tns.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tja.yj20258.top

[Q34] 每组取第一条
来源：http://jsu.ctjpmb.com

SELECT * FROM (
来源：http://xat.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://noo.jyoumei.cn

) t WHERE rn = 1;
来源：http://fgd.bjfxy.top

[Q35] 内连接
来源：http://sbj.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jxy.meibo888.top

[Q36] 左连接
来源：http://nsq.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ivp.mhx1999.top

[Q37] 右连接
来源：http://let.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fyy.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://ecu.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://biy.hammf.cn

[Q39] 自连接（查上下级）
来源：http://brd.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qxi.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fmn.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gxm.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://snk.52xcode.cn

[Q41] 多表连接
来源：http://jqm.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yui.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://rfg.tian-w.cn

JOIN products p ON p.id = o.product_id;
来源：http://seh.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://qdw.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://zmt.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bvj.zhengqikj.top

[Q43] 标量子查询
来源：http://xei.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gta.yueranfly.top

[Q44] IN 子查询
来源：http://snz.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lhw.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://xxn.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klt.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://inf.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fsp.xuanzx.com

[Q47] 与平均值比较
来源：http://tbn.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://naq.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://uwb.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rne.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://aqo.feifeiyinyue.top

[Q49] 更新单行
来源：http://tor.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sxg.dashuyun.cn

[Q50] 批量更新
来源：http://rxz.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sfp.cdnleiting.top

[Q51] 用子查询更新
来源：http://xsf.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qsm.smart0.xyz

[Q52] 删除指定行
来源：http://rrm.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://zoy.yj20258.top

[Q53] 按条件删除
来源：http://roe.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hml.hfpthk.cn

[Q54] 清空表
来源：http://mgv.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://jbr.fehbvm.com

[Q55] 排名（并列占位）
来源：http://djt.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vbz.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://xkh.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rtj.chenzaomai.com

[Q57] 行号
来源：http://pqk.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yjn.hongshengwenyu.top

[Q58] 累计求和
来源：http://zel.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xwb.hnqzz.top

[Q59] 分组内累计
来源：http://tho.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://byw.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://icw.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jqx.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://emi.smart0.xyz

[Q61] 移动平均
来源：http://pzy.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rdu.snrcjt.cn

[Q62] 分组占比
来源：http://kax.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qda.hfpthk.cn

[Q63] 开启事务
来源：http://hng.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ieb.jqgufenzy.top

[Q64] 提交事务
来源：http://fvi.cqqwz.cn

COMMIT;
来源：http://edr.hesvh.cn

[Q65] 回滚事务
来源：http://yzq.yfazqb.com

ROLLBACK;
来源：http://orx.aibaodan.cn

[Q66] 行锁查询
来源：http://wvd.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjt.ivvv.top

[Q67] 设置隔离级别
来源：http://mhd.chenjidiqi.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ugp.gaohongyu789.top

[Q68] 保存点
来源：http://dds.fzhhl.top

SAVEPOINT sp1;
来源：http://hmo.yuanzhike.top

ROLLBACK TO sp1;
来源：http://xuf.jiagoushi.top

[Q69] 查看执行计划
来源：http://xiy.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgl.nwbrower.top

[Q70] 更新统计信息
来源：http://xyk.tian-w.cn

ANALYZE TABLE users;
来源：http://qqx.chenlongwang.top

[Q71] 查看建表语句
来源：http://eaq.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bes.haohaochexian.top

[Q72] 查看索引
来源：http://rxf.hywenlv.cn

SHOW INDEX FROM users;
来源：http://bem.jinqigufen.top

[Q73] 查看表状态
来源：http://ksb.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lah.xziqi.cn

[Q74] 强制使用索引
来源：http://ktw.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vxn.gaohongyu789.top

[Q75] 日期格式化
来源：http://vvt.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lje.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://way.gogol.net.cn

[Q76] 按天统计
来源：http://wrs.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pwr.zdqjudy.top

[Q77] 时间加减
来源：http://dkf.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iqg.chenlongwang.top

[Q78] 当前时间
来源：http://tws.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hcv.uphjek.com

[Q79] 字符串拼接
来源：http://mfd.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kfk.cashguo.top

[Q80] 字符串截取
来源：http://ajx.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovi.svipenyu.cn

[Q81] 字符串替换
来源：http://ssg.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sgc.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://uap.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zdr.vehdjk.com

[Q83] 大小写转换
来源：http://ewz.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ynb.yuanzhike.top

[Q84] 去除首尾空格
来源：http://wcc.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://zse.ydzc1.top

[Q85] 数值取整
来源：http://gqd.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zsg.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://vjr.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vpt.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://ptt.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wxw.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://cfr.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jpf.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hgq.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ukx.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oyu.yuanzhike.top

[Q90] 生成序号列
来源：http://rgy.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wqk.guowangkeji.top

================================================================================
来源：http://aal.vqdsnc.cn

R. Bash 专题
来源：http://rpd.ehwqpu.com

================================================================================
来源：http://wmt.jiagoushi.top

[R01] shebang 与严格模式
来源：http://mmt.hnqzz.top

#!/usr/bin/env bash
来源：http://alc.meibo888.top

set -euo pipefail
来源：http://tha.jinqigufen.top

[R02] 变量赋值与使用
来源：http://vls.yj20258.top

name="Tom"; echo "$name"
来源：http://yob.redwolf501.top

[R03] 只读变量
来源：http://oux.yvedp.cn

readonly PI=3.14
来源：http://nzl.yuanzhike.top

[R04] 位置参数
来源：http://bvt.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://itg.yonumen.top

[R05] 参数默认值
来源：http://otn.hammf.cn

name="${1:-default}"
来源：http://sos.guannengcc.top

[R06] 判断命令是否存在
来源：http://jys.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bkg.gaohongyu789.top

[R07] if 判断文件
来源：http://aes.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gaa.cashguo.top

[R08] 数值比较
来源：http://znz.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uun.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://oey.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://npv.nanxuanxn.top

[R10] 正则匹配
来源：http://cmy.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ucs.9152youxi.cn

[R11] case 多分支
来源：http://mxd.nanxinkj.top

case "$1" in
来源：http://rdg.sxryk.cn

start) echo "启动" ;;
来源：http://phh.xylfe.cn

stop)  echo "停止" ;;
来源：http://dhl.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://aqd.hnqzz.top


<!-- 参考信息 -->