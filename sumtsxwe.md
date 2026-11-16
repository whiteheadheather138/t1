代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jvd.gogol.net.cn

[R54] 比较两个文件
来源：http://ytx.vehdjk.com

diff a.txt b.txt
来源：http://jnj.cucudq.cn

[R55] 压缩与解压
来源：http://eee.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qvd.yanxiufei.cn

[R56] 远程拷贝
来源：http://sri.shuidangran.top

scp file user@host:/path/
来源：http://ybe.zhoulong.xyz

[R57] 远程执行命令
来源：http://jfy.jiagoushi.top

ssh user@host 'uptime'
来源：http://myi.tian-w.cn

[R58] 下载文件
来源：http://vka.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wrd.zhixingplan.top

[R59] 发 POST JSON
来源：http://mhd.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://akj.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://yym.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tkz.hammf.cn

[R61] 磁盘占用
来源：http://pnh.jinqigfzy.top

df -h;  du -sh *
来源：http://bds.zdbjq.cn

[R62] 找最占空间的文件
来源：http://qis.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://ctk.quarkkingdee.top

[R63] 内存与进程
来源：http://aai.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://dqb.ywan-chungtsiang.top

[R64] 结束进程
来源：http://str.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://rcp.yuanzhike.top

[R65] 查看端口占用
来源：http://ren.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://alw.dashuyun.cn

[R66] 定时任务
来源：http://mct.zhengqikj.top

crontab -e;  crontab -l
来源：http://pfn.fengsongda.top

[R67] 生成随机十六进制串
来源：http://rad.cashguo.top

openssl rand -hex 16
来源：http://rfc.fzhhl.top

[R68] 计算文件校验值
来源：http://tpe.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vfm.nanxuanxn.top

[R69] 生成随机密码
来源：http://llj.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://kci.zhixingplan.top

[R70] 时间戳与互转
来源：http://hrq.yj20258.top

date +%s;  date -d @1700000000
来源：http://ahg.tian-w.cn

[R71] 日期格式化
来源：http://bcu.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://njb.zdqjudy.top

[R72] 等待端口就绪
来源：http://idi.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jzz.yfazqb.com

[R73] 分割大日志
来源：http://kga.ydzc1.top

split -l 1000 big.log part_
来源：http://fci.chenlongwang.top

[R74] 批量重命名
来源：http://fwy.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mgu.vehdjk.com

[R75] 导出环境变量
来源：http://stf.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pbe.jqgfzy.top

[R76] 使用临时文件
来源：http://zzt.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ogj.yanxiufei.cn

[R77] 读取用户输入
来源：http://ltz.svipenyu.cn

read -rp "请输入: " ans
来源：http://xhr.ydjk.org.cn

[R78] 交互式菜单
来源：http://lzc.sufxvd.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zge.ydjk.org.cn

[R79] 解析命令行选项
来源：http://zbe.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lzc.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://sdh.quarkkingdee.top

time ./run.sh
来源：http://mmy.bbcook.cn

================================================================================
来源：http://akx.quarkkingdee.top

S. C / C++ 专题
来源：http://rew.dianchejie.cn

================================================================================
来源：http://qjz.yj202588.top

[S01] C：Hello World
来源：http://jyd.shangyingyoupin.top

#include <stdio.h>
来源：http://yqx.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rtg.daria6918.cn

[S02] C：变量与格式化输出
来源：http://otb.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://xup.9152youxi.cn

[S03] C：读入整数
来源：http://cao.sxryk.cn

int x; scanf("%d", &x);
来源：http://nbe.ehwqpu.com

[S04] C：字符串复制
来源：http://fyw.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://mrm.hywenlv.cn

[S05] C：字符串长度
来源：http://uwc.nwbrower.top

strlen(s)
来源：http://fhz.pengpengdd.cyou

[S06] C：字符串比较
来源：http://pwt.yonumen.top

strcmp(a, b) == 0
来源：http://aqn.chenlongwang.top

[S07] C：数组遍历求和
来源：http://epl.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xnr.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://yhl.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xbc.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://hcx.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xpb.nanxuanxn.top

[S10] C：指针与解引用
来源：http://eul.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://rpo.gotoacloud.top

[S11] C：逐行读文件
来源：http://eeu.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://vzj.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vwe.ppjwa.cn

fclose(f);
来源：http://nwv.quarkkingdee.top

[S12] C：写文件
来源：http://yiv.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yvz.shuidangran.top

[S13] C：宏定义
来源：http://ilb.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qau.shuidangran.top

[S14] C：枚举
来源：http://afj.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://mzr.52xcode.cn

[S15] C：类型转换
来源：http://hwj.xylfe.cn

(double) a / b
来源：http://mvd.jinqigufen.top

[S16] C：位操作置位
来源：http://sec.ppjwa.cn

x |= (1 << 3);
来源：http://cxr.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://iod.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://brt.smart0.xyz

[S18] C：命令行参数
来源：http://idd.daria6918.cn

int main(int argc, char **argv)
来源：http://sdt.cqqwz.cn

[S19] C：快速排序
来源：http://aqq.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://cei.hammf.cn

[S20] C：二分查找
来源：http://mzv.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ais.iojbl.cn

[S21] C：字符类别判断
来源：http://rut.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fqt.zdbjq.cn

[S22] C：字符串转数字
来源：http://ucc.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tsk.gzhubu.top

[S23] C：随机数
来源：http://tii.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dbf.cqqwz.cn

[S24] C：获取本地时间
来源：http://zvx.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcl.fehbvm.com

[S25] C：内存拷贝
来源：http://oif.uphjek.com

memcpy(dst, src, n);
来源：http://ybd.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://bfd.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://pdq.xuanzx.com

[S27] C：定义常量
来源：http://yoj.snrcjt.cn

const double PI = 3.14159;
来源：http://wso.cucudq.cn

[S28] C：静态变量
来源：http://kif.shanyushiyangkeji.top

static int counter = 0;
来源：http://pld.nanxinkj.top

[S29] C：变参函数
来源：http://pnt.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ehd.jqgufenzy.top

[S30] C：头文件保护
来源：http://ayo.cucudq.cn

#ifndef X_H
来源：http://olx.daxiang520.top

#define X_H
来源：http://tox.xingfuxueyuan.xyz

#endif
来源：http://rwl.jlsjyb.cn

[S31] C++：Hello World
来源：http://sbx.hfpthk.cn

#include <iostream>
来源：http://ncn.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://wyu.vehdjk.com

[S32] C++：字符串
来源：http://dqi.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://boy.gotoacloud.top

[S33] C++：vector 增删
来源：http://swu.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jnr.xuanzx.com

[S34] C++：遍历 vector
来源：http://cfd.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://obv.ydzc1.top

[S35] C++：map
来源：http://dos.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yqk.cheryme.top

[S36] C++：unordered_map
来源：http://pdc.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ovm.gogol.net.cn

[S37] C++：set
来源：http://drk.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rhf.sjlbkw.cn

[S38] C++：排序
来源：http://tlc.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://fua.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://bvs.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pxs.zycfv.cn

[S40] C++：查找元素
来源：http://kam.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ott.yj202588.top

[S41] C++：类与构造函数
来源：http://xpx.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ohh.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://jzj.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://mjh.shzxlz.cn

[S43] C++：智能指针
来源：http://dxy.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://hvq.redwolf501.top

[S44] C++：引用传参
来源：http://hkz.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://rqu.c1oappe.top

[S45] C++：lambda
来源：http://qjz.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://cyw.shangyingyoupin.top

[S46] C++：函数模板
来源：http://zjg.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://azf.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://sim.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://phe.ydzc1.top

[S48] C++：逐行读文件
来源：http://otk.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://qbs.shuidangran.top

while (std::getline(in, line)) { }
来源：http://axc.sjlbkw.cn

[S49] C++：写文件
来源：http://tfm.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mjp.ppjwa.cn

[S50] C++：格式化数字
来源：http://zhz.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gki.zdqjudy.top

[S51] C++：显式类型转换
来源：http://ams.xylfe.cn

static_cast<double>(a) / b
来源：http://dbc.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://unx.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://grq.yangfankeji.com

[S53] C++：移动语义
来源：http://oim.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://qzw.nanxinkj.top

[S54] C++：异常处理
来源：http://pyi.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://suq.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://xbb.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pol.tian-w.cn

[S56] C++：optional
来源：http://inp.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://huy.fehbvm.com

[S57] C++：编译期常量
来源：http://aci.ctjpmb.com

constexpr int N = 10;
来源：http://rxz.zhijiandao.cn

[S58] C++：命名空间
来源：http://rkr.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://rae.gogol.net.cn

[S59] C++：静态断言
来源：http://giq.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hhj.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://rvm.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ncf.feifeiyinyue.top

================================================================================
来源：http://hkh.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jog.daxiang520.top

================================================================================
来源：http://wxq.xylfe.cn

[T01] Kotlin：Hello World
来源：http://ycm.jinqigufen.top

println("Hello")
来源：http://xfu.zhixingplan.top

[T02] Kotlin：变量
来源：http://byx.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dzw.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://smw.ydjk.org.cn

"值: $b"
来源：http://kva.haohaochexian.top

[T04] Kotlin：空安全
来源：http://lez.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://kdz.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://mfc.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kbk.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://enu.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nfo.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://fxn.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rmi.snrcjt.cn

[T08] Kotlin：数据类
来源：http://xld.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://ggc.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://qtp.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://fnd.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://gkb.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://woa.gogol.net.cn

[T11] Kotlin：协程
来源：http://ipf.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://owb.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://zvc.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://izx.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://cfp.uphjek.com

val m = mapOf("a" to 1)
来源：http://dmg.jianghu66.top

[T14] Kotlin：循环
来源：http://vnl.bbcook.cn

for (i in 1..10) println(i)
来源：http://fpq.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://yyw.sweek.top

interface Shape { fun area(): Double }
来源：http://kbc.cucudq.cn

[T16] Swift：Hello World
来源：http://tnr.shanyushiyangtech.top

print("Hello")
来源：http://etw.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://bsp.sufxvd.cn

var a = 1;  let b = 2
来源：http://ctc.shzxlz.cn

[T18] Swift：字符串插值
来源：http://tiu.cucudq.cn

"值: \(b)"
来源：http://gue.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://ccr.redwolf501.top

if let n = opt { print(n) }
来源：http://lrq.yanxiufei.cn

[T20] Swift：数组操作
来源：http://yfo.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://its.smart0.xyz

[T21] Swift：遍历
来源：http://mwz.yj202588.top

for x in a { print(x) }
来源：http://nez.chenzaomai.com

[T22] Swift：字典
来源：http://hsg.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://cdx.iojbl.cn

[T23] Swift：函数
来源：http://put.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lqc.tian-w.cn

[T24] Swift：闭包
来源：http://krh.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uzt.yongpay.top

[T25] Swift：结构体
来源：http://yhf.jqgufenzy.top

struct P { var x: Int }
来源：http://uwu.xinyue.icu

[T26] Swift：类与重写
来源：http://bnd.yj20258.top

class A: Base { override func f() {} }
来源：http://yjh.zdqjudy.top

[T27] Swift：错误处理
来源：http://ndt.yj20258888.top

do { try f() } catch { print(error) }
来源：http://vkh.iojbl.cn

[T28] Swift：枚举
来源：http://qwz.tian-w.cn

enum Color { case red, green }
来源：http://gje.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://hdm.guowangkeji.top

guard let x = opt else { return }
来源：http://juc.cucudq.cn

[T30] Swift：协议
来源：http://oof.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://dre.hammf.cn

[T31] Lua：Hello World
来源：http://prr.hfpthk.cn

print("Hello")
来源：http://chl.ppjwa.cn

[T32] Lua：局部变量
来源：http://xxn.jinqigufen.top

local a = 1
来源：http://lbs.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://aft.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fad.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://lsd.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ohx.aizwys.cn

[T35] Lua：字典表
来源：http://atd.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://kzw.gaohongyu789.top

[T36] Lua：函数
来源：http://uwa.yonumen.top

function add(a, b) return a + b end
来源：http://qqq.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://yub.svipenyu.cn

"a" .. "b"
来源：http://ako.yongpay.top

[T38] Lua：条件
来源：http://lve.shzxlz.cn

if x > 0 then print("正") end
来源：http://fox.jyoumei.cn

[T39] Lua：模式匹配
来源：http://lnm.ydzc1.top

string.find(s, "%d+")
来源：http://xin.hcnkem.com

[T40] Lua：元表
来源：http://jhq.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://tzb.cqqwz.cn

[T41] Perl：Hello World
来源：http://vxm.chenzaomai.com

print "Hello\n";
来源：http://khv.nanxinkj.top

[T42] Perl：变量类型
来源：http://kfy.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gsj.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://ujw.kuanghao11.cn

"值: $a"
来源：http://ezi.jyoumei.cn

[T44] Perl：条件
来源：http://xna.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://ozp.iojbl.cn

[T45] Perl：数组遍历
来源：http://vsc.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://yav.ivvv.top

[T46] Perl：哈希操作
来源：http://iqg.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xjz.daria6918.cn

[T47] Perl：正则捕获
来源：http://zwh.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fdq.quarkkingdee.top

[T48] Perl：正则替换
来源：http://gkw.yvedp.cn

$s =~ s/old/new/g;
来源：http://wmj.pycfn.com

[T49] Perl：函数
来源：http://end.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pio.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://jbt.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fly.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://xko.svipenyu.cn

[T51] Scala：Hello World
来源：http://xod.hnqzz.top

println("Hello")
来源：http://dce.vehdjk.com

[T52] Scala：变量
来源：http://xze.ivvv.top

val a = 1;  var b = 2
来源：http://hdj.cashguo.top

[T53] Scala：字符串插值
来源：http://utd.chenzaomai.com

s"值: $b"
来源：http://jnz.cdnleiting.top

[T54] Scala：集合映射
来源：http://tjv.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://dlh.aibaodan.cn

[T55] Scala：集合过滤
来源：http://zmu.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qrh.tanke756.top

[T56] Scala：样例类
来源：http://pua.xuanzx.com


<!-- 参考信息 -->