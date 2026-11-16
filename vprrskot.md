代发 wailian999

df -h;  du -sh *
来源：http://odt.cucudq.cn

[R62] 找最占空间的文件
来源：http://rjm.tanke756.top

du -ah . | sort -rh | head -10
来源：http://zku.xuetiantiany.cn

[R63] 内存与进程
来源：http://ank.pycfn.com

free -h;  ps aux | grep nginx
来源：http://ajh.yonumen.top

[R64] 结束进程
来源：http://icj.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://uhv.sysykeji.top

[R65] 查看端口占用
来源：http://kdj.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kes.yueranfly.top

[R66] 定时任务
来源：http://pmj.316326.xyz

crontab -e;  crontab -l
来源：http://zkh.ydzc1.top

[R67] 生成随机十六进制串
来源：http://oqc.hnxiangtu.top

openssl rand -hex 16
来源：http://zqe.hysaishi.cn

[R68] 计算文件校验值
来源：http://okf.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://lmk.tarul.cn

[R69] 生成随机密码
来源：http://slx.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://wer.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://qaq.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://bpp.mhx1999.top

[R71] 日期格式化
来源：http://irn.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qgj.epnwcf.com

[R72] 等待端口就绪
来源：http://qky.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://itw.hnqzz.top

[R73] 分割大日志
来源：http://jge.tarul.cn

split -l 1000 big.log part_
来源：http://vhi.hysaishi.cn

[R74] 批量重命名
来源：http://jlh.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vuv.xziqi.cn

[R75] 导出环境变量
来源：http://iuc.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://nnl.yj20258888.top

[R76] 使用临时文件
来源：http://hov.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxd.ppjwa.cn

[R77] 读取用户输入
来源：http://mgk.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://peu.cdnleiting.top

[R78] 交互式菜单
来源：http://lta.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bis.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://trs.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zlt.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://btu.aizwys.cn

time ./run.sh
来源：http://tdp.zdbjq.cn

================================================================================
来源：http://vab.sxryk.cn

S. C / C++ 专题
来源：http://vza.zhaomingkeji.xyz

================================================================================
来源：http://lgl.jinqigfzy.top

[S01] C：Hello World
来源：http://lay.shzxlz.cn

#include <stdio.h>
来源：http://loy.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vaw.yfazqb.com

[S02] C：变量与格式化输出
来源：http://paw.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://fgv.zhongyouzk.top

[S03] C：读入整数
来源：http://lpe.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://edt.sxryk.cn

[S04] C：字符串复制
来源：http://mbx.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://qtf.feifeiyinyue.top

[S05] C：字符串长度
来源：http://zwm.dashuyun.cn

strlen(s)
来源：http://nms.yfazqb.com

[S06] C：字符串比较
来源：http://kpa.nanxuanxn.top

strcmp(a, b) == 0
来源：http://bqs.jinqigufen.top

[S07] C：数组遍历求和
来源：http://fqj.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://urn.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://dbn.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zgb.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://toj.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aep.ehwqpu.com

[S10] C：指针与解引用
来源：http://nql.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://hky.yuanzhike.top

[S11] C：逐行读文件
来源：http://jne.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://ocu.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wla.shanyushiyangkeji.top

fclose(f);
来源：http://ruh.zhiwuduotai.top

[S12] C：写文件
来源：http://oax.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ivj.xuanzx.com

[S13] C：宏定义
来源：http://hyo.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwt.shuidangran.top

[S14] C：枚举
来源：http://njh.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://qod.yonumen.top

[S15] C：类型转换
来源：http://edm.nanxinkj.top

(double) a / b
来源：http://fcc.quarkkingdee.top

[S16] C：位操作置位
来源：http://bhy.zdbjq.cn

x |= (1 << 3);
来源：http://gbm.ybcxt.top

[S17] C：安全拼接字符串
来源：http://fgp.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rfk.zhongyouzk.top

[S18] C：命令行参数
来源：http://kxb.gzhubu.top

int main(int argc, char **argv)
来源：http://vvp.bjfxy.top

[S19] C：快速排序
来源：http://cmb.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://vkw.wangdashe.top

[S20] C：二分查找
来源：http://uxv.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://whs.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://fxc.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rnn.shuidangran.top

[S22] C：字符串转数字
来源：http://trl.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xny.havefunace.top

[S23] C：随机数
来源：http://lqg.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qwe.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://fgd.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://clq.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://hxm.fengsongda.top

memcpy(dst, src, n);
来源：http://bvw.cqqwz.cn

[S26] C：内存清零
来源：http://jbr.fzhhl.top

memset(a, 0, sizeof a);
来源：http://ctp.guowangkeji.top

[S27] C：定义常量
来源：http://soe.fktsv.cn

const double PI = 3.14159;
来源：http://lcc.yj20258.top

[S28] C：静态变量
来源：http://hia.andypj.xyz

static int counter = 0;
来源：http://sms.hcnkem.com

[S29] C：变参函数
来源：http://caw.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kny.yj202588.top

[S30] C：头文件保护
来源：http://ewi.nwbrower.top

#ifndef X_H
来源：http://sse.hfpthk.cn

#define X_H
来源：http://koj.fehbvm.com

#endif
来源：http://ofr.smart0.xyz

[S31] C++：Hello World
来源：http://occ.gaohongyu789.top

#include <iostream>
来源：http://bai.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://naa.wangshuangyany.cn

[S32] C++：字符串
来源：http://lij.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://zeh.yonumen.top

[S33] C++：vector 增删
来源：http://omg.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://swc.yj20258.top

[S34] C++：遍历 vector
来源：http://mle.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://pmd.andypj.xyz

[S35] C++：map
来源：http://yvd.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hqr.fengsongda.top

[S36] C++：unordered_map
来源：http://qjw.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iqa.zhiwuduotai.top

[S37] C++：set
来源：http://emq.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ogl.snrcjt.cn

[S38] C++：排序
来源：http://der.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://sdi.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://acd.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qrp.tanke756.top

[S40] C++：查找元素
来源：http://orv.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qua.yuanzhike.top

[S41] C++：类与构造函数
来源：http://fmt.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://loc.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://rbg.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://dyt.316326.xyz

[S43] C++：智能指针
来源：http://zsl.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://fay.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://uug.c1oappe.top

void inc(int &x) { ++x; }
来源：http://frr.yangfankeji.com

[S45] C++：lambda
来源：http://pgh.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ucd.9152youxi.cn

[S46] C++：函数模板
来源：http://wye.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ork.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://ttn.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucx.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://vqo.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://jun.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://ubv.xinyue.icu

[S49] C++：写文件
来源：http://mfl.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nvu.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://nhi.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yxc.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://npm.jianghu66.top

static_cast<double>(a) / b
来源：http://bui.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://msu.birdmap.top

int size() const noexcept { return n_; }
来源：http://ezo.ppjwa.cn

[S53] C++：移动语义
来源：http://xjc.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://nwh.hywenlv.cn

[S54] C++：异常处理
来源：http://tqw.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mok.jqgfzy.top

[S55] C++：结构化绑定
来源：http://mkp.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ubo.aizwys.cn

[S56] C++：optional
来源：http://mkk.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qiv.yongpay.top

[S57] C++：编译期常量
来源：http://fff.yuanzhike.top

constexpr int N = 10;
来源：http://zjw.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://hdg.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://fep.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://vnm.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zvm.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://ffv.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jih.yvedp.cn

================================================================================
来源：http://qel.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ibn.ydzc1.top

================================================================================
来源：http://jnx.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://btb.yueranfly.top

println("Hello")
来源：http://zrl.cucudq.cn

[T02] Kotlin：变量
来源：http://vus.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jgm.meibo888.top

[T03] Kotlin：字符串模板
来源：http://trx.xuanzx.com

"值: $b"
来源：http://wpp.uphjek.com

[T04] Kotlin：空安全
来源：http://loh.ybcxt.top

val n: String? = null;  n?.length
来源：http://rsb.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://xnz.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxc.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://rqt.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://llu.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://ghz.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ptm.ybcxt.top

[T08] Kotlin：数据类
来源：http://owj.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://rna.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://skz.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://opq.ivvv.top

[T10] Kotlin：默认参数
来源：http://lsi.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qzj.hnqzz.top

[T11] Kotlin：协程
来源：http://wxj.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ahq.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://lxy.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://ozq.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://jqh.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://otf.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://afo.sufxvd.cn

for (i in 1..10) println(i)
来源：http://azw.quarkkingdee.top

[T15] Kotlin：接口
来源：http://njn.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://qha.yj20258888.top

[T16] Swift：Hello World
来源：http://lvj.xziqi.cn

print("Hello")
来源：http://kke.hysaishi.cn

[T17] Swift：变量与常量
来源：http://hgl.yuxming.cn

var a = 1;  let b = 2
来源：http://qvw.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://pwq.hongshengwenyu.top

"值: \(b)"
来源：http://ksh.hysaishi.cn

[T19] Swift：可选绑定
来源：http://trf.bbcook.cn

if let n = opt { print(n) }
来源：http://jfv.gaohongyu789.top

[T20] Swift：数组操作
来源：http://gni.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cya.gogol.net.cn

[T21] Swift：遍历
来源：http://umo.iojbl.cn

for x in a { print(x) }
来源：http://bzj.hcnkem.com

[T22] Swift：字典
来源：http://sic.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jhl.redwolf501.top

[T23] Swift：函数
来源：http://bef.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dat.zdqjudy.top

[T24] Swift：闭包
来源：http://zvq.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pip.chenjidiqi.icu

[T25] Swift：结构体
来源：http://kcc.epnwcf.com

struct P { var x: Int }
来源：http://coj.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://pxi.nanxinkj.top

class A: Base { override func f() {} }
来源：http://pfx.fengsongda.top

[T27] Swift：错误处理
来源：http://ccu.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://hez.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://sma.nanxuanxn.top

enum Color { case red, green }
来源：http://ugk.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://pet.hnxiangtu.top

guard let x = opt else { return }
来源：http://gwa.wangshuangyany.cn

[T30] Swift：协议
来源：http://dec.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://vii.daxiang520.top

[T31] Lua：Hello World
来源：http://abn.hesvh.cn

print("Hello")
来源：http://rwh.chenlongwang.top

[T32] Lua：局部变量
来源：http://hnq.zdqjudy.top

local a = 1
来源：http://ajy.dianchejie.cn

[T33] Lua：表（数组）
来源：http://tdn.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xtk.hammf.cn

[T34] Lua：遍历表
来源：http://aux.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ayb.tarul.cn

[T35] Lua：字典表
来源：http://mxb.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://eyz.guannengcc.top

[T36] Lua：函数
来源：http://quv.guowangkeji.top

function add(a, b) return a + b end
来源：http://zwf.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://fly.pycfn.com

"a" .. "b"
来源：http://wkx.hywenlv.cn

[T38] Lua：条件
来源：http://ual.hfpthk.cn

if x > 0 then print("正") end
来源：http://gxr.havefunace.top

[T39] Lua：模式匹配
来源：http://koq.vqdsnc.cn

string.find(s, "%d+")
来源：http://gdq.xinyue.icu

[T40] Lua：元表
来源：http://abh.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://yrj.ydjk.org.cn

[T41] Perl：Hello World
来源：http://hwk.jinyuanbaomall.cn

print "Hello\n";
来源：http://awy.havefunace.top

[T42] Perl：变量类型
来源：http://ycf.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ilb.tanke756.top

[T43] Perl：字符串插值
来源：http://lbk.xuetiantiany.cn

"值: $a"
来源：http://caj.snrcjt.cn

[T44] Perl：条件
来源：http://xzx.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://tzl.yvedp.cn

[T45] Perl：数组遍历
来源：http://whc.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://kbv.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://ijl.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fvn.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://eio.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hix.zhixingplan.top

[T48] Perl：正则替换
来源：http://xdw.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://gte.jianghu66.top

[T49] Perl：函数
来源：http://bcd.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jwy.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://qiy.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oby.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://qiz.xuanzx.com

[T51] Scala：Hello World
来源：http://rlj.cdnleiting.top

println("Hello")
来源：http://mkl.fktsv.cn

[T52] Scala：变量
来源：http://ems.zdbjq.cn

val a = 1;  var b = 2
来源：http://ppl.zycfv.cn

[T53] Scala：字符串插值
来源：http://mdg.havefunace.top

s"值: $b"
来源：http://zce.epnwcf.com

[T54] Scala：集合映射
来源：http://bau.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://pqo.ctjpmb.com

[T55] Scala：集合过滤
来源：http://efw.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rva.zhiwuduotai.top

[T56] Scala：样例类
来源：http://zvc.zhixingplan.top

case class User(name: String, age: Int)
来源：http://dee.yj20258.top

[T57] Scala：模式匹配
来源：http://lrr.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hzd.shzxlz.cn

[T58] Scala：函数定义
来源：http://dvj.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rid.jqgufenzy.top

[T59] Scala：循环
来源：http://jno.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://rhw.gogol.net.cn

[T60] Scala：折叠
来源：http://wxj.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rgg.ydjk.org.cn

================================================================================
来源：http://xiz.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pkb.yonumen.top

================================================================================
来源：http://pgr.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://muf.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://kyj.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://lfl.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wet.ppjwa.cn


<!-- 参考信息 -->