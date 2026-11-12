代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ael.guowangkeji.top

[R56] 远程拷贝
来源：http://jhn.daxiang520.top

scp file user@host:/path/
来源：http://xtv.ivvv.top

[R57] 远程执行命令
来源：http://ylq.yj202588.top

ssh user@host 'uptime'
来源：http://kog.pycfn.com

[R58] 下载文件
来源：http://dbn.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://isj.vehdjk.com

[R59] 发 POST JSON
来源：http://frw.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://inn.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://peo.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ywj.daxiang520.top

[R61] 磁盘占用
来源：http://tvq.jiagoushi.top

df -h;  du -sh *
来源：http://meb.gzhubu.top

[R62] 找最占空间的文件
来源：http://ltw.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://hlj.dashuyun.cn

[R63] 内存与进程
来源：http://uau.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://oni.birdmap.top

[R64] 结束进程
来源：http://eyf.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://bwr.sysykeji.top

[R65] 查看端口占用
来源：http://kik.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://spc.ehwqpu.com

[R66] 定时任务
来源：http://tfw.cqqwz.cn

crontab -e;  crontab -l
来源：http://xvu.bjfxy.top

[R67] 生成随机十六进制串
来源：http://viz.ivvv.top

openssl rand -hex 16
来源：http://gjm.hnxiangtu.top

[R68] 计算文件校验值
来源：http://lwu.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://mnn.hongshengwenyu.top

[R69] 生成随机密码
来源：http://crh.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://wuz.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://ken.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://fhq.havefunace.top

[R71] 日期格式化
来源：http://aiz.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bir.hesvh.cn

[R72] 等待端口就绪
来源：http://fdy.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lvk.yj202588.top

[R73] 分割大日志
来源：http://vme.hammf.cn

split -l 1000 big.log part_
来源：http://wfx.gogol.net.cn

[R74] 批量重命名
来源：http://ygj.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kyd.jiagoushi.top

[R75] 导出环境变量
来源：http://hth.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://kvr.fehbvm.com

[R76] 使用临时文件
来源：http://lsy.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yiz.bjfxy.top

[R77] 读取用户输入
来源：http://diz.316326.xyz

read -rp "请输入: " ans
来源：http://vrw.shzxlz.cn

[R78] 交互式菜单
来源：http://tox.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aoj.gotoacloud.top

[R79] 解析命令行选项
来源：http://xwn.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://khd.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://tyj.kuanghao11.cn

time ./run.sh
来源：http://hei.yonumen.top

================================================================================
来源：http://hms.fehbvm.com

S. C / C++ 专题
来源：http://vvm.cheryme.top

================================================================================
来源：http://pdf.hnqzz.top

[S01] C：Hello World
来源：http://vzc.sweek.top

#include <stdio.h>
来源：http://pgh.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ntg.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://kub.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://xaf.yonumen.top

[S03] C：读入整数
来源：http://tqx.tarul.cn

int x; scanf("%d", &x);
来源：http://tpa.c1oappe.top

[S04] C：字符串复制
来源：http://zoc.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://psa.zycfv.cn

[S05] C：字符串长度
来源：http://rsl.epnwcf.com

strlen(s)
来源：http://flc.hammf.cn

[S06] C：字符串比较
来源：http://yae.fktsv.cn

strcmp(a, b) == 0
来源：http://vfq.tianlin.xyz

[S07] C：数组遍历求和
来源：http://oay.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iel.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://xwl.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oha.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://iuj.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pav.jinqigfzy.top

[S10] C：指针与解引用
来源：http://cof.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://nzr.zycfv.cn

[S11] C：逐行读文件
来源：http://opi.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://hxv.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mjm.shangyingyoupin.top

fclose(f);
来源：http://rey.yonumen.top

[S12] C：写文件
来源：http://jle.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ykx.tarul.cn

[S13] C：宏定义
来源：http://gtx.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ivl.mhx1999.top

[S14] C：枚举
来源：http://coz.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://rtn.pengpengdd.cyou

[S15] C：类型转换
来源：http://dbc.cdnleiting.top

(double) a / b
来源：http://kip.jqgufenzy.top

[S16] C：位操作置位
来源：http://rdt.yanxiufei.cn

x |= (1 << 3);
来源：http://urw.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://msj.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xyd.uphjek.com

[S18] C：命令行参数
来源：http://cyr.hysaishi.cn

int main(int argc, char **argv)
来源：http://nol.52xcode.cn

[S19] C：快速排序
来源：http://bbb.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://phn.hnqzz.top

[S20] C：二分查找
来源：http://xpn.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fda.yanxiufei.cn

[S21] C：字符类别判断
来源：http://jig.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gcu.zhongyouzk.top

[S22] C：字符串转数字
来源：http://rvr.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://uuc.cucudq.cn

[S23] C：随机数
来源：http://aaz.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nfl.wangdashe.top

[S24] C：获取本地时间
来源：http://eke.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jjk.nwbrower.top

[S25] C：内存拷贝
来源：http://ckm.gotoacloud.top

memcpy(dst, src, n);
来源：http://xqr.chenjidiqi.icu

[S26] C：内存清零
来源：http://akw.yonumen.top

memset(a, 0, sizeof a);
来源：http://kjr.fktsv.cn

[S27] C：定义常量
来源：http://efd.tianlin.xyz

const double PI = 3.14159;
来源：http://cel.pycfn.com

[S28] C：静态变量
来源：http://dld.hcnkem.com

static int counter = 0;
来源：http://bdb.hcnkem.com

[S29] C：变参函数
来源：http://qri.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://exa.yongpay.top

[S30] C：头文件保护
来源：http://nbh.yonumen.top

#ifndef X_H
来源：http://iav.cashguo.top

#define X_H
来源：http://ncl.svipenyu.cn

#endif
来源：http://fxv.xuetiantiany.cn

[S31] C++：Hello World
来源：http://ygd.feifeiyinyue.top

#include <iostream>
来源：http://bpj.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://rlq.yangfankeji.com

[S32] C++：字符串
来源：http://qmp.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://cxc.xuanzx.com

[S33] C++：vector 增删
来源：http://vbr.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vov.c1oappe.top

[S34] C++：遍历 vector
来源：http://bfd.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://hrl.quarkkingdee.top

[S35] C++：map
来源：http://gms.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dcp.smart0.xyz

[S36] C++：unordered_map
来源：http://csw.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uoe.yj20258.top

[S37] C++：set
来源：http://das.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rii.wangshuangyany.cn

[S38] C++：排序
来源：http://hdm.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://gbr.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://xaf.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cpt.xziqi.cn

[S40] C++：查找元素
来源：http://xfh.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mhq.yuanzhike.top

[S41] C++：类与构造函数
来源：http://ujo.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kgr.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://boj.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://wvi.pengpengdd.cyou

[S43] C++：智能指针
来源：http://npi.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://ubg.pycfn.com

[S44] C++：引用传参
来源：http://bob.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://jar.hcnkem.com

[S45] C++：lambda
来源：http://zyu.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://ume.quarkkingdee.top

[S46] C++：函数模板
来源：http://ufo.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://loc.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://zvr.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjf.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://qud.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jfn.yueranfly.top

while (std::getline(in, line)) { }
来源：http://ktr.xinyue.icu

[S49] C++：写文件
来源：http://sgi.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://opc.xinyue.icu

[S50] C++：格式化数字
来源：http://twa.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gaj.hnqzz.top

[S51] C++：显式类型转换
来源：http://ofr.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://wpx.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://udk.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://gkr.cqqwz.cn

[S53] C++：移动语义
来源：http://evg.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://tws.cdnleiting.top

[S54] C++：异常处理
来源：http://qrn.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvk.yuanzhike.top

[S55] C++：结构化绑定
来源：http://vlh.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://khi.hywenlv.cn

[S56] C++：optional
来源：http://zst.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lka.hywenlv.cn

[S57] C++：编译期常量
来源：http://jjr.zhengqikj.top

constexpr int N = 10;
来源：http://sbk.hnxiangtu.top

[S58] C++：命名空间
来源：http://ufl.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://vby.chenlongwang.top

[S59] C++：静态断言
来源：http://hpy.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://agn.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://fwj.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kcn.nwbrower.top

================================================================================
来源：http://tge.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mdh.aibaodan.cn

================================================================================
来源：http://vgq.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://myf.jinyuanbaomall.cn

println("Hello")
来源：http://efa.shuidangran.top

[T02] Kotlin：变量
来源：http://xtl.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mta.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://lnd.jqgufenzy.top

"值: $b"
来源：http://ima.zdqjudy.top

[T04] Kotlin：空安全
来源：http://pfo.yueranfly.top

val n: String? = null;  n?.length
来源：http://cma.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://gya.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zpq.daria6918.cn

[T06] Kotlin：集合映射
来源：http://mvu.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zwb.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://ltg.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yck.haohaochexian.top

[T08] Kotlin：数据类
来源：http://div.sweek.top

data class User(val name: String, val age: Int)
来源：http://qbm.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://ymz.pycfn.com

fun String.exclaim() = this + "!"
来源：http://veo.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://gie.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mgj.ctjpmb.com

[T11] Kotlin：协程
来源：http://huh.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sio.jianghu66.top

[T12] Kotlin：解构声明
来源：http://lcp.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://zic.tarul.cn

[T13] Kotlin：只读 Map
来源：http://cyl.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://qon.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://viw.xinyue.icu

for (i in 1..10) println(i)
来源：http://sxb.jinqigfzy.top

[T15] Kotlin：接口
来源：http://urc.ydzc1.top

interface Shape { fun area(): Double }
来源：http://pru.nwbrower.top

[T16] Swift：Hello World
来源：http://ymq.zdbjq.cn

print("Hello")
来源：http://qit.cheryme.top

[T17] Swift：变量与常量
来源：http://ias.hammf.cn

var a = 1;  let b = 2
来源：http://clq.jinqigufen.top

[T18] Swift：字符串插值
来源：http://nvz.wangdashe.top

"值: \(b)"
来源：http://kqh.sysykeji.top

[T19] Swift：可选绑定
来源：http://gau.sweek.top

if let n = opt { print(n) }
来源：http://mra.tarul.cn

[T20] Swift：数组操作
来源：http://kkp.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://cdk.nanxinkj.top

[T21] Swift：遍历
来源：http://ntt.tianlin.xyz

for x in a { print(x) }
来源：http://uvd.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://qam.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://hvx.yueranfly.top

[T23] Swift：函数
来源：http://rlb.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jpy.zhoulong.xyz

[T24] Swift：闭包
来源：http://xzp.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://xcm.sjlbkw.cn

[T25] Swift：结构体
来源：http://vyn.snrcjt.cn

struct P { var x: Int }
来源：http://udc.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://njq.ctjpmb.com

class A: Base { override func f() {} }
来源：http://nnm.dashuyun.cn

[T27] Swift：错误处理
来源：http://ium.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://crc.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://mcg.vehdjk.com

enum Color { case red, green }
来源：http://kju.uphjek.com

[T29] Swift：guard 提前返回
来源：http://slp.xuetiantiany.cn

guard let x = opt else { return }
来源：http://jxr.9152youxi.cn

[T30] Swift：协议
来源：http://dsq.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://vfx.c1oappe.top

[T31] Lua：Hello World
来源：http://joj.hnxiangtu.top

print("Hello")
来源：http://iho.jianghu66.top

[T32] Lua：局部变量
来源：http://bns.tianlin.xyz

local a = 1
来源：http://tnp.yueranfly.top

[T33] Lua：表（数组）
来源：http://mlq.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sil.ppjwa.cn

[T34] Lua：遍历表
来源：http://xcf.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pqa.sxryk.cn

[T35] Lua：字典表
来源：http://kro.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://rpd.bbcook.cn

[T36] Lua：函数
来源：http://xex.ctjpmb.com

function add(a, b) return a + b end
来源：http://auv.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://lha.chenzaomai.com

"a" .. "b"
来源：http://lxg.yuxming.cn

[T38] Lua：条件
来源：http://mnq.svipenyu.cn

if x > 0 then print("正") end
来源：http://brp.dianchejie.cn

[T39] Lua：模式匹配
来源：http://voo.gzhubu.top

string.find(s, "%d+")
来源：http://xpp.yuxming.cn

[T40] Lua：元表
来源：http://abk.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://krk.bbcook.cn

[T41] Perl：Hello World
来源：http://zxn.fktsv.cn

print "Hello\n";
来源：http://dke.ybcxt.top

[T42] Perl：变量类型
来源：http://vla.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xpv.daria6918.cn

[T43] Perl：字符串插值
来源：http://mbk.birdmap.top

"值: $a"
来源：http://rqp.aizwys.cn

[T44] Perl：条件
来源：http://wdt.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://pbq.aibaodan.cn

[T45] Perl：数组遍历
来源：http://qkq.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://piz.yongpay.top

[T46] Perl：哈希操作
来源：http://vhx.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zig.hcnkem.com

[T47] Perl：正则捕获
来源：http://ogg.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mmj.bbcook.cn

[T48] Perl：正则替换
来源：http://oud.yangfankeji.com

$s =~ s/old/new/g;
来源：http://lrf.dashuyun.cn

[T49] Perl：函数
来源：http://lae.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ybl.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://jds.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nac.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://evy.zhijiandao.cn

[T51] Scala：Hello World
来源：http://xsu.smart0.xyz

println("Hello")
来源：http://jhv.yuanzhike.top

[T52] Scala：变量
来源：http://xmk.daria6918.cn

val a = 1;  var b = 2
来源：http://tyx.hcnkem.com

[T53] Scala：字符串插值
来源：http://bba.iojbl.cn

s"值: $b"
来源：http://jev.hysaishi.cn

[T54] Scala：集合映射
来源：http://vrf.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://wkp.zdbjq.cn

[T55] Scala：集合过滤
来源：http://niw.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://uzy.quarkkingdee.top

[T56] Scala：样例类
来源：http://mbs.zdqjudy.top

case class User(name: String, age: Int)
来源：http://eaz.tarul.cn

[T57] Scala：模式匹配
来源：http://bmf.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zia.nanxinkj.top

[T58] Scala：函数定义
来源：http://dwg.havefunace.top


<!-- 参考信息 -->