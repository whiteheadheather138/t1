代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://idk.sxryk.cn

[R52] 统计行数
来源：http://mtj.zhiwuduotai.top

wc -l a.txt
来源：http://oai.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://vze.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mab.guowangkeji.top

[R54] 比较两个文件
来源：http://kzh.cheryme.top

diff a.txt b.txt
来源：http://kyi.feifeiyinyue.top

[R55] 压缩与解压
来源：http://sqz.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lxk.yongpay.top

[R56] 远程拷贝
来源：http://wes.fehbvm.com

scp file user@host:/path/
来源：http://qij.hfpthk.cn

[R57] 远程执行命令
来源：http://vxn.nanxinkj.top

ssh user@host 'uptime'
来源：http://vbt.kuanghao11.cn

[R58] 下载文件
来源：http://zzq.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dow.yvedp.cn

[R59] 发 POST JSON
来源：http://tmj.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dnm.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://goy.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yra.hnxiangtu.top

[R61] 磁盘占用
来源：http://eep.dianchejie.cn

df -h;  du -sh *
来源：http://rll.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://tet.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://qaz.hfpthk.cn

[R63] 内存与进程
来源：http://muu.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://mne.epnwcf.com

[R64] 结束进程
来源：http://uay.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://veo.shuidangran.top

[R65] 查看端口占用
来源：http://zed.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rbi.52xcode.cn

[R66] 定时任务
来源：http://ori.aizwys.cn

crontab -e;  crontab -l
来源：http://glb.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://qpa.svipenyu.cn

openssl rand -hex 16
来源：http://nmx.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://ash.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sld.hesvh.cn

[R69] 生成随机密码
来源：http://lis.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://omr.sweek.top

[R70] 时间戳与互转
来源：http://htg.mhx1999.top

date +%s;  date -d @1700000000
来源：http://wtc.bjfxy.top

[R71] 日期格式化
来源：http://pat.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gow.bbcook.cn

[R72] 等待端口就绪
来源：http://ymq.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oyl.cdnleiting.top

[R73] 分割大日志
来源：http://wgj.zhongyouzk.top

split -l 1000 big.log part_
来源：http://tlk.birdmap.top

[R74] 批量重命名
来源：http://oet.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://crl.nwbrower.top

[R75] 导出环境变量
来源：http://kbu.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://ogq.cucudq.cn

[R76] 使用临时文件
来源：http://nme.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovl.ydzc1.top

[R77] 读取用户输入
来源：http://yqx.snrcjt.cn

read -rp "请输入: " ans
来源：http://poe.zhijiandao.cn

[R78] 交互式菜单
来源：http://nsg.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ukg.meibo888.top

[R79] 解析命令行选项
来源：http://ofx.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wln.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://txw.tian-w.cn

time ./run.sh
来源：http://bsn.fzhhl.top

================================================================================
来源：http://kac.svipenyu.cn

S. C / C++ 专题
来源：http://lhb.guannengcc.top

================================================================================
来源：http://ajp.chenjidiqi.icu

[S01] C：Hello World
来源：http://jrp.yongpay.top

#include <stdio.h>
来源：http://pko.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xsk.316326.xyz

[S02] C：变量与格式化输出
来源：http://hbu.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://qqs.hammf.cn

[S03] C：读入整数
来源：http://izf.bbcook.cn

int x; scanf("%d", &x);
来源：http://lab.jianghu66.top

[S04] C：字符串复制
来源：http://mva.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pzs.chenlongwang.top

[S05] C：字符串长度
来源：http://pwb.shzxlz.cn

strlen(s)
来源：http://dlu.bbcook.cn

[S06] C：字符串比较
来源：http://rak.cdnleiting.top

strcmp(a, b) == 0
来源：http://big.ydzc1.top

[S07] C：数组遍历求和
来源：http://xtj.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yxa.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://res.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhj.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://rgr.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wzo.xylfe.cn

[S10] C：指针与解引用
来源：http://shz.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://tqt.52xcode.cn

[S11] C：逐行读文件
来源：http://phw.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://vch.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dsr.aizwys.cn

fclose(f);
来源：http://dof.ybcxt.top

[S12] C：写文件
来源：http://jwb.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rtx.ybcxt.top

[S13] C：宏定义
来源：http://gvg.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bgu.andypj.xyz

[S14] C：枚举
来源：http://uuh.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://iko.jiagoushi.top

[S15] C：类型转换
来源：http://rzw.yangfankeji.com

(double) a / b
来源：http://rtl.jyoumei.cn

[S16] C：位操作置位
来源：http://hks.yj202588.top

x |= (1 << 3);
来源：http://dlv.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://zzs.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jhn.redwolf501.top

[S18] C：命令行参数
来源：http://qzq.ppjwa.cn

int main(int argc, char **argv)
来源：http://dcj.tian-w.cn

[S19] C：快速排序
来源：http://crw.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cic.chenjidiqi.icu

[S20] C：二分查找
来源：http://uqy.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ifg.zhoulong.xyz

[S21] C：字符类别判断
来源：http://vdo.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uym.tian-w.cn

[S22] C：字符串转数字
来源：http://huz.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://owy.daxiang520.top

[S23] C：随机数
来源：http://xgk.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://bwq.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://prb.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pkx.sjlbkw.cn

[S25] C：内存拷贝
来源：http://bix.sysykeji.top

memcpy(dst, src, n);
来源：http://vzd.nanxuanxn.top

[S26] C：内存清零
来源：http://kks.fehbvm.com

memset(a, 0, sizeof a);
来源：http://byi.hysaishi.cn

[S27] C：定义常量
来源：http://lyz.tian-w.cn

const double PI = 3.14159;
来源：http://hll.dianchejie.cn

[S28] C：静态变量
来源：http://ywm.jqgfzy.top

static int counter = 0;
来源：http://pkd.kuanghao11.cn

[S29] C：变参函数
来源：http://jxd.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dew.andypj.xyz

[S30] C：头文件保护
来源：http://bqc.xingfuxueyuan.xyz

#ifndef X_H
来源：http://myc.guannengcc.top

#define X_H
来源：http://egi.feifeiyinyue.top

#endif
来源：http://uff.shangyingyoupin.top

[S31] C++：Hello World
来源：http://bag.xylfe.cn

#include <iostream>
来源：http://quz.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://wld.ctjpmb.com

[S32] C++：字符串
来源：http://ayx.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://cgz.havefunace.top

[S33] C++：vector 增删
来源：http://cqz.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://agf.iojbl.cn

[S34] C++：遍历 vector
来源：http://vwz.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://fhq.yj20258888.top

[S35] C++：map
来源：http://eoh.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wpd.pycfn.com

[S36] C++：unordered_map
来源：http://ynr.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://txd.xylfe.cn

[S37] C++：set
来源：http://inf.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jrf.iojbl.cn

[S38] C++：排序
来源：http://pqj.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://spc.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://kfp.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dnb.jiagoushi.top

[S40] C++：查找元素
来源：http://dlg.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aqy.316326.xyz

[S41] C++：类与构造函数
来源：http://ddy.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yki.cheryme.top

[S42] C++：继承与虚函数
来源：http://lai.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://tzh.zhoulong.xyz

[S43] C++：智能指针
来源：http://xiv.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://aqg.andypj.xyz

[S44] C++：引用传参
来源：http://ivu.fzhhl.top

void inc(int &x) { ++x; }
来源：http://gwr.hfpthk.cn

[S45] C++：lambda
来源：http://vgh.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://dvn.ivvv.top

[S46] C++：函数模板
来源：http://mbp.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://klb.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://ned.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://smy.andypj.xyz

[S48] C++：逐行读文件
来源：http://lph.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kuy.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://olp.0kj1m.cn

[S49] C++：写文件
来源：http://jhc.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iae.birdmap.top

[S50] C++：格式化数字
来源：http://arr.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lyb.ybcxt.top

[S51] C++：显式类型转换
来源：http://tku.jiagoushi.top

static_cast<double>(a) / b
来源：http://jyj.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://jns.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://bnw.cashguo.top

[S53] C++：移动语义
来源：http://bsk.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://mzn.ppjwa.cn

[S54] C++：异常处理
来源：http://nlw.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://klx.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://ezy.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hza.zhixingplan.top

[S56] C++：optional
来源：http://epj.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://men.vqdsnc.cn

[S57] C++：编译期常量
来源：http://pkx.sjlbkw.cn

constexpr int N = 10;
来源：http://lys.aibaodan.cn

[S58] C++：命名空间
来源：http://eeb.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://rlz.chenlongwang.top

[S59] C++：静态断言
来源：http://vgg.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xpk.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://qvj.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kbt.sjlbkw.cn

================================================================================
来源：http://ymo.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://goe.zhixingplan.top

================================================================================
来源：http://vop.bbcook.cn

[T01] Kotlin：Hello World
来源：http://qwh.ppjwa.cn

println("Hello")
来源：http://tci.pycfn.com

[T02] Kotlin：变量
来源：http://mii.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fkz.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://hxx.cashguo.top

"值: $b"
来源：http://cel.jyoumei.cn

[T04] Kotlin：空安全
来源：http://hjz.ivvv.top

val n: String? = null;  n?.length
来源：http://sdt.pycfn.com

[T05] Kotlin：when 表达式
来源：http://hae.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xaz.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://lsc.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dht.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://cvh.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ldw.dashuyun.cn

[T08] Kotlin：数据类
来源：http://olz.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://zrn.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://mhg.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://huz.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://kto.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://moe.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://tnp.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://vpq.jianghu66.top

[T12] Kotlin：解构声明
来源：http://vqk.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://evo.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://owc.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://hff.xziqi.cn

[T14] Kotlin：循环
来源：http://sgl.guowangkeji.top

for (i in 1..10) println(i)
来源：http://wqk.aibaodan.cn

[T15] Kotlin：接口
来源：http://kxm.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://sum.sjlbkw.cn

[T16] Swift：Hello World
来源：http://aeo.hammf.cn

print("Hello")
来源：http://bnm.jqgfzy.top

[T17] Swift：变量与常量
来源：http://aiz.birdmap.top

var a = 1;  let b = 2
来源：http://tjz.sweek.top

[T18] Swift：字符串插值
来源：http://ixu.guannengcc.top

"值: \(b)"
来源：http://wof.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://vli.hywenlv.cn

if let n = opt { print(n) }
来源：http://hdd.fengsongda.top

[T20] Swift：数组操作
来源：http://bdd.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://qjb.iojbl.cn

[T21] Swift：遍历
来源：http://fqn.quarkkingdee.top

for x in a { print(x) }
来源：http://kvx.chenlongwang.top

[T22] Swift：字典
来源：http://mgp.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oox.uphjek.com

[T23] Swift：函数
来源：http://mvc.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ahm.smart0.xyz

[T24] Swift：闭包
来源：http://fpm.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://idy.kuanghao11.cn

[T25] Swift：结构体
来源：http://eog.nwbrower.top

struct P { var x: Int }
来源：http://kpd.sysykeji.top

[T26] Swift：类与重写
来源：http://glv.tanke756.top

class A: Base { override func f() {} }
来源：http://mak.shanyushiyangkeji.top

[T27] Swift：错误处理
来源：http://kce.redwolf501.top

do { try f() } catch { print(error) }
来源：http://mlm.hnxiangtu.top

[T28] Swift：枚举
来源：http://wge.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://ycj.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://fvz.chenjidiqi.icu

guard let x = opt else { return }
来源：http://pbg.aizwys.cn

[T30] Swift：协议
来源：http://wqg.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://pqp.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://cox.jianghu66.top

print("Hello")
来源：http://qww.fktsv.cn

[T32] Lua：局部变量
来源：http://wrx.zhaomingkeji.xyz

local a = 1
来源：http://qoz.zdbjq.cn

[T33] Lua：表（数组）
来源：http://ydf.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xns.zhijiandao.cn

[T34] Lua：遍历表
来源：http://nyl.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jgo.shzxlz.cn

[T35] Lua：字典表
来源：http://jlu.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://mew.xuetiantiany.cn

[T36] Lua：函数
来源：http://rcy.yuxming.cn

function add(a, b) return a + b end
来源：http://dto.bjfxy.top

[T37] Lua：字符串拼接
来源：http://yyj.hammf.cn

"a" .. "b"
来源：http://xem.ydjk.org.cn

[T38] Lua：条件
来源：http://mql.0kj1m.cn

if x > 0 then print("正") end
来源：http://jky.epnwcf.com

[T39] Lua：模式匹配
来源：http://bju.cqqwz.cn

string.find(s, "%d+")
来源：http://txi.pengpengdd.cyou

[T40] Lua：元表
来源：http://oml.birdmap.top

setmetatable({}, { __index = base })
来源：http://nov.zycfv.cn

[T41] Perl：Hello World
来源：http://ppz.sjlbkw.cn

print "Hello\n";
来源：http://wez.nanxinkj.top

[T42] Perl：变量类型
来源：http://rmf.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fkz.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://qpy.shuidangran.top

"值: $a"
来源：http://xea.ydjk.org.cn

[T44] Perl：条件
来源：http://zxg.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://vdb.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://rxo.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://jve.jinqigufen.top

[T46] Perl：哈希操作
来源：http://rge.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xba.hcnkem.com

[T47] Perl：正则捕获
来源：http://nqo.nanxuanxn.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://plq.hammf.cn

[T48] Perl：正则替换
来源：http://qop.hywenlv.cn

$s =~ s/old/new/g;
来源：http://ybl.uphjek.com

[T49] Perl：函数
来源：http://gfh.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://loh.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://pzp.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nxf.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://wpt.hesvh.cn

[T51] Scala：Hello World
来源：http://trx.xylfe.cn

println("Hello")
来源：http://mwu.pengpengdd.cyou

[T52] Scala：变量
来源：http://fok.quarkkingdee.top

val a = 1;  var b = 2
来源：http://cid.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://hmn.redwolf501.top

s"值: $b"
来源：http://twk.sysykeji.top

[T54] Scala：集合映射
来源：http://fkq.meibo888.top


<!-- 参考信息 -->