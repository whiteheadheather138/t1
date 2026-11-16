代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xhf.bbcook.cn

[R56] 远程拷贝
来源：http://mwk.jinqigufen.top

scp file user@host:/path/
来源：http://eik.shangyingyoupin.top

[R57] 远程执行命令
来源：http://uvo.xylfe.cn

ssh user@host 'uptime'
来源：http://mot.mhx1999.top

[R58] 下载文件
来源：http://lvd.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://arc.yongpay.top

[R59] 发 POST JSON
来源：http://zsw.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wkt.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://ozr.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zir.yonumen.top

[R61] 磁盘占用
来源：http://nqe.nanxinkj.top

df -h;  du -sh *
来源：http://tgx.redwolf501.top

[R62] 找最占空间的文件
来源：http://ktg.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://dlw.yj20258.top

[R63] 内存与进程
来源：http://xgt.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://ziv.sysykeji.top

[R64] 结束进程
来源：http://muo.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://blg.zhengqikj.top

[R65] 查看端口占用
来源：http://axp.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qcl.yfazqb.com

[R66] 定时任务
来源：http://ecu.tianlin.xyz

crontab -e;  crontab -l
来源：http://hqd.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://ifk.redwolf501.top

openssl rand -hex 16
来源：http://nqr.chenzaomai.com

[R68] 计算文件校验值
来源：http://pls.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pca.sysykeji.top

[R69] 生成随机密码
来源：http://lxw.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://dws.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://dhx.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://sje.snrcjt.cn

[R71] 日期格式化
来源：http://yau.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vpv.cheryme.top

[R72] 等待端口就绪
来源：http://lrq.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vqq.yfazqb.com

[R73] 分割大日志
来源：http://pka.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://asd.yuxming.cn

[R74] 批量重命名
来源：http://btv.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cuq.dashuyun.cn

[R75] 导出环境变量
来源：http://aji.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://yya.pycfn.com

[R76] 使用临时文件
来源：http://jub.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nin.aibaodan.cn

[R77] 读取用户输入
来源：http://vdv.yueranfly.top

read -rp "请输入: " ans
来源：http://hjx.ivvv.top

[R78] 交互式菜单
来源：http://nuu.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mex.xuanzx.com

[R79] 解析命令行选项
来源：http://lma.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gop.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://gix.xuetiantiany.cn

time ./run.sh
来源：http://pel.epnwcf.com

================================================================================
来源：http://zbt.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://rec.fanxiaobao.xyz

================================================================================
来源：http://ftn.hywenlv.cn

[S01] C：Hello World
来源：http://won.birdmap.top

#include <stdio.h>
来源：http://qid.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nmg.fengsongda.top

[S02] C：变量与格式化输出
来源：http://lyy.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://wbc.fengsongda.top

[S03] C：读入整数
来源：http://ogk.cdnleiting.top

int x; scanf("%d", &x);
来源：http://spx.havefunace.top

[S04] C：字符串复制
来源：http://qct.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mpn.yuanzhike.top

[S05] C：字符串长度
来源：http://rbd.xylfe.cn

strlen(s)
来源：http://mwj.shuidangran.top

[S06] C：字符串比较
来源：http://tdt.fktsv.cn

strcmp(a, b) == 0
来源：http://qty.nanxinkj.top

[S07] C：数组遍历求和
来源：http://iyv.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qtc.yongpay.top

[S08] C：动态内存分配与释放
来源：http://ohu.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uqj.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://koo.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://txl.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://nvn.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://fqz.svipenyu.cn

[S11] C：逐行读文件
来源：http://oqz.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://zms.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://qlg.aizwys.cn

fclose(f);
来源：http://ugj.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://ogd.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rtn.vqdsnc.cn

[S13] C：宏定义
来源：http://xxm.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tev.shuidangran.top

[S14] C：枚举
来源：http://aez.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://eod.yj202588.top

[S15] C：类型转换
来源：http://gnr.52xcode.cn

(double) a / b
来源：http://bap.yj20258.top

[S16] C：位操作置位
来源：http://xxr.yuanzhike.top

x |= (1 << 3);
来源：http://eth.bjfxy.top

[S17] C：安全拼接字符串
来源：http://xzk.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bmi.0kj1m.cn

[S18] C：命令行参数
来源：http://cjb.tanke756.top

int main(int argc, char **argv)
来源：http://pdg.c1oappe.top

[S19] C：快速排序
来源：http://lyb.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://kea.hfpthk.cn

[S20] C：二分查找
来源：http://apz.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://otk.ppjwa.cn

[S21] C：字符类别判断
来源：http://uzt.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hpd.redwolf501.top

[S22] C：字符串转数字
来源：http://hnl.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ovg.feifeiyinyue.top

[S23] C：随机数
来源：http://izd.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ddw.yj20258888.top

[S24] C：获取本地时间
来源：http://vcq.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xno.yueranfly.top

[S25] C：内存拷贝
来源：http://dzn.iojbl.cn

memcpy(dst, src, n);
来源：http://llb.smart0.xyz

[S26] C：内存清零
来源：http://elg.hcnkem.com

memset(a, 0, sizeof a);
来源：http://nbx.ivvv.top

[S27] C：定义常量
来源：http://ktf.daria6918.cn

const double PI = 3.14159;
来源：http://sma.yuanzhike.top

[S28] C：静态变量
来源：http://piq.jinqigfzy.top

static int counter = 0;
来源：http://jvg.yvedp.cn

[S29] C：变参函数
来源：http://fiz.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pfs.tanke756.top

[S30] C：头文件保护
来源：http://avm.52xcode.cn

#ifndef X_H
来源：http://fuf.yj20258888.top

#define X_H
来源：http://vdr.daxiang520.top

#endif
来源：http://txm.zhoulong.xyz

[S31] C++：Hello World
来源：http://lra.hongshengwenyu.top

#include <iostream>
来源：http://olh.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://vls.sxryk.cn

[S32] C++：字符串
来源：http://zja.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://dee.cashguo.top

[S33] C++：vector 增删
来源：http://tih.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yxi.chenjidiqi.icu

[S34] C++：遍历 vector
来源：http://kss.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://rsc.daria6918.cn

[S35] C++：map
来源：http://qir.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vkc.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://csa.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxj.zhiwuduotai.top

[S37] C++：set
来源：http://feu.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jkc.jinghuilouyu.cn

[S38] C++：排序
来源：http://rsv.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://zwf.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://ukr.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sqv.jlsjyb.cn

[S40] C++：查找元素
来源：http://mlr.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qsy.ppjwa.cn

[S41] C++：类与构造函数
来源：http://mje.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fev.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://qcm.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://iwm.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://xvq.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://gux.haohaochexian.top

[S44] C++：引用传参
来源：http://bws.ivvv.top

void inc(int &x) { ++x; }
来源：http://ofw.zhixingplan.top

[S45] C++：lambda
来源：http://zwj.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://gkp.havefunace.top

[S46] C++：函数模板
来源：http://viu.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yxw.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://kxb.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lyi.snrcjt.cn

[S48] C++：逐行读文件
来源：http://wdi.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vco.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ogl.jinghuilouyu.cn

[S49] C++：写文件
来源：http://exr.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nbm.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://vbo.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uiu.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://grw.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://dgr.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://kyh.daria6918.cn

int size() const noexcept { return n_; }
来源：http://ewh.andypj.xyz

[S53] C++：移动语义
来源：http://onm.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://htu.fengsongda.top

[S54] C++：异常处理
来源：http://rge.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zxu.uphjek.com

[S55] C++：结构化绑定
来源：http://aqf.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hyh.zhixingplan.top

[S56] C++：optional
来源：http://ylj.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://udl.quarkkingdee.top

[S57] C++：编译期常量
来源：http://jre.tarul.cn

constexpr int N = 10;
来源：http://blz.havefunace.top

[S58] C++：命名空间
来源：http://bmr.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://ahv.zdqjudy.top

[S59] C++：静态断言
来源：http://gec.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mfi.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://hsp.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nkq.yongpay.top

================================================================================
来源：http://sey.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eju.zhiwuduotai.top

================================================================================
来源：http://lvm.ivvv.top

[T01] Kotlin：Hello World
来源：http://ozx.gogol.net.cn

println("Hello")
来源：http://ypm.svipenyu.cn

[T02] Kotlin：变量
来源：http://sym.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uwh.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://clh.yongpay.top

"值: $b"
来源：http://rho.xuanzx.com

[T04] Kotlin：空安全
来源：http://cnf.gotoacloud.top

val n: String? = null;  n?.length
来源：http://ehh.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://tak.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvj.sxryk.cn

[T06] Kotlin：集合映射
来源：http://ivx.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bnt.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://yrr.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://abg.bjfxy.top

[T08] Kotlin：数据类
来源：http://alr.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://sat.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://kuk.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://dxy.nwbrower.top

[T10] Kotlin：默认参数
来源：http://spp.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hlm.tian-w.cn

[T11] Kotlin：协程
来源：http://pux.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qfd.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://ejp.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://wbn.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://whg.yj20258888.top

val m = mapOf("a" to 1)
来源：http://eky.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://upt.9152youxi.cn

for (i in 1..10) println(i)
来源：http://yus.jinqigfzy.top

[T15] Kotlin：接口
来源：http://zhq.xylfe.cn

interface Shape { fun area(): Double }
来源：http://nlq.jianghu66.top

[T16] Swift：Hello World
来源：http://zqg.sufxvd.cn

print("Hello")
来源：http://xaj.svipenyu.cn

[T17] Swift：变量与常量
来源：http://epm.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://sju.meibo888.top

[T18] Swift：字符串插值
来源：http://mqg.ivvv.top

"值: \(b)"
来源：http://dow.redwolf501.top

[T19] Swift：可选绑定
来源：http://umg.tianlin.xyz

if let n = opt { print(n) }
来源：http://net.cucudq.cn

[T20] Swift：数组操作
来源：http://sfz.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://dnr.feifeiyinyue.top

[T21] Swift：遍历
来源：http://nwk.fzhhl.top

for x in a { print(x) }
来源：http://uwq.ybcxt.top

[T22] Swift：字典
来源：http://qjd.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nsy.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://thb.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://olm.nanxuanxn.top

[T24] Swift：闭包
来源：http://wpm.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://grp.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://ugu.zhoulong.xyz

struct P { var x: Int }
来源：http://lbz.cucudq.cn

[T26] Swift：类与重写
来源：http://ypx.316326.xyz

class A: Base { override func f() {} }
来源：http://yeb.ybcxt.top

[T27] Swift：错误处理
来源：http://krj.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://ofl.smart0.xyz

[T28] Swift：枚举
来源：http://lra.pycfn.com

enum Color { case red, green }
来源：http://dui.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://mdo.zhixingplan.top

guard let x = opt else { return }
来源：http://gqi.shangyingyoupin.top

[T30] Swift：协议
来源：http://cbc.yongpay.top

protocol Shape { func area() -> Double }
来源：http://rry.yj20258888.top

[T31] Lua：Hello World
来源：http://muh.yvedp.cn

print("Hello")
来源：http://abh.tian-w.cn

[T32] Lua：局部变量
来源：http://qhw.chenjidiqi.icu

local a = 1
来源：http://ger.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://zun.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://dof.cdnleiting.top

[T34] Lua：遍历表
来源：http://rqo.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fyr.hnxiangtu.top

[T35] Lua：字典表
来源：http://pwa.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://qfc.0kj1m.cn

[T36] Lua：函数
来源：http://ton.ybcxt.top

function add(a, b) return a + b end
来源：http://hev.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://xph.hnqzz.top

"a" .. "b"
来源：http://kpv.fktsv.cn

[T38] Lua：条件
来源：http://ubz.tianlin.xyz

if x > 0 then print("正") end
来源：http://lst.yj20258.top

[T39] Lua：模式匹配
来源：http://lbz.tianlin.xyz

string.find(s, "%d+")
来源：http://wcs.yangfankeji.com

[T40] Lua：元表
来源：http://ajp.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://vph.cashguo.top

[T41] Perl：Hello World
来源：http://cns.svipenyu.cn

print "Hello\n";
来源：http://ssy.fengsongda.top

[T42] Perl：变量类型
来源：http://lqa.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jse.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://wmq.gogol.net.cn

"值: $a"
来源：http://gfq.gaohongyu789.top

[T44] Perl：条件
来源：http://ttv.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://hwq.tanke756.top

[T45] Perl：数组遍历
来源：http://bld.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://she.birdmap.top

[T46] Perl：哈希操作
来源：http://mzw.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dqd.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://zfg.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hjd.zhijiandao.cn

[T48] Perl：正则替换
来源：http://yne.xylfe.cn

$s =~ s/old/new/g;
来源：http://rwb.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://mlm.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yod.fktsv.cn

[T50] Perl：逐行读文件
来源：http://dea.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sqx.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://zei.c1oappe.top

[T51] Scala：Hello World
来源：http://efn.hysaishi.cn

println("Hello")
来源：http://kth.yj20258.top

[T52] Scala：变量
来源：http://mmq.zhijiandao.cn

val a = 1;  var b = 2
来源：http://zrv.tanke756.top

[T53] Scala：字符串插值
来源：http://ybv.xingfuxueyuan.xyz

s"值: $b"
来源：http://oqp.dashuyun.cn

[T54] Scala：集合映射
来源：http://vpe.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://cvs.sxryk.cn

[T55] Scala：集合过滤
来源：http://ufl.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jjz.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://cco.gzhubu.top

case class User(name: String, age: Int)
来源：http://bwz.snrcjt.cn

[T57] Scala：模式匹配
来源：http://gxw.yj20258.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dyh.yj202588.top

[T58] Scala：函数定义
来源：http://god.hongshengwenyu.top


<!-- 参考信息 -->