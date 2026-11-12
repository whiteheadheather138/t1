代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hrd.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://muz.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://svd.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nvu.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hdj.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://szh.zycfv.cn

[P03] 生成短随机字符串
来源：http://hku.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cdv.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jjj.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tre.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yfd.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://twg.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://osc.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oxd.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zjw.kuanghao11.cn

[P04] 求长度
来源：http://jfl.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vau.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lzx.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dau.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tga.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://fmw.fktsv.cn

Go:   len(arr);  len(m)
来源：http://buh.cashguo.top

Ruby: x.length;  x.size
来源：http://onj.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://qic.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://jep.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://rit.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jtz.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jec.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yyx.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pnn.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://xqw.yonumen.top

Ruby: a == b
来源：http://flk.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytf.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://owu.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gdv.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://uxq.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://big.9152youxi.cn

TS:   if (x == null) {}
来源：http://cqi.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://crq.xinyue.icu

Go:   if x == nil {}
来源：http://yzq.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://inu.hammf.cn

C#:   if (x is null) {}
来源：http://czi.pengpengdd.cyou

[P07] 防抖与节流
来源：http://kkt.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wmf.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://uxl.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxc.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcy.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://avc.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vur.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://olt.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lal.havefunace.top

[P08] 处理浮点精度问题
来源：http://ljf.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://grm.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://efo.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hjd.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oqy.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xak.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ufx.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oik.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wbb.jinghuilouyu.cn

================================================================================
来源：http://ebh.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gbk.iojbl.cn

================================================================================
来源：http://ems.pengpengdd.cyou

[Q01] 创建表
来源：http://xbq.xuanzx.com

CREATE TABLE users (
来源：http://bjm.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://owq.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://tiq.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://xgg.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zpz.shuidangran.top

);
来源：http://drp.hfpthk.cn

[Q02] 创建带外键的表
来源：http://ckd.chenjidiqi.icu

CREATE TABLE orders (
来源：http://rvb.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rff.hfpthk.cn

user_id INT NOT NULL,
来源：http://mjl.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://axl.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qqw.sxryk.cn

);
来源：http://wsk.nanxuanxn.top

[Q03] 增加列
来源：http://hvg.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tmy.ybcxt.top

[Q04] 修改列类型
来源：http://hja.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ipj.yonumen.top

[Q05] 重命名列
来源：http://ijx.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dgo.cashguo.top

[Q06] 删除列
来源：http://fbb.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://rmy.ehwqpu.com

[Q07] 删除表
来源：http://der.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://quf.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://npp.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://apx.jinqigufen.top

[Q09] 创建唯一索引
来源：http://ilx.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iay.hcnkem.com

[Q10] 插入单行
来源：http://vmh.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iof.52xcode.cn

[Q11] 一次插入多行
来源：http://glz.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gbp.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://lhm.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://tmf.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://maw.iojbl.cn

[Q13] 忽略重复插入
来源：http://iko.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ukm.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://tmy.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pun.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mjb.redwolf501.top

[Q15] 查询全部
来源：http://itn.nanxuanxn.top

SELECT * FROM users;
来源：http://kss.sysykeji.top

[Q16] 查询指定列
来源：http://emk.sweek.top

SELECT id, name FROM users;
来源：http://iea.fehbvm.com

[Q17] 条件查询
来源：http://bia.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jqf.yuanzhike.top

[Q18] 模糊匹配
来源：http://pid.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pqr.nanxinkj.top

[Q19] 范围查询
来源：http://dvi.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lpy.52xcode.cn

[Q20] IN 列表
来源：http://nes.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ige.ctjpmb.com

[Q21] 空值判断
来源：http://zsx.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://eye.sweek.top

[Q22] 排序
来源：http://bnw.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hwq.hfpthk.cn

[Q23] 分页
来源：http://wji.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xty.xziqi.cn

[Q24] 去重
来源：http://wqt.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://zes.haohaochexian.top

[Q25] 只取前 N 条
来源：http://qxf.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://niw.fengsongda.top

[Q26] 计数
来源：http://ciq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://ipw.fzhhl.top

[Q27] 条件计数
来源：http://exw.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://meq.hysaishi.cn

[Q28] 求和与平均
来源：http://guh.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vnb.yangfankeji.com

[Q29] 最大最小值
来源：http://nvl.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ekh.mhx1999.top

[Q30] 分组统计
来源：http://tba.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jsz.tian-w.cn

[Q31] 分组后过滤
来源：http://diy.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kzh.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://iur.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jrz.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bhp.nanxinkj.top

[Q33] 多列分组
来源：http://hdw.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lsg.iojbl.cn

[Q34] 每组取第一条
来源：http://tju.kuanghao11.cn

SELECT * FROM (
来源：http://gdq.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mjb.andypj.xyz

) t WHERE rn = 1;
来源：http://soq.daria6918.cn

[Q35] 内连接
来源：http://foh.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rqx.zdqjudy.top

[Q36] 左连接
来源：http://kdo.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tjd.yongpay.top

[Q37] 右连接
来源：http://bpu.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://urh.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tkz.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lmb.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://htl.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xdu.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hlr.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qyj.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iol.wangdashe.top

[Q41] 多表连接
来源：http://kfg.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://piv.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://rvy.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://wvn.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://vjr.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://azs.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pyx.svipenyu.cn

[Q43] 标量子查询
来源：http://yuu.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lkf.hywenlv.cn

[Q44] IN 子查询
来源：http://mhr.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mdq.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://omt.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ugm.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nhi.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://glr.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://rjj.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://far.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://ina.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aex.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://sos.yj20258888.top

[Q49] 更新单行
来源：http://xup.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tws.xuanzx.com

[Q50] 批量更新
来源：http://fiv.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uox.fktsv.cn

[Q51] 用子查询更新
来源：http://dfh.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qzk.hesvh.cn

[Q52] 删除指定行
来源：http://unm.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://daj.meibo888.top

[Q53] 按条件删除
来源：http://tgr.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gxy.9152youxi.cn

[Q54] 清空表
来源：http://fhy.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://wso.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://nnj.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cgp.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://iap.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xwp.hcnkem.com

[Q57] 行号
来源：http://ewp.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ucq.zycfv.cn

[Q58] 累计求和
来源：http://siy.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mpk.aizwys.cn

[Q59] 分组内累计
来源：http://fkm.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vca.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://ykm.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://luz.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jho.wangdashe.top

[Q61] 移动平均
来源：http://spt.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://osw.pengpengdd.cyou

[Q62] 分组占比
来源：http://pdd.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://msq.fengsongda.top

[Q63] 开启事务
来源：http://mtj.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mii.zhijiandao.cn

[Q64] 提交事务
来源：http://jjq.jyoumei.cn

COMMIT;
来源：http://hjr.jinqigfzy.top

[Q65] 回滚事务
来源：http://dgm.zhoulong.xyz

ROLLBACK;
来源：http://dsy.ctjpmb.com

[Q66] 行锁查询
来源：http://tsm.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://krh.xinyue.icu

[Q67] 设置隔离级别
来源：http://yuo.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hue.guowangkeji.top

[Q68] 保存点
来源：http://lqh.epnwcf.com

SAVEPOINT sp1;
来源：http://xmf.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://nxw.tanke756.top

[Q69] 查看执行计划
来源：http://igi.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qpw.hcnkem.com

[Q70] 更新统计信息
来源：http://ljz.hcnkem.com

ANALYZE TABLE users;
来源：http://nox.zhoulong.xyz

[Q71] 查看建表语句
来源：http://leu.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tqs.gogol.net.cn

[Q72] 查看索引
来源：http://whx.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://zcv.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://nuc.yvedp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ppv.cheryme.top

[Q74] 强制使用索引
来源：http://wgm.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jov.ppjwa.cn

[Q75] 日期格式化
来源：http://upj.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cjn.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ybj.daria6918.cn

[Q76] 按天统计
来源：http://bcw.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aje.jinghuilouyu.cn

[Q77] 时间加减
来源：http://gdu.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qyu.aibaodan.cn

[Q78] 当前时间
来源：http://wmr.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cyy.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://pyi.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mzu.hongshengwenyu.top

[Q80] 字符串截取
来源：http://vjy.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dhp.yueranfly.top

[Q81] 字符串替换
来源：http://jqm.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yyf.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://hzf.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bbb.zhoulong.xyz

[Q83] 大小写转换
来源：http://lal.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lxz.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://mgu.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://rjv.fanxiaobao.xyz

[Q85] 数值取整
来源：http://izt.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oic.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://ylw.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jth.yj202588.top

[Q87] JSON 字段做条件
来源：http://xoc.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dgs.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://rsv.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://olh.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xac.ctjpmb.com

[Q89] 判断表是否存在
来源：http://niz.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xjo.jqgfzy.top

[Q90] 生成序号列
来源：http://wkk.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hnw.andypj.xyz

================================================================================
来源：http://qhx.aibaodan.cn

R. Bash 专题
来源：http://fhc.smart0.xyz

================================================================================
来源：http://ooo.gotoacloud.top

[R01] shebang 与严格模式
来源：http://six.ctjpmb.com

#!/usr/bin/env bash
来源：http://ggv.yongpay.top

set -euo pipefail
来源：http://hxc.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://zdc.tianlin.xyz

name="Tom"; echo "$name"
来源：http://hsl.pycfn.com

[R03] 只读变量
来源：http://trv.xylfe.cn

readonly PI=3.14
来源：http://dwz.dashuyun.cn

[R04] 位置参数
来源：http://cfo.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ucs.wangshuangyany.cn

[R05] 参数默认值
来源：http://aaq.epnwcf.com

name="${1:-default}"
来源：http://eid.dashuyun.cn

[R06] 判断命令是否存在
来源：http://gmj.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rrz.cdnleiting.top

[R07] if 判断文件
来源：http://nnj.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aqb.ppjwa.cn

[R08] 数值比较
来源：http://wsc.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bjn.zycfv.cn

[R09] 字符串比较
来源：http://phs.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mfc.yfazqb.com

[R10] 正则匹配
来源：http://sqr.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ogb.aibaodan.cn

[R11] case 多分支
来源：http://fax.cdnleiting.top

case "$1" in
来源：http://wdv.316326.xyz

start) echo "启动" ;;
来源：http://sez.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://oha.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://vec.dianchejie.cn

esac
来源：http://nod.ppjwa.cn

[R12] for 遍历文件
来源：http://fdr.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://uqs.zhiwuduotai.top

[R13] for 计数循环
来源：http://hke.iojbl.cn


<!-- 参考信息 -->