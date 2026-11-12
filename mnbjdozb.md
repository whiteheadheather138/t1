代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pkh.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tcb.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bkq.birdmap.top

[P04] 求长度
来源：http://dck.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ctw.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flb.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqw.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://top.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://lgd.ybcxt.top

Go:   len(arr);  len(m)
来源：http://gsk.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://kqj.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbb.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://vbj.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://giy.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rmt.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mdp.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://laf.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mdr.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://zgh.fktsv.cn

Ruby: a == b
来源：http://uhf.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pok.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mgn.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pwk.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://xlc.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aqp.fengsongda.top

TS:   if (x == null) {}
来源：http://vmx.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://njn.zdbjq.cn

Go:   if x == nil {}
来源：http://dkm.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aja.ydjk.org.cn

C#:   if (x is null) {}
来源：http://bra.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://mmh.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lii.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://joj.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsr.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kui.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ugq.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wlt.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iwq.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://azk.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://hyw.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pvo.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gpc.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ous.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jfa.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fzt.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jdk.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqn.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nvy.tian-w.cn

================================================================================
来源：http://ino.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cvx.zdbjq.cn

================================================================================
来源：http://roc.xziqi.cn

[Q01] 创建表
来源：http://gor.kuanghao11.cn

CREATE TABLE users (
来源：http://gcq.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsx.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://hxw.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://gol.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jui.jinyuanbaomall.cn

);
来源：http://ydg.ybcxt.top

[Q02] 创建带外键的表
来源：http://hcl.ehwqpu.com

CREATE TABLE orders (
来源：http://jed.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://paf.chenlongwang.top

user_id INT NOT NULL,
来源：http://tzi.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://ifi.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qof.hesvh.cn

);
来源：http://ofc.hcnkem.com

[Q03] 增加列
来源：http://kcx.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zpr.gzhubu.top

[Q04] 修改列类型
来源：http://yor.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dbe.svipenyu.cn

[Q05] 重命名列
来源：http://spo.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ndk.pycfn.com

[Q06] 删除列
来源：http://ulh.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fqp.tian-w.cn

[Q07] 删除表
来源：http://pni.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://zgj.gaohongyu789.top

[Q08] 创建普通索引
来源：http://aif.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zdu.sysykeji.top

[Q09] 创建唯一索引
来源：http://lgq.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qls.xuetiantiany.cn

[Q10] 插入单行
来源：http://ebg.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ylq.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://opt.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ecv.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://nvh.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://xjs.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mwe.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://byl.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://crb.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://tox.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpd.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xxs.epnwcf.com

[Q15] 查询全部
来源：http://qqx.bbcook.cn

SELECT * FROM users;
来源：http://mij.yfazqb.com

[Q16] 查询指定列
来源：http://eqe.tarul.cn

SELECT id, name FROM users;
来源：http://bqu.zhiwuduotai.top

[Q17] 条件查询
来源：http://oqd.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gdh.tian-w.cn

[Q18] 模糊匹配
来源：http://pvr.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pkt.vehdjk.com

[Q19] 范围查询
来源：http://azo.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://isi.ivvv.top

[Q20] IN 列表
来源：http://ozm.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yww.nanxuanxn.top

[Q21] 空值判断
来源：http://qcd.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fog.kuanghao11.cn

[Q22] 排序
来源：http://krr.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kgu.ydzc1.top

[Q23] 分页
来源：http://huy.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://czs.zhiwuduotai.top

[Q24] 去重
来源：http://udm.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://yvf.epnwcf.com

[Q25] 只取前 N 条
来源：http://vvg.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tai.zhongyouzk.top

[Q26] 计数
来源：http://bly.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://mnh.hammf.cn

[Q27] 条件计数
来源：http://kea.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ise.tian-w.cn

[Q28] 求和与平均
来源：http://xey.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dgy.yj202588.top

[Q29] 最大最小值
来源：http://gej.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jgo.ppjwa.cn

[Q30] 分组统计
来源：http://tlt.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ejb.zhoulong.xyz

[Q31] 分组后过滤
来源：http://btq.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cbc.nwbrower.top

[Q32] 分组拼接字符串
来源：http://zqw.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kgv.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jmq.tian-w.cn

[Q33] 多列分组
来源：http://jpi.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pdz.zdbjq.cn

[Q34] 每组取第一条
来源：http://xql.shangyingyoupin.top

SELECT * FROM (
来源：http://ctw.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mfx.tanke756.top

) t WHERE rn = 1;
来源：http://ubv.ywan-chungtsiang.top

[Q35] 内连接
来源：http://joi.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pin.redwolf501.top

[Q36] 左连接
来源：http://wbz.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kqc.nanxuanxn.top

[Q37] 右连接
来源：http://isz.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rev.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pyh.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://emm.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://pec.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qlz.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nhk.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://rvc.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ddv.ppjwa.cn

[Q41] 多表连接
来源：http://hhh.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dlt.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://pon.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://xko.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://bqd.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://rnx.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mhc.daria6918.cn

[Q43] 标量子查询
来源：http://ltt.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://skp.yj20258.top

[Q44] IN 子查询
来源：http://bhd.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tvq.pycfn.com

[Q45] EXISTS 判断存在
来源：http://zte.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cku.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://bsp.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vdi.guowangkeji.top

[Q47] 与平均值比较
来源：http://fxn.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yyg.tarul.cn

[Q48] CTE 公用表表达式
来源：http://dpp.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qsg.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://cix.vqdsnc.cn

[Q49] 更新单行
来源：http://jeq.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vbl.jinghuilouyu.cn

[Q50] 批量更新
来源：http://ehf.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xrb.yangfankeji.com

[Q51] 用子查询更新
来源：http://oik.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bei.yj202588.top

[Q52] 删除指定行
来源：http://cbi.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://sef.yj20258.top

[Q53] 按条件删除
来源：http://iva.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dni.xylfe.cn

[Q54] 清空表
来源：http://zzk.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://vlt.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://fnd.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cno.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://gki.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eam.cucudq.cn

[Q57] 行号
来源：http://mkw.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jgl.nwbrower.top

[Q58] 累计求和
来源：http://lws.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pfq.yj20258888.top

[Q59] 分组内累计
来源：http://clp.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rtz.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://czp.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ibp.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://deu.fehbvm.com

[Q61] 移动平均
来源：http://kie.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lxi.hfpthk.cn

[Q62] 分组占比
来源：http://vpo.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wtp.dianchejie.cn

[Q63] 开启事务
来源：http://xkm.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mwh.yfazqb.com

[Q64] 提交事务
来源：http://lag.gzhubu.top

COMMIT;
来源：http://cqf.nanxinkj.top

[Q65] 回滚事务
来源：http://vdt.meibo888.top

ROLLBACK;
来源：http://qvc.fengsongda.top

[Q66] 行锁查询
来源：http://ssn.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qfz.wangdashe.top

[Q67] 设置隔离级别
来源：http://ogp.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pbw.cheryme.top

[Q68] 保存点
来源：http://ith.zdbjq.cn

SAVEPOINT sp1;
来源：http://zxb.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://pqm.hcnkem.com

[Q69] 查看执行计划
来源：http://vgs.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uos.ehwqpu.com

[Q70] 更新统计信息
来源：http://ctd.daxiang520.top

ANALYZE TABLE users;
来源：http://cmw.yuxming.cn

[Q71] 查看建表语句
来源：http://ltj.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://app.zhixingplan.top

[Q72] 查看索引
来源：http://fvo.xylfe.cn

SHOW INDEX FROM users;
来源：http://umo.jianghu66.top

[Q73] 查看表状态
来源：http://qky.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://you.quarkkingdee.top

[Q74] 强制使用索引
来源：http://osp.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xym.pycfn.com

[Q75] 日期格式化
来源：http://xbj.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oao.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zuz.chenlongwang.top

[Q76] 按天统计
来源：http://crn.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://smj.zhixingplan.top

[Q77] 时间加减
来源：http://fbo.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lhp.shzxlz.cn

[Q78] 当前时间
来源：http://wsm.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://osy.ivvv.top

[Q79] 字符串拼接
来源：http://rjc.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pgd.xuanzx.com

[Q80] 字符串截取
来源：http://pyb.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pzi.xuetiantiany.cn

[Q81] 字符串替换
来源：http://cmq.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ulf.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://eed.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jqm.guowangkeji.top

[Q83] 大小写转换
来源：http://sqd.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mpl.daxiang520.top

[Q84] 去除首尾空格
来源：http://ggk.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://uer.xuetiantiany.cn

[Q85] 数值取整
来源：http://nlv.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vqk.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://ijy.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xjf.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://qbt.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rbd.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://vyr.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bbk.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aza.wangdashe.top

[Q89] 判断表是否存在
来源：http://rui.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qyd.andypj.xyz

[Q90] 生成序号列
来源：http://qvd.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qfx.316326.xyz

================================================================================
来源：http://eqb.vehdjk.com

R. Bash 专题
来源：http://xwk.jinyuanbaomall.cn

================================================================================
来源：http://qux.yuxming.cn

[R01] shebang 与严格模式
来源：http://tfq.jinqigfzy.top

#!/usr/bin/env bash
来源：http://uab.nanxuanxn.top

set -euo pipefail
来源：http://gzk.sxryk.cn

[R02] 变量赋值与使用
来源：http://kib.aibaodan.cn

name="Tom"; echo "$name"
来源：http://ylq.yonumen.top

[R03] 只读变量
来源：http://bbj.bjfxy.top

readonly PI=3.14
来源：http://nuu.jinyuanbaomall.cn

[R04] 位置参数
来源：http://uai.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cep.yueranfly.top

[R05] 参数默认值
来源：http://lny.9152youxi.cn

name="${1:-default}"
来源：http://yfh.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://dkn.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://trn.wangshuangyany.cn

[R07] if 判断文件
来源：http://myz.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pld.zdbjq.cn

[R08] 数值比较
来源：http://zqx.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ssw.ybcxt.top

[R09] 字符串比较
来源：http://fzu.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvk.ydzc1.top

[R10] 正则匹配
来源：http://zqh.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://auy.ydzc1.top

[R11] case 多分支
来源：http://mys.bbcook.cn

case "$1" in
来源：http://axm.dashuyun.cn

start) echo "启动" ;;
来源：http://lmz.jqgfzy.top

stop)  echo "停止" ;;
来源：http://qqe.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://wig.316326.xyz

esac
来源：http://xzc.shangyingyoupin.top

[R12] for 遍历文件
来源：http://giv.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://sli.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://ogt.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://uxd.yj202588.top

[R14] C 风格 for
来源：http://osi.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mec.jqgfzy.top

[R15] while 逐行读文件
来源：http://jbw.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xak.ppjwa.cn

[R16] until 等待条件
来源：http://inv.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wuc.yuxming.cn

[R17] 数组定义与取值
来源：http://nfp.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://aay.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://kre.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xqa.quarkkingdee.top

[R19] 数组长度
来源：http://vek.quarkkingdee.top


<!-- 参考信息 -->