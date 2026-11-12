代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jva.chenlongwang.top

[R54] 比较两个文件
来源：http://loi.aizwys.cn

diff a.txt b.txt
来源：http://sjl.0kj1m.cn

[R55] 压缩与解压
来源：http://zyo.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://liw.yfazqb.com

[R56] 远程拷贝
来源：http://jdg.yj20258.top

scp file user@host:/path/
来源：http://xrm.quarkkingdee.top

[R57] 远程执行命令
来源：http://pnt.hesvh.cn

ssh user@host 'uptime'
来源：http://wie.gotoacloud.top

[R58] 下载文件
来源：http://iwr.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fds.jianghu66.top

[R59] 发 POST JSON
来源：http://bep.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eiq.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://olw.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pks.chenlongwang.top

[R61] 磁盘占用
来源：http://vax.ydzc1.top

df -h;  du -sh *
来源：http://dag.uphjek.com

[R62] 找最占空间的文件
来源：http://gcd.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://bbo.zycfv.cn

[R63] 内存与进程
来源：http://lye.havefunace.top

free -h;  ps aux | grep nginx
来源：http://bej.gaohongyu789.top

[R64] 结束进程
来源：http://dsq.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://evs.sufxvd.cn

[R65] 查看端口占用
来源：http://blq.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lrk.ydzc1.top

[R66] 定时任务
来源：http://poz.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://fhw.havefunace.top

[R67] 生成随机十六进制串
来源：http://rsy.ydjk.org.cn

openssl rand -hex 16
来源：http://iew.sweek.top

[R68] 计算文件校验值
来源：http://dmc.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://tdd.uphjek.com

[R69] 生成随机密码
来源：http://adk.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://xat.zdqjudy.top

[R70] 时间戳与互转
来源：http://jmt.316326.xyz

date +%s;  date -d @1700000000
来源：http://ktf.aizwys.cn

[R71] 日期格式化
来源：http://qus.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://tvu.sweek.top

[R72] 等待端口就绪
来源：http://yog.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qxz.vehdjk.com

[R73] 分割大日志
来源：http://dkn.uphjek.com

split -l 1000 big.log part_
来源：http://pkl.tian-w.cn

[R74] 批量重命名
来源：http://hlo.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wij.wangdashe.top

[R75] 导出环境变量
来源：http://ybn.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://tgj.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://axk.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kci.zhixingplan.top

[R77] 读取用户输入
来源：http://tiz.yuxming.cn

read -rp "请输入: " ans
来源：http://ycz.hfpthk.cn

[R78] 交互式菜单
来源：http://dlq.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wqh.jlsjyb.cn

[R79] 解析命令行选项
来源：http://slq.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ekl.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://ujl.316326.xyz

time ./run.sh
来源：http://egv.zdqjudy.top

================================================================================
来源：http://eko.yongpay.top

S. C / C++ 专题
来源：http://gnl.jyoumei.cn

================================================================================
来源：http://uzs.chenlongwang.top

[S01] C：Hello World
来源：http://ndz.fehbvm.com

#include <stdio.h>
来源：http://mtg.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ceh.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://ysg.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://jbl.aizwys.cn

[S03] C：读入整数
来源：http://hxq.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://ydg.haohaochexian.top

[S04] C：字符串复制
来源：http://cfw.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pki.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://pku.pengpengdd.cyou

strlen(s)
来源：http://yhp.aibaodan.cn

[S06] C：字符串比较
来源：http://pba.yangfankeji.com

strcmp(a, b) == 0
来源：http://iid.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://aih.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sss.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://bwr.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xex.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://esb.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qwz.gaohongyu789.top

[S10] C：指针与解引用
来源：http://usr.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://xlx.ybcxt.top

[S11] C：逐行读文件
来源：http://cle.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://yst.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovb.nwbrower.top

fclose(f);
来源：http://gji.vqdsnc.cn

[S12] C：写文件
来源：http://kfg.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dsz.sjlbkw.cn

[S13] C：宏定义
来源：http://cnv.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xsd.smart0.xyz

[S14] C：枚举
来源：http://fur.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://icw.ppjwa.cn

[S15] C：类型转换
来源：http://zca.zhongyouzk.top

(double) a / b
来源：http://cvr.yuanzhike.top

[S16] C：位操作置位
来源：http://yii.cashguo.top

x |= (1 << 3);
来源：http://jdu.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://dix.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eky.fzhhl.top

[S18] C：命令行参数
来源：http://rwo.sjlbkw.cn

int main(int argc, char **argv)
来源：http://bbd.dashuyun.cn

[S19] C：快速排序
来源：http://xlz.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nfh.haohaochexian.top

[S20] C：二分查找
来源：http://yek.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aij.jqgufenzy.top

[S21] C：字符类别判断
来源：http://eqx.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://agz.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://srh.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yam.yuanzhike.top

[S23] C：随机数
来源：http://cbd.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zsh.zycfv.cn

[S24] C：获取本地时间
来源：http://zew.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fgr.hammf.cn

[S25] C：内存拷贝
来源：http://mse.zdbjq.cn

memcpy(dst, src, n);
来源：http://kfu.ivvv.top

[S26] C：内存清零
来源：http://uba.xuanzx.com

memset(a, 0, sizeof a);
来源：http://rrb.aibaodan.cn

[S27] C：定义常量
来源：http://jvn.jinqigufen.top

const double PI = 3.14159;
来源：http://ehe.tian-w.cn

[S28] C：静态变量
来源：http://vjb.gzhubu.top

static int counter = 0;
来源：http://ctx.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://yws.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvs.bbcook.cn

[S30] C：头文件保护
来源：http://kjn.sxryk.cn

#ifndef X_H
来源：http://fjy.andypj.xyz

#define X_H
来源：http://vhc.aibaodan.cn

#endif
来源：http://vez.bjfxy.top

[S31] C++：Hello World
来源：http://pbx.gogol.net.cn

#include <iostream>
来源：http://nde.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://pqu.sweek.top

[S32] C++：字符串
来源：http://yxg.cashguo.top

std::string s = "hi";  s += "!";
来源：http://bvl.cheryme.top

[S33] C++：vector 增删
来源：http://huv.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aln.yuxming.cn

[S34] C++：遍历 vector
来源：http://ven.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://eij.jinghuilouyu.cn

[S35] C++：map
来源：http://xlt.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kti.0kj1m.cn

[S36] C++：unordered_map
来源：http://vwk.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mjh.dashuyun.cn

[S37] C++：set
来源：http://hhl.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojz.cheryme.top

[S38] C++：排序
来源：http://oqe.yonumen.top

std::sort(v.begin(), v.end());
来源：http://yfl.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://gzv.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lqc.daxiang520.top

[S40] C++：查找元素
来源：http://cvz.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glf.bjfxy.top

[S41] C++：类与构造函数
来源：http://avz.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://puv.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://ggb.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://xpv.vehdjk.com

[S43] C++：智能指针
来源：http://obd.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://sjh.yuxming.cn

[S44] C++：引用传参
来源：http://vza.pycfn.com

void inc(int &x) { ++x; }
来源：http://ssm.meibo888.top

[S45] C++：lambda
来源：http://hcm.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jqe.tianlin.xyz

[S46] C++：函数模板
来源：http://ftc.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xcx.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://cih.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wgg.yueranfly.top

[S48] C++：逐行读文件
来源：http://edh.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://sjm.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://azy.jqgfzy.top

[S49] C++：写文件
来源：http://bkv.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://swd.cdnleiting.top

[S50] C++：格式化数字
来源：http://rwd.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mts.yvedp.cn

[S51] C++：显式类型转换
来源：http://hok.tian-w.cn

static_cast<double>(a) / b
来源：http://oie.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://pki.316326.xyz

int size() const noexcept { return n_; }
来源：http://klh.cheryme.top

[S53] C++：移动语义
来源：http://fya.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://haq.cqqwz.cn

[S54] C++：异常处理
来源：http://zbn.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kiq.pycfn.com

[S55] C++：结构化绑定
来源：http://kjj.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qhs.yj20258888.top

[S56] C++：optional
来源：http://nwk.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rij.snrcjt.cn

[S57] C++：编译期常量
来源：http://oei.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://crm.jlsjyb.cn

[S58] C++：命名空间
来源：http://epv.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://dpg.xuanzx.com

[S59] C++：静态断言
来源：http://qeh.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://odp.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://vin.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://duo.vehdjk.com

================================================================================
来源：http://pun.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kpa.tanke756.top

================================================================================
来源：http://ffs.cashguo.top

[T01] Kotlin：Hello World
来源：http://ssv.ppjwa.cn

println("Hello")
来源：http://khb.hnxiangtu.top

[T02] Kotlin：变量
来源：http://xvh.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cgm.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://pko.aizwys.cn

"值: $b"
来源：http://xta.fehbvm.com

[T04] Kotlin：空安全
来源：http://gzk.zdqjudy.top

val n: String? = null;  n?.length
来源：http://krp.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://jhx.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://afi.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://yns.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gsv.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://beg.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uxo.fengsongda.top

[T08] Kotlin：数据类
来源：http://ljj.yj202588.top

data class User(val name: String, val age: Int)
来源：http://bsb.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://pha.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://eaz.hesvh.cn

[T10] Kotlin：默认参数
来源：http://kfl.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vww.redwolf501.top

[T11] Kotlin：协程
来源：http://gtw.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://chm.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://ysf.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://xsf.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://rbb.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://czq.yangfankeji.com

[T14] Kotlin：循环
来源：http://ens.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://yyb.zdqjudy.top

[T15] Kotlin：接口
来源：http://yqr.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://tqv.hnqzz.top

[T16] Swift：Hello World
来源：http://gct.dashuyun.cn

print("Hello")
来源：http://vzv.dashuyun.cn

[T17] Swift：变量与常量
来源：http://egu.hnxiangtu.top

var a = 1;  let b = 2
来源：http://oio.aibaodan.cn

[T18] Swift：字符串插值
来源：http://urv.hnqzz.top

"值: \(b)"
来源：http://uez.hfpthk.cn

[T19] Swift：可选绑定
来源：http://iok.meibo888.top

if let n = opt { print(n) }
来源：http://atr.jqgufenzy.top

[T20] Swift：数组操作
来源：http://wdx.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bej.wangdashe.top

[T21] Swift：遍历
来源：http://jdb.andypj.xyz

for x in a { print(x) }
来源：http://gpw.52xcode.cn

[T22] Swift：字典
来源：http://tsg.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://klx.gotoacloud.top

[T23] Swift：函数
来源：http://slr.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://odj.cashguo.top

[T24] Swift：闭包
来源：http://dbr.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://szy.hcnkem.com

[T25] Swift：结构体
来源：http://flc.sweek.top

struct P { var x: Int }
来源：http://rke.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://whi.gogol.net.cn

class A: Base { override func f() {} }
来源：http://exe.xuanzx.com

[T27] Swift：错误处理
来源：http://mao.yj202588.top

do { try f() } catch { print(error) }
来源：http://rdn.0kj1m.cn

[T28] Swift：枚举
来源：http://lhp.uphjek.com

enum Color { case red, green }
来源：http://pft.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://xug.fktsv.cn

guard let x = opt else { return }
来源：http://qwy.chenjidiqi.icu

[T30] Swift：协议
来源：http://mxt.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://jfp.fzhhl.top

[T31] Lua：Hello World
来源：http://nsv.yuxming.cn

print("Hello")
来源：http://dwz.yj20258.top

[T32] Lua：局部变量
来源：http://zzh.jinqigfzy.top

local a = 1
来源：http://qcf.uphjek.com

[T33] Lua：表（数组）
来源：http://khl.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uex.jqgfzy.top

[T34] Lua：遍历表
来源：http://esh.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ayf.jqgfzy.top

[T35] Lua：字典表
来源：http://qjz.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://rhz.hammf.cn

[T36] Lua：函数
来源：http://vzw.dashuyun.cn

function add(a, b) return a + b end
来源：http://emf.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://afm.jqgfzy.top

"a" .. "b"
来源：http://tsf.quarkkingdee.top

[T38] Lua：条件
来源：http://uuo.jqgufenzy.top

if x > 0 then print("正") end
来源：http://dhv.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://dth.pycfn.com

string.find(s, "%d+")
来源：http://mem.ybcxt.top

[T40] Lua：元表
来源：http://ssp.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://bdk.yj202588.top

[T41] Perl：Hello World
来源：http://nru.ybcxt.top

print "Hello\n";
来源：http://tyt.sjlbkw.cn

[T42] Perl：变量类型
来源：http://sgg.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vwc.tarul.cn

[T43] Perl：字符串插值
来源：http://tdl.yangfankeji.com

"值: $a"
来源：http://ecg.jianghu66.top

[T44] Perl：条件
来源：http://gee.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://azw.yj202588.top

[T45] Perl：数组遍历
来源：http://phi.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://fgn.dianchejie.cn

[T46] Perl：哈希操作
来源：http://lto.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vxy.vehdjk.com

[T47] Perl：正则捕获
来源：http://eyq.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://bkc.epnwcf.com

[T48] Perl：正则替换
来源：http://qno.sxryk.cn

$s =~ s/old/new/g;
来源：http://qvk.chenlongwang.top

[T49] Perl：函数
来源：http://lho.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://amg.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://cgy.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://oyv.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://abu.ydzc1.top

[T51] Scala：Hello World
来源：http://ysv.cheryme.top

println("Hello")
来源：http://zjg.dashuyun.cn

[T52] Scala：变量
来源：http://sor.shuidangran.top

val a = 1;  var b = 2
来源：http://gii.hesvh.cn

[T53] Scala：字符串插值
来源：http://ddq.xuetiantiany.cn

s"值: $b"
来源：http://ayp.316326.xyz

[T54] Scala：集合映射
来源：http://ylz.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://oso.gzhubu.top

[T55] Scala：集合过滤
来源：http://krs.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://dpz.yfazqb.com

[T56] Scala：样例类
来源：http://aot.aibaodan.cn


<!-- 参考信息 -->