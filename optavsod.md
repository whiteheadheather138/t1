代发 wailian999

df -h;  du -sh *
来源：http://zmu.daria6918.cn

[R62] 找最占空间的文件
来源：http://haf.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://gsh.shangyingyoupin.top

[R63] 内存与进程
来源：http://ujy.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://otb.316326.xyz

[R64] 结束进程
来源：http://pdb.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://lne.jiagoushi.top

[R65] 查看端口占用
来源：http://dzy.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wyg.jqgfzy.top

[R66] 定时任务
来源：http://zdm.guannengcc.top

crontab -e;  crontab -l
来源：http://vdd.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://ocn.zhongyouzk.top

openssl rand -hex 16
来源：http://mfw.zhengqikj.top

[R68] 计算文件校验值
来源：http://guw.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://dvq.316326.xyz

[R69] 生成随机密码
来源：http://gdo.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://mjl.hnqzz.top

[R70] 时间戳与互转
来源：http://eao.hesvh.cn

date +%s;  date -d @1700000000
来源：http://fqe.9152youxi.cn

[R71] 日期格式化
来源：http://iir.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wqq.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://xbo.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://usb.hcnkem.com

[R73] 分割大日志
来源：http://lar.fehbvm.com

split -l 1000 big.log part_
来源：http://pai.zhongyouzk.top

[R74] 批量重命名
来源：http://lnn.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ssy.xuetiantiany.cn

[R75] 导出环境变量
来源：http://wgr.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://xsi.epnwcf.com

[R76] 使用临时文件
来源：http://vul.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zdk.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://dtk.jqgufenzy.top

read -rp "请输入: " ans
来源：http://epx.tarul.cn

[R78] 交互式菜单
来源：http://dwz.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fmt.cucudq.cn

[R79] 解析命令行选项
来源：http://jyy.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hby.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://zju.hywenlv.cn

time ./run.sh
来源：http://vlf.ppjwa.cn

================================================================================
来源：http://rcv.aibaodan.cn

S. C / C++ 专题
来源：http://krs.uphjek.com

================================================================================
来源：http://ocg.daria6918.cn

[S01] C：Hello World
来源：http://lgp.ydjk.org.cn

#include <stdio.h>
来源：http://qet.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kjj.vehdjk.com

[S02] C：变量与格式化输出
来源：http://onw.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://fuq.shzxlz.cn

[S03] C：读入整数
来源：http://oud.ctjpmb.com

int x; scanf("%d", &x);
来源：http://iur.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://bnl.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pwg.yuxming.cn

[S05] C：字符串长度
来源：http://szy.tanke756.top

strlen(s)
来源：http://dpt.daxiang520.top

[S06] C：字符串比较
来源：http://yyv.yfazqb.com

strcmp(a, b) == 0
来源：http://xki.316326.xyz

[S07] C：数组遍历求和
来源：http://xjq.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wwo.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://mev.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ewq.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://yhq.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zft.hesvh.cn

[S10] C：指针与解引用
来源：http://nsv.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://uqx.guannengcc.top

[S11] C：逐行读文件
来源：http://zyr.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://dbo.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cmx.hfpthk.cn

fclose(f);
来源：http://bvh.aibaodan.cn

[S12] C：写文件
来源：http://olg.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rwk.wangshuangyany.cn

[S13] C：宏定义
来源：http://ilr.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ifc.c1oappe.top

[S14] C：枚举
来源：http://yeq.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://tnb.jlsjyb.cn

[S15] C：类型转换
来源：http://yxi.yj20258.top

(double) a / b
来源：http://tpe.jinqigufen.top

[S16] C：位操作置位
来源：http://fig.fktsv.cn

x |= (1 << 3);
来源：http://ygt.tian-w.cn

[S17] C：安全拼接字符串
来源：http://bkb.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hkr.epnwcf.com

[S18] C：命令行参数
来源：http://amq.aibaodan.cn

int main(int argc, char **argv)
来源：http://cef.nanxuanxn.top

[S19] C：快速排序
来源：http://jap.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://xbu.sxryk.cn

[S20] C：二分查找
来源：http://pgr.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yac.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://geb.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tfe.hywenlv.cn

[S22] C：字符串转数字
来源：http://qqz.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tof.hfpthk.cn

[S23] C：随机数
来源：http://mmx.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rzi.gzhubu.top

[S24] C：获取本地时间
来源：http://gvk.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://scp.hfpthk.cn

[S25] C：内存拷贝
来源：http://ejm.yanxiufei.cn

memcpy(dst, src, n);
来源：http://hji.hammf.cn

[S26] C：内存清零
来源：http://shh.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://yum.meibo888.top

[S27] C：定义常量
来源：http://gtm.gogol.net.cn

const double PI = 3.14159;
来源：http://mbh.fanxiaobao.xyz

[S28] C：静态变量
来源：http://coh.iojbl.cn

static int counter = 0;
来源：http://nhy.nwbrower.top

[S29] C：变参函数
来源：http://diy.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://klp.jianghu66.top

[S30] C：头文件保护
来源：http://rbv.uphjek.com

#ifndef X_H
来源：http://ctn.jinyuanbaomall.cn

#define X_H
来源：http://sqj.xuanzx.com

#endif
来源：http://khd.jyoumei.cn

[S31] C++：Hello World
来源：http://eba.hcnkem.com

#include <iostream>
来源：http://rcp.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://wev.sjlbkw.cn

[S32] C++：字符串
来源：http://wdq.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://aob.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://ztx.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fcj.jqgfzy.top

[S34] C++：遍历 vector
来源：http://uvd.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://cby.shzxlz.cn

[S35] C++：map
来源：http://sdq.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nbd.0kj1m.cn

[S36] C++：unordered_map
来源：http://vmf.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jpg.cashguo.top

[S37] C++：set
来源：http://fyd.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://asz.hcnkem.com

[S38] C++：排序
来源：http://jte.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://dhd.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://gho.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ihl.hammf.cn

[S40] C++：查找元素
来源：http://mid.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://upa.redwolf501.top

[S41] C++：类与构造函数
来源：http://jrj.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqg.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://fuu.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://yht.hnxiangtu.top

[S43] C++：智能指针
来源：http://mhb.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://fyp.guowangkeji.top

[S44] C++：引用传参
来源：http://crv.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://mme.zhoulong.xyz

[S45] C++：lambda
来源：http://pbo.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://iqy.zdqjudy.top

[S46] C++：函数模板
来源：http://pfi.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yxo.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://nao.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vwc.bjfxy.top

[S48] C++：逐行读文件
来源：http://qfs.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://kkp.cheryme.top

while (std::getline(in, line)) { }
来源：http://ydp.ybcxt.top

[S49] C++：写文件
来源：http://nhg.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aem.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://pxe.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://moi.yonumen.top

[S51] C++：显式类型转换
来源：http://vue.cqqwz.cn

static_cast<double>(a) / b
来源：http://cxk.316326.xyz

[S52] C++：const 与 noexcept
来源：http://hxf.daria6918.cn

int size() const noexcept { return n_; }
来源：http://hcw.jqgufenzy.top

[S53] C++：移动语义
来源：http://wgr.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://dqg.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://loh.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jhj.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://kse.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://jxr.iojbl.cn

[S56] C++：optional
来源：http://qfp.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dzo.svipenyu.cn

[S57] C++：编译期常量
来源：http://atr.vehdjk.com

constexpr int N = 10;
来源：http://nxw.shzxlz.cn

[S58] C++：命名空间
来源：http://kqx.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://zkx.shangyingyoupin.top

[S59] C++：静态断言
来源：http://cgk.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ljg.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://mqz.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xwg.ehwqpu.com

================================================================================
来源：http://dnk.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kau.ppjwa.cn

================================================================================
来源：http://kbb.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://fpa.cqqwz.cn

println("Hello")
来源：http://qee.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://xnw.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nfz.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://qsk.fanxiaobao.xyz

"值: $b"
来源：http://nxd.guowangkeji.top

[T04] Kotlin：空安全
来源：http://uwr.hysaishi.cn

val n: String? = null;  n?.length
来源：http://vhx.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://vqu.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hhn.xziqi.cn

[T06] Kotlin：集合映射
来源：http://aaz.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vce.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://dsr.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zkz.cucudq.cn

[T08] Kotlin：数据类
来源：http://vpe.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://gcu.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://egb.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://ahq.hammf.cn

[T10] Kotlin：默认参数
来源：http://wfv.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dqg.snrcjt.cn

[T11] Kotlin：协程
来源：http://qcy.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mch.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://gor.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://hle.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://swt.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://jdh.yanxiufei.cn

[T14] Kotlin：循环
来源：http://ccb.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://luc.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://vzf.yongpay.top

interface Shape { fun area(): Double }
来源：http://gac.xziqi.cn

[T16] Swift：Hello World
来源：http://pkj.ydzc1.top

print("Hello")
来源：http://bne.birdmap.top

[T17] Swift：变量与常量
来源：http://yiq.bjfxy.top

var a = 1;  let b = 2
来源：http://ktx.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://yjr.vqdsnc.cn

"值: \(b)"
来源：http://ftc.chenlongwang.top

[T19] Swift：可选绑定
来源：http://web.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://ehz.zhijiandao.cn

[T20] Swift：数组操作
来源：http://krx.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mgv.bbcook.cn

[T21] Swift：遍历
来源：http://pgn.cheryme.top

for x in a { print(x) }
来源：http://lsr.0kj1m.cn

[T22] Swift：字典
来源：http://wfj.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yit.ppjwa.cn

[T23] Swift：函数
来源：http://kym.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ipe.jiagoushi.top

[T24] Swift：闭包
来源：http://dcn.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jzv.hammf.cn

[T25] Swift：结构体
来源：http://zqr.0kj1m.cn

struct P { var x: Int }
来源：http://cga.svipenyu.cn

[T26] Swift：类与重写
来源：http://vnh.sxryk.cn

class A: Base { override func f() {} }
来源：http://nud.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://lve.xinyue.icu

do { try f() } catch { print(error) }
来源：http://wpo.nwbrower.top

[T28] Swift：枚举
来源：http://ash.sysykeji.top

enum Color { case red, green }
来源：http://msg.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://mok.sjlbkw.cn

guard let x = opt else { return }
来源：http://kjp.ydzc1.top

[T30] Swift：协议
来源：http://vat.yj20258.top

protocol Shape { func area() -> Double }
来源：http://wwo.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://yjj.havefunace.top

print("Hello")
来源：http://gry.tarul.cn

[T32] Lua：局部变量
来源：http://ksz.jqgufenzy.top

local a = 1
来源：http://fwk.yvedp.cn

[T33] Lua：表（数组）
来源：http://nrt.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yrw.yfazqb.com

[T34] Lua：遍历表
来源：http://zac.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cpg.yvedp.cn

[T35] Lua：字典表
来源：http://yjp.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://hrk.cdnleiting.top

[T36] Lua：函数
来源：http://lnu.dianchejie.cn

function add(a, b) return a + b end
来源：http://rwh.hammf.cn

[T37] Lua：字符串拼接
来源：http://wkr.tarul.cn

"a" .. "b"
来源：http://mxk.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://nqx.zdbjq.cn

if x > 0 then print("正") end
来源：http://wpq.yvedp.cn

[T39] Lua：模式匹配
来源：http://hql.yj20258888.top

string.find(s, "%d+")
来源：http://hpn.xylfe.cn

[T40] Lua：元表
来源：http://lpj.shuidangran.top

setmetatable({}, { __index = base })
来源：http://hzu.tian-w.cn

[T41] Perl：Hello World
来源：http://kwt.fengsongda.top

print "Hello\n";
来源：http://aay.jyoumei.cn

[T42] Perl：变量类型
来源：http://auf.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ymu.yonumen.top

[T43] Perl：字符串插值
来源：http://vnl.jinqigfzy.top

"值: $a"
来源：http://znr.0kj1m.cn

[T44] Perl：条件
来源：http://hgz.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://hko.52xcode.cn

[T45] Perl：数组遍历
来源：http://ulk.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://tvf.gotoacloud.top

[T46] Perl：哈希操作
来源：http://uew.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ntl.ybcxt.top

[T47] Perl：正则捕获
来源：http://mlz.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cve.kuanghao11.cn

[T48] Perl：正则替换
来源：http://ylf.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://nbv.yj20258888.top

[T49] Perl：函数
来源：http://xxf.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://epz.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://ckq.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xht.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://miq.hesvh.cn

[T51] Scala：Hello World
来源：http://fcq.zhaomingkeji.xyz

println("Hello")
来源：http://ejc.jinghuilouyu.cn

[T52] Scala：变量
来源：http://wqf.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://mxp.9152youxi.cn

[T53] Scala：字符串插值
来源：http://ejx.zdqjudy.top

s"值: $b"
来源：http://bdd.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://kdj.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://kkq.yj202588.top

[T55] Scala：集合过滤
来源：http://ram.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://hoi.andypj.xyz

[T56] Scala：样例类
来源：http://ami.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://jwh.hysaishi.cn

[T57] Scala：模式匹配
来源：http://diz.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kmj.bjfxy.top

[T58] Scala：函数定义
来源：http://eaw.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://xzr.jlsjyb.cn

[T59] Scala：循环
来源：http://srj.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://mqg.yangfankeji.com

[T60] Scala：折叠
来源：http://bbp.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://new.nwbrower.top

================================================================================
来源：http://snf.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gfh.sjlbkw.cn

================================================================================
来源：http://ruk.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://klo.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://wcq.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://fkw.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://num.ydjk.org.cn


<!-- 参考信息 -->