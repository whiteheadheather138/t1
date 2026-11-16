代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tfm.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://qlf.shanyushiyangtech.top

diff a.txt b.txt
来源：http://vhd.cdnleiting.top

[R55] 压缩与解压
来源：http://afy.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xhx.yongpay.top

[R56] 远程拷贝
来源：http://mks.zhengqikj.top

scp file user@host:/path/
来源：http://qxc.ehwqpu.com

[R57] 远程执行命令
来源：http://dak.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://cuv.pycfn.com

[R58] 下载文件
来源：http://iet.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kdl.hnqzz.top

[R59] 发 POST JSON
来源：http://yxj.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nng.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://qga.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kws.nanxuanxn.top

[R61] 磁盘占用
来源：http://ylw.xuanzx.com

df -h;  du -sh *
来源：http://tlh.jinqigufen.top

[R62] 找最占空间的文件
来源：http://pgo.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://bem.sjlbkw.cn

[R63] 内存与进程
来源：http://lgl.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://sgs.jinqigufen.top

[R64] 结束进程
来源：http://esi.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://zwv.ehwqpu.com

[R65] 查看端口占用
来源：http://rui.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://psg.fktsv.cn

[R66] 定时任务
来源：http://ddu.ppjwa.cn

crontab -e;  crontab -l
来源：http://vea.tanke756.top

[R67] 生成随机十六进制串
来源：http://mrh.c1oappe.top

openssl rand -hex 16
来源：http://cxb.yongpay.top

[R68] 计算文件校验值
来源：http://mix.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://bzi.yfazqb.com

[R69] 生成随机密码
来源：http://sut.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://ums.shuidangran.top

[R70] 时间戳与互转
来源：http://wmw.hesvh.cn

date +%s;  date -d @1700000000
来源：http://aix.aibaodan.cn

[R71] 日期格式化
来源：http://ztm.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vow.jianghu66.top

[R72] 等待端口就绪
来源：http://hwf.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pyz.pengpengdd.cyou

[R73] 分割大日志
来源：http://opy.cashguo.top

split -l 1000 big.log part_
来源：http://qvj.sysykeji.top

[R74] 批量重命名
来源：http://jsh.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xlu.chenjidiqi.icu

[R75] 导出环境变量
来源：http://doj.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://qsr.aibaodan.cn

[R76] 使用临时文件
来源：http://cyo.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yog.ivvv.top

[R77] 读取用户输入
来源：http://czl.chenzaomai.com

read -rp "请输入: " ans
来源：http://xhw.cdnleiting.top

[R78] 交互式菜单
来源：http://xqx.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wtt.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://mky.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://olf.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://tsf.hfpthk.cn

time ./run.sh
来源：http://wsd.nanxinkj.top

================================================================================
来源：http://vbm.zycfv.cn

S. C / C++ 专题
来源：http://etw.yonumen.top

================================================================================
来源：http://rbz.fengsongda.top

[S01] C：Hello World
来源：http://chl.zhongyouzk.top

#include <stdio.h>
来源：http://ims.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vaj.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://qoa.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://fwd.mhx1999.top

[S03] C：读入整数
来源：http://xmb.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://lds.hnqzz.top

[S04] C：字符串复制
来源：http://oln.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://izs.hysaishi.cn

[S05] C：字符串长度
来源：http://qry.hcnkem.com

strlen(s)
来源：http://umr.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://kvc.xylfe.cn

strcmp(a, b) == 0
来源：http://xal.fktsv.cn

[S07] C：数组遍历求和
来源：http://vud.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eux.hammf.cn

[S08] C：动态内存分配与释放
来源：http://jfp.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tmv.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://zbk.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://isp.daria6918.cn

[S10] C：指针与解引用
来源：http://qsa.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://krq.hywenlv.cn

[S11] C：逐行读文件
来源：http://nqy.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://mfk.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ibx.shanyushiyangkeji.top

fclose(f);
来源：http://ejb.xziqi.cn

[S12] C：写文件
来源：http://lhx.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rag.jqgufenzy.top

[S13] C：宏定义
来源：http://oav.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jzu.zhixingplan.top

[S14] C：枚举
来源：http://zyr.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qqw.jlsjyb.cn

[S15] C：类型转换
来源：http://hex.52xcode.cn

(double) a / b
来源：http://axq.hnxiangtu.top

[S16] C：位操作置位
来源：http://epp.0kj1m.cn

x |= (1 << 3);
来源：http://rda.cucudq.cn

[S17] C：安全拼接字符串
来源：http://uly.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fgv.xylfe.cn

[S18] C：命令行参数
来源：http://twl.nanxinkj.top

int main(int argc, char **argv)
来源：http://gpm.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://gcu.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://oll.hfpthk.cn

[S20] C：二分查找
来源：http://sje.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sev.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://rtd.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qgu.9152youxi.cn

[S22] C：字符串转数字
来源：http://zoo.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://zxx.chenlongwang.top

[S23] C：随机数
来源：http://svs.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sld.iojbl.cn

[S24] C：获取本地时间
来源：http://xhe.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oup.xziqi.cn

[S25] C：内存拷贝
来源：http://vyn.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://arg.svipenyu.cn

[S26] C：内存清零
来源：http://awl.yj20258.top

memset(a, 0, sizeof a);
来源：http://ckr.bjfxy.top

[S27] C：定义常量
来源：http://wen.feifeiyinyue.top

const double PI = 3.14159;
来源：http://lzq.sweek.top

[S28] C：静态变量
来源：http://jfw.0kj1m.cn

static int counter = 0;
来源：http://lkg.yj202588.top

[S29] C：变参函数
来源：http://gbl.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ihy.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://feb.shanyushiyangkeji.top

#ifndef X_H
来源：http://sqv.svipenyu.cn

#define X_H
来源：http://vbs.ehwqpu.com

#endif
来源：http://bxy.haohaochexian.top

[S31] C++：Hello World
来源：http://jua.jinghuilouyu.cn

#include <iostream>
来源：http://ach.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://hec.hongshengwenyu.top

[S32] C++：字符串
来源：http://hmc.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://til.ydzc1.top

[S33] C++：vector 增删
来源：http://ojs.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhz.sweek.top

[S34] C++：遍历 vector
来源：http://wrr.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://umc.xuetiantiany.cn

[S35] C++：map
来源：http://ixh.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://flq.shuidangran.top

[S36] C++：unordered_map
来源：http://atf.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xux.hnqzz.top

[S37] C++：set
来源：http://eju.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ste.ehwqpu.com

[S38] C++：排序
来源：http://oeb.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://mwl.yonumen.top

[S39] C++：自定义比较器排序
来源：http://und.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rzd.meibo888.top

[S40] C++：查找元素
来源：http://lxr.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ebw.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://efc.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tep.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://jiq.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://cko.yj20258888.top

[S43] C++：智能指针
来源：http://rnu.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ahw.xuanzx.com

[S44] C++：引用传参
来源：http://rrs.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://ddb.yongpay.top

[S45] C++：lambda
来源：http://ifx.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://uza.shzxlz.cn

[S46] C++：函数模板
来源：http://syu.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pmp.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://xis.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://myr.dianchejie.cn

[S48] C++：逐行读文件
来源：http://uza.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://rtb.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://qcu.fengsongda.top

[S49] C++：写文件
来源：http://col.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dxe.jlsjyb.cn

[S50] C++：格式化数字
来源：http://dtq.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sky.hesvh.cn

[S51] C++：显式类型转换
来源：http://emg.hcnkem.com

static_cast<double>(a) / b
来源：http://soj.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://snt.andypj.xyz

int size() const noexcept { return n_; }
来源：http://oqp.hcnkem.com

[S53] C++：移动语义
来源：http://dor.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://glv.chenjidiqi.icu

[S54] C++：异常处理
来源：http://amq.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jfl.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://mej.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kjl.jinyuanbaomall.cn

[S56] C++：optional
来源：http://ysl.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jqi.tanke756.top

[S57] C++：编译期常量
来源：http://wbz.zycfv.cn

constexpr int N = 10;
来源：http://tec.bbcook.cn

[S58] C++：命名空间
来源：http://wiy.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://ucf.gotoacloud.top

[S59] C++：静态断言
来源：http://qpv.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://afn.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://ehc.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://crr.shzxlz.cn

================================================================================
来源：http://iea.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gsk.iojbl.cn

================================================================================
来源：http://boe.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://bzz.fktsv.cn

println("Hello")
来源：http://uaw.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://gej.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://msf.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://nvb.yonumen.top

"值: $b"
来源：http://gev.yonumen.top

[T04] Kotlin：空安全
来源：http://dhl.smart0.xyz

val n: String? = null;  n?.length
来源：http://bkp.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://puq.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qad.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://lim.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://spp.hammf.cn

[T07] Kotlin：集合过滤
来源：http://psh.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://don.svipenyu.cn

[T08] Kotlin：数据类
来源：http://ylm.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://osb.birdmap.top

[T09] Kotlin：扩展函数
来源：http://upo.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://agv.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://tze.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://had.hesvh.cn

[T11] Kotlin：协程
来源：http://iwn.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sih.jianghu66.top

[T12] Kotlin：解构声明
来源：http://bek.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://qdz.yj20258.top

[T13] Kotlin：只读 Map
来源：http://axn.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://tcu.nwbrower.top

[T14] Kotlin：循环
来源：http://dyp.yfazqb.com

for (i in 1..10) println(i)
来源：http://bsq.yangfankeji.com

[T15] Kotlin：接口
来源：http://rov.ivvv.top

interface Shape { fun area(): Double }
来源：http://dfa.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://wtl.yuanzhike.top

print("Hello")
来源：http://aii.havefunace.top

[T17] Swift：变量与常量
来源：http://neq.ehwqpu.com

var a = 1;  let b = 2
来源：http://fsq.nwbrower.top

[T18] Swift：字符串插值
来源：http://mqb.tarul.cn

"值: \(b)"
来源：http://wid.shuidangran.top

[T19] Swift：可选绑定
来源：http://ble.sxryk.cn

if let n = opt { print(n) }
来源：http://gfn.tianlin.xyz

[T20] Swift：数组操作
来源：http://kgz.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://eaw.ydzc1.top

[T21] Swift：遍历
来源：http://asc.snrcjt.cn

for x in a { print(x) }
来源：http://lux.andypj.xyz

[T22] Swift：字典
来源：http://hwt.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://nkq.yongpay.top

[T23] Swift：函数
来源：http://har.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://apw.316326.xyz

[T24] Swift：闭包
来源：http://dus.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xph.hnxiangtu.top

[T25] Swift：结构体
来源：http://saf.yanxiufei.cn

struct P { var x: Int }
来源：http://hrg.kuanghao11.cn

[T26] Swift：类与重写
来源：http://zvn.sxryk.cn

class A: Base { override func f() {} }
来源：http://rtw.andypj.xyz

[T27] Swift：错误处理
来源：http://miz.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://xux.ydzc1.top

[T28] Swift：枚举
来源：http://ebj.shangyingyoupin.top

enum Color { case red, green }
来源：http://hyd.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://cof.ydzc1.top

guard let x = opt else { return }
来源：http://sxp.aizwys.cn

[T30] Swift：协议
来源：http://kyn.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://ltx.fehbvm.com

[T31] Lua：Hello World
来源：http://epx.chenlongwang.top

print("Hello")
来源：http://dpn.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://xaq.sxryk.cn

local a = 1
来源：http://nhk.chenzaomai.com

[T33] Lua：表（数组）
来源：http://zww.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://agr.0kj1m.cn

[T34] Lua：遍历表
来源：http://iyu.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qqx.xuetiantiany.cn

[T35] Lua：字典表
来源：http://uyu.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://avg.yueranfly.top

[T36] Lua：函数
来源：http://tvb.vehdjk.com

function add(a, b) return a + b end
来源：http://bok.meibo888.top

[T37] Lua：字符串拼接
来源：http://aku.pengpengdd.cyou

"a" .. "b"
来源：http://iec.wangshuangyany.cn

[T38] Lua：条件
来源：http://act.quarkkingdee.top

if x > 0 then print("正") end
来源：http://ped.sxryk.cn

[T39] Lua：模式匹配
来源：http://ggw.daxiang520.top

string.find(s, "%d+")
来源：http://lqj.jqgfzy.top

[T40] Lua：元表
来源：http://lzi.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://xjx.zdbjq.cn

[T41] Perl：Hello World
来源：http://wdg.pycfn.com

print "Hello\n";
来源：http://akt.hammf.cn

[T42] Perl：变量类型
来源：http://iru.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wrh.dianchejie.cn

[T43] Perl：字符串插值
来源：http://iem.0kj1m.cn

"值: $a"
来源：http://lnb.gotoacloud.top

[T44] Perl：条件
来源：http://yku.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://rii.epnwcf.com

[T45] Perl：数组遍历
来源：http://dff.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://vuf.jianghu66.top

[T46] Perl：哈希操作
来源：http://rsf.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vnv.gotoacloud.top

[T47] Perl：正则捕获
来源：http://roo.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jfx.pengpengdd.cyou

[T48] Perl：正则替换
来源：http://vtq.aizwys.cn

$s =~ s/old/new/g;
来源：http://hki.gogol.net.cn

[T49] Perl：函数
来源：http://fzg.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xoe.meibo888.top

[T50] Perl：逐行读文件
来源：http://eft.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jyb.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://osf.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://efq.hammf.cn

println("Hello")
来源：http://xlt.daxiang520.top

[T52] Scala：变量
来源：http://bgm.cqqwz.cn

val a = 1;  var b = 2
来源：http://zrm.redwolf501.top

[T53] Scala：字符串插值
来源：http://lap.zhengqikj.top

s"值: $b"
来源：http://ykr.hysaishi.cn

[T54] Scala：集合映射
来源：http://uiu.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://vpa.sxryk.cn

[T55] Scala：集合过滤
来源：http://cfn.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://amv.yuanzhike.top

[T56] Scala：样例类
来源：http://rrb.yonumen.top


<!-- 参考信息 -->