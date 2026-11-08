代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：https://et.zhonguo1118.cn

[R48] awk 取指定列
来源：https://ne.zhonguo2118.cn

awk '{print $1, $3}' a.txt
来源：https://ma.zhonguo1118.cn

[R49] awk 带条件
来源：https://so.zhonguo1118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://ee.zhonguo7118.cn

[R50] awk 求和
来源：https://mg.zhonguo2118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://nb.zhonguo8118.cn

[R51] 排序去重取前几
来源：https://jv.zhonguo2118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://qu.zhonguo3118.cn

[R52] 统计行数
来源：https://lo.zhonguo2118.cn

wc -l a.txt
来源：https://pe.zhonguo7118.cn

[R53] 查看文件头与实时尾
来源：https://vz.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://wy.zhonguo6118.cn

[R54] 比较两个文件
来源：https://mh.zhonguo1118.cn

diff a.txt b.txt
来源：https://xe.zhonguo4118.cn

[R55] 压缩与解压
来源：https://hl.zhonguo2118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ds.zhonguo8118.cn

[R56] 远程拷贝
来源：https://jg.zhonguo1118.cn

scp file user@host:/path/
来源：https://zk.zhonguo7118.cn

[R57] 远程执行命令
来源：https://gl.zhonguo8118.cn

ssh user@host 'uptime'
来源：https://va.zhonguo6118.cn

[R58] 下载文件
来源：https://eg.zhonguo6118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://aw.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://ak.zhonguo6118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://fe.zhonguo8118.cn

[R60] 只看 HTTP 状态码
来源：https://gm.zhonguo2118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://qy.zhonguo5118.cn

[R61] 磁盘占用
来源：https://zt.zhonguo6118.cn

df -h;  du -sh *
来源：https://jb.zhonguo3118.cn

[R62] 找最占空间的文件
来源：https://an.zhonguo2118.cn

du -ah . | sort -rh | head -10
来源：https://hv.zhonguo3118.cn

[R63] 内存与进程
来源：https://nv.zhonguo1118.cn

free -h;  ps aux | grep nginx
来源：https://gi.zhonguo1118.cn

[R64] 结束进程
来源：https://zu.zhonguo8118.cn

kill -9 $(pgrep -f app.py)
来源：https://le.zhonguo6118.cn

[R65] 查看端口占用
来源：https://dn.zhonguo6118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://as.zhonguo1118.cn

[R66] 定时任务
来源：https://ln.zhonguo2118.cn

crontab -e;  crontab -l
来源：https://yv.zhonguo2118.cn

[R67] 生成随机十六进制串
来源：https://kj.zhonguo1118.cn

openssl rand -hex 16
来源：https://vr.zhonguo8118.cn

[R68] 计算文件校验值
来源：https://rq.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://hl.zhonguo8118.cn

[R69] 生成随机密码
来源：https://jj.zhonguo8118.cn

head -c 16 /dev/urandom | base64
来源：https://ip.zhonguo1118.cn

[R70] 时间戳与互转
来源：https://xf.zhonguo8118.cn

date +%s;  date -d @1700000000
来源：https://um.zhonguo5118.cn

[R71] 日期格式化
来源：https://lh.zhonguo8118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://cg.zhonguo2118.cn

[R72] 等待端口就绪
来源：https://bo.zhonguo3118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://gm.zhonguo3118.cn

[R73] 分割大日志
来源：https://nr.zhonguo2118.cn

split -l 1000 big.log part_
来源：https://ch.zhonguo3118.cn

[R74] 批量重命名
来源：https://ew.zhonguo3118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ii.zhonguo5118.cn

[R75] 导出环境变量
来源：https://xf.zhonguo8118.cn

export PATH="$HOME/bin:$PATH"
来源：https://kl.zhonguo5118.cn

[R76] 使用临时文件
来源：https://vd.zhonguo3118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://fd.zhonguo6118.cn

[R77] 读取用户输入
来源：https://mm.zhonguo6118.cn

read -rp "请输入: " ans
来源：https://nu.zhonguo6118.cn

[R78] 交互式菜单
来源：https://gh.zhonguo3118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://za.zhonguo1118.cn

[R79] 解析命令行选项
来源：https://fr.zhonguo6118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://gn.zhonguo1118.cn

[R80] 查看脚本执行耗时
来源：https://bc.zhonguo7118.cn

time ./run.sh
来源：https://jf.zhonguo3118.cn

================================================================================
来源：https://er.zhonguo2118.cn

S. C / C++ 专题
来源：https://na.zhonguo5118.cn

================================================================================
来源：https://pn.zhonguo2118.cn

[S01] C：Hello World
来源：https://ei.zhonguo2118.cn

#include <stdio.h>
来源：https://ix.zhonguo4118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://gi.zhonguo2118.cn

[S02] C：变量与格式化输出
来源：https://zy.zhonguo3118.cn

int a = 10; printf("%d\n", a);
来源：https://ha.zhonguo7118.cn

[S03] C：读入整数
来源：https://xd.zhonguo4118.cn

int x; scanf("%d", &x);
来源：https://ek.zhonguo4118.cn

[S04] C：字符串复制
来源：https://tl.zhonguo4118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://io.zhonguo7118.cn

[S05] C：字符串长度
来源：https://hk.zhonguo8118.cn

strlen(s)
来源：https://uz.zhonguo5118.cn

[S06] C：字符串比较
来源：https://zr.zhonguo7118.cn

strcmp(a, b) == 0
来源：https://oz.zhonguo8118.cn

[S07] C：数组遍历求和
来源：https://tv.zhonguo4118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://aq.zhonguo8118.cn

[S08] C：动态内存分配与释放
来源：https://rf.zhonguo1118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://ts.zhonguo2118.cn

[S09] C：结构体定义与初始化
来源：https://kj.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ue.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://bh.zhonguo1118.cn

int *p = &a;  *p = 5;
来源：https://im.zhonguo3118.cn

[S11] C：逐行读文件
来源：https://ke.zhonguo3118.cn

FILE *f = fopen("a.txt", "r");
来源：https://hu.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://zn.zhonguo4118.cn

fclose(f);
来源：https://pi.zhonguo2118.cn

[S12] C：写文件
来源：https://ak.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://ht.zhonguo1118.cn

[S13] C：宏定义
来源：https://dt.zhonguo5118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://tm.zhonguo3118.cn

[S14] C：枚举
来源：https://as.zhonguo4118.cn

enum Color { RED, GREEN, BLUE };
来源：https://pa.zhonguo6118.cn

[S15] C：类型转换
来源：https://mi.zhonguo5118.cn

(double) a / b
来源：https://qf.zhonguo7118.cn

[S16] C：位操作置位
来源：https://od.zhonguo2118.cn

x |= (1 << 3);
来源：https://bd.zhonguo3118.cn

[S17] C：安全拼接字符串
来源：https://ml.zhonguo5118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://zl.zhonguo4118.cn

[S18] C：命令行参数
来源：https://xa.zhonguo7118.cn

int main(int argc, char **argv)
来源：https://qy.zhonguo7118.cn

[S19] C：快速排序
来源：https://rp.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://rb.zhonguo2118.cn

[S20] C：二分查找
来源：https://wi.zhonguo1118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://wp.zhonguo3118.cn

[S21] C：字符类别判断
来源：https://yo.zhonguo1118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://ua.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://rq.zhonguo7118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://pz.zhonguo7118.cn

[S23] C：随机数
来源：https://az.zhonguo6118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://cz.zhonguo4118.cn

[S24] C：获取本地时间
来源：https://vr.zhonguo8118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://rp.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://vw.zhonguo4118.cn

memcpy(dst, src, n);
来源：https://at.zhonguo5118.cn

[S26] C：内存清零
来源：https://bl.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://al.zhonguo5118.cn

[S27] C：定义常量
来源：https://my.zhonguo5118.cn

const double PI = 3.14159;
来源：https://th.zhonguo7118.cn

[S28] C：静态变量
来源：https://ox.zhonguo2118.cn

static int counter = 0;
来源：https://ah.zhonguo6118.cn

[S29] C：变参函数
来源：https://ai.zhonguo4118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://mx.zhonguo1118.cn

[S30] C：头文件保护
来源：https://pr.zhonguo7118.cn

#ifndef X_H
来源：https://fv.zhonguo5118.cn

#define X_H
来源：https://up.zhonguo3118.cn

#endif
来源：https://ud.zhonguo3118.cn

[S31] C++：Hello World
来源：https://pg.zhonguo6118.cn

#include <iostream>
来源：https://oz.zhonguo5118.cn

int main() { std::cout << "Hello\n"; }
来源：https://vg.zhonguo7118.cn

[S32] C++：字符串
来源：https://kn.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://jz.zhonguo2118.cn

[S33] C++：vector 增删
来源：https://qt.zhonguo6118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://ev.zhonguo2118.cn

[S34] C++：遍历 vector
来源：https://ir.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://am.zhonguo5118.cn

[S35] C++：map
来源：https://cm.zhonguo3118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://vw.zhonguo1118.cn

[S36] C++：unordered_map
来源：https://oq.zhonguo7118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ce.zhonguo2118.cn

[S37] C++：set
来源：https://yo.zhonguo2118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://cu.zhonguo5118.cn

[S38] C++：排序
来源：https://yn.zhonguo6118.cn

std::sort(v.begin(), v.end());
来源：https://df.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://bc.zhonguo4118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://aa.zhonguo3118.cn

[S40] C++：查找元素
来源：https://on.zhonguo4118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://on.zhonguo1118.cn

[S41] C++：类与构造函数
来源：https://py.zhonguo5118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://oq.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://so.zhonguo8118.cn

class B : public Base { public: void f() override {} };
来源：https://bw.zhonguo7118.cn

[S43] C++：智能指针
来源：https://zh.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://zl.zhonguo4118.cn

[S44] C++：引用传参
来源：https://gf.zhonguo4118.cn

void inc(int &x) { ++x; }
来源：https://vj.zhonguo5118.cn

[S45] C++：lambda
来源：https://tl.zhonguo2118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://gm.zhonguo2118.cn

[S46] C++：函数模板
来源：https://cb.zhonguo5118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://ng.zhonguo6118.cn

[S47] C++：结构化绑定遍历
来源：https://rw.zhonguo4118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://bs.zhonguo1118.cn

[S48] C++：逐行读文件
来源：https://wa.zhonguo3118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://ah.zhonguo1118.cn

while (std::getline(in, line)) { }
来源：https://zv.zhonguo7118.cn

[S49] C++：写文件
来源：https://ea.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://fz.zhonguo3118.cn

[S50] C++：格式化数字
来源：https://zw.zhonguo6118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://sy.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://uq.zhonguo1118.cn

static_cast<double>(a) / b
来源：https://bu.zhonguo1118.cn

[S52] C++：const 与 noexcept
来源：https://ma.zhonguo6118.cn

int size() const noexcept { return n_; }
来源：https://im.zhonguo1118.cn

[S53] C++：移动语义
来源：https://ea.zhonguo3118.cn

std::vector<int> w = std::move(v);
来源：https://eq.zhonguo6118.cn

[S54] C++：异常处理
来源：https://sl.zhonguo8118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://xl.zhonguo8118.cn

[S55] C++：结构化绑定
来源：https://pv.zhonguo6118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://cu.zhonguo4118.cn

[S56] C++：optional
来源：https://hd.zhonguo2118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ot.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://ev.zhonguo4118.cn

constexpr int N = 10;
来源：https://jd.zhonguo8118.cn

[S58] C++：命名空间
来源：https://fh.zhonguo6118.cn

namespace ns { int f() { return 1; } }
来源：https://sf.zhonguo8118.cn

[S59] C++：静态断言
来源：https://hh.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://qk.zhonguo8118.cn

[S60] C++：遍历并删除元素
来源：https://fl.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://ub.zhonguo3118.cn

================================================================================
来源：https://bw.zhonguo7118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://gb.zhonguo4118.cn

================================================================================
来源：https://tq.zhonguo2118.cn

[T01] Kotlin：Hello World
来源：https://pn.zhonguo5118.cn

println("Hello")
来源：https://aa.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://yb.zhonguo7118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://dm.zhonguo8118.cn

[T03] Kotlin：字符串模板
来源：https://sh.zhonguo6118.cn

"值: $b"
来源：https://ux.zhonguo4118.cn

[T04] Kotlin：空安全
来源：https://jd.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://dq.zhonguo7118.cn

[T05] Kotlin：when 表达式
来源：https://hp.zhonguo7118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://sz.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://vq.zhonguo6118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://ng.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://lw.zhonguo6118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://oc.zhonguo2118.cn

[T08] Kotlin：数据类
来源：https://rl.zhonguo5118.cn

data class User(val name: String, val age: Int)
来源：https://ah.zhonguo4118.cn

[T09] Kotlin：扩展函数
来源：https://tb.zhonguo5118.cn

fun String.exclaim() = this + "!"
来源：https://hd.zhonguo2118.cn

[T10] Kotlin：默认参数
来源：https://yn.zhonguo1118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://ns.zhonguo1118.cn

[T11] Kotlin：协程
来源：https://kv.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://mv.zhonguo5118.cn

[T12] Kotlin：解构声明
来源：https://gb.zhonguo7118.cn

val (a, b) = Pair(1, 2)
来源：https://li.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://so.zhonguo1118.cn

val m = mapOf("a" to 1)
来源：https://eu.zhonguo5118.cn

[T14] Kotlin：循环
来源：https://nh.zhonguo8118.cn

for (i in 1..10) println(i)
来源：https://gm.zhonguo5118.cn

[T15] Kotlin：接口
来源：https://fq.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://io.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://aq.zhonguo5118.cn

print("Hello")
来源：https://gf.zhonguo1118.cn

[T17] Swift：变量与常量
来源：https://hh.zhonguo3118.cn

var a = 1;  let b = 2
来源：https://fe.zhonguo3118.cn

[T18] Swift：字符串插值
来源：https://oi.zhonguo1118.cn

"值: \(b)"
来源：https://fa.zhonguo8118.cn

[T19] Swift：可选绑定
来源：https://gz.zhonguo3118.cn

if let n = opt { print(n) }
来源：https://mc.zhonguo7118.cn

[T20] Swift：数组操作
来源：https://ga.zhonguo1118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://iz.zhonguo7118.cn

[T21] Swift：遍历
来源：https://eo.zhonguo5118.cn

for x in a { print(x) }
来源：https://vn.zhonguo6118.cn

[T22] Swift：字典
来源：https://zo.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://kf.zhonguo4118.cn

[T23] Swift：函数
来源：https://kq.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://os.zhonguo4118.cn

[T24] Swift：闭包
来源：https://li.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://hs.zhonguo4118.cn

[T25] Swift：结构体
来源：https://jr.zhonguo5118.cn

struct P { var x: Int }
来源：https://er.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://ss.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://at.zhonguo7118.cn

[T27] Swift：错误处理
来源：https://zx.zhonguo8118.cn

do { try f() } catch { print(error) }
来源：https://ve.zhonguo7118.cn

[T28] Swift：枚举
来源：https://gy.zhonguo6118.cn

enum Color { case red, green }
来源：https://hr.zhonguo3118.cn

[T29] Swift：guard 提前返回
来源：https://fp.zhonguo4118.cn

guard let x = opt else { return }
来源：https://yq.zhonguo1118.cn

[T30] Swift：协议
来源：https://cp.zhonguo3118.cn

protocol Shape { func area() -> Double }
来源：https://wq.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://uy.zhonguo2118.cn

print("Hello")
来源：https://jh.zhonguo3118.cn

[T32] Lua：局部变量
来源：https://np.zhonguo8118.cn

local a = 1
来源：https://ex.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://kf.zhonguo3118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://zl.zhonguo7118.cn

[T34] Lua：遍历表
来源：https://lc.zhonguo7118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://id.zhonguo1118.cn

[T35] Lua：字典表
来源：https://zm.zhonguo1118.cn

local d = { a = 1 };  d.b = 2
来源：https://wv.zhonguo7118.cn

[T36] Lua：函数
来源：https://sz.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://ky.zhonguo1118.cn

[T37] Lua：字符串拼接
来源：https://wv.zhonguo3118.cn

"a" .. "b"
来源：https://qe.zhonguo2118.cn

[T38] Lua：条件
来源：https://fz.zhonguo8118.cn

if x > 0 then print("正") end
来源：https://mj.zhonguo4118.cn

[T39] Lua：模式匹配
来源：https://zw.zhonguo3118.cn

string.find(s, "%d+")
来源：https://pg.zhonguo2118.cn

[T40] Lua：元表
来源：https://fc.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://sz.zhonguo4118.cn

[T41] Perl：Hello World
来源：https://jm.zhonguo7118.cn

print "Hello\n";
来源：https://xm.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://bv.zhonguo1118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://qg.zhonguo4118.cn

[T43] Perl：字符串插值
来源：https://lk.zhonguo4118.cn

"值: $a"
来源：https://jz.zhonguo6118.cn

[T44] Perl：条件
来源：https://wg.zhonguo6118.cn

if ($a > 0) { print "正"; }
来源：https://vs.zhonguo6118.cn

[T45] Perl：数组遍历
来源：https://yv.zhonguo3118.cn

for my $x (@arr) { print $x; }
来源：https://yd.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://qm.zhonguo7118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://xm.zhonguo2118.cn

[T47] Perl：正则捕获
来源：https://vl.zhonguo5118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://zz.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://yx.zhonguo4118.cn

$s =~ s/old/new/g;
来源：https://tp.zhonguo8118.cn

[T49] Perl：函数
来源：https://se.zhonguo6118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://vv.zhonguo1118.cn

[T50] Perl：逐行读文件
来源：https://qg.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://rz.zhonguo6118.cn


<!-- 参考信息 -->