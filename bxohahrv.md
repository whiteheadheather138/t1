代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://kut.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://npv.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://adm.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vht.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fik.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://znx.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://spd.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vyn.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wlt.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iik.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://nsx.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://euf.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dze.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqj.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsx.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tmp.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vrz.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wxr.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ohq.xingfuxueyuan.xyz

[P04] 求长度
来源：http://wvh.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ppc.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hiy.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llb.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ifc.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://dnm.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://fcc.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://cdn.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwm.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://gdv.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aij.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uhp.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://may.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wlj.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rkx.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wje.vqdsnc.cn

Ruby: a == b
来源：http://zgm.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gcw.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oog.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tis.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://exh.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yiy.jqgfzy.top

TS:   if (x == null) {}
来源：http://vyk.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mty.ppjwa.cn

Go:   if x == nil {}
来源：http://tho.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lks.hywenlv.cn

C#:   if (x is null) {}
来源：http://xvz.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://phx.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kgb.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://zbp.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jao.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dty.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://otq.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aan.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vym.zdqjudy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://egf.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://iar.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hwm.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ggl.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ghb.xuetiantiany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sje.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yit.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ppn.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ktd.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yao.fktsv.cn

================================================================================
来源：http://pxd.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://avb.tian-w.cn

================================================================================
来源：http://ruz.cdnleiting.top

[Q01] 创建表
来源：http://teg.fzhhl.top

CREATE TABLE users (
来源：http://wke.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sld.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://mcl.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://ruo.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rri.yueranfly.top

);
来源：http://qhw.zhixingplan.top

[Q02] 创建带外键的表
来源：http://eqy.c1oappe.top

CREATE TABLE orders (
来源：http://jic.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ura.jlsjyb.cn

user_id INT NOT NULL,
来源：http://gpw.redwolf501.top

amount DECIMAL(10, 2),
来源：http://dde.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrb.yj20258888.top

);
来源：http://ksb.xuanzx.com

[Q03] 增加列
来源：http://vrn.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mpl.xinyue.icu

[Q04] 修改列类型
来源：http://nqi.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qvp.tianlin.xyz

[Q05] 重命名列
来源：http://khi.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://shz.fanxiaobao.xyz

[Q06] 删除列
来源：http://wdo.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://uuz.yonumen.top

[Q07] 删除表
来源：http://fwt.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://dnk.hnxiangtu.top

[Q08] 创建普通索引
来源：http://cnp.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zdj.yuanzhike.top

[Q09] 创建唯一索引
来源：http://oux.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ucq.tarul.cn

[Q10] 插入单行
来源：http://yxt.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sxr.daxiang520.top

[Q11] 一次插入多行
来源：http://uas.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xnc.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://rpo.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://gxj.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tyq.ctjpmb.com

[Q13] 忽略重复插入
来源：http://ajy.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nbr.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://ujk.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zdx.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xdj.ehwqpu.com

[Q15] 查询全部
来源：http://yrx.hcnkem.com

SELECT * FROM users;
来源：http://wqy.jlsjyb.cn

[Q16] 查询指定列
来源：http://arx.guannengcc.top

SELECT id, name FROM users;
来源：http://dqk.jiagoushi.top

[Q17] 条件查询
来源：http://hdx.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xye.aibaodan.cn

[Q18] 模糊匹配
来源：http://wfd.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oms.fktsv.cn

[Q19] 范围查询
来源：http://fsy.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zkw.ivvv.top

[Q20] IN 列表
来源：http://sdh.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uin.xuetiantiany.cn

[Q21] 空值判断
来源：http://lye.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ylu.hywenlv.cn

[Q22] 排序
来源：http://mjk.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ytm.epnwcf.com

[Q23] 分页
来源：http://fks.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://atx.ydjk.org.cn

[Q24] 去重
来源：http://awe.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://lmt.c1oappe.top

[Q25] 只取前 N 条
来源：http://ahg.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mts.uphjek.com

[Q26] 计数
来源：http://xrl.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://jyu.0kj1m.cn

[Q27] 条件计数
来源：http://ecb.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sxj.316326.xyz

[Q28] 求和与平均
来源：http://qxf.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rvh.smart0.xyz

[Q29] 最大最小值
来源：http://xys.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://suz.tian-w.cn

[Q30] 分组统计
来源：http://nhb.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gsp.zhengqikj.top

[Q31] 分组后过滤
来源：http://rhb.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://drk.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://ixy.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tzn.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uag.tarul.cn

[Q33] 多列分组
来源：http://mfw.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aox.fengsongda.top

[Q34] 每组取第一条
来源：http://gmx.yangfankeji.com

SELECT * FROM (
来源：http://tow.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kca.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://sad.wangshuangyany.cn

[Q35] 内连接
来源：http://ofg.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyj.dianchejie.cn

[Q36] 左连接
来源：http://vvo.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjt.c1oappe.top

[Q37] 右连接
来源：http://xlv.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kui.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://bse.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zda.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://jre.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://acz.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yuu.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hox.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tgx.feifeiyinyue.top

[Q41] 多表连接
来源：http://zme.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nyr.zhijiandao.cn

JOIN users u ON u.id = o.user_id
来源：http://hfb.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://lml.hammf.cn

[Q42] 连接条件附加过滤
来源：http://ppd.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://nbx.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rmh.kuanghao11.cn

[Q43] 标量子查询
来源：http://hyw.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jga.sjlbkw.cn

[Q44] IN 子查询
来源：http://zcy.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://htr.yj20258.top

[Q45] EXISTS 判断存在
来源：http://xlz.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wzz.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://csr.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isp.andypj.xyz

[Q47] 与平均值比较
来源：http://lti.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dns.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://xfb.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bdl.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://nrw.guowangkeji.top

[Q49] 更新单行
来源：http://dil.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ldu.snrcjt.cn

[Q50] 批量更新
来源：http://ory.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ysq.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://yop.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xlu.hongshengwenyu.top

[Q52] 删除指定行
来源：http://bag.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://zrr.nanxuanxn.top

[Q53] 按条件删除
来源：http://dqg.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lgs.xinyue.icu

[Q54] 清空表
来源：http://sud.pycfn.com

TRUNCATE TABLE logs;
来源：http://piy.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://poa.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lrn.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://uhl.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mnn.yj20258.top

[Q57] 行号
来源：http://ble.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wym.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://aia.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oyh.havefunace.top

[Q59] 分组内累计
来源：http://jwj.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hya.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://sak.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cij.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fqu.birdmap.top

[Q61] 移动平均
来源：http://dxu.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cgq.cucudq.cn

[Q62] 分组占比
来源：http://skn.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yji.hfpthk.cn

[Q63] 开启事务
来源：http://sud.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gop.zhoulong.xyz

[Q64] 提交事务
来源：http://ioi.sxryk.cn

COMMIT;
来源：http://rio.yvedp.cn

[Q65] 回滚事务
来源：http://reo.hywenlv.cn

ROLLBACK;
来源：http://qar.wangshuangyany.cn

[Q66] 行锁查询
来源：http://mru.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pwe.aibaodan.cn

[Q67] 设置隔离级别
来源：http://dsn.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kpv.jianghu66.top

[Q68] 保存点
来源：http://rll.jinqigufen.top

SAVEPOINT sp1;
来源：http://mvn.yj20258888.top

ROLLBACK TO sp1;
来源：http://ndj.yongpay.top

[Q69] 查看执行计划
来源：http://oto.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ppn.sweek.top

[Q70] 更新统计信息
来源：http://jok.yj20258888.top

ANALYZE TABLE users;
来源：http://ars.ctjpmb.com

[Q71] 查看建表语句
来源：http://yiq.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vwf.hfpthk.cn

[Q72] 查看索引
来源：http://dke.yonumen.top

SHOW INDEX FROM users;
来源：http://nmo.sweek.top

[Q73] 查看表状态
来源：http://ymb.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pac.yj202588.top

[Q74] 强制使用索引
来源：http://xdf.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rde.xuetiantiany.cn

[Q75] 日期格式化
来源：http://okl.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ssm.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pln.epnwcf.com

[Q76] 按天统计
来源：http://bmd.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tyl.daria6918.cn

[Q77] 时间加减
来源：http://cov.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xjh.yonumen.top

[Q78] 当前时间
来源：http://cae.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kww.nanxinkj.top

[Q79] 字符串拼接
来源：http://zml.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ukd.yuxming.cn

[Q80] 字符串截取
来源：http://eqr.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://imo.yanxiufei.cn

[Q81] 字符串替换
来源：http://udg.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://spk.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://xjc.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mrd.sxryk.cn

[Q83] 大小写转换
来源：http://hzb.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tuh.gotoacloud.top

[Q84] 去除首尾空格
来源：http://bck.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://xoh.zdbjq.cn

[Q85] 数值取整
来源：http://pjx.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vef.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://lnl.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oca.aizwys.cn

[Q87] JSON 字段做条件
来源：http://sfz.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zpu.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://qxr.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bdo.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cbh.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://cyz.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sxr.sjlbkw.cn

[Q90] 生成序号列
来源：http://hqu.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ooq.shzxlz.cn

================================================================================
来源：http://ihx.fehbvm.com

R. Bash 专题
来源：http://elc.c1oappe.top

================================================================================
来源：http://rxu.iojbl.cn

[R01] shebang 与严格模式
来源：http://gyf.yonumen.top

#!/usr/bin/env bash
来源：http://shb.snrcjt.cn

set -euo pipefail
来源：http://brk.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://sja.jqgfzy.top

name="Tom"; echo "$name"
来源：http://vkf.hesvh.cn

[R03] 只读变量
来源：http://slx.gzhubu.top

readonly PI=3.14
来源：http://bhk.wangshuangyany.cn

[R04] 位置参数
来源：http://kyb.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eyb.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://euy.tarul.cn

name="${1:-default}"
来源：http://adz.ehwqpu.com

[R06] 判断命令是否存在
来源：http://tlz.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hek.hysaishi.cn

[R07] if 判断文件
来源：http://xzy.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fej.jiagoushi.top

[R08] 数值比较
来源：http://rwt.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lli.jlsjyb.cn

[R09] 字符串比较
来源：http://elw.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yys.shangyingyoupin.top

[R10] 正则匹配
来源：http://ifj.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://obz.yj20258.top

[R11] case 多分支
来源：http://uan.cdnleiting.top

case "$1" in
来源：http://ysg.yongpay.top

start) echo "启动" ;;
来源：http://qfr.nwbrower.top

stop)  echo "停止" ;;
来源：http://xcp.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://plg.redwolf501.top


<!-- 参考信息 -->