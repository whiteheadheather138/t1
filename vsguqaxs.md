代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://but.316326.xyz

[R50] awk 求和
来源：http://fdm.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cka.yuanzhike.top

[R51] 排序去重取前几
来源：http://gcy.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://msj.bjfxy.top

[R52] 统计行数
来源：http://iws.ctjpmb.com

wc -l a.txt
来源：http://crr.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://ync.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kjk.zhijiandao.cn

[R54] 比较两个文件
来源：http://lcb.cqqwz.cn

diff a.txt b.txt
来源：http://guu.yuxming.cn

[R55] 压缩与解压
来源：http://nax.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://omu.zhijiandao.cn

[R56] 远程拷贝
来源：http://rhw.zdbjq.cn

scp file user@host:/path/
来源：http://odm.shangyingyoupin.top

[R57] 远程执行命令
来源：http://blb.tarul.cn

ssh user@host 'uptime'
来源：http://aqv.shzxlz.cn

[R58] 下载文件
来源：http://wvw.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://beh.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://qnn.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fjj.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://rph.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://koq.havefunace.top

[R61] 磁盘占用
来源：http://vgd.vqdsnc.cn

df -h;  du -sh *
来源：http://wfn.ctjpmb.com

[R62] 找最占空间的文件
来源：http://jyx.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://kbv.52xcode.cn

[R63] 内存与进程
来源：http://plv.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://ikf.pycfn.com

[R64] 结束进程
来源：http://lnr.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://nlh.dianchejie.cn

[R65] 查看端口占用
来源：http://rfd.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xom.shanyushiyangkeji.top

[R66] 定时任务
来源：http://ycv.zhengqikj.top

crontab -e;  crontab -l
来源：http://jhn.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://xlq.hammf.cn

openssl rand -hex 16
来源：http://bxw.c1oappe.top

[R68] 计算文件校验值
来源：http://vrq.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://qcq.epnwcf.com

[R69] 生成随机密码
来源：http://mtm.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://kht.yangfankeji.com

[R70] 时间戳与互转
来源：http://toa.316326.xyz

date +%s;  date -d @1700000000
来源：http://pbd.yvedp.cn

[R71] 日期格式化
来源：http://eih.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://oyl.tianlin.xyz

[R72] 等待端口就绪
来源：http://zhz.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fdr.xuanzx.com

[R73] 分割大日志
来源：http://xxg.meibo888.top

split -l 1000 big.log part_
来源：http://iqa.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://ssz.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oxv.jinqigufen.top

[R75] 导出环境变量
来源：http://xgk.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://bbx.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://eae.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ehh.feifeiyinyue.top

[R77] 读取用户输入
来源：http://ukg.ydjk.org.cn

read -rp "请输入: " ans
来源：http://ohf.yj20258888.top

[R78] 交互式菜单
来源：http://jaj.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wkm.zhengqikj.top

[R79] 解析命令行选项
来源：http://auz.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pbd.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://ieh.ydzc1.top

time ./run.sh
来源：http://qye.chenzaomai.com

================================================================================
来源：http://uqa.cqqwz.cn

S. C / C++ 专题
来源：http://wjm.wangdashe.top

================================================================================
来源：http://bub.dashuyun.cn

[S01] C：Hello World
来源：http://kxi.ydjk.org.cn

#include <stdio.h>
来源：http://cso.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qcd.nwbrower.top

[S02] C：变量与格式化输出
来源：http://fwo.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://igy.sufxvd.cn

[S03] C：读入整数
来源：http://utz.fengsongda.top

int x; scanf("%d", &x);
来源：http://noe.daria6918.cn

[S04] C：字符串复制
来源：http://vkn.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://zoz.sjlbkw.cn

[S05] C：字符串长度
来源：http://cin.aibaodan.cn

strlen(s)
来源：http://qmb.bjfxy.top

[S06] C：字符串比较
来源：http://sdk.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://cpy.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://evv.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ywy.meibo888.top

[S08] C：动态内存分配与释放
来源：http://lhg.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hii.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://scc.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xjv.gaohongyu789.top

[S10] C：指针与解引用
来源：http://rcb.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://wgt.zhengqikj.top

[S11] C：逐行读文件
来源：http://kga.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://aec.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vek.feifeiyinyue.top

fclose(f);
来源：http://ezh.jiagoushi.top

[S12] C：写文件
来源：http://dvq.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tot.hammf.cn

[S13] C：宏定义
来源：http://mts.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gtu.jqgfzy.top

[S14] C：枚举
来源：http://tsh.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://vcn.yj202588.top

[S15] C：类型转换
来源：http://pci.zdbjq.cn

(double) a / b
来源：http://zbo.gaohongyu789.top

[S16] C：位操作置位
来源：http://iun.xylfe.cn

x |= (1 << 3);
来源：http://hfg.c1oappe.top

[S17] C：安全拼接字符串
来源：http://fry.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://flv.bjfxy.top

[S18] C：命令行参数
来源：http://rhj.jiagoushi.top

int main(int argc, char **argv)
来源：http://sbw.guannengcc.top

[S19] C：快速排序
来源：http://eqr.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://auy.xuanzx.com

[S20] C：二分查找
来源：http://yei.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvc.fengsongda.top

[S21] C：字符类别判断
来源：http://stz.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://por.yj202588.top

[S22] C：字符串转数字
来源：http://urz.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://yvt.uphjek.com

[S23] C：随机数
来源：http://ewl.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://qgp.cqqwz.cn

[S24] C：获取本地时间
来源：http://dov.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ixt.nanxinkj.top

[S25] C：内存拷贝
来源：http://tpj.zdqjudy.top

memcpy(dst, src, n);
来源：http://nra.yj202588.top

[S26] C：内存清零
来源：http://ahb.tanke756.top

memset(a, 0, sizeof a);
来源：http://ltk.shanyushiyangtech.top

[S27] C：定义常量
来源：http://ayu.ppjwa.cn

const double PI = 3.14159;
来源：http://tzb.svipenyu.cn

[S28] C：静态变量
来源：http://kpx.yj20258.top

static int counter = 0;
来源：http://ymh.nwbrower.top

[S29] C：变参函数
来源：http://ihp.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ran.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://tgs.yj20258.top

#ifndef X_H
来源：http://hyu.mhx1999.top

#define X_H
来源：http://rcl.wangdashe.top

#endif
来源：http://dro.kuanghao11.cn

[S31] C++：Hello World
来源：http://kin.shangyingyoupin.top

#include <iostream>
来源：http://smd.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://uvf.mhx1999.top

[S32] C++：字符串
来源：http://uoy.cashguo.top

std::string s = "hi";  s += "!";
来源：http://snn.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://snn.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pqz.yonumen.top

[S34] C++：遍历 vector
来源：http://kaf.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://moc.xingfuxueyuan.xyz

[S35] C++：map
来源：http://ylf.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ilm.tarul.cn

[S36] C++：unordered_map
来源：http://anh.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lmn.316326.xyz

[S37] C++：set
来源：http://cje.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jyv.pycfn.com

[S38] C++：排序
来源：http://mwp.pycfn.com

std::sort(v.begin(), v.end());
来源：http://njx.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://dui.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yws.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://ayc.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oug.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://jbu.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qmr.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://gex.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://zmo.yangfankeji.com

[S43] C++：智能指针
来源：http://lgn.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://tkh.sweek.top

[S44] C++：引用传参
来源：http://jxc.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://afb.yj20258888.top

[S45] C++：lambda
来源：http://tku.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ome.gzhubu.top

[S46] C++：函数模板
来源：http://iyz.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zsq.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://bxf.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://acg.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://udk.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://gws.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://myt.jiagoushi.top

[S49] C++：写文件
来源：http://dre.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ogx.guowangkeji.top

[S50] C++：格式化数字
来源：http://jne.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yzc.ivvv.top

[S51] C++：显式类型转换
来源：http://elk.tanke756.top

static_cast<double>(a) / b
来源：http://kdq.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://clj.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://rty.cdnleiting.top

[S53] C++：移动语义
来源：http://oid.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://qdf.vehdjk.com

[S54] C++：异常处理
来源：http://azk.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vkc.dianchejie.cn

[S55] C++：结构化绑定
来源：http://eaf.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bew.daria6918.cn

[S56] C++：optional
来源：http://onv.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gfy.hammf.cn

[S57] C++：编译期常量
来源：http://fcf.ydjk.org.cn

constexpr int N = 10;
来源：http://cqg.hongshengwenyu.top

[S58] C++：命名空间
来源：http://wau.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://sja.ybcxt.top

[S59] C++：静态断言
来源：http://xrq.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kcn.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://lfs.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zmw.guannengcc.top

================================================================================
来源：http://scc.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aqc.fengsongda.top

================================================================================
来源：http://syp.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://nlf.mhx1999.top

println("Hello")
来源：http://coz.hesvh.cn

[T02] Kotlin：变量
来源：http://zjb.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oks.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://nhi.epnwcf.com

"值: $b"
来源：http://eic.aizwys.cn

[T04] Kotlin：空安全
来源：http://ivb.xziqi.cn

val n: String? = null;  n?.length
来源：http://chd.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://xwa.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xpo.316326.xyz

[T06] Kotlin：集合映射
来源：http://ius.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hca.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://yjc.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://scg.nwbrower.top

[T08] Kotlin：数据类
来源：http://gyj.sweek.top

data class User(val name: String, val age: Int)
来源：http://lom.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://tdp.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://hdl.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://jml.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xpq.smart0.xyz

[T11] Kotlin：协程
来源：http://mxv.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixg.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://uxa.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://fou.hammf.cn

[T13] Kotlin：只读 Map
来源：http://iwj.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://gtf.fengsongda.top

[T14] Kotlin：循环
来源：http://unu.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://rxt.ydzc1.top

[T15] Kotlin：接口
来源：http://ryl.zycfv.cn

interface Shape { fun area(): Double }
来源：http://bpu.yuxming.cn

[T16] Swift：Hello World
来源：http://igy.ctjpmb.com

print("Hello")
来源：http://bpt.smart0.xyz

[T17] Swift：变量与常量
来源：http://vus.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://ntj.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://xve.shuidangran.top

"值: \(b)"
来源：http://who.havefunace.top

[T19] Swift：可选绑定
来源：http://bla.nanxuanxn.top

if let n = opt { print(n) }
来源：http://hip.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://rfa.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://lwi.yuxming.cn

[T21] Swift：遍历
来源：http://zmw.yuanzhike.top

for x in a { print(x) }
来源：http://xrn.chenjidiqi.icu

[T22] Swift：字典
来源：http://vba.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cac.yfazqb.com

[T23] Swift：函数
来源：http://hpy.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gow.ybcxt.top

[T24] Swift：闭包
来源：http://tln.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsa.guowangkeji.top

[T25] Swift：结构体
来源：http://kdl.birdmap.top

struct P { var x: Int }
来源：http://oxc.cqqwz.cn

[T26] Swift：类与重写
来源：http://nwk.hfpthk.cn

class A: Base { override func f() {} }
来源：http://irx.dianchejie.cn

[T27] Swift：错误处理
来源：http://yhm.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://tkc.pycfn.com

[T28] Swift：枚举
来源：http://oml.9152youxi.cn

enum Color { case red, green }
来源：http://pvc.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://pjk.yonumen.top

guard let x = opt else { return }
来源：http://vxx.52xcode.cn

[T30] Swift：协议
来源：http://cnu.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://msc.hysaishi.cn

[T31] Lua：Hello World
来源：http://jdh.zhijiandao.cn

print("Hello")
来源：http://mom.hcnkem.com

[T32] Lua：局部变量
来源：http://bui.vehdjk.com

local a = 1
来源：http://zwo.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://wux.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://exh.fzhhl.top

[T34] Lua：遍历表
来源：http://wff.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rqv.wangshuangyany.cn

[T35] Lua：字典表
来源：http://heo.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://xrp.chenlongwang.top

[T36] Lua：函数
来源：http://bcl.hysaishi.cn

function add(a, b) return a + b end
来源：http://wsg.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://msi.guannengcc.top

"a" .. "b"
来源：http://twe.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://umm.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://kur.vehdjk.com

[T39] Lua：模式匹配
来源：http://xvp.nanxinkj.top

string.find(s, "%d+")
来源：http://jyy.yj20258888.top

[T40] Lua：元表
来源：http://ryr.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://scs.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://rkb.hywenlv.cn

print "Hello\n";
来源：http://sdz.jyoumei.cn

[T42] Perl：变量类型
来源：http://ibk.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pql.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://wnp.jinyuanbaomall.cn

"值: $a"
来源：http://mvv.zhijiandao.cn

[T44] Perl：条件
来源：http://pbi.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://pch.zhixingplan.top

[T45] Perl：数组遍历
来源：http://koz.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://igt.daria6918.cn

[T46] Perl：哈希操作
来源：http://ueu.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yuw.wangdashe.top

[T47] Perl：正则捕获
来源：http://mwm.cucudq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jui.jlsjyb.cn

[T48] Perl：正则替换
来源：http://wus.guannengcc.top

$s =~ s/old/new/g;
来源：http://fbv.tian-w.cn

[T49] Perl：函数
来源：http://ysb.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xto.wangdashe.top

[T50] Perl：逐行读文件
来源：http://vlv.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://etf.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://szm.yfazqb.com

[T51] Scala：Hello World
来源：http://rwl.zhixingplan.top

println("Hello")
来源：http://mql.fktsv.cn

[T52] Scala：变量
来源：http://xtd.yfazqb.com


<!-- 参考信息 -->