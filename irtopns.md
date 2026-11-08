代发 wailian999

readonly PI=3.14
来源：https://ga.zhonguo7118.cn

[R04] 位置参数
来源：https://om.zhonguo3118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://vx.zhonguo3118.cn

[R05] 参数默认值
来源：https://cs.zhonguo7118.cn

name="${1:-default}"
来源：https://jl.zhonguo1118.cn

[R06] 判断命令是否存在
来源：https://av.zhonguo2118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://ey.zhonguo1118.cn

[R07] if 判断文件
来源：https://sj.zhonguo6118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://oh.zhonguo3118.cn

[R08] 数值比较
来源：https://xv.zhonguo6118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://rm.zhonguo6118.cn

[R09] 字符串比较
来源：https://as.zhonguo6118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://rx.zhonguo1118.cn

[R10] 正则匹配
来源：https://sy.zhonguo4118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ff.zhonguo3118.cn

[R11] case 多分支
来源：https://rv.zhonguo6118.cn

case "$1" in
来源：https://nf.zhonguo2118.cn

start) echo "启动" ;;
来源：https://bd.zhonguo1118.cn

stop)  echo "停止" ;;
来源：https://wn.zhonguo5118.cn

*)     echo "未知命令" ;;
来源：https://oe.zhonguo7118.cn

esac
来源：https://jj.zhonguo7118.cn

[R12] for 遍历文件
来源：https://wj.zhonguo8118.cn

for f in *.txt; do echo "$f"; done
来源：https://kq.zhonguo5118.cn

[R13] for 计数循环
来源：https://va.zhonguo6118.cn

for i in {1..10}; do echo "$i"; done
来源：https://hp.zhonguo4118.cn

[R14] C 风格 for
来源：https://hm.zhonguo2118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://rb.zhonguo2118.cn

[R15] while 逐行读文件
来源：https://oq.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://wh.zhonguo5118.cn

[R16] until 等待条件
来源：https://hh.zhonguo7118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://br.zhonguo1118.cn

[R17] 数组定义与取值
来源：https://kf.zhonguo7118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://gl.zhonguo3118.cn

[R18] 遍历数组
来源：https://py.zhonguo3118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://go.zhonguo1118.cn

[R19] 数组长度
来源：https://ol.zhonguo1118.cn

echo "${#arr[@]}"
来源：https://cb.zhonguo7118.cn

[R20] 关联数组（字典）
来源：https://sk.zhonguo4118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://iw.zhonguo8118.cn

[R21] 字符串长度
来源：https://qf.zhonguo4118.cn

echo "${#s}"
来源：https://ky.zhonguo6118.cn

[R22] 截取子串
来源：https://on.zhonguo6118.cn

echo "${s:0:5}"
来源：https://ff.zhonguo1118.cn

[R23] 字符串替换
来源：https://jt.zhonguo4118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://gi.zhonguo7118.cn

[R24] 大小写转换
来源：https://bk.zhonguo5118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://hk.zhonguo7118.cn

[R25] 去后缀 / 去前缀
来源：https://oj.zhonguo3118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://nm.zhonguo8118.cn

[R26] 命令替换
来源：https://ot.zhonguo3118.cn

now=$(date +%F); echo "$now"
来源：https://za.zhonguo8118.cn

[R27] 算术展开
来源：https://wi.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://he.zhonguo4118.cn

[R28] 浮点运算
来源：https://yl.zhonguo1118.cn

echo "scale=2; 10/3" | bc
来源：https://xr.zhonguo6118.cn

[R29] 定义函数
来源：https://lr.zhonguo7118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://fe.zhonguo1118.cn

[R30] 函数返回状态码
来源：https://yz.zhonguo7118.cn

f() { return 0; }; f || echo "失败了"
来源：https://mw.zhonguo6118.cn

[R31] 局部变量
来源：https://qi.zhonguo8118.cn

f() { local x=1; echo "$x"; }
来源：https://ej.zhonguo1118.cn

[R32] 参数个数校验
来源：https://vq.zhonguo1118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://ll.zhonguo1118.cn

[R33] 捕获错误并提示行号
来源：https://xo.zhonguo2118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://il.zhonguo5118.cn

[R34] 退出时清理
来源：https://fd.zhonguo1118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://vp.zhonguo7118.cn

[R35] 后台执行并等待
来源：https://te.zhonguo7118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://mv.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://me.zhonguo8118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://bf.zhonguo8118.cn

[R37] 把输出赋给变量
来源：https://ek.zhonguo1118.cn

files=$(ls -1)
来源：https://wu.zhonguo5118.cn

[R38] 管道串联
来源：https://yw.zhonguo4118.cn

cat a.txt | grep -i error | wc -l
来源：https://sq.zhonguo4118.cn

[R39] 重定向标准输出与错误
来源：https://vb.zhonguo4118.cn

cmd > out.log 2>&1
来源：https://hd.zhonguo3118.cn

[R40] 追加写日志
来源：https://ga.zhonguo2118.cn

echo "log" >> out.log
来源：https://qa.zhonguo2118.cn

[R41] 丢弃输出
来源：https://kb.zhonguo4118.cn

cmd >/dev/null 2>&1
来源：https://jw.zhonguo5118.cn

[R42] 输入重定向
来源：https://sj.zhonguo4118.cn

wc -l < a.txt
来源：https://ug.zhonguo8118.cn

[R43] 按名字查找文件
来源：https://er.zhonguo2118.cn

find . -name "*.log" -type f
来源：https://vb.zhonguo7118.cn

[R44] 按修改时间查找
来源：https://rn.zhonguo8118.cn

find . -mtime -7 -type f
来源：https://wq.zhonguo6118.cn

[R45] 批量删除
来源：https://rf.zhonguo2118.cn

find . -name "*.tmp" -delete
来源：https://if.zhonguo3118.cn

[R46] 递归替换文件内容
来源：https://rr.zhonguo5118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://vt.zhonguo2118.cn

[R47] sed 单行替换
来源：https://hz.zhonguo2118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://va.zhonguo1118.cn

[R48] awk 取指定列
来源：https://ao.zhonguo4118.cn

awk '{print $1, $3}' a.txt
来源：https://bo.zhonguo6118.cn

[R49] awk 带条件
来源：https://vu.zhonguo2118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ss.zhonguo3118.cn

[R50] awk 求和
来源：https://nf.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://jw.zhonguo8118.cn

[R51] 排序去重取前几
来源：https://sx.zhonguo3118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://kl.zhonguo7118.cn

[R52] 统计行数
来源：https://zk.zhonguo6118.cn

wc -l a.txt
来源：https://wp.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://aj.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://jo.zhonguo8118.cn

[R54] 比较两个文件
来源：https://ui.zhonguo5118.cn

diff a.txt b.txt
来源：https://yv.zhonguo2118.cn

[R55] 压缩与解压
来源：https://ko.zhonguo2118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ej.zhonguo2118.cn

[R56] 远程拷贝
来源：https://bp.zhonguo8118.cn

scp file user@host:/path/
来源：https://yz.zhonguo4118.cn

[R57] 远程执行命令
来源：https://nu.zhonguo2118.cn

ssh user@host 'uptime'
来源：https://ew.zhonguo1118.cn

[R58] 下载文件
来源：https://rl.zhonguo7118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://ri.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://dp.zhonguo3118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://hj.zhonguo4118.cn

[R60] 只看 HTTP 状态码
来源：https://ba.zhonguo1118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://ea.zhonguo2118.cn

[R61] 磁盘占用
来源：https://wx.zhonguo7118.cn

df -h;  du -sh *
来源：https://ek.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://gw.zhonguo4118.cn

du -ah . | sort -rh | head -10
来源：https://yf.zhonguo1118.cn

[R63] 内存与进程
来源：https://al.zhonguo3118.cn

free -h;  ps aux | grep nginx
来源：https://pa.zhonguo3118.cn

[R64] 结束进程
来源：https://vz.zhonguo3118.cn

kill -9 $(pgrep -f app.py)
来源：https://xm.zhonguo2118.cn

[R65] 查看端口占用
来源：https://nf.zhonguo7118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://oo.zhonguo1118.cn

[R66] 定时任务
来源：https://ni.zhonguo3118.cn

crontab -e;  crontab -l
来源：https://ta.zhonguo8118.cn

[R67] 生成随机十六进制串
来源：https://se.zhonguo1118.cn

openssl rand -hex 16
来源：https://xh.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://po.zhonguo4118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://hd.zhonguo2118.cn

[R69] 生成随机密码
来源：https://ng.zhonguo3118.cn

head -c 16 /dev/urandom | base64
来源：https://ny.zhonguo2118.cn

[R70] 时间戳与互转
来源：https://dd.zhonguo1118.cn

date +%s;  date -d @1700000000
来源：https://fc.zhonguo8118.cn

[R71] 日期格式化
来源：https://mq.zhonguo5118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://mv.zhonguo7118.cn

[R72] 等待端口就绪
来源：https://jq.zhonguo1118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://ct.zhonguo7118.cn

[R73] 分割大日志
来源：https://tx.zhonguo3118.cn

split -l 1000 big.log part_
来源：https://ci.zhonguo5118.cn

[R74] 批量重命名
来源：https://pq.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ox.zhonguo8118.cn

[R75] 导出环境变量
来源：https://zy.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://we.zhonguo2118.cn

[R76] 使用临时文件
来源：https://xk.zhonguo7118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://ik.zhonguo8118.cn

[R77] 读取用户输入
来源：https://hc.zhonguo3118.cn

read -rp "请输入: " ans
来源：https://sy.zhonguo4118.cn

[R78] 交互式菜单
来源：https://bv.zhonguo5118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://pt.zhonguo4118.cn

[R79] 解析命令行选项
来源：https://tk.zhonguo1118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://yi.zhonguo6118.cn

[R80] 查看脚本执行耗时
来源：https://ep.zhonguo6118.cn

time ./run.sh
来源：https://he.zhonguo7118.cn

================================================================================
来源：https://ru.zhonguo5118.cn

S. C / C++ 专题
来源：https://kj.zhonguo4118.cn

================================================================================
来源：https://mb.zhonguo3118.cn

[S01] C：Hello World
来源：https://xk.zhonguo5118.cn

#include <stdio.h>
来源：https://cl.zhonguo3118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://yr.zhonguo5118.cn

[S02] C：变量与格式化输出
来源：https://kw.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://au.zhonguo7118.cn

[S03] C：读入整数
来源：https://ol.zhonguo1118.cn

int x; scanf("%d", &x);
来源：https://ku.zhonguo2118.cn

[S04] C：字符串复制
来源：https://qq.zhonguo6118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://en.zhonguo4118.cn

[S05] C：字符串长度
来源：https://uy.zhonguo3118.cn

strlen(s)
来源：https://xs.zhonguo7118.cn

[S06] C：字符串比较
来源：https://mr.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://db.zhonguo1118.cn

[S07] C：数组遍历求和
来源：https://vd.zhonguo8118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://em.zhonguo6118.cn

[S08] C：动态内存分配与释放
来源：https://tl.zhonguo3118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://ru.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://eh.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ha.zhonguo5118.cn

[S10] C：指针与解引用
来源：https://gq.zhonguo6118.cn

int *p = &a;  *p = 5;
来源：https://sa.zhonguo1118.cn

[S11] C：逐行读文件
来源：https://cf.zhonguo4118.cn

FILE *f = fopen("a.txt", "r");
来源：https://sa.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ei.zhonguo2118.cn

fclose(f);
来源：https://fx.zhonguo5118.cn

[S12] C：写文件
来源：https://zx.zhonguo5118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://yc.zhonguo3118.cn

[S13] C：宏定义
来源：https://ph.zhonguo1118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://hn.zhonguo5118.cn

[S14] C：枚举
来源：https://jv.zhonguo4118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ax.zhonguo7118.cn

[S15] C：类型转换
来源：https://rt.zhonguo1118.cn

(double) a / b
来源：https://th.zhonguo6118.cn

[S16] C：位操作置位
来源：https://je.zhonguo6118.cn

x |= (1 << 3);
来源：https://xq.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://qc.zhonguo3118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://rw.zhonguo5118.cn

[S18] C：命令行参数
来源：https://ys.zhonguo2118.cn

int main(int argc, char **argv)
来源：https://wy.zhonguo4118.cn

[S19] C：快速排序
来源：https://iz.zhonguo4118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://bp.zhonguo8118.cn

[S20] C：二分查找
来源：https://bc.zhonguo5118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://iw.zhonguo6118.cn

[S21] C：字符类别判断
来源：https://qg.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://tv.zhonguo7118.cn

[S22] C：字符串转数字
来源：https://tm.zhonguo6118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://km.zhonguo3118.cn

[S23] C：随机数
来源：https://ae.zhonguo5118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://od.zhonguo6118.cn

[S24] C：获取本地时间
来源：https://wf.zhonguo8118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://en.zhonguo1118.cn

[S25] C：内存拷贝
来源：https://ne.zhonguo2118.cn

memcpy(dst, src, n);
来源：https://lr.zhonguo2118.cn

[S26] C：内存清零
来源：https://bg.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://in.zhonguo3118.cn

[S27] C：定义常量
来源：https://iw.zhonguo8118.cn

const double PI = 3.14159;
来源：https://db.zhonguo4118.cn

[S28] C：静态变量
来源：https://vs.zhonguo3118.cn

static int counter = 0;
来源：https://zf.zhonguo1118.cn

[S29] C：变参函数
来源：https://wt.zhonguo3118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://de.zhonguo8118.cn

[S30] C：头文件保护
来源：https://fi.zhonguo4118.cn

#ifndef X_H
来源：https://es.zhonguo1118.cn

#define X_H
来源：https://qv.zhonguo8118.cn

#endif
来源：https://hg.zhonguo7118.cn

[S31] C++：Hello World
来源：https://ws.zhonguo4118.cn

#include <iostream>
来源：https://hz.zhonguo3118.cn

int main() { std::cout << "Hello\n"; }
来源：https://av.zhonguo4118.cn

[S32] C++：字符串
来源：https://ov.zhonguo1118.cn

std::string s = "hi";  s += "!";
来源：https://sv.zhonguo2118.cn

[S33] C++：vector 增删
来源：https://al.zhonguo7118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://zu.zhonguo8118.cn

[S34] C++：遍历 vector
来源：https://qf.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://vp.zhonguo3118.cn

[S35] C++：map
来源：https://rt.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://xt.zhonguo3118.cn

[S36] C++：unordered_map
来源：https://zg.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://bx.zhonguo7118.cn

[S37] C++：set
来源：https://vg.zhonguo2118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://eb.zhonguo7118.cn

[S38] C++：排序
来源：https://qr.zhonguo5118.cn

std::sort(v.begin(), v.end());
来源：https://bs.zhonguo2118.cn

[S39] C++：自定义比较器排序
来源：https://wv.zhonguo2118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://du.zhonguo8118.cn

[S40] C++：查找元素
来源：https://eq.zhonguo3118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://xu.zhonguo7118.cn

[S41] C++：类与构造函数
来源：https://pf.zhonguo1118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://da.zhonguo4118.cn

[S42] C++：继承与虚函数
来源：https://xf.zhonguo7118.cn

class B : public Base { public: void f() override {} };
来源：https://te.zhonguo5118.cn

[S43] C++：智能指针
来源：https://yn.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://jb.zhonguo4118.cn

[S44] C++：引用传参
来源：https://rb.zhonguo6118.cn

void inc(int &x) { ++x; }
来源：https://tr.zhonguo4118.cn

[S45] C++：lambda
来源：https://pu.zhonguo6118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://lc.zhonguo4118.cn

[S46] C++：函数模板
来源：https://fn.zhonguo8118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://ru.zhonguo7118.cn

[S47] C++：结构化绑定遍历
来源：https://ww.zhonguo7118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://ci.zhonguo2118.cn

[S48] C++：逐行读文件
来源：https://pr.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://we.zhonguo1118.cn

while (std::getline(in, line)) { }
来源：https://kf.zhonguo4118.cn

[S49] C++：写文件
来源：https://wh.zhonguo6118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://qy.zhonguo6118.cn

[S50] C++：格式化数字
来源：https://wq.zhonguo2118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://na.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://zn.zhonguo5118.cn

static_cast<double>(a) / b
来源：https://tu.zhonguo2118.cn

[S52] C++：const 与 noexcept
来源：https://mu.zhonguo3118.cn

int size() const noexcept { return n_; }
来源：https://nz.zhonguo6118.cn

[S53] C++：移动语义
来源：https://de.zhonguo6118.cn

std::vector<int> w = std::move(v);
来源：https://rs.zhonguo5118.cn

[S54] C++：异常处理
来源：https://gf.zhonguo3118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ya.zhonguo3118.cn

[S55] C++：结构化绑定
来源：https://us.zhonguo8118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://vy.zhonguo7118.cn

[S56] C++：optional
来源：https://uu.zhonguo8118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://de.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://gd.zhonguo5118.cn

constexpr int N = 10;
来源：https://dl.zhonguo8118.cn

[S58] C++：命名空间
来源：https://ud.zhonguo2118.cn

namespace ns { int f() { return 1; } }
来源：https://mt.zhonguo7118.cn

[S59] C++：静态断言
来源：https://js.zhonguo4118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ru.zhonguo4118.cn

[S60] C++：遍历并删除元素
来源：https://la.zhonguo2118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://gm.zhonguo5118.cn

================================================================================
来源：https://ex.zhonguo2118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://wu.zhonguo4118.cn

================================================================================
来源：https://ja.zhonguo3118.cn

[T01] Kotlin：Hello World
来源：https://sv.zhonguo4118.cn

println("Hello")
来源：https://qc.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://zt.zhonguo2118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://te.zhonguo3118.cn

[T03] Kotlin：字符串模板
来源：https://fp.zhonguo7118.cn

"值: $b"
来源：https://tt.zhonguo5118.cn

[T04] Kotlin：空安全
来源：https://yf.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://mx.zhonguo5118.cn


<!-- 参考信息 -->