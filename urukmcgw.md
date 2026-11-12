代发 wailian999

free -h;  ps aux | grep nginx
来源：http://exn.c1oappe.top

[R64] 结束进程
来源：http://xoy.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://oqa.vqdsnc.cn

[R65] 查看端口占用
来源：http://ufb.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hsu.guowangkeji.top

[R66] 定时任务
来源：http://qgz.wangdashe.top

crontab -e;  crontab -l
来源：http://ddd.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://ych.yuanzhike.top

openssl rand -hex 16
来源：http://lvk.yj202588.top

[R68] 计算文件校验值
来源：http://wwc.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://rfw.zhijiandao.cn

[R69] 生成随机密码
来源：http://yxm.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://tau.zhengqikj.top

[R70] 时间戳与互转
来源：http://lvn.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://ejj.ivvv.top

[R71] 日期格式化
来源：http://dgl.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hhg.jinqigfzy.top

[R72] 等待端口就绪
来源：http://alb.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sye.birdmap.top

[R73] 分割大日志
来源：http://jeg.ivvv.top

split -l 1000 big.log part_
来源：http://nrk.birdmap.top

[R74] 批量重命名
来源：http://nhs.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ish.zhoulong.xyz

[R75] 导出环境变量
来源：http://lqm.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://cvl.cqqwz.cn

[R76] 使用临时文件
来源：http://vbb.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pzi.zycfv.cn

[R77] 读取用户输入
来源：http://wlt.shzxlz.cn

read -rp "请输入: " ans
来源：http://rqn.zycfv.cn

[R78] 交互式菜单
来源：http://fil.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rfg.jqgfzy.top

[R79] 解析命令行选项
来源：http://hiu.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xxy.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://mvp.nanxuanxn.top

time ./run.sh
来源：http://fwt.guannengcc.top

================================================================================
来源：http://wye.zdbjq.cn

S. C / C++ 专题
来源：http://yrv.cheryme.top

================================================================================
来源：http://uyq.nanxinkj.top

[S01] C：Hello World
来源：http://yir.vqdsnc.cn

#include <stdio.h>
来源：http://yau.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kzf.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://vcq.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://lgf.jiagoushi.top

[S03] C：读入整数
来源：http://gei.daria6918.cn

int x; scanf("%d", &x);
来源：http://xdd.ybcxt.top

[S04] C：字符串复制
来源：http://ukr.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xmy.cucudq.cn

[S05] C：字符串长度
来源：http://gjl.jinqigfzy.top

strlen(s)
来源：http://yyp.andypj.xyz

[S06] C：字符串比较
来源：http://vgt.haohaochexian.top

strcmp(a, b) == 0
来源：http://fcc.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://cbi.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iys.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://mxg.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cot.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://ssi.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gvj.vqdsnc.cn

[S10] C：指针与解引用
来源：http://bvy.uphjek.com

int *p = &a;  *p = 5;
来源：http://riv.gotoacloud.top

[S11] C：逐行读文件
来源：http://hba.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://env.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xtr.zhiwuduotai.top

fclose(f);
来源：http://frk.yonumen.top

[S12] C：写文件
来源：http://kbw.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qxl.ppjwa.cn

[S13] C：宏定义
来源：http://mdi.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://spv.shanyushiyangtech.top

[S14] C：枚举
来源：http://kxj.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://wop.c1oappe.top

[S15] C：类型转换
来源：http://bkr.jqgfzy.top

(double) a / b
来源：http://tux.aibaodan.cn

[S16] C：位操作置位
来源：http://sur.yueranfly.top

x |= (1 << 3);
来源：http://utb.tian-w.cn

[S17] C：安全拼接字符串
来源：http://ibe.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tgp.bjfxy.top

[S18] C：命令行参数
来源：http://fpw.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://qqc.0kj1m.cn

[S19] C：快速排序
来源：http://exd.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ryd.52xcode.cn

[S20] C：二分查找
来源：http://hfh.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bti.iojbl.cn

[S21] C：字符类别判断
来源：http://fhk.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yqv.jqgufenzy.top

[S22] C：字符串转数字
来源：http://daa.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://gex.jlsjyb.cn

[S23] C：随机数
来源：http://fbj.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yrx.c1oappe.top

[S24] C：获取本地时间
来源：http://ocr.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ayv.hnqzz.top

[S25] C：内存拷贝
来源：http://kze.yuxming.cn

memcpy(dst, src, n);
来源：http://jfq.0kj1m.cn

[S26] C：内存清零
来源：http://bwt.nwbrower.top

memset(a, 0, sizeof a);
来源：http://yqm.yvedp.cn

[S27] C：定义常量
来源：http://unq.cqqwz.cn

const double PI = 3.14159;
来源：http://yof.gaohongyu789.top

[S28] C：静态变量
来源：http://lkm.svipenyu.cn

static int counter = 0;
来源：http://mdf.shanyushiyangtech.top

[S29] C：变参函数
来源：http://pgm.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://grn.yfazqb.com

[S30] C：头文件保护
来源：http://pon.ywan-chungtsiang.top

#ifndef X_H
来源：http://squ.shangyingyoupin.top

#define X_H
来源：http://fsw.daxiang520.top

#endif
来源：http://woa.pycfn.com

[S31] C++：Hello World
来源：http://zlk.yangfankeji.com

#include <iostream>
来源：http://fvc.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://ilv.cqqwz.cn

[S32] C++：字符串
来源：http://heg.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://bww.guowangkeji.top

[S33] C++：vector 增删
来源：http://dqf.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rqn.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://ass.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://jry.52xcode.cn

[S35] C++：map
来源：http://irr.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://foy.cheryme.top

[S36] C++：unordered_map
来源：http://usf.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nua.jiagoushi.top

[S37] C++：set
来源：http://wrn.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kiz.zhoulong.xyz

[S38] C++：排序
来源：http://qxx.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://pxd.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://dkc.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vze.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://avq.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ebg.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://ypi.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://giv.ybcxt.top

[S42] C++：继承与虚函数
来源：http://tua.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://enp.tanke756.top

[S43] C++：智能指针
来源：http://vjs.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://gxm.ydzc1.top

[S44] C++：引用传参
来源：http://wmt.redwolf501.top

void inc(int &x) { ++x; }
来源：http://ytb.havefunace.top

[S45] C++：lambda
来源：http://wix.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wkq.tianlin.xyz

[S46] C++：函数模板
来源：http://zlj.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vip.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://ohr.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hmp.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://mey.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://hud.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://jfj.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://ado.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jeo.jlsjyb.cn

[S50] C++：格式化数字
来源：http://lty.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cft.bbcook.cn

[S51] C++：显式类型转换
来源：http://zpr.yj202588.top

static_cast<double>(a) / b
来源：http://khc.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://nyu.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://dlx.jlsjyb.cn

[S53] C++：移动语义
来源：http://sny.yonumen.top

std::vector<int> w = std::move(v);
来源：http://vnf.yuanzhike.top

[S54] C++：异常处理
来源：http://yka.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yhj.daria6918.cn

[S55] C++：结构化绑定
来源：http://bar.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qdu.quarkkingdee.top

[S56] C++：optional
来源：http://ipu.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jjo.hcnkem.com

[S57] C++：编译期常量
来源：http://adx.ctjpmb.com

constexpr int N = 10;
来源：http://omy.havefunace.top

[S58] C++：命名空间
来源：http://jjz.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://vsy.svipenyu.cn

[S59] C++：静态断言
来源：http://lqk.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yst.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://jie.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wuk.fanxiaobao.xyz

================================================================================
来源：http://bvh.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cyv.9152youxi.cn

================================================================================
来源：http://vqr.xylfe.cn

[T01] Kotlin：Hello World
来源：http://qbb.gogol.net.cn

println("Hello")
来源：http://xrb.9152youxi.cn

[T02] Kotlin：变量
来源：http://lge.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://krn.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://hkf.shzxlz.cn

"值: $b"
来源：http://tzl.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://jkk.sysykeji.top

val n: String? = null;  n?.length
来源：http://bql.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://bxo.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ysw.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://dhs.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ruy.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://jpy.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://viy.meibo888.top

[T08] Kotlin：数据类
来源：http://way.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://gai.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://jjd.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://ewm.ybcxt.top

[T10] Kotlin：默认参数
来源：http://yev.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mwt.yfazqb.com

[T11] Kotlin：协程
来源：http://fvd.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dti.fanxiaobao.xyz

[T12] Kotlin：解构声明
来源：http://trc.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://mcj.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://fzm.fktsv.cn

val m = mapOf("a" to 1)
来源：http://vsh.hcnkem.com

[T14] Kotlin：循环
来源：http://hce.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://rkf.shzxlz.cn

[T15] Kotlin：接口
来源：http://bmo.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://zbx.dianchejie.cn

[T16] Swift：Hello World
来源：http://vdn.zhiwuduotai.top

print("Hello")
来源：http://mse.yj202588.top

[T17] Swift：变量与常量
来源：http://lng.kuanghao11.cn

var a = 1;  let b = 2
来源：http://rny.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://sqv.yj20258888.top

"值: \(b)"
来源：http://eic.andypj.xyz

[T19] Swift：可选绑定
来源：http://kic.jyoumei.cn

if let n = opt { print(n) }
来源：http://bmz.uphjek.com

[T20] Swift：数组操作
来源：http://mxp.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cgc.xuetiantiany.cn

[T21] Swift：遍历
来源：http://pds.wangdashe.top

for x in a { print(x) }
来源：http://hmm.shzxlz.cn

[T22] Swift：字典
来源：http://mfb.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://ugm.yj202588.top

[T23] Swift：函数
来源：http://lku.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cly.wangdashe.top

[T24] Swift：闭包
来源：http://yvz.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://twh.dashuyun.cn

[T25] Swift：结构体
来源：http://ibl.svipenyu.cn

struct P { var x: Int }
来源：http://ylt.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://ezo.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://enj.gaohongyu789.top

[T27] Swift：错误处理
来源：http://cbi.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://puj.gaohongyu789.top

[T28] Swift：枚举
来源：http://fbh.svipenyu.cn

enum Color { case red, green }
来源：http://mxi.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://pfy.hesvh.cn

guard let x = opt else { return }
来源：http://xul.316326.xyz

[T30] Swift：协议
来源：http://lpn.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://ato.tian-w.cn

[T31] Lua：Hello World
来源：http://wlu.dashuyun.cn

print("Hello")
来源：http://adf.redwolf501.top

[T32] Lua：局部变量
来源：http://quy.vqdsnc.cn

local a = 1
来源：http://wui.cashguo.top

[T33] Lua：表（数组）
来源：http://ndv.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nzo.guowangkeji.top

[T34] Lua：遍历表
来源：http://cpt.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nwx.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://moj.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://gpx.tarul.cn

[T36] Lua：函数
来源：http://eda.yj20258.top

function add(a, b) return a + b end
来源：http://chl.yongpay.top

[T37] Lua：字符串拼接
来源：http://wkq.dashuyun.cn

"a" .. "b"
来源：http://vct.0kj1m.cn

[T38] Lua：条件
来源：http://hbk.bbcook.cn

if x > 0 then print("正") end
来源：http://ahh.meibo888.top

[T39] Lua：模式匹配
来源：http://sfd.yj202588.top

string.find(s, "%d+")
来源：http://wck.uphjek.com

[T40] Lua：元表
来源：http://cvz.guannengcc.top

setmetatable({}, { __index = base })
来源：http://epl.gogol.net.cn

[T41] Perl：Hello World
来源：http://usk.zhaomingkeji.xyz

print "Hello\n";
来源：http://mkr.jianghu66.top

[T42] Perl：变量类型
来源：http://ymi.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzk.nanxinkj.top

[T43] Perl：字符串插值
来源：http://qcw.havefunace.top

"值: $a"
来源：http://ini.cashguo.top

[T44] Perl：条件
来源：http://efb.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://dxv.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://sea.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://kac.svipenyu.cn

[T46] Perl：哈希操作
来源：http://yju.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vul.jianghu66.top

[T47] Perl：正则捕获
来源：http://qmu.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uno.sufxvd.cn

[T48] Perl：正则替换
来源：http://jze.gzhubu.top

$s =~ s/old/new/g;
来源：http://vxj.sjlbkw.cn

[T49] Perl：函数
来源：http://hnh.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uuj.fehbvm.com

[T50] Perl：逐行读文件
来源：http://zbx.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://kuy.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://lon.shzxlz.cn

[T51] Scala：Hello World
来源：http://tji.ywan-chungtsiang.top

println("Hello")
来源：http://xof.ivvv.top

[T52] Scala：变量
来源：http://ssd.yuxming.cn

val a = 1;  var b = 2
来源：http://jfc.316326.xyz

[T53] Scala：字符串插值
来源：http://sfz.yfazqb.com

s"值: $b"
来源：http://vln.jinqigfzy.top

[T54] Scala：集合映射
来源：http://xay.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://ftq.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://bow.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vnf.guowangkeji.top

[T56] Scala：样例类
来源：http://fri.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://hra.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://clg.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqc.yangfankeji.com

[T58] Scala：函数定义
来源：http://zid.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://slh.mhx1999.top

[T59] Scala：循环
来源：http://icn.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://vqq.52xcode.cn

[T60] Scala：折叠
来源：http://poc.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sga.dianchejie.cn

================================================================================
来源：http://eqm.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nms.quarkkingdee.top

================================================================================
来源：http://she.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://xum.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://nlc.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://oam.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xca.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://cmh.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ehv.daria6918.cn

[U04] Py：变量调试打印
来源：http://ejz.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gbq.hcnkem.com


<!-- 参考信息 -->