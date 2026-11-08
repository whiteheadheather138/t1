代发 wailian999

echo "${#arr[@]}"
来源：https://nj.zhonguo8118.cn

[R20] 关联数组（字典）
来源：https://po.zhonguo3118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://xl.zhonguo7118.cn

[R21] 字符串长度
来源：https://pm.zhonguo8118.cn

echo "${#s}"
来源：https://rz.zhonguo6118.cn

[R22] 截取子串
来源：https://ub.zhonguo3118.cn

echo "${s:0:5}"
来源：https://wl.zhonguo3118.cn

[R23] 字符串替换
来源：https://vz.zhonguo7118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://yf.zhonguo5118.cn

[R24] 大小写转换
来源：https://al.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://fm.zhonguo7118.cn

[R25] 去后缀 / 去前缀
来源：https://yz.zhonguo6118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://uf.zhonguo5118.cn

[R26] 命令替换
来源：https://rh.zhonguo7118.cn

now=$(date +%F); echo "$now"
来源：https://jh.zhonguo4118.cn

[R27] 算术展开
来源：https://co.zhonguo4118.cn

echo $((1 + 2 * 3))
来源：https://vt.zhonguo7118.cn

[R28] 浮点运算
来源：https://mn.zhonguo7118.cn

echo "scale=2; 10/3" | bc
来源：https://ab.zhonguo6118.cn

[R29] 定义函数
来源：https://hk.zhonguo5118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://my.zhonguo5118.cn

[R30] 函数返回状态码
来源：https://cp.zhonguo8118.cn

f() { return 0; }; f || echo "失败了"
来源：https://uo.zhonguo2118.cn

[R31] 局部变量
来源：https://wz.zhonguo6118.cn

f() { local x=1; echo "$x"; }
来源：https://og.zhonguo3118.cn

[R32] 参数个数校验
来源：https://og.zhonguo8118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://qm.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://nj.zhonguo5118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://dd.zhonguo3118.cn

[R34] 退出时清理
来源：https://yt.zhonguo1118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://kt.zhonguo7118.cn

[R35] 后台执行并等待
来源：https://qx.zhonguo4118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://sp.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://vi.zhonguo5118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://rf.zhonguo4118.cn

[R37] 把输出赋给变量
来源：https://id.zhonguo5118.cn

files=$(ls -1)
来源：https://nr.zhonguo1118.cn

[R38] 管道串联
来源：https://ef.zhonguo5118.cn

cat a.txt | grep -i error | wc -l
来源：https://ae.zhonguo8118.cn

[R39] 重定向标准输出与错误
来源：https://nh.zhonguo5118.cn

cmd > out.log 2>&1
来源：https://lq.zhonguo8118.cn

[R40] 追加写日志
来源：https://pp.zhonguo7118.cn

echo "log" >> out.log
来源：https://vp.zhonguo8118.cn

[R41] 丢弃输出
来源：https://fl.zhonguo4118.cn

cmd >/dev/null 2>&1
来源：https://mj.zhonguo3118.cn

[R42] 输入重定向
来源：https://cz.zhonguo3118.cn

wc -l < a.txt
来源：https://uy.zhonguo7118.cn

[R43] 按名字查找文件
来源：https://jd.zhonguo4118.cn

find . -name "*.log" -type f
来源：https://su.zhonguo6118.cn

[R44] 按修改时间查找
来源：https://bl.zhonguo2118.cn

find . -mtime -7 -type f
来源：https://jw.zhonguo2118.cn

[R45] 批量删除
来源：https://zs.zhonguo6118.cn

find . -name "*.tmp" -delete
来源：https://tw.zhonguo3118.cn

[R46] 递归替换文件内容
来源：https://ld.zhonguo5118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://od.zhonguo8118.cn

[R47] sed 单行替换
来源：https://rv.zhonguo4118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://fk.zhonguo7118.cn

[R48] awk 取指定列
来源：https://yu.zhonguo5118.cn

awk '{print $1, $3}' a.txt
来源：https://ws.zhonguo4118.cn

[R49] awk 带条件
来源：https://xf.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://je.zhonguo8118.cn

[R50] awk 求和
来源：https://mg.zhonguo7118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://ds.zhonguo8118.cn

[R51] 排序去重取前几
来源：https://gh.zhonguo8118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://ba.zhonguo4118.cn

[R52] 统计行数
来源：https://om.zhonguo7118.cn

wc -l a.txt
来源：https://qc.zhonguo7118.cn

[R53] 查看文件头与实时尾
来源：https://yh.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://ct.zhonguo1118.cn

[R54] 比较两个文件
来源：https://jg.zhonguo7118.cn

diff a.txt b.txt
来源：https://ha.zhonguo7118.cn

[R55] 压缩与解压
来源：https://im.zhonguo4118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://xc.zhonguo3118.cn

[R56] 远程拷贝
来源：https://us.zhonguo8118.cn

scp file user@host:/path/
来源：https://rv.zhonguo6118.cn

[R57] 远程执行命令
来源：https://jw.zhonguo4118.cn

ssh user@host 'uptime'
来源：https://eq.zhonguo1118.cn

[R58] 下载文件
来源：https://jg.zhonguo4118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://pw.zhonguo1118.cn

[R59] 发 POST JSON
来源：https://ur.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://gy.zhonguo7118.cn

[R60] 只看 HTTP 状态码
来源：https://nb.zhonguo7118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://jk.zhonguo6118.cn

[R61] 磁盘占用
来源：https://zx.zhonguo7118.cn

df -h;  du -sh *
来源：https://wi.zhonguo5118.cn

[R62] 找最占空间的文件
来源：https://oa.zhonguo8118.cn

du -ah . | sort -rh | head -10
来源：https://yj.zhonguo1118.cn

[R63] 内存与进程
来源：https://na.zhonguo8118.cn

free -h;  ps aux | grep nginx
来源：https://jo.zhonguo8118.cn

[R64] 结束进程
来源：https://kb.zhonguo8118.cn

kill -9 $(pgrep -f app.py)
来源：https://uf.zhonguo5118.cn

[R65] 查看端口占用
来源：https://mz.zhonguo8118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://md.zhonguo4118.cn

[R66] 定时任务
来源：https://id.zhonguo6118.cn

crontab -e;  crontab -l
来源：https://gv.zhonguo6118.cn

[R67] 生成随机十六进制串
来源：https://uj.zhonguo3118.cn

openssl rand -hex 16
来源：https://nv.zhonguo5118.cn

[R68] 计算文件校验值
来源：https://zf.zhonguo1118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://hz.zhonguo2118.cn

[R69] 生成随机密码
来源：https://ix.zhonguo6118.cn

head -c 16 /dev/urandom | base64
来源：https://qv.zhonguo8118.cn

[R70] 时间戳与互转
来源：https://bl.zhonguo3118.cn

date +%s;  date -d @1700000000
来源：https://oi.zhonguo2118.cn

[R71] 日期格式化
来源：https://ln.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ar.zhonguo4118.cn

[R72] 等待端口就绪
来源：https://uy.zhonguo4118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://kz.zhonguo5118.cn

[R73] 分割大日志
来源：https://sy.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://or.zhonguo8118.cn

[R74] 批量重命名
来源：https://lu.zhonguo7118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://pp.zhonguo6118.cn

[R75] 导出环境变量
来源：https://oa.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://vd.zhonguo3118.cn

[R76] 使用临时文件
来源：https://gs.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://qd.zhonguo6118.cn

[R77] 读取用户输入
来源：https://sk.zhonguo3118.cn

read -rp "请输入: " ans
来源：https://jk.zhonguo6118.cn

[R78] 交互式菜单
来源：https://sh.zhonguo5118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://ty.zhonguo7118.cn

[R79] 解析命令行选项
来源：https://hy.zhonguo3118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://ox.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://qy.zhonguo5118.cn

time ./run.sh
来源：https://xq.zhonguo5118.cn

================================================================================
来源：https://bk.zhonguo6118.cn

S. C / C++ 专题
来源：https://yb.zhonguo7118.cn

================================================================================
来源：https://jm.zhonguo4118.cn

[S01] C：Hello World
来源：https://eo.zhonguo3118.cn

#include <stdio.h>
来源：https://qd.zhonguo5118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://uz.zhonguo4118.cn

[S02] C：变量与格式化输出
来源：https://ss.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://eh.zhonguo6118.cn

[S03] C：读入整数
来源：https://pl.zhonguo2118.cn

int x; scanf("%d", &x);
来源：https://ix.zhonguo4118.cn

[S04] C：字符串复制
来源：https://or.zhonguo3118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://pg.zhonguo7118.cn

[S05] C：字符串长度
来源：https://eh.zhonguo2118.cn

strlen(s)
来源：https://la.zhonguo8118.cn

[S06] C：字符串比较
来源：https://gs.zhonguo7118.cn

strcmp(a, b) == 0
来源：https://si.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://tv.zhonguo7118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://yx.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://du.zhonguo1118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://sy.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://ia.zhonguo7118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://bj.zhonguo1118.cn

[S10] C：指针与解引用
来源：https://xh.zhonguo2118.cn

int *p = &a;  *p = 5;
来源：https://kt.zhonguo6118.cn

[S11] C：逐行读文件
来源：https://qv.zhonguo6118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ft.zhonguo3118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://qh.zhonguo2118.cn

fclose(f);
来源：https://au.zhonguo8118.cn

[S12] C：写文件
来源：https://ed.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://zx.zhonguo5118.cn

[S13] C：宏定义
来源：https://ns.zhonguo3118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://ap.zhonguo7118.cn

[S14] C：枚举
来源：https://vi.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://yd.zhonguo2118.cn

[S15] C：类型转换
来源：https://gi.zhonguo7118.cn

(double) a / b
来源：https://wb.zhonguo1118.cn

[S16] C：位操作置位
来源：https://fm.zhonguo5118.cn

x |= (1 << 3);
来源：https://ya.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://fk.zhonguo6118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://nm.zhonguo3118.cn

[S18] C：命令行参数
来源：https://ti.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://yb.zhonguo7118.cn

[S19] C：快速排序
来源：https://iw.zhonguo1118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://ec.zhonguo4118.cn

[S20] C：二分查找
来源：https://we.zhonguo7118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://vb.zhonguo1118.cn

[S21] C：字符类别判断
来源：https://ym.zhonguo4118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://am.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://hp.zhonguo7118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://fy.zhonguo5118.cn

[S23] C：随机数
来源：https://en.zhonguo1118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://co.zhonguo5118.cn

[S24] C：获取本地时间
来源：https://zt.zhonguo8118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://bx.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://op.zhonguo5118.cn

memcpy(dst, src, n);
来源：https://lo.zhonguo2118.cn

[S26] C：内存清零
来源：https://na.zhonguo4118.cn

memset(a, 0, sizeof a);
来源：https://ar.zhonguo6118.cn

[S27] C：定义常量
来源：https://tn.zhonguo1118.cn

const double PI = 3.14159;
来源：https://xv.zhonguo1118.cn

[S28] C：静态变量
来源：https://wf.zhonguo4118.cn

static int counter = 0;
来源：https://zy.zhonguo8118.cn

[S29] C：变参函数
来源：https://wp.zhonguo1118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://xz.zhonguo4118.cn

[S30] C：头文件保护
来源：https://gm.zhonguo2118.cn

#ifndef X_H
来源：https://nf.zhonguo5118.cn

#define X_H
来源：https://vk.zhonguo2118.cn

#endif
来源：https://vh.zhonguo1118.cn

[S31] C++：Hello World
来源：https://ow.zhonguo2118.cn

#include <iostream>
来源：https://xv.zhonguo4118.cn

int main() { std::cout << "Hello\n"; }
来源：https://jc.zhonguo6118.cn

[S32] C++：字符串
来源：https://pu.zhonguo8118.cn

std::string s = "hi";  s += "!";
来源：https://kq.zhonguo2118.cn

[S33] C++：vector 增删
来源：https://ru.zhonguo4118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://it.zhonguo1118.cn

[S34] C++：遍历 vector
来源：https://sg.zhonguo4118.cn

for (auto &x : v) { std::cout << x; }
来源：https://vt.zhonguo7118.cn

[S35] C++：map
来源：https://ka.zhonguo4118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://es.zhonguo2118.cn

[S36] C++：unordered_map
来源：https://uo.zhonguo8118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://zq.zhonguo7118.cn

[S37] C++：set
来源：https://fs.zhonguo8118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://rh.zhonguo6118.cn

[S38] C++：排序
来源：https://ow.zhonguo4118.cn

std::sort(v.begin(), v.end());
来源：https://ih.zhonguo4118.cn

[S39] C++：自定义比较器排序
来源：https://tf.zhonguo8118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://kz.zhonguo6118.cn

[S40] C++：查找元素
来源：https://xj.zhonguo3118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://bp.zhonguo7118.cn

[S41] C++：类与构造函数
来源：https://xo.zhonguo3118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://vq.zhonguo3118.cn

[S42] C++：继承与虚函数
来源：https://za.zhonguo6118.cn

class B : public Base { public: void f() override {} };
来源：https://jv.zhonguo8118.cn

[S43] C++：智能指针
来源：https://wm.zhonguo6118.cn

auto p = std::make_unique<int>(5);
来源：https://kk.zhonguo1118.cn

[S44] C++：引用传参
来源：https://zb.zhonguo2118.cn

void inc(int &x) { ++x; }
来源：https://af.zhonguo2118.cn

[S45] C++：lambda
来源：https://zi.zhonguo1118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://lp.zhonguo7118.cn

[S46] C++：函数模板
来源：https://sv.zhonguo5118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://uz.zhonguo2118.cn

[S47] C++：结构化绑定遍历
来源：https://xv.zhonguo5118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://bn.zhonguo1118.cn

[S48] C++：逐行读文件
来源：https://zf.zhonguo4118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://af.zhonguo8118.cn

while (std::getline(in, line)) { }
来源：https://ge.zhonguo8118.cn

[S49] C++：写文件
来源：https://mz.zhonguo4118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://pl.zhonguo1118.cn

[S50] C++：格式化数字
来源：https://sv.zhonguo2118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://fh.zhonguo3118.cn

[S51] C++：显式类型转换
来源：https://in.zhonguo7118.cn

static_cast<double>(a) / b
来源：https://ac.zhonguo5118.cn

[S52] C++：const 与 noexcept
来源：https://vw.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://kf.zhonguo4118.cn

[S53] C++：移动语义
来源：https://zd.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://ms.zhonguo6118.cn

[S54] C++：异常处理
来源：https://wx.zhonguo5118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://wh.zhonguo5118.cn

[S55] C++：结构化绑定
来源：https://fx.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://fz.zhonguo6118.cn

[S56] C++：optional
来源：https://vu.zhonguo7118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://gc.zhonguo3118.cn

[S57] C++：编译期常量
来源：https://tp.zhonguo1118.cn

constexpr int N = 10;
来源：https://lv.zhonguo6118.cn

[S58] C++：命名空间
来源：https://yv.zhonguo3118.cn

namespace ns { int f() { return 1; } }
来源：https://ht.zhonguo6118.cn

[S59] C++：静态断言
来源：https://kt.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://me.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://lf.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://le.zhonguo1118.cn

================================================================================
来源：https://dq.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://we.zhonguo8118.cn

================================================================================
来源：https://vn.zhonguo3118.cn

[T01] Kotlin：Hello World
来源：https://dl.zhonguo4118.cn

println("Hello")
来源：https://xr.zhonguo2118.cn

[T02] Kotlin：变量
来源：https://ru.zhonguo1118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://vi.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://sw.zhonguo2118.cn

"值: $b"
来源：https://wm.zhonguo7118.cn

[T04] Kotlin：空安全
来源：https://nx.zhonguo1118.cn

val n: String? = null;  n?.length
来源：https://bo.zhonguo8118.cn

[T05] Kotlin：when 表达式
来源：https://xd.zhonguo8118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://da.zhonguo2118.cn

[T06] Kotlin：集合映射
来源：https://uz.zhonguo2118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://bd.zhonguo3118.cn

[T07] Kotlin：集合过滤
来源：https://gm.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://ri.zhonguo1118.cn

[T08] Kotlin：数据类
来源：https://ok.zhonguo3118.cn

data class User(val name: String, val age: Int)
来源：https://mc.zhonguo5118.cn

[T09] Kotlin：扩展函数
来源：https://oq.zhonguo6118.cn

fun String.exclaim() = this + "!"
来源：https://sh.zhonguo3118.cn

[T10] Kotlin：默认参数
来源：https://ot.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://uv.zhonguo3118.cn

[T11] Kotlin：协程
来源：https://de.zhonguo4118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://xi.zhonguo5118.cn

[T12] Kotlin：解构声明
来源：https://sa.zhonguo3118.cn

val (a, b) = Pair(1, 2)
来源：https://lc.zhonguo6118.cn

[T13] Kotlin：只读 Map
来源：https://fl.zhonguo7118.cn

val m = mapOf("a" to 1)
来源：https://or.zhonguo3118.cn

[T14] Kotlin：循环
来源：https://ln.zhonguo4118.cn

for (i in 1..10) println(i)
来源：https://is.zhonguo3118.cn

[T15] Kotlin：接口
来源：https://yn.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://wa.zhonguo7118.cn

[T16] Swift：Hello World
来源：https://ow.zhonguo3118.cn

print("Hello")
来源：https://cu.zhonguo7118.cn

[T17] Swift：变量与常量
来源：https://mj.zhonguo3118.cn

var a = 1;  let b = 2
来源：https://sy.zhonguo4118.cn

[T18] Swift：字符串插值
来源：https://ox.zhonguo6118.cn

"值: \(b)"
来源：https://pm.zhonguo4118.cn

[T19] Swift：可选绑定
来源：https://cq.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://nc.zhonguo8118.cn

[T20] Swift：数组操作
来源：https://ma.zhonguo3118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://bl.zhonguo2118.cn

[T21] Swift：遍历
来源：https://sk.zhonguo2118.cn

for x in a { print(x) }
来源：https://qt.zhonguo1118.cn

[T22] Swift：字典
来源：https://vy.zhonguo3118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://vv.zhonguo1118.cn


<!-- 参考信息 -->