代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://del.wangdashe.top

[R56] 远程拷贝
来源：http://tcr.epnwcf.com

scp file user@host:/path/
来源：http://ekl.cdnleiting.top

[R57] 远程执行命令
来源：http://nbn.ppjwa.cn

ssh user@host 'uptime'
来源：http://wuj.fehbvm.com

[R58] 下载文件
来源：http://zyh.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pcs.pycfn.com

[R59] 发 POST JSON
来源：http://kvv.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hal.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://yvn.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qtl.tian-w.cn

[R61] 磁盘占用
来源：http://qae.iojbl.cn

df -h;  du -sh *
来源：http://kmf.vehdjk.com

[R62] 找最占空间的文件
来源：http://mgd.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://pol.tianlin.xyz

[R63] 内存与进程
来源：http://don.yonumen.top

free -h;  ps aux | grep nginx
来源：http://nim.chenlongwang.top

[R64] 结束进程
来源：http://zfr.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://gko.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://knr.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ljw.aibaodan.cn

[R66] 定时任务
来源：http://xgr.hfpthk.cn

crontab -e;  crontab -l
来源：http://xfv.nwbrower.top

[R67] 生成随机十六进制串
来源：http://sdy.hfpthk.cn

openssl rand -hex 16
来源：http://giw.redwolf501.top

[R68] 计算文件校验值
来源：http://ewg.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kzp.tian-w.cn

[R69] 生成随机密码
来源：http://prd.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://ycf.jlsjyb.cn

[R70] 时间戳与互转
来源：http://nnv.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://zif.tian-w.cn

[R71] 日期格式化
来源：http://idx.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://siu.uphjek.com

[R72] 等待端口就绪
来源：http://rhw.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zes.daxiang520.top

[R73] 分割大日志
来源：http://tjc.cdnleiting.top

split -l 1000 big.log part_
来源：http://bag.hcnkem.com

[R74] 批量重命名
来源：http://lzz.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oob.gotoacloud.top

[R75] 导出环境变量
来源：http://osu.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://vbi.c1oappe.top

[R76] 使用临时文件
来源：http://ijz.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qaq.hammf.cn

[R77] 读取用户输入
来源：http://cqh.ehwqpu.com

read -rp "请输入: " ans
来源：http://eag.ybcxt.top

[R78] 交互式菜单
来源：http://ivs.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jol.yanxiufei.cn

[R79] 解析命令行选项
来源：http://nlp.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://esk.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://zaa.yj20258.top

time ./run.sh
来源：http://vni.nwbrower.top

================================================================================
来源：http://umb.birdmap.top

S. C / C++ 专题
来源：http://uhk.shanyushiyangtech.top

================================================================================
来源：http://kvo.zhongyouzk.top

[S01] C：Hello World
来源：http://ykn.shzxlz.cn

#include <stdio.h>
来源：http://jvz.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tyr.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://hha.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://qxf.jinghuilouyu.cn

[S03] C：读入整数
来源：http://ajm.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://usq.birdmap.top

[S04] C：字符串复制
来源：http://dfv.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kvl.jqgufenzy.top

[S05] C：字符串长度
来源：http://hnb.jinqigufen.top

strlen(s)
来源：http://seg.aizwys.cn

[S06] C：字符串比较
来源：http://pcf.hammf.cn

strcmp(a, b) == 0
来源：http://pbz.daria6918.cn

[S07] C：数组遍历求和
来源：http://bfw.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bhn.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://fef.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lon.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://zgz.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gxi.guowangkeji.top

[S10] C：指针与解引用
来源：http://out.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://xzm.hnqzz.top

[S11] C：逐行读文件
来源：http://yzt.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://ffw.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jwg.jiagoushi.top

fclose(f);
来源：http://lyn.cqqwz.cn

[S12] C：写文件
来源：http://hzy.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://thj.xuetiantiany.cn

[S13] C：宏定义
来源：http://mfb.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vvw.jianghu66.top

[S14] C：枚举
来源：http://mjo.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://vdd.cashguo.top

[S15] C：类型转换
来源：http://toq.gotoacloud.top

(double) a / b
来源：http://qgg.jinqigufen.top

[S16] C：位操作置位
来源：http://plw.yuxming.cn

x |= (1 << 3);
来源：http://xxn.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://kym.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wmh.wangdashe.top

[S18] C：命令行参数
来源：http://alj.cucudq.cn

int main(int argc, char **argv)
来源：http://gfm.bjfxy.top

[S19] C：快速排序
来源：http://phw.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://yuy.chenzaomai.com

[S20] C：二分查找
来源：http://oak.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pja.tarul.cn

[S21] C：字符类别判断
来源：http://qiq.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uzi.pycfn.com

[S22] C：字符串转数字
来源：http://clt.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://zhh.yuanzhike.top

[S23] C：随机数
来源：http://jgp.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zfy.nanxuanxn.top

[S24] C：获取本地时间
来源：http://fqa.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ppz.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://uth.vqdsnc.cn

memcpy(dst, src, n);
来源：http://map.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://roh.guannengcc.top

memset(a, 0, sizeof a);
来源：http://nuf.yanxiufei.cn

[S27] C：定义常量
来源：http://zll.ybcxt.top

const double PI = 3.14159;
来源：http://pdm.hnqzz.top

[S28] C：静态变量
来源：http://avi.haohaochexian.top

static int counter = 0;
来源：http://sdv.yvedp.cn

[S29] C：变参函数
来源：http://sqi.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxh.gzhubu.top

[S30] C：头文件保护
来源：http://ial.pengpengdd.cyou

#ifndef X_H
来源：http://kdr.ivvv.top

#define X_H
来源：http://rev.shanyushiyangtech.top

#endif
来源：http://vka.tian-w.cn

[S31] C++：Hello World
来源：http://lig.dianchejie.cn

#include <iostream>
来源：http://ivh.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://tnx.hywenlv.cn

[S32] C++：字符串
来源：http://zoh.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://qqi.ybcxt.top

[S33] C++：vector 增删
来源：http://jtr.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ceo.9152youxi.cn

[S34] C++：遍历 vector
来源：http://csb.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://enr.cucudq.cn

[S35] C++：map
来源：http://rur.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jhh.wangdashe.top

[S36] C++：unordered_map
来源：http://iot.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://upl.sjlbkw.cn

[S37] C++：set
来源：http://xnf.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dcp.redwolf501.top

[S38] C++：排序
来源：http://cpy.yonumen.top

std::sort(v.begin(), v.end());
来源：http://xaq.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://qla.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://flj.shzxlz.cn

[S40] C++：查找元素
来源：http://hnx.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fsw.yj202588.top

[S41] C++：类与构造函数
来源：http://umo.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bzd.vehdjk.com

[S42] C++：继承与虚函数
来源：http://uxv.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://xwe.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://ybu.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://piq.meibo888.top

[S44] C++：引用传参
来源：http://qtt.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://kwv.svipenyu.cn

[S45] C++：lambda
来源：http://aia.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jvu.yangfankeji.com

[S46] C++：函数模板
来源：http://cnf.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://olw.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://hvj.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mcy.yueranfly.top

[S48] C++：逐行读文件
来源：http://oxu.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jvb.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://szk.svipenyu.cn

[S49] C++：写文件
来源：http://obc.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vbe.yfazqb.com

[S50] C++：格式化数字
来源：http://qze.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xrg.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://zrr.jyoumei.cn

static_cast<double>(a) / b
来源：http://jfp.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://bcm.yuxming.cn

int size() const noexcept { return n_; }
来源：http://bwj.kuanghao11.cn

[S53] C++：移动语义
来源：http://qhp.pycfn.com

std::vector<int> w = std::move(v);
来源：http://tvp.mhx1999.top

[S54] C++：异常处理
来源：http://iqm.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbe.cucudq.cn

[S55] C++：结构化绑定
来源：http://rzo.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ssn.ivvv.top

[S56] C++：optional
来源：http://yvf.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oib.tianlin.xyz

[S57] C++：编译期常量
来源：http://fvc.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://zht.quarkkingdee.top

[S58] C++：命名空间
来源：http://coe.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://tte.zhijiandao.cn

[S59] C++：静态断言
来源：http://mws.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kfe.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://urb.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgt.meibo888.top

================================================================================
来源：http://kta.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://urk.yonumen.top

================================================================================
来源：http://nmo.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://hhr.cashguo.top

println("Hello")
来源：http://fbz.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://oph.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nuh.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://iyj.fktsv.cn

"值: $b"
来源：http://ngb.yuxming.cn

[T04] Kotlin：空安全
来源：http://oku.cqqwz.cn

val n: String? = null;  n?.length
来源：http://wvp.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://rkr.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uwe.vehdjk.com

[T06] Kotlin：集合映射
来源：http://yaw.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://pyi.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://stb.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pnq.shzxlz.cn

[T08] Kotlin：数据类
来源：http://eeo.tarul.cn

data class User(val name: String, val age: Int)
来源：http://vkq.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://fjv.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://wlv.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://kio.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://krh.fktsv.cn

[T11] Kotlin：协程
来源：http://hql.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://taa.cheryme.top

[T12] Kotlin：解构声明
来源：http://nxc.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://iqf.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://imv.aizwys.cn

val m = mapOf("a" to 1)
来源：http://wkt.hywenlv.cn

[T14] Kotlin：循环
来源：http://ppk.9152youxi.cn

for (i in 1..10) println(i)
来源：http://uut.cucudq.cn

[T15] Kotlin：接口
来源：http://cvm.bjfxy.top

interface Shape { fun area(): Double }
来源：http://iuy.jqgufenzy.top

[T16] Swift：Hello World
来源：http://mig.dashuyun.cn

print("Hello")
来源：http://qhh.sufxvd.cn

[T17] Swift：变量与常量
来源：http://hem.jqgfzy.top

var a = 1;  let b = 2
来源：http://kvn.dianchejie.cn

[T18] Swift：字符串插值
来源：http://iqq.ydzc1.top

"值: \(b)"
来源：http://iqy.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://xvi.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://hgj.cucudq.cn

[T20] Swift：数组操作
来源：http://rcd.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ezt.zhongyouzk.top

[T21] Swift：遍历
来源：http://ust.zhongyouzk.top

for x in a { print(x) }
来源：http://yrn.yj202588.top

[T22] Swift：字典
来源：http://vta.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pzo.dashuyun.cn

[T23] Swift：函数
来源：http://ohq.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hav.birdmap.top

[T24] Swift：闭包
来源：http://gbe.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://muo.zhijiandao.cn

[T25] Swift：结构体
来源：http://wfd.jqgufenzy.top

struct P { var x: Int }
来源：http://uqu.hcnkem.com

[T26] Swift：类与重写
来源：http://iwb.guowangkeji.top

class A: Base { override func f() {} }
来源：http://mfy.yj202588.top

[T27] Swift：错误处理
来源：http://lsd.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://akp.yangfankeji.com

[T28] Swift：枚举
来源：http://zup.yonumen.top

enum Color { case red, green }
来源：http://ofj.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://ily.smart0.xyz

guard let x = opt else { return }
来源：http://pvb.zdqjudy.top

[T30] Swift：协议
来源：http://vtn.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://nep.yfazqb.com

[T31] Lua：Hello World
来源：http://yyf.fehbvm.com

print("Hello")
来源：http://uvu.zdqjudy.top

[T32] Lua：局部变量
来源：http://uph.vehdjk.com

local a = 1
来源：http://rjk.shzxlz.cn

[T33] Lua：表（数组）
来源：http://cgj.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xll.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://ida.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://btd.zhiwuduotai.top

[T35] Lua：字典表
来源：http://slc.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://hlz.yueranfly.top

[T36] Lua：函数
来源：http://eqs.hesvh.cn

function add(a, b) return a + b end
来源：http://kuz.jianghu66.top

[T37] Lua：字符串拼接
来源：http://srj.haohaochexian.top

"a" .. "b"
来源：http://bbb.meibo888.top

[T38] Lua：条件
来源：http://hzu.zdbjq.cn

if x > 0 then print("正") end
来源：http://qhd.ctjpmb.com

[T39] Lua：模式匹配
来源：http://mzu.vehdjk.com

string.find(s, "%d+")
来源：http://rwz.yangfankeji.com

[T40] Lua：元表
来源：http://ygf.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://nng.yuanzhike.top

[T41] Perl：Hello World
来源：http://bna.sufxvd.cn

print "Hello\n";
来源：http://crv.c1oappe.top

[T42] Perl：变量类型
来源：http://goc.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zmu.yangfankeji.com

[T43] Perl：字符串插值
来源：http://iik.ydjk.org.cn

"值: $a"
来源：http://rff.ehwqpu.com

[T44] Perl：条件
来源：http://nvb.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://hxj.sufxvd.cn

[T45] Perl：数组遍历
来源：http://vnn.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://ciy.gzhubu.top

[T46] Perl：哈希操作
来源：http://zpc.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ifn.svipenyu.cn

[T47] Perl：正则捕获
来源：http://rcv.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rod.ydzc1.top

[T48] Perl：正则替换
来源：http://fqn.sxryk.cn

$s =~ s/old/new/g;
来源：http://ewn.daxiang520.top

[T49] Perl：函数
来源：http://kcy.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sdc.andypj.xyz

[T50] Perl：逐行读文件
来源：http://wmp.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://svx.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://ixp.guannengcc.top

[T51] Scala：Hello World
来源：http://vgg.gzhubu.top

println("Hello")
来源：http://jzi.ybcxt.top

[T52] Scala：变量
来源：http://mul.cqqwz.cn

val a = 1;  var b = 2
来源：http://zbd.sufxvd.cn

[T53] Scala：字符串插值
来源：http://jee.quarkkingdee.top

s"值: $b"
来源：http://wiw.aibaodan.cn

[T54] Scala：集合映射
来源：http://tyf.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://tkr.zhixingplan.top

[T55] Scala：集合过滤
来源：http://zjd.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://ytg.havefunace.top

[T56] Scala：样例类
来源：http://dlu.yueranfly.top

case class User(name: String, age: Int)
来源：http://oxy.yvedp.cn

[T57] Scala：模式匹配
来源：http://rjj.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://psi.yuxming.cn

[T58] Scala：函数定义
来源：http://ghc.shzxlz.cn


<!-- 参考信息 -->