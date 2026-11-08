代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://kl.zhonguo1118.cn

[Q32] 分组拼接字符串
来源：https://qg.zhonguo6118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://gz.zhonguo6118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://gc.zhonguo5118.cn

[Q33] 多列分组
来源：https://fp.zhonguo7118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://eq.zhonguo5118.cn

[Q34] 每组取第一条
来源：https://xi.zhonguo5118.cn

SELECT * FROM (
来源：https://gq.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://pj.zhonguo5118.cn

) t WHERE rn = 1;
来源：https://zc.zhonguo6118.cn

[Q35] 内连接
来源：https://hu.zhonguo5118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://sd.zhonguo3118.cn

[Q36] 左连接
来源：https://yq.zhonguo8118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://wh.zhonguo1118.cn

[Q37] 右连接
来源：https://rj.zhonguo8118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://nu.zhonguo5118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://pf.zhonguo5118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://ra.zhonguo8118.cn

[Q39] 自连接（查上下级）
来源：https://ks.zhonguo3118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://hd.zhonguo8118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://gl.zhonguo4118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://sx.zhonguo8118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://ua.zhonguo1118.cn

[Q41] 多表连接
来源：https://nw.zhonguo3118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://sd.zhonguo5118.cn

JOIN users u ON u.id = o.user_id
来源：https://xg.zhonguo3118.cn

JOIN products p ON p.id = o.product_id;
来源：https://qe.zhonguo6118.cn

[Q42] 连接条件附加过滤
来源：https://by.zhonguo6118.cn

SELECT u.name, o.amount FROM users u
来源：https://ja.zhonguo2118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://yk.zhonguo3118.cn

[Q43] 标量子查询
来源：https://dg.zhonguo7118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://jp.zhonguo6118.cn

[Q44] IN 子查询
来源：https://sd.zhonguo7118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://qj.zhonguo2118.cn

[Q45] EXISTS 判断存在
来源：https://yq.zhonguo7118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://qs.zhonguo4118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://xo.zhonguo5118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://kx.zhonguo8118.cn

[Q47] 与平均值比较
来源：https://aa.zhonguo8118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://nu.zhonguo1118.cn

[Q48] CTE 公用表表达式
来源：https://hq.zhonguo1118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://yj.zhonguo8118.cn

SELECT * FROM t WHERE c > 5;
来源：https://is.zhonguo5118.cn

[Q49] 更新单行
来源：https://st.zhonguo8118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://mk.zhonguo8118.cn

[Q50] 批量更新
来源：https://nu.zhonguo7118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://kk.zhonguo3118.cn

[Q51] 用子查询更新
来源：https://ts.zhonguo2118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://be.zhonguo5118.cn

[Q52] 删除指定行
来源：https://pn.zhonguo5118.cn

DELETE FROM users WHERE id = 10;
来源：https://eq.zhonguo5118.cn

[Q53] 按条件删除
来源：https://pc.zhonguo5118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://qo.zhonguo6118.cn

[Q54] 清空表
来源：https://vk.zhonguo4118.cn

TRUNCATE TABLE logs;
来源：https://gv.zhonguo2118.cn

[Q55] 排名（并列占位）
来源：https://yv.zhonguo5118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://ge.zhonguo3118.cn

[Q56] 密集排名（并列不占位）
来源：https://bk.zhonguo5118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://yw.zhonguo4118.cn

[Q57] 行号
来源：https://em.zhonguo4118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://fn.zhonguo4118.cn

[Q58] 累计求和
来源：https://xj.zhonguo3118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://jl.zhonguo3118.cn

[Q59] 分组内累计
来源：https://pp.zhonguo1118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://hc.zhonguo3118.cn

[Q60] 取上一行 / 下一行
来源：https://lx.zhonguo6118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://mj.zhonguo1118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://et.zhonguo3118.cn

[Q61] 移动平均
来源：https://gm.zhonguo8118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://ka.zhonguo1118.cn

[Q62] 分组占比
来源：https://yh.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://rr.zhonguo2118.cn

[Q63] 开启事务
来源：https://ec.zhonguo1118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://cq.zhonguo6118.cn

[Q64] 提交事务
来源：https://wo.zhonguo1118.cn

COMMIT;
来源：https://mg.zhonguo5118.cn

[Q65] 回滚事务
来源：https://je.zhonguo6118.cn

ROLLBACK;
来源：https://ge.zhonguo7118.cn

[Q66] 行锁查询
来源：https://yj.zhonguo5118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://zc.zhonguo6118.cn

[Q67] 设置隔离级别
来源：https://tv.zhonguo4118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://kv.zhonguo1118.cn

[Q68] 保存点
来源：https://wh.zhonguo8118.cn

SAVEPOINT sp1;
来源：https://xb.zhonguo6118.cn

ROLLBACK TO sp1;
来源：https://vj.zhonguo8118.cn

[Q69] 查看执行计划
来源：https://sn.zhonguo5118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://fw.zhonguo8118.cn

[Q70] 更新统计信息
来源：https://ii.zhonguo7118.cn

ANALYZE TABLE users;
来源：https://ib.zhonguo4118.cn

[Q71] 查看建表语句
来源：https://dv.zhonguo3118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://mf.zhonguo5118.cn

[Q72] 查看索引
来源：https://tp.zhonguo5118.cn

SHOW INDEX FROM users;
来源：https://ej.zhonguo8118.cn

[Q73] 查看表状态
来源：https://lg.zhonguo7118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://ib.zhonguo5118.cn

[Q74] 强制使用索引
来源：https://mz.zhonguo7118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://fm.zhonguo3118.cn

[Q75] 日期格式化
来源：https://dp.zhonguo6118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://hk.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://kb.zhonguo1118.cn

[Q76] 按天统计
来源：https://by.zhonguo2118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://av.zhonguo1118.cn

[Q77] 时间加减
来源：https://pa.zhonguo7118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://dl.zhonguo8118.cn

[Q78] 当前时间
来源：https://ib.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://ic.zhonguo4118.cn

[Q79] 字符串拼接
来源：https://np.zhonguo1118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://wd.zhonguo7118.cn

[Q80] 字符串截取
来源：https://nd.zhonguo4118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://kz.zhonguo1118.cn

[Q81] 字符串替换
来源：https://db.zhonguo8118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://oa.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://fm.zhonguo1118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://vc.zhonguo6118.cn

[Q83] 大小写转换
来源：https://yp.zhonguo4118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://dj.zhonguo2118.cn

[Q84] 去除首尾空格
来源：https://jm.zhonguo4118.cn

SELECT TRIM(name) FROM users;
来源：https://bn.zhonguo2118.cn

[Q85] 数值取整
来源：https://bd.zhonguo7118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://nu.zhonguo6118.cn

[Q86] 读取 JSON 字段
来源：https://gl.zhonguo4118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://zy.zhonguo1118.cn

[Q87] JSON 字段做条件
来源：https://pq.zhonguo2118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://lk.zhonguo8118.cn

[Q88] 行转列（条件聚合）
来源：https://wc.zhonguo5118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://pq.zhonguo4118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://qd.zhonguo5118.cn

[Q89] 判断表是否存在
来源：https://vd.zhonguo1118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://bg.zhonguo8118.cn

[Q90] 生成序号列
来源：https://cb.zhonguo7118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ai.zhonguo3118.cn

================================================================================
来源：https://nb.zhonguo4118.cn

R. Bash 专题
来源：https://tu.zhonguo6118.cn

================================================================================
来源：https://ks.zhonguo1118.cn

[R01] shebang 与严格模式
来源：https://sh.zhonguo8118.cn

#!/usr/bin/env bash
来源：https://yj.zhonguo4118.cn

set -euo pipefail
来源：https://yd.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://ce.zhonguo8118.cn

name="Tom"; echo "$name"
来源：https://fk.zhonguo8118.cn

[R03] 只读变量
来源：https://go.zhonguo1118.cn

readonly PI=3.14
来源：https://lm.zhonguo3118.cn

[R04] 位置参数
来源：https://rb.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://ro.zhonguo4118.cn

[R05] 参数默认值
来源：https://bl.zhonguo2118.cn

name="${1:-default}"
来源：https://wc.zhonguo1118.cn

[R06] 判断命令是否存在
来源：https://wx.zhonguo2118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://ki.zhonguo8118.cn

[R07] if 判断文件
来源：https://er.zhonguo5118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://ma.zhonguo1118.cn

[R08] 数值比较
来源：https://lr.zhonguo2118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://nf.zhonguo6118.cn

[R09] 字符串比较
来源：https://xc.zhonguo2118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ww.zhonguo1118.cn

[R10] 正则匹配
来源：https://sq.zhonguo7118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://pg.zhonguo1118.cn

[R11] case 多分支
来源：https://zs.zhonguo4118.cn

case "$1" in
来源：https://of.zhonguo4118.cn

start) echo "启动" ;;
来源：https://bf.zhonguo6118.cn

stop)  echo "停止" ;;
来源：https://xw.zhonguo5118.cn

*)     echo "未知命令" ;;
来源：https://yu.zhonguo7118.cn

esac
来源：https://dm.zhonguo6118.cn

[R12] for 遍历文件
来源：https://nv.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://ow.zhonguo3118.cn

[R13] for 计数循环
来源：https://xd.zhonguo6118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ue.zhonguo3118.cn

[R14] C 风格 for
来源：https://dg.zhonguo5118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://cc.zhonguo8118.cn

[R15] while 逐行读文件
来源：https://uy.zhonguo6118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://yn.zhonguo2118.cn

[R16] until 等待条件
来源：https://we.zhonguo6118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://vx.zhonguo3118.cn

[R17] 数组定义与取值
来源：https://fl.zhonguo5118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://rr.zhonguo5118.cn

[R18] 遍历数组
来源：https://ny.zhonguo4118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://zo.zhonguo7118.cn

[R19] 数组长度
来源：https://cl.zhonguo2118.cn

echo "${#arr[@]}"
来源：https://qe.zhonguo5118.cn

[R20] 关联数组（字典）
来源：https://dm.zhonguo4118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://od.zhonguo3118.cn

[R21] 字符串长度
来源：https://tc.zhonguo2118.cn

echo "${#s}"
来源：https://bq.zhonguo3118.cn

[R22] 截取子串
来源：https://rt.zhonguo2118.cn

echo "${s:0:5}"
来源：https://cw.zhonguo6118.cn

[R23] 字符串替换
来源：https://zf.zhonguo7118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://wd.zhonguo6118.cn

[R24] 大小写转换
来源：https://ri.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ps.zhonguo3118.cn

[R25] 去后缀 / 去前缀
来源：https://gw.zhonguo7118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://ji.zhonguo5118.cn

[R26] 命令替换
来源：https://jo.zhonguo5118.cn

now=$(date +%F); echo "$now"
来源：https://xw.zhonguo6118.cn

[R27] 算术展开
来源：https://au.zhonguo3118.cn

echo $((1 + 2 * 3))
来源：https://kc.zhonguo4118.cn

[R28] 浮点运算
来源：https://bx.zhonguo4118.cn

echo "scale=2; 10/3" | bc
来源：https://vi.zhonguo3118.cn

[R29] 定义函数
来源：https://ak.zhonguo7118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://em.zhonguo2118.cn

[R30] 函数返回状态码
来源：https://fr.zhonguo6118.cn

f() { return 0; }; f || echo "失败了"
来源：https://oe.zhonguo4118.cn

[R31] 局部变量
来源：https://du.zhonguo6118.cn

f() { local x=1; echo "$x"; }
来源：https://ty.zhonguo5118.cn

[R32] 参数个数校验
来源：https://pm.zhonguo5118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://zx.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://nh.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://ee.zhonguo5118.cn

[R34] 退出时清理
来源：https://nb.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://da.zhonguo7118.cn

[R35] 后台执行并等待
来源：https://gw.zhonguo3118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://yh.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://df.zhonguo4118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://sz.zhonguo2118.cn

[R37] 把输出赋给变量
来源：https://nz.zhonguo1118.cn

files=$(ls -1)
来源：https://op.zhonguo2118.cn

[R38] 管道串联
来源：https://ra.zhonguo4118.cn

cat a.txt | grep -i error | wc -l
来源：https://fn.zhonguo1118.cn

[R39] 重定向标准输出与错误
来源：https://ek.zhonguo5118.cn

cmd > out.log 2>&1
来源：https://dp.zhonguo4118.cn

[R40] 追加写日志
来源：https://ar.zhonguo7118.cn

echo "log" >> out.log
来源：https://ld.zhonguo3118.cn

[R41] 丢弃输出
来源：https://rn.zhonguo8118.cn

cmd >/dev/null 2>&1
来源：https://em.zhonguo1118.cn

[R42] 输入重定向
来源：https://cb.zhonguo6118.cn

wc -l < a.txt
来源：https://rf.zhonguo1118.cn

[R43] 按名字查找文件
来源：https://st.zhonguo2118.cn

find . -name "*.log" -type f
来源：https://xb.zhonguo5118.cn

[R44] 按修改时间查找
来源：https://rj.zhonguo6118.cn

find . -mtime -7 -type f
来源：https://ce.zhonguo3118.cn

[R45] 批量删除
来源：https://zs.zhonguo1118.cn

find . -name "*.tmp" -delete
来源：https://dm.zhonguo1118.cn

[R46] 递归替换文件内容
来源：https://zm.zhonguo3118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://oe.zhonguo1118.cn

[R47] sed 单行替换
来源：https://lf.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://mb.zhonguo4118.cn

[R48] awk 取指定列
来源：https://tn.zhonguo5118.cn

awk '{print $1, $3}' a.txt
来源：https://rn.zhonguo7118.cn

[R49] awk 带条件
来源：https://ga.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://zu.zhonguo1118.cn

[R50] awk 求和
来源：https://uk.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://re.zhonguo8118.cn

[R51] 排序去重取前几
来源：https://gx.zhonguo5118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://en.zhonguo6118.cn

[R52] 统计行数
来源：https://dl.zhonguo8118.cn

wc -l a.txt
来源：https://jb.zhonguo2118.cn

[R53] 查看文件头与实时尾
来源：https://bf.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://cc.zhonguo4118.cn

[R54] 比较两个文件
来源：https://ls.zhonguo8118.cn

diff a.txt b.txt
来源：https://fj.zhonguo3118.cn

[R55] 压缩与解压
来源：https://mz.zhonguo5118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://hs.zhonguo3118.cn

[R56] 远程拷贝
来源：https://mr.zhonguo6118.cn

scp file user@host:/path/
来源：https://sz.zhonguo3118.cn

[R57] 远程执行命令
来源：https://fh.zhonguo4118.cn

ssh user@host 'uptime'
来源：https://vx.zhonguo3118.cn

[R58] 下载文件
来源：https://hv.zhonguo7118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://dq.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://nm.zhonguo4118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://fq.zhonguo5118.cn

[R60] 只看 HTTP 状态码
来源：https://yd.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://mm.zhonguo6118.cn

[R61] 磁盘占用
来源：https://ee.zhonguo1118.cn

df -h;  du -sh *
来源：https://hj.zhonguo8118.cn

[R62] 找最占空间的文件
来源：https://fl.zhonguo4118.cn

du -ah . | sort -rh | head -10
来源：https://kp.zhonguo4118.cn

[R63] 内存与进程
来源：https://td.zhonguo5118.cn

free -h;  ps aux | grep nginx
来源：https://ta.zhonguo5118.cn

[R64] 结束进程
来源：https://yo.zhonguo2118.cn

kill -9 $(pgrep -f app.py)
来源：https://xr.zhonguo6118.cn

[R65] 查看端口占用
来源：https://zq.zhonguo1118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://wl.zhonguo3118.cn

[R66] 定时任务
来源：https://yh.zhonguo8118.cn

crontab -e;  crontab -l
来源：https://cb.zhonguo6118.cn

[R67] 生成随机十六进制串
来源：https://ic.zhonguo5118.cn

openssl rand -hex 16
来源：https://lv.zhonguo2118.cn

[R68] 计算文件校验值
来源：https://dt.zhonguo7118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://iw.zhonguo5118.cn

[R69] 生成随机密码
来源：https://ab.zhonguo4118.cn

head -c 16 /dev/urandom | base64
来源：https://we.zhonguo8118.cn

[R70] 时间戳与互转
来源：https://rf.zhonguo2118.cn

date +%s;  date -d @1700000000
来源：https://ul.zhonguo7118.cn

[R71] 日期格式化
来源：https://or.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ef.zhonguo1118.cn

[R72] 等待端口就绪
来源：https://zb.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://yb.zhonguo7118.cn

[R73] 分割大日志
来源：https://zh.zhonguo8118.cn

split -l 1000 big.log part_
来源：https://eq.zhonguo8118.cn

[R74] 批量重命名
来源：https://sr.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://tn.zhonguo7118.cn

[R75] 导出环境变量
来源：https://de.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://qj.zhonguo4118.cn

[R76] 使用临时文件
来源：https://sp.zhonguo5118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://bu.zhonguo2118.cn

[R77] 读取用户输入
来源：https://tv.zhonguo7118.cn

read -rp "请输入: " ans
来源：https://vc.zhonguo7118.cn

[R78] 交互式菜单
来源：https://or.zhonguo8118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://pu.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://gf.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://qk.zhonguo2118.cn

[R80] 查看脚本执行耗时
来源：https://ps.zhonguo6118.cn

time ./run.sh
来源：https://ha.zhonguo8118.cn

================================================================================
来源：https://eb.zhonguo5118.cn


<!-- 参考信息 -->