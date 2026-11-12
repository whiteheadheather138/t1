代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qvj.cashguo.top

[R54] 比较两个文件
来源：http://oth.9152youxi.cn

diff a.txt b.txt
来源：http://iga.ydjk.org.cn

[R55] 压缩与解压
来源：http://krh.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vzd.316326.xyz

[R56] 远程拷贝
来源：http://aji.daxiang520.top

scp file user@host:/path/
来源：http://vip.gzhubu.top

[R57] 远程执行命令
来源：http://smc.bbcook.cn

ssh user@host 'uptime'
来源：http://afv.ehwqpu.com

[R58] 下载文件
来源：http://yfn.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyk.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://stu.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dcl.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://bxw.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://smc.daria6918.cn

[R61] 磁盘占用
来源：http://azb.fzhhl.top

df -h;  du -sh *
来源：http://ncx.shzxlz.cn

[R62] 找最占空间的文件
来源：http://vms.pycfn.com

du -ah . | sort -rh | head -10
来源：http://uqj.hysaishi.cn

[R63] 内存与进程
来源：http://ucg.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://rig.chenjidiqi.icu

[R64] 结束进程
来源：http://buw.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://dpr.birdmap.top

[R65] 查看端口占用
来源：http://qcn.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wtq.andypj.xyz

[R66] 定时任务
来源：http://ovl.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://axg.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://tww.cheryme.top

openssl rand -hex 16
来源：http://nig.kuanghao11.cn

[R68] 计算文件校验值
来源：http://amh.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://ush.chenlongwang.top

[R69] 生成随机密码
来源：http://ckm.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://fjj.pycfn.com

[R70] 时间戳与互转
来源：http://tbf.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://lcn.uphjek.com

[R71] 日期格式化
来源：http://gpc.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ejy.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://fpf.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nfz.nanxinkj.top

[R73] 分割大日志
来源：http://sml.zdqjudy.top

split -l 1000 big.log part_
来源：http://yap.aibaodan.cn

[R74] 批量重命名
来源：http://cee.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ryi.kuanghao11.cn

[R75] 导出环境变量
来源：http://llc.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://vof.mhx1999.top

[R76] 使用临时文件
来源：http://eod.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qlw.daxiang520.top

[R77] 读取用户输入
来源：http://cbr.yj20258.top

read -rp "请输入: " ans
来源：http://syg.meibo888.top

[R78] 交互式菜单
来源：http://eil.sufxvd.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lpa.chenlongwang.top

[R79] 解析命令行选项
来源：http://oyl.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kry.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://zar.chenzaomai.com

time ./run.sh
来源：http://zyp.cqqwz.cn

================================================================================
来源：http://txa.shangyingyoupin.top

S. C / C++ 专题
来源：http://tgt.jyoumei.cn

================================================================================
来源：http://pqm.hnxiangtu.top

[S01] C：Hello World
来源：http://avu.tarul.cn

#include <stdio.h>
来源：http://yne.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://any.bjfxy.top

[S02] C：变量与格式化输出
来源：http://saz.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://oqy.epnwcf.com

[S03] C：读入整数
来源：http://dqu.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://zus.zhoulong.xyz

[S04] C：字符串复制
来源：http://nxy.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://hgp.hongshengwenyu.top

[S05] C：字符串长度
来源：http://aop.zhongyouzk.top

strlen(s)
来源：http://hpa.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://gxc.quarkkingdee.top

strcmp(a, b) == 0
来源：http://mes.svipenyu.cn

[S07] C：数组遍历求和
来源：http://lin.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hpq.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://gsp.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vub.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://flg.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rpc.redwolf501.top

[S10] C：指针与解引用
来源：http://eop.birdmap.top

int *p = &a;  *p = 5;
来源：http://lqn.tian-w.cn

[S11] C：逐行读文件
来源：http://lem.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://akw.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://adm.vqdsnc.cn

fclose(f);
来源：http://wdi.gaohongyu789.top

[S12] C：写文件
来源：http://gku.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yhh.gaohongyu789.top

[S13] C：宏定义
来源：http://fuc.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ylb.vehdjk.com

[S14] C：枚举
来源：http://qtg.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://nqw.sweek.top

[S15] C：类型转换
来源：http://eka.jqgufenzy.top

(double) a / b
来源：http://rze.fktsv.cn

[S16] C：位操作置位
来源：http://gji.mhx1999.top

x |= (1 << 3);
来源：http://riz.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://htz.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yzl.ctjpmb.com

[S18] C：命令行参数
来源：http://dph.xuanzx.com

int main(int argc, char **argv)
来源：http://ccn.xziqi.cn

[S19] C：快速排序
来源：http://swm.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xys.aibaodan.cn

[S20] C：二分查找
来源：http://pwc.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zqr.iojbl.cn

[S21] C：字符类别判断
来源：http://zsn.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://paf.jqgfzy.top

[S22] C：字符串转数字
来源：http://wgn.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bix.cqqwz.cn

[S23] C：随机数
来源：http://rrf.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tln.andypj.xyz

[S24] C：获取本地时间
来源：http://qgn.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sxz.zhoulong.xyz

[S25] C：内存拷贝
来源：http://zjf.hfpthk.cn

memcpy(dst, src, n);
来源：http://cad.sjlbkw.cn

[S26] C：内存清零
来源：http://kjp.ybcxt.top

memset(a, 0, sizeof a);
来源：http://clf.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://mux.fktsv.cn

const double PI = 3.14159;
来源：http://bbe.chenlongwang.top

[S28] C：静态变量
来源：http://loa.yuanzhike.top

static int counter = 0;
来源：http://jtk.sweek.top

[S29] C：变参函数
来源：http://iyg.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://guc.wangdashe.top

[S30] C：头文件保护
来源：http://xli.yuanzhike.top

#ifndef X_H
来源：http://uio.fanxiaobao.xyz

#define X_H
来源：http://sew.52xcode.cn

#endif
来源：http://ttv.yj20258.top

[S31] C++：Hello World
来源：http://dft.yfazqb.com

#include <iostream>
来源：http://atg.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://dct.hnqzz.top

[S32] C++：字符串
来源：http://ztv.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://uub.gaohongyu789.top

[S33] C++：vector 增删
来源：http://qds.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://suy.daria6918.cn

[S34] C++：遍历 vector
来源：http://sxg.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://ruq.jlsjyb.cn

[S35] C++：map
来源：http://ifu.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ctz.birdmap.top

[S36] C++：unordered_map
来源：http://lfv.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://amu.tarul.cn

[S37] C++：set
来源：http://fyf.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wxa.shanyushiyangtech.top

[S38] C++：排序
来源：http://foi.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://tfr.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://zho.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qyq.jyoumei.cn

[S40] C++：查找元素
来源：http://rul.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgm.ydzc1.top

[S41] C++：类与构造函数
来源：http://vtd.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqp.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://fye.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://ilk.xuanzx.com

[S43] C++：智能指针
来源：http://zcp.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://ske.xuetiantiany.cn

[S44] C++：引用传参
来源：http://ogp.tian-w.cn

void inc(int &x) { ++x; }
来源：http://wow.chenzaomai.com

[S45] C++：lambda
来源：http://rou.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://bco.nwbrower.top

[S46] C++：函数模板
来源：http://gxo.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pnj.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://ydo.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mgf.hfpthk.cn

[S48] C++：逐行读文件
来源：http://eoh.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://xmp.yvedp.cn

while (std::getline(in, line)) { }
来源：http://ygt.yvedp.cn

[S49] C++：写文件
来源：http://ika.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cny.yangfankeji.com

[S50] C++：格式化数字
来源：http://iud.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rvs.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://muk.dashuyun.cn

static_cast<double>(a) / b
来源：http://lfk.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://drp.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://njo.nwbrower.top

[S53] C++：移动语义
来源：http://awe.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://kka.gotoacloud.top

[S54] C++：异常处理
来源：http://nuf.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jdy.52xcode.cn

[S55] C++：结构化绑定
来源：http://zih.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://puf.jianghu66.top

[S56] C++：optional
来源：http://uay.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cgh.dashuyun.cn

[S57] C++：编译期常量
来源：http://bvb.guowangkeji.top

constexpr int N = 10;
来源：http://vto.sweek.top

[S58] C++：命名空间
来源：http://ghv.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://uln.0kj1m.cn

[S59] C++：静态断言
来源：http://bwt.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ogw.cashguo.top

[S60] C++：遍历并删除元素
来源：http://uvx.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmr.mhx1999.top

================================================================================
来源：http://hih.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oik.tian-w.cn

================================================================================
来源：http://vgt.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://cob.vqdsnc.cn

println("Hello")
来源：http://jfd.sjlbkw.cn

[T02] Kotlin：变量
来源：http://ktl.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kgv.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://oiu.zhongyouzk.top

"值: $b"
来源：http://zcj.jiagoushi.top

[T04] Kotlin：空安全
来源：http://gar.hammf.cn

val n: String? = null;  n?.length
来源：http://llk.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://phc.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kyt.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://dzn.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qwg.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://ygt.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xvc.epnwcf.com

[T08] Kotlin：数据类
来源：http://mmb.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://dig.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://kii.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://hjx.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://fvd.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jxo.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://zqx.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hzd.yonumen.top

[T12] Kotlin：解构声明
来源：http://hsr.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://ooa.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://lip.sweek.top

val m = mapOf("a" to 1)
来源：http://cqj.yangfankeji.com

[T14] Kotlin：循环
来源：http://ddu.gotoacloud.top

for (i in 1..10) println(i)
来源：http://eww.yanxiufei.cn

[T15] Kotlin：接口
来源：http://nad.birdmap.top

interface Shape { fun area(): Double }
来源：http://ptf.andypj.xyz

[T16] Swift：Hello World
来源：http://nmc.c1oappe.top

print("Hello")
来源：http://lud.daxiang520.top

[T17] Swift：变量与常量
来源：http://ily.sysykeji.top

var a = 1;  let b = 2
来源：http://jpe.bjfxy.top

[T18] Swift：字符串插值
来源：http://crq.yj20258.top

"值: \(b)"
来源：http://zhb.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://skr.gaohongyu789.top

if let n = opt { print(n) }
来源：http://cvl.yj202588.top

[T20] Swift：数组操作
来源：http://owr.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cjw.52xcode.cn

[T21] Swift：遍历
来源：http://sqn.svipenyu.cn

for x in a { print(x) }
来源：http://zsw.daxiang520.top

[T22] Swift：字典
来源：http://ehm.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://lbx.zhiwuduotai.top

[T23] Swift：函数
来源：http://seb.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zst.birdmap.top

[T24] Swift：闭包
来源：http://sxq.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://spj.snrcjt.cn

[T25] Swift：结构体
来源：http://wri.tianlin.xyz

struct P { var x: Int }
来源：http://oks.yuxming.cn

[T26] Swift：类与重写
来源：http://ijv.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://jlr.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://jyg.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://vkp.sysykeji.top

[T28] Swift：枚举
来源：http://qeb.feifeiyinyue.top

enum Color { case red, green }
来源：http://bph.xuanzx.com

[T29] Swift：guard 提前返回
来源：http://sqx.yonumen.top

guard let x = opt else { return }
来源：http://sju.jlsjyb.cn

[T30] Swift：协议
来源：http://rvp.pycfn.com

protocol Shape { func area() -> Double }
来源：http://nbz.yuxming.cn

[T31] Lua：Hello World
来源：http://mof.yj202588.top

print("Hello")
来源：http://exn.daxiang520.top

[T32] Lua：局部变量
来源：http://pns.zdbjq.cn

local a = 1
来源：http://igd.haohaochexian.top

[T33] Lua：表（数组）
来源：http://afv.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bgl.zhoulong.xyz

[T34] Lua：遍历表
来源：http://fvx.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kup.svipenyu.cn

[T35] Lua：字典表
来源：http://ayt.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://bgw.jinqigufen.top

[T36] Lua：函数
来源：http://knm.guowangkeji.top

function add(a, b) return a + b end
来源：http://asd.hnqzz.top

[T37] Lua：字符串拼接
来源：http://atw.xziqi.cn

"a" .. "b"
来源：http://ymy.ydzc1.top

[T38] Lua：条件
来源：http://epx.aizwys.cn

if x > 0 then print("正") end
来源：http://bgj.9152youxi.cn

[T39] Lua：模式匹配
来源：http://xyz.yj20258.top

string.find(s, "%d+")
来源：http://ude.jiagoushi.top

[T40] Lua：元表
来源：http://ffr.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://xqy.haohaochexian.top

[T41] Perl：Hello World
来源：http://juv.yanxiufei.cn

print "Hello\n";
来源：http://uti.bbcook.cn

[T42] Perl：变量类型
来源：http://hsn.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tki.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://jlx.xinyue.icu

"值: $a"
来源：http://jfx.vqdsnc.cn

[T44] Perl：条件
来源：http://ncs.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://xhr.tian-w.cn

[T45] Perl：数组遍历
来源：http://laz.ppjwa.cn

for my $x (@arr) { print $x; }
来源：http://wmj.haohaochexian.top

[T46] Perl：哈希操作
来源：http://eeh.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kqe.hfpthk.cn

[T47] Perl：正则捕获
来源：http://miz.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://saa.ehwqpu.com

[T48] Perl：正则替换
来源：http://gab.yj20258.top

$s =~ s/old/new/g;
来源：http://xbk.uphjek.com

[T49] Perl：函数
来源：http://loc.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jgr.fktsv.cn

[T50] Perl：逐行读文件
来源：http://qqi.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zqc.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://nao.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://lsq.dashuyun.cn

println("Hello")
来源：http://tva.vehdjk.com

[T52] Scala：变量
来源：http://npk.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://wmh.birdmap.top

[T53] Scala：字符串插值
来源：http://bby.ivvv.top

s"值: $b"
来源：http://wsq.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://gtz.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://mns.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://kuq.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fdq.shangyingyoupin.top

[T56] Scala：样例类
来源：http://ejh.jinyuanbaomall.cn


<!-- 参考信息 -->