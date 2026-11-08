代发 wailian999

ANALYZE TABLE users;
来源：https://sf.zhonguo2118.cn

[Q71] 查看建表语句
来源：https://qv.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://uo.zhonguo3118.cn

[Q72] 查看索引
来源：https://ma.zhonguo4118.cn

SHOW INDEX FROM users;
来源：https://bh.zhonguo2118.cn

[Q73] 查看表状态
来源：https://ic.zhonguo7118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://zy.zhonguo4118.cn

[Q74] 强制使用索引
来源：https://qn.zhonguo6118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://nb.zhonguo8118.cn

[Q75] 日期格式化
来源：https://fg.zhonguo4118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://tf.zhonguo1118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://hq.zhonguo2118.cn

[Q76] 按天统计
来源：https://kw.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://th.zhonguo8118.cn

[Q77] 时间加减
来源：https://zr.zhonguo4118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://oj.zhonguo1118.cn

[Q78] 当前时间
来源：https://oj.zhonguo4118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://hi.zhonguo5118.cn

[Q79] 字符串拼接
来源：https://cy.zhonguo4118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://ih.zhonguo4118.cn

[Q80] 字符串截取
来源：https://zk.zhonguo8118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://lc.zhonguo7118.cn

[Q81] 字符串替换
来源：https://gf.zhonguo2118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://gc.zhonguo1118.cn

[Q82] 字符长度与字节长度
来源：https://sm.zhonguo4118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://lq.zhonguo2118.cn

[Q83] 大小写转换
来源：https://oa.zhonguo2118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ib.zhonguo6118.cn

[Q84] 去除首尾空格
来源：https://zy.zhonguo6118.cn

SELECT TRIM(name) FROM users;
来源：https://mm.zhonguo4118.cn

[Q85] 数值取整
来源：https://zq.zhonguo2118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://xv.zhonguo5118.cn

[Q86] 读取 JSON 字段
来源：https://mj.zhonguo8118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://iv.zhonguo5118.cn

[Q87] JSON 字段做条件
来源：https://lj.zhonguo5118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://dp.zhonguo4118.cn

[Q88] 行转列（条件聚合）
来源：https://xh.zhonguo4118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://bf.zhonguo1118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://bf.zhonguo3118.cn

[Q89] 判断表是否存在
来源：https://vb.zhonguo8118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://rg.zhonguo6118.cn

[Q90] 生成序号列
来源：https://wv.zhonguo3118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://tc.zhonguo4118.cn

================================================================================
来源：https://xd.zhonguo4118.cn

R. Bash 专题
来源：https://vd.zhonguo2118.cn

================================================================================
来源：https://ub.zhonguo7118.cn

[R01] shebang 与严格模式
来源：https://bh.zhonguo4118.cn

#!/usr/bin/env bash
来源：https://dy.zhonguo2118.cn

set -euo pipefail
来源：https://ko.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://pu.zhonguo4118.cn

name="Tom"; echo "$name"
来源：https://yj.zhonguo7118.cn

[R03] 只读变量
来源：https://bc.zhonguo3118.cn

readonly PI=3.14
来源：https://na.zhonguo4118.cn

[R04] 位置参数
来源：https://dp.zhonguo8118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://pv.zhonguo1118.cn

[R05] 参数默认值
来源：https://zd.zhonguo5118.cn

name="${1:-default}"
来源：https://mv.zhonguo4118.cn

[R06] 判断命令是否存在
来源：https://oq.zhonguo1118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://wl.zhonguo8118.cn

[R07] if 判断文件
来源：https://ow.zhonguo7118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://lw.zhonguo2118.cn

[R08] 数值比较
来源：https://yy.zhonguo1118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://xn.zhonguo3118.cn

[R09] 字符串比较
来源：https://er.zhonguo4118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ng.zhonguo1118.cn

[R10] 正则匹配
来源：https://qo.zhonguo3118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://lz.zhonguo3118.cn

[R11] case 多分支
来源：https://sz.zhonguo5118.cn

case "$1" in
来源：https://tt.zhonguo5118.cn

start) echo "启动" ;;
来源：https://aj.zhonguo5118.cn

stop)  echo "停止" ;;
来源：https://bz.zhonguo5118.cn

*)     echo "未知命令" ;;
来源：https://ei.zhonguo8118.cn

esac
来源：https://gt.zhonguo2118.cn

[R12] for 遍历文件
来源：https://cl.zhonguo3118.cn

for f in *.txt; do echo "$f"; done
来源：https://ds.zhonguo2118.cn

[R13] for 计数循环
来源：https://po.zhonguo7118.cn

for i in {1..10}; do echo "$i"; done
来源：https://lt.zhonguo7118.cn

[R14] C 风格 for
来源：https://rh.zhonguo1118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://ic.zhonguo7118.cn

[R15] while 逐行读文件
来源：https://ex.zhonguo1118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://ah.zhonguo7118.cn

[R16] until 等待条件
来源：https://pe.zhonguo2118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://hz.zhonguo6118.cn

[R17] 数组定义与取值
来源：https://uo.zhonguo7118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://kg.zhonguo6118.cn

[R18] 遍历数组
来源：https://uj.zhonguo1118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://la.zhonguo3118.cn

[R19] 数组长度
来源：https://vf.zhonguo7118.cn

echo "${#arr[@]}"
来源：https://ur.zhonguo5118.cn

[R20] 关联数组（字典）
来源：https://qh.zhonguo3118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://fj.zhonguo3118.cn

[R21] 字符串长度
来源：https://mc.zhonguo7118.cn

echo "${#s}"
来源：https://ri.zhonguo4118.cn

[R22] 截取子串
来源：https://bv.zhonguo3118.cn

echo "${s:0:5}"
来源：https://rh.zhonguo5118.cn

[R23] 字符串替换
来源：https://ci.zhonguo1118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://st.zhonguo8118.cn

[R24] 大小写转换
来源：https://nh.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://co.zhonguo7118.cn

[R25] 去后缀 / 去前缀
来源：https://jb.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://bq.zhonguo5118.cn

[R26] 命令替换
来源：https://vu.zhonguo4118.cn

now=$(date +%F); echo "$now"
来源：https://ff.zhonguo3118.cn

[R27] 算术展开
来源：https://kz.zhonguo3118.cn

echo $((1 + 2 * 3))
来源：https://mh.zhonguo6118.cn

[R28] 浮点运算
来源：https://ye.zhonguo8118.cn

echo "scale=2; 10/3" | bc
来源：https://vb.zhonguo5118.cn

[R29] 定义函数
来源：https://ms.zhonguo2118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://vp.zhonguo6118.cn

[R30] 函数返回状态码
来源：https://xa.zhonguo8118.cn

f() { return 0; }; f || echo "失败了"
来源：https://vr.zhonguo3118.cn

[R31] 局部变量
来源：https://rv.zhonguo3118.cn

f() { local x=1; echo "$x"; }
来源：https://hd.zhonguo8118.cn

[R32] 参数个数校验
来源：https://ll.zhonguo4118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://hj.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://kf.zhonguo1118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://le.zhonguo2118.cn

[R34] 退出时清理
来源：https://sc.zhonguo5118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://pv.zhonguo8118.cn

[R35] 后台执行并等待
来源：https://za.zhonguo3118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://du.zhonguo5118.cn

[R36] 并发执行多个任务
来源：https://yc.zhonguo8118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://mg.zhonguo6118.cn

[R37] 把输出赋给变量
来源：https://pn.zhonguo6118.cn

files=$(ls -1)
来源：https://mn.zhonguo1118.cn

[R38] 管道串联
来源：https://yx.zhonguo5118.cn

cat a.txt | grep -i error | wc -l
来源：https://yl.zhonguo5118.cn

[R39] 重定向标准输出与错误
来源：https://wb.zhonguo7118.cn

cmd > out.log 2>&1
来源：https://pn.zhonguo8118.cn

[R40] 追加写日志
来源：https://oo.zhonguo7118.cn

echo "log" >> out.log
来源：https://zu.zhonguo1118.cn

[R41] 丢弃输出
来源：https://ma.zhonguo5118.cn

cmd >/dev/null 2>&1
来源：https://zf.zhonguo6118.cn

[R42] 输入重定向
来源：https://xl.zhonguo8118.cn

wc -l < a.txt
来源：https://pt.zhonguo6118.cn

[R43] 按名字查找文件
来源：https://iy.zhonguo1118.cn

find . -name "*.log" -type f
来源：https://et.zhonguo3118.cn

[R44] 按修改时间查找
来源：https://ee.zhonguo6118.cn

find . -mtime -7 -type f
来源：https://qt.zhonguo5118.cn

[R45] 批量删除
来源：https://cx.zhonguo3118.cn

find . -name "*.tmp" -delete
来源：https://sg.zhonguo1118.cn

[R46] 递归替换文件内容
来源：https://eg.zhonguo4118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://zc.zhonguo8118.cn

[R47] sed 单行替换
来源：https://hl.zhonguo6118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://rc.zhonguo8118.cn

[R48] awk 取指定列
来源：https://ek.zhonguo7118.cn

awk '{print $1, $3}' a.txt
来源：https://oh.zhonguo7118.cn

[R49] awk 带条件
来源：https://od.zhonguo3118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ja.zhonguo2118.cn

[R50] awk 求和
来源：https://lw.zhonguo2118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://xg.zhonguo5118.cn

[R51] 排序去重取前几
来源：https://yu.zhonguo7118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://hn.zhonguo1118.cn

[R52] 统计行数
来源：https://yn.zhonguo5118.cn

wc -l a.txt
来源：https://un.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://ga.zhonguo7118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://bw.zhonguo4118.cn

[R54] 比较两个文件
来源：https://xq.zhonguo6118.cn

diff a.txt b.txt
来源：https://qf.zhonguo6118.cn

[R55] 压缩与解压
来源：https://hw.zhonguo6118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ya.zhonguo8118.cn

[R56] 远程拷贝
来源：https://bl.zhonguo5118.cn

scp file user@host:/path/
来源：https://fz.zhonguo6118.cn

[R57] 远程执行命令
来源：https://qj.zhonguo1118.cn

ssh user@host 'uptime'
来源：https://tg.zhonguo3118.cn

[R58] 下载文件
来源：https://id.zhonguo2118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://jz.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://qi.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://dg.zhonguo3118.cn

[R60] 只看 HTTP 状态码
来源：https://to.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://jm.zhonguo6118.cn

[R61] 磁盘占用
来源：https://pf.zhonguo6118.cn

df -h;  du -sh *
来源：https://bx.zhonguo4118.cn

[R62] 找最占空间的文件
来源：https://qe.zhonguo1118.cn

du -ah . | sort -rh | head -10
来源：https://ic.zhonguo5118.cn

[R63] 内存与进程
来源：https://rq.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://ma.zhonguo1118.cn

[R64] 结束进程
来源：https://sp.zhonguo1118.cn

kill -9 $(pgrep -f app.py)
来源：https://kr.zhonguo3118.cn

[R65] 查看端口占用
来源：https://pg.zhonguo5118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://fe.zhonguo2118.cn

[R66] 定时任务
来源：https://uo.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://fq.zhonguo1118.cn

[R67] 生成随机十六进制串
来源：https://sw.zhonguo5118.cn

openssl rand -hex 16
来源：https://kb.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://cl.zhonguo1118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://xf.zhonguo6118.cn

[R69] 生成随机密码
来源：https://bd.zhonguo5118.cn

head -c 16 /dev/urandom | base64
来源：https://ew.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://hb.zhonguo1118.cn

date +%s;  date -d @1700000000
来源：https://rg.zhonguo7118.cn

[R71] 日期格式化
来源：https://oe.zhonguo1118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://vt.zhonguo1118.cn

[R72] 等待端口就绪
来源：https://xh.zhonguo1118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://fw.zhonguo8118.cn

[R73] 分割大日志
来源：https://bz.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://qr.zhonguo2118.cn

[R74] 批量重命名
来源：https://oq.zhonguo8118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://tf.zhonguo3118.cn

[R75] 导出环境变量
来源：https://al.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://gi.zhonguo7118.cn

[R76] 使用临时文件
来源：https://tg.zhonguo3118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://uq.zhonguo6118.cn

[R77] 读取用户输入
来源：https://pc.zhonguo7118.cn

read -rp "请输入: " ans
来源：https://us.zhonguo5118.cn

[R78] 交互式菜单
来源：https://bc.zhonguo3118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://le.zhonguo6118.cn

[R79] 解析命令行选项
来源：https://jf.zhonguo8118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://hz.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://oe.zhonguo1118.cn

time ./run.sh
来源：https://fe.zhonguo6118.cn

================================================================================
来源：https://bj.zhonguo6118.cn

S. C / C++ 专题
来源：https://qt.zhonguo2118.cn

================================================================================
来源：https://lo.zhonguo3118.cn

[S01] C：Hello World
来源：https://qj.zhonguo6118.cn

#include <stdio.h>
来源：https://gy.zhonguo3118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://mt.zhonguo5118.cn

[S02] C：变量与格式化输出
来源：https://im.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://wz.zhonguo8118.cn

[S03] C：读入整数
来源：https://mu.zhonguo7118.cn

int x; scanf("%d", &x);
来源：https://nr.zhonguo8118.cn

[S04] C：字符串复制
来源：https://nk.zhonguo7118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://xr.zhonguo2118.cn

[S05] C：字符串长度
来源：https://qu.zhonguo7118.cn

strlen(s)
来源：https://lu.zhonguo5118.cn

[S06] C：字符串比较
来源：https://xv.zhonguo4118.cn

strcmp(a, b) == 0
来源：https://yl.zhonguo1118.cn

[S07] C：数组遍历求和
来源：https://oe.zhonguo8118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://xr.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://vr.zhonguo3118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://qr.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://na.zhonguo7118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://hh.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://qg.zhonguo2118.cn

int *p = &a;  *p = 5;
来源：https://xl.zhonguo1118.cn

[S11] C：逐行读文件
来源：https://ul.zhonguo2118.cn

FILE *f = fopen("a.txt", "r");
来源：https://vk.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://jj.zhonguo7118.cn

fclose(f);
来源：https://gh.zhonguo1118.cn

[S12] C：写文件
来源：https://xz.zhonguo5118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://vh.zhonguo4118.cn

[S13] C：宏定义
来源：https://hg.zhonguo7118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://rd.zhonguo6118.cn

[S14] C：枚举
来源：https://jq.zhonguo6118.cn

enum Color { RED, GREEN, BLUE };
来源：https://mw.zhonguo6118.cn

[S15] C：类型转换
来源：https://ey.zhonguo2118.cn

(double) a / b
来源：https://no.zhonguo7118.cn

[S16] C：位操作置位
来源：https://mp.zhonguo5118.cn

x |= (1 << 3);
来源：https://vf.zhonguo5118.cn

[S17] C：安全拼接字符串
来源：https://wt.zhonguo4118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://en.zhonguo5118.cn

[S18] C：命令行参数
来源：https://pl.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://rb.zhonguo5118.cn

[S19] C：快速排序
来源：https://sx.zhonguo1118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://pu.zhonguo3118.cn

[S20] C：二分查找
来源：https://iy.zhonguo3118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://wd.zhonguo3118.cn

[S21] C：字符类别判断
来源：https://ae.zhonguo2118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://yo.zhonguo3118.cn

[S22] C：字符串转数字
来源：https://pe.zhonguo3118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://pv.zhonguo1118.cn

[S23] C：随机数
来源：https://mh.zhonguo2118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ev.zhonguo6118.cn

[S24] C：获取本地时间
来源：https://up.zhonguo5118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ul.zhonguo1118.cn

[S25] C：内存拷贝
来源：https://zs.zhonguo5118.cn

memcpy(dst, src, n);
来源：https://cl.zhonguo7118.cn

[S26] C：内存清零
来源：https://qr.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://lk.zhonguo4118.cn

[S27] C：定义常量
来源：https://cn.zhonguo6118.cn

const double PI = 3.14159;
来源：https://mp.zhonguo1118.cn

[S28] C：静态变量
来源：https://ug.zhonguo1118.cn

static int counter = 0;
来源：https://dn.zhonguo6118.cn

[S29] C：变参函数
来源：https://tu.zhonguo4118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://mh.zhonguo3118.cn

[S30] C：头文件保护
来源：https://zu.zhonguo4118.cn

#ifndef X_H
来源：https://ju.zhonguo3118.cn

#define X_H
来源：https://xh.zhonguo8118.cn

#endif
来源：https://bg.zhonguo3118.cn

[S31] C++：Hello World
来源：https://kj.zhonguo1118.cn

#include <iostream>
来源：https://og.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://pd.zhonguo7118.cn

[S32] C++：字符串
来源：https://jp.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://kt.zhonguo7118.cn

[S33] C++：vector 增删
来源：https://dj.zhonguo4118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://da.zhonguo8118.cn

[S34] C++：遍历 vector
来源：https://km.zhonguo2118.cn

for (auto &x : v) { std::cout << x; }
来源：https://cm.zhonguo2118.cn

[S35] C++：map
来源：https://zq.zhonguo3118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://bc.zhonguo6118.cn

[S36] C++：unordered_map
来源：https://ie.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://vs.zhonguo4118.cn

[S37] C++：set
来源：https://qi.zhonguo7118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://yl.zhonguo4118.cn

[S38] C++：排序
来源：https://az.zhonguo8118.cn

std::sort(v.begin(), v.end());
来源：https://ih.zhonguo6118.cn

[S39] C++：自定义比较器排序
来源：https://lg.zhonguo3118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://ja.zhonguo3118.cn

[S40] C++：查找元素
来源：https://zb.zhonguo3118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://lb.zhonguo3118.cn


<!-- 参考信息 -->