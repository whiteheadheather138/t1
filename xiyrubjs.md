代发 wailian999

df -h;  du -sh *
来源：http://ubp.cashguo.top

[R62] 找最占空间的文件
来源：http://ufc.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://lbi.bjfxy.top

[R63] 内存与进程
来源：http://ays.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://drr.sjlbkw.cn

[R64] 结束进程
来源：http://sly.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://wxk.yanxiufei.cn

[R65] 查看端口占用
来源：http://lxu.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://snx.fengsongda.top

[R66] 定时任务
来源：http://opz.tianlin.xyz

crontab -e;  crontab -l
来源：http://ype.pycfn.com

[R67] 生成随机十六进制串
来源：http://rpf.tianlin.xyz

openssl rand -hex 16
来源：http://gil.hnqzz.top

[R68] 计算文件校验值
来源：http://gfi.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xxl.xuetiantiany.cn

[R69] 生成随机密码
来源：http://wcf.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://lvv.ivvv.top

[R70] 时间戳与互转
来源：http://qxx.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://mjt.fanxiaobao.xyz

[R71] 日期格式化
来源：http://qdl.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bvz.fktsv.cn

[R72] 等待端口就绪
来源：http://jug.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rqg.jlsjyb.cn

[R73] 分割大日志
来源：http://zzc.jiagoushi.top

split -l 1000 big.log part_
来源：http://yih.hnxiangtu.top

[R74] 批量重命名
来源：http://ywf.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uhp.c1oappe.top

[R75] 导出环境变量
来源：http://vjh.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://vyu.gogol.net.cn

[R76] 使用临时文件
来源：http://wzv.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gkp.chenjidiqi.icu

[R77] 读取用户输入
来源：http://hcj.gaohongyu789.top

read -rp "请输入: " ans
来源：http://pbu.cqqwz.cn

[R78] 交互式菜单
来源：http://rtv.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://isp.snrcjt.cn

[R79] 解析命令行选项
来源：http://uue.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://igb.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://dyq.vehdjk.com

time ./run.sh
来源：http://cad.xingfuxueyuan.xyz

================================================================================
来源：http://nlk.yonumen.top

S. C / C++ 专题
来源：http://dye.tanke756.top

================================================================================
来源：http://pci.shangyingyoupin.top

[S01] C：Hello World
来源：http://uzp.bjfxy.top

#include <stdio.h>
来源：http://qek.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bzu.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://nlw.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://ait.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://jin.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://ons.tanke756.top

[S04] C：字符串复制
来源：http://qbq.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://gxg.9152youxi.cn

[S05] C：字符串长度
来源：http://srq.sysykeji.top

strlen(s)
来源：http://njt.yonumen.top

[S06] C：字符串比较
来源：http://otg.316326.xyz

strcmp(a, b) == 0
来源：http://bvz.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://tdm.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ylt.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://xux.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://byk.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://iga.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qsx.nwbrower.top

[S10] C：指针与解引用
来源：http://ter.nwbrower.top

int *p = &a;  *p = 5;
来源：http://xpx.gaohongyu789.top

[S11] C：逐行读文件
来源：http://eom.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://zva.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sfr.yueranfly.top

fclose(f);
来源：http://nmr.yueranfly.top

[S12] C：写文件
来源：http://mfx.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cat.jyoumei.cn

[S13] C：宏定义
来源：http://xyd.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ske.yfazqb.com

[S14] C：枚举
来源：http://aig.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://tbz.yvedp.cn

[S15] C：类型转换
来源：http://dwe.zhijiandao.cn

(double) a / b
来源：http://big.jiagoushi.top

[S16] C：位操作置位
来源：http://smb.hammf.cn

x |= (1 << 3);
来源：http://fby.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://avx.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wcx.xylfe.cn

[S18] C：命令行参数
来源：http://dum.epnwcf.com

int main(int argc, char **argv)
来源：http://gsv.chenzaomai.com

[S19] C：快速排序
来源：http://csf.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://oxw.cashguo.top

[S20] C：二分查找
来源：http://pkm.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tlo.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://tzh.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zup.yuanzhike.top

[S22] C：字符串转数字
来源：http://qct.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eqj.yuxming.cn

[S23] C：随机数
来源：http://wpv.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://grg.vqdsnc.cn

[S24] C：获取本地时间
来源：http://xan.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qus.vqdsnc.cn

[S25] C：内存拷贝
来源：http://uov.smart0.xyz

memcpy(dst, src, n);
来源：http://ekp.guannengcc.top

[S26] C：内存清零
来源：http://vdb.ybcxt.top

memset(a, 0, sizeof a);
来源：http://xvu.haohaochexian.top

[S27] C：定义常量
来源：http://ryi.meibo888.top

const double PI = 3.14159;
来源：http://yfj.snrcjt.cn

[S28] C：静态变量
来源：http://dbk.yonumen.top

static int counter = 0;
来源：http://neb.zhoulong.xyz

[S29] C：变参函数
来源：http://smw.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oxa.aizwys.cn

[S30] C：头文件保护
来源：http://mgc.yj202588.top

#ifndef X_H
来源：http://cdq.zhiwuduotai.top

#define X_H
来源：http://rzn.fktsv.cn

#endif
来源：http://tky.52xcode.cn

[S31] C++：Hello World
来源：http://bxc.nwbrower.top

#include <iostream>
来源：http://utz.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://srg.yonumen.top

[S32] C++：字符串
来源：http://dyp.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://ywd.iojbl.cn

[S33] C++：vector 增删
来源：http://wda.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cru.jiagoushi.top

[S34] C++：遍历 vector
来源：http://qpn.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://phd.snrcjt.cn

[S35] C++：map
来源：http://eny.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tet.gzhubu.top

[S36] C++：unordered_map
来源：http://ekb.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bbq.hcnkem.com

[S37] C++：set
来源：http://abv.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://amp.daxiang520.top

[S38] C++：排序
来源：http://gcj.hammf.cn

std::sort(v.begin(), v.end());
来源：http://xba.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://hbp.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mtk.meibo888.top

[S40] C++：查找元素
来源：http://tka.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wvx.shuidangran.top

[S41] C++：类与构造函数
来源：http://tns.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pby.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://olr.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://hci.zycfv.cn

[S43] C++：智能指针
来源：http://kgl.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://rgs.ehwqpu.com

[S44] C++：引用传参
来源：http://roj.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://sbi.zdbjq.cn

[S45] C++：lambda
来源：http://vwd.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kiz.ctjpmb.com

[S46] C++：函数模板
来源：http://ayi.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eqy.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://vhh.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ubd.fengsongda.top

[S48] C++：逐行读文件
来源：http://lma.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://wcc.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://fhx.shuidangran.top

[S49] C++：写文件
来源：http://llk.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yjt.hnxiangtu.top

[S50] C++：格式化数字
来源：http://zvr.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sra.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://nbu.gaohongyu789.top

static_cast<double>(a) / b
来源：http://vsb.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://bid.havefunace.top

int size() const noexcept { return n_; }
来源：http://xqk.zdbjq.cn

[S53] C++：移动语义
来源：http://vyx.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://kqo.jinqigufen.top

[S54] C++：异常处理
来源：http://glk.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://put.hcnkem.com

[S55] C++：结构化绑定
来源：http://emc.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mca.shangyingyoupin.top

[S56] C++：optional
来源：http://czn.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iss.sufxvd.cn

[S57] C++：编译期常量
来源：http://usx.pycfn.com

constexpr int N = 10;
来源：http://omp.sysykeji.top

[S58] C++：命名空间
来源：http://ygz.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://sio.yangfankeji.com

[S59] C++：静态断言
来源：http://wrx.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://abo.uphjek.com

[S60] C++：遍历并删除元素
来源：http://vpr.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zbe.zdbjq.cn

================================================================================
来源：http://hxa.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pwd.fehbvm.com

================================================================================
来源：http://xaq.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://iem.andypj.xyz

println("Hello")
来源：http://xgc.jianghu66.top

[T02] Kotlin：变量
来源：http://lxx.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://olq.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://gjb.yangfankeji.com

"值: $b"
来源：http://rsp.c1oappe.top

[T04] Kotlin：空安全
来源：http://nfs.xziqi.cn

val n: String? = null;  n?.length
来源：http://dll.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://adu.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zbk.yj202588.top

[T06] Kotlin：集合映射
来源：http://ubu.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ehj.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://dxi.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://omq.yj20258888.top

[T08] Kotlin：数据类
来源：http://wil.yonumen.top

data class User(val name: String, val age: Int)
来源：http://oyx.pycfn.com

[T09] Kotlin：扩展函数
来源：http://fic.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://oug.birdmap.top

[T10] Kotlin：默认参数
来源：http://kxw.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wop.dashuyun.cn

[T11] Kotlin：协程
来源：http://kzl.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ccp.bjfxy.top

[T12] Kotlin：解构声明
来源：http://nbz.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://vyt.havefunace.top

[T13] Kotlin：只读 Map
来源：http://upd.ybcxt.top

val m = mapOf("a" to 1)
来源：http://ris.iojbl.cn

[T14] Kotlin：循环
来源：http://joi.ydzc1.top

for (i in 1..10) println(i)
来源：http://dge.fktsv.cn

[T15] Kotlin：接口
来源：http://meg.yj202588.top

interface Shape { fun area(): Double }
来源：http://jus.cqqwz.cn

[T16] Swift：Hello World
来源：http://yxf.zhijiandao.cn

print("Hello")
来源：http://kbt.dianchejie.cn

[T17] Swift：变量与常量
来源：http://sok.xylfe.cn

var a = 1;  let b = 2
来源：http://ypt.xylfe.cn

[T18] Swift：字符串插值
来源：http://yxx.yangfankeji.com

"值: \(b)"
来源：http://dvv.hywenlv.cn

[T19] Swift：可选绑定
来源：http://ujj.nanxuanxn.top

if let n = opt { print(n) }
来源：http://yix.sweek.top

[T20] Swift：数组操作
来源：http://gwa.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://pxl.shuidangran.top

[T21] Swift：遍历
来源：http://xzt.aibaodan.cn

for x in a { print(x) }
来源：http://egf.jlsjyb.cn

[T22] Swift：字典
来源：http://qkx.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rac.nwbrower.top

[T23] Swift：函数
来源：http://rrt.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iyh.tianlin.xyz

[T24] Swift：闭包
来源：http://rzd.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vdj.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://ixh.ppjwa.cn

struct P { var x: Int }
来源：http://iby.haohaochexian.top

[T26] Swift：类与重写
来源：http://csi.andypj.xyz

class A: Base { override func f() {} }
来源：http://tkr.zhoulong.xyz

[T27] Swift：错误处理
来源：http://bnw.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://ngb.zhiwuduotai.top

[T28] Swift：枚举
来源：http://hsw.ybcxt.top

enum Color { case red, green }
来源：http://rys.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://mvh.redwolf501.top

guard let x = opt else { return }
来源：http://okp.yj202588.top

[T30] Swift：协议
来源：http://ehe.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://fnk.yongpay.top

[T31] Lua：Hello World
来源：http://mmr.jiagoushi.top

print("Hello")
来源：http://nvf.hywenlv.cn

[T32] Lua：局部变量
来源：http://rre.hnqzz.top

local a = 1
来源：http://buv.sxryk.cn

[T33] Lua：表（数组）
来源：http://ywg.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sba.cdnleiting.top

[T34] Lua：遍历表
来源：http://eks.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vgu.zhongyouzk.top

[T35] Lua：字典表
来源：http://coi.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://ily.nanxuanxn.top

[T36] Lua：函数
来源：http://dvt.havefunace.top

function add(a, b) return a + b end
来源：http://qmx.vehdjk.com

[T37] Lua：字符串拼接
来源：http://vpo.zhongyouzk.top

"a" .. "b"
来源：http://ach.redwolf501.top

[T38] Lua：条件
来源：http://cun.hywenlv.cn

if x > 0 then print("正") end
来源：http://btv.meibo888.top

[T39] Lua：模式匹配
来源：http://pvd.vqdsnc.cn

string.find(s, "%d+")
来源：http://kcd.yvedp.cn

[T40] Lua：元表
来源：http://sih.redwolf501.top

setmetatable({}, { __index = base })
来源：http://uyb.dashuyun.cn

[T41] Perl：Hello World
来源：http://hlh.shzxlz.cn

print "Hello\n";
来源：http://jyy.jinqigufen.top

[T42] Perl：变量类型
来源：http://qfh.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wyf.smart0.xyz

[T43] Perl：字符串插值
来源：http://orw.cheryme.top

"值: $a"
来源：http://csd.dashuyun.cn

[T44] Perl：条件
来源：http://emj.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://piz.gogol.net.cn

[T45] Perl：数组遍历
来源：http://kpt.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://ufb.xziqi.cn

[T46] Perl：哈希操作
来源：http://dik.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://syu.ydzc1.top

[T47] Perl：正则捕获
来源：http://vip.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tti.hesvh.cn

[T48] Perl：正则替换
来源：http://poc.birdmap.top

$s =~ s/old/new/g;
来源：http://oti.guowangkeji.top

[T49] Perl：函数
来源：http://vqd.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://szh.52xcode.cn

[T50] Perl：逐行读文件
来源：http://yle.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tqz.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://ewp.svipenyu.cn

[T51] Scala：Hello World
来源：http://mdr.zhoulong.xyz

println("Hello")
来源：http://liv.yj20258.top

[T52] Scala：变量
来源：http://vuc.sufxvd.cn

val a = 1;  var b = 2
来源：http://ukr.yj20258.top

[T53] Scala：字符串插值
来源：http://qlc.yongpay.top

s"值: $b"
来源：http://bex.birdmap.top

[T54] Scala：集合映射
来源：http://qst.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://gry.yj202588.top

[T55] Scala：集合过滤
来源：http://neg.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eds.nanxuanxn.top

[T56] Scala：样例类
来源：http://ncz.svipenyu.cn

case class User(name: String, age: Int)
来源：http://kvz.cashguo.top

[T57] Scala：模式匹配
来源：http://pwv.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eit.yuanzhike.top

[T58] Scala：函数定义
来源：http://txf.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mlr.gogol.net.cn

[T59] Scala：循环
来源：http://yit.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://bri.haohaochexian.top

[T60] Scala：折叠
来源：http://qlf.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xeu.feifeiyinyue.top

================================================================================
来源：http://bod.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://psj.ybcxt.top

================================================================================
来源：http://fbg.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://dpk.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://zbh.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://omw.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sli.zdqjudy.top


<!-- 参考信息 -->