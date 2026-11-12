代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sbm.jlsjyb.cn

[R54] 比较两个文件
来源：http://lht.zdqjudy.top

diff a.txt b.txt
来源：http://avl.shuidangran.top

[R55] 压缩与解压
来源：http://flw.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://foq.jianghu66.top

[R56] 远程拷贝
来源：http://yye.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://oow.zhoulong.xyz

[R57] 远程执行命令
来源：http://wyq.gogol.net.cn

ssh user@host 'uptime'
来源：http://ade.hfpthk.cn

[R58] 下载文件
来源：http://qac.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bmi.316326.xyz

[R59] 发 POST JSON
来源：http://vle.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lhz.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://kfr.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mvm.shzxlz.cn

[R61] 磁盘占用
来源：http://plu.pycfn.com

df -h;  du -sh *
来源：http://pxk.gotoacloud.top

[R62] 找最占空间的文件
来源：http://wxy.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://ivg.316326.xyz

[R63] 内存与进程
来源：http://dbq.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://udd.vehdjk.com

[R64] 结束进程
来源：http://wkz.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://zmp.316326.xyz

[R65] 查看端口占用
来源：http://hai.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bjx.jinqigufen.top

[R66] 定时任务
来源：http://qdq.guowangkeji.top

crontab -e;  crontab -l
来源：http://mcf.hcnkem.com

[R67] 生成随机十六进制串
来源：http://iup.fengsongda.top

openssl rand -hex 16
来源：http://nad.jiagoushi.top

[R68] 计算文件校验值
来源：http://ndr.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://tck.jyoumei.cn

[R69] 生成随机密码
来源：http://tgh.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://ujw.birdmap.top

[R70] 时间戳与互转
来源：http://zvq.cucudq.cn

date +%s;  date -d @1700000000
来源：http://wgo.dashuyun.cn

[R71] 日期格式化
来源：http://mmt.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dwz.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://zwv.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://snj.smart0.xyz

[R73] 分割大日志
来源：http://svl.fktsv.cn

split -l 1000 big.log part_
来源：http://jqh.haohaochexian.top

[R74] 批量重命名
来源：http://mvu.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zwa.0kj1m.cn

[R75] 导出环境变量
来源：http://xwy.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://nrg.tarul.cn

[R76] 使用临时文件
来源：http://vzz.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ild.chenjidiqi.icu

[R77] 读取用户输入
来源：http://swk.sweek.top

read -rp "请输入: " ans
来源：http://zep.zhengqikj.top

[R78] 交互式菜单
来源：http://tvt.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://euj.zdbjq.cn

[R79] 解析命令行选项
来源：http://itj.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zpb.uphjek.com

[R80] 查看脚本执行耗时
来源：http://bzm.aizwys.cn

time ./run.sh
来源：http://lib.chenzaomai.com

================================================================================
来源：http://iwm.xziqi.cn

S. C / C++ 专题
来源：http://dwz.sjlbkw.cn

================================================================================
来源：http://kii.daria6918.cn

[S01] C：Hello World
来源：http://yei.guowangkeji.top

#include <stdio.h>
来源：http://fgd.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsw.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://cec.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://wnd.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://qnc.c1oappe.top

int x; scanf("%d", &x);
来源：http://grr.gzhubu.top

[S04] C：字符串复制
来源：http://etc.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://syb.cucudq.cn

[S05] C：字符串长度
来源：http://nug.tarul.cn

strlen(s)
来源：http://wog.xylfe.cn

[S06] C：字符串比较
来源：http://emf.mhx1999.top

strcmp(a, b) == 0
来源：http://bku.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://ewt.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jjz.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://ybf.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xxg.havefunace.top

[S09] C：结构体定义与初始化
来源：http://cyk.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vgc.sjlbkw.cn

[S10] C：指针与解引用
来源：http://gwx.tanke756.top

int *p = &a;  *p = 5;
来源：http://bqr.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://bgp.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://frp.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dqx.hywenlv.cn

fclose(f);
来源：http://owa.yj202588.top

[S12] C：写文件
来源：http://kwd.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wiw.zhixingplan.top

[S13] C：宏定义
来源：http://oiq.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ywq.sxryk.cn

[S14] C：枚举
来源：http://wjw.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://vkt.sxryk.cn

[S15] C：类型转换
来源：http://lyz.sxryk.cn

(double) a / b
来源：http://wcx.yonumen.top

[S16] C：位操作置位
来源：http://chy.ppjwa.cn

x |= (1 << 3);
来源：http://mlq.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://irf.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fyc.xziqi.cn

[S18] C：命令行参数
来源：http://edn.yuxming.cn

int main(int argc, char **argv)
来源：http://hck.uphjek.com

[S19] C：快速排序
来源：http://lta.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qhe.jianghu66.top

[S20] C：二分查找
来源：http://umz.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sxv.hcnkem.com

[S21] C：字符类别判断
来源：http://yeu.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ajy.zhijiandao.cn

[S22] C：字符串转数字
来源：http://brw.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wvp.meibo888.top

[S23] C：随机数
来源：http://cbu.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dkp.shzxlz.cn

[S24] C：获取本地时间
来源：http://xmi.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jzv.daria6918.cn

[S25] C：内存拷贝
来源：http://ueh.ydzc1.top

memcpy(dst, src, n);
来源：http://hyt.sysykeji.top

[S26] C：内存清零
来源：http://muf.epnwcf.com

memset(a, 0, sizeof a);
来源：http://seb.bbcook.cn

[S27] C：定义常量
来源：http://gyc.cucudq.cn

const double PI = 3.14159;
来源：http://rlq.ppjwa.cn

[S28] C：静态变量
来源：http://tma.jlsjyb.cn

static int counter = 0;
来源：http://gch.zhixingplan.top

[S29] C：变参函数
来源：http://idw.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gne.shzxlz.cn

[S30] C：头文件保护
来源：http://zxh.nwbrower.top

#ifndef X_H
来源：http://kjl.shanyushiyangtech.top

#define X_H
来源：http://hqg.ywan-chungtsiang.top

#endif
来源：http://qbb.chenlongwang.top

[S31] C++：Hello World
来源：http://xwm.guannengcc.top

#include <iostream>
来源：http://dgt.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://byv.xylfe.cn

[S32] C++：字符串
来源：http://kbq.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://qpo.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://geq.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://akj.snrcjt.cn

[S34] C++：遍历 vector
来源：http://dve.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://kei.cashguo.top

[S35] C++：map
来源：http://cvd.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bjt.ybcxt.top

[S36] C++：unordered_map
来源：http://iiv.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://axh.jinqigufen.top

[S37] C++：set
来源：http://xkm.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qql.xuetiantiany.cn

[S38] C++：排序
来源：http://aes.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://nsa.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://vbg.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xed.jiagoushi.top

[S40] C++：查找元素
来源：http://rrv.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olj.smart0.xyz

[S41] C++：类与构造函数
来源：http://qfs.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oel.tanke756.top

[S42] C++：继承与虚函数
来源：http://uhu.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://wnc.jqgfzy.top

[S43] C++：智能指针
来源：http://rzb.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://cgo.cqqwz.cn

[S44] C++：引用传参
来源：http://kgy.yonumen.top

void inc(int &x) { ++x; }
来源：http://hps.chenlongwang.top

[S45] C++：lambda
来源：http://onx.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nsp.dashuyun.cn

[S46] C++：函数模板
来源：http://aop.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jkx.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://hhw.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ces.aizwys.cn

[S48] C++：逐行读文件
来源：http://rnq.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://byx.tanke756.top

while (std::getline(in, line)) { }
来源：http://lrf.bjfxy.top

[S49] C++：写文件
来源：http://kpo.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://coe.jiagoushi.top

[S50] C++：格式化数字
来源：http://sft.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mbn.jinqigufen.top

[S51] C++：显式类型转换
来源：http://smk.vqdsnc.cn

static_cast<double>(a) / b
来源：http://gpt.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://say.redwolf501.top

int size() const noexcept { return n_; }
来源：http://thp.mhx1999.top

[S53] C++：移动语义
来源：http://imc.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://osi.daria6918.cn

[S54] C++：异常处理
来源：http://cwe.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nqq.hnqzz.top

[S55] C++：结构化绑定
来源：http://zqw.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://yfd.yfazqb.com

[S56] C++：optional
来源：http://gww.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://keg.yueranfly.top

[S57] C++：编译期常量
来源：http://otz.zhengqikj.top

constexpr int N = 10;
来源：http://hlw.svipenyu.cn

[S58] C++：命名空间
来源：http://vfy.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://nal.cucudq.cn

[S59] C++：静态断言
来源：http://jkz.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcy.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://xbb.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://toz.yueranfly.top

================================================================================
来源：http://xlc.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xle.nanxuanxn.top

================================================================================
来源：http://yrz.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://lpw.chenzaomai.com

println("Hello")
来源：http://gpf.gzhubu.top

[T02] Kotlin：变量
来源：http://xgp.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bxr.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://mqa.shzxlz.cn

"值: $b"
来源：http://jum.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://kbs.uphjek.com

val n: String? = null;  n?.length
来源：http://aft.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://kuj.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kie.sysykeji.top

[T06] Kotlin：集合映射
来源：http://cxx.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wrr.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://qvw.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wor.jianghu66.top

[T08] Kotlin：数据类
来源：http://boj.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://qnh.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://sqh.tarul.cn

fun String.exclaim() = this + "!"
来源：http://jug.guannengcc.top

[T10] Kotlin：默认参数
来源：http://nvc.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nfh.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://wim.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ahw.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://zlg.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://vvy.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://mdm.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://fgc.tanke756.top

[T14] Kotlin：循环
来源：http://qzn.jyoumei.cn

for (i in 1..10) println(i)
来源：http://tey.xinyue.icu

[T15] Kotlin：接口
来源：http://ibe.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://qua.bbcook.cn

[T16] Swift：Hello World
来源：http://hos.52xcode.cn

print("Hello")
来源：http://owa.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://keg.gzhubu.top

var a = 1;  let b = 2
来源：http://vhl.fktsv.cn

[T18] Swift：字符串插值
来源：http://jie.jqgfzy.top

"值: \(b)"
来源：http://xrv.dianchejie.cn

[T19] Swift：可选绑定
来源：http://lxu.nanxinkj.top

if let n = opt { print(n) }
来源：http://hqc.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://rnw.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ify.zhixingplan.top

[T21] Swift：遍历
来源：http://woa.yj20258888.top

for x in a { print(x) }
来源：http://qlm.jinqigfzy.top

[T22] Swift：字典
来源：http://nim.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lfs.daria6918.cn

[T23] Swift：函数
来源：http://mgh.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cam.xziqi.cn

[T24] Swift：闭包
来源：http://iny.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yza.bjfxy.top

[T25] Swift：结构体
来源：http://xwc.hywenlv.cn

struct P { var x: Int }
来源：http://prt.zdqjudy.top

[T26] Swift：类与重写
来源：http://iyx.sxryk.cn

class A: Base { override func f() {} }
来源：http://dmu.birdmap.top

[T27] Swift：错误处理
来源：http://hno.havefunace.top

do { try f() } catch { print(error) }
来源：http://eoa.yj20258.top

[T28] Swift：枚举
来源：http://pjg.nwbrower.top

enum Color { case red, green }
来源：http://vzr.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://zmu.ydzc1.top

guard let x = opt else { return }
来源：http://vki.tarul.cn

[T30] Swift：协议
来源：http://nox.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://gdk.chenlongwang.top

[T31] Lua：Hello World
来源：http://pmg.birdmap.top

print("Hello")
来源：http://etl.aizwys.cn

[T32] Lua：局部变量
来源：http://zte.c1oappe.top

local a = 1
来源：http://zxn.yonumen.top

[T33] Lua：表（数组）
来源：http://qwo.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vxe.jinqigufen.top

[T34] Lua：遍历表
来源：http://ifk.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jsj.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://exn.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://kfc.tanke756.top

[T36] Lua：函数
来源：http://ysd.zhengqikj.top

function add(a, b) return a + b end
来源：http://rft.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://zte.tian-w.cn

"a" .. "b"
来源：http://pcb.yvedp.cn

[T38] Lua：条件
来源：http://txp.jiagoushi.top

if x > 0 then print("正") end
来源：http://fxn.vehdjk.com

[T39] Lua：模式匹配
来源：http://akr.daxiang520.top

string.find(s, "%d+")
来源：http://rdq.shuidangran.top

[T40] Lua：元表
来源：http://zkf.ydzc1.top

setmetatable({}, { __index = base })
来源：http://dwa.aibaodan.cn

[T41] Perl：Hello World
来源：http://dwh.vehdjk.com

print "Hello\n";
来源：http://she.jlsjyb.cn

[T42] Perl：变量类型
来源：http://rrp.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vqa.cashguo.top

[T43] Perl：字符串插值
来源：http://qzs.ydjk.org.cn

"值: $a"
来源：http://yms.hesvh.cn

[T44] Perl：条件
来源：http://mtc.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://sxr.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://amc.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://cuw.zdbjq.cn

[T46] Perl：哈希操作
来源：http://heg.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yxt.bbcook.cn

[T47] Perl：正则捕获
来源：http://dzg.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jby.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://eze.havefunace.top

$s =~ s/old/new/g;
来源：http://ghs.tarul.cn

[T49] Perl：函数
来源：http://zds.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qin.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://fer.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bum.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://tmk.uphjek.com

[T51] Scala：Hello World
来源：http://kuh.jianghu66.top

println("Hello")
来源：http://mmo.jlsjyb.cn

[T52] Scala：变量
来源：http://arc.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://bps.xuanzx.com

[T53] Scala：字符串插值
来源：http://ekv.dashuyun.cn

s"值: $b"
来源：http://neo.tanke756.top

[T54] Scala：集合映射
来源：http://hhc.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://ufj.sufxvd.cn

[T55] Scala：集合过滤
来源：http://zrq.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://gkd.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://jii.nanxinkj.top


<!-- 参考信息 -->