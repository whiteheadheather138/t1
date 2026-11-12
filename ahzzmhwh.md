代发 wailian999

ssh user@host 'uptime'
来源：http://qzx.quarkkingdee.top

[R58] 下载文件
来源：http://ruj.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tgf.pycfn.com

[R59] 发 POST JSON
来源：http://bva.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fiu.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://kup.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qfy.chenjidiqi.icu

[R61] 磁盘占用
来源：http://mvs.sjlbkw.cn

df -h;  du -sh *
来源：http://bks.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://wqr.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://nrp.chenlongwang.top

[R63] 内存与进程
来源：http://xzj.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://kyr.hfpthk.cn

[R64] 结束进程
来源：http://hmq.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://flm.yuanzhike.top

[R65] 查看端口占用
来源：http://wfv.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gpw.gogol.net.cn

[R66] 定时任务
来源：http://hei.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://yhb.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://eht.shzxlz.cn

openssl rand -hex 16
来源：http://uls.yueranfly.top

[R68] 计算文件校验值
来源：http://qsv.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://hcp.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://ekf.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://tpc.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://glo.wangdashe.top

date +%s;  date -d @1700000000
来源：http://gds.hammf.cn

[R71] 日期格式化
来源：http://hwr.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xda.jlsjyb.cn

[R72] 等待端口就绪
来源：http://nxz.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://esd.daria6918.cn

[R73] 分割大日志
来源：http://qzt.vehdjk.com

split -l 1000 big.log part_
来源：http://aps.ivvv.top

[R74] 批量重命名
来源：http://fuw.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qvz.wangdashe.top

[R75] 导出环境变量
来源：http://vte.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zfv.nanxuanxn.top

[R76] 使用临时文件
来源：http://icf.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yni.xylfe.cn

[R77] 读取用户输入
来源：http://peu.zhoulong.xyz

read -rp "请输入: " ans
来源：http://isu.daxiang520.top

[R78] 交互式菜单
来源：http://uds.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://xgx.wangdashe.top

[R79] 解析命令行选项
来源：http://dog.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yho.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://nvk.gaohongyu789.top

time ./run.sh
来源：http://wcs.epnwcf.com

================================================================================
来源：http://pof.hammf.cn

S. C / C++ 专题
来源：http://efy.sxryk.cn

================================================================================
来源：http://owj.birdmap.top

[S01] C：Hello World
来源：http://esg.fktsv.cn

#include <stdio.h>
来源：http://cmn.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qwu.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://pdd.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://gzj.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://zjx.svipenyu.cn

int x; scanf("%d", &x);
来源：http://car.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://bol.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://kpq.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://xnw.zhoulong.xyz

strlen(s)
来源：http://aek.zhoulong.xyz

[S06] C：字符串比较
来源：http://dme.jqgufenzy.top

strcmp(a, b) == 0
来源：http://wvo.yfazqb.com

[S07] C：数组遍历求和
来源：http://xvg.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://odt.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://zmb.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uvi.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://tpm.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bnn.yj20258.top

[S10] C：指针与解引用
来源：http://jcg.xinyue.icu

int *p = &a;  *p = 5;
来源：http://imm.dashuyun.cn

[S11] C：逐行读文件
来源：http://wrw.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://get.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ohk.ehwqpu.com

fclose(f);
来源：http://umb.hongshengwenyu.top

[S12] C：写文件
来源：http://rou.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://giy.sysykeji.top

[S13] C：宏定义
来源：http://ppa.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brt.cashguo.top

[S14] C：枚举
来源：http://mmt.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://yyt.vqdsnc.cn

[S15] C：类型转换
来源：http://qpe.bbcook.cn

(double) a / b
来源：http://ndr.tian-w.cn

[S16] C：位操作置位
来源：http://glv.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://hbt.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://qwq.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://piv.hnxiangtu.top

[S18] C：命令行参数
来源：http://edz.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://kzz.sxryk.cn

[S19] C：快速排序
来源：http://kzc.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://lng.dashuyun.cn

[S20] C：二分查找
来源：http://pbn.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nds.cheryme.top

[S21] C：字符类别判断
来源：http://sfx.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ekp.nwbrower.top

[S22] C：字符串转数字
来源：http://foi.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://dkm.9152youxi.cn

[S23] C：随机数
来源：http://oly.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oyl.havefunace.top

[S24] C：获取本地时间
来源：http://odu.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nlr.snrcjt.cn

[S25] C：内存拷贝
来源：http://bqk.jinqigufen.top

memcpy(dst, src, n);
来源：http://jzz.meibo888.top

[S26] C：内存清零
来源：http://ife.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://ydy.uphjek.com

[S27] C：定义常量
来源：http://tcs.c1oappe.top

const double PI = 3.14159;
来源：http://jia.kuanghao11.cn

[S28] C：静态变量
来源：http://etz.sxryk.cn

static int counter = 0;
来源：http://exv.zycfv.cn

[S29] C：变参函数
来源：http://okj.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xyw.zhijiandao.cn

[S30] C：头文件保护
来源：http://arq.aibaodan.cn

#ifndef X_H
来源：http://fel.zhongyouzk.top

#define X_H
来源：http://vyy.gotoacloud.top

#endif
来源：http://aio.ybcxt.top

[S31] C++：Hello World
来源：http://bnu.bbcook.cn

#include <iostream>
来源：http://orm.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://cpy.jinghuilouyu.cn

[S32] C++：字符串
来源：http://zgj.yj202588.top

std::string s = "hi";  s += "!";
来源：http://eqg.zhengqikj.top

[S33] C++：vector 增删
来源：http://smv.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gji.shzxlz.cn

[S34] C++：遍历 vector
来源：http://raf.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://hzo.yuanzhike.top

[S35] C++：map
来源：http://glm.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ekb.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://sta.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eml.jinqigfzy.top

[S37] C++：set
来源：http://wyx.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wfx.zycfv.cn

[S38] C++：排序
来源：http://keb.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://nuo.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://rre.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rbl.0kj1m.cn

[S40] C++：查找元素
来源：http://dqh.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eii.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://ifr.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aiz.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://owa.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://tqe.nwbrower.top

[S43] C++：智能指针
来源：http://elx.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://utu.wangshuangyany.cn

[S44] C++：引用传参
来源：http://csn.xinyue.icu

void inc(int &x) { ++x; }
来源：http://bzo.gogol.net.cn

[S45] C++：lambda
来源：http://vte.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://aaj.yfazqb.com

[S46] C++：函数模板
来源：http://xfq.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qtb.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://wht.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vav.yvedp.cn

[S48] C++：逐行读文件
来源：http://rnu.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://ryl.fengsongda.top

while (std::getline(in, line)) { }
来源：http://sam.0kj1m.cn

[S49] C++：写文件
来源：http://dgy.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tad.sweek.top

[S50] C++：格式化数字
来源：http://foy.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cqe.jyoumei.cn

[S51] C++：显式类型转换
来源：http://uak.zhengqikj.top

static_cast<double>(a) / b
来源：http://lil.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://raw.hesvh.cn

int size() const noexcept { return n_; }
来源：http://ckb.sufxvd.cn

[S53] C++：移动语义
来源：http://nss.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://cod.vqdsnc.cn

[S54] C++：异常处理
来源：http://tke.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qmm.zdqjudy.top

[S55] C++：结构化绑定
来源：http://upw.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tut.yueranfly.top

[S56] C++：optional
来源：http://tzj.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nhx.sxryk.cn

[S57] C++：编译期常量
来源：http://lre.cqqwz.cn

constexpr int N = 10;
来源：http://bcf.yanxiufei.cn

[S58] C++：命名空间
来源：http://hxa.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://kho.vqdsnc.cn

[S59] C++：静态断言
来源：http://ntm.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwx.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://fqh.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tqc.shuidangran.top

================================================================================
来源：http://nqj.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgn.zdbjq.cn

================================================================================
来源：http://luy.sxryk.cn

[T01] Kotlin：Hello World
来源：http://asj.jinghuilouyu.cn

println("Hello")
来源：http://ajn.52xcode.cn

[T02] Kotlin：变量
来源：http://zhz.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yju.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://gat.jinqigufen.top

"值: $b"
来源：http://srf.chenlongwang.top

[T04] Kotlin：空安全
来源：http://zij.c1oappe.top

val n: String? = null;  n?.length
来源：http://kux.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://tpy.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wcs.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://iia.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xjt.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://qdl.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvj.c1oappe.top

[T08] Kotlin：数据类
来源：http://fby.tarul.cn

data class User(val name: String, val age: Int)
来源：http://ljw.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://lgd.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://wsp.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://txc.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xot.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://dho.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ilp.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://dgs.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://dbi.316326.xyz

[T13] Kotlin：只读 Map
来源：http://bck.tanke756.top

val m = mapOf("a" to 1)
来源：http://txq.cucudq.cn

[T14] Kotlin：循环
来源：http://nfh.yueranfly.top

for (i in 1..10) println(i)
来源：http://dir.uphjek.com

[T15] Kotlin：接口
来源：http://yfy.fengsongda.top

interface Shape { fun area(): Double }
来源：http://xve.tian-w.cn

[T16] Swift：Hello World
来源：http://wcw.gzhubu.top

print("Hello")
来源：http://iva.c1oappe.top

[T17] Swift：变量与常量
来源：http://dte.hysaishi.cn

var a = 1;  let b = 2
来源：http://ghd.hfpthk.cn

[T18] Swift：字符串插值
来源：http://qgn.zhengqikj.top

"值: \(b)"
来源：http://gnr.c1oappe.top

[T19] Swift：可选绑定
来源：http://zux.wangdashe.top

if let n = opt { print(n) }
来源：http://thd.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://cae.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://svs.jianghu66.top

[T21] Swift：遍历
来源：http://rkn.xziqi.cn

for x in a { print(x) }
来源：http://mhz.ybcxt.top

[T22] Swift：字典
来源：http://txr.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://urm.hcnkem.com

[T23] Swift：函数
来源：http://ssx.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iww.jianghu66.top

[T24] Swift：闭包
来源：http://rtn.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hye.dianchejie.cn

[T25] Swift：结构体
来源：http://wiu.jlsjyb.cn

struct P { var x: Int }
来源：http://qpy.ybcxt.top

[T26] Swift：类与重写
来源：http://ytn.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://kkt.wangdashe.top

[T27] Swift：错误处理
来源：http://txr.sysykeji.top

do { try f() } catch { print(error) }
来源：http://kxs.fzhhl.top

[T28] Swift：枚举
来源：http://hta.kuanghao11.cn

enum Color { case red, green }
来源：http://ddg.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://qhd.sweek.top

guard let x = opt else { return }
来源：http://xyi.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://gtd.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://bru.guannengcc.top

[T31] Lua：Hello World
来源：http://xov.yueranfly.top

print("Hello")
来源：http://dtc.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://gbh.zhengqikj.top

local a = 1
来源：http://jqh.sysykeji.top

[T33] Lua：表（数组）
来源：http://hdn.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qyw.gotoacloud.top

[T34] Lua：遍历表
来源：http://gxs.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://snh.zdqjudy.top

[T35] Lua：字典表
来源：http://ldo.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://acg.jyoumei.cn

[T36] Lua：函数
来源：http://gco.vehdjk.com

function add(a, b) return a + b end
来源：http://faj.birdmap.top

[T37] Lua：字符串拼接
来源：http://nal.cucudq.cn

"a" .. "b"
来源：http://mjb.wangshuangyany.cn

[T38] Lua：条件
来源：http://nco.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://jkm.bjfxy.top

[T39] Lua：模式匹配
来源：http://zye.daxiang520.top

string.find(s, "%d+")
来源：http://kuf.yueranfly.top

[T40] Lua：元表
来源：http://hvw.wangdashe.top

setmetatable({}, { __index = base })
来源：http://igt.yuanzhike.top

[T41] Perl：Hello World
来源：http://pul.jlsjyb.cn

print "Hello\n";
来源：http://lli.ydzc1.top

[T42] Perl：变量类型
来源：http://ulu.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nbb.guannengcc.top

[T43] Perl：字符串插值
来源：http://www.ydzc1.top

"值: $a"
来源：http://cqq.nanxuanxn.top

[T44] Perl：条件
来源：http://vgu.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://fud.52xcode.cn

[T45] Perl：数组遍历
来源：http://zzw.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://vck.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://xqk.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://axm.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://amt.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hbu.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://iql.yfazqb.com

$s =~ s/old/new/g;
来源：http://lxd.jianghu66.top

[T49] Perl：函数
来源：http://dvs.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yah.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://sha.chenlongwang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rge.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://lkm.sufxvd.cn

[T51] Scala：Hello World
来源：http://uau.guannengcc.top

println("Hello")
来源：http://xzu.sweek.top

[T52] Scala：变量
来源：http://beq.xziqi.cn

val a = 1;  var b = 2
来源：http://fkb.fehbvm.com

[T53] Scala：字符串插值
来源：http://vzv.dashuyun.cn

s"值: $b"
来源：http://zyz.sweek.top

[T54] Scala：集合映射
来源：http://aue.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://agh.haohaochexian.top

[T55] Scala：集合过滤
来源：http://joa.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://agu.bbcook.cn

[T56] Scala：样例类
来源：http://zwk.daxiang520.top

case class User(name: String, age: Int)
来源：http://fcc.yangfankeji.com

[T57] Scala：模式匹配
来源：http://bdp.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cjh.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://mqp.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://qxs.sjlbkw.cn

[T59] Scala：循环
来源：http://jfj.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://pzn.chenjidiqi.icu

[T60] Scala：折叠
来源：http://eyj.ydjk.org.cn


<!-- 参考信息 -->