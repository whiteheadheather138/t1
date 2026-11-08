代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://cj.zhonguo4118.cn

[Q32] 分组拼接字符串
来源：https://qt.zhonguo4118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://wk.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://zb.zhonguo4118.cn

[Q33] 多列分组
来源：https://ur.zhonguo1118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://wx.zhonguo2118.cn

[Q34] 每组取第一条
来源：https://xw.zhonguo6118.cn

SELECT * FROM (
来源：https://mn.zhonguo5118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://nd.zhonguo2118.cn

) t WHERE rn = 1;
来源：https://ne.zhonguo6118.cn

[Q35] 内连接
来源：https://yg.zhonguo4118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://mm.zhonguo2118.cn

[Q36] 左连接
来源：https://ip.zhonguo8118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://se.zhonguo5118.cn

[Q37] 右连接
来源：https://bj.zhonguo8118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://iz.zhonguo6118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://sm.zhonguo7118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://pb.zhonguo8118.cn

[Q39] 自连接（查上下级）
来源：https://ka.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://ml.zhonguo5118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://xk.zhonguo2118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://kq.zhonguo1118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://vr.zhonguo4118.cn

[Q41] 多表连接
来源：https://kk.zhonguo2118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://sf.zhonguo6118.cn

JOIN users u ON u.id = o.user_id
来源：https://yz.zhonguo8118.cn

JOIN products p ON p.id = o.product_id;
来源：https://se.zhonguo1118.cn

[Q42] 连接条件附加过滤
来源：https://jh.zhonguo1118.cn

SELECT u.name, o.amount FROM users u
来源：https://sx.zhonguo5118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://aj.zhonguo1118.cn

[Q43] 标量子查询
来源：https://ey.zhonguo1118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://hu.zhonguo2118.cn

[Q44] IN 子查询
来源：https://cl.zhonguo8118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://yl.zhonguo7118.cn

[Q45] EXISTS 判断存在
来源：https://jw.zhonguo2118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://mc.zhonguo2118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://zg.zhonguo3118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://dc.zhonguo1118.cn

[Q47] 与平均值比较
来源：https://nd.zhonguo1118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://ek.zhonguo1118.cn

[Q48] CTE 公用表表达式
来源：https://mw.zhonguo7118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://qk.zhonguo5118.cn

SELECT * FROM t WHERE c > 5;
来源：https://po.zhonguo2118.cn

[Q49] 更新单行
来源：https://mv.zhonguo1118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://cd.zhonguo5118.cn

[Q50] 批量更新
来源：https://zf.zhonguo8118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://gu.zhonguo6118.cn

[Q51] 用子查询更新
来源：https://xp.zhonguo8118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://hd.zhonguo1118.cn

[Q52] 删除指定行
来源：https://yt.zhonguo2118.cn

DELETE FROM users WHERE id = 10;
来源：https://wc.zhonguo8118.cn

[Q53] 按条件删除
来源：https://xr.zhonguo6118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://al.zhonguo4118.cn

[Q54] 清空表
来源：https://bt.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://zs.zhonguo8118.cn

[Q55] 排名（并列占位）
来源：https://dj.zhonguo4118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://oh.zhonguo7118.cn

[Q56] 密集排名（并列不占位）
来源：https://bk.zhonguo1118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://if.zhonguo2118.cn

[Q57] 行号
来源：https://bi.zhonguo6118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://ie.zhonguo5118.cn

[Q58] 累计求和
来源：https://cr.zhonguo1118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://fc.zhonguo7118.cn

[Q59] 分组内累计
来源：https://vi.zhonguo6118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://em.zhonguo3118.cn

[Q60] 取上一行 / 下一行
来源：https://fr.zhonguo4118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://ux.zhonguo8118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://gp.zhonguo4118.cn

[Q61] 移动平均
来源：https://iv.zhonguo1118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://be.zhonguo3118.cn

[Q62] 分组占比
来源：https://nt.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://hz.zhonguo6118.cn

[Q63] 开启事务
来源：https://ok.zhonguo5118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://pm.zhonguo1118.cn

[Q64] 提交事务
来源：https://ji.zhonguo8118.cn

COMMIT;
来源：https://zv.zhonguo4118.cn

[Q65] 回滚事务
来源：https://km.zhonguo1118.cn

ROLLBACK;
来源：https://rq.zhonguo1118.cn

[Q66] 行锁查询
来源：https://po.zhonguo6118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://cv.zhonguo4118.cn

[Q67] 设置隔离级别
来源：https://ha.zhonguo5118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://mt.zhonguo3118.cn

[Q68] 保存点
来源：https://yc.zhonguo6118.cn

SAVEPOINT sp1;
来源：https://eo.zhonguo6118.cn

ROLLBACK TO sp1;
来源：https://vv.zhonguo8118.cn

[Q69] 查看执行计划
来源：https://yw.zhonguo1118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://cp.zhonguo7118.cn

[Q70] 更新统计信息
来源：https://xq.zhonguo6118.cn

ANALYZE TABLE users;
来源：https://nh.zhonguo2118.cn

[Q71] 查看建表语句
来源：https://yp.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://xk.zhonguo7118.cn

[Q72] 查看索引
来源：https://ym.zhonguo7118.cn

SHOW INDEX FROM users;
来源：https://lv.zhonguo3118.cn

[Q73] 查看表状态
来源：https://qc.zhonguo7118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://ej.zhonguo1118.cn

[Q74] 强制使用索引
来源：https://ay.zhonguo8118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://dz.zhonguo4118.cn

[Q75] 日期格式化
来源：https://gx.zhonguo3118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://sl.zhonguo3118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://me.zhonguo5118.cn

[Q76] 按天统计
来源：https://bj.zhonguo5118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://fs.zhonguo3118.cn

[Q77] 时间加减
来源：https://ek.zhonguo6118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://uv.zhonguo2118.cn

[Q78] 当前时间
来源：https://xk.zhonguo8118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://dy.zhonguo5118.cn

[Q79] 字符串拼接
来源：https://pc.zhonguo2118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://jt.zhonguo7118.cn

[Q80] 字符串截取
来源：https://og.zhonguo1118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://ib.zhonguo3118.cn

[Q81] 字符串替换
来源：https://rt.zhonguo2118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://bq.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://mk.zhonguo4118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://cs.zhonguo3118.cn

[Q83] 大小写转换
来源：https://em.zhonguo7118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://rw.zhonguo6118.cn

[Q84] 去除首尾空格
来源：https://nm.zhonguo7118.cn

SELECT TRIM(name) FROM users;
来源：https://dm.zhonguo1118.cn

[Q85] 数值取整
来源：https://ad.zhonguo8118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://dp.zhonguo8118.cn

[Q86] 读取 JSON 字段
来源：https://ft.zhonguo5118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://kh.zhonguo6118.cn

[Q87] JSON 字段做条件
来源：https://kk.zhonguo5118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://oq.zhonguo5118.cn

[Q88] 行转列（条件聚合）
来源：https://jp.zhonguo3118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://wb.zhonguo7118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://of.zhonguo5118.cn

[Q89] 判断表是否存在
来源：https://xv.zhonguo7118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://zr.zhonguo4118.cn

[Q90] 生成序号列
来源：https://rg.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ml.zhonguo3118.cn

================================================================================
来源：https://cw.zhonguo4118.cn

R. Bash 专题
来源：https://uz.zhonguo4118.cn

================================================================================
来源：https://fs.zhonguo7118.cn

[R01] shebang 与严格模式
来源：https://iz.zhonguo4118.cn

#!/usr/bin/env bash
来源：https://wm.zhonguo2118.cn

set -euo pipefail
来源：https://wo.zhonguo3118.cn

[R02] 变量赋值与使用
来源：https://vx.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://iu.zhonguo7118.cn

[R03] 只读变量
来源：https://uf.zhonguo8118.cn

readonly PI=3.14
来源：https://uu.zhonguo6118.cn

[R04] 位置参数
来源：https://bv.zhonguo1118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://nn.zhonguo1118.cn

[R05] 参数默认值
来源：https://zn.zhonguo5118.cn

name="${1:-default}"
来源：https://hb.zhonguo4118.cn

[R06] 判断命令是否存在
来源：https://ds.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://at.zhonguo8118.cn

[R07] if 判断文件
来源：https://vd.zhonguo7118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://oc.zhonguo4118.cn

[R08] 数值比较
来源：https://rh.zhonguo5118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://gk.zhonguo2118.cn

[R09] 字符串比较
来源：https://zl.zhonguo3118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ya.zhonguo2118.cn

[R10] 正则匹配
来源：https://yq.zhonguo6118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://gq.zhonguo7118.cn

[R11] case 多分支
来源：https://zr.zhonguo2118.cn

case "$1" in
来源：https://qu.zhonguo8118.cn

start) echo "启动" ;;
来源：https://dd.zhonguo8118.cn

stop)  echo "停止" ;;
来源：https://im.zhonguo3118.cn

*)     echo "未知命令" ;;
来源：https://eg.zhonguo6118.cn

esac
来源：https://fa.zhonguo7118.cn

[R12] for 遍历文件
来源：https://sf.zhonguo2118.cn

for f in *.txt; do echo "$f"; done
来源：https://hy.zhonguo1118.cn

[R13] for 计数循环
来源：https://qw.zhonguo2118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ps.zhonguo8118.cn

[R14] C 风格 for
来源：https://ne.zhonguo3118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://ok.zhonguo3118.cn

[R15] while 逐行读文件
来源：https://tl.zhonguo3118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://we.zhonguo1118.cn

[R16] until 等待条件
来源：https://nc.zhonguo5118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://cf.zhonguo8118.cn

[R17] 数组定义与取值
来源：https://lc.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://wy.zhonguo4118.cn

[R18] 遍历数组
来源：https://oa.zhonguo8118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://ma.zhonguo8118.cn

[R19] 数组长度
来源：https://jt.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://gd.zhonguo8118.cn

[R20] 关联数组（字典）
来源：https://yd.zhonguo2118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://kt.zhonguo1118.cn

[R21] 字符串长度
来源：https://cw.zhonguo6118.cn

echo "${#s}"
来源：https://ot.zhonguo8118.cn

[R22] 截取子串
来源：https://xp.zhonguo1118.cn

echo "${s:0:5}"
来源：https://sx.zhonguo5118.cn

[R23] 字符串替换
来源：https://of.zhonguo1118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://gn.zhonguo7118.cn

[R24] 大小写转换
来源：https://nk.zhonguo2118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://jz.zhonguo8118.cn

[R25] 去后缀 / 去前缀
来源：https://ay.zhonguo7118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://ev.zhonguo6118.cn

[R26] 命令替换
来源：https://ef.zhonguo3118.cn

now=$(date +%F); echo "$now"
来源：https://gv.zhonguo3118.cn

[R27] 算术展开
来源：https://xj.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://dw.zhonguo8118.cn

[R28] 浮点运算
来源：https://md.zhonguo7118.cn

echo "scale=2; 10/3" | bc
来源：https://vs.zhonguo1118.cn

[R29] 定义函数
来源：https://su.zhonguo1118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://zn.zhonguo1118.cn

[R30] 函数返回状态码
来源：https://he.zhonguo4118.cn

f() { return 0; }; f || echo "失败了"
来源：https://pf.zhonguo6118.cn

[R31] 局部变量
来源：https://fz.zhonguo8118.cn

f() { local x=1; echo "$x"; }
来源：https://dk.zhonguo5118.cn

[R32] 参数个数校验
来源：https://dh.zhonguo7118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://lw.zhonguo3118.cn

[R33] 捕获错误并提示行号
来源：https://nx.zhonguo8118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://wp.zhonguo7118.cn

[R34] 退出时清理
来源：https://xw.zhonguo2118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://cf.zhonguo2118.cn

[R35] 后台执行并等待
来源：https://mb.zhonguo7118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://ts.zhonguo1118.cn

[R36] 并发执行多个任务
来源：https://tk.zhonguo3118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://zg.zhonguo8118.cn

[R37] 把输出赋给变量
来源：https://ok.zhonguo8118.cn

files=$(ls -1)
来源：https://ij.zhonguo3118.cn

[R38] 管道串联
来源：https://yt.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://ps.zhonguo2118.cn

[R39] 重定向标准输出与错误
来源：https://bm.zhonguo4118.cn

cmd > out.log 2>&1
来源：https://xl.zhonguo5118.cn

[R40] 追加写日志
来源：https://qp.zhonguo8118.cn

echo "log" >> out.log
来源：https://sy.zhonguo5118.cn

[R41] 丢弃输出
来源：https://as.zhonguo1118.cn

cmd >/dev/null 2>&1
来源：https://mh.zhonguo5118.cn

[R42] 输入重定向
来源：https://pk.zhonguo2118.cn

wc -l < a.txt
来源：https://gr.zhonguo2118.cn

[R43] 按名字查找文件
来源：https://gx.zhonguo7118.cn

find . -name "*.log" -type f
来源：https://vi.zhonguo6118.cn

[R44] 按修改时间查找
来源：https://ew.zhonguo5118.cn

find . -mtime -7 -type f
来源：https://cj.zhonguo4118.cn

[R45] 批量删除
来源：https://gk.zhonguo1118.cn

find . -name "*.tmp" -delete
来源：https://in.zhonguo5118.cn

[R46] 递归替换文件内容
来源：https://ri.zhonguo8118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://ou.zhonguo4118.cn

[R47] sed 单行替换
来源：https://nk.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://gi.zhonguo6118.cn

[R48] awk 取指定列
来源：https://mk.zhonguo7118.cn

awk '{print $1, $3}' a.txt
来源：https://mw.zhonguo1118.cn

[R49] awk 带条件
来源：https://jz.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://yu.zhonguo7118.cn

[R50] awk 求和
来源：https://cx.zhonguo2118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://zy.zhonguo4118.cn

[R51] 排序去重取前几
来源：https://uu.zhonguo7118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://rn.zhonguo8118.cn

[R52] 统计行数
来源：https://jd.zhonguo3118.cn

wc -l a.txt
来源：https://ly.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://ag.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://dl.zhonguo2118.cn

[R54] 比较两个文件
来源：https://co.zhonguo5118.cn

diff a.txt b.txt
来源：https://ba.zhonguo2118.cn

[R55] 压缩与解压
来源：https://qe.zhonguo2118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://vq.zhonguo6118.cn

[R56] 远程拷贝
来源：https://xr.zhonguo7118.cn

scp file user@host:/path/
来源：https://vy.zhonguo1118.cn

[R57] 远程执行命令
来源：https://zm.zhonguo7118.cn

ssh user@host 'uptime'
来源：https://wv.zhonguo2118.cn

[R58] 下载文件
来源：https://an.zhonguo5118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://mw.zhonguo1118.cn

[R59] 发 POST JSON
来源：https://wx.zhonguo8118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://vz.zhonguo3118.cn

[R60] 只看 HTTP 状态码
来源：https://um.zhonguo3118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://lw.zhonguo7118.cn

[R61] 磁盘占用
来源：https://ud.zhonguo3118.cn

df -h;  du -sh *
来源：https://hj.zhonguo8118.cn

[R62] 找最占空间的文件
来源：https://dn.zhonguo2118.cn

du -ah . | sort -rh | head -10
来源：https://zo.zhonguo3118.cn

[R63] 内存与进程
来源：https://ow.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://pt.zhonguo4118.cn

[R64] 结束进程
来源：https://rs.zhonguo3118.cn

kill -9 $(pgrep -f app.py)
来源：https://hx.zhonguo5118.cn

[R65] 查看端口占用
来源：https://lc.zhonguo5118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://tq.zhonguo4118.cn

[R66] 定时任务
来源：https://eh.zhonguo4118.cn

crontab -e;  crontab -l
来源：https://ku.zhonguo8118.cn

[R67] 生成随机十六进制串
来源：https://vv.zhonguo1118.cn

openssl rand -hex 16
来源：https://pz.zhonguo3118.cn

[R68] 计算文件校验值
来源：https://zi.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://bq.zhonguo2118.cn

[R69] 生成随机密码
来源：https://qn.zhonguo4118.cn

head -c 16 /dev/urandom | base64
来源：https://ya.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://xf.zhonguo8118.cn

date +%s;  date -d @1700000000
来源：https://xm.zhonguo1118.cn

[R71] 日期格式化
来源：https://iz.zhonguo5118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://vv.zhonguo6118.cn

[R72] 等待端口就绪
来源：https://ez.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://ha.zhonguo6118.cn

[R73] 分割大日志
来源：https://xc.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://fr.zhonguo3118.cn

[R74] 批量重命名
来源：https://du.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://bt.zhonguo2118.cn

[R75] 导出环境变量
来源：https://zn.zhonguo8118.cn

export PATH="$HOME/bin:$PATH"
来源：https://gj.zhonguo8118.cn

[R76] 使用临时文件
来源：https://ah.zhonguo7118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://li.zhonguo4118.cn

[R77] 读取用户输入
来源：https://zd.zhonguo1118.cn

read -rp "请输入: " ans
来源：https://uq.zhonguo5118.cn

[R78] 交互式菜单
来源：https://aa.zhonguo7118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://uj.zhonguo4118.cn

[R79] 解析命令行选项
来源：https://xv.zhonguo5118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://ph.zhonguo8118.cn

[R80] 查看脚本执行耗时
来源：https://ph.zhonguo3118.cn

time ./run.sh
来源：https://tz.zhonguo4118.cn

================================================================================
来源：https://iv.zhonguo2118.cn


<!-- 参考信息 -->