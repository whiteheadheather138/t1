代发 wailian999

cmd >/dev/null 2>&1
来源：https://xb.zhonguo7118.cn

[R42] 输入重定向
来源：https://qg.zhonguo4118.cn

wc -l < a.txt
来源：https://dq.zhonguo3118.cn

[R43] 按名字查找文件
来源：https://jy.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://ts.zhonguo8118.cn

[R44] 按修改时间查找
来源：https://ik.zhonguo2118.cn

find . -mtime -7 -type f
来源：https://qi.zhonguo3118.cn

[R45] 批量删除
来源：https://by.zhonguo1118.cn

find . -name "*.tmp" -delete
来源：https://pn.zhonguo4118.cn

[R46] 递归替换文件内容
来源：https://ls.zhonguo8118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://fr.zhonguo6118.cn

[R47] sed 单行替换
来源：https://zm.zhonguo2118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://em.zhonguo7118.cn

[R48] awk 取指定列
来源：https://wz.zhonguo4118.cn

awk '{print $1, $3}' a.txt
来源：https://dy.zhonguo4118.cn

[R49] awk 带条件
来源：https://qc.zhonguo7118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://lv.zhonguo1118.cn

[R50] awk 求和
来源：https://qk.zhonguo3118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://un.zhonguo5118.cn

[R51] 排序去重取前几
来源：https://ws.zhonguo6118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://un.zhonguo1118.cn

[R52] 统计行数
来源：https://sk.zhonguo1118.cn

wc -l a.txt
来源：https://ho.zhonguo7118.cn

[R53] 查看文件头与实时尾
来源：https://cp.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://xr.zhonguo4118.cn

[R54] 比较两个文件
来源：https://xq.zhonguo1118.cn

diff a.txt b.txt
来源：https://dg.zhonguo4118.cn

[R55] 压缩与解压
来源：https://nt.zhonguo5118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://if.zhonguo8118.cn

[R56] 远程拷贝
来源：https://ct.zhonguo2118.cn

scp file user@host:/path/
来源：https://wb.zhonguo2118.cn

[R57] 远程执行命令
来源：https://vb.zhonguo5118.cn

ssh user@host 'uptime'
来源：https://mq.zhonguo1118.cn

[R58] 下载文件
来源：https://fi.zhonguo8118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://do.zhonguo8118.cn

[R59] 发 POST JSON
来源：https://hc.zhonguo2118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://lg.zhonguo5118.cn

[R60] 只看 HTTP 状态码
来源：https://yi.zhonguo1118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://ji.zhonguo1118.cn

[R61] 磁盘占用
来源：https://kv.zhonguo7118.cn

df -h;  du -sh *
来源：https://ew.zhonguo2118.cn

[R62] 找最占空间的文件
来源：https://vm.zhonguo2118.cn

du -ah . | sort -rh | head -10
来源：https://uu.zhonguo2118.cn

[R63] 内存与进程
来源：https://ei.zhonguo4118.cn

free -h;  ps aux | grep nginx
来源：https://oe.zhonguo1118.cn

[R64] 结束进程
来源：https://cy.zhonguo2118.cn

kill -9 $(pgrep -f app.py)
来源：https://rq.zhonguo8118.cn

[R65] 查看端口占用
来源：https://av.zhonguo7118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://ko.zhonguo4118.cn

[R66] 定时任务
来源：https://ln.zhonguo3118.cn

crontab -e;  crontab -l
来源：https://ey.zhonguo3118.cn

[R67] 生成随机十六进制串
来源：https://je.zhonguo6118.cn

openssl rand -hex 16
来源：https://dw.zhonguo1118.cn

[R68] 计算文件校验值
来源：https://rv.zhonguo4118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://oh.zhonguo8118.cn

[R69] 生成随机密码
来源：https://gq.zhonguo5118.cn

head -c 16 /dev/urandom | base64
来源：https://iv.zhonguo2118.cn

[R70] 时间戳与互转
来源：https://yy.zhonguo5118.cn

date +%s;  date -d @1700000000
来源：https://fw.zhonguo6118.cn

[R71] 日期格式化
来源：https://iz.zhonguo7118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ar.zhonguo4118.cn

[R72] 等待端口就绪
来源：https://ab.zhonguo5118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://pn.zhonguo4118.cn

[R73] 分割大日志
来源：https://op.zhonguo5118.cn

split -l 1000 big.log part_
来源：https://ge.zhonguo6118.cn

[R74] 批量重命名
来源：https://em.zhonguo6118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ii.zhonguo7118.cn

[R75] 导出环境变量
来源：https://rd.zhonguo3118.cn

export PATH="$HOME/bin:$PATH"
来源：https://iv.zhonguo2118.cn

[R76] 使用临时文件
来源：https://ny.zhonguo7118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://bf.zhonguo4118.cn

[R77] 读取用户输入
来源：https://bh.zhonguo3118.cn

read -rp "请输入: " ans
来源：https://fj.zhonguo6118.cn

[R78] 交互式菜单
来源：https://gq.zhonguo6118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://on.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://uz.zhonguo8118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://nf.zhonguo3118.cn

[R80] 查看脚本执行耗时
来源：https://fr.zhonguo6118.cn

time ./run.sh
来源：https://ca.zhonguo4118.cn

================================================================================
来源：https://rb.zhonguo3118.cn

S. C / C++ 专题
来源：https://ap.zhonguo6118.cn

================================================================================
来源：https://wp.zhonguo8118.cn

[S01] C：Hello World
来源：https://oy.zhonguo7118.cn

#include <stdio.h>
来源：https://qa.zhonguo6118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://dd.zhonguo2118.cn

[S02] C：变量与格式化输出
来源：https://py.zhonguo4118.cn

int a = 10; printf("%d\n", a);
来源：https://il.zhonguo5118.cn

[S03] C：读入整数
来源：https://no.zhonguo2118.cn

int x; scanf("%d", &x);
来源：https://bb.zhonguo3118.cn

[S04] C：字符串复制
来源：https://yu.zhonguo1118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://dd.zhonguo6118.cn

[S05] C：字符串长度
来源：https://pd.zhonguo3118.cn

strlen(s)
来源：https://ph.zhonguo1118.cn

[S06] C：字符串比较
来源：https://by.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://ey.zhonguo3118.cn

[S07] C：数组遍历求和
来源：https://le.zhonguo5118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://lj.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://nt.zhonguo3118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://md.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://hq.zhonguo3118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://sy.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://zl.zhonguo5118.cn

int *p = &a;  *p = 5;
来源：https://rx.zhonguo2118.cn

[S11] C：逐行读文件
来源：https://ip.zhonguo1118.cn

FILE *f = fopen("a.txt", "r");
来源：https://hf.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://dk.zhonguo3118.cn

fclose(f);
来源：https://zv.zhonguo3118.cn

[S12] C：写文件
来源：https://qo.zhonguo7118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://pj.zhonguo2118.cn

[S13] C：宏定义
来源：https://gt.zhonguo5118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://gl.zhonguo7118.cn

[S14] C：枚举
来源：https://mp.zhonguo2118.cn

enum Color { RED, GREEN, BLUE };
来源：https://dz.zhonguo8118.cn

[S15] C：类型转换
来源：https://de.zhonguo4118.cn

(double) a / b
来源：https://of.zhonguo2118.cn

[S16] C：位操作置位
来源：https://xz.zhonguo1118.cn

x |= (1 << 3);
来源：https://ne.zhonguo7118.cn

[S17] C：安全拼接字符串
来源：https://ip.zhonguo8118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ys.zhonguo7118.cn

[S18] C：命令行参数
来源：https://cv.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://dx.zhonguo6118.cn

[S19] C：快速排序
来源：https://va.zhonguo5118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://kc.zhonguo7118.cn

[S20] C：二分查找
来源：https://go.zhonguo2118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://ey.zhonguo1118.cn

[S21] C：字符类别判断
来源：https://kg.zhonguo5118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://ev.zhonguo6118.cn

[S22] C：字符串转数字
来源：https://iv.zhonguo4118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://qm.zhonguo7118.cn

[S23] C：随机数
来源：https://bk.zhonguo8118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://uk.zhonguo6118.cn

[S24] C：获取本地时间
来源：https://rg.zhonguo8118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ua.zhonguo2118.cn

[S25] C：内存拷贝
来源：https://an.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://qy.zhonguo4118.cn

[S26] C：内存清零
来源：https://uk.zhonguo1118.cn

memset(a, 0, sizeof a);
来源：https://gv.zhonguo2118.cn

[S27] C：定义常量
来源：https://er.zhonguo6118.cn

const double PI = 3.14159;
来源：https://mp.zhonguo7118.cn

[S28] C：静态变量
来源：https://oz.zhonguo6118.cn

static int counter = 0;
来源：https://ha.zhonguo5118.cn

[S29] C：变参函数
来源：https://kg.zhonguo1118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://io.zhonguo3118.cn

[S30] C：头文件保护
来源：https://oh.zhonguo2118.cn

#ifndef X_H
来源：https://tn.zhonguo4118.cn

#define X_H
来源：https://is.zhonguo8118.cn

#endif
来源：https://lw.zhonguo4118.cn

[S31] C++：Hello World
来源：https://zn.zhonguo4118.cn

#include <iostream>
来源：https://vj.zhonguo8118.cn

int main() { std::cout << "Hello\n"; }
来源：https://yy.zhonguo7118.cn

[S32] C++：字符串
来源：https://xm.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://kd.zhonguo3118.cn

[S33] C++：vector 增删
来源：https://gx.zhonguo3118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://im.zhonguo6118.cn

[S34] C++：遍历 vector
来源：https://tb.zhonguo8118.cn

for (auto &x : v) { std::cout << x; }
来源：https://uv.zhonguo4118.cn

[S35] C++：map
来源：https://gc.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://sc.zhonguo3118.cn

[S36] C++：unordered_map
来源：https://oq.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ul.zhonguo3118.cn

[S37] C++：set
来源：https://xo.zhonguo6118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://gw.zhonguo1118.cn

[S38] C++：排序
来源：https://dl.zhonguo6118.cn

std::sort(v.begin(), v.end());
来源：https://hx.zhonguo3118.cn

[S39] C++：自定义比较器排序
来源：https://dp.zhonguo1118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://xz.zhonguo1118.cn

[S40] C++：查找元素
来源：https://if.zhonguo7118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://jj.zhonguo6118.cn

[S41] C++：类与构造函数
来源：https://jn.zhonguo5118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://jx.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://zc.zhonguo8118.cn

class B : public Base { public: void f() override {} };
来源：https://ji.zhonguo8118.cn

[S43] C++：智能指针
来源：https://nf.zhonguo3118.cn

auto p = std::make_unique<int>(5);
来源：https://od.zhonguo6118.cn

[S44] C++：引用传参
来源：https://ey.zhonguo3118.cn

void inc(int &x) { ++x; }
来源：https://so.zhonguo7118.cn

[S45] C++：lambda
来源：https://rq.zhonguo6118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://cs.zhonguo7118.cn

[S46] C++：函数模板
来源：https://qz.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://eo.zhonguo2118.cn

[S47] C++：结构化绑定遍历
来源：https://oh.zhonguo3118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://gj.zhonguo6118.cn

[S48] C++：逐行读文件
来源：https://go.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://wu.zhonguo6118.cn

while (std::getline(in, line)) { }
来源：https://kq.zhonguo4118.cn

[S49] C++：写文件
来源：https://xi.zhonguo5118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://ey.zhonguo2118.cn

[S50] C++：格式化数字
来源：https://hn.zhonguo5118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://ko.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://zv.zhonguo8118.cn

static_cast<double>(a) / b
来源：https://ux.zhonguo4118.cn

[S52] C++：const 与 noexcept
来源：https://fv.zhonguo7118.cn

int size() const noexcept { return n_; }
来源：https://tw.zhonguo5118.cn

[S53] C++：移动语义
来源：https://pl.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://gv.zhonguo3118.cn

[S54] C++：异常处理
来源：https://dw.zhonguo2118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://hl.zhonguo8118.cn

[S55] C++：结构化绑定
来源：https://rn.zhonguo3118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ou.zhonguo7118.cn

[S56] C++：optional
来源：https://pe.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://wf.zhonguo8118.cn

[S57] C++：编译期常量
来源：https://js.zhonguo5118.cn

constexpr int N = 10;
来源：https://gg.zhonguo3118.cn

[S58] C++：命名空间
来源：https://tt.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://sn.zhonguo7118.cn

[S59] C++：静态断言
来源：https://wr.zhonguo4118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://za.zhonguo2118.cn

[S60] C++：遍历并删除元素
来源：https://se.zhonguo2118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://sn.zhonguo5118.cn

================================================================================
来源：https://yh.zhonguo5118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://yc.zhonguo6118.cn

================================================================================
来源：https://xx.zhonguo7118.cn

[T01] Kotlin：Hello World
来源：https://el.zhonguo4118.cn

println("Hello")
来源：https://kh.zhonguo2118.cn

[T02] Kotlin：变量
来源：https://zm.zhonguo6118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://mz.zhonguo3118.cn

[T03] Kotlin：字符串模板
来源：https://hv.zhonguo2118.cn

"值: $b"
来源：https://us.zhonguo7118.cn

[T04] Kotlin：空安全
来源：https://cj.zhonguo1118.cn

val n: String? = null;  n?.length
来源：https://cq.zhonguo5118.cn

[T05] Kotlin：when 表达式
来源：https://bi.zhonguo5118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://ci.zhonguo1118.cn

[T06] Kotlin：集合映射
来源：https://qu.zhonguo1118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://zq.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://lp.zhonguo1118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://po.zhonguo8118.cn

[T08] Kotlin：数据类
来源：https://cs.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://cr.zhonguo6118.cn

[T09] Kotlin：扩展函数
来源：https://bv.zhonguo6118.cn

fun String.exclaim() = this + "!"
来源：https://mn.zhonguo2118.cn

[T10] Kotlin：默认参数
来源：https://tg.zhonguo3118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://zu.zhonguo7118.cn

[T11] Kotlin：协程
来源：https://or.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://ad.zhonguo5118.cn

[T12] Kotlin：解构声明
来源：https://rp.zhonguo2118.cn

val (a, b) = Pair(1, 2)
来源：https://fq.zhonguo3118.cn

[T13] Kotlin：只读 Map
来源：https://hy.zhonguo8118.cn

val m = mapOf("a" to 1)
来源：https://gk.zhonguo1118.cn

[T14] Kotlin：循环
来源：https://yd.zhonguo3118.cn

for (i in 1..10) println(i)
来源：https://ky.zhonguo5118.cn

[T15] Kotlin：接口
来源：https://pa.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://no.zhonguo4118.cn

[T16] Swift：Hello World
来源：https://mx.zhonguo1118.cn

print("Hello")
来源：https://qu.zhonguo3118.cn

[T17] Swift：变量与常量
来源：https://gv.zhonguo3118.cn

var a = 1;  let b = 2
来源：https://oq.zhonguo7118.cn

[T18] Swift：字符串插值
来源：https://vx.zhonguo6118.cn

"值: \(b)"
来源：https://ab.zhonguo7118.cn

[T19] Swift：可选绑定
来源：https://eb.zhonguo4118.cn

if let n = opt { print(n) }
来源：https://qv.zhonguo3118.cn

[T20] Swift：数组操作
来源：https://qb.zhonguo8118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://cn.zhonguo3118.cn

[T21] Swift：遍历
来源：https://vu.zhonguo3118.cn

for x in a { print(x) }
来源：https://bj.zhonguo3118.cn

[T22] Swift：字典
来源：https://kc.zhonguo2118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://yd.zhonguo7118.cn

[T23] Swift：函数
来源：https://ue.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://be.zhonguo6118.cn

[T24] Swift：闭包
来源：https://tp.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://cn.zhonguo8118.cn

[T25] Swift：结构体
来源：https://gq.zhonguo5118.cn

struct P { var x: Int }
来源：https://qf.zhonguo7118.cn

[T26] Swift：类与重写
来源：https://mp.zhonguo7118.cn

class A: Base { override func f() {} }
来源：https://og.zhonguo7118.cn

[T27] Swift：错误处理
来源：https://nf.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://lc.zhonguo5118.cn

[T28] Swift：枚举
来源：https://ub.zhonguo8118.cn

enum Color { case red, green }
来源：https://mx.zhonguo6118.cn

[T29] Swift：guard 提前返回
来源：https://nn.zhonguo3118.cn

guard let x = opt else { return }
来源：https://bn.zhonguo4118.cn

[T30] Swift：协议
来源：https://rp.zhonguo6118.cn

protocol Shape { func area() -> Double }
来源：https://ys.zhonguo5118.cn

[T31] Lua：Hello World
来源：https://gq.zhonguo5118.cn

print("Hello")
来源：https://gp.zhonguo5118.cn

[T32] Lua：局部变量
来源：https://dl.zhonguo2118.cn

local a = 1
来源：https://pg.zhonguo2118.cn

[T33] Lua：表（数组）
来源：https://bb.zhonguo2118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://on.zhonguo5118.cn

[T34] Lua：遍历表
来源：https://fi.zhonguo5118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://ml.zhonguo6118.cn

[T35] Lua：字典表
来源：https://sc.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://mu.zhonguo6118.cn

[T36] Lua：函数
来源：https://zv.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://ho.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://lz.zhonguo3118.cn

"a" .. "b"
来源：https://ue.zhonguo3118.cn

[T38] Lua：条件
来源：https://ww.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://rw.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://yw.zhonguo5118.cn

string.find(s, "%d+")
来源：https://ue.zhonguo8118.cn

[T40] Lua：元表
来源：https://jt.zhonguo7118.cn

setmetatable({}, { __index = base })
来源：https://sj.zhonguo8118.cn

[T41] Perl：Hello World
来源：https://pr.zhonguo5118.cn

print "Hello\n";
来源：https://xf.zhonguo3118.cn

[T42] Perl：变量类型
来源：https://yz.zhonguo3118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://tn.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://yh.zhonguo6118.cn

"值: $a"
来源：https://by.zhonguo5118.cn

[T44] Perl：条件
来源：https://be.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://fv.zhonguo6118.cn


<!-- 参考信息 -->