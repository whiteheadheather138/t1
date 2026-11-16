代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsg.xuetiantiany.cn

[R54] 比较两个文件
来源：http://ajw.pycfn.com

diff a.txt b.txt
来源：http://brm.hammf.cn

[R55] 压缩与解压
来源：http://qqe.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iii.hongshengwenyu.top

[R56] 远程拷贝
来源：http://brt.aizwys.cn

scp file user@host:/path/
来源：http://rau.zhixingplan.top

[R57] 远程执行命令
来源：http://muq.hnqzz.top

ssh user@host 'uptime'
来源：http://pgz.shanyushiyangkeji.top

[R58] 下载文件
来源：http://cyp.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hds.xziqi.cn

[R59] 发 POST JSON
来源：http://cek.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqw.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://xes.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpf.quarkkingdee.top

[R61] 磁盘占用
来源：http://qyz.smart0.xyz

df -h;  du -sh *
来源：http://wfr.zdbjq.cn

[R62] 找最占空间的文件
来源：http://ccs.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://ovv.fanxiaobao.xyz

[R63] 内存与进程
来源：http://wdb.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://ewh.xuetiantiany.cn

[R64] 结束进程
来源：http://elp.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://egj.hfpthk.cn

[R65] 查看端口占用
来源：http://aiw.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fwe.yongpay.top

[R66] 定时任务
来源：http://vxs.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://qyi.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://fpd.bjfxy.top

openssl rand -hex 16
来源：http://csi.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://nhc.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://mww.shangyingyoupin.top

[R69] 生成随机密码
来源：http://dmf.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://gsi.yonumen.top

[R70] 时间戳与互转
来源：http://lfq.tian-w.cn

date +%s;  date -d @1700000000
来源：http://std.shuidangran.top

[R71] 日期格式化
来源：http://pfi.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lse.hcnkem.com

[R72] 等待端口就绪
来源：http://xde.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wzc.fengsongda.top

[R73] 分割大日志
来源：http://lrf.tianlin.xyz

split -l 1000 big.log part_
来源：http://xrn.yongpay.top

[R74] 批量重命名
来源：http://lnu.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://izx.sufxvd.cn

[R75] 导出环境变量
来源：http://nuo.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://mhs.xinyue.icu

[R76] 使用临时文件
来源：http://zpm.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wdk.ehwqpu.com

[R77] 读取用户输入
来源：http://oop.9152youxi.cn

read -rp "请输入: " ans
来源：http://jqq.9152youxi.cn

[R78] 交互式菜单
来源：http://jnq.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://eix.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://wsf.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ypl.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://yqm.hysaishi.cn

time ./run.sh
来源：http://wkt.daria6918.cn

================================================================================
来源：http://zyx.guannengcc.top

S. C / C++ 专题
来源：http://eut.52xcode.cn

================================================================================
来源：http://vyo.uphjek.com

[S01] C：Hello World
来源：http://ywr.daxiang520.top

#include <stdio.h>
来源：http://lke.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://erk.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://cba.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://sfg.aizwys.cn

[S03] C：读入整数
来源：http://nbb.zdqjudy.top

int x; scanf("%d", &x);
来源：http://nvw.yueranfly.top

[S04] C：字符串复制
来源：http://dvt.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dst.0kj1m.cn

[S05] C：字符串长度
来源：http://unu.fzhhl.top

strlen(s)
来源：http://bke.fzhhl.top

[S06] C：字符串比较
来源：http://lcf.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://jik.hfpthk.cn

[S07] C：数组遍历求和
来源：http://nuo.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nbq.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://dll.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ewl.sweek.top

[S09] C：结构体定义与初始化
来源：http://eus.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iyd.vqdsnc.cn

[S10] C：指针与解引用
来源：http://hyx.yueranfly.top

int *p = &a;  *p = 5;
来源：http://rdz.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://unl.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://owi.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://qyz.ybcxt.top

fclose(f);
来源：http://gnr.yj20258888.top

[S12] C：写文件
来源：http://eba.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gbw.fanxiaobao.xyz

[S13] C：宏定义
来源：http://mbl.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://juo.ydjk.org.cn

[S14] C：枚举
来源：http://htv.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://xrd.nanxuanxn.top

[S15] C：类型转换
来源：http://cwo.shanyushiyangtech.top

(double) a / b
来源：http://jap.birdmap.top

[S16] C：位操作置位
来源：http://ids.sysykeji.top

x |= (1 << 3);
来源：http://ibt.iojbl.cn

[S17] C：安全拼接字符串
来源：http://ywd.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jjg.yuxming.cn

[S18] C：命令行参数
来源：http://zmw.0kj1m.cn

int main(int argc, char **argv)
来源：http://vkd.hysaishi.cn

[S19] C：快速排序
来源：http://xff.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://vtj.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://tor.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bhd.fehbvm.com

[S21] C：字符类别判断
来源：http://pcs.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nth.fktsv.cn

[S22] C：字符串转数字
来源：http://hlw.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xho.redwolf501.top

[S23] C：随机数
来源：http://xww.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://izk.kuanghao11.cn

[S24] C：获取本地时间
来源：http://dmq.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://etc.daria6918.cn

[S25] C：内存拷贝
来源：http://luh.zdbjq.cn

memcpy(dst, src, n);
来源：http://tit.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://jtb.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://zpz.yangfankeji.com

[S27] C：定义常量
来源：http://wec.feifeiyinyue.top

const double PI = 3.14159;
来源：http://vdi.aibaodan.cn

[S28] C：静态变量
来源：http://vdg.shanyushiyangtech.top

static int counter = 0;
来源：http://lln.sjlbkw.cn

[S29] C：变参函数
来源：http://qve.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oek.havefunace.top

[S30] C：头文件保护
来源：http://bxr.shuidangran.top

#ifndef X_H
来源：http://cos.tanke756.top

#define X_H
来源：http://mxb.ydjk.org.cn

#endif
来源：http://qkm.sysykeji.top

[S31] C++：Hello World
来源：http://umh.ydzc1.top

#include <iostream>
来源：http://ntq.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://kkc.jinqigfzy.top

[S32] C++：字符串
来源：http://lhu.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://llm.zhijiandao.cn

[S33] C++：vector 增删
来源：http://znf.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://knv.ctjpmb.com

[S34] C++：遍历 vector
来源：http://zde.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://yqa.yj202588.top

[S35] C++：map
来源：http://qmn.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fzr.meibo888.top

[S36] C++：unordered_map
来源：http://ekh.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xfh.wangdashe.top

[S37] C++：set
来源：http://vao.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xqg.ctjpmb.com

[S38] C++：排序
来源：http://fal.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://jaa.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://nig.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cuu.xylfe.cn

[S40] C++：查找元素
来源：http://pvi.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dkn.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://vzr.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yak.xziqi.cn

[S42] C++：继承与虚函数
来源：http://hni.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://djd.chenjidiqi.icu

[S43] C++：智能指针
来源：http://evo.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://lxh.haohaochexian.top

[S44] C++：引用传参
来源：http://ojf.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://qyk.zhixingplan.top

[S45] C++：lambda
来源：http://cdv.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://rei.zhengqikj.top

[S46] C++：函数模板
来源：http://lee.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yjd.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://imc.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bnm.316326.xyz

[S48] C++：逐行读文件
来源：http://npm.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://sam.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://roq.yonumen.top

[S49] C++：写文件
来源：http://ybd.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ayt.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://fyb.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oek.yueranfly.top

[S51] C++：显式类型转换
来源：http://wlq.xylfe.cn

static_cast<double>(a) / b
来源：http://hpr.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://uxv.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://yrx.zhijiandao.cn

[S53] C++：移动语义
来源：http://nsc.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://doq.cdnleiting.top

[S54] C++：异常处理
来源：http://ktf.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qsx.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://ctm.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://myt.cashguo.top

[S56] C++：optional
来源：http://hbo.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zlo.fengsongda.top

[S57] C++：编译期常量
来源：http://hwi.nwbrower.top

constexpr int N = 10;
来源：http://rqu.ybcxt.top

[S58] C++：命名空间
来源：http://zgy.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://qhf.jlsjyb.cn

[S59] C++：静态断言
来源：http://vtl.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://egt.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://exb.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qul.bjfxy.top

================================================================================
来源：http://arj.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xrz.birdmap.top

================================================================================
来源：http://efq.xuanzx.com

[T01] Kotlin：Hello World
来源：http://gun.cheryme.top

println("Hello")
来源：http://zml.chenlongwang.top

[T02] Kotlin：变量
来源：http://aeg.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://euw.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://xxg.hongshengwenyu.top

"值: $b"
来源：http://xzc.hesvh.cn

[T04] Kotlin：空安全
来源：http://eyh.cdnleiting.top

val n: String? = null;  n?.length
来源：http://fbs.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://mhg.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://prg.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://iwm.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mzx.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://npy.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vlh.tanke756.top

[T08] Kotlin：数据类
来源：http://wlu.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://vne.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://kao.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://zdp.gzhubu.top

[T10] Kotlin：默认参数
来源：http://oat.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pvg.yvedp.cn

[T11] Kotlin：协程
来源：http://odp.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jqc.shuidangran.top

[T12] Kotlin：解构声明
来源：http://bxp.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://pop.birdmap.top

[T13] Kotlin：只读 Map
来源：http://tgx.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://zls.c1oappe.top

[T14] Kotlin：循环
来源：http://los.hysaishi.cn

for (i in 1..10) println(i)
来源：http://lps.xylfe.cn

[T15] Kotlin：接口
来源：http://ngy.yuxming.cn

interface Shape { fun area(): Double }
来源：http://oxu.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://eoe.9152youxi.cn

print("Hello")
来源：http://iaz.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://ioq.cdnleiting.top

var a = 1;  let b = 2
来源：http://uzp.zdqjudy.top

[T18] Swift：字符串插值
来源：http://lxl.dianchejie.cn

"值: \(b)"
来源：http://nmh.yfazqb.com

[T19] Swift：可选绑定
来源：http://hym.tarul.cn

if let n = opt { print(n) }
来源：http://meu.daria6918.cn

[T20] Swift：数组操作
来源：http://loc.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tau.sufxvd.cn

[T21] Swift：遍历
来源：http://aqr.zdqjudy.top

for x in a { print(x) }
来源：http://ocf.yanxiufei.cn

[T22] Swift：字典
来源：http://omd.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://xui.hysaishi.cn

[T23] Swift：函数
来源：http://gaj.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kil.yanxiufei.cn

[T24] Swift：闭包
来源：http://ugo.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://zel.shangyingyoupin.top

[T25] Swift：结构体
来源：http://yye.quarkkingdee.top

struct P { var x: Int }
来源：http://oun.dianchejie.cn

[T26] Swift：类与重写
来源：http://gwa.jinqigufen.top

class A: Base { override func f() {} }
来源：http://vre.cdnleiting.top

[T27] Swift：错误处理
来源：http://dzs.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://xbx.9152youxi.cn

[T28] Swift：枚举
来源：http://skk.hcnkem.com

enum Color { case red, green }
来源：http://wwu.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://amx.zhixingplan.top

guard let x = opt else { return }
来源：http://cqp.yj202588.top

[T30] Swift：协议
来源：http://phc.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://ted.chenzaomai.com

[T31] Lua：Hello World
来源：http://jcv.yueranfly.top

print("Hello")
来源：http://mfj.fzhhl.top

[T32] Lua：局部变量
来源：http://hwk.hfpthk.cn

local a = 1
来源：http://ylr.zhengqikj.top

[T33] Lua：表（数组）
来源：http://ayx.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yqx.chenlongwang.top

[T34] Lua：遍历表
来源：http://vtk.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://soa.sufxvd.cn

[T35] Lua：字典表
来源：http://uhr.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://cep.quarkkingdee.top

[T36] Lua：函数
来源：http://tax.dashuyun.cn

function add(a, b) return a + b end
来源：http://oqy.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://omc.ybcxt.top

"a" .. "b"
来源：http://lkb.yvedp.cn

[T38] Lua：条件
来源：http://tgj.sufxvd.cn

if x > 0 then print("正") end
来源：http://zaq.meibo888.top

[T39] Lua：模式匹配
来源：http://coa.aizwys.cn

string.find(s, "%d+")
来源：http://nvx.hammf.cn

[T40] Lua：元表
来源：http://cca.havefunace.top

setmetatable({}, { __index = base })
来源：http://dgf.fehbvm.com

[T41] Perl：Hello World
来源：http://jpv.xuetiantiany.cn

print "Hello\n";
来源：http://nih.jiagoushi.top

[T42] Perl：变量类型
来源：http://egt.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kpr.yuanzhike.top

[T43] Perl：字符串插值
来源：http://bey.xziqi.cn

"值: $a"
来源：http://izo.zhijiandao.cn

[T44] Perl：条件
来源：http://lcg.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://sqd.cashguo.top

[T45] Perl：数组遍历
来源：http://eko.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://qlx.hysaishi.cn

[T46] Perl：哈希操作
来源：http://xvt.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://elv.snrcjt.cn

[T47] Perl：正则捕获
来源：http://imi.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zzp.shzxlz.cn

[T48] Perl：正则替换
来源：http://hwj.jiagoushi.top

$s =~ s/old/new/g;
来源：http://vjh.fktsv.cn

[T49] Perl：函数
来源：http://gau.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ivh.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://yod.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://onu.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://zbq.hesvh.cn

[T51] Scala：Hello World
来源：http://sdu.yongpay.top

println("Hello")
来源：http://blb.0kj1m.cn

[T52] Scala：变量
来源：http://mjt.fzhhl.top

val a = 1;  var b = 2
来源：http://nxv.fengsongda.top

[T53] Scala：字符串插值
来源：http://yag.shzxlz.cn

s"值: $b"
来源：http://ktk.dashuyun.cn

[T54] Scala：集合映射
来源：http://fbx.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://bqb.meibo888.top

[T55] Scala：集合过滤
来源：http://wfv.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://oxw.hnqzz.top

[T56] Scala：样例类
来源：http://lyo.hysaishi.cn


<!-- 参考信息 -->