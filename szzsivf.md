代发 wailian999

[Q61] 移动平均
来源：https://gw.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://pf.zhonguo8118.cn

[Q62] 分组占比
来源：https://ow.zhonguo1118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://xg.zhonguo4118.cn

[Q63] 开启事务
来源：https://vt.zhonguo3118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://ur.zhonguo4118.cn

[Q64] 提交事务
来源：https://aw.zhonguo3118.cn

COMMIT;
来源：https://dn.zhonguo7118.cn

[Q65] 回滚事务
来源：https://rr.zhonguo5118.cn

ROLLBACK;
来源：https://zr.zhonguo2118.cn

[Q66] 行锁查询
来源：https://xn.zhonguo6118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://ad.zhonguo8118.cn

[Q67] 设置隔离级别
来源：https://vv.zhonguo8118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://zj.zhonguo3118.cn

[Q68] 保存点
来源：https://ut.zhonguo4118.cn

SAVEPOINT sp1;
来源：https://vx.zhonguo6118.cn

ROLLBACK TO sp1;
来源：https://rf.zhonguo5118.cn

[Q69] 查看执行计划
来源：https://mq.zhonguo8118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://fy.zhonguo6118.cn

[Q70] 更新统计信息
来源：https://wr.zhonguo1118.cn

ANALYZE TABLE users;
来源：https://ml.zhonguo3118.cn

[Q71] 查看建表语句
来源：https://by.zhonguo1118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://tf.zhonguo5118.cn

[Q72] 查看索引
来源：https://xo.zhonguo6118.cn

SHOW INDEX FROM users;
来源：https://um.zhonguo7118.cn

[Q73] 查看表状态
来源：https://wz.zhonguo7118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://or.zhonguo5118.cn

[Q74] 强制使用索引
来源：https://cf.zhonguo4118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://tf.zhonguo1118.cn

[Q75] 日期格式化
来源：https://ix.zhonguo6118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://zz.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://xe.zhonguo7118.cn

[Q76] 按天统计
来源：https://ey.zhonguo2118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://pn.zhonguo4118.cn

[Q77] 时间加减
来源：https://wi.zhonguo2118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://bl.zhonguo1118.cn

[Q78] 当前时间
来源：https://gf.zhonguo4118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://sq.zhonguo7118.cn

[Q79] 字符串拼接
来源：https://go.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://wr.zhonguo1118.cn

[Q80] 字符串截取
来源：https://mo.zhonguo7118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://ox.zhonguo5118.cn

[Q81] 字符串替换
来源：https://lu.zhonguo5118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://tj.zhonguo2118.cn

[Q82] 字符长度与字节长度
来源：https://cf.zhonguo6118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://pq.zhonguo1118.cn

[Q83] 大小写转换
来源：https://rx.zhonguo5118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ph.zhonguo1118.cn

[Q84] 去除首尾空格
来源：https://gf.zhonguo4118.cn

SELECT TRIM(name) FROM users;
来源：https://lg.zhonguo5118.cn

[Q85] 数值取整
来源：https://ya.zhonguo6118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://xi.zhonguo5118.cn

[Q86] 读取 JSON 字段
来源：https://ld.zhonguo7118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://on.zhonguo3118.cn

[Q87] JSON 字段做条件
来源：https://ow.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://xr.zhonguo4118.cn

[Q88] 行转列（条件聚合）
来源：https://ub.zhonguo8118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://tl.zhonguo2118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://eh.zhonguo6118.cn

[Q89] 判断表是否存在
来源：https://pu.zhonguo8118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://ca.zhonguo8118.cn

[Q90] 生成序号列
来源：https://bv.zhonguo5118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ja.zhonguo1118.cn

================================================================================
来源：https://le.zhonguo8118.cn

R. Bash 专题
来源：https://yn.zhonguo8118.cn

================================================================================
来源：https://dv.zhonguo1118.cn

[R01] shebang 与严格模式
来源：https://eq.zhonguo8118.cn

#!/usr/bin/env bash
来源：https://th.zhonguo8118.cn

set -euo pipefail
来源：https://vq.zhonguo4118.cn

[R02] 变量赋值与使用
来源：https://fc.zhonguo3118.cn

name="Tom"; echo "$name"
来源：https://rj.zhonguo3118.cn

[R03] 只读变量
来源：https://ba.zhonguo4118.cn

readonly PI=3.14
来源：https://tr.zhonguo6118.cn

[R04] 位置参数
来源：https://oh.zhonguo8118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://mq.zhonguo1118.cn

[R05] 参数默认值
来源：https://lv.zhonguo8118.cn

name="${1:-default}"
来源：https://bm.zhonguo8118.cn

[R06] 判断命令是否存在
来源：https://ag.zhonguo1118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://kk.zhonguo1118.cn

[R07] if 判断文件
来源：https://dr.zhonguo7118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://bg.zhonguo6118.cn

[R08] 数值比较
来源：https://vt.zhonguo7118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://su.zhonguo4118.cn

[R09] 字符串比较
来源：https://eg.zhonguo6118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://fj.zhonguo6118.cn

[R10] 正则匹配
来源：https://gy.zhonguo2118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://hk.zhonguo2118.cn

[R11] case 多分支
来源：https://uu.zhonguo5118.cn

case "$1" in
来源：https://vi.zhonguo7118.cn

start) echo "启动" ;;
来源：https://xl.zhonguo5118.cn

stop)  echo "停止" ;;
来源：https://rj.zhonguo7118.cn

*)     echo "未知命令" ;;
来源：https://vw.zhonguo4118.cn

esac
来源：https://ih.zhonguo5118.cn

[R12] for 遍历文件
来源：https://cm.zhonguo4118.cn

for f in *.txt; do echo "$f"; done
来源：https://ym.zhonguo8118.cn

[R13] for 计数循环
来源：https://ep.zhonguo7118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ry.zhonguo3118.cn

[R14] C 风格 for
来源：https://re.zhonguo7118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://li.zhonguo7118.cn

[R15] while 逐行读文件
来源：https://vv.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://qu.zhonguo5118.cn

[R16] until 等待条件
来源：https://ga.zhonguo6118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://vd.zhonguo4118.cn

[R17] 数组定义与取值
来源：https://ay.zhonguo5118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://wi.zhonguo3118.cn

[R18] 遍历数组
来源：https://ji.zhonguo2118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://wv.zhonguo1118.cn

[R19] 数组长度
来源：https://tl.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://bu.zhonguo1118.cn

[R20] 关联数组（字典）
来源：https://qb.zhonguo1118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://vx.zhonguo8118.cn

[R21] 字符串长度
来源：https://hb.zhonguo5118.cn

echo "${#s}"
来源：https://ns.zhonguo5118.cn

[R22] 截取子串
来源：https://pw.zhonguo4118.cn

echo "${s:0:5}"
来源：https://zc.zhonguo7118.cn

[R23] 字符串替换
来源：https://gs.zhonguo2118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://ud.zhonguo2118.cn

[R24] 大小写转换
来源：https://ae.zhonguo8118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ub.zhonguo8118.cn

[R25] 去后缀 / 去前缀
来源：https://zt.zhonguo3118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://ys.zhonguo2118.cn

[R26] 命令替换
来源：https://uk.zhonguo3118.cn

now=$(date +%F); echo "$now"
来源：https://ij.zhonguo7118.cn

[R27] 算术展开
来源：https://pp.zhonguo1118.cn

echo $((1 + 2 * 3))
来源：https://mu.zhonguo7118.cn

[R28] 浮点运算
来源：https://nu.zhonguo5118.cn

echo "scale=2; 10/3" | bc
来源：https://dx.zhonguo1118.cn

[R29] 定义函数
来源：https://wh.zhonguo2118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://le.zhonguo6118.cn

[R30] 函数返回状态码
来源：https://ok.zhonguo5118.cn

f() { return 0; }; f || echo "失败了"
来源：https://gr.zhonguo1118.cn

[R31] 局部变量
来源：https://gb.zhonguo1118.cn

f() { local x=1; echo "$x"; }
来源：https://ht.zhonguo4118.cn

[R32] 参数个数校验
来源：https://yr.zhonguo3118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://ki.zhonguo1118.cn

[R33] 捕获错误并提示行号
来源：https://pk.zhonguo8118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://bn.zhonguo2118.cn

[R34] 退出时清理
来源：https://bz.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://rk.zhonguo6118.cn

[R35] 后台执行并等待
来源：https://tv.zhonguo5118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://na.zhonguo8118.cn

[R36] 并发执行多个任务
来源：https://zx.zhonguo1118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://ih.zhonguo7118.cn

[R37] 把输出赋给变量
来源：https://wi.zhonguo7118.cn

files=$(ls -1)
来源：https://sx.zhonguo3118.cn

[R38] 管道串联
来源：https://wm.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://fa.zhonguo2118.cn

[R39] 重定向标准输出与错误
来源：https://uu.zhonguo2118.cn

cmd > out.log 2>&1
来源：https://lv.zhonguo7118.cn

[R40] 追加写日志
来源：https://ur.zhonguo5118.cn

echo "log" >> out.log
来源：https://yh.zhonguo2118.cn

[R41] 丢弃输出
来源：https://eu.zhonguo2118.cn

cmd >/dev/null 2>&1
来源：https://iu.zhonguo5118.cn

[R42] 输入重定向
来源：https://kh.zhonguo7118.cn

wc -l < a.txt
来源：https://ia.zhonguo2118.cn

[R43] 按名字查找文件
来源：https://rl.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://oy.zhonguo4118.cn

[R44] 按修改时间查找
来源：https://hf.zhonguo8118.cn

find . -mtime -7 -type f
来源：https://jn.zhonguo2118.cn

[R45] 批量删除
来源：https://rx.zhonguo8118.cn

find . -name "*.tmp" -delete
来源：https://ri.zhonguo1118.cn

[R46] 递归替换文件内容
来源：https://aq.zhonguo7118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://jd.zhonguo8118.cn

[R47] sed 单行替换
来源：https://jt.zhonguo7118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://rh.zhonguo4118.cn

[R48] awk 取指定列
来源：https://dj.zhonguo4118.cn

awk '{print $1, $3}' a.txt
来源：https://lm.zhonguo3118.cn

[R49] awk 带条件
来源：https://fk.zhonguo2118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ef.zhonguo4118.cn

[R50] awk 求和
来源：https://ra.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://iu.zhonguo8118.cn

[R51] 排序去重取前几
来源：https://ay.zhonguo3118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://zx.zhonguo4118.cn

[R52] 统计行数
来源：https://gq.zhonguo7118.cn

wc -l a.txt
来源：https://hp.zhonguo8118.cn

[R53] 查看文件头与实时尾
来源：https://fa.zhonguo3118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://in.zhonguo3118.cn

[R54] 比较两个文件
来源：https://or.zhonguo8118.cn

diff a.txt b.txt
来源：https://nh.zhonguo1118.cn

[R55] 压缩与解压
来源：https://mc.zhonguo1118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://sv.zhonguo5118.cn

[R56] 远程拷贝
来源：https://in.zhonguo1118.cn

scp file user@host:/path/
来源：https://nl.zhonguo7118.cn

[R57] 远程执行命令
来源：https://hz.zhonguo2118.cn

ssh user@host 'uptime'
来源：https://on.zhonguo5118.cn

[R58] 下载文件
来源：https://uc.zhonguo3118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://qj.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://xs.zhonguo7118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://ch.zhonguo1118.cn

[R60] 只看 HTTP 状态码
来源：https://tg.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://nn.zhonguo1118.cn

[R61] 磁盘占用
来源：https://tl.zhonguo2118.cn

df -h;  du -sh *
来源：https://mz.zhonguo8118.cn

[R62] 找最占空间的文件
来源：https://eg.zhonguo7118.cn

du -ah . | sort -rh | head -10
来源：https://fn.zhonguo4118.cn

[R63] 内存与进程
来源：https://cc.zhonguo2118.cn

free -h;  ps aux | grep nginx
来源：https://mj.zhonguo8118.cn

[R64] 结束进程
来源：https://bc.zhonguo4118.cn

kill -9 $(pgrep -f app.py)
来源：https://wq.zhonguo8118.cn

[R65] 查看端口占用
来源：https://fb.zhonguo2118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://zy.zhonguo7118.cn

[R66] 定时任务
来源：https://uk.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://ea.zhonguo4118.cn

[R67] 生成随机十六进制串
来源：https://ys.zhonguo7118.cn

openssl rand -hex 16
来源：https://kd.zhonguo8118.cn

[R68] 计算文件校验值
来源：https://zx.zhonguo1118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://wp.zhonguo2118.cn

[R69] 生成随机密码
来源：https://hx.zhonguo5118.cn

head -c 16 /dev/urandom | base64
来源：https://cz.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://ki.zhonguo5118.cn

date +%s;  date -d @1700000000
来源：https://yw.zhonguo2118.cn

[R71] 日期格式化
来源：https://yx.zhonguo7118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://dl.zhonguo3118.cn

[R72] 等待端口就绪
来源：https://pc.zhonguo2118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://nc.zhonguo5118.cn

[R73] 分割大日志
来源：https://xm.zhonguo6118.cn

split -l 1000 big.log part_
来源：https://ef.zhonguo6118.cn

[R74] 批量重命名
来源：https://jk.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ae.zhonguo1118.cn

[R75] 导出环境变量
来源：https://tz.zhonguo4118.cn

export PATH="$HOME/bin:$PATH"
来源：https://sk.zhonguo5118.cn

[R76] 使用临时文件
来源：https://uu.zhonguo4118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://do.zhonguo1118.cn

[R77] 读取用户输入
来源：https://hn.zhonguo1118.cn

read -rp "请输入: " ans
来源：https://xq.zhonguo1118.cn

[R78] 交互式菜单
来源：https://wq.zhonguo8118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://wy.zhonguo8118.cn

[R79] 解析命令行选项
来源：https://qu.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://up.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://zg.zhonguo2118.cn

time ./run.sh
来源：https://bv.zhonguo4118.cn

================================================================================
来源：https://qa.zhonguo5118.cn

S. C / C++ 专题
来源：https://nb.zhonguo3118.cn

================================================================================
来源：https://pa.zhonguo7118.cn

[S01] C：Hello World
来源：https://zn.zhonguo2118.cn

#include <stdio.h>
来源：https://qu.zhonguo7118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://xs.zhonguo8118.cn

[S02] C：变量与格式化输出
来源：https://zd.zhonguo1118.cn

int a = 10; printf("%d\n", a);
来源：https://um.zhonguo7118.cn

[S03] C：读入整数
来源：https://wf.zhonguo3118.cn

int x; scanf("%d", &x);
来源：https://bz.zhonguo1118.cn

[S04] C：字符串复制
来源：https://lu.zhonguo6118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://uf.zhonguo5118.cn

[S05] C：字符串长度
来源：https://jj.zhonguo5118.cn

strlen(s)
来源：https://dz.zhonguo4118.cn

[S06] C：字符串比较
来源：https://ge.zhonguo2118.cn

strcmp(a, b) == 0
来源：https://rc.zhonguo3118.cn

[S07] C：数组遍历求和
来源：https://kv.zhonguo5118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://as.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://yk.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://xw.zhonguo3118.cn

[S09] C：结构体定义与初始化
来源：https://kt.zhonguo6118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://qy.zhonguo1118.cn

[S10] C：指针与解引用
来源：https://tm.zhonguo3118.cn

int *p = &a;  *p = 5;
来源：https://ll.zhonguo5118.cn

[S11] C：逐行读文件
来源：https://om.zhonguo1118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ca.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://dj.zhonguo1118.cn

fclose(f);
来源：https://ue.zhonguo5118.cn

[S12] C：写文件
来源：https://ec.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://bp.zhonguo7118.cn

[S13] C：宏定义
来源：https://am.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://td.zhonguo3118.cn

[S14] C：枚举
来源：https://hk.zhonguo5118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ei.zhonguo8118.cn

[S15] C：类型转换
来源：https://jb.zhonguo1118.cn

(double) a / b
来源：https://ea.zhonguo6118.cn

[S16] C：位操作置位
来源：https://cg.zhonguo3118.cn

x |= (1 << 3);
来源：https://sf.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://be.zhonguo4118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://rf.zhonguo5118.cn

[S18] C：命令行参数
来源：https://ak.zhonguo7118.cn

int main(int argc, char **argv)
来源：https://cb.zhonguo2118.cn

[S19] C：快速排序
来源：https://pj.zhonguo2118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://vk.zhonguo7118.cn

[S20] C：二分查找
来源：https://oo.zhonguo5118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://cv.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://bz.zhonguo6118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://pn.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://rp.zhonguo5118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://ic.zhonguo8118.cn

[S23] C：随机数
来源：https://cf.zhonguo8118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ph.zhonguo3118.cn

[S24] C：获取本地时间
来源：https://eq.zhonguo4118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ae.zhonguo8118.cn

[S25] C：内存拷贝
来源：https://jv.zhonguo1118.cn

memcpy(dst, src, n);
来源：https://rp.zhonguo6118.cn

[S26] C：内存清零
来源：https://ha.zhonguo6118.cn

memset(a, 0, sizeof a);
来源：https://vu.zhonguo7118.cn

[S27] C：定义常量
来源：https://lt.zhonguo2118.cn

const double PI = 3.14159;
来源：https://nx.zhonguo8118.cn

[S28] C：静态变量
来源：https://jh.zhonguo8118.cn

static int counter = 0;
来源：https://kb.zhonguo8118.cn

[S29] C：变参函数
来源：https://ok.zhonguo4118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://ao.zhonguo4118.cn

[S30] C：头文件保护
来源：https://jq.zhonguo8118.cn

#ifndef X_H
来源：https://pr.zhonguo4118.cn

#define X_H
来源：https://sq.zhonguo2118.cn

#endif
来源：https://gv.zhonguo3118.cn

[S31] C++：Hello World
来源：https://hg.zhonguo4118.cn


<!-- 参考信息 -->