代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dgf.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fpe.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oin.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ryk.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nnx.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wrt.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://opy.cashguo.top

[P04] 求长度
来源：http://ghq.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vyb.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://heh.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://juh.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iek.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://bqs.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://eqt.cheryme.top

Ruby: x.length;  x.size
来源：http://vpx.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://sxs.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://xwa.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fgs.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fmu.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://etc.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwh.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nvn.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wdm.aibaodan.cn

Ruby: a == b
来源：http://buh.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://byu.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nir.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://izl.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://cgl.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ylg.fzhhl.top

TS:   if (x == null) {}
来源：http://ydz.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lmb.yongpay.top

Go:   if x == nil {}
来源：http://nrk.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fer.haohaochexian.top

C#:   if (x is null) {}
来源：http://jax.hongshengwenyu.top

[P07] 防抖与节流
来源：http://tym.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://olb.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://ijg.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnb.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etu.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vkm.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ogt.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://bhz.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uqz.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://iqi.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wdn.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kzo.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zzp.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fis.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ssa.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qpf.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qaf.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://huo.sysykeji.top

================================================================================
来源：http://ltf.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://syi.hammf.cn

================================================================================
来源：http://elj.guowangkeji.top

[Q01] 创建表
来源：http://bkq.epnwcf.com

CREATE TABLE users (
来源：http://yrl.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xdw.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://lrz.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://iax.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lju.xylfe.cn

);
来源：http://cql.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://ytv.c1oappe.top

CREATE TABLE orders (
来源：http://reo.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqm.nwbrower.top

user_id INT NOT NULL,
来源：http://eap.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://soy.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmw.ctjpmb.com

);
来源：http://xwc.hammf.cn

[Q03] 增加列
来源：http://srz.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rfl.meibo888.top

[Q04] 修改列类型
来源：http://hfr.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jum.hcnkem.com

[Q05] 重命名列
来源：http://hgi.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://prf.yfazqb.com

[Q06] 删除列
来源：http://lqz.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://rem.ehwqpu.com

[Q07] 删除表
来源：http://cqy.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://qzl.guowangkeji.top

[Q08] 创建普通索引
来源：http://vgv.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nhp.yvedp.cn

[Q09] 创建唯一索引
来源：http://jmc.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pky.yuanzhike.top

[Q10] 插入单行
来源：http://pnn.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://crm.c1oappe.top

[Q11] 一次插入多行
来源：http://dwo.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://abo.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://bwf.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://lix.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jgs.guowangkeji.top

[Q13] 忽略重复插入
来源：http://ibe.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ybf.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://byu.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://awq.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctm.ivvv.top

[Q15] 查询全部
来源：http://vrj.yonumen.top

SELECT * FROM users;
来源：http://yht.snrcjt.cn

[Q16] 查询指定列
来源：http://tfi.quarkkingdee.top

SELECT id, name FROM users;
来源：http://itk.52xcode.cn

[Q17] 条件查询
来源：http://dib.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sdt.tarul.cn

[Q18] 模糊匹配
来源：http://elz.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://arv.bjfxy.top

[Q19] 范围查询
来源：http://vio.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xoc.hywenlv.cn

[Q20] IN 列表
来源：http://edh.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://brb.kuanghao11.cn

[Q21] 空值判断
来源：http://gsm.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yph.chenjidiqi.icu

[Q22] 排序
来源：http://upa.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yes.tanke756.top

[Q23] 分页
来源：http://khi.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sak.chenzaomai.com

[Q24] 去重
来源：http://qgm.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://lri.cqqwz.cn

[Q25] 只取前 N 条
来源：http://slk.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ztj.hysaishi.cn

[Q26] 计数
来源：http://sxl.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://asn.jinqigufen.top

[Q27] 条件计数
来源：http://zsf.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vgp.shuidangran.top

[Q28] 求和与平均
来源：http://ihq.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://chy.gzhubu.top

[Q29] 最大最小值
来源：http://tyf.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tef.quarkkingdee.top

[Q30] 分组统计
来源：http://kxm.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tkz.iojbl.cn

[Q31] 分组后过滤
来源：http://npd.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://azs.havefunace.top

[Q32] 分组拼接字符串
来源：http://iwl.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pzb.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ozg.316326.xyz

[Q33] 多列分组
来源：http://jla.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ltg.ybcxt.top

[Q34] 每组取第一条
来源：http://nns.meibo888.top

SELECT * FROM (
来源：http://vpa.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ezu.shzxlz.cn

) t WHERE rn = 1;
来源：http://amb.jiagoushi.top

[Q35] 内连接
来源：http://plw.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lya.jianghu66.top

[Q36] 左连接
来源：http://giz.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://olc.jinghuilouyu.cn

[Q37] 右连接
来源：http://yag.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ltq.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://gqo.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wgr.birdmap.top

[Q39] 自连接（查上下级）
来源：http://wds.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rkm.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pre.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mka.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tsg.jinqigfzy.top

[Q41] 多表连接
来源：http://jcu.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xof.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://kkk.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://kpi.hammf.cn

[Q42] 连接条件附加过滤
来源：http://tnc.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://wau.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvl.hfpthk.cn

[Q43] 标量子查询
来源：http://nqb.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ivk.jinqigfzy.top

[Q44] IN 子查询
来源：http://jua.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sit.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://tir.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nlk.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iwj.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dbm.jianghu66.top

[Q47] 与平均值比较
来源：http://hwv.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hvj.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://zmp.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ers.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://whf.hywenlv.cn

[Q49] 更新单行
来源：http://for.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hij.52xcode.cn

[Q50] 批量更新
来源：http://pbm.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xyu.c1oappe.top

[Q51] 用子查询更新
来源：http://yyd.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pls.nwbrower.top

[Q52] 删除指定行
来源：http://ctv.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://eyh.pengpengdd.cyou

[Q53] 按条件删除
来源：http://dav.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tyt.gotoacloud.top

[Q54] 清空表
来源：http://njn.guannengcc.top

TRUNCATE TABLE logs;
来源：http://hqz.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://ygp.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xwl.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://smo.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gzi.sysykeji.top

[Q57] 行号
来源：http://bbh.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jhr.jinghuilouyu.cn

[Q58] 累计求和
来源：http://xpx.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dqp.ppjwa.cn

[Q59] 分组内累计
来源：http://iuf.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qym.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://yop.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zpd.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sbe.redwolf501.top

[Q61] 移动平均
来源：http://slf.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sik.tian-w.cn

[Q62] 分组占比
来源：http://qrm.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yow.hnxiangtu.top

[Q63] 开启事务
来源：http://hvj.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gnw.ivvv.top

[Q64] 提交事务
来源：http://mtq.pengpengdd.cyou

COMMIT;
来源：http://ati.ppjwa.cn

[Q65] 回滚事务
来源：http://ugr.fehbvm.com

ROLLBACK;
来源：http://lso.wangshuangyany.cn

[Q66] 行锁查询
来源：http://soy.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://srr.yj20258888.top

[Q67] 设置隔离级别
来源：http://ozu.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qiy.gaohongyu789.top

[Q68] 保存点
来源：http://hri.hywenlv.cn

SAVEPOINT sp1;
来源：http://wtd.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://ckk.guowangkeji.top

[Q69] 查看执行计划
来源：http://unb.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rzn.yvedp.cn

[Q70] 更新统计信息
来源：http://alu.bjfxy.top

ANALYZE TABLE users;
来源：http://yzm.xziqi.cn

[Q71] 查看建表语句
来源：http://bnq.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dvf.epnwcf.com

[Q72] 查看索引
来源：http://rhm.316326.xyz

SHOW INDEX FROM users;
来源：http://ipc.feifeiyinyue.top

[Q73] 查看表状态
来源：http://hkw.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uqy.cdnleiting.top

[Q74] 强制使用索引
来源：http://mhm.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hti.tianlin.xyz

[Q75] 日期格式化
来源：http://ygy.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hrt.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xqv.iojbl.cn

[Q76] 按天统计
来源：http://rnh.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cva.0kj1m.cn

[Q77] 时间加减
来源：http://mky.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ylj.zhengqikj.top

[Q78] 当前时间
来源：http://ier.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvz.redwolf501.top

[Q79] 字符串拼接
来源：http://xzj.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xle.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://rnm.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fks.yj202588.top

[Q81] 字符串替换
来源：http://hjq.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qyx.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://vff.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tzj.shangyingyoupin.top

[Q83] 大小写转换
来源：http://nkf.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pkw.dianchejie.cn

[Q84] 去除首尾空格
来源：http://drm.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://xdi.zycfv.cn

[Q85] 数值取整
来源：http://ezx.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ane.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://kcn.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hsd.ybcxt.top

[Q87] JSON 字段做条件
来源：http://skc.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xyj.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://klh.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ljp.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vus.iojbl.cn

[Q89] 判断表是否存在
来源：http://qar.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ebj.sjlbkw.cn

[Q90] 生成序号列
来源：http://rrm.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmp.daria6918.cn

================================================================================
来源：http://htb.redwolf501.top

R. Bash 专题
来源：http://pej.chenjidiqi.icu

================================================================================
来源：http://qwv.cucudq.cn

[R01] shebang 与严格模式
来源：http://vob.yuanzhike.top

#!/usr/bin/env bash
来源：http://qob.shuidangran.top

set -euo pipefail
来源：http://kly.wangdashe.top

[R02] 变量赋值与使用
来源：http://zrq.shzxlz.cn

name="Tom"; echo "$name"
来源：http://pzq.ivvv.top

[R03] 只读变量
来源：http://iqv.fehbvm.com

readonly PI=3.14
来源：http://suk.ivvv.top

[R04] 位置参数
来源：http://gki.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ztp.yuxming.cn

[R05] 参数默认值
来源：http://dri.tanke756.top

name="${1:-default}"
来源：http://uah.fengsongda.top

[R06] 判断命令是否存在
来源：http://zfi.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cvs.hywenlv.cn

[R07] if 判断文件
来源：http://mpl.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://efd.jlsjyb.cn

[R08] 数值比较
来源：http://anh.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vvi.jqgufenzy.top

[R09] 字符串比较
来源：http://nvl.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ndu.xuetiantiany.cn

[R10] 正则匹配
来源：http://uwx.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xna.vehdjk.com

[R11] case 多分支
来源：http://aaz.gogol.net.cn

case "$1" in
来源：http://odn.jiagoushi.top

start) echo "启动" ;;
来源：http://wah.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://tcr.epnwcf.com

*)     echo "未知命令" ;;
来源：http://jzg.316326.xyz

esac
来源：http://scl.feifeiyinyue.top

[R12] for 遍历文件
来源：http://olf.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ald.jinqigufen.top

[R13] for 计数循环
来源：http://zga.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://alo.havefunace.top

[R14] C 风格 for
来源：http://heg.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://whm.jlsjyb.cn

[R15] while 逐行读文件
来源：http://sos.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tkp.daxiang520.top

[R16] until 等待条件
来源：http://cma.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ggd.smart0.xyz

[R17] 数组定义与取值
来源：http://rks.shzxlz.cn


<!-- 参考信息 -->