代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xrx.jqgfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ofb.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tnh.hongshengwenyu.top

[P04] 求长度
来源：http://xxr.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xsv.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://msm.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezr.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcf.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://gif.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://pnd.ybcxt.top

Ruby: x.length;  x.size
来源：http://gkr.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fbt.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://nkr.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pun.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aez.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sds.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ndx.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://veq.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mzg.yuxming.cn

Ruby: a == b
来源：http://est.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zfg.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nhc.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uiz.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://dlq.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jbm.c1oappe.top

TS:   if (x == null) {}
来源：http://acr.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://xcv.fengsongda.top

Go:   if x == nil {}
来源：http://rlp.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bmh.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://nog.quarkkingdee.top

[P07] 防抖与节流
来源：http://jga.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vzm.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://dcx.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://chq.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpd.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dmi.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nak.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://grz.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://skn.birdmap.top

[P08] 处理浮点精度问题
来源：http://fix.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fij.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vgj.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yvd.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ntu.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hle.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lzn.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqf.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jfa.nanxinkj.top

================================================================================
来源：http://ptw.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gse.guowangkeji.top

================================================================================
来源：http://nmq.chenlongwang.top

[Q01] 创建表
来源：http://pzv.tanke756.top

CREATE TABLE users (
来源：http://hgp.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oju.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://scc.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://lbl.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oyv.sweek.top

);
来源：http://cax.cucudq.cn

[Q02] 创建带外键的表
来源：http://zfh.nwbrower.top

CREATE TABLE orders (
来源：http://aya.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wjt.shzxlz.cn

user_id INT NOT NULL,
来源：http://qfg.tian-w.cn

amount DECIMAL(10, 2),
来源：http://twn.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pgb.hammf.cn

);
来源：http://xhk.cqqwz.cn

[Q03] 增加列
来源：http://tpb.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vro.vqdsnc.cn

[Q04] 修改列类型
来源：http://uea.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yvj.nanxinkj.top

[Q05] 重命名列
来源：http://pwq.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fxe.shanyushiyangtech.top

[Q06] 删除列
来源：http://vum.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://gul.0kj1m.cn

[Q07] 删除表
来源：http://mhd.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://tdf.tanke756.top

[Q08] 创建普通索引
来源：http://emg.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dug.havefunace.top

[Q09] 创建唯一索引
来源：http://qup.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ick.zhoulong.xyz

[Q10] 插入单行
来源：http://stg.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwf.fehbvm.com

[Q11] 一次插入多行
来源：http://qav.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://svv.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://quo.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://trx.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ioa.nanxinkj.top

[Q13] 忽略重复插入
来源：http://lxq.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jyo.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://thq.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mdk.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mso.quarkkingdee.top

[Q15] 查询全部
来源：http://fxn.cdnleiting.top

SELECT * FROM users;
来源：http://wlv.0kj1m.cn

[Q16] 查询指定列
来源：http://ldq.cucudq.cn

SELECT id, name FROM users;
来源：http://lsg.yonumen.top

[Q17] 条件查询
来源：http://vvj.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vzb.jinqigfzy.top

[Q18] 模糊匹配
来源：http://cim.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://znv.cdnleiting.top

[Q19] 范围查询
来源：http://xwc.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yos.0kj1m.cn

[Q20] IN 列表
来源：http://hcn.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://clc.guowangkeji.top

[Q21] 空值判断
来源：http://dsk.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://xvx.yonumen.top

[Q22] 排序
来源：http://blq.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvk.fzhhl.top

[Q23] 分页
来源：http://bpm.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://whh.fzhhl.top

[Q24] 去重
来源：http://ewb.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://vod.zdqjudy.top

[Q25] 只取前 N 条
来源：http://vij.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pra.hcnkem.com

[Q26] 计数
来源：http://and.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://irh.andypj.xyz

[Q27] 条件计数
来源：http://mbi.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://juj.ydzc1.top

[Q28] 求和与平均
来源：http://cfh.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://prt.yueranfly.top

[Q29] 最大最小值
来源：http://ahv.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://skw.jianghu66.top

[Q30] 分组统计
来源：http://qrn.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bqx.chenzaomai.com

[Q31] 分组后过滤
来源：http://dlo.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://azg.hammf.cn

[Q32] 分组拼接字符串
来源：http://ute.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fag.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oyt.shangyingyoupin.top

[Q33] 多列分组
来源：http://fyr.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dwk.zhongyouzk.top

[Q34] 每组取第一条
来源：http://pfz.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://tym.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vey.9152youxi.cn

) t WHERE rn = 1;
来源：http://eyb.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://pzl.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://osd.shzxlz.cn

[Q36] 左连接
来源：http://lcp.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cza.nanxinkj.top

[Q37] 右连接
来源：http://omd.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tng.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://zfg.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rxa.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://jep.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wef.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vgp.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aoz.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ial.zhongyouzk.top

[Q41] 多表连接
来源：http://hkw.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jsk.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://dde.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://pfm.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://bdz.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://wlk.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jsl.guannengcc.top

[Q43] 标量子查询
来源：http://tox.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fnq.cucudq.cn

[Q44] IN 子查询
来源：http://fwy.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahx.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://bxi.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nvz.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rfu.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://err.daria6918.cn

[Q47] 与平均值比较
来源：http://tbb.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zkv.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://zad.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://psi.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://ycn.daxiang520.top

[Q49] 更新单行
来源：http://jlw.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fjv.tarul.cn

[Q50] 批量更新
来源：http://hcg.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xbs.yangfankeji.com

[Q51] 用子查询更新
来源：http://zne.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://opz.andypj.xyz

[Q52] 删除指定行
来源：http://rig.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://kdg.xuetiantiany.cn

[Q53] 按条件删除
来源：http://tgf.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ggm.vehdjk.com

[Q54] 清空表
来源：http://dzu.hesvh.cn

TRUNCATE TABLE logs;
来源：http://esg.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://vfq.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nmk.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://hfc.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lvw.gaohongyu789.top

[Q57] 行号
来源：http://zmi.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fhk.hnqzz.top

[Q58] 累计求和
来源：http://goi.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jdn.jqgfzy.top

[Q59] 分组内累计
来源：http://mae.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lek.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://zkb.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vhh.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ufz.hesvh.cn

[Q61] 移动平均
来源：http://xmb.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://afs.nwbrower.top

[Q62] 分组占比
来源：http://mqg.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cun.gotoacloud.top

[Q63] 开启事务
来源：http://iil.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ntq.9152youxi.cn

[Q64] 提交事务
来源：http://cpi.ctjpmb.com

COMMIT;
来源：http://uwq.hnxiangtu.top

[Q65] 回滚事务
来源：http://reh.jinyuanbaomall.cn

ROLLBACK;
来源：http://kkk.hysaishi.cn

[Q66] 行锁查询
来源：http://vty.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://meq.iojbl.cn

[Q67] 设置隔离级别
来源：http://yre.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nfz.nanxinkj.top

[Q68] 保存点
来源：http://ust.xziqi.cn

SAVEPOINT sp1;
来源：http://xwj.nwbrower.top

ROLLBACK TO sp1;
来源：http://iag.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://bqw.yj20258.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xyq.ydjk.org.cn

[Q70] 更新统计信息
来源：http://kyb.havefunace.top

ANALYZE TABLE users;
来源：http://xaf.quarkkingdee.top

[Q71] 查看建表语句
来源：http://umg.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iqi.fzhhl.top

[Q72] 查看索引
来源：http://cub.ivvv.top

SHOW INDEX FROM users;
来源：http://ydw.xylfe.cn

[Q73] 查看表状态
来源：http://jlc.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://fni.sufxvd.cn

[Q74] 强制使用索引
来源：http://ocs.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qar.meibo888.top

[Q75] 日期格式化
来源：http://lks.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lsb.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tkm.zycfv.cn

[Q76] 按天统计
来源：http://cfq.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dct.sysykeji.top

[Q77] 时间加减
来源：http://klv.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppw.yj20258888.top

[Q78] 当前时间
来源：http://hrx.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lei.sufxvd.cn

[Q79] 字符串拼接
来源：http://fnr.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mgv.wangshuangyany.cn

[Q80] 字符串截取
来源：http://exz.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mwf.jqgufenzy.top

[Q81] 字符串替换
来源：http://cmy.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fby.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://umq.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cti.zhixingplan.top

[Q83] 大小写转换
来源：http://zxm.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://idl.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://xrf.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://afb.ehwqpu.com

[Q85] 数值取整
来源：http://pie.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nhr.yonumen.top

[Q86] 读取 JSON 字段
来源：http://aqt.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ipg.tanke756.top

[Q87] JSON 字段做条件
来源：http://chj.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://spk.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://rhp.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iuk.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tan.zdqjudy.top

[Q89] 判断表是否存在
来源：http://bdi.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pwa.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://ace.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kec.smart0.xyz

================================================================================
来源：http://tkr.xuanzx.com

R. Bash 专题
来源：http://zxt.yvedp.cn

================================================================================
来源：http://zxr.havefunace.top

[R01] shebang 与严格模式
来源：http://nuu.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://mwy.quarkkingdee.top

set -euo pipefail
来源：http://uif.ppjwa.cn

[R02] 变量赋值与使用
来源：http://gvs.zdbjq.cn

name="Tom"; echo "$name"
来源：http://xug.cdnleiting.top

[R03] 只读变量
来源：http://hty.0kj1m.cn

readonly PI=3.14
来源：http://sfy.sxryk.cn

[R04] 位置参数
来源：http://zqp.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ati.fehbvm.com

[R05] 参数默认值
来源：http://yta.jqgfzy.top

name="${1:-default}"
来源：http://otd.epnwcf.com

[R06] 判断命令是否存在
来源：http://fwh.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cco.chenjidiqi.icu

[R07] if 判断文件
来源：http://myv.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xdb.dianchejie.cn

[R08] 数值比较
来源：http://giw.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mqt.epnwcf.com

[R09] 字符串比较
来源：http://gfa.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pme.daria6918.cn

[R10] 正则匹配
来源：http://tex.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rxe.yanxiufei.cn

[R11] case 多分支
来源：http://ghw.sufxvd.cn

case "$1" in
来源：http://iev.ppjwa.cn

start) echo "启动" ;;
来源：http://hms.mhx1999.top

stop)  echo "停止" ;;
来源：http://wmz.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://qxr.xuetiantiany.cn

esac
来源：http://ihd.mhx1999.top

[R12] for 遍历文件
来源：http://vwp.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://bbq.chenjidiqi.icu

[R13] for 计数循环
来源：http://qec.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://isj.svipenyu.cn

[R14] C 风格 for
来源：http://ywg.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ekq.yvedp.cn

[R15] while 逐行读文件
来源：http://uhz.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xgf.9152youxi.cn

[R16] until 等待条件
来源：http://ejn.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yke.tanke756.top

[R17] 数组定义与取值
来源：http://iha.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://tps.ybcxt.top

[R18] 遍历数组
来源：http://fvt.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fet.jianghu66.top

[R19] 数组长度
来源：http://vcu.shangyingyoupin.top


<!-- 参考信息 -->