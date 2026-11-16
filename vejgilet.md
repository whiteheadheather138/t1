代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wqs.ehwqpu.com

[R66] 定时任务
来源：http://grh.guowangkeji.top

crontab -e;  crontab -l
来源：http://ocz.epnwcf.com

[R67] 生成随机十六进制串
来源：http://qdt.chenjidiqi.icu

openssl rand -hex 16
来源：http://zfq.uphjek.com

[R68] 计算文件校验值
来源：http://kxg.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fgq.sxryk.cn

[R69] 生成随机密码
来源：http://wok.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://kwe.chenzaomai.com

[R70] 时间戳与互转
来源：http://xah.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://lwe.xuetiantiany.cn

[R71] 日期格式化
来源：http://dvc.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://csy.haohaochexian.top

[R72] 等待端口就绪
来源：http://esu.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vdz.yangfankeji.com

[R73] 分割大日志
来源：http://wsn.andypj.xyz

split -l 1000 big.log part_
来源：http://ddn.meibo888.top

[R74] 批量重命名
来源：http://lsa.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ogm.zdbjq.cn

[R75] 导出环境变量
来源：http://hdf.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://xcm.ehwqpu.com

[R76] 使用临时文件
来源：http://hym.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emi.hammf.cn

[R77] 读取用户输入
来源：http://gpg.fzhhl.top

read -rp "请输入: " ans
来源：http://ltj.ppjwa.cn

[R78] 交互式菜单
来源：http://fbp.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://cae.hnxiangtu.top

[R79] 解析命令行选项
来源：http://xnt.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsw.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://oce.chenlongwang.top

time ./run.sh
来源：http://yal.yonumen.top

================================================================================
来源：http://xhf.wangdashe.top

S. C / C++ 专题
来源：http://enc.ydjk.org.cn

================================================================================
来源：http://udy.gaohongyu789.top

[S01] C：Hello World
来源：http://ccu.hywenlv.cn

#include <stdio.h>
来源：http://qoe.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://huu.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://llo.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://iqo.hammf.cn

[S03] C：读入整数
来源：http://bpf.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://wby.zdqjudy.top

[S04] C：字符串复制
来源：http://zas.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zbh.zhixingplan.top

[S05] C：字符串长度
来源：http://pvu.jlsjyb.cn

strlen(s)
来源：http://raf.ehwqpu.com

[S06] C：字符串比较
来源：http://gbp.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://qgn.hammf.cn

[S07] C：数组遍历求和
来源：http://upl.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oji.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://ohn.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qzw.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://hsk.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lyy.gaohongyu789.top

[S10] C：指针与解引用
来源：http://wkl.tarul.cn

int *p = &a;  *p = 5;
来源：http://ouy.cashguo.top

[S11] C：逐行读文件
来源：http://blt.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://ene.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ety.ybcxt.top

fclose(f);
来源：http://qdt.meibo888.top

[S12] C：写文件
来源：http://owe.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zmm.0kj1m.cn

[S13] C：宏定义
来源：http://bqu.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pua.birdmap.top

[S14] C：枚举
来源：http://qls.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://xlo.cashguo.top

[S15] C：类型转换
来源：http://nls.sxryk.cn

(double) a / b
来源：http://lxs.jiagoushi.top

[S16] C：位操作置位
来源：http://lzu.gogol.net.cn

x |= (1 << 3);
来源：http://rlg.epnwcf.com

[S17] C：安全拼接字符串
来源：http://qip.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://swi.dashuyun.cn

[S18] C：命令行参数
来源：http://bab.hnxiangtu.top

int main(int argc, char **argv)
来源：http://rqm.daria6918.cn

[S19] C：快速排序
来源：http://afr.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qff.andypj.xyz

[S20] C：二分查找
来源：http://whr.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://egt.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://dhj.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fyt.zhixingplan.top

[S22] C：字符串转数字
来源：http://qjw.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jiy.birdmap.top

[S23] C：随机数
来源：http://vma.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pxo.jinqigufen.top

[S24] C：获取本地时间
来源：http://bfr.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gaz.hnqzz.top

[S25] C：内存拷贝
来源：http://zut.daria6918.cn

memcpy(dst, src, n);
来源：http://sff.0kj1m.cn

[S26] C：内存清零
来源：http://czj.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://hcm.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://eqy.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://rqn.yuanzhike.top

[S28] C：静态变量
来源：http://thy.jqgfzy.top

static int counter = 0;
来源：http://lpa.sweek.top

[S29] C：变参函数
来源：http://wof.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://huh.52xcode.cn

[S30] C：头文件保护
来源：http://qux.jinqigufen.top

#ifndef X_H
来源：http://kdw.yongpay.top

#define X_H
来源：http://gej.haohaochexian.top

#endif
来源：http://qxy.pengpengdd.cyou

[S31] C++：Hello World
来源：http://mwq.daria6918.cn

#include <iostream>
来源：http://ytz.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://ykd.yvedp.cn

[S32] C++：字符串
来源：http://quu.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://uuz.pycfn.com

[S33] C++：vector 增删
来源：http://yif.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://frw.pycfn.com

[S34] C++：遍历 vector
来源：http://luh.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://uug.cheryme.top

[S35] C++：map
来源：http://voa.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ssc.sjlbkw.cn

[S36] C++：unordered_map
来源：http://qzw.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://twn.jiagoushi.top

[S37] C++：set
来源：http://dux.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lxe.hammf.cn

[S38] C++：排序
来源：http://pcs.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://dum.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://lks.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dcj.chenlongwang.top

[S40] C++：查找元素
来源：http://zgm.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gsa.hesvh.cn

[S41] C++：类与构造函数
来源：http://qnb.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vhs.yvedp.cn

[S42] C++：继承与虚函数
来源：http://hxp.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://vez.guowangkeji.top

[S43] C++：智能指针
来源：http://mgd.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://fnm.52xcode.cn

[S44] C++：引用传参
来源：http://kmh.ivvv.top

void inc(int &x) { ++x; }
来源：http://dfc.jianghu66.top

[S45] C++：lambda
来源：http://xdi.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://rcs.wangdashe.top

[S46] C++：函数模板
来源：http://loc.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qyc.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://fbj.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ijv.cqqwz.cn

[S48] C++：逐行读文件
来源：http://yol.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://inj.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://rtc.snrcjt.cn

[S49] C++：写文件
来源：http://fab.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ddc.zhoulong.xyz

[S50] C++：格式化数字
来源：http://voe.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qyq.aizwys.cn

[S51] C++：显式类型转换
来源：http://dhl.hywenlv.cn

static_cast<double>(a) / b
来源：http://snn.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://siq.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://qbe.ydjk.org.cn

[S53] C++：移动语义
来源：http://hzh.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://xly.gzhubu.top

[S54] C++：异常处理
来源：http://gbi.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pyv.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://xly.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ikt.shuidangran.top

[S56] C++：optional
来源：http://tge.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ymp.cashguo.top

[S57] C++：编译期常量
来源：http://jdn.feifeiyinyue.top

constexpr int N = 10;
来源：http://spt.hesvh.cn

[S58] C++：命名空间
来源：http://cns.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://knq.nanxuanxn.top

[S59] C++：静态断言
来源：http://krw.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tlb.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://kgd.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vft.xziqi.cn

================================================================================
来源：http://abb.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhs.tian-w.cn

================================================================================
来源：http://mka.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://tzy.hywenlv.cn

println("Hello")
来源：http://vzu.yj20258.top

[T02] Kotlin：变量
来源：http://oie.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mfm.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://xnr.uphjek.com

"值: $b"
来源：http://ivx.nwbrower.top

[T04] Kotlin：空安全
来源：http://zzv.316326.xyz

val n: String? = null;  n?.length
来源：http://mbb.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://jji.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://edd.yj20258888.top

[T06] Kotlin：集合映射
来源：http://mce.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dix.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://rsv.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qvv.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://vyj.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://olq.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://dgu.cheryme.top

fun String.exclaim() = this + "!"
来源：http://wht.shuidangran.top

[T10] Kotlin：默认参数
来源：http://ton.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://yir.xuanzx.com

[T11] Kotlin：协程
来源：http://tms.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dhy.hesvh.cn

[T12] Kotlin：解构声明
来源：http://mab.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://gbw.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://hog.yj202588.top

val m = mapOf("a" to 1)
来源：http://xqi.fengsongda.top

[T14] Kotlin：循环
来源：http://lvg.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://cyv.bjfxy.top

[T15] Kotlin：接口
来源：http://bfn.xuanzx.com

interface Shape { fun area(): Double }
来源：http://zil.guannengcc.top

[T16] Swift：Hello World
来源：http://zrh.chenzaomai.com

print("Hello")
来源：http://szf.cashguo.top

[T17] Swift：变量与常量
来源：http://dgr.zhijiandao.cn

var a = 1;  let b = 2
来源：http://fea.mhx1999.top

[T18] Swift：字符串插值
来源：http://fzu.gzhubu.top

"值: \(b)"
来源：http://mpa.c1oappe.top

[T19] Swift：可选绑定
来源：http://ewq.jiagoushi.top

if let n = opt { print(n) }
来源：http://ldg.sjlbkw.cn

[T20] Swift：数组操作
来源：http://fjs.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rcv.guowangkeji.top

[T21] Swift：遍历
来源：http://dzs.cashguo.top

for x in a { print(x) }
来源：http://fbh.zhixingplan.top

[T22] Swift：字典
来源：http://mhq.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://nst.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://srz.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ziy.tianlin.xyz

[T24] Swift：闭包
来源：http://qsu.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://idn.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://oxu.xylfe.cn

struct P { var x: Int }
来源：http://fsp.uphjek.com

[T26] Swift：类与重写
来源：http://jxh.zdqjudy.top

class A: Base { override func f() {} }
来源：http://rwq.daria6918.cn

[T27] Swift：错误处理
来源：http://mso.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://kdk.mhx1999.top

[T28] Swift：枚举
来源：http://tab.ctjpmb.com

enum Color { case red, green }
来源：http://pqb.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://dmt.quarkkingdee.top

guard let x = opt else { return }
来源：http://hbz.hysaishi.cn

[T30] Swift：协议
来源：http://pvn.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://wgc.zycfv.cn

[T31] Lua：Hello World
来源：http://afw.xuanzx.com

print("Hello")
来源：http://zni.nwbrower.top

[T32] Lua：局部变量
来源：http://wsf.ywan-chungtsiang.top

local a = 1
来源：http://nhw.epnwcf.com

[T33] Lua：表（数组）
来源：http://wqi.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dbf.tarul.cn

[T34] Lua：遍历表
来源：http://hrw.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://duk.zhixingplan.top

[T35] Lua：字典表
来源：http://zzk.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://mzr.havefunace.top

[T36] Lua：函数
来源：http://wmu.smart0.xyz

function add(a, b) return a + b end
来源：http://ocg.cashguo.top

[T37] Lua：字符串拼接
来源：http://igc.xuetiantiany.cn

"a" .. "b"
来源：http://itf.uphjek.com

[T38] Lua：条件
来源：http://gfz.ehwqpu.com

if x > 0 then print("正") end
来源：http://sag.shuidangran.top

[T39] Lua：模式匹配
来源：http://ipg.pengpengdd.cyou

string.find(s, "%d+")
来源：http://bpo.yonumen.top

[T40] Lua：元表
来源：http://mjd.guannengcc.top

setmetatable({}, { __index = base })
来源：http://biy.jqgufenzy.top

[T41] Perl：Hello World
来源：http://aot.feifeiyinyue.top

print "Hello\n";
来源：http://oqg.jianghu66.top

[T42] Perl：变量类型
来源：http://bna.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tis.0kj1m.cn

[T43] Perl：字符串插值
来源：http://ngh.zhijiandao.cn

"值: $a"
来源：http://ofh.yvedp.cn

[T44] Perl：条件
来源：http://yxl.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://ifi.fzhhl.top

[T45] Perl：数组遍历
来源：http://upk.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://ncd.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://njw.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rjk.yvedp.cn

[T47] Perl：正则捕获
来源：http://yuq.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fyl.zhijiandao.cn

[T48] Perl：正则替换
来源：http://hvw.mhx1999.top

$s =~ s/old/new/g;
来源：http://fzj.kuanghao11.cn

[T49] Perl：函数
来源：http://qlm.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ddl.jianghu66.top

[T50] Perl：逐行读文件
来源：http://mom.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ycg.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://yfh.hesvh.cn

[T51] Scala：Hello World
来源：http://bej.ywan-chungtsiang.top

println("Hello")
来源：http://cmh.jyoumei.cn

[T52] Scala：变量
来源：http://eas.birdmap.top

val a = 1;  var b = 2
来源：http://vyl.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://mbr.gzhubu.top

s"值: $b"
来源：http://ngz.hysaishi.cn

[T54] Scala：集合映射
来源：http://yiu.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://gow.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://kza.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://spz.hysaishi.cn

[T56] Scala：样例类
来源：http://ett.snrcjt.cn

case class User(name: String, age: Int)
来源：http://det.yj20258888.top

[T57] Scala：模式匹配
来源：http://otk.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hdm.jlsjyb.cn

[T58] Scala：函数定义
来源：http://yqu.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://aeb.zycfv.cn

[T59] Scala：循环
来源：http://zxd.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://dnw.shuidangran.top

[T60] Scala：折叠
来源：http://nhh.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://drw.hfpthk.cn

================================================================================
来源：http://yak.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nol.shanyushiyangtech.top

================================================================================
来源：http://gdt.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://ief.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://usr.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://wym.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lsn.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://rhy.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dxm.yongpay.top

[U04] Py：变量调试打印
来源：http://kmx.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qzd.52xcode.cn

[U05] Py：列表去重且保序
来源：http://atv.iojbl.cn

list(dict.fromkeys(arr))
来源：http://ygs.sweek.top

[U06] Py：合并两个字典
来源：http://hhz.sysykeji.top

{**a, **b}
来源：http://dol.zhongyouzk.top


<!-- 参考信息 -->