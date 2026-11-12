代发 wailian999

ssh user@host 'uptime'
来源：http://whe.zhijiandao.cn

[R58] 下载文件
来源：http://inp.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qeb.c1oappe.top

[R59] 发 POST JSON
来源：http://lct.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xtv.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://fbj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uyp.9152youxi.cn

[R61] 磁盘占用
来源：http://ema.pycfn.com

df -h;  du -sh *
来源：http://ues.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://hfm.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://mhz.nwbrower.top

[R63] 内存与进程
来源：http://pqo.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://xkg.shanyushiyangtech.top

[R64] 结束进程
来源：http://liv.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://vsp.bjfxy.top

[R65] 查看端口占用
来源：http://wja.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xix.zhiwuduotai.top

[R66] 定时任务
来源：http://odf.xuanzx.com

crontab -e;  crontab -l
来源：http://pzn.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://usg.ehwqpu.com

openssl rand -hex 16
来源：http://kkp.epnwcf.com

[R68] 计算文件校验值
来源：http://zyq.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://ccp.sweek.top

[R69] 生成随机密码
来源：http://kfl.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://ewz.hnxiangtu.top

[R70] 时间戳与互转
来源：http://zjp.wangdashe.top

date +%s;  date -d @1700000000
来源：http://hte.hongshengwenyu.top

[R71] 日期格式化
来源：http://ulc.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yhs.gzhubu.top

[R72] 等待端口就绪
来源：http://ecy.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dlp.haohaochexian.top

[R73] 分割大日志
来源：http://aby.cheryme.top

split -l 1000 big.log part_
来源：http://xgs.ydzc1.top

[R74] 批量重命名
来源：http://haz.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://goa.0kj1m.cn

[R75] 导出环境变量
来源：http://mvd.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://xiw.zhongyouzk.top

[R76] 使用临时文件
来源：http://xqb.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fha.ydzc1.top

[R77] 读取用户输入
来源：http://ddp.aibaodan.cn

read -rp "请输入: " ans
来源：http://muv.jiagoushi.top

[R78] 交互式菜单
来源：http://rnr.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kwj.ehwqpu.com

[R79] 解析命令行选项
来源：http://heg.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lux.tanke756.top

[R80] 查看脚本执行耗时
来源：http://ymo.snrcjt.cn

time ./run.sh
来源：http://ahk.yj202588.top

================================================================================
来源：http://fml.gaohongyu789.top

S. C / C++ 专题
来源：http://lce.yangfankeji.com

================================================================================
来源：http://hlc.zhengqikj.top

[S01] C：Hello World
来源：http://euc.yuxming.cn

#include <stdio.h>
来源：http://lwv.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ava.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://gnm.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://cyw.xylfe.cn

[S03] C：读入整数
来源：http://rvn.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://dvw.jyoumei.cn

[S04] C：字符串复制
来源：http://upj.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://kvu.bjfxy.top

[S05] C：字符串长度
来源：http://ybr.yj202588.top

strlen(s)
来源：http://vet.vqdsnc.cn

[S06] C：字符串比较
来源：http://afl.gogol.net.cn

strcmp(a, b) == 0
来源：http://wya.zycfv.cn

[S07] C：数组遍历求和
来源：http://ixo.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://suu.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://qme.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://awc.yongpay.top

[S09] C：结构体定义与初始化
来源：http://ogf.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vml.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://fhh.birdmap.top

int *p = &a;  *p = 5;
来源：http://faa.zycfv.cn

[S11] C：逐行读文件
来源：http://apd.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://vfz.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://djq.havefunace.top

fclose(f);
来源：http://tps.gotoacloud.top

[S12] C：写文件
来源：http://ldh.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://doq.vehdjk.com

[S13] C：宏定义
来源：http://lyi.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kez.nanxuanxn.top

[S14] C：枚举
来源：http://jrv.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://dvc.snrcjt.cn

[S15] C：类型转换
来源：http://xby.andypj.xyz

(double) a / b
来源：http://dgq.yj202588.top

[S16] C：位操作置位
来源：http://ltd.wangdashe.top

x |= (1 << 3);
来源：http://lgx.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://pvv.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dct.yongpay.top

[S18] C：命令行参数
来源：http://zrz.fengsongda.top

int main(int argc, char **argv)
来源：http://mxy.9152youxi.cn

[S19] C：快速排序
来源：http://fmo.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://dyj.jinqigufen.top

[S20] C：二分查找
来源：http://spr.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xft.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://btx.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://njh.zhengqikj.top

[S22] C：字符串转数字
来源：http://tfs.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://vmj.haohaochexian.top

[S23] C：随机数
来源：http://sbg.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://qsm.cucudq.cn

[S24] C：获取本地时间
来源：http://ngd.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dsm.fzhhl.top

[S25] C：内存拷贝
来源：http://duz.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://lth.shanyushiyangtech.top

[S26] C：内存清零
来源：http://rgp.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://wov.0kj1m.cn

[S27] C：定义常量
来源：http://efk.zdbjq.cn

const double PI = 3.14159;
来源：http://gno.yfazqb.com

[S28] C：静态变量
来源：http://pkn.xuanzx.com

static int counter = 0;
来源：http://zbt.feifeiyinyue.top

[S29] C：变参函数
来源：http://jxt.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eqs.xziqi.cn

[S30] C：头文件保护
来源：http://qjh.xylfe.cn

#ifndef X_H
来源：http://uyn.cashguo.top

#define X_H
来源：http://ebp.yj202588.top

#endif
来源：http://zoh.kuanghao11.cn

[S31] C++：Hello World
来源：http://utq.yvedp.cn

#include <iostream>
来源：http://chn.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://kwm.52xcode.cn

[S32] C++：字符串
来源：http://vub.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://vqv.havefunace.top

[S33] C++：vector 增删
来源：http://sgt.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ffe.bjfxy.top

[S34] C++：遍历 vector
来源：http://ddx.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://iof.yj202588.top

[S35] C++：map
来源：http://lit.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gsm.wangdashe.top

[S36] C++：unordered_map
来源：http://ivw.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zcb.birdmap.top

[S37] C++：set
来源：http://giy.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jhu.9152youxi.cn

[S38] C++：排序
来源：http://rks.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://xin.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://elr.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rtw.quarkkingdee.top

[S40] C++：查找元素
来源：http://cxh.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qhk.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://gvn.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gky.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://nty.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://grv.sweek.top

[S43] C++：智能指针
来源：http://oip.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://qay.yuanzhike.top

[S44] C++：引用传参
来源：http://srv.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://gsg.zhongyouzk.top

[S45] C++：lambda
来源：http://czr.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://fmv.nanxuanxn.top

[S46] C++：函数模板
来源：http://jvx.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rnc.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://uxi.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gny.xuanzx.com

[S48] C++：逐行读文件
来源：http://nsl.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://hrm.yonumen.top

while (std::getline(in, line)) { }
来源：http://hvm.jyoumei.cn

[S49] C++：写文件
来源：http://map.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kiv.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://fnq.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dcb.nwbrower.top

[S51] C++：显式类型转换
来源：http://sbz.zhengqikj.top

static_cast<double>(a) / b
来源：http://dph.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://bdu.fzhhl.top

int size() const noexcept { return n_; }
来源：http://vnj.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://kkl.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://prv.epnwcf.com

[S54] C++：异常处理
来源：http://lre.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iog.yj20258888.top

[S55] C++：结构化绑定
来源：http://wiv.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jic.yangfankeji.com

[S56] C++：optional
来源：http://ohr.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kmc.xinyue.icu

[S57] C++：编译期常量
来源：http://map.xziqi.cn

constexpr int N = 10;
来源：http://svz.jqgufenzy.top

[S58] C++：命名空间
来源：http://cfn.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://irv.hywenlv.cn

[S59] C++：静态断言
来源：http://amp.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://idz.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://wwq.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dhz.zhongyouzk.top

================================================================================
来源：http://wws.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hal.yangfankeji.com

================================================================================
来源：http://vqc.tian-w.cn

[T01] Kotlin：Hello World
来源：http://lsu.cdnleiting.top

println("Hello")
来源：http://tlc.iojbl.cn

[T02] Kotlin：变量
来源：http://pde.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pwf.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://xau.hfpthk.cn

"值: $b"
来源：http://fpx.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://sgn.hysaishi.cn

val n: String? = null;  n?.length
来源：http://gdc.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://cek.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wkx.fktsv.cn

[T06] Kotlin：集合映射
来源：http://iej.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://vdh.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://hbm.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lyz.xziqi.cn

[T08] Kotlin：数据类
来源：http://duu.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://itj.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://omi.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://fxy.fzhhl.top

[T10] Kotlin：默认参数
来源：http://zpl.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lsy.ivvv.top

[T11] Kotlin：协程
来源：http://ogc.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uzd.sysykeji.top

[T12] Kotlin：解构声明
来源：http://kwl.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://rtw.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://tsz.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://wla.hywenlv.cn

[T14] Kotlin：循环
来源：http://vfp.tarul.cn

for (i in 1..10) println(i)
来源：http://ujs.shzxlz.cn

[T15] Kotlin：接口
来源：http://ujj.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://pcd.nanxuanxn.top

[T16] Swift：Hello World
来源：http://yzv.jinyuanbaomall.cn

print("Hello")
来源：http://ltr.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://tmh.yuanzhike.top

var a = 1;  let b = 2
来源：http://kgc.epnwcf.com

[T18] Swift：字符串插值
来源：http://hdk.zdqjudy.top

"值: \(b)"
来源：http://wvl.smart0.xyz

[T19] Swift：可选绑定
来源：http://wsv.tarul.cn

if let n = opt { print(n) }
来源：http://lyw.fzhhl.top

[T20] Swift：数组操作
来源：http://yyu.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://kzk.vqdsnc.cn

[T21] Swift：遍历
来源：http://vuq.uphjek.com

for x in a { print(x) }
来源：http://jax.cdnleiting.top

[T22] Swift：字典
来源：http://vqa.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://vrt.yuanzhike.top

[T23] Swift：函数
来源：http://exm.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bzm.pycfn.com

[T24] Swift：闭包
来源：http://anf.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rze.shangyingyoupin.top

[T25] Swift：结构体
来源：http://kkj.xuanzx.com

struct P { var x: Int }
来源：http://mas.epnwcf.com

[T26] Swift：类与重写
来源：http://hfi.sysykeji.top

class A: Base { override func f() {} }
来源：http://twj.uphjek.com

[T27] Swift：错误处理
来源：http://trd.yj20258888.top

do { try f() } catch { print(error) }
来源：http://xga.dashuyun.cn

[T28] Swift：枚举
来源：http://vta.cashguo.top

enum Color { case red, green }
来源：http://xsi.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://ewj.epnwcf.com

guard let x = opt else { return }
来源：http://heu.snrcjt.cn

[T30] Swift：协议
来源：http://evd.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://uqw.cdnleiting.top

[T31] Lua：Hello World
来源：http://ihy.dashuyun.cn

print("Hello")
来源：http://fry.jiagoushi.top

[T32] Lua：局部变量
来源：http://ykz.iojbl.cn

local a = 1
来源：http://dye.tanke756.top

[T33] Lua：表（数组）
来源：http://poh.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dln.tanke756.top

[T34] Lua：遍历表
来源：http://bdt.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pie.pycfn.com

[T35] Lua：字典表
来源：http://uzo.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://hyf.gogol.net.cn

[T36] Lua：函数
来源：http://vyt.ppjwa.cn

function add(a, b) return a + b end
来源：http://pkb.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://mfi.zdqjudy.top

"a" .. "b"
来源：http://avc.redwolf501.top

[T38] Lua：条件
来源：http://eqp.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://rkq.yfazqb.com

[T39] Lua：模式匹配
来源：http://sew.zycfv.cn

string.find(s, "%d+")
来源：http://fyf.shangyingyoupin.top

[T40] Lua：元表
来源：http://doi.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://ahs.redwolf501.top

[T41] Perl：Hello World
来源：http://vir.xziqi.cn

print "Hello\n";
来源：http://ifw.sxryk.cn

[T42] Perl：变量类型
来源：http://qqm.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vfx.tianlin.xyz

[T43] Perl：字符串插值
来源：http://hsu.dashuyun.cn

"值: $a"
来源：http://mes.yangfankeji.com

[T44] Perl：条件
来源：http://ygr.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://jaj.vehdjk.com

[T45] Perl：数组遍历
来源：http://vlu.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://sdw.ivvv.top

[T46] Perl：哈希操作
来源：http://ekc.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wep.fktsv.cn

[T47] Perl：正则捕获
来源：http://bal.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rse.bbcook.cn

[T48] Perl：正则替换
来源：http://mdr.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://jyc.jiagoushi.top

[T49] Perl：函数
来源：http://usi.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wjj.gzhubu.top

[T50] Perl：逐行读文件
来源：http://mwa.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cct.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://qbq.gotoacloud.top

[T51] Scala：Hello World
来源：http://uje.sufxvd.cn

println("Hello")
来源：http://sbp.guannengcc.top

[T52] Scala：变量
来源：http://vzr.xuanzx.com

val a = 1;  var b = 2
来源：http://agf.haohaochexian.top

[T53] Scala：字符串插值
来源：http://jph.nwbrower.top

s"值: $b"
来源：http://tnx.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://xnc.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://vvx.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://gko.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://fos.xuetiantiany.cn

[T56] Scala：样例类
来源：http://jco.tanke756.top

case class User(name: String, age: Int)
来源：http://tng.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://nck.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tfp.52xcode.cn

[T58] Scala：函数定义
来源：http://axr.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://dnt.haohaochexian.top

[T59] Scala：循环
来源：http://dkc.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://dgo.xuetiantiany.cn

[T60] Scala：折叠
来源：http://dwv.nwbrower.top


<!-- 参考信息 -->