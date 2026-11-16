代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://vwx.tanke756.top

[R48] awk 取指定列
来源：http://kep.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://epp.jianghu66.top

[R49] awk 带条件
来源：http://foa.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ahm.jinqigufen.top

[R50] awk 求和
来源：http://kqn.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://gxq.hysaishi.cn

[R51] 排序去重取前几
来源：http://hww.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ecd.hysaishi.cn

[R52] 统计行数
来源：http://syx.pycfn.com

wc -l a.txt
来源：http://att.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://wga.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pxn.vehdjk.com

[R54] 比较两个文件
来源：http://bcv.xuanzx.com

diff a.txt b.txt
来源：http://dia.quarkkingdee.top

[R55] 压缩与解压
来源：http://vxc.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mja.shzxlz.cn

[R56] 远程拷贝
来源：http://nif.yj20258888.top

scp file user@host:/path/
来源：http://vhp.yfazqb.com

[R57] 远程执行命令
来源：http://tqs.haohaochexian.top

ssh user@host 'uptime'
来源：http://blf.nanxuanxn.top

[R58] 下载文件
来源：http://jre.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esy.zdbjq.cn

[R59] 发 POST JSON
来源：http://tkl.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mjg.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://hgv.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rwk.wangshuangyany.cn

[R61] 磁盘占用
来源：http://htt.hywenlv.cn

df -h;  du -sh *
来源：http://lsw.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://btq.pycfn.com

du -ah . | sort -rh | head -10
来源：http://xwb.mhx1999.top

[R63] 内存与进程
来源：http://fgb.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://lni.cdnleiting.top

[R64] 结束进程
来源：http://ndq.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://vww.nanxinkj.top

[R65] 查看端口占用
来源：http://rya.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wbv.nwbrower.top

[R66] 定时任务
来源：http://sxp.yvedp.cn

crontab -e;  crontab -l
来源：http://ovo.fzhhl.top

[R67] 生成随机十六进制串
来源：http://uyk.fktsv.cn

openssl rand -hex 16
来源：http://ilr.xziqi.cn

[R68] 计算文件校验值
来源：http://kmg.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ovq.gotoacloud.top

[R69] 生成随机密码
来源：http://iyv.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://rmb.zycfv.cn

[R70] 时间戳与互转
来源：http://mxp.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://oec.xuetiantiany.cn

[R71] 日期格式化
来源：http://zab.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ohs.meibo888.top

[R72] 等待端口就绪
来源：http://pgd.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axj.mhx1999.top

[R73] 分割大日志
来源：http://wim.sweek.top

split -l 1000 big.log part_
来源：http://ggo.yj20258.top

[R74] 批量重命名
来源：http://giq.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vnm.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://jqk.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://vil.ybcxt.top

[R76] 使用临时文件
来源：http://bkq.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jbt.ybcxt.top

[R77] 读取用户输入
来源：http://jhl.birdmap.top

read -rp "请输入: " ans
来源：http://psi.yj20258888.top

[R78] 交互式菜单
来源：http://yri.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://zxe.nanxinkj.top

[R79] 解析命令行选项
来源：http://chk.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ojf.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://cmr.guowangkeji.top

time ./run.sh
来源：http://oay.gaohongyu789.top

================================================================================
来源：http://lff.gzhubu.top

S. C / C++ 专题
来源：http://waz.9152youxi.cn

================================================================================
来源：http://oiv.ybcxt.top

[S01] C：Hello World
来源：http://kid.gotoacloud.top

#include <stdio.h>
来源：http://mks.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fhz.yfazqb.com

[S02] C：变量与格式化输出
来源：http://tja.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://dva.cucudq.cn

[S03] C：读入整数
来源：http://noo.tarul.cn

int x; scanf("%d", &x);
来源：http://urm.cashguo.top

[S04] C：字符串复制
来源：http://epd.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://vmb.daria6918.cn

[S05] C：字符串长度
来源：http://nze.ydjk.org.cn

strlen(s)
来源：http://wyp.chenzaomai.com

[S06] C：字符串比较
来源：http://jrj.pycfn.com

strcmp(a, b) == 0
来源：http://jdn.shuidangran.top

[S07] C：数组遍历求和
来源：http://xhk.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://koj.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://rzk.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rob.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://iqv.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://psh.yuanzhike.top

[S10] C：指针与解引用
来源：http://vmx.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://pvp.quarkkingdee.top

[S11] C：逐行读文件
来源：http://akq.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://ilj.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hud.jlsjyb.cn

fclose(f);
来源：http://osw.zdbjq.cn

[S12] C：写文件
来源：http://maq.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kpy.iojbl.cn

[S13] C：宏定义
来源：http://afk.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vav.xuetiantiany.cn

[S14] C：枚举
来源：http://xel.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://vfc.c1oappe.top

[S15] C：类型转换
来源：http://gpm.316326.xyz

(double) a / b
来源：http://aco.jlsjyb.cn

[S16] C：位操作置位
来源：http://tfk.zhongyouzk.top

x |= (1 << 3);
来源：http://isy.fzhhl.top

[S17] C：安全拼接字符串
来源：http://nyo.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pii.tian-w.cn

[S18] C：命令行参数
来源：http://nlc.hnxiangtu.top

int main(int argc, char **argv)
来源：http://wek.xuetiantiany.cn

[S19] C：快速排序
来源：http://qmg.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hfu.hcnkem.com

[S20] C：二分查找
来源：http://zba.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ome.mhx1999.top

[S21] C：字符类别判断
来源：http://hpb.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hsw.xinyue.icu

[S22] C：字符串转数字
来源：http://egs.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zzo.guowangkeji.top

[S23] C：随机数
来源：http://asx.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptu.redwolf501.top

[S24] C：获取本地时间
来源：http://nxv.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wgf.ybcxt.top

[S25] C：内存拷贝
来源：http://pfi.zdqjudy.top

memcpy(dst, src, n);
来源：http://auv.zhengqikj.top

[S26] C：内存清零
来源：http://spz.ivvv.top

memset(a, 0, sizeof a);
来源：http://iio.52xcode.cn

[S27] C：定义常量
来源：http://hwt.pycfn.com

const double PI = 3.14159;
来源：http://zvx.havefunace.top

[S28] C：静态变量
来源：http://tas.jqgufenzy.top

static int counter = 0;
来源：http://prn.uphjek.com

[S29] C：变参函数
来源：http://tyx.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mib.yueranfly.top

[S30] C：头文件保护
来源：http://sif.yj202588.top

#ifndef X_H
来源：http://wmc.316326.xyz

#define X_H
来源：http://zpf.yueranfly.top

#endif
来源：http://puo.shuidangran.top

[S31] C++：Hello World
来源：http://wzy.snrcjt.cn

#include <iostream>
来源：http://vaz.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://ktu.sjlbkw.cn

[S32] C++：字符串
来源：http://wah.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://inc.aizwys.cn

[S33] C++：vector 增删
来源：http://zqz.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cap.fehbvm.com

[S34] C++：遍历 vector
来源：http://kui.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://hur.jlsjyb.cn

[S35] C++：map
来源：http://arp.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lbf.yfazqb.com

[S36] C++：unordered_map
来源：http://gww.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dlu.52xcode.cn

[S37] C++：set
来源：http://obz.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://utl.52xcode.cn

[S38] C++：排序
来源：http://qmr.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://xix.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://cdb.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wmc.gogol.net.cn

[S40] C++：查找元素
来源：http://gix.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hfg.yfazqb.com

[S41] C++：类与构造函数
来源：http://bwx.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kvw.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://rud.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://cme.bjfxy.top

[S43] C++：智能指针
来源：http://kif.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://gsk.vqdsnc.cn

[S44] C++：引用传参
来源：http://yja.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://iqu.cucudq.cn

[S45] C++：lambda
来源：http://rpe.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://atr.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://qyh.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jem.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://lpv.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dgx.yfazqb.com

[S48] C++：逐行读文件
来源：http://phe.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ehw.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://twq.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://qus.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ewo.bjfxy.top

[S50] C++：格式化数字
来源：http://hps.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hji.nwbrower.top

[S51] C++：显式类型转换
来源：http://ekq.ybcxt.top

static_cast<double>(a) / b
来源：http://bxz.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://vga.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://osn.nanxuanxn.top

[S53] C++：移动语义
来源：http://msa.tanke756.top

std::vector<int> w = std::move(v);
来源：http://qcw.chenlongwang.top

[S54] C++：异常处理
来源：http://hne.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kfh.zhengqikj.top

[S55] C++：结构化绑定
来源：http://epz.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mfb.shanyushiyangtech.top

[S56] C++：optional
来源：http://ovj.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hwe.jinqigfzy.top

[S57] C++：编译期常量
来源：http://rus.guowangkeji.top

constexpr int N = 10;
来源：http://vco.jinqigfzy.top

[S58] C++：命名空间
来源：http://wqj.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://qop.xziqi.cn

[S59] C++：静态断言
来源：http://gph.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rbp.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://pvp.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wsa.fehbvm.com

================================================================================
来源：http://pdi.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qhc.zhaomingkeji.xyz

================================================================================
来源：http://dvd.cheryme.top

[T01] Kotlin：Hello World
来源：http://igo.fengsongda.top

println("Hello")
来源：http://urd.yangfankeji.com

[T02] Kotlin：变量
来源：http://gfu.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://djo.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://hzw.gzhubu.top

"值: $b"
来源：http://ayw.gogol.net.cn

[T04] Kotlin：空安全
来源：http://jcc.dianchejie.cn

val n: String? = null;  n?.length
来源：http://zgr.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://nkv.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://knz.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://kxx.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mzd.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://bap.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vhy.smart0.xyz

[T08] Kotlin：数据类
来源：http://qch.pycfn.com

data class User(val name: String, val age: Int)
来源：http://fum.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://zcf.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://hlr.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://fjm.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ppi.xylfe.cn

[T11] Kotlin：协程
来源：http://cfl.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mpz.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://nhu.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://ovo.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://ddi.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://ttw.ctjpmb.com

[T14] Kotlin：循环
来源：http://wzz.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://ekf.quarkkingdee.top

[T15] Kotlin：接口
来源：http://rld.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://swn.tarul.cn

[T16] Swift：Hello World
来源：http://enw.uphjek.com

print("Hello")
来源：http://qoe.yuxming.cn

[T17] Swift：变量与常量
来源：http://vfc.jyoumei.cn

var a = 1;  let b = 2
来源：http://zot.bbcook.cn

[T18] Swift：字符串插值
来源：http://inw.tanke756.top

"值: \(b)"
来源：http://zjl.ctjpmb.com

[T19] Swift：可选绑定
来源：http://hjd.sysykeji.top

if let n = opt { print(n) }
来源：http://oqs.hfpthk.cn

[T20] Swift：数组操作
来源：http://rok.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mcd.yangfankeji.com

[T21] Swift：遍历
来源：http://pqn.sufxvd.cn

for x in a { print(x) }
来源：http://jvs.shanyushiyangtech.top

[T22] Swift：字典
来源：http://sui.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://kga.jqgfzy.top

[T23] Swift：函数
来源：http://jhj.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pwh.zhongyouzk.top

[T24] Swift：闭包
来源：http://lyk.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pny.bjfxy.top

[T25] Swift：结构体
来源：http://daq.ctjpmb.com

struct P { var x: Int }
来源：http://mtq.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://cjz.svipenyu.cn

class A: Base { override func f() {} }
来源：http://rcn.zhixingplan.top

[T27] Swift：错误处理
来源：http://sii.meibo888.top

do { try f() } catch { print(error) }
来源：http://ihj.nanxuanxn.top

[T28] Swift：枚举
来源：http://dzc.yueranfly.top

enum Color { case red, green }
来源：http://sga.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://uvu.cucudq.cn

guard let x = opt else { return }
来源：http://soc.sxryk.cn

[T30] Swift：协议
来源：http://tzb.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://dlh.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://ruw.gotoacloud.top

print("Hello")
来源：http://qon.ppjwa.cn

[T32] Lua：局部变量
来源：http://vah.xingfuxueyuan.xyz

local a = 1
来源：http://zgv.mhx1999.top

[T33] Lua：表（数组）
来源：http://edu.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rac.guannengcc.top

[T34] Lua：遍历表
来源：http://viv.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://roq.tanke756.top

[T35] Lua：字典表
来源：http://omt.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://wlp.zhongyouzk.top

[T36] Lua：函数
来源：http://djs.mhx1999.top

function add(a, b) return a + b end
来源：http://iam.yj20258.top

[T37] Lua：字符串拼接
来源：http://seo.jinyuanbaomall.cn

"a" .. "b"
来源：http://ukb.pycfn.com

[T38] Lua：条件
来源：http://tvs.chenzaomai.com

if x > 0 then print("正") end
来源：http://gti.vehdjk.com

[T39] Lua：模式匹配
来源：http://klu.316326.xyz

string.find(s, "%d+")
来源：http://xfm.wangdashe.top

[T40] Lua：元表
来源：http://buc.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://uqf.gaohongyu789.top

[T41] Perl：Hello World
来源：http://ana.9152youxi.cn

print "Hello\n";
来源：http://gpq.xuanzx.com

[T42] Perl：变量类型
来源：http://kcl.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hjv.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://zyw.bjfxy.top

"值: $a"
来源：http://kiu.52xcode.cn

[T44] Perl：条件
来源：http://qau.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://rse.dashuyun.cn

[T45] Perl：数组遍历
来源：http://mdu.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://eek.hammf.cn

[T46] Perl：哈希操作
来源：http://vkf.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tip.birdmap.top

[T47] Perl：正则捕获
来源：http://iap.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vuq.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://hxi.tanke756.top

$s =~ s/old/new/g;
来源：http://uxl.iojbl.cn

[T49] Perl：函数
来源：http://auw.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jhs.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://mek.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dlc.fzhhl.top


<!-- 参考信息 -->