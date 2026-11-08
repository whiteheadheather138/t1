代发 wailian999

[Q76] 按天统计
来源：https://at.zhonguo3118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://lk.zhonguo7118.cn

[Q77] 时间加减
来源：https://av.zhonguo5118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://di.zhonguo3118.cn

[Q78] 当前时间
来源：https://fk.zhonguo1118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://oc.zhonguo4118.cn

[Q79] 字符串拼接
来源：https://ef.zhonguo2118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://dl.zhonguo1118.cn

[Q80] 字符串截取
来源：https://xh.zhonguo8118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://qb.zhonguo2118.cn

[Q81] 字符串替换
来源：https://ja.zhonguo1118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://zt.zhonguo2118.cn

[Q82] 字符长度与字节长度
来源：https://xa.zhonguo8118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://hb.zhonguo2118.cn

[Q83] 大小写转换
来源：https://mc.zhonguo3118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://bc.zhonguo2118.cn

[Q84] 去除首尾空格
来源：https://an.zhonguo6118.cn

SELECT TRIM(name) FROM users;
来源：https://li.zhonguo4118.cn

[Q85] 数值取整
来源：https://hw.zhonguo3118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://ru.zhonguo6118.cn

[Q86] 读取 JSON 字段
来源：https://uk.zhonguo4118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://je.zhonguo2118.cn

[Q87] JSON 字段做条件
来源：https://er.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://dt.zhonguo8118.cn

[Q88] 行转列（条件聚合）
来源：https://rz.zhonguo7118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://um.zhonguo7118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://fs.zhonguo1118.cn

[Q89] 判断表是否存在
来源：https://jb.zhonguo1118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://ia.zhonguo5118.cn

[Q90] 生成序号列
来源：https://zo.zhonguo8118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://qi.zhonguo2118.cn

================================================================================
来源：https://qw.zhonguo4118.cn

R. Bash 专题
来源：https://ra.zhonguo7118.cn

================================================================================
来源：https://ze.zhonguo2118.cn

[R01] shebang 与严格模式
来源：https://td.zhonguo4118.cn

#!/usr/bin/env bash
来源：https://cp.zhonguo4118.cn

set -euo pipefail
来源：https://lp.zhonguo8118.cn

[R02] 变量赋值与使用
来源：https://sb.zhonguo4118.cn

name="Tom"; echo "$name"
来源：https://tm.zhonguo3118.cn

[R03] 只读变量
来源：https://bz.zhonguo7118.cn

readonly PI=3.14
来源：https://mu.zhonguo5118.cn

[R04] 位置参数
来源：https://qq.zhonguo7118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://my.zhonguo6118.cn

[R05] 参数默认值
来源：https://qg.zhonguo4118.cn

name="${1:-default}"
来源：https://xw.zhonguo8118.cn

[R06] 判断命令是否存在
来源：https://ps.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://uw.zhonguo6118.cn

[R07] if 判断文件
来源：https://ud.zhonguo4118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://lj.zhonguo8118.cn

[R08] 数值比较
来源：https://bm.zhonguo7118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://hd.zhonguo1118.cn

[R09] 字符串比较
来源：https://yw.zhonguo4118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ck.zhonguo8118.cn

[R10] 正则匹配
来源：https://tb.zhonguo3118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://yg.zhonguo7118.cn

[R11] case 多分支
来源：https://vz.zhonguo1118.cn

case "$1" in
来源：https://ip.zhonguo2118.cn

start) echo "启动" ;;
来源：https://zp.zhonguo5118.cn

stop)  echo "停止" ;;
来源：https://zx.zhonguo2118.cn

*)     echo "未知命令" ;;
来源：https://vb.zhonguo6118.cn

esac
来源：https://ke.zhonguo8118.cn

[R12] for 遍历文件
来源：https://ty.zhonguo7118.cn

for f in *.txt; do echo "$f"; done
来源：https://mx.zhonguo6118.cn

[R13] for 计数循环
来源：https://rg.zhonguo2118.cn

for i in {1..10}; do echo "$i"; done
来源：https://wg.zhonguo6118.cn

[R14] C 风格 for
来源：https://yb.zhonguo7118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://hh.zhonguo4118.cn

[R15] while 逐行读文件
来源：https://ef.zhonguo8118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://qh.zhonguo8118.cn

[R16] until 等待条件
来源：https://nd.zhonguo6118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://po.zhonguo6118.cn

[R17] 数组定义与取值
来源：https://sh.zhonguo7118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://nj.zhonguo8118.cn

[R18] 遍历数组
来源：https://vh.zhonguo5118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://by.zhonguo6118.cn

[R19] 数组长度
来源：https://cg.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://wd.zhonguo1118.cn

[R20] 关联数组（字典）
来源：https://kh.zhonguo8118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://po.zhonguo5118.cn

[R21] 字符串长度
来源：https://sm.zhonguo3118.cn

echo "${#s}"
来源：https://sr.zhonguo7118.cn

[R22] 截取子串
来源：https://uv.zhonguo7118.cn

echo "${s:0:5}"
来源：https://nm.zhonguo1118.cn

[R23] 字符串替换
来源：https://fq.zhonguo6118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://gm.zhonguo6118.cn

[R24] 大小写转换
来源：https://ru.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ee.zhonguo5118.cn

[R25] 去后缀 / 去前缀
来源：https://gj.zhonguo3118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://gw.zhonguo8118.cn

[R26] 命令替换
来源：https://qy.zhonguo6118.cn

now=$(date +%F); echo "$now"
来源：https://ii.zhonguo6118.cn

[R27] 算术展开
来源：https://ed.zhonguo3118.cn

echo $((1 + 2 * 3))
来源：https://cu.zhonguo4118.cn

[R28] 浮点运算
来源：https://ab.zhonguo5118.cn

echo "scale=2; 10/3" | bc
来源：https://zj.zhonguo7118.cn

[R29] 定义函数
来源：https://oj.zhonguo3118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://bp.zhonguo7118.cn

[R30] 函数返回状态码
来源：https://oy.zhonguo7118.cn

f() { return 0; }; f || echo "失败了"
来源：https://qs.zhonguo7118.cn

[R31] 局部变量
来源：https://rp.zhonguo8118.cn

f() { local x=1; echo "$x"; }
来源：https://fc.zhonguo5118.cn

[R32] 参数个数校验
来源：https://ra.zhonguo6118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://wl.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://uf.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://kp.zhonguo1118.cn

[R34] 退出时清理
来源：https://gs.zhonguo4118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://ud.zhonguo5118.cn

[R35] 后台执行并等待
来源：https://ej.zhonguo2118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://vb.zhonguo1118.cn

[R36] 并发执行多个任务
来源：https://ve.zhonguo6118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://gb.zhonguo4118.cn

[R37] 把输出赋给变量
来源：https://ny.zhonguo1118.cn

files=$(ls -1)
来源：https://ca.zhonguo6118.cn

[R38] 管道串联
来源：https://am.zhonguo2118.cn

cat a.txt | grep -i error | wc -l
来源：https://tw.zhonguo4118.cn

[R39] 重定向标准输出与错误
来源：https://jq.zhonguo3118.cn

cmd > out.log 2>&1
来源：https://zo.zhonguo5118.cn

[R40] 追加写日志
来源：https://pr.zhonguo2118.cn

echo "log" >> out.log
来源：https://qi.zhonguo8118.cn

[R41] 丢弃输出
来源：https://gf.zhonguo2118.cn

cmd >/dev/null 2>&1
来源：https://ba.zhonguo6118.cn

[R42] 输入重定向
来源：https://nm.zhonguo6118.cn

wc -l < a.txt
来源：https://vj.zhonguo8118.cn

[R43] 按名字查找文件
来源：https://vc.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://do.zhonguo8118.cn

[R44] 按修改时间查找
来源：https://jn.zhonguo6118.cn

find . -mtime -7 -type f
来源：https://cg.zhonguo6118.cn

[R45] 批量删除
来源：https://dq.zhonguo2118.cn

find . -name "*.tmp" -delete
来源：https://sm.zhonguo4118.cn

[R46] 递归替换文件内容
来源：https://bf.zhonguo5118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://wp.zhonguo7118.cn

[R47] sed 单行替换
来源：https://fu.zhonguo7118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://qu.zhonguo3118.cn

[R48] awk 取指定列
来源：https://ck.zhonguo2118.cn

awk '{print $1, $3}' a.txt
来源：https://ph.zhonguo5118.cn

[R49] awk 带条件
来源：https://qy.zhonguo4118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://fm.zhonguo3118.cn

[R50] awk 求和
来源：https://bf.zhonguo8118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://qq.zhonguo3118.cn

[R51] 排序去重取前几
来源：https://uj.zhonguo8118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://ik.zhonguo4118.cn

[R52] 统计行数
来源：https://jv.zhonguo6118.cn

wc -l a.txt
来源：https://wj.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://gp.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://np.zhonguo7118.cn

[R54] 比较两个文件
来源：https://lz.zhonguo6118.cn

diff a.txt b.txt
来源：https://wu.zhonguo5118.cn

[R55] 压缩与解压
来源：https://hh.zhonguo7118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ap.zhonguo6118.cn

[R56] 远程拷贝
来源：https://ke.zhonguo4118.cn

scp file user@host:/path/
来源：https://rp.zhonguo2118.cn

[R57] 远程执行命令
来源：https://ll.zhonguo6118.cn

ssh user@host 'uptime'
来源：https://qe.zhonguo7118.cn

[R58] 下载文件
来源：https://pq.zhonguo8118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://gs.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://fq.zhonguo7118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://ed.zhonguo8118.cn

[R60] 只看 HTTP 状态码
来源：https://bu.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://pm.zhonguo4118.cn

[R61] 磁盘占用
来源：https://hi.zhonguo4118.cn

df -h;  du -sh *
来源：https://rn.zhonguo3118.cn

[R62] 找最占空间的文件
来源：https://ay.zhonguo3118.cn

du -ah . | sort -rh | head -10
来源：https://up.zhonguo6118.cn

[R63] 内存与进程
来源：https://nq.zhonguo2118.cn

free -h;  ps aux | grep nginx
来源：https://af.zhonguo5118.cn

[R64] 结束进程
来源：https://om.zhonguo5118.cn

kill -9 $(pgrep -f app.py)
来源：https://ie.zhonguo5118.cn

[R65] 查看端口占用
来源：https://br.zhonguo3118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://rg.zhonguo2118.cn

[R66] 定时任务
来源：https://gn.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://uw.zhonguo1118.cn

[R67] 生成随机十六进制串
来源：https://ox.zhonguo7118.cn

openssl rand -hex 16
来源：https://dw.zhonguo5118.cn

[R68] 计算文件校验值
来源：https://hu.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://gq.zhonguo2118.cn

[R69] 生成随机密码
来源：https://tn.zhonguo2118.cn

head -c 16 /dev/urandom | base64
来源：https://tf.zhonguo2118.cn

[R70] 时间戳与互转
来源：https://bv.zhonguo7118.cn

date +%s;  date -d @1700000000
来源：https://cn.zhonguo7118.cn

[R71] 日期格式化
来源：https://qs.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://jr.zhonguo7118.cn

[R72] 等待端口就绪
来源：https://tl.zhonguo8118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://nz.zhonguo5118.cn

[R73] 分割大日志
来源：https://vh.zhonguo5118.cn

split -l 1000 big.log part_
来源：https://og.zhonguo7118.cn

[R74] 批量重命名
来源：https://mt.zhonguo5118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://nm.zhonguo2118.cn

[R75] 导出环境变量
来源：https://ji.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://or.zhonguo8118.cn

[R76] 使用临时文件
来源：https://ov.zhonguo1118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://cc.zhonguo8118.cn

[R77] 读取用户输入
来源：https://jx.zhonguo2118.cn

read -rp "请输入: " ans
来源：https://ln.zhonguo4118.cn

[R78] 交互式菜单
来源：https://ut.zhonguo4118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://ef.zhonguo8118.cn

[R79] 解析命令行选项
来源：https://bz.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://uq.zhonguo7118.cn

[R80] 查看脚本执行耗时
来源：https://hv.zhonguo5118.cn

time ./run.sh
来源：https://tl.zhonguo4118.cn

================================================================================
来源：https://aw.zhonguo3118.cn

S. C / C++ 专题
来源：https://oc.zhonguo6118.cn

================================================================================
来源：https://kl.zhonguo5118.cn

[S01] C：Hello World
来源：https://ip.zhonguo6118.cn

#include <stdio.h>
来源：https://qd.zhonguo5118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://kl.zhonguo8118.cn

[S02] C：变量与格式化输出
来源：https://ll.zhonguo3118.cn

int a = 10; printf("%d\n", a);
来源：https://ca.zhonguo6118.cn

[S03] C：读入整数
来源：https://ey.zhonguo2118.cn

int x; scanf("%d", &x);
来源：https://xf.zhonguo2118.cn

[S04] C：字符串复制
来源：https://mh.zhonguo8118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://cd.zhonguo6118.cn

[S05] C：字符串长度
来源：https://sl.zhonguo2118.cn

strlen(s)
来源：https://oc.zhonguo6118.cn

[S06] C：字符串比较
来源：https://al.zhonguo6118.cn

strcmp(a, b) == 0
来源：https://gt.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://ap.zhonguo2118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://rc.zhonguo7118.cn

[S08] C：动态内存分配与释放
来源：https://dq.zhonguo1118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://nq.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://oy.zhonguo1118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://to.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://fy.zhonguo3118.cn

int *p = &a;  *p = 5;
来源：https://wj.zhonguo2118.cn

[S11] C：逐行读文件
来源：https://tc.zhonguo3118.cn

FILE *f = fopen("a.txt", "r");
来源：https://kj.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://fj.zhonguo4118.cn

fclose(f);
来源：https://hc.zhonguo2118.cn

[S12] C：写文件
来源：https://zn.zhonguo6118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://nz.zhonguo5118.cn

[S13] C：宏定义
来源：https://mp.zhonguo2118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://xt.zhonguo5118.cn

[S14] C：枚举
来源：https://wa.zhonguo3118.cn

enum Color { RED, GREEN, BLUE };
来源：https://vt.zhonguo5118.cn

[S15] C：类型转换
来源：https://jf.zhonguo1118.cn

(double) a / b
来源：https://ex.zhonguo5118.cn

[S16] C：位操作置位
来源：https://kf.zhonguo7118.cn

x |= (1 << 3);
来源：https://nv.zhonguo7118.cn

[S17] C：安全拼接字符串
来源：https://cp.zhonguo1118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ei.zhonguo7118.cn

[S18] C：命令行参数
来源：https://pz.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://wf.zhonguo7118.cn

[S19] C：快速排序
来源：https://fi.zhonguo8118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://tl.zhonguo3118.cn

[S20] C：二分查找
来源：https://gt.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://fz.zhonguo7118.cn

[S21] C：字符类别判断
来源：https://fp.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://al.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://ny.zhonguo2118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://aw.zhonguo1118.cn

[S23] C：随机数
来源：https://aw.zhonguo2118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ji.zhonguo2118.cn

[S24] C：获取本地时间
来源：https://vu.zhonguo3118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://fi.zhonguo5118.cn

[S25] C：内存拷贝
来源：https://xh.zhonguo3118.cn

memcpy(dst, src, n);
来源：https://js.zhonguo3118.cn

[S26] C：内存清零
来源：https://ib.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://qs.zhonguo7118.cn

[S27] C：定义常量
来源：https://ro.zhonguo3118.cn

const double PI = 3.14159;
来源：https://pp.zhonguo1118.cn

[S28] C：静态变量
来源：https://na.zhonguo5118.cn

static int counter = 0;
来源：https://ho.zhonguo7118.cn

[S29] C：变参函数
来源：https://xk.zhonguo7118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://uz.zhonguo3118.cn

[S30] C：头文件保护
来源：https://zn.zhonguo7118.cn

#ifndef X_H
来源：https://zq.zhonguo7118.cn

#define X_H
来源：https://ct.zhonguo5118.cn

#endif
来源：https://rg.zhonguo1118.cn

[S31] C++：Hello World
来源：https://wm.zhonguo8118.cn

#include <iostream>
来源：https://tu.zhonguo6118.cn

int main() { std::cout << "Hello\n"; }
来源：https://fz.zhonguo2118.cn

[S32] C++：字符串
来源：https://xc.zhonguo7118.cn

std::string s = "hi";  s += "!";
来源：https://rk.zhonguo7118.cn

[S33] C++：vector 增删
来源：https://bt.zhonguo4118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://wx.zhonguo4118.cn

[S34] C++：遍历 vector
来源：https://yv.zhonguo1118.cn

for (auto &x : v) { std::cout << x; }
来源：https://ys.zhonguo7118.cn

[S35] C++：map
来源：https://gx.zhonguo6118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://in.zhonguo6118.cn

[S36] C++：unordered_map
来源：https://nd.zhonguo5118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://dt.zhonguo8118.cn

[S37] C++：set
来源：https://sr.zhonguo4118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://ni.zhonguo6118.cn

[S38] C++：排序
来源：https://vb.zhonguo4118.cn

std::sort(v.begin(), v.end());
来源：https://ac.zhonguo3118.cn

[S39] C++：自定义比较器排序
来源：https://yl.zhonguo5118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://kt.zhonguo8118.cn

[S40] C++：查找元素
来源：https://ox.zhonguo8118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://gf.zhonguo6118.cn

[S41] C++：类与构造函数
来源：https://xi.zhonguo2118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://og.zhonguo3118.cn

[S42] C++：继承与虚函数
来源：https://fy.zhonguo1118.cn

class B : public Base { public: void f() override {} };
来源：https://ba.zhonguo4118.cn

[S43] C++：智能指针
来源：https://hc.zhonguo6118.cn

auto p = std::make_unique<int>(5);
来源：https://bn.zhonguo7118.cn

[S44] C++：引用传参
来源：https://iy.zhonguo8118.cn

void inc(int &x) { ++x; }
来源：https://eb.zhonguo8118.cn

[S45] C++：lambda
来源：https://ap.zhonguo8118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://zd.zhonguo1118.cn

[S46] C++：函数模板
来源：https://bk.zhonguo8118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://dt.zhonguo2118.cn


<!-- 参考信息 -->