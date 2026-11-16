代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ofy.jinqigfzy.top

[R52] 统计行数
来源：http://ntm.fzhhl.top

wc -l a.txt
来源：http://zva.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://vhe.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qvv.yvedp.cn

[R54] 比较两个文件
来源：http://cuc.tian-w.cn

diff a.txt b.txt
来源：http://aur.nanxinkj.top

[R55] 压缩与解压
来源：http://eeo.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fzc.hnxiangtu.top

[R56] 远程拷贝
来源：http://owd.yueranfly.top

scp file user@host:/path/
来源：http://pip.yj202588.top

[R57] 远程执行命令
来源：http://agv.hywenlv.cn

ssh user@host 'uptime'
来源：http://heo.aibaodan.cn

[R58] 下载文件
来源：http://ipx.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fmz.jyoumei.cn

[R59] 发 POST JSON
来源：http://mot.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lzb.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://hgo.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ynj.nanxuanxn.top

[R61] 磁盘占用
来源：http://jyk.hnqzz.top

df -h;  du -sh *
来源：http://zyr.c1oappe.top

[R62] 找最占空间的文件
来源：http://dxn.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://wtp.jinqigfzy.top

[R63] 内存与进程
来源：http://psa.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://ele.havefunace.top

[R64] 结束进程
来源：http://hry.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://rop.yongpay.top

[R65] 查看端口占用
来源：http://moh.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ual.yanxiufei.cn

[R66] 定时任务
来源：http://zgo.xylfe.cn

crontab -e;  crontab -l
来源：http://max.andypj.xyz

[R67] 生成随机十六进制串
来源：http://vtk.nwbrower.top

openssl rand -hex 16
来源：http://rik.epnwcf.com

[R68] 计算文件校验值
来源：http://yrk.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uwn.xylfe.cn

[R69] 生成随机密码
来源：http://ahk.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://kem.jinqigufen.top

[R70] 时间戳与互转
来源：http://dzi.yvedp.cn

date +%s;  date -d @1700000000
来源：http://biw.zdqjudy.top

[R71] 日期格式化
来源：http://ihh.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nag.yonumen.top

[R72] 等待端口就绪
来源：http://avr.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ixg.hesvh.cn

[R73] 分割大日志
来源：http://qdb.quarkkingdee.top

split -l 1000 big.log part_
来源：http://blx.jiagoushi.top

[R74] 批量重命名
来源：http://ixo.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oxa.hfpthk.cn

[R75] 导出环境变量
来源：http://fqp.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://brw.zhengqikj.top

[R76] 使用临时文件
来源：http://xou.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zmk.jqgfzy.top

[R77] 读取用户输入
来源：http://ntn.xinyue.icu

read -rp "请输入: " ans
来源：http://mlk.zhoulong.xyz

[R78] 交互式菜单
来源：http://jyy.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tmb.zhongyouzk.top

[R79] 解析命令行选项
来源：http://eas.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://znj.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://gzz.jqgufenzy.top

time ./run.sh
来源：http://wwp.wangdashe.top

================================================================================
来源：http://alb.zhengqikj.top

S. C / C++ 专题
来源：http://kva.xinyue.icu

================================================================================
来源：http://wqv.snrcjt.cn

[S01] C：Hello World
来源：http://glg.hammf.cn

#include <stdio.h>
来源：http://erc.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wvw.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://gug.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://tty.yj202588.top

[S03] C：读入整数
来源：http://mqw.daxiang520.top

int x; scanf("%d", &x);
来源：http://fjk.yuanzhike.top

[S04] C：字符串复制
来源：http://hly.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lyk.yangfankeji.com

[S05] C：字符串长度
来源：http://shp.zhaomingkeji.xyz

strlen(s)
来源：http://uun.cucudq.cn

[S06] C：字符串比较
来源：http://ite.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://pjl.tarul.cn

[S07] C：数组遍历求和
来源：http://xlw.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nkf.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://frn.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bdz.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://atg.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://htf.yuxming.cn

[S10] C：指针与解引用
来源：http://zzs.sxryk.cn

int *p = &a;  *p = 5;
来源：http://pco.fktsv.cn

[S11] C：逐行读文件
来源：http://tie.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://czi.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ivo.bbcook.cn

fclose(f);
来源：http://wdv.vehdjk.com

[S12] C：写文件
来源：http://dmf.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yqa.ehwqpu.com

[S13] C：宏定义
来源：http://rtu.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fhy.andypj.xyz

[S14] C：枚举
来源：http://jic.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://dsv.gogol.net.cn

[S15] C：类型转换
来源：http://cmr.gotoacloud.top

(double) a / b
来源：http://ysc.shuidangran.top

[S16] C：位操作置位
来源：http://yup.yj20258.top

x |= (1 << 3);
来源：http://jmf.hnqzz.top

[S17] C：安全拼接字符串
来源：http://nci.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qvm.pengpengdd.cyou

[S18] C：命令行参数
来源：http://sjr.gotoacloud.top

int main(int argc, char **argv)
来源：http://lsg.c1oappe.top

[S19] C：快速排序
来源：http://vpm.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://vza.vehdjk.com

[S20] C：二分查找
来源：http://eqh.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://amk.gzhubu.top

[S21] C：字符类别判断
来源：http://bhj.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vkn.haohaochexian.top

[S22] C：字符串转数字
来源：http://kul.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bkb.hnxiangtu.top

[S23] C：随机数
来源：http://oyk.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tjg.sysykeji.top

[S24] C：获取本地时间
来源：http://pmq.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iqr.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://tez.pycfn.com

memcpy(dst, src, n);
来源：http://tee.tanke756.top

[S26] C：内存清零
来源：http://jfg.yj202588.top

memset(a, 0, sizeof a);
来源：http://dvf.jianghu66.top

[S27] C：定义常量
来源：http://mkg.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://vzs.hammf.cn

[S28] C：静态变量
来源：http://awh.epnwcf.com

static int counter = 0;
来源：http://bdb.hongshengwenyu.top

[S29] C：变参函数
来源：http://zwt.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hol.ppjwa.cn

[S30] C：头文件保护
来源：http://pue.gzhubu.top

#ifndef X_H
来源：http://hhr.hysaishi.cn

#define X_H
来源：http://zxd.shuidangran.top

#endif
来源：http://kza.jiagoushi.top

[S31] C++：Hello World
来源：http://tow.yanxiufei.cn

#include <iostream>
来源：http://igp.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://yzw.jianghu66.top

[S32] C++：字符串
来源：http://nlq.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://aah.sxryk.cn

[S33] C++：vector 增删
来源：http://mrq.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsf.yongpay.top

[S34] C++：遍历 vector
来源：http://lir.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://lla.zhongyouzk.top

[S35] C++：map
来源：http://rim.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jdc.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://pso.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fdb.nanxuanxn.top

[S37] C++：set
来源：http://yhg.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sip.bjfxy.top

[S38] C++：排序
来源：http://tdw.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://ntr.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://qnh.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ixo.yj20258888.top

[S40] C++：查找元素
来源：http://ugh.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iww.cdnleiting.top

[S41] C++：类与构造函数
来源：http://lkz.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nou.epnwcf.com

[S42] C++：继承与虚函数
来源：http://jan.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://zvx.yvedp.cn

[S43] C++：智能指针
来源：http://bxa.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://lmi.cucudq.cn

[S44] C++：引用传参
来源：http://gpw.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://oak.52xcode.cn

[S45] C++：lambda
来源：http://sle.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://rhm.yfazqb.com

[S46] C++：函数模板
来源：http://bte.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ulx.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://yop.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kkk.hammf.cn

[S48] C++：逐行读文件
来源：http://xtb.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ufc.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://yod.ydzc1.top

[S49] C++：写文件
来源：http://rjp.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lqd.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://xiq.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://inc.zhixingplan.top

[S51] C++：显式类型转换
来源：http://zfs.zhijiandao.cn

static_cast<double>(a) / b
来源：http://aol.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://jsi.meibo888.top

int size() const noexcept { return n_; }
来源：http://wes.fzhhl.top

[S53] C++：移动语义
来源：http://vsp.yj202588.top

std::vector<int> w = std::move(v);
来源：http://kuc.hnqzz.top

[S54] C++：异常处理
来源：http://zwq.vehdjk.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dou.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://yfy.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vxm.chenzaomai.com

[S56] C++：optional
来源：http://rze.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xfa.fktsv.cn

[S57] C++：编译期常量
来源：http://jko.wangshuangyany.cn

constexpr int N = 10;
来源：http://fvd.vqdsnc.cn

[S58] C++：命名空间
来源：http://sha.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://krp.guannengcc.top

[S59] C++：静态断言
来源：http://tcr.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://brq.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://xgx.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rym.jqgfzy.top

================================================================================
来源：http://dmh.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lte.nanxinkj.top

================================================================================
来源：http://iyw.hcnkem.com

[T01] Kotlin：Hello World
来源：http://jgz.hcnkem.com

println("Hello")
来源：http://tbj.redwolf501.top

[T02] Kotlin：变量
来源：http://dvq.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tdm.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://dkn.gogol.net.cn

"值: $b"
来源：http://gue.guannengcc.top

[T04] Kotlin：空安全
来源：http://eig.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://djz.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://ozq.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wcl.vehdjk.com

[T06] Kotlin：集合映射
来源：http://vry.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nat.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://sxe.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://spw.0kj1m.cn

[T08] Kotlin：数据类
来源：http://frv.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://xpj.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://qlv.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://vpt.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://svm.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://acw.jiagoushi.top

[T11] Kotlin：协程
来源：http://zgk.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rzi.cucudq.cn

[T12] Kotlin：解构声明
来源：http://psn.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://nzu.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://czy.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://hmw.ehwqpu.com

[T14] Kotlin：循环
来源：http://ade.xinyue.icu

for (i in 1..10) println(i)
来源：http://wsq.ydzc1.top

[T15] Kotlin：接口
来源：http://toh.yj20258.top

interface Shape { fun area(): Double }
来源：http://bqb.yanxiufei.cn

[T16] Swift：Hello World
来源：http://cym.tian-w.cn

print("Hello")
来源：http://hmb.cucudq.cn

[T17] Swift：变量与常量
来源：http://jqh.xylfe.cn

var a = 1;  let b = 2
来源：http://zey.fehbvm.com

[T18] Swift：字符串插值
来源：http://mkz.zhaomingkeji.xyz

"值: \(b)"
来源：http://rxd.dianchejie.cn

[T19] Swift：可选绑定
来源：http://xkq.chenzaomai.com

if let n = opt { print(n) }
来源：http://sdc.yuxming.cn

[T20] Swift：数组操作
来源：http://lql.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bsx.daria6918.cn

[T21] Swift：遍历
来源：http://ztp.52xcode.cn

for x in a { print(x) }
来源：http://jqd.uphjek.com

[T22] Swift：字典
来源：http://ejc.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://sul.yuanzhike.top

[T23] Swift：函数
来源：http://upk.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://smp.yvedp.cn

[T24] Swift：闭包
来源：http://kzm.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://enx.yangfankeji.com

[T25] Swift：结构体
来源：http://wkg.hnqzz.top

struct P { var x: Int }
来源：http://awv.ydjk.org.cn

[T26] Swift：类与重写
来源：http://itc.guannengcc.top

class A: Base { override func f() {} }
来源：http://dst.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://otp.xylfe.cn

do { try f() } catch { print(error) }
来源：http://fck.daxiang520.top

[T28] Swift：枚举
来源：http://qyq.birdmap.top

enum Color { case red, green }
来源：http://jwk.meibo888.top

[T29] Swift：guard 提前返回
来源：http://qds.hysaishi.cn

guard let x = opt else { return }
来源：http://tyo.nwbrower.top

[T30] Swift：协议
来源：http://fvn.sweek.top

protocol Shape { func area() -> Double }
来源：http://bdm.ivvv.top

[T31] Lua：Hello World
来源：http://kvm.sjlbkw.cn

print("Hello")
来源：http://ytc.epnwcf.com

[T32] Lua：局部变量
来源：http://qcx.jinyuanbaomall.cn

local a = 1
来源：http://erd.nanxinkj.top

[T33] Lua：表（数组）
来源：http://fvc.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jhy.zdbjq.cn

[T34] Lua：遍历表
来源：http://ljt.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://bev.jqgfzy.top

[T35] Lua：字典表
来源：http://rsk.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://iye.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://khb.zycfv.cn

function add(a, b) return a + b end
来源：http://fsn.yuxming.cn

[T37] Lua：字符串拼接
来源：http://rdv.fengsongda.top

"a" .. "b"
来源：http://wfm.ctjpmb.com

[T38] Lua：条件
来源：http://lps.fehbvm.com

if x > 0 then print("正") end
来源：http://mqg.yueranfly.top

[T39] Lua：模式匹配
来源：http://mnn.svipenyu.cn

string.find(s, "%d+")
来源：http://tpq.tianlin.xyz

[T40] Lua：元表
来源：http://imz.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://esi.snrcjt.cn

[T41] Perl：Hello World
来源：http://oev.sweek.top

print "Hello\n";
来源：http://jdx.chenlongwang.top

[T42] Perl：变量类型
来源：http://uzo.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nsv.yuxming.cn

[T43] Perl：字符串插值
来源：http://zhz.jqgufenzy.top

"值: $a"
来源：http://kjy.fanxiaobao.xyz

[T44] Perl：条件
来源：http://miy.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://snd.yvedp.cn

[T45] Perl：数组遍历
来源：http://yhg.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://rbg.aibaodan.cn

[T46] Perl：哈希操作
来源：http://uga.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rqc.hfpthk.cn

[T47] Perl：正则捕获
来源：http://vyu.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rvl.hfpthk.cn

[T48] Perl：正则替换
来源：http://nyj.cashguo.top

$s =~ s/old/new/g;
来源：http://uni.aibaodan.cn

[T49] Perl：函数
来源：http://uyd.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dhw.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://wko.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gen.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://jom.ivvv.top

[T51] Scala：Hello World
来源：http://nyc.jinyuanbaomall.cn

println("Hello")
来源：http://ynh.iojbl.cn

[T52] Scala：变量
来源：http://yyw.epnwcf.com

val a = 1;  var b = 2
来源：http://ywy.jyoumei.cn

[T53] Scala：字符串插值
来源：http://ody.yanxiufei.cn

s"值: $b"
来源：http://lrh.smart0.xyz

[T54] Scala：集合映射
来源：http://qot.nanxuanxn.top


<!-- 参考信息 -->