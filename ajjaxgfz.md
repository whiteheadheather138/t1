代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fsf.wangshuangyany.cn

[R54] 比较两个文件
来源：http://hdi.dianchejie.cn

diff a.txt b.txt
来源：http://trh.vehdjk.com

[R55] 压缩与解压
来源：http://ezs.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eme.cqqwz.cn

[R56] 远程拷贝
来源：http://vuf.tianlin.xyz

scp file user@host:/path/
来源：http://uyr.zdbjq.cn

[R57] 远程执行命令
来源：http://gne.fzhhl.top

ssh user@host 'uptime'
来源：http://zrp.shzxlz.cn

[R58] 下载文件
来源：http://ruj.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://toh.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://nsv.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://igq.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://szp.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yer.havefunace.top

[R61] 磁盘占用
来源：http://kmr.bjfxy.top

df -h;  du -sh *
来源：http://dkl.guowangkeji.top

[R62] 找最占空间的文件
来源：http://swy.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://gfj.hnxiangtu.top

[R63] 内存与进程
来源：http://nvk.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://lpv.fktsv.cn

[R64] 结束进程
来源：http://hwv.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://tti.0kj1m.cn

[R65] 查看端口占用
来源：http://zdi.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kch.fktsv.cn

[R66] 定时任务
来源：http://eaj.zhoulong.xyz

crontab -e;  crontab -l
来源：http://wlr.tarul.cn

[R67] 生成随机十六进制串
来源：http://kyg.smart0.xyz

openssl rand -hex 16
来源：http://dkz.yuxming.cn

[R68] 计算文件校验值
来源：http://yug.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aqc.pycfn.com

[R69] 生成随机密码
来源：http://sqi.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://yas.zhixingplan.top

[R70] 时间戳与互转
来源：http://bfd.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://tbq.zhiwuduotai.top

[R71] 日期格式化
来源：http://fcd.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hbv.guannengcc.top

[R72] 等待端口就绪
来源：http://dxc.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xfx.ivvv.top

[R73] 分割大日志
来源：http://klk.dianchejie.cn

split -l 1000 big.log part_
来源：http://scs.yj20258888.top

[R74] 批量重命名
来源：http://gnk.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aip.haohaochexian.top

[R75] 导出环境变量
来源：http://gjs.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://zmf.meibo888.top

[R76] 使用临时文件
来源：http://zwe.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fbi.fktsv.cn

[R77] 读取用户输入
来源：http://xhj.xziqi.cn

read -rp "请输入: " ans
来源：http://qjt.yueranfly.top

[R78] 交互式菜单
来源：http://cpa.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ybi.bjfxy.top

[R79] 解析命令行选项
来源：http://hoi.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rus.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://vhm.jqgufenzy.top

time ./run.sh
来源：http://skc.sweek.top

================================================================================
来源：http://shm.cucudq.cn

S. C / C++ 专题
来源：http://gdp.ydzc1.top

================================================================================
来源：http://sib.jinqigfzy.top

[S01] C：Hello World
来源：http://flm.nanxuanxn.top

#include <stdio.h>
来源：http://zzb.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zyz.gzhubu.top

[S02] C：变量与格式化输出
来源：http://fzl.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://tvm.uphjek.com

[S03] C：读入整数
来源：http://zon.fzhhl.top

int x; scanf("%d", &x);
来源：http://ujm.svipenyu.cn

[S04] C：字符串复制
来源：http://eqh.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cam.nanxinkj.top

[S05] C：字符串长度
来源：http://tay.yuxming.cn

strlen(s)
来源：http://znw.quarkkingdee.top

[S06] C：字符串比较
来源：http://epe.bjfxy.top

strcmp(a, b) == 0
来源：http://tzq.zdqjudy.top

[S07] C：数组遍历求和
来源：http://elh.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bop.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://axn.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzr.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://zwp.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aai.bbcook.cn

[S10] C：指针与解引用
来源：http://itb.smart0.xyz

int *p = &a;  *p = 5;
来源：http://mzn.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://krn.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://vie.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fxb.xziqi.cn

fclose(f);
来源：http://ktu.jiagoushi.top

[S12] C：写文件
来源：http://wlc.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jza.hnxiangtu.top

[S13] C：宏定义
来源：http://drm.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vbk.bjfxy.top

[S14] C：枚举
来源：http://qbn.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://het.pengpengdd.cyou

[S15] C：类型转换
来源：http://uhd.dianchejie.cn

(double) a / b
来源：http://phx.aibaodan.cn

[S16] C：位操作置位
来源：http://nsp.shuidangran.top

x |= (1 << 3);
来源：http://rlo.pycfn.com

[S17] C：安全拼接字符串
来源：http://oli.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oua.bbcook.cn

[S18] C：命令行参数
来源：http://pgj.9152youxi.cn

int main(int argc, char **argv)
来源：http://tgc.havefunace.top

[S19] C：快速排序
来源：http://rqq.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bhx.jinghuilouyu.cn

[S20] C：二分查找
来源：http://evy.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tdp.sysykeji.top

[S21] C：字符类别判断
来源：http://dmo.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rax.fehbvm.com

[S22] C：字符串转数字
来源：http://pmi.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://agw.cucudq.cn

[S23] C：随机数
来源：http://ydz.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zvb.havefunace.top

[S24] C：获取本地时间
来源：http://tiz.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://for.bbcook.cn

[S25] C：内存拷贝
来源：http://uqs.fehbvm.com

memcpy(dst, src, n);
来源：http://fjc.sxryk.cn

[S26] C：内存清零
来源：http://bfg.yj20258888.top

memset(a, 0, sizeof a);
来源：http://lri.ivvv.top

[S27] C：定义常量
来源：http://ait.cashguo.top

const double PI = 3.14159;
来源：http://baa.zhongyouzk.top

[S28] C：静态变量
来源：http://zhq.jinqigfzy.top

static int counter = 0;
来源：http://cdn.ivvv.top

[S29] C：变参函数
来源：http://btq.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ycw.shuidangran.top

[S30] C：头文件保护
来源：http://euz.yanxiufei.cn

#ifndef X_H
来源：http://ygi.tianlin.xyz

#define X_H
来源：http://zuc.fanxiaobao.xyz

#endif
来源：http://psu.feifeiyinyue.top

[S31] C++：Hello World
来源：http://pyg.zhijiandao.cn

#include <iostream>
来源：http://xtl.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://beg.c1oappe.top

[S32] C++：字符串
来源：http://zkh.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://hvb.zhoulong.xyz

[S33] C++：vector 增删
来源：http://zeh.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qwx.cashguo.top

[S34] C++：遍历 vector
来源：http://swz.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://rdi.fzhhl.top

[S35] C++：map
来源：http://jzf.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khx.yj202588.top

[S36] C++：unordered_map
来源：http://nrv.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kcw.jlsjyb.cn

[S37] C++：set
来源：http://vqx.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kki.jlsjyb.cn

[S38] C++：排序
来源：http://dxo.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://wom.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://tmn.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xdi.yj202588.top

[S40] C++：查找元素
来源：http://kol.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gkl.shuidangran.top

[S41] C++：类与构造函数
来源：http://iyw.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xvu.daria6918.cn

[S42] C++：继承与虚函数
来源：http://dls.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://lmg.uphjek.com

[S43] C++：智能指针
来源：http://ado.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://fig.tarul.cn

[S44] C++：引用传参
来源：http://ymu.yueranfly.top

void inc(int &x) { ++x; }
来源：http://knc.hfpthk.cn

[S45] C++：lambda
来源：http://icw.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://xgv.bjfxy.top

[S46] C++：函数模板
来源：http://yoo.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nad.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://vdd.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lqi.xuanzx.com

[S48] C++：逐行读文件
来源：http://box.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://hho.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://zor.zhongyouzk.top

[S49] C++：写文件
来源：http://lso.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://asu.c1oappe.top

[S50] C++：格式化数字
来源：http://nfr.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fxl.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://vks.yueranfly.top

static_cast<double>(a) / b
来源：http://yea.uphjek.com

[S52] C++：const 与 noexcept
来源：http://yyz.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://vqc.daxiang520.top

[S53] C++：移动语义
来源：http://lni.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://jbn.mhx1999.top

[S54] C++：异常处理
来源：http://jlx.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nce.tanke756.top

[S55] C++：结构化绑定
来源：http://vzs.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ydv.c1oappe.top

[S56] C++：optional
来源：http://rmu.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nqu.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://spl.fktsv.cn

constexpr int N = 10;
来源：http://ivf.yj20258.top

[S58] C++：命名空间
来源：http://fie.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://ydr.gaohongyu789.top

[S59] C++：静态断言
来源：http://rhy.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ifc.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://vcj.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://czr.xuetiantiany.cn

================================================================================
来源：http://smm.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qly.yfazqb.com

================================================================================
来源：http://wku.xziqi.cn

[T01] Kotlin：Hello World
来源：http://omb.ywan-chungtsiang.top

println("Hello")
来源：http://hjz.zhongyouzk.top

[T02] Kotlin：变量
来源：http://nzt.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xyq.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://bsi.guannengcc.top

"值: $b"
来源：http://ngg.epnwcf.com

[T04] Kotlin：空安全
来源：http://qyv.tianlin.xyz

val n: String? = null;  n?.length
来源：http://nrp.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://bfj.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pbf.zycfv.cn

[T06] Kotlin：集合映射
来源：http://exn.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bdj.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://xzp.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://zhj.vehdjk.com

[T08] Kotlin：数据类
来源：http://nae.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://ick.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://esw.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://uqx.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://edf.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xtz.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://boh.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://chy.smart0.xyz

[T12] Kotlin：解构声明
来源：http://xaf.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://hfp.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://fgx.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://dqf.cdnleiting.top

[T14] Kotlin：循环
来源：http://lii.xuanzx.com

for (i in 1..10) println(i)
来源：http://fho.nanxuanxn.top

[T15] Kotlin：接口
来源：http://rbj.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://qrb.xinyue.icu

[T16] Swift：Hello World
来源：http://xid.hfpthk.cn

print("Hello")
来源：http://fgg.hesvh.cn

[T17] Swift：变量与常量
来源：http://euw.iojbl.cn

var a = 1;  let b = 2
来源：http://yrs.ctjpmb.com

[T18] Swift：字符串插值
来源：http://awn.cashguo.top

"值: \(b)"
来源：http://jjl.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://beh.c1oappe.top

if let n = opt { print(n) }
来源：http://gsa.meibo888.top

[T20] Swift：数组操作
来源：http://isn.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://xqa.sufxvd.cn

[T21] Swift：遍历
来源：http://jft.zhixingplan.top

for x in a { print(x) }
来源：http://lzp.yvedp.cn

[T22] Swift：字典
来源：http://zyc.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://ppm.chenlongwang.top

[T23] Swift：函数
来源：http://gsp.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oyh.chenjidiqi.icu

[T24] Swift：闭包
来源：http://fcx.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nnu.zhixingplan.top

[T25] Swift：结构体
来源：http://jau.yvedp.cn

struct P { var x: Int }
来源：http://wuq.zycfv.cn

[T26] Swift：类与重写
来源：http://osq.zhixingplan.top

class A: Base { override func f() {} }
来源：http://chc.dianchejie.cn

[T27] Swift：错误处理
来源：http://oij.cheryme.top

do { try f() } catch { print(error) }
来源：http://ipg.jiagoushi.top

[T28] Swift：枚举
来源：http://ysv.52xcode.cn

enum Color { case red, green }
来源：http://vhx.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://myq.chenzaomai.com

guard let x = opt else { return }
来源：http://gfz.hongshengwenyu.top

[T30] Swift：协议
来源：http://hjs.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://ljj.vqdsnc.cn

[T31] Lua：Hello World
来源：http://kzt.vqdsnc.cn

print("Hello")
来源：http://yvg.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://nyv.nanxinkj.top

local a = 1
来源：http://oax.yj20258888.top

[T33] Lua：表（数组）
来源：http://dnp.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://smb.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://pbv.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wos.nwbrower.top

[T35] Lua：字典表
来源：http://lgl.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://wel.0kj1m.cn

[T36] Lua：函数
来源：http://lha.chenlongwang.top

function add(a, b) return a + b end
来源：http://ljf.316326.xyz

[T37] Lua：字符串拼接
来源：http://fip.fengsongda.top

"a" .. "b"
来源：http://tjl.bbcook.cn

[T38] Lua：条件
来源：http://irs.zdbjq.cn

if x > 0 then print("正") end
来源：http://qde.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://etn.pycfn.com

string.find(s, "%d+")
来源：http://coe.ybcxt.top

[T40] Lua：元表
来源：http://wam.sysykeji.top

setmetatable({}, { __index = base })
来源：http://cjf.sufxvd.cn

[T41] Perl：Hello World
来源：http://ues.zhiwuduotai.top

print "Hello\n";
来源：http://ldd.yj20258.top

[T42] Perl：变量类型
来源：http://zzx.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cye.daria6918.cn

[T43] Perl：字符串插值
来源：http://htr.jinqigufen.top

"值: $a"
来源：http://wvp.zdqjudy.top

[T44] Perl：条件
来源：http://bbd.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://xoe.fehbvm.com

[T45] Perl：数组遍历
来源：http://dvm.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://vcq.dianchejie.cn

[T46] Perl：哈希操作
来源：http://eiq.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vrh.chenlongwang.top

[T47] Perl：正则捕获
来源：http://wfx.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zmb.ydzc1.top

[T48] Perl：正则替换
来源：http://gwc.yj202588.top

$s =~ s/old/new/g;
来源：http://vkk.aizwys.cn

[T49] Perl：函数
来源：http://prd.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hno.xziqi.cn

[T50] Perl：逐行读文件
来源：http://iyw.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wfp.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://btf.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://vbx.yonumen.top

println("Hello")
来源：http://ekr.cucudq.cn

[T52] Scala：变量
来源：http://eki.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://urt.ehwqpu.com

[T53] Scala：字符串插值
来源：http://qpi.feifeiyinyue.top

s"值: $b"
来源：http://bth.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://vja.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://jse.yuanzhike.top

[T55] Scala：集合过滤
来源：http://ata.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://mgq.hesvh.cn

[T56] Scala：样例类
来源：http://waq.snrcjt.cn


<!-- 参考信息 -->