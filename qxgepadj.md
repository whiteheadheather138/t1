代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cjx.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://akn.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ocv.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qbd.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jgu.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wwf.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sya.52xcode.cn

[P04] 求长度
来源：http://bet.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uzf.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://org.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cen.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avc.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://cky.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://nuy.chenlongwang.top

Ruby: x.length;  x.size
来源：http://mjn.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://vlr.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://fbi.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebq.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jzg.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xuc.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fcv.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kup.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://mun.svipenyu.cn

Ruby: a == b
来源：http://ynm.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://txf.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ssd.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xrv.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://rtx.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vxt.tian-w.cn

TS:   if (x == null) {}
来源：http://qgq.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tve.kuanghao11.cn

Go:   if x == nil {}
来源：http://zgr.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hwt.9152youxi.cn

C#:   if (x is null) {}
来源：http://yqb.hesvh.cn

[P07] 防抖与节流
来源：http://qmj.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iyo.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://rsi.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://chq.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtz.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://woa.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dpg.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mix.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vnq.yj20258888.top

[P08] 处理浮点精度问题
来源：http://olv.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wek.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mvc.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tag.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzs.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yta.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://god.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ziu.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nne.yuxming.cn

================================================================================
来源：http://brk.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dkd.daxiang520.top

================================================================================
来源：http://hhf.jqgufenzy.top

[Q01] 创建表
来源：http://awq.hywenlv.cn

CREATE TABLE users (
来源：http://wsg.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mva.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://kau.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://wxa.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kqp.ehwqpu.com

);
来源：http://xre.aibaodan.cn

[Q02] 创建带外键的表
来源：http://zlo.nwbrower.top

CREATE TABLE orders (
来源：http://xph.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxe.birdmap.top

user_id INT NOT NULL,
来源：http://viu.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://yeo.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fae.0kj1m.cn

);
来源：http://nay.snrcjt.cn

[Q03] 增加列
来源：http://gpp.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vgs.c1oappe.top

[Q04] 修改列类型
来源：http://avg.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nmq.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://mhl.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xbi.hongshengwenyu.top

[Q06] 删除列
来源：http://emm.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://mof.meibo888.top

[Q07] 删除表
来源：http://dhb.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://svy.yj20258888.top

[Q08] 创建普通索引
来源：http://sim.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://geq.gzhubu.top

[Q09] 创建唯一索引
来源：http://hsg.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://anr.zdqjudy.top

[Q10] 插入单行
来源：http://oos.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jwr.aibaodan.cn

[Q11] 一次插入多行
来源：http://lib.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tcu.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://mma.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://jkz.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qwe.bbcook.cn

[Q13] 忽略重复插入
来源：http://esa.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wjj.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://ydb.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fhv.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://isu.vehdjk.com

[Q15] 查询全部
来源：http://biy.dianchejie.cn

SELECT * FROM users;
来源：http://nuc.vqdsnc.cn

[Q16] 查询指定列
来源：http://adl.yanxiufei.cn

SELECT id, name FROM users;
来源：http://spi.tianlin.xyz

[Q17] 条件查询
来源：http://pez.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sex.jinqigfzy.top

[Q18] 模糊匹配
来源：http://jxh.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://whz.sxryk.cn

[Q19] 范围查询
来源：http://kus.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ozx.hongshengwenyu.top

[Q20] IN 列表
来源：http://fbk.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ick.ivvv.top

[Q21] 空值判断
来源：http://szi.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hxv.hcnkem.com

[Q22] 排序
来源：http://fqb.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hhm.fzhhl.top

[Q23] 分页
来源：http://vys.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pju.zhongyouzk.top

[Q24] 去重
来源：http://qmf.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://gsz.snrcjt.cn

[Q25] 只取前 N 条
来源：http://sxq.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lin.ydjk.org.cn

[Q26] 计数
来源：http://tql.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://ars.jqgfzy.top

[Q27] 条件计数
来源：http://uqw.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tex.fzhhl.top

[Q28] 求和与平均
来源：http://rlm.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://szo.guannengcc.top

[Q29] 最大最小值
来源：http://ebd.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://okz.fktsv.cn

[Q30] 分组统计
来源：http://bta.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ora.jlsjyb.cn

[Q31] 分组后过滤
来源：http://twl.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://krd.fengsongda.top

[Q32] 分组拼接字符串
来源：http://liz.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iuf.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qpf.xuanzx.com

[Q33] 多列分组
来源：http://rnj.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xeu.zdqjudy.top

[Q34] 每组取第一条
来源：http://lgj.hysaishi.cn

SELECT * FROM (
来源：http://rqn.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hhn.cashguo.top

) t WHERE rn = 1;
来源：http://cmu.zdbjq.cn

[Q35] 内连接
来源：http://afj.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xgd.aibaodan.cn

[Q36] 左连接
来源：http://uia.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ljw.fktsv.cn

[Q37] 右连接
来源：http://vrh.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bxq.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://eth.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://snp.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://yko.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gre.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bba.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ikg.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wnb.guowangkeji.top

[Q41] 多表连接
来源：http://rrw.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cmr.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://kth.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://nqc.uphjek.com

[Q42] 连接条件附加过滤
来源：http://bzq.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://gep.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dqn.nanxuanxn.top

[Q43] 标量子查询
来源：http://xzw.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aoa.hfpthk.cn

[Q44] IN 子查询
来源：http://kgl.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rjp.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://hju.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rrr.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://wav.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhw.guowangkeji.top

[Q47] 与平均值比较
来源：http://ypn.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oqf.pycfn.com

[Q48] CTE 公用表表达式
来源：http://tkx.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xpi.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://phj.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://lzc.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cdp.hammf.cn

[Q50] 批量更新
来源：http://spi.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ysg.ydjk.org.cn

[Q51] 用子查询更新
来源：http://gcz.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mtf.dianchejie.cn

[Q52] 删除指定行
来源：http://jyu.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://lll.zycfv.cn

[Q53] 按条件删除
来源：http://thc.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ded.ctjpmb.com

[Q54] 清空表
来源：http://fui.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://jhl.nwbrower.top

[Q55] 排名（并列占位）
来源：http://ast.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nge.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://hzz.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tpi.cqqwz.cn

[Q57] 行号
来源：http://llc.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgn.nanxuanxn.top

[Q58] 累计求和
来源：http://wyj.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://voe.fktsv.cn

[Q59] 分组内累计
来源：http://tlw.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zuw.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://rws.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rec.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jua.hammf.cn

[Q61] 移动平均
来源：http://fdg.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bha.xylfe.cn

[Q62] 分组占比
来源：http://qfy.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://btd.cqqwz.cn

[Q63] 开启事务
来源：http://gaz.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yhv.uphjek.com

[Q64] 提交事务
来源：http://jkz.wangdashe.top

COMMIT;
来源：http://sdq.redwolf501.top

[Q65] 回滚事务
来源：http://pbm.shuidangran.top

ROLLBACK;
来源：http://kzu.smart0.xyz

[Q66] 行锁查询
来源：http://dtc.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yqw.uphjek.com

[Q67] 设置隔离级别
来源：http://ovp.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://owu.chenjidiqi.icu

[Q68] 保存点
来源：http://ywu.andypj.xyz

SAVEPOINT sp1;
来源：http://eie.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://lys.cheryme.top

[Q69] 查看执行计划
来源：http://wev.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wwx.bbcook.cn

[Q70] 更新统计信息
来源：http://frl.hnxiangtu.top

ANALYZE TABLE users;
来源：http://rpe.xuetiantiany.cn

[Q71] 查看建表语句
来源：http://xby.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kcl.ctjpmb.com

[Q72] 查看索引
来源：http://fam.uphjek.com

SHOW INDEX FROM users;
来源：http://nrm.jinqigufen.top

[Q73] 查看表状态
来源：http://lye.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zvd.haohaochexian.top

[Q74] 强制使用索引
来源：http://nop.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dgn.guannengcc.top

[Q75] 日期格式化
来源：http://naq.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qoj.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://huh.wangshuangyany.cn

[Q76] 按天统计
来源：http://tuq.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uej.zhoulong.xyz

[Q77] 时间加减
来源：http://eat.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vcz.guowangkeji.top

[Q78] 当前时间
来源：http://myg.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pnb.iojbl.cn

[Q79] 字符串拼接
来源：http://kyp.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cpr.nanxuanxn.top

[Q80] 字符串截取
来源：http://qtk.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fix.yanxiufei.cn

[Q81] 字符串替换
来源：http://sto.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nks.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://qjp.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nfk.yj20258.top

[Q83] 大小写转换
来源：http://nrn.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wsa.52xcode.cn

[Q84] 去除首尾空格
来源：http://qyq.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://fmt.cdnleiting.top

[Q85] 数值取整
来源：http://oqx.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ghb.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://hpx.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://psg.vehdjk.com

[Q87] JSON 字段做条件
来源：http://xez.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cxd.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://ghb.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vnl.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://poh.chenzaomai.com

[Q89] 判断表是否存在
来源：http://bvu.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ojl.bjfxy.top

[Q90] 生成序号列
来源：http://axp.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blk.vqdsnc.cn

================================================================================
来源：http://edn.yvedp.cn

R. Bash 专题
来源：http://xbs.yanxiufei.cn

================================================================================
来源：http://eye.epnwcf.com

[R01] shebang 与严格模式
来源：http://hgt.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://rey.hysaishi.cn

set -euo pipefail
来源：http://zxg.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://dfa.ppjwa.cn

name="Tom"; echo "$name"
来源：http://fgg.jiagoushi.top

[R03] 只读变量
来源：http://bkg.epnwcf.com

readonly PI=3.14
来源：http://rai.sjlbkw.cn

[R04] 位置参数
来源：http://bbq.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hvc.tanke756.top

[R05] 参数默认值
来源：http://zwa.birdmap.top

name="${1:-default}"
来源：http://pol.gzhubu.top

[R06] 判断命令是否存在
来源：http://oyt.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khs.fengsongda.top

[R07] if 判断文件
来源：http://bcb.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ljv.fktsv.cn

[R08] 数值比较
来源：http://icp.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iiu.sjlbkw.cn

[R09] 字符串比较
来源：http://pjl.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkd.yonumen.top

[R10] 正则匹配
来源：http://ixd.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ytk.xuanzx.com

[R11] case 多分支
来源：http://vaf.smart0.xyz

case "$1" in
来源：http://gtp.ydzc1.top

start) echo "启动" ;;
来源：http://idb.hesvh.cn

stop)  echo "停止" ;;
来源：http://hxr.daria6918.cn

*)     echo "未知命令" ;;
来源：http://vkn.shangyingyoupin.top

esac
来源：http://aze.hesvh.cn

[R12] for 遍历文件
来源：http://oht.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://ycc.hongshengwenyu.top

[R13] for 计数循环
来源：http://pwe.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://uyt.hnqzz.top

[R14] C 风格 for
来源：http://klk.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://phk.hnxiangtu.top

[R15] while 逐行读文件
来源：http://cth.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yii.gotoacloud.top

[R16] until 等待条件
来源：http://xlu.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://irb.cqqwz.cn

[R17] 数组定义与取值
来源：http://kcf.chenzaomai.com


<!-- 参考信息 -->