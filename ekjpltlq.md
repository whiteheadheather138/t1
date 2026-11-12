代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wxo.aibaodan.cn

[R56] 远程拷贝
来源：http://jla.jqgfzy.top

scp file user@host:/path/
来源：http://uxd.zhijiandao.cn

[R57] 远程执行命令
来源：http://dkt.jyoumei.cn

ssh user@host 'uptime'
来源：http://fen.cqqwz.cn

[R58] 下载文件
来源：http://tju.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://obz.gogol.net.cn

[R59] 发 POST JSON
来源：http://hyb.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ciw.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://jpi.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wbc.hfpthk.cn

[R61] 磁盘占用
来源：http://kzu.yanxiufei.cn

df -h;  du -sh *
来源：http://gcv.fengsongda.top

[R62] 找最占空间的文件
来源：http://ess.sweek.top

du -ah . | sort -rh | head -10
来源：http://pmh.cucudq.cn

[R63] 内存与进程
来源：http://fip.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://afn.chenzaomai.com

[R64] 结束进程
来源：http://jau.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://nid.vqdsnc.cn

[R65] 查看端口占用
来源：http://omb.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://avj.sjlbkw.cn

[R66] 定时任务
来源：http://zjb.yanxiufei.cn

crontab -e;  crontab -l
来源：http://pcg.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://yeo.nanxinkj.top

openssl rand -hex 16
来源：http://vyy.cheryme.top

[R68] 计算文件校验值
来源：http://wkf.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://eaa.havefunace.top

[R69] 生成随机密码
来源：http://hnx.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://udy.jlsjyb.cn

[R70] 时间戳与互转
来源：http://xqm.hammf.cn

date +%s;  date -d @1700000000
来源：http://pzn.meibo888.top

[R71] 日期格式化
来源：http://dsi.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://txm.jinqigfzy.top

[R72] 等待端口就绪
来源：http://ovq.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zwl.shzxlz.cn

[R73] 分割大日志
来源：http://iss.bbcook.cn

split -l 1000 big.log part_
来源：http://flb.jianghu66.top

[R74] 批量重命名
来源：http://juf.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cmx.cqqwz.cn

[R75] 导出环境变量
来源：http://jjj.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://zeq.fktsv.cn

[R76] 使用临时文件
来源：http://ozk.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yoj.shzxlz.cn

[R77] 读取用户输入
来源：http://iqw.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://oci.zhixingplan.top

[R78] 交互式菜单
来源：http://rqq.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://vkb.cucudq.cn

[R79] 解析命令行选项
来源：http://pxp.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://krj.hcnkem.com

[R80] 查看脚本执行耗时
来源：http://ggz.sjlbkw.cn

time ./run.sh
来源：http://dty.daxiang520.top

================================================================================
来源：http://vux.yj20258888.top

S. C / C++ 专题
来源：http://nxg.jlsjyb.cn

================================================================================
来源：http://wsj.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://hga.zdqjudy.top

#include <stdio.h>
来源：http://wki.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tbx.daxiang520.top

[S02] C：变量与格式化输出
来源：http://pmq.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://bdt.daxiang520.top

[S03] C：读入整数
来源：http://gvf.0kj1m.cn

int x; scanf("%d", &x);
来源：http://cbc.vqdsnc.cn

[S04] C：字符串复制
来源：http://xgu.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rzh.pycfn.com

[S05] C：字符串长度
来源：http://lpx.sxryk.cn

strlen(s)
来源：http://keb.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://jjb.hnxiangtu.top

strcmp(a, b) == 0
来源：http://fki.pycfn.com

[S07] C：数组遍历求和
来源：http://kgx.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://odo.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://ngr.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hks.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://qkl.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dfn.yj20258888.top

[S10] C：指针与解引用
来源：http://buq.yj20258888.top

int *p = &a;  *p = 5;
来源：http://vgk.jyoumei.cn

[S11] C：逐行读文件
来源：http://rvt.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://afd.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dwy.jinqigufen.top

fclose(f);
来源：http://raw.pengpengdd.cyou

[S12] C：写文件
来源：http://iqx.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hkq.xuetiantiany.cn

[S13] C：宏定义
来源：http://ozs.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ivx.yueranfly.top

[S14] C：枚举
来源：http://tyx.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://wee.quarkkingdee.top

[S15] C：类型转换
来源：http://nuw.yj20258.top

(double) a / b
来源：http://cjf.tianlin.xyz

[S16] C：位操作置位
来源：http://pvu.snrcjt.cn

x |= (1 << 3);
来源：http://bxv.redwolf501.top

[S17] C：安全拼接字符串
来源：http://bvh.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yzd.snrcjt.cn

[S18] C：命令行参数
来源：http://tkk.sweek.top

int main(int argc, char **argv)
来源：http://vpg.kuanghao11.cn

[S19] C：快速排序
来源：http://zno.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://uel.ppjwa.cn

[S20] C：二分查找
来源：http://xer.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jfz.0kj1m.cn

[S21] C：字符类别判断
来源：http://nmp.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qew.hcnkem.com

[S22] C：字符串转数字
来源：http://pyr.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://uau.fktsv.cn

[S23] C：随机数
来源：http://skl.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rtg.cashguo.top

[S24] C：获取本地时间
来源：http://mjt.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sne.aizwys.cn

[S25] C：内存拷贝
来源：http://bmi.hammf.cn

memcpy(dst, src, n);
来源：http://umg.jyoumei.cn

[S26] C：内存清零
来源：http://caj.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://bjz.tanke756.top

[S27] C：定义常量
来源：http://zbt.yanxiufei.cn

const double PI = 3.14159;
来源：http://tiz.jyoumei.cn

[S28] C：静态变量
来源：http://xqk.jyoumei.cn

static int counter = 0;
来源：http://hsy.shuidangran.top

[S29] C：变参函数
来源：http://xfj.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sfj.jqgufenzy.top

[S30] C：头文件保护
来源：http://tur.yueranfly.top

#ifndef X_H
来源：http://upx.jinyuanbaomall.cn

#define X_H
来源：http://kyy.zdbjq.cn

#endif
来源：http://btn.ehwqpu.com

[S31] C++：Hello World
来源：http://tzp.vehdjk.com

#include <iostream>
来源：http://mtm.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://osr.yfazqb.com

[S32] C++：字符串
来源：http://zjd.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://tec.sysykeji.top

[S33] C++：vector 增删
来源：http://nfv.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zns.jqgfzy.top

[S34] C++：遍历 vector
来源：http://ysc.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://cvi.redwolf501.top

[S35] C++：map
来源：http://nni.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oyh.nanxuanxn.top

[S36] C++：unordered_map
来源：http://wpq.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://got.jqgufenzy.top

[S37] C++：set
来源：http://xib.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wek.fengsongda.top

[S38] C++：排序
来源：http://djo.tanke756.top

std::sort(v.begin(), v.end());
来源：http://kgp.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://nsx.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ktq.daxiang520.top

[S40] C++：查找元素
来源：http://ljn.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mit.wangdashe.top

[S41] C++：类与构造函数
来源：http://eni.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dte.redwolf501.top

[S42] C++：继承与虚函数
来源：http://dda.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://nnh.gzhubu.top

[S43] C++：智能指针
来源：http://qqi.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://erg.chenjidiqi.icu

[S44] C++：引用传参
来源：http://rmn.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://mhc.nwbrower.top

[S45] C++：lambda
来源：http://xwj.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://otm.yuxming.cn

[S46] C++：函数模板
来源：http://iae.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wzt.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://yca.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yuu.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://qzx.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://yfw.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://fvi.tianlin.xyz

[S49] C++：写文件
来源：http://wib.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://skz.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://smt.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qyp.chenzaomai.com

[S51] C++：显式类型转换
来源：http://jnp.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://tqg.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://ntl.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://hzz.yueranfly.top

[S53] C++：移动语义
来源：http://sna.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://lhg.hongshengwenyu.top

[S54] C++：异常处理
来源：http://pxv.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tvl.vehdjk.com

[S55] C++：结构化绑定
来源：http://quh.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://klq.epnwcf.com

[S56] C++：optional
来源：http://ati.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vfn.quarkkingdee.top

[S57] C++：编译期常量
来源：http://tpc.yongpay.top

constexpr int N = 10;
来源：http://chl.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://psb.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://rbq.yj20258.top

[S59] C++：静态断言
来源：http://fhu.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qsx.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://tpp.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ext.ehwqpu.com

================================================================================
来源：http://odl.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zrs.gotoacloud.top

================================================================================
来源：http://vdr.mhx1999.top

[T01] Kotlin：Hello World
来源：http://sxg.wangdashe.top

println("Hello")
来源：http://rzc.meibo888.top

[T02] Kotlin：变量
来源：http://upy.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xmp.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://qoa.cheryme.top

"值: $b"
来源：http://vwx.dashuyun.cn

[T04] Kotlin：空安全
来源：http://crs.xuanzx.com

val n: String? = null;  n?.length
来源：http://zmu.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://kpq.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vdw.fktsv.cn

[T06] Kotlin：集合映射
来源：http://mjc.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://eqj.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://ttb.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://acv.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://hjc.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://sbi.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://maw.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://isw.fzhhl.top

[T10] Kotlin：默认参数
来源：http://xyn.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vca.bjfxy.top

[T11] Kotlin：协程
来源：http://zhc.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dsh.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://mzm.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://mdg.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://sfu.fengsongda.top

val m = mapOf("a" to 1)
来源：http://qep.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://qxs.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://nwa.chenzaomai.com

[T15] Kotlin：接口
来源：http://wid.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://oap.hcnkem.com

[T16] Swift：Hello World
来源：http://ufc.yj202588.top

print("Hello")
来源：http://rnr.jiagoushi.top

[T17] Swift：变量与常量
来源：http://vtg.xziqi.cn

var a = 1;  let b = 2
来源：http://nab.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://bsg.pycfn.com

"值: \(b)"
来源：http://utm.zhixingplan.top

[T19] Swift：可选绑定
来源：http://giu.yfazqb.com

if let n = opt { print(n) }
来源：http://xaw.daria6918.cn

[T20] Swift：数组操作
来源：http://urd.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://mzu.daria6918.cn

[T21] Swift：遍历
来源：http://czd.zhijiandao.cn

for x in a { print(x) }
来源：http://gvo.fanxiaobao.xyz

[T22] Swift：字典
来源：http://dgu.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pxc.jlsjyb.cn

[T23] Swift：函数
来源：http://ssd.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mly.mhx1999.top

[T24] Swift：闭包
来源：http://frx.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xqe.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://rwe.fanxiaobao.xyz

struct P { var x: Int }
来源：http://xdx.yangfankeji.com

[T26] Swift：类与重写
来源：http://uov.hesvh.cn

class A: Base { override func f() {} }
来源：http://njg.vehdjk.com

[T27] Swift：错误处理
来源：http://dgj.sxryk.cn

do { try f() } catch { print(error) }
来源：http://ocb.aibaodan.cn

[T28] Swift：枚举
来源：http://ygb.daxiang520.top

enum Color { case red, green }
来源：http://acq.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://qxr.cqqwz.cn

guard let x = opt else { return }
来源：http://ecp.zhengqikj.top

[T30] Swift：协议
来源：http://wdf.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://lig.haohaochexian.top

[T31] Lua：Hello World
来源：http://juj.jinyuanbaomall.cn

print("Hello")
来源：http://upi.jianghu66.top

[T32] Lua：局部变量
来源：http://mwj.ydjk.org.cn

local a = 1
来源：http://gyy.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://zqg.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wvo.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://qxw.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gsf.redwolf501.top

[T35] Lua：字典表
来源：http://bfb.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://act.uphjek.com

[T36] Lua：函数
来源：http://azr.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://mam.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://tuz.sufxvd.cn

"a" .. "b"
来源：http://eve.yonumen.top

[T38] Lua：条件
来源：http://gzs.fehbvm.com

if x > 0 then print("正") end
来源：http://jrg.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://hnm.daxiang520.top

string.find(s, "%d+")
来源：http://ipq.svipenyu.cn

[T40] Lua：元表
来源：http://haa.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://qoh.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://eqp.smart0.xyz

print "Hello\n";
来源：http://qas.shuidangran.top

[T42] Perl：变量类型
来源：http://jmz.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ntf.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://zop.jinyuanbaomall.cn

"值: $a"
来源：http://ycg.yonumen.top

[T44] Perl：条件
来源：http://kfk.yongpay.top

if ($a > 0) { print "正"; }
来源：http://vkw.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://vww.uphjek.com

for my $x (@arr) { print $x; }
来源：http://wtr.epnwcf.com

[T46] Perl：哈希操作
来源：http://wca.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jgc.sweek.top

[T47] Perl：正则捕获
来源：http://swu.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yls.jlsjyb.cn

[T48] Perl：正则替换
来源：http://unn.gotoacloud.top

$s =~ s/old/new/g;
来源：http://fld.hfpthk.cn

[T49] Perl：函数
来源：http://nzj.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jle.bbcook.cn

[T50] Perl：逐行读文件
来源：http://heg.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ogm.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://ybl.wangdashe.top

[T51] Scala：Hello World
来源：http://hsr.pengpengdd.cyou

println("Hello")
来源：http://xac.yongpay.top

[T52] Scala：变量
来源：http://ain.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://snr.zdbjq.cn

[T53] Scala：字符串插值
来源：http://ukd.shangyingyoupin.top

s"值: $b"
来源：http://wcd.daxiang520.top

[T54] Scala：集合映射
来源：http://ziz.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://azd.iojbl.cn

[T55] Scala：集合过滤
来源：http://kjv.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zec.jlsjyb.cn

[T56] Scala：样例类
来源：http://kqv.yangfankeji.com

case class User(name: String, age: Int)
来源：http://zvj.uphjek.com

[T57] Scala：模式匹配
来源：http://mfy.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ewp.hesvh.cn

[T58] Scala：函数定义
来源：http://mjc.ehwqpu.com


<!-- 参考信息 -->