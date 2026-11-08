代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://mb.zhonguo7118.cn

[Q32] 分组拼接字符串
来源：https://yg.zhonguo8118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://hr.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://zq.zhonguo6118.cn

[Q33] 多列分组
来源：https://io.zhonguo8118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://im.zhonguo6118.cn

[Q34] 每组取第一条
来源：https://du.zhonguo8118.cn

SELECT * FROM (
来源：https://aj.zhonguo7118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://ua.zhonguo7118.cn

) t WHERE rn = 1;
来源：https://fk.zhonguo3118.cn

[Q35] 内连接
来源：https://ln.zhonguo1118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://xp.zhonguo5118.cn

[Q36] 左连接
来源：https://rp.zhonguo1118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://yr.zhonguo1118.cn

[Q37] 右连接
来源：https://le.zhonguo4118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://sh.zhonguo2118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://jh.zhonguo5118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://lp.zhonguo4118.cn

[Q39] 自连接（查上下级）
来源：https://mx.zhonguo1118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://rp.zhonguo3118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://rl.zhonguo7118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://mx.zhonguo3118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://nb.zhonguo1118.cn

[Q41] 多表连接
来源：https://ed.zhonguo3118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://qa.zhonguo5118.cn

JOIN users u ON u.id = o.user_id
来源：https://zp.zhonguo1118.cn

JOIN products p ON p.id = o.product_id;
来源：https://up.zhonguo3118.cn

[Q42] 连接条件附加过滤
来源：https://rk.zhonguo2118.cn

SELECT u.name, o.amount FROM users u
来源：https://jh.zhonguo6118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://ox.zhonguo4118.cn

[Q43] 标量子查询
来源：https://dt.zhonguo1118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://eb.zhonguo3118.cn

[Q44] IN 子查询
来源：https://bb.zhonguo3118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://di.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://xc.zhonguo7118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://ju.zhonguo6118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://tz.zhonguo2118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://su.zhonguo1118.cn

[Q47] 与平均值比较
来源：https://wl.zhonguo5118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://bt.zhonguo6118.cn

[Q48] CTE 公用表表达式
来源：https://zu.zhonguo8118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://oa.zhonguo5118.cn

SELECT * FROM t WHERE c > 5;
来源：https://ae.zhonguo5118.cn

[Q49] 更新单行
来源：https://lz.zhonguo4118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://rp.zhonguo7118.cn

[Q50] 批量更新
来源：https://qg.zhonguo5118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://kt.zhonguo6118.cn

[Q51] 用子查询更新
来源：https://qy.zhonguo3118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://xy.zhonguo2118.cn

[Q52] 删除指定行
来源：https://dv.zhonguo6118.cn

DELETE FROM users WHERE id = 10;
来源：https://dw.zhonguo4118.cn

[Q53] 按条件删除
来源：https://xt.zhonguo2118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://yl.zhonguo5118.cn

[Q54] 清空表
来源：https://ch.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://pq.zhonguo4118.cn

[Q55] 排名（并列占位）
来源：https://yx.zhonguo3118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://ej.zhonguo5118.cn

[Q56] 密集排名（并列不占位）
来源：https://vd.zhonguo4118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://te.zhonguo8118.cn

[Q57] 行号
来源：https://kt.zhonguo1118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://kt.zhonguo1118.cn

[Q58] 累计求和
来源：https://jg.zhonguo1118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://vk.zhonguo7118.cn

[Q59] 分组内累计
来源：https://zm.zhonguo4118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://py.zhonguo8118.cn

[Q60] 取上一行 / 下一行
来源：https://cj.zhonguo3118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://fe.zhonguo2118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://pv.zhonguo2118.cn

[Q61] 移动平均
来源：https://ss.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://hx.zhonguo4118.cn

[Q62] 分组占比
来源：https://kk.zhonguo5118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://fx.zhonguo4118.cn

[Q63] 开启事务
来源：https://ei.zhonguo1118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://ba.zhonguo2118.cn

[Q64] 提交事务
来源：https://zi.zhonguo7118.cn

COMMIT;
来源：https://yk.zhonguo1118.cn

[Q65] 回滚事务
来源：https://ph.zhonguo4118.cn

ROLLBACK;
来源：https://iz.zhonguo4118.cn

[Q66] 行锁查询
来源：https://fp.zhonguo5118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://jd.zhonguo7118.cn

[Q67] 设置隔离级别
来源：https://as.zhonguo3118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://cr.zhonguo2118.cn

[Q68] 保存点
来源：https://gt.zhonguo5118.cn

SAVEPOINT sp1;
来源：https://qg.zhonguo8118.cn

ROLLBACK TO sp1;
来源：https://df.zhonguo7118.cn

[Q69] 查看执行计划
来源：https://pw.zhonguo7118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://dh.zhonguo5118.cn

[Q70] 更新统计信息
来源：https://xm.zhonguo2118.cn

ANALYZE TABLE users;
来源：https://rt.zhonguo5118.cn

[Q71] 查看建表语句
来源：https://gt.zhonguo6118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://hk.zhonguo8118.cn

[Q72] 查看索引
来源：https://iu.zhonguo5118.cn

SHOW INDEX FROM users;
来源：https://nd.zhonguo3118.cn

[Q73] 查看表状态
来源：https://bo.zhonguo3118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://mk.zhonguo8118.cn

[Q74] 强制使用索引
来源：https://nb.zhonguo4118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://da.zhonguo3118.cn

[Q75] 日期格式化
来源：https://xu.zhonguo2118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://lc.zhonguo5118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://ej.zhonguo2118.cn

[Q76] 按天统计
来源：https://fu.zhonguo1118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://cc.zhonguo6118.cn

[Q77] 时间加减
来源：https://pb.zhonguo6118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://yt.zhonguo8118.cn

[Q78] 当前时间
来源：https://vi.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://hg.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://do.zhonguo2118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://lu.zhonguo5118.cn

[Q80] 字符串截取
来源：https://md.zhonguo5118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://uv.zhonguo4118.cn

[Q81] 字符串替换
来源：https://yp.zhonguo4118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://aa.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://hx.zhonguo3118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://iu.zhonguo1118.cn

[Q83] 大小写转换
来源：https://dr.zhonguo4118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://yt.zhonguo7118.cn

[Q84] 去除首尾空格
来源：https://rt.zhonguo3118.cn

SELECT TRIM(name) FROM users;
来源：https://sf.zhonguo4118.cn

[Q85] 数值取整
来源：https://tx.zhonguo2118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://qi.zhonguo8118.cn

[Q86] 读取 JSON 字段
来源：https://im.zhonguo6118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://hd.zhonguo1118.cn

[Q87] JSON 字段做条件
来源：https://zm.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://gu.zhonguo6118.cn

[Q88] 行转列（条件聚合）
来源：https://qq.zhonguo8118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://bq.zhonguo5118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://jz.zhonguo6118.cn

[Q89] 判断表是否存在
来源：https://lp.zhonguo3118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://sx.zhonguo3118.cn

[Q90] 生成序号列
来源：https://yn.zhonguo8118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://hx.zhonguo4118.cn

================================================================================
来源：https://or.zhonguo6118.cn

R. Bash 专题
来源：https://ul.zhonguo5118.cn

================================================================================
来源：https://sx.zhonguo1118.cn

[R01] shebang 与严格模式
来源：https://qz.zhonguo6118.cn

#!/usr/bin/env bash
来源：https://yz.zhonguo3118.cn

set -euo pipefail
来源：https://hd.zhonguo1118.cn

[R02] 变量赋值与使用
来源：https://ff.zhonguo1118.cn

name="Tom"; echo "$name"
来源：https://gh.zhonguo7118.cn

[R03] 只读变量
来源：https://dj.zhonguo1118.cn

readonly PI=3.14
来源：https://km.zhonguo6118.cn

[R04] 位置参数
来源：https://wl.zhonguo7118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://eb.zhonguo8118.cn

[R05] 参数默认值
来源：https://kn.zhonguo4118.cn

name="${1:-default}"
来源：https://xw.zhonguo3118.cn

[R06] 判断命令是否存在
来源：https://za.zhonguo1118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://wl.zhonguo5118.cn

[R07] if 判断文件
来源：https://ri.zhonguo4118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://al.zhonguo2118.cn

[R08] 数值比较
来源：https://wo.zhonguo6118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://bu.zhonguo7118.cn

[R09] 字符串比较
来源：https://oc.zhonguo4118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://mh.zhonguo7118.cn

[R10] 正则匹配
来源：https://rf.zhonguo8118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://pn.zhonguo7118.cn

[R11] case 多分支
来源：https://bw.zhonguo8118.cn

case "$1" in
来源：https://pn.zhonguo3118.cn

start) echo "启动" ;;
来源：https://ea.zhonguo2118.cn

stop)  echo "停止" ;;
来源：https://jj.zhonguo4118.cn

*)     echo "未知命令" ;;
来源：https://sg.zhonguo8118.cn

esac
来源：https://rc.zhonguo7118.cn

[R12] for 遍历文件
来源：https://ij.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://wp.zhonguo6118.cn

[R13] for 计数循环
来源：https://lk.zhonguo7118.cn

for i in {1..10}; do echo "$i"; done
来源：https://db.zhonguo3118.cn

[R14] C 风格 for
来源：https://fs.zhonguo3118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://ae.zhonguo3118.cn

[R15] while 逐行读文件
来源：https://og.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://ej.zhonguo7118.cn

[R16] until 等待条件
来源：https://xl.zhonguo4118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://ng.zhonguo3118.cn

[R17] 数组定义与取值
来源：https://pf.zhonguo3118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://yw.zhonguo2118.cn

[R18] 遍历数组
来源：https://ly.zhonguo6118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://qt.zhonguo2118.cn

[R19] 数组长度
来源：https://at.zhonguo3118.cn

echo "${#arr[@]}"
来源：https://he.zhonguo3118.cn

[R20] 关联数组（字典）
来源：https://wf.zhonguo3118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://oi.zhonguo4118.cn

[R21] 字符串长度
来源：https://yx.zhonguo5118.cn

echo "${#s}"
来源：https://sy.zhonguo5118.cn

[R22] 截取子串
来源：https://pi.zhonguo2118.cn

echo "${s:0:5}"
来源：https://aq.zhonguo8118.cn

[R23] 字符串替换
来源：https://nt.zhonguo6118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://am.zhonguo3118.cn

[R24] 大小写转换
来源：https://jt.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://gn.zhonguo2118.cn

[R25] 去后缀 / 去前缀
来源：https://pr.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://cl.zhonguo2118.cn

[R26] 命令替换
来源：https://ju.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://or.zhonguo3118.cn

[R27] 算术展开
来源：https://eb.zhonguo7118.cn

echo $((1 + 2 * 3))
来源：https://gc.zhonguo4118.cn

[R28] 浮点运算
来源：https://yb.zhonguo1118.cn

echo "scale=2; 10/3" | bc
来源：https://tk.zhonguo2118.cn

[R29] 定义函数
来源：https://yn.zhonguo8118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://sf.zhonguo6118.cn

[R30] 函数返回状态码
来源：https://eo.zhonguo1118.cn

f() { return 0; }; f || echo "失败了"
来源：https://bn.zhonguo3118.cn

[R31] 局部变量
来源：https://nc.zhonguo3118.cn

f() { local x=1; echo "$x"; }
来源：https://vn.zhonguo3118.cn

[R32] 参数个数校验
来源：https://qk.zhonguo7118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://cc.zhonguo4118.cn

[R33] 捕获错误并提示行号
来源：https://sp.zhonguo6118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://qd.zhonguo2118.cn

[R34] 退出时清理
来源：https://ve.zhonguo4118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://wc.zhonguo3118.cn

[R35] 后台执行并等待
来源：https://je.zhonguo3118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://js.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://md.zhonguo2118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://fv.zhonguo4118.cn

[R37] 把输出赋给变量
来源：https://rl.zhonguo8118.cn

files=$(ls -1)
来源：https://hp.zhonguo1118.cn

[R38] 管道串联
来源：https://xl.zhonguo3118.cn

cat a.txt | grep -i error | wc -l
来源：https://wr.zhonguo5118.cn

[R39] 重定向标准输出与错误
来源：https://yt.zhonguo6118.cn

cmd > out.log 2>&1
来源：https://go.zhonguo1118.cn

[R40] 追加写日志
来源：https://fx.zhonguo7118.cn

echo "log" >> out.log
来源：https://da.zhonguo8118.cn

[R41] 丢弃输出
来源：https://nd.zhonguo3118.cn

cmd >/dev/null 2>&1
来源：https://py.zhonguo3118.cn

[R42] 输入重定向
来源：https://zz.zhonguo7118.cn

wc -l < a.txt
来源：https://uy.zhonguo5118.cn

[R43] 按名字查找文件
来源：https://pl.zhonguo1118.cn

find . -name "*.log" -type f
来源：https://hc.zhonguo4118.cn

[R44] 按修改时间查找
来源：https://ys.zhonguo1118.cn

find . -mtime -7 -type f
来源：https://vk.zhonguo4118.cn

[R45] 批量删除
来源：https://sj.zhonguo3118.cn

find . -name "*.tmp" -delete
来源：https://ac.zhonguo1118.cn

[R46] 递归替换文件内容
来源：https://ns.zhonguo6118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://px.zhonguo2118.cn

[R47] sed 单行替换
来源：https://md.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://ob.zhonguo2118.cn

[R48] awk 取指定列
来源：https://hm.zhonguo5118.cn

awk '{print $1, $3}' a.txt
来源：https://ht.zhonguo7118.cn

[R49] awk 带条件
来源：https://vy.zhonguo7118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://jc.zhonguo1118.cn

[R50] awk 求和
来源：https://qc.zhonguo3118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://ts.zhonguo7118.cn

[R51] 排序去重取前几
来源：https://bt.zhonguo5118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://wb.zhonguo6118.cn

[R52] 统计行数
来源：https://md.zhonguo8118.cn

wc -l a.txt
来源：https://vp.zhonguo3118.cn

[R53] 查看文件头与实时尾
来源：https://az.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://aj.zhonguo7118.cn

[R54] 比较两个文件
来源：https://vj.zhonguo2118.cn

diff a.txt b.txt
来源：https://if.zhonguo7118.cn

[R55] 压缩与解压
来源：https://fr.zhonguo6118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://bl.zhonguo5118.cn

[R56] 远程拷贝
来源：https://dj.zhonguo8118.cn

scp file user@host:/path/
来源：https://fd.zhonguo5118.cn

[R57] 远程执行命令
来源：https://vl.zhonguo7118.cn

ssh user@host 'uptime'
来源：https://pd.zhonguo7118.cn

[R58] 下载文件
来源：https://ef.zhonguo6118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://ol.zhonguo7118.cn

[R59] 发 POST JSON
来源：https://rp.zhonguo6118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://xw.zhonguo8118.cn

[R60] 只看 HTTP 状态码
来源：https://xd.zhonguo6118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://vy.zhonguo2118.cn

[R61] 磁盘占用
来源：https://xe.zhonguo7118.cn

df -h;  du -sh *
来源：https://fb.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://wl.zhonguo8118.cn

du -ah . | sort -rh | head -10
来源：https://px.zhonguo4118.cn

[R63] 内存与进程
来源：https://ws.zhonguo3118.cn

free -h;  ps aux | grep nginx
来源：https://oj.zhonguo8118.cn

[R64] 结束进程
来源：https://fr.zhonguo1118.cn

kill -9 $(pgrep -f app.py)
来源：https://vi.zhonguo7118.cn

[R65] 查看端口占用
来源：https://kr.zhonguo4118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://jd.zhonguo1118.cn

[R66] 定时任务
来源：https://wo.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://nw.zhonguo7118.cn

[R67] 生成随机十六进制串
来源：https://ew.zhonguo6118.cn

openssl rand -hex 16
来源：https://sf.zhonguo2118.cn

[R68] 计算文件校验值
来源：https://zn.zhonguo2118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://xx.zhonguo2118.cn

[R69] 生成随机密码
来源：https://zv.zhonguo2118.cn

head -c 16 /dev/urandom | base64
来源：https://hm.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://ut.zhonguo4118.cn

date +%s;  date -d @1700000000
来源：https://sc.zhonguo3118.cn

[R71] 日期格式化
来源：https://vt.zhonguo2118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ag.zhonguo7118.cn

[R72] 等待端口就绪
来源：https://vn.zhonguo7118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://df.zhonguo2118.cn

[R73] 分割大日志
来源：https://pn.zhonguo8118.cn

split -l 1000 big.log part_
来源：https://jy.zhonguo3118.cn

[R74] 批量重命名
来源：https://on.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://qk.zhonguo5118.cn

[R75] 导出环境变量
来源：https://lh.zhonguo3118.cn

export PATH="$HOME/bin:$PATH"
来源：https://rk.zhonguo5118.cn

[R76] 使用临时文件
来源：https://yx.zhonguo4118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://za.zhonguo2118.cn

[R77] 读取用户输入
来源：https://tm.zhonguo8118.cn

read -rp "请输入: " ans
来源：https://mh.zhonguo4118.cn

[R78] 交互式菜单
来源：https://uh.zhonguo2118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://ci.zhonguo2118.cn

[R79] 解析命令行选项
来源：https://eo.zhonguo4118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://oe.zhonguo4118.cn

[R80] 查看脚本执行耗时
来源：https://il.zhonguo4118.cn

time ./run.sh
来源：https://ie.zhonguo3118.cn

================================================================================
来源：https://qe.zhonguo6118.cn


<!-- 参考信息 -->