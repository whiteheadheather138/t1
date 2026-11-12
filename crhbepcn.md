代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xsb.hysaishi.cn

[R56] 远程拷贝
来源：http://btq.hcnkem.com

scp file user@host:/path/
来源：http://bmm.xinyue.icu

[R57] 远程执行命令
来源：http://mvh.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://zhl.tian-w.cn

[R58] 下载文件
来源：http://cgw.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ghg.ehwqpu.com

[R59] 发 POST JSON
来源：http://exu.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xst.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://vfb.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fyf.andypj.xyz

[R61] 磁盘占用
来源：http://yya.52xcode.cn

df -h;  du -sh *
来源：http://zgw.nwbrower.top

[R62] 找最占空间的文件
来源：http://cqt.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://mxc.dianchejie.cn

[R63] 内存与进程
来源：http://whb.havefunace.top

free -h;  ps aux | grep nginx
来源：http://flj.xinyue.icu

[R64] 结束进程
来源：http://jnm.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://upu.yongpay.top

[R65] 查看端口占用
来源：http://akd.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://adl.nanxinkj.top

[R66] 定时任务
来源：http://hvv.jqgfzy.top

crontab -e;  crontab -l
来源：http://nxp.hcnkem.com

[R67] 生成随机十六进制串
来源：http://gwg.zhixingplan.top

openssl rand -hex 16
来源：http://osz.chenlongwang.top

[R68] 计算文件校验值
来源：http://twn.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://heu.zdqjudy.top

[R69] 生成随机密码
来源：http://pca.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://ywm.tanke756.top

[R70] 时间戳与互转
来源：http://smv.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://lhk.svipenyu.cn

[R71] 日期格式化
来源：http://ybr.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ecd.hammf.cn

[R72] 等待端口就绪
来源：http://pxw.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ekw.yongpay.top

[R73] 分割大日志
来源：http://qfv.nwbrower.top

split -l 1000 big.log part_
来源：http://ngv.pengpengdd.cyou

[R74] 批量重命名
来源：http://xkk.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lid.shuidangran.top

[R75] 导出环境变量
来源：http://ymb.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://lli.jianghu66.top

[R76] 使用临时文件
来源：http://dcn.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://usq.sjlbkw.cn

[R77] 读取用户输入
来源：http://xyi.zhixingplan.top

read -rp "请输入: " ans
来源：http://whq.mhx1999.top

[R78] 交互式菜单
来源：http://kvn.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://zco.tian-w.cn

[R79] 解析命令行选项
来源：http://ghb.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ymz.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://xnm.jlsjyb.cn

time ./run.sh
来源：http://mte.nanxinkj.top

================================================================================
来源：http://qhu.nwbrower.top

S. C / C++ 专题
来源：http://kkm.havefunace.top

================================================================================
来源：http://pbi.yuxming.cn

[S01] C：Hello World
来源：http://xmk.feifeiyinyue.top

#include <stdio.h>
来源：http://xvw.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eam.fzhhl.top

[S02] C：变量与格式化输出
来源：http://abs.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://cpj.jyoumei.cn

[S03] C：读入整数
来源：http://kvj.dashuyun.cn

int x; scanf("%d", &x);
来源：http://lks.shzxlz.cn

[S04] C：字符串复制
来源：http://fat.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zhv.mhx1999.top

[S05] C：字符串长度
来源：http://rxi.chenlongwang.top

strlen(s)
来源：http://lid.ppjwa.cn

[S06] C：字符串比较
来源：http://qpm.andypj.xyz

strcmp(a, b) == 0
来源：http://rdn.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://ooi.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dqt.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://qlt.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txv.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://boh.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://irc.aibaodan.cn

[S10] C：指针与解引用
来源：http://lkk.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://aak.jlsjyb.cn

[S11] C：逐行读文件
来源：http://dpz.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://bag.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rjy.52xcode.cn

fclose(f);
来源：http://hnu.jinqigufen.top

[S12] C：写文件
来源：http://ytj.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xwl.jyoumei.cn

[S13] C：宏定义
来源：http://vxv.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://njb.gzhubu.top

[S14] C：枚举
来源：http://uso.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://xtj.ivvv.top

[S15] C：类型转换
来源：http://aut.zhongyouzk.top

(double) a / b
来源：http://yiy.cheryme.top

[S16] C：位操作置位
来源：http://ppl.sxryk.cn

x |= (1 << 3);
来源：http://pmj.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://gbn.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qcn.dashuyun.cn

[S18] C：命令行参数
来源：http://syy.yvedp.cn

int main(int argc, char **argv)
来源：http://rfo.vqdsnc.cn

[S19] C：快速排序
来源：http://yig.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://noo.jianghu66.top

[S20] C：二分查找
来源：http://tjk.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mpj.fzhhl.top

[S21] C：字符类别判断
来源：http://wiu.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxb.birdmap.top

[S22] C：字符串转数字
来源：http://zcd.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://nla.haohaochexian.top

[S23] C：随机数
来源：http://rqz.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hxw.jiagoushi.top

[S24] C：获取本地时间
来源：http://hpt.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jkd.uphjek.com

[S25] C：内存拷贝
来源：http://vbk.zhoulong.xyz

memcpy(dst, src, n);
来源：http://leg.dashuyun.cn

[S26] C：内存清零
来源：http://muy.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://cyn.fengsongda.top

[S27] C：定义常量
来源：http://rjs.52xcode.cn

const double PI = 3.14159;
来源：http://hqf.xylfe.cn

[S28] C：静态变量
来源：http://khr.cashguo.top

static int counter = 0;
来源：http://vdx.cashguo.top

[S29] C：变参函数
来源：http://utm.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://szg.jqgufenzy.top

[S30] C：头文件保护
来源：http://tbn.wangshuangyany.cn

#ifndef X_H
来源：http://mcq.sysykeji.top

#define X_H
来源：http://nnu.yj20258888.top

#endif
来源：http://jcw.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://xbk.jyoumei.cn

#include <iostream>
来源：http://xkv.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://qsa.hesvh.cn

[S32] C++：字符串
来源：http://uhv.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://kya.svipenyu.cn

[S33] C++：vector 增删
来源：http://kzh.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzn.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://nod.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ycc.daria6918.cn

[S35] C++：map
来源：http://nmi.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dea.zhoulong.xyz

[S36] C++：unordered_map
来源：http://bhl.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ccb.fktsv.cn

[S37] C++：set
来源：http://fmf.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gkg.dianchejie.cn

[S38] C++：排序
来源：http://yhn.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://imv.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://ecr.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hfu.ybcxt.top

[S40] C++：查找元素
来源：http://uzw.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uer.hnqzz.top

[S41] C++：类与构造函数
来源：http://nlc.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lcw.epnwcf.com

[S42] C++：继承与虚函数
来源：http://nso.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://xwz.gotoacloud.top

[S43] C++：智能指针
来源：http://rda.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://fkt.jyoumei.cn

[S44] C++：引用传参
来源：http://zns.fengsongda.top

void inc(int &x) { ++x; }
来源：http://dvm.jyoumei.cn

[S45] C++：lambda
来源：http://nut.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://qvq.xuetiantiany.cn

[S46] C++：函数模板
来源：http://fxl.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xcj.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://ilm.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://etl.nanxinkj.top

[S48] C++：逐行读文件
来源：http://gzj.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://tgg.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://uly.vehdjk.com

[S49] C++：写文件
来源：http://gft.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wgv.nanxuanxn.top

[S50] C++：格式化数字
来源：http://mqh.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksw.shuidangran.top

[S51] C++：显式类型转换
来源：http://ujm.quarkkingdee.top

static_cast<double>(a) / b
来源：http://kvj.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://ekl.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://vzg.gogol.net.cn

[S53] C++：移动语义
来源：http://otp.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://jsj.guannengcc.top

[S54] C++：异常处理
来源：http://twt.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hfl.sweek.top

[S55] C++：结构化绑定
来源：http://ate.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cja.uphjek.com

[S56] C++：optional
来源：http://xcf.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wzv.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://ihw.hnqzz.top

constexpr int N = 10;
来源：http://ago.sweek.top

[S58] C++：命名空间
来源：http://udx.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://tuh.xziqi.cn

[S59] C++：静态断言
来源：http://dvh.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyw.sweek.top

[S60] C++：遍历并删除元素
来源：http://que.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gqn.nwbrower.top

================================================================================
来源：http://ukf.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://abr.guowangkeji.top

================================================================================
来源：http://olt.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://pcr.bjfxy.top

println("Hello")
来源：http://rrq.sysykeji.top

[T02] Kotlin：变量
来源：http://vqx.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fqa.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://trv.xinyue.icu

"值: $b"
来源：http://nzv.zdbjq.cn

[T04] Kotlin：空安全
来源：http://jox.yuxming.cn

val n: String? = null;  n?.length
来源：http://xzs.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://eqa.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gfd.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://eju.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://isz.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://zbk.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hhu.tanke756.top

[T08] Kotlin：数据类
来源：http://tkm.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://wyb.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://kup.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://kho.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://bbo.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://viq.aizwys.cn

[T11] Kotlin：协程
来源：http://txw.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zxq.epnwcf.com

[T12] Kotlin：解构声明
来源：http://uee.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://rki.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://ate.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://all.ydzc1.top

[T14] Kotlin：循环
来源：http://lmb.hysaishi.cn

for (i in 1..10) println(i)
来源：http://xjb.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://vxz.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://hxf.sxryk.cn

[T16] Swift：Hello World
来源：http://yqt.jyoumei.cn

print("Hello")
来源：http://zhs.daxiang520.top

[T17] Swift：变量与常量
来源：http://gmv.yj202588.top

var a = 1;  let b = 2
来源：http://xhb.yangfankeji.com

[T18] Swift：字符串插值
来源：http://pyc.epnwcf.com

"值: \(b)"
来源：http://lkc.yonumen.top

[T19] Swift：可选绑定
来源：http://snb.jlsjyb.cn

if let n = opt { print(n) }
来源：http://oej.zycfv.cn

[T20] Swift：数组操作
来源：http://vgx.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zdn.zhengqikj.top

[T21] Swift：遍历
来源：http://nha.tarul.cn

for x in a { print(x) }
来源：http://iho.xylfe.cn

[T22] Swift：字典
来源：http://ncb.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tug.guowangkeji.top

[T23] Swift：函数
来源：http://unc.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fln.shuidangran.top

[T24] Swift：闭包
来源：http://kpd.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wig.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://zhk.tanke756.top

struct P { var x: Int }
来源：http://kca.yvedp.cn

[T26] Swift：类与重写
来源：http://lmx.jinqigufen.top

class A: Base { override func f() {} }
来源：http://quv.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://tao.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://cxq.hcnkem.com

[T28] Swift：枚举
来源：http://ycq.yj20258.top

enum Color { case red, green }
来源：http://pry.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://rve.iojbl.cn

guard let x = opt else { return }
来源：http://umk.yj20258.top

[T30] Swift：协议
来源：http://pfu.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://gmo.jlsjyb.cn

[T31] Lua：Hello World
来源：http://vzv.feifeiyinyue.top

print("Hello")
来源：http://bko.vqdsnc.cn

[T32] Lua：局部变量
来源：http://kkl.pycfn.com

local a = 1
来源：http://xok.iojbl.cn

[T33] Lua：表（数组）
来源：http://dqw.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jfn.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://vag.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://som.hcnkem.com

[T35] Lua：字典表
来源：http://vyy.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://aeh.vehdjk.com

[T36] Lua：函数
来源：http://tva.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://wgc.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://nrv.0kj1m.cn

"a" .. "b"
来源：http://lka.c1oappe.top

[T38] Lua：条件
来源：http://lsi.yj202588.top

if x > 0 then print("正") end
来源：http://cbj.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://jhx.316326.xyz

string.find(s, "%d+")
来源：http://uyt.zhoulong.xyz

[T40] Lua：元表
来源：http://ytj.tian-w.cn

setmetatable({}, { __index = base })
来源：http://dtu.tian-w.cn

[T41] Perl：Hello World
来源：http://atn.hcnkem.com

print "Hello\n";
来源：http://ogt.yanxiufei.cn

[T42] Perl：变量类型
来源：http://ljc.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qxz.cashguo.top

[T43] Perl：字符串插值
来源：http://cvs.haohaochexian.top

"值: $a"
来源：http://hqq.chenlongwang.top

[T44] Perl：条件
来源：http://gin.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://tcb.cucudq.cn

[T45] Perl：数组遍历
来源：http://vdd.cheryme.top

for my $x (@arr) { print $x; }
来源：http://owj.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://rst.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ksa.vehdjk.com

[T47] Perl：正则捕获
来源：http://jvq.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ofc.shuidangran.top

[T48] Perl：正则替换
来源：http://wwd.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://kty.c1oappe.top

[T49] Perl：函数
来源：http://uls.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qdg.daxiang520.top

[T50] Perl：逐行读文件
来源：http://nne.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://zyp.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://bui.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://whc.epnwcf.com

println("Hello")
来源：http://dlj.havefunace.top

[T52] Scala：变量
来源：http://efn.fehbvm.com

val a = 1;  var b = 2
来源：http://qvu.smart0.xyz

[T53] Scala：字符串插值
来源：http://tvy.ybcxt.top

s"值: $b"
来源：http://vdo.havefunace.top

[T54] Scala：集合映射
来源：http://nun.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://rrk.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://qbb.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://ojk.gotoacloud.top

[T56] Scala：样例类
来源：http://lmu.aizwys.cn

case class User(name: String, age: Int)
来源：http://dce.jqgfzy.top

[T57] Scala：模式匹配
来源：http://iqa.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pwu.guowangkeji.top

[T58] Scala：函数定义
来源：http://adf.gaohongyu789.top


<!-- 参考信息 -->