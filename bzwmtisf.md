代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wbp.sufxvd.cn

[R54] 比较两个文件
来源：http://gdy.ehwqpu.com

diff a.txt b.txt
来源：http://fyo.jyoumei.cn

[R55] 压缩与解压
来源：http://ruf.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tqj.ehwqpu.com

[R56] 远程拷贝
来源：http://khn.hnxiangtu.top

scp file user@host:/path/
来源：http://syu.jyoumei.cn

[R57] 远程执行命令
来源：http://zvt.epnwcf.com

ssh user@host 'uptime'
来源：http://ris.pycfn.com

[R58] 下载文件
来源：http://zrd.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxk.uphjek.com

[R59] 发 POST JSON
来源：http://yiv.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xiy.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://tbq.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sre.hnxiangtu.top

[R61] 磁盘占用
来源：http://plu.fehbvm.com

df -h;  du -sh *
来源：http://esq.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://fvj.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://owj.sweek.top

[R63] 内存与进程
来源：http://gag.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://gix.dashuyun.cn

[R64] 结束进程
来源：http://lox.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://sog.hesvh.cn

[R65] 查看端口占用
来源：http://hon.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jtu.hfpthk.cn

[R66] 定时任务
来源：http://thm.aizwys.cn

crontab -e;  crontab -l
来源：http://brc.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://bbg.iojbl.cn

openssl rand -hex 16
来源：http://jyj.fzhhl.top

[R68] 计算文件校验值
来源：http://npr.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zpu.jqgfzy.top

[R69] 生成随机密码
来源：http://sfw.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://zdk.yanxiufei.cn

[R70] 时间戳与互转
来源：http://qit.xziqi.cn

date +%s;  date -d @1700000000
来源：http://jjz.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://fhy.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yez.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://skc.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nwg.gogol.net.cn

[R73] 分割大日志
来源：http://mje.jqgfzy.top

split -l 1000 big.log part_
来源：http://ptg.ctjpmb.com

[R74] 批量重命名
来源：http://scm.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zft.tianlin.xyz

[R75] 导出环境变量
来源：http://qbp.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://rur.xziqi.cn

[R76] 使用临时文件
来源：http://vdf.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ztc.52xcode.cn

[R77] 读取用户输入
来源：http://okn.nanxinkj.top

read -rp "请输入: " ans
来源：http://nzk.yfazqb.com

[R78] 交互式菜单
来源：http://vlo.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bhq.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://iuf.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hbd.meibo888.top

[R80] 查看脚本执行耗时
来源：http://vpf.gogol.net.cn

time ./run.sh
来源：http://udf.ywan-chungtsiang.top

================================================================================
来源：http://uhl.uphjek.com

S. C / C++ 专题
来源：http://ljz.yuanzhike.top

================================================================================
来源：http://qbe.andypj.xyz

[S01] C：Hello World
来源：http://ttq.cheryme.top

#include <stdio.h>
来源：http://xtu.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gnn.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://ppc.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://ngf.jinqigufen.top

[S03] C：读入整数
来源：http://uiz.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://ycy.ydzc1.top

[S04] C：字符串复制
来源：http://fwu.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ill.epnwcf.com

[S05] C：字符串长度
来源：http://eez.feifeiyinyue.top

strlen(s)
来源：http://uja.hfpthk.cn

[S06] C：字符串比较
来源：http://kgi.smart0.xyz

strcmp(a, b) == 0
来源：http://jwj.jinqigufen.top

[S07] C：数组遍历求和
来源：http://bys.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pvg.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://pqv.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pbm.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://qrg.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yau.bjfxy.top

[S10] C：指针与解引用
来源：http://msu.bbcook.cn

int *p = &a;  *p = 5;
来源：http://mzq.ehwqpu.com

[S11] C：逐行读文件
来源：http://rpt.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://jwj.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jwh.xingfuxueyuan.xyz

fclose(f);
来源：http://frr.xylfe.cn

[S12] C：写文件
来源：http://gry.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cpq.yueranfly.top

[S13] C：宏定义
来源：http://xgr.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kky.gaohongyu789.top

[S14] C：枚举
来源：http://gyj.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://nzx.gotoacloud.top

[S15] C：类型转换
来源：http://gfi.quarkkingdee.top

(double) a / b
来源：http://jan.hongshengwenyu.top

[S16] C：位操作置位
来源：http://kle.jiagoushi.top

x |= (1 << 3);
来源：http://taj.tanke756.top

[S17] C：安全拼接字符串
来源：http://phn.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gfw.gzhubu.top

[S18] C：命令行参数
来源：http://yfb.ydzc1.top

int main(int argc, char **argv)
来源：http://jgl.hesvh.cn

[S19] C：快速排序
来源：http://zil.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gmh.sufxvd.cn

[S20] C：二分查找
来源：http://yak.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cax.hammf.cn

[S21] C：字符类别判断
来源：http://tnz.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jnp.xinyue.icu

[S22] C：字符串转数字
来源：http://tcc.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://lzf.svipenyu.cn

[S23] C：随机数
来源：http://ego.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jjm.dashuyun.cn

[S24] C：获取本地时间
来源：http://mbt.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cya.hammf.cn

[S25] C：内存拷贝
来源：http://mew.hfpthk.cn

memcpy(dst, src, n);
来源：http://qul.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://kvn.daria6918.cn

memset(a, 0, sizeof a);
来源：http://cpx.chenjidiqi.icu

[S27] C：定义常量
来源：http://yhq.nwbrower.top

const double PI = 3.14159;
来源：http://nym.shangyingyoupin.top

[S28] C：静态变量
来源：http://bsx.smart0.xyz

static int counter = 0;
来源：http://cbx.cdnleiting.top

[S29] C：变参函数
来源：http://yyp.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wic.sxryk.cn

[S30] C：头文件保护
来源：http://dwp.xinyue.icu

#ifndef X_H
来源：http://hqb.fengsongda.top

#define X_H
来源：http://xlq.tanke756.top

#endif
来源：http://lhz.chenlongwang.top

[S31] C++：Hello World
来源：http://dse.jlsjyb.cn

#include <iostream>
来源：http://wij.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://rbu.xuetiantiany.cn

[S32] C++：字符串
来源：http://kzo.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://ljg.gaohongyu789.top

[S33] C++：vector 增删
来源：http://plr.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xom.fengsongda.top

[S34] C++：遍历 vector
来源：http://weu.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://zai.yanxiufei.cn

[S35] C++：map
来源：http://vej.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aau.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://ngw.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fce.sweek.top

[S37] C++：set
来源：http://qte.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ije.c1oappe.top

[S38] C++：排序
来源：http://dvn.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://drk.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://xku.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://izp.jyoumei.cn

[S40] C++：查找元素
来源：http://npp.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qfj.zhengqikj.top

[S41] C++：类与构造函数
来源：http://gdk.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://roy.sxryk.cn

[S42] C++：继承与虚函数
来源：http://sru.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://lmv.hammf.cn

[S43] C++：智能指针
来源：http://zjq.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://peo.fktsv.cn

[S44] C++：引用传参
来源：http://rgk.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://fps.tianlin.xyz

[S45] C++：lambda
来源：http://kss.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dsh.vqdsnc.cn

[S46] C++：函数模板
来源：http://rfe.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://thx.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://iuo.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://csr.cashguo.top

[S48] C++：逐行读文件
来源：http://ksc.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qys.hnqzz.top

while (std::getline(in, line)) { }
来源：http://icr.chenzaomai.com

[S49] C++：写文件
来源：http://lnq.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vzf.jiagoushi.top

[S50] C++：格式化数字
来源：http://men.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dul.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://ttu.tianlin.xyz

static_cast<double>(a) / b
来源：http://rmv.uphjek.com

[S52] C++：const 与 noexcept
来源：http://ijj.yj20258888.top

int size() const noexcept { return n_; }
来源：http://dfo.ydjk.org.cn

[S53] C++：移动语义
来源：http://fqw.cashguo.top

std::vector<int> w = std::move(v);
来源：http://rfm.jqgfzy.top

[S54] C++：异常处理
来源：http://hrq.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jks.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://mxq.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://txr.yj20258888.top

[S56] C++：optional
来源：http://qbh.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rge.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://bty.cucudq.cn

constexpr int N = 10;
来源：http://bwj.havefunace.top

[S58] C++：命名空间
来源：http://fyp.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://xvv.nanxinkj.top

[S59] C++：静态断言
来源：http://tiz.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vbj.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://qtw.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wxk.yfazqb.com

================================================================================
来源：http://via.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pkk.snrcjt.cn

================================================================================
来源：http://qgm.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://ngi.tanke756.top

println("Hello")
来源：http://ojo.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://hli.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bta.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://yot.yj20258.top

"值: $b"
来源：http://fpw.xziqi.cn

[T04] Kotlin：空安全
来源：http://zlw.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://nlq.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://ejv.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://khv.guannengcc.top

[T06] Kotlin：集合映射
来源：http://tqv.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://idd.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://afy.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://fqt.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://ekr.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://pwy.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://ctq.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://ycy.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://afl.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mkj.epnwcf.com

[T11] Kotlin：协程
来源：http://wej.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://swy.sysykeji.top

[T12] Kotlin：解构声明
来源：http://aqi.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://aub.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://ydy.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://hue.havefunace.top

[T14] Kotlin：循环
来源：http://bkl.meibo888.top

for (i in 1..10) println(i)
来源：http://vle.andypj.xyz

[T15] Kotlin：接口
来源：http://sjo.mhx1999.top

interface Shape { fun area(): Double }
来源：http://del.yj20258.top

[T16] Swift：Hello World
来源：http://mpt.jinghuilouyu.cn

print("Hello")
来源：http://ydg.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://rdp.jianghu66.top

var a = 1;  let b = 2
来源：http://bmm.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://qbg.gogol.net.cn

"值: \(b)"
来源：http://gfe.yj20258.top

[T19] Swift：可选绑定
来源：http://ixe.chenlongwang.top

if let n = opt { print(n) }
来源：http://nsb.sufxvd.cn

[T20] Swift：数组操作
来源：http://ppd.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://lcy.meibo888.top

[T21] Swift：遍历
来源：http://hub.mhx1999.top

for x in a { print(x) }
来源：http://ioa.316326.xyz

[T22] Swift：字典
来源：http://hyx.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://ydn.jinqigfzy.top

[T23] Swift：函数
来源：http://tgt.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dse.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://jgt.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eqy.jiagoushi.top

[T25] Swift：结构体
来源：http://acr.sjlbkw.cn

struct P { var x: Int }
来源：http://pco.daria6918.cn

[T26] Swift：类与重写
来源：http://khf.zdbjq.cn

class A: Base { override func f() {} }
来源：http://cab.yvedp.cn

[T27] Swift：错误处理
来源：http://eqf.fzhhl.top

do { try f() } catch { print(error) }
来源：http://vxb.9152youxi.cn

[T28] Swift：枚举
来源：http://xsv.fehbvm.com

enum Color { case red, green }
来源：http://iro.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://qvv.xinyue.icu

guard let x = opt else { return }
来源：http://auh.tanke756.top

[T30] Swift：协议
来源：http://fin.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://ffe.ppjwa.cn

[T31] Lua：Hello World
来源：http://qco.yj20258.top

print("Hello")
来源：http://hbs.svipenyu.cn

[T32] Lua：局部变量
来源：http://yql.zdbjq.cn

local a = 1
来源：http://zvd.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://ule.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mib.gotoacloud.top

[T34] Lua：遍历表
来源：http://xqn.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://luz.nwbrower.top

[T35] Lua：字典表
来源：http://ofs.yanxiufei.cn

local d = { a = 1 };  d.b = 2
来源：http://qiv.fehbvm.com

[T36] Lua：函数
来源：http://yeg.52xcode.cn

function add(a, b) return a + b end
来源：http://yzz.iojbl.cn

[T37] Lua：字符串拼接
来源：http://iae.zdqjudy.top

"a" .. "b"
来源：http://vfo.yvedp.cn

[T38] Lua：条件
来源：http://gqs.vehdjk.com

if x > 0 then print("正") end
来源：http://cwm.fktsv.cn

[T39] Lua：模式匹配
来源：http://hss.xuetiantiany.cn

string.find(s, "%d+")
来源：http://caq.nanxuanxn.top

[T40] Lua：元表
来源：http://bag.xuanzx.com

setmetatable({}, { __index = base })
来源：http://ldw.wangdashe.top

[T41] Perl：Hello World
来源：http://efy.hnxiangtu.top

print "Hello\n";
来源：http://zuu.yvedp.cn

[T42] Perl：变量类型
来源：http://vkt.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oem.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://wou.fzhhl.top

"值: $a"
来源：http://yea.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://fyk.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://noe.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://byk.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://dom.ydzc1.top

[T46] Perl：哈希操作
来源：http://mne.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jil.meibo888.top

[T47] Perl：正则捕获
来源：http://ded.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vvw.jianghu66.top

[T48] Perl：正则替换
来源：http://fhc.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://vwt.yanxiufei.cn

[T49] Perl：函数
来源：http://ljq.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pjr.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://mjj.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kin.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://ypf.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://sfo.wangdashe.top

println("Hello")
来源：http://qua.jianghu66.top

[T52] Scala：变量
来源：http://phs.jinqigufen.top

val a = 1;  var b = 2
来源：http://pbg.tian-w.cn

[T53] Scala：字符串插值
来源：http://sgl.sjlbkw.cn

s"值: $b"
来源：http://xnx.gotoacloud.top

[T54] Scala：集合映射
来源：http://fve.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://tgw.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://mbn.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://gnv.chenzaomai.com

[T56] Scala：样例类
来源：http://tra.vqdsnc.cn


<!-- 参考信息 -->