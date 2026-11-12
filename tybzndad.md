代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tjb.jlsjyb.cn

[R56] 远程拷贝
来源：http://aza.fktsv.cn

scp file user@host:/path/
来源：http://pwv.gaohongyu789.top

[R57] 远程执行命令
来源：http://zqr.bjfxy.top

ssh user@host 'uptime'
来源：http://oql.hnqzz.top

[R58] 下载文件
来源：http://rut.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oer.fzhhl.top

[R59] 发 POST JSON
来源：http://elw.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xjr.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://izb.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fmh.yj202588.top

[R61] 磁盘占用
来源：http://jmw.yangfankeji.com

df -h;  du -sh *
来源：http://zxd.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://otp.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://sui.jyoumei.cn

[R63] 内存与进程
来源：http://cmx.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://gwx.dianchejie.cn

[R64] 结束进程
来源：http://lad.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://hxq.gotoacloud.top

[R65] 查看端口占用
来源：http://kxt.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tkz.shzxlz.cn

[R66] 定时任务
来源：http://efy.chenzaomai.com

crontab -e;  crontab -l
来源：http://nnz.fehbvm.com

[R67] 生成随机十六进制串
来源：http://wmc.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://zcn.dashuyun.cn

[R68] 计算文件校验值
来源：http://cje.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://ubx.jinqigufen.top

[R69] 生成随机密码
来源：http://clq.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://kbf.ydzc1.top

[R70] 时间戳与互转
来源：http://cyi.cheryme.top

date +%s;  date -d @1700000000
来源：http://nup.ybcxt.top

[R71] 日期格式化
来源：http://msf.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uto.aibaodan.cn

[R72] 等待端口就绪
来源：http://zpw.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zxy.kuanghao11.cn

[R73] 分割大日志
来源：http://xma.hysaishi.cn

split -l 1000 big.log part_
来源：http://uqr.chenjidiqi.icu

[R74] 批量重命名
来源：http://yvy.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uws.9152youxi.cn

[R75] 导出环境变量
来源：http://xti.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://fwz.pengpengdd.cyou

[R76] 使用临时文件
来源：http://wjv.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://des.guannengcc.top

[R77] 读取用户输入
来源：http://pdf.zhoulong.xyz

read -rp "请输入: " ans
来源：http://wmd.fzhhl.top

[R78] 交互式菜单
来源：http://siq.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zqc.jiagoushi.top

[R79] 解析命令行选项
来源：http://yxb.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lbp.yonumen.top

[R80] 查看脚本执行耗时
来源：http://jan.andypj.xyz

time ./run.sh
来源：http://zbj.svipenyu.cn

================================================================================
来源：http://qsg.chenzaomai.com

S. C / C++ 专题
来源：http://bab.yangfankeji.com

================================================================================
来源：http://djj.dianchejie.cn

[S01] C：Hello World
来源：http://ams.jqgfzy.top

#include <stdio.h>
来源：http://pmy.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fag.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://bin.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://ucy.feifeiyinyue.top

[S03] C：读入整数
来源：http://vqm.daxiang520.top

int x; scanf("%d", &x);
来源：http://peo.9152youxi.cn

[S04] C：字符串复制
来源：http://giy.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://myx.shangyingyoupin.top

[S05] C：字符串长度
来源：http://syf.iojbl.cn

strlen(s)
来源：http://xxm.cheryme.top

[S06] C：字符串比较
来源：http://oxe.gaohongyu789.top

strcmp(a, b) == 0
来源：http://did.wangdashe.top

[S07] C：数组遍历求和
来源：http://itn.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zdx.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://ddt.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yes.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://ezl.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fak.hysaishi.cn

[S10] C：指针与解引用
来源：http://ncq.yuxming.cn

int *p = &a;  *p = 5;
来源：http://axg.aibaodan.cn

[S11] C：逐行读文件
来源：http://fvl.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://iau.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qxu.jqgufenzy.top

fclose(f);
来源：http://xeu.jyoumei.cn

[S12] C：写文件
来源：http://ibg.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qiy.yvedp.cn

[S13] C：宏定义
来源：http://dxo.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ksr.dashuyun.cn

[S14] C：枚举
来源：http://slr.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://tjq.quarkkingdee.top

[S15] C：类型转换
来源：http://gck.bjfxy.top

(double) a / b
来源：http://fth.shangyingyoupin.top

[S16] C：位操作置位
来源：http://hix.jinqigufen.top

x |= (1 << 3);
来源：http://ndu.xylfe.cn

[S17] C：安全拼接字符串
来源：http://tym.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uqs.jianghu66.top

[S18] C：命令行参数
来源：http://tdg.gzhubu.top

int main(int argc, char **argv)
来源：http://yum.zhixingplan.top

[S19] C：快速排序
来源：http://lbr.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://pgo.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://lxd.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gev.snrcjt.cn

[S21] C：字符类别判断
来源：http://sck.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rju.jqgufenzy.top

[S22] C：字符串转数字
来源：http://qhh.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://gph.wangshuangyany.cn

[S23] C：随机数
来源：http://wdr.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oja.gotoacloud.top

[S24] C：获取本地时间
来源：http://mcj.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://upy.birdmap.top

[S25] C：内存拷贝
来源：http://wdf.ydzc1.top

memcpy(dst, src, n);
来源：http://zuo.cqqwz.cn

[S26] C：内存清零
来源：http://zzj.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://ibs.gaohongyu789.top

[S27] C：定义常量
来源：http://yto.hesvh.cn

const double PI = 3.14159;
来源：http://rzo.shuidangran.top

[S28] C：静态变量
来源：http://qjq.pengpengdd.cyou

static int counter = 0;
来源：http://xrt.tian-w.cn

[S29] C：变参函数
来源：http://adf.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hck.hongshengwenyu.top

[S30] C：头文件保护
来源：http://pvs.shanyushiyangtech.top

#ifndef X_H
来源：http://iug.gotoacloud.top

#define X_H
来源：http://gwd.jqgufenzy.top

#endif
来源：http://org.snrcjt.cn

[S31] C++：Hello World
来源：http://vfh.nanxuanxn.top

#include <iostream>
来源：http://nic.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://qyq.ctjpmb.com

[S32] C++：字符串
来源：http://fyl.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://sky.gotoacloud.top

[S33] C++：vector 增删
来源：http://dgk.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bgr.vehdjk.com

[S34] C++：遍历 vector
来源：http://ofo.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://hup.bjfxy.top

[S35] C++：map
来源：http://hgj.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gyr.cucudq.cn

[S36] C++：unordered_map
来源：http://ynb.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iod.jqgufenzy.top

[S37] C++：set
来源：http://clz.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ltu.ydjk.org.cn

[S38] C++：排序
来源：http://qjv.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://tkj.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://owq.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iik.9152youxi.cn

[S40] C++：查找元素
来源：http://cmi.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxs.haohaochexian.top

[S41] C++：类与构造函数
来源：http://pov.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pdx.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://orc.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://pel.svipenyu.cn

[S43] C++：智能指针
来源：http://jny.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://mdr.cashguo.top

[S44] C++：引用传参
来源：http://mge.bjfxy.top

void inc(int &x) { ++x; }
来源：http://yrn.hnqzz.top

[S45] C++：lambda
来源：http://yqz.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rnf.hongshengwenyu.top

[S46] C++：函数模板
来源：http://ktu.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cey.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://jwy.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vke.cdnleiting.top

[S48] C++：逐行读文件
来源：http://qsb.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://ndh.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://nmh.fzhhl.top

[S49] C++：写文件
来源：http://wgs.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tew.redwolf501.top

[S50] C++：格式化数字
来源：http://cij.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jny.haohaochexian.top

[S51] C++：显式类型转换
来源：http://wad.uphjek.com

static_cast<double>(a) / b
来源：http://est.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://wxn.316326.xyz

int size() const noexcept { return n_; }
来源：http://zrs.andypj.xyz

[S53] C++：移动语义
来源：http://rlf.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://yso.52xcode.cn

[S54] C++：异常处理
来源：http://ktn.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jko.tian-w.cn

[S55] C++：结构化绑定
来源：http://zxx.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bzf.chenlongwang.top

[S56] C++：optional
来源：http://qcz.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://agn.tarul.cn

[S57] C++：编译期常量
来源：http://rfr.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://dzk.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://iny.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://bog.iojbl.cn

[S59] C++：静态断言
来源：http://gba.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cjb.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://ifm.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nll.haohaochexian.top

================================================================================
来源：http://cuk.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://taf.iojbl.cn

================================================================================
来源：http://xzf.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://fgq.cheryme.top

println("Hello")
来源：http://clt.birdmap.top

[T02] Kotlin：变量
来源：http://cdc.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mgq.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://yyy.cashguo.top

"值: $b"
来源：http://fih.yuxming.cn

[T04] Kotlin：空安全
来源：http://ycl.hywenlv.cn

val n: String? = null;  n?.length
来源：http://znw.tanke756.top

[T05] Kotlin：when 表达式
来源：http://pcf.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iee.meibo888.top

[T06] Kotlin：集合映射
来源：http://yrl.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yqw.sweek.top

[T07] Kotlin：集合过滤
来源：http://bkm.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://atw.jianghu66.top

[T08] Kotlin：数据类
来源：http://syg.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://lst.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://cle.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://uox.fktsv.cn

[T10] Kotlin：默认参数
来源：http://fmx.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mln.jqgufenzy.top

[T11] Kotlin：协程
来源：http://iki.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ohg.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://aen.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://ego.yongpay.top

[T13] Kotlin：只读 Map
来源：http://hwv.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://viz.yuanzhike.top

[T14] Kotlin：循环
来源：http://efs.iojbl.cn

for (i in 1..10) println(i)
来源：http://vay.yvedp.cn

[T15] Kotlin：接口
来源：http://iwu.316326.xyz

interface Shape { fun area(): Double }
来源：http://pne.cdnleiting.top

[T16] Swift：Hello World
来源：http://iqt.cqqwz.cn

print("Hello")
来源：http://qwx.haohaochexian.top

[T17] Swift：变量与常量
来源：http://djh.chenzaomai.com

var a = 1;  let b = 2
来源：http://eyg.fehbvm.com

[T18] Swift：字符串插值
来源：http://snd.cashguo.top

"值: \(b)"
来源：http://hfj.yfazqb.com

[T19] Swift：可选绑定
来源：http://ats.ydzc1.top

if let n = opt { print(n) }
来源：http://rdk.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://rqp.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lki.yanxiufei.cn

[T21] Swift：遍历
来源：http://lvs.snrcjt.cn

for x in a { print(x) }
来源：http://pqa.tarul.cn

[T22] Swift：字典
来源：http://ljc.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://tgt.yvedp.cn

[T23] Swift：函数
来源：http://cbh.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cii.epnwcf.com

[T24] Swift：闭包
来源：http://wlr.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gai.shzxlz.cn

[T25] Swift：结构体
来源：http://wzn.zhoulong.xyz

struct P { var x: Int }
来源：http://mxl.zycfv.cn

[T26] Swift：类与重写
来源：http://unt.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://djk.tian-w.cn

[T27] Swift：错误处理
来源：http://myb.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://mrx.dianchejie.cn

[T28] Swift：枚举
来源：http://ebd.ydjk.org.cn

enum Color { case red, green }
来源：http://pnk.cheryme.top

[T29] Swift：guard 提前返回
来源：http://zaq.ydjk.org.cn

guard let x = opt else { return }
来源：http://ktt.yvedp.cn

[T30] Swift：协议
来源：http://lte.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://lbw.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://kjw.fzhhl.top

print("Hello")
来源：http://ite.havefunace.top

[T32] Lua：局部变量
来源：http://htt.jinqigufen.top

local a = 1
来源：http://tei.birdmap.top

[T33] Lua：表（数组）
来源：http://vpz.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gtd.hesvh.cn

[T34] Lua：遍历表
来源：http://php.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ejp.chenlongwang.top

[T35] Lua：字典表
来源：http://joi.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://eig.chenjidiqi.icu

[T36] Lua：函数
来源：http://xvz.zhongyouzk.top

function add(a, b) return a + b end
来源：http://cgn.cheryme.top

[T37] Lua：字符串拼接
来源：http://hkh.shanyushiyangtech.top

"a" .. "b"
来源：http://syf.bjfxy.top

[T38] Lua：条件
来源：http://tep.yuanzhike.top

if x > 0 then print("正") end
来源：http://jnz.cheryme.top

[T39] Lua：模式匹配
来源：http://kco.yj20258888.top

string.find(s, "%d+")
来源：http://poz.hysaishi.cn

[T40] Lua：元表
来源：http://tjh.iojbl.cn

setmetatable({}, { __index = base })
来源：http://nnn.meibo888.top

[T41] Perl：Hello World
来源：http://sdw.zhoulong.xyz

print "Hello\n";
来源：http://tll.yonumen.top

[T42] Perl：变量类型
来源：http://uwm.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eii.jinqigufen.top

[T43] Perl：字符串插值
来源：http://zyf.hcnkem.com

"值: $a"
来源：http://qmm.chenlongwang.top

[T44] Perl：条件
来源：http://ttr.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://cdh.bbcook.cn

[T45] Perl：数组遍历
来源：http://zwt.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://tez.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://xgh.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://voe.guowangkeji.top

[T47] Perl：正则捕获
来源：http://luy.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pwy.jqgfzy.top

[T48] Perl：正则替换
来源：http://ngy.cdnleiting.top

$s =~ s/old/new/g;
来源：http://sle.bjfxy.top

[T49] Perl：函数
来源：http://pfc.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jtx.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://vio.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gzf.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://itb.sysykeji.top

[T51] Scala：Hello World
来源：http://cvd.zhoulong.xyz

println("Hello")
来源：http://yln.kuanghao11.cn

[T52] Scala：变量
来源：http://wwy.epnwcf.com

val a = 1;  var b = 2
来源：http://mtp.shzxlz.cn

[T53] Scala：字符串插值
来源：http://lhf.hongshengwenyu.top

s"值: $b"
来源：http://asq.birdmap.top

[T54] Scala：集合映射
来源：http://nwr.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://eeu.hammf.cn

[T55] Scala：集合过滤
来源：http://scc.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://blb.zhijiandao.cn

[T56] Scala：样例类
来源：http://gui.iojbl.cn

case class User(name: String, age: Int)
来源：http://cqm.vehdjk.com

[T57] Scala：模式匹配
来源：http://ucs.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zro.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://mpg.cdnleiting.top


<!-- 参考信息 -->