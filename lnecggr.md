代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://bt.zhonguo8118.cn

[R56] 远程拷贝
来源：https://ii.zhonguo6118.cn

scp file user@host:/path/
来源：https://rj.zhonguo4118.cn

[R57] 远程执行命令
来源：https://hj.zhonguo2118.cn

ssh user@host 'uptime'
来源：https://kx.zhonguo8118.cn

[R58] 下载文件
来源：https://gy.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://tp.zhonguo2118.cn

[R59] 发 POST JSON
来源：https://ok.zhonguo7118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://rm.zhonguo5118.cn

[R60] 只看 HTTP 状态码
来源：https://nl.zhonguo4118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://ds.zhonguo3118.cn

[R61] 磁盘占用
来源：https://zo.zhonguo7118.cn

df -h;  du -sh *
来源：https://zw.zhonguo6118.cn

[R62] 找最占空间的文件
来源：https://pv.zhonguo4118.cn

du -ah . | sort -rh | head -10
来源：https://to.zhonguo3118.cn

[R63] 内存与进程
来源：https://qj.zhonguo8118.cn

free -h;  ps aux | grep nginx
来源：https://lv.zhonguo1118.cn

[R64] 结束进程
来源：https://gr.zhonguo4118.cn

kill -9 $(pgrep -f app.py)
来源：https://vs.zhonguo4118.cn

[R65] 查看端口占用
来源：https://pt.zhonguo8118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://vs.zhonguo7118.cn

[R66] 定时任务
来源：https://og.zhonguo8118.cn

crontab -e;  crontab -l
来源：https://do.zhonguo2118.cn

[R67] 生成随机十六进制串
来源：https://kt.zhonguo5118.cn

openssl rand -hex 16
来源：https://yf.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://jf.zhonguo1118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://xt.zhonguo6118.cn

[R69] 生成随机密码
来源：https://fw.zhonguo5118.cn

head -c 16 /dev/urandom | base64
来源：https://mr.zhonguo6118.cn

[R70] 时间戳与互转
来源：https://sv.zhonguo6118.cn

date +%s;  date -d @1700000000
来源：https://st.zhonguo5118.cn

[R71] 日期格式化
来源：https://ge.zhonguo2118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://id.zhonguo7118.cn

[R72] 等待端口就绪
来源：https://fp.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://ey.zhonguo2118.cn

[R73] 分割大日志
来源：https://rx.zhonguo6118.cn

split -l 1000 big.log part_
来源：https://ua.zhonguo5118.cn

[R74] 批量重命名
来源：https://cf.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://tk.zhonguo4118.cn

[R75] 导出环境变量
来源：https://nb.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://wa.zhonguo3118.cn

[R76] 使用临时文件
来源：https://yo.zhonguo7118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://kg.zhonguo3118.cn

[R77] 读取用户输入
来源：https://io.zhonguo4118.cn

read -rp "请输入: " ans
来源：https://oa.zhonguo4118.cn

[R78] 交互式菜单
来源：https://hp.zhonguo7118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://mv.zhonguo3118.cn

[R79] 解析命令行选项
来源：https://xq.zhonguo1118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://ku.zhonguo7118.cn

[R80] 查看脚本执行耗时
来源：https://ch.zhonguo8118.cn

time ./run.sh
来源：https://ye.zhonguo2118.cn

================================================================================
来源：https://wq.zhonguo7118.cn

S. C / C++ 专题
来源：https://jb.zhonguo8118.cn

================================================================================
来源：https://ky.zhonguo3118.cn

[S01] C：Hello World
来源：https://zl.zhonguo6118.cn

#include <stdio.h>
来源：https://en.zhonguo2118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://xm.zhonguo5118.cn

[S02] C：变量与格式化输出
来源：https://bj.zhonguo2118.cn

int a = 10; printf("%d\n", a);
来源：https://ht.zhonguo6118.cn

[S03] C：读入整数
来源：https://rd.zhonguo3118.cn

int x; scanf("%d", &x);
来源：https://kc.zhonguo1118.cn

[S04] C：字符串复制
来源：https://ps.zhonguo3118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://ff.zhonguo1118.cn

[S05] C：字符串长度
来源：https://io.zhonguo1118.cn

strlen(s)
来源：https://dn.zhonguo7118.cn

[S06] C：字符串比较
来源：https://ji.zhonguo1118.cn

strcmp(a, b) == 0
来源：https://xs.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://ci.zhonguo2118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://xh.zhonguo1118.cn

[S08] C：动态内存分配与释放
来源：https://mi.zhonguo5118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://qf.zhonguo4118.cn

[S09] C：结构体定义与初始化
来源：https://ky.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://fc.zhonguo1118.cn

[S10] C：指针与解引用
来源：https://cg.zhonguo1118.cn

int *p = &a;  *p = 5;
来源：https://ph.zhonguo1118.cn

[S11] C：逐行读文件
来源：https://hf.zhonguo2118.cn

FILE *f = fopen("a.txt", "r");
来源：https://pv.zhonguo2118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://hl.zhonguo2118.cn

fclose(f);
来源：https://xx.zhonguo8118.cn

[S12] C：写文件
来源：https://bs.zhonguo4118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://td.zhonguo2118.cn

[S13] C：宏定义
来源：https://yp.zhonguo1118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://md.zhonguo2118.cn

[S14] C：枚举
来源：https://lc.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://lx.zhonguo2118.cn

[S15] C：类型转换
来源：https://iw.zhonguo7118.cn

(double) a / b
来源：https://zx.zhonguo8118.cn

[S16] C：位操作置位
来源：https://ub.zhonguo8118.cn

x |= (1 << 3);
来源：https://lx.zhonguo1118.cn

[S17] C：安全拼接字符串
来源：https://ij.zhonguo6118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://jq.zhonguo8118.cn

[S18] C：命令行参数
来源：https://yz.zhonguo7118.cn

int main(int argc, char **argv)
来源：https://ch.zhonguo1118.cn

[S19] C：快速排序
来源：https://ex.zhonguo5118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://xh.zhonguo3118.cn

[S20] C：二分查找
来源：https://fv.zhonguo7118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://dt.zhonguo1118.cn

[S21] C：字符类别判断
来源：https://cl.zhonguo8118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://np.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://sk.zhonguo5118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://ik.zhonguo1118.cn

[S23] C：随机数
来源：https://lu.zhonguo8118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://rl.zhonguo8118.cn

[S24] C：获取本地时间
来源：https://hr.zhonguo2118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://aa.zhonguo5118.cn

[S25] C：内存拷贝
来源：https://un.zhonguo1118.cn

memcpy(dst, src, n);
来源：https://fn.zhonguo2118.cn

[S26] C：内存清零
来源：https://bc.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://hq.zhonguo8118.cn

[S27] C：定义常量
来源：https://uh.zhonguo7118.cn

const double PI = 3.14159;
来源：https://ag.zhonguo3118.cn

[S28] C：静态变量
来源：https://rs.zhonguo3118.cn

static int counter = 0;
来源：https://yw.zhonguo3118.cn

[S29] C：变参函数
来源：https://sj.zhonguo7118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://se.zhonguo8118.cn

[S30] C：头文件保护
来源：https://ty.zhonguo8118.cn

#ifndef X_H
来源：https://ef.zhonguo6118.cn

#define X_H
来源：https://xs.zhonguo8118.cn

#endif
来源：https://ng.zhonguo2118.cn

[S31] C++：Hello World
来源：https://lr.zhonguo7118.cn

#include <iostream>
来源：https://ld.zhonguo1118.cn

int main() { std::cout << "Hello\n"; }
来源：https://uf.zhonguo3118.cn

[S32] C++：字符串
来源：https://hq.zhonguo4118.cn

std::string s = "hi";  s += "!";
来源：https://ir.zhonguo1118.cn

[S33] C++：vector 增删
来源：https://qf.zhonguo5118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://im.zhonguo2118.cn

[S34] C++：遍历 vector
来源：https://zl.zhonguo3118.cn

for (auto &x : v) { std::cout << x; }
来源：https://xs.zhonguo6118.cn

[S35] C++：map
来源：https://nb.zhonguo6118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://fa.zhonguo5118.cn

[S36] C++：unordered_map
来源：https://xu.zhonguo7118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://st.zhonguo2118.cn

[S37] C++：set
来源：https://dr.zhonguo2118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://jp.zhonguo5118.cn

[S38] C++：排序
来源：https://cr.zhonguo8118.cn

std::sort(v.begin(), v.end());
来源：https://wz.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://bj.zhonguo3118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://qd.zhonguo3118.cn

[S40] C++：查找元素
来源：https://hn.zhonguo8118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://we.zhonguo5118.cn

[S41] C++：类与构造函数
来源：https://fl.zhonguo5118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://gv.zhonguo2118.cn

[S42] C++：继承与虚函数
来源：https://bi.zhonguo8118.cn

class B : public Base { public: void f() override {} };
来源：https://zf.zhonguo3118.cn

[S43] C++：智能指针
来源：https://ig.zhonguo8118.cn

auto p = std::make_unique<int>(5);
来源：https://jq.zhonguo2118.cn

[S44] C++：引用传参
来源：https://gx.zhonguo3118.cn

void inc(int &x) { ++x; }
来源：https://og.zhonguo8118.cn

[S45] C++：lambda
来源：https://ta.zhonguo8118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://oz.zhonguo6118.cn

[S46] C++：函数模板
来源：https://bq.zhonguo6118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://zc.zhonguo5118.cn

[S47] C++：结构化绑定遍历
来源：https://me.zhonguo1118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://su.zhonguo4118.cn

[S48] C++：逐行读文件
来源：https://qi.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://ho.zhonguo4118.cn

while (std::getline(in, line)) { }
来源：https://fc.zhonguo8118.cn

[S49] C++：写文件
来源：https://tg.zhonguo7118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://rq.zhonguo8118.cn

[S50] C++：格式化数字
来源：https://ls.zhonguo7118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://oa.zhonguo3118.cn

[S51] C++：显式类型转换
来源：https://oj.zhonguo6118.cn

static_cast<double>(a) / b
来源：https://xj.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://lz.zhonguo4118.cn

int size() const noexcept { return n_; }
来源：https://ir.zhonguo8118.cn

[S53] C++：移动语义
来源：https://by.zhonguo7118.cn

std::vector<int> w = std::move(v);
来源：https://tf.zhonguo4118.cn

[S54] C++：异常处理
来源：https://ig.zhonguo6118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://gs.zhonguo3118.cn

[S55] C++：结构化绑定
来源：https://mx.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://kz.zhonguo5118.cn

[S56] C++：optional
来源：https://qp.zhonguo2118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://dg.zhonguo8118.cn

[S57] C++：编译期常量
来源：https://rv.zhonguo8118.cn

constexpr int N = 10;
来源：https://gt.zhonguo6118.cn

[S58] C++：命名空间
来源：https://xx.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://vx.zhonguo4118.cn

[S59] C++：静态断言
来源：https://ih.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ie.zhonguo8118.cn

[S60] C++：遍历并删除元素
来源：https://ds.zhonguo8118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://xs.zhonguo5118.cn

================================================================================
来源：https://gg.zhonguo5118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://ib.zhonguo3118.cn

================================================================================
来源：https://td.zhonguo3118.cn

[T01] Kotlin：Hello World
来源：https://bs.zhonguo7118.cn

println("Hello")
来源：https://eo.zhonguo4118.cn

[T02] Kotlin：变量
来源：https://iz.zhonguo2118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://vb.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://sm.zhonguo3118.cn

"值: $b"
来源：https://xh.zhonguo5118.cn

[T04] Kotlin：空安全
来源：https://jo.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://re.zhonguo1118.cn

[T05] Kotlin：when 表达式
来源：https://st.zhonguo2118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://io.zhonguo5118.cn

[T06] Kotlin：集合映射
来源：https://ki.zhonguo3118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://ev.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://qx.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://pf.zhonguo3118.cn

[T08] Kotlin：数据类
来源：https://wp.zhonguo8118.cn

data class User(val name: String, val age: Int)
来源：https://sn.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://zm.zhonguo3118.cn

fun String.exclaim() = this + "!"
来源：https://yb.zhonguo4118.cn

[T10] Kotlin：默认参数
来源：https://um.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://co.zhonguo7118.cn

[T11] Kotlin：协程
来源：https://xb.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://ji.zhonguo8118.cn

[T12] Kotlin：解构声明
来源：https://ll.zhonguo1118.cn

val (a, b) = Pair(1, 2)
来源：https://nf.zhonguo1118.cn

[T13] Kotlin：只读 Map
来源：https://na.zhonguo1118.cn

val m = mapOf("a" to 1)
来源：https://co.zhonguo2118.cn

[T14] Kotlin：循环
来源：https://vz.zhonguo4118.cn

for (i in 1..10) println(i)
来源：https://dq.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://uz.zhonguo2118.cn

interface Shape { fun area(): Double }
来源：https://qb.zhonguo6118.cn

[T16] Swift：Hello World
来源：https://or.zhonguo3118.cn

print("Hello")
来源：https://jc.zhonguo2118.cn

[T17] Swift：变量与常量
来源：https://nz.zhonguo1118.cn

var a = 1;  let b = 2
来源：https://wi.zhonguo4118.cn

[T18] Swift：字符串插值
来源：https://tr.zhonguo8118.cn

"值: \(b)"
来源：https://uy.zhonguo1118.cn

[T19] Swift：可选绑定
来源：https://vw.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://py.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://vl.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://xk.zhonguo2118.cn

[T21] Swift：遍历
来源：https://vy.zhonguo2118.cn

for x in a { print(x) }
来源：https://qn.zhonguo1118.cn

[T22] Swift：字典
来源：https://pt.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://ol.zhonguo4118.cn

[T23] Swift：函数
来源：https://rm.zhonguo8118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://uh.zhonguo6118.cn

[T24] Swift：闭包
来源：https://qe.zhonguo1118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://ox.zhonguo8118.cn

[T25] Swift：结构体
来源：https://hn.zhonguo3118.cn

struct P { var x: Int }
来源：https://wl.zhonguo4118.cn

[T26] Swift：类与重写
来源：https://rd.zhonguo1118.cn

class A: Base { override func f() {} }
来源：https://wc.zhonguo4118.cn

[T27] Swift：错误处理
来源：https://ob.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://ca.zhonguo4118.cn

[T28] Swift：枚举
来源：https://ip.zhonguo2118.cn

enum Color { case red, green }
来源：https://ns.zhonguo5118.cn

[T29] Swift：guard 提前返回
来源：https://to.zhonguo1118.cn

guard let x = opt else { return }
来源：https://ra.zhonguo3118.cn

[T30] Swift：协议
来源：https://yd.zhonguo7118.cn

protocol Shape { func area() -> Double }
来源：https://bz.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://pf.zhonguo6118.cn

print("Hello")
来源：https://be.zhonguo5118.cn

[T32] Lua：局部变量
来源：https://qz.zhonguo3118.cn

local a = 1
来源：https://ms.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://xr.zhonguo3118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://ng.zhonguo7118.cn

[T34] Lua：遍历表
来源：https://gc.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://lq.zhonguo6118.cn

[T35] Lua：字典表
来源：https://am.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://pl.zhonguo4118.cn

[T36] Lua：函数
来源：https://hz.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://jx.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://cj.zhonguo6118.cn

"a" .. "b"
来源：https://km.zhonguo5118.cn

[T38] Lua：条件
来源：https://vd.zhonguo1118.cn

if x > 0 then print("正") end
来源：https://dv.zhonguo4118.cn

[T39] Lua：模式匹配
来源：https://fr.zhonguo2118.cn

string.find(s, "%d+")
来源：https://ki.zhonguo3118.cn

[T40] Lua：元表
来源：https://oa.zhonguo2118.cn

setmetatable({}, { __index = base })
来源：https://nn.zhonguo3118.cn

[T41] Perl：Hello World
来源：https://qy.zhonguo1118.cn

print "Hello\n";
来源：https://cv.zhonguo7118.cn

[T42] Perl：变量类型
来源：https://no.zhonguo5118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ab.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://jg.zhonguo7118.cn

"值: $a"
来源：https://ot.zhonguo2118.cn

[T44] Perl：条件
来源：https://cy.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://pd.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://ub.zhonguo3118.cn

for my $x (@arr) { print $x; }
来源：https://we.zhonguo7118.cn

[T46] Perl：哈希操作
来源：https://lm.zhonguo8118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://as.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://eu.zhonguo4118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://uq.zhonguo4118.cn

[T48] Perl：正则替换
来源：https://ri.zhonguo7118.cn

$s =~ s/old/new/g;
来源：https://tm.zhonguo5118.cn

[T49] Perl：函数
来源：https://qx.zhonguo1118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://by.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://it.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://gz.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://yb.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://hd.zhonguo8118.cn

println("Hello")
来源：https://ev.zhonguo4118.cn

[T52] Scala：变量
来源：https://ly.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://zx.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://rw.zhonguo7118.cn

s"值: $b"
来源：https://fk.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://hw.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://cv.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://id.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://gk.zhonguo2118.cn

[T56] Scala：样例类
来源：https://tm.zhonguo6118.cn

case class User(name: String, age: Int)
来源：https://uq.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://tr.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://vd.zhonguo3118.cn

[T58] Scala：函数定义
来源：https://ip.zhonguo6118.cn


<!-- 参考信息 -->