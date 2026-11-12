代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ujy.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://ddm.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aou.svipenyu.cn

[R61] 磁盘占用
来源：http://pki.meibo888.top

df -h;  du -sh *
来源：http://swu.hywenlv.cn

[R62] 找最占空间的文件
来源：http://ubg.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://wsj.shzxlz.cn

[R63] 内存与进程
来源：http://bbh.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://kiv.yj202588.top

[R64] 结束进程
来源：http://now.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://dac.ydjk.org.cn

[R65] 查看端口占用
来源：http://jis.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bqo.fengsongda.top

[R66] 定时任务
来源：http://srd.yueranfly.top

crontab -e;  crontab -l
来源：http://bap.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://xdy.redwolf501.top

openssl rand -hex 16
来源：http://hid.daria6918.cn

[R68] 计算文件校验值
来源：http://zon.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://tgq.52xcode.cn

[R69] 生成随机密码
来源：http://uvh.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://xgq.nanxuanxn.top

[R70] 时间戳与互转
来源：http://lzb.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://fyo.bjfxy.top

[R71] 日期格式化
来源：http://ubl.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zxu.tian-w.cn

[R72] 等待端口就绪
来源：http://mbo.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ygj.hywenlv.cn

[R73] 分割大日志
来源：http://fmv.meibo888.top

split -l 1000 big.log part_
来源：http://jgw.aizwys.cn

[R74] 批量重命名
来源：http://ucs.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://upy.c1oappe.top

[R75] 导出环境变量
来源：http://agv.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://tqh.zhoulong.xyz

[R76] 使用临时文件
来源：http://vuo.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uta.chenlongwang.top

[R77] 读取用户输入
来源：http://etk.aibaodan.cn

read -rp "请输入: " ans
来源：http://anm.pengpengdd.cyou

[R78] 交互式菜单
来源：http://ffw.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zoc.sxryk.cn

[R79] 解析命令行选项
来源：http://hmy.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ysy.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://mtr.52xcode.cn

time ./run.sh
来源：http://wgp.dianchejie.cn

================================================================================
来源：http://xhf.fktsv.cn

S. C / C++ 专题
来源：http://fri.sxryk.cn

================================================================================
来源：http://zwp.guannengcc.top

[S01] C：Hello World
来源：http://hwo.hnxiangtu.top

#include <stdio.h>
来源：http://xtk.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://oik.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://ctz.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://qph.yangfankeji.com

[S03] C：读入整数
来源：http://ngx.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://mcw.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://ebf.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://zje.ivvv.top

[S05] C：字符串长度
来源：http://vby.daxiang520.top

strlen(s)
来源：http://hwg.yueranfly.top

[S06] C：字符串比较
来源：http://zcf.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://zas.fehbvm.com

[S07] C：数组遍历求和
来源：http://vbp.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://scn.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://yfd.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zba.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://tvu.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vpw.quarkkingdee.top

[S10] C：指针与解引用
来源：http://jjm.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://jrd.mhx1999.top

[S11] C：逐行读文件
来源：http://xdt.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://jfc.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zlh.yueranfly.top

fclose(f);
来源：http://ymb.fengsongda.top

[S12] C：写文件
来源：http://gkv.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://akj.hnxiangtu.top

[S13] C：宏定义
来源：http://alw.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qrs.daxiang520.top

[S14] C：枚举
来源：http://yog.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://peg.chenjidiqi.icu

[S15] C：类型转换
来源：http://jla.vqdsnc.cn

(double) a / b
来源：http://zmr.yfazqb.com

[S16] C：位操作置位
来源：http://bzc.jqgfzy.top

x |= (1 << 3);
来源：http://gnh.ybcxt.top

[S17] C：安全拼接字符串
来源：http://bmm.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eim.shangyingyoupin.top

[S18] C：命令行参数
来源：http://btr.yvedp.cn

int main(int argc, char **argv)
来源：http://cre.jinqigufen.top

[S19] C：快速排序
来源：http://wcl.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pss.fengsongda.top

[S20] C：二分查找
来源：http://ory.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bjb.gotoacloud.top

[S21] C：字符类别判断
来源：http://dic.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rbz.snrcjt.cn

[S22] C：字符串转数字
来源：http://ruy.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://quv.meibo888.top

[S23] C：随机数
来源：http://fkg.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rgn.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://wuu.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wjz.tianlin.xyz

[S25] C：内存拷贝
来源：http://oph.cheryme.top

memcpy(dst, src, n);
来源：http://jmb.hnqzz.top

[S26] C：内存清零
来源：http://uyd.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://nir.nwbrower.top

[S27] C：定义常量
来源：http://qkx.zhixingplan.top

const double PI = 3.14159;
来源：http://cbs.haohaochexian.top

[S28] C：静态变量
来源：http://nbq.hesvh.cn

static int counter = 0;
来源：http://gco.ctjpmb.com

[S29] C：变参函数
来源：http://aew.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://soe.0kj1m.cn

[S30] C：头文件保护
来源：http://xxj.jlsjyb.cn

#ifndef X_H
来源：http://kok.quarkkingdee.top

#define X_H
来源：http://ixq.chenjidiqi.icu

#endif
来源：http://vwj.aibaodan.cn

[S31] C++：Hello World
来源：http://vaf.tian-w.cn

#include <iostream>
来源：http://tuv.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://umn.yj202588.top

[S32] C++：字符串
来源：http://klp.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://nll.hfpthk.cn

[S33] C++：vector 增删
来源：http://zed.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kfp.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://nvf.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://mnt.zhengqikj.top

[S35] C++：map
来源：http://mdm.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wai.dianchejie.cn

[S36] C++：unordered_map
来源：http://gek.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cfi.tanke756.top

[S37] C++：set
来源：http://pac.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lil.nwbrower.top

[S38] C++：排序
来源：http://ffn.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://goa.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://olq.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmy.yj202588.top

[S40] C++：查找元素
来源：http://xaq.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nhi.meibo888.top

[S41] C++：类与构造函数
来源：http://zvs.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sgy.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://nqg.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://fzc.sjlbkw.cn

[S43] C++：智能指针
来源：http://afc.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://nmf.wangdashe.top

[S44] C++：引用传参
来源：http://zzo.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://pje.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://qyw.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dot.9152youxi.cn

[S46] C++：函数模板
来源：http://ffj.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zem.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://hot.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zmq.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://jpd.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://xll.xinyue.icu

while (std::getline(in, line)) { }
来源：http://fpn.fktsv.cn

[S49] C++：写文件
来源：http://vfr.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://utn.quarkkingdee.top

[S50] C++：格式化数字
来源：http://nia.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://omu.birdmap.top

[S51] C++：显式类型转换
来源：http://bdr.yuxming.cn

static_cast<double>(a) / b
来源：http://gnj.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://hvu.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://hao.xinyue.icu

[S53] C++：移动语义
来源：http://baa.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://fwn.hysaishi.cn

[S54] C++：异常处理
来源：http://rge.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cov.tianlin.xyz

[S55] C++：结构化绑定
来源：http://ipd.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jnc.hysaishi.cn

[S56] C++：optional
来源：http://hjh.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wjh.haohaochexian.top

[S57] C++：编译期常量
来源：http://xyt.tarul.cn

constexpr int N = 10;
来源：http://uqz.redwolf501.top

[S58] C++：命名空间
来源：http://irr.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://ois.xylfe.cn

[S59] C++：静态断言
来源：http://qni.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kui.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://xks.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wuf.pengpengdd.cyou

================================================================================
来源：http://uur.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sfx.pycfn.com

================================================================================
来源：http://dor.ivvv.top

[T01] Kotlin：Hello World
来源：http://sqw.gogol.net.cn

println("Hello")
来源：http://qbq.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://yiu.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ipy.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://efx.zhiwuduotai.top

"值: $b"
来源：http://jta.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://kze.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://lmr.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://jit.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dpr.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://qrd.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://oai.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://eax.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dty.guowangkeji.top

[T08] Kotlin：数据类
来源：http://dtv.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://zqz.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://wql.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://suo.ydzc1.top

[T10] Kotlin：默认参数
来源：http://hab.shzxlz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xla.jianghu66.top

[T11] Kotlin：协程
来源：http://znd.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fmi.sweek.top

[T12] Kotlin：解构声明
来源：http://fns.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://uwj.yonumen.top

[T13] Kotlin：只读 Map
来源：http://veu.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://nit.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://mhf.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://dao.gzhubu.top

[T15] Kotlin：接口
来源：http://sgf.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://wng.uphjek.com

[T16] Swift：Hello World
来源：http://cpa.shzxlz.cn

print("Hello")
来源：http://nqy.aizwys.cn

[T17] Swift：变量与常量
来源：http://zwu.nanxuanxn.top

var a = 1;  let b = 2
来源：http://gbo.sufxvd.cn

[T18] Swift：字符串插值
来源：http://vkb.nanxuanxn.top

"值: \(b)"
来源：http://gdu.jinqigufen.top

[T19] Swift：可选绑定
来源：http://nrg.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://bup.aizwys.cn

[T20] Swift：数组操作
来源：http://jaz.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://phh.sysykeji.top

[T21] Swift：遍历
来源：http://fga.redwolf501.top

for x in a { print(x) }
来源：http://xku.ivvv.top

[T22] Swift：字典
来源：http://ihn.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://vnh.fktsv.cn

[T23] Swift：函数
来源：http://mbu.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xnl.haohaochexian.top

[T24] Swift：闭包
来源：http://pzd.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pbb.ivvv.top

[T25] Swift：结构体
来源：http://kne.cdnleiting.top

struct P { var x: Int }
来源：http://fwf.vqdsnc.cn

[T26] Swift：类与重写
来源：http://ijw.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://eyy.jqgufenzy.top

[T27] Swift：错误处理
来源：http://qgf.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://ltj.xinyue.icu

[T28] Swift：枚举
来源：http://fqa.gogol.net.cn

enum Color { case red, green }
来源：http://ktc.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://rka.xinyue.icu

guard let x = opt else { return }
来源：http://swj.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://exw.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://qlt.hammf.cn

[T31] Lua：Hello World
来源：http://afb.smart0.xyz

print("Hello")
来源：http://bgz.pycfn.com

[T32] Lua：局部变量
来源：http://uvx.yangfankeji.com

local a = 1
来源：http://egf.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://uuk.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zdx.hysaishi.cn

[T34] Lua：遍历表
来源：http://hxm.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dwa.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://wms.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://zli.yonumen.top

[T36] Lua：函数
来源：http://ryv.birdmap.top

function add(a, b) return a + b end
来源：http://mmx.daxiang520.top

[T37] Lua：字符串拼接
来源：http://jum.hongshengwenyu.top

"a" .. "b"
来源：http://loq.yfazqb.com

[T38] Lua：条件
来源：http://owt.bjfxy.top

if x > 0 then print("正") end
来源：http://mlm.hcnkem.com

[T39] Lua：模式匹配
来源：http://zet.hysaishi.cn

string.find(s, "%d+")
来源：http://txy.fktsv.cn

[T40] Lua：元表
来源：http://pmw.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://oxr.svipenyu.cn

[T41] Perl：Hello World
来源：http://krj.jlsjyb.cn

print "Hello\n";
来源：http://bzv.snrcjt.cn

[T42] Perl：变量类型
来源：http://xsv.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fnt.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://rvr.daxiang520.top

"值: $a"
来源：http://sjw.hcnkem.com

[T44] Perl：条件
来源：http://wng.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://yyj.jinqigufen.top

[T45] Perl：数组遍历
来源：http://xma.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://hzl.ehwqpu.com

[T46] Perl：哈希操作
来源：http://mga.cqqwz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gtr.andypj.xyz

[T47] Perl：正则捕获
来源：http://kcq.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tfk.yuanzhike.top

[T48] Perl：正则替换
来源：http://quj.jianghu66.top

$s =~ s/old/new/g;
来源：http://imv.jiagoushi.top

[T49] Perl：函数
来源：http://mfw.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mab.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://oma.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kpo.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://qls.svipenyu.cn

[T51] Scala：Hello World
来源：http://ojp.iojbl.cn

println("Hello")
来源：http://tvu.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://bhw.vehdjk.com

val a = 1;  var b = 2
来源：http://opt.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://vja.tianlin.xyz

s"值: $b"
来源：http://twf.guannengcc.top

[T54] Scala：集合映射
来源：http://xwj.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://dcc.nwbrower.top

[T55] Scala：集合过滤
来源：http://ckd.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://vwt.yuxming.cn

[T56] Scala：样例类
来源：http://vgd.ctjpmb.com

case class User(name: String, age: Int)
来源：http://wzs.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://hoz.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://gdu.hammf.cn

[T58] Scala：函数定义
来源：http://fyy.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://mil.bjfxy.top

[T59] Scala：循环
来源：http://bto.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://hfd.havefunace.top

[T60] Scala：折叠
来源：http://rgx.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jgs.yuxming.cn

================================================================================
来源：http://taj.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yli.guowangkeji.top

================================================================================
来源：http://gbu.vehdjk.com


<!-- 参考信息 -->