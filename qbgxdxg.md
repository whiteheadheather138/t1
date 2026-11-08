代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://jn.zhonguo8118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://bf.zhonguo6118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://wp.zhonguo6118.cn

Ruby: a == b
来源：https://oo.zhonguo6118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://zx.zhonguo8118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://nb.zhonguo7118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://jg.zhonguo8118.cn

PHP:  if (empty($x)) {}
来源：https://sc.zhonguo4118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://qf.zhonguo6118.cn

TS:   if (x == null) {}
来源：https://qn.zhonguo7118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://lu.zhonguo7118.cn

Go:   if x == nil {}
来源：https://rg.zhonguo4118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://rr.zhonguo1118.cn

C#:   if (x is null) {}
来源：https://pw.zhonguo8118.cn

[P07] 防抖与节流
来源：https://xy.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://zb.zhonguo4118.cn

PHP:  // 手写时间戳比较
来源：https://zu.zhonguo2118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://tz.zhonguo1118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://sm.zhonguo6118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://cv.zhonguo3118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://oz.zhonguo8118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://tk.zhonguo5118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://cj.zhonguo2118.cn

[P08] 处理浮点精度问题
来源：https://um.zhonguo4118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://hw.zhonguo2118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://xw.zhonguo1118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://he.zhonguo8118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://pk.zhonguo1118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://bp.zhonguo4118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://mi.zhonguo4118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://zt.zhonguo7118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://ed.zhonguo2118.cn

================================================================================
来源：https://xe.zhonguo6118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://lu.zhonguo7118.cn

================================================================================
来源：https://rv.zhonguo6118.cn

[Q01] 创建表
来源：https://ca.zhonguo2118.cn

CREATE TABLE users (
来源：https://hr.zhonguo6118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://yx.zhonguo5118.cn

name VARCHAR(50) NOT NULL,
来源：https://ss.zhonguo1118.cn

email VARCHAR(100) UNIQUE,
来源：https://qs.zhonguo3118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://jt.zhonguo7118.cn

);
来源：https://rz.zhonguo8118.cn

[Q02] 创建带外键的表
来源：https://nx.zhonguo2118.cn

CREATE TABLE orders (
来源：https://yq.zhonguo2118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://ll.zhonguo6118.cn

user_id INT NOT NULL,
来源：https://ul.zhonguo1118.cn

amount DECIMAL(10, 2),
来源：https://vj.zhonguo1118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://vi.zhonguo7118.cn

);
来源：https://ae.zhonguo1118.cn

[Q03] 增加列
来源：https://at.zhonguo1118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://au.zhonguo7118.cn

[Q04] 修改列类型
来源：https://tu.zhonguo4118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://zo.zhonguo2118.cn

[Q05] 重命名列
来源：https://uj.zhonguo5118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://dn.zhonguo3118.cn

[Q06] 删除列
来源：https://vu.zhonguo8118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://uw.zhonguo8118.cn

[Q07] 删除表
来源：https://jb.zhonguo4118.cn

DROP TABLE IF EXISTS orders;
来源：https://st.zhonguo4118.cn

[Q08] 创建普通索引
来源：https://fp.zhonguo5118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://af.zhonguo8118.cn

[Q09] 创建唯一索引
来源：https://pj.zhonguo6118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://st.zhonguo1118.cn

[Q10] 插入单行
来源：https://vm.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://hh.zhonguo6118.cn

[Q11] 一次插入多行
来源：https://xe.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://gv.zhonguo2118.cn

[Q12] 插入后取自增 ID
来源：https://bj.zhonguo1118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://tc.zhonguo1118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://aq.zhonguo6118.cn

[Q13] 忽略重复插入
来源：https://bm.zhonguo4118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://yy.zhonguo3118.cn

[Q14] 存在则更新（upsert）
来源：https://dh.zhonguo3118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://fm.zhonguo7118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://ll.zhonguo6118.cn

[Q15] 查询全部
来源：https://fl.zhonguo4118.cn

SELECT * FROM users;
来源：https://ic.zhonguo1118.cn

[Q16] 查询指定列
来源：https://hf.zhonguo8118.cn

SELECT id, name FROM users;
来源：https://xd.zhonguo4118.cn

[Q17] 条件查询
来源：https://lr.zhonguo7118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://hb.zhonguo6118.cn

[Q18] 模糊匹配
来源：https://sh.zhonguo4118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://ed.zhonguo2118.cn

[Q19] 范围查询
来源：https://aq.zhonguo7118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://gk.zhonguo4118.cn

[Q20] IN 列表
来源：https://vn.zhonguo6118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://ax.zhonguo2118.cn

[Q21] 空值判断
来源：https://ao.zhonguo1118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://uo.zhonguo7118.cn

[Q22] 排序
来源：https://wf.zhonguo3118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://gb.zhonguo6118.cn

[Q23] 分页
来源：https://bi.zhonguo3118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://pe.zhonguo6118.cn

[Q24] 去重
来源：https://ao.zhonguo3118.cn

SELECT DISTINCT city FROM users;
来源：https://zg.zhonguo6118.cn

[Q25] 只取前 N 条
来源：https://jm.zhonguo2118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://rz.zhonguo8118.cn

[Q26] 计数
来源：https://mo.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://wv.zhonguo3118.cn

[Q27] 条件计数
来源：https://bk.zhonguo3118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://vx.zhonguo4118.cn

[Q28] 求和与平均
来源：https://lw.zhonguo2118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://ci.zhonguo5118.cn

[Q29] 最大最小值
来源：https://yi.zhonguo2118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://gj.zhonguo3118.cn

[Q30] 分组统计
来源：https://rn.zhonguo1118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://nn.zhonguo6118.cn

[Q31] 分组后过滤
来源：https://uv.zhonguo3118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://ln.zhonguo3118.cn

[Q32] 分组拼接字符串
来源：https://kb.zhonguo3118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://pe.zhonguo7118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://ou.zhonguo6118.cn

[Q33] 多列分组
来源：https://dw.zhonguo2118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://mx.zhonguo6118.cn

[Q34] 每组取第一条
来源：https://ks.zhonguo6118.cn

SELECT * FROM (
来源：https://uf.zhonguo1118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://lr.zhonguo4118.cn

) t WHERE rn = 1;
来源：https://qf.zhonguo6118.cn

[Q35] 内连接
来源：https://po.zhonguo8118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://gv.zhonguo6118.cn

[Q36] 左连接
来源：https://hf.zhonguo1118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://hn.zhonguo7118.cn

[Q37] 右连接
来源：https://dl.zhonguo2118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://yp.zhonguo8118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://gh.zhonguo5118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://bh.zhonguo4118.cn

[Q39] 自连接（查上下级）
来源：https://az.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://yd.zhonguo7118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://qn.zhonguo2118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://nf.zhonguo1118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://ix.zhonguo3118.cn

[Q41] 多表连接
来源：https://vs.zhonguo4118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://lb.zhonguo2118.cn

JOIN users u ON u.id = o.user_id
来源：https://zp.zhonguo1118.cn

JOIN products p ON p.id = o.product_id;
来源：https://ft.zhonguo7118.cn

[Q42] 连接条件附加过滤
来源：https://wx.zhonguo4118.cn

SELECT u.name, o.amount FROM users u
来源：https://fs.zhonguo1118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://xt.zhonguo7118.cn

[Q43] 标量子查询
来源：https://nk.zhonguo5118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://vj.zhonguo7118.cn

[Q44] IN 子查询
来源：https://qs.zhonguo5118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://lp.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://ls.zhonguo6118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://kt.zhonguo3118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://jv.zhonguo1118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://dd.zhonguo7118.cn

[Q47] 与平均值比较
来源：https://ft.zhonguo8118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://ii.zhonguo4118.cn

[Q48] CTE 公用表表达式
来源：https://bj.zhonguo4118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://yh.zhonguo4118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ij.zhonguo4118.cn

[Q49] 更新单行
来源：https://cb.zhonguo7118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://vz.zhonguo7118.cn

[Q50] 批量更新
来源：https://gc.zhonguo8118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://gt.zhonguo4118.cn

[Q51] 用子查询更新
来源：https://co.zhonguo8118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://cr.zhonguo3118.cn

[Q52] 删除指定行
来源：https://zb.zhonguo8118.cn

DELETE FROM users WHERE id = 10;
来源：https://xv.zhonguo3118.cn

[Q53] 按条件删除
来源：https://wn.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://xs.zhonguo6118.cn

[Q54] 清空表
来源：https://ft.zhonguo1118.cn

TRUNCATE TABLE logs;
来源：https://sd.zhonguo4118.cn

[Q55] 排名（并列占位）
来源：https://ej.zhonguo4118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://su.zhonguo1118.cn

[Q56] 密集排名（并列不占位）
来源：https://io.zhonguo1118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://xo.zhonguo1118.cn

[Q57] 行号
来源：https://qu.zhonguo2118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://vo.zhonguo1118.cn

[Q58] 累计求和
来源：https://iv.zhonguo2118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://zp.zhonguo7118.cn

[Q59] 分组内累计
来源：https://bi.zhonguo2118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://xj.zhonguo2118.cn

[Q60] 取上一行 / 下一行
来源：https://eq.zhonguo7118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://ej.zhonguo7118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://eu.zhonguo7118.cn

[Q61] 移动平均
来源：https://ml.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://ng.zhonguo3118.cn

[Q62] 分组占比
来源：https://bb.zhonguo5118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://ag.zhonguo2118.cn

[Q63] 开启事务
来源：https://dn.zhonguo7118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://bq.zhonguo3118.cn

[Q64] 提交事务
来源：https://mn.zhonguo8118.cn

COMMIT;
来源：https://vj.zhonguo7118.cn

[Q65] 回滚事务
来源：https://pn.zhonguo5118.cn

ROLLBACK;
来源：https://yh.zhonguo1118.cn

[Q66] 行锁查询
来源：https://sd.zhonguo7118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://iw.zhonguo7118.cn

[Q67] 设置隔离级别
来源：https://wa.zhonguo6118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://tp.zhonguo7118.cn

[Q68] 保存点
来源：https://wn.zhonguo3118.cn

SAVEPOINT sp1;
来源：https://to.zhonguo6118.cn

ROLLBACK TO sp1;
来源：https://ja.zhonguo8118.cn

[Q69] 查看执行计划
来源：https://ts.zhonguo2118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://fc.zhonguo8118.cn

[Q70] 更新统计信息
来源：https://ek.zhonguo6118.cn

ANALYZE TABLE users;
来源：https://pf.zhonguo7118.cn

[Q71] 查看建表语句
来源：https://wi.zhonguo4118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://vi.zhonguo1118.cn

[Q72] 查看索引
来源：https://nw.zhonguo3118.cn

SHOW INDEX FROM users;
来源：https://rf.zhonguo8118.cn

[Q73] 查看表状态
来源：https://cn.zhonguo8118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://rv.zhonguo7118.cn

[Q74] 强制使用索引
来源：https://dp.zhonguo4118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://gu.zhonguo1118.cn

[Q75] 日期格式化
来源：https://cc.zhonguo3118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://sf.zhonguo4118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://aw.zhonguo5118.cn

[Q76] 按天统计
来源：https://bj.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ah.zhonguo8118.cn

[Q77] 时间加减
来源：https://pg.zhonguo5118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://eo.zhonguo6118.cn

[Q78] 当前时间
来源：https://ch.zhonguo8118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://xk.zhonguo5118.cn

[Q79] 字符串拼接
来源：https://uh.zhonguo3118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://ay.zhonguo1118.cn

[Q80] 字符串截取
来源：https://rm.zhonguo6118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://jl.zhonguo6118.cn

[Q81] 字符串替换
来源：https://qi.zhonguo1118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://lo.zhonguo7118.cn

[Q82] 字符长度与字节长度
来源：https://wr.zhonguo2118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://bz.zhonguo2118.cn

[Q83] 大小写转换
来源：https://mf.zhonguo4118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ho.zhonguo1118.cn

[Q84] 去除首尾空格
来源：https://qc.zhonguo2118.cn

SELECT TRIM(name) FROM users;
来源：https://vs.zhonguo4118.cn

[Q85] 数值取整
来源：https://ml.zhonguo4118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://tv.zhonguo2118.cn

[Q86] 读取 JSON 字段
来源：https://vj.zhonguo6118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://lo.zhonguo8118.cn

[Q87] JSON 字段做条件
来源：https://lp.zhonguo4118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://iq.zhonguo6118.cn

[Q88] 行转列（条件聚合）
来源：https://en.zhonguo6118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://ye.zhonguo8118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://eg.zhonguo2118.cn

[Q89] 判断表是否存在
来源：https://hw.zhonguo5118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://hc.zhonguo6118.cn

[Q90] 生成序号列
来源：https://ve.zhonguo5118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ho.zhonguo8118.cn

================================================================================
来源：https://zs.zhonguo8118.cn

R. Bash 专题
来源：https://cy.zhonguo8118.cn

================================================================================
来源：https://da.zhonguo3118.cn

[R01] shebang 与严格模式
来源：https://rh.zhonguo6118.cn

#!/usr/bin/env bash
来源：https://fn.zhonguo5118.cn

set -euo pipefail
来源：https://nv.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://eg.zhonguo6118.cn

name="Tom"; echo "$name"
来源：https://ni.zhonguo8118.cn

[R03] 只读变量
来源：https://st.zhonguo5118.cn

readonly PI=3.14
来源：https://zx.zhonguo7118.cn

[R04] 位置参数
来源：https://wi.zhonguo3118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://yg.zhonguo1118.cn

[R05] 参数默认值
来源：https://fm.zhonguo8118.cn

name="${1:-default}"
来源：https://ag.zhonguo6118.cn

[R06] 判断命令是否存在
来源：https://qk.zhonguo5118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://tt.zhonguo6118.cn

[R07] if 判断文件
来源：https://gv.zhonguo4118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://qm.zhonguo6118.cn

[R08] 数值比较
来源：https://vi.zhonguo1118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ht.zhonguo1118.cn

[R09] 字符串比较
来源：https://zw.zhonguo2118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://au.zhonguo8118.cn

[R10] 正则匹配
来源：https://ri.zhonguo4118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ms.zhonguo4118.cn

[R11] case 多分支
来源：https://hw.zhonguo2118.cn

case "$1" in
来源：https://mv.zhonguo7118.cn

start) echo "启动" ;;
来源：https://jj.zhonguo8118.cn

stop)  echo "停止" ;;
来源：https://kn.zhonguo3118.cn

*)     echo "未知命令" ;;
来源：https://ib.zhonguo1118.cn

esac
来源：https://gp.zhonguo7118.cn

[R12] for 遍历文件
来源：https://bl.zhonguo8118.cn

for f in *.txt; do echo "$f"; done
来源：https://gv.zhonguo4118.cn

[R13] for 计数循环
来源：https://af.zhonguo3118.cn

for i in {1..10}; do echo "$i"; done
来源：https://hx.zhonguo5118.cn

[R14] C 风格 for
来源：https://bv.zhonguo3118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://il.zhonguo8118.cn

[R15] while 逐行读文件
来源：https://lj.zhonguo1118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://yu.zhonguo3118.cn

[R16] until 等待条件
来源：https://il.zhonguo4118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://km.zhonguo8118.cn

[R17] 数组定义与取值
来源：https://bi.zhonguo5118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://vf.zhonguo2118.cn

[R18] 遍历数组
来源：https://uf.zhonguo7118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://aj.zhonguo6118.cn

[R19] 数组长度
来源：https://ud.zhonguo7118.cn

echo "${#arr[@]}"
来源：https://vs.zhonguo8118.cn

[R20] 关联数组（字典）
来源：https://kq.zhonguo2118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://jy.zhonguo5118.cn

[R21] 字符串长度
来源：https://qi.zhonguo2118.cn

echo "${#s}"
来源：https://am.zhonguo2118.cn

[R22] 截取子串
来源：https://aa.zhonguo6118.cn

echo "${s:0:5}"
来源：https://fc.zhonguo2118.cn

[R23] 字符串替换
来源：https://ek.zhonguo4118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://ta.zhonguo8118.cn

[R24] 大小写转换
来源：https://xs.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://xa.zhonguo3118.cn

[R25] 去后缀 / 去前缀
来源：https://jd.zhonguo1118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://pc.zhonguo5118.cn

[R26] 命令替换
来源：https://ru.zhonguo6118.cn

now=$(date +%F); echo "$now"
来源：https://vk.zhonguo8118.cn

[R27] 算术展开
来源：https://dw.zhonguo7118.cn


<!-- 参考信息 -->