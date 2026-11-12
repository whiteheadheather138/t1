代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jpb.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://jba.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aqj.gaohongyu789.top

[P04] 求长度
来源：http://umv.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xcb.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ctp.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvw.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xda.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://ksp.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://fho.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://sbj.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fps.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ipf.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://lla.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ktf.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bse.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://djt.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rxw.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://cag.aizwys.cn

Ruby: a == b
来源：http://eif.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vvj.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lqz.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://une.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://fjs.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vxy.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://jvm.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://lke.cucudq.cn

Go:   if x == nil {}
来源：http://bqj.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vmx.zhoulong.xyz

C#:   if (x is null) {}
来源：http://cvl.tianlin.xyz

[P07] 防抖与节流
来源：http://zvw.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://okz.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://vuv.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrk.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xeh.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dhe.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jcd.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bwu.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xwa.havefunace.top

[P08] 处理浮点精度问题
来源：http://rtb.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pgg.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ziq.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ihi.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zhp.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://djy.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eum.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pha.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mcn.zhongyouzk.top

================================================================================
来源：http://byn.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pww.shuidangran.top

================================================================================
来源：http://pmd.ctjpmb.com

[Q01] 创建表
来源：http://omq.guowangkeji.top

CREATE TABLE users (
来源：http://fhs.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fft.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://iap.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://gmv.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kxz.daxiang520.top

);
来源：http://ijs.cdnleiting.top

[Q02] 创建带外键的表
来源：http://dlk.ctjpmb.com

CREATE TABLE orders (
来源：http://mlh.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ucw.jqgfzy.top

user_id INT NOT NULL,
来源：http://akd.tanke756.top

amount DECIMAL(10, 2),
来源：http://qqu.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bci.cdnleiting.top

);
来源：http://bna.jianghu66.top

[Q03] 增加列
来源：http://wke.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qei.jinqigfzy.top

[Q04] 修改列类型
来源：http://nrr.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mdc.shzxlz.cn

[Q05] 重命名列
来源：http://dgy.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lbe.gzhubu.top

[Q06] 删除列
来源：http://bir.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://urw.pycfn.com

[Q07] 删除表
来源：http://reb.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://wyr.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://qra.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bcj.zycfv.cn

[Q09] 创建唯一索引
来源：http://bzb.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aep.hcnkem.com

[Q10] 插入单行
来源：http://xxr.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xlc.birdmap.top

[Q11] 一次插入多行
来源：http://fln.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dwa.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://crs.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oyp.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iel.pycfn.com

[Q13] 忽略重复插入
来源：http://yyd.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://msh.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://iuo.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ebk.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://esv.ivvv.top

[Q15] 查询全部
来源：http://jzm.cashguo.top

SELECT * FROM users;
来源：http://egc.hesvh.cn

[Q16] 查询指定列
来源：http://nlt.hnqzz.top

SELECT id, name FROM users;
来源：http://eqe.zhongyouzk.top

[Q17] 条件查询
来源：http://mzu.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zso.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://byk.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dap.hongshengwenyu.top

[Q19] 范围查询
来源：http://syt.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lrt.meibo888.top

[Q20] IN 列表
来源：http://mgl.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://puk.yvedp.cn

[Q21] 空值判断
来源：http://rti.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://any.tian-w.cn

[Q22] 排序
来源：http://gpt.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kci.tianlin.xyz

[Q23] 分页
来源：http://loy.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xnc.yangfankeji.com

[Q24] 去重
来源：http://gps.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://ndq.aizwys.cn

[Q25] 只取前 N 条
来源：http://woe.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iqk.ivvv.top

[Q26] 计数
来源：http://gbr.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://tpc.ppjwa.cn

[Q27] 条件计数
来源：http://cjb.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mjl.yfazqb.com

[Q28] 求和与平均
来源：http://irf.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://exi.hnxiangtu.top

[Q29] 最大最小值
来源：http://ngp.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fyi.yj202588.top

[Q30] 分组统计
来源：http://btz.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vkg.shuidangran.top

[Q31] 分组后过滤
来源：http://dwp.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ifq.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://mqu.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bnd.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://opx.pengpengdd.cyou

[Q33] 多列分组
来源：http://lqi.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hur.tarul.cn

[Q34] 每组取第一条
来源：http://dfk.shuidangran.top

SELECT * FROM (
来源：http://bfx.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qmn.snrcjt.cn

) t WHERE rn = 1;
来源：http://tan.zdqjudy.top

[Q35] 内连接
来源：http://buy.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://axj.gotoacloud.top

[Q36] 左连接
来源：http://ntw.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kpf.shuidangran.top

[Q37] 右连接
来源：http://oqc.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tdi.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://kih.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rah.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://nho.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qzm.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bhw.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://opy.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fho.yuxming.cn

[Q41] 多表连接
来源：http://qao.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ssj.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://bok.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://usq.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://ipq.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://jtx.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cgt.yj202588.top

[Q43] 标量子查询
来源：http://txi.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://olp.gotoacloud.top

[Q44] IN 子查询
来源：http://pdj.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nhs.yongpay.top

[Q45] EXISTS 判断存在
来源：http://lvx.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bbu.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://doe.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ljo.yuanzhike.top

[Q47] 与平均值比较
来源：http://eyi.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rau.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://gru.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ems.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://ezo.shzxlz.cn

[Q49] 更新单行
来源：http://xmg.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://klo.tarul.cn

[Q50] 批量更新
来源：http://fzp.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qrm.jinqigufen.top

[Q51] 用子查询更新
来源：http://ylb.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hmq.yueranfly.top

[Q52] 删除指定行
来源：http://lmn.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://hcx.wangshuangyany.cn

[Q53] 按条件删除
来源：http://bxx.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dpo.mhx1999.top

[Q54] 清空表
来源：http://pow.yuxming.cn

TRUNCATE TABLE logs;
来源：http://ewq.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://luu.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dqe.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://gpt.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zey.yvedp.cn

[Q57] 行号
来源：http://amn.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgh.9152youxi.cn

[Q58] 累计求和
来源：http://wha.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ziu.ydzc1.top

[Q59] 分组内累计
来源：http://nts.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yht.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://abz.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pac.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mdt.meibo888.top

[Q61] 移动平均
来源：http://ybr.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mmh.yvedp.cn

[Q62] 分组占比
来源：http://kie.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wec.shuidangran.top

[Q63] 开启事务
来源：http://skv.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://alw.sweek.top

[Q64] 提交事务
来源：http://slo.fktsv.cn

COMMIT;
来源：http://gcl.ppjwa.cn

[Q65] 回滚事务
来源：http://aro.birdmap.top

ROLLBACK;
来源：http://xoi.snrcjt.cn

[Q66] 行锁查询
来源：http://kwa.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sue.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://nmk.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ueg.gaohongyu789.top

[Q68] 保存点
来源：http://msl.hesvh.cn

SAVEPOINT sp1;
来源：http://ypo.andypj.xyz

ROLLBACK TO sp1;
来源：http://nqz.yj20258.top

[Q69] 查看执行计划
来源：http://tkt.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rlu.zhoulong.xyz

[Q70] 更新统计信息
来源：http://yaw.vqdsnc.cn

ANALYZE TABLE users;
来源：http://irm.hfpthk.cn

[Q71] 查看建表语句
来源：http://oxx.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kwz.pycfn.com

[Q72] 查看索引
来源：http://nba.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://ssv.0kj1m.cn

[Q73] 查看表状态
来源：http://mvj.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pro.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://rpq.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xvm.birdmap.top

[Q75] 日期格式化
来源：http://ujf.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ynk.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tmg.c1oappe.top

[Q76] 按天统计
来源：http://for.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kve.ivvv.top

[Q77] 时间加减
来源：http://qza.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rpl.sxryk.cn

[Q78] 当前时间
来源：http://phd.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ycd.daria6918.cn

[Q79] 字符串拼接
来源：http://sea.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lgo.yj20258888.top

[Q80] 字符串截取
来源：http://sls.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uev.316326.xyz

[Q81] 字符串替换
来源：http://cqq.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kqr.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://qiy.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kes.hnxiangtu.top

[Q83] 大小写转换
来源：http://utu.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hxr.jianghu66.top

[Q84] 去除首尾空格
来源：http://eeo.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://cac.nanxuanxn.top

[Q85] 数值取整
来源：http://rqr.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bzu.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://zps.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dgo.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://fmj.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wnb.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://vvx.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aru.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xco.guannengcc.top

[Q89] 判断表是否存在
来源：http://rrf.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ydy.jqgufenzy.top

[Q90] 生成序号列
来源：http://oxu.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cco.zhongyouzk.top

================================================================================
来源：http://tjr.hysaishi.cn

R. Bash 专题
来源：http://qpf.daria6918.cn

================================================================================
来源：http://wrf.hnqzz.top

[R01] shebang 与严格模式
来源：http://vrz.chenlongwang.top

#!/usr/bin/env bash
来源：http://yiy.yongpay.top

set -euo pipefail
来源：http://hng.hammf.cn

[R02] 变量赋值与使用
来源：http://ywz.jinqigufen.top

name="Tom"; echo "$name"
来源：http://rya.guowangkeji.top

[R03] 只读变量
来源：http://tmm.zdqjudy.top

readonly PI=3.14
来源：http://ehm.vqdsnc.cn

[R04] 位置参数
来源：http://wod.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvq.jianghu66.top

[R05] 参数默认值
来源：http://ops.xuanzx.com

name="${1:-default}"
来源：http://btf.tanke756.top

[R06] 判断命令是否存在
来源：http://zcy.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uxw.fktsv.cn

[R07] if 判断文件
来源：http://ryu.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jjo.hysaishi.cn

[R08] 数值比较
来源：http://wjf.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://lxb.aizwys.cn

[R09] 字符串比较
来源：http://lqm.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aue.zycfv.cn

[R10] 正则匹配
来源：http://ber.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://umt.ywan-chungtsiang.top

[R11] case 多分支
来源：http://wiv.fengsongda.top

case "$1" in
来源：http://diq.hnqzz.top

start) echo "启动" ;;
来源：http://vfn.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://spr.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://mrq.hnqzz.top

esac
来源：http://buj.nanxuanxn.top

[R12] for 遍历文件
来源：http://idc.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://uhk.sjlbkw.cn

[R13] for 计数循环
来源：http://hma.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://yoj.svipenyu.cn

[R14] C 风格 for
来源：http://ayl.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zdc.yueranfly.top

[R15] while 逐行读文件
来源：http://ncx.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://odh.chenlongwang.top

[R16] until 等待条件
来源：http://xxo.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://muj.smart0.xyz

[R17] 数组定义与取值
来源：http://jih.hfpthk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mev.xuanzx.com

[R18] 遍历数组
来源：http://ocv.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jwz.hesvh.cn

[R19] 数组长度
来源：http://erl.9152youxi.cn


<!-- 参考信息 -->