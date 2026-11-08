代发 wailian999

free -h;  ps aux | grep nginx
来源：https://nf.zhonguo1118.cn

[R64] 结束进程
来源：https://so.zhonguo6118.cn

kill -9 $(pgrep -f app.py)
来源：https://ym.zhonguo1118.cn

[R65] 查看端口占用
来源：https://pj.zhonguo7118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://uj.zhonguo7118.cn

[R66] 定时任务
来源：https://zn.zhonguo7118.cn

crontab -e;  crontab -l
来源：https://pv.zhonguo7118.cn

[R67] 生成随机十六进制串
来源：https://dz.zhonguo3118.cn

openssl rand -hex 16
来源：https://ff.zhonguo3118.cn

[R68] 计算文件校验值
来源：https://am.zhonguo5118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://ve.zhonguo4118.cn

[R69] 生成随机密码
来源：https://im.zhonguo6118.cn

head -c 16 /dev/urandom | base64
来源：https://ah.zhonguo7118.cn

[R70] 时间戳与互转
来源：https://nn.zhonguo7118.cn

date +%s;  date -d @1700000000
来源：https://hz.zhonguo1118.cn

[R71] 日期格式化
来源：https://lm.zhonguo2118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://dj.zhonguo3118.cn

[R72] 等待端口就绪
来源：https://be.zhonguo2118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://cj.zhonguo4118.cn

[R73] 分割大日志
来源：https://pu.zhonguo1118.cn

split -l 1000 big.log part_
来源：https://mt.zhonguo8118.cn

[R74] 批量重命名
来源：https://uj.zhonguo5118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://mq.zhonguo7118.cn

[R75] 导出环境变量
来源：https://bw.zhonguo5118.cn

export PATH="$HOME/bin:$PATH"
来源：https://sr.zhonguo7118.cn

[R76] 使用临时文件
来源：https://rp.zhonguo6118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://tl.zhonguo6118.cn

[R77] 读取用户输入
来源：https://nb.zhonguo7118.cn

read -rp "请输入: " ans
来源：https://rn.zhonguo4118.cn

[R78] 交互式菜单
来源：https://qm.zhonguo1118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://sr.zhonguo6118.cn

[R79] 解析命令行选项
来源：https://xi.zhonguo7118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://ds.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://cu.zhonguo4118.cn

time ./run.sh
来源：https://wo.zhonguo8118.cn

================================================================================
来源：https://nh.zhonguo4118.cn

S. C / C++ 专题
来源：https://ud.zhonguo7118.cn

================================================================================
来源：https://uc.zhonguo6118.cn

[S01] C：Hello World
来源：https://kg.zhonguo4118.cn

#include <stdio.h>
来源：https://yg.zhonguo3118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://wy.zhonguo6118.cn

[S02] C：变量与格式化输出
来源：https://ds.zhonguo2118.cn

int a = 10; printf("%d\n", a);
来源：https://hs.zhonguo7118.cn

[S03] C：读入整数
来源：https://rc.zhonguo2118.cn

int x; scanf("%d", &x);
来源：https://ig.zhonguo2118.cn

[S04] C：字符串复制
来源：https://cj.zhonguo2118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://lr.zhonguo5118.cn

[S05] C：字符串长度
来源：https://hi.zhonguo1118.cn

strlen(s)
来源：https://bw.zhonguo1118.cn

[S06] C：字符串比较
来源：https://at.zhonguo5118.cn

strcmp(a, b) == 0
来源：https://up.zhonguo4118.cn

[S07] C：数组遍历求和
来源：https://oy.zhonguo8118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://jl.zhonguo1118.cn

[S08] C：动态内存分配与释放
来源：https://nw.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://wu.zhonguo5118.cn

[S09] C：结构体定义与初始化
来源：https://ws.zhonguo7118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://sh.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://uv.zhonguo4118.cn

int *p = &a;  *p = 5;
来源：https://jc.zhonguo6118.cn

[S11] C：逐行读文件
来源：https://yc.zhonguo8118.cn

FILE *f = fopen("a.txt", "r");
来源：https://iy.zhonguo3118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ug.zhonguo2118.cn

fclose(f);
来源：https://sy.zhonguo3118.cn

[S12] C：写文件
来源：https://tb.zhonguo5118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://rw.zhonguo7118.cn

[S13] C：宏定义
来源：https://an.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://aj.zhonguo3118.cn

[S14] C：枚举
来源：https://fe.zhonguo4118.cn

enum Color { RED, GREEN, BLUE };
来源：https://tu.zhonguo7118.cn

[S15] C：类型转换
来源：https://fr.zhonguo3118.cn

(double) a / b
来源：https://rq.zhonguo1118.cn

[S16] C：位操作置位
来源：https://eo.zhonguo6118.cn

x |= (1 << 3);
来源：https://ny.zhonguo8118.cn

[S17] C：安全拼接字符串
来源：https://ok.zhonguo3118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://zl.zhonguo4118.cn

[S18] C：命令行参数
来源：https://pb.zhonguo5118.cn

int main(int argc, char **argv)
来源：https://wp.zhonguo1118.cn

[S19] C：快速排序
来源：https://fi.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://pi.zhonguo2118.cn

[S20] C：二分查找
来源：https://iw.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://bw.zhonguo3118.cn

[S21] C：字符类别判断
来源：https://lz.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://vs.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://fa.zhonguo6118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://vu.zhonguo4118.cn

[S23] C：随机数
来源：https://zl.zhonguo8118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://dm.zhonguo5118.cn

[S24] C：获取本地时间
来源：https://zj.zhonguo5118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://qj.zhonguo6118.cn

[S25] C：内存拷贝
来源：https://te.zhonguo8118.cn

memcpy(dst, src, n);
来源：https://wd.zhonguo3118.cn

[S26] C：内存清零
来源：https://hk.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://xk.zhonguo6118.cn

[S27] C：定义常量
来源：https://kv.zhonguo4118.cn

const double PI = 3.14159;
来源：https://qu.zhonguo2118.cn

[S28] C：静态变量
来源：https://yu.zhonguo6118.cn

static int counter = 0;
来源：https://qc.zhonguo6118.cn

[S29] C：变参函数
来源：https://tc.zhonguo3118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://pn.zhonguo1118.cn

[S30] C：头文件保护
来源：https://sv.zhonguo7118.cn

#ifndef X_H
来源：https://rk.zhonguo1118.cn

#define X_H
来源：https://hx.zhonguo6118.cn

#endif
来源：https://oa.zhonguo3118.cn

[S31] C++：Hello World
来源：https://la.zhonguo8118.cn

#include <iostream>
来源：https://bg.zhonguo2118.cn

int main() { std::cout << "Hello\n"; }
来源：https://cc.zhonguo4118.cn

[S32] C++：字符串
来源：https://ok.zhonguo4118.cn

std::string s = "hi";  s += "!";
来源：https://hc.zhonguo3118.cn

[S33] C++：vector 增删
来源：https://qk.zhonguo5118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://ok.zhonguo2118.cn

[S34] C++：遍历 vector
来源：https://cl.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://dr.zhonguo4118.cn

[S35] C++：map
来源：https://lp.zhonguo2118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://hg.zhonguo8118.cn

[S36] C++：unordered_map
来源：https://ht.zhonguo5118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://fx.zhonguo5118.cn

[S37] C++：set
来源：https://on.zhonguo1118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://oz.zhonguo2118.cn

[S38] C++：排序
来源：https://ip.zhonguo1118.cn

std::sort(v.begin(), v.end());
来源：https://dj.zhonguo3118.cn

[S39] C++：自定义比较器排序
来源：https://ji.zhonguo7118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://uy.zhonguo1118.cn

[S40] C++：查找元素
来源：https://pw.zhonguo2118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://nh.zhonguo6118.cn

[S41] C++：类与构造函数
来源：https://wj.zhonguo1118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://vv.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://aj.zhonguo6118.cn

class B : public Base { public: void f() override {} };
来源：https://qy.zhonguo5118.cn

[S43] C++：智能指针
来源：https://bp.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://ht.zhonguo5118.cn

[S44] C++：引用传参
来源：https://ma.zhonguo1118.cn

void inc(int &x) { ++x; }
来源：https://xj.zhonguo5118.cn

[S45] C++：lambda
来源：https://lt.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://wy.zhonguo2118.cn

[S46] C++：函数模板
来源：https://ae.zhonguo5118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://jh.zhonguo7118.cn

[S47] C++：结构化绑定遍历
来源：https://pf.zhonguo7118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://nh.zhonguo2118.cn

[S48] C++：逐行读文件
来源：https://nx.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://et.zhonguo8118.cn

while (std::getline(in, line)) { }
来源：https://rd.zhonguo7118.cn

[S49] C++：写文件
来源：https://ah.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://aw.zhonguo8118.cn

[S50] C++：格式化数字
来源：https://xm.zhonguo1118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://il.zhonguo6118.cn

[S51] C++：显式类型转换
来源：https://wc.zhonguo3118.cn

static_cast<double>(a) / b
来源：https://yv.zhonguo8118.cn

[S52] C++：const 与 noexcept
来源：https://od.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://ar.zhonguo5118.cn

[S53] C++：移动语义
来源：https://ow.zhonguo8118.cn

std::vector<int> w = std::move(v);
来源：https://jh.zhonguo1118.cn

[S54] C++：异常处理
来源：https://ly.zhonguo2118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ul.zhonguo6118.cn

[S55] C++：结构化绑定
来源：https://nn.zhonguo5118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://se.zhonguo5118.cn

[S56] C++：optional
来源：https://ot.zhonguo1118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://wb.zhonguo5118.cn

[S57] C++：编译期常量
来源：https://pb.zhonguo6118.cn

constexpr int N = 10;
来源：https://ta.zhonguo2118.cn

[S58] C++：命名空间
来源：https://zy.zhonguo7118.cn

namespace ns { int f() { return 1; } }
来源：https://yr.zhonguo5118.cn

[S59] C++：静态断言
来源：https://ej.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://yo.zhonguo2118.cn

[S60] C++：遍历并删除元素
来源：https://xm.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://ac.zhonguo4118.cn

================================================================================
来源：https://mi.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://bf.zhonguo7118.cn

================================================================================
来源：https://bd.zhonguo8118.cn

[T01] Kotlin：Hello World
来源：https://st.zhonguo1118.cn

println("Hello")
来源：https://qs.zhonguo4118.cn

[T02] Kotlin：变量
来源：https://cj.zhonguo1118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://uk.zhonguo7118.cn

[T03] Kotlin：字符串模板
来源：https://lw.zhonguo4118.cn

"值: $b"
来源：https://es.zhonguo6118.cn

[T04] Kotlin：空安全
来源：https://zn.zhonguo6118.cn

val n: String? = null;  n?.length
来源：https://co.zhonguo6118.cn

[T05] Kotlin：when 表达式
来源：https://yg.zhonguo2118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://ff.zhonguo2118.cn

[T06] Kotlin：集合映射
来源：https://yi.zhonguo7118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://nc.zhonguo5118.cn

[T07] Kotlin：集合过滤
来源：https://gc.zhonguo2118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://zs.zhonguo7118.cn

[T08] Kotlin：数据类
来源：https://xn.zhonguo5118.cn

data class User(val name: String, val age: Int)
来源：https://yh.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://cu.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://sq.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://sj.zhonguo5118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://fd.zhonguo1118.cn

[T11] Kotlin：协程
来源：https://wq.zhonguo3118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://es.zhonguo4118.cn

[T12] Kotlin：解构声明
来源：https://of.zhonguo1118.cn

val (a, b) = Pair(1, 2)
来源：https://cx.zhonguo4118.cn

[T13] Kotlin：只读 Map
来源：https://nd.zhonguo3118.cn

val m = mapOf("a" to 1)
来源：https://gz.zhonguo2118.cn

[T14] Kotlin：循环
来源：https://vc.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://pw.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://ev.zhonguo5118.cn

interface Shape { fun area(): Double }
来源：https://hj.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://lx.zhonguo6118.cn

print("Hello")
来源：https://za.zhonguo8118.cn

[T17] Swift：变量与常量
来源：https://jh.zhonguo7118.cn

var a = 1;  let b = 2
来源：https://mv.zhonguo4118.cn

[T18] Swift：字符串插值
来源：https://wq.zhonguo1118.cn

"值: \(b)"
来源：https://gk.zhonguo1118.cn

[T19] Swift：可选绑定
来源：https://re.zhonguo1118.cn

if let n = opt { print(n) }
来源：https://hc.zhonguo4118.cn

[T20] Swift：数组操作
来源：https://yh.zhonguo6118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://ef.zhonguo1118.cn

[T21] Swift：遍历
来源：https://eo.zhonguo3118.cn

for x in a { print(x) }
来源：https://zu.zhonguo6118.cn

[T22] Swift：字典
来源：https://nz.zhonguo8118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://om.zhonguo7118.cn

[T23] Swift：函数
来源：https://tm.zhonguo2118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://rs.zhonguo3118.cn

[T24] Swift：闭包
来源：https://br.zhonguo2118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://wx.zhonguo7118.cn

[T25] Swift：结构体
来源：https://wq.zhonguo2118.cn

struct P { var x: Int }
来源：https://xr.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://ro.zhonguo6118.cn

class A: Base { override func f() {} }
来源：https://mb.zhonguo1118.cn

[T27] Swift：错误处理
来源：https://tw.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://px.zhonguo8118.cn

[T28] Swift：枚举
来源：https://uj.zhonguo7118.cn

enum Color { case red, green }
来源：https://ct.zhonguo5118.cn

[T29] Swift：guard 提前返回
来源：https://vd.zhonguo2118.cn

guard let x = opt else { return }
来源：https://jt.zhonguo7118.cn

[T30] Swift：协议
来源：https://sc.zhonguo1118.cn

protocol Shape { func area() -> Double }
来源：https://ti.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://mg.zhonguo7118.cn

print("Hello")
来源：https://wf.zhonguo1118.cn

[T32] Lua：局部变量
来源：https://az.zhonguo5118.cn

local a = 1
来源：https://is.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://gc.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://jm.zhonguo8118.cn

[T34] Lua：遍历表
来源：https://gp.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://nz.zhonguo3118.cn

[T35] Lua：字典表
来源：https://ct.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://fp.zhonguo4118.cn

[T36] Lua：函数
来源：https://hz.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://pr.zhonguo5118.cn

[T37] Lua：字符串拼接
来源：https://iv.zhonguo6118.cn

"a" .. "b"
来源：https://nf.zhonguo7118.cn

[T38] Lua：条件
来源：https://iw.zhonguo4118.cn

if x > 0 then print("正") end
来源：https://sg.zhonguo1118.cn

[T39] Lua：模式匹配
来源：https://qi.zhonguo4118.cn

string.find(s, "%d+")
来源：https://sy.zhonguo3118.cn

[T40] Lua：元表
来源：https://gr.zhonguo3118.cn

setmetatable({}, { __index = base })
来源：https://aa.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://cn.zhonguo7118.cn

print "Hello\n";
来源：https://js.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://el.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://bi.zhonguo4118.cn

[T43] Perl：字符串插值
来源：https://ot.zhonguo4118.cn

"值: $a"
来源：https://yt.zhonguo6118.cn

[T44] Perl：条件
来源：https://ou.zhonguo7118.cn

if ($a > 0) { print "正"; }
来源：https://ae.zhonguo4118.cn

[T45] Perl：数组遍历
来源：https://ey.zhonguo5118.cn

for my $x (@arr) { print $x; }
来源：https://wr.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://er.zhonguo2118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://xp.zhonguo2118.cn

[T47] Perl：正则捕获
来源：https://ft.zhonguo8118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://hk.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://vj.zhonguo2118.cn

$s =~ s/old/new/g;
来源：https://be.zhonguo4118.cn

[T49] Perl：函数
来源：https://ap.zhonguo8118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://tg.zhonguo5118.cn

[T50] Perl：逐行读文件
来源：https://zt.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://ph.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://cq.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://as.zhonguo5118.cn

println("Hello")
来源：https://uu.zhonguo3118.cn

[T52] Scala：变量
来源：https://ox.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://jm.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://il.zhonguo4118.cn

s"值: $b"
来源：https://ly.zhonguo1118.cn

[T54] Scala：集合映射
来源：https://rg.zhonguo7118.cn

List(1, 2, 3).map(_ * 2)
来源：https://wm.zhonguo4118.cn

[T55] Scala：集合过滤
来源：https://hl.zhonguo4118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://in.zhonguo3118.cn

[T56] Scala：样例类
来源：https://mb.zhonguo3118.cn

case class User(name: String, age: Int)
来源：https://jj.zhonguo6118.cn

[T57] Scala：模式匹配
来源：https://jb.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://md.zhonguo7118.cn

[T58] Scala：函数定义
来源：https://sb.zhonguo3118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ys.zhonguo2118.cn

[T59] Scala：循环
来源：https://sz.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://wu.zhonguo5118.cn

[T60] Scala：折叠
来源：https://qq.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://cz.zhonguo5118.cn

================================================================================
来源：https://dw.zhonguo5118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://di.zhonguo6118.cn

================================================================================
来源：https://gl.zhonguo1118.cn

[U01] Py：创建虚拟环境
来源：https://fp.zhonguo7118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://iz.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://xv.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://vi.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://pg.zhonguo1118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://xx.zhonguo6118.cn

[U04] Py：变量调试打印
来源：https://jy.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://tz.zhonguo1118.cn


<!-- 参考信息 -->