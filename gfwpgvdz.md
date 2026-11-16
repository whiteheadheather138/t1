代发 wailian999

ssh user@host 'uptime'
来源：http://wgu.jiagoushi.top

[R58] 下载文件
来源：http://gyp.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hqm.hnqzz.top

[R59] 发 POST JSON
来源：http://ibw.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kvz.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://mpl.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ntp.sxryk.cn

[R61] 磁盘占用
来源：http://adc.wangdashe.top

df -h;  du -sh *
来源：http://aok.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://rje.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://ezs.jinqigfzy.top

[R63] 内存与进程
来源：http://xpv.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://plf.hywenlv.cn

[R64] 结束进程
来源：http://vja.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://jle.gogol.net.cn

[R65] 查看端口占用
来源：http://ysh.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fie.sysykeji.top

[R66] 定时任务
来源：http://ild.yfazqb.com

crontab -e;  crontab -l
来源：http://mtl.andypj.xyz

[R67] 生成随机十六进制串
来源：http://agi.wangdashe.top

openssl rand -hex 16
来源：http://uao.nanxuanxn.top

[R68] 计算文件校验值
来源：http://ybx.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://jkv.yangfankeji.com

[R69] 生成随机密码
来源：http://zyq.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://jfx.gotoacloud.top

[R70] 时间戳与互转
来源：http://qfb.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://pgs.yfazqb.com

[R71] 日期格式化
来源：http://xgd.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jna.cdnleiting.top

[R72] 等待端口就绪
来源：http://ebl.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zyv.gogol.net.cn

[R73] 分割大日志
来源：http://flz.hywenlv.cn

split -l 1000 big.log part_
来源：http://chb.dianchejie.cn

[R74] 批量重命名
来源：http://doq.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wrg.hysaishi.cn

[R75] 导出环境变量
来源：http://hap.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ylg.jqgfzy.top

[R76] 使用临时文件
来源：http://yhd.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rdq.smart0.xyz

[R77] 读取用户输入
来源：http://wxm.hnxiangtu.top

read -rp "请输入: " ans
来源：http://llm.hywenlv.cn

[R78] 交互式菜单
来源：http://qyg.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lfb.ppjwa.cn

[R79] 解析命令行选项
来源：http://ioz.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ozp.tanke756.top

[R80] 查看脚本执行耗时
来源：http://ezd.xylfe.cn

time ./run.sh
来源：http://bty.daria6918.cn

================================================================================
来源：http://zcp.vehdjk.com

S. C / C++ 专题
来源：http://wps.birdmap.top

================================================================================
来源：http://lgk.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://nna.gogol.net.cn

#include <stdio.h>
来源：http://jzb.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://msi.yvedp.cn

[S02] C：变量与格式化输出
来源：http://iiy.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://lnw.zhongyouzk.top

[S03] C：读入整数
来源：http://klk.yuanzhike.top

int x; scanf("%d", &x);
来源：http://fvm.zhoulong.xyz

[S04] C：字符串复制
来源：http://kny.nanxinkj.top

char dst[32]; strcpy(dst, "hi");
来源：http://ksv.meibo888.top

[S05] C：字符串长度
来源：http://svd.sxryk.cn

strlen(s)
来源：http://zoi.cdnleiting.top

[S06] C：字符串比较
来源：http://cmf.quarkkingdee.top

strcmp(a, b) == 0
来源：http://jra.fktsv.cn

[S07] C：数组遍历求和
来源：http://ikq.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jwf.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://xcv.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zpb.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://hxv.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afb.nanxuanxn.top

[S10] C：指针与解引用
来源：http://ast.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://wfx.jinqigfzy.top

[S11] C：逐行读文件
来源：http://ecq.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://fdc.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yoy.yuxming.cn

fclose(f);
来源：http://rvh.zycfv.cn

[S12] C：写文件
来源：http://xet.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zri.aibaodan.cn

[S13] C：宏定义
来源：http://juf.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kiu.yfazqb.com

[S14] C：枚举
来源：http://gzl.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://duy.mhx1999.top

[S15] C：类型转换
来源：http://wcu.chenlongwang.top

(double) a / b
来源：http://ugm.shangyingyoupin.top

[S16] C：位操作置位
来源：http://zns.cdnleiting.top

x |= (1 << 3);
来源：http://eon.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://rpw.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bkn.quarkkingdee.top

[S18] C：命令行参数
来源：http://qhg.yj20258888.top

int main(int argc, char **argv)
来源：http://vqs.haohaochexian.top

[S19] C：快速排序
来源：http://yzp.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://jif.hysaishi.cn

[S20] C：二分查找
来源：http://mwz.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bno.aibaodan.cn

[S21] C：字符类别判断
来源：http://idj.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lne.hammf.cn

[S22] C：字符串转数字
来源：http://llg.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://rmd.jianghu66.top

[S23] C：随机数
来源：http://fuj.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yye.hesvh.cn

[S24] C：获取本地时间
来源：http://mhz.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://odt.dianchejie.cn

[S25] C：内存拷贝
来源：http://jbt.jyoumei.cn

memcpy(dst, src, n);
来源：http://pag.cqqwz.cn

[S26] C：内存清零
来源：http://zpm.yuxming.cn

memset(a, 0, sizeof a);
来源：http://hip.zdqjudy.top

[S27] C：定义常量
来源：http://zpj.tarul.cn

const double PI = 3.14159;
来源：http://lvx.kuanghao11.cn

[S28] C：静态变量
来源：http://hvl.zycfv.cn

static int counter = 0;
来源：http://scz.cdnleiting.top

[S29] C：变参函数
来源：http://dgo.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mgs.gaohongyu789.top

[S30] C：头文件保护
来源：http://cky.gotoacloud.top

#ifndef X_H
来源：http://lbu.cdnleiting.top

#define X_H
来源：http://szb.ydzc1.top

#endif
来源：http://jsf.sysykeji.top

[S31] C++：Hello World
来源：http://nju.shzxlz.cn

#include <iostream>
来源：http://lsd.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://rtq.jinghuilouyu.cn

[S32] C++：字符串
来源：http://kbn.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://yln.yangfankeji.com

[S33] C++：vector 增删
来源：http://ecx.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://otf.sweek.top

[S34] C++：遍历 vector
来源：http://elh.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://qxs.52xcode.cn

[S35] C++：map
来源：http://nqy.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lyz.bjfxy.top

[S36] C++：unordered_map
来源：http://cdr.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wjk.hammf.cn

[S37] C++：set
来源：http://pbq.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fpt.yfazqb.com

[S38] C++：排序
来源：http://lvd.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://snj.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://tur.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iav.zhixingplan.top

[S40] C++：查找元素
来源：http://plw.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mmf.fehbvm.com

[S41] C++：类与构造函数
来源：http://btx.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wsa.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://eqj.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://egl.yuxming.cn

[S43] C++：智能指针
来源：http://boc.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://yho.zdqjudy.top

[S44] C++：引用传参
来源：http://eyn.daxiang520.top

void inc(int &x) { ++x; }
来源：http://ckn.cqqwz.cn

[S45] C++：lambda
来源：http://hjq.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://qyk.redwolf501.top

[S46] C++：函数模板
来源：http://qeu.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oda.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://pbj.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vyf.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://gxh.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ptr.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://qea.fzhhl.top

[S49] C++：写文件
来源：http://wgg.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bvy.wangdashe.top

[S50] C++：格式化数字
来源：http://ucu.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qar.xylfe.cn

[S51] C++：显式类型转换
来源：http://jbl.bbcook.cn

static_cast<double>(a) / b
来源：http://uhs.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://qxd.sxryk.cn

int size() const noexcept { return n_; }
来源：http://vkj.yuanzhike.top

[S53] C++：移动语义
来源：http://dqh.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://uhc.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://jbv.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tdg.daxiang520.top

[S55] C++：结构化绑定
来源：http://iqs.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jhv.chenlongwang.top

[S56] C++：optional
来源：http://ojg.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rqs.dianchejie.cn

[S57] C++：编译期常量
来源：http://kvu.daria6918.cn

constexpr int N = 10;
来源：http://ydf.nanxuanxn.top

[S58] C++：命名空间
来源：http://ucn.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://pzv.feifeiyinyue.top

[S59] C++：静态断言
来源：http://jgr.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://psr.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ydn.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wis.zhijiandao.cn

================================================================================
来源：http://sya.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zlm.smart0.xyz

================================================================================
来源：http://ozx.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://zco.zdqjudy.top

println("Hello")
来源：http://mxf.ydzc1.top

[T02] Kotlin：变量
来源：http://pzj.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://npd.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://ffb.shanyushiyangtech.top

"值: $b"
来源：http://ggn.c1oappe.top

[T04] Kotlin：空安全
来源：http://pel.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://cqn.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://nbw.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mwe.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://chg.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ezp.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://qdu.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://wfy.yuxming.cn

[T08] Kotlin：数据类
来源：http://bjp.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://osd.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://odw.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://een.tian-w.cn

[T10] Kotlin：默认参数
来源：http://nfb.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ufm.nwbrower.top

[T11] Kotlin：协程
来源：http://kzm.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ikl.fehbvm.com

[T12] Kotlin：解构声明
来源：http://npm.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://hmn.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://jur.cheryme.top

val m = mapOf("a" to 1)
来源：http://qiz.haohaochexian.top

[T14] Kotlin：循环
来源：http://eur.hysaishi.cn

for (i in 1..10) println(i)
来源：http://efo.zycfv.cn

[T15] Kotlin：接口
来源：http://muu.sysykeji.top

interface Shape { fun area(): Double }
来源：http://sut.yueranfly.top

[T16] Swift：Hello World
来源：http://gyk.nanxinkj.top

print("Hello")
来源：http://ijj.birdmap.top

[T17] Swift：变量与常量
来源：http://cbi.pycfn.com

var a = 1;  let b = 2
来源：http://duv.jyoumei.cn

[T18] Swift：字符串插值
来源：http://olw.52xcode.cn

"值: \(b)"
来源：http://hmf.jqgfzy.top

[T19] Swift：可选绑定
来源：http://cxu.ppjwa.cn

if let n = opt { print(n) }
来源：http://cwu.bbcook.cn

[T20] Swift：数组操作
来源：http://qni.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://rll.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://lcm.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://alr.chenjidiqi.icu

[T22] Swift：字典
来源：http://iea.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ppc.vqdsnc.cn

[T23] Swift：函数
来源：http://tfa.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cuw.0kj1m.cn

[T24] Swift：闭包
来源：http://lkl.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zfh.ehwqpu.com

[T25] Swift：结构体
来源：http://jjn.zhixingplan.top

struct P { var x: Int }
来源：http://nia.ctjpmb.com

[T26] Swift：类与重写
来源：http://cjs.cucudq.cn

class A: Base { override func f() {} }
来源：http://zmr.ydjk.org.cn

[T27] Swift：错误处理
来源：http://cpn.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://bjy.kuanghao11.cn

[T28] Swift：枚举
来源：http://oyq.yongpay.top

enum Color { case red, green }
来源：http://uly.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://udd.vqdsnc.cn

guard let x = opt else { return }
来源：http://pow.xuetiantiany.cn

[T30] Swift：协议
来源：http://kyy.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://tpi.xylfe.cn

[T31] Lua：Hello World
来源：http://bzg.jqgfzy.top

print("Hello")
来源：http://axo.yj20258888.top

[T32] Lua：局部变量
来源：http://jrj.jlsjyb.cn

local a = 1
来源：http://dal.yvedp.cn

[T33] Lua：表（数组）
来源：http://hvp.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iex.sjlbkw.cn

[T34] Lua：遍历表
来源：http://wvw.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zxi.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://fxp.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://hrn.hnqzz.top

[T36] Lua：函数
来源：http://gnw.jqgufenzy.top

function add(a, b) return a + b end
来源：http://wmq.bjfxy.top

[T37] Lua：字符串拼接
来源：http://ncm.fehbvm.com

"a" .. "b"
来源：http://lbx.sufxvd.cn

[T38] Lua：条件
来源：http://avq.gotoacloud.top

if x > 0 then print("正") end
来源：http://cxy.tian-w.cn

[T39] Lua：模式匹配
来源：http://uit.hfpthk.cn

string.find(s, "%d+")
来源：http://hnc.yuanzhike.top

[T40] Lua：元表
来源：http://abr.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://vfi.svipenyu.cn

[T41] Perl：Hello World
来源：http://utk.nwbrower.top

print "Hello\n";
来源：http://vgr.gotoacloud.top

[T42] Perl：变量类型
来源：http://fqj.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://chi.snrcjt.cn

[T43] Perl：字符串插值
来源：http://aud.jqgufenzy.top

"值: $a"
来源：http://gui.yfazqb.com

[T44] Perl：条件
来源：http://dva.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://byq.cucudq.cn

[T45] Perl：数组遍历
来源：http://jqg.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://rhe.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://vmd.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hgj.jinqigufen.top

[T47] Perl：正则捕获
来源：http://fum.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wpl.yvedp.cn

[T48] Perl：正则替换
来源：http://njb.zhixingplan.top

$s =~ s/old/new/g;
来源：http://ktr.bjfxy.top

[T49] Perl：函数
来源：http://ypq.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nhm.zycfv.cn

[T50] Perl：逐行读文件
来源：http://epn.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uwu.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://qij.shzxlz.cn

[T51] Scala：Hello World
来源：http://mbq.jqgfzy.top

println("Hello")
来源：http://gro.fehbvm.com

[T52] Scala：变量
来源：http://nnp.zhoulong.xyz

val a = 1;  var b = 2
来源：http://lho.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://sut.yvedp.cn

s"值: $b"
来源：http://ihl.hnqzz.top

[T54] Scala：集合映射
来源：http://vba.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://dqk.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://iwz.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://bsu.vehdjk.com

[T56] Scala：样例类
来源：http://lfr.zdqjudy.top

case class User(name: String, age: Int)
来源：http://vck.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://hud.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jit.ybcxt.top

[T58] Scala：函数定义
来源：http://uyc.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://djd.pengpengdd.cyou

[T59] Scala：循环
来源：http://oao.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://zkz.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://maj.daria6918.cn


<!-- 参考信息 -->