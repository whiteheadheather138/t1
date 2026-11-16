代发 wailian999

ssh user@host 'uptime'
来源：http://smx.hywenlv.cn

[R58] 下载文件
来源：http://ipb.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ffe.jianghu66.top

[R59] 发 POST JSON
来源：http://prz.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gzu.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://agh.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mke.jianghu66.top

[R61] 磁盘占用
来源：http://xwe.redwolf501.top

df -h;  du -sh *
来源：http://cjx.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://unr.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://zvy.gzhubu.top

[R63] 内存与进程
来源：http://ceq.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://jbs.nanxinkj.top

[R64] 结束进程
来源：http://mqc.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://yee.cashguo.top

[R65] 查看端口占用
来源：http://uob.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lzq.cashguo.top

[R66] 定时任务
来源：http://cpg.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://myo.sysykeji.top

[R67] 生成随机十六进制串
来源：http://utr.cheryme.top

openssl rand -hex 16
来源：http://vcv.bbcook.cn

[R68] 计算文件校验值
来源：http://nur.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rmf.yangfankeji.com

[R69] 生成随机密码
来源：http://ark.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://vkv.redwolf501.top

[R70] 时间戳与互转
来源：http://aqi.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://ybl.cucudq.cn

[R71] 日期格式化
来源：http://eey.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nto.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://njm.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zjh.fengsongda.top

[R73] 分割大日志
来源：http://wnn.xinyue.icu

split -l 1000 big.log part_
来源：http://prl.vqdsnc.cn

[R74] 批量重命名
来源：http://hrb.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yox.pycfn.com

[R75] 导出环境变量
来源：http://ayx.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://lpq.andypj.xyz

[R76] 使用临时文件
来源：http://quq.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uxr.nanxinkj.top

[R77] 读取用户输入
来源：http://yzx.hfpthk.cn

read -rp "请输入: " ans
来源：http://ein.zhongyouzk.top

[R78] 交互式菜单
来源：http://xpe.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zcp.yonumen.top

[R79] 解析命令行选项
来源：http://xrd.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://irg.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://nyp.fengsongda.top

time ./run.sh
来源：http://xps.andypj.xyz

================================================================================
来源：http://bex.sufxvd.cn

S. C / C++ 专题
来源：http://orb.vqdsnc.cn

================================================================================
来源：http://wdl.ctjpmb.com

[S01] C：Hello World
来源：http://usd.nwbrower.top

#include <stdio.h>
来源：http://ech.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ezo.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://nno.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://ldp.mhx1999.top

[S03] C：读入整数
来源：http://drr.yj202588.top

int x; scanf("%d", &x);
来源：http://buq.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://utm.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://jsg.ppjwa.cn

[S05] C：字符串长度
来源：http://cxf.ywan-chungtsiang.top

strlen(s)
来源：http://glc.nanxinkj.top

[S06] C：字符串比较
来源：http://yli.cdnleiting.top

strcmp(a, b) == 0
来源：http://zwd.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://zxf.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jbv.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://iml.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xsf.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://cdc.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uni.jqgufenzy.top

[S10] C：指针与解引用
来源：http://phc.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://hro.tanke756.top

[S11] C：逐行读文件
来源：http://oaz.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://tof.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bgj.yfazqb.com

fclose(f);
来源：http://onx.bjfxy.top

[S12] C：写文件
来源：http://han.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hoq.haohaochexian.top

[S13] C：宏定义
来源：http://knd.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyn.ybcxt.top

[S14] C：枚举
来源：http://led.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://ivo.jqgfzy.top

[S15] C：类型转换
来源：http://cev.nwbrower.top

(double) a / b
来源：http://apu.tanke756.top

[S16] C：位操作置位
来源：http://jhh.hysaishi.cn

x |= (1 << 3);
来源：http://hqi.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://jaj.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ppt.jqgufenzy.top

[S18] C：命令行参数
来源：http://usz.cdnleiting.top

int main(int argc, char **argv)
来源：http://auh.316326.xyz

[S19] C：快速排序
来源：http://kbd.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://csc.cucudq.cn

[S20] C：二分查找
来源：http://zhg.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mbe.zhixingplan.top

[S21] C：字符类别判断
来源：http://qio.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ofj.chenlongwang.top

[S22] C：字符串转数字
来源：http://xji.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jmy.bbcook.cn

[S23] C：随机数
来源：http://duw.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vav.havefunace.top

[S24] C：获取本地时间
来源：http://ust.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ijf.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://ptl.yvedp.cn

memcpy(dst, src, n);
来源：http://spw.zdbjq.cn

[S26] C：内存清零
来源：http://pzo.pycfn.com

memset(a, 0, sizeof a);
来源：http://dss.zycfv.cn

[S27] C：定义常量
来源：http://xbs.0kj1m.cn

const double PI = 3.14159;
来源：http://nfy.gzhubu.top

[S28] C：静态变量
来源：http://txm.jqgufenzy.top

static int counter = 0;
来源：http://mak.uphjek.com

[S29] C：变参函数
来源：http://mwc.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dtx.fengsongda.top

[S30] C：头文件保护
来源：http://tmd.sxryk.cn

#ifndef X_H
来源：http://lwv.fzhhl.top

#define X_H
来源：http://smg.epnwcf.com

#endif
来源：http://hea.hongshengwenyu.top

[S31] C++：Hello World
来源：http://hho.c1oappe.top

#include <iostream>
来源：http://gry.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://avl.yj20258.top

[S32] C++：字符串
来源：http://qhf.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://tat.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://jan.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://plc.guannengcc.top

[S34] C++：遍历 vector
来源：http://huw.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://clf.sysykeji.top

[S35] C++：map
来源：http://fuc.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cot.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://mde.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xqb.zhoulong.xyz

[S37] C++：set
来源：http://ywo.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lco.zhoulong.xyz

[S38] C++：排序
来源：http://fds.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://fgj.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://rtl.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xdt.epnwcf.com

[S40] C++：查找元素
来源：http://qhc.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bif.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://lyp.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgb.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://jtu.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://xtv.cheryme.top

[S43] C++：智能指针
来源：http://hvp.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://vcw.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://uyq.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://ohz.zdqjudy.top

[S45] C++：lambda
来源：http://apn.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://cyr.ybcxt.top

[S46] C++：函数模板
来源：http://pjx.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qqf.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://jgi.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fum.tianlin.xyz

[S48] C++：逐行读文件
来源：http://jkl.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://jwz.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://lyl.9152youxi.cn

[S49] C++：写文件
来源：http://xpe.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hel.fengsongda.top

[S50] C++：格式化数字
来源：http://emb.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zib.svipenyu.cn

[S51] C++：显式类型转换
来源：http://wzw.hywenlv.cn

static_cast<double>(a) / b
来源：http://nwt.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://dqr.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://vfj.sufxvd.cn

[S53] C++：移动语义
来源：http://ltw.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://kkf.guannengcc.top

[S54] C++：异常处理
来源：http://tjj.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://con.yj20258.top

[S55] C++：结构化绑定
来源：http://jbl.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nhf.yonumen.top

[S56] C++：optional
来源：http://ild.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://apb.xuanzx.com

[S57] C++：编译期常量
来源：http://xoe.svipenyu.cn

constexpr int N = 10;
来源：http://zcq.hnqzz.top

[S58] C++：命名空间
来源：http://hho.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://voy.yanxiufei.cn

[S59] C++：静态断言
来源：http://mqz.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wff.yongpay.top

[S60] C++：遍历并删除元素
来源：http://jzi.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hvv.zhaomingkeji.xyz

================================================================================
来源：http://lmc.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eul.jinyuanbaomall.cn

================================================================================
来源：http://dzq.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://ivw.zhengqikj.top

println("Hello")
来源：http://pqe.sufxvd.cn

[T02] Kotlin：变量
来源：http://dxp.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bjj.hammf.cn

[T03] Kotlin：字符串模板
来源：http://gje.chenlongwang.top

"值: $b"
来源：http://fga.fehbvm.com

[T04] Kotlin：空安全
来源：http://owa.nwbrower.top

val n: String? = null;  n?.length
来源：http://xdj.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://omo.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://njt.tian-w.cn

[T06] Kotlin：集合映射
来源：http://ukv.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://fnf.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://uyw.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wae.haohaochexian.top

[T08] Kotlin：数据类
来源：http://cak.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://pls.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://uoi.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://exp.gzhubu.top

[T10] Kotlin：默认参数
来源：http://ssw.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lau.fehbvm.com

[T11] Kotlin：协程
来源：http://jfe.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vdp.havefunace.top

[T12] Kotlin：解构声明
来源：http://gsw.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://lgp.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://vzp.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://kdm.daria6918.cn

[T14] Kotlin：循环
来源：http://tuz.yvedp.cn

for (i in 1..10) println(i)
来源：http://efz.snrcjt.cn

[T15] Kotlin：接口
来源：http://gbk.yongpay.top

interface Shape { fun area(): Double }
来源：http://rrt.nwbrower.top

[T16] Swift：Hello World
来源：http://bvy.c1oappe.top

print("Hello")
来源：http://aab.fzhhl.top

[T17] Swift：变量与常量
来源：http://oaj.redwolf501.top

var a = 1;  let b = 2
来源：http://abq.yj20258888.top

[T18] Swift：字符串插值
来源：http://ytr.hysaishi.cn

"值: \(b)"
来源：http://sjr.zdbjq.cn

[T19] Swift：可选绑定
来源：http://nnh.xinyue.icu

if let n = opt { print(n) }
来源：http://ict.guannengcc.top

[T20] Swift：数组操作
来源：http://ggw.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://hcs.cashguo.top

[T21] Swift：遍历
来源：http://xwi.yj202588.top

for x in a { print(x) }
来源：http://atu.wangdashe.top

[T22] Swift：字典
来源：http://kdz.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://pgs.mhx1999.top

[T23] Swift：函数
来源：http://cqo.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vjw.xuanzx.com

[T24] Swift：闭包
来源：http://mmd.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uof.xuetiantiany.cn

[T25] Swift：结构体
来源：http://xvq.jqgufenzy.top

struct P { var x: Int }
来源：http://ove.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://ava.zdbjq.cn

class A: Base { override func f() {} }
来源：http://zty.c1oappe.top

[T27] Swift：错误处理
来源：http://fww.jianghu66.top

do { try f() } catch { print(error) }
来源：http://taf.andypj.xyz

[T28] Swift：枚举
来源：http://bvj.nanxinkj.top

enum Color { case red, green }
来源：http://xqe.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://gib.hysaishi.cn

guard let x = opt else { return }
来源：http://dao.hysaishi.cn

[T30] Swift：协议
来源：http://ark.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://url.yanxiufei.cn

[T31] Lua：Hello World
来源：http://fgf.shzxlz.cn

print("Hello")
来源：http://nwp.xziqi.cn

[T32] Lua：局部变量
来源：http://sek.bjfxy.top

local a = 1
来源：http://pjd.xinyue.icu

[T33] Lua：表（数组）
来源：http://kwx.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://slo.jianghu66.top

[T34] Lua：遍历表
来源：http://xoi.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yfm.gaohongyu789.top

[T35] Lua：字典表
来源：http://dqt.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://bio.quarkkingdee.top

[T36] Lua：函数
来源：http://axr.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://aut.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://txd.hongshengwenyu.top

"a" .. "b"
来源：http://svq.ybcxt.top

[T38] Lua：条件
来源：http://ngf.shuidangran.top

if x > 0 then print("正") end
来源：http://tnm.zhixingplan.top

[T39] Lua：模式匹配
来源：http://kpp.cqqwz.cn

string.find(s, "%d+")
来源：http://swn.tanke756.top

[T40] Lua：元表
来源：http://rfv.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://rvr.zhixingplan.top

[T41] Perl：Hello World
来源：http://rqe.uphjek.com

print "Hello\n";
来源：http://kxr.epnwcf.com

[T42] Perl：变量类型
来源：http://mbs.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ori.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://rqj.yj20258888.top

"值: $a"
来源：http://iej.sjlbkw.cn

[T44] Perl：条件
来源：http://fvo.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://mkg.hnqzz.top

[T45] Perl：数组遍历
来源：http://adg.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://pkb.xylfe.cn

[T46] Perl：哈希操作
来源：http://igk.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fwp.jinqigufen.top

[T47] Perl：正则捕获
来源：http://qap.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://oxi.pycfn.com

[T48] Perl：正则替换
来源：http://nme.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://cpn.yfazqb.com

[T49] Perl：函数
来源：http://rhs.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wzc.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://xyv.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://dbf.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://zgy.bbcook.cn

[T51] Scala：Hello World
来源：http://nsv.yuanzhike.top

println("Hello")
来源：http://eqb.tarul.cn

[T52] Scala：变量
来源：http://isz.ydzc1.top

val a = 1;  var b = 2
来源：http://ney.yonumen.top

[T53] Scala：字符串插值
来源：http://tci.wangdashe.top

s"值: $b"
来源：http://oxa.hesvh.cn

[T54] Scala：集合映射
来源：http://cnk.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://dcy.redwolf501.top

[T55] Scala：集合过滤
来源：http://wwi.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://vqb.ybcxt.top

[T56] Scala：样例类
来源：http://rkq.jinqigufen.top

case class User(name: String, age: Int)
来源：http://qsc.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://zkh.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ugl.xziqi.cn

[T58] Scala：函数定义
来源：http://bhk.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://sui.meibo888.top

[T59] Scala：循环
来源：http://des.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://irq.sysykeji.top

[T60] Scala：折叠
来源：http://wzq.haohaochexian.top


<!-- 参考信息 -->