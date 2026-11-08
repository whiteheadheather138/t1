代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://qq.zhonguo4118.cn

);
来源：https://wl.zhonguo3118.cn

[Q02] 创建带外键的表
来源：https://ll.zhonguo8118.cn

CREATE TABLE orders (
来源：https://ms.zhonguo4118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://lk.zhonguo6118.cn

user_id INT NOT NULL,
来源：https://iw.zhonguo7118.cn

amount DECIMAL(10, 2),
来源：https://kx.zhonguo5118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://ud.zhonguo8118.cn

);
来源：https://ag.zhonguo2118.cn

[Q03] 增加列
来源：https://pk.zhonguo3118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://qe.zhonguo8118.cn

[Q04] 修改列类型
来源：https://jx.zhonguo3118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://rg.zhonguo3118.cn

[Q05] 重命名列
来源：https://nc.zhonguo1118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://sh.zhonguo1118.cn

[Q06] 删除列
来源：https://wf.zhonguo5118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://pn.zhonguo4118.cn

[Q07] 删除表
来源：https://si.zhonguo7118.cn

DROP TABLE IF EXISTS orders;
来源：https://fi.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://us.zhonguo4118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://pu.zhonguo4118.cn

[Q09] 创建唯一索引
来源：https://oi.zhonguo6118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://pd.zhonguo8118.cn

[Q10] 插入单行
来源：https://xu.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://xx.zhonguo6118.cn

[Q11] 一次插入多行
来源：https://wf.zhonguo5118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://tt.zhonguo1118.cn

[Q12] 插入后取自增 ID
来源：https://gg.zhonguo4118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://nc.zhonguo1118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://ko.zhonguo1118.cn

[Q13] 忽略重复插入
来源：https://nq.zhonguo7118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://yy.zhonguo7118.cn

[Q14] 存在则更新（upsert）
来源：https://zf.zhonguo4118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://hg.zhonguo8118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://yy.zhonguo7118.cn

[Q15] 查询全部
来源：https://id.zhonguo8118.cn

SELECT * FROM users;
来源：https://cr.zhonguo3118.cn

[Q16] 查询指定列
来源：https://wl.zhonguo3118.cn

SELECT id, name FROM users;
来源：https://qy.zhonguo3118.cn

[Q17] 条件查询
来源：https://qe.zhonguo4118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://yc.zhonguo2118.cn

[Q18] 模糊匹配
来源：https://dl.zhonguo5118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://jh.zhonguo3118.cn

[Q19] 范围查询
来源：https://or.zhonguo6118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://xz.zhonguo5118.cn

[Q20] IN 列表
来源：https://zh.zhonguo7118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://vn.zhonguo5118.cn

[Q21] 空值判断
来源：https://rr.zhonguo7118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://or.zhonguo3118.cn

[Q22] 排序
来源：https://wr.zhonguo3118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://xu.zhonguo6118.cn

[Q23] 分页
来源：https://sq.zhonguo6118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://lj.zhonguo7118.cn

[Q24] 去重
来源：https://yu.zhonguo1118.cn

SELECT DISTINCT city FROM users;
来源：https://dz.zhonguo8118.cn

[Q25] 只取前 N 条
来源：https://vk.zhonguo4118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://rr.zhonguo7118.cn

[Q26] 计数
来源：https://ce.zhonguo2118.cn

SELECT COUNT(*) FROM users;
来源：https://fw.zhonguo6118.cn

[Q27] 条件计数
来源：https://at.zhonguo6118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://xz.zhonguo6118.cn

[Q28] 求和与平均
来源：https://bk.zhonguo6118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://kg.zhonguo5118.cn

[Q29] 最大最小值
来源：https://sh.zhonguo5118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://ia.zhonguo2118.cn

[Q30] 分组统计
来源：https://yv.zhonguo7118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://wi.zhonguo6118.cn

[Q31] 分组后过滤
来源：https://et.zhonguo7118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://kv.zhonguo6118.cn

[Q32] 分组拼接字符串
来源：https://vs.zhonguo2118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://av.zhonguo8118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://ii.zhonguo5118.cn

[Q33] 多列分组
来源：https://pa.zhonguo8118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://wb.zhonguo1118.cn

[Q34] 每组取第一条
来源：https://vr.zhonguo2118.cn

SELECT * FROM (
来源：https://ba.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://jn.zhonguo2118.cn

) t WHERE rn = 1;
来源：https://rv.zhonguo1118.cn

[Q35] 内连接
来源：https://zz.zhonguo7118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://el.zhonguo2118.cn

[Q36] 左连接
来源：https://kg.zhonguo4118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://tm.zhonguo6118.cn

[Q37] 右连接
来源：https://jn.zhonguo1118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://jp.zhonguo5118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://qf.zhonguo3118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://or.zhonguo8118.cn

[Q39] 自连接（查上下级）
来源：https://vy.zhonguo2118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://vp.zhonguo1118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://nw.zhonguo4118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://om.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://sy.zhonguo8118.cn

[Q41] 多表连接
来源：https://sk.zhonguo8118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://tk.zhonguo3118.cn

JOIN users u ON u.id = o.user_id
来源：https://ff.zhonguo1118.cn

JOIN products p ON p.id = o.product_id;
来源：https://oy.zhonguo6118.cn

[Q42] 连接条件附加过滤
来源：https://ug.zhonguo5118.cn

SELECT u.name, o.amount FROM users u
来源：https://zr.zhonguo6118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://hq.zhonguo5118.cn

[Q43] 标量子查询
来源：https://jz.zhonguo8118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://it.zhonguo7118.cn

[Q44] IN 子查询
来源：https://ub.zhonguo1118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://pz.zhonguo6118.cn

[Q45] EXISTS 判断存在
来源：https://gc.zhonguo4118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://uc.zhonguo6118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://ni.zhonguo7118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://qh.zhonguo4118.cn

[Q47] 与平均值比较
来源：https://rx.zhonguo6118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://pe.zhonguo2118.cn

[Q48] CTE 公用表表达式
来源：https://zt.zhonguo6118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://uk.zhonguo6118.cn

SELECT * FROM t WHERE c > 5;
来源：https://hb.zhonguo6118.cn

[Q49] 更新单行
来源：https://aa.zhonguo8118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://bb.zhonguo8118.cn

[Q50] 批量更新
来源：https://ti.zhonguo4118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://kn.zhonguo5118.cn

[Q51] 用子查询更新
来源：https://ce.zhonguo4118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://yp.zhonguo5118.cn

[Q52] 删除指定行
来源：https://sf.zhonguo3118.cn

DELETE FROM users WHERE id = 10;
来源：https://jw.zhonguo8118.cn

[Q53] 按条件删除
来源：https://hu.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://ji.zhonguo7118.cn

[Q54] 清空表
来源：https://le.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://jm.zhonguo4118.cn

[Q55] 排名（并列占位）
来源：https://yf.zhonguo8118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://ec.zhonguo2118.cn

[Q56] 密集排名（并列不占位）
来源：https://gd.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://we.zhonguo2118.cn

[Q57] 行号
来源：https://mk.zhonguo4118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://fd.zhonguo8118.cn

[Q58] 累计求和
来源：https://cv.zhonguo1118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://kw.zhonguo3118.cn

[Q59] 分组内累计
来源：https://pb.zhonguo5118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://fn.zhonguo2118.cn

[Q60] 取上一行 / 下一行
来源：https://dc.zhonguo1118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://xm.zhonguo3118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://he.zhonguo7118.cn

[Q61] 移动平均
来源：https://ye.zhonguo4118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://yu.zhonguo8118.cn

[Q62] 分组占比
来源：https://yd.zhonguo5118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://ev.zhonguo5118.cn

[Q63] 开启事务
来源：https://qw.zhonguo7118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://gj.zhonguo6118.cn

[Q64] 提交事务
来源：https://nm.zhonguo2118.cn

COMMIT;
来源：https://dm.zhonguo4118.cn

[Q65] 回滚事务
来源：https://al.zhonguo8118.cn

ROLLBACK;
来源：https://oq.zhonguo8118.cn

[Q66] 行锁查询
来源：https://fm.zhonguo3118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://bd.zhonguo4118.cn

[Q67] 设置隔离级别
来源：https://eu.zhonguo8118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://ka.zhonguo7118.cn

[Q68] 保存点
来源：https://hf.zhonguo7118.cn

SAVEPOINT sp1;
来源：https://vd.zhonguo1118.cn

ROLLBACK TO sp1;
来源：https://yy.zhonguo3118.cn

[Q69] 查看执行计划
来源：https://gi.zhonguo4118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://yf.zhonguo6118.cn

[Q70] 更新统计信息
来源：https://eu.zhonguo6118.cn

ANALYZE TABLE users;
来源：https://ey.zhonguo7118.cn

[Q71] 查看建表语句
来源：https://zw.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://bq.zhonguo3118.cn

[Q72] 查看索引
来源：https://st.zhonguo8118.cn

SHOW INDEX FROM users;
来源：https://ht.zhonguo8118.cn

[Q73] 查看表状态
来源：https://ug.zhonguo4118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://vx.zhonguo7118.cn

[Q74] 强制使用索引
来源：https://xf.zhonguo3118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://ri.zhonguo1118.cn

[Q75] 日期格式化
来源：https://zl.zhonguo6118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://ub.zhonguo4118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://ca.zhonguo4118.cn

[Q76] 按天统计
来源：https://xr.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://lb.zhonguo4118.cn

[Q77] 时间加减
来源：https://hb.zhonguo3118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://uu.zhonguo7118.cn

[Q78] 当前时间
来源：https://tq.zhonguo5118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://ei.zhonguo5118.cn

[Q79] 字符串拼接
来源：https://ql.zhonguo6118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://md.zhonguo3118.cn

[Q80] 字符串截取
来源：https://at.zhonguo3118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://vb.zhonguo5118.cn

[Q81] 字符串替换
来源：https://mw.zhonguo3118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://kz.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://og.zhonguo1118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://uy.zhonguo5118.cn

[Q83] 大小写转换
来源：https://zv.zhonguo8118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://rw.zhonguo2118.cn

[Q84] 去除首尾空格
来源：https://qi.zhonguo1118.cn

SELECT TRIM(name) FROM users;
来源：https://or.zhonguo1118.cn

[Q85] 数值取整
来源：https://ve.zhonguo2118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://fd.zhonguo3118.cn

[Q86] 读取 JSON 字段
来源：https://cv.zhonguo2118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://jy.zhonguo4118.cn

[Q87] JSON 字段做条件
来源：https://hn.zhonguo7118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://ag.zhonguo4118.cn

[Q88] 行转列（条件聚合）
来源：https://im.zhonguo4118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://ea.zhonguo8118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://ns.zhonguo5118.cn

[Q89] 判断表是否存在
来源：https://kx.zhonguo7118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://qt.zhonguo5118.cn

[Q90] 生成序号列
来源：https://xo.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://vz.zhonguo6118.cn

================================================================================
来源：https://sv.zhonguo8118.cn

R. Bash 专题
来源：https://nd.zhonguo4118.cn

================================================================================
来源：https://su.zhonguo6118.cn

[R01] shebang 与严格模式
来源：https://pg.zhonguo7118.cn

#!/usr/bin/env bash
来源：https://iu.zhonguo7118.cn

set -euo pipefail
来源：https://rf.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://pz.zhonguo3118.cn

name="Tom"; echo "$name"
来源：https://bo.zhonguo8118.cn

[R03] 只读变量
来源：https://wl.zhonguo1118.cn

readonly PI=3.14
来源：https://fr.zhonguo4118.cn

[R04] 位置参数
来源：https://cw.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://ky.zhonguo3118.cn

[R05] 参数默认值
来源：https://mx.zhonguo1118.cn

name="${1:-default}"
来源：https://yq.zhonguo7118.cn

[R06] 判断命令是否存在
来源：https://yu.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://uy.zhonguo6118.cn

[R07] if 判断文件
来源：https://vy.zhonguo3118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://ur.zhonguo6118.cn

[R08] 数值比较
来源：https://yo.zhonguo2118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://he.zhonguo6118.cn

[R09] 字符串比较
来源：https://aw.zhonguo8118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ra.zhonguo7118.cn

[R10] 正则匹配
来源：https://lb.zhonguo4118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://po.zhonguo3118.cn

[R11] case 多分支
来源：https://wa.zhonguo1118.cn

case "$1" in
来源：https://zh.zhonguo1118.cn

start) echo "启动" ;;
来源：https://me.zhonguo3118.cn

stop)  echo "停止" ;;
来源：https://yf.zhonguo7118.cn

*)     echo "未知命令" ;;
来源：https://rh.zhonguo6118.cn

esac
来源：https://cp.zhonguo5118.cn

[R12] for 遍历文件
来源：https://hy.zhonguo4118.cn

for f in *.txt; do echo "$f"; done
来源：https://vg.zhonguo8118.cn

[R13] for 计数循环
来源：https://qh.zhonguo3118.cn

for i in {1..10}; do echo "$i"; done
来源：https://et.zhonguo7118.cn

[R14] C 风格 for
来源：https://hd.zhonguo3118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://px.zhonguo6118.cn

[R15] while 逐行读文件
来源：https://wy.zhonguo8118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://tl.zhonguo5118.cn

[R16] until 等待条件
来源：https://tp.zhonguo5118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://ne.zhonguo4118.cn

[R17] 数组定义与取值
来源：https://hl.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://up.zhonguo5118.cn

[R18] 遍历数组
来源：https://fc.zhonguo7118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://tz.zhonguo3118.cn

[R19] 数组长度
来源：https://rm.zhonguo5118.cn

echo "${#arr[@]}"
来源：https://xt.zhonguo2118.cn

[R20] 关联数组（字典）
来源：https://wf.zhonguo3118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://mj.zhonguo3118.cn

[R21] 字符串长度
来源：https://xd.zhonguo2118.cn

echo "${#s}"
来源：https://ph.zhonguo1118.cn

[R22] 截取子串
来源：https://xs.zhonguo3118.cn

echo "${s:0:5}"
来源：https://ct.zhonguo7118.cn

[R23] 字符串替换
来源：https://px.zhonguo6118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://rt.zhonguo3118.cn

[R24] 大小写转换
来源：https://yl.zhonguo8118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://iw.zhonguo1118.cn

[R25] 去后缀 / 去前缀
来源：https://sr.zhonguo5118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://cj.zhonguo4118.cn

[R26] 命令替换
来源：https://be.zhonguo4118.cn

now=$(date +%F); echo "$now"
来源：https://rk.zhonguo8118.cn

[R27] 算术展开
来源：https://ps.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://ua.zhonguo2118.cn

[R28] 浮点运算
来源：https://sx.zhonguo8118.cn

echo "scale=2; 10/3" | bc
来源：https://pl.zhonguo6118.cn

[R29] 定义函数
来源：https://qf.zhonguo6118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://gj.zhonguo3118.cn

[R30] 函数返回状态码
来源：https://tv.zhonguo2118.cn

f() { return 0; }; f || echo "失败了"
来源：https://pd.zhonguo3118.cn

[R31] 局部变量
来源：https://xz.zhonguo2118.cn

f() { local x=1; echo "$x"; }
来源：https://rc.zhonguo6118.cn

[R32] 参数个数校验
来源：https://gy.zhonguo3118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://wb.zhonguo2118.cn

[R33] 捕获错误并提示行号
来源：https://nf.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://pp.zhonguo3118.cn

[R34] 退出时清理
来源：https://ai.zhonguo1118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://bg.zhonguo3118.cn

[R35] 后台执行并等待
来源：https://qy.zhonguo4118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://el.zhonguo1118.cn

[R36] 并发执行多个任务
来源：https://is.zhonguo2118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://pq.zhonguo5118.cn

[R37] 把输出赋给变量
来源：https://uj.zhonguo1118.cn

files=$(ls -1)
来源：https://eh.zhonguo2118.cn

[R38] 管道串联
来源：https://bs.zhonguo7118.cn

cat a.txt | grep -i error | wc -l
来源：https://re.zhonguo6118.cn

[R39] 重定向标准输出与错误
来源：https://xf.zhonguo2118.cn

cmd > out.log 2>&1
来源：https://lr.zhonguo6118.cn

[R40] 追加写日志
来源：https://sr.zhonguo7118.cn

echo "log" >> out.log
来源：https://qy.zhonguo7118.cn

[R41] 丢弃输出
来源：https://xh.zhonguo4118.cn

cmd >/dev/null 2>&1
来源：https://co.zhonguo1118.cn

[R42] 输入重定向
来源：https://vu.zhonguo3118.cn

wc -l < a.txt
来源：https://dd.zhonguo8118.cn

[R43] 按名字查找文件
来源：https://qj.zhonguo8118.cn

find . -name "*.log" -type f
来源：https://dt.zhonguo7118.cn

[R44] 按修改时间查找
来源：https://nx.zhonguo2118.cn

find . -mtime -7 -type f
来源：https://ox.zhonguo8118.cn

[R45] 批量删除
来源：https://iz.zhonguo5118.cn

find . -name "*.tmp" -delete
来源：https://tf.zhonguo2118.cn

[R46] 递归替换文件内容
来源：https://ff.zhonguo6118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://oo.zhonguo6118.cn

[R47] sed 单行替换
来源：https://pg.zhonguo7118.cn


<!-- 参考信息 -->