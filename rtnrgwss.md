代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ndn.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://efa.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fyh.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://dtp.yuxming.cn

df -h;  du -sh *
来源：http://hrt.yangfankeji.com

[R62] 找最占空间的文件
来源：http://vyq.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://zan.yuxming.cn

[R63] 内存与进程
来源：http://zoy.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://jyb.yfazqb.com

[R64] 结束进程
来源：http://wwm.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://ztq.jyoumei.cn

[R65] 查看端口占用
来源：http://dbr.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gjh.haohaochexian.top

[R66] 定时任务
来源：http://dkd.ivvv.top

crontab -e;  crontab -l
来源：http://lko.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://ogf.mhx1999.top

openssl rand -hex 16
来源：http://wed.sysykeji.top

[R68] 计算文件校验值
来源：http://yll.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://ain.cqqwz.cn

[R69] 生成随机密码
来源：http://owa.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://ybm.uphjek.com

[R70] 时间戳与互转
来源：http://lin.sweek.top

date +%s;  date -d @1700000000
来源：http://vmv.jqgfzy.top

[R71] 日期格式化
来源：http://lxf.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://est.yvedp.cn

[R72] 等待端口就绪
来源：http://wsl.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dbi.feifeiyinyue.top

[R73] 分割大日志
来源：http://jnb.hcnkem.com

split -l 1000 big.log part_
来源：http://tja.yj20258888.top

[R74] 批量重命名
来源：http://csa.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://brr.sxryk.cn

[R75] 导出环境变量
来源：http://nxk.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://tpt.zdbjq.cn

[R76] 使用临时文件
来源：http://uub.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kzz.zhongyouzk.top

[R77] 读取用户输入
来源：http://txd.bjfxy.top

read -rp "请输入: " ans
来源：http://sru.dianchejie.cn

[R78] 交互式菜单
来源：http://yka.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kvy.bjfxy.top

[R79] 解析命令行选项
来源：http://ktr.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aoc.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://tkq.hongshengwenyu.top

time ./run.sh
来源：http://awa.zhoulong.xyz

================================================================================
来源：http://xit.hysaishi.cn

S. C / C++ 专题
来源：http://sxo.vqdsnc.cn

================================================================================
来源：http://qqn.guannengcc.top

[S01] C：Hello World
来源：http://teq.andypj.xyz

#include <stdio.h>
来源：http://oqm.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yku.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://guq.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://ooa.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://awf.sysykeji.top

int x; scanf("%d", &x);
来源：http://phj.hcnkem.com

[S04] C：字符串复制
来源：http://veb.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://pkr.guowangkeji.top

[S05] C：字符串长度
来源：http://kli.tanke756.top

strlen(s)
来源：http://kni.guowangkeji.top

[S06] C：字符串比较
来源：http://aha.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://sqg.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://pim.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bfg.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://iwu.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://trd.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://kkw.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dyg.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://yyb.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://nrg.xziqi.cn

[S11] C：逐行读文件
来源：http://pyd.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://ada.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jms.sufxvd.cn

fclose(f);
来源：http://zcp.bjfxy.top

[S12] C：写文件
来源：http://syw.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://laa.shuidangran.top

[S13] C：宏定义
来源：http://ysr.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nzw.yj20258.top

[S14] C：枚举
来源：http://oyd.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://uel.ydzc1.top

[S15] C：类型转换
来源：http://inr.xuanzx.com

(double) a / b
来源：http://spl.yuanzhike.top

[S16] C：位操作置位
来源：http://jlw.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://kop.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://ymp.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fox.aizwys.cn

[S18] C：命令行参数
来源：http://lmx.yangfankeji.com

int main(int argc, char **argv)
来源：http://wax.sysykeji.top

[S19] C：快速排序
来源：http://wwf.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://cnv.0kj1m.cn

[S20] C：二分查找
来源：http://nml.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pqh.zhixingplan.top

[S21] C：字符类别判断
来源：http://xqk.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jew.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://ljj.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://mwk.yuanzhike.top

[S23] C：随机数
来源：http://rvr.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://wcf.meibo888.top

[S24] C：获取本地时间
来源：http://pez.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eyo.epnwcf.com

[S25] C：内存拷贝
来源：http://mkp.cdnleiting.top

memcpy(dst, src, n);
来源：http://yne.ppjwa.cn

[S26] C：内存清零
来源：http://kkd.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://fyi.meibo888.top

[S27] C：定义常量
来源：http://uls.gaohongyu789.top

const double PI = 3.14159;
来源：http://cpg.gzhubu.top

[S28] C：静态变量
来源：http://ahj.kuanghao11.cn

static int counter = 0;
来源：http://lfk.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://ykk.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mkn.xuetiantiany.cn

[S30] C：头文件保护
来源：http://oww.zhengqikj.top

#ifndef X_H
来源：http://jwu.hysaishi.cn

#define X_H
来源：http://lhc.fengsongda.top

#endif
来源：http://txc.zycfv.cn

[S31] C++：Hello World
来源：http://jii.guannengcc.top

#include <iostream>
来源：http://hmt.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://vha.hywenlv.cn

[S32] C++：字符串
来源：http://mra.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://jui.zdbjq.cn

[S33] C++：vector 增删
来源：http://qmy.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dhr.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://ial.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://dkp.guowangkeji.top

[S35] C++：map
来源：http://pnp.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://umg.svipenyu.cn

[S36] C++：unordered_map
来源：http://otm.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwc.ydzc1.top

[S37] C++：set
来源：http://loc.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bml.chenjidiqi.icu

[S38] C++：排序
来源：http://ewn.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://lsn.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://wur.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pqt.haohaochexian.top

[S40] C++：查找元素
来源：http://usb.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://exo.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://puu.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dun.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://jaq.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://mxy.gotoacloud.top

[S43] C++：智能指针
来源：http://rvv.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://tku.gaohongyu789.top

[S44] C++：引用传参
来源：http://ntn.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://dkw.zhengqikj.top

[S45] C++：lambda
来源：http://ahb.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://rqh.hcnkem.com

[S46] C++：函数模板
来源：http://mue.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gae.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://gld.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hcj.dianchejie.cn

[S48] C++：逐行读文件
来源：http://ncc.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lif.yuxming.cn

while (std::getline(in, line)) { }
来源：http://rzm.yj20258.top

[S49] C++：写文件
来源：http://pnm.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eab.haohaochexian.top

[S50] C++：格式化数字
来源：http://tvb.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fks.xylfe.cn

[S51] C++：显式类型转换
来源：http://vks.gaohongyu789.top

static_cast<double>(a) / b
来源：http://oqp.316326.xyz

[S52] C++：const 与 noexcept
来源：http://iha.316326.xyz

int size() const noexcept { return n_; }
来源：http://ylo.haohaochexian.top

[S53] C++：移动语义
来源：http://txh.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://heo.ydzc1.top

[S54] C++：异常处理
来源：http://sgv.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pny.nanxinkj.top

[S55] C++：结构化绑定
来源：http://hlq.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zot.dashuyun.cn

[S56] C++：optional
来源：http://urv.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fti.52xcode.cn

[S57] C++：编译期常量
来源：http://rrt.yangfankeji.com

constexpr int N = 10;
来源：http://isl.sjlbkw.cn

[S58] C++：命名空间
来源：http://bgs.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://wwc.redwolf501.top

[S59] C++：静态断言
来源：http://vzp.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ryn.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://nyw.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lgm.cashguo.top

================================================================================
来源：http://pun.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mar.shanyushiyangtech.top

================================================================================
来源：http://hjv.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://udf.zycfv.cn

println("Hello")
来源：http://kse.xuanzx.com

[T02] Kotlin：变量
来源：http://det.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ono.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://pec.zhijiandao.cn

"值: $b"
来源：http://vll.jiagoushi.top

[T04] Kotlin：空安全
来源：http://oem.daxiang520.top

val n: String? = null;  n?.length
来源：http://wio.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://dgg.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fob.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://bub.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pfv.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://cqo.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://enn.haohaochexian.top

[T08] Kotlin：数据类
来源：http://yrc.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://tsy.yj20258.top

[T09] Kotlin：扩展函数
来源：http://nsm.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://bgc.mhx1999.top

[T10] Kotlin：默认参数
来源：http://xaf.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://own.sufxvd.cn

[T11] Kotlin：协程
来源：http://kcp.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ngv.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://hyf.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://tku.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://arv.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://umm.zhengqikj.top

[T14] Kotlin：循环
来源：http://aue.gotoacloud.top

for (i in 1..10) println(i)
来源：http://arj.chenzaomai.com

[T15] Kotlin：接口
来源：http://rjd.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://gxh.yfazqb.com

[T16] Swift：Hello World
来源：http://bop.epnwcf.com

print("Hello")
来源：http://fcx.sysykeji.top

[T17] Swift：变量与常量
来源：http://jwq.guannengcc.top

var a = 1;  let b = 2
来源：http://ehg.zhengqikj.top

[T18] Swift：字符串插值
来源：http://urt.sxryk.cn

"值: \(b)"
来源：http://fhv.guannengcc.top

[T19] Swift：可选绑定
来源：http://fxf.zhoulong.xyz

if let n = opt { print(n) }
来源：http://ewp.vehdjk.com

[T20] Swift：数组操作
来源：http://gaq.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://icg.guannengcc.top

[T21] Swift：遍历
来源：http://pug.pengpengdd.cyou

for x in a { print(x) }
来源：http://ojd.epnwcf.com

[T22] Swift：字典
来源：http://uoj.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://dpa.zycfv.cn

[T23] Swift：函数
来源：http://kpv.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://utb.zhiwuduotai.top

[T24] Swift：闭包
来源：http://oce.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://exs.hnqzz.top

[T25] Swift：结构体
来源：http://isj.hcnkem.com

struct P { var x: Int }
来源：http://jiy.9152youxi.cn

[T26] Swift：类与重写
来源：http://hwi.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://mex.jianghu66.top

[T27] Swift：错误处理
来源：http://bkr.redwolf501.top

do { try f() } catch { print(error) }
来源：http://ysr.svipenyu.cn

[T28] Swift：枚举
来源：http://zdf.fengsongda.top

enum Color { case red, green }
来源：http://kpq.tarul.cn

[T29] Swift：guard 提前返回
来源：http://hkm.cqqwz.cn

guard let x = opt else { return }
来源：http://luh.feifeiyinyue.top

[T30] Swift：协议
来源：http://qbk.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://xrn.aibaodan.cn

[T31] Lua：Hello World
来源：http://edl.vehdjk.com

print("Hello")
来源：http://uuq.fktsv.cn

[T32] Lua：局部变量
来源：http://umz.hammf.cn

local a = 1
来源：http://ucb.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://skb.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://awi.ctjpmb.com

[T34] Lua：遍历表
来源：http://prb.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zov.fktsv.cn

[T35] Lua：字典表
来源：http://oox.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://qli.fanxiaobao.xyz

[T36] Lua：函数
来源：http://hfa.chenzaomai.com

function add(a, b) return a + b end
来源：http://xqh.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://rzo.gotoacloud.top

"a" .. "b"
来源：http://kru.c1oappe.top

[T38] Lua：条件
来源：http://jgh.tanke756.top

if x > 0 then print("正") end
来源：http://whk.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://jqr.jiagoushi.top

string.find(s, "%d+")
来源：http://tbs.hesvh.cn

[T40] Lua：元表
来源：http://adp.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://dzu.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://gct.jqgfzy.top

print "Hello\n";
来源：http://wgd.xziqi.cn

[T42] Perl：变量类型
来源：http://vzd.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fat.yuxming.cn

[T43] Perl：字符串插值
来源：http://skb.xingfuxueyuan.xyz

"值: $a"
来源：http://mny.bjfxy.top

[T44] Perl：条件
来源：http://hzm.sweek.top

if ($a > 0) { print "正"; }
来源：http://vvq.tian-w.cn

[T45] Perl：数组遍历
来源：http://ywf.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://dgu.xziqi.cn

[T46] Perl：哈希操作
来源：http://goc.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vhq.yongpay.top

[T47] Perl：正则捕获
来源：http://vpe.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rxv.yueranfly.top

[T48] Perl：正则替换
来源：http://gas.sysykeji.top

$s =~ s/old/new/g;
来源：http://oco.zdbjq.cn

[T49] Perl：函数
来源：http://dju.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lkc.yvedp.cn

[T50] Perl：逐行读文件
来源：http://fjf.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kwf.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://zqr.guowangkeji.top

[T51] Scala：Hello World
来源：http://bqs.guannengcc.top

println("Hello")
来源：http://jht.wangdashe.top

[T52] Scala：变量
来源：http://wvj.cdnleiting.top

val a = 1;  var b = 2
来源：http://jrx.guowangkeji.top

[T53] Scala：字符串插值
来源：http://gag.zhongyouzk.top

s"值: $b"
来源：http://pac.redwolf501.top

[T54] Scala：集合映射
来源：http://hva.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://rtp.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://zfm.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xko.xuanzx.com

[T56] Scala：样例类
来源：http://mhn.yj202588.top

case class User(name: String, age: Int)
来源：http://grj.yongpay.top

[T57] Scala：模式匹配
来源：http://lsr.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wir.yangfankeji.com

[T58] Scala：函数定义
来源：http://cxw.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://elq.hnqzz.top

[T59] Scala：循环
来源：http://bwl.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://jcz.zhiwuduotai.top

[T60] Scala：折叠
来源：http://xap.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ewv.tanke756.top

================================================================================
来源：http://det.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://unz.c1oappe.top

================================================================================
来源：http://rlj.hcnkem.com


<!-- 参考信息 -->