代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：https://hs.zhonguo1118.cn

[R14] C 风格 for
来源：https://ng.zhonguo4118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://yz.zhonguo6118.cn

[R15] while 逐行读文件
来源：https://qo.zhonguo5118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://kw.zhonguo1118.cn

[R16] until 等待条件
来源：https://lf.zhonguo5118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://da.zhonguo6118.cn

[R17] 数组定义与取值
来源：https://cc.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://wf.zhonguo3118.cn

[R18] 遍历数组
来源：https://oy.zhonguo3118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://mk.zhonguo1118.cn

[R19] 数组长度
来源：https://bj.zhonguo8118.cn

echo "${#arr[@]}"
来源：https://sw.zhonguo7118.cn

[R20] 关联数组（字典）
来源：https://vu.zhonguo4118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://qt.zhonguo1118.cn

[R21] 字符串长度
来源：https://ck.zhonguo4118.cn

echo "${#s}"
来源：https://fq.zhonguo6118.cn

[R22] 截取子串
来源：https://ms.zhonguo3118.cn

echo "${s:0:5}"
来源：https://on.zhonguo3118.cn

[R23] 字符串替换
来源：https://in.zhonguo2118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://tc.zhonguo1118.cn

[R24] 大小写转换
来源：https://og.zhonguo1118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://lz.zhonguo3118.cn

[R25] 去后缀 / 去前缀
来源：https://ay.zhonguo2118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://be.zhonguo1118.cn

[R26] 命令替换
来源：https://tk.zhonguo8118.cn

now=$(date +%F); echo "$now"
来源：https://oj.zhonguo6118.cn

[R27] 算术展开
来源：https://bi.zhonguo8118.cn

echo $((1 + 2 * 3))
来源：https://pn.zhonguo5118.cn

[R28] 浮点运算
来源：https://le.zhonguo5118.cn

echo "scale=2; 10/3" | bc
来源：https://zr.zhonguo6118.cn

[R29] 定义函数
来源：https://bw.zhonguo1118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://hj.zhonguo3118.cn

[R30] 函数返回状态码
来源：https://lh.zhonguo1118.cn

f() { return 0; }; f || echo "失败了"
来源：https://yw.zhonguo1118.cn

[R31] 局部变量
来源：https://rl.zhonguo3118.cn

f() { local x=1; echo "$x"; }
来源：https://nf.zhonguo7118.cn

[R32] 参数个数校验
来源：https://wt.zhonguo2118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://ib.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://au.zhonguo7118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://qc.zhonguo2118.cn

[R34] 退出时清理
来源：https://bt.zhonguo1118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://wf.zhonguo7118.cn

[R35] 后台执行并等待
来源：https://lc.zhonguo3118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://vb.zhonguo1118.cn

[R36] 并发执行多个任务
来源：https://hy.zhonguo6118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://ob.zhonguo7118.cn

[R37] 把输出赋给变量
来源：https://cl.zhonguo7118.cn

files=$(ls -1)
来源：https://wk.zhonguo1118.cn

[R38] 管道串联
来源：https://fu.zhonguo4118.cn

cat a.txt | grep -i error | wc -l
来源：https://ts.zhonguo8118.cn

[R39] 重定向标准输出与错误
来源：https://wz.zhonguo4118.cn

cmd > out.log 2>&1
来源：https://nw.zhonguo1118.cn

[R40] 追加写日志
来源：https://bv.zhonguo6118.cn

echo "log" >> out.log
来源：https://qx.zhonguo6118.cn

[R41] 丢弃输出
来源：https://wx.zhonguo7118.cn

cmd >/dev/null 2>&1
来源：https://lg.zhonguo4118.cn

[R42] 输入重定向
来源：https://ri.zhonguo5118.cn

wc -l < a.txt
来源：https://ks.zhonguo6118.cn

[R43] 按名字查找文件
来源：https://wn.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://ra.zhonguo5118.cn

[R44] 按修改时间查找
来源：https://mx.zhonguo1118.cn

find . -mtime -7 -type f
来源：https://ek.zhonguo1118.cn

[R45] 批量删除
来源：https://qu.zhonguo2118.cn

find . -name "*.tmp" -delete
来源：https://kr.zhonguo8118.cn

[R46] 递归替换文件内容
来源：https://fp.zhonguo7118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://wu.zhonguo6118.cn

[R47] sed 单行替换
来源：https://wu.zhonguo4118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://il.zhonguo8118.cn

[R48] awk 取指定列
来源：https://yt.zhonguo6118.cn

awk '{print $1, $3}' a.txt
来源：https://vy.zhonguo6118.cn

[R49] awk 带条件
来源：https://co.zhonguo8118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ta.zhonguo7118.cn

[R50] awk 求和
来源：https://dr.zhonguo5118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://qy.zhonguo1118.cn

[R51] 排序去重取前几
来源：https://yl.zhonguo6118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://cn.zhonguo3118.cn

[R52] 统计行数
来源：https://zi.zhonguo1118.cn

wc -l a.txt
来源：https://qq.zhonguo4118.cn

[R53] 查看文件头与实时尾
来源：https://al.zhonguo3118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://wm.zhonguo6118.cn

[R54] 比较两个文件
来源：https://oy.zhonguo8118.cn

diff a.txt b.txt
来源：https://et.zhonguo1118.cn

[R55] 压缩与解压
来源：https://zc.zhonguo5118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://xk.zhonguo4118.cn

[R56] 远程拷贝
来源：https://dv.zhonguo2118.cn

scp file user@host:/path/
来源：https://yy.zhonguo1118.cn

[R57] 远程执行命令
来源：https://bv.zhonguo8118.cn

ssh user@host 'uptime'
来源：https://hc.zhonguo2118.cn

[R58] 下载文件
来源：https://pq.zhonguo5118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://cx.zhonguo7118.cn

[R59] 发 POST JSON
来源：https://vh.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://xt.zhonguo8118.cn

[R60] 只看 HTTP 状态码
来源：https://ql.zhonguo6118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://nt.zhonguo7118.cn

[R61] 磁盘占用
来源：https://no.zhonguo6118.cn

df -h;  du -sh *
来源：https://yz.zhonguo4118.cn

[R62] 找最占空间的文件
来源：https://id.zhonguo4118.cn

du -ah . | sort -rh | head -10
来源：https://ds.zhonguo8118.cn

[R63] 内存与进程
来源：https://tc.zhonguo7118.cn

free -h;  ps aux | grep nginx
来源：https://ss.zhonguo1118.cn

[R64] 结束进程
来源：https://qz.zhonguo1118.cn

kill -9 $(pgrep -f app.py)
来源：https://rs.zhonguo5118.cn

[R65] 查看端口占用
来源：https://qo.zhonguo3118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://qf.zhonguo1118.cn

[R66] 定时任务
来源：https://rz.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://vh.zhonguo7118.cn

[R67] 生成随机十六进制串
来源：https://nj.zhonguo4118.cn

openssl rand -hex 16
来源：https://rg.zhonguo6118.cn

[R68] 计算文件校验值
来源：https://tw.zhonguo6118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://iv.zhonguo4118.cn

[R69] 生成随机密码
来源：https://md.zhonguo7118.cn

head -c 16 /dev/urandom | base64
来源：https://ej.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://cb.zhonguo5118.cn

date +%s;  date -d @1700000000
来源：https://hr.zhonguo6118.cn

[R71] 日期格式化
来源：https://aj.zhonguo2118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://zj.zhonguo5118.cn

[R72] 等待端口就绪
来源：https://em.zhonguo8118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://oe.zhonguo2118.cn

[R73] 分割大日志
来源：https://mb.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://mv.zhonguo8118.cn

[R74] 批量重命名
来源：https://oz.zhonguo5118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://xo.zhonguo8118.cn

[R75] 导出环境变量
来源：https://mn.zhonguo8118.cn

export PATH="$HOME/bin:$PATH"
来源：https://qu.zhonguo6118.cn

[R76] 使用临时文件
来源：https://wl.zhonguo4118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://ji.zhonguo6118.cn

[R77] 读取用户输入
来源：https://rn.zhonguo5118.cn

read -rp "请输入: " ans
来源：https://lf.zhonguo1118.cn

[R78] 交互式菜单
来源：https://mb.zhonguo7118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://ar.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://ua.zhonguo1118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://zi.zhonguo8118.cn

[R80] 查看脚本执行耗时
来源：https://kz.zhonguo7118.cn

time ./run.sh
来源：https://bq.zhonguo4118.cn

================================================================================
来源：https://ru.zhonguo3118.cn

S. C / C++ 专题
来源：https://jf.zhonguo1118.cn

================================================================================
来源：https://xs.zhonguo5118.cn

[S01] C：Hello World
来源：https://od.zhonguo6118.cn

#include <stdio.h>
来源：https://ol.zhonguo8118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://ke.zhonguo2118.cn

[S02] C：变量与格式化输出
来源：https://if.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://hf.zhonguo1118.cn

[S03] C：读入整数
来源：https://hc.zhonguo5118.cn

int x; scanf("%d", &x);
来源：https://fa.zhonguo2118.cn

[S04] C：字符串复制
来源：https://wx.zhonguo7118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://dq.zhonguo8118.cn

[S05] C：字符串长度
来源：https://sp.zhonguo7118.cn

strlen(s)
来源：https://ad.zhonguo8118.cn

[S06] C：字符串比较
来源：https://lx.zhonguo1118.cn

strcmp(a, b) == 0
来源：https://iw.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://uw.zhonguo7118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://do.zhonguo7118.cn

[S08] C：动态内存分配与释放
来源：https://xi.zhonguo8118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://lh.zhonguo2118.cn

[S09] C：结构体定义与初始化
来源：https://oq.zhonguo3118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://mp.zhonguo1118.cn

[S10] C：指针与解引用
来源：https://yg.zhonguo4118.cn

int *p = &a;  *p = 5;
来源：https://zi.zhonguo4118.cn

[S11] C：逐行读文件
来源：https://ud.zhonguo8118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ra.zhonguo1118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://mc.zhonguo6118.cn

fclose(f);
来源：https://mz.zhonguo6118.cn

[S12] C：写文件
来源：https://rs.zhonguo3118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://bt.zhonguo6118.cn

[S13] C：宏定义
来源：https://fx.zhonguo6118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://zb.zhonguo7118.cn

[S14] C：枚举
来源：https://xq.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ms.zhonguo4118.cn

[S15] C：类型转换
来源：https://de.zhonguo8118.cn

(double) a / b
来源：https://jt.zhonguo7118.cn

[S16] C：位操作置位
来源：https://on.zhonguo4118.cn

x |= (1 << 3);
来源：https://wf.zhonguo3118.cn

[S17] C：安全拼接字符串
来源：https://td.zhonguo6118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://qj.zhonguo1118.cn

[S18] C：命令行参数
来源：https://jo.zhonguo6118.cn

int main(int argc, char **argv)
来源：https://li.zhonguo1118.cn

[S19] C：快速排序
来源：https://mf.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://xr.zhonguo8118.cn

[S20] C：二分查找
来源：https://cj.zhonguo8118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://cp.zhonguo2118.cn

[S21] C：字符类别判断
来源：https://rm.zhonguo1118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://tw.zhonguo7118.cn

[S22] C：字符串转数字
来源：https://jv.zhonguo3118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://qt.zhonguo2118.cn

[S23] C：随机数
来源：https://dw.zhonguo3118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://za.zhonguo7118.cn

[S24] C：获取本地时间
来源：https://tc.zhonguo1118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://yd.zhonguo3118.cn

[S25] C：内存拷贝
来源：https://vt.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://fd.zhonguo7118.cn

[S26] C：内存清零
来源：https://vm.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://xo.zhonguo7118.cn

[S27] C：定义常量
来源：https://yx.zhonguo2118.cn

const double PI = 3.14159;
来源：https://ws.zhonguo5118.cn

[S28] C：静态变量
来源：https://sa.zhonguo1118.cn

static int counter = 0;
来源：https://bw.zhonguo8118.cn

[S29] C：变参函数
来源：https://hx.zhonguo2118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://gk.zhonguo4118.cn

[S30] C：头文件保护
来源：https://po.zhonguo2118.cn

#ifndef X_H
来源：https://jf.zhonguo4118.cn

#define X_H
来源：https://ic.zhonguo2118.cn

#endif
来源：https://js.zhonguo7118.cn

[S31] C++：Hello World
来源：https://mo.zhonguo3118.cn

#include <iostream>
来源：https://fq.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://xb.zhonguo5118.cn

[S32] C++：字符串
来源：https://yo.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://rh.zhonguo8118.cn

[S33] C++：vector 增删
来源：https://rg.zhonguo1118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://tc.zhonguo6118.cn

[S34] C++：遍历 vector
来源：https://qv.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://vo.zhonguo1118.cn

[S35] C++：map
来源：https://gu.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://li.zhonguo5118.cn

[S36] C++：unordered_map
来源：https://ah.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ui.zhonguo8118.cn

[S37] C++：set
来源：https://jx.zhonguo8118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://et.zhonguo5118.cn

[S38] C++：排序
来源：https://ul.zhonguo6118.cn

std::sort(v.begin(), v.end());
来源：https://lg.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://tm.zhonguo4118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://dt.zhonguo5118.cn

[S40] C++：查找元素
来源：https://oy.zhonguo1118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://cp.zhonguo5118.cn

[S41] C++：类与构造函数
来源：https://cq.zhonguo2118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://tx.zhonguo4118.cn

[S42] C++：继承与虚函数
来源：https://zm.zhonguo2118.cn

class B : public Base { public: void f() override {} };
来源：https://ux.zhonguo7118.cn

[S43] C++：智能指针
来源：https://yh.zhonguo4118.cn

auto p = std::make_unique<int>(5);
来源：https://zv.zhonguo7118.cn

[S44] C++：引用传参
来源：https://yq.zhonguo5118.cn

void inc(int &x) { ++x; }
来源：https://fb.zhonguo3118.cn

[S45] C++：lambda
来源：https://py.zhonguo2118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://qk.zhonguo6118.cn

[S46] C++：函数模板
来源：https://wb.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://ej.zhonguo6118.cn

[S47] C++：结构化绑定遍历
来源：https://vk.zhonguo2118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://ou.zhonguo5118.cn

[S48] C++：逐行读文件
来源：https://kg.zhonguo7118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://di.zhonguo1118.cn

while (std::getline(in, line)) { }
来源：https://po.zhonguo5118.cn

[S49] C++：写文件
来源：https://qt.zhonguo7118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://ha.zhonguo8118.cn

[S50] C++：格式化数字
来源：https://sg.zhonguo8118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://jb.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://ms.zhonguo7118.cn

static_cast<double>(a) / b
来源：https://pb.zhonguo4118.cn

[S52] C++：const 与 noexcept
来源：https://hd.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://ml.zhonguo8118.cn

[S53] C++：移动语义
来源：https://jm.zhonguo2118.cn

std::vector<int> w = std::move(v);
来源：https://mi.zhonguo6118.cn

[S54] C++：异常处理
来源：https://yk.zhonguo6118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://sc.zhonguo8118.cn

[S55] C++：结构化绑定
来源：https://dv.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ls.zhonguo7118.cn

[S56] C++：optional
来源：https://ps.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://vg.zhonguo6118.cn

[S57] C++：编译期常量
来源：https://fo.zhonguo2118.cn

constexpr int N = 10;
来源：https://jp.zhonguo1118.cn

[S58] C++：命名空间
来源：https://lp.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://zk.zhonguo1118.cn

[S59] C++：静态断言
来源：https://kg.zhonguo7118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://za.zhonguo6118.cn

[S60] C++：遍历并删除元素
来源：https://fi.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://xi.zhonguo3118.cn

================================================================================
来源：https://iq.zhonguo7118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://cm.zhonguo3118.cn

================================================================================
来源：https://kg.zhonguo6118.cn

[T01] Kotlin：Hello World
来源：https://bx.zhonguo6118.cn

println("Hello")
来源：https://hx.zhonguo3118.cn

[T02] Kotlin：变量
来源：https://zq.zhonguo5118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://xv.zhonguo6118.cn

[T03] Kotlin：字符串模板
来源：https://wn.zhonguo3118.cn

"值: $b"
来源：https://er.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://hu.zhonguo4118.cn

val n: String? = null;  n?.length
来源：https://je.zhonguo1118.cn

[T05] Kotlin：when 表达式
来源：https://xc.zhonguo8118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://wf.zhonguo5118.cn

[T06] Kotlin：集合映射
来源：https://wz.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://nm.zhonguo7118.cn

[T07] Kotlin：集合过滤
来源：https://tn.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://si.zhonguo6118.cn

[T08] Kotlin：数据类
来源：https://pg.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://kp.zhonguo5118.cn

[T09] Kotlin：扩展函数
来源：https://bf.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://pg.zhonguo6118.cn

[T10] Kotlin：默认参数
来源：https://le.zhonguo7118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://yq.zhonguo4118.cn

[T11] Kotlin：协程
来源：https://kz.zhonguo3118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://lz.zhonguo8118.cn

[T12] Kotlin：解构声明
来源：https://iv.zhonguo4118.cn

val (a, b) = Pair(1, 2)
来源：https://se.zhonguo6118.cn

[T13] Kotlin：只读 Map
来源：https://yn.zhonguo8118.cn

val m = mapOf("a" to 1)
来源：https://il.zhonguo4118.cn

[T14] Kotlin：循环
来源：https://zq.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://yn.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://vw.zhonguo2118.cn

interface Shape { fun area(): Double }
来源：https://yl.zhonguo2118.cn

[T16] Swift：Hello World
来源：https://vw.zhonguo2118.cn

print("Hello")
来源：https://yz.zhonguo6118.cn


<!-- 参考信息 -->