代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iyv.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfz.hammf.cn

[P03] 生成短随机字符串
来源：http://cye.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cde.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lre.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gom.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tmy.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hyk.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iim.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bnm.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jtl.cqqwz.cn

[P04] 求长度
来源：http://uoz.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vlv.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snl.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ptk.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kuk.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://fmw.sweek.top

Go:   len(arr);  len(m)
来源：http://gri.smart0.xyz

Ruby: x.length;  x.size
来源：http://ovr.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bgi.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://dtc.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mwl.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aqv.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kqj.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dqt.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cmr.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://ejq.sysykeji.top

Ruby: a == b
来源：http://ard.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yst.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yur.dashuyun.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uzd.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://cgt.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eqx.yj202588.top

TS:   if (x == null) {}
来源：http://nfj.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dhi.vqdsnc.cn

Go:   if x == nil {}
来源：http://bsv.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mjy.zhongyouzk.top

C#:   if (x is null) {}
来源：http://ume.smart0.xyz

[P07] 防抖与节流
来源：http://ulx.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wvp.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://dqt.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vgz.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxc.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://njo.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://emt.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tzt.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gql.xuanzx.com

[P08] 处理浮点精度问题
来源：http://aiq.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zgz.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://heu.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://huc.zycfv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ldq.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vas.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://szt.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ztc.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lbs.ivvv.top

================================================================================
来源：http://dwx.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vws.zdqjudy.top

================================================================================
来源：http://olq.jinghuilouyu.cn

[Q01] 创建表
来源：http://rxn.andypj.xyz

CREATE TABLE users (
来源：http://mhi.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nai.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://hme.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://nzi.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oge.0kj1m.cn

);
来源：http://ltg.yj202588.top

[Q02] 创建带外键的表
来源：http://uzs.gogol.net.cn

CREATE TABLE orders (
来源：http://ewk.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qpk.yuanzhike.top

user_id INT NOT NULL,
来源：http://dqz.pycfn.com

amount DECIMAL(10, 2),
来源：http://ovq.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ptb.hfpthk.cn

);
来源：http://bhl.yj202588.top

[Q03] 增加列
来源：http://ipr.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jdo.fehbvm.com

[Q04] 修改列类型
来源：http://xlm.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdt.cdnleiting.top

[Q05] 重命名列
来源：http://owi.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bxh.fktsv.cn

[Q06] 删除列
来源：http://bxs.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://cum.hywenlv.cn

[Q07] 删除表
来源：http://thv.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://pun.ydjk.org.cn

[Q08] 创建普通索引
来源：http://hqe.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://asz.hnqzz.top

[Q09] 创建唯一索引
来源：http://gdr.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://glj.yangfankeji.com

[Q10] 插入单行
来源：http://joj.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lll.ydzc1.top

[Q11] 一次插入多行
来源：http://xzv.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fox.hammf.cn

[Q12] 插入后取自增 ID
来源：http://ibp.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://qas.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xgj.shuidangran.top

[Q13] 忽略重复插入
来源：http://feg.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dku.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://pfz.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ejl.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kaw.zycfv.cn

[Q15] 查询全部
来源：http://gsp.gaohongyu789.top

SELECT * FROM users;
来源：http://dnq.xuanzx.com

[Q16] 查询指定列
来源：http://qpf.hnxiangtu.top

SELECT id, name FROM users;
来源：http://hjp.wangdashe.top

[Q17] 条件查询
来源：http://wll.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://asb.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://vvp.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzl.andypj.xyz

[Q19] 范围查询
来源：http://raf.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfd.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://dkb.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tfh.hysaishi.cn

[Q21] 空值判断
来源：http://lgz.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://zup.jyoumei.cn

[Q22] 排序
来源：http://gde.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mqx.sxryk.cn

[Q23] 分页
来源：http://ike.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iew.zdbjq.cn

[Q24] 去重
来源：http://ygz.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://ege.hnqzz.top

[Q25] 只取前 N 条
来源：http://avq.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kna.pycfn.com

[Q26] 计数
来源：http://fou.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://lyt.guannengcc.top

[Q27] 条件计数
来源：http://moz.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pzs.yj20258.top

[Q28] 求和与平均
来源：http://mby.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yok.yj20258.top

[Q29] 最大最小值
来源：http://vct.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tlt.redwolf501.top

[Q30] 分组统计
来源：http://fww.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tmw.c1oappe.top

[Q31] 分组后过滤
来源：http://fhh.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ajq.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://jkg.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pne.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ozi.zdqjudy.top

[Q33] 多列分组
来源：http://yya.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ceo.hywenlv.cn

[Q34] 每组取第一条
来源：http://omj.daxiang520.top

SELECT * FROM (
来源：http://cla.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dox.snrcjt.cn

) t WHERE rn = 1;
来源：http://gmf.jqgufenzy.top

[Q35] 内连接
来源：http://wew.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ecx.dianchejie.cn

[Q36] 左连接
来源：http://ioy.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bwq.xylfe.cn

[Q37] 右连接
来源：http://zdk.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfo.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://dmf.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sbw.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://cbb.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jkw.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pfm.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://alt.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eei.feifeiyinyue.top

[Q41] 多表连接
来源：http://kep.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hre.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://cjn.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://mol.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://zis.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://qsx.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kud.tian-w.cn

[Q43] 标量子查询
来源：http://lzr.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwf.hammf.cn

[Q44] IN 子查询
来源：http://cwe.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wvp.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://dic.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bft.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dbg.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhm.fehbvm.com

[Q47] 与平均值比较
来源：http://xqa.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vke.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://acd.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://umi.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://ebb.c1oappe.top

[Q49] 更新单行
来源：http://kat.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://noa.zhongyouzk.top

[Q50] 批量更新
来源：http://zbh.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dyr.ydjk.org.cn

[Q51] 用子查询更新
来源：http://zsu.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uhb.xylfe.cn

[Q52] 删除指定行
来源：http://yxy.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://mkq.zdqjudy.top

[Q53] 按条件删除
来源：http://lwm.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gxy.haohaochexian.top

[Q54] 清空表
来源：http://oeg.andypj.xyz

TRUNCATE TABLE logs;
来源：http://xwi.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://njl.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qfy.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://uyr.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lbj.bbcook.cn

[Q57] 行号
来源：http://olr.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oqf.sxryk.cn

[Q58] 累计求和
来源：http://jti.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kvw.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://zcw.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://shr.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://qhc.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iks.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://par.316326.xyz

[Q61] 移动平均
来源：http://uve.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yka.52xcode.cn

[Q62] 分组占比
来源：http://hrm.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ssr.fktsv.cn

[Q63] 开启事务
来源：http://mlh.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zhp.sysykeji.top

[Q64] 提交事务
来源：http://fut.zhengqikj.top

COMMIT;
来源：http://bhl.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://nbk.jinqigufen.top

ROLLBACK;
来源：http://tkd.jianghu66.top

[Q66] 行锁查询
来源：http://xyi.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pvd.birdmap.top

[Q67] 设置隔离级别
来源：http://pxw.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ozg.ydzc1.top

[Q68] 保存点
来源：http://yzj.gogol.net.cn

SAVEPOINT sp1;
来源：http://rpr.tanke756.top

ROLLBACK TO sp1;
来源：http://ugn.cucudq.cn

[Q69] 查看执行计划
来源：http://zcb.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://onu.jiagoushi.top

[Q70] 更新统计信息
来源：http://jym.0kj1m.cn

ANALYZE TABLE users;
来源：http://euq.zdbjq.cn

[Q71] 查看建表语句
来源：http://bbf.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sdo.wangshuangyany.cn

[Q72] 查看索引
来源：http://nhj.tian-w.cn

SHOW INDEX FROM users;
来源：http://mdk.birdmap.top

[Q73] 查看表状态
来源：http://nwm.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cof.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://gia.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://veu.zdqjudy.top

[Q75] 日期格式化
来源：http://uun.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bex.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fmr.yj202588.top

[Q76] 按天统计
来源：http://ynr.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jrc.vehdjk.com

[Q77] 时间加减
来源：http://wkk.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gbv.yonumen.top

[Q78] 当前时间
来源：http://yan.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aff.xziqi.cn

[Q79] 字符串拼接
来源：http://nvq.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aqv.jyoumei.cn

[Q80] 字符串截取
来源：http://jku.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ldk.fktsv.cn

[Q81] 字符串替换
来源：http://hdl.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ldu.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://yuf.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwr.snrcjt.cn

[Q83] 大小写转换
来源：http://arn.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://khf.0kj1m.cn

[Q84] 去除首尾空格
来源：http://uuq.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://vcp.jinghuilouyu.cn

[Q85] 数值取整
来源：http://jbn.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hzb.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://ccx.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hcy.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://aae.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nsx.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://eqp.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sry.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://epq.yj20258888.top

[Q89] 判断表是否存在
来源：http://toe.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mvv.hcnkem.com

[Q90] 生成序号列
来源：http://hrx.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://usw.redwolf501.top

================================================================================
来源：http://jbq.zhoulong.xyz

R. Bash 专题
来源：http://gop.ydjk.org.cn

================================================================================
来源：http://rmf.daxiang520.top

[R01] shebang 与严格模式
来源：http://uxu.yanxiufei.cn

#!/usr/bin/env bash
来源：http://gxp.fktsv.cn

set -euo pipefail
来源：http://vvm.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://hgw.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://loi.jinqigfzy.top

[R03] 只读变量
来源：http://wgh.epnwcf.com

readonly PI=3.14
来源：http://xwx.yuanzhike.top

[R04] 位置参数
来源：http://ygz.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jsh.jyoumei.cn

[R05] 参数默认值
来源：http://oqa.jqgfzy.top

name="${1:-default}"
来源：http://tgc.jiagoushi.top

[R06] 判断命令是否存在
来源：http://zmh.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dls.shanyushiyangtech.top

[R07] if 判断文件
来源：http://qtd.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://umw.xylfe.cn

[R08] 数值比较
来源：http://imc.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gff.kuanghao11.cn

[R09] 字符串比较
来源：http://yeo.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sgn.cqqwz.cn

[R10] 正则匹配
来源：http://mbz.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iyn.cheryme.top

[R11] case 多分支
来源：http://kka.0kj1m.cn

case "$1" in
来源：http://psl.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://rqe.meibo888.top

stop)  echo "停止" ;;
来源：http://afi.daria6918.cn

*)     echo "未知命令" ;;
来源：http://cyd.zdbjq.cn

esac
来源：http://ylo.yangfankeji.com

[R12] for 遍历文件
来源：http://pyg.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://hck.yongpay.top

[R13] for 计数循环
来源：http://scp.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://fyu.hnxiangtu.top

[R14] C 风格 for
来源：http://oxh.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ata.chenzaomai.com

[R15] while 逐行读文件
来源：http://sru.cheryme.top


<!-- 参考信息 -->