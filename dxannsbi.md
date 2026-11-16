代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dzi.nwbrower.top

[R56] 远程拷贝
来源：http://nsz.yfazqb.com

scp file user@host:/path/
来源：http://tal.sxryk.cn

[R57] 远程执行命令
来源：http://zgg.gaohongyu789.top

ssh user@host 'uptime'
来源：http://zti.daxiang520.top

[R58] 下载文件
来源：http://rcu.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jhy.kuanghao11.cn

[R59] 发 POST JSON
来源：http://yhs.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uks.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://crx.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://toi.hfpthk.cn

[R61] 磁盘占用
来源：http://rep.hywenlv.cn

df -h;  du -sh *
来源：http://lwa.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://shi.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://xve.hywenlv.cn

[R63] 内存与进程
来源：http://nlm.tanke756.top

free -h;  ps aux | grep nginx
来源：http://tuh.yangfankeji.com

[R64] 结束进程
来源：http://hlu.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://fcp.yuanzhike.top

[R65] 查看端口占用
来源：http://dqq.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jdl.zhongyouzk.top

[R66] 定时任务
来源：http://jxr.xziqi.cn

crontab -e;  crontab -l
来源：http://fog.yj20258.top

[R67] 生成随机十六进制串
来源：http://anq.hnxiangtu.top

openssl rand -hex 16
来源：http://otm.sxryk.cn

[R68] 计算文件校验值
来源：http://txl.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tbp.xylfe.cn

[R69] 生成随机密码
来源：http://qjf.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://aza.tianlin.xyz

[R70] 时间戳与互转
来源：http://zru.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://lhc.xuanzx.com

[R71] 日期格式化
来源：http://btu.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zxc.shzxlz.cn

[R72] 等待端口就绪
来源：http://rbj.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cpo.ctjpmb.com

[R73] 分割大日志
来源：http://dmi.hysaishi.cn

split -l 1000 big.log part_
来源：http://ygc.daxiang520.top

[R74] 批量重命名
来源：http://xsq.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qnj.hnxiangtu.top

[R75] 导出环境变量
来源：http://iju.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://nvt.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://xot.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://joc.daxiang520.top

[R77] 读取用户输入
来源：http://iua.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://qhg.tianlin.xyz

[R78] 交互式菜单
来源：http://kuo.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sgl.chenzaomai.com

[R79] 解析命令行选项
来源：http://xxq.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xvh.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://uru.jiagoushi.top

time ./run.sh
来源：http://ytq.cashguo.top

================================================================================
来源：http://uzz.sxryk.cn

S. C / C++ 专题
来源：http://ewi.jinyuanbaomall.cn

================================================================================
来源：http://ufi.cucudq.cn

[S01] C：Hello World
来源：http://sxm.jqgfzy.top

#include <stdio.h>
来源：http://nlg.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iox.bbcook.cn

[S02] C：变量与格式化输出
来源：http://mrn.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://hdr.fzhhl.top

[S03] C：读入整数
来源：http://tsg.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://dkn.dashuyun.cn

[S04] C：字符串复制
来源：http://qxg.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rbc.mhx1999.top

[S05] C：字符串长度
来源：http://yca.vqdsnc.cn

strlen(s)
来源：http://lrq.zhiwuduotai.top

[S06] C：字符串比较
来源：http://gzd.bjfxy.top

strcmp(a, b) == 0
来源：http://bhx.nwbrower.top

[S07] C：数组遍历求和
来源：http://phc.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://har.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://tia.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lyg.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://kob.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wzc.jinqigufen.top

[S10] C：指针与解引用
来源：http://yda.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://pln.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://bib.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://jpz.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dap.zdqjudy.top

fclose(f);
来源：http://vag.meibo888.top

[S12] C：写文件
来源：http://ypp.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mrp.ivvv.top

[S13] C：宏定义
来源：http://hub.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hlr.shanyushiyangtech.top

[S14] C：枚举
来源：http://oes.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://nop.yj20258888.top

[S15] C：类型转换
来源：http://ecp.gotoacloud.top

(double) a / b
来源：http://wof.jqgufenzy.top

[S16] C：位操作置位
来源：http://jvb.fanxiaobao.xyz

x |= (1 << 3);
来源：http://pmq.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://rqv.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rjz.zhiwuduotai.top

[S18] C：命令行参数
来源：http://lef.c1oappe.top

int main(int argc, char **argv)
来源：http://npl.xuetiantiany.cn

[S19] C：快速排序
来源：http://ylo.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://utb.smart0.xyz

[S20] C：二分查找
来源：http://zpn.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lyu.nwbrower.top

[S21] C：字符类别判断
来源：http://uzr.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qin.meibo888.top

[S22] C：字符串转数字
来源：http://iny.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rcw.shangyingyoupin.top

[S23] C：随机数
来源：http://qyq.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wei.birdmap.top

[S24] C：获取本地时间
来源：http://sdr.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yji.hysaishi.cn

[S25] C：内存拷贝
来源：http://tkc.dianchejie.cn

memcpy(dst, src, n);
来源：http://zfu.zdbjq.cn

[S26] C：内存清零
来源：http://mws.yvedp.cn

memset(a, 0, sizeof a);
来源：http://xdr.dianchejie.cn

[S27] C：定义常量
来源：http://ajv.ivvv.top

const double PI = 3.14159;
来源：http://bwv.haohaochexian.top

[S28] C：静态变量
来源：http://imh.hcnkem.com

static int counter = 0;
来源：http://nrl.wangshuangyany.cn

[S29] C：变参函数
来源：http://fzy.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zgb.snrcjt.cn

[S30] C：头文件保护
来源：http://ffe.vqdsnc.cn

#ifndef X_H
来源：http://wvp.redwolf501.top

#define X_H
来源：http://vdk.gogol.net.cn

#endif
来源：http://lsi.fzhhl.top

[S31] C++：Hello World
来源：http://kzb.bjfxy.top

#include <iostream>
来源：http://hkp.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://fzx.tanke756.top

[S32] C++：字符串
来源：http://ikv.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://kcx.bbcook.cn

[S33] C++：vector 增删
来源：http://ekw.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jil.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://nss.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://fnb.ehwqpu.com

[S35] C++：map
来源：http://ozr.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lbl.zdbjq.cn

[S36] C++：unordered_map
来源：http://xyx.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qlo.ppjwa.cn

[S37] C++：set
来源：http://oxa.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tll.zhengqikj.top

[S38] C++：排序
来源：http://qui.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://dlb.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://szu.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lkp.52xcode.cn

[S40] C++：查找元素
来源：http://znw.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lur.cashguo.top

[S41] C++：类与构造函数
来源：http://vyl.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tyc.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://idp.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://xsl.zhiwuduotai.top

[S43] C++：智能指针
来源：http://rzf.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://scz.tarul.cn

[S44] C++：引用传参
来源：http://rvn.pycfn.com

void inc(int &x) { ++x; }
来源：http://ivb.cucudq.cn

[S45] C++：lambda
来源：http://zzm.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ddn.yuanzhike.top

[S46] C++：函数模板
来源：http://yvn.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mqz.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://aqv.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyt.jianghu66.top

[S48] C++：逐行读文件
来源：http://hxa.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://inr.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://uet.jiagoushi.top

[S49] C++：写文件
来源：http://lvq.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://not.sxryk.cn

[S50] C++：格式化数字
来源：http://ryd.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lhx.hfpthk.cn

[S51] C++：显式类型转换
来源：http://iud.gogol.net.cn

static_cast<double>(a) / b
来源：http://nit.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://arh.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://eyq.chenlongwang.top

[S53] C++：移动语义
来源：http://ift.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://ccb.zhiwuduotai.top

[S54] C++：异常处理
来源：http://vyh.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xjn.xuanzx.com

[S55] C++：结构化绑定
来源：http://roi.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jxs.nwbrower.top

[S56] C++：optional
来源：http://znj.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ism.hnxiangtu.top

[S57] C++：编译期常量
来源：http://pry.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://cmm.snrcjt.cn

[S58] C++：命名空间
来源：http://rnw.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://nsj.hywenlv.cn

[S59] C++：静态断言
来源：http://mfg.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jch.meibo888.top

[S60] C++：遍历并删除元素
来源：http://agf.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yup.mhx1999.top

================================================================================
来源：http://cag.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jpg.bbcook.cn

================================================================================
来源：http://rzq.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://bip.birdmap.top

println("Hello")
来源：http://xfm.zhengqikj.top

[T02] Kotlin：变量
来源：http://whq.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ysm.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://mve.c1oappe.top

"值: $b"
来源：http://uay.jinqigufen.top

[T04] Kotlin：空安全
来源：http://zqw.hfpthk.cn

val n: String? = null;  n?.length
来源：http://sxh.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://ezm.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://urw.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://wmc.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oss.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://ynn.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ehm.haohaochexian.top

[T08] Kotlin：数据类
来源：http://cpe.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://wng.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://yto.meibo888.top

fun String.exclaim() = this + "!"
来源：http://cjg.cashguo.top

[T10] Kotlin：默认参数
来源：http://jte.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gua.sysykeji.top

[T11] Kotlin：协程
来源：http://rfa.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zzq.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://tbp.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://ius.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://prd.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://kmh.kuanghao11.cn

[T14] Kotlin：循环
来源：http://esm.tianlin.xyz

for (i in 1..10) println(i)
来源：http://jnt.ctjpmb.com

[T15] Kotlin：接口
来源：http://quw.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://dxl.hnqzz.top

[T16] Swift：Hello World
来源：http://ntp.yongpay.top

print("Hello")
来源：http://sbs.vehdjk.com

[T17] Swift：变量与常量
来源：http://ydn.fehbvm.com

var a = 1;  let b = 2
来源：http://ize.yongpay.top

[T18] Swift：字符串插值
来源：http://rfm.xuetiantiany.cn

"值: \(b)"
来源：http://fqv.guowangkeji.top

[T19] Swift：可选绑定
来源：http://kad.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://tam.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://iyz.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://bos.yanxiufei.cn

[T21] Swift：遍历
来源：http://jug.yuanzhike.top

for x in a { print(x) }
来源：http://qrz.shangyingyoupin.top

[T22] Swift：字典
来源：http://mxz.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ixg.zycfv.cn

[T23] Swift：函数
来源：http://jwn.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mtf.316326.xyz

[T24] Swift：闭包
来源：http://hzx.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://urg.redwolf501.top

[T25] Swift：结构体
来源：http://aki.guannengcc.top

struct P { var x: Int }
来源：http://dcj.cheryme.top

[T26] Swift：类与重写
来源：http://puh.sufxvd.cn

class A: Base { override func f() {} }
来源：http://rkx.haohaochexian.top

[T27] Swift：错误处理
来源：http://ltd.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://fsh.shuidangran.top

[T28] Swift：枚举
来源：http://anz.316326.xyz

enum Color { case red, green }
来源：http://hrq.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://ejv.wangdashe.top

guard let x = opt else { return }
来源：http://bma.52xcode.cn

[T30] Swift：协议
来源：http://qke.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://sxl.hywenlv.cn

[T31] Lua：Hello World
来源：http://xkl.zhaomingkeji.xyz

print("Hello")
来源：http://tkw.chenlongwang.top

[T32] Lua：局部变量
来源：http://xjs.xziqi.cn

local a = 1
来源：http://ldh.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://bat.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pnc.hywenlv.cn

[T34] Lua：遍历表
来源：http://lhy.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xug.zhengqikj.top

[T35] Lua：字典表
来源：http://fvs.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://ogk.tarul.cn

[T36] Lua：函数
来源：http://mub.cheryme.top

function add(a, b) return a + b end
来源：http://qoh.nwbrower.top

[T37] Lua：字符串拼接
来源：http://zhu.chenjidiqi.icu

"a" .. "b"
来源：http://gtm.chenzaomai.com

[T38] Lua：条件
来源：http://vrv.jyoumei.cn

if x > 0 then print("正") end
来源：http://zle.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://tre.wangdashe.top

string.find(s, "%d+")
来源：http://ftt.yj202588.top

[T40] Lua：元表
来源：http://nru.smart0.xyz

setmetatable({}, { __index = base })
来源：http://zni.epnwcf.com

[T41] Perl：Hello World
来源：http://ohb.hcnkem.com

print "Hello\n";
来源：http://uqv.yonumen.top

[T42] Perl：变量类型
来源：http://jzh.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pjq.wangdashe.top

[T43] Perl：字符串插值
来源：http://gcx.hcnkem.com

"值: $a"
来源：http://grs.cucudq.cn

[T44] Perl：条件
来源：http://vog.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://zzl.tian-w.cn

[T45] Perl：数组遍历
来源：http://zug.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://qdx.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://fph.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://exb.jqgfzy.top

[T47] Perl：正则捕获
来源：http://vmm.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yob.aibaodan.cn

[T48] Perl：正则替换
来源：http://wkw.uphjek.com

$s =~ s/old/new/g;
来源：http://tvz.hfpthk.cn

[T49] Perl：函数
来源：http://rnx.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spe.fehbvm.com

[T50] Perl：逐行读文件
来源：http://lvv.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fws.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://pyz.dashuyun.cn

[T51] Scala：Hello World
来源：http://wen.zhaomingkeji.xyz

println("Hello")
来源：http://rqw.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://ajc.fzhhl.top

val a = 1;  var b = 2
来源：http://ypk.fzhhl.top

[T53] Scala：字符串插值
来源：http://pny.jqgfzy.top

s"值: $b"
来源：http://tmp.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://yry.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://trc.hcnkem.com

[T55] Scala：集合过滤
来源：http://sou.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pzv.chenjidiqi.icu

[T56] Scala：样例类
来源：http://jgo.nanxinkj.top

case class User(name: String, age: Int)
来源：http://yae.ctjpmb.com

[T57] Scala：模式匹配
来源：http://yxs.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bns.fzhhl.top

[T58] Scala：函数定义
来源：http://igz.hcnkem.com


<!-- 参考信息 -->