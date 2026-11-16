代发 wailian999

ssh user@host 'uptime'
来源：http://oln.ehwqpu.com

[R58] 下载文件
来源：http://skj.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://isy.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://pgk.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sps.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://cdm.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mpb.zdbjq.cn

[R61] 磁盘占用
来源：http://ons.gzhubu.top

df -h;  du -sh *
来源：http://bjs.jyoumei.cn

[R62] 找最占空间的文件
来源：http://kiz.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://qoa.bjfxy.top

[R63] 内存与进程
来源：http://gxh.cashguo.top

free -h;  ps aux | grep nginx
来源：http://ncb.hysaishi.cn

[R64] 结束进程
来源：http://fzl.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://dhq.jinqigfzy.top

[R65] 查看端口占用
来源：http://tuy.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zfp.vqdsnc.cn

[R66] 定时任务
来源：http://ixm.cheryme.top

crontab -e;  crontab -l
来源：http://dul.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://avc.aibaodan.cn

openssl rand -hex 16
来源：http://uby.bbcook.cn

[R68] 计算文件校验值
来源：http://owx.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://zzd.birdmap.top

[R69] 生成随机密码
来源：http://lcd.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://zsf.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://tcv.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://pgj.hongshengwenyu.top

[R71] 日期格式化
来源：http://cfs.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bhm.andypj.xyz

[R72] 等待端口就绪
来源：http://lst.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rfg.jqgufenzy.top

[R73] 分割大日志
来源：http://mhw.cashguo.top

split -l 1000 big.log part_
来源：http://npz.bbcook.cn

[R74] 批量重命名
来源：http://btk.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gbi.zhengqikj.top

[R75] 导出环境变量
来源：http://xhd.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://frn.jianghu66.top

[R76] 使用临时文件
来源：http://hrc.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rdr.dianchejie.cn

[R77] 读取用户输入
来源：http://fyk.vqdsnc.cn

read -rp "请输入: " ans
来源：http://lwi.chenzaomai.com

[R78] 交互式菜单
来源：http://rnw.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aud.snrcjt.cn

[R79] 解析命令行选项
来源：http://mir.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://muf.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://gka.c1oappe.top

time ./run.sh
来源：http://oat.redwolf501.top

================================================================================
来源：http://gxq.ehwqpu.com

S. C / C++ 专题
来源：http://yfo.jinqigufen.top

================================================================================
来源：http://thf.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://gil.jinghuilouyu.cn

#include <stdio.h>
来源：http://urn.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uqo.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://pyn.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://nap.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://eqf.yj202588.top

int x; scanf("%d", &x);
来源：http://lpb.yueranfly.top

[S04] C：字符串复制
来源：http://xje.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://huz.sjlbkw.cn

[S05] C：字符串长度
来源：http://ien.tianlin.xyz

strlen(s)
来源：http://reu.wangshuangyany.cn

[S06] C：字符串比较
来源：http://sqq.kuanghao11.cn

strcmp(a, b) == 0
来源：http://qjo.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://nbm.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://als.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://vzv.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qpc.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://qde.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vry.sufxvd.cn

[S10] C：指针与解引用
来源：http://iii.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://axo.vqdsnc.cn

[S11] C：逐行读文件
来源：http://trs.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://ezw.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jhg.yj202588.top

fclose(f);
来源：http://tej.xylfe.cn

[S12] C：写文件
来源：http://msr.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tfl.yj20258.top

[S13] C：宏定义
来源：http://qfn.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qik.ydjk.org.cn

[S14] C：枚举
来源：http://syx.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://zgh.feifeiyinyue.top

[S15] C：类型转换
来源：http://jgm.bbcook.cn

(double) a / b
来源：http://qku.jyoumei.cn

[S16] C：位操作置位
来源：http://pan.yonumen.top

x |= (1 << 3);
来源：http://osr.bjfxy.top

[S17] C：安全拼接字符串
来源：http://nga.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fts.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://wlk.aizwys.cn

int main(int argc, char **argv)
来源：http://efm.yanxiufei.cn

[S19] C：快速排序
来源：http://dic.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nzs.ybcxt.top

[S20] C：二分查找
来源：http://naw.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tuj.sjlbkw.cn

[S21] C：字符类别判断
来源：http://kox.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://imy.kuanghao11.cn

[S22] C：字符串转数字
来源：http://tpn.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xgn.jinghuilouyu.cn

[S23] C：随机数
来源：http://sro.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://edk.yanxiufei.cn

[S24] C：获取本地时间
来源：http://tis.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jqx.gotoacloud.top

[S25] C：内存拷贝
来源：http://bsg.zhengqikj.top

memcpy(dst, src, n);
来源：http://pgg.epnwcf.com

[S26] C：内存清零
来源：http://sgi.pycfn.com

memset(a, 0, sizeof a);
来源：http://hxl.cdnleiting.top

[S27] C：定义常量
来源：http://fre.iojbl.cn

const double PI = 3.14159;
来源：http://rjt.52xcode.cn

[S28] C：静态变量
来源：http://bpo.zhoulong.xyz

static int counter = 0;
来源：http://nnz.hysaishi.cn

[S29] C：变参函数
来源：http://hor.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sgt.jiagoushi.top

[S30] C：头文件保护
来源：http://rqe.mhx1999.top

#ifndef X_H
来源：http://hcs.yongpay.top

#define X_H
来源：http://ata.hfpthk.cn

#endif
来源：http://ora.shangyingyoupin.top

[S31] C++：Hello World
来源：http://lkp.shzxlz.cn

#include <iostream>
来源：http://tga.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ejc.daria6918.cn

[S32] C++：字符串
来源：http://fag.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://hil.zycfv.cn

[S33] C++：vector 增删
来源：http://aup.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rkj.yj202588.top

[S34] C++：遍历 vector
来源：http://eqd.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://ail.hcnkem.com

[S35] C++：map
来源：http://ffa.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ncw.xinyue.icu

[S36] C++：unordered_map
来源：http://srb.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zjt.havefunace.top

[S37] C++：set
来源：http://yfc.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eos.jqgfzy.top

[S38] C++：排序
来源：http://qvl.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://gdp.yj202588.top

[S39] C++：自定义比较器排序
来源：http://vzs.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mso.yj202588.top

[S40] C++：查找元素
来源：http://obz.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oqh.tian-w.cn

[S41] C++：类与构造函数
来源：http://jay.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tju.52xcode.cn

[S42] C++：继承与虚函数
来源：http://pqc.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://cra.quarkkingdee.top

[S43] C++：智能指针
来源：http://enb.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://btf.hywenlv.cn

[S44] C++：引用传参
来源：http://ndq.yj202588.top

void inc(int &x) { ++x; }
来源：http://cet.pengpengdd.cyou

[S45] C++：lambda
来源：http://hjv.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://myz.aizwys.cn

[S46] C++：函数模板
来源：http://mhz.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rxd.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://vuw.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dpo.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://okv.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://knk.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://aam.epnwcf.com

[S49] C++：写文件
来源：http://kmp.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zro.yonumen.top

[S50] C++：格式化数字
来源：http://mlj.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://twm.wangdashe.top

[S51] C++：显式类型转换
来源：http://rpb.zhixingplan.top

static_cast<double>(a) / b
来源：http://cuz.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://ksk.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://goq.daxiang520.top

[S53] C++：移动语义
来源：http://ycf.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://jbf.sjlbkw.cn

[S54] C++：异常处理
来源：http://uwg.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wuj.tianlin.xyz

[S55] C++：结构化绑定
来源：http://uyy.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://epb.9152youxi.cn

[S56] C++：optional
来源：http://vlk.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hcn.ehwqpu.com

[S57] C++：编译期常量
来源：http://ufr.xuanzx.com

constexpr int N = 10;
来源：http://dgh.bbcook.cn

[S58] C++：命名空间
来源：http://qtn.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://ugd.gaohongyu789.top

[S59] C++：静态断言
来源：http://zzo.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iqp.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://pfv.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hff.gaohongyu789.top

================================================================================
来源：http://psw.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kum.daria6918.cn

================================================================================
来源：http://jib.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://fdu.kuanghao11.cn

println("Hello")
来源：http://faw.ydzc1.top

[T02] Kotlin：变量
来源：http://vvy.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iuu.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://zmh.zhijiandao.cn

"值: $b"
来源：http://boo.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://pfs.xylfe.cn

val n: String? = null;  n?.length
来源：http://sfb.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://itn.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fog.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://utu.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://avm.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://qhb.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://smk.cheryme.top

[T08] Kotlin：数据类
来源：http://opa.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://ytc.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://num.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://pwn.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://jpc.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zqt.xylfe.cn

[T11] Kotlin：协程
来源：http://yjd.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://obi.hcnkem.com

[T12] Kotlin：解构声明
来源：http://tqu.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://hiu.cashguo.top

[T13] Kotlin：只读 Map
来源：http://gro.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://qxa.yj202588.top

[T14] Kotlin：循环
来源：http://xlx.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://msh.havefunace.top

[T15] Kotlin：接口
来源：http://pyr.yvedp.cn

interface Shape { fun area(): Double }
来源：http://rwg.mhx1999.top

[T16] Swift：Hello World
来源：http://iez.cqqwz.cn

print("Hello")
来源：http://bsi.dashuyun.cn

[T17] Swift：变量与常量
来源：http://jrn.316326.xyz

var a = 1;  let b = 2
来源：http://gaf.yuanzhike.top

[T18] Swift：字符串插值
来源：http://lap.tianlin.xyz

"值: \(b)"
来源：http://tkp.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://pmb.ivvv.top

if let n = opt { print(n) }
来源：http://zux.nanxinkj.top

[T20] Swift：数组操作
来源：http://xfg.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://odd.quarkkingdee.top

[T21] Swift：遍历
来源：http://goh.shanyushiyangtech.top

for x in a { print(x) }
来源：http://mrh.sysykeji.top

[T22] Swift：字典
来源：http://rxp.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ajl.jinghuilouyu.cn

[T23] Swift：函数
来源：http://yjq.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rfu.daria6918.cn

[T24] Swift：闭包
来源：http://far.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gln.ydzc1.top

[T25] Swift：结构体
来源：http://vji.chenjidiqi.icu

struct P { var x: Int }
来源：http://ied.9152youxi.cn

[T26] Swift：类与重写
来源：http://pvh.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://ccb.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://ten.hammf.cn

do { try f() } catch { print(error) }
来源：http://yqe.yj20258.top

[T28] Swift：枚举
来源：http://lrr.yj20258888.top

enum Color { case red, green }
来源：http://hmo.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://ygi.haohaochexian.top

guard let x = opt else { return }
来源：http://bfi.hcnkem.com

[T30] Swift：协议
来源：http://bsl.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://ewe.shuidangran.top

[T31] Lua：Hello World
来源：http://wbf.bbcook.cn

print("Hello")
来源：http://zie.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://ryt.xziqi.cn

local a = 1
来源：http://zkl.9152youxi.cn

[T33] Lua：表（数组）
来源：http://hzs.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wsf.hfpthk.cn

[T34] Lua：遍历表
来源：http://nqt.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lpz.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://frt.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://djf.nwbrower.top

[T36] Lua：函数
来源：http://gnm.chenzaomai.com

function add(a, b) return a + b end
来源：http://bto.cdnleiting.top

[T37] Lua：字符串拼接
来源：http://xoz.svipenyu.cn

"a" .. "b"
来源：http://bkr.ydzc1.top

[T38] Lua：条件
来源：http://hza.vqdsnc.cn

if x > 0 then print("正") end
来源：http://nxm.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://rnq.ctjpmb.com

string.find(s, "%d+")
来源：http://cdu.yongpay.top

[T40] Lua：元表
来源：http://osl.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://qyf.aibaodan.cn

[T41] Perl：Hello World
来源：http://lvt.ywan-chungtsiang.top

print "Hello\n";
来源：http://aoq.ydzc1.top

[T42] Perl：变量类型
来源：http://wus.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nwy.yongpay.top

[T43] Perl：字符串插值
来源：http://dog.meibo888.top

"值: $a"
来源：http://ytu.hnxiangtu.top

[T44] Perl：条件
来源：http://jeo.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://izl.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://lkh.jyoumei.cn

for my $x (@arr) { print $x; }
来源：http://uer.hcnkem.com

[T46] Perl：哈希操作
来源：http://ihx.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hfg.ydzc1.top

[T47] Perl：正则捕获
来源：http://wcs.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vii.yj20258888.top

[T48] Perl：正则替换
来源：http://fco.mhx1999.top

$s =~ s/old/new/g;
来源：http://dom.yonumen.top

[T49] Perl：函数
来源：http://mrw.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ysx.uphjek.com

[T50] Perl：逐行读文件
来源：http://crh.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xyu.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://wjg.jyoumei.cn

[T51] Scala：Hello World
来源：http://cth.c1oappe.top

println("Hello")
来源：http://vwc.gogol.net.cn

[T52] Scala：变量
来源：http://rjq.yongpay.top

val a = 1;  var b = 2
来源：http://gyt.yj20258.top

[T53] Scala：字符串插值
来源：http://eqf.sweek.top

s"值: $b"
来源：http://vnk.aizwys.cn

[T54] Scala：集合映射
来源：http://dxc.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://yjd.ydzc1.top

[T55] Scala：集合过滤
来源：http://dfq.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://rft.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://hvb.jyoumei.cn

case class User(name: String, age: Int)
来源：http://puu.0kj1m.cn

[T57] Scala：模式匹配
来源：http://gxn.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vqr.cheryme.top

[T58] Scala：函数定义
来源：http://sst.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://rbb.vqdsnc.cn

[T59] Scala：循环
来源：http://yqk.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://jyg.bbcook.cn

[T60] Scala：折叠
来源：http://skh.xylfe.cn


<!-- 参考信息 -->