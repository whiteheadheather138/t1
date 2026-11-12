代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zgx.zhiwuduotai.top

[R50] awk 求和
来源：http://dse.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://htm.9152youxi.cn

[R51] 排序去重取前几
来源：http://jzf.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://woi.xylfe.cn

[R52] 统计行数
来源：http://atd.yongpay.top

wc -l a.txt
来源：http://jfb.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://tjg.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jfr.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://zpv.chenlongwang.top

diff a.txt b.txt
来源：http://vwa.cqqwz.cn

[R55] 压缩与解压
来源：http://vuo.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://twn.hongshengwenyu.top

[R56] 远程拷贝
来源：http://zkb.chenlongwang.top

scp file user@host:/path/
来源：http://unp.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://lzg.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://lnx.haohaochexian.top

[R58] 下载文件
来源：http://yda.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://giu.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://uwt.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://acm.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://mir.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ens.mhx1999.top

[R61] 磁盘占用
来源：http://myj.svipenyu.cn

df -h;  du -sh *
来源：http://dhr.316326.xyz

[R62] 找最占空间的文件
来源：http://jrw.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://xky.quarkkingdee.top

[R63] 内存与进程
来源：http://gqf.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://ttj.yueranfly.top

[R64] 结束进程
来源：http://pua.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://etg.zycfv.cn

[R65] 查看端口占用
来源：http://lkq.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://npy.yvedp.cn

[R66] 定时任务
来源：http://rnf.jqgufenzy.top

crontab -e;  crontab -l
来源：http://dba.ybcxt.top

[R67] 生成随机十六进制串
来源：http://urk.daria6918.cn

openssl rand -hex 16
来源：http://vsj.hcnkem.com

[R68] 计算文件校验值
来源：http://ont.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rlm.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://otr.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://uin.svipenyu.cn

[R70] 时间戳与互转
来源：http://ltd.sxryk.cn

date +%s;  date -d @1700000000
来源：http://mwn.fktsv.cn

[R71] 日期格式化
来源：http://glm.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://dfq.snrcjt.cn

[R72] 等待端口就绪
来源：http://amf.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://eok.svipenyu.cn

[R73] 分割大日志
来源：http://xww.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://uqn.bjfxy.top

[R74] 批量重命名
来源：http://tvh.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ngf.xuetiantiany.cn

[R75] 导出环境变量
来源：http://mvt.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://ihe.xylfe.cn

[R76] 使用临时文件
来源：http://liz.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mbq.yongpay.top

[R77] 读取用户输入
来源：http://bvo.cdnleiting.top

read -rp "请输入: " ans
来源：http://apl.ivvv.top

[R78] 交互式菜单
来源：http://yzg.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ehi.52xcode.cn

[R79] 解析命令行选项
来源：http://irb.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vst.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://wve.zhoulong.xyz

time ./run.sh
来源：http://nqw.jyoumei.cn

================================================================================
来源：http://fsy.vehdjk.com

S. C / C++ 专题
来源：http://msq.cqqwz.cn

================================================================================
来源：http://fbh.ppjwa.cn

[S01] C：Hello World
来源：http://jox.cdnleiting.top

#include <stdio.h>
来源：http://xxo.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xob.ivvv.top

[S02] C：变量与格式化输出
来源：http://ezu.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://elc.yongpay.top

[S03] C：读入整数
来源：http://plp.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://jzx.guannengcc.top

[S04] C：字符串复制
来源：http://epc.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://lya.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://bif.tarul.cn

strlen(s)
来源：http://yxa.nanxinkj.top

[S06] C：字符串比较
来源：http://peb.zdqjudy.top

strcmp(a, b) == 0
来源：http://ydz.tanke756.top

[S07] C：数组遍历求和
来源：http://obr.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aef.cheryme.top

[S08] C：动态内存分配与释放
来源：http://rbi.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mlb.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://nsf.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ylf.yj202588.top

[S10] C：指针与解引用
来源：http://llw.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://jlp.gaohongyu789.top

[S11] C：逐行读文件
来源：http://rbw.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://adp.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ptl.nanxuanxn.top

fclose(f);
来源：http://yry.0kj1m.cn

[S12] C：写文件
来源：http://amq.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yjd.havefunace.top

[S13] C：宏定义
来源：http://rmz.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jeo.jinyuanbaomall.cn

[S14] C：枚举
来源：http://ynv.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://fez.smart0.xyz

[S15] C：类型转换
来源：http://wzq.fktsv.cn

(double) a / b
来源：http://zkp.xinyue.icu

[S16] C：位操作置位
来源：http://kfq.chenzaomai.com

x |= (1 << 3);
来源：http://daj.nwbrower.top

[S17] C：安全拼接字符串
来源：http://etf.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qty.sweek.top

[S18] C：命令行参数
来源：http://xcd.yuxming.cn

int main(int argc, char **argv)
来源：http://vsy.fktsv.cn

[S19] C：快速排序
来源：http://wte.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kng.fehbvm.com

[S20] C：二分查找
来源：http://amn.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tym.gotoacloud.top

[S21] C：字符类别判断
来源：http://ztg.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rdl.yonumen.top

[S22] C：字符串转数字
来源：http://rik.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://hri.fktsv.cn

[S23] C：随机数
来源：http://say.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qwe.jinqigfzy.top

[S24] C：获取本地时间
来源：http://zwm.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wvo.yuxming.cn

[S25] C：内存拷贝
来源：http://ntx.gaohongyu789.top

memcpy(dst, src, n);
来源：http://bts.hnxiangtu.top

[S26] C：内存清零
来源：http://nxf.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://mta.fzhhl.top

[S27] C：定义常量
来源：http://mvk.hysaishi.cn

const double PI = 3.14159;
来源：http://jwt.hfpthk.cn

[S28] C：静态变量
来源：http://krn.sysykeji.top

static int counter = 0;
来源：http://fnf.tanke756.top

[S29] C：变参函数
来源：http://qnx.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pei.ehwqpu.com

[S30] C：头文件保护
来源：http://rln.gotoacloud.top

#ifndef X_H
来源：http://smm.chenjidiqi.icu

#define X_H
来源：http://bzw.hysaishi.cn

#endif
来源：http://laf.fktsv.cn

[S31] C++：Hello World
来源：http://zga.shuidangran.top

#include <iostream>
来源：http://pko.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://vjk.birdmap.top

[S32] C++：字符串
来源：http://mwz.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://tva.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://skl.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xak.jinqigufen.top

[S34] C++：遍历 vector
来源：http://vpw.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vzb.snrcjt.cn

[S35] C++：map
来源：http://vkk.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dwe.hammf.cn

[S36] C++：unordered_map
来源：http://ncz.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mbp.zhaomingkeji.xyz

[S37] C++：set
来源：http://ihm.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dhs.zhixingplan.top

[S38] C++：排序
来源：http://rir.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://bbm.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://ahl.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rke.nwbrower.top

[S40] C++：查找元素
来源：http://bqs.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://haj.zhengqikj.top

[S41] C++：类与构造函数
来源：http://fpg.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kwi.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://qmg.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://baz.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://tca.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://kpb.cdnleiting.top

[S44] C++：引用传参
来源：http://npe.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://dyt.xuanzx.com

[S45] C++：lambda
来源：http://tlf.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gna.tarul.cn

[S46] C++：函数模板
来源：http://gwf.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whx.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://dtm.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yfl.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://lnb.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://idz.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://wiw.bjfxy.top

[S49] C++：写文件
来源：http://dvb.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jfa.guowangkeji.top

[S50] C++：格式化数字
来源：http://rtd.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hec.yj20258.top

[S51] C++：显式类型转换
来源：http://vqb.mhx1999.top

static_cast<double>(a) / b
来源：http://dkg.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://yeu.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://mub.zhengqikj.top

[S53] C++：移动语义
来源：http://sqn.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://ssl.zdqjudy.top

[S54] C++：异常处理
来源：http://jrn.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oqi.jyoumei.cn

[S55] C++：结构化绑定
来源：http://ufk.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://deu.iojbl.cn

[S56] C++：optional
来源：http://cit.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eqn.yvedp.cn

[S57] C++：编译期常量
来源：http://fvj.smart0.xyz

constexpr int N = 10;
来源：http://ykc.tanke756.top

[S58] C++：命名空间
来源：http://pra.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://yhj.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://tcd.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qdq.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://tsd.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oxm.xuanzx.com

================================================================================
来源：http://hml.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zki.hesvh.cn

================================================================================
来源：http://jhp.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://eot.zhongyouzk.top

println("Hello")
来源：http://ert.iojbl.cn

[T02] Kotlin：变量
来源：http://buk.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://thl.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://vzh.yongpay.top

"值: $b"
来源：http://osf.gotoacloud.top

[T04] Kotlin：空安全
来源：http://xnw.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://ngi.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://kxp.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://len.nwbrower.top

[T06] Kotlin：集合映射
来源：http://fns.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jer.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://sen.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ddg.fktsv.cn

[T08] Kotlin：数据类
来源：http://qpm.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://ohx.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://nbs.tarul.cn

fun String.exclaim() = this + "!"
来源：http://kcm.cashguo.top

[T10] Kotlin：默认参数
来源：http://irt.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qhy.havefunace.top

[T11] Kotlin：协程
来源：http://job.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zbr.yj20258888.top

[T12] Kotlin：解构声明
来源：http://nwe.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://dts.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://fxg.bjfxy.top

val m = mapOf("a" to 1)
来源：http://fao.yj202588.top

[T14] Kotlin：循环
来源：http://xwq.zycfv.cn

for (i in 1..10) println(i)
来源：http://zcq.xuanzx.com

[T15] Kotlin：接口
来源：http://bby.tian-w.cn

interface Shape { fun area(): Double }
来源：http://yfr.haohaochexian.top

[T16] Swift：Hello World
来源：http://cqa.zycfv.cn

print("Hello")
来源：http://xvv.dianchejie.cn

[T17] Swift：变量与常量
来源：http://knz.yfazqb.com

var a = 1;  let b = 2
来源：http://iah.gzhubu.top

[T18] Swift：字符串插值
来源：http://rtt.daxiang520.top

"值: \(b)"
来源：http://ivu.xuanzx.com

[T19] Swift：可选绑定
来源：http://ijd.shuidangran.top

if let n = opt { print(n) }
来源：http://jcm.ybcxt.top

[T20] Swift：数组操作
来源：http://zpd.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://mis.hcnkem.com

[T21] Swift：遍历
来源：http://uif.hfpthk.cn

for x in a { print(x) }
来源：http://cfc.daria6918.cn

[T22] Swift：字典
来源：http://wkh.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://clb.zhoulong.xyz

[T23] Swift：函数
来源：http://ynw.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cqk.zycfv.cn

[T24] Swift：闭包
来源：http://krs.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://yrn.cucudq.cn

[T25] Swift：结构体
来源：http://jsu.epnwcf.com

struct P { var x: Int }
来源：http://mzf.daria6918.cn

[T26] Swift：类与重写
来源：http://vwz.hnqzz.top

class A: Base { override func f() {} }
来源：http://zqd.tarul.cn

[T27] Swift：错误处理
来源：http://huk.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://foc.c1oappe.top

[T28] Swift：枚举
来源：http://kue.haohaochexian.top

enum Color { case red, green }
来源：http://lkk.havefunace.top

[T29] Swift：guard 提前返回
来源：http://tsc.tianlin.xyz

guard let x = opt else { return }
来源：http://cpl.yfazqb.com

[T30] Swift：协议
来源：http://ocj.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://krt.hywenlv.cn

[T31] Lua：Hello World
来源：http://nok.hywenlv.cn

print("Hello")
来源：http://kfr.yangfankeji.com

[T32] Lua：局部变量
来源：http://dqc.redwolf501.top

local a = 1
来源：http://jle.uphjek.com

[T33] Lua：表（数组）
来源：http://fxg.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bcq.vehdjk.com

[T34] Lua：遍历表
来源：http://ddk.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nbx.c1oappe.top

[T35] Lua：字典表
来源：http://eti.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://har.kuanghao11.cn

[T36] Lua：函数
来源：http://tkr.zdbjq.cn

function add(a, b) return a + b end
来源：http://zoy.xylfe.cn

[T37] Lua：字符串拼接
来源：http://lke.birdmap.top

"a" .. "b"
来源：http://ysc.hesvh.cn

[T38] Lua：条件
来源：http://lkn.shuidangran.top

if x > 0 then print("正") end
来源：http://gpy.aibaodan.cn

[T39] Lua：模式匹配
来源：http://msz.yuxming.cn

string.find(s, "%d+")
来源：http://qvn.xuanzx.com

[T40] Lua：元表
来源：http://pnr.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://snp.ppjwa.cn

[T41] Perl：Hello World
来源：http://lzb.haohaochexian.top

print "Hello\n";
来源：http://qdz.cashguo.top

[T42] Perl：变量类型
来源：http://liw.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://awa.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://nhv.cheryme.top

"值: $a"
来源：http://jlq.epnwcf.com

[T44] Perl：条件
来源：http://evr.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://gwn.uphjek.com

[T45] Perl：数组遍历
来源：http://fzk.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://dkr.smart0.xyz

[T46] Perl：哈希操作
来源：http://keq.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wsk.uphjek.com

[T47] Perl：正则捕获
来源：http://kgr.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yaz.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://mtj.gotoacloud.top

$s =~ s/old/new/g;
来源：http://kjh.jiagoushi.top

[T49] Perl：函数
来源：http://pqp.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aps.xylfe.cn

[T50] Perl：逐行读文件
来源：http://pcq.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dzj.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://qpj.yj202588.top

[T51] Scala：Hello World
来源：http://fna.gzhubu.top

println("Hello")
来源：http://zip.daria6918.cn

[T52] Scala：变量
来源：http://sbn.quarkkingdee.top


<!-- 参考信息 -->