代发 wailian999

[Q36] 左连接
来源：https://dz.zhonguo1118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://pg.zhonguo5118.cn

[Q37] 右连接
来源：https://gh.zhonguo3118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://sj.zhonguo2118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://tf.zhonguo1118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://vu.zhonguo7118.cn

[Q39] 自连接（查上下级）
来源：https://bi.zhonguo5118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://hb.zhonguo7118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://jp.zhonguo1118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://gc.zhonguo3118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://gu.zhonguo5118.cn

[Q41] 多表连接
来源：https://nq.zhonguo1118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://oy.zhonguo6118.cn

JOIN users u ON u.id = o.user_id
来源：https://ae.zhonguo8118.cn

JOIN products p ON p.id = o.product_id;
来源：https://bd.zhonguo4118.cn

[Q42] 连接条件附加过滤
来源：https://hr.zhonguo4118.cn

SELECT u.name, o.amount FROM users u
来源：https://jg.zhonguo6118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://mx.zhonguo6118.cn

[Q43] 标量子查询
来源：https://rr.zhonguo8118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://th.zhonguo2118.cn

[Q44] IN 子查询
来源：https://qm.zhonguo2118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://fb.zhonguo6118.cn

[Q45] EXISTS 判断存在
来源：https://eq.zhonguo2118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://le.zhonguo3118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://qz.zhonguo6118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://mj.zhonguo1118.cn

[Q47] 与平均值比较
来源：https://xt.zhonguo2118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://ap.zhonguo5118.cn

[Q48] CTE 公用表表达式
来源：https://hh.zhonguo6118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://rc.zhonguo5118.cn

SELECT * FROM t WHERE c > 5;
来源：https://nu.zhonguo8118.cn

[Q49] 更新单行
来源：https://vc.zhonguo3118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://tg.zhonguo2118.cn

[Q50] 批量更新
来源：https://nr.zhonguo5118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://bh.zhonguo5118.cn

[Q51] 用子查询更新
来源：https://rv.zhonguo7118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://vr.zhonguo7118.cn

[Q52] 删除指定行
来源：https://ly.zhonguo3118.cn

DELETE FROM users WHERE id = 10;
来源：https://qc.zhonguo8118.cn

[Q53] 按条件删除
来源：https://yy.zhonguo4118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://oz.zhonguo5118.cn

[Q54] 清空表
来源：https://jn.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://cf.zhonguo6118.cn

[Q55] 排名（并列占位）
来源：https://uv.zhonguo2118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://xl.zhonguo3118.cn

[Q56] 密集排名（并列不占位）
来源：https://mw.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://ay.zhonguo1118.cn

[Q57] 行号
来源：https://xz.zhonguo5118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://qr.zhonguo2118.cn

[Q58] 累计求和
来源：https://tr.zhonguo8118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://ow.zhonguo8118.cn

[Q59] 分组内累计
来源：https://md.zhonguo4118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://sx.zhonguo4118.cn

[Q60] 取上一行 / 下一行
来源：https://mx.zhonguo1118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://wc.zhonguo8118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://ix.zhonguo8118.cn

[Q61] 移动平均
来源：https://oi.zhonguo7118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://yx.zhonguo8118.cn

[Q62] 分组占比
来源：https://ky.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://xk.zhonguo8118.cn

[Q63] 开启事务
来源：https://le.zhonguo6118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://ht.zhonguo7118.cn

[Q64] 提交事务
来源：https://bh.zhonguo1118.cn

COMMIT;
来源：https://hy.zhonguo3118.cn

[Q65] 回滚事务
来源：https://lu.zhonguo5118.cn

ROLLBACK;
来源：https://zt.zhonguo6118.cn

[Q66] 行锁查询
来源：https://rh.zhonguo8118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://ow.zhonguo3118.cn

[Q67] 设置隔离级别
来源：https://dx.zhonguo3118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://wu.zhonguo5118.cn

[Q68] 保存点
来源：https://ov.zhonguo5118.cn

SAVEPOINT sp1;
来源：https://ga.zhonguo4118.cn

ROLLBACK TO sp1;
来源：https://qb.zhonguo1118.cn

[Q69] 查看执行计划
来源：https://hn.zhonguo7118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://hp.zhonguo1118.cn

[Q70] 更新统计信息
来源：https://vl.zhonguo3118.cn

ANALYZE TABLE users;
来源：https://pl.zhonguo2118.cn

[Q71] 查看建表语句
来源：https://iq.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://va.zhonguo3118.cn

[Q72] 查看索引
来源：https://kt.zhonguo5118.cn

SHOW INDEX FROM users;
来源：https://rc.zhonguo4118.cn

[Q73] 查看表状态
来源：https://zb.zhonguo8118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://av.zhonguo1118.cn

[Q74] 强制使用索引
来源：https://cy.zhonguo3118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://dc.zhonguo2118.cn

[Q75] 日期格式化
来源：https://an.zhonguo5118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://fz.zhonguo7118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://sq.zhonguo5118.cn

[Q76] 按天统计
来源：https://hz.zhonguo3118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ye.zhonguo8118.cn

[Q77] 时间加减
来源：https://ps.zhonguo5118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://ya.zhonguo1118.cn

[Q78] 当前时间
来源：https://mv.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://kk.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://jm.zhonguo1118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://ja.zhonguo3118.cn

[Q80] 字符串截取
来源：https://zl.zhonguo1118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://pd.zhonguo3118.cn

[Q81] 字符串替换
来源：https://gh.zhonguo4118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://fx.zhonguo2118.cn

[Q82] 字符长度与字节长度
来源：https://ks.zhonguo4118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://sm.zhonguo4118.cn

[Q83] 大小写转换
来源：https://fl.zhonguo5118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://yh.zhonguo1118.cn

[Q84] 去除首尾空格
来源：https://qg.zhonguo8118.cn

SELECT TRIM(name) FROM users;
来源：https://ui.zhonguo5118.cn

[Q85] 数值取整
来源：https://gg.zhonguo5118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://rl.zhonguo5118.cn

[Q86] 读取 JSON 字段
来源：https://zk.zhonguo4118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://ph.zhonguo2118.cn

[Q87] JSON 字段做条件
来源：https://qw.zhonguo5118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://ir.zhonguo8118.cn

[Q88] 行转列（条件聚合）
来源：https://pn.zhonguo6118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://sz.zhonguo1118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://lz.zhonguo2118.cn

[Q89] 判断表是否存在
来源：https://cl.zhonguo2118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://hl.zhonguo5118.cn

[Q90] 生成序号列
来源：https://mg.zhonguo2118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://zw.zhonguo8118.cn

================================================================================
来源：https://vq.zhonguo4118.cn

R. Bash 专题
来源：https://du.zhonguo7118.cn

================================================================================
来源：https://za.zhonguo8118.cn

[R01] shebang 与严格模式
来源：https://ji.zhonguo1118.cn

#!/usr/bin/env bash
来源：https://vc.zhonguo1118.cn

set -euo pipefail
来源：https://xy.zhonguo1118.cn

[R02] 变量赋值与使用
来源：https://mt.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://rj.zhonguo1118.cn

[R03] 只读变量
来源：https://pb.zhonguo4118.cn

readonly PI=3.14
来源：https://gm.zhonguo7118.cn

[R04] 位置参数
来源：https://sy.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://lt.zhonguo6118.cn

[R05] 参数默认值
来源：https://qi.zhonguo6118.cn

name="${1:-default}"
来源：https://rz.zhonguo1118.cn

[R06] 判断命令是否存在
来源：https://kh.zhonguo2118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://mg.zhonguo2118.cn

[R07] if 判断文件
来源：https://wv.zhonguo2118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://bb.zhonguo3118.cn

[R08] 数值比较
来源：https://ks.zhonguo8118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ww.zhonguo3118.cn

[R09] 字符串比较
来源：https://ac.zhonguo4118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://xg.zhonguo3118.cn

[R10] 正则匹配
来源：https://tw.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://wl.zhonguo7118.cn

[R11] case 多分支
来源：https://rh.zhonguo2118.cn

case "$1" in
来源：https://tu.zhonguo8118.cn

start) echo "启动" ;;
来源：https://hr.zhonguo6118.cn

stop)  echo "停止" ;;
来源：https://ct.zhonguo4118.cn

*)     echo "未知命令" ;;
来源：https://lh.zhonguo8118.cn

esac
来源：https://fs.zhonguo4118.cn

[R12] for 遍历文件
来源：https://nv.zhonguo2118.cn

for f in *.txt; do echo "$f"; done
来源：https://xv.zhonguo6118.cn

[R13] for 计数循环
来源：https://pb.zhonguo3118.cn

for i in {1..10}; do echo "$i"; done
来源：https://kw.zhonguo7118.cn

[R14] C 风格 for
来源：https://jc.zhonguo3118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://dj.zhonguo2118.cn

[R15] while 逐行读文件
来源：https://jp.zhonguo1118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://qt.zhonguo3118.cn

[R16] until 等待条件
来源：https://wx.zhonguo4118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://hu.zhonguo7118.cn

[R17] 数组定义与取值
来源：https://xt.zhonguo5118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://rk.zhonguo3118.cn

[R18] 遍历数组
来源：https://xy.zhonguo6118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://mv.zhonguo8118.cn

[R19] 数组长度
来源：https://ee.zhonguo2118.cn

echo "${#arr[@]}"
来源：https://dk.zhonguo8118.cn

[R20] 关联数组（字典）
来源：https://tr.zhonguo1118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://or.zhonguo3118.cn

[R21] 字符串长度
来源：https://rl.zhonguo1118.cn

echo "${#s}"
来源：https://oy.zhonguo3118.cn

[R22] 截取子串
来源：https://zi.zhonguo8118.cn

echo "${s:0:5}"
来源：https://rp.zhonguo5118.cn

[R23] 字符串替换
来源：https://ph.zhonguo7118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://es.zhonguo4118.cn

[R24] 大小写转换
来源：https://jw.zhonguo4118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ig.zhonguo2118.cn

[R25] 去后缀 / 去前缀
来源：https://jy.zhonguo7118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://dp.zhonguo6118.cn

[R26] 命令替换
来源：https://pi.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://kn.zhonguo7118.cn

[R27] 算术展开
来源：https://gu.zhonguo5118.cn

echo $((1 + 2 * 3))
来源：https://aq.zhonguo5118.cn

[R28] 浮点运算
来源：https://dw.zhonguo1118.cn

echo "scale=2; 10/3" | bc
来源：https://ev.zhonguo7118.cn

[R29] 定义函数
来源：https://fv.zhonguo6118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://wd.zhonguo3118.cn

[R30] 函数返回状态码
来源：https://nr.zhonguo6118.cn

f() { return 0; }; f || echo "失败了"
来源：https://qx.zhonguo3118.cn

[R31] 局部变量
来源：https://ft.zhonguo1118.cn

f() { local x=1; echo "$x"; }
来源：https://cs.zhonguo3118.cn

[R32] 参数个数校验
来源：https://iw.zhonguo1118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://vm.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://jz.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://dc.zhonguo2118.cn

[R34] 退出时清理
来源：https://vi.zhonguo7118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://bp.zhonguo3118.cn

[R35] 后台执行并等待
来源：https://yt.zhonguo3118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://he.zhonguo6118.cn

[R36] 并发执行多个任务
来源：https://so.zhonguo3118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://yb.zhonguo6118.cn

[R37] 把输出赋给变量
来源：https://xw.zhonguo5118.cn

files=$(ls -1)
来源：https://yg.zhonguo8118.cn

[R38] 管道串联
来源：https://aw.zhonguo5118.cn

cat a.txt | grep -i error | wc -l
来源：https://rq.zhonguo4118.cn

[R39] 重定向标准输出与错误
来源：https://ib.zhonguo5118.cn

cmd > out.log 2>&1
来源：https://yv.zhonguo3118.cn

[R40] 追加写日志
来源：https://vv.zhonguo8118.cn

echo "log" >> out.log
来源：https://uv.zhonguo3118.cn

[R41] 丢弃输出
来源：https://bc.zhonguo3118.cn

cmd >/dev/null 2>&1
来源：https://pt.zhonguo2118.cn

[R42] 输入重定向
来源：https://tu.zhonguo4118.cn

wc -l < a.txt
来源：https://th.zhonguo2118.cn

[R43] 按名字查找文件
来源：https://fg.zhonguo2118.cn

find . -name "*.log" -type f
来源：https://je.zhonguo3118.cn

[R44] 按修改时间查找
来源：https://ik.zhonguo8118.cn

find . -mtime -7 -type f
来源：https://rx.zhonguo5118.cn

[R45] 批量删除
来源：https://po.zhonguo7118.cn

find . -name "*.tmp" -delete
来源：https://ci.zhonguo5118.cn

[R46] 递归替换文件内容
来源：https://qk.zhonguo6118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://hh.zhonguo5118.cn

[R47] sed 单行替换
来源：https://ic.zhonguo3118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://qz.zhonguo2118.cn

[R48] awk 取指定列
来源：https://pt.zhonguo4118.cn

awk '{print $1, $3}' a.txt
来源：https://gm.zhonguo7118.cn

[R49] awk 带条件
来源：https://mv.zhonguo8118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ka.zhonguo2118.cn

[R50] awk 求和
来源：https://me.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://ad.zhonguo5118.cn

[R51] 排序去重取前几
来源：https://qz.zhonguo2118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://qe.zhonguo3118.cn

[R52] 统计行数
来源：https://ux.zhonguo8118.cn

wc -l a.txt
来源：https://lr.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://rw.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://rq.zhonguo8118.cn

[R54] 比较两个文件
来源：https://mh.zhonguo6118.cn

diff a.txt b.txt
来源：https://wt.zhonguo8118.cn

[R55] 压缩与解压
来源：https://gf.zhonguo8118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ys.zhonguo1118.cn

[R56] 远程拷贝
来源：https://ns.zhonguo8118.cn

scp file user@host:/path/
来源：https://vc.zhonguo5118.cn

[R57] 远程执行命令
来源：https://bs.zhonguo4118.cn

ssh user@host 'uptime'
来源：https://re.zhonguo4118.cn

[R58] 下载文件
来源：https://lc.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://vb.zhonguo3118.cn

[R59] 发 POST JSON
来源：https://xw.zhonguo5118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://lm.zhonguo6118.cn

[R60] 只看 HTTP 状态码
来源：https://xn.zhonguo7118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://ph.zhonguo8118.cn

[R61] 磁盘占用
来源：https://uz.zhonguo5118.cn

df -h;  du -sh *
来源：https://iy.zhonguo3118.cn

[R62] 找最占空间的文件
来源：https://iz.zhonguo3118.cn

du -ah . | sort -rh | head -10
来源：https://ig.zhonguo4118.cn

[R63] 内存与进程
来源：https://lj.zhonguo8118.cn

free -h;  ps aux | grep nginx
来源：https://kp.zhonguo8118.cn

[R64] 结束进程
来源：https://kc.zhonguo6118.cn

kill -9 $(pgrep -f app.py)
来源：https://nq.zhonguo4118.cn

[R65] 查看端口占用
来源：https://ii.zhonguo6118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://uk.zhonguo6118.cn

[R66] 定时任务
来源：https://em.zhonguo5118.cn

crontab -e;  crontab -l
来源：https://xb.zhonguo3118.cn

[R67] 生成随机十六进制串
来源：https://ab.zhonguo8118.cn

openssl rand -hex 16
来源：https://db.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://wd.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://yn.zhonguo7118.cn

[R69] 生成随机密码
来源：https://jr.zhonguo1118.cn

head -c 16 /dev/urandom | base64
来源：https://ja.zhonguo1118.cn

[R70] 时间戳与互转
来源：https://mg.zhonguo6118.cn

date +%s;  date -d @1700000000
来源：https://os.zhonguo1118.cn

[R71] 日期格式化
来源：https://av.zhonguo7118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://vz.zhonguo5118.cn

[R72] 等待端口就绪
来源：https://tm.zhonguo1118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://pa.zhonguo2118.cn

[R73] 分割大日志
来源：https://dl.zhonguo5118.cn

split -l 1000 big.log part_
来源：https://dt.zhonguo6118.cn

[R74] 批量重命名
来源：https://ua.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://uw.zhonguo7118.cn

[R75] 导出环境变量
来源：https://nf.zhonguo2118.cn

export PATH="$HOME/bin:$PATH"
来源：https://ue.zhonguo4118.cn

[R76] 使用临时文件
来源：https://vq.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://gy.zhonguo7118.cn

[R77] 读取用户输入
来源：https://ff.zhonguo7118.cn

read -rp "请输入: " ans
来源：https://jk.zhonguo5118.cn

[R78] 交互式菜单
来源：https://bb.zhonguo8118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://bq.zhonguo1118.cn

[R79] 解析命令行选项
来源：https://vv.zhonguo8118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://da.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://hz.zhonguo7118.cn

time ./run.sh
来源：https://jy.zhonguo6118.cn

================================================================================
来源：https://eq.zhonguo6118.cn

S. C / C++ 专题
来源：https://rs.zhonguo8118.cn

================================================================================
来源：https://tx.zhonguo8118.cn

[S01] C：Hello World
来源：https://tl.zhonguo4118.cn

#include <stdio.h>
来源：https://wf.zhonguo1118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://ys.zhonguo4118.cn

[S02] C：变量与格式化输出
来源：https://pc.zhonguo5118.cn

int a = 10; printf("%d\n", a);
来源：https://fd.zhonguo7118.cn

[S03] C：读入整数
来源：https://xi.zhonguo6118.cn

int x; scanf("%d", &x);
来源：https://sv.zhonguo1118.cn

[S04] C：字符串复制
来源：https://xc.zhonguo4118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://dp.zhonguo2118.cn

[S05] C：字符串长度
来源：https://lm.zhonguo2118.cn


<!-- 参考信息 -->