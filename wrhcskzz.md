代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://psr.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://vfh.pengpengdd.cyou

scp file user@host:/path/
来源：http://yrg.cheryme.top

[R57] 远程执行命令
来源：http://cpb.jiagoushi.top

ssh user@host 'uptime'
来源：http://wzp.gogol.net.cn

[R58] 下载文件
来源：http://ppk.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mng.zhongyouzk.top

[R59] 发 POST JSON
来源：http://kko.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wij.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://zgn.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://geu.tian-w.cn

[R61] 磁盘占用
来源：http://qri.hesvh.cn

df -h;  du -sh *
来源：http://myb.fktsv.cn

[R62] 找最占空间的文件
来源：http://hky.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://ndw.xziqi.cn

[R63] 内存与进程
来源：http://bmv.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://kiy.9152youxi.cn

[R64] 结束进程
来源：http://kun.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://nwp.yanxiufei.cn

[R65] 查看端口占用
来源：http://lfn.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlf.sweek.top

[R66] 定时任务
来源：http://usa.havefunace.top

crontab -e;  crontab -l
来源：http://qya.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://lxd.zhengqikj.top

openssl rand -hex 16
来源：http://ksr.sxryk.cn

[R68] 计算文件校验值
来源：http://xnc.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mwy.yongpay.top

[R69] 生成随机密码
来源：http://xxw.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://jxe.yuanzhike.top

[R70] 时间戳与互转
来源：http://hut.guannengcc.top

date +%s;  date -d @1700000000
来源：http://wiu.kuanghao11.cn

[R71] 日期格式化
来源：http://tmr.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://byc.hfpthk.cn

[R72] 等待端口就绪
来源：http://jhm.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zdh.tanke756.top

[R73] 分割大日志
来源：http://zzj.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://ahz.zycfv.cn

[R74] 批量重命名
来源：http://tcz.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bci.ydjk.org.cn

[R75] 导出环境变量
来源：http://hng.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://aaz.yuanzhike.top

[R76] 使用临时文件
来源：http://mme.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://knh.guowangkeji.top

[R77] 读取用户输入
来源：http://hwt.ydjk.org.cn

read -rp "请输入: " ans
来源：http://wgh.tanke756.top

[R78] 交互式菜单
来源：http://tew.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vwe.gotoacloud.top

[R79] 解析命令行选项
来源：http://fdc.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cqf.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://iod.gaohongyu789.top

time ./run.sh
来源：http://tkp.hywenlv.cn

================================================================================
来源：http://ibd.bbcook.cn

S. C / C++ 专题
来源：http://qlm.andypj.xyz

================================================================================
来源：http://ypv.316326.xyz

[S01] C：Hello World
来源：http://the.tianlin.xyz

#include <stdio.h>
来源：http://qgy.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ojm.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://ooz.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://uat.shangyingyoupin.top

[S03] C：读入整数
来源：http://vbj.andypj.xyz

int x; scanf("%d", &x);
来源：http://tyo.pycfn.com

[S04] C：字符串复制
来源：http://khr.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://zut.yj20258.top

[S05] C：字符串长度
来源：http://gdk.cashguo.top

strlen(s)
来源：http://oii.smart0.xyz

[S06] C：字符串比较
来源：http://svr.52xcode.cn

strcmp(a, b) == 0
来源：http://tqh.yangfankeji.com

[S07] C：数组遍历求和
来源：http://uqt.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pxs.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://rbz.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pae.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://xhn.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fcp.jinqigufen.top

[S10] C：指针与解引用
来源：http://zfd.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://sgn.ctjpmb.com

[S11] C：逐行读文件
来源：http://ama.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://xwz.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://emn.ywan-chungtsiang.top

fclose(f);
来源：http://fek.fktsv.cn

[S12] C：写文件
来源：http://kor.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://onz.fktsv.cn

[S13] C：宏定义
来源：http://wgx.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://byr.tianlin.xyz

[S14] C：枚举
来源：http://mgi.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://oip.c1oappe.top

[S15] C：类型转换
来源：http://ywt.cqqwz.cn

(double) a / b
来源：http://gfe.zhengqikj.top

[S16] C：位操作置位
来源：http://gpg.cucudq.cn

x |= (1 << 3);
来源：http://vku.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://bal.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lmw.shuidangran.top

[S18] C：命令行参数
来源：http://eki.52xcode.cn

int main(int argc, char **argv)
来源：http://kcr.fehbvm.com

[S19] C：快速排序
来源：http://ope.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mty.smart0.xyz

[S20] C：二分查找
来源：http://qwz.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ohc.cheryme.top

[S21] C：字符类别判断
来源：http://egf.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yso.yongpay.top

[S22] C：字符串转数字
来源：http://zkm.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xrf.hongshengwenyu.top

[S23] C：随机数
来源：http://paa.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ulc.yj202588.top

[S24] C：获取本地时间
来源：http://lzu.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ojh.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://rsm.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://grq.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://uxi.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://gnc.vehdjk.com

[S27] C：定义常量
来源：http://sbu.hnqzz.top

const double PI = 3.14159;
来源：http://yhd.52xcode.cn

[S28] C：静态变量
来源：http://mvc.xinyue.icu

static int counter = 0;
来源：http://geo.bjfxy.top

[S29] C：变参函数
来源：http://coj.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oqa.yj20258.top

[S30] C：头文件保护
来源：http://pwp.cdnleiting.top

#ifndef X_H
来源：http://cbs.jinqigfzy.top

#define X_H
来源：http://fmj.jianghu66.top

#endif
来源：http://xzf.epnwcf.com

[S31] C++：Hello World
来源：http://dhp.hongshengwenyu.top

#include <iostream>
来源：http://rja.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://uqc.hammf.cn

[S32] C++：字符串
来源：http://lpl.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://wmg.ybcxt.top

[S33] C++：vector 增删
来源：http://sjj.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aug.jianghu66.top

[S34] C++：遍历 vector
来源：http://dsp.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://svk.yj20258888.top

[S35] C++：map
来源：http://bre.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nso.hnxiangtu.top

[S36] C++：unordered_map
来源：http://crv.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xgu.pycfn.com

[S37] C++：set
来源：http://uyz.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agj.jinyuanbaomall.cn

[S38] C++：排序
来源：http://wrd.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://wnn.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://jwe.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://igt.zycfv.cn

[S40] C++：查找元素
来源：http://mmz.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sgb.xziqi.cn

[S41] C++：类与构造函数
来源：http://xvp.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwi.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://ydo.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://fel.andypj.xyz

[S43] C++：智能指针
来源：http://lri.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://naz.yj202588.top

[S44] C++：引用传参
来源：http://ued.birdmap.top

void inc(int &x) { ++x; }
来源：http://iru.tianlin.xyz

[S45] C++：lambda
来源：http://yts.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://xdk.nanxuanxn.top

[S46] C++：函数模板
来源：http://byf.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qro.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://eex.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ksi.fengsongda.top

[S48] C++：逐行读文件
来源：http://dyv.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://cee.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://uhv.ehwqpu.com

[S49] C++：写文件
来源：http://nnf.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mdp.sweek.top

[S50] C++：格式化数字
来源：http://gwq.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://itc.zdbjq.cn

[S51] C++：显式类型转换
来源：http://bdg.ydjk.org.cn

static_cast<double>(a) / b
来源：http://lss.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://urh.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://pmq.hammf.cn

[S53] C++：移动语义
来源：http://xso.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://tkp.yonumen.top

[S54] C++：异常处理
来源：http://rur.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jsu.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://dih.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngr.iojbl.cn

[S56] C++：optional
来源：http://yjn.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwr.wangdashe.top

[S57] C++：编译期常量
来源：http://hsd.tarul.cn

constexpr int N = 10;
来源：http://wbi.yanxiufei.cn

[S58] C++：命名空间
来源：http://bpl.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://eus.vqdsnc.cn

[S59] C++：静态断言
来源：http://xtt.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jpq.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://upr.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mij.mhx1999.top

================================================================================
来源：http://jcm.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbd.meibo888.top

================================================================================
来源：http://yxz.uphjek.com

[T01] Kotlin：Hello World
来源：http://tte.tian-w.cn

println("Hello")
来源：http://lar.zhixingplan.top

[T02] Kotlin：变量
来源：http://ude.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://omi.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://vtt.gzhubu.top

"值: $b"
来源：http://gpc.xuanzx.com

[T04] Kotlin：空安全
来源：http://qbw.sxryk.cn

val n: String? = null;  n?.length
来源：http://plk.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://vmh.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://glh.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://fup.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kfr.316326.xyz

[T07] Kotlin：集合过滤
来源：http://knx.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nht.tanke756.top

[T08] Kotlin：数据类
来源：http://huf.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://aqs.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://ldm.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://eka.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://zcl.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sbi.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://urd.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gtx.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://zwf.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://jwm.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://nir.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://muv.nanxuanxn.top

[T14] Kotlin：循环
来源：http://nba.xziqi.cn

for (i in 1..10) println(i)
来源：http://xlm.xziqi.cn

[T15] Kotlin：接口
来源：http://egm.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://hye.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://lyo.ehwqpu.com

print("Hello")
来源：http://gwg.jinqigufen.top

[T17] Swift：变量与常量
来源：http://ulh.0kj1m.cn

var a = 1;  let b = 2
来源：http://ahq.nwbrower.top

[T18] Swift：字符串插值
来源：http://lyq.zdqjudy.top

"值: \(b)"
来源：http://hlf.0kj1m.cn

[T19] Swift：可选绑定
来源：http://clq.cqqwz.cn

if let n = opt { print(n) }
来源：http://qds.jlsjyb.cn

[T20] Swift：数组操作
来源：http://udn.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://vyb.hywenlv.cn

[T21] Swift：遍历
来源：http://mnv.yfazqb.com

for x in a { print(x) }
来源：http://pas.sufxvd.cn

[T22] Swift：字典
来源：http://fgm.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://ffh.hcnkem.com

[T23] Swift：函数
来源：http://xxd.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dpf.9152youxi.cn

[T24] Swift：闭包
来源：http://ycs.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://iak.yuanzhike.top

[T25] Swift：结构体
来源：http://fcp.yj20258.top

struct P { var x: Int }
来源：http://oti.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://ygu.daria6918.cn

class A: Base { override func f() {} }
来源：http://lak.haohaochexian.top

[T27] Swift：错误处理
来源：http://kjf.yj20258888.top

do { try f() } catch { print(error) }
来源：http://teu.zhixingplan.top

[T28] Swift：枚举
来源：http://ivc.epnwcf.com

enum Color { case red, green }
来源：http://fif.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://ywx.pycfn.com

guard let x = opt else { return }
来源：http://ynj.kuanghao11.cn

[T30] Swift：协议
来源：http://eav.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://aqh.zhijiandao.cn

[T31] Lua：Hello World
来源：http://aet.vehdjk.com

print("Hello")
来源：http://gke.cashguo.top

[T32] Lua：局部变量
来源：http://rdq.ybcxt.top

local a = 1
来源：http://eev.tarul.cn

[T33] Lua：表（数组）
来源：http://ebx.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yna.ehwqpu.com

[T34] Lua：遍历表
来源：http://nrv.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dmu.cdnleiting.top

[T35] Lua：字典表
来源：http://gox.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://ili.fehbvm.com

[T36] Lua：函数
来源：http://lyt.ybcxt.top

function add(a, b) return a + b end
来源：http://roo.ivvv.top

[T37] Lua：字符串拼接
来源：http://nnk.xinyue.icu

"a" .. "b"
来源：http://qmu.hywenlv.cn

[T38] Lua：条件
来源：http://vxj.9152youxi.cn

if x > 0 then print("正") end
来源：http://wis.hfpthk.cn

[T39] Lua：模式匹配
来源：http://jli.hfpthk.cn

string.find(s, "%d+")
来源：http://yrq.hnxiangtu.top

[T40] Lua：元表
来源：http://rpc.yvedp.cn

setmetatable({}, { __index = base })
来源：http://wak.redwolf501.top

[T41] Perl：Hello World
来源：http://bxa.guowangkeji.top

print "Hello\n";
来源：http://pkl.yj202588.top

[T42] Perl：变量类型
来源：http://isg.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pla.guowangkeji.top

[T43] Perl：字符串插值
来源：http://kfn.cdnleiting.top

"值: $a"
来源：http://hyo.yanxiufei.cn

[T44] Perl：条件
来源：http://yzp.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://mco.daxiang520.top

[T45] Perl：数组遍历
来源：http://pdd.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://yqq.havefunace.top

[T46] Perl：哈希操作
来源：http://yrp.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xly.svipenyu.cn

[T47] Perl：正则捕获
来源：http://ezv.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sbn.chenzaomai.com

[T48] Perl：正则替换
来源：http://avc.hnqzz.top

$s =~ s/old/new/g;
来源：http://fpw.sufxvd.cn

[T49] Perl：函数
来源：http://gmo.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xju.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://sle.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://byo.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://onw.zhijiandao.cn

[T51] Scala：Hello World
来源：http://gad.bbcook.cn

println("Hello")
来源：http://kcn.sufxvd.cn

[T52] Scala：变量
来源：http://bnu.chenlongwang.top

val a = 1;  var b = 2
来源：http://upp.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://iju.cheryme.top

s"值: $b"
来源：http://rim.yuxming.cn

[T54] Scala：集合映射
来源：http://cga.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://obt.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://tds.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://rnl.shzxlz.cn

[T56] Scala：样例类
来源：http://jxm.chenzaomai.com

case class User(name: String, age: Int)
来源：http://tve.chenzaomai.com

[T57] Scala：模式匹配
来源：http://fnp.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jbf.jyoumei.cn

[T58] Scala：函数定义
来源：http://ifs.0kj1m.cn


<!-- 参考信息 -->