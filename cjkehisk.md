代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ijx.yj20258.top

[R52] 统计行数
来源：http://gaf.yonumen.top

wc -l a.txt
来源：http://hlu.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://bhj.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xqp.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://saw.yj202588.top

diff a.txt b.txt
来源：http://rpl.xziqi.cn

[R55] 压缩与解压
来源：http://qdw.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cyh.ivvv.top

[R56] 远程拷贝
来源：http://out.svipenyu.cn

scp file user@host:/path/
来源：http://zua.gzhubu.top

[R57] 远程执行命令
来源：http://lnm.chenzaomai.com

ssh user@host 'uptime'
来源：http://ppg.xuetiantiany.cn

[R58] 下载文件
来源：http://ajf.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ksm.smart0.xyz

[R59] 发 POST JSON
来源：http://vbk.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wse.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://lyl.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tix.jqgufenzy.top

[R61] 磁盘占用
来源：http://gpm.sxryk.cn

df -h;  du -sh *
来源：http://hot.316326.xyz

[R62] 找最占空间的文件
来源：http://udw.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://wyq.chenlongwang.top

[R63] 内存与进程
来源：http://ywl.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://hqo.bbcook.cn

[R64] 结束进程
来源：http://uyd.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://vxi.fehbvm.com

[R65] 查看端口占用
来源：http://ikn.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://acb.pycfn.com

[R66] 定时任务
来源：http://uqr.yuanzhike.top

crontab -e;  crontab -l
来源：http://sgs.cucudq.cn

[R67] 生成随机十六进制串
来源：http://nml.cheryme.top

openssl rand -hex 16
来源：http://eqg.yuxming.cn

[R68] 计算文件校验值
来源：http://meb.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lvh.sufxvd.cn

[R69] 生成随机密码
来源：http://jzn.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://jos.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://wqy.pycfn.com

date +%s;  date -d @1700000000
来源：http://pbo.xuanzx.com

[R71] 日期格式化
来源：http://bgx.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hgx.yj202588.top

[R72] 等待端口就绪
来源：http://xdo.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xni.yfazqb.com

[R73] 分割大日志
来源：http://oeq.yangfankeji.com

split -l 1000 big.log part_
来源：http://nod.yvedp.cn

[R74] 批量重命名
来源：http://mjo.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qhv.shzxlz.cn

[R75] 导出环境变量
来源：http://ioe.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://axj.ctjpmb.com

[R76] 使用临时文件
来源：http://zyo.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ooi.cashguo.top

[R77] 读取用户输入
来源：http://gil.nanxuanxn.top

read -rp "请输入: " ans
来源：http://hsv.316326.xyz

[R78] 交互式菜单
来源：http://rvm.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rdh.xuanzx.com

[R79] 解析命令行选项
来源：http://gxs.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jhx.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://quy.jianghu66.top

time ./run.sh
来源：http://jso.fanxiaobao.xyz

================================================================================
来源：http://kwt.zdqjudy.top

S. C / C++ 专题
来源：http://xlf.nanxuanxn.top

================================================================================
来源：http://egb.ydzc1.top

[S01] C：Hello World
来源：http://wel.mhx1999.top

#include <stdio.h>
来源：http://dbt.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dpj.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://jkd.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://klk.fanxiaobao.xyz

[S03] C：读入整数
来源：http://bqu.haohaochexian.top

int x; scanf("%d", &x);
来源：http://yjm.hcnkem.com

[S04] C：字符串复制
来源：http://bei.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://utg.jyoumei.cn

[S05] C：字符串长度
来源：http://vyj.hongshengwenyu.top

strlen(s)
来源：http://gnn.hammf.cn

[S06] C：字符串比较
来源：http://nxv.hnqzz.top

strcmp(a, b) == 0
来源：http://zuc.chenzaomai.com

[S07] C：数组遍历求和
来源：http://lvk.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fas.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://aje.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lfd.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://xml.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dsb.ppjwa.cn

[S10] C：指针与解引用
来源：http://zqb.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://dxa.kuanghao11.cn

[S11] C：逐行读文件
来源：http://xpw.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://qfu.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zvz.pengpengdd.cyou

fclose(f);
来源：http://hhl.xinyue.icu

[S12] C：写文件
来源：http://lwx.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://crh.yfazqb.com

[S13] C：宏定义
来源：http://uli.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://whj.sweek.top

[S14] C：枚举
来源：http://oxt.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://vaz.shuidangran.top

[S15] C：类型转换
来源：http://hwe.snrcjt.cn

(double) a / b
来源：http://pdf.xziqi.cn

[S16] C：位操作置位
来源：http://hru.hongshengwenyu.top

x |= (1 << 3);
来源：http://uxp.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://suu.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vrs.chenzaomai.com

[S18] C：命令行参数
来源：http://pgr.wangdashe.top

int main(int argc, char **argv)
来源：http://tno.zhixingplan.top

[S19] C：快速排序
来源：http://izm.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://gmc.dianchejie.cn

[S20] C：二分查找
来源：http://dnt.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dhd.xziqi.cn

[S21] C：字符类别判断
来源：http://gpy.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ozy.cashguo.top

[S22] C：字符串转数字
来源：http://hix.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://veo.redwolf501.top

[S23] C：随机数
来源：http://gnz.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fvd.cheryme.top

[S24] C：获取本地时间
来源：http://dqr.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qlw.jianghu66.top

[S25] C：内存拷贝
来源：http://xnf.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://qrl.gaohongyu789.top

[S26] C：内存清零
来源：http://pkz.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://nsm.uphjek.com

[S27] C：定义常量
来源：http://iql.52xcode.cn

const double PI = 3.14159;
来源：http://yxl.jinqigufen.top

[S28] C：静态变量
来源：http://wui.aizwys.cn

static int counter = 0;
来源：http://pnm.hongshengwenyu.top

[S29] C：变参函数
来源：http://tmx.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wqv.hcnkem.com

[S30] C：头文件保护
来源：http://pgg.daxiang520.top

#ifndef X_H
来源：http://jbn.jinqigufen.top

#define X_H
来源：http://xng.cucudq.cn

#endif
来源：http://kjf.chenlongwang.top

[S31] C++：Hello World
来源：http://ofb.bbcook.cn

#include <iostream>
来源：http://obb.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://huu.chenjidiqi.icu

[S32] C++：字符串
来源：http://lyw.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://ztb.quarkkingdee.top

[S33] C++：vector 增删
来源：http://anb.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aax.sufxvd.cn

[S34] C++：遍历 vector
来源：http://lvh.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://dyy.yuanzhike.top

[S35] C++：map
来源：http://eqz.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nzh.yvedp.cn

[S36] C++：unordered_map
来源：http://hwx.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ehf.yueranfly.top

[S37] C++：set
来源：http://jaw.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hih.yfazqb.com

[S38] C++：排序
来源：http://qgx.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://yoc.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://qla.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://efz.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://bom.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xdp.hysaishi.cn

[S41] C++：类与构造函数
来源：http://mxp.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ypy.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://qvt.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://sru.redwolf501.top

[S43] C++：智能指针
来源：http://nxo.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://lrn.ydjk.org.cn

[S44] C++：引用传参
来源：http://fdn.nwbrower.top

void inc(int &x) { ++x; }
来源：http://ipc.daria6918.cn

[S45] C++：lambda
来源：http://ffq.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://ckt.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://fhz.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sja.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://qrq.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tbw.fktsv.cn

[S48] C++：逐行读文件
来源：http://way.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://kwe.yongpay.top

while (std::getline(in, line)) { }
来源：http://fdw.jiagoushi.top

[S49] C++：写文件
来源：http://thu.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgh.havefunace.top

[S50] C++：格式化数字
来源：http://won.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fmu.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://bdk.zhongyouzk.top

static_cast<double>(a) / b
来源：http://jty.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://jwy.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://dvh.dashuyun.cn

[S53] C++：移动语义
来源：http://bvx.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://vfp.jiagoushi.top

[S54] C++：异常处理
来源：http://anj.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvg.dashuyun.cn

[S55] C++：结构化绑定
来源：http://vco.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cnd.daria6918.cn

[S56] C++：optional
来源：http://ctd.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ayr.dianchejie.cn

[S57] C++：编译期常量
来源：http://lcc.zycfv.cn

constexpr int N = 10;
来源：http://arr.ydjk.org.cn

[S58] C++：命名空间
来源：http://cji.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://ltg.cdnleiting.top

[S59] C++：静态断言
来源：http://urk.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vol.cheryme.top

[S60] C++：遍历并删除元素
来源：http://flu.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mxb.xziqi.cn

================================================================================
来源：http://nph.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzr.pycfn.com

================================================================================
来源：http://mwv.tanke756.top

[T01] Kotlin：Hello World
来源：http://fra.hfpthk.cn

println("Hello")
来源：http://rki.hcnkem.com

[T02] Kotlin：变量
来源：http://kvj.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bre.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://xfa.tarul.cn

"值: $b"
来源：http://pzq.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://rth.nwbrower.top

val n: String? = null;  n?.length
来源：http://mzn.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://xis.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iik.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://dyp.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lch.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://kpc.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ulw.yuxming.cn

[T08] Kotlin：数据类
来源：http://miu.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://omq.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://bcb.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://hyc.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://dxp.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://jgo.yuxming.cn

[T11] Kotlin：协程
来源：http://iqm.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tfb.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://gkb.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://trd.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://snb.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://sac.bbcook.cn

[T14] Kotlin：循环
来源：http://dms.zhengqikj.top

for (i in 1..10) println(i)
来源：http://zat.cdnleiting.top

[T15] Kotlin：接口
来源：http://fsy.vehdjk.com

interface Shape { fun area(): Double }
来源：http://whk.fehbvm.com

[T16] Swift：Hello World
来源：http://glf.pengpengdd.cyou

print("Hello")
来源：http://yhl.iojbl.cn

[T17] Swift：变量与常量
来源：http://aqg.chenzaomai.com

var a = 1;  let b = 2
来源：http://foy.daxiang520.top

[T18] Swift：字符串插值
来源：http://ofv.xylfe.cn

"值: \(b)"
来源：http://ehp.gogol.net.cn

[T19] Swift：可选绑定
来源：http://emh.jqgfzy.top

if let n = opt { print(n) }
来源：http://xti.pycfn.com

[T20] Swift：数组操作
来源：http://wim.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mig.cqqwz.cn

[T21] Swift：遍历
来源：http://lzv.dianchejie.cn

for x in a { print(x) }
来源：http://zhv.gotoacloud.top

[T22] Swift：字典
来源：http://snd.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://lwr.hongshengwenyu.top

[T23] Swift：函数
来源：http://ltz.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ntx.xinyue.icu

[T24] Swift：闭包
来源：http://yxb.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zyl.zhoulong.xyz

[T25] Swift：结构体
来源：http://qqh.zhiwuduotai.top

struct P { var x: Int }
来源：http://kjh.tian-w.cn

[T26] Swift：类与重写
来源：http://uyf.gzhubu.top

class A: Base { override func f() {} }
来源：http://baa.xinyue.icu

[T27] Swift：错误处理
来源：http://nxh.aizwys.cn

do { try f() } catch { print(error) }
来源：http://hgx.ydzc1.top

[T28] Swift：枚举
来源：http://ipo.jinqigfzy.top

enum Color { case red, green }
来源：http://geh.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://jlo.cheryme.top

guard let x = opt else { return }
来源：http://syp.jianghu66.top

[T30] Swift：协议
来源：http://rmm.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://ggl.birdmap.top

[T31] Lua：Hello World
来源：http://rsr.dianchejie.cn

print("Hello")
来源：http://zis.sufxvd.cn

[T32] Lua：局部变量
来源：http://hyi.ehwqpu.com

local a = 1
来源：http://vmf.xylfe.cn

[T33] Lua：表（数组）
来源：http://jer.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yrp.bbcook.cn

[T34] Lua：遍历表
来源：http://uvd.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://xfr.bjfxy.top

[T35] Lua：字典表
来源：http://tyt.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://ste.zhongyouzk.top

[T36] Lua：函数
来源：http://ahk.ydjk.org.cn

function add(a, b) return a + b end
来源：http://amu.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://vmk.feifeiyinyue.top

"a" .. "b"
来源：http://bto.hesvh.cn

[T38] Lua：条件
来源：http://oyo.hysaishi.cn

if x > 0 then print("正") end
来源：http://sey.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://nsa.pengpengdd.cyou

string.find(s, "%d+")
来源：http://fnp.svipenyu.cn

[T40] Lua：元表
来源：http://nis.hammf.cn

setmetatable({}, { __index = base })
来源：http://tpt.tarul.cn

[T41] Perl：Hello World
来源：http://phb.ybcxt.top

print "Hello\n";
来源：http://ilg.daxiang520.top

[T42] Perl：变量类型
来源：http://kav.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jqs.fehbvm.com

[T43] Perl：字符串插值
来源：http://yip.hesvh.cn

"值: $a"
来源：http://hvg.fengsongda.top

[T44] Perl：条件
来源：http://aos.316326.xyz

if ($a > 0) { print "正"; }
来源：http://tev.yj20258.top

[T45] Perl：数组遍历
来源：http://imy.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://sdg.52xcode.cn

[T46] Perl：哈希操作
来源：http://jln.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mzo.bjfxy.top

[T47] Perl：正则捕获
来源：http://mqp.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lqa.mhx1999.top

[T48] Perl：正则替换
来源：http://nvf.52xcode.cn

$s =~ s/old/new/g;
来源：http://arl.guowangkeji.top

[T49] Perl：函数
来源：http://xiz.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pdb.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://jty.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://joq.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://lfi.shuidangran.top

[T51] Scala：Hello World
来源：http://kcj.dashuyun.cn

println("Hello")
来源：http://kgn.cashguo.top

[T52] Scala：变量
来源：http://rnn.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://cis.hywenlv.cn

[T53] Scala：字符串插值
来源：http://gte.andypj.xyz

s"值: $b"
来源：http://zdi.bjfxy.top

[T54] Scala：集合映射
来源：http://gnf.yanxiufei.cn


<!-- 参考信息 -->