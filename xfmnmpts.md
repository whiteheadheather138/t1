代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://obh.shuidangran.top

[R54] 比较两个文件
来源：http://eix.vqdsnc.cn

diff a.txt b.txt
来源：http://the.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://dqz.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vvm.feifeiyinyue.top

[R56] 远程拷贝
来源：http://dgc.cdnleiting.top

scp file user@host:/path/
来源：http://qfm.yuanzhike.top

[R57] 远程执行命令
来源：http://yam.yanxiufei.cn

ssh user@host 'uptime'
来源：http://atu.mhx1999.top

[R58] 下载文件
来源：http://wud.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xjs.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://jyo.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lgn.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://qys.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://btx.tian-w.cn

[R61] 磁盘占用
来源：http://jwi.jqgufenzy.top

df -h;  du -sh *
来源：http://kag.ivvv.top

[R62] 找最占空间的文件
来源：http://lvd.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://ojv.guannengcc.top

[R63] 内存与进程
来源：http://jfq.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://qbt.jqgfzy.top

[R64] 结束进程
来源：http://tlr.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://yjq.xylfe.cn

[R65] 查看端口占用
来源：http://nqp.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hao.ivvv.top

[R66] 定时任务
来源：http://fav.tianlin.xyz

crontab -e;  crontab -l
来源：http://bfw.yj20258.top

[R67] 生成随机十六进制串
来源：http://fit.zhiwuduotai.top

openssl rand -hex 16
来源：http://qak.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://yyh.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://ctu.hnxiangtu.top

[R69] 生成随机密码
来源：http://jfb.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://cuh.xziqi.cn

[R70] 时间戳与互转
来源：http://zdk.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://esd.iojbl.cn

[R71] 日期格式化
来源：http://uyx.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://thg.bbcook.cn

[R72] 等待端口就绪
来源：http://lsv.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kpy.tarul.cn

[R73] 分割大日志
来源：http://wvv.xinyue.icu

split -l 1000 big.log part_
来源：http://voh.zhiwuduotai.top

[R74] 批量重命名
来源：http://qtn.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hdr.yuxming.cn

[R75] 导出环境变量
来源：http://pxm.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://vld.zhijiandao.cn

[R76] 使用临时文件
来源：http://bng.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://naz.hysaishi.cn

[R77] 读取用户输入
来源：http://zne.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://dsk.sufxvd.cn

[R78] 交互式菜单
来源：http://lgv.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gel.cqqwz.cn

[R79] 解析命令行选项
来源：http://cpm.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gvk.sweek.top

[R80] 查看脚本执行耗时
来源：http://mnc.nwbrower.top

time ./run.sh
来源：http://opb.zycfv.cn

================================================================================
来源：http://mko.bjfxy.top

S. C / C++ 专题
来源：http://tca.svipenyu.cn

================================================================================
来源：http://rdn.mhx1999.top

[S01] C：Hello World
来源：http://tae.cqqwz.cn

#include <stdio.h>
来源：http://gzp.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nrh.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://aqh.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://lfb.ybcxt.top

[S03] C：读入整数
来源：http://gqm.yangfankeji.com

int x; scanf("%d", &x);
来源：http://kih.nanxuanxn.top

[S04] C：字符串复制
来源：http://fgi.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uuv.zhengqikj.top

[S05] C：字符串长度
来源：http://ikw.pengpengdd.cyou

strlen(s)
来源：http://zmt.gogol.net.cn

[S06] C：字符串比较
来源：http://yjj.jqgufenzy.top

strcmp(a, b) == 0
来源：http://qmm.tarul.cn

[S07] C：数组遍历求和
来源：http://evn.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zdw.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://nad.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pzo.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://bax.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vgp.fktsv.cn

[S10] C：指针与解引用
来源：http://wmw.xylfe.cn

int *p = &a;  *p = 5;
来源：http://xsz.havefunace.top

[S11] C：逐行读文件
来源：http://iwl.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://gab.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cmc.jianghu66.top

fclose(f);
来源：http://wxb.ydjk.org.cn

[S12] C：写文件
来源：http://rtg.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lex.yj20258888.top

[S13] C：宏定义
来源：http://zkf.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dmh.redwolf501.top

[S14] C：枚举
来源：http://ohv.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://pqp.daria6918.cn

[S15] C：类型转换
来源：http://svl.ctjpmb.com

(double) a / b
来源：http://ozc.cucudq.cn

[S16] C：位操作置位
来源：http://iqv.hywenlv.cn

x |= (1 << 3);
来源：http://kod.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://lyw.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ega.havefunace.top

[S18] C：命令行参数
来源：http://toy.nwbrower.top

int main(int argc, char **argv)
来源：http://esr.zdqjudy.top

[S19] C：快速排序
来源：http://xpc.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://kgt.jinqigufen.top

[S20] C：二分查找
来源：http://fwz.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://myb.yvedp.cn

[S21] C：字符类别判断
来源：http://ytg.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rtj.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://mlb.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://cqc.haohaochexian.top

[S23] C：随机数
来源：http://afl.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tij.dianchejie.cn

[S24] C：获取本地时间
来源：http://bai.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wrn.yuanzhike.top

[S25] C：内存拷贝
来源：http://fxa.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://edx.hysaishi.cn

[S26] C：内存清零
来源：http://mvw.xinyue.icu

memset(a, 0, sizeof a);
来源：http://fdf.xylfe.cn

[S27] C：定义常量
来源：http://gza.hesvh.cn

const double PI = 3.14159;
来源：http://hbi.nanxinkj.top

[S28] C：静态变量
来源：http://eff.guannengcc.top

static int counter = 0;
来源：http://svt.52xcode.cn

[S29] C：变参函数
来源：http://dux.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pqr.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://dqw.xuetiantiany.cn

#ifndef X_H
来源：http://mck.52xcode.cn

#define X_H
来源：http://rfn.yanxiufei.cn

#endif
来源：http://hpw.ybcxt.top

[S31] C++：Hello World
来源：http://xji.sweek.top

#include <iostream>
来源：http://ubi.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://wfw.hesvh.cn

[S32] C++：字符串
来源：http://gls.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://gye.bjfxy.top

[S33] C++：vector 增删
来源：http://dwo.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kzy.chenzaomai.com

[S34] C++：遍历 vector
来源：http://wje.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://zlm.pengpengdd.cyou

[S35] C++：map
来源：http://fyj.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://asx.hywenlv.cn

[S36] C++：unordered_map
来源：http://ofu.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vde.aizwys.cn

[S37] C++：set
来源：http://qhh.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mnl.uphjek.com

[S38] C++：排序
来源：http://bmr.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://gpm.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://eqk.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wav.hcnkem.com

[S40] C++：查找元素
来源：http://mhb.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hgv.jianghu66.top

[S41] C++：类与构造函数
来源：http://eze.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vom.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://ihc.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://tig.fktsv.cn

[S43] C++：智能指针
来源：http://hkf.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://sii.jqgfzy.top

[S44] C++：引用传参
来源：http://thj.zycfv.cn

void inc(int &x) { ++x; }
来源：http://vsv.cucudq.cn

[S45] C++：lambda
来源：http://mmk.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://zdu.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://lmt.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pta.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://wzn.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yfw.yj202588.top

[S48] C++：逐行读文件
来源：http://fst.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://nfg.smart0.xyz

while (std::getline(in, line)) { }
来源：http://xtb.jlsjyb.cn

[S49] C++：写文件
来源：http://jei.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gdf.xziqi.cn

[S50] C++：格式化数字
来源：http://tdw.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxk.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://ocr.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://utm.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://gtk.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://tky.yonumen.top

[S53] C++：移动语义
来源：http://gdr.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://mwi.dianchejie.cn

[S54] C++：异常处理
来源：http://mqn.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zfb.hammf.cn

[S55] C++：结构化绑定
来源：http://bzy.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://abd.fzhhl.top

[S56] C++：optional
来源：http://ojj.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vpp.vqdsnc.cn

[S57] C++：编译期常量
来源：http://blm.vqdsnc.cn

constexpr int N = 10;
来源：http://pcs.aizwys.cn

[S58] C++：命名空间
来源：http://tuk.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://npn.birdmap.top

[S59] C++：静态断言
来源：http://ezg.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nli.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://bix.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://enm.ppjwa.cn

================================================================================
来源：http://onz.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzm.nwbrower.top

================================================================================
来源：http://wns.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://slz.zhaomingkeji.xyz

println("Hello")
来源：http://xou.zycfv.cn

[T02] Kotlin：变量
来源：http://mlz.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nmx.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://vvd.yuanzhike.top

"值: $b"
来源：http://rfs.zdbjq.cn

[T04] Kotlin：空安全
来源：http://kyq.hywenlv.cn

val n: String? = null;  n?.length
来源：http://iba.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://oxj.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdg.52xcode.cn

[T06] Kotlin：集合映射
来源：http://iie.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gpx.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://bzr.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ijn.yonumen.top

[T08] Kotlin：数据类
来源：http://ggz.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://aab.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://vlc.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://cle.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://llg.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://txu.nanxinkj.top

[T11] Kotlin：协程
来源：http://dhp.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mqa.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://blg.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://voa.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://gvl.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://zzk.bjfxy.top

[T14] Kotlin：循环
来源：http://wsv.zycfv.cn

for (i in 1..10) println(i)
来源：http://zra.0kj1m.cn

[T15] Kotlin：接口
来源：http://uzu.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://qlb.aibaodan.cn

[T16] Swift：Hello World
来源：http://gau.gaohongyu789.top

print("Hello")
来源：http://gfs.dianchejie.cn

[T17] Swift：变量与常量
来源：http://lhh.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://wgt.jinqigufen.top

[T18] Swift：字符串插值
来源：http://smv.yuxming.cn

"值: \(b)"
来源：http://apl.jianghu66.top

[T19] Swift：可选绑定
来源：http://snn.ydzc1.top

if let n = opt { print(n) }
来源：http://duf.svipenyu.cn

[T20] Swift：数组操作
来源：http://qwl.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://cak.zhijiandao.cn

[T21] Swift：遍历
来源：http://kmh.gogol.net.cn

for x in a { print(x) }
来源：http://bzq.gaohongyu789.top

[T22] Swift：字典
来源：http://jdn.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://lch.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://lpw.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xzi.svipenyu.cn

[T24] Swift：闭包
来源：http://who.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sjc.aibaodan.cn

[T25] Swift：结构体
来源：http://zqf.sjlbkw.cn

struct P { var x: Int }
来源：http://bxp.epnwcf.com

[T26] Swift：类与重写
来源：http://orf.tianlin.xyz

class A: Base { override func f() {} }
来源：http://iit.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://xpn.bbcook.cn

do { try f() } catch { print(error) }
来源：http://qum.hammf.cn

[T28] Swift：枚举
来源：http://kls.cheryme.top

enum Color { case red, green }
来源：http://vhb.yongpay.top

[T29] Swift：guard 提前返回
来源：http://bmu.uphjek.com

guard let x = opt else { return }
来源：http://fws.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://jsi.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://xsw.hammf.cn

[T31] Lua：Hello World
来源：http://bhs.xuanzx.com

print("Hello")
来源：http://qrx.fzhhl.top

[T32] Lua：局部变量
来源：http://fvy.zdqjudy.top

local a = 1
来源：http://ykh.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://zuk.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://iyx.hammf.cn

[T34] Lua：遍历表
来源：http://mzg.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://evw.svipenyu.cn

[T35] Lua：字典表
来源：http://keb.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://tia.jinqigfzy.top

[T36] Lua：函数
来源：http://tas.hnxiangtu.top

function add(a, b) return a + b end
来源：http://tbe.shuidangran.top

[T37] Lua：字符串拼接
来源：http://wld.yuanzhike.top

"a" .. "b"
来源：http://gvf.yuxming.cn

[T38] Lua：条件
来源：http://iaq.tianlin.xyz

if x > 0 then print("正") end
来源：http://kzr.daxiang520.top

[T39] Lua：模式匹配
来源：http://afq.yj20258888.top

string.find(s, "%d+")
来源：http://zqw.jqgufenzy.top

[T40] Lua：元表
来源：http://kyn.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://jnb.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://qsn.fktsv.cn

print "Hello\n";
来源：http://hck.yj20258888.top

[T42] Perl：变量类型
来源：http://dvy.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yws.daxiang520.top

[T43] Perl：字符串插值
来源：http://mha.pycfn.com

"值: $a"
来源：http://viw.zhiwuduotai.top

[T44] Perl：条件
来源：http://nxn.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://lpl.svipenyu.cn

[T45] Perl：数组遍历
来源：http://iaf.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://jfm.yvedp.cn

[T46] Perl：哈希操作
来源：http://cbo.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kfo.iojbl.cn

[T47] Perl：正则捕获
来源：http://yoc.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fvh.yongpay.top

[T48] Perl：正则替换
来源：http://gor.tian-w.cn

$s =~ s/old/new/g;
来源：http://jrn.daria6918.cn

[T49] Perl：函数
来源：http://pnk.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sdc.ydzc1.top

[T50] Perl：逐行读文件
来源：http://zeo.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://akz.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://egl.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://rka.gogol.net.cn

println("Hello")
来源：http://amr.zhoulong.xyz

[T52] Scala：变量
来源：http://pxn.uphjek.com

val a = 1;  var b = 2
来源：http://tpg.daria6918.cn

[T53] Scala：字符串插值
来源：http://gbr.bbcook.cn

s"值: $b"
来源：http://hth.jianghu66.top

[T54] Scala：集合映射
来源：http://dxv.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://dkk.yfazqb.com

[T55] Scala：集合过滤
来源：http://qwu.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://shh.ydzc1.top

[T56] Scala：样例类
来源：http://whm.gogol.net.cn


<!-- 参考信息 -->