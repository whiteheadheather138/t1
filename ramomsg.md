代发 wailian999

echo "${#s}"
来源：https://bv.zhonguo8118.cn

[R22] 截取子串
来源：https://hx.zhonguo6118.cn

echo "${s:0:5}"
来源：https://cd.zhonguo4118.cn

[R23] 字符串替换
来源：https://vn.zhonguo3118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://av.zhonguo1118.cn

[R24] 大小写转换
来源：https://vg.zhonguo6118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://vd.zhonguo2118.cn

[R25] 去后缀 / 去前缀
来源：https://vw.zhonguo7118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://bv.zhonguo2118.cn

[R26] 命令替换
来源：https://ag.zhonguo4118.cn

now=$(date +%F); echo "$now"
来源：https://pk.zhonguo1118.cn

[R27] 算术展开
来源：https://ih.zhonguo8118.cn

echo $((1 + 2 * 3))
来源：https://ik.zhonguo3118.cn

[R28] 浮点运算
来源：https://ak.zhonguo1118.cn

echo "scale=2; 10/3" | bc
来源：https://ej.zhonguo8118.cn

[R29] 定义函数
来源：https://tj.zhonguo4118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://as.zhonguo8118.cn

[R30] 函数返回状态码
来源：https://fs.zhonguo5118.cn

f() { return 0; }; f || echo "失败了"
来源：https://fr.zhonguo3118.cn

[R31] 局部变量
来源：https://sy.zhonguo5118.cn

f() { local x=1; echo "$x"; }
来源：https://bq.zhonguo1118.cn

[R32] 参数个数校验
来源：https://qx.zhonguo2118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://ot.zhonguo6118.cn

[R33] 捕获错误并提示行号
来源：https://cg.zhonguo3118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://vq.zhonguo2118.cn

[R34] 退出时清理
来源：https://td.zhonguo5118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://cc.zhonguo4118.cn

[R35] 后台执行并等待
来源：https://xe.zhonguo6118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://cp.zhonguo4118.cn

[R36] 并发执行多个任务
来源：https://rz.zhonguo5118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://ev.zhonguo2118.cn

[R37] 把输出赋给变量
来源：https://pi.zhonguo7118.cn

files=$(ls -1)
来源：https://vu.zhonguo2118.cn

[R38] 管道串联
来源：https://xz.zhonguo4118.cn

cat a.txt | grep -i error | wc -l
来源：https://il.zhonguo8118.cn

[R39] 重定向标准输出与错误
来源：https://nx.zhonguo2118.cn

cmd > out.log 2>&1
来源：https://sw.zhonguo8118.cn

[R40] 追加写日志
来源：https://wv.zhonguo1118.cn

echo "log" >> out.log
来源：https://av.zhonguo2118.cn

[R41] 丢弃输出
来源：https://ja.zhonguo6118.cn

cmd >/dev/null 2>&1
来源：https://cb.zhonguo8118.cn

[R42] 输入重定向
来源：https://kw.zhonguo5118.cn

wc -l < a.txt
来源：https://di.zhonguo1118.cn

[R43] 按名字查找文件
来源：https://wu.zhonguo1118.cn

find . -name "*.log" -type f
来源：https://np.zhonguo3118.cn

[R44] 按修改时间查找
来源：https://jn.zhonguo5118.cn

find . -mtime -7 -type f
来源：https://ly.zhonguo1118.cn

[R45] 批量删除
来源：https://ej.zhonguo6118.cn

find . -name "*.tmp" -delete
来源：https://wv.zhonguo6118.cn

[R46] 递归替换文件内容
来源：https://np.zhonguo4118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://fs.zhonguo6118.cn

[R47] sed 单行替换
来源：https://ql.zhonguo7118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://gi.zhonguo6118.cn

[R48] awk 取指定列
来源：https://xa.zhonguo8118.cn

awk '{print $1, $3}' a.txt
来源：https://ut.zhonguo3118.cn

[R49] awk 带条件
来源：https://rs.zhonguo2118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://gt.zhonguo3118.cn

[R50] awk 求和
来源：https://qn.zhonguo1118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://rf.zhonguo4118.cn

[R51] 排序去重取前几
来源：https://ig.zhonguo7118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://gy.zhonguo4118.cn

[R52] 统计行数
来源：https://jg.zhonguo3118.cn

wc -l a.txt
来源：https://wo.zhonguo4118.cn

[R53] 查看文件头与实时尾
来源：https://cr.zhonguo5118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://xx.zhonguo2118.cn

[R54] 比较两个文件
来源：https://qn.zhonguo4118.cn

diff a.txt b.txt
来源：https://zg.zhonguo4118.cn

[R55] 压缩与解压
来源：https://ey.zhonguo7118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://ai.zhonguo2118.cn

[R56] 远程拷贝
来源：https://rv.zhonguo7118.cn

scp file user@host:/path/
来源：https://cr.zhonguo6118.cn

[R57] 远程执行命令
来源：https://sn.zhonguo8118.cn

ssh user@host 'uptime'
来源：https://bf.zhonguo1118.cn

[R58] 下载文件
来源：https://qd.zhonguo1118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://pi.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://jw.zhonguo5118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://el.zhonguo1118.cn

[R60] 只看 HTTP 状态码
来源：https://xg.zhonguo1118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://wa.zhonguo8118.cn

[R61] 磁盘占用
来源：https://yj.zhonguo6118.cn

df -h;  du -sh *
来源：https://bl.zhonguo5118.cn

[R62] 找最占空间的文件
来源：https://sf.zhonguo1118.cn

du -ah . | sort -rh | head -10
来源：https://ld.zhonguo7118.cn

[R63] 内存与进程
来源：https://fc.zhonguo7118.cn

free -h;  ps aux | grep nginx
来源：https://dp.zhonguo8118.cn

[R64] 结束进程
来源：https://eh.zhonguo8118.cn

kill -9 $(pgrep -f app.py)
来源：https://xd.zhonguo1118.cn

[R65] 查看端口占用
来源：https://et.zhonguo6118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://uq.zhonguo5118.cn

[R66] 定时任务
来源：https://xf.zhonguo5118.cn

crontab -e;  crontab -l
来源：https://us.zhonguo2118.cn

[R67] 生成随机十六进制串
来源：https://cz.zhonguo4118.cn

openssl rand -hex 16
来源：https://oc.zhonguo4118.cn

[R68] 计算文件校验值
来源：https://ll.zhonguo3118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://kw.zhonguo6118.cn

[R69] 生成随机密码
来源：https://yl.zhonguo7118.cn

head -c 16 /dev/urandom | base64
来源：https://ll.zhonguo4118.cn

[R70] 时间戳与互转
来源：https://gd.zhonguo1118.cn

date +%s;  date -d @1700000000
来源：https://kc.zhonguo3118.cn

[R71] 日期格式化
来源：https://ay.zhonguo3118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://aw.zhonguo8118.cn

[R72] 等待端口就绪
来源：https://zh.zhonguo4118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://te.zhonguo6118.cn

[R73] 分割大日志
来源：https://im.zhonguo6118.cn

split -l 1000 big.log part_
来源：https://rj.zhonguo7118.cn

[R74] 批量重命名
来源：https://qn.zhonguo5118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ww.zhonguo5118.cn

[R75] 导出环境变量
来源：https://ca.zhonguo2118.cn

export PATH="$HOME/bin:$PATH"
来源：https://mm.zhonguo4118.cn

[R76] 使用临时文件
来源：https://vp.zhonguo5118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://fx.zhonguo6118.cn

[R77] 读取用户输入
来源：https://ma.zhonguo2118.cn

read -rp "请输入: " ans
来源：https://bt.zhonguo8118.cn

[R78] 交互式菜单
来源：https://br.zhonguo4118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://sm.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://hy.zhonguo3118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://qk.zhonguo7118.cn

[R80] 查看脚本执行耗时
来源：https://ui.zhonguo6118.cn

time ./run.sh
来源：https://ux.zhonguo2118.cn

================================================================================
来源：https://ea.zhonguo4118.cn

S. C / C++ 专题
来源：https://tq.zhonguo6118.cn

================================================================================
来源：https://oa.zhonguo4118.cn

[S01] C：Hello World
来源：https://cp.zhonguo3118.cn

#include <stdio.h>
来源：https://rf.zhonguo3118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://dn.zhonguo3118.cn

[S02] C：变量与格式化输出
来源：https://ln.zhonguo2118.cn

int a = 10; printf("%d\n", a);
来源：https://eu.zhonguo1118.cn

[S03] C：读入整数
来源：https://uy.zhonguo8118.cn

int x; scanf("%d", &x);
来源：https://nk.zhonguo7118.cn

[S04] C：字符串复制
来源：https://ok.zhonguo1118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://vc.zhonguo3118.cn

[S05] C：字符串长度
来源：https://sb.zhonguo3118.cn

strlen(s)
来源：https://vv.zhonguo3118.cn

[S06] C：字符串比较
来源：https://dt.zhonguo2118.cn

strcmp(a, b) == 0
来源：https://qy.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://jf.zhonguo4118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://yv.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://sw.zhonguo5118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://ei.zhonguo6118.cn

[S09] C：结构体定义与初始化
来源：https://go.zhonguo1118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://hv.zhonguo1118.cn

[S10] C：指针与解引用
来源：https://jz.zhonguo4118.cn

int *p = &a;  *p = 5;
来源：https://ur.zhonguo2118.cn

[S11] C：逐行读文件
来源：https://ck.zhonguo2118.cn

FILE *f = fopen("a.txt", "r");
来源：https://pj.zhonguo5118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ht.zhonguo3118.cn

fclose(f);
来源：https://qs.zhonguo8118.cn

[S12] C：写文件
来源：https://cz.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://hr.zhonguo6118.cn

[S13] C：宏定义
来源：https://sd.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://et.zhonguo6118.cn

[S14] C：枚举
来源：https://fp.zhonguo7118.cn

enum Color { RED, GREEN, BLUE };
来源：https://hx.zhonguo1118.cn

[S15] C：类型转换
来源：https://fm.zhonguo6118.cn

(double) a / b
来源：https://mj.zhonguo7118.cn

[S16] C：位操作置位
来源：https://bm.zhonguo4118.cn

x |= (1 << 3);
来源：https://kk.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://fw.zhonguo8118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://nt.zhonguo5118.cn

[S18] C：命令行参数
来源：https://tl.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://bj.zhonguo6118.cn

[S19] C：快速排序
来源：https://vp.zhonguo2118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://oo.zhonguo8118.cn

[S20] C：二分查找
来源：https://yk.zhonguo3118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://mu.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://ji.zhonguo6118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://ku.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://ib.zhonguo5118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://lf.zhonguo2118.cn

[S23] C：随机数
来源：https://jj.zhonguo2118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://wo.zhonguo7118.cn

[S24] C：获取本地时间
来源：https://gw.zhonguo1118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ir.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://bs.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://nc.zhonguo6118.cn

[S26] C：内存清零
来源：https://wm.zhonguo1118.cn

memset(a, 0, sizeof a);
来源：https://qh.zhonguo4118.cn

[S27] C：定义常量
来源：https://bb.zhonguo4118.cn

const double PI = 3.14159;
来源：https://ks.zhonguo8118.cn

[S28] C：静态变量
来源：https://ig.zhonguo8118.cn

static int counter = 0;
来源：https://wv.zhonguo1118.cn

[S29] C：变参函数
来源：https://tz.zhonguo6118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://np.zhonguo3118.cn

[S30] C：头文件保护
来源：https://gb.zhonguo3118.cn

#ifndef X_H
来源：https://zb.zhonguo7118.cn

#define X_H
来源：https://kw.zhonguo6118.cn

#endif
来源：https://gg.zhonguo5118.cn

[S31] C++：Hello World
来源：https://te.zhonguo7118.cn

#include <iostream>
来源：https://hu.zhonguo5118.cn

int main() { std::cout << "Hello\n"; }
来源：https://bv.zhonguo3118.cn

[S32] C++：字符串
来源：https://yk.zhonguo1118.cn

std::string s = "hi";  s += "!";
来源：https://nz.zhonguo6118.cn

[S33] C++：vector 增删
来源：https://as.zhonguo3118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://xn.zhonguo4118.cn

[S34] C++：遍历 vector
来源：https://ko.zhonguo6118.cn

for (auto &x : v) { std::cout << x; }
来源：https://ap.zhonguo1118.cn

[S35] C++：map
来源：https://cw.zhonguo1118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://dp.zhonguo6118.cn

[S36] C++：unordered_map
来源：https://uy.zhonguo2118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://eb.zhonguo3118.cn

[S37] C++：set
来源：https://qv.zhonguo8118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://wv.zhonguo5118.cn

[S38] C++：排序
来源：https://ps.zhonguo4118.cn

std::sort(v.begin(), v.end());
来源：https://wm.zhonguo2118.cn

[S39] C++：自定义比较器排序
来源：https://qq.zhonguo7118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://cz.zhonguo1118.cn

[S40] C++：查找元素
来源：https://th.zhonguo2118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://qd.zhonguo4118.cn

[S41] C++：类与构造函数
来源：https://zr.zhonguo7118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://od.zhonguo2118.cn

[S42] C++：继承与虚函数
来源：https://fr.zhonguo2118.cn

class B : public Base { public: void f() override {} };
来源：https://mp.zhonguo1118.cn

[S43] C++：智能指针
来源：https://hc.zhonguo3118.cn

auto p = std::make_unique<int>(5);
来源：https://xq.zhonguo8118.cn

[S44] C++：引用传参
来源：https://gr.zhonguo7118.cn

void inc(int &x) { ++x; }
来源：https://oi.zhonguo8118.cn

[S45] C++：lambda
来源：https://xc.zhonguo2118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://at.zhonguo7118.cn

[S46] C++：函数模板
来源：https://ny.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://wf.zhonguo3118.cn

[S47] C++：结构化绑定遍历
来源：https://rm.zhonguo8118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://wy.zhonguo2118.cn

[S48] C++：逐行读文件
来源：https://ej.zhonguo2118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://tx.zhonguo8118.cn

while (std::getline(in, line)) { }
来源：https://bc.zhonguo5118.cn

[S49] C++：写文件
来源：https://cq.zhonguo7118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://no.zhonguo5118.cn

[S50] C++：格式化数字
来源：https://gr.zhonguo5118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://nk.zhonguo6118.cn

[S51] C++：显式类型转换
来源：https://hk.zhonguo2118.cn

static_cast<double>(a) / b
来源：https://tr.zhonguo4118.cn

[S52] C++：const 与 noexcept
来源：https://zz.zhonguo3118.cn

int size() const noexcept { return n_; }
来源：https://lr.zhonguo4118.cn

[S53] C++：移动语义
来源：https://ei.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://hf.zhonguo4118.cn

[S54] C++：异常处理
来源：https://ft.zhonguo3118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ar.zhonguo8118.cn

[S55] C++：结构化绑定
来源：https://kc.zhonguo8118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://jf.zhonguo5118.cn

[S56] C++：optional
来源：https://fa.zhonguo8118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://dn.zhonguo3118.cn

[S57] C++：编译期常量
来源：https://hd.zhonguo7118.cn

constexpr int N = 10;
来源：https://sa.zhonguo5118.cn

[S58] C++：命名空间
来源：https://dm.zhonguo2118.cn

namespace ns { int f() { return 1; } }
来源：https://sc.zhonguo6118.cn

[S59] C++：静态断言
来源：https://ze.zhonguo8118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ey.zhonguo4118.cn

[S60] C++：遍历并删除元素
来源：https://dz.zhonguo5118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://ak.zhonguo3118.cn

================================================================================
来源：https://nw.zhonguo8118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://ct.zhonguo8118.cn

================================================================================
来源：https://oq.zhonguo6118.cn

[T01] Kotlin：Hello World
来源：https://tg.zhonguo8118.cn

println("Hello")
来源：https://cn.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://bi.zhonguo4118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://dh.zhonguo7118.cn

[T03] Kotlin：字符串模板
来源：https://pr.zhonguo5118.cn

"值: $b"
来源：https://ri.zhonguo5118.cn

[T04] Kotlin：空安全
来源：https://pi.zhonguo5118.cn

val n: String? = null;  n?.length
来源：https://eu.zhonguo8118.cn

[T05] Kotlin：when 表达式
来源：https://pn.zhonguo1118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://kz.zhonguo7118.cn

[T06] Kotlin：集合映射
来源：https://gr.zhonguo7118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://cs.zhonguo4118.cn

[T07] Kotlin：集合过滤
来源：https://ag.zhonguo3118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://si.zhonguo5118.cn

[T08] Kotlin：数据类
来源：https://ei.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://ow.zhonguo5118.cn

[T09] Kotlin：扩展函数
来源：https://cm.zhonguo1118.cn

fun String.exclaim() = this + "!"
来源：https://ev.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://xb.zhonguo1118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://jp.zhonguo4118.cn

[T11] Kotlin：协程
来源：https://xt.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://gl.zhonguo8118.cn

[T12] Kotlin：解构声明
来源：https://rw.zhonguo7118.cn

val (a, b) = Pair(1, 2)
来源：https://du.zhonguo5118.cn

[T13] Kotlin：只读 Map
来源：https://mj.zhonguo7118.cn

val m = mapOf("a" to 1)
来源：https://oz.zhonguo4118.cn

[T14] Kotlin：循环
来源：https://gy.zhonguo1118.cn

for (i in 1..10) println(i)
来源：https://nv.zhonguo1118.cn

[T15] Kotlin：接口
来源：https://vf.zhonguo2118.cn

interface Shape { fun area(): Double }
来源：https://pt.zhonguo1118.cn

[T16] Swift：Hello World
来源：https://jv.zhonguo8118.cn

print("Hello")
来源：https://de.zhonguo3118.cn

[T17] Swift：变量与常量
来源：https://sa.zhonguo8118.cn

var a = 1;  let b = 2
来源：https://qf.zhonguo3118.cn

[T18] Swift：字符串插值
来源：https://iz.zhonguo7118.cn

"值: \(b)"
来源：https://kn.zhonguo3118.cn

[T19] Swift：可选绑定
来源：https://xl.zhonguo8118.cn

if let n = opt { print(n) }
来源：https://wi.zhonguo4118.cn

[T20] Swift：数组操作
来源：https://wv.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://xl.zhonguo3118.cn

[T21] Swift：遍历
来源：https://ys.zhonguo3118.cn

for x in a { print(x) }
来源：https://kd.zhonguo4118.cn

[T22] Swift：字典
来源：https://be.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://yz.zhonguo8118.cn

[T23] Swift：函数
来源：https://bq.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://gt.zhonguo1118.cn

[T24] Swift：闭包
来源：https://wb.zhonguo8118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://sz.zhonguo7118.cn


<!-- 参考信息 -->