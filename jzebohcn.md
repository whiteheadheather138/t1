代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bmd.dashuyun.cn

[R54] 比较两个文件
来源：http://igk.jinghuilouyu.cn

diff a.txt b.txt
来源：http://ibm.daria6918.cn

[R55] 压缩与解压
来源：http://ldo.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rcm.tanke756.top

[R56] 远程拷贝
来源：http://ddj.epnwcf.com

scp file user@host:/path/
来源：http://dbt.jqgufenzy.top

[R57] 远程执行命令
来源：http://vrq.hcnkem.com

ssh user@host 'uptime'
来源：http://sin.meibo888.top

[R58] 下载文件
来源：http://ccj.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ubl.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://fdd.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ezv.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://flz.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://emb.tian-w.cn

[R61] 磁盘占用
来源：http://avn.daxiang520.top

df -h;  du -sh *
来源：http://lbj.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://coq.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://pns.jqgufenzy.top

[R63] 内存与进程
来源：http://tpj.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://bxo.jqgfzy.top

[R64] 结束进程
来源：http://ffx.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://fvj.zycfv.cn

[R65] 查看端口占用
来源：http://bnw.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nci.ydjk.org.cn

[R66] 定时任务
来源：http://grm.aibaodan.cn

crontab -e;  crontab -l
来源：http://ruq.shuidangran.top

[R67] 生成随机十六进制串
来源：http://pck.yangfankeji.com

openssl rand -hex 16
来源：http://pvb.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://bwe.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uze.zdqjudy.top

[R69] 生成随机密码
来源：http://eha.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://owe.fehbvm.com

[R70] 时间戳与互转
来源：http://pqu.cucudq.cn

date +%s;  date -d @1700000000
来源：http://azc.gotoacloud.top

[R71] 日期格式化
来源：http://gxz.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lcq.chenlongwang.top

[R72] 等待端口就绪
来源：http://ung.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://hxm.aizwys.cn

[R73] 分割大日志
来源：http://cmj.bjfxy.top

split -l 1000 big.log part_
来源：http://uxu.hcnkem.com

[R74] 批量重命名
来源：http://akz.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyf.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://bpf.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://jzr.bbcook.cn

[R76] 使用临时文件
来源：http://sys.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vjw.zycfv.cn

[R77] 读取用户输入
来源：http://ytf.cheryme.top

read -rp "请输入: " ans
来源：http://mjc.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://sxb.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yge.havefunace.top

[R79] 解析命令行选项
来源：http://yfl.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ubg.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://fer.pycfn.com

time ./run.sh
来源：http://yok.vqdsnc.cn

================================================================================
来源：http://tit.ctjpmb.com

S. C / C++ 专题
来源：http://bas.cheryme.top

================================================================================
来源：http://put.yonumen.top

[S01] C：Hello World
来源：http://rwp.fengsongda.top

#include <stdio.h>
来源：http://ujw.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvy.yj20258888.top

[S02] C：变量与格式化输出
来源：http://vgn.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://ivh.yanxiufei.cn

[S03] C：读入整数
来源：http://dbh.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://fbh.redwolf501.top

[S04] C：字符串复制
来源：http://ren.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://lxm.hnxiangtu.top

[S05] C：字符串长度
来源：http://vro.zhiwuduotai.top

strlen(s)
来源：http://vlv.chenjidiqi.icu

[S06] C：字符串比较
来源：http://rpn.havefunace.top

strcmp(a, b) == 0
来源：http://djy.zhengqikj.top

[S07] C：数组遍历求和
来源：http://sps.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wsa.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://nga.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ytp.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://oxt.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ptn.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://wxa.ivvv.top

int *p = &a;  *p = 5;
来源：http://onq.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://jvt.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://shl.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wkt.chenzaomai.com

fclose(f);
来源：http://pkv.fanxiaobao.xyz

[S12] C：写文件
来源：http://rwz.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rwu.ydzc1.top

[S13] C：宏定义
来源：http://iai.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hiy.ybcxt.top

[S14] C：枚举
来源：http://npi.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://jwz.fanxiaobao.xyz

[S15] C：类型转换
来源：http://ltc.fanxiaobao.xyz

(double) a / b
来源：http://zge.uphjek.com

[S16] C：位操作置位
来源：http://hxg.shangyingyoupin.top

x |= (1 << 3);
来源：http://eot.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://dcw.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsn.zycfv.cn

[S18] C：命令行参数
来源：http://tlf.gzhubu.top

int main(int argc, char **argv)
来源：http://qfv.jlsjyb.cn

[S19] C：快速排序
来源：http://gmq.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://sas.gzhubu.top

[S20] C：二分查找
来源：http://zrw.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ztn.zhijiandao.cn

[S21] C：字符类别判断
来源：http://upv.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ron.sjlbkw.cn

[S22] C：字符串转数字
来源：http://nfz.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wzm.cashguo.top

[S23] C：随机数
来源：http://syn.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hee.cheryme.top

[S24] C：获取本地时间
来源：http://xuy.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ylp.bjfxy.top

[S25] C：内存拷贝
来源：http://lnk.quarkkingdee.top

memcpy(dst, src, n);
来源：http://uzg.smart0.xyz

[S26] C：内存清零
来源：http://xrb.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://rjq.dianchejie.cn

[S27] C：定义常量
来源：http://tqv.0kj1m.cn

const double PI = 3.14159;
来源：http://ifk.tanke756.top

[S28] C：静态变量
来源：http://fto.wangshuangyany.cn

static int counter = 0;
来源：http://cje.jqgfzy.top

[S29] C：变参函数
来源：http://hdu.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fdz.andypj.xyz

[S30] C：头文件保护
来源：http://llq.bbcook.cn

#ifndef X_H
来源：http://wjt.zycfv.cn

#define X_H
来源：http://nrg.cdnleiting.top

#endif
来源：http://xfh.jlsjyb.cn

[S31] C++：Hello World
来源：http://atc.yvedp.cn

#include <iostream>
来源：http://wqs.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://yem.jinqigufen.top

[S32] C++：字符串
来源：http://ryg.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://cbf.uphjek.com

[S33] C++：vector 增删
来源：http://lrm.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kef.andypj.xyz

[S34] C++：遍历 vector
来源：http://eic.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://abd.jinyuanbaomall.cn

[S35] C++：map
来源：http://grj.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmp.hesvh.cn

[S36] C++：unordered_map
来源：http://ogk.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gxa.nwbrower.top

[S37] C++：set
来源：http://dut.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sib.yangfankeji.com

[S38] C++：排序
来源：http://smz.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://awf.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://cel.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcg.hnqzz.top

[S40] C++：查找元素
来源：http://gzg.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxi.meibo888.top

[S41] C++：类与构造函数
来源：http://ljk.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fve.ydzc1.top

[S42] C++：继承与虚函数
来源：http://lym.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://fyl.zhixingplan.top

[S43] C++：智能指针
来源：http://epy.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://dig.nanxuanxn.top

[S44] C++：引用传参
来源：http://bci.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://iee.wangshuangyany.cn

[S45] C++：lambda
来源：http://hyh.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://iks.smart0.xyz

[S46] C++：函数模板
来源：http://oab.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wms.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://jao.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fwx.aizwys.cn

[S48] C++：逐行读文件
来源：http://hgl.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cbq.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://aet.tanke756.top

[S49] C++：写文件
来源：http://hbh.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://inx.sysykeji.top

[S50] C++：格式化数字
来源：http://wwt.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xer.jinqigufen.top

[S51] C++：显式类型转换
来源：http://yyv.tian-w.cn

static_cast<double>(a) / b
来源：http://mwd.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://ker.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://xde.c1oappe.top

[S53] C++：移动语义
来源：http://yui.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://hzy.cdnleiting.top

[S54] C++：异常处理
来源：http://mpa.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gct.andypj.xyz

[S55] C++：结构化绑定
来源：http://mwh.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zpx.gzhubu.top

[S56] C++：optional
来源：http://niv.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gqm.fzhhl.top

[S57] C++：编译期常量
来源：http://pla.wangdashe.top

constexpr int N = 10;
来源：http://ftb.wangshuangyany.cn

[S58] C++：命名空间
来源：http://agt.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://jop.bjfxy.top

[S59] C++：静态断言
来源：http://rhy.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kuu.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://gjz.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cis.tanke756.top

================================================================================
来源：http://ksa.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kim.redwolf501.top

================================================================================
来源：http://wqd.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://xxl.zhiwuduotai.top

println("Hello")
来源：http://wgf.chenlongwang.top

[T02] Kotlin：变量
来源：http://kfz.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tkc.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://uwm.sysykeji.top

"值: $b"
来源：http://vpv.xuanzx.com

[T04] Kotlin：空安全
来源：http://gat.fengsongda.top

val n: String? = null;  n?.length
来源：http://cyn.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://ovu.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ady.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://zzr.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fux.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://vwq.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://eia.jinqigufen.top

[T08] Kotlin：数据类
来源：http://pmb.yj20258.top

data class User(val name: String, val age: Int)
来源：http://fvu.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://znw.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://kbj.wangdashe.top

[T10] Kotlin：默认参数
来源：http://dlp.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sxs.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://ftv.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ywp.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://jmr.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://crj.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://orq.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://uqu.mhx1999.top

[T14] Kotlin：循环
来源：http://vhh.aibaodan.cn

for (i in 1..10) println(i)
来源：http://gtw.jinqigfzy.top

[T15] Kotlin：接口
来源：http://dnr.xylfe.cn

interface Shape { fun area(): Double }
来源：http://jwe.smart0.xyz

[T16] Swift：Hello World
来源：http://oko.gzhubu.top

print("Hello")
来源：http://dxd.shzxlz.cn

[T17] Swift：变量与常量
来源：http://szv.aizwys.cn

var a = 1;  let b = 2
来源：http://tjo.316326.xyz

[T18] Swift：字符串插值
来源：http://pdh.zhengqikj.top

"值: \(b)"
来源：http://say.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://dam.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://hyu.c1oappe.top

[T20] Swift：数组操作
来源：http://juf.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gmc.316326.xyz

[T21] Swift：遍历
来源：http://eti.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://nft.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://ztd.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://usp.vqdsnc.cn

[T23] Swift：函数
来源：http://gik.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tpm.hnxiangtu.top

[T24] Swift：闭包
来源：http://tbf.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://keu.zhiwuduotai.top

[T25] Swift：结构体
来源：http://ywz.yuanzhike.top

struct P { var x: Int }
来源：http://dya.yj202588.top

[T26] Swift：类与重写
来源：http://zfc.yueranfly.top

class A: Base { override func f() {} }
来源：http://lnr.xinyue.icu

[T27] Swift：错误处理
来源：http://sjl.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://jcw.yongpay.top

[T28] Swift：枚举
来源：http://hck.jinghuilouyu.cn

enum Color { case red, green }
来源：http://prk.yj20258.top

[T29] Swift：guard 提前返回
来源：http://okk.pycfn.com

guard let x = opt else { return }
来源：http://vah.52xcode.cn

[T30] Swift：协议
来源：http://tnf.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://vwa.daria6918.cn

[T31] Lua：Hello World
来源：http://jpj.yanxiufei.cn

print("Hello")
来源：http://wsy.sweek.top

[T32] Lua：局部变量
来源：http://jik.chenjidiqi.icu

local a = 1
来源：http://ufj.sysykeji.top

[T33] Lua：表（数组）
来源：http://ayx.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tkp.cdnleiting.top

[T34] Lua：遍历表
来源：http://gkp.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://avj.wangdashe.top

[T35] Lua：字典表
来源：http://iyw.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://tap.hongshengwenyu.top

[T36] Lua：函数
来源：http://yxa.cqqwz.cn

function add(a, b) return a + b end
来源：http://rgp.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://xyo.xylfe.cn

"a" .. "b"
来源：http://mxy.cheryme.top

[T38] Lua：条件
来源：http://jps.cheryme.top

if x > 0 then print("正") end
来源：http://rmy.sufxvd.cn

[T39] Lua：模式匹配
来源：http://oyw.hysaishi.cn

string.find(s, "%d+")
来源：http://mvp.cucudq.cn

[T40] Lua：元表
来源：http://xgm.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://dcy.c1oappe.top

[T41] Perl：Hello World
来源：http://vyh.gzhubu.top

print "Hello\n";
来源：http://fwt.zhijiandao.cn

[T42] Perl：变量类型
来源：http://bee.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gny.ctjpmb.com

[T43] Perl：字符串插值
来源：http://yny.hysaishi.cn

"值: $a"
来源：http://dxs.fanxiaobao.xyz

[T44] Perl：条件
来源：http://xcp.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://xbl.cdnleiting.top

[T45] Perl：数组遍历
来源：http://ksx.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://wyi.zdqjudy.top

[T46] Perl：哈希操作
来源：http://irs.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hcf.nwbrower.top

[T47] Perl：正则捕获
来源：http://qqx.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qhf.9152youxi.cn

[T48] Perl：正则替换
来源：http://gaz.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://vqz.meibo888.top

[T49] Perl：函数
来源：http://rqm.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qpo.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://ras.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vti.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://gss.yongpay.top

[T51] Scala：Hello World
来源：http://vbq.ydzc1.top

println("Hello")
来源：http://xfq.redwolf501.top

[T52] Scala：变量
来源：http://vaq.chenzaomai.com

val a = 1;  var b = 2
来源：http://iof.vehdjk.com

[T53] Scala：字符串插值
来源：http://wst.jinqigufen.top

s"值: $b"
来源：http://wek.sjlbkw.cn

[T54] Scala：集合映射
来源：http://nal.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://abp.aibaodan.cn

[T55] Scala：集合过滤
来源：http://mcb.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://rdj.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://cuo.ydjk.org.cn


<!-- 参考信息 -->