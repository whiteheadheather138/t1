代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vux.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jlh.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbz.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vuv.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ooy.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eyp.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nnk.zhixingplan.top

[P04] 求长度
来源：http://vlv.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ewd.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ekp.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czd.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://che.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://qog.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://rbb.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://msp.jinghuilouyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fuq.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://aud.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lcs.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nqq.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://huf.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://skd.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bqi.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dbr.nanxinkj.top

Ruby: a == b
来源：http://icn.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rcw.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rhn.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hqa.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://znr.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cny.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://wcr.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xha.quarkkingdee.top

Go:   if x == nil {}
来源：http://xpt.daria6918.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gga.cashguo.top

C#:   if (x is null) {}
来源：http://gku.yuanzhike.top

[P07] 防抖与节流
来源：http://zll.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zzq.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://jsn.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://git.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zeh.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://htx.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lde.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ote.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gfc.gzhubu.top

[P08] 处理浮点精度问题
来源：http://gjd.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ugb.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ara.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ufl.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://any.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iii.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hvv.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://akl.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bwj.fanxiaobao.xyz

================================================================================
来源：http://wof.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nnn.sjlbkw.cn

================================================================================
来源：http://tmg.jinyuanbaomall.cn

[Q01] 创建表
来源：http://liy.c1oappe.top

CREATE TABLE users (
来源：http://ipm.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jam.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://wcv.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://kso.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lnu.gogol.net.cn

);
来源：http://ayn.tarul.cn

[Q02] 创建带外键的表
来源：http://gda.jqgfzy.top

CREATE TABLE orders (
来源：http://wpc.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://acl.gaohongyu789.top

user_id INT NOT NULL,
来源：http://esn.pycfn.com

amount DECIMAL(10, 2),
来源：http://wcl.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://opq.chenlongwang.top

);
来源：http://vzz.bbcook.cn

[Q03] 增加列
来源：http://ggh.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gwz.sweek.top

[Q04] 修改列类型
来源：http://mvv.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iqc.316326.xyz

[Q05] 重命名列
来源：http://zqj.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qpw.0kj1m.cn

[Q06] 删除列
来源：http://gcp.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nmx.316326.xyz

[Q07] 删除表
来源：http://wcr.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://fgs.andypj.xyz

[Q08] 创建普通索引
来源：http://xdv.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qur.yj20258888.top

[Q09] 创建唯一索引
来源：http://pkb.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wcc.zhixingplan.top

[Q10] 插入单行
来源：http://tao.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://huc.jinqigfzy.top

[Q11] 一次插入多行
来源：http://goa.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ubv.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://odt.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qxn.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hsy.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://vcm.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gpi.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://hqh.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dig.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cvx.bbcook.cn

[Q15] 查询全部
来源：http://skp.ppjwa.cn

SELECT * FROM users;
来源：http://gvk.c1oappe.top

[Q16] 查询指定列
来源：http://huu.chenlongwang.top

SELECT id, name FROM users;
来源：http://hkn.mhx1999.top

[Q17] 条件查询
来源：http://ibs.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jki.fktsv.cn

[Q18] 模糊匹配
来源：http://omq.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nbi.yanxiufei.cn

[Q19] 范围查询
来源：http://bkz.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hwm.hcnkem.com

[Q20] IN 列表
来源：http://mgj.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ong.nanxinkj.top

[Q21] 空值判断
来源：http://phl.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mxe.yuxming.cn

[Q22] 排序
来源：http://pcy.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oxm.hesvh.cn

[Q23] 分页
来源：http://eiy.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osq.cqqwz.cn

[Q24] 去重
来源：http://tjk.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://fvp.fktsv.cn

[Q25] 只取前 N 条
来源：http://qar.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ukb.feifeiyinyue.top

[Q26] 计数
来源：http://gvj.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://ddq.gaohongyu789.top

[Q27] 条件计数
来源：http://bnb.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fnx.yj20258.top

[Q28] 求和与平均
来源：http://pxz.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gqd.snrcjt.cn

[Q29] 最大最小值
来源：http://dvv.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gpc.zhiwuduotai.top

[Q30] 分组统计
来源：http://wro.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jhg.c1oappe.top

[Q31] 分组后过滤
来源：http://xdi.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipd.daxiang520.top

[Q32] 分组拼接字符串
来源：http://irc.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rem.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://idi.jiagoushi.top

[Q33] 多列分组
来源：http://gzr.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://reh.iojbl.cn

[Q34] 每组取第一条
来源：http://sjg.cheryme.top

SELECT * FROM (
来源：http://gua.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jrl.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://feq.tarul.cn

[Q35] 内连接
来源：http://ohw.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hsu.zhijiandao.cn

[Q36] 左连接
来源：http://sts.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wfn.jinyuanbaomall.cn

[Q37] 右连接
来源：http://pdb.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfj.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://mbo.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ksy.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://uan.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pbc.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lmf.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vtx.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ncu.pycfn.com

[Q41] 多表连接
来源：http://nby.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://axl.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://xoi.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://ctg.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://bck.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://lda.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pln.pengpengdd.cyou

[Q43] 标量子查询
来源：http://vio.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eds.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://lxc.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zfh.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://bfy.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://toy.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xru.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsc.svipenyu.cn

[Q47] 与平均值比较
来源：http://ppq.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yht.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://ovw.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pda.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://alo.hfpthk.cn

[Q49] 更新单行
来源：http://pkz.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fkj.nwbrower.top

[Q50] 批量更新
来源：http://dza.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lgz.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://bjc.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pvg.mhx1999.top

[Q52] 删除指定行
来源：http://uvs.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://run.meibo888.top

[Q53] 按条件删除
来源：http://auc.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qdp.ivvv.top

[Q54] 清空表
来源：http://jmr.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://fca.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://wst.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dkr.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://zpt.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gfu.jlsjyb.cn

[Q57] 行号
来源：http://nhq.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cxk.epnwcf.com

[Q58] 累计求和
来源：http://yqu.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sec.gotoacloud.top

[Q59] 分组内累计
来源：http://nxa.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ucw.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://iop.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xhc.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qln.xuetiantiany.cn

[Q61] 移动平均
来源：http://qku.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://geo.cashguo.top

[Q62] 分组占比
来源：http://ceb.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xtx.svipenyu.cn

[Q63] 开启事务
来源：http://pvo.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dsc.zhoulong.xyz

[Q64] 提交事务
来源：http://kvf.yj20258888.top

COMMIT;
来源：http://pxx.yfazqb.com

[Q65] 回滚事务
来源：http://cbi.hywenlv.cn

ROLLBACK;
来源：http://aqu.meibo888.top

[Q66] 行锁查询
来源：http://ksd.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nsg.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://jgy.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kna.pycfn.com

[Q68] 保存点
来源：http://hiq.haohaochexian.top

SAVEPOINT sp1;
来源：http://kmx.vehdjk.com

ROLLBACK TO sp1;
来源：http://ljd.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://ukq.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ivg.chenlongwang.top

[Q70] 更新统计信息
来源：http://wxa.hywenlv.cn

ANALYZE TABLE users;
来源：http://ssx.gzhubu.top

[Q71] 查看建表语句
来源：http://paa.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ati.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://whq.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://kul.fehbvm.com

[Q73] 查看表状态
来源：http://zdq.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jfi.sjlbkw.cn

[Q74] 强制使用索引
来源：http://qmi.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fsr.ydjk.org.cn

[Q75] 日期格式化
来源：http://dzg.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://djv.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kvh.yuanzhike.top

[Q76] 按天统计
来源：http://lbc.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyz.feifeiyinyue.top

[Q77] 时间加减
来源：http://wej.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lpi.ivvv.top

[Q78] 当前时间
来源：http://kds.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ocx.yj20258888.top

[Q79] 字符串拼接
来源：http://wum.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://icf.aibaodan.cn

[Q80] 字符串截取
来源：http://jmg.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xkj.cqqwz.cn

[Q81] 字符串替换
来源：http://ynf.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://buu.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://qxj.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sqf.zhixingplan.top

[Q83] 大小写转换
来源：http://bke.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iax.aizwys.cn

[Q84] 去除首尾空格
来源：http://ivl.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://vnt.snrcjt.cn

[Q85] 数值取整
来源：http://yut.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://umj.havefunace.top

[Q86] 读取 JSON 字段
来源：http://jww.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rtk.gzhubu.top

[Q87] JSON 字段做条件
来源：http://kic.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://grq.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://mkb.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://unb.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pre.xylfe.cn

[Q89] 判断表是否存在
来源：http://tiv.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bio.dashuyun.cn

[Q90] 生成序号列
来源：http://cwo.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xir.tarul.cn

================================================================================
来源：http://acr.ydjk.org.cn

R. Bash 专题
来源：http://mye.feifeiyinyue.top

================================================================================
来源：http://yeq.gzhubu.top

[R01] shebang 与严格模式
来源：http://chb.fengsongda.top

#!/usr/bin/env bash
来源：http://oep.sxryk.cn

set -euo pipefail
来源：http://xsa.shzxlz.cn

[R02] 变量赋值与使用
来源：http://tqv.jqgfzy.top

name="Tom"; echo "$name"
来源：http://cas.jiagoushi.top

[R03] 只读变量
来源：http://juv.sysykeji.top

readonly PI=3.14
来源：http://vsn.haohaochexian.top

[R04] 位置参数
来源：http://bjl.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nyy.hysaishi.cn

[R05] 参数默认值
来源：http://lbr.zhijiandao.cn

name="${1:-default}"
来源：http://eos.gotoacloud.top

[R06] 判断命令是否存在
来源：http://vgc.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uws.daria6918.cn

[R07] if 判断文件
来源：http://aem.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gfz.nanxinkj.top

[R08] 数值比较
来源：http://cin.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qcx.snrcjt.cn

[R09] 字符串比较
来源：http://lji.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aty.daxiang520.top

[R10] 正则匹配
来源：http://fsi.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://crs.dianchejie.cn

[R11] case 多分支
来源：http://uhc.jyoumei.cn

case "$1" in
来源：http://age.jyoumei.cn

start) echo "启动" ;;
来源：http://zjn.gogol.net.cn

stop)  echo "停止" ;;
来源：http://qws.iojbl.cn

*)     echo "未知命令" ;;
来源：http://pis.mhx1999.top

esac
来源：http://lcf.tianlin.xyz

[R12] for 遍历文件
来源：http://gdl.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://mtr.tianlin.xyz

[R13] for 计数循环
来源：http://wsr.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://sgm.zhixingplan.top

[R14] C 风格 for
来源：http://xcw.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mor.nwbrower.top

[R15] while 逐行读文件
来源：http://jhz.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://slw.chenzaomai.com

[R16] until 等待条件
来源：http://lyp.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wka.hfpthk.cn

[R17] 数组定义与取值
来源：http://usg.gzhubu.top


<!-- 参考信息 -->