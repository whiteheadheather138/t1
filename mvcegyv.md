代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ph.zhonguo2118.cn

[R50] awk 求和
来源：https://va.zhonguo8118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://sa.zhonguo5118.cn

[R51] 排序去重取前几
来源：https://ud.zhonguo4118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://mk.zhonguo8118.cn

[R52] 统计行数
来源：https://rm.zhonguo8118.cn

wc -l a.txt
来源：https://bm.zhonguo1118.cn

[R53] 查看文件头与实时尾
来源：https://hr.zhonguo2118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://qj.zhonguo5118.cn

[R54] 比较两个文件
来源：https://af.zhonguo1118.cn

diff a.txt b.txt
来源：https://ry.zhonguo3118.cn

[R55] 压缩与解压
来源：https://yo.zhonguo1118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://uu.zhonguo4118.cn

[R56] 远程拷贝
来源：https://qp.zhonguo6118.cn

scp file user@host:/path/
来源：https://un.zhonguo4118.cn

[R57] 远程执行命令
来源：https://on.zhonguo7118.cn

ssh user@host 'uptime'
来源：https://kg.zhonguo8118.cn

[R58] 下载文件
来源：https://sw.zhonguo8118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://se.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://bo.zhonguo8118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://eu.zhonguo2118.cn

[R60] 只看 HTTP 状态码
来源：https://xp.zhonguo2118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://lb.zhonguo1118.cn

[R61] 磁盘占用
来源：https://hj.zhonguo3118.cn

df -h;  du -sh *
来源：https://yz.zhonguo6118.cn

[R62] 找最占空间的文件
来源：https://vo.zhonguo6118.cn

du -ah . | sort -rh | head -10
来源：https://et.zhonguo5118.cn

[R63] 内存与进程
来源：https://el.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://ik.zhonguo3118.cn

[R64] 结束进程
来源：https://li.zhonguo6118.cn

kill -9 $(pgrep -f app.py)
来源：https://xi.zhonguo1118.cn

[R65] 查看端口占用
来源：https://ux.zhonguo5118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://lp.zhonguo3118.cn

[R66] 定时任务
来源：https://wq.zhonguo1118.cn

crontab -e;  crontab -l
来源：https://px.zhonguo5118.cn

[R67] 生成随机十六进制串
来源：https://ri.zhonguo3118.cn

openssl rand -hex 16
来源：https://ov.zhonguo8118.cn

[R68] 计算文件校验值
来源：https://ur.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://wp.zhonguo7118.cn

[R69] 生成随机密码
来源：https://pn.zhonguo8118.cn

head -c 16 /dev/urandom | base64
来源：https://ip.zhonguo2118.cn

[R70] 时间戳与互转
来源：https://ss.zhonguo7118.cn

date +%s;  date -d @1700000000
来源：https://xh.zhonguo3118.cn

[R71] 日期格式化
来源：https://br.zhonguo4118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://rg.zhonguo2118.cn

[R72] 等待端口就绪
来源：https://dw.zhonguo7118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://kn.zhonguo1118.cn

[R73] 分割大日志
来源：https://ny.zhonguo7118.cn

split -l 1000 big.log part_
来源：https://fw.zhonguo8118.cn

[R74] 批量重命名
来源：https://ps.zhonguo6118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://dl.zhonguo2118.cn

[R75] 导出环境变量
来源：https://vo.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://sb.zhonguo6118.cn

[R76] 使用临时文件
来源：https://qh.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://if.zhonguo4118.cn

[R77] 读取用户输入
来源：https://rn.zhonguo4118.cn

read -rp "请输入: " ans
来源：https://ut.zhonguo1118.cn

[R78] 交互式菜单
来源：https://sc.zhonguo3118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://sc.zhonguo1118.cn

[R79] 解析命令行选项
来源：https://nq.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://ix.zhonguo1118.cn

[R80] 查看脚本执行耗时
来源：https://me.zhonguo7118.cn

time ./run.sh
来源：https://az.zhonguo6118.cn

================================================================================
来源：https://wq.zhonguo4118.cn

S. C / C++ 专题
来源：https://vz.zhonguo5118.cn

================================================================================
来源：https://is.zhonguo1118.cn

[S01] C：Hello World
来源：https://lp.zhonguo1118.cn

#include <stdio.h>
来源：https://ez.zhonguo1118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://id.zhonguo2118.cn

[S02] C：变量与格式化输出
来源：https://za.zhonguo8118.cn

int a = 10; printf("%d\n", a);
来源：https://ri.zhonguo4118.cn

[S03] C：读入整数
来源：https://km.zhonguo3118.cn

int x; scanf("%d", &x);
来源：https://mi.zhonguo8118.cn

[S04] C：字符串复制
来源：https://vh.zhonguo2118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://md.zhonguo6118.cn

[S05] C：字符串长度
来源：https://aq.zhonguo5118.cn

strlen(s)
来源：https://yv.zhonguo1118.cn

[S06] C：字符串比较
来源：https://uk.zhonguo6118.cn

strcmp(a, b) == 0
来源：https://yz.zhonguo3118.cn

[S07] C：数组遍历求和
来源：https://qo.zhonguo8118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://cv.zhonguo2118.cn

[S08] C：动态内存分配与释放
来源：https://ri.zhonguo1118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://uv.zhonguo1118.cn

[S09] C：结构体定义与初始化
来源：https://mp.zhonguo7118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://kr.zhonguo3118.cn

[S10] C：指针与解引用
来源：https://dg.zhonguo3118.cn

int *p = &a;  *p = 5;
来源：https://an.zhonguo3118.cn

[S11] C：逐行读文件
来源：https://zr.zhonguo1118.cn

FILE *f = fopen("a.txt", "r");
来源：https://mf.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://tr.zhonguo1118.cn

fclose(f);
来源：https://en.zhonguo2118.cn

[S12] C：写文件
来源：https://ej.zhonguo1118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://zp.zhonguo2118.cn

[S13] C：宏定义
来源：https://if.zhonguo8118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://ee.zhonguo7118.cn

[S14] C：枚举
来源：https://tp.zhonguo4118.cn

enum Color { RED, GREEN, BLUE };
来源：https://bf.zhonguo6118.cn

[S15] C：类型转换
来源：https://ii.zhonguo2118.cn

(double) a / b
来源：https://je.zhonguo8118.cn

[S16] C：位操作置位
来源：https://uw.zhonguo5118.cn

x |= (1 << 3);
来源：https://et.zhonguo6118.cn

[S17] C：安全拼接字符串
来源：https://tb.zhonguo7118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://sd.zhonguo8118.cn

[S18] C：命令行参数
来源：https://ka.zhonguo2118.cn

int main(int argc, char **argv)
来源：https://zm.zhonguo5118.cn

[S19] C：快速排序
来源：https://rl.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://xv.zhonguo2118.cn

[S20] C：二分查找
来源：https://es.zhonguo6118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://zb.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://ym.zhonguo5118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://je.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://ti.zhonguo2118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://mr.zhonguo1118.cn

[S23] C：随机数
来源：https://cf.zhonguo3118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://up.zhonguo4118.cn

[S24] C：获取本地时间
来源：https://xy.zhonguo4118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://za.zhonguo3118.cn

[S25] C：内存拷贝
来源：https://ge.zhonguo1118.cn

memcpy(dst, src, n);
来源：https://bf.zhonguo6118.cn

[S26] C：内存清零
来源：https://bw.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://xm.zhonguo5118.cn

[S27] C：定义常量
来源：https://fk.zhonguo7118.cn

const double PI = 3.14159;
来源：https://ww.zhonguo4118.cn

[S28] C：静态变量
来源：https://ay.zhonguo7118.cn

static int counter = 0;
来源：https://kn.zhonguo5118.cn

[S29] C：变参函数
来源：https://xo.zhonguo2118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://km.zhonguo4118.cn

[S30] C：头文件保护
来源：https://kd.zhonguo5118.cn

#ifndef X_H
来源：https://uc.zhonguo5118.cn

#define X_H
来源：https://dq.zhonguo7118.cn

#endif
来源：https://gn.zhonguo7118.cn

[S31] C++：Hello World
来源：https://eo.zhonguo6118.cn

#include <iostream>
来源：https://gx.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://tp.zhonguo7118.cn

[S32] C++：字符串
来源：https://dn.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://cm.zhonguo4118.cn

[S33] C++：vector 增删
来源：https://dg.zhonguo5118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://vx.zhonguo8118.cn

[S34] C++：遍历 vector
来源：https://qa.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://gu.zhonguo5118.cn

[S35] C++：map
来源：https://hr.zhonguo4118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://xu.zhonguo2118.cn

[S36] C++：unordered_map
来源：https://ac.zhonguo3118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://dv.zhonguo8118.cn

[S37] C++：set
来源：https://sk.zhonguo5118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://fx.zhonguo1118.cn

[S38] C++：排序
来源：https://ph.zhonguo3118.cn

std::sort(v.begin(), v.end());
来源：https://xo.zhonguo5118.cn

[S39] C++：自定义比较器排序
来源：https://fa.zhonguo7118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://yl.zhonguo4118.cn

[S40] C++：查找元素
来源：https://xo.zhonguo2118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://ux.zhonguo8118.cn

[S41] C++：类与构造函数
来源：https://fm.zhonguo6118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://yf.zhonguo3118.cn

[S42] C++：继承与虚函数
来源：https://zx.zhonguo5118.cn

class B : public Base { public: void f() override {} };
来源：https://sl.zhonguo4118.cn

[S43] C++：智能指针
来源：https://ak.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://ct.zhonguo2118.cn

[S44] C++：引用传参
来源：https://be.zhonguo8118.cn

void inc(int &x) { ++x; }
来源：https://oo.zhonguo5118.cn

[S45] C++：lambda
来源：https://gz.zhonguo3118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://tr.zhonguo4118.cn

[S46] C++：函数模板
来源：https://fx.zhonguo6118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://gt.zhonguo5118.cn

[S47] C++：结构化绑定遍历
来源：https://uz.zhonguo6118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://cy.zhonguo7118.cn

[S48] C++：逐行读文件
来源：https://ho.zhonguo4118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://as.zhonguo2118.cn

while (std::getline(in, line)) { }
来源：https://eo.zhonguo5118.cn

[S49] C++：写文件
来源：https://bv.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://up.zhonguo4118.cn

[S50] C++：格式化数字
来源：https://df.zhonguo4118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://dy.zhonguo1118.cn

[S51] C++：显式类型转换
来源：https://ma.zhonguo7118.cn

static_cast<double>(a) / b
来源：https://oy.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://kj.zhonguo5118.cn

int size() const noexcept { return n_; }
来源：https://cz.zhonguo5118.cn

[S53] C++：移动语义
来源：https://qv.zhonguo7118.cn

std::vector<int> w = std::move(v);
来源：https://sy.zhonguo2118.cn

[S54] C++：异常处理
来源：https://ot.zhonguo4118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://om.zhonguo2118.cn

[S55] C++：结构化绑定
来源：https://hd.zhonguo5118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://mk.zhonguo6118.cn

[S56] C++：optional
来源：https://mi.zhonguo4118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://bj.zhonguo5118.cn

[S57] C++：编译期常量
来源：https://xm.zhonguo2118.cn

constexpr int N = 10;
来源：https://fo.zhonguo4118.cn

[S58] C++：命名空间
来源：https://xx.zhonguo4118.cn

namespace ns { int f() { return 1; } }
来源：https://kt.zhonguo1118.cn

[S59] C++：静态断言
来源：https://ew.zhonguo7118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://mj.zhonguo6118.cn

[S60] C++：遍历并删除元素
来源：https://si.zhonguo3118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://hp.zhonguo5118.cn

================================================================================
来源：https://rh.zhonguo3118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://fm.zhonguo5118.cn

================================================================================
来源：https://kx.zhonguo2118.cn

[T01] Kotlin：Hello World
来源：https://gr.zhonguo4118.cn

println("Hello")
来源：https://gv.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://wo.zhonguo8118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://fx.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://oi.zhonguo8118.cn

"值: $b"
来源：https://pj.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://wy.zhonguo8118.cn

val n: String? = null;  n?.length
来源：https://pa.zhonguo8118.cn

[T05] Kotlin：when 表达式
来源：https://sn.zhonguo1118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://el.zhonguo1118.cn

[T06] Kotlin：集合映射
来源：https://og.zhonguo3118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://uc.zhonguo8118.cn

[T07] Kotlin：集合过滤
来源：https://eh.zhonguo7118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://xy.zhonguo6118.cn

[T08] Kotlin：数据类
来源：https://vg.zhonguo8118.cn

data class User(val name: String, val age: Int)
来源：https://pa.zhonguo1118.cn

[T09] Kotlin：扩展函数
来源：https://tq.zhonguo3118.cn

fun String.exclaim() = this + "!"
来源：https://ev.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://ha.zhonguo3118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://gc.zhonguo6118.cn

[T11] Kotlin：协程
来源：https://zy.zhonguo5118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://zf.zhonguo5118.cn

[T12] Kotlin：解构声明
来源：https://kv.zhonguo1118.cn

val (a, b) = Pair(1, 2)
来源：https://ka.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://tx.zhonguo1118.cn

val m = mapOf("a" to 1)
来源：https://ra.zhonguo7118.cn

[T14] Kotlin：循环
来源：https://na.zhonguo3118.cn

for (i in 1..10) println(i)
来源：https://lr.zhonguo2118.cn

[T15] Kotlin：接口
来源：https://ra.zhonguo5118.cn

interface Shape { fun area(): Double }
来源：https://im.zhonguo5118.cn

[T16] Swift：Hello World
来源：https://zh.zhonguo5118.cn

print("Hello")
来源：https://gy.zhonguo7118.cn

[T17] Swift：变量与常量
来源：https://ye.zhonguo4118.cn

var a = 1;  let b = 2
来源：https://bw.zhonguo8118.cn

[T18] Swift：字符串插值
来源：https://ju.zhonguo6118.cn

"值: \(b)"
来源：https://lg.zhonguo7118.cn

[T19] Swift：可选绑定
来源：https://ps.zhonguo5118.cn

if let n = opt { print(n) }
来源：https://ua.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://fk.zhonguo8118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://mf.zhonguo6118.cn

[T21] Swift：遍历
来源：https://tn.zhonguo4118.cn

for x in a { print(x) }
来源：https://dk.zhonguo4118.cn

[T22] Swift：字典
来源：https://yp.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://xo.zhonguo4118.cn

[T23] Swift：函数
来源：https://qy.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://ch.zhonguo6118.cn

[T24] Swift：闭包
来源：https://gm.zhonguo5118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://fp.zhonguo5118.cn

[T25] Swift：结构体
来源：https://bh.zhonguo6118.cn

struct P { var x: Int }
来源：https://ra.zhonguo1118.cn

[T26] Swift：类与重写
来源：https://al.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://bk.zhonguo2118.cn

[T27] Swift：错误处理
来源：https://eg.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://qf.zhonguo2118.cn

[T28] Swift：枚举
来源：https://wq.zhonguo2118.cn

enum Color { case red, green }
来源：https://ok.zhonguo1118.cn

[T29] Swift：guard 提前返回
来源：https://xb.zhonguo3118.cn

guard let x = opt else { return }
来源：https://lh.zhonguo7118.cn

[T30] Swift：协议
来源：https://bj.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://xh.zhonguo5118.cn

[T31] Lua：Hello World
来源：https://me.zhonguo5118.cn

print("Hello")
来源：https://ap.zhonguo3118.cn

[T32] Lua：局部变量
来源：https://nw.zhonguo3118.cn

local a = 1
来源：https://jv.zhonguo8118.cn

[T33] Lua：表（数组）
来源：https://ih.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://rs.zhonguo5118.cn

[T34] Lua：遍历表
来源：https://vz.zhonguo3118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://em.zhonguo7118.cn

[T35] Lua：字典表
来源：https://es.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://xs.zhonguo6118.cn

[T36] Lua：函数
来源：https://mo.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://mw.zhonguo4118.cn

[T37] Lua：字符串拼接
来源：https://to.zhonguo4118.cn

"a" .. "b"
来源：https://nf.zhonguo2118.cn

[T38] Lua：条件
来源：https://ea.zhonguo7118.cn

if x > 0 then print("正") end
来源：https://uv.zhonguo8118.cn

[T39] Lua：模式匹配
来源：https://ho.zhonguo3118.cn

string.find(s, "%d+")
来源：https://cw.zhonguo7118.cn

[T40] Lua：元表
来源：https://fq.zhonguo1118.cn

setmetatable({}, { __index = base })
来源：https://gz.zhonguo4118.cn

[T41] Perl：Hello World
来源：https://km.zhonguo5118.cn

print "Hello\n";
来源：https://ly.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://rz.zhonguo1118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://il.zhonguo5118.cn

[T43] Perl：字符串插值
来源：https://gu.zhonguo1118.cn

"值: $a"
来源：https://dq.zhonguo1118.cn

[T44] Perl：条件
来源：https://ao.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://ay.zhonguo6118.cn

[T45] Perl：数组遍历
来源：https://es.zhonguo6118.cn

for my $x (@arr) { print $x; }
来源：https://vt.zhonguo8118.cn

[T46] Perl：哈希操作
来源：https://yl.zhonguo1118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://eg.zhonguo2118.cn

[T47] Perl：正则捕获
来源：https://bu.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://kf.zhonguo4118.cn

[T48] Perl：正则替换
来源：https://ul.zhonguo3118.cn

$s =~ s/old/new/g;
来源：https://my.zhonguo7118.cn

[T49] Perl：函数
来源：https://qa.zhonguo6118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://sz.zhonguo7118.cn

[T50] Perl：逐行读文件
来源：https://pl.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://aj.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://an.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://kq.zhonguo5118.cn

println("Hello")
来源：https://tl.zhonguo2118.cn

[T52] Scala：变量
来源：https://gc.zhonguo4118.cn


<!-- 参考信息 -->