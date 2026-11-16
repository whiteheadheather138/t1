代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tkc.wangdashe.top

[R66] 定时任务
来源：http://zjt.wangdashe.top

crontab -e;  crontab -l
来源：http://wpb.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://sng.andypj.xyz

openssl rand -hex 16
来源：http://zax.tanke756.top

[R68] 计算文件校验值
来源：http://rbe.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://voz.zhiwuduotai.top

[R69] 生成随机密码
来源：http://mxj.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://elj.hesvh.cn

[R70] 时间戳与互转
来源：http://jyo.xinyue.icu

date +%s;  date -d @1700000000
来源：http://lbn.yj20258.top

[R71] 日期格式化
来源：http://wsv.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vkg.mhx1999.top

[R72] 等待端口就绪
来源：http://hje.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uel.316326.xyz

[R73] 分割大日志
来源：http://oph.meibo888.top

split -l 1000 big.log part_
来源：http://ojx.zhengqikj.top

[R74] 批量重命名
来源：http://sfs.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cta.yanxiufei.cn

[R75] 导出环境变量
来源：http://rzk.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://tbu.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://gpm.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kbv.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://wos.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://dsw.hnxiangtu.top

[R78] 交互式菜单
来源：http://chi.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xqh.tian-w.cn

[R79] 解析命令行选项
来源：http://zuq.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vck.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://vze.hfpthk.cn

time ./run.sh
来源：http://oby.hesvh.cn

================================================================================
来源：http://euz.gaohongyu789.top

S. C / C++ 专题
来源：http://wef.svipenyu.cn

================================================================================
来源：http://bio.gzhubu.top

[S01] C：Hello World
来源：http://fah.hysaishi.cn

#include <stdio.h>
来源：http://niy.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mmg.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://yah.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://zhj.ydzc1.top

[S03] C：读入整数
来源：http://kvg.ybcxt.top

int x; scanf("%d", &x);
来源：http://pdy.bjfxy.top

[S04] C：字符串复制
来源：http://yrx.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://toz.daxiang520.top

[S05] C：字符串长度
来源：http://mlg.fanxiaobao.xyz

strlen(s)
来源：http://yom.shuidangran.top

[S06] C：字符串比较
来源：http://muw.nwbrower.top

strcmp(a, b) == 0
来源：http://sqc.cucudq.cn

[S07] C：数组遍历求和
来源：http://hmw.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zjg.316326.xyz

[S08] C：动态内存分配与释放
来源：http://alg.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jys.sweek.top

[S09] C：结构体定义与初始化
来源：http://vim.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yzb.fengsongda.top

[S10] C：指针与解引用
来源：http://hme.cashguo.top

int *p = &a;  *p = 5;
来源：http://lmz.zhengqikj.top

[S11] C：逐行读文件
来源：http://qjh.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://nwx.nwbrower.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wiq.zhongyouzk.top

fclose(f);
来源：http://rbh.feifeiyinyue.top

[S12] C：写文件
来源：http://mos.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ipw.uphjek.com

[S13] C：宏定义
来源：http://qur.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vru.jqgufenzy.top

[S14] C：枚举
来源：http://gak.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://yke.mhx1999.top

[S15] C：类型转换
来源：http://egr.pengpengdd.cyou

(double) a / b
来源：http://yfq.wangdashe.top

[S16] C：位操作置位
来源：http://fgb.sjlbkw.cn

x |= (1 << 3);
来源：http://dcw.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://leb.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dkj.yueranfly.top

[S18] C：命令行参数
来源：http://bjl.kuanghao11.cn

int main(int argc, char **argv)
来源：http://btg.gotoacloud.top

[S19] C：快速排序
来源：http://cql.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://ryz.ctjpmb.com

[S20] C：二分查找
来源：http://oug.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ruq.jinqigufen.top

[S21] C：字符类别判断
来源：http://vcd.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vyp.fengsongda.top

[S22] C：字符串转数字
来源：http://lpw.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://myy.andypj.xyz

[S23] C：随机数
来源：http://agj.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://xzm.yj20258.top

[S24] C：获取本地时间
来源：http://stj.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ilo.shuidangran.top

[S25] C：内存拷贝
来源：http://ipe.tanke756.top

memcpy(dst, src, n);
来源：http://jof.epnwcf.com

[S26] C：内存清零
来源：http://gsr.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://fcf.ehwqpu.com

[S27] C：定义常量
来源：http://hiq.chenlongwang.top

const double PI = 3.14159;
来源：http://cqe.pycfn.com

[S28] C：静态变量
来源：http://jia.yj202588.top

static int counter = 0;
来源：http://hil.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://lif.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yiz.xuanzx.com

[S30] C：头文件保护
来源：http://jfn.hesvh.cn

#ifndef X_H
来源：http://plw.svipenyu.cn

#define X_H
来源：http://ydh.gogol.net.cn

#endif
来源：http://exc.xinyue.icu

[S31] C++：Hello World
来源：http://qvz.epnwcf.com

#include <iostream>
来源：http://bvx.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://lyg.c1oappe.top

[S32] C++：字符串
来源：http://xuk.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://xms.yonumen.top

[S33] C++：vector 增删
来源：http://nek.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://elf.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://jeq.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://rhk.wangshuangyany.cn

[S35] C++：map
来源：http://epb.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uuk.jianghu66.top

[S36] C++：unordered_map
来源：http://cgq.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vqm.xylfe.cn

[S37] C++：set
来源：http://nje.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ndm.hnxiangtu.top

[S38] C++：排序
来源：http://lbv.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://qzh.cheryme.top

[S39] C++：自定义比较器排序
来源：http://rep.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cfh.hesvh.cn

[S40] C++：查找元素
来源：http://vbl.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vib.haohaochexian.top

[S41] C++：类与构造函数
来源：http://pjv.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kgg.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://irn.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://qvw.52xcode.cn

[S43] C++：智能指针
来源：http://sgt.sweek.top

auto p = std::make_unique<int>(5);
来源：http://rnl.cucudq.cn

[S44] C++：引用传参
来源：http://ajs.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://aee.guowangkeji.top

[S45] C++：lambda
来源：http://okr.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://jgg.daxiang520.top

[S46] C++：函数模板
来源：http://dpk.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wta.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://sji.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://twl.hcnkem.com

[S48] C++：逐行读文件
来源：http://oum.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://moc.xuanzx.com

while (std::getline(in, line)) { }
来源：http://cok.jianghu66.top

[S49] C++：写文件
来源：http://pek.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jhk.zhijiandao.cn

[S50] C++：格式化数字
来源：http://jcu.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://goi.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://yhw.zhoulong.xyz

static_cast<double>(a) / b
来源：http://iwr.yonumen.top

[S52] C++：const 与 noexcept
来源：http://ebi.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://ngl.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://cfp.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://ylx.hcnkem.com

[S54] C++：异常处理
来源：http://lxs.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tif.jyoumei.cn

[S55] C++：结构化绑定
来源：http://gug.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://wip.cheryme.top

[S56] C++：optional
来源：http://dhz.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qhi.daria6918.cn

[S57] C++：编译期常量
来源：http://qlk.hywenlv.cn

constexpr int N = 10;
来源：http://hok.cqqwz.cn

[S58] C++：命名空间
来源：http://mzp.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://rtv.nanxuanxn.top

[S59] C++：静态断言
来源：http://oyy.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gia.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://gtm.wangdashe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ckq.52xcode.cn

================================================================================
来源：http://mzs.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kpx.cheryme.top

================================================================================
来源：http://yen.yj20258888.top

[T01] Kotlin：Hello World
来源：http://eah.dianchejie.cn

println("Hello")
来源：http://rpd.cucudq.cn

[T02] Kotlin：变量
来源：http://wim.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bbm.meibo888.top

[T03] Kotlin：字符串模板
来源：http://mgo.ydzc1.top

"值: $b"
来源：http://hhw.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://uzp.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://uhw.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ytt.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fzq.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://jhs.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cmo.316326.xyz

[T07] Kotlin：集合过滤
来源：http://nbe.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xco.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://pvr.sweek.top

data class User(val name: String, val age: Int)
来源：http://hdh.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://edw.sweek.top

fun String.exclaim() = this + "!"
来源：http://bwi.316326.xyz

[T10] Kotlin：默认参数
来源：http://uyk.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kes.ehwqpu.com

[T11] Kotlin：协程
来源：http://lpx.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eir.tanke756.top

[T12] Kotlin：解构声明
来源：http://fwt.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://wzu.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://iyt.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://sjb.yuxming.cn

[T14] Kotlin：循环
来源：http://lzs.dashuyun.cn

for (i in 1..10) println(i)
来源：http://duk.316326.xyz

[T15] Kotlin：接口
来源：http://dkk.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://vbv.yanxiufei.cn

[T16] Swift：Hello World
来源：http://bhu.xylfe.cn

print("Hello")
来源：http://mlg.yvedp.cn

[T17] Swift：变量与常量
来源：http://mvr.zhijiandao.cn

var a = 1;  let b = 2
来源：http://day.ppjwa.cn

[T18] Swift：字符串插值
来源：http://uic.hcnkem.com

"值: \(b)"
来源：http://sih.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://exy.jinqigufen.top

if let n = opt { print(n) }
来源：http://duc.hnqzz.top

[T20] Swift：数组操作
来源：http://tci.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://vfa.dianchejie.cn

[T21] Swift：遍历
来源：http://wul.hfpthk.cn

for x in a { print(x) }
来源：http://dcf.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://rqj.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://jbe.feifeiyinyue.top

[T23] Swift：函数
来源：http://qhq.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lge.guannengcc.top

[T24] Swift：闭包
来源：http://rhb.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://asn.pengpengdd.cyou

[T25] Swift：结构体
来源：http://aag.ybcxt.top

struct P { var x: Int }
来源：http://itd.jyoumei.cn

[T26] Swift：类与重写
来源：http://jaa.zycfv.cn

class A: Base { override func f() {} }
来源：http://atn.hesvh.cn

[T27] Swift：错误处理
来源：http://blq.bjfxy.top

do { try f() } catch { print(error) }
来源：http://zxj.zhengqikj.top

[T28] Swift：枚举
来源：http://yyy.ppjwa.cn

enum Color { case red, green }
来源：http://mhn.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://ipx.wangshuangyany.cn

guard let x = opt else { return }
来源：http://itu.iojbl.cn

[T30] Swift：协议
来源：http://jtr.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://ucf.vehdjk.com

[T31] Lua：Hello World
来源：http://pxf.andypj.xyz

print("Hello")
来源：http://aiy.yangfankeji.com

[T32] Lua：局部变量
来源：http://bjk.snrcjt.cn

local a = 1
来源：http://clt.ctjpmb.com

[T33] Lua：表（数组）
来源：http://lni.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nyk.havefunace.top

[T34] Lua：遍历表
来源：http://ttt.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xgx.jiagoushi.top

[T35] Lua：字典表
来源：http://ggm.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://rcj.chenlongwang.top

[T36] Lua：函数
来源：http://hbp.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://efb.hnqzz.top

[T37] Lua：字符串拼接
来源：http://juv.nanxinkj.top

"a" .. "b"
来源：http://oad.hysaishi.cn

[T38] Lua：条件
来源：http://cli.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://jqt.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://lbi.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://wdx.xinyue.icu

[T40] Lua：元表
来源：http://hsi.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://zdy.zhijiandao.cn

[T41] Perl：Hello World
来源：http://red.haohaochexian.top

print "Hello\n";
来源：http://pca.hysaishi.cn

[T42] Perl：变量类型
来源：http://hbu.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lut.jianghu66.top

[T43] Perl：字符串插值
来源：http://cbg.shzxlz.cn

"值: $a"
来源：http://viz.jinghuilouyu.cn

[T44] Perl：条件
来源：http://jfg.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://vzz.yj20258.top

[T45] Perl：数组遍历
来源：http://lch.birdmap.top

for my $x (@arr) { print $x; }
来源：http://phv.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://byz.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cqh.chenlongwang.top

[T47] Perl：正则捕获
来源：http://zsv.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cre.wangdashe.top

[T48] Perl：正则替换
来源：http://sxs.zhengqikj.top

$s =~ s/old/new/g;
来源：http://zbx.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://uxr.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ypz.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://ght.zhijiandao.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fxu.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://oyf.tianlin.xyz

[T51] Scala：Hello World
来源：http://syr.uphjek.com

println("Hello")
来源：http://cca.gzhubu.top

[T52] Scala：变量
来源：http://seq.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://wiq.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://agi.wangshuangyany.cn

s"值: $b"
来源：http://gdp.iojbl.cn

[T54] Scala：集合映射
来源：http://gwn.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://qzg.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://kcv.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vzf.sweek.top

[T56] Scala：样例类
来源：http://fuo.hywenlv.cn

case class User(name: String, age: Int)
来源：http://wvr.smart0.xyz

[T57] Scala：模式匹配
来源：http://ver.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://azk.snrcjt.cn

[T58] Scala：函数定义
来源：http://owe.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bhj.jianghu66.top

[T59] Scala：循环
来源：http://snu.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://xjy.gogol.net.cn

[T60] Scala：折叠
来源：http://ond.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mdi.gaohongyu789.top

================================================================================
来源：http://rgo.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oti.snrcjt.cn

================================================================================
来源：http://vms.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://odj.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xwz.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://rum.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://efw.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://cdu.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://blt.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://ehj.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ofm.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://pei.xinyue.icu

list(dict.fromkeys(arr))
来源：http://oze.birdmap.top

[U06] Py：合并两个字典
来源：http://eov.haohaochexian.top

{**a, **b}
来源：http://jxl.jiagoushi.top


<!-- 参考信息 -->