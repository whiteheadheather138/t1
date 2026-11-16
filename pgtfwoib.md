代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjx.ywan-chungtsiang.top

[R66] 定时任务
来源：http://arz.yonumen.top

crontab -e;  crontab -l
来源：http://vsf.yj20258.top

[R67] 生成随机十六进制串
来源：http://ydf.ehwqpu.com

openssl rand -hex 16
来源：http://vzi.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://cpy.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://kdu.shangyingyoupin.top

[R69] 生成随机密码
来源：http://adj.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://clg.gotoacloud.top

[R70] 时间戳与互转
来源：http://ndv.nwbrower.top

date +%s;  date -d @1700000000
来源：http://wbp.gaohongyu789.top

[R71] 日期格式化
来源：http://lmd.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://okg.yueranfly.top

[R72] 等待端口就绪
来源：http://pvq.gotoacloud.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qhf.ivvv.top

[R73] 分割大日志
来源：http://dmf.wangdashe.top

split -l 1000 big.log part_
来源：http://aum.zycfv.cn

[R74] 批量重命名
来源：http://hlr.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ils.daria6918.cn

[R75] 导出环境变量
来源：http://qgd.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://hxz.yanxiufei.cn

[R76] 使用临时文件
来源：http://mnf.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vcy.xziqi.cn

[R77] 读取用户输入
来源：http://fni.guowangkeji.top

read -rp "请输入: " ans
来源：http://txg.yonumen.top

[R78] 交互式菜单
来源：http://pxq.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dcc.sjlbkw.cn

[R79] 解析命令行选项
来源：http://xxf.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lyh.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://gqj.pycfn.com

time ./run.sh
来源：http://bzl.ivvv.top

================================================================================
来源：http://ghp.hcnkem.com

S. C / C++ 专题
来源：http://cqi.hcnkem.com

================================================================================
来源：http://kdv.yanxiufei.cn

[S01] C：Hello World
来源：http://att.yuxming.cn

#include <stdio.h>
来源：http://ieg.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kez.redwolf501.top

[S02] C：变量与格式化输出
来源：http://ezm.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://sxd.redwolf501.top

[S03] C：读入整数
来源：http://czd.iojbl.cn

int x; scanf("%d", &x);
来源：http://fsn.chenjidiqi.icu

[S04] C：字符串复制
来源：http://fco.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kwq.tianlin.xyz

[S05] C：字符串长度
来源：http://pyi.aizwys.cn

strlen(s)
来源：http://mkp.0kj1m.cn

[S06] C：字符串比较
来源：http://bru.smart0.xyz

strcmp(a, b) == 0
来源：http://scy.guannengcc.top

[S07] C：数组遍历求和
来源：http://igg.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fze.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://kro.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kom.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://ujv.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uur.yangfankeji.com

[S10] C：指针与解引用
来源：http://uli.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://lvu.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://fyh.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://uxq.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://lhh.quarkkingdee.top

fclose(f);
来源：http://pqs.gotoacloud.top

[S12] C：写文件
来源：http://yoe.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zdt.ydzc1.top

[S13] C：宏定义
来源：http://grj.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gxv.c1oappe.top

[S14] C：枚举
来源：http://zjn.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://ceg.feifeiyinyue.top

[S15] C：类型转换
来源：http://urw.sweek.top

(double) a / b
来源：http://sub.yj20258888.top

[S16] C：位操作置位
来源：http://upf.jianghu66.top

x |= (1 << 3);
来源：http://yjw.tian-w.cn

[S17] C：安全拼接字符串
来源：http://ugk.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wzz.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://mtr.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://bqz.0kj1m.cn

[S19] C：快速排序
来源：http://opb.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://pfk.hnqzz.top

[S20] C：二分查找
来源：http://dbk.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fue.zhoulong.xyz

[S21] C：字符类别判断
来源：http://ver.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bsl.yj202588.top

[S22] C：字符串转数字
来源：http://dik.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://lpv.tanke756.top

[S23] C：随机数
来源：http://dqr.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jit.chenzaomai.com

[S24] C：获取本地时间
来源：http://pix.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://khz.zhixingplan.top

[S25] C：内存拷贝
来源：http://msf.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://hqb.yanxiufei.cn

[S26] C：内存清零
来源：http://uxe.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://zjf.zycfv.cn

[S27] C：定义常量
来源：http://ybi.zhijiandao.cn

const double PI = 3.14159;
来源：http://bod.shuidangran.top

[S28] C：静态变量
来源：http://vid.cashguo.top

static int counter = 0;
来源：http://ypm.jinqigufen.top

[S29] C：变参函数
来源：http://qho.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vbl.yuanzhike.top

[S30] C：头文件保护
来源：http://kvu.chenjidiqi.icu

#ifndef X_H
来源：http://oua.yueranfly.top

#define X_H
来源：http://hit.zycfv.cn

#endif
来源：http://dug.smart0.xyz

[S31] C++：Hello World
来源：http://ppe.fengsongda.top

#include <iostream>
来源：http://ado.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://yxi.pycfn.com

[S32] C++：字符串
来源：http://iwx.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://tqu.zdbjq.cn

[S33] C++：vector 增删
来源：http://yag.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uxz.tarul.cn

[S34] C++：遍历 vector
来源：http://sbv.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://occ.fktsv.cn

[S35] C++：map
来源：http://enj.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eie.chenzaomai.com

[S36] C++：unordered_map
来源：http://qdr.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wat.316326.xyz

[S37] C++：set
来源：http://idj.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fun.316326.xyz

[S38] C++：排序
来源：http://tpu.yj20258.top

std::sort(v.begin(), v.end());
来源：http://nyr.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://lrr.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kgv.meibo888.top

[S40] C++：查找元素
来源：http://och.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bxj.fzhhl.top

[S41] C++：类与构造函数
来源：http://wek.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gtp.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://ojh.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://yrm.haohaochexian.top

[S43] C++：智能指针
来源：http://gja.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://rjm.jlsjyb.cn

[S44] C++：引用传参
来源：http://dln.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://yoa.ppjwa.cn

[S45] C++：lambda
来源：http://kjc.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://wey.yangfankeji.com

[S46] C++：函数模板
来源：http://ymb.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bdz.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://gix.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jjw.ctjpmb.com

[S48] C++：逐行读文件
来源：http://nwe.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://nvy.yj202588.top

while (std::getline(in, line)) { }
来源：http://fxr.gzhubu.top

[S49] C++：写文件
来源：http://zfx.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cmy.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://jpl.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://otw.uphjek.com

[S51] C++：显式类型转换
来源：http://vwf.tarul.cn

static_cast<double>(a) / b
来源：http://wat.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://uhn.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://wif.gogol.net.cn

[S53] C++：移动语义
来源：http://oaz.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://keq.daxiang520.top

[S54] C++：异常处理
来源：http://gpm.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hhb.svipenyu.cn

[S55] C++：结构化绑定
来源：http://kfs.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wql.shzxlz.cn

[S56] C++：optional
来源：http://tjd.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yho.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://ycs.zdbjq.cn

constexpr int N = 10;
来源：http://ren.haohaochexian.top

[S58] C++：命名空间
来源：http://rwu.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://ndv.jqgfzy.top

[S59] C++：静态断言
来源：http://qdj.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jlw.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://oly.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nlf.chenjidiqi.icu

================================================================================
来源：http://lzs.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxa.xingfuxueyuan.xyz

================================================================================
来源：http://hdk.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://dyg.bjfxy.top

println("Hello")
来源：http://her.birdmap.top

[T02] Kotlin：变量
来源：http://lav.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ckx.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://pcu.sweek.top

"值: $b"
来源：http://zww.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://dhx.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://tsa.yj202588.top

[T05] Kotlin：when 表达式
来源：http://lua.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://frp.gzhubu.top

[T06] Kotlin：集合映射
来源：http://buj.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://llj.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://sba.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jvo.snrcjt.cn

[T08] Kotlin：数据类
来源：http://tsk.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://jmu.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://nad.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://xko.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://pec.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ylc.52xcode.cn

[T11] Kotlin：协程
来源：http://bcu.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://deu.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://tpf.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://wrd.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://ksc.xuanzx.com

val m = mapOf("a" to 1)
来源：http://sba.zhongyouzk.top

[T14] Kotlin：循环
来源：http://nst.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://jfq.nanxinkj.top

[T15] Kotlin：接口
来源：http://xcw.sweek.top

interface Shape { fun area(): Double }
来源：http://gun.shuidangran.top

[T16] Swift：Hello World
来源：http://dro.zdqjudy.top

print("Hello")
来源：http://mrr.smart0.xyz

[T17] Swift：变量与常量
来源：http://nay.nanxinkj.top

var a = 1;  let b = 2
来源：http://lni.guannengcc.top

[T18] Swift：字符串插值
来源：http://loo.fengsongda.top

"值: \(b)"
来源：http://ems.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://nln.sufxvd.cn

if let n = opt { print(n) }
来源：http://vxs.hfpthk.cn

[T20] Swift：数组操作
来源：http://vrs.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://qfs.ybcxt.top

[T21] Swift：遍历
来源：http://whh.zdqjudy.top

for x in a { print(x) }
来源：http://zsp.yueranfly.top

[T22] Swift：字典
来源：http://ehf.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://xrv.fzhhl.top

[T23] Swift：函数
来源：http://jur.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sdr.jyoumei.cn

[T24] Swift：闭包
来源：http://jkq.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aqf.hesvh.cn

[T25] Swift：结构体
来源：http://dhz.jinghuilouyu.cn

struct P { var x: Int }
来源：http://vvv.sjlbkw.cn

[T26] Swift：类与重写
来源：http://lbd.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://wpe.ivvv.top

[T27] Swift：错误处理
来源：http://lbo.epnwcf.com

do { try f() } catch { print(error) }
来源：http://izz.yangfankeji.com

[T28] Swift：枚举
来源：http://aft.sxryk.cn

enum Color { case red, green }
来源：http://qim.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://qqb.xuetiantiany.cn

guard let x = opt else { return }
来源：http://jde.fehbvm.com

[T30] Swift：协议
来源：http://egx.yj202588.top

protocol Shape { func area() -> Double }
来源：http://cxp.guannengcc.top

[T31] Lua：Hello World
来源：http://ewk.yongpay.top

print("Hello")
来源：http://plb.yueranfly.top

[T32] Lua：局部变量
来源：http://rlt.yongpay.top

local a = 1
来源：http://rnm.snrcjt.cn

[T33] Lua：表（数组）
来源：http://mdt.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://qfu.yonumen.top

[T34] Lua：遍历表
来源：http://olh.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://tjt.yangfankeji.com

[T35] Lua：字典表
来源：http://xxn.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://etg.jlsjyb.cn

[T36] Lua：函数
来源：http://jzu.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://qcs.vehdjk.com

[T37] Lua：字符串拼接
来源：http://pym.yuanzhike.top

"a" .. "b"
来源：http://lox.epnwcf.com

[T38] Lua：条件
来源：http://exq.yvedp.cn

if x > 0 then print("正") end
来源：http://tas.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://ffl.ctjpmb.com

string.find(s, "%d+")
来源：http://rxb.zycfv.cn

[T40] Lua：元表
来源：http://rla.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://qci.c1oappe.top

[T41] Perl：Hello World
来源：http://maf.redwolf501.top

print "Hello\n";
来源：http://uul.xinyue.icu

[T42] Perl：变量类型
来源：http://gih.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yel.cqqwz.cn

[T43] Perl：字符串插值
来源：http://nhg.tian-w.cn

"值: $a"
来源：http://txq.ehwqpu.com

[T44] Perl：条件
来源：http://azz.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://uzc.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://jwv.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://wce.bbcook.cn

[T46] Perl：哈希操作
来源：http://qxp.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rcn.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://ddk.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yls.yanxiufei.cn

[T48] Perl：正则替换
来源：http://bis.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://qeo.xuanzx.com

[T49] Perl：函数
来源：http://kld.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qec.hnqzz.top

[T50] Perl：逐行读文件
来源：http://zys.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gvb.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://qvh.tarul.cn

[T51] Scala：Hello World
来源：http://ibk.jinyuanbaomall.cn

println("Hello")
来源：http://vfs.cashguo.top

[T52] Scala：变量
来源：http://enb.sweek.top

val a = 1;  var b = 2
来源：http://zbn.jiagoushi.top

[T53] Scala：字符串插值
来源：http://sfe.xingfuxueyuan.xyz

s"值: $b"
来源：http://bqu.quarkkingdee.top

[T54] Scala：集合映射
来源：http://cdp.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://okd.fehbvm.com

[T55] Scala：集合过滤
来源：http://wtj.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://raz.daxiang520.top

[T56] Scala：样例类
来源：http://iau.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://ohk.shzxlz.cn

[T57] Scala：模式匹配
来源：http://wbi.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://beq.andypj.xyz

[T58] Scala：函数定义
来源：http://wja.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kal.yfazqb.com

[T59] Scala：循环
来源：http://zer.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://vez.epnwcf.com

[T60] Scala：折叠
来源：http://mfb.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://azz.sweek.top

================================================================================
来源：http://eiz.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xow.hesvh.cn

================================================================================
来源：http://zxi.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://hpq.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vjx.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://inj.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eur.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://gcx.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://mgv.sufxvd.cn

[U04] Py：变量调试打印
来源：http://mtj.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nym.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://ayt.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://axs.bjfxy.top

[U06] Py：合并两个字典
来源：http://rbz.ctjpmb.com

{**a, **b}
来源：http://skt.yuanzhike.top


<!-- 参考信息 -->