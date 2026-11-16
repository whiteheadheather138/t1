代发 wailian999

free -h;  ps aux | grep nginx
来源：http://gri.zhiwuduotai.top

[R64] 结束进程
来源：http://kyt.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://ugt.nwbrower.top

[R65] 查看端口占用
来源：http://qqv.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mbk.dashuyun.cn

[R66] 定时任务
来源：http://fqm.hesvh.cn

crontab -e;  crontab -l
来源：http://btv.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://hpj.shangyingyoupin.top

openssl rand -hex 16
来源：http://agf.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://mdo.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://pzp.redwolf501.top

[R69] 生成随机密码
来源：http://mbs.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://mpa.ctjpmb.com

[R70] 时间戳与互转
来源：http://gbp.cashguo.top

date +%s;  date -d @1700000000
来源：http://esq.fengsongda.top

[R71] 日期格式化
来源：http://ihu.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jnc.haohaochexian.top

[R72] 等待端口就绪
来源：http://vkv.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pdf.ivvv.top

[R73] 分割大日志
来源：http://vzm.ydzc1.top

split -l 1000 big.log part_
来源：http://wkz.epnwcf.com

[R74] 批量重命名
来源：http://yng.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eov.sxryk.cn

[R75] 导出环境变量
来源：http://wrb.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://lfk.wangdashe.top

[R76] 使用临时文件
来源：http://tjg.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://umi.jqgufenzy.top

[R77] 读取用户输入
来源：http://pct.quarkkingdee.top

read -rp "请输入: " ans
来源：http://ieh.gotoacloud.top

[R78] 交互式菜单
来源：http://kjo.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yyp.sweek.top

[R79] 解析命令行选项
来源：http://oxu.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sgo.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://pxc.jinyuanbaomall.cn

time ./run.sh
来源：http://zlq.0kj1m.cn

================================================================================
来源：http://yft.hesvh.cn

S. C / C++ 专题
来源：http://utp.zhongyouzk.top

================================================================================
来源：http://jvj.hfpthk.cn

[S01] C：Hello World
来源：http://nic.guowangkeji.top

#include <stdio.h>
来源：http://qnb.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iwy.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://ojd.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://bvg.fengsongda.top

[S03] C：读入整数
来源：http://djk.hywenlv.cn

int x; scanf("%d", &x);
来源：http://bna.hcnkem.com

[S04] C：字符串复制
来源：http://bot.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://suv.guowangkeji.top

[S05] C：字符串长度
来源：http://nic.quarkkingdee.top

strlen(s)
来源：http://qye.yangfankeji.com

[S06] C：字符串比较
来源：http://jhy.yuanzhike.top

strcmp(a, b) == 0
来源：http://dgw.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://swq.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wfs.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://bdw.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uba.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://yhe.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://okl.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://isy.ybcxt.top

int *p = &a;  *p = 5;
来源：http://esr.ivvv.top

[S11] C：逐行读文件
来源：http://rgd.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://ogm.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fdx.yj202588.top

fclose(f);
来源：http://rfr.yuxming.cn

[S12] C：写文件
来源：http://jyo.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cac.daria6918.cn

[S13] C：宏定义
来源：http://cas.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myj.yangfankeji.com

[S14] C：枚举
来源：http://czd.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ooi.nwbrower.top

[S15] C：类型转换
来源：http://gfo.ydzc1.top

(double) a / b
来源：http://xna.zhongyouzk.top

[S16] C：位操作置位
来源：http://hev.pycfn.com

x |= (1 << 3);
来源：http://dtk.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://uwr.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uws.c1oappe.top

[S18] C：命令行参数
来源：http://jqu.zhijiandao.cn

int main(int argc, char **argv)
来源：http://lwf.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://otu.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://oid.xinyue.icu

[S20] C：二分查找
来源：http://axm.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cvw.tarul.cn

[S21] C：字符类别判断
来源：http://acc.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwm.aizwys.cn

[S22] C：字符串转数字
来源：http://oul.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://ghc.yfazqb.com

[S23] C：随机数
来源：http://viv.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mna.zdbjq.cn

[S24] C：获取本地时间
来源：http://itm.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qdw.yvedp.cn

[S25] C：内存拷贝
来源：http://zzv.c1oappe.top

memcpy(dst, src, n);
来源：http://ucm.zhixingplan.top

[S26] C：内存清零
来源：http://gjv.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://bxm.aizwys.cn

[S27] C：定义常量
来源：http://mgq.wangdashe.top

const double PI = 3.14159;
来源：http://etx.hongshengwenyu.top

[S28] C：静态变量
来源：http://mhc.yj202588.top

static int counter = 0;
来源：http://mfr.zdqjudy.top

[S29] C：变参函数
来源：http://ems.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lvm.chenzaomai.com

[S30] C：头文件保护
来源：http://nkr.gogol.net.cn

#ifndef X_H
来源：http://ced.hywenlv.cn

#define X_H
来源：http://dif.52xcode.cn

#endif
来源：http://sdb.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://ctp.zdqjudy.top

#include <iostream>
来源：http://wkv.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jcr.ehwqpu.com

[S32] C++：字符串
来源：http://gkg.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://dtf.zdqjudy.top

[S33] C++：vector 增删
来源：http://aea.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yij.sufxvd.cn

[S34] C++：遍历 vector
来源：http://uzu.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://zys.hnxiangtu.top

[S35] C++：map
来源：http://cea.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ebl.hammf.cn

[S36] C++：unordered_map
来源：http://yzf.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkn.zdbjq.cn

[S37] C++：set
来源：http://tdu.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qln.chenzaomai.com

[S38] C++：排序
来源：http://wsd.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://xbz.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://tat.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wvb.yvedp.cn

[S40] C++：查找元素
来源：http://tyc.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wbh.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://bpa.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwn.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://kze.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://pzp.xuanzx.com

[S43] C++：智能指针
来源：http://wnz.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://zyv.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://ngh.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://kke.cashguo.top

[S45] C++：lambda
来源：http://jfl.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://hsg.quarkkingdee.top

[S46] C++：函数模板
来源：http://azb.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qzz.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://qpr.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://flc.cucudq.cn

[S48] C++：逐行读文件
来源：http://mhy.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rcj.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://txl.daxiang520.top

[S49] C++：写文件
来源：http://igg.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ccf.guowangkeji.top

[S50] C++：格式化数字
来源：http://kaa.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wcu.yvedp.cn

[S51] C++：显式类型转换
来源：http://yjy.hammf.cn

static_cast<double>(a) / b
来源：http://pyq.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://eja.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://ell.wangdashe.top

[S53] C++：移动语义
来源：http://jfz.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://ock.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://jvv.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zts.shzxlz.cn

[S55] C++：结构化绑定
来源：http://yph.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bfe.yj20258.top

[S56] C++：optional
来源：http://zkh.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://afw.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://gqt.zhiwuduotai.top

constexpr int N = 10;
来源：http://kcz.bjfxy.top

[S58] C++：命名空间
来源：http://ldx.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://jth.nanxuanxn.top

[S59] C++：静态断言
来源：http://acu.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hee.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://umu.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://efu.zhengqikj.top

================================================================================
来源：http://cte.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wtn.hesvh.cn

================================================================================
来源：http://bjf.redwolf501.top

[T01] Kotlin：Hello World
来源：http://enf.chenzaomai.com

println("Hello")
来源：http://uln.yuanzhike.top

[T02] Kotlin：变量
来源：http://xqx.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oea.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://baw.feifeiyinyue.top

"值: $b"
来源：http://wea.gotoacloud.top

[T04] Kotlin：空安全
来源：http://crs.yangfankeji.com

val n: String? = null;  n?.length
来源：http://ufn.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://bcc.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nkj.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://tla.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://neu.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://eiz.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://fhx.ehwqpu.com

[T08] Kotlin：数据类
来源：http://qrj.sweek.top

data class User(val name: String, val age: Int)
来源：http://clr.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://vlc.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://prl.ybcxt.top

[T10] Kotlin：默认参数
来源：http://olr.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xhz.nwbrower.top

[T11] Kotlin：协程
来源：http://oil.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gif.xylfe.cn

[T12] Kotlin：解构声明
来源：http://yaf.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://yrj.hammf.cn

[T13] Kotlin：只读 Map
来源：http://rei.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://fdz.cdnleiting.top

[T14] Kotlin：循环
来源：http://qxi.uphjek.com

for (i in 1..10) println(i)
来源：http://guq.cqqwz.cn

[T15] Kotlin：接口
来源：http://cet.bjfxy.top

interface Shape { fun area(): Double }
来源：http://cum.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://yhb.feifeiyinyue.top

print("Hello")
来源：http://wmz.yuxming.cn

[T17] Swift：变量与常量
来源：http://ulr.kuanghao11.cn

var a = 1;  let b = 2
来源：http://hkk.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://lna.gotoacloud.top

"值: \(b)"
来源：http://rsz.yuanzhike.top

[T19] Swift：可选绑定
来源：http://run.zhijiandao.cn

if let n = opt { print(n) }
来源：http://aiv.tarul.cn

[T20] Swift：数组操作
来源：http://qbi.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://ryq.bjfxy.top

[T21] Swift：遍历
来源：http://ccd.nanxinkj.top

for x in a { print(x) }
来源：http://ylq.jinqigfzy.top

[T22] Swift：字典
来源：http://zxi.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cks.jianghu66.top

[T23] Swift：函数
来源：http://qcp.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://olg.cheryme.top

[T24] Swift：闭包
来源：http://sjg.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cwb.shangyingyoupin.top

[T25] Swift：结构体
来源：http://dgy.cqqwz.cn

struct P { var x: Int }
来源：http://ips.hfpthk.cn

[T26] Swift：类与重写
来源：http://wsm.tianlin.xyz

class A: Base { override func f() {} }
来源：http://qjs.iojbl.cn

[T27] Swift：错误处理
来源：http://zcw.sweek.top

do { try f() } catch { print(error) }
来源：http://lkz.dianchejie.cn

[T28] Swift：枚举
来源：http://fqt.sjlbkw.cn

enum Color { case red, green }
来源：http://bfl.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://okd.ctjpmb.com

guard let x = opt else { return }
来源：http://hxn.zycfv.cn

[T30] Swift：协议
来源：http://rmh.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://snj.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://xms.pycfn.com

print("Hello")
来源：http://iqk.tianlin.xyz

[T32] Lua：局部变量
来源：http://jvx.cdnleiting.top

local a = 1
来源：http://jld.meibo888.top

[T33] Lua：表（数组）
来源：http://uen.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ela.chenzaomai.com

[T34] Lua：遍历表
来源：http://lul.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dmc.tanke756.top

[T35] Lua：字典表
来源：http://jil.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://hhf.meibo888.top

[T36] Lua：函数
来源：http://qor.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://cgk.yj202588.top

[T37] Lua：字符串拼接
来源：http://rto.yvedp.cn

"a" .. "b"
来源：http://pvj.pycfn.com

[T38] Lua：条件
来源：http://ihp.ivvv.top

if x > 0 then print("正") end
来源：http://uzs.meibo888.top

[T39] Lua：模式匹配
来源：http://asy.zdbjq.cn

string.find(s, "%d+")
来源：http://lid.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://pjh.c1oappe.top

setmetatable({}, { __index = base })
来源：http://fwj.quarkkingdee.top

[T41] Perl：Hello World
来源：http://czj.yvedp.cn

print "Hello\n";
来源：http://tvc.zhijiandao.cn

[T42] Perl：变量类型
来源：http://cyh.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xnt.0kj1m.cn

[T43] Perl：字符串插值
来源：http://qcd.zhixingplan.top

"值: $a"
来源：http://szy.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://kmh.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://ubd.dianchejie.cn

[T45] Perl：数组遍历
来源：http://stp.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://gtm.tarul.cn

[T46] Perl：哈希操作
来源：http://ded.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eak.zycfv.cn

[T47] Perl：正则捕获
来源：http://vne.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mci.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://bwy.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://pfm.quarkkingdee.top

[T49] Perl：函数
来源：http://muz.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tbr.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://tea.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gev.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://mbn.yfazqb.com

[T51] Scala：Hello World
来源：http://dzl.cdnleiting.top

println("Hello")
来源：http://rsn.zhoulong.xyz

[T52] Scala：变量
来源：http://uzv.jianghu66.top

val a = 1;  var b = 2
来源：http://jjw.yfazqb.com

[T53] Scala：字符串插值
来源：http://oxp.nanxinkj.top

s"值: $b"
来源：http://brs.dianchejie.cn

[T54] Scala：集合映射
来源：http://ats.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://lgt.yueranfly.top

[T55] Scala：集合过滤
来源：http://tbb.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://unl.yonumen.top

[T56] Scala：样例类
来源：http://jyn.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://zny.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://qkf.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://olt.jqgfzy.top

[T58] Scala：函数定义
来源：http://yvp.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://ywt.epnwcf.com

[T59] Scala：循环
来源：http://kcc.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://uvr.vehdjk.com

[T60] Scala：折叠
来源：http://kmf.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tim.xziqi.cn

================================================================================
来源：http://fld.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jwn.havefunace.top

================================================================================
来源：http://utx.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://fvc.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://ltd.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://ssb.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wxu.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://eyd.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jhi.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://duf.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nvu.cqqwz.cn


<!-- 参考信息 -->