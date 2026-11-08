代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://xt.zhonguo6118.cn

C#:   if (x is null) {}
来源：https://yd.zhonguo1118.cn

[P07] 防抖与节流
来源：https://xz.zhonguo3118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://qz.zhonguo7118.cn

PHP:  // 手写时间戳比较
来源：https://uw.zhonguo3118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://iw.zhonguo5118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ha.zhonguo2118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://ug.zhonguo1118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://wf.zhonguo7118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://fz.zhonguo6118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://ty.zhonguo7118.cn

[P08] 处理浮点精度问题
来源：https://vg.zhonguo7118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://lm.zhonguo4118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://ao.zhonguo4118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://jj.zhonguo3118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://jg.zhonguo8118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://bk.zhonguo2118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://vg.zhonguo6118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://jy.zhonguo8118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://za.zhonguo7118.cn

================================================================================
来源：https://sr.zhonguo1118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://gs.zhonguo8118.cn

================================================================================
来源：https://gc.zhonguo1118.cn

[Q01] 创建表
来源：https://ay.zhonguo4118.cn

CREATE TABLE users (
来源：https://hb.zhonguo7118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://ly.zhonguo7118.cn

name VARCHAR(50) NOT NULL,
来源：https://hh.zhonguo5118.cn

email VARCHAR(100) UNIQUE,
来源：https://dz.zhonguo5118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://ar.zhonguo4118.cn

);
来源：https://uk.zhonguo6118.cn

[Q02] 创建带外键的表
来源：https://nt.zhonguo7118.cn

CREATE TABLE orders (
来源：https://pr.zhonguo6118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://im.zhonguo4118.cn

user_id INT NOT NULL,
来源：https://dm.zhonguo4118.cn

amount DECIMAL(10, 2),
来源：https://fj.zhonguo4118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://rw.zhonguo3118.cn

);
来源：https://go.zhonguo7118.cn

[Q03] 增加列
来源：https://us.zhonguo8118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://nu.zhonguo3118.cn

[Q04] 修改列类型
来源：https://yd.zhonguo4118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://bs.zhonguo5118.cn

[Q05] 重命名列
来源：https://zl.zhonguo8118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://oc.zhonguo3118.cn

[Q06] 删除列
来源：https://ag.zhonguo8118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://ks.zhonguo3118.cn

[Q07] 删除表
来源：https://mo.zhonguo7118.cn

DROP TABLE IF EXISTS orders;
来源：https://wq.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://zw.zhonguo6118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://kn.zhonguo5118.cn

[Q09] 创建唯一索引
来源：https://fz.zhonguo2118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://vg.zhonguo4118.cn

[Q10] 插入单行
来源：https://yz.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://fm.zhonguo1118.cn

[Q11] 一次插入多行
来源：https://qp.zhonguo4118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://md.zhonguo6118.cn

[Q12] 插入后取自增 ID
来源：https://ml.zhonguo1118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://gj.zhonguo7118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://kn.zhonguo1118.cn

[Q13] 忽略重复插入
来源：https://zi.zhonguo6118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://ym.zhonguo6118.cn

[Q14] 存在则更新（upsert）
来源：https://jk.zhonguo1118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://vg.zhonguo8118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://qt.zhonguo7118.cn

[Q15] 查询全部
来源：https://oi.zhonguo8118.cn

SELECT * FROM users;
来源：https://gj.zhonguo6118.cn

[Q16] 查询指定列
来源：https://kk.zhonguo8118.cn

SELECT id, name FROM users;
来源：https://ff.zhonguo3118.cn

[Q17] 条件查询
来源：https://go.zhonguo3118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://cg.zhonguo2118.cn

[Q18] 模糊匹配
来源：https://zd.zhonguo5118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://eb.zhonguo8118.cn

[Q19] 范围查询
来源：https://yn.zhonguo4118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://kv.zhonguo7118.cn

[Q20] IN 列表
来源：https://ur.zhonguo2118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://de.zhonguo3118.cn

[Q21] 空值判断
来源：https://ap.zhonguo6118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://hl.zhonguo8118.cn

[Q22] 排序
来源：https://xk.zhonguo1118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://xp.zhonguo2118.cn

[Q23] 分页
来源：https://kx.zhonguo3118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://ck.zhonguo2118.cn

[Q24] 去重
来源：https://yn.zhonguo8118.cn

SELECT DISTINCT city FROM users;
来源：https://wm.zhonguo3118.cn

[Q25] 只取前 N 条
来源：https://be.zhonguo5118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://sh.zhonguo8118.cn

[Q26] 计数
来源：https://vm.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://az.zhonguo4118.cn

[Q27] 条件计数
来源：https://zl.zhonguo1118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://pl.zhonguo3118.cn

[Q28] 求和与平均
来源：https://cw.zhonguo4118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://ts.zhonguo6118.cn

[Q29] 最大最小值
来源：https://py.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://qd.zhonguo8118.cn

[Q30] 分组统计
来源：https://av.zhonguo3118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ub.zhonguo7118.cn

[Q31] 分组后过滤
来源：https://gm.zhonguo4118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://rg.zhonguo5118.cn

[Q32] 分组拼接字符串
来源：https://cm.zhonguo1118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://zy.zhonguo2118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://uh.zhonguo2118.cn

[Q33] 多列分组
来源：https://sp.zhonguo2118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ul.zhonguo8118.cn

[Q34] 每组取第一条
来源：https://hp.zhonguo6118.cn

SELECT * FROM (
来源：https://cp.zhonguo1118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://ov.zhonguo2118.cn

) t WHERE rn = 1;
来源：https://vg.zhonguo1118.cn

[Q35] 内连接
来源：https://hm.zhonguo4118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://nv.zhonguo5118.cn

[Q36] 左连接
来源：https://fs.zhonguo8118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://ig.zhonguo7118.cn

[Q37] 右连接
来源：https://yk.zhonguo2118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://ip.zhonguo4118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://nf.zhonguo3118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://nq.zhonguo5118.cn

[Q39] 自连接（查上下级）
来源：https://vg.zhonguo2118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://ue.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://ug.zhonguo3118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://xg.zhonguo4118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://ml.zhonguo4118.cn

[Q41] 多表连接
来源：https://lg.zhonguo3118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://gn.zhonguo3118.cn

JOIN users u ON u.id = o.user_id
来源：https://ov.zhonguo6118.cn

JOIN products p ON p.id = o.product_id;
来源：https://nv.zhonguo6118.cn

[Q42] 连接条件附加过滤
来源：https://rt.zhonguo6118.cn

SELECT u.name, o.amount FROM users u
来源：https://ir.zhonguo7118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://yr.zhonguo1118.cn

[Q43] 标量子查询
来源：https://lo.zhonguo6118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://he.zhonguo8118.cn

[Q44] IN 子查询
来源：https://zr.zhonguo5118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://ha.zhonguo3118.cn

[Q45] EXISTS 判断存在
来源：https://gm.zhonguo3118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://ck.zhonguo7118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://xp.zhonguo2118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://xd.zhonguo3118.cn

[Q47] 与平均值比较
来源：https://tz.zhonguo7118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://hw.zhonguo8118.cn

[Q48] CTE 公用表表达式
来源：https://gp.zhonguo5118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://nw.zhonguo1118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ii.zhonguo2118.cn

[Q49] 更新单行
来源：https://jj.zhonguo4118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://td.zhonguo2118.cn

[Q50] 批量更新
来源：https://mx.zhonguo2118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://jw.zhonguo3118.cn

[Q51] 用子查询更新
来源：https://ph.zhonguo1118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://vk.zhonguo6118.cn

[Q52] 删除指定行
来源：https://om.zhonguo2118.cn

DELETE FROM users WHERE id = 10;
来源：https://vh.zhonguo2118.cn

[Q53] 按条件删除
来源：https://qt.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://hb.zhonguo7118.cn

[Q54] 清空表
来源：https://zi.zhonguo4118.cn

TRUNCATE TABLE logs;
来源：https://uq.zhonguo2118.cn

[Q55] 排名（并列占位）
来源：https://kb.zhonguo6118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://vt.zhonguo1118.cn

[Q56] 密集排名（并列不占位）
来源：https://ie.zhonguo1118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://kp.zhonguo3118.cn

[Q57] 行号
来源：https://io.zhonguo4118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://ym.zhonguo6118.cn

[Q58] 累计求和
来源：https://si.zhonguo7118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://up.zhonguo1118.cn

[Q59] 分组内累计
来源：https://qr.zhonguo4118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://hq.zhonguo3118.cn

[Q60] 取上一行 / 下一行
来源：https://dq.zhonguo7118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://bt.zhonguo5118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://be.zhonguo8118.cn

[Q61] 移动平均
来源：https://ly.zhonguo1118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://tq.zhonguo3118.cn

[Q62] 分组占比
来源：https://gk.zhonguo3118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://st.zhonguo2118.cn

[Q63] 开启事务
来源：https://es.zhonguo8118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://li.zhonguo8118.cn

[Q64] 提交事务
来源：https://mv.zhonguo7118.cn

COMMIT;
来源：https://kr.zhonguo6118.cn

[Q65] 回滚事务
来源：https://ex.zhonguo2118.cn

ROLLBACK;
来源：https://ao.zhonguo8118.cn

[Q66] 行锁查询
来源：https://pd.zhonguo8118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://zk.zhonguo4118.cn

[Q67] 设置隔离级别
来源：https://av.zhonguo3118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://qx.zhonguo6118.cn

[Q68] 保存点
来源：https://wq.zhonguo3118.cn

SAVEPOINT sp1;
来源：https://yv.zhonguo8118.cn

ROLLBACK TO sp1;
来源：https://pl.zhonguo1118.cn

[Q69] 查看执行计划
来源：https://fg.zhonguo5118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://ws.zhonguo3118.cn

[Q70] 更新统计信息
来源：https://ju.zhonguo6118.cn

ANALYZE TABLE users;
来源：https://hb.zhonguo2118.cn

[Q71] 查看建表语句
来源：https://fd.zhonguo4118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://hg.zhonguo2118.cn

[Q72] 查看索引
来源：https://wk.zhonguo2118.cn

SHOW INDEX FROM users;
来源：https://qy.zhonguo3118.cn

[Q73] 查看表状态
来源：https://gh.zhonguo1118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://gi.zhonguo2118.cn

[Q74] 强制使用索引
来源：https://mo.zhonguo5118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://ac.zhonguo8118.cn

[Q75] 日期格式化
来源：https://vg.zhonguo6118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://sb.zhonguo7118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://oh.zhonguo7118.cn

[Q76] 按天统计
来源：https://gz.zhonguo1118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://xt.zhonguo4118.cn

[Q77] 时间加减
来源：https://at.zhonguo4118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://py.zhonguo3118.cn

[Q78] 当前时间
来源：https://jz.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://po.zhonguo8118.cn

[Q79] 字符串拼接
来源：https://dg.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://xo.zhonguo3118.cn

[Q80] 字符串截取
来源：https://hi.zhonguo1118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://lm.zhonguo8118.cn

[Q81] 字符串替换
来源：https://vy.zhonguo4118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://lo.zhonguo7118.cn

[Q82] 字符长度与字节长度
来源：https://rl.zhonguo2118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://rp.zhonguo3118.cn

[Q83] 大小写转换
来源：https://lc.zhonguo2118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ki.zhonguo4118.cn

[Q84] 去除首尾空格
来源：https://et.zhonguo1118.cn

SELECT TRIM(name) FROM users;
来源：https://zr.zhonguo6118.cn

[Q85] 数值取整
来源：https://nm.zhonguo4118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://ya.zhonguo1118.cn

[Q86] 读取 JSON 字段
来源：https://tu.zhonguo5118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://wq.zhonguo5118.cn

[Q87] JSON 字段做条件
来源：https://co.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://uy.zhonguo4118.cn

[Q88] 行转列（条件聚合）
来源：https://ap.zhonguo2118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://gg.zhonguo4118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://ci.zhonguo3118.cn

[Q89] 判断表是否存在
来源：https://wp.zhonguo7118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://ff.zhonguo4118.cn

[Q90] 生成序号列
来源：https://qp.zhonguo3118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://go.zhonguo6118.cn

================================================================================
来源：https://rl.zhonguo4118.cn

R. Bash 专题
来源：https://px.zhonguo1118.cn

================================================================================
来源：https://cd.zhonguo1118.cn

[R01] shebang 与严格模式
来源：https://lf.zhonguo8118.cn

#!/usr/bin/env bash
来源：https://ej.zhonguo4118.cn

set -euo pipefail
来源：https://mo.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://tb.zhonguo1118.cn

name="Tom"; echo "$name"
来源：https://rr.zhonguo4118.cn

[R03] 只读变量
来源：https://vl.zhonguo8118.cn

readonly PI=3.14
来源：https://lv.zhonguo3118.cn

[R04] 位置参数
来源：https://vi.zhonguo7118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://an.zhonguo3118.cn

[R05] 参数默认值
来源：https://me.zhonguo5118.cn

name="${1:-default}"
来源：https://yz.zhonguo3118.cn

[R06] 判断命令是否存在
来源：https://ii.zhonguo4118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://bd.zhonguo2118.cn

[R07] if 判断文件
来源：https://yh.zhonguo5118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://pi.zhonguo6118.cn

[R08] 数值比较
来源：https://uc.zhonguo6118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://wt.zhonguo7118.cn

[R09] 字符串比较
来源：https://cu.zhonguo2118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://mn.zhonguo5118.cn

[R10] 正则匹配
来源：https://gi.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://bl.zhonguo2118.cn

[R11] case 多分支
来源：https://qj.zhonguo5118.cn

case "$1" in
来源：https://ym.zhonguo3118.cn

start) echo "启动" ;;
来源：https://ae.zhonguo7118.cn

stop)  echo "停止" ;;
来源：https://ws.zhonguo2118.cn

*)     echo "未知命令" ;;
来源：https://dw.zhonguo7118.cn

esac
来源：https://yx.zhonguo7118.cn

[R12] for 遍历文件
来源：https://ih.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://wd.zhonguo7118.cn

[R13] for 计数循环
来源：https://ct.zhonguo7118.cn

for i in {1..10}; do echo "$i"; done
来源：https://at.zhonguo4118.cn

[R14] C 风格 for
来源：https://yr.zhonguo6118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://mh.zhonguo1118.cn

[R15] while 逐行读文件
来源：https://ef.zhonguo3118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://mo.zhonguo1118.cn

[R16] until 等待条件
来源：https://fe.zhonguo3118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://bl.zhonguo4118.cn

[R17] 数组定义与取值
来源：https://vs.zhonguo7118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://ef.zhonguo1118.cn

[R18] 遍历数组
来源：https://ni.zhonguo4118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://kn.zhonguo2118.cn

[R19] 数组长度
来源：https://gw.zhonguo4118.cn

echo "${#arr[@]}"
来源：https://nj.zhonguo3118.cn

[R20] 关联数组（字典）
来源：https://rp.zhonguo8118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://xv.zhonguo1118.cn

[R21] 字符串长度
来源：https://tb.zhonguo7118.cn

echo "${#s}"
来源：https://vx.zhonguo8118.cn

[R22] 截取子串
来源：https://gq.zhonguo1118.cn

echo "${s:0:5}"
来源：https://ev.zhonguo5118.cn

[R23] 字符串替换
来源：https://fe.zhonguo8118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://sb.zhonguo3118.cn

[R24] 大小写转换
来源：https://im.zhonguo2118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ze.zhonguo3118.cn

[R25] 去后缀 / 去前缀
来源：https://li.zhonguo3118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://vw.zhonguo6118.cn

[R26] 命令替换
来源：https://ei.zhonguo7118.cn

now=$(date +%F); echo "$now"
来源：https://ox.zhonguo7118.cn

[R27] 算术展开
来源：https://va.zhonguo7118.cn

echo $((1 + 2 * 3))
来源：https://cx.zhonguo3118.cn

[R28] 浮点运算
来源：https://xs.zhonguo6118.cn

echo "scale=2; 10/3" | bc
来源：https://ov.zhonguo5118.cn

[R29] 定义函数
来源：https://jv.zhonguo6118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://cy.zhonguo4118.cn

[R30] 函数返回状态码
来源：https://jz.zhonguo8118.cn

f() { return 0; }; f || echo "失败了"
来源：https://bj.zhonguo6118.cn

[R31] 局部变量
来源：https://nv.zhonguo2118.cn

f() { local x=1; echo "$x"; }
来源：https://ye.zhonguo6118.cn

[R32] 参数个数校验
来源：https://ha.zhonguo7118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://ns.zhonguo2118.cn

[R33] 捕获错误并提示行号
来源：https://wt.zhonguo5118.cn


<!-- 参考信息 -->