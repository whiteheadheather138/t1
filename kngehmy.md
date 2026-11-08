代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://wa.zhonguo7118.cn

[Q90] 生成序号列
来源：https://wa.zhonguo5118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://ky.zhonguo1118.cn

================================================================================
来源：https://zb.zhonguo1118.cn

R. Bash 专题
来源：https://nw.zhonguo2118.cn

================================================================================
来源：https://iu.zhonguo1118.cn

[R01] shebang 与严格模式
来源：https://us.zhonguo1118.cn

#!/usr/bin/env bash
来源：https://jt.zhonguo8118.cn

set -euo pipefail
来源：https://mh.zhonguo4118.cn

[R02] 变量赋值与使用
来源：https://xs.zhonguo3118.cn

name="Tom"; echo "$name"
来源：https://dh.zhonguo2118.cn

[R03] 只读变量
来源：https://nw.zhonguo6118.cn

readonly PI=3.14
来源：https://lh.zhonguo7118.cn

[R04] 位置参数
来源：https://di.zhonguo1118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://dr.zhonguo3118.cn

[R05] 参数默认值
来源：https://gn.zhonguo6118.cn

name="${1:-default}"
来源：https://lr.zhonguo2118.cn

[R06] 判断命令是否存在
来源：https://rl.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://wj.zhonguo6118.cn

[R07] if 判断文件
来源：https://jb.zhonguo6118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://ks.zhonguo7118.cn

[R08] 数值比较
来源：https://wh.zhonguo7118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://ez.zhonguo4118.cn

[R09] 字符串比较
来源：https://yw.zhonguo6118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://fc.zhonguo4118.cn

[R10] 正则匹配
来源：https://xn.zhonguo7118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://pn.zhonguo1118.cn

[R11] case 多分支
来源：https://kb.zhonguo1118.cn

case "$1" in
来源：https://gy.zhonguo1118.cn

start) echo "启动" ;;
来源：https://uw.zhonguo3118.cn

stop)  echo "停止" ;;
来源：https://ug.zhonguo5118.cn

*)     echo "未知命令" ;;
来源：https://cc.zhonguo6118.cn

esac
来源：https://to.zhonguo6118.cn

[R12] for 遍历文件
来源：https://bd.zhonguo6118.cn

for f in *.txt; do echo "$f"; done
来源：https://qh.zhonguo6118.cn

[R13] for 计数循环
来源：https://qj.zhonguo2118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ot.zhonguo1118.cn

[R14] C 风格 for
来源：https://pg.zhonguo1118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://nh.zhonguo8118.cn

[R15] while 逐行读文件
来源：https://gl.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://iq.zhonguo7118.cn

[R16] until 等待条件
来源：https://pv.zhonguo1118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://de.zhonguo6118.cn

[R17] 数组定义与取值
来源：https://ww.zhonguo8118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://ay.zhonguo3118.cn

[R18] 遍历数组
来源：https://py.zhonguo6118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://qy.zhonguo8118.cn

[R19] 数组长度
来源：https://je.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://jb.zhonguo2118.cn

[R20] 关联数组（字典）
来源：https://br.zhonguo7118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://ix.zhonguo1118.cn

[R21] 字符串长度
来源：https://cx.zhonguo5118.cn

echo "${#s}"
来源：https://tt.zhonguo4118.cn

[R22] 截取子串
来源：https://sg.zhonguo7118.cn

echo "${s:0:5}"
来源：https://ze.zhonguo6118.cn

[R23] 字符串替换
来源：https://kd.zhonguo7118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://yl.zhonguo8118.cn

[R24] 大小写转换
来源：https://ec.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://yy.zhonguo8118.cn

[R25] 去后缀 / 去前缀
来源：https://bk.zhonguo5118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://qe.zhonguo2118.cn

[R26] 命令替换
来源：https://ut.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://sm.zhonguo8118.cn

[R27] 算术展开
来源：https://rt.zhonguo1118.cn

echo $((1 + 2 * 3))
来源：https://en.zhonguo6118.cn

[R28] 浮点运算
来源：https://ob.zhonguo7118.cn

echo "scale=2; 10/3" | bc
来源：https://wt.zhonguo8118.cn

[R29] 定义函数
来源：https://rv.zhonguo2118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://rz.zhonguo8118.cn

[R30] 函数返回状态码
来源：https://rk.zhonguo2118.cn

f() { return 0; }; f || echo "失败了"
来源：https://cr.zhonguo1118.cn

[R31] 局部变量
来源：https://pe.zhonguo8118.cn

f() { local x=1; echo "$x"; }
来源：https://qs.zhonguo8118.cn

[R32] 参数个数校验
来源：https://in.zhonguo7118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://yu.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://kf.zhonguo5118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://xk.zhonguo2118.cn

[R34] 退出时清理
来源：https://vq.zhonguo4118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://mz.zhonguo6118.cn

[R35] 后台执行并等待
来源：https://rs.zhonguo5118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://vg.zhonguo8118.cn

[R36] 并发执行多个任务
来源：https://px.zhonguo6118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://wn.zhonguo4118.cn

[R37] 把输出赋给变量
来源：https://vi.zhonguo4118.cn

files=$(ls -1)
来源：https://kh.zhonguo6118.cn

[R38] 管道串联
来源：https://jy.zhonguo6118.cn

cat a.txt | grep -i error | wc -l
来源：https://sd.zhonguo3118.cn

[R39] 重定向标准输出与错误
来源：https://dr.zhonguo7118.cn

cmd > out.log 2>&1
来源：https://dy.zhonguo4118.cn

[R40] 追加写日志
来源：https://ru.zhonguo2118.cn

echo "log" >> out.log
来源：https://rn.zhonguo1118.cn

[R41] 丢弃输出
来源：https://tf.zhonguo6118.cn

cmd >/dev/null 2>&1
来源：https://ay.zhonguo3118.cn

[R42] 输入重定向
来源：https://cg.zhonguo8118.cn

wc -l < a.txt
来源：https://ej.zhonguo4118.cn

[R43] 按名字查找文件
来源：https://uo.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://gt.zhonguo8118.cn

[R44] 按修改时间查找
来源：https://zw.zhonguo4118.cn

find . -mtime -7 -type f
来源：https://nj.zhonguo2118.cn

[R45] 批量删除
来源：https://km.zhonguo5118.cn

find . -name "*.tmp" -delete
来源：https://wm.zhonguo6118.cn

[R46] 递归替换文件内容
来源：https://sf.zhonguo3118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://fx.zhonguo6118.cn

[R47] sed 单行替换
来源：https://dg.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://kr.zhonguo7118.cn

[R48] awk 取指定列
来源：https://ka.zhonguo5118.cn

awk '{print $1, $3}' a.txt
来源：https://zr.zhonguo3118.cn

[R49] awk 带条件
来源：https://sb.zhonguo4118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ru.zhonguo8118.cn

[R50] awk 求和
来源：https://le.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://vq.zhonguo4118.cn

[R51] 排序去重取前几
来源：https://md.zhonguo6118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://ko.zhonguo3118.cn

[R52] 统计行数
来源：https://uh.zhonguo4118.cn

wc -l a.txt
来源：https://wm.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://dv.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://yy.zhonguo7118.cn

[R54] 比较两个文件
来源：https://oj.zhonguo5118.cn

diff a.txt b.txt
来源：https://jq.zhonguo4118.cn

[R55] 压缩与解压
来源：https://vb.zhonguo1118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://wb.zhonguo1118.cn

[R56] 远程拷贝
来源：https://yh.zhonguo8118.cn

scp file user@host:/path/
来源：https://ih.zhonguo4118.cn

[R57] 远程执行命令
来源：https://qr.zhonguo6118.cn

ssh user@host 'uptime'
来源：https://lh.zhonguo7118.cn

[R58] 下载文件
来源：https://oy.zhonguo4118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://ih.zhonguo4118.cn

[R59] 发 POST JSON
来源：https://sq.zhonguo6118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://kc.zhonguo5118.cn

[R60] 只看 HTTP 状态码
来源：https://lz.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://mq.zhonguo4118.cn

[R61] 磁盘占用
来源：https://mp.zhonguo8118.cn

df -h;  du -sh *
来源：https://ph.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://ur.zhonguo1118.cn

du -ah . | sort -rh | head -10
来源：https://wy.zhonguo7118.cn

[R63] 内存与进程
来源：https://db.zhonguo3118.cn

free -h;  ps aux | grep nginx
来源：https://vn.zhonguo8118.cn

[R64] 结束进程
来源：https://qq.zhonguo8118.cn

kill -9 $(pgrep -f app.py)
来源：https://qt.zhonguo3118.cn

[R65] 查看端口占用
来源：https://vj.zhonguo6118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://xq.zhonguo5118.cn

[R66] 定时任务
来源：https://rd.zhonguo3118.cn

crontab -e;  crontab -l
来源：https://vp.zhonguo5118.cn

[R67] 生成随机十六进制串
来源：https://ux.zhonguo7118.cn

openssl rand -hex 16
来源：https://rm.zhonguo3118.cn

[R68] 计算文件校验值
来源：https://mg.zhonguo8118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://rj.zhonguo1118.cn

[R69] 生成随机密码
来源：https://cx.zhonguo5118.cn

head -c 16 /dev/urandom | base64
来源：https://fh.zhonguo8118.cn

[R70] 时间戳与互转
来源：https://cd.zhonguo1118.cn

date +%s;  date -d @1700000000
来源：https://mf.zhonguo5118.cn

[R71] 日期格式化
来源：https://gf.zhonguo5118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://fx.zhonguo1118.cn

[R72] 等待端口就绪
来源：https://sx.zhonguo6118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://lq.zhonguo7118.cn

[R73] 分割大日志
来源：https://tk.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://mb.zhonguo8118.cn

[R74] 批量重命名
来源：https://xf.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://bi.zhonguo3118.cn

[R75] 导出环境变量
来源：https://rx.zhonguo3118.cn

export PATH="$HOME/bin:$PATH"
来源：https://jx.zhonguo5118.cn

[R76] 使用临时文件
来源：https://hu.zhonguo2118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://nr.zhonguo5118.cn

[R77] 读取用户输入
来源：https://ww.zhonguo4118.cn

read -rp "请输入: " ans
来源：https://yx.zhonguo6118.cn

[R78] 交互式菜单
来源：https://sv.zhonguo3118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://zk.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://es.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://do.zhonguo2118.cn

[R80] 查看脚本执行耗时
来源：https://cv.zhonguo1118.cn

time ./run.sh
来源：https://fb.zhonguo4118.cn

================================================================================
来源：https://wt.zhonguo3118.cn

S. C / C++ 专题
来源：https://ec.zhonguo7118.cn

================================================================================
来源：https://bq.zhonguo7118.cn

[S01] C：Hello World
来源：https://cu.zhonguo1118.cn

#include <stdio.h>
来源：https://th.zhonguo4118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://im.zhonguo4118.cn

[S02] C：变量与格式化输出
来源：https://ot.zhonguo3118.cn

int a = 10; printf("%d\n", a);
来源：https://su.zhonguo1118.cn

[S03] C：读入整数
来源：https://xh.zhonguo8118.cn

int x; scanf("%d", &x);
来源：https://xc.zhonguo7118.cn

[S04] C：字符串复制
来源：https://uj.zhonguo4118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://gf.zhonguo4118.cn

[S05] C：字符串长度
来源：https://vf.zhonguo7118.cn

strlen(s)
来源：https://rg.zhonguo6118.cn

[S06] C：字符串比较
来源：https://zn.zhonguo5118.cn

strcmp(a, b) == 0
来源：https://va.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://rn.zhonguo3118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://tb.zhonguo8118.cn

[S08] C：动态内存分配与释放
来源：https://la.zhonguo2118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://si.zhonguo1118.cn

[S09] C：结构体定义与初始化
来源：https://ll.zhonguo6118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ps.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://ou.zhonguo8118.cn

int *p = &a;  *p = 5;
来源：https://je.zhonguo7118.cn

[S11] C：逐行读文件
来源：https://zm.zhonguo5118.cn

FILE *f = fopen("a.txt", "r");
来源：https://fk.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://al.zhonguo3118.cn

fclose(f);
来源：https://oq.zhonguo8118.cn

[S12] C：写文件
来源：https://uu.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://tc.zhonguo1118.cn

[S13] C：宏定义
来源：https://qy.zhonguo3118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://xy.zhonguo2118.cn

[S14] C：枚举
来源：https://ux.zhonguo7118.cn

enum Color { RED, GREEN, BLUE };
来源：https://jn.zhonguo6118.cn

[S15] C：类型转换
来源：https://na.zhonguo8118.cn

(double) a / b
来源：https://zp.zhonguo7118.cn

[S16] C：位操作置位
来源：https://fi.zhonguo3118.cn

x |= (1 << 3);
来源：https://mt.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://dy.zhonguo6118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://fd.zhonguo2118.cn

[S18] C：命令行参数
来源：https://cn.zhonguo6118.cn

int main(int argc, char **argv)
来源：https://ss.zhonguo1118.cn

[S19] C：快速排序
来源：https://om.zhonguo7118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://ls.zhonguo6118.cn

[S20] C：二分查找
来源：https://in.zhonguo8118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://ur.zhonguo2118.cn

[S21] C：字符类别判断
来源：https://up.zhonguo2118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://si.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://to.zhonguo8118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://tm.zhonguo6118.cn

[S23] C：随机数
来源：https://xw.zhonguo3118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://yz.zhonguo2118.cn

[S24] C：获取本地时间
来源：https://yo.zhonguo3118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://mf.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://jp.zhonguo4118.cn

memcpy(dst, src, n);
来源：https://ly.zhonguo8118.cn

[S26] C：内存清零
来源：https://xu.zhonguo8118.cn

memset(a, 0, sizeof a);
来源：https://xs.zhonguo6118.cn

[S27] C：定义常量
来源：https://dz.zhonguo7118.cn

const double PI = 3.14159;
来源：https://cv.zhonguo5118.cn

[S28] C：静态变量
来源：https://ka.zhonguo5118.cn

static int counter = 0;
来源：https://mt.zhonguo8118.cn

[S29] C：变参函数
来源：https://cx.zhonguo7118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://uh.zhonguo2118.cn

[S30] C：头文件保护
来源：https://ah.zhonguo6118.cn

#ifndef X_H
来源：https://oo.zhonguo7118.cn

#define X_H
来源：https://gv.zhonguo2118.cn

#endif
来源：https://la.zhonguo6118.cn

[S31] C++：Hello World
来源：https://hb.zhonguo4118.cn

#include <iostream>
来源：https://oc.zhonguo3118.cn

int main() { std::cout << "Hello\n"; }
来源：https://zf.zhonguo2118.cn

[S32] C++：字符串
来源：https://zs.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://wi.zhonguo3118.cn

[S33] C++：vector 增删
来源：https://kd.zhonguo2118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://bj.zhonguo6118.cn

[S34] C++：遍历 vector
来源：https://yb.zhonguo3118.cn

for (auto &x : v) { std::cout << x; }
来源：https://vc.zhonguo2118.cn

[S35] C++：map
来源：https://zb.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://mb.zhonguo2118.cn

[S36] C++：unordered_map
来源：https://yk.zhonguo2118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://zd.zhonguo8118.cn

[S37] C++：set
来源：https://iy.zhonguo1118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://yz.zhonguo8118.cn

[S38] C++：排序
来源：https://tn.zhonguo1118.cn

std::sort(v.begin(), v.end());
来源：https://qp.zhonguo4118.cn

[S39] C++：自定义比较器排序
来源：https://hg.zhonguo5118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://qi.zhonguo2118.cn

[S40] C++：查找元素
来源：https://oi.zhonguo7118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://dv.zhonguo6118.cn

[S41] C++：类与构造函数
来源：https://ty.zhonguo2118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://kx.zhonguo8118.cn

[S42] C++：继承与虚函数
来源：https://xe.zhonguo7118.cn

class B : public Base { public: void f() override {} };
来源：https://xo.zhonguo8118.cn

[S43] C++：智能指针
来源：https://mi.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://ck.zhonguo8118.cn

[S44] C++：引用传参
来源：https://uj.zhonguo7118.cn

void inc(int &x) { ++x; }
来源：https://qm.zhonguo8118.cn

[S45] C++：lambda
来源：https://jw.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://px.zhonguo6118.cn

[S46] C++：函数模板
来源：https://nq.zhonguo8118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://cn.zhonguo3118.cn

[S47] C++：结构化绑定遍历
来源：https://jh.zhonguo4118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://el.zhonguo8118.cn

[S48] C++：逐行读文件
来源：https://md.zhonguo2118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://yk.zhonguo6118.cn

while (std::getline(in, line)) { }
来源：https://aw.zhonguo5118.cn

[S49] C++：写文件
来源：https://br.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://pm.zhonguo1118.cn

[S50] C++：格式化数字
来源：https://zb.zhonguo4118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://um.zhonguo5118.cn

[S51] C++：显式类型转换
来源：https://tf.zhonguo3118.cn

static_cast<double>(a) / b
来源：https://xx.zhonguo1118.cn

[S52] C++：const 与 noexcept
来源：https://nr.zhonguo1118.cn

int size() const noexcept { return n_; }
来源：https://pl.zhonguo6118.cn

[S53] C++：移动语义
来源：https://iz.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://hi.zhonguo2118.cn

[S54] C++：异常处理
来源：https://on.zhonguo5118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ic.zhonguo5118.cn

[S55] C++：结构化绑定
来源：https://tn.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://vi.zhonguo6118.cn

[S56] C++：optional
来源：https://br.zhonguo7118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ho.zhonguo7118.cn

[S57] C++：编译期常量
来源：https://ns.zhonguo4118.cn

constexpr int N = 10;
来源：https://mk.zhonguo2118.cn

[S58] C++：命名空间
来源：https://kt.zhonguo8118.cn

namespace ns { int f() { return 1; } }
来源：https://ra.zhonguo2118.cn

[S59] C++：静态断言
来源：https://dp.zhonguo4118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://fu.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://vm.zhonguo3118.cn


<!-- 参考信息 -->