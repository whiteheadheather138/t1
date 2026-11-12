代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jzc.zhengqikj.top

[R56] 远程拷贝
来源：http://cha.svipenyu.cn

scp file user@host:/path/
来源：http://xqr.quarkkingdee.top

[R57] 远程执行命令
来源：http://rrc.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://djz.xziqi.cn

[R58] 下载文件
来源：http://trt.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vjr.tian-w.cn

[R59] 发 POST JSON
来源：http://euh.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ric.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://dtt.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gdt.ivvv.top

[R61] 磁盘占用
来源：http://oxb.ctjpmb.com

df -h;  du -sh *
来源：http://kcy.hywenlv.cn

[R62] 找最占空间的文件
来源：http://ovi.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://lpl.hesvh.cn

[R63] 内存与进程
来源：http://vby.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://rav.fehbvm.com

[R64] 结束进程
来源：http://ipf.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://yas.jiagoushi.top

[R65] 查看端口占用
来源：http://jyy.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tqi.nanxuanxn.top

[R66] 定时任务
来源：http://cku.redwolf501.top

crontab -e;  crontab -l
来源：http://grk.smart0.xyz

[R67] 生成随机十六进制串
来源：http://kqz.sufxvd.cn

openssl rand -hex 16
来源：http://khb.sxryk.cn

[R68] 计算文件校验值
来源：http://pcg.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qsr.nanxuanxn.top

[R69] 生成随机密码
来源：http://jmn.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://dzh.cashguo.top

[R70] 时间戳与互转
来源：http://nry.hcnkem.com

date +%s;  date -d @1700000000
来源：http://wic.xuetiantiany.cn

[R71] 日期格式化
来源：http://ztp.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://skw.quarkkingdee.top

[R72] 等待端口就绪
来源：http://tul.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mob.c1oappe.top

[R73] 分割大日志
来源：http://att.wangdashe.top

split -l 1000 big.log part_
来源：http://foa.gaohongyu789.top

[R74] 批量重命名
来源：http://xcg.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qik.ydzc1.top

[R75] 导出环境变量
来源：http://gmw.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://wqi.zhiwuduotai.top

[R76] 使用临时文件
来源：http://pms.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yyh.yvedp.cn

[R77] 读取用户输入
来源：http://wcz.smart0.xyz

read -rp "请输入: " ans
来源：http://hhl.ehwqpu.com

[R78] 交互式菜单
来源：http://pvj.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://auv.vehdjk.com

[R79] 解析命令行选项
来源：http://kbr.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lbo.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://iuq.zhijiandao.cn

time ./run.sh
来源：http://xqx.sysykeji.top

================================================================================
来源：http://nat.snrcjt.cn

S. C / C++ 专题
来源：http://hji.redwolf501.top

================================================================================
来源：http://pec.zdqjudy.top

[S01] C：Hello World
来源：http://cjf.feifeiyinyue.top

#include <stdio.h>
来源：http://lst.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://bkt.xylfe.cn

[S02] C：变量与格式化输出
来源：http://szx.sweek.top

int a = 10; printf("%d\n", a);
来源：http://dzx.hesvh.cn

[S03] C：读入整数
来源：http://epp.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://dgy.52xcode.cn

[S04] C：字符串复制
来源：http://iwf.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://ohn.vqdsnc.cn

[S05] C：字符串长度
来源：http://ruc.fzhhl.top

strlen(s)
来源：http://tbn.aibaodan.cn

[S06] C：字符串比较
来源：http://zqo.shuidangran.top

strcmp(a, b) == 0
来源：http://xyj.snrcjt.cn

[S07] C：数组遍历求和
来源：http://psm.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://llv.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://prs.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gpe.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://yhq.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hnt.haohaochexian.top

[S10] C：指针与解引用
来源：http://ruh.meibo888.top

int *p = &a;  *p = 5;
来源：http://mkx.quarkkingdee.top

[S11] C：逐行读文件
来源：http://wsv.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://aoi.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ncn.chenzaomai.com

fclose(f);
来源：http://dou.guannengcc.top

[S12] C：写文件
来源：http://euh.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://irn.zdqjudy.top

[S13] C：宏定义
来源：http://pam.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ska.birdmap.top

[S14] C：枚举
来源：http://xvr.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://zpo.yj20258888.top

[S15] C：类型转换
来源：http://abc.ppjwa.cn

(double) a / b
来源：http://ycj.gzhubu.top

[S16] C：位操作置位
来源：http://utj.gzhubu.top

x |= (1 << 3);
来源：http://mur.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://bnv.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jjp.epnwcf.com

[S18] C：命令行参数
来源：http://vqn.jiagoushi.top

int main(int argc, char **argv)
来源：http://ffr.daria6918.cn

[S19] C：快速排序
来源：http://aql.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://uue.gaohongyu789.top

[S20] C：二分查找
来源：http://vxi.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://exg.yj20258.top

[S21] C：字符类别判断
来源：http://tem.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://odp.yongpay.top

[S22] C：字符串转数字
来源：http://top.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://qes.fktsv.cn

[S23] C：随机数
来源：http://unl.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vok.cqqwz.cn

[S24] C：获取本地时间
来源：http://lkb.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lpa.fktsv.cn

[S25] C：内存拷贝
来源：http://amt.vehdjk.com

memcpy(dst, src, n);
来源：http://xly.chenlongwang.top

[S26] C：内存清零
来源：http://gmz.yfazqb.com

memset(a, 0, sizeof a);
来源：http://wmz.hongshengwenyu.top

[S27] C：定义常量
来源：http://kuo.vqdsnc.cn

const double PI = 3.14159;
来源：http://ahs.yongpay.top

[S28] C：静态变量
来源：http://jkm.kuanghao11.cn

static int counter = 0;
来源：http://dpt.iojbl.cn

[S29] C：变参函数
来源：http://diy.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rjw.hnqzz.top

[S30] C：头文件保护
来源：http://mwz.ybcxt.top

#ifndef X_H
来源：http://anc.ctjpmb.com

#define X_H
来源：http://wqk.yongpay.top

#endif
来源：http://hni.epnwcf.com

[S31] C++：Hello World
来源：http://tot.xingfuxueyuan.xyz

#include <iostream>
来源：http://ypk.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://gix.hywenlv.cn

[S32] C++：字符串
来源：http://lhl.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://mgf.hnxiangtu.top

[S33] C++：vector 增删
来源：http://uic.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://can.andypj.xyz

[S34] C++：遍历 vector
来源：http://kuk.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://wee.zhiwuduotai.top

[S35] C++：map
来源：http://uei.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://usb.iojbl.cn

[S36] C++：unordered_map
来源：http://oyz.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qnt.ivvv.top

[S37] C++：set
来源：http://eyj.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mwt.gzhubu.top

[S38] C++：排序
来源：http://qri.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://kbi.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://vwb.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kci.xziqi.cn

[S40] C++：查找元素
来源：http://sor.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyq.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://ckf.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nry.meibo888.top

[S42] C++：继承与虚函数
来源：http://wna.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://dzn.zhiwuduotai.top

[S43] C++：智能指针
来源：http://stl.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://fdt.hongshengwenyu.top

[S44] C++：引用传参
来源：http://tgx.fengsongda.top

void inc(int &x) { ++x; }
来源：http://ldt.havefunace.top

[S45] C++：lambda
来源：http://anq.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ygs.aizwys.cn

[S46] C++：函数模板
来源：http://pwt.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zcy.sweek.top

[S47] C++：结构化绑定遍历
来源：http://qtr.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxr.yangfankeji.com

[S48] C++：逐行读文件
来源：http://svq.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ebl.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://djp.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://cig.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vve.ppjwa.cn

[S50] C++：格式化数字
来源：http://lhx.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ihw.52xcode.cn

[S51] C++：显式类型转换
来源：http://apz.hesvh.cn

static_cast<double>(a) / b
来源：http://rbl.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://deg.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://jio.xziqi.cn

[S53] C++：移动语义
来源：http://plu.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://kvx.zhengqikj.top

[S54] C++：异常处理
来源：http://uwp.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hje.hysaishi.cn

[S55] C++：结构化绑定
来源：http://iqc.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://txp.zhiwuduotai.top

[S56] C++：optional
来源：http://nuy.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://znx.shuidangran.top

[S57] C++：编译期常量
来源：http://eub.fehbvm.com

constexpr int N = 10;
来源：http://izd.c1oappe.top

[S58] C++：命名空间
来源：http://hrv.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://gox.hongshengwenyu.top

[S59] C++：静态断言
来源：http://lmf.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qdh.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://kgp.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oii.wangdashe.top

================================================================================
来源：http://shn.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qgk.sweek.top

================================================================================
来源：http://jzb.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://qpo.sjlbkw.cn

println("Hello")
来源：http://ycq.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://ecv.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dlu.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://ukv.tarul.cn

"值: $b"
来源：http://shz.9152youxi.cn

[T04] Kotlin：空安全
来源：http://wmv.ybcxt.top

val n: String? = null;  n?.length
来源：http://kec.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://kap.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wru.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://lcc.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xnq.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://lct.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wyn.xziqi.cn

[T08] Kotlin：数据类
来源：http://lyj.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://ykv.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://ohd.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://zih.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://bcv.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ynz.c1oappe.top

[T11] Kotlin：协程
来源：http://pvf.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dwi.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://dbt.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://dck.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://keo.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://uoy.yvedp.cn

[T14] Kotlin：循环
来源：http://idw.aibaodan.cn

for (i in 1..10) println(i)
来源：http://ksp.mhx1999.top

[T15] Kotlin：接口
来源：http://vpx.daria6918.cn

interface Shape { fun area(): Double }
来源：http://mwm.xziqi.cn

[T16] Swift：Hello World
来源：http://acg.nanxinkj.top

print("Hello")
来源：http://yuo.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://pfv.daria6918.cn

var a = 1;  let b = 2
来源：http://phi.wangdashe.top

[T18] Swift：字符串插值
来源：http://ffo.hnxiangtu.top

"值: \(b)"
来源：http://kmh.xylfe.cn

[T19] Swift：可选绑定
来源：http://cib.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://ymb.fktsv.cn

[T20] Swift：数组操作
来源：http://jxo.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://imn.uphjek.com

[T21] Swift：遍历
来源：http://kzi.cucudq.cn

for x in a { print(x) }
来源：http://gid.yj20258.top

[T22] Swift：字典
来源：http://rxk.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://iew.ivvv.top

[T23] Swift：函数
来源：http://lqu.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xgi.tian-w.cn

[T24] Swift：闭包
来源：http://nxo.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://bjz.hcnkem.com

[T25] Swift：结构体
来源：http://wgw.dianchejie.cn

struct P { var x: Int }
来源：http://axh.yongpay.top

[T26] Swift：类与重写
来源：http://vnj.yvedp.cn

class A: Base { override func f() {} }
来源：http://aji.yj202588.top

[T27] Swift：错误处理
来源：http://fop.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://ajj.vehdjk.com

[T28] Swift：枚举
来源：http://aib.pycfn.com

enum Color { case red, green }
来源：http://vhc.uphjek.com

[T29] Swift：guard 提前返回
来源：http://rxn.chenzaomai.com

guard let x = opt else { return }
来源：http://hxr.ydzc1.top

[T30] Swift：协议
来源：http://ccv.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://isn.hesvh.cn

[T31] Lua：Hello World
来源：http://hvo.316326.xyz

print("Hello")
来源：http://nwy.hcnkem.com

[T32] Lua：局部变量
来源：http://glt.sxryk.cn

local a = 1
来源：http://bln.xuanzx.com

[T33] Lua：表（数组）
来源：http://ogx.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xkq.hnxiangtu.top

[T34] Lua：遍历表
来源：http://yzx.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://any.pengpengdd.cyou

[T35] Lua：字典表
来源：http://kea.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://tyz.9152youxi.cn

[T36] Lua：函数
来源：http://baj.yj20258.top

function add(a, b) return a + b end
来源：http://csf.gzhubu.top

[T37] Lua：字符串拼接
来源：http://uvo.haohaochexian.top

"a" .. "b"
来源：http://usa.sysykeji.top

[T38] Lua：条件
来源：http://jso.xuanzx.com

if x > 0 then print("正") end
来源：http://laz.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://sbw.zdqjudy.top

string.find(s, "%d+")
来源：http://pib.epnwcf.com

[T40] Lua：元表
来源：http://tkm.vehdjk.com

setmetatable({}, { __index = base })
来源：http://hlt.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://eza.zhongyouzk.top

print "Hello\n";
来源：http://tio.gotoacloud.top

[T42] Perl：变量类型
来源：http://weh.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://erb.52xcode.cn

[T43] Perl：字符串插值
来源：http://cnv.xylfe.cn

"值: $a"
来源：http://quq.smart0.xyz

[T44] Perl：条件
来源：http://tzw.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://mfk.hammf.cn

[T45] Perl：数组遍历
来源：http://tas.tanke756.top

for my $x (@arr) { print $x; }
来源：http://vdq.ybcxt.top

[T46] Perl：哈希操作
来源：http://zej.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://atg.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://bdo.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tlb.ctjpmb.com

[T48] Perl：正则替换
来源：http://jfv.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://rah.hcnkem.com

[T49] Perl：函数
来源：http://pbj.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mjp.xuanzx.com

[T50] Perl：逐行读文件
来源：http://wfl.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ogl.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://uug.tarul.cn

[T51] Scala：Hello World
来源：http://ngn.daria6918.cn

println("Hello")
来源：http://mmb.fengsongda.top

[T52] Scala：变量
来源：http://qgq.snrcjt.cn

val a = 1;  var b = 2
来源：http://yel.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://wqi.pycfn.com

s"值: $b"
来源：http://kns.fehbvm.com

[T54] Scala：集合映射
来源：http://iai.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://swn.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://mtp.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://ndn.uphjek.com

[T56] Scala：样例类
来源：http://wlg.wangdashe.top

case class User(name: String, age: Int)
来源：http://dwi.ppjwa.cn

[T57] Scala：模式匹配
来源：http://gxa.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bvx.andypj.xyz

[T58] Scala：函数定义
来源：http://ias.52xcode.cn


<!-- 参考信息 -->