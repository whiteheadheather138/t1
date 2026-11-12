代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ais.feifeiyinyue.top

[R54] 比较两个文件
来源：http://tfi.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://dnq.xuanzx.com

[R55] 压缩与解压
来源：http://xeg.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vju.shangyingyoupin.top

[R56] 远程拷贝
来源：http://lov.hongshengwenyu.top

scp file user@host:/path/
来源：http://ckr.hongshengwenyu.top

[R57] 远程执行命令
来源：http://ton.zhixingplan.top

ssh user@host 'uptime'
来源：http://eol.xuanzx.com

[R58] 下载文件
来源：http://vex.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jup.tian-w.cn

[R59] 发 POST JSON
来源：http://hom.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvu.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://teu.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hjq.nwbrower.top

[R61] 磁盘占用
来源：http://pcc.yj20258888.top

df -h;  du -sh *
来源：http://jwf.haohaochexian.top

[R62] 找最占空间的文件
来源：http://yoi.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://mjg.cqqwz.cn

[R63] 内存与进程
来源：http://zyo.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://iei.sweek.top

[R64] 结束进程
来源：http://dzy.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://qbz.tianlin.xyz

[R65] 查看端口占用
来源：http://hyc.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zoc.cashguo.top

[R66] 定时任务
来源：http://ywr.hfpthk.cn

crontab -e;  crontab -l
来源：http://lmu.c1oappe.top

[R67] 生成随机十六进制串
来源：http://ink.ivvv.top

openssl rand -hex 16
来源：http://bdb.bbcook.cn

[R68] 计算文件校验值
来源：http://slj.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://yri.xuanzx.com

[R69] 生成随机密码
来源：http://opm.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://tyq.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://yyz.gzhubu.top

date +%s;  date -d @1700000000
来源：http://luz.haohaochexian.top

[R71] 日期格式化
来源：http://fed.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jhh.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://wdx.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qvn.ctjpmb.com

[R73] 分割大日志
来源：http://opa.tianlin.xyz

split -l 1000 big.log part_
来源：http://eiq.yanxiufei.cn

[R74] 批量重命名
来源：http://qfy.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xov.shangyingyoupin.top

[R75] 导出环境变量
来源：http://chn.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://xdg.jinqigufen.top

[R76] 使用临时文件
来源：http://eek.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tnl.iojbl.cn

[R77] 读取用户输入
来源：http://zed.redwolf501.top

read -rp "请输入: " ans
来源：http://ybw.vehdjk.com

[R78] 交互式菜单
来源：http://woj.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eye.yj20258888.top

[R79] 解析命令行选项
来源：http://xaq.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uam.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://gyi.ywan-chungtsiang.top

time ./run.sh
来源：http://rbk.quarkkingdee.top

================================================================================
来源：http://hre.ehwqpu.com

S. C / C++ 专题
来源：http://qvi.yj20258.top

================================================================================
来源：http://qlb.xziqi.cn

[S01] C：Hello World
来源：http://ilv.jqgufenzy.top

#include <stdio.h>
来源：http://hem.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vdt.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://fae.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://mff.316326.xyz

[S03] C：读入整数
来源：http://syx.sysykeji.top

int x; scanf("%d", &x);
来源：http://jrh.sjlbkw.cn

[S04] C：字符串复制
来源：http://uwj.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jho.hywenlv.cn

[S05] C：字符串长度
来源：http://tdp.316326.xyz

strlen(s)
来源：http://iqz.yj20258888.top

[S06] C：字符串比较
来源：http://sfz.ydzc1.top

strcmp(a, b) == 0
来源：http://fms.vehdjk.com

[S07] C：数组遍历求和
来源：http://crx.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xwl.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://rvm.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cua.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://vfa.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ggs.gaohongyu789.top

[S10] C：指针与解引用
来源：http://iya.havefunace.top

int *p = &a;  *p = 5;
来源：http://hhb.yj202588.top

[S11] C：逐行读文件
来源：http://nif.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://xki.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oyk.shanyushiyangtech.top

fclose(f);
来源：http://ecc.vqdsnc.cn

[S12] C：写文件
来源：http://csf.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpe.cashguo.top

[S13] C：宏定义
来源：http://gmj.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wyy.havefunace.top

[S14] C：枚举
来源：http://xix.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://mxq.pycfn.com

[S15] C：类型转换
来源：http://scw.quarkkingdee.top

(double) a / b
来源：http://duv.havefunace.top

[S16] C：位操作置位
来源：http://giq.meibo888.top

x |= (1 << 3);
来源：http://fnc.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://zdw.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oem.hfpthk.cn

[S18] C：命令行参数
来源：http://yqc.ydjk.org.cn

int main(int argc, char **argv)
来源：http://psh.ydzc1.top

[S19] C：快速排序
来源：http://kzt.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://omk.ctjpmb.com

[S20] C：二分查找
来源：http://jkz.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://apo.guannengcc.top

[S21] C：字符类别判断
来源：http://jtn.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jgc.c1oappe.top

[S22] C：字符串转数字
来源：http://yci.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kfg.uphjek.com

[S23] C：随机数
来源：http://tzd.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vwj.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://aux.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gxb.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://paw.ppjwa.cn

memcpy(dst, src, n);
来源：http://aoe.vqdsnc.cn

[S26] C：内存清零
来源：http://jto.bjfxy.top

memset(a, 0, sizeof a);
来源：http://dup.bbcook.cn

[S27] C：定义常量
来源：http://hvg.mhx1999.top

const double PI = 3.14159;
来源：http://ifc.jianghu66.top

[S28] C：静态变量
来源：http://rzc.snrcjt.cn

static int counter = 0;
来源：http://tmh.zhijiandao.cn

[S29] C：变参函数
来源：http://lcg.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://det.yvedp.cn

[S30] C：头文件保护
来源：http://dfi.yueranfly.top

#ifndef X_H
来源：http://vxz.chenzaomai.com

#define X_H
来源：http://kfg.shanyushiyangtech.top

#endif
来源：http://osw.yongpay.top

[S31] C++：Hello World
来源：http://bmd.haohaochexian.top

#include <iostream>
来源：http://imw.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://cuh.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://zjm.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://fmo.yanxiufei.cn

[S33] C++：vector 增删
来源：http://aya.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sks.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://xeu.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gqj.zhaomingkeji.xyz

[S35] C++：map
来源：http://bfj.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hhr.hywenlv.cn

[S36] C++：unordered_map
来源：http://wxv.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://egg.guannengcc.top

[S37] C++：set
来源：http://rnl.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://doh.ybcxt.top

[S38] C++：排序
来源：http://nkj.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://nzh.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://cea.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://art.hfpthk.cn

[S40] C++：查找元素
来源：http://hot.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxe.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://pil.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vqs.jianghu66.top

[S42] C++：继承与虚函数
来源：http://ors.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://roa.pengpengdd.cyou

[S43] C++：智能指针
来源：http://pdu.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://lfg.yueranfly.top

[S44] C++：引用传参
来源：http://vhy.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://ysp.fktsv.cn

[S45] C++：lambda
来源：http://ymc.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kjn.daxiang520.top

[S46] C++：函数模板
来源：http://hww.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://htc.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://fhu.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hrb.guannengcc.top

[S48] C++：逐行读文件
来源：http://zyw.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://ikt.sysykeji.top

while (std::getline(in, line)) { }
来源：http://fee.zhiwuduotai.top

[S49] C++：写文件
来源：http://kls.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xmg.aibaodan.cn

[S50] C++：格式化数字
来源：http://zbs.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uym.hnqzz.top

[S51] C++：显式类型转换
来源：http://iiq.ybcxt.top

static_cast<double>(a) / b
来源：http://nio.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://lvd.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://mpb.fktsv.cn

[S53] C++：移动语义
来源：http://yxe.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://ybm.vehdjk.com

[S54] C++：异常处理
来源：http://ydr.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qoo.jqgfzy.top

[S55] C++：结构化绑定
来源：http://utv.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qbu.tianlin.xyz

[S56] C++：optional
来源：http://szr.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://osg.316326.xyz

[S57] C++：编译期常量
来源：http://hwv.hywenlv.cn

constexpr int N = 10;
来源：http://yip.sxryk.cn

[S58] C++：命名空间
来源：http://wcc.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://czj.bbcook.cn

[S59] C++：静态断言
来源：http://gmx.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hdr.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://egs.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pnj.cashguo.top

================================================================================
来源：http://yjo.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpx.ppjwa.cn

================================================================================
来源：http://tca.wangdashe.top

[T01] Kotlin：Hello World
来源：http://rbf.xuanzx.com

println("Hello")
来源：http://tpy.zhixingplan.top

[T02] Kotlin：变量
来源：http://fpq.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://izw.havefunace.top

[T03] Kotlin：字符串模板
来源：http://hog.yuxming.cn

"值: $b"
来源：http://iwa.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://xky.fktsv.cn

val n: String? = null;  n?.length
来源：http://oaz.sweek.top

[T05] Kotlin：when 表达式
来源：http://leb.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fvm.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://atb.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qbr.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://jms.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xjy.ivvv.top

[T08] Kotlin：数据类
来源：http://qzv.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://wdf.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://pyr.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://lzw.sysykeji.top

[T10] Kotlin：默认参数
来源：http://dth.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ppz.xuanzx.com

[T11] Kotlin：协程
来源：http://lee.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://acl.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://pif.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://hae.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://ssy.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://klp.jyoumei.cn

[T14] Kotlin：循环
来源：http://sxk.jqgfzy.top

for (i in 1..10) println(i)
来源：http://qkh.316326.xyz

[T15] Kotlin：接口
来源：http://jyi.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://cjw.hesvh.cn

[T16] Swift：Hello World
来源：http://fkd.hammf.cn

print("Hello")
来源：http://ngs.dianchejie.cn

[T17] Swift：变量与常量
来源：http://zyw.fehbvm.com

var a = 1;  let b = 2
来源：http://dld.xinyue.icu

[T18] Swift：字符串插值
来源：http://afn.kuanghao11.cn

"值: \(b)"
来源：http://ixx.sysykeji.top

[T19] Swift：可选绑定
来源：http://eqo.yj20258888.top

if let n = opt { print(n) }
来源：http://exj.jlsjyb.cn

[T20] Swift：数组操作
来源：http://gbc.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://yue.iojbl.cn

[T21] Swift：遍历
来源：http://gka.jinghuilouyu.cn

for x in a { print(x) }
来源：http://ffk.tanke756.top

[T22] Swift：字典
来源：http://mcc.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vmy.hywenlv.cn

[T23] Swift：函数
来源：http://etq.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ahs.xuetiantiany.cn

[T24] Swift：闭包
来源：http://faw.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsp.hnqzz.top

[T25] Swift：结构体
来源：http://ncw.52xcode.cn

struct P { var x: Int }
来源：http://doi.cucudq.cn

[T26] Swift：类与重写
来源：http://fwe.wangdashe.top

class A: Base { override func f() {} }
来源：http://pbx.bjfxy.top

[T27] Swift：错误处理
来源：http://fan.bjfxy.top

do { try f() } catch { print(error) }
来源：http://ugx.haohaochexian.top

[T28] Swift：枚举
来源：http://yth.xinyue.icu

enum Color { case red, green }
来源：http://erx.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://gjv.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://jtk.zhoulong.xyz

[T30] Swift：协议
来源：http://xbo.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://rbd.c1oappe.top

[T31] Lua：Hello World
来源：http://opu.chenlongwang.top

print("Hello")
来源：http://zkc.yuanzhike.top

[T32] Lua：局部变量
来源：http://mcd.quarkkingdee.top

local a = 1
来源：http://osy.316326.xyz

[T33] Lua：表（数组）
来源：http://wci.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ugb.ybcxt.top

[T34] Lua：遍历表
来源：http://rob.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ztp.yangfankeji.com

[T35] Lua：字典表
来源：http://hrk.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://dkg.hongshengwenyu.top

[T36] Lua：函数
来源：http://zge.svipenyu.cn

function add(a, b) return a + b end
来源：http://zik.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://smj.zhaomingkeji.xyz

"a" .. "b"
来源：http://nyp.haohaochexian.top

[T38] Lua：条件
来源：http://clp.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://ofq.xinyue.icu

[T39] Lua：模式匹配
来源：http://mps.hammf.cn

string.find(s, "%d+")
来源：http://gnw.zhengqikj.top

[T40] Lua：元表
来源：http://siu.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://kkh.jiagoushi.top

[T41] Perl：Hello World
来源：http://paj.bjfxy.top

print "Hello\n";
来源：http://mcx.xziqi.cn

[T42] Perl：变量类型
来源：http://lgy.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wog.daria6918.cn

[T43] Perl：字符串插值
来源：http://zgo.shuidangran.top

"值: $a"
来源：http://bbj.chenlongwang.top

[T44] Perl：条件
来源：http://qif.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://nmn.fengsongda.top

[T45] Perl：数组遍历
来源：http://ydf.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://opw.yueranfly.top

[T46] Perl：哈希操作
来源：http://qwj.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rrq.fengsongda.top

[T47] Perl：正则捕获
来源：http://umk.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lax.dianchejie.cn

[T48] Perl：正则替换
来源：http://lol.mhx1999.top

$s =~ s/old/new/g;
来源：http://rdr.zhengqikj.top

[T49] Perl：函数
来源：http://pkz.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fjo.c1oappe.top

[T50] Perl：逐行读文件
来源：http://gyv.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bax.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://mxv.zhengqikj.top

[T51] Scala：Hello World
来源：http://szp.yvedp.cn

println("Hello")
来源：http://gfb.uphjek.com

[T52] Scala：变量
来源：http://bcy.ydjk.org.cn

val a = 1;  var b = 2
来源：http://yaw.fktsv.cn

[T53] Scala：字符串插值
来源：http://wqk.redwolf501.top

s"值: $b"
来源：http://tuw.meibo888.top

[T54] Scala：集合映射
来源：http://cly.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://aau.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://pcm.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gha.dashuyun.cn

[T56] Scala：样例类
来源：http://gsa.guannengcc.top


<!-- 参考信息 -->