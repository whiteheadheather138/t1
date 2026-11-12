代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oko.svipenyu.cn

[R56] 远程拷贝
来源：http://mrj.haohaochexian.top

scp file user@host:/path/
来源：http://zmb.yongpay.top

[R57] 远程执行命令
来源：http://lzc.jinqigfzy.top

ssh user@host 'uptime'
来源：http://hfq.sweek.top

[R58] 下载文件
来源：http://kfu.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://htu.zhijiandao.cn

[R59] 发 POST JSON
来源：http://ndb.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsg.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://fta.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://avy.wangdashe.top

[R61] 磁盘占用
来源：http://amg.uphjek.com

df -h;  du -sh *
来源：http://zoe.xuanzx.com

[R62] 找最占空间的文件
来源：http://yns.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://edw.nanxuanxn.top

[R63] 内存与进程
来源：http://xwg.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://ffa.sysykeji.top

[R64] 结束进程
来源：http://mug.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://ecb.guowangkeji.top

[R65] 查看端口占用
来源：http://toh.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjd.andypj.xyz

[R66] 定时任务
来源：http://ayp.haohaochexian.top

crontab -e;  crontab -l
来源：http://qsg.hammf.cn

[R67] 生成随机十六进制串
来源：http://dzq.guowangkeji.top

openssl rand -hex 16
来源：http://mzb.wangdashe.top

[R68] 计算文件校验值
来源：http://asu.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://knq.nanxinkj.top

[R69] 生成随机密码
来源：http://rke.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://drc.yfazqb.com

[R70] 时间戳与互转
来源：http://bbm.bbcook.cn

date +%s;  date -d @1700000000
来源：http://wjn.zdbjq.cn

[R71] 日期格式化
来源：http://gkv.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccb.zhijiandao.cn

[R72] 等待端口就绪
来源：http://tzb.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ixw.andypj.xyz

[R73] 分割大日志
来源：http://pxe.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://izi.fzhhl.top

[R74] 批量重命名
来源：http://vyp.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://obx.shuidangran.top

[R75] 导出环境变量
来源：http://hob.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://tvt.ydzc1.top

[R76] 使用临时文件
来源：http://ioy.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://smy.zhijiandao.cn

[R77] 读取用户输入
来源：http://vvb.cdnleiting.top

read -rp "请输入: " ans
来源：http://nwi.tian-w.cn

[R78] 交互式菜单
来源：http://hxc.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uhf.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://qjc.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nlo.cheryme.top

[R80] 查看脚本执行耗时
来源：http://xhn.yuxming.cn

time ./run.sh
来源：http://bll.yueranfly.top

================================================================================
来源：http://aan.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://guz.gzhubu.top

================================================================================
来源：http://ggh.andypj.xyz

[S01] C：Hello World
来源：http://aio.zhijiandao.cn

#include <stdio.h>
来源：http://zui.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymp.yuxming.cn

[S02] C：变量与格式化输出
来源：http://was.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://jzb.zhengqikj.top

[S03] C：读入整数
来源：http://iej.jiagoushi.top

int x; scanf("%d", &x);
来源：http://jvy.pycfn.com

[S04] C：字符串复制
来源：http://tqg.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://xtt.sjlbkw.cn

[S05] C：字符串长度
来源：http://ewh.aizwys.cn

strlen(s)
来源：http://wua.sxryk.cn

[S06] C：字符串比较
来源：http://xyn.fengsongda.top

strcmp(a, b) == 0
来源：http://syo.daria6918.cn

[S07] C：数组遍历求和
来源：http://ggr.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sko.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://lth.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rbp.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://wke.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tmx.tian-w.cn

[S10] C：指针与解引用
来源：http://cuv.gzhubu.top

int *p = &a;  *p = 5;
来源：http://ese.gaohongyu789.top

[S11] C：逐行读文件
来源：http://fyj.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://mza.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://tic.kuanghao11.cn

fclose(f);
来源：http://yol.wangdashe.top

[S12] C：写文件
来源：http://uqg.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://koh.zhiwuduotai.top

[S13] C：宏定义
来源：http://yhs.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lfp.shangyingyoupin.top

[S14] C：枚举
来源：http://sgq.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://cxg.nanxuanxn.top

[S15] C：类型转换
来源：http://hpa.ehwqpu.com

(double) a / b
来源：http://szn.fehbvm.com

[S16] C：位操作置位
来源：http://ned.cucudq.cn

x |= (1 << 3);
来源：http://qyn.yj20258.top

[S17] C：安全拼接字符串
来源：http://cdd.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bgx.havefunace.top

[S18] C：命令行参数
来源：http://mqj.shuidangran.top

int main(int argc, char **argv)
来源：http://qnu.shzxlz.cn

[S19] C：快速排序
来源：http://jhn.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://jfp.ppjwa.cn

[S20] C：二分查找
来源：http://xzq.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://noe.gotoacloud.top

[S21] C：字符类别判断
来源：http://mcg.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xmb.yuxming.cn

[S22] C：字符串转数字
来源：http://ome.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://qxg.ivvv.top

[S23] C：随机数
来源：http://ioc.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dpi.chenzaomai.com

[S24] C：获取本地时间
来源：http://opg.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nex.guowangkeji.top

[S25] C：内存拷贝
来源：http://xau.guowangkeji.top

memcpy(dst, src, n);
来源：http://ofw.hammf.cn

[S26] C：内存清零
来源：http://nnc.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://qiz.sufxvd.cn

[S27] C：定义常量
来源：http://nij.wangshuangyany.cn

const double PI = 3.14159;
来源：http://qch.wangshuangyany.cn

[S28] C：静态变量
来源：http://cxq.tianlin.xyz

static int counter = 0;
来源：http://nqn.jianghu66.top

[S29] C：变参函数
来源：http://ent.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ksk.dianchejie.cn

[S30] C：头文件保护
来源：http://ysv.cqqwz.cn

#ifndef X_H
来源：http://xbt.gotoacloud.top

#define X_H
来源：http://ajv.hammf.cn

#endif
来源：http://fil.gaohongyu789.top

[S31] C++：Hello World
来源：http://mgr.nanxinkj.top

#include <iostream>
来源：http://ror.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://nbq.chenlongwang.top

[S32] C++：字符串
来源：http://mwj.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://ass.jqgfzy.top

[S33] C++：vector 增删
来源：http://hwd.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gsm.yj202588.top

[S34] C++：遍历 vector
来源：http://jwo.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://ohz.hysaishi.cn

[S35] C++：map
来源：http://lmq.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thh.yvedp.cn

[S36] C++：unordered_map
来源：http://alm.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dnx.chenjidiqi.icu

[S37] C++：set
来源：http://otm.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vjk.zdbjq.cn

[S38] C++：排序
来源：http://sqq.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://fiv.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ohj.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ifz.daxiang520.top

[S40] C++：查找元素
来源：http://nfr.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qyy.hysaishi.cn

[S41] C++：类与构造函数
来源：http://hwy.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wiz.ydzc1.top

[S42] C++：继承与虚函数
来源：http://vmz.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://zpk.jqgufenzy.top

[S43] C++：智能指针
来源：http://mde.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://kci.yonumen.top

[S44] C++：引用传参
来源：http://ozn.meibo888.top

void inc(int &x) { ++x; }
来源：http://edh.nanxuanxn.top

[S45] C++：lambda
来源：http://wrg.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://axo.havefunace.top

[S46] C++：函数模板
来源：http://ebm.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tmb.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://tpt.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgi.hnqzz.top

[S48] C++：逐行读文件
来源：http://emm.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://tga.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://kuf.hongshengwenyu.top

[S49] C++：写文件
来源：http://kep.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hjd.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://mrd.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fgz.guowangkeji.top

[S51] C++：显式类型转换
来源：http://qaq.c1oappe.top

static_cast<double>(a) / b
来源：http://rsd.ivvv.top

[S52] C++：const 与 noexcept
来源：http://cvt.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://cqb.andypj.xyz

[S53] C++：移动语义
来源：http://fdt.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://tte.zhengqikj.top

[S54] C++：异常处理
来源：http://vog.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvf.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://rtj.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lte.jlsjyb.cn

[S56] C++：optional
来源：http://cok.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://diq.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://mpg.gzhubu.top

constexpr int N = 10;
来源：http://eud.chenzaomai.com

[S58] C++：命名空间
来源：http://yya.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://fzl.jinqigfzy.top

[S59] C++：静态断言
来源：http://pvy.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://njf.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://lga.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vrs.svipenyu.cn

================================================================================
来源：http://fhb.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qeq.chenlongwang.top

================================================================================
来源：http://vhn.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://aza.uphjek.com

println("Hello")
来源：http://nkt.guannengcc.top

[T02] Kotlin：变量
来源：http://kbr.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mii.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://qdf.guannengcc.top

"值: $b"
来源：http://ljm.fengsongda.top

[T04] Kotlin：空安全
来源：http://fve.redwolf501.top

val n: String? = null;  n?.length
来源：http://gou.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://hyf.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vuk.yuxming.cn

[T06] Kotlin：集合映射
来源：http://ldf.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eyh.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://pqn.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdl.hnqzz.top

[T08] Kotlin：数据类
来源：http://pda.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://moz.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://yuz.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://aeg.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://obh.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://crj.yfazqb.com

[T11] Kotlin：协程
来源：http://fqj.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pjm.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://jee.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://ofi.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://xml.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://hqh.cashguo.top

[T14] Kotlin：循环
来源：http://rjg.iojbl.cn

for (i in 1..10) println(i)
来源：http://gtm.52xcode.cn

[T15] Kotlin：接口
来源：http://pkv.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://dlv.hammf.cn

[T16] Swift：Hello World
来源：http://kea.shanyushiyangkeji.top

print("Hello")
来源：http://nte.snrcjt.cn

[T17] Swift：变量与常量
来源：http://zgq.316326.xyz

var a = 1;  let b = 2
来源：http://mxp.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://hje.cdnleiting.top

"值: \(b)"
来源：http://ipf.cdnleiting.top

[T19] Swift：可选绑定
来源：http://smc.tianlin.xyz

if let n = opt { print(n) }
来源：http://fea.redwolf501.top

[T20] Swift：数组操作
来源：http://zln.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yve.hysaishi.cn

[T21] Swift：遍历
来源：http://gpx.shzxlz.cn

for x in a { print(x) }
来源：http://zgd.nanxuanxn.top

[T22] Swift：字典
来源：http://gho.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://zdv.sweek.top

[T23] Swift：函数
来源：http://ctt.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kka.aibaodan.cn

[T24] Swift：闭包
来源：http://ypn.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bws.yonumen.top

[T25] Swift：结构体
来源：http://tsr.yangfankeji.com

struct P { var x: Int }
来源：http://dzd.vehdjk.com

[T26] Swift：类与重写
来源：http://cno.snrcjt.cn

class A: Base { override func f() {} }
来源：http://xhd.hammf.cn

[T27] Swift：错误处理
来源：http://xwl.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://uno.quarkkingdee.top

[T28] Swift：枚举
来源：http://wsi.shangyingyoupin.top

enum Color { case red, green }
来源：http://yqo.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://wwx.snrcjt.cn

guard let x = opt else { return }
来源：http://qhh.fzhhl.top

[T30] Swift：协议
来源：http://lcd.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://fdo.daxiang520.top

[T31] Lua：Hello World
来源：http://mbn.xziqi.cn

print("Hello")
来源：http://bak.fengsongda.top

[T32] Lua：局部变量
来源：http://prt.yuanzhike.top

local a = 1
来源：http://tsm.andypj.xyz

[T33] Lua：表（数组）
来源：http://ooo.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yje.c1oappe.top

[T34] Lua：遍历表
来源：http://fpk.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oes.316326.xyz

[T35] Lua：字典表
来源：http://bwj.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://reo.birdmap.top

[T36] Lua：函数
来源：http://wmh.ydjk.org.cn

function add(a, b) return a + b end
来源：http://cpl.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://qoz.gotoacloud.top

"a" .. "b"
来源：http://gsi.xuetiantiany.cn

[T38] Lua：条件
来源：http://inc.ydjk.org.cn

if x > 0 then print("正") end
来源：http://xel.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://ybv.zycfv.cn

string.find(s, "%d+")
来源：http://lwd.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://gpx.hesvh.cn

setmetatable({}, { __index = base })
来源：http://vgg.quarkkingdee.top

[T41] Perl：Hello World
来源：http://adp.dashuyun.cn

print "Hello\n";
来源：http://rwl.zhengqikj.top

[T42] Perl：变量类型
来源：http://sdl.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tix.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://lki.tian-w.cn

"值: $a"
来源：http://vhn.nwbrower.top

[T44] Perl：条件
来源：http://dts.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://ljd.tanke756.top

[T45] Perl：数组遍历
来源：http://dag.yonumen.top

for my $x (@arr) { print $x; }
来源：http://gie.c1oappe.top

[T46] Perl：哈希操作
来源：http://wnh.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hhg.dashuyun.cn

[T47] Perl：正则捕获
来源：http://ggh.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zxb.yueranfly.top

[T48] Perl：正则替换
来源：http://qip.sweek.top

$s =~ s/old/new/g;
来源：http://ndz.xinyue.icu

[T49] Perl：函数
来源：http://fcu.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mgn.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://dpz.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xiq.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://tig.yonumen.top

[T51] Scala：Hello World
来源：http://rfr.tian-w.cn

println("Hello")
来源：http://sya.0kj1m.cn

[T52] Scala：变量
来源：http://ocg.yanxiufei.cn

val a = 1;  var b = 2
来源：http://hdd.fengsongda.top

[T53] Scala：字符串插值
来源：http://goy.yj20258.top

s"值: $b"
来源：http://ane.hfpthk.cn

[T54] Scala：集合映射
来源：http://svo.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://jjg.zdqjudy.top

[T55] Scala：集合过滤
来源：http://mjr.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://akz.yvedp.cn

[T56] Scala：样例类
来源：http://yzq.fktsv.cn

case class User(name: String, age: Int)
来源：http://znm.ctjpmb.com

[T57] Scala：模式匹配
来源：http://mvl.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://wtl.gaohongyu789.top

[T58] Scala：函数定义
来源：http://igr.hesvh.cn


<!-- 参考信息 -->