代发 wailian999

[Q76] 按天统计
来源：https://gr.zhonguo4118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://me.zhonguo2118.cn

[Q77] 时间加减
来源：https://on.zhonguo6118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://mx.zhonguo5118.cn

[Q78] 当前时间
来源：https://xs.zhonguo3118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://uf.zhonguo8118.cn

[Q79] 字符串拼接
来源：https://zt.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://oi.zhonguo6118.cn

[Q80] 字符串截取
来源：https://xe.zhonguo8118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://cj.zhonguo2118.cn

[Q81] 字符串替换
来源：https://wg.zhonguo8118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://ct.zhonguo6118.cn

[Q82] 字符长度与字节长度
来源：https://xi.zhonguo5118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://pf.zhonguo5118.cn

[Q83] 大小写转换
来源：https://vu.zhonguo6118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://be.zhonguo5118.cn

[Q84] 去除首尾空格
来源：https://cm.zhonguo6118.cn

SELECT TRIM(name) FROM users;
来源：https://py.zhonguo6118.cn

[Q85] 数值取整
来源：https://df.zhonguo4118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://hy.zhonguo3118.cn

[Q86] 读取 JSON 字段
来源：https://je.zhonguo5118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://ud.zhonguo2118.cn

[Q87] JSON 字段做条件
来源：https://cu.zhonguo5118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://xw.zhonguo5118.cn

[Q88] 行转列（条件聚合）
来源：https://vp.zhonguo6118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://of.zhonguo3118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://nb.zhonguo6118.cn

[Q89] 判断表是否存在
来源：https://cw.zhonguo2118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://eh.zhonguo4118.cn

[Q90] 生成序号列
来源：https://ek.zhonguo2118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://kp.zhonguo7118.cn

================================================================================
来源：https://sl.zhonguo6118.cn

R. Bash 专题
来源：https://dk.zhonguo7118.cn

================================================================================
来源：https://ke.zhonguo5118.cn

[R01] shebang 与严格模式
来源：https://pn.zhonguo8118.cn

#!/usr/bin/env bash
来源：https://no.zhonguo1118.cn

set -euo pipefail
来源：https://tw.zhonguo5118.cn

[R02] 变量赋值与使用
来源：https://jx.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://fr.zhonguo3118.cn

[R03] 只读变量
来源：https://av.zhonguo6118.cn

readonly PI=3.14
来源：https://pb.zhonguo7118.cn

[R04] 位置参数
来源：https://yn.zhonguo2118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://cx.zhonguo3118.cn

[R05] 参数默认值
来源：https://ux.zhonguo2118.cn

name="${1:-default}"
来源：https://nc.zhonguo7118.cn

[R06] 判断命令是否存在
来源：https://kc.zhonguo2118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://gx.zhonguo4118.cn

[R07] if 判断文件
来源：https://db.zhonguo2118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://jr.zhonguo1118.cn

[R08] 数值比较
来源：https://zm.zhonguo2118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://fz.zhonguo7118.cn

[R09] 字符串比较
来源：https://dp.zhonguo4118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://ow.zhonguo8118.cn

[R10] 正则匹配
来源：https://op.zhonguo7118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ax.zhonguo5118.cn

[R11] case 多分支
来源：https://de.zhonguo2118.cn

case "$1" in
来源：https://is.zhonguo3118.cn

start) echo "启动" ;;
来源：https://pg.zhonguo8118.cn

stop)  echo "停止" ;;
来源：https://fd.zhonguo7118.cn

*)     echo "未知命令" ;;
来源：https://iu.zhonguo5118.cn

esac
来源：https://hz.zhonguo4118.cn

[R12] for 遍历文件
来源：https://dl.zhonguo3118.cn

for f in *.txt; do echo "$f"; done
来源：https://vg.zhonguo3118.cn

[R13] for 计数循环
来源：https://eo.zhonguo3118.cn

for i in {1..10}; do echo "$i"; done
来源：https://gu.zhonguo8118.cn

[R14] C 风格 for
来源：https://yx.zhonguo1118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://kn.zhonguo7118.cn

[R15] while 逐行读文件
来源：https://eg.zhonguo7118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://za.zhonguo2118.cn

[R16] until 等待条件
来源：https://ht.zhonguo7118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://nn.zhonguo7118.cn

[R17] 数组定义与取值
来源：https://bx.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://nt.zhonguo1118.cn

[R18] 遍历数组
来源：https://mq.zhonguo3118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://vy.zhonguo5118.cn

[R19] 数组长度
来源：https://zi.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://tw.zhonguo5118.cn

[R20] 关联数组（字典）
来源：https://ev.zhonguo7118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://dr.zhonguo5118.cn

[R21] 字符串长度
来源：https://il.zhonguo3118.cn

echo "${#s}"
来源：https://zt.zhonguo2118.cn

[R22] 截取子串
来源：https://jr.zhonguo1118.cn

echo "${s:0:5}"
来源：https://ih.zhonguo2118.cn

[R23] 字符串替换
来源：https://ma.zhonguo1118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://fz.zhonguo1118.cn

[R24] 大小写转换
来源：https://li.zhonguo4118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://ov.zhonguo5118.cn

[R25] 去后缀 / 去前缀
来源：https://ym.zhonguo1118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://yf.zhonguo7118.cn

[R26] 命令替换
来源：https://ru.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://kc.zhonguo5118.cn

[R27] 算术展开
来源：https://nj.zhonguo2118.cn

echo $((1 + 2 * 3))
来源：https://jx.zhonguo1118.cn

[R28] 浮点运算
来源：https://ug.zhonguo2118.cn

echo "scale=2; 10/3" | bc
来源：https://fv.zhonguo2118.cn

[R29] 定义函数
来源：https://cv.zhonguo1118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://xm.zhonguo1118.cn

[R30] 函数返回状态码
来源：https://cc.zhonguo3118.cn

f() { return 0; }; f || echo "失败了"
来源：https://uf.zhonguo7118.cn

[R31] 局部变量
来源：https://pc.zhonguo8118.cn

f() { local x=1; echo "$x"; }
来源：https://pr.zhonguo1118.cn

[R32] 参数个数校验
来源：https://jn.zhonguo5118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://kj.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://uo.zhonguo6118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://fo.zhonguo3118.cn

[R34] 退出时清理
来源：https://zo.zhonguo8118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://ea.zhonguo2118.cn

[R35] 后台执行并等待
来源：https://xd.zhonguo4118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://nb.zhonguo4118.cn

[R36] 并发执行多个任务
来源：https://is.zhonguo7118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://be.zhonguo1118.cn

[R37] 把输出赋给变量
来源：https://qu.zhonguo4118.cn

files=$(ls -1)
来源：https://lj.zhonguo8118.cn

[R38] 管道串联
来源：https://pm.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://kw.zhonguo8118.cn

[R39] 重定向标准输出与错误
来源：https://bt.zhonguo7118.cn

cmd > out.log 2>&1
来源：https://ng.zhonguo7118.cn

[R40] 追加写日志
来源：https://pr.zhonguo5118.cn

echo "log" >> out.log
来源：https://qe.zhonguo3118.cn

[R41] 丢弃输出
来源：https://yj.zhonguo7118.cn

cmd >/dev/null 2>&1
来源：https://zt.zhonguo6118.cn

[R42] 输入重定向
来源：https://sg.zhonguo4118.cn

wc -l < a.txt
来源：https://jj.zhonguo5118.cn

[R43] 按名字查找文件
来源：https://lt.zhonguo3118.cn

find . -name "*.log" -type f
来源：https://oq.zhonguo1118.cn

[R44] 按修改时间查找
来源：https://rz.zhonguo3118.cn

find . -mtime -7 -type f
来源：https://he.zhonguo2118.cn

[R45] 批量删除
来源：https://ki.zhonguo8118.cn

find . -name "*.tmp" -delete
来源：https://hk.zhonguo3118.cn

[R46] 递归替换文件内容
来源：https://dv.zhonguo2118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://py.zhonguo7118.cn

[R47] sed 单行替换
来源：https://tx.zhonguo4118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://qe.zhonguo8118.cn

[R48] awk 取指定列
来源：https://on.zhonguo5118.cn

awk '{print $1, $3}' a.txt
来源：https://bm.zhonguo6118.cn

[R49] awk 带条件
来源：https://ri.zhonguo4118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://gj.zhonguo5118.cn

[R50] awk 求和
来源：https://ig.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://ru.zhonguo2118.cn

[R51] 排序去重取前几
来源：https://na.zhonguo4118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://cy.zhonguo5118.cn

[R52] 统计行数
来源：https://uk.zhonguo2118.cn

wc -l a.txt
来源：https://xq.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://rx.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://si.zhonguo5118.cn

[R54] 比较两个文件
来源：https://zn.zhonguo2118.cn

diff a.txt b.txt
来源：https://ax.zhonguo4118.cn

[R55] 压缩与解压
来源：https://jb.zhonguo8118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://mu.zhonguo6118.cn

[R56] 远程拷贝
来源：https://pn.zhonguo4118.cn

scp file user@host:/path/
来源：https://ck.zhonguo2118.cn

[R57] 远程执行命令
来源：https://ef.zhonguo7118.cn

ssh user@host 'uptime'
来源：https://fy.zhonguo4118.cn

[R58] 下载文件
来源：https://bt.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://tq.zhonguo7118.cn

[R59] 发 POST JSON
来源：https://qf.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://sd.zhonguo5118.cn

[R60] 只看 HTTP 状态码
来源：https://kr.zhonguo7118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://bi.zhonguo4118.cn

[R61] 磁盘占用
来源：https://vw.zhonguo6118.cn

df -h;  du -sh *
来源：https://vc.zhonguo5118.cn

[R62] 找最占空间的文件
来源：https://ce.zhonguo4118.cn

du -ah . | sort -rh | head -10
来源：https://up.zhonguo8118.cn

[R63] 内存与进程
来源：https://wc.zhonguo1118.cn

free -h;  ps aux | grep nginx
来源：https://fj.zhonguo7118.cn

[R64] 结束进程
来源：https://kx.zhonguo1118.cn

kill -9 $(pgrep -f app.py)
来源：https://mk.zhonguo1118.cn

[R65] 查看端口占用
来源：https://ov.zhonguo1118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://rw.zhonguo4118.cn

[R66] 定时任务
来源：https://ot.zhonguo1118.cn

crontab -e;  crontab -l
来源：https://bs.zhonguo7118.cn

[R67] 生成随机十六进制串
来源：https://ns.zhonguo5118.cn

openssl rand -hex 16
来源：https://lt.zhonguo2118.cn

[R68] 计算文件校验值
来源：https://xi.zhonguo7118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://yq.zhonguo2118.cn

[R69] 生成随机密码
来源：https://tz.zhonguo2118.cn

head -c 16 /dev/urandom | base64
来源：https://im.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://np.zhonguo4118.cn

date +%s;  date -d @1700000000
来源：https://wm.zhonguo3118.cn

[R71] 日期格式化
来源：https://ts.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ge.zhonguo2118.cn

[R72] 等待端口就绪
来源：https://cy.zhonguo7118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://ge.zhonguo4118.cn

[R73] 分割大日志
来源：https://qn.zhonguo8118.cn

split -l 1000 big.log part_
来源：https://kt.zhonguo8118.cn

[R74] 批量重命名
来源：https://jo.zhonguo8118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://eg.zhonguo4118.cn

[R75] 导出环境变量
来源：https://sz.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://uc.zhonguo1118.cn

[R76] 使用临时文件
来源：https://zz.zhonguo4118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://ok.zhonguo5118.cn

[R77] 读取用户输入
来源：https://ny.zhonguo8118.cn

read -rp "请输入: " ans
来源：https://ae.zhonguo2118.cn

[R78] 交互式菜单
来源：https://vk.zhonguo2118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://rg.zhonguo6118.cn

[R79] 解析命令行选项
来源：https://ki.zhonguo7118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://rz.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://xr.zhonguo7118.cn

time ./run.sh
来源：https://lm.zhonguo8118.cn

================================================================================
来源：https://cr.zhonguo7118.cn

S. C / C++ 专题
来源：https://xi.zhonguo2118.cn

================================================================================
来源：https://kd.zhonguo5118.cn

[S01] C：Hello World
来源：https://ld.zhonguo7118.cn

#include <stdio.h>
来源：https://dy.zhonguo2118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://sa.zhonguo7118.cn

[S02] C：变量与格式化输出
来源：https://va.zhonguo7118.cn

int a = 10; printf("%d\n", a);
来源：https://pb.zhonguo1118.cn

[S03] C：读入整数
来源：https://qu.zhonguo7118.cn

int x; scanf("%d", &x);
来源：https://sk.zhonguo5118.cn

[S04] C：字符串复制
来源：https://fo.zhonguo4118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://ib.zhonguo7118.cn

[S05] C：字符串长度
来源：https://ef.zhonguo7118.cn

strlen(s)
来源：https://ip.zhonguo3118.cn

[S06] C：字符串比较
来源：https://lu.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://sf.zhonguo2118.cn

[S07] C：数组遍历求和
来源：https://sg.zhonguo6118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://ce.zhonguo4118.cn

[S08] C：动态内存分配与释放
来源：https://gv.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://qb.zhonguo7118.cn

[S09] C：结构体定义与初始化
来源：https://du.zhonguo1118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://mx.zhonguo5118.cn

[S10] C：指针与解引用
来源：https://zv.zhonguo1118.cn

int *p = &a;  *p = 5;
来源：https://br.zhonguo7118.cn

[S11] C：逐行读文件
来源：https://qb.zhonguo7118.cn

FILE *f = fopen("a.txt", "r");
来源：https://um.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ek.zhonguo4118.cn

fclose(f);
来源：https://kp.zhonguo1118.cn

[S12] C：写文件
来源：https://bm.zhonguo7118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://ke.zhonguo8118.cn

[S13] C：宏定义
来源：https://ai.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://fl.zhonguo7118.cn

[S14] C：枚举
来源：https://ah.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://dj.zhonguo6118.cn

[S15] C：类型转换
来源：https://aw.zhonguo2118.cn

(double) a / b
来源：https://jo.zhonguo4118.cn

[S16] C：位操作置位
来源：https://rm.zhonguo2118.cn

x |= (1 << 3);
来源：https://ph.zhonguo1118.cn

[S17] C：安全拼接字符串
来源：https://fk.zhonguo5118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ap.zhonguo6118.cn

[S18] C：命令行参数
来源：https://tp.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://mm.zhonguo8118.cn

[S19] C：快速排序
来源：https://fm.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://cs.zhonguo4118.cn

[S20] C：二分查找
来源：https://ti.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://ok.zhonguo7118.cn

[S21] C：字符类别判断
来源：https://ry.zhonguo4118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://ag.zhonguo7118.cn

[S22] C：字符串转数字
来源：https://aq.zhonguo8118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://pg.zhonguo5118.cn

[S23] C：随机数
来源：https://gf.zhonguo2118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://bo.zhonguo7118.cn

[S24] C：获取本地时间
来源：https://eq.zhonguo5118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://kn.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://fd.zhonguo8118.cn

memcpy(dst, src, n);
来源：https://kz.zhonguo4118.cn

[S26] C：内存清零
来源：https://lj.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://fw.zhonguo5118.cn

[S27] C：定义常量
来源：https://pp.zhonguo6118.cn

const double PI = 3.14159;
来源：https://hy.zhonguo1118.cn

[S28] C：静态变量
来源：https://by.zhonguo7118.cn

static int counter = 0;
来源：https://wb.zhonguo6118.cn

[S29] C：变参函数
来源：https://kb.zhonguo8118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://ha.zhonguo3118.cn

[S30] C：头文件保护
来源：https://zy.zhonguo6118.cn

#ifndef X_H
来源：https://gs.zhonguo4118.cn

#define X_H
来源：https://en.zhonguo1118.cn

#endif
来源：https://ep.zhonguo3118.cn

[S31] C++：Hello World
来源：https://bd.zhonguo3118.cn

#include <iostream>
来源：https://sm.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://xk.zhonguo4118.cn

[S32] C++：字符串
来源：https://sv.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://xd.zhonguo5118.cn

[S33] C++：vector 增删
来源：https://vt.zhonguo3118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://kf.zhonguo2118.cn

[S34] C++：遍历 vector
来源：https://vc.zhonguo4118.cn

for (auto &x : v) { std::cout << x; }
来源：https://wn.zhonguo4118.cn

[S35] C++：map
来源：https://wv.zhonguo3118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://wf.zhonguo5118.cn

[S36] C++：unordered_map
来源：https://as.zhonguo2118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://rc.zhonguo1118.cn

[S37] C++：set
来源：https://nt.zhonguo3118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://pg.zhonguo8118.cn

[S38] C++：排序
来源：https://wv.zhonguo8118.cn

std::sort(v.begin(), v.end());
来源：https://pu.zhonguo7118.cn

[S39] C++：自定义比较器排序
来源：https://am.zhonguo3118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://qt.zhonguo4118.cn

[S40] C++：查找元素
来源：https://xn.zhonguo7118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://sh.zhonguo7118.cn

[S41] C++：类与构造函数
来源：https://jh.zhonguo8118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://gw.zhonguo2118.cn

[S42] C++：继承与虚函数
来源：https://iw.zhonguo7118.cn

class B : public Base { public: void f() override {} };
来源：https://qw.zhonguo7118.cn

[S43] C++：智能指针
来源：https://xi.zhonguo8118.cn

auto p = std::make_unique<int>(5);
来源：https://eb.zhonguo2118.cn

[S44] C++：引用传参
来源：https://qb.zhonguo7118.cn

void inc(int &x) { ++x; }
来源：https://il.zhonguo4118.cn

[S45] C++：lambda
来源：https://lz.zhonguo5118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://js.zhonguo5118.cn

[S46] C++：函数模板
来源：https://jt.zhonguo8118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://eg.zhonguo4118.cn


<!-- 参考信息 -->