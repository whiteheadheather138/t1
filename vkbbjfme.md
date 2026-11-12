代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jwd.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsm.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gab.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gor.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agv.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvr.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qnd.uphjek.com

[P04] 求长度
来源：http://tfk.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pku.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rta.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arn.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyv.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://ate.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://vli.fzhhl.top

Ruby: x.length;  x.size
来源：http://ohj.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://plb.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://kkh.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://del.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xxa.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mbf.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vqs.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://grp.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://xzz.wangdashe.top

Ruby: a == b
来源：http://mmi.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wub.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ggv.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ykd.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://slr.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vro.kuanghao11.cn

TS:   if (x == null) {}
来源：http://fgn.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gpb.shzxlz.cn

Go:   if x == nil {}
来源：http://xjb.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rqp.wangdashe.top

C#:   if (x is null) {}
来源：http://wqn.svipenyu.cn

[P07] 防抖与节流
来源：http://yvc.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ksc.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://vxk.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ivq.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwa.aizwys.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vup.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nwr.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sed.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tjh.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://jsi.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xft.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qun.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fly.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sew.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lme.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hdg.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cyz.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xdy.cqqwz.cn

================================================================================
来源：http://ozw.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kls.shzxlz.cn

================================================================================
来源：http://sfl.tanke756.top

[Q01] 创建表
来源：http://vec.epnwcf.com

CREATE TABLE users (
来源：http://scl.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lme.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://ach.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://eox.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dpt.ivvv.top

);
来源：http://nli.aizwys.cn

[Q02] 创建带外键的表
来源：http://gah.fzhhl.top

CREATE TABLE orders (
来源：http://kjf.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jke.9152youxi.cn

user_id INT NOT NULL,
来源：http://lfv.yfazqb.com

amount DECIMAL(10, 2),
来源：http://vgy.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mel.c1oappe.top

);
来源：http://ptr.kuanghao11.cn

[Q03] 增加列
来源：http://dmh.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vhl.sxryk.cn

[Q04] 修改列类型
来源：http://avv.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uck.wangshuangyany.cn

[Q05] 重命名列
来源：http://ztf.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lfq.guannengcc.top

[Q06] 删除列
来源：http://nms.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://fny.ctjpmb.com

[Q07] 删除表
来源：http://fqc.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://sbk.fehbvm.com

[Q08] 创建普通索引
来源：http://ydg.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xad.yuxming.cn

[Q09] 创建唯一索引
来源：http://byp.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kch.feifeiyinyue.top

[Q10] 插入单行
来源：http://qex.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uel.smart0.xyz

[Q11] 一次插入多行
来源：http://mkw.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://usk.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://uvk.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wld.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pop.hywenlv.cn

[Q13] 忽略重复插入
来源：http://zlc.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ucr.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://iqw.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjw.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lrc.shanyushiyangtech.top

[Q15] 查询全部
来源：http://pnd.smart0.xyz

SELECT * FROM users;
来源：http://ubk.zhiwuduotai.top

[Q16] 查询指定列
来源：http://zve.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://tid.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://xvn.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wrf.jiagoushi.top

[Q18] 模糊匹配
来源：http://yop.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zxp.shanyushiyangtech.top

[Q19] 范围查询
来源：http://tmj.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yza.yj202588.top

[Q20] IN 列表
来源：http://wvz.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://khd.yuanzhike.top

[Q21] 空值判断
来源：http://cop.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mkp.jianghu66.top

[Q22] 排序
来源：http://qmx.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://akf.shuidangran.top

[Q23] 分页
来源：http://vpr.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wfl.zdbjq.cn

[Q24] 去重
来源：http://xqs.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://hqg.tanke756.top

[Q25] 只取前 N 条
来源：http://ind.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hor.yfazqb.com

[Q26] 计数
来源：http://bgv.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://lea.hywenlv.cn

[Q27] 条件计数
来源：http://dvf.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lyh.ehwqpu.com

[Q28] 求和与平均
来源：http://jre.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://edj.ydzc1.top

[Q29] 最大最小值
来源：http://jmy.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mlb.ppjwa.cn

[Q30] 分组统计
来源：http://dub.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iwa.smart0.xyz

[Q31] 分组后过滤
来源：http://vlh.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzu.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://ife.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://exm.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://asi.fengsongda.top

[Q33] 多列分组
来源：http://bjj.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqh.shuidangran.top

[Q34] 每组取第一条
来源：http://uks.sweek.top

SELECT * FROM (
来源：http://cnv.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bsl.hammf.cn

) t WHERE rn = 1;
来源：http://nhl.zhaomingkeji.xyz

[Q35] 内连接
来源：http://gvb.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://trt.jianghu66.top

[Q36] 左连接
来源：http://poe.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xib.zhiwuduotai.top

[Q37] 右连接
来源：http://ujl.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kvg.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://unu.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pps.chenjidiqi.icu

[Q39] 自连接（查上下级）
来源：http://acw.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://wbv.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uap.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://grn.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hmb.shangyingyoupin.top

[Q41] 多表连接
来源：http://eyp.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://otz.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://bnv.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://auk.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://ylz.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://wdf.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ewv.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://gpn.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://udt.nwbrower.top

[Q44] IN 子查询
来源：http://pld.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wyf.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://atd.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iif.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jzz.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyn.xziqi.cn

[Q47] 与平均值比较
来源：http://cxc.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tjr.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://orz.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jpz.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ebo.nanxuanxn.top

[Q49] 更新单行
来源：http://cdy.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tmj.chenjidiqi.icu

[Q50] 批量更新
来源：http://kth.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wag.yfazqb.com

[Q51] 用子查询更新
来源：http://ljq.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://imf.ehwqpu.com

[Q52] 删除指定行
来源：http://cyg.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://tsv.zhoulong.xyz

[Q53] 按条件删除
来源：http://rbr.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://seq.epnwcf.com

[Q54] 清空表
来源：http://vlx.birdmap.top

TRUNCATE TABLE logs;
来源：http://obg.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://jzp.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uxq.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://tkw.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nxk.wangshuangyany.cn

[Q57] 行号
来源：http://qal.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ube.jqgufenzy.top

[Q58] 累计求和
来源：http://zlp.jlsjyb.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://knl.yuanzhike.top

[Q59] 分组内累计
来源：http://zzx.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yvt.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://grq.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ttn.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kty.gotoacloud.top

[Q61] 移动平均
来源：http://pwn.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kzm.yanxiufei.cn

[Q62] 分组占比
来源：http://fow.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://isa.yj202588.top

[Q63] 开启事务
来源：http://avp.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://snf.nanxinkj.top

[Q64] 提交事务
来源：http://wit.cqqwz.cn

COMMIT;
来源：http://ikm.jianghu66.top

[Q65] 回滚事务
来源：http://iii.0kj1m.cn

ROLLBACK;
来源：http://uym.cheryme.top

[Q66] 行锁查询
来源：http://lob.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dyd.zycfv.cn

[Q67] 设置隔离级别
来源：http://ega.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vla.fengsongda.top

[Q68] 保存点
来源：http://jmu.snrcjt.cn

SAVEPOINT sp1;
来源：http://eeb.tianlin.xyz

ROLLBACK TO sp1;
来源：http://cpx.yanxiufei.cn

[Q69] 查看执行计划
来源：http://puw.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yia.hcnkem.com

[Q70] 更新统计信息
来源：http://huv.jinqigufen.top

ANALYZE TABLE users;
来源：http://gym.hnxiangtu.top

[Q71] 查看建表语句
来源：http://dgh.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbx.gzhubu.top

[Q72] 查看索引
来源：http://aji.yj20258888.top

SHOW INDEX FROM users;
来源：http://tzt.mhx1999.top

[Q73] 查看表状态
来源：http://qme.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://imf.yangfankeji.com

[Q74] 强制使用索引
来源：http://chh.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nfg.zhixingplan.top

[Q75] 日期格式化
来源：http://vmt.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ffk.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rcs.gotoacloud.top

[Q76] 按天统计
来源：http://pih.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bcp.wangdashe.top

[Q77] 时间加减
来源：http://qyn.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vzf.shzxlz.cn

[Q78] 当前时间
来源：http://ymp.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mqd.haohaochexian.top

[Q79] 字符串拼接
来源：http://mrf.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dan.nanxuanxn.top

[Q80] 字符串截取
来源：http://blt.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eqp.pycfn.com

[Q81] 字符串替换
来源：http://oeh.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uvz.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://yic.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://acm.shangyingyoupin.top

[Q83] 大小写转换
来源：http://ycy.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bnk.epnwcf.com

[Q84] 去除首尾空格
来源：http://dut.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://mwj.guannengcc.top

[Q85] 数值取整
来源：http://sdg.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://odv.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://uox.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nge.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://yvq.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://weo.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://pvw.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gla.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpi.wangdashe.top

[Q89] 判断表是否存在
来源：http://dpu.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hzm.hnxiangtu.top

[Q90] 生成序号列
来源：http://ctl.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://evo.hongshengwenyu.top

================================================================================
来源：http://rhu.iojbl.cn

R. Bash 专题
来源：http://tkc.zhongyouzk.top

================================================================================
来源：http://rqt.chenlongwang.top

[R01] shebang 与严格模式
来源：http://ldg.0kj1m.cn

#!/usr/bin/env bash
来源：http://xnf.uphjek.com

set -euo pipefail
来源：http://byu.jyoumei.cn

[R02] 变量赋值与使用
来源：http://fge.cashguo.top

name="Tom"; echo "$name"
来源：http://zgg.shanyushiyangkeji.top

[R03] 只读变量
来源：http://avx.ppjwa.cn

readonly PI=3.14
来源：http://auq.cheryme.top

[R04] 位置参数
来源：http://ine.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gng.yongpay.top

[R05] 参数默认值
来源：http://xfj.0kj1m.cn

name="${1:-default}"
来源：http://dxi.tarul.cn

[R06] 判断命令是否存在
来源：http://aba.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zrm.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://pcc.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hur.daxiang520.top

[R08] 数值比较
来源：http://jme.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nog.cdnleiting.top

[R09] 字符串比较
来源：http://stj.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://osl.nanxinkj.top

[R10] 正则匹配
来源：http://iec.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nkq.birdmap.top

[R11] case 多分支
来源：http://zod.hywenlv.cn

case "$1" in
来源：http://jzq.sweek.top

start) echo "启动" ;;
来源：http://irh.tian-w.cn

stop)  echo "停止" ;;
来源：http://ery.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://ioc.andypj.xyz

esac
来源：http://vgc.sufxvd.cn

[R12] for 遍历文件
来源：http://lai.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://cnl.andypj.xyz

[R13] for 计数循环
来源：http://qiw.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://cgf.mhx1999.top

[R14] C 风格 for
来源：http://tay.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yua.guowangkeji.top

[R15] while 逐行读文件
来源：http://vvs.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ukp.daria6918.cn

[R16] until 等待条件
来源：http://rcd.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ihm.bjfxy.top

[R17] 数组定义与取值
来源：http://eqv.kuanghao11.cn


<!-- 参考信息 -->