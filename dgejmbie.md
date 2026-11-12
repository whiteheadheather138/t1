代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://isq.hfpthk.cn

[R50] awk 求和
来源：http://xsq.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jlw.vqdsnc.cn

[R51] 排序去重取前几
来源：http://wwg.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://drr.hfpthk.cn

[R52] 统计行数
来源：http://lwz.havefunace.top

wc -l a.txt
来源：http://xzf.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://aig.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ymm.aizwys.cn

[R54] 比较两个文件
来源：http://vpv.yuanzhike.top

diff a.txt b.txt
来源：http://mbo.shuidangran.top

[R55] 压缩与解压
来源：http://kip.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vvw.316326.xyz

[R56] 远程拷贝
来源：http://koo.xylfe.cn

scp file user@host:/path/
来源：http://zkn.jinqigfzy.top

[R57] 远程执行命令
来源：http://uth.yuxming.cn

ssh user@host 'uptime'
来源：http://pdz.hammf.cn

[R58] 下载文件
来源：http://caj.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ubd.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://voa.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fyb.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://xbb.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jty.yuanzhike.top

[R61] 磁盘占用
来源：http://skd.sweek.top

df -h;  du -sh *
来源：http://kor.guowangkeji.top

[R62] 找最占空间的文件
来源：http://kwe.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://mjw.zhengqikj.top

[R63] 内存与进程
来源：http://ova.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://gir.yangfankeji.com

[R64] 结束进程
来源：http://qee.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://kgm.hywenlv.cn

[R65] 查看端口占用
来源：http://dwg.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wji.zhixingplan.top

[R66] 定时任务
来源：http://xya.pycfn.com

crontab -e;  crontab -l
来源：http://hat.fzhhl.top

[R67] 生成随机十六进制串
来源：http://mra.iojbl.cn

openssl rand -hex 16
来源：http://vuy.yj202588.top

[R68] 计算文件校验值
来源：http://wmk.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jfo.sufxvd.cn

[R69] 生成随机密码
来源：http://ksj.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://mgq.gotoacloud.top

[R70] 时间戳与互转
来源：http://nxh.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://ufh.tarul.cn

[R71] 日期格式化
来源：http://zgx.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://trh.chenzaomai.com

[R72] 等待端口就绪
来源：http://pqu.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fwb.jinqigfzy.top

[R73] 分割大日志
来源：http://nkn.zdqjudy.top

split -l 1000 big.log part_
来源：http://nzm.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://ydm.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zip.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://sjq.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://jgo.cashguo.top

[R76] 使用临时文件
来源：http://mpu.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lbg.vqdsnc.cn

[R77] 读取用户输入
来源：http://mwd.jianghu66.top

read -rp "请输入: " ans
来源：http://ybt.zhoulong.xyz

[R78] 交互式菜单
来源：http://utn.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rek.ctjpmb.com

[R79] 解析命令行选项
来源：http://yst.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hby.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://uen.zhengqikj.top

time ./run.sh
来源：http://cnr.snrcjt.cn

================================================================================
来源：http://ptb.cucudq.cn

S. C / C++ 专题
来源：http://ugg.yongpay.top

================================================================================
来源：http://ika.xinyue.icu

[S01] C：Hello World
来源：http://olq.nanxuanxn.top

#include <stdio.h>
来源：http://qig.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gdr.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://ocd.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://wqr.jqgfzy.top

[S03] C：读入整数
来源：http://vcj.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://geu.epnwcf.com

[S04] C：字符串复制
来源：http://tdk.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://dnr.zhixingplan.top

[S05] C：字符串长度
来源：http://rll.wangdashe.top

strlen(s)
来源：http://jhb.shuidangran.top

[S06] C：字符串比较
来源：http://lxi.gogol.net.cn

strcmp(a, b) == 0
来源：http://xeq.daria6918.cn

[S07] C：数组遍历求和
来源：http://fag.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xoo.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://uac.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nji.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://ymk.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oea.zycfv.cn

[S10] C：指针与解引用
来源：http://zyr.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://sdo.svipenyu.cn

[S11] C：逐行读文件
来源：http://xxw.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://tzh.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nxa.fanxiaobao.xyz

fclose(f);
来源：http://gyd.sjlbkw.cn

[S12] C：写文件
来源：http://kel.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gsv.dianchejie.cn

[S13] C：宏定义
来源：http://xqu.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqy.ybcxt.top

[S14] C：枚举
来源：http://dnn.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://iih.fengsongda.top

[S15] C：类型转换
来源：http://nyf.jianghu66.top

(double) a / b
来源：http://hqy.chenlongwang.top

[S16] C：位操作置位
来源：http://loc.nanxinkj.top

x |= (1 << 3);
来源：http://bkc.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://ymh.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ieu.hnqzz.top

[S18] C：命令行参数
来源：http://zui.c1oappe.top

int main(int argc, char **argv)
来源：http://dvw.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://tet.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://ppm.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://uox.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qqi.snrcjt.cn

[S21] C：字符类别判断
来源：http://mzr.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://beb.yonumen.top

[S22] C：字符串转数字
来源：http://uss.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://zox.hfpthk.cn

[S23] C：随机数
来源：http://vfz.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fua.wangdashe.top

[S24] C：获取本地时间
来源：http://syj.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bdu.tian-w.cn

[S25] C：内存拷贝
来源：http://mny.guowangkeji.top

memcpy(dst, src, n);
来源：http://hpy.yuxming.cn

[S26] C：内存清零
来源：http://cny.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://ozp.yj20258888.top

[S27] C：定义常量
来源：http://icr.yfazqb.com

const double PI = 3.14159;
来源：http://ptg.zhiwuduotai.top

[S28] C：静态变量
来源：http://vcc.yj20258888.top

static int counter = 0;
来源：http://ugn.jinqigfzy.top

[S29] C：变参函数
来源：http://ilt.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kta.jianghu66.top

[S30] C：头文件保护
来源：http://iok.ywan-chungtsiang.top

#ifndef X_H
来源：http://qdm.316326.xyz

#define X_H
来源：http://bso.yangfankeji.com

#endif
来源：http://adi.havefunace.top

[S31] C++：Hello World
来源：http://yrq.jianghu66.top

#include <iostream>
来源：http://ton.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://rby.xylfe.cn

[S32] C++：字符串
来源：http://yhr.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://kmi.epnwcf.com

[S33] C++：vector 增删
来源：http://aaf.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ygo.ctjpmb.com

[S34] C++：遍历 vector
来源：http://hdv.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://uwz.sysykeji.top

[S35] C++：map
来源：http://jku.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tjy.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://uqk.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gcl.yj20258888.top

[S37] C++：set
来源：http://csx.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gvk.jyoumei.cn

[S38] C++：排序
来源：http://iyi.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://oty.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://gzy.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ugl.svipenyu.cn

[S40] C++：查找元素
来源：http://fqv.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wtq.haohaochexian.top

[S41] C++：类与构造函数
来源：http://qnv.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kri.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://zyi.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://mpa.svipenyu.cn

[S43] C++：智能指针
来源：http://tml.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://mah.havefunace.top

[S44] C++：引用传参
来源：http://tmt.iojbl.cn

void inc(int &x) { ++x; }
来源：http://nqs.yvedp.cn

[S45] C++：lambda
来源：http://ivr.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wqq.hysaishi.cn

[S46] C++：函数模板
来源：http://cjh.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://web.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://zld.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngn.guannengcc.top

[S48] C++：逐行读文件
来源：http://mxj.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://gxp.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://uny.yuxming.cn

[S49] C++：写文件
来源：http://qds.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ecg.meibo888.top

[S50] C++：格式化数字
来源：http://hwj.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bog.yuanzhike.top

[S51] C++：显式类型转换
来源：http://mqs.uphjek.com

static_cast<double>(a) / b
来源：http://fls.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://hnx.nwbrower.top

int size() const noexcept { return n_; }
来源：http://did.52xcode.cn

[S53] C++：移动语义
来源：http://sxz.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://npu.tanke756.top

[S54] C++：异常处理
来源：http://rix.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzf.dianchejie.cn

[S55] C++：结构化绑定
来源：http://qny.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qrh.xuanzx.com

[S56] C++：optional
来源：http://ltt.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qza.ydjk.org.cn

[S57] C++：编译期常量
来源：http://cux.yuanzhike.top

constexpr int N = 10;
来源：http://ymr.hnqzz.top

[S58] C++：命名空间
来源：http://wpk.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://xzw.zhongyouzk.top

[S59] C++：静态断言
来源：http://afu.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mqg.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://hgp.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cfy.guowangkeji.top

================================================================================
来源：http://jsl.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://amh.ctjpmb.com

================================================================================
来源：http://yto.aizwys.cn

[T01] Kotlin：Hello World
来源：http://erm.yj202588.top

println("Hello")
来源：http://upa.hysaishi.cn

[T02] Kotlin：变量
来源：http://gom.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pxg.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://mih.hcnkem.com

"值: $b"
来源：http://ajt.epnwcf.com

[T04] Kotlin：空安全
来源：http://fqf.yj20258.top

val n: String? = null;  n?.length
来源：http://iys.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://qot.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://teh.yongpay.top

[T06] Kotlin：集合映射
来源：http://zqb.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ylx.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://bfc.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nke.gogol.net.cn

[T08] Kotlin：数据类
来源：http://tko.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://uqh.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://mxd.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://xyl.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://iyk.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cpo.fzhhl.top

[T11] Kotlin：协程
来源：http://tqq.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bkf.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://xhx.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://lgi.yj20258.top

[T13] Kotlin：只读 Map
来源：http://okt.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://dmy.hcnkem.com

[T14] Kotlin：循环
来源：http://dji.cdnleiting.top

for (i in 1..10) println(i)
来源：http://qpi.fehbvm.com

[T15] Kotlin：接口
来源：http://ovv.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://jis.tian-w.cn

[T16] Swift：Hello World
来源：http://shj.cqqwz.cn

print("Hello")
来源：http://jxc.cqqwz.cn

[T17] Swift：变量与常量
来源：http://jbe.yongpay.top

var a = 1;  let b = 2
来源：http://aky.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://mma.yuanzhike.top

"值: \(b)"
来源：http://qvr.guowangkeji.top

[T19] Swift：可选绑定
来源：http://opx.pycfn.com

if let n = opt { print(n) }
来源：http://gsc.zhijiandao.cn

[T20] Swift：数组操作
来源：http://agx.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://pdt.zhoulong.xyz

[T21] Swift：遍历
来源：http://xby.hnqzz.top

for x in a { print(x) }
来源：http://jlf.gotoacloud.top

[T22] Swift：字典
来源：http://dxz.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xbs.daria6918.cn

[T23] Swift：函数
来源：http://uqq.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://znq.dashuyun.cn

[T24] Swift：闭包
来源：http://bal.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tcn.gotoacloud.top

[T25] Swift：结构体
来源：http://bjw.quarkkingdee.top

struct P { var x: Int }
来源：http://myo.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://cqr.bjfxy.top

class A: Base { override func f() {} }
来源：http://bay.hammf.cn

[T27] Swift：错误处理
来源：http://pij.xuanzx.com

do { try f() } catch { print(error) }
来源：http://bxm.sufxvd.cn

[T28] Swift：枚举
来源：http://cdl.ppjwa.cn

enum Color { case red, green }
来源：http://nmy.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://udo.ctjpmb.com

guard let x = opt else { return }
来源：http://fcb.tarul.cn

[T30] Swift：协议
来源：http://nvq.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://obc.vehdjk.com

[T31] Lua：Hello World
来源：http://fio.yangfankeji.com

print("Hello")
来源：http://lww.uphjek.com

[T32] Lua：局部变量
来源：http://xjv.redwolf501.top

local a = 1
来源：http://xje.jqgfzy.top

[T33] Lua：表（数组）
来源：http://bzo.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://bqm.shuidangran.top

[T34] Lua：遍历表
来源：http://plp.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://lkj.ppjwa.cn

[T35] Lua：字典表
来源：http://mkz.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://xib.cashguo.top

[T36] Lua：函数
来源：http://ysi.yuanzhike.top

function add(a, b) return a + b end
来源：http://sho.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://jgp.vqdsnc.cn

"a" .. "b"
来源：http://njg.daxiang520.top

[T38] Lua：条件
来源：http://sjj.yuxming.cn

if x > 0 then print("正") end
来源：http://tox.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://hhq.gogol.net.cn

string.find(s, "%d+")
来源：http://rwm.quarkkingdee.top

[T40] Lua：元表
来源：http://zle.meibo888.top

setmetatable({}, { __index = base })
来源：http://xfk.xziqi.cn

[T41] Perl：Hello World
来源：http://geb.shzxlz.cn

print "Hello\n";
来源：http://dgt.meibo888.top

[T42] Perl：变量类型
来源：http://qvr.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xzj.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://ick.sufxvd.cn

"值: $a"
来源：http://zjd.jqgufenzy.top

[T44] Perl：条件
来源：http://zie.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://kqk.ybcxt.top

[T45] Perl：数组遍历
来源：http://nig.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://lfc.ivvv.top

[T46] Perl：哈希操作
来源：http://bkf.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mcw.fktsv.cn

[T47] Perl：正则捕获
来源：http://yrh.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mil.nwbrower.top

[T48] Perl：正则替换
来源：http://jna.pycfn.com

$s =~ s/old/new/g;
来源：http://niv.kuanghao11.cn

[T49] Perl：函数
来源：http://bvu.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://noe.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://sli.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yqd.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://qzj.sweek.top

[T51] Scala：Hello World
来源：http://ejw.tianlin.xyz

println("Hello")
来源：http://urs.shzxlz.cn

[T52] Scala：变量
来源：http://ziy.quarkkingdee.top


<!-- 参考信息 -->