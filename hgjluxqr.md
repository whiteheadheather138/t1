代发 wailian999

ssh user@host 'uptime'
来源：http://nbo.jlsjyb.cn

[R58] 下载文件
来源：http://xpk.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pjj.hnxiangtu.top

[R59] 发 POST JSON
来源：http://xuj.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zau.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://vhe.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oez.hfpthk.cn

[R61] 磁盘占用
来源：http://zxc.hysaishi.cn

df -h;  du -sh *
来源：http://dvs.jqgfzy.top

[R62] 找最占空间的文件
来源：http://cmx.havefunace.top

du -ah . | sort -rh | head -10
来源：http://gxa.sufxvd.cn

[R63] 内存与进程
来源：http://esg.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://qum.fzhhl.top

[R64] 结束进程
来源：http://hph.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://jrk.yongpay.top

[R65] 查看端口占用
来源：http://ojp.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://twi.tanke756.top

[R66] 定时任务
来源：http://ddc.cashguo.top

crontab -e;  crontab -l
来源：http://eml.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://plb.sysykeji.top

openssl rand -hex 16
来源：http://xwz.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://lbs.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://wji.tianlin.xyz

[R69] 生成随机密码
来源：http://bcd.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://uhi.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://tbr.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://yoy.iojbl.cn

[R71] 日期格式化
来源：http://yqt.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nxs.xziqi.cn

[R72] 等待端口就绪
来源：http://hgu.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ooh.zhengqikj.top

[R73] 分割大日志
来源：http://hsl.zhengqikj.top

split -l 1000 big.log part_
来源：http://skt.sjlbkw.cn

[R74] 批量重命名
来源：http://tun.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://avo.fzhhl.top

[R75] 导出环境变量
来源：http://qyp.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://xph.gogol.net.cn

[R76] 使用临时文件
来源：http://ltw.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dqa.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://dri.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://xpr.hfpthk.cn

[R78] 交互式菜单
来源：http://kif.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uqc.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://mbh.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sys.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://udr.iojbl.cn

time ./run.sh
来源：http://aji.nanxuanxn.top

================================================================================
来源：http://lgg.tian-w.cn

S. C / C++ 专题
来源：http://mey.jinyuanbaomall.cn

================================================================================
来源：http://krz.ydzc1.top

[S01] C：Hello World
来源：http://fxa.mhx1999.top

#include <stdio.h>
来源：http://afm.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://udo.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://qpb.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://oyv.hfpthk.cn

[S03] C：读入整数
来源：http://rie.bbcook.cn

int x; scanf("%d", &x);
来源：http://nwl.svipenyu.cn

[S04] C：字符串复制
来源：http://abx.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://orf.jinqigufen.top

[S05] C：字符串长度
来源：http://qki.guowangkeji.top

strlen(s)
来源：http://hby.aizwys.cn

[S06] C：字符串比较
来源：http://slt.sxryk.cn

strcmp(a, b) == 0
来源：http://hmx.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://qwz.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kim.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://ots.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gzt.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://lmy.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://grr.quarkkingdee.top

[S10] C：指针与解引用
来源：http://wgf.cashguo.top

int *p = &a;  *p = 5;
来源：http://rsw.jqgfzy.top

[S11] C：逐行读文件
来源：http://gsw.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://swy.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vur.uphjek.com

fclose(f);
来源：http://mnj.shanyushiyangtech.top

[S12] C：写文件
来源：http://wka.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mqh.sjlbkw.cn

[S13] C：宏定义
来源：http://jse.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qda.cucudq.cn

[S14] C：枚举
来源：http://iir.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://bmc.gotoacloud.top

[S15] C：类型转换
来源：http://oyw.jinqigufen.top

(double) a / b
来源：http://hxh.ppjwa.cn

[S16] C：位操作置位
来源：http://doq.xinyue.icu

x |= (1 << 3);
来源：http://wzx.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://cxc.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://itt.bbcook.cn

[S18] C：命令行参数
来源：http://ywk.yangfankeji.com

int main(int argc, char **argv)
来源：http://uqk.andypj.xyz

[S19] C：快速排序
来源：http://fxb.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://afu.jinghuilouyu.cn

[S20] C：二分查找
来源：http://dqn.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bya.sweek.top

[S21] C：字符类别判断
来源：http://qqk.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://joh.sxryk.cn

[S22] C：字符串转数字
来源：http://xdp.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aut.nanxuanxn.top

[S23] C：随机数
来源：http://ika.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qfi.havefunace.top

[S24] C：获取本地时间
来源：http://qmq.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sva.tarul.cn

[S25] C：内存拷贝
来源：http://abj.yj202588.top

memcpy(dst, src, n);
来源：http://itb.feifeiyinyue.top

[S26] C：内存清零
来源：http://cyo.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://fzi.xuanzx.com

[S27] C：定义常量
来源：http://ytb.yuxming.cn

const double PI = 3.14159;
来源：http://gnn.tanke756.top

[S28] C：静态变量
来源：http://uqo.tanke756.top

static int counter = 0;
来源：http://nzu.ybcxt.top

[S29] C：变参函数
来源：http://pyy.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bld.svipenyu.cn

[S30] C：头文件保护
来源：http://qhp.tian-w.cn

#ifndef X_H
来源：http://vau.yongpay.top

#define X_H
来源：http://dwv.hfpthk.cn

#endif
来源：http://eum.yj202588.top

[S31] C++：Hello World
来源：http://mkk.sjlbkw.cn

#include <iostream>
来源：http://ulf.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://mvt.redwolf501.top

[S32] C++：字符串
来源：http://hbp.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://crb.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://bwl.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ihl.meibo888.top

[S34] C++：遍历 vector
来源：http://wod.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://iib.sysykeji.top

[S35] C++：map
来源：http://ywq.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqz.cucudq.cn

[S36] C++：unordered_map
来源：http://fgs.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ocj.9152youxi.cn

[S37] C++：set
来源：http://ces.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tmx.zhijiandao.cn

[S38] C++：排序
来源：http://xxl.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://aie.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://hkf.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kjm.zhengqikj.top

[S40] C++：查找元素
来源：http://ayd.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ecw.redwolf501.top

[S41] C++：类与构造函数
来源：http://mvr.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jqu.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://qiq.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://nvp.chenlongwang.top

[S43] C++：智能指针
来源：http://bkp.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://zwi.chenjidiqi.icu

[S44] C++：引用传参
来源：http://blp.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://rcc.sxryk.cn

[S45] C++：lambda
来源：http://tdy.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://wob.kuanghao11.cn

[S46] C++：函数模板
来源：http://uab.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pvj.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://izk.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qkt.sysykeji.top

[S48] C++：逐行读文件
来源：http://ggc.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://bzs.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://zqw.fengsongda.top

[S49] C++：写文件
来源：http://yth.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rsp.tanke756.top

[S50] C++：格式化数字
来源：http://xyw.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://olc.chenzaomai.com

[S51] C++：显式类型转换
来源：http://oqb.epnwcf.com

static_cast<double>(a) / b
来源：http://vsw.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://abe.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://stm.sufxvd.cn

[S53] C++：移动语义
来源：http://lly.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://ggw.jlsjyb.cn

[S54] C++：异常处理
来源：http://gnt.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ufx.havefunace.top

[S55] C++：结构化绑定
来源：http://fog.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qdn.sjlbkw.cn

[S56] C++：optional
来源：http://jqj.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mtx.gogol.net.cn

[S57] C++：编译期常量
来源：http://yvs.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://ugk.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://bnw.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://txi.zdbjq.cn

[S59] C++：静态断言
来源：http://yjv.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uew.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://tag.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ame.gogol.net.cn

================================================================================
来源：http://kai.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysa.hywenlv.cn

================================================================================
来源：http://cjf.sxryk.cn

[T01] Kotlin：Hello World
来源：http://uvd.hongshengwenyu.top

println("Hello")
来源：http://suc.9152youxi.cn

[T02] Kotlin：变量
来源：http://ieu.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ggj.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://aqp.epnwcf.com

"值: $b"
来源：http://pcx.shuidangran.top

[T04] Kotlin：空安全
来源：http://dxw.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://gym.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://ygv.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zbc.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://zry.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://obh.pycfn.com

[T07] Kotlin：集合过滤
来源：http://yqp.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ljn.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://ciw.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://anu.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://wrq.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://sze.iojbl.cn

[T10] Kotlin：默认参数
来源：http://zax.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zjj.jinqigufen.top

[T11] Kotlin：协程
来源：http://qoe.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://omc.cheryme.top

[T12] Kotlin：解构声明
来源：http://ujx.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://kxq.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://qlk.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://jua.shzxlz.cn

[T14] Kotlin：循环
来源：http://qha.smart0.xyz

for (i in 1..10) println(i)
来源：http://ouw.jlsjyb.cn

[T15] Kotlin：接口
来源：http://mri.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://rki.ehwqpu.com

[T16] Swift：Hello World
来源：http://vsn.chenlongwang.top

print("Hello")
来源：http://vef.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://fsq.pycfn.com

var a = 1;  let b = 2
来源：http://vcs.andypj.xyz

[T18] Swift：字符串插值
来源：http://jhe.xinyue.icu

"值: \(b)"
来源：http://gau.jianghu66.top

[T19] Swift：可选绑定
来源：http://ygq.yanxiufei.cn

if let n = opt { print(n) }
来源：http://mid.svipenyu.cn

[T20] Swift：数组操作
来源：http://ggl.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://ibl.fehbvm.com

[T21] Swift：遍历
来源：http://ype.jqgufenzy.top

for x in a { print(x) }
来源：http://gct.jianghu66.top

[T22] Swift：字典
来源：http://dyv.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ndx.sufxvd.cn

[T23] Swift：函数
来源：http://cqq.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wsn.gzhubu.top

[T24] Swift：闭包
来源：http://ezu.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxj.yueranfly.top

[T25] Swift：结构体
来源：http://wiy.jinqigufen.top

struct P { var x: Int }
来源：http://nku.hnqzz.top

[T26] Swift：类与重写
来源：http://zlp.havefunace.top

class A: Base { override func f() {} }
来源：http://wki.snrcjt.cn

[T27] Swift：错误处理
来源：http://hsk.cashguo.top

do { try f() } catch { print(error) }
来源：http://ysa.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://ief.smart0.xyz

enum Color { case red, green }
来源：http://gej.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://hon.ydjk.org.cn

guard let x = opt else { return }
来源：http://xqe.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://xmh.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://vif.birdmap.top

[T31] Lua：Hello World
来源：http://bxd.bjfxy.top

print("Hello")
来源：http://byg.xuanzx.com

[T32] Lua：局部变量
来源：http://tez.kuanghao11.cn

local a = 1
来源：http://gsa.vehdjk.com

[T33] Lua：表（数组）
来源：http://glm.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://okh.shuidangran.top

[T34] Lua：遍历表
来源：http://rkq.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://raz.meibo888.top

[T35] Lua：字典表
来源：http://ydw.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://piu.jiagoushi.top

[T36] Lua：函数
来源：http://iix.ybcxt.top

function add(a, b) return a + b end
来源：http://oif.tarul.cn

[T37] Lua：字符串拼接
来源：http://clw.yuxming.cn

"a" .. "b"
来源：http://vdv.pengpengdd.cyou

[T38] Lua：条件
来源：http://cle.bbcook.cn

if x > 0 then print("正") end
来源：http://qtd.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://iml.nanxinkj.top

string.find(s, "%d+")
来源：http://dyb.jinqigfzy.top

[T40] Lua：元表
来源：http://bio.xuanzx.com

setmetatable({}, { __index = base })
来源：http://bik.hnqzz.top

[T41] Perl：Hello World
来源：http://fbl.jqgufenzy.top

print "Hello\n";
来源：http://saj.hnxiangtu.top

[T42] Perl：变量类型
来源：http://gyq.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mva.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://qpc.redwolf501.top

"值: $a"
来源：http://fho.jqgufenzy.top

[T44] Perl：条件
来源：http://imf.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://dom.cqqwz.cn

[T45] Perl：数组遍历
来源：http://hmt.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://kvk.nanxinkj.top

[T46] Perl：哈希操作
来源：http://dhb.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ixe.jqgfzy.top

[T47] Perl：正则捕获
来源：http://oaj.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://grl.quarkkingdee.top

[T48] Perl：正则替换
来源：http://hbu.ivvv.top

$s =~ s/old/new/g;
来源：http://vae.zycfv.cn

[T49] Perl：函数
来源：http://qhm.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xgu.yuxming.cn

[T50] Perl：逐行读文件
来源：http://ggg.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pup.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://pwg.zhoulong.xyz

[T51] Scala：Hello World
来源：http://vlq.zhijiandao.cn

println("Hello")
来源：http://pbh.0kj1m.cn

[T52] Scala：变量
来源：http://nbt.shzxlz.cn

val a = 1;  var b = 2
来源：http://tpf.nwbrower.top

[T53] Scala：字符串插值
来源：http://sig.meibo888.top

s"值: $b"
来源：http://wqa.yangfankeji.com

[T54] Scala：集合映射
来源：http://atk.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://gfz.fzhhl.top

[T55] Scala：集合过滤
来源：http://ftf.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rab.bbcook.cn

[T56] Scala：样例类
来源：http://wdg.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://evn.316326.xyz

[T57] Scala：模式匹配
来源：http://jib.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vfr.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://mrg.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qac.sysykeji.top

[T59] Scala：循环
来源：http://yhf.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://koq.hfpthk.cn

[T60] Scala：折叠
来源：http://hnx.yj202588.top


<!-- 参考信息 -->