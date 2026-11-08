代发 wailian999

[Q67] 设置隔离级别
来源：https://ut.zhonguo7118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://wd.zhonguo1118.cn

[Q68] 保存点
来源：https://iw.zhonguo1118.cn

SAVEPOINT sp1;
来源：https://as.zhonguo5118.cn

ROLLBACK TO sp1;
来源：https://lg.zhonguo1118.cn

[Q69] 查看执行计划
来源：https://tn.zhonguo7118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://au.zhonguo4118.cn

[Q70] 更新统计信息
来源：https://qo.zhonguo5118.cn

ANALYZE TABLE users;
来源：https://ys.zhonguo7118.cn

[Q71] 查看建表语句
来源：https://ya.zhonguo2118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://ty.zhonguo1118.cn

[Q72] 查看索引
来源：https://vt.zhonguo2118.cn

SHOW INDEX FROM users;
来源：https://cq.zhonguo7118.cn

[Q73] 查看表状态
来源：https://rk.zhonguo3118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://kp.zhonguo5118.cn

[Q74] 强制使用索引
来源：https://il.zhonguo4118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://lr.zhonguo8118.cn

[Q75] 日期格式化
来源：https://rq.zhonguo7118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://wf.zhonguo1118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://ym.zhonguo4118.cn

[Q76] 按天统计
来源：https://yv.zhonguo2118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://mp.zhonguo3118.cn

[Q77] 时间加减
来源：https://jd.zhonguo7118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://fd.zhonguo4118.cn

[Q78] 当前时间
来源：https://or.zhonguo6118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://me.zhonguo8118.cn

[Q79] 字符串拼接
来源：https://ae.zhonguo2118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://ic.zhonguo2118.cn

[Q80] 字符串截取
来源：https://qj.zhonguo6118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://ll.zhonguo1118.cn

[Q81] 字符串替换
来源：https://ye.zhonguo8118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://st.zhonguo1118.cn

[Q82] 字符长度与字节长度
来源：https://wq.zhonguo4118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://gn.zhonguo8118.cn

[Q83] 大小写转换
来源：https://nj.zhonguo3118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://rv.zhonguo1118.cn

[Q84] 去除首尾空格
来源：https://vs.zhonguo2118.cn

SELECT TRIM(name) FROM users;
来源：https://kb.zhonguo1118.cn

[Q85] 数值取整
来源：https://cl.zhonguo2118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://rh.zhonguo3118.cn

[Q86] 读取 JSON 字段
来源：https://kn.zhonguo7118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://tp.zhonguo5118.cn

[Q87] JSON 字段做条件
来源：https://zz.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://pe.zhonguo7118.cn

[Q88] 行转列（条件聚合）
来源：https://vk.zhonguo8118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://tj.zhonguo7118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://bj.zhonguo5118.cn

[Q89] 判断表是否存在
来源：https://pe.zhonguo4118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://sb.zhonguo4118.cn

[Q90] 生成序号列
来源：https://jr.zhonguo1118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://uy.zhonguo7118.cn

================================================================================
来源：https://bw.zhonguo4118.cn

R. Bash 专题
来源：https://dm.zhonguo2118.cn

================================================================================
来源：https://lw.zhonguo6118.cn

[R01] shebang 与严格模式
来源：https://kc.zhonguo7118.cn

#!/usr/bin/env bash
来源：https://he.zhonguo2118.cn

set -euo pipefail
来源：https://dq.zhonguo6118.cn

[R02] 变量赋值与使用
来源：https://be.zhonguo8118.cn

name="Tom"; echo "$name"
来源：https://wl.zhonguo2118.cn

[R03] 只读变量
来源：https://la.zhonguo4118.cn

readonly PI=3.14
来源：https://zv.zhonguo5118.cn

[R04] 位置参数
来源：https://mn.zhonguo8118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://is.zhonguo3118.cn

[R05] 参数默认值
来源：https://by.zhonguo1118.cn

name="${1:-default}"
来源：https://gq.zhonguo6118.cn

[R06] 判断命令是否存在
来源：https://ld.zhonguo4118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://gz.zhonguo7118.cn

[R07] if 判断文件
来源：https://he.zhonguo1118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://rb.zhonguo1118.cn

[R08] 数值比较
来源：https://eq.zhonguo3118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ae.zhonguo8118.cn

[R09] 字符串比较
来源：https://fz.zhonguo6118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://fi.zhonguo6118.cn

[R10] 正则匹配
来源：https://nt.zhonguo6118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://dv.zhonguo5118.cn

[R11] case 多分支
来源：https://vb.zhonguo2118.cn

case "$1" in
来源：https://ig.zhonguo8118.cn

start) echo "启动" ;;
来源：https://tn.zhonguo5118.cn

stop)  echo "停止" ;;
来源：https://xp.zhonguo7118.cn

*)     echo "未知命令" ;;
来源：https://lq.zhonguo3118.cn

esac
来源：https://ng.zhonguo3118.cn

[R12] for 遍历文件
来源：https://vf.zhonguo6118.cn

for f in *.txt; do echo "$f"; done
来源：https://uu.zhonguo2118.cn

[R13] for 计数循环
来源：https://px.zhonguo8118.cn

for i in {1..10}; do echo "$i"; done
来源：https://yn.zhonguo7118.cn

[R14] C 风格 for
来源：https://ur.zhonguo7118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://fr.zhonguo7118.cn

[R15] while 逐行读文件
来源：https://wd.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://da.zhonguo8118.cn

[R16] until 等待条件
来源：https://hk.zhonguo5118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://qn.zhonguo1118.cn

[R17] 数组定义与取值
来源：https://rd.zhonguo6118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://bf.zhonguo6118.cn

[R18] 遍历数组
来源：https://yk.zhonguo6118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://wk.zhonguo2118.cn

[R19] 数组长度
来源：https://ab.zhonguo4118.cn

echo "${#arr[@]}"
来源：https://zb.zhonguo7118.cn

[R20] 关联数组（字典）
来源：https://re.zhonguo6118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://fj.zhonguo5118.cn

[R21] 字符串长度
来源：https://xl.zhonguo2118.cn

echo "${#s}"
来源：https://mb.zhonguo1118.cn

[R22] 截取子串
来源：https://qe.zhonguo5118.cn

echo "${s:0:5}"
来源：https://kl.zhonguo8118.cn

[R23] 字符串替换
来源：https://dy.zhonguo2118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://kz.zhonguo8118.cn

[R24] 大小写转换
来源：https://ed.zhonguo3118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://dq.zhonguo6118.cn

[R25] 去后缀 / 去前缀
来源：https://mn.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://ix.zhonguo4118.cn

[R26] 命令替换
来源：https://wc.zhonguo7118.cn

now=$(date +%F); echo "$now"
来源：https://lu.zhonguo4118.cn

[R27] 算术展开
来源：https://cn.zhonguo2118.cn

echo $((1 + 2 * 3))
来源：https://ms.zhonguo6118.cn

[R28] 浮点运算
来源：https://ow.zhonguo8118.cn

echo "scale=2; 10/3" | bc
来源：https://ay.zhonguo3118.cn

[R29] 定义函数
来源：https://so.zhonguo6118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://ee.zhonguo6118.cn

[R30] 函数返回状态码
来源：https://gy.zhonguo8118.cn

f() { return 0; }; f || echo "失败了"
来源：https://tf.zhonguo6118.cn

[R31] 局部变量
来源：https://vl.zhonguo6118.cn

f() { local x=1; echo "$x"; }
来源：https://sx.zhonguo4118.cn

[R32] 参数个数校验
来源：https://dd.zhonguo2118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://gw.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://ao.zhonguo2118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://tw.zhonguo4118.cn

[R34] 退出时清理
来源：https://tj.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://lu.zhonguo1118.cn

[R35] 后台执行并等待
来源：https://id.zhonguo2118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://du.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://tq.zhonguo5118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://ub.zhonguo7118.cn

[R37] 把输出赋给变量
来源：https://nv.zhonguo6118.cn

files=$(ls -1)
来源：https://cu.zhonguo8118.cn

[R38] 管道串联
来源：https://yu.zhonguo7118.cn

cat a.txt | grep -i error | wc -l
来源：https://sv.zhonguo5118.cn

[R39] 重定向标准输出与错误
来源：https://mo.zhonguo1118.cn

cmd > out.log 2>&1
来源：https://xp.zhonguo8118.cn

[R40] 追加写日志
来源：https://gm.zhonguo6118.cn

echo "log" >> out.log
来源：https://ts.zhonguo3118.cn

[R41] 丢弃输出
来源：https://nh.zhonguo8118.cn

cmd >/dev/null 2>&1
来源：https://wa.zhonguo2118.cn

[R42] 输入重定向
来源：https://ue.zhonguo4118.cn

wc -l < a.txt
来源：https://aj.zhonguo4118.cn

[R43] 按名字查找文件
来源：https://om.zhonguo1118.cn

find . -name "*.log" -type f
来源：https://sz.zhonguo2118.cn

[R44] 按修改时间查找
来源：https://ie.zhonguo3118.cn

find . -mtime -7 -type f
来源：https://wn.zhonguo5118.cn

[R45] 批量删除
来源：https://dd.zhonguo7118.cn

find . -name "*.tmp" -delete
来源：https://uh.zhonguo7118.cn

[R46] 递归替换文件内容
来源：https://lu.zhonguo3118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://vv.zhonguo4118.cn

[R47] sed 单行替换
来源：https://fh.zhonguo6118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://lp.zhonguo6118.cn

[R48] awk 取指定列
来源：https://nc.zhonguo1118.cn

awk '{print $1, $3}' a.txt
来源：https://ss.zhonguo7118.cn

[R49] awk 带条件
来源：https://mt.zhonguo4118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://gi.zhonguo5118.cn

[R50] awk 求和
来源：https://ka.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://wd.zhonguo4118.cn

[R51] 排序去重取前几
来源：https://vu.zhonguo6118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://qh.zhonguo2118.cn

[R52] 统计行数
来源：https://uy.zhonguo3118.cn

wc -l a.txt
来源：https://pj.zhonguo3118.cn

[R53] 查看文件头与实时尾
来源：https://qd.zhonguo1118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://ni.zhonguo4118.cn

[R54] 比较两个文件
来源：https://ks.zhonguo5118.cn

diff a.txt b.txt
来源：https://xa.zhonguo4118.cn

[R55] 压缩与解压
来源：https://uc.zhonguo2118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://is.zhonguo3118.cn

[R56] 远程拷贝
来源：https://mt.zhonguo2118.cn

scp file user@host:/path/
来源：https://bj.zhonguo1118.cn

[R57] 远程执行命令
来源：https://ho.zhonguo8118.cn

ssh user@host 'uptime'
来源：https://tq.zhonguo5118.cn

[R58] 下载文件
来源：https://qb.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://kx.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://so.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://kv.zhonguo4118.cn

[R60] 只看 HTTP 状态码
来源：https://mt.zhonguo2118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://yw.zhonguo7118.cn

[R61] 磁盘占用
来源：https://ae.zhonguo5118.cn

df -h;  du -sh *
来源：https://gd.zhonguo5118.cn

[R62] 找最占空间的文件
来源：https://fg.zhonguo8118.cn

du -ah . | sort -rh | head -10
来源：https://xt.zhonguo8118.cn

[R63] 内存与进程
来源：https://md.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://zn.zhonguo2118.cn

[R64] 结束进程
来源：https://cz.zhonguo1118.cn

kill -9 $(pgrep -f app.py)
来源：https://vc.zhonguo6118.cn

[R65] 查看端口占用
来源：https://tl.zhonguo7118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://tf.zhonguo1118.cn

[R66] 定时任务
来源：https://ib.zhonguo5118.cn

crontab -e;  crontab -l
来源：https://hz.zhonguo4118.cn

[R67] 生成随机十六进制串
来源：https://ut.zhonguo3118.cn

openssl rand -hex 16
来源：https://gw.zhonguo5118.cn

[R68] 计算文件校验值
来源：https://yc.zhonguo5118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://cb.zhonguo3118.cn

[R69] 生成随机密码
来源：https://xa.zhonguo4118.cn

head -c 16 /dev/urandom | base64
来源：https://oj.zhonguo5118.cn

[R70] 时间戳与互转
来源：https://jb.zhonguo7118.cn

date +%s;  date -d @1700000000
来源：https://as.zhonguo4118.cn

[R71] 日期格式化
来源：https://zy.zhonguo5118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://qb.zhonguo7118.cn

[R72] 等待端口就绪
来源：https://ag.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://kz.zhonguo6118.cn

[R73] 分割大日志
来源：https://re.zhonguo6118.cn

split -l 1000 big.log part_
来源：https://az.zhonguo3118.cn

[R74] 批量重命名
来源：https://gu.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://dm.zhonguo5118.cn

[R75] 导出环境变量
来源：https://hx.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://xb.zhonguo3118.cn

[R76] 使用临时文件
来源：https://cd.zhonguo2118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://af.zhonguo5118.cn

[R77] 读取用户输入
来源：https://uf.zhonguo2118.cn

read -rp "请输入: " ans
来源：https://vy.zhonguo5118.cn

[R78] 交互式菜单
来源：https://xp.zhonguo5118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://lb.zhonguo2118.cn

[R79] 解析命令行选项
来源：https://fo.zhonguo3118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://yb.zhonguo7118.cn

[R80] 查看脚本执行耗时
来源：https://lz.zhonguo3118.cn

time ./run.sh
来源：https://jn.zhonguo1118.cn

================================================================================
来源：https://fh.zhonguo7118.cn

S. C / C++ 专题
来源：https://sj.zhonguo4118.cn

================================================================================
来源：https://hm.zhonguo7118.cn

[S01] C：Hello World
来源：https://ku.zhonguo7118.cn

#include <stdio.h>
来源：https://vj.zhonguo8118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://hq.zhonguo1118.cn

[S02] C：变量与格式化输出
来源：https://jk.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://ht.zhonguo8118.cn

[S03] C：读入整数
来源：https://od.zhonguo5118.cn

int x; scanf("%d", &x);
来源：https://qt.zhonguo7118.cn

[S04] C：字符串复制
来源：https://dw.zhonguo6118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://db.zhonguo5118.cn

[S05] C：字符串长度
来源：https://cz.zhonguo1118.cn

strlen(s)
来源：https://vk.zhonguo3118.cn

[S06] C：字符串比较
来源：https://wa.zhonguo7118.cn

strcmp(a, b) == 0
来源：https://dz.zhonguo4118.cn

[S07] C：数组遍历求和
来源：https://ke.zhonguo7118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://oe.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://gd.zhonguo4118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://rk.zhonguo1118.cn

[S09] C：结构体定义与初始化
来源：https://zd.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://di.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://oc.zhonguo1118.cn

int *p = &a;  *p = 5;
来源：https://sy.zhonguo6118.cn

[S11] C：逐行读文件
来源：https://hv.zhonguo4118.cn

FILE *f = fopen("a.txt", "r");
来源：https://oo.zhonguo1118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://sw.zhonguo2118.cn

fclose(f);
来源：https://ek.zhonguo3118.cn

[S12] C：写文件
来源：https://od.zhonguo7118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://km.zhonguo1118.cn

[S13] C：宏定义
来源：https://wf.zhonguo3118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://uj.zhonguo4118.cn

[S14] C：枚举
来源：https://as.zhonguo7118.cn

enum Color { RED, GREEN, BLUE };
来源：https://yt.zhonguo5118.cn

[S15] C：类型转换
来源：https://zg.zhonguo8118.cn

(double) a / b
来源：https://ye.zhonguo5118.cn

[S16] C：位操作置位
来源：https://zi.zhonguo1118.cn

x |= (1 << 3);
来源：https://nr.zhonguo1118.cn

[S17] C：安全拼接字符串
来源：https://kb.zhonguo8118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://xz.zhonguo4118.cn

[S18] C：命令行参数
来源：https://sd.zhonguo4118.cn

int main(int argc, char **argv)
来源：https://do.zhonguo3118.cn

[S19] C：快速排序
来源：https://gd.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://cn.zhonguo2118.cn

[S20] C：二分查找
来源：https://rz.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://qu.zhonguo2118.cn

[S21] C：字符类别判断
来源：https://sv.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://bv.zhonguo4118.cn

[S22] C：字符串转数字
来源：https://sp.zhonguo6118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://vw.zhonguo6118.cn

[S23] C：随机数
来源：https://qf.zhonguo5118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://dv.zhonguo6118.cn

[S24] C：获取本地时间
来源：https://xv.zhonguo4118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://pe.zhonguo3118.cn

[S25] C：内存拷贝
来源：https://fz.zhonguo1118.cn

memcpy(dst, src, n);
来源：https://vn.zhonguo5118.cn

[S26] C：内存清零
来源：https://cw.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://oz.zhonguo7118.cn

[S27] C：定义常量
来源：https://hn.zhonguo1118.cn

const double PI = 3.14159;
来源：https://ig.zhonguo4118.cn

[S28] C：静态变量
来源：https://qi.zhonguo5118.cn

static int counter = 0;
来源：https://gn.zhonguo5118.cn

[S29] C：变参函数
来源：https://sj.zhonguo1118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://vh.zhonguo5118.cn

[S30] C：头文件保护
来源：https://rj.zhonguo5118.cn

#ifndef X_H
来源：https://fx.zhonguo8118.cn

#define X_H
来源：https://dr.zhonguo7118.cn

#endif
来源：https://wz.zhonguo7118.cn

[S31] C++：Hello World
来源：https://gg.zhonguo7118.cn

#include <iostream>
来源：https://tu.zhonguo6118.cn

int main() { std::cout << "Hello\n"; }
来源：https://ak.zhonguo5118.cn

[S32] C++：字符串
来源：https://kv.zhonguo5118.cn

std::string s = "hi";  s += "!";
来源：https://pl.zhonguo3118.cn

[S33] C++：vector 增删
来源：https://nl.zhonguo6118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://jn.zhonguo5118.cn

[S34] C++：遍历 vector
来源：https://up.zhonguo4118.cn

for (auto &x : v) { std::cout << x; }
来源：https://pp.zhonguo4118.cn

[S35] C++：map
来源：https://ez.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://hh.zhonguo3118.cn

[S36] C++：unordered_map
来源：https://rw.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://wj.zhonguo2118.cn


<!-- 参考信息 -->