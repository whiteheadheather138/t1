代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://yc.zhonguo6118.cn

[Q11] 一次插入多行
来源：https://zn.zhonguo4118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://ft.zhonguo5118.cn

[Q12] 插入后取自增 ID
来源：https://me.zhonguo3118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://bt.zhonguo1118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://so.zhonguo4118.cn

[Q13] 忽略重复插入
来源：https://py.zhonguo4118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://jk.zhonguo4118.cn

[Q14] 存在则更新（upsert）
来源：https://tr.zhonguo2118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://gs.zhonguo7118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://av.zhonguo6118.cn

[Q15] 查询全部
来源：https://hr.zhonguo8118.cn

SELECT * FROM users;
来源：https://zv.zhonguo8118.cn

[Q16] 查询指定列
来源：https://lo.zhonguo3118.cn

SELECT id, name FROM users;
来源：https://bl.zhonguo5118.cn

[Q17] 条件查询
来源：https://ff.zhonguo2118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://ow.zhonguo3118.cn

[Q18] 模糊匹配
来源：https://yz.zhonguo4118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://af.zhonguo6118.cn

[Q19] 范围查询
来源：https://gl.zhonguo1118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://bz.zhonguo5118.cn

[Q20] IN 列表
来源：https://le.zhonguo4118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://cg.zhonguo8118.cn

[Q21] 空值判断
来源：https://gv.zhonguo7118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://cx.zhonguo4118.cn

[Q22] 排序
来源：https://kr.zhonguo1118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://qb.zhonguo2118.cn

[Q23] 分页
来源：https://tr.zhonguo2118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://mi.zhonguo5118.cn

[Q24] 去重
来源：https://xb.zhonguo1118.cn

SELECT DISTINCT city FROM users;
来源：https://pe.zhonguo1118.cn

[Q25] 只取前 N 条
来源：https://gc.zhonguo1118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://bf.zhonguo6118.cn

[Q26] 计数
来源：https://zi.zhonguo8118.cn

SELECT COUNT(*) FROM users;
来源：https://xb.zhonguo5118.cn

[Q27] 条件计数
来源：https://hl.zhonguo2118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://rd.zhonguo4118.cn

[Q28] 求和与平均
来源：https://le.zhonguo7118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://ol.zhonguo6118.cn

[Q29] 最大最小值
来源：https://dw.zhonguo8118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://ha.zhonguo1118.cn

[Q30] 分组统计
来源：https://ag.zhonguo3118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://qs.zhonguo4118.cn

[Q31] 分组后过滤
来源：https://fx.zhonguo5118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://tt.zhonguo3118.cn

[Q32] 分组拼接字符串
来源：https://ly.zhonguo3118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://of.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://ak.zhonguo2118.cn

[Q33] 多列分组
来源：https://ru.zhonguo3118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://yo.zhonguo5118.cn

[Q34] 每组取第一条
来源：https://fz.zhonguo6118.cn

SELECT * FROM (
来源：https://tc.zhonguo8118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://wk.zhonguo3118.cn

) t WHERE rn = 1;
来源：https://gw.zhonguo8118.cn

[Q35] 内连接
来源：https://vv.zhonguo5118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://pj.zhonguo4118.cn

[Q36] 左连接
来源：https://kk.zhonguo3118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://er.zhonguo4118.cn

[Q37] 右连接
来源：https://ca.zhonguo8118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://kl.zhonguo1118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://fw.zhonguo1118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://vy.zhonguo2118.cn

[Q39] 自连接（查上下级）
来源：https://jr.zhonguo7118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://rx.zhonguo3118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://mc.zhonguo5118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://ii.zhonguo7118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://lm.zhonguo7118.cn

[Q41] 多表连接
来源：https://ku.zhonguo6118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://uh.zhonguo3118.cn

JOIN users u ON u.id = o.user_id
来源：https://oe.zhonguo1118.cn

JOIN products p ON p.id = o.product_id;
来源：https://ns.zhonguo8118.cn

[Q42] 连接条件附加过滤
来源：https://re.zhonguo8118.cn

SELECT u.name, o.amount FROM users u
来源：https://oy.zhonguo7118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://cd.zhonguo3118.cn

[Q43] 标量子查询
来源：https://sn.zhonguo8118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://im.zhonguo3118.cn

[Q44] IN 子查询
来源：https://zu.zhonguo3118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://my.zhonguo2118.cn

[Q45] EXISTS 判断存在
来源：https://sp.zhonguo7118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://jx.zhonguo1118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://rg.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://mc.zhonguo3118.cn

[Q47] 与平均值比较
来源：https://yi.zhonguo3118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://ie.zhonguo1118.cn

[Q48] CTE 公用表表达式
来源：https://xb.zhonguo1118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://fg.zhonguo6118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ez.zhonguo4118.cn

[Q49] 更新单行
来源：https://dp.zhonguo1118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://tr.zhonguo2118.cn

[Q50] 批量更新
来源：https://rs.zhonguo4118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://gt.zhonguo8118.cn

[Q51] 用子查询更新
来源：https://cf.zhonguo8118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://yb.zhonguo4118.cn

[Q52] 删除指定行
来源：https://qa.zhonguo8118.cn

DELETE FROM users WHERE id = 10;
来源：https://ac.zhonguo4118.cn

[Q53] 按条件删除
来源：https://yx.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://jt.zhonguo6118.cn

[Q54] 清空表
来源：https://qm.zhonguo7118.cn

TRUNCATE TABLE logs;
来源：https://ty.zhonguo1118.cn

[Q55] 排名（并列占位）
来源：https://hy.zhonguo5118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://hs.zhonguo4118.cn

[Q56] 密集排名（并列不占位）
来源：https://tn.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://jq.zhonguo1118.cn

[Q57] 行号
来源：https://fq.zhonguo3118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://ne.zhonguo2118.cn

[Q58] 累计求和
来源：https://qq.zhonguo7118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://sd.zhonguo7118.cn

[Q59] 分组内累计
来源：https://kr.zhonguo1118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://wj.zhonguo6118.cn

[Q60] 取上一行 / 下一行
来源：https://qj.zhonguo3118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://ym.zhonguo1118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://ue.zhonguo8118.cn

[Q61] 移动平均
来源：https://bl.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://zt.zhonguo7118.cn

[Q62] 分组占比
来源：https://vk.zhonguo8118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://ik.zhonguo7118.cn

[Q63] 开启事务
来源：https://hx.zhonguo3118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://re.zhonguo8118.cn

[Q64] 提交事务
来源：https://kp.zhonguo5118.cn

COMMIT;
来源：https://er.zhonguo4118.cn

[Q65] 回滚事务
来源：https://yr.zhonguo7118.cn

ROLLBACK;
来源：https://nq.zhonguo6118.cn

[Q66] 行锁查询
来源：https://lc.zhonguo4118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://oo.zhonguo5118.cn

[Q67] 设置隔离级别
来源：https://px.zhonguo3118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://sl.zhonguo6118.cn

[Q68] 保存点
来源：https://ou.zhonguo3118.cn

SAVEPOINT sp1;
来源：https://kz.zhonguo5118.cn

ROLLBACK TO sp1;
来源：https://rx.zhonguo1118.cn

[Q69] 查看执行计划
来源：https://hp.zhonguo7118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://ly.zhonguo6118.cn

[Q70] 更新统计信息
来源：https://jx.zhonguo5118.cn

ANALYZE TABLE users;
来源：https://up.zhonguo7118.cn

[Q71] 查看建表语句
来源：https://bv.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://wb.zhonguo2118.cn

[Q72] 查看索引
来源：https://sx.zhonguo2118.cn

SHOW INDEX FROM users;
来源：https://ao.zhonguo1118.cn

[Q73] 查看表状态
来源：https://dl.zhonguo2118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://qc.zhonguo8118.cn

[Q74] 强制使用索引
来源：https://gq.zhonguo8118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://gb.zhonguo6118.cn

[Q75] 日期格式化
来源：https://mm.zhonguo7118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://mq.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://by.zhonguo1118.cn

[Q76] 按天统计
来源：https://ur.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://se.zhonguo3118.cn

[Q77] 时间加减
来源：https://zq.zhonguo5118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://cb.zhonguo7118.cn

[Q78] 当前时间
来源：https://mo.zhonguo3118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://qn.zhonguo7118.cn

[Q79] 字符串拼接
来源：https://wg.zhonguo4118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://fh.zhonguo5118.cn

[Q80] 字符串截取
来源：https://bz.zhonguo7118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://ly.zhonguo1118.cn

[Q81] 字符串替换
来源：https://ab.zhonguo5118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://zn.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://hu.zhonguo8118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://jm.zhonguo5118.cn

[Q83] 大小写转换
来源：https://an.zhonguo8118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://it.zhonguo2118.cn

[Q84] 去除首尾空格
来源：https://vm.zhonguo3118.cn

SELECT TRIM(name) FROM users;
来源：https://rg.zhonguo2118.cn

[Q85] 数值取整
来源：https://oc.zhonguo3118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://ih.zhonguo8118.cn

[Q86] 读取 JSON 字段
来源：https://ce.zhonguo8118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://oh.zhonguo7118.cn

[Q87] JSON 字段做条件
来源：https://tn.zhonguo2118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://hs.zhonguo7118.cn

[Q88] 行转列（条件聚合）
来源：https://cr.zhonguo6118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://pv.zhonguo2118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://tf.zhonguo7118.cn

[Q89] 判断表是否存在
来源：https://jj.zhonguo3118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://at.zhonguo8118.cn

[Q90] 生成序号列
来源：https://ew.zhonguo1118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://pu.zhonguo5118.cn

================================================================================
来源：https://po.zhonguo3118.cn

R. Bash 专题
来源：https://ap.zhonguo4118.cn

================================================================================
来源：https://cp.zhonguo6118.cn

[R01] shebang 与严格模式
来源：https://hq.zhonguo6118.cn

#!/usr/bin/env bash
来源：https://nw.zhonguo2118.cn

set -euo pipefail
来源：https://lo.zhonguo2118.cn

[R02] 变量赋值与使用
来源：https://ld.zhonguo6118.cn

name="Tom"; echo "$name"
来源：https://wa.zhonguo2118.cn

[R03] 只读变量
来源：https://ls.zhonguo5118.cn

readonly PI=3.14
来源：https://bn.zhonguo3118.cn

[R04] 位置参数
来源：https://bb.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://rv.zhonguo6118.cn

[R05] 参数默认值
来源：https://sj.zhonguo1118.cn

name="${1:-default}"
来源：https://qr.zhonguo4118.cn

[R06] 判断命令是否存在
来源：https://dr.zhonguo5118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://mp.zhonguo6118.cn

[R07] if 判断文件
来源：https://su.zhonguo6118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://pc.zhonguo4118.cn

[R08] 数值比较
来源：https://oa.zhonguo5118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://xy.zhonguo3118.cn

[R09] 字符串比较
来源：https://ex.zhonguo5118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://st.zhonguo2118.cn

[R10] 正则匹配
来源：https://jd.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ot.zhonguo1118.cn

[R11] case 多分支
来源：https://bc.zhonguo6118.cn

case "$1" in
来源：https://zb.zhonguo8118.cn

start) echo "启动" ;;
来源：https://ah.zhonguo6118.cn

stop)  echo "停止" ;;
来源：https://aw.zhonguo4118.cn

*)     echo "未知命令" ;;
来源：https://bv.zhonguo6118.cn

esac
来源：https://rp.zhonguo1118.cn

[R12] for 遍历文件
来源：https://kk.zhonguo4118.cn

for f in *.txt; do echo "$f"; done
来源：https://ai.zhonguo5118.cn

[R13] for 计数循环
来源：https://jx.zhonguo6118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ru.zhonguo4118.cn

[R14] C 风格 for
来源：https://vh.zhonguo1118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://ko.zhonguo2118.cn

[R15] while 逐行读文件
来源：https://ys.zhonguo8118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://cs.zhonguo5118.cn

[R16] until 等待条件
来源：https://mz.zhonguo6118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://kn.zhonguo8118.cn

[R17] 数组定义与取值
来源：https://lf.zhonguo8118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://tt.zhonguo7118.cn

[R18] 遍历数组
来源：https://id.zhonguo4118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://ge.zhonguo7118.cn

[R19] 数组长度
来源：https://qp.zhonguo6118.cn

echo "${#arr[@]}"
来源：https://zf.zhonguo2118.cn

[R20] 关联数组（字典）
来源：https://hn.zhonguo7118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://nh.zhonguo6118.cn

[R21] 字符串长度
来源：https://wm.zhonguo7118.cn

echo "${#s}"
来源：https://sc.zhonguo5118.cn

[R22] 截取子串
来源：https://nh.zhonguo1118.cn

echo "${s:0:5}"
来源：https://vs.zhonguo8118.cn

[R23] 字符串替换
来源：https://di.zhonguo2118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://xd.zhonguo2118.cn

[R24] 大小写转换
来源：https://ng.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://co.zhonguo3118.cn

[R25] 去后缀 / 去前缀
来源：https://vl.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://yn.zhonguo4118.cn

[R26] 命令替换
来源：https://hi.zhonguo8118.cn

now=$(date +%F); echo "$now"
来源：https://mr.zhonguo3118.cn

[R27] 算术展开
来源：https://po.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://tg.zhonguo1118.cn

[R28] 浮点运算
来源：https://mi.zhonguo7118.cn

echo "scale=2; 10/3" | bc
来源：https://hr.zhonguo5118.cn

[R29] 定义函数
来源：https://gm.zhonguo6118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://en.zhonguo2118.cn

[R30] 函数返回状态码
来源：https://ay.zhonguo4118.cn

f() { return 0; }; f || echo "失败了"
来源：https://bp.zhonguo8118.cn

[R31] 局部变量
来源：https://nr.zhonguo4118.cn

f() { local x=1; echo "$x"; }
来源：https://zn.zhonguo8118.cn

[R32] 参数个数校验
来源：https://ui.zhonguo8118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://zj.zhonguo2118.cn

[R33] 捕获错误并提示行号
来源：https://tm.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://oo.zhonguo3118.cn

[R34] 退出时清理
来源：https://wf.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://sp.zhonguo6118.cn

[R35] 后台执行并等待
来源：https://rs.zhonguo8118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://vy.zhonguo4118.cn

[R36] 并发执行多个任务
来源：https://jp.zhonguo3118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://mn.zhonguo7118.cn

[R37] 把输出赋给变量
来源：https://rm.zhonguo6118.cn

files=$(ls -1)
来源：https://mj.zhonguo3118.cn

[R38] 管道串联
来源：https://wd.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://dz.zhonguo8118.cn

[R39] 重定向标准输出与错误
来源：https://qt.zhonguo7118.cn

cmd > out.log 2>&1
来源：https://ob.zhonguo5118.cn

[R40] 追加写日志
来源：https://wa.zhonguo2118.cn

echo "log" >> out.log
来源：https://kp.zhonguo5118.cn

[R41] 丢弃输出
来源：https://ip.zhonguo5118.cn

cmd >/dev/null 2>&1
来源：https://mi.zhonguo5118.cn

[R42] 输入重定向
来源：https://qk.zhonguo3118.cn

wc -l < a.txt
来源：https://zq.zhonguo5118.cn

[R43] 按名字查找文件
来源：https://zy.zhonguo3118.cn

find . -name "*.log" -type f
来源：https://wj.zhonguo7118.cn

[R44] 按修改时间查找
来源：https://ue.zhonguo4118.cn

find . -mtime -7 -type f
来源：https://at.zhonguo7118.cn

[R45] 批量删除
来源：https://sm.zhonguo1118.cn

find . -name "*.tmp" -delete
来源：https://rq.zhonguo7118.cn

[R46] 递归替换文件内容
来源：https://wn.zhonguo3118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://lj.zhonguo6118.cn

[R47] sed 单行替换
来源：https://vn.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://ju.zhonguo2118.cn

[R48] awk 取指定列
来源：https://gm.zhonguo2118.cn

awk '{print $1, $3}' a.txt
来源：https://yq.zhonguo4118.cn

[R49] awk 带条件
来源：https://vk.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://sa.zhonguo3118.cn

[R50] awk 求和
来源：https://ka.zhonguo3118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://kc.zhonguo6118.cn

[R51] 排序去重取前几
来源：https://mp.zhonguo5118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://ss.zhonguo8118.cn

[R52] 统计行数
来源：https://nr.zhonguo8118.cn

wc -l a.txt
来源：https://ki.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://bu.zhonguo6118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://vk.zhonguo8118.cn

[R54] 比较两个文件
来源：https://nz.zhonguo5118.cn

diff a.txt b.txt
来源：https://hy.zhonguo7118.cn

[R55] 压缩与解压
来源：https://gz.zhonguo2118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://wj.zhonguo8118.cn

[R56] 远程拷贝
来源：https://dj.zhonguo2118.cn

scp file user@host:/path/
来源：https://ku.zhonguo5118.cn

[R57] 远程执行命令
来源：https://iq.zhonguo3118.cn

ssh user@host 'uptime'
来源：https://vo.zhonguo5118.cn

[R58] 下载文件
来源：https://qw.zhonguo3118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://yx.zhonguo6118.cn

[R59] 发 POST JSON
来源：https://iq.zhonguo3118.cn


<!-- 参考信息 -->