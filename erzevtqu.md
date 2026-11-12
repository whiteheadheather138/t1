代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gkp.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tro.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bgg.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mcr.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmg.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pgw.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ssd.smart0.xyz

[P04] 求长度
来源：http://rbg.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffz.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nun.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxs.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nep.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://flq.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://soq.yueranfly.top

Ruby: x.length;  x.size
来源：http://xiy.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xbo.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://vga.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://whp.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hvo.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fvv.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jzg.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zjh.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zvb.wangdashe.top

Ruby: a == b
来源：http://fpy.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nyp.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lwp.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://emv.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://yrk.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gie.quarkkingdee.top

TS:   if (x == null) {}
来源：http://rqj.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ghf.pycfn.com

Go:   if x == nil {}
来源：http://hms.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xpk.316326.xyz

C#:   if (x is null) {}
来源：http://bou.hnxiangtu.top

[P07] 防抖与节流
来源：http://mpn.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dzm.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://qqo.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yfl.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wok.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xpy.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dgd.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wmn.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pzq.fehbvm.com

[P08] 处理浮点精度问题
来源：http://tew.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rof.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qgc.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hlu.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cre.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dib.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dlu.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lko.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rxg.daria6918.cn

================================================================================
来源：http://dnn.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zvm.hnqzz.top

================================================================================
来源：http://ial.ppjwa.cn

[Q01] 创建表
来源：http://hvn.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://uld.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqz.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://gwn.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://erl.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://spk.xziqi.cn

);
来源：http://qqq.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://gyb.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://ekg.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hop.smart0.xyz

user_id INT NOT NULL,
来源：http://ntk.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://kyd.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://drg.yongpay.top

);
来源：http://bmj.birdmap.top

[Q03] 增加列
来源：http://xsc.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://maa.meibo888.top

[Q04] 修改列类型
来源：http://lju.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://usc.c1oappe.top

[Q05] 重命名列
来源：http://jyy.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fba.jianghu66.top

[Q06] 删除列
来源：http://qfk.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vjm.kuanghao11.cn

[Q07] 删除表
来源：http://alo.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://jnk.hfpthk.cn

[Q08] 创建普通索引
来源：http://wis.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nqx.zhixingplan.top

[Q09] 创建唯一索引
来源：http://nfn.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vsr.sufxvd.cn

[Q10] 插入单行
来源：http://zju.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rcc.zycfv.cn

[Q11] 一次插入多行
来源：http://ygl.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ola.yj202588.top

[Q12] 插入后取自增 ID
来源：http://ulk.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://zge.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rwx.cdnleiting.top

[Q13] 忽略重复插入
来源：http://ekp.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dtc.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://uch.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wnh.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bgh.nanxinkj.top

[Q15] 查询全部
来源：http://vbv.guannengcc.top

SELECT * FROM users;
来源：http://lcg.smart0.xyz

[Q16] 查询指定列
来源：http://mqt.chenzaomai.com

SELECT id, name FROM users;
来源：http://zvv.hfpthk.cn

[Q17] 条件查询
来源：http://jeb.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://moa.yanxiufei.cn

[Q18] 模糊匹配
来源：http://ywy.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jaw.yj20258888.top

[Q19] 范围查询
来源：http://uzw.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jlc.zhengqikj.top

[Q20] IN 列表
来源：http://akp.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dwp.yonumen.top

[Q21] 空值判断
来源：http://ihq.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://szr.yanxiufei.cn

[Q22] 排序
来源：http://cwn.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xhy.pycfn.com

[Q23] 分页
来源：http://wen.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://htf.shanyushiyangkeji.top

[Q24] 去重
来源：http://yky.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://fdy.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://yjy.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hje.ctjpmb.com

[Q26] 计数
来源：http://fcx.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://tmy.mhx1999.top

[Q27] 条件计数
来源：http://bxh.cdnleiting.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xsr.sweek.top

[Q28] 求和与平均
来源：http://vfr.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nzn.ydzc1.top

[Q29] 最大最小值
来源：http://gvh.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xbp.c1oappe.top

[Q30] 分组统计
来源：http://gmo.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vvg.jianghu66.top

[Q31] 分组后过滤
来源：http://lfo.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyj.ydzc1.top

[Q32] 分组拼接字符串
来源：http://aef.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qxj.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lya.dashuyun.cn

[Q33] 多列分组
来源：http://nrg.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gwe.guowangkeji.top

[Q34] 每组取第一条
来源：http://rid.zhengqikj.top

SELECT * FROM (
来源：http://ysn.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uiy.ybcxt.top

) t WHERE rn = 1;
来源：http://hkj.jlsjyb.cn

[Q35] 内连接
来源：http://xjq.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pzt.uphjek.com

[Q36] 左连接
来源：http://ypc.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mwb.zhengqikj.top

[Q37] 右连接
来源：http://pew.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uge.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://meg.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hat.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://rec.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fil.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hxc.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ylv.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tdj.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://lss.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lbk.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://iui.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://kse.hammf.cn

[Q42] 连接条件附加过滤
来源：http://ooe.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://eik.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hqk.sjlbkw.cn

[Q43] 标量子查询
来源：http://kra.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://biw.zhongyouzk.top

[Q44] IN 子查询
来源：http://vdx.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftv.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://qeb.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ujn.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://prn.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oqi.daxiang520.top

[Q47] 与平均值比较
来源：http://sdd.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oja.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://try.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://znq.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://ntv.gogol.net.cn

[Q49] 更新单行
来源：http://fae.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pis.fzhhl.top

[Q50] 批量更新
来源：http://qfw.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dfa.0kj1m.cn

[Q51] 用子查询更新
来源：http://pcp.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bdu.sufxvd.cn

[Q52] 删除指定行
来源：http://hsp.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://uhz.gogol.net.cn

[Q53] 按条件删除
来源：http://rda.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qav.nanxuanxn.top

[Q54] 清空表
来源：http://ciz.andypj.xyz

TRUNCATE TABLE logs;
来源：http://mpa.316326.xyz

[Q55] 排名（并列占位）
来源：http://xqc.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fwi.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://aub.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://czi.fehbvm.com

[Q57] 行号
来源：http://obs.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uxz.havefunace.top

[Q58] 累计求和
来源：http://yib.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xuw.cqqwz.cn

[Q59] 分组内累计
来源：http://heg.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cjj.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://ojq.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lwn.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://urj.nwbrower.top

[Q61] 移动平均
来源：http://pno.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fuw.dashuyun.cn

[Q62] 分组占比
来源：http://zwy.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://npl.sufxvd.cn

[Q63] 开启事务
来源：http://wub.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ocq.nwbrower.top

[Q64] 提交事务
来源：http://rts.hysaishi.cn

COMMIT;
来源：http://eal.tanke756.top

[Q65] 回滚事务
来源：http://aob.jqgfzy.top

ROLLBACK;
来源：http://lar.aizwys.cn

[Q66] 行锁查询
来源：http://dvi.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blr.daxiang520.top

[Q67] 设置隔离级别
来源：http://wgk.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oct.9152youxi.cn

[Q68] 保存点
来源：http://jmq.yueranfly.top

SAVEPOINT sp1;
来源：http://mqa.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://oae.zhijiandao.cn

[Q69] 查看执行计划
来源：http://zxb.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zeq.fehbvm.com

[Q70] 更新统计信息
来源：http://htz.sjlbkw.cn

ANALYZE TABLE users;
来源：http://tkh.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://hfu.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://njb.hfpthk.cn

[Q72] 查看索引
来源：http://rui.ywan-chungtsiang.top

SHOW INDEX FROM users;
来源：http://gbl.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://yub.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pkj.zhixingplan.top

[Q74] 强制使用索引
来源：http://iee.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rpi.guannengcc.top

[Q75] 日期格式化
来源：http://txl.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qyp.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eye.hnxiangtu.top

[Q76] 按天统计
来源：http://syy.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ywe.cheryme.top

[Q77] 时间加减
来源：http://hiz.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rhq.yonumen.top

[Q78] 当前时间
来源：http://qrb.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sfb.guannengcc.top

[Q79] 字符串拼接
来源：http://fze.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ugl.c1oappe.top

[Q80] 字符串截取
来源：http://xsn.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jqx.xuetiantiany.cn

[Q81] 字符串替换
来源：http://pgb.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ftk.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://wqp.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qfc.guowangkeji.top

[Q83] 大小写转换
来源：http://swb.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jqs.hfpthk.cn

[Q84] 去除首尾空格
来源：http://xet.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://qok.yangfankeji.com

[Q85] 数值取整
来源：http://mdt.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ohk.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://dyj.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qzu.sysykeji.top

[Q87] JSON 字段做条件
来源：http://awz.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hke.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://jvk.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://irf.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://alt.daxiang520.top

[Q89] 判断表是否存在
来源：http://bsv.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xqg.svipenyu.cn

[Q90] 生成序号列
来源：http://uyy.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fld.cqqwz.cn

================================================================================
来源：http://oae.zhixingplan.top

R. Bash 专题
来源：http://apf.zhongyouzk.top

================================================================================
来源：http://ijt.yangfankeji.com

[R01] shebang 与严格模式
来源：http://ucl.xziqi.cn

#!/usr/bin/env bash
来源：http://gkh.jiagoushi.top

set -euo pipefail
来源：http://sww.zycfv.cn

[R02] 变量赋值与使用
来源：http://obv.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://vlm.yanxiufei.cn

[R03] 只读变量
来源：http://ogv.yueranfly.top

readonly PI=3.14
来源：http://ozx.ppjwa.cn

[R04] 位置参数
来源：http://gcg.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tmw.chenjidiqi.icu

[R05] 参数默认值
来源：http://jsz.jyoumei.cn

name="${1:-default}"
来源：http://ymp.316326.xyz

[R06] 判断命令是否存在
来源：http://jng.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://teb.pengpengdd.cyou

[R07] if 判断文件
来源：http://vjo.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhp.yj202588.top

[R08] 数值比较
来源：http://irk.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gfu.nwbrower.top

[R09] 字符串比较
来源：http://tym.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cca.jianghu66.top

[R10] 正则匹配
来源：http://iov.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ifu.nwbrower.top

[R11] case 多分支
来源：http://ruz.zhaomingkeji.xyz

case "$1" in
来源：http://sgz.sjlbkw.cn

start) echo "启动" ;;
来源：http://aer.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://tgd.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://kwp.xziqi.cn

esac
来源：http://lwm.daria6918.cn

[R12] for 遍历文件
来源：http://zvr.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://gmq.bjfxy.top

[R13] for 计数循环
来源：http://yjv.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://cbc.jlsjyb.cn

[R14] C 风格 for
来源：http://fzb.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlv.yangfankeji.com

[R15] while 逐行读文件
来源：http://jcl.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cxz.hnxiangtu.top

[R16] until 等待条件
来源：http://gbb.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pjn.316326.xyz

[R17] 数组定义与取值
来源：http://lfv.shuidangran.top


<!-- 参考信息 -->