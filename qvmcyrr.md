代发 wailian999

[Q44] IN 子查询
来源：https://rk.zhonguo2118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://ig.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://xu.zhonguo8118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://fv.zhonguo5118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://vj.zhonguo8118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://yf.zhonguo3118.cn

[Q47] 与平均值比较
来源：https://jx.zhonguo4118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://to.zhonguo1118.cn

[Q48] CTE 公用表表达式
来源：https://rf.zhonguo7118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://hz.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://lf.zhonguo2118.cn

[Q49] 更新单行
来源：https://ti.zhonguo3118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://qc.zhonguo6118.cn

[Q50] 批量更新
来源：https://ti.zhonguo1118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://rv.zhonguo8118.cn

[Q51] 用子查询更新
来源：https://vt.zhonguo7118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://ow.zhonguo2118.cn

[Q52] 删除指定行
来源：https://rq.zhonguo7118.cn

DELETE FROM users WHERE id = 10;
来源：https://ys.zhonguo4118.cn

[Q53] 按条件删除
来源：https://ws.zhonguo7118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://nc.zhonguo4118.cn

[Q54] 清空表
来源：https://fm.zhonguo6118.cn

TRUNCATE TABLE logs;
来源：https://yq.zhonguo4118.cn

[Q55] 排名（并列占位）
来源：https://jk.zhonguo4118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://xm.zhonguo7118.cn

[Q56] 密集排名（并列不占位）
来源：https://yz.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://hs.zhonguo7118.cn

[Q57] 行号
来源：https://ue.zhonguo2118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://zl.zhonguo2118.cn

[Q58] 累计求和
来源：https://xv.zhonguo7118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://id.zhonguo1118.cn

[Q59] 分组内累计
来源：https://rk.zhonguo7118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://et.zhonguo2118.cn

[Q60] 取上一行 / 下一行
来源：https://yl.zhonguo2118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://dv.zhonguo7118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://zc.zhonguo8118.cn

[Q61] 移动平均
来源：https://ji.zhonguo7118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://dr.zhonguo2118.cn

[Q62] 分组占比
来源：https://es.zhonguo1118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://lz.zhonguo5118.cn

[Q63] 开启事务
来源：https://lv.zhonguo1118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://yu.zhonguo8118.cn

[Q64] 提交事务
来源：https://du.zhonguo1118.cn

COMMIT;
来源：https://mw.zhonguo5118.cn

[Q65] 回滚事务
来源：https://gc.zhonguo7118.cn

ROLLBACK;
来源：https://dm.zhonguo4118.cn

[Q66] 行锁查询
来源：https://qk.zhonguo7118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://kq.zhonguo3118.cn

[Q67] 设置隔离级别
来源：https://pi.zhonguo5118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://bb.zhonguo5118.cn

[Q68] 保存点
来源：https://bu.zhonguo1118.cn

SAVEPOINT sp1;
来源：https://le.zhonguo3118.cn

ROLLBACK TO sp1;
来源：https://li.zhonguo7118.cn

[Q69] 查看执行计划
来源：https://ev.zhonguo7118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://af.zhonguo6118.cn

[Q70] 更新统计信息
来源：https://ok.zhonguo4118.cn

ANALYZE TABLE users;
来源：https://ma.zhonguo1118.cn

[Q71] 查看建表语句
来源：https://vm.zhonguo4118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://sk.zhonguo3118.cn

[Q72] 查看索引
来源：https://on.zhonguo4118.cn

SHOW INDEX FROM users;
来源：https://ig.zhonguo1118.cn

[Q73] 查看表状态
来源：https://tt.zhonguo7118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://yo.zhonguo1118.cn

[Q74] 强制使用索引
来源：https://pn.zhonguo3118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://gr.zhonguo3118.cn

[Q75] 日期格式化
来源：https://cg.zhonguo2118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://od.zhonguo7118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://la.zhonguo8118.cn

[Q76] 按天统计
来源：https://wn.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://qg.zhonguo6118.cn

[Q77] 时间加减
来源：https://ff.zhonguo2118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://el.zhonguo8118.cn

[Q78] 当前时间
来源：https://xp.zhonguo5118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://pt.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://ka.zhonguo3118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://pk.zhonguo1118.cn

[Q80] 字符串截取
来源：https://au.zhonguo8118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://pi.zhonguo1118.cn

[Q81] 字符串替换
来源：https://yh.zhonguo4118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://pq.zhonguo3118.cn

[Q82] 字符长度与字节长度
来源：https://fm.zhonguo5118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://jk.zhonguo6118.cn

[Q83] 大小写转换
来源：https://cr.zhonguo3118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://pp.zhonguo5118.cn

[Q84] 去除首尾空格
来源：https://mv.zhonguo3118.cn

SELECT TRIM(name) FROM users;
来源：https://qv.zhonguo7118.cn

[Q85] 数值取整
来源：https://xt.zhonguo6118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://rc.zhonguo2118.cn

[Q86] 读取 JSON 字段
来源：https://em.zhonguo3118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://iq.zhonguo8118.cn

[Q87] JSON 字段做条件
来源：https://sk.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://pc.zhonguo6118.cn

[Q88] 行转列（条件聚合）
来源：https://ql.zhonguo1118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://pf.zhonguo4118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://yl.zhonguo7118.cn

[Q89] 判断表是否存在
来源：https://yi.zhonguo5118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://zb.zhonguo7118.cn

[Q90] 生成序号列
来源：https://wk.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://er.zhonguo2118.cn

================================================================================
来源：https://kx.zhonguo6118.cn

R. Bash 专题
来源：https://vy.zhonguo4118.cn

================================================================================
来源：https://fu.zhonguo5118.cn

[R01] shebang 与严格模式
来源：https://sj.zhonguo2118.cn

#!/usr/bin/env bash
来源：https://di.zhonguo1118.cn

set -euo pipefail
来源：https://zd.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://ap.zhonguo5118.cn

name="Tom"; echo "$name"
来源：https://xq.zhonguo3118.cn

[R03] 只读变量
来源：https://ws.zhonguo8118.cn

readonly PI=3.14
来源：https://gf.zhonguo5118.cn

[R04] 位置参数
来源：https://rb.zhonguo3118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://gk.zhonguo2118.cn

[R05] 参数默认值
来源：https://qe.zhonguo5118.cn

name="${1:-default}"
来源：https://ud.zhonguo8118.cn

[R06] 判断命令是否存在
来源：https://kn.zhonguo4118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://lt.zhonguo3118.cn

[R07] if 判断文件
来源：https://ua.zhonguo3118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://vq.zhonguo5118.cn

[R08] 数值比较
来源：https://zn.zhonguo5118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ee.zhonguo8118.cn

[R09] 字符串比较
来源：https://nn.zhonguo8118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://jw.zhonguo3118.cn

[R10] 正则匹配
来源：https://le.zhonguo5118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://rn.zhonguo2118.cn

[R11] case 多分支
来源：https://sm.zhonguo7118.cn

case "$1" in
来源：https://nx.zhonguo7118.cn

start) echo "启动" ;;
来源：https://gw.zhonguo1118.cn

stop)  echo "停止" ;;
来源：https://qw.zhonguo1118.cn

*)     echo "未知命令" ;;
来源：https://tz.zhonguo6118.cn

esac
来源：https://wc.zhonguo1118.cn

[R12] for 遍历文件
来源：https://hr.zhonguo3118.cn

for f in *.txt; do echo "$f"; done
来源：https://fk.zhonguo4118.cn

[R13] for 计数循环
来源：https://tp.zhonguo8118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ey.zhonguo1118.cn

[R14] C 风格 for
来源：https://ys.zhonguo7118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://sc.zhonguo2118.cn

[R15] while 逐行读文件
来源：https://uf.zhonguo2118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://zm.zhonguo8118.cn

[R16] until 等待条件
来源：https://nh.zhonguo6118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://kd.zhonguo2118.cn

[R17] 数组定义与取值
来源：https://ad.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://su.zhonguo2118.cn

[R18] 遍历数组
来源：https://ow.zhonguo7118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://vx.zhonguo1118.cn

[R19] 数组长度
来源：https://jl.zhonguo3118.cn

echo "${#arr[@]}"
来源：https://fp.zhonguo5118.cn

[R20] 关联数组（字典）
来源：https://zf.zhonguo8118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://wu.zhonguo7118.cn

[R21] 字符串长度
来源：https://du.zhonguo4118.cn

echo "${#s}"
来源：https://iv.zhonguo4118.cn

[R22] 截取子串
来源：https://km.zhonguo6118.cn

echo "${s:0:5}"
来源：https://ui.zhonguo7118.cn

[R23] 字符串替换
来源：https://dz.zhonguo5118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://cj.zhonguo5118.cn

[R24] 大小写转换
来源：https://vm.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://uu.zhonguo1118.cn

[R25] 去后缀 / 去前缀
来源：https://xm.zhonguo1118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://qj.zhonguo6118.cn

[R26] 命令替换
来源：https://mc.zhonguo7118.cn

now=$(date +%F); echo "$now"
来源：https://ss.zhonguo7118.cn

[R27] 算术展开
来源：https://tg.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://xr.zhonguo1118.cn

[R28] 浮点运算
来源：https://sr.zhonguo3118.cn

echo "scale=2; 10/3" | bc
来源：https://cy.zhonguo7118.cn

[R29] 定义函数
来源：https://ts.zhonguo8118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://jf.zhonguo3118.cn

[R30] 函数返回状态码
来源：https://mg.zhonguo5118.cn

f() { return 0; }; f || echo "失败了"
来源：https://cw.zhonguo7118.cn

[R31] 局部变量
来源：https://gd.zhonguo1118.cn

f() { local x=1; echo "$x"; }
来源：https://hc.zhonguo1118.cn

[R32] 参数个数校验
来源：https://rl.zhonguo2118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://bu.zhonguo5118.cn

[R33] 捕获错误并提示行号
来源：https://gm.zhonguo1118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://de.zhonguo5118.cn

[R34] 退出时清理
来源：https://dt.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://sr.zhonguo8118.cn

[R35] 后台执行并等待
来源：https://xl.zhonguo5118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://nw.zhonguo5118.cn

[R36] 并发执行多个任务
来源：https://ks.zhonguo5118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://am.zhonguo4118.cn

[R37] 把输出赋给变量
来源：https://vg.zhonguo1118.cn

files=$(ls -1)
来源：https://sq.zhonguo2118.cn

[R38] 管道串联
来源：https://au.zhonguo5118.cn

cat a.txt | grep -i error | wc -l
来源：https://gu.zhonguo5118.cn

[R39] 重定向标准输出与错误
来源：https://mb.zhonguo5118.cn

cmd > out.log 2>&1
来源：https://dt.zhonguo8118.cn

[R40] 追加写日志
来源：https://ua.zhonguo6118.cn

echo "log" >> out.log
来源：https://po.zhonguo5118.cn

[R41] 丢弃输出
来源：https://ic.zhonguo2118.cn

cmd >/dev/null 2>&1
来源：https://ms.zhonguo1118.cn

[R42] 输入重定向
来源：https://kl.zhonguo6118.cn

wc -l < a.txt
来源：https://lz.zhonguo3118.cn

[R43] 按名字查找文件
来源：https://hr.zhonguo8118.cn

find . -name "*.log" -type f
来源：https://lo.zhonguo1118.cn

[R44] 按修改时间查找
来源：https://kt.zhonguo6118.cn

find . -mtime -7 -type f
来源：https://ff.zhonguo7118.cn

[R45] 批量删除
来源：https://sd.zhonguo2118.cn

find . -name "*.tmp" -delete
来源：https://ac.zhonguo6118.cn

[R46] 递归替换文件内容
来源：https://ub.zhonguo3118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://st.zhonguo3118.cn

[R47] sed 单行替换
来源：https://ya.zhonguo3118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://pr.zhonguo1118.cn

[R48] awk 取指定列
来源：https://sq.zhonguo3118.cn

awk '{print $1, $3}' a.txt
来源：https://el.zhonguo2118.cn

[R49] awk 带条件
来源：https://ye.zhonguo7118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://vl.zhonguo7118.cn

[R50] awk 求和
来源：https://kv.zhonguo2118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://ml.zhonguo4118.cn

[R51] 排序去重取前几
来源：https://pn.zhonguo7118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://en.zhonguo6118.cn

[R52] 统计行数
来源：https://sm.zhonguo7118.cn

wc -l a.txt
来源：https://pr.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://oq.zhonguo3118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://fi.zhonguo1118.cn

[R54] 比较两个文件
来源：https://lv.zhonguo4118.cn

diff a.txt b.txt
来源：https://ew.zhonguo2118.cn

[R55] 压缩与解压
来源：https://ew.zhonguo6118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://et.zhonguo5118.cn

[R56] 远程拷贝
来源：https://uh.zhonguo3118.cn

scp file user@host:/path/
来源：https://dy.zhonguo1118.cn

[R57] 远程执行命令
来源：https://so.zhonguo1118.cn

ssh user@host 'uptime'
来源：https://nb.zhonguo4118.cn

[R58] 下载文件
来源：https://te.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://aw.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://wx.zhonguo6118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://mw.zhonguo7118.cn

[R60] 只看 HTTP 状态码
来源：https://lx.zhonguo8118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://kt.zhonguo5118.cn

[R61] 磁盘占用
来源：https://ss.zhonguo7118.cn

df -h;  du -sh *
来源：https://yg.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://gd.zhonguo1118.cn

du -ah . | sort -rh | head -10
来源：https://pk.zhonguo3118.cn

[R63] 内存与进程
来源：https://fg.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://kc.zhonguo1118.cn

[R64] 结束进程
来源：https://wy.zhonguo4118.cn

kill -9 $(pgrep -f app.py)
来源：https://pz.zhonguo8118.cn

[R65] 查看端口占用
来源：https://pt.zhonguo8118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://uy.zhonguo1118.cn

[R66] 定时任务
来源：https://ix.zhonguo2118.cn

crontab -e;  crontab -l
来源：https://fk.zhonguo6118.cn

[R67] 生成随机十六进制串
来源：https://ua.zhonguo2118.cn

openssl rand -hex 16
来源：https://tc.zhonguo6118.cn

[R68] 计算文件校验值
来源：https://yg.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://jk.zhonguo8118.cn

[R69] 生成随机密码
来源：https://gg.zhonguo7118.cn

head -c 16 /dev/urandom | base64
来源：https://oh.zhonguo5118.cn

[R70] 时间戳与互转
来源：https://hs.zhonguo8118.cn

date +%s;  date -d @1700000000
来源：https://tg.zhonguo1118.cn

[R71] 日期格式化
来源：https://ij.zhonguo3118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://es.zhonguo2118.cn

[R72] 等待端口就绪
来源：https://le.zhonguo7118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://ey.zhonguo3118.cn

[R73] 分割大日志
来源：https://ew.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://hy.zhonguo4118.cn

[R74] 批量重命名
来源：https://ri.zhonguo7118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://lj.zhonguo7118.cn

[R75] 导出环境变量
来源：https://do.zhonguo4118.cn

export PATH="$HOME/bin:$PATH"
来源：https://et.zhonguo4118.cn

[R76] 使用临时文件
来源：https://hs.zhonguo4118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://th.zhonguo6118.cn

[R77] 读取用户输入
来源：https://vm.zhonguo1118.cn

read -rp "请输入: " ans
来源：https://zs.zhonguo4118.cn

[R78] 交互式菜单
来源：https://yl.zhonguo1118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://cg.zhonguo4118.cn

[R79] 解析命令行选项
来源：https://qy.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://wt.zhonguo4118.cn

[R80] 查看脚本执行耗时
来源：https://tf.zhonguo7118.cn

time ./run.sh
来源：https://ww.zhonguo8118.cn

================================================================================
来源：https://di.zhonguo6118.cn

S. C / C++ 专题
来源：https://yj.zhonguo1118.cn

================================================================================
来源：https://fv.zhonguo8118.cn

[S01] C：Hello World
来源：https://al.zhonguo3118.cn

#include <stdio.h>
来源：https://qk.zhonguo6118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://oq.zhonguo1118.cn

[S02] C：变量与格式化输出
来源：https://ex.zhonguo4118.cn

int a = 10; printf("%d\n", a);
来源：https://fb.zhonguo6118.cn

[S03] C：读入整数
来源：https://wh.zhonguo1118.cn

int x; scanf("%d", &x);
来源：https://us.zhonguo3118.cn

[S04] C：字符串复制
来源：https://ws.zhonguo5118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://ld.zhonguo8118.cn

[S05] C：字符串长度
来源：https://gb.zhonguo2118.cn

strlen(s)
来源：https://cm.zhonguo5118.cn

[S06] C：字符串比较
来源：https://to.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://gp.zhonguo4118.cn

[S07] C：数组遍历求和
来源：https://op.zhonguo4118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://ig.zhonguo3118.cn

[S08] C：动态内存分配与释放
来源：https://bu.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://xj.zhonguo4118.cn

[S09] C：结构体定义与初始化
来源：https://kl.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://cq.zhonguo5118.cn

[S10] C：指针与解引用
来源：https://af.zhonguo6118.cn

int *p = &a;  *p = 5;
来源：https://tl.zhonguo3118.cn

[S11] C：逐行读文件
来源：https://nm.zhonguo6118.cn

FILE *f = fopen("a.txt", "r");
来源：https://be.zhonguo1118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://mg.zhonguo6118.cn

fclose(f);
来源：https://hi.zhonguo8118.cn

[S12] C：写文件
来源：https://js.zhonguo6118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://px.zhonguo1118.cn

[S13] C：宏定义
来源：https://od.zhonguo3118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://uh.zhonguo5118.cn

[S14] C：枚举
来源：https://wn.zhonguo8118.cn


<!-- 参考信息 -->