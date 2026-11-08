代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://wt.zhonguo6118.cn

[R60] 只看 HTTP 状态码
来源：https://zz.zhonguo6118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://cp.zhonguo7118.cn

[R61] 磁盘占用
来源：https://fw.zhonguo6118.cn

df -h;  du -sh *
来源：https://ur.zhonguo4118.cn

[R62] 找最占空间的文件
来源：https://kz.zhonguo2118.cn

du -ah . | sort -rh | head -10
来源：https://zd.zhonguo5118.cn

[R63] 内存与进程
来源：https://ra.zhonguo8118.cn

free -h;  ps aux | grep nginx
来源：https://yk.zhonguo8118.cn

[R64] 结束进程
来源：https://sk.zhonguo2118.cn

kill -9 $(pgrep -f app.py)
来源：https://qx.zhonguo4118.cn

[R65] 查看端口占用
来源：https://kh.zhonguo2118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://nh.zhonguo8118.cn

[R66] 定时任务
来源：https://av.zhonguo5118.cn

crontab -e;  crontab -l
来源：https://mc.zhonguo2118.cn

[R67] 生成随机十六进制串
来源：https://px.zhonguo4118.cn

openssl rand -hex 16
来源：https://mw.zhonguo4118.cn

[R68] 计算文件校验值
来源：https://ql.zhonguo2118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://tk.zhonguo1118.cn

[R69] 生成随机密码
来源：https://eo.zhonguo7118.cn

head -c 16 /dev/urandom | base64
来源：https://ic.zhonguo8118.cn

[R70] 时间戳与互转
来源：https://jn.zhonguo8118.cn

date +%s;  date -d @1700000000
来源：https://yz.zhonguo8118.cn

[R71] 日期格式化
来源：https://oh.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://vu.zhonguo5118.cn

[R72] 等待端口就绪
来源：https://cs.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://du.zhonguo3118.cn

[R73] 分割大日志
来源：https://ut.zhonguo3118.cn

split -l 1000 big.log part_
来源：https://iz.zhonguo3118.cn

[R74] 批量重命名
来源：https://tf.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://rm.zhonguo6118.cn

[R75] 导出环境变量
来源：https://qb.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://tg.zhonguo4118.cn

[R76] 使用临时文件
来源：https://er.zhonguo1118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://qq.zhonguo4118.cn

[R77] 读取用户输入
来源：https://cx.zhonguo3118.cn

read -rp "请输入: " ans
来源：https://lp.zhonguo1118.cn

[R78] 交互式菜单
来源：https://em.zhonguo6118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://hl.zhonguo8118.cn

[R79] 解析命令行选项
来源：https://xk.zhonguo5118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://vz.zhonguo6118.cn

[R80] 查看脚本执行耗时
来源：https://ba.zhonguo5118.cn

time ./run.sh
来源：https://zx.zhonguo5118.cn

================================================================================
来源：https://xl.zhonguo5118.cn

S. C / C++ 专题
来源：https://mp.zhonguo1118.cn

================================================================================
来源：https://ps.zhonguo1118.cn

[S01] C：Hello World
来源：https://ba.zhonguo1118.cn

#include <stdio.h>
来源：https://sf.zhonguo2118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://ch.zhonguo4118.cn

[S02] C：变量与格式化输出
来源：https://vo.zhonguo7118.cn

int a = 10; printf("%d\n", a);
来源：https://qm.zhonguo7118.cn

[S03] C：读入整数
来源：https://jw.zhonguo1118.cn

int x; scanf("%d", &x);
来源：https://jf.zhonguo4118.cn

[S04] C：字符串复制
来源：https://ua.zhonguo7118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://kb.zhonguo5118.cn

[S05] C：字符串长度
来源：https://cv.zhonguo7118.cn

strlen(s)
来源：https://ot.zhonguo8118.cn

[S06] C：字符串比较
来源：https://nq.zhonguo2118.cn

strcmp(a, b) == 0
来源：https://df.zhonguo1118.cn

[S07] C：数组遍历求和
来源：https://tq.zhonguo3118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://ur.zhonguo7118.cn

[S08] C：动态内存分配与释放
来源：https://gk.zhonguo4118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://ka.zhonguo4118.cn

[S09] C：结构体定义与初始化
来源：https://ga.zhonguo8118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://yg.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://ow.zhonguo1118.cn

int *p = &a;  *p = 5;
来源：https://kd.zhonguo6118.cn

[S11] C：逐行读文件
来源：https://ss.zhonguo2118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ou.zhonguo2118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://rt.zhonguo7118.cn

fclose(f);
来源：https://jo.zhonguo1118.cn

[S12] C：写文件
来源：https://qi.zhonguo4118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://jn.zhonguo6118.cn

[S13] C：宏定义
来源：https://au.zhonguo7118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://dy.zhonguo2118.cn

[S14] C：枚举
来源：https://op.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ma.zhonguo2118.cn

[S15] C：类型转换
来源：https://el.zhonguo2118.cn

(double) a / b
来源：https://by.zhonguo2118.cn

[S16] C：位操作置位
来源：https://cf.zhonguo3118.cn

x |= (1 << 3);
来源：https://bd.zhonguo6118.cn

[S17] C：安全拼接字符串
来源：https://pj.zhonguo3118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ah.zhonguo3118.cn

[S18] C：命令行参数
来源：https://fd.zhonguo5118.cn

int main(int argc, char **argv)
来源：https://yd.zhonguo6118.cn

[S19] C：快速排序
来源：https://ac.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://ot.zhonguo1118.cn

[S20] C：二分查找
来源：https://df.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://hc.zhonguo3118.cn

[S21] C：字符类别判断
来源：https://iq.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://kv.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://fc.zhonguo3118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://dl.zhonguo6118.cn

[S23] C：随机数
来源：https://jy.zhonguo7118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ua.zhonguo4118.cn

[S24] C：获取本地时间
来源：https://rd.zhonguo2118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://fp.zhonguo4118.cn

[S25] C：内存拷贝
来源：https://wk.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://sz.zhonguo2118.cn

[S26] C：内存清零
来源：https://zk.zhonguo8118.cn

memset(a, 0, sizeof a);
来源：https://fr.zhonguo3118.cn

[S27] C：定义常量
来源：https://rj.zhonguo1118.cn

const double PI = 3.14159;
来源：https://pj.zhonguo5118.cn

[S28] C：静态变量
来源：https://ef.zhonguo3118.cn

static int counter = 0;
来源：https://ia.zhonguo1118.cn

[S29] C：变参函数
来源：https://so.zhonguo2118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://kg.zhonguo4118.cn

[S30] C：头文件保护
来源：https://zc.zhonguo4118.cn

#ifndef X_H
来源：https://ik.zhonguo1118.cn

#define X_H
来源：https://ye.zhonguo8118.cn

#endif
来源：https://uq.zhonguo2118.cn

[S31] C++：Hello World
来源：https://kv.zhonguo3118.cn

#include <iostream>
来源：https://dm.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://qg.zhonguo1118.cn

[S32] C++：字符串
来源：https://ly.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://wj.zhonguo8118.cn

[S33] C++：vector 增删
来源：https://yy.zhonguo3118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://ho.zhonguo5118.cn

[S34] C++：遍历 vector
来源：https://es.zhonguo1118.cn

for (auto &x : v) { std::cout << x; }
来源：https://zs.zhonguo5118.cn

[S35] C++：map
来源：https://qu.zhonguo7118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://vf.zhonguo4118.cn

[S36] C++：unordered_map
来源：https://kx.zhonguo7118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://al.zhonguo5118.cn

[S37] C++：set
来源：https://ar.zhonguo1118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://fu.zhonguo1118.cn

[S38] C++：排序
来源：https://pm.zhonguo2118.cn

std::sort(v.begin(), v.end());
来源：https://kp.zhonguo6118.cn

[S39] C++：自定义比较器排序
来源：https://dx.zhonguo7118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://pn.zhonguo6118.cn

[S40] C++：查找元素
来源：https://ab.zhonguo1118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://mc.zhonguo3118.cn

[S41] C++：类与构造函数
来源：https://iv.zhonguo1118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://tl.zhonguo1118.cn

[S42] C++：继承与虚函数
来源：https://ry.zhonguo6118.cn

class B : public Base { public: void f() override {} };
来源：https://zj.zhonguo1118.cn

[S43] C++：智能指针
来源：https://xc.zhonguo4118.cn

auto p = std::make_unique<int>(5);
来源：https://zh.zhonguo6118.cn

[S44] C++：引用传参
来源：https://mj.zhonguo2118.cn

void inc(int &x) { ++x; }
来源：https://km.zhonguo8118.cn

[S45] C++：lambda
来源：https://xi.zhonguo5118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://in.zhonguo3118.cn

[S46] C++：函数模板
来源：https://xj.zhonguo6118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://gv.zhonguo2118.cn

[S47] C++：结构化绑定遍历
来源：https://bq.zhonguo1118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://zd.zhonguo1118.cn

[S48] C++：逐行读文件
来源：https://nh.zhonguo1118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://iv.zhonguo4118.cn

while (std::getline(in, line)) { }
来源：https://th.zhonguo4118.cn

[S49] C++：写文件
来源：https://rl.zhonguo6118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://yb.zhonguo1118.cn

[S50] C++：格式化数字
来源：https://vb.zhonguo4118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://gj.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://ny.zhonguo4118.cn

static_cast<double>(a) / b
来源：https://ek.zhonguo2118.cn

[S52] C++：const 与 noexcept
来源：https://iu.zhonguo5118.cn

int size() const noexcept { return n_; }
来源：https://iu.zhonguo5118.cn

[S53] C++：移动语义
来源：https://wm.zhonguo6118.cn

std::vector<int> w = std::move(v);
来源：https://la.zhonguo7118.cn

[S54] C++：异常处理
来源：https://nn.zhonguo4118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://hk.zhonguo3118.cn

[S55] C++：结构化绑定
来源：https://ju.zhonguo4118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://te.zhonguo7118.cn

[S56] C++：optional
来源：https://ca.zhonguo2118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://jy.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://jf.zhonguo4118.cn

constexpr int N = 10;
来源：https://mq.zhonguo5118.cn

[S58] C++：命名空间
来源：https://hv.zhonguo8118.cn

namespace ns { int f() { return 1; } }
来源：https://lj.zhonguo3118.cn

[S59] C++：静态断言
来源：https://hs.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://mk.zhonguo8118.cn

[S60] C++：遍历并删除元素
来源：https://sv.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://zs.zhonguo8118.cn

================================================================================
来源：https://fw.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://dh.zhonguo1118.cn

================================================================================
来源：https://dk.zhonguo7118.cn

[T01] Kotlin：Hello World
来源：https://eo.zhonguo1118.cn

println("Hello")
来源：https://we.zhonguo4118.cn

[T02] Kotlin：变量
来源：https://mv.zhonguo7118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://ma.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://ga.zhonguo1118.cn

"值: $b"
来源：https://un.zhonguo7118.cn

[T04] Kotlin：空安全
来源：https://qb.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://cp.zhonguo2118.cn

[T05] Kotlin：when 表达式
来源：https://zg.zhonguo6118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://oz.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://eq.zhonguo2118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://wt.zhonguo1118.cn

[T07] Kotlin：集合过滤
来源：https://lw.zhonguo1118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://uj.zhonguo8118.cn

[T08] Kotlin：数据类
来源：https://vq.zhonguo3118.cn

data class User(val name: String, val age: Int)
来源：https://yi.zhonguo6118.cn

[T09] Kotlin：扩展函数
来源：https://ai.zhonguo1118.cn

fun String.exclaim() = this + "!"
来源：https://sb.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://gm.zhonguo4118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://nc.zhonguo2118.cn

[T11] Kotlin：协程
来源：https://xb.zhonguo7118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://om.zhonguo1118.cn

[T12] Kotlin：解构声明
来源：https://ed.zhonguo2118.cn

val (a, b) = Pair(1, 2)
来源：https://et.zhonguo6118.cn

[T13] Kotlin：只读 Map
来源：https://hm.zhonguo4118.cn

val m = mapOf("a" to 1)
来源：https://mr.zhonguo8118.cn

[T14] Kotlin：循环
来源：https://am.zhonguo2118.cn

for (i in 1..10) println(i)
来源：https://bt.zhonguo5118.cn

[T15] Kotlin：接口
来源：https://io.zhonguo5118.cn

interface Shape { fun area(): Double }
来源：https://qf.zhonguo7118.cn

[T16] Swift：Hello World
来源：https://ox.zhonguo7118.cn

print("Hello")
来源：https://st.zhonguo7118.cn

[T17] Swift：变量与常量
来源：https://jk.zhonguo7118.cn

var a = 1;  let b = 2
来源：https://lr.zhonguo5118.cn

[T18] Swift：字符串插值
来源：https://ax.zhonguo7118.cn

"值: \(b)"
来源：https://vw.zhonguo4118.cn

[T19] Swift：可选绑定
来源：https://pr.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://xs.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://hb.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://qf.zhonguo4118.cn

[T21] Swift：遍历
来源：https://hu.zhonguo3118.cn

for x in a { print(x) }
来源：https://ud.zhonguo3118.cn

[T22] Swift：字典
来源：https://ve.zhonguo6118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://ky.zhonguo5118.cn

[T23] Swift：函数
来源：https://vq.zhonguo6118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://ud.zhonguo7118.cn

[T24] Swift：闭包
来源：https://wj.zhonguo1118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://mc.zhonguo8118.cn

[T25] Swift：结构体
来源：https://hu.zhonguo2118.cn

struct P { var x: Int }
来源：https://ju.zhonguo6118.cn

[T26] Swift：类与重写
来源：https://nk.zhonguo4118.cn

class A: Base { override func f() {} }
来源：https://zi.zhonguo5118.cn

[T27] Swift：错误处理
来源：https://qy.zhonguo8118.cn

do { try f() } catch { print(error) }
来源：https://cu.zhonguo3118.cn

[T28] Swift：枚举
来源：https://ww.zhonguo7118.cn

enum Color { case red, green }
来源：https://ka.zhonguo7118.cn

[T29] Swift：guard 提前返回
来源：https://ur.zhonguo4118.cn

guard let x = opt else { return }
来源：https://cx.zhonguo6118.cn

[T30] Swift：协议
来源：https://dt.zhonguo1118.cn

protocol Shape { func area() -> Double }
来源：https://kc.zhonguo2118.cn

[T31] Lua：Hello World
来源：https://wl.zhonguo3118.cn

print("Hello")
来源：https://ww.zhonguo2118.cn

[T32] Lua：局部变量
来源：https://wy.zhonguo4118.cn

local a = 1
来源：https://cs.zhonguo4118.cn

[T33] Lua：表（数组）
来源：https://oy.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://gh.zhonguo8118.cn

[T34] Lua：遍历表
来源：https://is.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://xy.zhonguo3118.cn

[T35] Lua：字典表
来源：https://rz.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://gl.zhonguo8118.cn

[T36] Lua：函数
来源：https://qo.zhonguo5118.cn

function add(a, b) return a + b end
来源：https://od.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://jw.zhonguo1118.cn

"a" .. "b"
来源：https://xr.zhonguo1118.cn

[T38] Lua：条件
来源：https://vu.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://tg.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://mi.zhonguo1118.cn

string.find(s, "%d+")
来源：https://vn.zhonguo8118.cn

[T40] Lua：元表
来源：https://ku.zhonguo8118.cn

setmetatable({}, { __index = base })
来源：https://uh.zhonguo3118.cn

[T41] Perl：Hello World
来源：https://fx.zhonguo4118.cn

print "Hello\n";
来源：https://yi.zhonguo3118.cn

[T42] Perl：变量类型
来源：https://rl.zhonguo5118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://bu.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://cg.zhonguo8118.cn

"值: $a"
来源：https://hv.zhonguo1118.cn

[T44] Perl：条件
来源：https://pe.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://zc.zhonguo2118.cn

[T45] Perl：数组遍历
来源：https://ir.zhonguo5118.cn

for my $x (@arr) { print $x; }
来源：https://sl.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://xx.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://kn.zhonguo1118.cn

[T47] Perl：正则捕获
来源：https://xx.zhonguo3118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://cl.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://fe.zhonguo4118.cn

$s =~ s/old/new/g;
来源：https://sf.zhonguo1118.cn

[T49] Perl：函数
来源：https://nn.zhonguo8118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://kq.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://vx.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://dg.zhonguo5118.cn

while (my $line = <$fh>) { print $line; }
来源：https://cn.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://yp.zhonguo8118.cn

println("Hello")
来源：https://ao.zhonguo1118.cn

[T52] Scala：变量
来源：https://sp.zhonguo5118.cn

val a = 1;  var b = 2
来源：https://uy.zhonguo6118.cn

[T53] Scala：字符串插值
来源：https://up.zhonguo1118.cn

s"值: $b"
来源：https://ch.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://fx.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://zc.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://ci.zhonguo4118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://tx.zhonguo8118.cn

[T56] Scala：样例类
来源：https://iy.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://td.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://vt.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://cd.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://tz.zhonguo8118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ca.zhonguo3118.cn

[T59] Scala：循环
来源：https://ss.zhonguo4118.cn

for (i <- 1 to 10) println(i)
来源：https://fq.zhonguo1118.cn

[T60] Scala：折叠
来源：https://ow.zhonguo6118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://hy.zhonguo4118.cn

================================================================================
来源：https://vr.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://rf.zhonguo6118.cn

================================================================================
来源：https://ou.zhonguo2118.cn


<!-- 参考信息 -->