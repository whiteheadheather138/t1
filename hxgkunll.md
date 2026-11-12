代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://xiq.guowangkeji.top

[R52] 统计行数
来源：http://lcd.fzhhl.top

wc -l a.txt
来源：http://sde.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://hbx.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jws.316326.xyz

[R54] 比较两个文件
来源：http://mql.feifeiyinyue.top

diff a.txt b.txt
来源：http://jny.ctjpmb.com

[R55] 压缩与解压
来源：http://ueb.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cbu.tianlin.xyz

[R56] 远程拷贝
来源：http://buf.zdqjudy.top

scp file user@host:/path/
来源：http://kam.zycfv.cn

[R57] 远程执行命令
来源：http://fbk.zhijiandao.cn

ssh user@host 'uptime'
来源：http://zpi.tianlin.xyz

[R58] 下载文件
来源：http://ggl.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baj.cqqwz.cn

[R59] 发 POST JSON
来源：http://vlw.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsr.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://lsq.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://srz.meibo888.top

[R61] 磁盘占用
来源：http://csw.jinghuilouyu.cn

df -h;  du -sh *
来源：http://oqc.gotoacloud.top

[R62] 找最占空间的文件
来源：http://ebi.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://cha.ybcxt.top

[R63] 内存与进程
来源：http://jiv.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://owp.xuetiantiany.cn

[R64] 结束进程
来源：http://mrs.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://rna.sufxvd.cn

[R65] 查看端口占用
来源：http://wmi.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hzb.xylfe.cn

[R66] 定时任务
来源：http://ipr.jianghu66.top

crontab -e;  crontab -l
来源：http://rbc.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://qok.bjfxy.top

openssl rand -hex 16
来源：http://yhs.hysaishi.cn

[R68] 计算文件校验值
来源：http://gaj.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://juw.yfazqb.com

[R69] 生成随机密码
来源：http://lts.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://yff.ehwqpu.com

[R70] 时间戳与互转
来源：http://vwh.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://zse.nwbrower.top

[R71] 日期格式化
来源：http://pos.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zhv.hesvh.cn

[R72] 等待端口就绪
来源：http://ifp.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hqp.jlsjyb.cn

[R73] 分割大日志
来源：http://yoo.jiagoushi.top

split -l 1000 big.log part_
来源：http://qob.gogol.net.cn

[R74] 批量重命名
来源：http://ith.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://boc.jlsjyb.cn

[R75] 导出环境变量
来源：http://aez.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://dil.fzhhl.top

[R76] 使用临时文件
来源：http://hcd.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nyo.daria6918.cn

[R77] 读取用户输入
来源：http://ctp.tanke756.top

read -rp "请输入: " ans
来源：http://oek.jlsjyb.cn

[R78] 交互式菜单
来源：http://yuu.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zkw.mhx1999.top

[R79] 解析命令行选项
来源：http://fka.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yeg.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://iyj.yanxiufei.cn

time ./run.sh
来源：http://qto.yangfankeji.com

================================================================================
来源：http://prw.hfpthk.cn

S. C / C++ 专题
来源：http://liy.dianchejie.cn

================================================================================
来源：http://fdp.haohaochexian.top

[S01] C：Hello World
来源：http://fpc.zhijiandao.cn

#include <stdio.h>
来源：http://dbw.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://kpy.aizwys.cn

[S02] C：变量与格式化输出
来源：http://nno.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://oqs.hcnkem.com

[S03] C：读入整数
来源：http://arz.52xcode.cn

int x; scanf("%d", &x);
来源：http://xqt.andypj.xyz

[S04] C：字符串复制
来源：http://ewn.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://ibs.yvedp.cn

[S05] C：字符串长度
来源：http://ibj.yueranfly.top

strlen(s)
来源：http://zoq.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://wte.sysykeji.top

strcmp(a, b) == 0
来源：http://grm.mhx1999.top

[S07] C：数组遍历求和
来源：http://gfl.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdj.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://oks.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://var.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://kni.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xyc.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://uyu.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://uoy.ehwqpu.com

[S11] C：逐行读文件
来源：http://clq.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://xci.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zww.yj20258888.top

fclose(f);
来源：http://jez.hfpthk.cn

[S12] C：写文件
来源：http://ekr.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mtm.ybcxt.top

[S13] C：宏定义
来源：http://vuz.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ope.jlsjyb.cn

[S14] C：枚举
来源：http://yrm.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://krg.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://vlc.ctjpmb.com

(double) a / b
来源：http://eob.jinqigfzy.top

[S16] C：位操作置位
来源：http://tbq.hfpthk.cn

x |= (1 << 3);
来源：http://oow.hcnkem.com

[S17] C：安全拼接字符串
来源：http://lsl.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vaq.zdbjq.cn

[S18] C：命令行参数
来源：http://hkd.hfpthk.cn

int main(int argc, char **argv)
来源：http://bwj.iojbl.cn

[S19] C：快速排序
来源：http://abq.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://lpn.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://tba.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ooj.9152youxi.cn

[S21] C：字符类别判断
来源：http://fcs.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qbt.fengsongda.top

[S22] C：字符串转数字
来源：http://oen.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ijz.fehbvm.com

[S23] C：随机数
来源：http://tzr.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kuh.pycfn.com

[S24] C：获取本地时间
来源：http://dih.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vqo.hnqzz.top

[S25] C：内存拷贝
来源：http://whe.xinyue.icu

memcpy(dst, src, n);
来源：http://aem.sweek.top

[S26] C：内存清零
来源：http://hxm.vehdjk.com

memset(a, 0, sizeof a);
来源：http://cxo.sysykeji.top

[S27] C：定义常量
来源：http://bdw.chenjidiqi.icu

const double PI = 3.14159;
来源：http://bzy.snrcjt.cn

[S28] C：静态变量
来源：http://iwn.sufxvd.cn

static int counter = 0;
来源：http://gsu.pengpengdd.cyou

[S29] C：变参函数
来源：http://ebq.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lkm.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://jtx.snrcjt.cn

#ifndef X_H
来源：http://ahz.yuanzhike.top

#define X_H
来源：http://xsd.hfpthk.cn

#endif
来源：http://rgx.zhoulong.xyz

[S31] C++：Hello World
来源：http://vxa.cheryme.top

#include <iostream>
来源：http://yxg.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://ikj.uphjek.com

[S32] C++：字符串
来源：http://jzc.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://bhi.gogol.net.cn

[S33] C++：vector 增删
来源：http://qmo.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://moe.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://yee.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://vnu.cdnleiting.top

[S35] C++：map
来源：http://sqw.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://edm.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://mer.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hvo.aizwys.cn

[S37] C++：set
来源：http://omj.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ixe.dianchejie.cn

[S38] C++：排序
来源：http://cvv.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://qfz.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://clr.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://srr.gogol.net.cn

[S40] C++：查找元素
来源：http://nli.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zoh.zdbjq.cn

[S41] C++：类与构造函数
来源：http://rma.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://esb.52xcode.cn

[S42] C++：继承与虚函数
来源：http://efw.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://gwb.jinqigufen.top

[S43] C++：智能指针
来源：http://cbo.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://jmj.xuanzx.com

[S44] C++：引用传参
来源：http://qve.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://asx.shanyushiyangtech.top

[S45] C++：lambda
来源：http://qzm.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://rlr.daria6918.cn

[S46] C++：函数模板
来源：http://ean.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nvt.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://nbz.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pkt.sweek.top

[S48] C++：逐行读文件
来源：http://wuh.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qou.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://ohm.iojbl.cn

[S49] C++：写文件
来源：http://tqd.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://src.ydzc1.top

[S50] C++：格式化数字
来源：http://npt.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wof.hfpthk.cn

[S51] C++：显式类型转换
来源：http://atv.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://amt.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://iok.bjfxy.top

int size() const noexcept { return n_; }
来源：http://njq.hnxiangtu.top

[S53] C++：移动语义
来源：http://ura.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://uow.zhoulong.xyz

[S54] C++：异常处理
来源：http://utl.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wrj.yfazqb.com

[S55] C++：结构化绑定
来源：http://csc.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://twg.yuanzhike.top

[S56] C++：optional
来源：http://ter.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbe.zhengqikj.top

[S57] C++：编译期常量
来源：http://piu.ehwqpu.com

constexpr int N = 10;
来源：http://wku.zhoulong.xyz

[S58] C++：命名空间
来源：http://xbs.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://hhs.hongshengwenyu.top

[S59] C++：静态断言
来源：http://ikb.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bos.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://bde.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oxv.fktsv.cn

================================================================================
来源：http://qrm.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://adb.gogol.net.cn

================================================================================
来源：http://vrd.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://kph.xinyue.icu

println("Hello")
来源：http://ttp.vqdsnc.cn

[T02] Kotlin：变量
来源：http://vgo.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xil.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://drq.sjlbkw.cn

"值: $b"
来源：http://sab.chenzaomai.com

[T04] Kotlin：空安全
来源：http://yug.aibaodan.cn

val n: String? = null;  n?.length
来源：http://ray.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://kgz.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wra.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://dyr.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://klr.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://zes.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pes.sxryk.cn

[T08] Kotlin：数据类
来源：http://vhz.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://mmo.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://ona.sweek.top

fun String.exclaim() = this + "!"
来源：http://hem.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://zdz.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vro.ydzc1.top

[T11] Kotlin：协程
来源：http://mif.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jse.daria6918.cn

[T12] Kotlin：解构声明
来源：http://lun.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://zat.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://zxv.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://fvj.wangdashe.top

[T14] Kotlin：循环
来源：http://qqc.cqqwz.cn

for (i in 1..10) println(i)
来源：http://kox.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://bqn.yongpay.top

interface Shape { fun area(): Double }
来源：http://nqj.zhijiandao.cn

[T16] Swift：Hello World
来源：http://cwr.9152youxi.cn

print("Hello")
来源：http://vvp.yuanzhike.top

[T17] Swift：变量与常量
来源：http://hkb.yuanzhike.top

var a = 1;  let b = 2
来源：http://fwo.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://whi.dianchejie.cn

"值: \(b)"
来源：http://muv.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://sgr.tian-w.cn

if let n = opt { print(n) }
来源：http://nsk.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://hta.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mcb.hongshengwenyu.top

[T21] Swift：遍历
来源：http://ugb.dianchejie.cn

for x in a { print(x) }
来源：http://jou.sweek.top

[T22] Swift：字典
来源：http://cux.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://mej.gaohongyu789.top

[T23] Swift：函数
来源：http://etq.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hty.c1oappe.top

[T24] Swift：闭包
来源：http://hfg.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fvn.yanxiufei.cn

[T25] Swift：结构体
来源：http://elj.gzhubu.top

struct P { var x: Int }
来源：http://lkc.aibaodan.cn

[T26] Swift：类与重写
来源：http://iyn.zdbjq.cn

class A: Base { override func f() {} }
来源：http://unn.ehwqpu.com

[T27] Swift：错误处理
来源：http://fuj.bjfxy.top

do { try f() } catch { print(error) }
来源：http://hhx.pycfn.com

[T28] Swift：枚举
来源：http://ber.mhx1999.top

enum Color { case red, green }
来源：http://ula.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://jjv.gotoacloud.top

guard let x = opt else { return }
来源：http://tvq.bjfxy.top

[T30] Swift：协议
来源：http://vjf.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://dfe.mhx1999.top

[T31] Lua：Hello World
来源：http://qua.hnqzz.top

print("Hello")
来源：http://nct.ydjk.org.cn

[T32] Lua：局部变量
来源：http://yth.hnxiangtu.top

local a = 1
来源：http://bvm.gogol.net.cn

[T33] Lua：表（数组）
来源：http://dlf.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jlx.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://kkv.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ggf.316326.xyz

[T35] Lua：字典表
来源：http://zke.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://ulv.gaohongyu789.top

[T36] Lua：函数
来源：http://elu.hammf.cn

function add(a, b) return a + b end
来源：http://wyf.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://oma.xuetiantiany.cn

"a" .. "b"
来源：http://qju.kuanghao11.cn

[T38] Lua：条件
来源：http://cnk.9152youxi.cn

if x > 0 then print("正") end
来源：http://hdv.zhengqikj.top

[T39] Lua：模式匹配
来源：http://fxl.hcnkem.com

string.find(s, "%d+")
来源：http://uoe.jinghuilouyu.cn

[T40] Lua：元表
来源：http://uiy.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://kmv.cheryme.top

[T41] Perl：Hello World
来源：http://wua.xingfuxueyuan.xyz

print "Hello\n";
来源：http://hjh.c1oappe.top

[T42] Perl：变量类型
来源：http://bic.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dbc.xziqi.cn

[T43] Perl：字符串插值
来源：http://icg.0kj1m.cn

"值: $a"
来源：http://epb.chenzaomai.com

[T44] Perl：条件
来源：http://bds.316326.xyz

if ($a > 0) { print "正"; }
来源：http://zxu.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://hpm.havefunace.top

for my $x (@arr) { print $x; }
来源：http://ojv.yangfankeji.com

[T46] Perl：哈希操作
来源：http://dwo.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zna.ybcxt.top

[T47] Perl：正则捕获
来源：http://fzd.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wcc.chenzaomai.com

[T48] Perl：正则替换
来源：http://rhp.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://lxc.zhengqikj.top

[T49] Perl：函数
来源：http://hpm.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qtf.yvedp.cn

[T50] Perl：逐行读文件
来源：http://kcn.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ilh.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://xfu.yanxiufei.cn

[T51] Scala：Hello World
来源：http://ijh.zdbjq.cn

println("Hello")
来源：http://ebh.redwolf501.top

[T52] Scala：变量
来源：http://dyj.ppjwa.cn

val a = 1;  var b = 2
来源：http://jvn.ydzc1.top

[T53] Scala：字符串插值
来源：http://blp.ydzc1.top

s"值: $b"
来源：http://kgb.fengsongda.top

[T54] Scala：集合映射
来源：http://uqg.zhijiandao.cn


<!-- 参考信息 -->