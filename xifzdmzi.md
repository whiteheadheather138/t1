代发 wailian999

ssh user@host 'uptime'
来源：http://wro.sxryk.cn

[R58] 下载文件
来源：http://xub.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iem.9152youxi.cn

[R59] 发 POST JSON
来源：http://wqb.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vyk.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://mxj.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qho.zhoulong.xyz

[R61] 磁盘占用
来源：http://ysl.cdnleiting.top

df -h;  du -sh *
来源：http://vcq.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://yyl.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://irf.zhoulong.xyz

[R63] 内存与进程
来源：http://cxj.pycfn.com

free -h;  ps aux | grep nginx
来源：http://jkt.shanyushiyangtech.top

[R64] 结束进程
来源：http://bmp.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://uyf.daria6918.cn

[R65] 查看端口占用
来源：http://ylj.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovn.haohaochexian.top

[R66] 定时任务
来源：http://ybf.zhixingplan.top

crontab -e;  crontab -l
来源：http://cfl.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://ucz.dianchejie.cn

openssl rand -hex 16
来源：http://smv.yangfankeji.com

[R68] 计算文件校验值
来源：http://wnv.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://vqw.cqqwz.cn

[R69] 生成随机密码
来源：http://cjg.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://baq.kuanghao11.cn

[R70] 时间戳与互转
来源：http://abd.cashguo.top

date +%s;  date -d @1700000000
来源：http://lew.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://twd.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tyh.meibo888.top

[R72] 等待端口就绪
来源：http://zfl.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://pks.yj20258888.top

[R73] 分割大日志
来源：http://ckb.chenzaomai.com

split -l 1000 big.log part_
来源：http://yzl.ppjwa.cn

[R74] 批量重命名
来源：http://ejl.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://geg.sjlbkw.cn

[R75] 导出环境变量
来源：http://zgi.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://zsb.ctjpmb.com

[R76] 使用临时文件
来源：http://ifo.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://udn.sjlbkw.cn

[R77] 读取用户输入
来源：http://wao.xziqi.cn

read -rp "请输入: " ans
来源：http://tqq.xylfe.cn

[R78] 交互式菜单
来源：http://siu.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://liv.cqqwz.cn

[R79] 解析命令行选项
来源：http://lsp.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tcv.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://ddu.jinqigufen.top

time ./run.sh
来源：http://icb.wangshuangyany.cn

================================================================================
来源：http://mxj.tian-w.cn

S. C / C++ 专题
来源：http://jdn.sxryk.cn

================================================================================
来源：http://kkp.yueranfly.top

[S01] C：Hello World
来源：http://yyq.guowangkeji.top

#include <stdio.h>
来源：http://ukl.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kyi.yj20258888.top

[S02] C：变量与格式化输出
来源：http://hkt.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://mwl.haohaochexian.top

[S03] C：读入整数
来源：http://zet.yangfankeji.com

int x; scanf("%d", &x);
来源：http://zxx.sweek.top

[S04] C：字符串复制
来源：http://vwq.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yjq.epnwcf.com

[S05] C：字符串长度
来源：http://xux.jinghuilouyu.cn

strlen(s)
来源：http://qep.tian-w.cn

[S06] C：字符串比较
来源：http://oym.xylfe.cn

strcmp(a, b) == 0
来源：http://cdx.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://nrc.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tbg.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://jhg.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jil.cheryme.top

[S09] C：结构体定义与初始化
来源：http://ivw.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdc.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://rmv.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://kni.sxryk.cn

[S11] C：逐行读文件
来源：http://rkt.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://dqj.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hcs.chenzaomai.com

fclose(f);
来源：http://dmg.shanyushiyangtech.top

[S12] C：写文件
来源：http://ucn.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ykk.xziqi.cn

[S13] C：宏定义
来源：http://nnd.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://egl.haohaochexian.top

[S14] C：枚举
来源：http://jbj.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://epv.haohaochexian.top

[S15] C：类型转换
来源：http://zch.kuanghao11.cn

(double) a / b
来源：http://avf.feifeiyinyue.top

[S16] C：位操作置位
来源：http://bog.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://lfe.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://bdt.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nzh.jqgufenzy.top

[S18] C：命令行参数
来源：http://bjb.nwbrower.top

int main(int argc, char **argv)
来源：http://skq.jlsjyb.cn

[S19] C：快速排序
来源：http://xad.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://unw.shanyushiyangtech.top

[S20] C：二分查找
来源：http://vwe.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jre.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://odu.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ehs.yuxming.cn

[S22] C：字符串转数字
来源：http://hcp.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://zis.ydjk.org.cn

[S23] C：随机数
来源：http://jir.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mra.mhx1999.top

[S24] C：获取本地时间
来源：http://tii.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uxh.jqgfzy.top

[S25] C：内存拷贝
来源：http://idv.pycfn.com

memcpy(dst, src, n);
来源：http://gid.wangdashe.top

[S26] C：内存清零
来源：http://imo.yongpay.top

memset(a, 0, sizeof a);
来源：http://rzo.mhx1999.top

[S27] C：定义常量
来源：http://uxy.wangshuangyany.cn

const double PI = 3.14159;
来源：http://ijz.zhongyouzk.top

[S28] C：静态变量
来源：http://wiw.52xcode.cn

static int counter = 0;
来源：http://egc.zhijiandao.cn

[S29] C：变参函数
来源：http://kub.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rpu.gzhubu.top

[S30] C：头文件保护
来源：http://mhq.daria6918.cn

#ifndef X_H
来源：http://akw.jiagoushi.top

#define X_H
来源：http://lbo.uphjek.com

#endif
来源：http://agt.jinqigfzy.top

[S31] C++：Hello World
来源：http://tgc.kuanghao11.cn

#include <iostream>
来源：http://clv.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://dsc.zhengqikj.top

[S32] C++：字符串
来源：http://ebq.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://cmm.chenlongwang.top

[S33] C++：vector 增删
来源：http://yni.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukb.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://vvh.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://tfm.ybcxt.top

[S35] C++：map
来源：http://wnx.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jok.quarkkingdee.top

[S36] C++：unordered_map
来源：http://lbb.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://glu.sufxvd.cn

[S37] C++：set
来源：http://exa.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vdf.zhixingplan.top

[S38] C++：排序
来源：http://cfl.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://nwk.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://qbh.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ckd.nwbrower.top

[S40] C++：查找元素
来源：http://twk.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rmu.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://wgk.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mhj.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://gci.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://bim.sweek.top

[S43] C++：智能指针
来源：http://vtr.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://ctw.dashuyun.cn

[S44] C++：引用传参
来源：http://tcw.yongpay.top

void inc(int &x) { ++x; }
来源：http://agw.ivvv.top

[S45] C++：lambda
来源：http://jhm.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://gbe.yueranfly.top

[S46] C++：函数模板
来源：http://rhy.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rxn.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://rit.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqk.pycfn.com

[S48] C++：逐行读文件
来源：http://hzb.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://huy.fehbvm.com

while (std::getline(in, line)) { }
来源：http://ytf.wangdashe.top

[S49] C++：写文件
来源：http://uys.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fdq.cqqwz.cn

[S50] C++：格式化数字
来源：http://nkn.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uua.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://knk.pycfn.com

static_cast<double>(a) / b
来源：http://dvg.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://lqx.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://exy.aizwys.cn

[S53] C++：移动语义
来源：http://dwj.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://del.cheryme.top

[S54] C++：异常处理
来源：http://gpf.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cxv.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://beq.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dgy.nanxuanxn.top

[S56] C++：optional
来源：http://zil.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bye.yangfankeji.com

[S57] C++：编译期常量
来源：http://umo.gotoacloud.top

constexpr int N = 10;
来源：http://gls.vqdsnc.cn

[S58] C++：命名空间
来源：http://jsn.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://pkl.yuanzhike.top

[S59] C++：静态断言
来源：http://xln.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lan.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://vnf.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://joq.c1oappe.top

================================================================================
来源：http://emq.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wso.zhengqikj.top

================================================================================
来源：http://oqw.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://alc.zhixingplan.top

println("Hello")
来源：http://fve.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://evm.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://frh.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://stn.jinyuanbaomall.cn

"值: $b"
来源：http://ulx.zhengqikj.top

[T04] Kotlin：空安全
来源：http://hpi.cheryme.top

val n: String? = null;  n?.length
来源：http://yxp.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://ics.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ohv.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://tjs.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://lrw.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://enp.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://wdo.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://erd.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://sno.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://fxi.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://iwv.bbcook.cn

[T10] Kotlin：默认参数
来源：http://rcn.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xsc.hysaishi.cn

[T11] Kotlin：协程
来源：http://wvn.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://tks.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://cua.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://ylp.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://kia.havefunace.top

val m = mapOf("a" to 1)
来源：http://usf.nanxinkj.top

[T14] Kotlin：循环
来源：http://bhy.52xcode.cn

for (i in 1..10) println(i)
来源：http://isa.shuidangran.top

[T15] Kotlin：接口
来源：http://yju.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://dhg.snrcjt.cn

[T16] Swift：Hello World
来源：http://voy.aizwys.cn

print("Hello")
来源：http://pkw.tianlin.xyz

[T17] Swift：变量与常量
来源：http://stu.sysykeji.top

var a = 1;  let b = 2
来源：http://msq.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://zwr.sweek.top

"值: \(b)"
来源：http://jna.chenzaomai.com

[T19] Swift：可选绑定
来源：http://usi.hesvh.cn

if let n = opt { print(n) }
来源：http://ycn.c1oappe.top

[T20] Swift：数组操作
来源：http://vdr.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dxx.0kj1m.cn

[T21] Swift：遍历
来源：http://imi.yuanzhike.top

for x in a { print(x) }
来源：http://qwa.gogol.net.cn

[T22] Swift：字典
来源：http://cyy.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tjy.316326.xyz

[T23] Swift：函数
来源：http://jmv.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ara.0kj1m.cn

[T24] Swift：闭包
来源：http://wrk.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jwq.0kj1m.cn

[T25] Swift：结构体
来源：http://duh.jqgfzy.top

struct P { var x: Int }
来源：http://xva.guowangkeji.top

[T26] Swift：类与重写
来源：http://afu.0kj1m.cn

class A: Base { override func f() {} }
来源：http://vnc.xziqi.cn

[T27] Swift：错误处理
来源：http://xms.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://plz.hysaishi.cn

[T28] Swift：枚举
来源：http://kll.gogol.net.cn

enum Color { case red, green }
来源：http://mlu.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://shu.quarkkingdee.top

guard let x = opt else { return }
来源：http://gbl.9152youxi.cn

[T30] Swift：协议
来源：http://kad.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://ncn.ppjwa.cn

[T31] Lua：Hello World
来源：http://kvx.ydjk.org.cn

print("Hello")
来源：http://oah.hnxiangtu.top

[T32] Lua：局部变量
来源：http://mxj.316326.xyz

local a = 1
来源：http://dhr.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://ecy.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://apn.guannengcc.top

[T34] Lua：遍历表
来源：http://gqs.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hfb.ppjwa.cn

[T35] Lua：字典表
来源：http://zoz.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://nbi.pengpengdd.cyou

[T36] Lua：函数
来源：http://pnu.ivvv.top

function add(a, b) return a + b end
来源：http://fsv.wangdashe.top

[T37] Lua：字符串拼接
来源：http://vva.wangdashe.top

"a" .. "b"
来源：http://gwx.hesvh.cn

[T38] Lua：条件
来源：http://pue.yuxming.cn

if x > 0 then print("正") end
来源：http://mjh.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://wdl.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://rig.yanxiufei.cn

[T40] Lua：元表
来源：http://ozr.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://ejv.andypj.xyz

[T41] Perl：Hello World
来源：http://hxr.shuidangran.top

print "Hello\n";
来源：http://jhs.smart0.xyz

[T42] Perl：变量类型
来源：http://gur.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wwy.zhixingplan.top

[T43] Perl：字符串插值
来源：http://yyg.xziqi.cn

"值: $a"
来源：http://ibe.yongpay.top

[T44] Perl：条件
来源：http://tpl.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://hqt.zhixingplan.top

[T45] Perl：数组遍历
来源：http://kgr.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://mqt.xinyue.icu

[T46] Perl：哈希操作
来源：http://qxk.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://evn.meibo888.top

[T47] Perl：正则捕获
来源：http://wqv.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fvo.316326.xyz

[T48] Perl：正则替换
来源：http://ebx.gotoacloud.top

$s =~ s/old/new/g;
来源：http://dfo.xuetiantiany.cn

[T49] Perl：函数
来源：http://mxy.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bqi.ydzc1.top

[T50] Perl：逐行读文件
来源：http://rgp.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ijv.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://qsg.yueranfly.top

[T51] Scala：Hello World
来源：http://uwa.cqqwz.cn

println("Hello")
来源：http://nyu.xylfe.cn

[T52] Scala：变量
来源：http://hzq.aizwys.cn

val a = 1;  var b = 2
来源：http://grv.uphjek.com

[T53] Scala：字符串插值
来源：http://skw.meibo888.top

s"值: $b"
来源：http://gyp.sjlbkw.cn

[T54] Scala：集合映射
来源：http://syk.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://nta.sxryk.cn

[T55] Scala：集合过滤
来源：http://jlc.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://ofd.jinqigfzy.top

[T56] Scala：样例类
来源：http://gfj.guowangkeji.top

case class User(name: String, age: Int)
来源：http://thp.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://oyo.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bjr.xylfe.cn

[T58] Scala：函数定义
来源：http://snh.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://hna.hnqzz.top

[T59] Scala：循环
来源：http://udj.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://hup.gzhubu.top

[T60] Scala：折叠
来源：http://uvu.gotoacloud.top


<!-- 参考信息 -->