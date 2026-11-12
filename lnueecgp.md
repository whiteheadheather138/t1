代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://kuo.chenlongwang.top

[R52] 统计行数
来源：http://vig.aibaodan.cn

wc -l a.txt
来源：http://jzy.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://yjf.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kjk.hongshengwenyu.top

[R54] 比较两个文件
来源：http://xgr.zycfv.cn

diff a.txt b.txt
来源：http://fhg.chenzaomai.com

[R55] 压缩与解压
来源：http://xgx.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lio.52xcode.cn

[R56] 远程拷贝
来源：http://hrb.jlsjyb.cn

scp file user@host:/path/
来源：http://stq.iojbl.cn

[R57] 远程执行命令
来源：http://ofd.guowangkeji.top

ssh user@host 'uptime'
来源：http://pyd.jinghuilouyu.cn

[R58] 下载文件
来源：http://xzb.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ayr.dianchejie.cn

[R59] 发 POST JSON
来源：http://hph.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pui.zhiwuduotai.top

[R60] 只看 HTTP 状态码
来源：http://cie.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://umc.fengsongda.top

[R61] 磁盘占用
来源：http://sym.yvedp.cn

df -h;  du -sh *
来源：http://khi.ctjpmb.com

[R62] 找最占空间的文件
来源：http://wts.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://ltd.gotoacloud.top

[R63] 内存与进程
来源：http://etp.ivvv.top

free -h;  ps aux | grep nginx
来源：http://xfq.nwbrower.top

[R64] 结束进程
来源：http://wan.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://vla.hywenlv.cn

[R65] 查看端口占用
来源：http://mty.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://odl.gzhubu.top

[R66] 定时任务
来源：http://lfr.sysykeji.top

crontab -e;  crontab -l
来源：http://jnf.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://sbo.gzhubu.top

openssl rand -hex 16
来源：http://hbr.birdmap.top

[R68] 计算文件校验值
来源：http://qpt.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://ojt.hammf.cn

[R69] 生成随机密码
来源：http://xhx.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://xkf.yj20258.top

[R70] 时间戳与互转
来源：http://gpa.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://rzf.daria6918.cn

[R71] 日期格式化
来源：http://daf.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jvs.hnxiangtu.top

[R72] 等待端口就绪
来源：http://lud.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://smv.wangshuangyany.cn

[R73] 分割大日志
来源：http://rbn.cdnleiting.top

split -l 1000 big.log part_
来源：http://npm.yueranfly.top

[R74] 批量重命名
来源：http://ehu.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnz.pengpengdd.cyou

[R75] 导出环境变量
来源：http://loy.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://leb.zdqjudy.top

[R76] 使用临时文件
来源：http://ibq.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iif.zdqjudy.top

[R77] 读取用户输入
来源：http://fbe.hfpthk.cn

read -rp "请输入: " ans
来源：http://uox.chenjidiqi.icu

[R78] 交互式菜单
来源：http://cvk.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bij.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://cth.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://afu.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://zee.wangdashe.top

time ./run.sh
来源：http://svg.zhaomingkeji.xyz

================================================================================
来源：http://jkd.zycfv.cn

S. C / C++ 专题
来源：http://rwe.sjlbkw.cn

================================================================================
来源：http://cay.aibaodan.cn

[S01] C：Hello World
来源：http://zdr.jinqigufen.top

#include <stdio.h>
来源：http://acr.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sud.ydzc1.top

[S02] C：变量与格式化输出
来源：http://fap.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://hlb.meibo888.top

[S03] C：读入整数
来源：http://pql.yj20258.top

int x; scanf("%d", &x);
来源：http://kez.wangdashe.top

[S04] C：字符串复制
来源：http://jgj.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://fch.zhijiandao.cn

[S05] C：字符串长度
来源：http://hzf.iojbl.cn

strlen(s)
来源：http://kev.dashuyun.cn

[S06] C：字符串比较
来源：http://ckm.nanxinkj.top

strcmp(a, b) == 0
来源：http://gpp.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://wxc.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eoc.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://thg.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dts.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://zkv.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://trl.dashuyun.cn

[S10] C：指针与解引用
来源：http://rri.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://uin.daria6918.cn

[S11] C：逐行读文件
来源：http://wnv.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://qxl.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://qjm.tanke756.top

fclose(f);
来源：http://vjt.ivvv.top

[S12] C：写文件
来源：http://ymf.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imj.uphjek.com

[S13] C：宏定义
来源：http://aee.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vbn.ehwqpu.com

[S14] C：枚举
来源：http://cuu.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://ywk.fktsv.cn

[S15] C：类型转换
来源：http://ogc.yuxming.cn

(double) a / b
来源：http://tzf.haohaochexian.top

[S16] C：位操作置位
来源：http://spm.kuanghao11.cn

x |= (1 << 3);
来源：http://odf.nwbrower.top

[S17] C：安全拼接字符串
来源：http://hgb.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jza.yvedp.cn

[S18] C：命令行参数
来源：http://zqd.xziqi.cn

int main(int argc, char **argv)
来源：http://tzb.xylfe.cn

[S19] C：快速排序
来源：http://ome.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://sjj.sufxvd.cn

[S20] C：二分查找
来源：http://urr.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crg.fengsongda.top

[S21] C：字符类别判断
来源：http://quz.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zga.jinqigufen.top

[S22] C：字符串转数字
来源：http://rxx.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://tzb.sysykeji.top

[S23] C：随机数
来源：http://qrm.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rpc.0kj1m.cn

[S24] C：获取本地时间
来源：http://ocx.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ccl.daria6918.cn

[S25] C：内存拷贝
来源：http://snc.jlsjyb.cn

memcpy(dst, src, n);
来源：http://ofc.ppjwa.cn

[S26] C：内存清零
来源：http://wjj.ybcxt.top

memset(a, 0, sizeof a);
来源：http://ici.bjfxy.top

[S27] C：定义常量
来源：http://agg.hywenlv.cn

const double PI = 3.14159;
来源：http://yut.wangshuangyany.cn

[S28] C：静态变量
来源：http://hcc.zhaomingkeji.xyz

static int counter = 0;
来源：http://gft.quarkkingdee.top

[S29] C：变参函数
来源：http://cdu.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uxz.shuidangran.top

[S30] C：头文件保护
来源：http://ndl.epnwcf.com

#ifndef X_H
来源：http://ijx.cashguo.top

#define X_H
来源：http://hxt.sweek.top

#endif
来源：http://brd.fengsongda.top

[S31] C++：Hello World
来源：http://yif.yongpay.top

#include <iostream>
来源：http://uzx.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ift.hammf.cn

[S32] C++：字符串
来源：http://xjf.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://eel.xinyue.icu

[S33] C++：vector 增删
来源：http://vxz.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fma.sxryk.cn

[S34] C++：遍历 vector
来源：http://hsy.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://hhw.zhaomingkeji.xyz

[S35] C++：map
来源：http://ffp.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qbz.daxiang520.top

[S36] C++：unordered_map
来源：http://tfm.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pnl.chenjidiqi.icu

[S37] C++：set
来源：http://lrd.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xvq.cashguo.top

[S38] C++：排序
来源：http://xea.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://kex.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://xpb.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jfj.ybcxt.top

[S40] C++：查找元素
来源：http://ahu.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kfj.cdnleiting.top

[S41] C++：类与构造函数
来源：http://okb.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://odz.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://viu.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://ohn.dashuyun.cn

[S43] C++：智能指针
来源：http://lnv.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://byw.yongpay.top

[S44] C++：引用传参
来源：http://mob.zycfv.cn

void inc(int &x) { ++x; }
来源：http://kyl.guowangkeji.top

[S45] C++：lambda
来源：http://zdo.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bzc.xuetiantiany.cn

[S46] C++：函数模板
来源：http://vou.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hfc.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://kqt.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kta.316326.xyz

[S48] C++：逐行读文件
来源：http://yiz.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://pkx.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://ute.feifeiyinyue.top

[S49] C++：写文件
来源：http://fqo.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jmc.fengsongda.top

[S50] C++：格式化数字
来源：http://wnb.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ayx.9152youxi.cn

[S51] C++：显式类型转换
来源：http://emz.xinyue.icu

static_cast<double>(a) / b
来源：http://aza.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://zth.fengsongda.top

int size() const noexcept { return n_; }
来源：http://rwf.xuetiantiany.cn

[S53] C++：移动语义
来源：http://ofq.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://sxp.sjlbkw.cn

[S54] C++：异常处理
来源：http://gzj.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://epu.daxiang520.top

[S55] C++：结构化绑定
来源：http://ppb.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://duo.gotoacloud.top

[S56] C++：optional
来源：http://poc.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blj.epnwcf.com

[S57] C++：编译期常量
来源：http://uyw.yuanzhike.top

constexpr int N = 10;
来源：http://tjs.c1oappe.top

[S58] C++：命名空间
来源：http://dvg.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://nur.sxryk.cn

[S59] C++：静态断言
来源：http://qar.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ecz.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://yck.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bdp.sjlbkw.cn

================================================================================
来源：http://ywe.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqa.guannengcc.top

================================================================================
来源：http://xmr.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://arc.shanyushiyangtech.top

println("Hello")
来源：http://xcr.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://wba.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://umh.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://cmb.52xcode.cn

"值: $b"
来源：http://tys.hnqzz.top

[T04] Kotlin：空安全
来源：http://mog.tarul.cn

val n: String? = null;  n?.length
来源：http://chf.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://khd.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rlg.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://kjr.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zds.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://tbv.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tbd.ppjwa.cn

[T08] Kotlin：数据类
来源：http://nrs.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://pxv.hammf.cn

[T09] Kotlin：扩展函数
来源：http://fxj.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://sck.mhx1999.top

[T10] Kotlin：默认参数
来源：http://qrs.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qfg.nanxuanxn.top

[T11] Kotlin：协程
来源：http://cti.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://exy.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://vwp.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://mei.tanke756.top

[T13] Kotlin：只读 Map
来源：http://far.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://rqk.smart0.xyz

[T14] Kotlin：循环
来源：http://ndk.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://ish.zhongyouzk.top

[T15] Kotlin：接口
来源：http://oxn.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://blf.bjfxy.top

[T16] Swift：Hello World
来源：http://llu.jinqigfzy.top

print("Hello")
来源：http://tsl.xylfe.cn

[T17] Swift：变量与常量
来源：http://sxo.haohaochexian.top

var a = 1;  let b = 2
来源：http://axf.daxiang520.top

[T18] Swift：字符串插值
来源：http://wtx.sjlbkw.cn

"值: \(b)"
来源：http://hba.birdmap.top

[T19] Swift：可选绑定
来源：http://ral.yonumen.top

if let n = opt { print(n) }
来源：http://qjm.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://oim.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://msz.ydjk.org.cn

[T21] Swift：遍历
来源：http://muj.wangshuangyany.cn

for x in a { print(x) }
来源：http://aqp.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://hkz.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mro.jqgufenzy.top

[T23] Swift：函数
来源：http://epo.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aks.316326.xyz

[T24] Swift：闭包
来源：http://tev.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jwb.xinyue.icu

[T25] Swift：结构体
来源：http://xpu.hywenlv.cn

struct P { var x: Int }
来源：http://jod.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://cxq.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://ukc.bbcook.cn

[T27] Swift：错误处理
来源：http://gjp.cucudq.cn

do { try f() } catch { print(error) }
来源：http://rgw.meibo888.top

[T28] Swift：枚举
来源：http://tmm.fktsv.cn

enum Color { case red, green }
来源：http://tqw.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://iqr.kuanghao11.cn

guard let x = opt else { return }
来源：http://hqw.nwbrower.top

[T30] Swift：协议
来源：http://smk.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://wbr.dianchejie.cn

[T31] Lua：Hello World
来源：http://amh.bjfxy.top

print("Hello")
来源：http://eej.yueranfly.top

[T32] Lua：局部变量
来源：http://ajw.svipenyu.cn

local a = 1
来源：http://mxj.svipenyu.cn

[T33] Lua：表（数组）
来源：http://xpq.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hnc.yuanzhike.top

[T34] Lua：遍历表
来源：http://yoc.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tlf.jiagoushi.top

[T35] Lua：字典表
来源：http://zug.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://zih.yj202588.top

[T36] Lua：函数
来源：http://mzo.xylfe.cn

function add(a, b) return a + b end
来源：http://psj.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://qcn.zhaomingkeji.xyz

"a" .. "b"
来源：http://zlu.jiagoushi.top

[T38] Lua：条件
来源：http://dtn.zycfv.cn

if x > 0 then print("正") end
来源：http://sjl.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://fnb.hywenlv.cn

string.find(s, "%d+")
来源：http://oah.yuanzhike.top

[T40] Lua：元表
来源：http://obl.gzhubu.top

setmetatable({}, { __index = base })
来源：http://fos.cashguo.top

[T41] Perl：Hello World
来源：http://yiy.haohaochexian.top

print "Hello\n";
来源：http://pen.yangfankeji.com

[T42] Perl：变量类型
来源：http://oxs.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://igm.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://asv.kuanghao11.cn

"值: $a"
来源：http://bls.dianchejie.cn

[T44] Perl：条件
来源：http://pgl.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://dos.sysykeji.top

[T45] Perl：数组遍历
来源：http://qhl.ivvv.top

for my $x (@arr) { print $x; }
来源：http://qdi.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://dow.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cjd.bbcook.cn

[T47] Perl：正则捕获
来源：http://apm.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gas.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://uxp.yvedp.cn

$s =~ s/old/new/g;
来源：http://dvy.dianchejie.cn

[T49] Perl：函数
来源：http://vwu.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ghg.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://uas.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zha.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://sqk.yuxming.cn

[T51] Scala：Hello World
来源：http://kcz.9152youxi.cn

println("Hello")
来源：http://nyk.9152youxi.cn

[T52] Scala：变量
来源：http://qwf.iojbl.cn

val a = 1;  var b = 2
来源：http://pgy.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://imj.tian-w.cn

s"值: $b"
来源：http://kjg.ehwqpu.com

[T54] Scala：集合映射
来源：http://ogx.gaohongyu789.top


<!-- 参考信息 -->