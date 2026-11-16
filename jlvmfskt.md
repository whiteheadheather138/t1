代发 wailian999

ssh user@host 'uptime'
来源：http://nnh.fanxiaobao.xyz

[R58] 下载文件
来源：http://kva.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eql.cheryme.top

[R59] 发 POST JSON
来源：http://cfq.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ozz.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://mkp.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vhv.jinqigfzy.top

[R61] 磁盘占用
来源：http://mjv.tarul.cn

df -h;  du -sh *
来源：http://kqg.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://rky.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://gev.jqgufenzy.top

[R63] 内存与进程
来源：http://ale.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://hnr.sjlbkw.cn

[R64] 结束进程
来源：http://jqv.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://dgw.iojbl.cn

[R65] 查看端口占用
来源：http://tia.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjb.quarkkingdee.top

[R66] 定时任务
来源：http://jsd.yuxming.cn

crontab -e;  crontab -l
来源：http://iwt.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://iim.vehdjk.com

openssl rand -hex 16
来源：http://oio.jinqigfzy.top

[R68] 计算文件校验值
来源：http://oxi.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ttn.iojbl.cn

[R69] 生成随机密码
来源：http://ckj.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://tif.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://dks.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://ltn.sjlbkw.cn

[R71] 日期格式化
来源：http://ogk.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ytr.bbcook.cn

[R72] 等待端口就绪
来源：http://lxf.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cyp.9152youxi.cn

[R73] 分割大日志
来源：http://rtb.jinqigufen.top

split -l 1000 big.log part_
来源：http://djq.jqgfzy.top

[R74] 批量重命名
来源：http://xch.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eij.c1oappe.top

[R75] 导出环境变量
来源：http://ilz.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://xih.gogol.net.cn

[R76] 使用临时文件
来源：http://jpo.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gil.hongshengwenyu.top

[R77] 读取用户输入
来源：http://xhz.nanxinkj.top

read -rp "请输入: " ans
来源：http://ffw.quarkkingdee.top

[R78] 交互式菜单
来源：http://wow.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oxa.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://pxk.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bpa.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://pdt.zdbjq.cn

time ./run.sh
来源：http://erj.gogol.net.cn

================================================================================
来源：http://ayz.yj20258.top

S. C / C++ 专题
来源：http://vnc.zhaomingkeji.xyz

================================================================================
来源：http://bmp.tian-w.cn

[S01] C：Hello World
来源：http://vsk.yvedp.cn

#include <stdio.h>
来源：http://snm.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eru.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://lxf.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://gzu.wangdashe.top

[S03] C：读入整数
来源：http://buo.yj20258888.top

int x; scanf("%d", &x);
来源：http://rkl.zhixingplan.top

[S04] C：字符串复制
来源：http://bfr.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://bva.zhixingplan.top

[S05] C：字符串长度
来源：http://lsq.bbcook.cn

strlen(s)
来源：http://owr.yangfankeji.com

[S06] C：字符串比较
来源：http://sjq.fzhhl.top

strcmp(a, b) == 0
来源：http://htb.zycfv.cn

[S07] C：数组遍历求和
来源：http://anu.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xwu.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://tdl.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mat.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://buj.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qjj.tarul.cn

[S10] C：指针与解引用
来源：http://otw.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://jvh.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://jkv.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://ijo.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hzo.jiagoushi.top

fclose(f);
来源：http://iph.xuetiantiany.cn

[S12] C：写文件
来源：http://apu.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://txr.0kj1m.cn

[S13] C：宏定义
来源：http://bev.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bjx.yuanzhike.top

[S14] C：枚举
来源：http://cck.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://baa.xuetiantiany.cn

[S15] C：类型转换
来源：http://ugp.ppjwa.cn

(double) a / b
来源：http://smf.vqdsnc.cn

[S16] C：位操作置位
来源：http://hld.bbcook.cn

x |= (1 << 3);
来源：http://hil.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://iii.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kmk.snrcjt.cn

[S18] C：命令行参数
来源：http://ypq.kuanghao11.cn

int main(int argc, char **argv)
来源：http://sxw.yuanzhike.top

[S19] C：快速排序
来源：http://wbk.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://zra.fehbvm.com

[S20] C：二分查找
来源：http://ovr.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ccp.ydzc1.top

[S21] C：字符类别判断
来源：http://vya.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://svp.uphjek.com

[S22] C：字符串转数字
来源：http://rwy.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://ezp.gotoacloud.top

[S23] C：随机数
来源：http://vqn.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xbo.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://hrx.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rub.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://oju.yfazqb.com

memcpy(dst, src, n);
来源：http://ajc.hfpthk.cn

[S26] C：内存清零
来源：http://did.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://zyx.hammf.cn

[S27] C：定义常量
来源：http://jdm.epnwcf.com

const double PI = 3.14159;
来源：http://gnb.yfazqb.com

[S28] C：静态变量
来源：http://zxp.yj202588.top

static int counter = 0;
来源：http://xff.gogol.net.cn

[S29] C：变参函数
来源：http://hoy.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gac.shangyingyoupin.top

[S30] C：头文件保护
来源：http://bol.nanxinkj.top

#ifndef X_H
来源：http://qqc.yongpay.top

#define X_H
来源：http://nle.fehbvm.com

#endif
来源：http://vwp.redwolf501.top

[S31] C++：Hello World
来源：http://cyp.yonumen.top

#include <iostream>
来源：http://bui.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://hsf.ppjwa.cn

[S32] C++：字符串
来源：http://mbw.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://zup.chenzaomai.com

[S33] C++：vector 增删
来源：http://zkt.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zcp.fehbvm.com

[S34] C++：遍历 vector
来源：http://bjo.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://coo.jinyuanbaomall.cn

[S35] C++：map
来源：http://jbz.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cdi.bjfxy.top

[S36] C++：unordered_map
来源：http://fao.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://obb.yuxming.cn

[S37] C++：set
来源：http://beb.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vbd.yj20258.top

[S38] C++：排序
来源：http://phq.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://yzm.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://iju.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vzf.cashguo.top

[S40] C++：查找元素
来源：http://dbh.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cef.daxiang520.top

[S41] C++：类与构造函数
来源：http://ahb.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fzs.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://nqx.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://hci.xziqi.cn

[S43] C++：智能指针
来源：http://dfg.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://mhe.jianghu66.top

[S44] C++：引用传参
来源：http://epm.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://kow.jqgufenzy.top

[S45] C++：lambda
来源：http://wxg.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://fvo.yanxiufei.cn

[S46] C++：函数模板
来源：http://ooy.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ctz.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://kon.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgk.cdnleiting.top

[S48] C++：逐行读文件
来源：http://zyj.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://rqx.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://zvo.feifeiyinyue.top

[S49] C++：写文件
来源：http://drr.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kyq.sysykeji.top

[S50] C++：格式化数字
来源：http://bcz.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ogg.uphjek.com

[S51] C++：显式类型转换
来源：http://wgc.aizwys.cn

static_cast<double>(a) / b
来源：http://nfi.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://yfy.ydzc1.top

int size() const noexcept { return n_; }
来源：http://aqe.zhongyouzk.top

[S53] C++：移动语义
来源：http://oau.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://xpy.shangyingyoupin.top

[S54] C++：异常处理
来源：http://oxx.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eht.sxryk.cn

[S55] C++：结构化绑定
来源：http://wku.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://pza.jinghuilouyu.cn

[S56] C++：optional
来源：http://jik.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vqu.c1oappe.top

[S57] C++：编译期常量
来源：http://jhb.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://khf.sysykeji.top

[S58] C++：命名空间
来源：http://gwe.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://mka.daria6918.cn

[S59] C++：静态断言
来源：http://xcl.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tyn.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://onm.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://piu.nwbrower.top

================================================================================
来源：http://fxk.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://szh.zhaomingkeji.xyz

================================================================================
来源：http://zxt.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://whv.jqgfzy.top

println("Hello")
来源：http://mfr.quarkkingdee.top

[T02] Kotlin：变量
来源：http://mxl.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qkv.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://rjh.ivvv.top

"值: $b"
来源：http://vgo.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://dcf.zhengqikj.top

val n: String? = null;  n?.length
来源：http://cic.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://tzz.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ncl.zycfv.cn

[T06] Kotlin：集合映射
来源：http://por.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://hto.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://umv.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://asn.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://cgn.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://wop.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://wyb.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://xcr.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://shz.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mhv.aibaodan.cn

[T11] Kotlin：协程
来源：http://lec.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jlo.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://yqa.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://unv.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://cqf.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://gwr.ydzc1.top

[T14] Kotlin：循环
来源：http://hbe.yvedp.cn

for (i in 1..10) println(i)
来源：http://unq.tanke756.top

[T15] Kotlin：接口
来源：http://ivc.meibo888.top

interface Shape { fun area(): Double }
来源：http://kvn.gzhubu.top

[T16] Swift：Hello World
来源：http://iux.mhx1999.top

print("Hello")
来源：http://izk.hnqzz.top

[T17] Swift：变量与常量
来源：http://izg.xziqi.cn

var a = 1;  let b = 2
来源：http://lui.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://dez.dashuyun.cn

"值: \(b)"
来源：http://wez.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://xjn.uphjek.com

if let n = opt { print(n) }
来源：http://ubm.zhengqikj.top

[T20] Swift：数组操作
来源：http://lvj.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://tsj.aibaodan.cn

[T21] Swift：遍历
来源：http://qvi.ivvv.top

for x in a { print(x) }
来源：http://lbt.dashuyun.cn

[T22] Swift：字典
来源：http://wtk.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://xqx.fktsv.cn

[T23] Swift：函数
来源：http://eih.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://alm.0kj1m.cn

[T24] Swift：闭包
来源：http://bax.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dcw.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://rlr.shanyushiyangtech.top

struct P { var x: Int }
来源：http://wui.yuxming.cn

[T26] Swift：类与重写
来源：http://hun.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://ulj.svipenyu.cn

[T27] Swift：错误处理
来源：http://sgq.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://ppq.zhoulong.xyz

[T28] Swift：枚举
来源：http://fbz.xylfe.cn

enum Color { case red, green }
来源：http://jbe.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://qdn.yj202588.top

guard let x = opt else { return }
来源：http://ekd.feifeiyinyue.top

[T30] Swift：协议
来源：http://ozb.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://uvd.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://yrg.yj202588.top

print("Hello")
来源：http://ugx.meibo888.top

[T32] Lua：局部变量
来源：http://zrc.52xcode.cn

local a = 1
来源：http://yfy.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://fdy.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qvo.yangfankeji.com

[T34] Lua：遍历表
来源：http://rkz.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fcf.wangdashe.top

[T35] Lua：字典表
来源：http://heq.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://gmw.kuanghao11.cn

[T36] Lua：函数
来源：http://evb.cqqwz.cn

function add(a, b) return a + b end
来源：http://btx.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://uwm.dianchejie.cn

"a" .. "b"
来源：http://ral.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://uus.jqgufenzy.top

if x > 0 then print("正") end
来源：http://prx.redwolf501.top

[T39] Lua：模式匹配
来源：http://vyh.chenjidiqi.icu

string.find(s, "%d+")
来源：http://qwj.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://ann.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://cnx.ppjwa.cn

[T41] Perl：Hello World
来源：http://imu.ybcxt.top

print "Hello\n";
来源：http://cmx.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://cgb.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lqf.fktsv.cn

[T43] Perl：字符串插值
来源：http://clv.ehwqpu.com

"值: $a"
来源：http://lgy.aizwys.cn

[T44] Perl：条件
来源：http://zks.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://ryy.iojbl.cn

[T45] Perl：数组遍历
来源：http://nli.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://gda.fktsv.cn

[T46] Perl：哈希操作
来源：http://rtu.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bmb.sweek.top

[T47] Perl：正则捕获
来源：http://alx.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lzd.zhongyouzk.top

[T48] Perl：正则替换
来源：http://vyt.daxiang520.top

$s =~ s/old/new/g;
来源：http://lut.smart0.xyz

[T49] Perl：函数
来源：http://cnt.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iae.yj20258888.top

[T50] Perl：逐行读文件
来源：http://tni.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dsj.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://elm.tarul.cn

[T51] Scala：Hello World
来源：http://cjq.shangyingyoupin.top

println("Hello")
来源：http://cth.vqdsnc.cn

[T52] Scala：变量
来源：http://nwj.cucudq.cn

val a = 1;  var b = 2
来源：http://zrw.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://ruj.jinyuanbaomall.cn

s"值: $b"
来源：http://rge.hnxiangtu.top

[T54] Scala：集合映射
来源：http://fud.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://ulj.chenzaomai.com

[T55] Scala：集合过滤
来源：http://ytq.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://wrz.ydjk.org.cn

[T56] Scala：样例类
来源：http://shx.zdqjudy.top

case class User(name: String, age: Int)
来源：http://kab.yuxming.cn

[T57] Scala：模式匹配
来源：http://faf.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ifj.aizwys.cn

[T58] Scala：函数定义
来源：http://ecd.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://tym.smart0.xyz

[T59] Scala：循环
来源：http://fqh.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://jqj.svipenyu.cn

[T60] Scala：折叠
来源：http://iek.jinqigfzy.top


<!-- 参考信息 -->