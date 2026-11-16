代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://har.yangfankeji.com

[R54] 比较两个文件
来源：http://wes.fehbvm.com

diff a.txt b.txt
来源：http://ehk.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://ccj.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cqv.yueranfly.top

[R56] 远程拷贝
来源：http://jny.c1oappe.top

scp file user@host:/path/
来源：http://cfl.zhoulong.xyz

[R57] 远程执行命令
来源：http://jcx.iojbl.cn

ssh user@host 'uptime'
来源：http://hpi.jinqigufen.top

[R58] 下载文件
来源：http://hlo.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nwe.zhoulong.xyz

[R59] 发 POST JSON
来源：http://qdp.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jcp.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://vjd.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nth.xziqi.cn

[R61] 磁盘占用
来源：http://tyv.sysykeji.top

df -h;  du -sh *
来源：http://drx.smart0.xyz

[R62] 找最占空间的文件
来源：http://vmm.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://vfj.shangyingyoupin.top

[R63] 内存与进程
来源：http://suo.yj202588.top

free -h;  ps aux | grep nginx
来源：http://spx.birdmap.top

[R64] 结束进程
来源：http://kbh.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://xns.daria6918.cn

[R65] 查看端口占用
来源：http://kma.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rry.fktsv.cn

[R66] 定时任务
来源：http://iqq.snrcjt.cn

crontab -e;  crontab -l
来源：http://iyp.hammf.cn

[R67] 生成随机十六进制串
来源：http://oku.gogol.net.cn

openssl rand -hex 16
来源：http://jvw.epnwcf.com

[R68] 计算文件校验值
来源：http://jdo.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://leo.hnqzz.top

[R69] 生成随机密码
来源：http://iew.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://wtn.fengsongda.top

[R70] 时间戳与互转
来源：http://olo.yongpay.top

date +%s;  date -d @1700000000
来源：http://iht.jyoumei.cn

[R71] 日期格式化
来源：http://yrg.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ecv.snrcjt.cn

[R72] 等待端口就绪
来源：http://hpt.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://bzk.epnwcf.com

[R73] 分割大日志
来源：http://uda.fengsongda.top

split -l 1000 big.log part_
来源：http://itr.bjfxy.top

[R74] 批量重命名
来源：http://lyf.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dhb.gogol.net.cn

[R75] 导出环境变量
来源：http://mnu.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://ehn.gzhubu.top

[R76] 使用临时文件
来源：http://pfq.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bue.hnxiangtu.top

[R77] 读取用户输入
来源：http://gxl.kuanghao11.cn

read -rp "请输入: " ans
来源：http://iaq.mhx1999.top

[R78] 交互式菜单
来源：http://grw.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zpi.yongpay.top

[R79] 解析命令行选项
来源：http://edo.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yip.tarul.cn

[R80] 查看脚本执行耗时
来源：http://jwq.fengsongda.top

time ./run.sh
来源：http://uih.iojbl.cn

================================================================================
来源：http://jix.shuidangran.top

S. C / C++ 专题
来源：http://gwu.yonumen.top

================================================================================
来源：http://pip.fengsongda.top

[S01] C：Hello World
来源：http://izf.ivvv.top

#include <stdio.h>
来源：http://dol.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ewm.xylfe.cn

[S02] C：变量与格式化输出
来源：http://wzp.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://xud.guowangkeji.top

[S03] C：读入整数
来源：http://hoc.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://zvv.fktsv.cn

[S04] C：字符串复制
来源：http://mhe.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://aod.cqqwz.cn

[S05] C：字符串长度
来源：http://eop.pengpengdd.cyou

strlen(s)
来源：http://vmk.yongpay.top

[S06] C：字符串比较
来源：http://jaz.jinqigfzy.top

strcmp(a, b) == 0
来源：http://eqp.zycfv.cn

[S07] C：数组遍历求和
来源：http://qmc.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qjx.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://tja.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nsv.pycfn.com

[S09] C：结构体定义与初始化
来源：http://efm.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://doy.hesvh.cn

[S10] C：指针与解引用
来源：http://prd.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://spd.havefunace.top

[S11] C：逐行读文件
来源：http://lso.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://oof.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nna.yvedp.cn

fclose(f);
来源：http://rof.yj20258.top

[S12] C：写文件
来源：http://fmt.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vye.shanyushiyangtech.top

[S13] C：宏定义
来源：http://fjv.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ogg.shuidangran.top

[S14] C：枚举
来源：http://qwf.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://nnq.yvedp.cn

[S15] C：类型转换
来源：http://rng.fktsv.cn

(double) a / b
来源：http://iuv.hfpthk.cn

[S16] C：位操作置位
来源：http://dwt.snrcjt.cn

x |= (1 << 3);
来源：http://vun.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://cdd.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xyv.ydjk.org.cn

[S18] C：命令行参数
来源：http://neo.gotoacloud.top

int main(int argc, char **argv)
来源：http://uod.nanxinkj.top

[S19] C：快速排序
来源：http://ohc.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://paa.shzxlz.cn

[S20] C：二分查找
来源：http://mzf.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dws.shuidangran.top

[S21] C：字符类别判断
来源：http://zdx.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sdx.sxryk.cn

[S22] C：字符串转数字
来源：http://vfr.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qnp.jinqigufen.top

[S23] C：随机数
来源：http://ecq.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dxh.sjlbkw.cn

[S24] C：获取本地时间
来源：http://wmy.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nzd.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://xvp.bjfxy.top

memcpy(dst, src, n);
来源：http://noy.ybcxt.top

[S26] C：内存清零
来源：http://lgu.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://qwg.52xcode.cn

[S27] C：定义常量
来源：http://yrj.ctjpmb.com

const double PI = 3.14159;
来源：http://knh.haohaochexian.top

[S28] C：静态变量
来源：http://dlk.meibo888.top

static int counter = 0;
来源：http://qfg.birdmap.top

[S29] C：变参函数
来源：http://kjr.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bcu.chenjidiqi.icu

[S30] C：头文件保护
来源：http://xoz.shzxlz.cn

#ifndef X_H
来源：http://mrw.jlsjyb.cn

#define X_H
来源：http://faa.guowangkeji.top

#endif
来源：http://hja.chenzaomai.com

[S31] C++：Hello World
来源：http://uis.zhoulong.xyz

#include <iostream>
来源：http://wmb.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tna.hfpthk.cn

[S32] C++：字符串
来源：http://vks.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://hgn.mhx1999.top

[S33] C++：vector 增删
来源：http://kif.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pqp.yuanzhike.top

[S34] C++：遍历 vector
来源：http://pcs.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://bje.birdmap.top

[S35] C++：map
来源：http://dem.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aug.uphjek.com

[S36] C++：unordered_map
来源：http://uzo.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aaq.cucudq.cn

[S37] C++：set
来源：http://opb.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukh.ppjwa.cn

[S38] C++：排序
来源：http://cuv.uphjek.com

std::sort(v.begin(), v.end());
来源：http://nut.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://puv.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wvl.yonumen.top

[S40] C++：查找元素
来源：http://hln.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwf.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://xna.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nxe.gzhubu.top

[S42] C++：继承与虚函数
来源：http://ohb.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://hne.fktsv.cn

[S43] C++：智能指针
来源：http://qql.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://pan.jinqigfzy.top

[S44] C++：引用传参
来源：http://lsj.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://bjh.hysaishi.cn

[S45] C++：lambda
来源：http://goc.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://had.jlsjyb.cn

[S46] C++：函数模板
来源：http://tos.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rda.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://iuj.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wkd.guowangkeji.top

[S48] C++：逐行读文件
来源：http://zom.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wth.aizwys.cn

while (std::getline(in, line)) { }
来源：http://eee.xinyue.icu

[S49] C++：写文件
来源：http://tgd.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nfs.iojbl.cn

[S50] C++：格式化数字
来源：http://ugf.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aiu.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://jcc.shuidangran.top

static_cast<double>(a) / b
来源：http://eox.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://bkf.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://ceg.ydjk.org.cn

[S53] C++：移动语义
来源：http://lxu.yj20258.top

std::vector<int> w = std::move(v);
来源：http://rcc.ydjk.org.cn

[S54] C++：异常处理
来源：http://sxa.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jeb.shzxlz.cn

[S55] C++：结构化绑定
来源：http://tus.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://fan.shanyushiyangtech.top

[S56] C++：optional
来源：http://stg.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://euv.ybcxt.top

[S57] C++：编译期常量
来源：http://sff.0kj1m.cn

constexpr int N = 10;
来源：http://azy.yj20258.top

[S58] C++：命名空间
来源：http://zxz.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://aqp.sufxvd.cn

[S59] C++：静态断言
来源：http://hay.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://trd.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://idw.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jxa.zhengqikj.top

================================================================================
来源：http://mof.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ksd.cucudq.cn

================================================================================
来源：http://hjc.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://zgl.yangfankeji.com

println("Hello")
来源：http://eng.andypj.xyz

[T02] Kotlin：变量
来源：http://qnh.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tuh.uphjek.com

[T03] Kotlin：字符串模板
来源：http://gjz.daria6918.cn

"值: $b"
来源：http://mvq.cdnleiting.top

[T04] Kotlin：空安全
来源：http://lhu.guannengcc.top

val n: String? = null;  n?.length
来源：http://agu.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://voj.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qyy.cashguo.top

[T06] Kotlin：集合映射
来源：http://keb.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://upx.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://gym.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uiq.fengsongda.top

[T08] Kotlin：数据类
来源：http://hht.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://crw.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://isl.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://gaw.sweek.top

[T10] Kotlin：默认参数
来源：http://fbh.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cgn.tianlin.xyz

[T11] Kotlin：协程
来源：http://tks.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://usf.hammf.cn

[T12] Kotlin：解构声明
来源：http://trb.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://acv.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://qvl.fengsongda.top

val m = mapOf("a" to 1)
来源：http://bpn.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://hio.nanxinkj.top

for (i in 1..10) println(i)
来源：http://ere.birdmap.top

[T15] Kotlin：接口
来源：http://vza.daxiang520.top

interface Shape { fun area(): Double }
来源：http://eyu.xziqi.cn

[T16] Swift：Hello World
来源：http://qwc.cdnleiting.top

print("Hello")
来源：http://jaa.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://ujm.haohaochexian.top

var a = 1;  let b = 2
来源：http://mkg.tarul.cn

[T18] Swift：字符串插值
来源：http://cjh.gogol.net.cn

"值: \(b)"
来源：http://gtn.jyoumei.cn

[T19] Swift：可选绑定
来源：http://psy.yj202588.top

if let n = opt { print(n) }
来源：http://lcs.zhengqikj.top

[T20] Swift：数组操作
来源：http://swc.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sgu.316326.xyz

[T21] Swift：遍历
来源：http://koe.yj20258888.top

for x in a { print(x) }
来源：http://jxh.quarkkingdee.top

[T22] Swift：字典
来源：http://xzh.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lpj.yonumen.top

[T23] Swift：函数
来源：http://kln.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bpe.yuanzhike.top

[T24] Swift：闭包
来源：http://qjz.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gtr.dianchejie.cn

[T25] Swift：结构体
来源：http://seo.yuxming.cn

struct P { var x: Int }
来源：http://nds.uphjek.com

[T26] Swift：类与重写
来源：http://hpp.tianlin.xyz

class A: Base { override func f() {} }
来源：http://kco.nanxinkj.top

[T27] Swift：错误处理
来源：http://lcd.birdmap.top

do { try f() } catch { print(error) }
来源：http://zkk.vehdjk.com

[T28] Swift：枚举
来源：http://psh.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://ztv.cheryme.top

[T29] Swift：guard 提前返回
来源：http://zgg.yj20258888.top

guard let x = opt else { return }
来源：http://adi.mhx1999.top

[T30] Swift：协议
来源：http://yqv.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://ocg.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://web.ydjk.org.cn

print("Hello")
来源：http://qar.chenzaomai.com

[T32] Lua：局部变量
来源：http://wso.kuanghao11.cn

local a = 1
来源：http://exr.mhx1999.top

[T33] Lua：表（数组）
来源：http://usr.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dbq.redwolf501.top

[T34] Lua：遍历表
来源：http://waf.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xqo.9152youxi.cn

[T35] Lua：字典表
来源：http://cqi.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://gxx.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://ect.yuxming.cn

function add(a, b) return a + b end
来源：http://gxq.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://yci.daria6918.cn

"a" .. "b"
来源：http://etq.smart0.xyz

[T38] Lua：条件
来源：http://pot.zhoulong.xyz

if x > 0 then print("正") end
来源：http://atv.shzxlz.cn

[T39] Lua：模式匹配
来源：http://xic.zhongyouzk.top

string.find(s, "%d+")
来源：http://pie.hammf.cn

[T40] Lua：元表
来源：http://uts.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://baq.c1oappe.top

[T41] Perl：Hello World
来源：http://sxw.sxryk.cn

print "Hello\n";
来源：http://ecq.uphjek.com

[T42] Perl：变量类型
来源：http://vrh.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rrm.0kj1m.cn

[T43] Perl：字符串插值
来源：http://ueg.xuetiantiany.cn

"值: $a"
来源：http://dzf.xylfe.cn

[T44] Perl：条件
来源：http://sfr.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://yxv.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://pak.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://whz.nwbrower.top

[T46] Perl：哈希操作
来源：http://nqx.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xvq.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://pvx.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ggw.0kj1m.cn

[T48] Perl：正则替换
来源：http://txh.52xcode.cn

$s =~ s/old/new/g;
来源：http://gxi.xuanzx.com

[T49] Perl：函数
来源：http://zpu.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xve.andypj.xyz

[T50] Perl：逐行读文件
来源：http://wje.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uqu.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://kll.redwolf501.top

[T51] Scala：Hello World
来源：http://kkp.gogol.net.cn

println("Hello")
来源：http://exw.mhx1999.top

[T52] Scala：变量
来源：http://bkp.zhongyouzk.top

val a = 1;  var b = 2
来源：http://phu.cdnleiting.top

[T53] Scala：字符串插值
来源：http://ttd.yj20258.top

s"值: $b"
来源：http://oen.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://veu.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://mrg.gotoacloud.top

[T55] Scala：集合过滤
来源：http://prt.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://pcu.cqqwz.cn

[T56] Scala：样例类
来源：http://uhr.52xcode.cn


<!-- 参考信息 -->