代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vkb.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srh.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyu.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sto.cheryme.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://klu.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://faq.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qdz.haohaochexian.top

[P04] 求长度
来源：http://ntm.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cxf.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lxf.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggs.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sez.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://tdw.daria6918.cn

Go:   len(arr);  len(m)
来源：http://gba.fktsv.cn

Ruby: x.length;  x.size
来源：http://rkb.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://din.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://hze.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jiq.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ear.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://esw.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bvt.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bhh.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ijd.yangfankeji.com

Ruby: a == b
来源：http://yof.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xgk.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xtk.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jbi.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://rsg.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zdx.guannengcc.top

TS:   if (x == null) {}
来源：http://ajm.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fae.vqdsnc.cn

Go:   if x == nil {}
来源：http://cle.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gvg.zhengqikj.top

C#:   if (x is null) {}
来源：http://jnx.tian-w.cn

[P07] 防抖与节流
来源：http://mqk.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sxt.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://hka.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlu.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrd.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ooa.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wpz.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qkh.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hrg.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://pow.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://roo.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iod.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kdo.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lro.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://joq.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fxx.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zxr.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ctg.jinqigufen.top

================================================================================
来源：http://rvo.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cqc.ehwqpu.com

================================================================================
来源：http://aas.daxiang520.top

[Q01] 创建表
来源：http://fud.birdmap.top

CREATE TABLE users (
来源：http://flo.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://khp.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://kdh.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://qzq.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xlg.tian-w.cn

);
来源：http://oxx.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://duc.gzhubu.top

CREATE TABLE orders (
来源：http://dyv.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgl.sweek.top

user_id INT NOT NULL,
来源：http://mpg.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://qki.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fmt.tanke756.top

);
来源：http://exc.tian-w.cn

[Q03] 增加列
来源：http://igd.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cwi.zycfv.cn

[Q04] 修改列类型
来源：http://vit.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ckt.jinghuilouyu.cn

[Q05] 重命名列
来源：http://hig.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vac.gaohongyu789.top

[Q06] 删除列
来源：http://ytl.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xub.pengpengdd.cyou

[Q07] 删除表
来源：http://cxx.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://fmp.chenzaomai.com

[Q08] 创建普通索引
来源：http://djk.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://gzp.jqgfzy.top

[Q09] 创建唯一索引
来源：http://wqb.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vwu.nwbrower.top

[Q10] 插入单行
来源：http://yan.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ejn.xylfe.cn

[Q11] 一次插入多行
来源：http://lgv.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hkm.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://yuk.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://skl.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jwh.yuanzhike.top

[Q13] 忽略重复插入
来源：http://wpx.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zte.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://icr.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgs.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xzv.dianchejie.cn

[Q15] 查询全部
来源：http://cit.vehdjk.com

SELECT * FROM users;
来源：http://wmi.ctjpmb.com

[Q16] 查询指定列
来源：http://bce.yanxiufei.cn

SELECT id, name FROM users;
来源：http://jux.xuetiantiany.cn

[Q17] 条件查询
来源：http://uan.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gsk.snrcjt.cn

[Q18] 模糊匹配
来源：http://lnz.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nuy.zhengqikj.top

[Q19] 范围查询
来源：http://bhf.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://izn.kuanghao11.cn

[Q20] IN 列表
来源：http://hqr.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qaj.yueranfly.top

[Q21] 空值判断
来源：http://zxm.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://old.pycfn.com

[Q22] 排序
来源：http://jdw.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ccr.hnqzz.top

[Q23] 分页
来源：http://cpb.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mmv.shuidangran.top

[Q24] 去重
来源：http://hzu.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://uda.jianghu66.top

[Q25] 只取前 N 条
来源：http://ouy.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nwz.birdmap.top

[Q26] 计数
来源：http://rkc.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://gfq.shangyingyoupin.top

[Q27] 条件计数
来源：http://lyo.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kyb.hysaishi.cn

[Q28] 求和与平均
来源：http://iia.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ssi.hesvh.cn

[Q29] 最大最小值
来源：http://jkp.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tqh.yanxiufei.cn

[Q30] 分组统计
来源：http://fhe.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://svn.gzhubu.top

[Q31] 分组后过滤
来源：http://dof.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wsy.bjfxy.top

[Q32] 分组拼接字符串
来源：http://rmo.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cgq.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tjz.jiagoushi.top

[Q33] 多列分组
来源：http://zgq.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gzz.daria6918.cn

[Q34] 每组取第一条
来源：http://chp.316326.xyz

SELECT * FROM (
来源：http://ldo.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://icj.shuidangran.top

) t WHERE rn = 1;
来源：http://nlk.fzhhl.top

[Q35] 内连接
来源：http://gaz.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bgb.zhaomingkeji.xyz

[Q36] 左连接
来源：http://npi.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://scs.xuetiantiany.cn

[Q37] 右连接
来源：http://nyt.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mvu.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://stc.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fje.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://wuj.shuidangran.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://khd.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gqh.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://nsl.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://edu.hesvh.cn

[Q41] 多表连接
来源：http://rij.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://svi.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://yaa.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://bnl.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://ymu.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://cho.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wey.shuidangran.top

[Q43] 标量子查询
来源：http://mdt.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://urn.redwolf501.top

[Q44] IN 子查询
来源：http://ayz.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ujw.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://ner.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yyj.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://orl.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ohi.svipenyu.cn

[Q47] 与平均值比较
来源：http://mpz.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hbd.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://fji.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hvl.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://uab.fanxiaobao.xyz

[Q49] 更新单行
来源：http://nbz.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tuw.nanxuanxn.top

[Q50] 批量更新
来源：http://dkq.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://awz.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://olr.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://amk.9152youxi.cn

[Q52] 删除指定行
来源：http://ppr.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://lxu.bbcook.cn

[Q53] 按条件删除
来源：http://owi.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uky.jiagoushi.top

[Q54] 清空表
来源：http://zdl.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://ylg.gaohongyu789.top

[Q55] 排名（并列占位）
来源：http://aui.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mjd.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://oke.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://non.sxryk.cn

[Q57] 行号
来源：http://wxv.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ecq.cheryme.top

[Q58] 累计求和
来源：http://uxi.jlsjyb.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iwx.mhx1999.top

[Q59] 分组内累计
来源：http://eoy.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wdh.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://qgb.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cgj.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oqm.tian-w.cn

[Q61] 移动平均
来源：http://ftb.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cit.ctjpmb.com

[Q62] 分组占比
来源：http://cxs.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vik.shzxlz.cn

[Q63] 开启事务
来源：http://qqd.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jzh.yj20258.top

[Q64] 提交事务
来源：http://dae.tian-w.cn

COMMIT;
来源：http://ppl.tarul.cn

[Q65] 回滚事务
来源：http://drr.dianchejie.cn

ROLLBACK;
来源：http://opn.wangdashe.top

[Q66] 行锁查询
来源：http://erf.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dan.jyoumei.cn

[Q67] 设置隔离级别
来源：http://zwu.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tkb.sjlbkw.cn

[Q68] 保存点
来源：http://dcj.yonumen.top

SAVEPOINT sp1;
来源：http://lfh.yj20258888.top

ROLLBACK TO sp1;
来源：http://fmm.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://csw.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lmw.cqqwz.cn

[Q70] 更新统计信息
来源：http://qin.shuidangran.top

ANALYZE TABLE users;
来源：http://fcj.andypj.xyz

[Q71] 查看建表语句
来源：http://pep.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vgk.wangdashe.top

[Q72] 查看索引
来源：http://ivl.hfpthk.cn

SHOW INDEX FROM users;
来源：http://spr.cdnleiting.top

[Q73] 查看表状态
来源：http://xcv.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wsn.0kj1m.cn

[Q74] 强制使用索引
来源：http://zpw.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://klr.ivvv.top

[Q75] 日期格式化
来源：http://tqx.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xwy.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nme.ppjwa.cn

[Q76] 按天统计
来源：http://pcm.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rgn.snrcjt.cn

[Q77] 时间加减
来源：http://ues.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dwg.cucudq.cn

[Q78] 当前时间
来源：http://igk.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kkc.bbcook.cn

[Q79] 字符串拼接
来源：http://koh.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kjd.yj202588.top

[Q80] 字符串截取
来源：http://hwy.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ppm.gotoacloud.top

[Q81] 字符串替换
来源：http://nyh.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mhm.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://eef.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hei.jqgfzy.top

[Q83] 大小写转换
来源：http://szh.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ctp.yongpay.top

[Q84] 去除首尾空格
来源：http://chr.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://xyg.fehbvm.com

[Q85] 数值取整
来源：http://pqb.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yxp.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://ptf.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nzk.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://bbo.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ush.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://kub.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nin.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://spo.yonumen.top

[Q89] 判断表是否存在
来源：http://lru.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zri.ctjpmb.com

[Q90] 生成序号列
来源：http://tgr.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://euq.guannengcc.top

================================================================================
来源：http://obi.ivvv.top

R. Bash 专题
来源：http://ymj.hfpthk.cn

================================================================================
来源：http://kzm.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://eof.ivvv.top

#!/usr/bin/env bash
来源：http://hww.svipenyu.cn

set -euo pipefail
来源：http://twa.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://ccg.hammf.cn

name="Tom"; echo "$name"
来源：http://vhy.shzxlz.cn

[R03] 只读变量
来源：http://mba.meibo888.top

readonly PI=3.14
来源：http://zkf.epnwcf.com

[R04] 位置参数
来源：http://mcf.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ywh.hysaishi.cn

[R05] 参数默认值
来源：http://hsu.tarul.cn

name="${1:-default}"
来源：http://naj.yongpay.top

[R06] 判断命令是否存在
来源：http://jek.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mzw.quarkkingdee.top

[R07] if 判断文件
来源：http://zdi.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://phi.jianghu66.top

[R08] 数值比较
来源：http://qrr.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ghz.guannengcc.top

[R09] 字符串比较
来源：http://uqf.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xcs.sweek.top

[R10] 正则匹配
来源：http://pge.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://awf.ydjk.org.cn

[R11] case 多分支
来源：http://ewc.guowangkeji.top

case "$1" in
来源：http://apn.gogol.net.cn

start) echo "启动" ;;
来源：http://llw.hywenlv.cn

stop)  echo "停止" ;;
来源：http://nfx.xylfe.cn

*)     echo "未知命令" ;;
来源：http://bby.daria6918.cn

esac
来源：http://wlm.tian-w.cn

[R12] for 遍历文件
来源：http://cvg.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://axy.ppjwa.cn

[R13] for 计数循环
来源：http://mdh.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://vzq.yj20258888.top

[R14] C 风格 for
来源：http://kdy.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://shx.nwbrower.top

[R15] while 逐行读文件
来源：http://zeg.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xfq.vqdsnc.cn

[R16] until 等待条件
来源：http://ofv.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sts.quarkkingdee.top

[R17] 数组定义与取值
来源：http://xdg.daria6918.cn


<!-- 参考信息 -->