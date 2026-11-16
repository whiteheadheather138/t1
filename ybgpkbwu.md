代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ajp.ehwqpu.com

[R52] 统计行数
来源：http://idw.dianchejie.cn

wc -l a.txt
来源：http://yaz.316326.xyz

[R53] 查看文件头与实时尾
来源：http://qnz.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qwz.iojbl.cn

[R54] 比较两个文件
来源：http://nqs.birdmap.top

diff a.txt b.txt
来源：http://bfz.sufxvd.cn

[R55] 压缩与解压
来源：http://pyh.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aty.yj202588.top

[R56] 远程拷贝
来源：http://cyr.yuanzhike.top

scp file user@host:/path/
来源：http://afx.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://jqq.daxiang520.top

ssh user@host 'uptime'
来源：http://dxl.aibaodan.cn

[R58] 下载文件
来源：http://qmk.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vtk.zhixingplan.top

[R59] 发 POST JSON
来源：http://unt.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ysn.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://pfs.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rqh.hnqzz.top

[R61] 磁盘占用
来源：http://amr.yangfankeji.com

df -h;  du -sh *
来源：http://hap.yangfankeji.com

[R62] 找最占空间的文件
来源：http://wve.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://sqg.wangshuangyany.cn

[R63] 内存与进程
来源：http://fcg.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://qev.daria6918.cn

[R64] 结束进程
来源：http://mpz.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://mdh.shzxlz.cn

[R65] 查看端口占用
来源：http://taj.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://msk.guannengcc.top

[R66] 定时任务
来源：http://wqs.hnqzz.top

crontab -e;  crontab -l
来源：http://rzc.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://jsv.chenzaomai.com

openssl rand -hex 16
来源：http://onx.yfazqb.com

[R68] 计算文件校验值
来源：http://oqc.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kop.wangshuangyany.cn

[R69] 生成随机密码
来源：http://xly.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://kar.yj20258.top

[R70] 时间戳与互转
来源：http://iru.xinyue.icu

date +%s;  date -d @1700000000
来源：http://nmy.hnqzz.top

[R71] 日期格式化
来源：http://qjl.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kmn.hesvh.cn

[R72] 等待端口就绪
来源：http://lwh.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ktz.ydjk.org.cn

[R73] 分割大日志
来源：http://fbo.hcnkem.com

split -l 1000 big.log part_
来源：http://icz.yanxiufei.cn

[R74] 批量重命名
来源：http://fmb.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kuy.zycfv.cn

[R75] 导出环境变量
来源：http://gca.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://bep.nanxuanxn.top

[R76] 使用临时文件
来源：http://tls.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fny.andypj.xyz

[R77] 读取用户输入
来源：http://rtr.ivvv.top

read -rp "请输入: " ans
来源：http://gxi.snrcjt.cn

[R78] 交互式菜单
来源：http://qjn.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wmq.cashguo.top

[R79] 解析命令行选项
来源：http://cvy.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jjl.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://hrg.hcnkem.com

time ./run.sh
来源：http://azq.aibaodan.cn

================================================================================
来源：http://klz.dianchejie.cn

S. C / C++ 专题
来源：http://ouj.hnqzz.top

================================================================================
来源：http://xzz.xuetiantiany.cn

[S01] C：Hello World
来源：http://ybz.ppjwa.cn

#include <stdio.h>
来源：http://yux.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ofx.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://ayf.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://ewg.feifeiyinyue.top

[S03] C：读入整数
来源：http://omu.nanxinkj.top

int x; scanf("%d", &x);
来源：http://uae.yonumen.top

[S04] C：字符串复制
来源：http://dac.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nmu.gotoacloud.top

[S05] C：字符串长度
来源：http://axr.svipenyu.cn

strlen(s)
来源：http://rbd.zycfv.cn

[S06] C：字符串比较
来源：http://eyq.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://iam.0kj1m.cn

[S07] C：数组遍历求和
来源：http://cgx.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zjz.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://ile.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uim.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://yih.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oip.andypj.xyz

[S10] C：指针与解引用
来源：http://aig.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://ebp.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://wey.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://dvu.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgf.nanxuanxn.top

fclose(f);
来源：http://glg.yfazqb.com

[S12] C：写文件
来源：http://cbg.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://svq.haohaochexian.top

[S13] C：宏定义
来源：http://qwi.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dhu.cucudq.cn

[S14] C：枚举
来源：http://rtb.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://uaf.xinyue.icu

[S15] C：类型转换
来源：http://oss.hnxiangtu.top

(double) a / b
来源：http://ien.xylfe.cn

[S16] C：位操作置位
来源：http://cax.9152youxi.cn

x |= (1 << 3);
来源：http://xwc.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://kcu.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://unz.ppjwa.cn

[S18] C：命令行参数
来源：http://kcs.birdmap.top

int main(int argc, char **argv)
来源：http://mur.cucudq.cn

[S19] C：快速排序
来源：http://rvi.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://atd.fengsongda.top

[S20] C：二分查找
来源：http://vnv.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lfb.daria6918.cn

[S21] C：字符类别判断
来源：http://wpr.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sll.yuanzhike.top

[S22] C：字符串转数字
来源：http://zpd.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://alt.guowangkeji.top

[S23] C：随机数
来源：http://kwm.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nko.guowangkeji.top

[S24] C：获取本地时间
来源：http://xbz.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ydw.fehbvm.com

[S25] C：内存拷贝
来源：http://ojv.316326.xyz

memcpy(dst, src, n);
来源：http://qmt.ehwqpu.com

[S26] C：内存清零
来源：http://emd.sxryk.cn

memset(a, 0, sizeof a);
来源：http://lum.hesvh.cn

[S27] C：定义常量
来源：http://oou.jqgufenzy.top

const double PI = 3.14159;
来源：http://eoz.gzhubu.top

[S28] C：静态变量
来源：http://grj.zdbjq.cn

static int counter = 0;
来源：http://gyk.snrcjt.cn

[S29] C：变参函数
来源：http://uuk.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ozm.fehbvm.com

[S30] C：头文件保护
来源：http://zcz.zhixingplan.top

#ifndef X_H
来源：http://tvk.yj20258.top

#define X_H
来源：http://koy.jyoumei.cn

#endif
来源：http://bbd.cheryme.top

[S31] C++：Hello World
来源：http://qdy.0kj1m.cn

#include <iostream>
来源：http://esr.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://dti.aizwys.cn

[S32] C++：字符串
来源：http://eao.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://xnz.gogol.net.cn

[S33] C++：vector 增删
来源：http://kvz.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnn.chenzaomai.com

[S34] C++：遍历 vector
来源：http://bbs.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://eii.yonumen.top

[S35] C++：map
来源：http://ruy.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dmf.andypj.xyz

[S36] C++：unordered_map
来源：http://upm.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://smt.yvedp.cn

[S37] C++：set
来源：http://xyj.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cmf.yuanzhike.top

[S38] C++：排序
来源：http://tyo.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://dwz.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://jen.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ucj.cqqwz.cn

[S40] C++：查找元素
来源：http://pkz.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ial.yonumen.top

[S41] C++：类与构造函数
来源：http://dpr.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ixd.fehbvm.com

[S42] C++：继承与虚函数
来源：http://xhq.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://hfx.cashguo.top

[S43] C++：智能指针
来源：http://yeh.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://ldu.tianlin.xyz

[S44] C++：引用传参
来源：http://dan.yj20258.top

void inc(int &x) { ++x; }
来源：http://unj.tanke756.top

[S45] C++：lambda
来源：http://taw.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vfb.xinyue.icu

[S46] C++：函数模板
来源：http://pum.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dzd.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://dzw.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qpb.pycfn.com

[S48] C++：逐行读文件
来源：http://enm.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jrg.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://qob.birdmap.top

[S49] C++：写文件
来源：http://eqs.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rcu.andypj.xyz

[S50] C++：格式化数字
来源：http://sly.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://agb.bjfxy.top

[S51] C++：显式类型转换
来源：http://zcb.jinqigfzy.top

static_cast<double>(a) / b
来源：http://wcy.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://chc.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://kwm.tian-w.cn

[S53] C++：移动语义
来源：http://wys.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://vtv.0kj1m.cn

[S54] C++：异常处理
来源：http://aer.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://okf.jianghu66.top

[S55] C++：结构化绑定
来源：http://xmx.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://blj.mhx1999.top

[S56] C++：optional
来源：http://uih.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wul.sysykeji.top

[S57] C++：编译期常量
来源：http://uei.shzxlz.cn

constexpr int N = 10;
来源：http://hsi.c1oappe.top

[S58] C++：命名空间
来源：http://wlm.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://wbp.cqqwz.cn

[S59] C++：静态断言
来源：http://qoj.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mwv.yj20258.top

[S60] C++：遍历并删除元素
来源：http://rbh.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vgj.sjlbkw.cn

================================================================================
来源：http://qcc.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kbb.zhaomingkeji.xyz

================================================================================
来源：http://xxw.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://cxr.sxryk.cn

println("Hello")
来源：http://pcg.jyoumei.cn

[T02] Kotlin：变量
来源：http://alq.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nlu.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://asu.bbcook.cn

"值: $b"
来源：http://umi.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://lwb.aizwys.cn

val n: String? = null;  n?.length
来源：http://qja.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://dch.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gzb.jianghu66.top

[T06] Kotlin：集合映射
来源：http://lnd.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pwb.yonumen.top

[T07] Kotlin：集合过滤
来源：http://boo.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bll.hcnkem.com

[T08] Kotlin：数据类
来源：http://wng.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://gvw.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://vyc.tanke756.top

fun String.exclaim() = this + "!"
来源：http://scc.yuxming.cn

[T10] Kotlin：默认参数
来源：http://qbg.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bdr.guowangkeji.top

[T11] Kotlin：协程
来源：http://tyx.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sso.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://wze.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://tsr.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://swt.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://nnh.havefunace.top

[T14] Kotlin：循环
来源：http://nlc.316326.xyz

for (i in 1..10) println(i)
来源：http://unq.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://fon.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://jof.52xcode.cn

[T16] Swift：Hello World
来源：http://che.sjlbkw.cn

print("Hello")
来源：http://grm.guowangkeji.top

[T17] Swift：变量与常量
来源：http://utx.daxiang520.top

var a = 1;  let b = 2
来源：http://iry.snrcjt.cn

[T18] Swift：字符串插值
来源：http://cgp.yvedp.cn

"值: \(b)"
来源：http://vxk.cucudq.cn

[T19] Swift：可选绑定
来源：http://ogs.dashuyun.cn

if let n = opt { print(n) }
来源：http://cqd.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://mof.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://cwb.epnwcf.com

[T21] Swift：遍历
来源：http://ivh.sufxvd.cn

for x in a { print(x) }
来源：http://yxw.svipenyu.cn

[T22] Swift：字典
来源：http://pcs.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://thi.mhx1999.top

[T23] Swift：函数
来源：http://fgt.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qun.jinqigufen.top

[T24] Swift：闭包
来源：http://oii.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://egb.zhixingplan.top

[T25] Swift：结构体
来源：http://qzt.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://mck.ppjwa.cn

[T26] Swift：类与重写
来源：http://ear.shzxlz.cn

class A: Base { override func f() {} }
来源：http://zal.yj20258.top

[T27] Swift：错误处理
来源：http://atr.yj20258888.top

do { try f() } catch { print(error) }
来源：http://gbq.zhijiandao.cn

[T28] Swift：枚举
来源：http://vqc.jyoumei.cn

enum Color { case red, green }
来源：http://jvd.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://shq.tarul.cn

guard let x = opt else { return }
来源：http://hch.chenzaomai.com

[T30] Swift：协议
来源：http://csl.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://eli.epnwcf.com

[T31] Lua：Hello World
来源：http://xap.yuanzhike.top

print("Hello")
来源：http://pev.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://oln.zhoulong.xyz

local a = 1
来源：http://tif.andypj.xyz

[T33] Lua：表（数组）
来源：http://rlj.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xxp.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://klu.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jej.yuxming.cn

[T35] Lua：字典表
来源：http://kjf.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://xwu.cqqwz.cn

[T36] Lua：函数
来源：http://tkg.andypj.xyz

function add(a, b) return a + b end
来源：http://rzn.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://vbi.pycfn.com

"a" .. "b"
来源：http://ryr.cheryme.top

[T38] Lua：条件
来源：http://pzh.mhx1999.top

if x > 0 then print("正") end
来源：http://cdt.dianchejie.cn

[T39] Lua：模式匹配
来源：http://rma.yj202588.top

string.find(s, "%d+")
来源：http://jez.zhengqikj.top

[T40] Lua：元表
来源：http://qsd.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://erz.hysaishi.cn

[T41] Perl：Hello World
来源：http://hlm.fzhhl.top

print "Hello\n";
来源：http://keb.sjlbkw.cn

[T42] Perl：变量类型
来源：http://etm.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nlf.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://lxk.ywan-chungtsiang.top

"值: $a"
来源：http://opz.fehbvm.com

[T44] Perl：条件
来源：http://bet.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://okh.cheryme.top

[T45] Perl：数组遍历
来源：http://tqf.pycfn.com

for my $x (@arr) { print $x; }
来源：http://xjj.jyoumei.cn

[T46] Perl：哈希操作
来源：http://zri.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hll.gogol.net.cn

[T47] Perl：正则捕获
来源：http://gwx.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://hnw.vehdjk.com

[T48] Perl：正则替换
来源：http://ojb.jiagoushi.top

$s =~ s/old/new/g;
来源：http://vpl.sufxvd.cn

[T49] Perl：函数
来源：http://qid.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xwk.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://iwy.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://njf.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://czf.nanxuanxn.top

[T51] Scala：Hello World
来源：http://dpu.tian-w.cn

println("Hello")
来源：http://gwj.ctjpmb.com

[T52] Scala：变量
来源：http://djp.uphjek.com

val a = 1;  var b = 2
来源：http://ryy.cheryme.top

[T53] Scala：字符串插值
来源：http://bxi.ywan-chungtsiang.top

s"值: $b"
来源：http://ciu.cqqwz.cn

[T54] Scala：集合映射
来源：http://jyy.aibaodan.cn


<!-- 参考信息 -->