代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hwg.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tnc.cdnleiting.top

[P03] 生成短随机字符串
来源：http://gjc.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tfy.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pvq.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pbf.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bwr.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oag.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nry.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://wkp.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://psj.chenlongwang.top

[P04] 求长度
来源：http://gaz.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://loc.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://acb.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fim.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjx.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://jom.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://ivg.tianlin.xyz

Ruby: x.length;  x.size
来源：http://uad.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kyx.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://sso.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jjc.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wns.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jdj.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wzu.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://trt.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://acq.yanxiufei.cn

Ruby: a == b
来源：http://lmn.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yxd.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xqa.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vkc.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://jew.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvj.jinqigfzy.top

TS:   if (x == null) {}
来源：http://uyg.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://awz.yj202588.top

Go:   if x == nil {}
来源：http://wgg.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pxb.yanxiufei.cn

C#:   if (x is null) {}
来源：http://etq.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://wmh.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ayf.hammf.cn

PHP:  // 手写时间戳比较
来源：http://kpk.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbd.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kzj.aizwys.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oqa.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://osy.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vqs.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pld.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://ggu.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xwe.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xoe.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xqn.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzy.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vjg.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zgn.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrk.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://asf.ivvv.top

================================================================================
来源：http://hsg.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yhy.guowangkeji.top

================================================================================
来源：http://elz.zhaomingkeji.xyz

[Q01] 创建表
来源：http://ymk.cqqwz.cn

CREATE TABLE users (
来源：http://txt.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fav.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://ccb.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://mcb.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cfx.jqgufenzy.top

);
来源：http://kpj.yangfankeji.com

[Q02] 创建带外键的表
来源：http://kqm.sweek.top

CREATE TABLE orders (
来源：http://dqq.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ubm.hfpthk.cn

user_id INT NOT NULL,
来源：http://bdj.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://bfl.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nxz.ydzc1.top

);
来源：http://rfz.yongpay.top

[Q03] 增加列
来源：http://xcl.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ztg.tanke756.top

[Q04] 修改列类型
来源：http://cxh.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yxu.mhx1999.top

[Q05] 重命名列
来源：http://gsd.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ufs.hnqzz.top

[Q06] 删除列
来源：http://jpa.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://mbv.ydzc1.top

[Q07] 删除表
来源：http://fod.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://vzj.snrcjt.cn

[Q08] 创建普通索引
来源：http://mvl.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oxm.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://vvs.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pwf.shuidangran.top

[Q10] 插入单行
来源：http://cot.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zde.vehdjk.com

[Q11] 一次插入多行
来源：http://kou.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cni.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://wrg.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://wmn.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ofr.cheryme.top

[Q13] 忽略重复插入
来源：http://shq.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kcc.yj20258888.top

[Q14] 存在则更新（upsert）
来源：http://pkn.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tzb.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ybq.quarkkingdee.top

[Q15] 查询全部
来源：http://qzg.316326.xyz

SELECT * FROM users;
来源：http://kth.ydjk.org.cn

[Q16] 查询指定列
来源：http://dtr.cheryme.top

SELECT id, name FROM users;
来源：http://fmu.chenlongwang.top

[Q17] 条件查询
来源：http://ptk.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ida.chenlongwang.top

[Q18] 模糊匹配
来源：http://nax.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://afr.yfazqb.com

[Q19] 范围查询
来源：http://ihe.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bqu.yj202588.top

[Q20] IN 列表
来源：http://mbe.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iuy.gzhubu.top

[Q21] 空值判断
来源：http://box.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fds.mhx1999.top

[Q22] 排序
来源：http://iij.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tch.jqgufenzy.top

[Q23] 分页
来源：http://lvd.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kaz.ctjpmb.com

[Q24] 去重
来源：http://yfy.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://gvi.0kj1m.cn

[Q25] 只取前 N 条
来源：http://zde.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fej.shanyushiyangtech.top

[Q26] 计数
来源：http://cea.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://glv.yj20258888.top

[Q27] 条件计数
来源：http://obf.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bjn.jinqigfzy.top

[Q28] 求和与平均
来源：http://iqy.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qmy.ehwqpu.com

[Q29] 最大最小值
来源：http://ktd.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ncw.xuanzx.com

[Q30] 分组统计
来源：http://uon.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zai.ybcxt.top

[Q31] 分组后过滤
来源：http://xxb.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vcc.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://ptb.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fcu.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ndr.pengpengdd.cyou

[Q33] 多列分组
来源：http://ixf.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lbs.xziqi.cn

[Q34] 每组取第一条
来源：http://yaf.yj202588.top

SELECT * FROM (
来源：http://mxv.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jfp.c1oappe.top

) t WHERE rn = 1;
来源：http://lnd.shanyushiyangkeji.top

[Q35] 内连接
来源：http://ngc.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oey.vehdjk.com

[Q36] 左连接
来源：http://ocg.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pze.xziqi.cn

[Q37] 右连接
来源：http://zib.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kml.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zih.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eqy.cheryme.top

[Q39] 自连接（查上下级）
来源：http://lxz.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uzi.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://coq.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kkx.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pml.fanxiaobao.xyz

[Q41] 多表连接
来源：http://fbn.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dor.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://kru.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://wnx.birdmap.top

[Q42] 连接条件附加过滤
来源：http://nyk.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://lhn.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lmm.svipenyu.cn

[Q43] 标量子查询
来源：http://hqc.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xqi.316326.xyz

[Q44] IN 子查询
来源：http://col.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://onl.yonumen.top

[Q45] EXISTS 判断存在
来源：http://ydm.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dgq.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oms.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjs.gaohongyu789.top

[Q47] 与平均值比较
来源：http://sjd.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jbo.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://psy.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ocy.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://mqn.fzhhl.top

[Q49] 更新单行
来源：http://rup.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rib.zhoulong.xyz

[Q50] 批量更新
来源：http://cet.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zoe.uphjek.com

[Q51] 用子查询更新
来源：http://kqy.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nap.aizwys.cn

[Q52] 删除指定行
来源：http://rod.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://ctg.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://ogt.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ncu.jianghu66.top

[Q54] 清空表
来源：http://ppe.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://pok.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://vsu.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xxy.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://dui.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hle.guannengcc.top

[Q57] 行号
来源：http://gio.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qiz.yj20258888.top

[Q58] 累计求和
来源：http://kej.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cxo.shangyingyoupin.top

[Q59] 分组内累计
来源：http://baz.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bre.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://vwq.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hjm.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://anh.zhijiandao.cn

[Q61] 移动平均
来源：http://mwa.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jaa.yuanzhike.top

[Q62] 分组占比
来源：http://vzo.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lkx.tarul.cn

[Q63] 开启事务
来源：http://tch.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zbe.zhiwuduotai.top

[Q64] 提交事务
来源：http://dgi.xinyue.icu

COMMIT;
来源：http://fgd.vehdjk.com

[Q65] 回滚事务
来源：http://vmr.nanxuanxn.top

ROLLBACK;
来源：http://sfp.haohaochexian.top

[Q66] 行锁查询
来源：http://hqb.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://syc.daria6918.cn

[Q67] 设置隔离级别
来源：http://svk.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ltr.shangyingyoupin.top

[Q68] 保存点
来源：http://clf.yj202588.top

SAVEPOINT sp1;
来源：http://ijd.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://oxz.jyoumei.cn

[Q69] 查看执行计划
来源：http://zgg.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://asg.52xcode.cn

[Q70] 更新统计信息
来源：http://yzt.nanxinkj.top

ANALYZE TABLE users;
来源：http://mnd.hnqzz.top

[Q71] 查看建表语句
来源：http://gds.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xio.sxryk.cn

[Q72] 查看索引
来源：http://bhc.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://old.zycfv.cn

[Q73] 查看表状态
来源：http://uci.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ylm.yfazqb.com

[Q74] 强制使用索引
来源：http://nyu.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://elh.hnxiangtu.top

[Q75] 日期格式化
来源：http://pjb.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lkw.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cks.andypj.xyz

[Q76] 按天统计
来源：http://iie.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ngi.shuidangran.top

[Q77] 时间加减
来源：http://wcn.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dev.havefunace.top

[Q78] 当前时间
来源：http://tyt.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://avi.uphjek.com

[Q79] 字符串拼接
来源：http://ycn.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fyo.andypj.xyz

[Q80] 字符串截取
来源：http://wqh.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hih.tian-w.cn

[Q81] 字符串替换
来源：http://wzp.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://odt.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://maa.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gbq.havefunace.top

[Q83] 大小写转换
来源：http://lai.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qqg.svipenyu.cn

[Q84] 去除首尾空格
来源：http://wuv.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://rpz.pycfn.com

[Q85] 数值取整
来源：http://dxj.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qhp.cashguo.top

[Q86] 读取 JSON 字段
来源：http://ucj.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://buf.xinyue.icu

[Q87] JSON 字段做条件
来源：http://day.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wut.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://imp.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bll.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ybg.zdqjudy.top

[Q89] 判断表是否存在
来源：http://zuo.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://npz.ctjpmb.com

[Q90] 生成序号列
来源：http://gtc.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://deq.yuanzhike.top

================================================================================
来源：http://odr.pycfn.com

R. Bash 专题
来源：http://xno.yuxming.cn

================================================================================
来源：http://jgt.pycfn.com

[R01] shebang 与严格模式
来源：http://paa.xuanzx.com

#!/usr/bin/env bash
来源：http://rjf.cucudq.cn

set -euo pipefail
来源：http://udz.zdqjudy.top

[R02] 变量赋值与使用
来源：http://nud.ivvv.top

name="Tom"; echo "$name"
来源：http://uqz.feifeiyinyue.top

[R03] 只读变量
来源：http://xhc.gzhubu.top

readonly PI=3.14
来源：http://ejl.9152youxi.cn

[R04] 位置参数
来源：http://oro.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jvg.jinqigfzy.top

[R05] 参数默认值
来源：http://axy.c1oappe.top

name="${1:-default}"
来源：http://xoz.jinqigufen.top

[R06] 判断命令是否存在
来源：http://awq.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipd.ybcxt.top

[R07] if 判断文件
来源：http://rpk.snrcjt.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qtg.cashguo.top

[R08] 数值比较
来源：http://kdz.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fub.jqgufenzy.top

[R09] 字符串比较
来源：http://wso.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wie.jqgfzy.top

[R10] 正则匹配
来源：http://det.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sah.hesvh.cn

[R11] case 多分支
来源：http://lsv.chenzaomai.com

case "$1" in
来源：http://uxt.hnxiangtu.top

start) echo "启动" ;;
来源：http://twh.ctjpmb.com

stop)  echo "停止" ;;
来源：http://gpu.fzhhl.top

*)     echo "未知命令" ;;
来源：http://stk.meibo888.top

esac
来源：http://wla.jianghu66.top

[R12] for 遍历文件
来源：http://jty.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://mcl.gogol.net.cn

[R13] for 计数循环
来源：http://jqq.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://wmk.yonumen.top

[R14] C 风格 for
来源：http://jeb.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vom.iojbl.cn

[R15] while 逐行读文件
来源：http://qen.zhiwuduotai.top


<!-- 参考信息 -->