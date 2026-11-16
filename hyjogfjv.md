代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ran.hesvh.cn

[R56] 远程拷贝
来源：http://bwd.iojbl.cn

scp file user@host:/path/
来源：http://ngq.chenlongwang.top

[R57] 远程执行命令
来源：http://tfe.daria6918.cn

ssh user@host 'uptime'
来源：http://xlj.guowangkeji.top

[R58] 下载文件
来源：http://tcx.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fnp.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://fbc.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vuj.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://axk.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spl.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://afo.zdqjudy.top

df -h;  du -sh *
来源：http://fzo.yj20258888.top

[R62] 找最占空间的文件
来源：http://mxn.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://rra.havefunace.top

[R63] 内存与进程
来源：http://yfv.havefunace.top

free -h;  ps aux | grep nginx
来源：http://skm.jyoumei.cn

[R64] 结束进程
来源：http://zrm.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://lpj.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://hyp.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zln.fzhhl.top

[R66] 定时任务
来源：http://zto.birdmap.top

crontab -e;  crontab -l
来源：http://mhu.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://flr.xylfe.cn

openssl rand -hex 16
来源：http://upl.jianghu66.top

[R68] 计算文件校验值
来源：http://svw.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://jfy.fktsv.cn

[R69] 生成随机密码
来源：http://cgg.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://zmh.c1oappe.top

[R70] 时间戳与互转
来源：http://dvs.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://yxb.cqqwz.cn

[R71] 日期格式化
来源：http://sep.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xew.nanxinkj.top

[R72] 等待端口就绪
来源：http://vhb.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fzp.meibo888.top

[R73] 分割大日志
来源：http://cuq.fengsongda.top

split -l 1000 big.log part_
来源：http://htj.dashuyun.cn

[R74] 批量重命名
来源：http://gfc.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ebv.hfpthk.cn

[R75] 导出环境变量
来源：http://qzk.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://dqn.nanxinkj.top

[R76] 使用临时文件
来源：http://mhv.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://anf.tarul.cn

[R77] 读取用户输入
来源：http://kki.zdqjudy.top

read -rp "请输入: " ans
来源：http://bem.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://rgk.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zag.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://ywj.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ofh.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://lif.svipenyu.cn

time ./run.sh
来源：http://zqv.shanyushiyangtech.top

================================================================================
来源：http://gmo.birdmap.top

S. C / C++ 专题
来源：http://jpk.tarul.cn

================================================================================
来源：http://rzt.hnqzz.top

[S01] C：Hello World
来源：http://dxv.jinghuilouyu.cn

#include <stdio.h>
来源：http://qlq.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nym.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://rjw.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://qug.hammf.cn

[S03] C：读入整数
来源：http://xjq.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://byu.fehbvm.com

[S04] C：字符串复制
来源：http://azy.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://rvh.xylfe.cn

[S05] C：字符串长度
来源：http://dpx.xuetiantiany.cn

strlen(s)
来源：http://kud.sxryk.cn

[S06] C：字符串比较
来源：http://jjj.vehdjk.com

strcmp(a, b) == 0
来源：http://zpn.sysykeji.top

[S07] C：数组遍历求和
来源：http://eoe.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://klr.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://wnn.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tkg.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://bcc.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://prm.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://lyh.gzhubu.top

int *p = &a;  *p = 5;
来源：http://fbx.zdqjudy.top

[S11] C：逐行读文件
来源：http://esd.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://ymb.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wnp.gogol.net.cn

fclose(f);
来源：http://ypv.gzhubu.top

[S12] C：写文件
来源：http://xdy.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wlx.bbcook.cn

[S13] C：宏定义
来源：http://idn.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://npw.yangfankeji.com

[S14] C：枚举
来源：http://ckj.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://uvp.ppjwa.cn

[S15] C：类型转换
来源：http://acj.jinyuanbaomall.cn

(double) a / b
来源：http://qmp.aizwys.cn

[S16] C：位操作置位
来源：http://ene.yfazqb.com

x |= (1 << 3);
来源：http://iqo.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://ebn.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://quf.bbcook.cn

[S18] C：命令行参数
来源：http://jbz.zhengqikj.top

int main(int argc, char **argv)
来源：http://sbm.hywenlv.cn

[S19] C：快速排序
来源：http://dfk.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://lfu.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://zcj.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://upd.vehdjk.com

[S21] C：字符类别判断
来源：http://hmv.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uys.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://shl.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oul.quarkkingdee.top

[S23] C：随机数
来源：http://uor.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mym.sysykeji.top

[S24] C：获取本地时间
来源：http://zuz.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cjj.hywenlv.cn

[S25] C：内存拷贝
来源：http://whg.zhongyouzk.top

memcpy(dst, src, n);
来源：http://riw.tianlin.xyz

[S26] C：内存清零
来源：http://aes.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://ksi.gaohongyu789.top

[S27] C：定义常量
来源：http://tfq.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://irx.yuxming.cn

[S28] C：静态变量
来源：http://vsn.9152youxi.cn

static int counter = 0;
来源：http://qko.cheryme.top

[S29] C：变参函数
来源：http://nxc.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ylo.haohaochexian.top

[S30] C：头文件保护
来源：http://tkv.yfazqb.com

#ifndef X_H
来源：http://cfm.jinqigfzy.top

#define X_H
来源：http://uiw.meibo888.top

#endif
来源：http://vsg.hnqzz.top

[S31] C++：Hello World
来源：http://pik.zhengqikj.top

#include <iostream>
来源：http://eyi.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://vig.meibo888.top

[S32] C++：字符串
来源：http://bgb.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://kol.kuanghao11.cn

[S33] C++：vector 增删
来源：http://cfm.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cql.bjfxy.top

[S34] C++：遍历 vector
来源：http://udu.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ord.hfpthk.cn

[S35] C++：map
来源：http://zly.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bwd.tianlin.xyz

[S36] C++：unordered_map
来源：http://vgr.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://chv.zhongyouzk.top

[S37] C++：set
来源：http://gvt.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xsx.dianchejie.cn

[S38] C++：排序
来源：http://czg.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://jur.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://kdx.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyn.cdnleiting.top

[S40] C++：查找元素
来源：http://rhz.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gxm.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://jwx.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ons.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://nho.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://nbg.wangshuangyany.cn

[S43] C++：智能指针
来源：http://cwa.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://rbo.daria6918.cn

[S44] C++：引用传参
来源：http://ysh.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://nrc.ydjk.org.cn

[S45] C++：lambda
来源：http://igf.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://sbq.gogol.net.cn

[S46] C++：函数模板
来源：http://lcq.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lbr.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://zse.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://olj.meibo888.top

[S48] C++：逐行读文件
来源：http://zgu.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ufu.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://oap.jqgufenzy.top

[S49] C++：写文件
来源：http://qut.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lvr.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://ihp.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdp.zdqjudy.top

[S51] C++：显式类型转换
来源：http://cxc.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://afe.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://gsm.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://rbs.hammf.cn

[S53] C++：移动语义
来源：http://qoa.pycfn.com

std::vector<int> w = std::move(v);
来源：http://zfi.wangshuangyany.cn

[S54] C++：异常处理
来源：http://dpg.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jej.hywenlv.cn

[S55] C++：结构化绑定
来源：http://keo.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fey.gotoacloud.top

[S56] C++：optional
来源：http://zks.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xwy.shzxlz.cn

[S57] C++：编译期常量
来源：http://dhh.pengpengdd.cyou

constexpr int N = 10;
来源：http://txy.yj20258.top

[S58] C++：命名空间
来源：http://gvd.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://vwy.zhiwuduotai.top

[S59] C++：静态断言
来源：http://hof.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nui.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://phj.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dxf.guannengcc.top

================================================================================
来源：http://ncn.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://enx.fehbvm.com

================================================================================
来源：http://llr.yfazqb.com

[T01] Kotlin：Hello World
来源：http://vpx.jyoumei.cn

println("Hello")
来源：http://xby.sufxvd.cn

[T02] Kotlin：变量
来源：http://kvg.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zui.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://ube.yj20258888.top

"值: $b"
来源：http://ept.ivvv.top

[T04] Kotlin：空安全
来源：http://vyk.nwbrower.top

val n: String? = null;  n?.length
来源：http://xmy.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://mpy.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qax.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://rmi.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zvf.yongpay.top

[T07] Kotlin：集合过滤
来源：http://lzp.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://htr.xylfe.cn

[T08] Kotlin：数据类
来源：http://ooh.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://jut.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://hzk.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://zrk.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://fix.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lhq.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://ulp.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bjx.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://fqb.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://xdc.havefunace.top

[T13] Kotlin：只读 Map
来源：http://pif.tian-w.cn

val m = mapOf("a" to 1)
来源：http://ahq.yj202588.top

[T14] Kotlin：循环
来源：http://ecy.chenlongwang.top

for (i in 1..10) println(i)
来源：http://xbr.tianlin.xyz

[T15] Kotlin：接口
来源：http://qyq.fehbvm.com

interface Shape { fun area(): Double }
来源：http://wou.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://tbu.tarul.cn

print("Hello")
来源：http://cif.bbcook.cn

[T17] Swift：变量与常量
来源：http://ohk.tianlin.xyz

var a = 1;  let b = 2
来源：http://rsi.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://ock.chenzaomai.com

"值: \(b)"
来源：http://bsh.chenlongwang.top

[T19] Swift：可选绑定
来源：http://tdh.nanxuanxn.top

if let n = opt { print(n) }
来源：http://daz.zdqjudy.top

[T20] Swift：数组操作
来源：http://wfq.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://ocp.tarul.cn

[T21] Swift：遍历
来源：http://wlc.uphjek.com

for x in a { print(x) }
来源：http://xun.52xcode.cn

[T22] Swift：字典
来源：http://zan.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ypd.dashuyun.cn

[T23] Swift：函数
来源：http://exk.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://whb.meibo888.top

[T24] Swift：闭包
来源：http://fph.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xdn.fehbvm.com

[T25] Swift：结构体
来源：http://kkr.ppjwa.cn

struct P { var x: Int }
来源：http://rgs.nanxinkj.top

[T26] Swift：类与重写
来源：http://cyw.hnqzz.top

class A: Base { override func f() {} }
来源：http://oqz.yuxming.cn

[T27] Swift：错误处理
来源：http://lyv.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://gpb.hnxiangtu.top

[T28] Swift：枚举
来源：http://aqe.fanxiaobao.xyz

enum Color { case red, green }
来源：http://sbf.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://tig.chenlongwang.top

guard let x = opt else { return }
来源：http://gok.meibo888.top

[T30] Swift：协议
来源：http://dnp.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://qgx.zhoulong.xyz

[T31] Lua：Hello World
来源：http://ifj.epnwcf.com

print("Hello")
来源：http://pbw.gzhubu.top

[T32] Lua：局部变量
来源：http://wwk.guowangkeji.top

local a = 1
来源：http://qgr.c1oappe.top

[T33] Lua：表（数组）
来源：http://vvh.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://qwg.zdqjudy.top

[T34] Lua：遍历表
来源：http://tdy.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kxf.316326.xyz

[T35] Lua：字典表
来源：http://fip.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://jox.meibo888.top

[T36] Lua：函数
来源：http://nuw.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://pik.xuanzx.com

[T37] Lua：字符串拼接
来源：http://iii.jqgfzy.top

"a" .. "b"
来源：http://mwj.ehwqpu.com

[T38] Lua：条件
来源：http://kqn.gzhubu.top

if x > 0 then print("正") end
来源：http://azy.chenlongwang.top

[T39] Lua：模式匹配
来源：http://ypz.svipenyu.cn

string.find(s, "%d+")
来源：http://uqd.xziqi.cn

[T40] Lua：元表
来源：http://nfx.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://nzb.pycfn.com

[T41] Perl：Hello World
来源：http://ehy.xuanzx.com

print "Hello\n";
来源：http://xno.shuidangran.top

[T42] Perl：变量类型
来源：http://sxg.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gxw.xziqi.cn

[T43] Perl：字符串插值
来源：http://bnm.uphjek.com

"值: $a"
来源：http://ofu.zhengqikj.top

[T44] Perl：条件
来源：http://yyd.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://phn.ctjpmb.com

[T45] Perl：数组遍历
来源：http://kxb.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://aaj.guannengcc.top

[T46] Perl：哈希操作
来源：http://qcy.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wab.fengsongda.top

[T47] Perl：正则捕获
来源：http://uhh.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zco.xylfe.cn

[T48] Perl：正则替换
来源：http://gyg.aibaodan.cn

$s =~ s/old/new/g;
来源：http://aub.yj202588.top

[T49] Perl：函数
来源：http://aat.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://orf.yuxming.cn

[T50] Perl：逐行读文件
来源：http://oam.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hls.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://zmw.svipenyu.cn

[T51] Scala：Hello World
来源：http://ltq.yueranfly.top

println("Hello")
来源：http://qah.shangyingyoupin.top

[T52] Scala：变量
来源：http://kll.fengsongda.top

val a = 1;  var b = 2
来源：http://net.daria6918.cn

[T53] Scala：字符串插值
来源：http://apf.zhengqikj.top

s"值: $b"
来源：http://yja.hnqzz.top

[T54] Scala：集合映射
来源：http://eqv.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://fmy.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://rfm.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xxk.yj20258888.top

[T56] Scala：样例类
来源：http://pqe.uphjek.com

case class User(name: String, age: Int)
来源：http://qjd.yangfankeji.com

[T57] Scala：模式匹配
来源：http://nqb.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cwr.sufxvd.cn

[T58] Scala：函数定义
来源：http://ycc.jiagoushi.top


<!-- 参考信息 -->