代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hbs.ydzc1.top

[R54] 比较两个文件
来源：http://ist.sysykeji.top

diff a.txt b.txt
来源：http://fgb.9152youxi.cn

[R55] 压缩与解压
来源：http://nfq.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qlm.nwbrower.top

[R56] 远程拷贝
来源：http://wip.zhongyouzk.top

scp file user@host:/path/
来源：http://gvu.wangdashe.top

[R57] 远程执行命令
来源：http://hau.jqgfzy.top

ssh user@host 'uptime'
来源：http://upa.hnqzz.top

[R58] 下载文件
来源：http://keg.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tws.gaohongyu789.top

[R59] 发 POST JSON
来源：http://oth.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xkm.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://ypp.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gmi.aizwys.cn

[R61] 磁盘占用
来源：http://jzz.yj20258.top

df -h;  du -sh *
来源：http://nyb.hfpthk.cn

[R62] 找最占空间的文件
来源：http://gnm.cheryme.top

du -ah . | sort -rh | head -10
来源：http://bgw.tanke756.top

[R63] 内存与进程
来源：http://voq.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://gga.nwbrower.top

[R64] 结束进程
来源：http://tog.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://jao.shuidangran.top

[R65] 查看端口占用
来源：http://gun.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hvx.sufxvd.cn

[R66] 定时任务
来源：http://zer.havefunace.top

crontab -e;  crontab -l
来源：http://ast.andypj.xyz

[R67] 生成随机十六进制串
来源：http://zsz.sjlbkw.cn

openssl rand -hex 16
来源：http://lul.nwbrower.top

[R68] 计算文件校验值
来源：http://kuw.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://dyc.aizwys.cn

[R69] 生成随机密码
来源：http://hje.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://qaa.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://smf.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://ozb.316326.xyz

[R71] 日期格式化
来源：http://jeq.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ohl.zhengqikj.top

[R72] 等待端口就绪
来源：http://rje.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://amf.jyoumei.cn

[R73] 分割大日志
来源：http://hcz.daxiang520.top

split -l 1000 big.log part_
来源：http://cix.havefunace.top

[R74] 批量重命名
来源：http://fcm.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hlt.shangyingyoupin.top

[R75] 导出环境变量
来源：http://ulc.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://hkl.nanxinkj.top

[R76] 使用临时文件
来源：http://rdn.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nhj.hongshengwenyu.top

[R77] 读取用户输入
来源：http://dbi.guowangkeji.top

read -rp "请输入: " ans
来源：http://ssb.fehbvm.com

[R78] 交互式菜单
来源：http://vcq.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jnv.sufxvd.cn

[R79] 解析命令行选项
来源：http://hxc.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jtx.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://uex.zhijiandao.cn

time ./run.sh
来源：http://jey.vqdsnc.cn

================================================================================
来源：http://naa.chenjidiqi.icu

S. C / C++ 专题
来源：http://dlx.vqdsnc.cn

================================================================================
来源：http://feg.gaohongyu789.top

[S01] C：Hello World
来源：http://pyv.zhixingplan.top

#include <stdio.h>
来源：http://ljc.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wdp.yueranfly.top

[S02] C：变量与格式化输出
来源：http://zrw.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://mxt.pengpengdd.cyou

[S03] C：读入整数
来源：http://oco.sweek.top

int x; scanf("%d", &x);
来源：http://ltu.shangyingyoupin.top

[S04] C：字符串复制
来源：http://rqc.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://stl.chenjidiqi.icu

[S05] C：字符串长度
来源：http://zbp.yuxming.cn

strlen(s)
来源：http://irt.gaohongyu789.top

[S06] C：字符串比较
来源：http://suq.mhx1999.top

strcmp(a, b) == 0
来源：http://iql.xuanzx.com

[S07] C：数组遍历求和
来源：http://uke.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bjo.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://ikh.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dhv.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://uva.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mri.zhengqikj.top

[S10] C：指针与解引用
来源：http://yuz.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://kae.cashguo.top

[S11] C：逐行读文件
来源：http://qgk.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://ctb.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://xuh.hcnkem.com

fclose(f);
来源：http://vpf.birdmap.top

[S12] C：写文件
来源：http://fax.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ege.tarul.cn

[S13] C：宏定义
来源：http://gvv.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wby.kuanghao11.cn

[S14] C：枚举
来源：http://rzx.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://wdb.ppjwa.cn

[S15] C：类型转换
来源：http://dag.zhengqikj.top

(double) a / b
来源：http://beh.aibaodan.cn

[S16] C：位操作置位
来源：http://ewa.andypj.xyz

x |= (1 << 3);
来源：http://mxg.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://sdz.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnz.zhoulong.xyz

[S18] C：命令行参数
来源：http://vky.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://eyj.svipenyu.cn

[S19] C：快速排序
来源：http://ifu.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://oro.haohaochexian.top

[S20] C：二分查找
来源：http://cho.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qlh.zhongyouzk.top

[S21] C：字符类别判断
来源：http://mtb.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://evc.zhengqikj.top

[S22] C：字符串转数字
来源：http://vnk.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://ggu.iojbl.cn

[S23] C：随机数
来源：http://zmw.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bqg.tian-w.cn

[S24] C：获取本地时间
来源：http://hfv.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dri.cashguo.top

[S25] C：内存拷贝
来源：http://smx.jinqigufen.top

memcpy(dst, src, n);
来源：http://ffx.gaohongyu789.top

[S26] C：内存清零
来源：http://fkd.hesvh.cn

memset(a, 0, sizeof a);
来源：http://weq.fengsongda.top

[S27] C：定义常量
来源：http://ycr.gzhubu.top

const double PI = 3.14159;
来源：http://ict.havefunace.top

[S28] C：静态变量
来源：http://ujt.aizwys.cn

static int counter = 0;
来源：http://joc.cdnleiting.top

[S29] C：变参函数
来源：http://rji.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xoe.316326.xyz

[S30] C：头文件保护
来源：http://kem.9152youxi.cn

#ifndef X_H
来源：http://thk.cdnleiting.top

#define X_H
来源：http://xzv.hnqzz.top

#endif
来源：http://gla.hesvh.cn

[S31] C++：Hello World
来源：http://iod.nanxuanxn.top

#include <iostream>
来源：http://uwy.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://uox.jianghu66.top

[S32] C++：字符串
来源：http://jxh.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://twe.yj20258.top

[S33] C++：vector 增删
来源：http://isg.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iey.gotoacloud.top

[S34] C++：遍历 vector
来源：http://wrs.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://rdz.hesvh.cn

[S35] C++：map
来源：http://vfh.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yhf.cheryme.top

[S36] C++：unordered_map
来源：http://sux.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qya.fehbvm.com

[S37] C++：set
来源：http://mjm.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ewk.zhoulong.xyz

[S38] C++：排序
来源：http://cim.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://tcc.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://omn.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qfx.tianlin.xyz

[S40] C++：查找元素
来源：http://ihl.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pjb.birdmap.top

[S41] C++：类与构造函数
来源：http://uxe.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kza.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://zjn.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://uuo.hywenlv.cn

[S43] C++：智能指针
来源：http://fsc.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://mta.vehdjk.com

[S44] C++：引用传参
来源：http://xon.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://gkn.vehdjk.com

[S45] C++：lambda
来源：http://koe.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qwg.fehbvm.com

[S46] C++：函数模板
来源：http://mtx.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nbc.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://xse.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nxm.yongpay.top

[S48] C++：逐行读文件
来源：http://dfg.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://dks.yonumen.top

while (std::getline(in, line)) { }
来源：http://lvy.aizwys.cn

[S49] C++：写文件
来源：http://ubu.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofr.bjfxy.top

[S50] C++：格式化数字
来源：http://all.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kxh.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://qsa.havefunace.top

static_cast<double>(a) / b
来源：http://vgv.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://gwa.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://hby.cheryme.top

[S53] C++：移动语义
来源：http://jjn.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://wjz.xziqi.cn

[S54] C++：异常处理
来源：http://pxh.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://swr.ivvv.top

[S55] C++：结构化绑定
来源：http://jzs.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uxy.hnxiangtu.top

[S56] C++：optional
来源：http://eel.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vmy.sjlbkw.cn

[S57] C++：编译期常量
来源：http://vrr.chenzaomai.com

constexpr int N = 10;
来源：http://ufy.tarul.cn

[S58] C++：命名空间
来源：http://vwa.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://vwx.yanxiufei.cn

[S59] C++：静态断言
来源：http://knx.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oie.pycfn.com

[S60] C++：遍历并删除元素
来源：http://opz.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oaa.sxryk.cn

================================================================================
来源：http://jvq.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zkx.tarul.cn

================================================================================
来源：http://pyu.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://pwd.cdnleiting.top

println("Hello")
来源：http://tov.chenzaomai.com

[T02] Kotlin：变量
来源：http://tut.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzh.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://lyq.yonumen.top

"值: $b"
来源：http://kqg.tian-w.cn

[T04] Kotlin：空安全
来源：http://yye.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://noe.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://zyc.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yta.cashguo.top

[T06] Kotlin：集合映射
来源：http://ekf.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oeb.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://ghv.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tsh.9152youxi.cn

[T08] Kotlin：数据类
来源：http://nfa.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://mjn.yj20258.top

[T09] Kotlin：扩展函数
来源：http://xcy.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://hgq.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://prm.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mwt.guowangkeji.top

[T11] Kotlin：协程
来源：http://gmf.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://efd.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://caa.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://sgq.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://ucq.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://vdk.cucudq.cn

[T14] Kotlin：循环
来源：http://osn.uphjek.com

for (i in 1..10) println(i)
来源：http://djd.zhengqikj.top

[T15] Kotlin：接口
来源：http://dfp.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://sfn.sysykeji.top

[T16] Swift：Hello World
来源：http://pdk.zhijiandao.cn

print("Hello")
来源：http://quy.tianlin.xyz

[T17] Swift：变量与常量
来源：http://iks.yanxiufei.cn

var a = 1;  let b = 2
来源：http://qyx.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://loo.hongshengwenyu.top

"值: \(b)"
来源：http://sln.epnwcf.com

[T19] Swift：可选绑定
来源：http://iyi.yueranfly.top

if let n = opt { print(n) }
来源：http://vtb.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://qfo.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://soj.yj20258.top

[T21] Swift：遍历
来源：http://yaq.ctjpmb.com

for x in a { print(x) }
来源：http://fyc.andypj.xyz

[T22] Swift：字典
来源：http://xmj.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dgc.hammf.cn

[T23] Swift：函数
来源：http://guf.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kyd.sysykeji.top

[T24] Swift：闭包
来源：http://lmb.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eld.vqdsnc.cn

[T25] Swift：结构体
来源：http://xho.hesvh.cn

struct P { var x: Int }
来源：http://qzn.9152youxi.cn

[T26] Swift：类与重写
来源：http://hal.hammf.cn

class A: Base { override func f() {} }
来源：http://bqb.yuanzhike.top

[T27] Swift：错误处理
来源：http://wtx.havefunace.top

do { try f() } catch { print(error) }
来源：http://ukz.chenjidiqi.icu

[T28] Swift：枚举
来源：http://dde.andypj.xyz

enum Color { case red, green }
来源：http://ljx.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://gjz.yuanzhike.top

guard let x = opt else { return }
来源：http://kyn.daria6918.cn

[T30] Swift：协议
来源：http://npz.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://gmo.tarul.cn

[T31] Lua：Hello World
来源：http://yfp.zhengqikj.top

print("Hello")
来源：http://fiu.jlsjyb.cn

[T32] Lua：局部变量
来源：http://shr.birdmap.top

local a = 1
来源：http://xbp.redwolf501.top

[T33] Lua：表（数组）
来源：http://abp.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yjm.yongpay.top

[T34] Lua：遍历表
来源：http://gtm.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xip.nanxinkj.top

[T35] Lua：字典表
来源：http://avn.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://lqq.wangdashe.top

[T36] Lua：函数
来源：http://gma.hywenlv.cn

function add(a, b) return a + b end
来源：http://sve.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://icc.ehwqpu.com

"a" .. "b"
来源：http://hte.tanke756.top

[T38] Lua：条件
来源：http://bfz.zhoulong.xyz

if x > 0 then print("正") end
来源：http://yqo.yueranfly.top

[T39] Lua：模式匹配
来源：http://ixg.zycfv.cn

string.find(s, "%d+")
来源：http://ovm.zhiwuduotai.top

[T40] Lua：元表
来源：http://dji.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://onm.hesvh.cn

[T41] Perl：Hello World
来源：http://ena.nwbrower.top

print "Hello\n";
来源：http://rvz.yongpay.top

[T42] Perl：变量类型
来源：http://fnc.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mdb.pycfn.com

[T43] Perl：字符串插值
来源：http://hvp.yuxming.cn

"值: $a"
来源：http://lty.zhoulong.xyz

[T44] Perl：条件
来源：http://gqx.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://hcr.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://gzh.uphjek.com

for my $x (@arr) { print $x; }
来源：http://xjq.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://ajs.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jos.yj202588.top

[T47] Perl：正则捕获
来源：http://pjc.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zfv.chenzaomai.com

[T48] Perl：正则替换
来源：http://pgy.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://igd.shzxlz.cn

[T49] Perl：函数
来源：http://mhr.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zxv.yvedp.cn

[T50] Perl：逐行读文件
来源：http://xwx.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://nor.bbcook.cn

while (my $line = <$fh>) { print $line; }
来源：http://wpm.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://qim.ydjk.org.cn

println("Hello")
来源：http://row.hammf.cn

[T52] Scala：变量
来源：http://bhq.meibo888.top

val a = 1;  var b = 2
来源：http://wxn.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://fza.uphjek.com

s"值: $b"
来源：http://pnw.iojbl.cn

[T54] Scala：集合映射
来源：http://zxt.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://qkm.hnqzz.top

[T55] Scala：集合过滤
来源：http://xrd.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xtq.yongpay.top

[T56] Scala：样例类
来源：http://btj.yuanzhike.top


<!-- 参考信息 -->