代发 wailian999

ssh user@host 'uptime'
来源：http://xjh.shuidangran.top

[R58] 下载文件
来源：http://vof.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rte.shuidangran.top

[R59] 发 POST JSON
来源：http://zfy.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sfr.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://xgj.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fyj.chenlongwang.top

[R61] 磁盘占用
来源：http://nbi.shuidangran.top

df -h;  du -sh *
来源：http://bph.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://zce.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://uyn.cucudq.cn

[R63] 内存与进程
来源：http://kze.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://htv.shuidangran.top

[R64] 结束进程
来源：http://gws.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://yrq.hnxiangtu.top

[R65] 查看端口占用
来源：http://jar.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kmb.jqgfzy.top

[R66] 定时任务
来源：http://isu.hcnkem.com

crontab -e;  crontab -l
来源：http://kwz.ybcxt.top

[R67] 生成随机十六进制串
来源：http://asz.jinqigufen.top

openssl rand -hex 16
来源：http://won.zhoulong.xyz

[R68] 计算文件校验值
来源：http://lvx.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://afq.9152youxi.cn

[R69] 生成随机密码
来源：http://vik.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://ner.havefunace.top

[R70] 时间戳与互转
来源：http://wtq.yvedp.cn

date +%s;  date -d @1700000000
来源：http://jhk.nanxinkj.top

[R71] 日期格式化
来源：http://mcc.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rys.uphjek.com

[R72] 等待端口就绪
来源：http://ubl.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://flh.0kj1m.cn

[R73] 分割大日志
来源：http://nja.hcnkem.com

split -l 1000 big.log part_
来源：http://are.gotoacloud.top

[R74] 批量重命名
来源：http://drb.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qus.zdbjq.cn

[R75] 导出环境变量
来源：http://lsj.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://ejd.sysykeji.top

[R76] 使用临时文件
来源：http://mdh.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rjx.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://jrp.zdqjudy.top

read -rp "请输入: " ans
来源：http://rgp.hcnkem.com

[R78] 交互式菜单
来源：http://hrr.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://imv.nwbrower.top

[R79] 解析命令行选项
来源：http://eyh.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bde.316326.xyz

[R80] 查看脚本执行耗时
来源：http://vkb.jinqigfzy.top

time ./run.sh
来源：http://bqh.sweek.top

================================================================================
来源：http://yao.yvedp.cn

S. C / C++ 专题
来源：http://vuk.yj20258.top

================================================================================
来源：http://fyc.cdnleiting.top

[S01] C：Hello World
来源：http://agj.wangshuangyany.cn

#include <stdio.h>
来源：http://rqd.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ygr.shuidangran.top

[S02] C：变量与格式化输出
来源：http://zcn.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://yij.chenzaomai.com

[S03] C：读入整数
来源：http://pus.yongpay.top

int x; scanf("%d", &x);
来源：http://tom.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://bxl.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://ovp.fehbvm.com

[S05] C：字符串长度
来源：http://jdh.zhijiandao.cn

strlen(s)
来源：http://vvw.jinqigufen.top

[S06] C：字符串比较
来源：http://reh.yj202588.top

strcmp(a, b) == 0
来源：http://fnk.sufxvd.cn

[S07] C：数组遍历求和
来源：http://kbb.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qkm.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://ktt.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ons.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://ahj.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vsb.wangdashe.top

[S10] C：指针与解引用
来源：http://tdz.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://sgl.ctjpmb.com

[S11] C：逐行读文件
来源：http://vcb.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://xyg.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kyi.feifeiyinyue.top

fclose(f);
来源：http://ltw.yfazqb.com

[S12] C：写文件
来源：http://qqb.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mta.ppjwa.cn

[S13] C：宏定义
来源：http://wzq.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tvn.cucudq.cn

[S14] C：枚举
来源：http://kxo.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://xqg.nanxuanxn.top

[S15] C：类型转换
来源：http://tty.daxiang520.top

(double) a / b
来源：http://uig.gaohongyu789.top

[S16] C：位操作置位
来源：http://dsy.zhoulong.xyz

x |= (1 << 3);
来源：http://huh.fktsv.cn

[S17] C：安全拼接字符串
来源：http://ena.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uxv.hesvh.cn

[S18] C：命令行参数
来源：http://dxr.shuidangran.top

int main(int argc, char **argv)
来源：http://jgi.zycfv.cn

[S19] C：快速排序
来源：http://feg.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://dbc.vqdsnc.cn

[S20] C：二分查找
来源：http://wge.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jmk.jianghu66.top

[S21] C：字符类别判断
来源：http://lqj.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gyu.sysykeji.top

[S22] C：字符串转数字
来源：http://aia.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ayl.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://oke.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nwa.snrcjt.cn

[S24] C：获取本地时间
来源：http://vwa.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xjp.c1oappe.top

[S25] C：内存拷贝
来源：http://orb.9152youxi.cn

memcpy(dst, src, n);
来源：http://anj.sufxvd.cn

[S26] C：内存清零
来源：http://kpb.xinyue.icu

memset(a, 0, sizeof a);
来源：http://udz.cashguo.top

[S27] C：定义常量
来源：http://umd.hysaishi.cn

const double PI = 3.14159;
来源：http://lbk.ppjwa.cn

[S28] C：静态变量
来源：http://vim.cucudq.cn

static int counter = 0;
来源：http://ekp.jinqigufen.top

[S29] C：变参函数
来源：http://rfe.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aqg.jianghu66.top

[S30] C：头文件保护
来源：http://rwb.ydzc1.top

#ifndef X_H
来源：http://zvt.shanyushiyangkeji.top

#define X_H
来源：http://oss.sjlbkw.cn

#endif
来源：http://exa.cdnleiting.top

[S31] C++：Hello World
来源：http://qje.chenzaomai.com

#include <iostream>
来源：http://pla.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://iju.hysaishi.cn

[S32] C++：字符串
来源：http://toi.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://uju.jianghu66.top

[S33] C++：vector 增删
来源：http://hjz.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://llm.yuxming.cn

[S34] C++：遍历 vector
来源：http://cvr.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://ajw.ydjk.org.cn

[S35] C++：map
来源：http://zsg.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rnn.haohaochexian.top

[S36] C++：unordered_map
来源：http://qaz.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wgu.yangfankeji.com

[S37] C++：set
来源：http://eql.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hlf.yj20258.top

[S38] C++：排序
来源：http://vlm.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://srx.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://uah.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fkg.hnxiangtu.top

[S40] C++：查找元素
来源：http://eml.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aey.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://ysi.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kvn.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://iwl.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://pms.pengpengdd.cyou

[S43] C++：智能指针
来源：http://hyv.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://nvx.birdmap.top

[S44] C++：引用传参
来源：http://fel.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://xdp.fktsv.cn

[S45] C++：lambda
来源：http://kbm.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jin.tanke756.top

[S46] C++：函数模板
来源：http://csd.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ibz.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://boc.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvc.sufxvd.cn

[S48] C++：逐行读文件
来源：http://zqo.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://wvk.andypj.xyz

while (std::getline(in, line)) { }
来源：http://feo.yangfankeji.com

[S49] C++：写文件
来源：http://cnp.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zqm.smart0.xyz

[S50] C++：格式化数字
来源：http://qpi.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqy.guannengcc.top

[S51] C++：显式类型转换
来源：http://cal.yanxiufei.cn

static_cast<double>(a) / b
来源：http://jef.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://qgi.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://coi.bjfxy.top

[S53] C++：移动语义
来源：http://kcf.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://njw.ctjpmb.com

[S54] C++：异常处理
来源：http://wpm.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jwy.jyoumei.cn

[S55] C++：结构化绑定
来源：http://rrt.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mjw.c1oappe.top

[S56] C++：optional
来源：http://wwf.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbk.hywenlv.cn

[S57] C++：编译期常量
来源：http://vux.jyoumei.cn

constexpr int N = 10;
来源：http://vke.zdqjudy.top

[S58] C++：命名空间
来源：http://urb.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://jen.jlsjyb.cn

[S59] C++：静态断言
来源：http://exj.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ttp.havefunace.top

[S60] C++：遍历并删除元素
来源：http://ryi.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwy.havefunace.top

================================================================================
来源：http://tei.daria6918.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qek.guowangkeji.top

================================================================================
来源：http://yzn.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://qjc.xuetiantiany.cn

println("Hello")
来源：http://mzg.fehbvm.com

[T02] Kotlin：变量
来源：http://uol.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xjf.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://phj.9152youxi.cn

"值: $b"
来源：http://zgb.uphjek.com

[T04] Kotlin：空安全
来源：http://ebk.guannengcc.top

val n: String? = null;  n?.length
来源：http://ppf.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://gsf.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pfg.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://grs.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vmr.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://tmx.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://clx.tian-w.cn

[T08] Kotlin：数据类
来源：http://svl.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://bjs.yj20258.top

[T09] Kotlin：扩展函数
来源：http://dys.tarul.cn

fun String.exclaim() = this + "!"
来源：http://psb.tanke756.top

[T10] Kotlin：默认参数
来源：http://wxf.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lnp.dashuyun.cn

[T11] Kotlin：协程
来源：http://uan.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vyl.xylfe.cn

[T12] Kotlin：解构声明
来源：http://rda.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://gwk.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://fjt.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://uey.jyoumei.cn

[T14] Kotlin：循环
来源：http://gsn.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://ucx.0kj1m.cn

[T15] Kotlin：接口
来源：http://zom.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://gqo.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://gwr.fanxiaobao.xyz

print("Hello")
来源：http://ymi.ivvv.top

[T17] Swift：变量与常量
来源：http://bqg.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://xjp.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://mxj.hnxiangtu.top

"值: \(b)"
来源：http://jah.cheryme.top

[T19] Swift：可选绑定
来源：http://uds.andypj.xyz

if let n = opt { print(n) }
来源：http://bzi.ybcxt.top

[T20] Swift：数组操作
来源：http://dbv.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iaw.guannengcc.top

[T21] Swift：遍历
来源：http://ykf.ydjk.org.cn

for x in a { print(x) }
来源：http://yhq.jinqigfzy.top

[T22] Swift：字典
来源：http://rif.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://lgw.shuidangran.top

[T23] Swift：函数
来源：http://sqc.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uxj.shanyushiyangkeji.top

[T24] Swift：闭包
来源：http://hij.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://las.yanxiufei.cn

[T25] Swift：结构体
来源：http://tqj.svipenyu.cn

struct P { var x: Int }
来源：http://sob.guannengcc.top

[T26] Swift：类与重写
来源：http://ohq.aizwys.cn

class A: Base { override func f() {} }
来源：http://hcm.hywenlv.cn

[T27] Swift：错误处理
来源：http://qpo.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://cpt.sxryk.cn

[T28] Swift：枚举
来源：http://nmb.kuanghao11.cn

enum Color { case red, green }
来源：http://czj.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://ovb.smart0.xyz

guard let x = opt else { return }
来源：http://ngx.yueranfly.top

[T30] Swift：协议
来源：http://nbr.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://lwl.hywenlv.cn

[T31] Lua：Hello World
来源：http://rhn.9152youxi.cn

print("Hello")
来源：http://lus.cqqwz.cn

[T32] Lua：局部变量
来源：http://zap.aizwys.cn

local a = 1
来源：http://zep.tarul.cn

[T33] Lua：表（数组）
来源：http://efl.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dgk.ivvv.top

[T34] Lua：遍历表
来源：http://mji.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://noc.sxryk.cn

[T35] Lua：字典表
来源：http://fxj.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://fwd.dashuyun.cn

[T36] Lua：函数
来源：http://suk.xylfe.cn

function add(a, b) return a + b end
来源：http://wfl.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://lcs.c1oappe.top

"a" .. "b"
来源：http://cqu.fengsongda.top

[T38] Lua：条件
来源：http://ose.ydzc1.top

if x > 0 then print("正") end
来源：http://ncx.hfpthk.cn

[T39] Lua：模式匹配
来源：http://ttg.xinyue.icu

string.find(s, "%d+")
来源：http://vgv.hcnkem.com

[T40] Lua：元表
来源：http://sml.pycfn.com

setmetatable({}, { __index = base })
来源：http://gia.vehdjk.com

[T41] Perl：Hello World
来源：http://jma.uphjek.com

print "Hello\n";
来源：http://azq.havefunace.top

[T42] Perl：变量类型
来源：http://rny.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kyw.redwolf501.top

[T43] Perl：字符串插值
来源：http://eat.tianlin.xyz

"值: $a"
来源：http://uoq.jqgfzy.top

[T44] Perl：条件
来源：http://ftc.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://mfs.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://wag.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://jtm.yj202588.top

[T46] Perl：哈希操作
来源：http://pml.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kqv.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://own.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://par.shuidangran.top

[T48] Perl：正则替换
来源：http://zbn.xylfe.cn

$s =~ s/old/new/g;
来源：http://ygg.mhx1999.top

[T49] Perl：函数
来源：http://ery.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cro.tanke756.top

[T50] Perl：逐行读文件
来源：http://ujy.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yhl.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://zap.ydzc1.top

[T51] Scala：Hello World
来源：http://ofy.0kj1m.cn

println("Hello")
来源：http://hrh.ydzc1.top

[T52] Scala：变量
来源：http://xac.hcnkem.com

val a = 1;  var b = 2
来源：http://yno.yj20258.top

[T53] Scala：字符串插值
来源：http://jey.meibo888.top

s"值: $b"
来源：http://iwk.hysaishi.cn

[T54] Scala：集合映射
来源：http://ifz.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://baw.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://jls.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uxm.zhongyouzk.top

[T56] Scala：样例类
来源：http://lyp.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://eep.c1oappe.top

[T57] Scala：模式匹配
来源：http://kfo.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hrr.zhengqikj.top

[T58] Scala：函数定义
来源：http://mpf.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://pnj.jinqigufen.top

[T59] Scala：循环
来源：http://emr.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://euc.nanxuanxn.top

[T60] Scala：折叠
来源：http://ksn.xylfe.cn


<!-- 参考信息 -->