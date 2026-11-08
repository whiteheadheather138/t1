代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：https://kl.zhonguo3118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://qt.zhonguo5118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://op.zhonguo2118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://tv.zhonguo8118.cn

Java: list.size();  map.size();  s.length()
来源：https://kg.zhonguo5118.cn

Go:   len(arr);  len(m)
来源：https://wv.zhonguo7118.cn

Ruby: x.length;  x.size
来源：https://vr.zhonguo5118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://lq.zhonguo1118.cn

[P05] 判断两个对象内容是否相等
来源：https://ky.zhonguo6118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://ni.zhonguo6118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://fs.zhonguo2118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://qf.zhonguo4118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://wm.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://tx.zhonguo3118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://rz.zhonguo4118.cn

Ruby: a == b
来源：https://yg.zhonguo7118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://st.zhonguo5118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://lc.zhonguo5118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://fz.zhonguo2118.cn

PHP:  if (empty($x)) {}
来源：https://no.zhonguo3118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://vk.zhonguo2118.cn

TS:   if (x == null) {}
来源：https://ts.zhonguo5118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://mb.zhonguo8118.cn

Go:   if x == nil {}
来源：https://tl.zhonguo4118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://ud.zhonguo7118.cn

C#:   if (x is null) {}
来源：https://uy.zhonguo6118.cn

[P07] 防抖与节流
来源：https://bi.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://lu.zhonguo2118.cn

PHP:  // 手写时间戳比较
来源：https://ld.zhonguo4118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://li.zhonguo8118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://rt.zhonguo3118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://oo.zhonguo1118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://ee.zhonguo4118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://vs.zhonguo8118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://bd.zhonguo8118.cn

[P08] 处理浮点精度问题
来源：https://so.zhonguo7118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://im.zhonguo3118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://hm.zhonguo5118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://wm.zhonguo5118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://ji.zhonguo8118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://nz.zhonguo3118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://gj.zhonguo1118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://ue.zhonguo4118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ky.zhonguo2118.cn

================================================================================
来源：https://rt.zhonguo8118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://gw.zhonguo8118.cn

================================================================================
来源：https://aj.zhonguo3118.cn

[Q01] 创建表
来源：https://fq.zhonguo5118.cn

CREATE TABLE users (
来源：https://sj.zhonguo8118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://jw.zhonguo2118.cn

name VARCHAR(50) NOT NULL,
来源：https://mq.zhonguo5118.cn

email VARCHAR(100) UNIQUE,
来源：https://ul.zhonguo7118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://ig.zhonguo7118.cn

);
来源：https://zn.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://ts.zhonguo6118.cn

CREATE TABLE orders (
来源：https://rp.zhonguo5118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://qe.zhonguo3118.cn

user_id INT NOT NULL,
来源：https://la.zhonguo8118.cn

amount DECIMAL(10, 2),
来源：https://ta.zhonguo7118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://vj.zhonguo1118.cn

);
来源：https://mz.zhonguo1118.cn

[Q03] 增加列
来源：https://ld.zhonguo8118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://se.zhonguo6118.cn

[Q04] 修改列类型
来源：https://ua.zhonguo6118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://dw.zhonguo5118.cn

[Q05] 重命名列
来源：https://mq.zhonguo6118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://wj.zhonguo1118.cn

[Q06] 删除列
来源：https://dp.zhonguo4118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://gg.zhonguo7118.cn

[Q07] 删除表
来源：https://ks.zhonguo7118.cn

DROP TABLE IF EXISTS orders;
来源：https://mr.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://xe.zhonguo7118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://sq.zhonguo2118.cn

[Q09] 创建唯一索引
来源：https://xj.zhonguo7118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://tc.zhonguo4118.cn

[Q10] 插入单行
来源：https://mq.zhonguo8118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://nz.zhonguo2118.cn

[Q11] 一次插入多行
来源：https://qn.zhonguo2118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://eu.zhonguo1118.cn

[Q12] 插入后取自增 ID
来源：https://tr.zhonguo8118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://gb.zhonguo1118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://vy.zhonguo2118.cn

[Q13] 忽略重复插入
来源：https://np.zhonguo3118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://fm.zhonguo3118.cn

[Q14] 存在则更新（upsert）
来源：https://td.zhonguo4118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://yr.zhonguo8118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://sp.zhonguo8118.cn

[Q15] 查询全部
来源：https://lh.zhonguo4118.cn

SELECT * FROM users;
来源：https://aw.zhonguo5118.cn

[Q16] 查询指定列
来源：https://wc.zhonguo4118.cn

SELECT id, name FROM users;
来源：https://kb.zhonguo1118.cn

[Q17] 条件查询
来源：https://hp.zhonguo8118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://vv.zhonguo7118.cn

[Q18] 模糊匹配
来源：https://hv.zhonguo8118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://nk.zhonguo5118.cn

[Q19] 范围查询
来源：https://wr.zhonguo1118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://uy.zhonguo8118.cn

[Q20] IN 列表
来源：https://jt.zhonguo1118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://bi.zhonguo6118.cn

[Q21] 空值判断
来源：https://ds.zhonguo7118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://ks.zhonguo3118.cn

[Q22] 排序
来源：https://ul.zhonguo4118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://oo.zhonguo1118.cn

[Q23] 分页
来源：https://cp.zhonguo8118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://xn.zhonguo2118.cn

[Q24] 去重
来源：https://wu.zhonguo2118.cn

SELECT DISTINCT city FROM users;
来源：https://hh.zhonguo7118.cn

[Q25] 只取前 N 条
来源：https://iz.zhonguo2118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://hy.zhonguo3118.cn

[Q26] 计数
来源：https://uc.zhonguo6118.cn

SELECT COUNT(*) FROM users;
来源：https://ye.zhonguo5118.cn

[Q27] 条件计数
来源：https://wj.zhonguo5118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://jc.zhonguo6118.cn

[Q28] 求和与平均
来源：https://mp.zhonguo7118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://kg.zhonguo6118.cn

[Q29] 最大最小值
来源：https://re.zhonguo3118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://qn.zhonguo5118.cn

[Q30] 分组统计
来源：https://ie.zhonguo2118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ri.zhonguo2118.cn

[Q31] 分组后过滤
来源：https://sn.zhonguo4118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://hx.zhonguo6118.cn

[Q32] 分组拼接字符串
来源：https://lm.zhonguo3118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://xq.zhonguo7118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://kp.zhonguo8118.cn

[Q33] 多列分组
来源：https://te.zhonguo2118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://de.zhonguo5118.cn

[Q34] 每组取第一条
来源：https://tr.zhonguo4118.cn

SELECT * FROM (
来源：https://it.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://ir.zhonguo7118.cn

) t WHERE rn = 1;
来源：https://dx.zhonguo3118.cn

[Q35] 内连接
来源：https://qx.zhonguo4118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://gq.zhonguo8118.cn

[Q36] 左连接
来源：https://cf.zhonguo8118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://oa.zhonguo5118.cn

[Q37] 右连接
来源：https://yc.zhonguo1118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://zb.zhonguo5118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://ie.zhonguo4118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://wt.zhonguo2118.cn

[Q39] 自连接（查上下级）
来源：https://ok.zhonguo8118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://hz.zhonguo8118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://eo.zhonguo6118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://gr.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://fz.zhonguo3118.cn

[Q41] 多表连接
来源：https://as.zhonguo6118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://ns.zhonguo1118.cn

JOIN users u ON u.id = o.user_id
来源：https://zu.zhonguo6118.cn

JOIN products p ON p.id = o.product_id;
来源：https://yh.zhonguo4118.cn

[Q42] 连接条件附加过滤
来源：https://cz.zhonguo3118.cn

SELECT u.name, o.amount FROM users u
来源：https://ag.zhonguo8118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://ml.zhonguo8118.cn

[Q43] 标量子查询
来源：https://jg.zhonguo4118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://su.zhonguo6118.cn

[Q44] IN 子查询
来源：https://es.zhonguo8118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://pi.zhonguo8118.cn

[Q45] EXISTS 判断存在
来源：https://rf.zhonguo5118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://ih.zhonguo4118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://ac.zhonguo7118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://oe.zhonguo6118.cn

[Q47] 与平均值比较
来源：https://ae.zhonguo8118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://gh.zhonguo7118.cn

[Q48] CTE 公用表表达式
来源：https://hn.zhonguo2118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://ka.zhonguo7118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ec.zhonguo1118.cn

[Q49] 更新单行
来源：https://pi.zhonguo6118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://ui.zhonguo8118.cn

[Q50] 批量更新
来源：https://tv.zhonguo5118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://xr.zhonguo6118.cn

[Q51] 用子查询更新
来源：https://xr.zhonguo5118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://zw.zhonguo6118.cn

[Q52] 删除指定行
来源：https://wo.zhonguo4118.cn

DELETE FROM users WHERE id = 10;
来源：https://kl.zhonguo4118.cn

[Q53] 按条件删除
来源：https://lb.zhonguo1118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://fu.zhonguo3118.cn

[Q54] 清空表
来源：https://ou.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://at.zhonguo1118.cn

[Q55] 排名（并列占位）
来源：https://op.zhonguo1118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://tj.zhonguo6118.cn

[Q56] 密集排名（并列不占位）
来源：https://oa.zhonguo3118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://ix.zhonguo8118.cn

[Q57] 行号
来源：https://we.zhonguo1118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://dk.zhonguo4118.cn

[Q58] 累计求和
来源：https://yp.zhonguo8118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://mb.zhonguo4118.cn

[Q59] 分组内累计
来源：https://gn.zhonguo1118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://lm.zhonguo7118.cn

[Q60] 取上一行 / 下一行
来源：https://tb.zhonguo3118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://ux.zhonguo1118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://xf.zhonguo2118.cn

[Q61] 移动平均
来源：https://zd.zhonguo1118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://go.zhonguo7118.cn

[Q62] 分组占比
来源：https://es.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://xt.zhonguo3118.cn

[Q63] 开启事务
来源：https://ms.zhonguo7118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://va.zhonguo4118.cn

[Q64] 提交事务
来源：https://za.zhonguo3118.cn

COMMIT;
来源：https://gw.zhonguo1118.cn

[Q65] 回滚事务
来源：https://sp.zhonguo8118.cn

ROLLBACK;
来源：https://vl.zhonguo2118.cn

[Q66] 行锁查询
来源：https://bz.zhonguo4118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://of.zhonguo3118.cn

[Q67] 设置隔离级别
来源：https://jx.zhonguo2118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://fk.zhonguo8118.cn

[Q68] 保存点
来源：https://hb.zhonguo7118.cn

SAVEPOINT sp1;
来源：https://og.zhonguo7118.cn

ROLLBACK TO sp1;
来源：https://kg.zhonguo7118.cn

[Q69] 查看执行计划
来源：https://kk.zhonguo6118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://cz.zhonguo2118.cn

[Q70] 更新统计信息
来源：https://sj.zhonguo7118.cn

ANALYZE TABLE users;
来源：https://mf.zhonguo4118.cn

[Q71] 查看建表语句
来源：https://vr.zhonguo6118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://cc.zhonguo6118.cn

[Q72] 查看索引
来源：https://np.zhonguo2118.cn

SHOW INDEX FROM users;
来源：https://qd.zhonguo2118.cn

[Q73] 查看表状态
来源：https://jf.zhonguo3118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://tu.zhonguo3118.cn

[Q74] 强制使用索引
来源：https://ih.zhonguo4118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://si.zhonguo3118.cn

[Q75] 日期格式化
来源：https://kc.zhonguo5118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://lo.zhonguo4118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://rt.zhonguo4118.cn

[Q76] 按天统计
来源：https://zc.zhonguo1118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ex.zhonguo5118.cn

[Q77] 时间加减
来源：https://gd.zhonguo4118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://kw.zhonguo7118.cn

[Q78] 当前时间
来源：https://ju.zhonguo7118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://ec.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://da.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://af.zhonguo3118.cn

[Q80] 字符串截取
来源：https://rt.zhonguo8118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://qr.zhonguo8118.cn

[Q81] 字符串替换
来源：https://am.zhonguo6118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://yd.zhonguo1118.cn

[Q82] 字符长度与字节长度
来源：https://su.zhonguo2118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://su.zhonguo3118.cn

[Q83] 大小写转换
来源：https://bl.zhonguo2118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ef.zhonguo4118.cn

[Q84] 去除首尾空格
来源：https://ul.zhonguo7118.cn

SELECT TRIM(name) FROM users;
来源：https://sj.zhonguo7118.cn

[Q85] 数值取整
来源：https://mk.zhonguo1118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://dc.zhonguo4118.cn

[Q86] 读取 JSON 字段
来源：https://rr.zhonguo6118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://mc.zhonguo6118.cn

[Q87] JSON 字段做条件
来源：https://fq.zhonguo2118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://su.zhonguo5118.cn

[Q88] 行转列（条件聚合）
来源：https://nb.zhonguo3118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://ak.zhonguo1118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://gf.zhonguo6118.cn

[Q89] 判断表是否存在
来源：https://fy.zhonguo8118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://ep.zhonguo5118.cn

[Q90] 生成序号列
来源：https://rn.zhonguo7118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://fu.zhonguo6118.cn

================================================================================
来源：https://he.zhonguo1118.cn

R. Bash 专题
来源：https://fj.zhonguo5118.cn

================================================================================
来源：https://ca.zhonguo4118.cn

[R01] shebang 与严格模式
来源：https://fv.zhonguo4118.cn

#!/usr/bin/env bash
来源：https://rp.zhonguo5118.cn

set -euo pipefail
来源：https://xp.zhonguo1118.cn

[R02] 变量赋值与使用
来源：https://jl.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://nx.zhonguo4118.cn

[R03] 只读变量
来源：https://qj.zhonguo7118.cn

readonly PI=3.14
来源：https://sd.zhonguo7118.cn

[R04] 位置参数
来源：https://nd.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://ic.zhonguo1118.cn

[R05] 参数默认值
来源：https://nh.zhonguo2118.cn

name="${1:-default}"
来源：https://jm.zhonguo1118.cn

[R06] 判断命令是否存在
来源：https://gy.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://qx.zhonguo6118.cn

[R07] if 判断文件
来源：https://nx.zhonguo3118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://cz.zhonguo4118.cn

[R08] 数值比较
来源：https://wp.zhonguo6118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://yt.zhonguo1118.cn

[R09] 字符串比较
来源：https://vf.zhonguo1118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://zr.zhonguo4118.cn

[R10] 正则匹配
来源：https://xg.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://lg.zhonguo6118.cn

[R11] case 多分支
来源：https://qr.zhonguo1118.cn

case "$1" in
来源：https://yb.zhonguo3118.cn

start) echo "启动" ;;
来源：https://so.zhonguo7118.cn

stop)  echo "停止" ;;
来源：https://iu.zhonguo1118.cn

*)     echo "未知命令" ;;
来源：https://vw.zhonguo1118.cn

esac
来源：https://lx.zhonguo3118.cn

[R12] for 遍历文件
来源：https://qb.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://jc.zhonguo2118.cn

[R13] for 计数循环
来源：https://zr.zhonguo3118.cn

for i in {1..10}; do echo "$i"; done
来源：https://pk.zhonguo5118.cn

[R14] C 风格 for
来源：https://nl.zhonguo8118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://ma.zhonguo5118.cn

[R15] while 逐行读文件
来源：https://xo.zhonguo7118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://nx.zhonguo5118.cn

[R16] until 等待条件
来源：https://yi.zhonguo7118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://bp.zhonguo5118.cn

[R17] 数组定义与取值
来源：https://uf.zhonguo3118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://ey.zhonguo3118.cn

[R18] 遍历数组
来源：https://zg.zhonguo3118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://og.zhonguo7118.cn

[R19] 数组长度
来源：https://yi.zhonguo4118.cn

echo "${#arr[@]}"
来源：https://ft.zhonguo7118.cn

[R20] 关联数组（字典）
来源：https://mo.zhonguo7118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://zf.zhonguo7118.cn

[R21] 字符串长度
来源：https://fm.zhonguo6118.cn


<!-- 参考信息 -->