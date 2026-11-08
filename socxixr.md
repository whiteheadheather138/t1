代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：https://px.zhonguo8118.cn

[Q07] 删除表
来源：https://os.zhonguo2118.cn

DROP TABLE IF EXISTS orders;
来源：https://qz.zhonguo8118.cn

[Q08] 创建普通索引
来源：https://pr.zhonguo1118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://iq.zhonguo3118.cn

[Q09] 创建唯一索引
来源：https://km.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://na.zhonguo2118.cn

[Q10] 插入单行
来源：https://ch.zhonguo6118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://jc.zhonguo7118.cn

[Q11] 一次插入多行
来源：https://os.zhonguo4118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://hm.zhonguo7118.cn

[Q12] 插入后取自增 ID
来源：https://bs.zhonguo5118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://kv.zhonguo8118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://sw.zhonguo8118.cn

[Q13] 忽略重复插入
来源：https://vw.zhonguo5118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://gn.zhonguo3118.cn

[Q14] 存在则更新（upsert）
来源：https://of.zhonguo2118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://wv.zhonguo3118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://il.zhonguo1118.cn

[Q15] 查询全部
来源：https://ru.zhonguo5118.cn

SELECT * FROM users;
来源：https://pa.zhonguo7118.cn

[Q16] 查询指定列
来源：https://cl.zhonguo6118.cn

SELECT id, name FROM users;
来源：https://st.zhonguo7118.cn

[Q17] 条件查询
来源：https://qr.zhonguo4118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://mq.zhonguo2118.cn

[Q18] 模糊匹配
来源：https://so.zhonguo3118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://mk.zhonguo6118.cn

[Q19] 范围查询
来源：https://qm.zhonguo6118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://si.zhonguo8118.cn

[Q20] IN 列表
来源：https://tw.zhonguo8118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://on.zhonguo1118.cn

[Q21] 空值判断
来源：https://uj.zhonguo3118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://tz.zhonguo4118.cn

[Q22] 排序
来源：https://qw.zhonguo6118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://ou.zhonguo3118.cn

[Q23] 分页
来源：https://tt.zhonguo4118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://ua.zhonguo7118.cn

[Q24] 去重
来源：https://xs.zhonguo7118.cn

SELECT DISTINCT city FROM users;
来源：https://gb.zhonguo1118.cn

[Q25] 只取前 N 条
来源：https://rl.zhonguo5118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://ff.zhonguo2118.cn

[Q26] 计数
来源：https://ya.zhonguo2118.cn

SELECT COUNT(*) FROM users;
来源：https://xu.zhonguo6118.cn

[Q27] 条件计数
来源：https://mn.zhonguo2118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://oq.zhonguo2118.cn

[Q28] 求和与平均
来源：https://qi.zhonguo4118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://gx.zhonguo3118.cn

[Q29] 最大最小值
来源：https://ql.zhonguo5118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://ma.zhonguo7118.cn

[Q30] 分组统计
来源：https://yk.zhonguo1118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://po.zhonguo1118.cn

[Q31] 分组后过滤
来源：https://xn.zhonguo1118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://yy.zhonguo4118.cn

[Q32] 分组拼接字符串
来源：https://wq.zhonguo7118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://hm.zhonguo8118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://vc.zhonguo5118.cn

[Q33] 多列分组
来源：https://mn.zhonguo1118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ga.zhonguo4118.cn

[Q34] 每组取第一条
来源：https://hq.zhonguo3118.cn

SELECT * FROM (
来源：https://oa.zhonguo2118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://wc.zhonguo8118.cn

) t WHERE rn = 1;
来源：https://qd.zhonguo3118.cn

[Q35] 内连接
来源：https://jj.zhonguo5118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://ia.zhonguo7118.cn

[Q36] 左连接
来源：https://gn.zhonguo7118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://kt.zhonguo5118.cn

[Q37] 右连接
来源：https://wq.zhonguo4118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://cz.zhonguo4118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://jt.zhonguo2118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://zj.zhonguo3118.cn

[Q39] 自连接（查上下级）
来源：https://ov.zhonguo4118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://hi.zhonguo6118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://qb.zhonguo4118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://kd.zhonguo3118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://tn.zhonguo1118.cn

[Q41] 多表连接
来源：https://lf.zhonguo8118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://vx.zhonguo1118.cn

JOIN users u ON u.id = o.user_id
来源：https://ka.zhonguo2118.cn

JOIN products p ON p.id = o.product_id;
来源：https://vq.zhonguo4118.cn

[Q42] 连接条件附加过滤
来源：https://lp.zhonguo8118.cn

SELECT u.name, o.amount FROM users u
来源：https://qr.zhonguo6118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://hv.zhonguo3118.cn

[Q43] 标量子查询
来源：https://fr.zhonguo5118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://oc.zhonguo5118.cn

[Q44] IN 子查询
来源：https://gq.zhonguo4118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://vi.zhonguo2118.cn

[Q45] EXISTS 判断存在
来源：https://ds.zhonguo2118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://sy.zhonguo8118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://ll.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://zv.zhonguo8118.cn

[Q47] 与平均值比较
来源：https://iw.zhonguo5118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://hq.zhonguo2118.cn

[Q48] CTE 公用表表达式
来源：https://wx.zhonguo6118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://co.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://yg.zhonguo7118.cn

[Q49] 更新单行
来源：https://gm.zhonguo1118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://mk.zhonguo5118.cn

[Q50] 批量更新
来源：https://iz.zhonguo3118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://yj.zhonguo2118.cn

[Q51] 用子查询更新
来源：https://id.zhonguo8118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://hh.zhonguo2118.cn

[Q52] 删除指定行
来源：https://wt.zhonguo6118.cn

DELETE FROM users WHERE id = 10;
来源：https://rs.zhonguo2118.cn

[Q53] 按条件删除
来源：https://vp.zhonguo2118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://bk.zhonguo5118.cn

[Q54] 清空表
来源：https://ur.zhonguo6118.cn

TRUNCATE TABLE logs;
来源：https://gb.zhonguo6118.cn

[Q55] 排名（并列占位）
来源：https://sr.zhonguo1118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://ce.zhonguo5118.cn

[Q56] 密集排名（并列不占位）
来源：https://vf.zhonguo5118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://rd.zhonguo7118.cn

[Q57] 行号
来源：https://vl.zhonguo7118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://bx.zhonguo6118.cn

[Q58] 累计求和
来源：https://yg.zhonguo5118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://vw.zhonguo6118.cn

[Q59] 分组内累计
来源：https://kk.zhonguo6118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://xa.zhonguo5118.cn

[Q60] 取上一行 / 下一行
来源：https://fm.zhonguo2118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://gj.zhonguo6118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://fj.zhonguo8118.cn

[Q61] 移动平均
来源：https://tn.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://tr.zhonguo8118.cn

[Q62] 分组占比
来源：https://de.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://cj.zhonguo4118.cn

[Q63] 开启事务
来源：https://jd.zhonguo4118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://at.zhonguo5118.cn

[Q64] 提交事务
来源：https://kk.zhonguo8118.cn

COMMIT;
来源：https://jl.zhonguo2118.cn

[Q65] 回滚事务
来源：https://vl.zhonguo6118.cn

ROLLBACK;
来源：https://fy.zhonguo6118.cn

[Q66] 行锁查询
来源：https://jq.zhonguo4118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://pb.zhonguo8118.cn

[Q67] 设置隔离级别
来源：https://rh.zhonguo2118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://if.zhonguo7118.cn

[Q68] 保存点
来源：https://ov.zhonguo3118.cn

SAVEPOINT sp1;
来源：https://pp.zhonguo1118.cn

ROLLBACK TO sp1;
来源：https://hb.zhonguo4118.cn

[Q69] 查看执行计划
来源：https://pp.zhonguo3118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://qz.zhonguo4118.cn

[Q70] 更新统计信息
来源：https://ay.zhonguo3118.cn

ANALYZE TABLE users;
来源：https://er.zhonguo6118.cn

[Q71] 查看建表语句
来源：https://dj.zhonguo1118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://pa.zhonguo2118.cn

[Q72] 查看索引
来源：https://ke.zhonguo6118.cn

SHOW INDEX FROM users;
来源：https://iy.zhonguo5118.cn

[Q73] 查看表状态
来源：https://am.zhonguo8118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://sy.zhonguo1118.cn

[Q74] 强制使用索引
来源：https://lq.zhonguo1118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://so.zhonguo5118.cn

[Q75] 日期格式化
来源：https://tb.zhonguo4118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://ym.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://om.zhonguo7118.cn

[Q76] 按天统计
来源：https://zf.zhonguo2118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ub.zhonguo1118.cn

[Q77] 时间加减
来源：https://td.zhonguo1118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://ol.zhonguo5118.cn

[Q78] 当前时间
来源：https://kr.zhonguo8118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://oi.zhonguo7118.cn

[Q79] 字符串拼接
来源：https://jv.zhonguo4118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://eg.zhonguo6118.cn

[Q80] 字符串截取
来源：https://ao.zhonguo3118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://fa.zhonguo5118.cn

[Q81] 字符串替换
来源：https://qf.zhonguo3118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://bf.zhonguo7118.cn

[Q82] 字符长度与字节长度
来源：https://xb.zhonguo3118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://br.zhonguo7118.cn

[Q83] 大小写转换
来源：https://se.zhonguo7118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://wr.zhonguo7118.cn

[Q84] 去除首尾空格
来源：https://ne.zhonguo6118.cn

SELECT TRIM(name) FROM users;
来源：https://ly.zhonguo6118.cn

[Q85] 数值取整
来源：https://pk.zhonguo4118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://sv.zhonguo3118.cn

[Q86] 读取 JSON 字段
来源：https://wn.zhonguo5118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://lc.zhonguo8118.cn

[Q87] JSON 字段做条件
来源：https://uk.zhonguo7118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://wh.zhonguo6118.cn

[Q88] 行转列（条件聚合）
来源：https://xh.zhonguo6118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://wy.zhonguo3118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://wl.zhonguo5118.cn

[Q89] 判断表是否存在
来源：https://dy.zhonguo5118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://th.zhonguo1118.cn

[Q90] 生成序号列
来源：https://vk.zhonguo8118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ll.zhonguo2118.cn

================================================================================
来源：https://vm.zhonguo4118.cn

R. Bash 专题
来源：https://ec.zhonguo5118.cn

================================================================================
来源：https://fz.zhonguo3118.cn

[R01] shebang 与严格模式
来源：https://by.zhonguo3118.cn

#!/usr/bin/env bash
来源：https://fx.zhonguo4118.cn

set -euo pipefail
来源：https://ay.zhonguo1118.cn

[R02] 变量赋值与使用
来源：https://xi.zhonguo4118.cn

name="Tom"; echo "$name"
来源：https://ud.zhonguo2118.cn

[R03] 只读变量
来源：https://zh.zhonguo6118.cn

readonly PI=3.14
来源：https://ln.zhonguo1118.cn

[R04] 位置参数
来源：https://kq.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://ab.zhonguo2118.cn

[R05] 参数默认值
来源：https://zy.zhonguo7118.cn

name="${1:-default}"
来源：https://bw.zhonguo2118.cn

[R06] 判断命令是否存在
来源：https://yc.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://wr.zhonguo8118.cn

[R07] if 判断文件
来源：https://ab.zhonguo6118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://ni.zhonguo1118.cn

[R08] 数值比较
来源：https://ri.zhonguo6118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ue.zhonguo8118.cn

[R09] 字符串比较
来源：https://sn.zhonguo1118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ot.zhonguo7118.cn

[R10] 正则匹配
来源：https://vv.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://af.zhonguo5118.cn

[R11] case 多分支
来源：https://jd.zhonguo6118.cn

case "$1" in
来源：https://rr.zhonguo7118.cn

start) echo "启动" ;;
来源：https://rn.zhonguo2118.cn

stop)  echo "停止" ;;
来源：https://ot.zhonguo2118.cn

*)     echo "未知命令" ;;
来源：https://iv.zhonguo3118.cn

esac
来源：https://ny.zhonguo6118.cn

[R12] for 遍历文件
来源：https://mi.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://wo.zhonguo2118.cn

[R13] for 计数循环
来源：https://ib.zhonguo1118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ld.zhonguo6118.cn

[R14] C 风格 for
来源：https://gx.zhonguo5118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://sf.zhonguo4118.cn

[R15] while 逐行读文件
来源：https://gx.zhonguo2118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://bb.zhonguo5118.cn

[R16] until 等待条件
来源：https://fd.zhonguo3118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://qh.zhonguo7118.cn

[R17] 数组定义与取值
来源：https://ci.zhonguo6118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://yy.zhonguo4118.cn

[R18] 遍历数组
来源：https://jd.zhonguo4118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://ir.zhonguo4118.cn

[R19] 数组长度
来源：https://fx.zhonguo8118.cn

echo "${#arr[@]}"
来源：https://vf.zhonguo1118.cn

[R20] 关联数组（字典）
来源：https://oc.zhonguo4118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://fw.zhonguo3118.cn

[R21] 字符串长度
来源：https://rq.zhonguo1118.cn

echo "${#s}"
来源：https://pd.zhonguo6118.cn

[R22] 截取子串
来源：https://sl.zhonguo5118.cn

echo "${s:0:5}"
来源：https://li.zhonguo7118.cn

[R23] 字符串替换
来源：https://kd.zhonguo6118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://hm.zhonguo3118.cn

[R24] 大小写转换
来源：https://xn.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://py.zhonguo1118.cn

[R25] 去后缀 / 去前缀
来源：https://ta.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://by.zhonguo3118.cn

[R26] 命令替换
来源：https://jp.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://vb.zhonguo4118.cn

[R27] 算术展开
来源：https://tl.zhonguo7118.cn

echo $((1 + 2 * 3))
来源：https://ml.zhonguo7118.cn

[R28] 浮点运算
来源：https://zn.zhonguo6118.cn

echo "scale=2; 10/3" | bc
来源：https://uj.zhonguo1118.cn

[R29] 定义函数
来源：https://ih.zhonguo3118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://un.zhonguo5118.cn

[R30] 函数返回状态码
来源：https://xn.zhonguo3118.cn

f() { return 0; }; f || echo "失败了"
来源：https://gj.zhonguo1118.cn

[R31] 局部变量
来源：https://zr.zhonguo4118.cn

f() { local x=1; echo "$x"; }
来源：https://nu.zhonguo8118.cn

[R32] 参数个数校验
来源：https://tc.zhonguo1118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://fm.zhonguo3118.cn

[R33] 捕获错误并提示行号
来源：https://ej.zhonguo3118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://dx.zhonguo2118.cn

[R34] 退出时清理
来源：https://hl.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://kr.zhonguo6118.cn

[R35] 后台执行并等待
来源：https://ay.zhonguo7118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://yp.zhonguo5118.cn

[R36] 并发执行多个任务
来源：https://ol.zhonguo7118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://fs.zhonguo3118.cn

[R37] 把输出赋给变量
来源：https://vn.zhonguo4118.cn

files=$(ls -1)
来源：https://nf.zhonguo5118.cn

[R38] 管道串联
来源：https://kb.zhonguo8118.cn

cat a.txt | grep -i error | wc -l
来源：https://sd.zhonguo4118.cn

[R39] 重定向标准输出与错误
来源：https://my.zhonguo5118.cn

cmd > out.log 2>&1
来源：https://sm.zhonguo2118.cn

[R40] 追加写日志
来源：https://og.zhonguo8118.cn

echo "log" >> out.log
来源：https://hf.zhonguo7118.cn

[R41] 丢弃输出
来源：https://yf.zhonguo8118.cn

cmd >/dev/null 2>&1
来源：https://nb.zhonguo3118.cn

[R42] 输入重定向
来源：https://gm.zhonguo3118.cn

wc -l < a.txt
来源：https://jk.zhonguo6118.cn

[R43] 按名字查找文件
来源：https://bf.zhonguo2118.cn

find . -name "*.log" -type f
来源：https://vx.zhonguo3118.cn

[R44] 按修改时间查找
来源：https://tz.zhonguo3118.cn

find . -mtime -7 -type f
来源：https://er.zhonguo4118.cn

[R45] 批量删除
来源：https://xr.zhonguo4118.cn

find . -name "*.tmp" -delete
来源：https://ap.zhonguo6118.cn

[R46] 递归替换文件内容
来源：https://bn.zhonguo1118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://ou.zhonguo2118.cn

[R47] sed 单行替换
来源：https://xb.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://xp.zhonguo6118.cn

[R48] awk 取指定列
来源：https://qb.zhonguo7118.cn

awk '{print $1, $3}' a.txt
来源：https://uz.zhonguo5118.cn

[R49] awk 带条件
来源：https://hf.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ep.zhonguo4118.cn

[R50] awk 求和
来源：https://xc.zhonguo4118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://xg.zhonguo1118.cn

[R51] 排序去重取前几
来源：https://yg.zhonguo7118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://gz.zhonguo2118.cn

[R52] 统计行数
来源：https://pp.zhonguo7118.cn

wc -l a.txt
来源：https://yg.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://zz.zhonguo2118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://uv.zhonguo8118.cn

[R54] 比较两个文件
来源：https://za.zhonguo7118.cn

diff a.txt b.txt
来源：https://fg.zhonguo6118.cn

[R55] 压缩与解压
来源：https://hu.zhonguo2118.cn


<!-- 参考信息 -->