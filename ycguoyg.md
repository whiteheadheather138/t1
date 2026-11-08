代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：https://sp.zhonguo5118.cn

[Q50] 批量更新
来源：https://ng.zhonguo3118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://bc.zhonguo1118.cn

[Q51] 用子查询更新
来源：https://jo.zhonguo8118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://xw.zhonguo5118.cn

[Q52] 删除指定行
来源：https://ge.zhonguo7118.cn

DELETE FROM users WHERE id = 10;
来源：https://ee.zhonguo4118.cn

[Q53] 按条件删除
来源：https://sz.zhonguo7118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://hd.zhonguo7118.cn

[Q54] 清空表
来源：https://hd.zhonguo8118.cn

TRUNCATE TABLE logs;
来源：https://no.zhonguo5118.cn

[Q55] 排名（并列占位）
来源：https://nn.zhonguo6118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://je.zhonguo2118.cn

[Q56] 密集排名（并列不占位）
来源：https://hh.zhonguo3118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://th.zhonguo6118.cn

[Q57] 行号
来源：https://bx.zhonguo2118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://ff.zhonguo1118.cn

[Q58] 累计求和
来源：https://ol.zhonguo7118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://df.zhonguo3118.cn

[Q59] 分组内累计
来源：https://ip.zhonguo1118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://hm.zhonguo3118.cn

[Q60] 取上一行 / 下一行
来源：https://lu.zhonguo5118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://us.zhonguo3118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://nl.zhonguo1118.cn

[Q61] 移动平均
来源：https://og.zhonguo7118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://qc.zhonguo6118.cn

[Q62] 分组占比
来源：https://ed.zhonguo5118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://ys.zhonguo6118.cn

[Q63] 开启事务
来源：https://kx.zhonguo8118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://sp.zhonguo8118.cn

[Q64] 提交事务
来源：https://bv.zhonguo5118.cn

COMMIT;
来源：https://kf.zhonguo2118.cn

[Q65] 回滚事务
来源：https://rg.zhonguo1118.cn

ROLLBACK;
来源：https://ff.zhonguo3118.cn

[Q66] 行锁查询
来源：https://pg.zhonguo3118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://zj.zhonguo5118.cn

[Q67] 设置隔离级别
来源：https://nd.zhonguo3118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://zu.zhonguo8118.cn

[Q68] 保存点
来源：https://dy.zhonguo2118.cn

SAVEPOINT sp1;
来源：https://gx.zhonguo5118.cn

ROLLBACK TO sp1;
来源：https://kb.zhonguo2118.cn

[Q69] 查看执行计划
来源：https://tb.zhonguo5118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://sa.zhonguo8118.cn

[Q70] 更新统计信息
来源：https://fo.zhonguo6118.cn

ANALYZE TABLE users;
来源：https://qd.zhonguo8118.cn

[Q71] 查看建表语句
来源：https://zh.zhonguo1118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://sp.zhonguo5118.cn

[Q72] 查看索引
来源：https://io.zhonguo6118.cn

SHOW INDEX FROM users;
来源：https://qw.zhonguo3118.cn

[Q73] 查看表状态
来源：https://uq.zhonguo1118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://bd.zhonguo8118.cn

[Q74] 强制使用索引
来源：https://ko.zhonguo5118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://tn.zhonguo3118.cn

[Q75] 日期格式化
来源：https://dq.zhonguo1118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://ig.zhonguo5118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://vf.zhonguo3118.cn

[Q76] 按天统计
来源：https://qg.zhonguo6118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ce.zhonguo8118.cn

[Q77] 时间加减
来源：https://ha.zhonguo4118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://ko.zhonguo4118.cn

[Q78] 当前时间
来源：https://uq.zhonguo4118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://my.zhonguo8118.cn

[Q79] 字符串拼接
来源：https://ec.zhonguo4118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://bo.zhonguo6118.cn

[Q80] 字符串截取
来源：https://yb.zhonguo2118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://to.zhonguo8118.cn

[Q81] 字符串替换
来源：https://ip.zhonguo3118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://sb.zhonguo6118.cn

[Q82] 字符长度与字节长度
来源：https://kb.zhonguo3118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://jh.zhonguo8118.cn

[Q83] 大小写转换
来源：https://ua.zhonguo2118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://xs.zhonguo1118.cn

[Q84] 去除首尾空格
来源：https://qu.zhonguo3118.cn

SELECT TRIM(name) FROM users;
来源：https://jg.zhonguo4118.cn

[Q85] 数值取整
来源：https://nu.zhonguo7118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://on.zhonguo1118.cn

[Q86] 读取 JSON 字段
来源：https://lf.zhonguo5118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://xc.zhonguo1118.cn

[Q87] JSON 字段做条件
来源：https://sb.zhonguo2118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://ls.zhonguo2118.cn

[Q88] 行转列（条件聚合）
来源：https://zq.zhonguo2118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://zo.zhonguo2118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://mm.zhonguo7118.cn

[Q89] 判断表是否存在
来源：https://ta.zhonguo1118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://eh.zhonguo4118.cn

[Q90] 生成序号列
来源：https://qm.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://km.zhonguo7118.cn

================================================================================
来源：https://be.zhonguo4118.cn

R. Bash 专题
来源：https://on.zhonguo8118.cn

================================================================================
来源：https://gv.zhonguo8118.cn

[R01] shebang 与严格模式
来源：https://km.zhonguo4118.cn

#!/usr/bin/env bash
来源：https://et.zhonguo4118.cn

set -euo pipefail
来源：https://kx.zhonguo1118.cn

[R02] 变量赋值与使用
来源：https://dt.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://ml.zhonguo6118.cn

[R03] 只读变量
来源：https://vq.zhonguo4118.cn

readonly PI=3.14
来源：https://oy.zhonguo1118.cn

[R04] 位置参数
来源：https://tk.zhonguo6118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://me.zhonguo2118.cn

[R05] 参数默认值
来源：https://zz.zhonguo3118.cn

name="${1:-default}"
来源：https://sz.zhonguo6118.cn

[R06] 判断命令是否存在
来源：https://ai.zhonguo6118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://ct.zhonguo3118.cn

[R07] if 判断文件
来源：https://zw.zhonguo6118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://xg.zhonguo6118.cn

[R08] 数值比较
来源：https://hq.zhonguo1118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://lm.zhonguo3118.cn

[R09] 字符串比较
来源：https://un.zhonguo5118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://lq.zhonguo8118.cn

[R10] 正则匹配
来源：https://cl.zhonguo6118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ny.zhonguo8118.cn

[R11] case 多分支
来源：https://zf.zhonguo1118.cn

case "$1" in
来源：https://xk.zhonguo2118.cn

start) echo "启动" ;;
来源：https://ws.zhonguo5118.cn

stop)  echo "停止" ;;
来源：https://zk.zhonguo8118.cn

*)     echo "未知命令" ;;
来源：https://ca.zhonguo3118.cn

esac
来源：https://kq.zhonguo7118.cn

[R12] for 遍历文件
来源：https://ph.zhonguo5118.cn

for f in *.txt; do echo "$f"; done
来源：https://jo.zhonguo3118.cn

[R13] for 计数循环
来源：https://ua.zhonguo2118.cn

for i in {1..10}; do echo "$i"; done
来源：https://il.zhonguo5118.cn

[R14] C 风格 for
来源：https://we.zhonguo6118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://cp.zhonguo2118.cn

[R15] while 逐行读文件
来源：https://bj.zhonguo3118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://ex.zhonguo5118.cn

[R16] until 等待条件
来源：https://kc.zhonguo1118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://ho.zhonguo4118.cn

[R17] 数组定义与取值
来源：https://oj.zhonguo7118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://gt.zhonguo3118.cn

[R18] 遍历数组
来源：https://zp.zhonguo1118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://qt.zhonguo7118.cn

[R19] 数组长度
来源：https://ug.zhonguo3118.cn

echo "${#arr[@]}"
来源：https://px.zhonguo3118.cn

[R20] 关联数组（字典）
来源：https://ct.zhonguo3118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://mn.zhonguo6118.cn

[R21] 字符串长度
来源：https://bu.zhonguo1118.cn

echo "${#s}"
来源：https://oz.zhonguo6118.cn

[R22] 截取子串
来源：https://vb.zhonguo3118.cn

echo "${s:0:5}"
来源：https://br.zhonguo7118.cn

[R23] 字符串替换
来源：https://ox.zhonguo5118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://rz.zhonguo5118.cn

[R24] 大小写转换
来源：https://yk.zhonguo8118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ru.zhonguo2118.cn

[R25] 去后缀 / 去前缀
来源：https://us.zhonguo1118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://fm.zhonguo4118.cn

[R26] 命令替换
来源：https://ks.zhonguo2118.cn

now=$(date +%F); echo "$now"
来源：https://ow.zhonguo6118.cn

[R27] 算术展开
来源：https://ne.zhonguo1118.cn

echo $((1 + 2 * 3))
来源：https://sh.zhonguo1118.cn

[R28] 浮点运算
来源：https://gg.zhonguo4118.cn

echo "scale=2; 10/3" | bc
来源：https://sh.zhonguo2118.cn

[R29] 定义函数
来源：https://aw.zhonguo8118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://nk.zhonguo1118.cn

[R30] 函数返回状态码
来源：https://vw.zhonguo3118.cn

f() { return 0; }; f || echo "失败了"
来源：https://pd.zhonguo1118.cn

[R31] 局部变量
来源：https://lk.zhonguo1118.cn

f() { local x=1; echo "$x"; }
来源：https://ly.zhonguo1118.cn

[R32] 参数个数校验
来源：https://jp.zhonguo8118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://xz.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://iu.zhonguo3118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://pv.zhonguo2118.cn

[R34] 退出时清理
来源：https://ww.zhonguo1118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://ln.zhonguo3118.cn

[R35] 后台执行并等待
来源：https://lj.zhonguo7118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://xo.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://pk.zhonguo4118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://sk.zhonguo6118.cn

[R37] 把输出赋给变量
来源：https://es.zhonguo6118.cn

files=$(ls -1)
来源：https://wl.zhonguo7118.cn

[R38] 管道串联
来源：https://jr.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://ux.zhonguo4118.cn

[R39] 重定向标准输出与错误
来源：https://kp.zhonguo8118.cn

cmd > out.log 2>&1
来源：https://nf.zhonguo6118.cn

[R40] 追加写日志
来源：https://bc.zhonguo6118.cn

echo "log" >> out.log
来源：https://fg.zhonguo1118.cn

[R41] 丢弃输出
来源：https://vj.zhonguo1118.cn

cmd >/dev/null 2>&1
来源：https://rb.zhonguo8118.cn

[R42] 输入重定向
来源：https://se.zhonguo8118.cn

wc -l < a.txt
来源：https://iv.zhonguo8118.cn

[R43] 按名字查找文件
来源：https://uh.zhonguo7118.cn

find . -name "*.log" -type f
来源：https://rn.zhonguo6118.cn

[R44] 按修改时间查找
来源：https://ij.zhonguo3118.cn

find . -mtime -7 -type f
来源：https://rg.zhonguo1118.cn

[R45] 批量删除
来源：https://xu.zhonguo4118.cn

find . -name "*.tmp" -delete
来源：https://us.zhonguo3118.cn

[R46] 递归替换文件内容
来源：https://vj.zhonguo5118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://oi.zhonguo5118.cn

[R47] sed 单行替换
来源：https://iz.zhonguo4118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://jx.zhonguo8118.cn

[R48] awk 取指定列
来源：https://oh.zhonguo1118.cn

awk '{print $1, $3}' a.txt
来源：https://wh.zhonguo7118.cn

[R49] awk 带条件
来源：https://gq.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://yg.zhonguo2118.cn

[R50] awk 求和
来源：https://bc.zhonguo5118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://qm.zhonguo1118.cn

[R51] 排序去重取前几
来源：https://zl.zhonguo8118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://qm.zhonguo6118.cn

[R52] 统计行数
来源：https://tr.zhonguo2118.cn

wc -l a.txt
来源：https://bu.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://do.zhonguo3118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://pe.zhonguo7118.cn

[R54] 比较两个文件
来源：https://ke.zhonguo6118.cn

diff a.txt b.txt
来源：https://xb.zhonguo8118.cn

[R55] 压缩与解压
来源：https://gr.zhonguo1118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ey.zhonguo5118.cn

[R56] 远程拷贝
来源：https://jk.zhonguo3118.cn

scp file user@host:/path/
来源：https://sj.zhonguo7118.cn

[R57] 远程执行命令
来源：https://wx.zhonguo6118.cn

ssh user@host 'uptime'
来源：https://oc.zhonguo6118.cn

[R58] 下载文件
来源：https://bx.zhonguo2118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://yn.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://iv.zhonguo5118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://rz.zhonguo4118.cn

[R60] 只看 HTTP 状态码
来源：https://lf.zhonguo1118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://th.zhonguo4118.cn

[R61] 磁盘占用
来源：https://yy.zhonguo5118.cn

df -h;  du -sh *
来源：https://lk.zhonguo8118.cn

[R62] 找最占空间的文件
来源：https://hj.zhonguo1118.cn

du -ah . | sort -rh | head -10
来源：https://cm.zhonguo3118.cn

[R63] 内存与进程
来源：https://in.zhonguo7118.cn

free -h;  ps aux | grep nginx
来源：https://ao.zhonguo7118.cn

[R64] 结束进程
来源：https://pn.zhonguo6118.cn

kill -9 $(pgrep -f app.py)
来源：https://tn.zhonguo5118.cn

[R65] 查看端口占用
来源：https://hi.zhonguo5118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://rz.zhonguo5118.cn

[R66] 定时任务
来源：https://hx.zhonguo2118.cn

crontab -e;  crontab -l
来源：https://lk.zhonguo3118.cn

[R67] 生成随机十六进制串
来源：https://je.zhonguo3118.cn

openssl rand -hex 16
来源：https://xi.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://uv.zhonguo4118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://ri.zhonguo4118.cn

[R69] 生成随机密码
来源：https://jb.zhonguo8118.cn

head -c 16 /dev/urandom | base64
来源：https://rp.zhonguo7118.cn

[R70] 时间戳与互转
来源：https://tk.zhonguo8118.cn

date +%s;  date -d @1700000000
来源：https://dm.zhonguo8118.cn

[R71] 日期格式化
来源：https://kr.zhonguo2118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://hg.zhonguo1118.cn

[R72] 等待端口就绪
来源：https://fu.zhonguo7118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://un.zhonguo1118.cn

[R73] 分割大日志
来源：https://aa.zhonguo7118.cn

split -l 1000 big.log part_
来源：https://vi.zhonguo1118.cn

[R74] 批量重命名
来源：https://ea.zhonguo4118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://wx.zhonguo5118.cn

[R75] 导出环境变量
来源：https://tz.zhonguo1118.cn

export PATH="$HOME/bin:$PATH"
来源：https://wv.zhonguo6118.cn

[R76] 使用临时文件
来源：https://xi.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://de.zhonguo8118.cn

[R77] 读取用户输入
来源：https://hx.zhonguo4118.cn

read -rp "请输入: " ans
来源：https://cn.zhonguo8118.cn

[R78] 交互式菜单
来源：https://vv.zhonguo7118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://lw.zhonguo1118.cn

[R79] 解析命令行选项
来源：https://am.zhonguo4118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://yb.zhonguo3118.cn

[R80] 查看脚本执行耗时
来源：https://tw.zhonguo4118.cn

time ./run.sh
来源：https://ii.zhonguo3118.cn

================================================================================
来源：https://ea.zhonguo8118.cn

S. C / C++ 专题
来源：https://or.zhonguo1118.cn

================================================================================
来源：https://hb.zhonguo3118.cn

[S01] C：Hello World
来源：https://cg.zhonguo1118.cn

#include <stdio.h>
来源：https://kv.zhonguo4118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://tm.zhonguo7118.cn

[S02] C：变量与格式化输出
来源：https://nc.zhonguo5118.cn

int a = 10; printf("%d\n", a);
来源：https://ql.zhonguo7118.cn

[S03] C：读入整数
来源：https://zq.zhonguo6118.cn

int x; scanf("%d", &x);
来源：https://ve.zhonguo3118.cn

[S04] C：字符串复制
来源：https://il.zhonguo4118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://vt.zhonguo5118.cn

[S05] C：字符串长度
来源：https://ak.zhonguo4118.cn

strlen(s)
来源：https://sy.zhonguo6118.cn

[S06] C：字符串比较
来源：https://vm.zhonguo4118.cn

strcmp(a, b) == 0
来源：https://iq.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://ej.zhonguo5118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://gf.zhonguo3118.cn

[S08] C：动态内存分配与释放
来源：https://rk.zhonguo6118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://yw.zhonguo3118.cn

[S09] C：结构体定义与初始化
来源：https://ly.zhonguo4118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://jd.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://zm.zhonguo4118.cn

int *p = &a;  *p = 5;
来源：https://ia.zhonguo5118.cn

[S11] C：逐行读文件
来源：https://xw.zhonguo6118.cn

FILE *f = fopen("a.txt", "r");
来源：https://gj.zhonguo3118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://oa.zhonguo7118.cn

fclose(f);
来源：https://nd.zhonguo4118.cn

[S12] C：写文件
来源：https://jr.zhonguo4118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://bk.zhonguo3118.cn

[S13] C：宏定义
来源：https://ll.zhonguo2118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://hy.zhonguo4118.cn

[S14] C：枚举
来源：https://aw.zhonguo7118.cn

enum Color { RED, GREEN, BLUE };
来源：https://st.zhonguo7118.cn

[S15] C：类型转换
来源：https://pg.zhonguo1118.cn

(double) a / b
来源：https://nr.zhonguo7118.cn

[S16] C：位操作置位
来源：https://uq.zhonguo3118.cn

x |= (1 << 3);
来源：https://rw.zhonguo8118.cn

[S17] C：安全拼接字符串
来源：https://uq.zhonguo7118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://nz.zhonguo2118.cn

[S18] C：命令行参数
来源：https://yl.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://xa.zhonguo6118.cn

[S19] C：快速排序
来源：https://mg.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://qe.zhonguo6118.cn

[S20] C：二分查找
来源：https://yx.zhonguo2118.cn


<!-- 参考信息 -->