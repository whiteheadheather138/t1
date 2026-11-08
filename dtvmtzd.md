代发 wailian999

ssh user@host 'uptime'
来源：https://rc.zhonguo8118.cn

[R58] 下载文件
来源：https://xr.zhonguo8118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://tl.zhonguo3118.cn

[R59] 发 POST JSON
来源：https://vh.zhonguo5118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://ut.zhonguo3118.cn

[R60] 只看 HTTP 状态码
来源：https://yz.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://so.zhonguo4118.cn

[R61] 磁盘占用
来源：https://an.zhonguo8118.cn

df -h;  du -sh *
来源：https://be.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://gn.zhonguo5118.cn

du -ah . | sort -rh | head -10
来源：https://fj.zhonguo8118.cn

[R63] 内存与进程
来源：https://vd.zhonguo6118.cn

free -h;  ps aux | grep nginx
来源：https://ma.zhonguo8118.cn

[R64] 结束进程
来源：https://wl.zhonguo2118.cn

kill -9 $(pgrep -f app.py)
来源：https://bx.zhonguo5118.cn

[R65] 查看端口占用
来源：https://ba.zhonguo5118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://js.zhonguo8118.cn

[R66] 定时任务
来源：https://nx.zhonguo8118.cn

crontab -e;  crontab -l
来源：https://yx.zhonguo1118.cn

[R67] 生成随机十六进制串
来源：https://gb.zhonguo4118.cn

openssl rand -hex 16
来源：https://zt.zhonguo5118.cn

[R68] 计算文件校验值
来源：https://jq.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://xw.zhonguo6118.cn

[R69] 生成随机密码
来源：https://gw.zhonguo6118.cn

head -c 16 /dev/urandom | base64
来源：https://am.zhonguo2118.cn

[R70] 时间戳与互转
来源：https://hx.zhonguo5118.cn

date +%s;  date -d @1700000000
来源：https://iw.zhonguo3118.cn

[R71] 日期格式化
来源：https://rx.zhonguo5118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://yw.zhonguo4118.cn

[R72] 等待端口就绪
来源：https://yf.zhonguo3118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://wb.zhonguo3118.cn

[R73] 分割大日志
来源：https://tg.zhonguo3118.cn

split -l 1000 big.log part_
来源：https://xm.zhonguo7118.cn

[R74] 批量重命名
来源：https://oz.zhonguo1118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://fd.zhonguo7118.cn

[R75] 导出环境变量
来源：https://qp.zhonguo5118.cn

export PATH="$HOME/bin:$PATH"
来源：https://yz.zhonguo7118.cn

[R76] 使用临时文件
来源：https://cb.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://us.zhonguo1118.cn

[R77] 读取用户输入
来源：https://nq.zhonguo2118.cn

read -rp "请输入: " ans
来源：https://hr.zhonguo5118.cn

[R78] 交互式菜单
来源：https://uc.zhonguo8118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://dc.zhonguo7118.cn

[R79] 解析命令行选项
来源：https://ru.zhonguo6118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://fj.zhonguo1118.cn

[R80] 查看脚本执行耗时
来源：https://sq.zhonguo1118.cn

time ./run.sh
来源：https://sp.zhonguo5118.cn

================================================================================
来源：https://fa.zhonguo7118.cn

S. C / C++ 专题
来源：https://df.zhonguo3118.cn

================================================================================
来源：https://xg.zhonguo2118.cn

[S01] C：Hello World
来源：https://ps.zhonguo2118.cn

#include <stdio.h>
来源：https://rm.zhonguo7118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://lc.zhonguo8118.cn

[S02] C：变量与格式化输出
来源：https://dz.zhonguo7118.cn

int a = 10; printf("%d\n", a);
来源：https://iq.zhonguo8118.cn

[S03] C：读入整数
来源：https://np.zhonguo5118.cn

int x; scanf("%d", &x);
来源：https://rs.zhonguo3118.cn

[S04] C：字符串复制
来源：https://fj.zhonguo6118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://or.zhonguo2118.cn

[S05] C：字符串长度
来源：https://gb.zhonguo3118.cn

strlen(s)
来源：https://sk.zhonguo3118.cn

[S06] C：字符串比较
来源：https://xa.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://mo.zhonguo4118.cn

[S07] C：数组遍历求和
来源：https://ci.zhonguo5118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://on.zhonguo1118.cn

[S08] C：动态内存分配与释放
来源：https://qt.zhonguo4118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://yp.zhonguo3118.cn

[S09] C：结构体定义与初始化
来源：https://xb.zhonguo4118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://xf.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://im.zhonguo2118.cn

int *p = &a;  *p = 5;
来源：https://md.zhonguo8118.cn

[S11] C：逐行读文件
来源：https://en.zhonguo5118.cn

FILE *f = fopen("a.txt", "r");
来源：https://jl.zhonguo4118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ps.zhonguo5118.cn

fclose(f);
来源：https://px.zhonguo1118.cn

[S12] C：写文件
来源：https://tw.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://jd.zhonguo8118.cn

[S13] C：宏定义
来源：https://mc.zhonguo7118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://xq.zhonguo4118.cn

[S14] C：枚举
来源：https://ig.zhonguo2118.cn

enum Color { RED, GREEN, BLUE };
来源：https://rz.zhonguo6118.cn

[S15] C：类型转换
来源：https://ci.zhonguo2118.cn

(double) a / b
来源：https://ci.zhonguo5118.cn

[S16] C：位操作置位
来源：https://yu.zhonguo1118.cn

x |= (1 << 3);
来源：https://ij.zhonguo3118.cn

[S17] C：安全拼接字符串
来源：https://jq.zhonguo2118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ts.zhonguo5118.cn

[S18] C：命令行参数
来源：https://yc.zhonguo4118.cn

int main(int argc, char **argv)
来源：https://ei.zhonguo5118.cn

[S19] C：快速排序
来源：https://bf.zhonguo4118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://ue.zhonguo7118.cn

[S20] C：二分查找
来源：https://em.zhonguo2118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://gg.zhonguo2118.cn

[S21] C：字符类别判断
来源：https://ys.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://jf.zhonguo2118.cn

[S22] C：字符串转数字
来源：https://pe.zhonguo5118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://je.zhonguo5118.cn

[S23] C：随机数
来源：https://gg.zhonguo4118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ba.zhonguo3118.cn

[S24] C：获取本地时间
来源：https://pu.zhonguo2118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://hb.zhonguo4118.cn

[S25] C：内存拷贝
来源：https://pf.zhonguo8118.cn

memcpy(dst, src, n);
来源：https://kf.zhonguo2118.cn

[S26] C：内存清零
来源：https://ic.zhonguo5118.cn

memset(a, 0, sizeof a);
来源：https://pa.zhonguo6118.cn

[S27] C：定义常量
来源：https://pv.zhonguo4118.cn

const double PI = 3.14159;
来源：https://qn.zhonguo2118.cn

[S28] C：静态变量
来源：https://kq.zhonguo6118.cn

static int counter = 0;
来源：https://pw.zhonguo5118.cn

[S29] C：变参函数
来源：https://zx.zhonguo1118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://dm.zhonguo6118.cn

[S30] C：头文件保护
来源：https://zw.zhonguo8118.cn

#ifndef X_H
来源：https://en.zhonguo2118.cn

#define X_H
来源：https://an.zhonguo2118.cn

#endif
来源：https://tj.zhonguo2118.cn

[S31] C++：Hello World
来源：https://in.zhonguo1118.cn

#include <iostream>
来源：https://fz.zhonguo4118.cn

int main() { std::cout << "Hello\n"; }
来源：https://qv.zhonguo8118.cn

[S32] C++：字符串
来源：https://qo.zhonguo8118.cn

std::string s = "hi";  s += "!";
来源：https://xf.zhonguo5118.cn

[S33] C++：vector 增删
来源：https://qb.zhonguo7118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://bc.zhonguo6118.cn

[S34] C++：遍历 vector
来源：https://ft.zhonguo3118.cn

for (auto &x : v) { std::cout << x; }
来源：https://tu.zhonguo3118.cn

[S35] C++：map
来源：https://jz.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://od.zhonguo4118.cn

[S36] C++：unordered_map
来源：https://eo.zhonguo5118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://yw.zhonguo3118.cn

[S37] C++：set
来源：https://hv.zhonguo6118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://yc.zhonguo5118.cn

[S38] C++：排序
来源：https://bo.zhonguo3118.cn

std::sort(v.begin(), v.end());
来源：https://eq.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://uz.zhonguo8118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://xz.zhonguo3118.cn

[S40] C++：查找元素
来源：https://zs.zhonguo4118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://si.zhonguo6118.cn

[S41] C++：类与构造函数
来源：https://yn.zhonguo8118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://hc.zhonguo3118.cn

[S42] C++：继承与虚函数
来源：https://et.zhonguo4118.cn

class B : public Base { public: void f() override {} };
来源：https://df.zhonguo3118.cn

[S43] C++：智能指针
来源：https://xc.zhonguo5118.cn

auto p = std::make_unique<int>(5);
来源：https://zq.zhonguo8118.cn

[S44] C++：引用传参
来源：https://bs.zhonguo6118.cn

void inc(int &x) { ++x; }
来源：https://ar.zhonguo5118.cn

[S45] C++：lambda
来源：https://dq.zhonguo3118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://eg.zhonguo6118.cn

[S46] C++：函数模板
来源：https://wr.zhonguo6118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://yg.zhonguo4118.cn

[S47] C++：结构化绑定遍历
来源：https://ej.zhonguo7118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://ls.zhonguo4118.cn

[S48] C++：逐行读文件
来源：https://lb.zhonguo6118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://vv.zhonguo5118.cn

while (std::getline(in, line)) { }
来源：https://iq.zhonguo1118.cn

[S49] C++：写文件
来源：https://hd.zhonguo5118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://kr.zhonguo2118.cn

[S50] C++：格式化数字
来源：https://mi.zhonguo1118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://pg.zhonguo7118.cn

[S51] C++：显式类型转换
来源：https://rj.zhonguo2118.cn

static_cast<double>(a) / b
来源：https://dq.zhonguo5118.cn

[S52] C++：const 与 noexcept
来源：https://id.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://mi.zhonguo3118.cn

[S53] C++：移动语义
来源：https://xf.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://za.zhonguo3118.cn

[S54] C++：异常处理
来源：https://bp.zhonguo4118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://os.zhonguo6118.cn

[S55] C++：结构化绑定
来源：https://qe.zhonguo8118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ds.zhonguo5118.cn

[S56] C++：optional
来源：https://wq.zhonguo4118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://pp.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://or.zhonguo2118.cn

constexpr int N = 10;
来源：https://rj.zhonguo5118.cn

[S58] C++：命名空间
来源：https://nr.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://nu.zhonguo8118.cn

[S59] C++：静态断言
来源：https://ot.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://no.zhonguo5118.cn

[S60] C++：遍历并删除元素
来源：https://tr.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://hy.zhonguo5118.cn

================================================================================
来源：https://ii.zhonguo7118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://fm.zhonguo2118.cn

================================================================================
来源：https://jd.zhonguo6118.cn

[T01] Kotlin：Hello World
来源：https://pm.zhonguo1118.cn

println("Hello")
来源：https://hm.zhonguo2118.cn

[T02] Kotlin：变量
来源：https://sx.zhonguo4118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://du.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://bd.zhonguo2118.cn

"值: $b"
来源：https://gu.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://ip.zhonguo3118.cn

val n: String? = null;  n?.length
来源：https://pn.zhonguo4118.cn

[T05] Kotlin：when 表达式
来源：https://cq.zhonguo4118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://fm.zhonguo3118.cn

[T06] Kotlin：集合映射
来源：https://ot.zhonguo1118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://ka.zhonguo3118.cn

[T07] Kotlin：集合过滤
来源：https://xx.zhonguo8118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://mc.zhonguo3118.cn

[T08] Kotlin：数据类
来源：https://wa.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://nk.zhonguo4118.cn

[T09] Kotlin：扩展函数
来源：https://qc.zhonguo2118.cn

fun String.exclaim() = this + "!"
来源：https://fa.zhonguo1118.cn

[T10] Kotlin：默认参数
来源：https://wr.zhonguo2118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://uw.zhonguo4118.cn

[T11] Kotlin：协程
来源：https://lj.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://sb.zhonguo3118.cn

[T12] Kotlin：解构声明
来源：https://qx.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://eg.zhonguo2118.cn

[T13] Kotlin：只读 Map
来源：https://bn.zhonguo3118.cn

val m = mapOf("a" to 1)
来源：https://ks.zhonguo7118.cn

[T14] Kotlin：循环
来源：https://zl.zhonguo2118.cn

for (i in 1..10) println(i)
来源：https://gy.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://ly.zhonguo2118.cn

interface Shape { fun area(): Double }
来源：https://bo.zhonguo2118.cn

[T16] Swift：Hello World
来源：https://fd.zhonguo4118.cn

print("Hello")
来源：https://ye.zhonguo6118.cn

[T17] Swift：变量与常量
来源：https://vm.zhonguo8118.cn

var a = 1;  let b = 2
来源：https://hj.zhonguo5118.cn

[T18] Swift：字符串插值
来源：https://zo.zhonguo8118.cn

"值: \(b)"
来源：https://ik.zhonguo7118.cn

[T19] Swift：可选绑定
来源：https://cz.zhonguo1118.cn

if let n = opt { print(n) }
来源：https://gs.zhonguo4118.cn

[T20] Swift：数组操作
来源：https://dg.zhonguo5118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://xp.zhonguo7118.cn

[T21] Swift：遍历
来源：https://gk.zhonguo2118.cn

for x in a { print(x) }
来源：https://gf.zhonguo4118.cn

[T22] Swift：字典
来源：https://yv.zhonguo5118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://re.zhonguo4118.cn

[T23] Swift：函数
来源：https://gz.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://he.zhonguo7118.cn

[T24] Swift：闭包
来源：https://rb.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://lo.zhonguo5118.cn

[T25] Swift：结构体
来源：https://sa.zhonguo8118.cn

struct P { var x: Int }
来源：https://nn.zhonguo6118.cn

[T26] Swift：类与重写
来源：https://ca.zhonguo4118.cn

class A: Base { override func f() {} }
来源：https://ug.zhonguo3118.cn

[T27] Swift：错误处理
来源：https://cw.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://ns.zhonguo4118.cn

[T28] Swift：枚举
来源：https://kq.zhonguo4118.cn

enum Color { case red, green }
来源：https://hl.zhonguo5118.cn

[T29] Swift：guard 提前返回
来源：https://aq.zhonguo3118.cn

guard let x = opt else { return }
来源：https://vu.zhonguo7118.cn

[T30] Swift：协议
来源：https://of.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://on.zhonguo8118.cn

[T31] Lua：Hello World
来源：https://sm.zhonguo3118.cn

print("Hello")
来源：https://qo.zhonguo1118.cn

[T32] Lua：局部变量
来源：https://yf.zhonguo1118.cn

local a = 1
来源：https://ir.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://lg.zhonguo6118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://ae.zhonguo1118.cn

[T34] Lua：遍历表
来源：https://jt.zhonguo4118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://sa.zhonguo5118.cn

[T35] Lua：字典表
来源：https://ok.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://rj.zhonguo8118.cn

[T36] Lua：函数
来源：https://ol.zhonguo8118.cn

function add(a, b) return a + b end
来源：https://re.zhonguo4118.cn

[T37] Lua：字符串拼接
来源：https://tm.zhonguo2118.cn

"a" .. "b"
来源：https://id.zhonguo2118.cn

[T38] Lua：条件
来源：https://by.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://kz.zhonguo7118.cn

[T39] Lua：模式匹配
来源：https://zp.zhonguo2118.cn

string.find(s, "%d+")
来源：https://xp.zhonguo3118.cn

[T40] Lua：元表
来源：https://pi.zhonguo8118.cn

setmetatable({}, { __index = base })
来源：https://ew.zhonguo7118.cn

[T41] Perl：Hello World
来源：https://ek.zhonguo4118.cn

print "Hello\n";
来源：https://dk.zhonguo1118.cn

[T42] Perl：变量类型
来源：https://zb.zhonguo5118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ca.zhonguo5118.cn

[T43] Perl：字符串插值
来源：https://or.zhonguo7118.cn

"值: $a"
来源：https://hh.zhonguo2118.cn

[T44] Perl：条件
来源：https://bs.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://fg.zhonguo5118.cn

[T45] Perl：数组遍历
来源：https://rj.zhonguo8118.cn

for my $x (@arr) { print $x; }
来源：https://yh.zhonguo1118.cn

[T46] Perl：哈希操作
来源：https://ag.zhonguo8118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://mn.zhonguo5118.cn

[T47] Perl：正则捕获
来源：https://tm.zhonguo3118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://ws.zhonguo3118.cn

[T48] Perl：正则替换
来源：https://qa.zhonguo4118.cn

$s =~ s/old/new/g;
来源：https://yg.zhonguo7118.cn

[T49] Perl：函数
来源：https://vz.zhonguo6118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://zq.zhonguo4118.cn

[T50] Perl：逐行读文件
来源：https://ou.zhonguo5118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://es.zhonguo4118.cn

while (my $line = <$fh>) { print $line; }
来源：https://pq.zhonguo1118.cn

[T51] Scala：Hello World
来源：https://uv.zhonguo4118.cn

println("Hello")
来源：https://kq.zhonguo7118.cn

[T52] Scala：变量
来源：https://xl.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://ui.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://qv.zhonguo1118.cn

s"值: $b"
来源：https://hw.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://ub.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://lt.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://gq.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://zu.zhonguo5118.cn

[T56] Scala：样例类
来源：https://ac.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://tl.zhonguo3118.cn

[T57] Scala：模式匹配
来源：https://gh.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://ym.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://xq.zhonguo7118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://wn.zhonguo3118.cn

[T59] Scala：循环
来源：https://ui.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://ik.zhonguo8118.cn

[T60] Scala：折叠
来源：https://ez.zhonguo6118.cn


<!-- 参考信息 -->