代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tlk.316326.xyz

[R56] 远程拷贝
来源：http://ldb.redwolf501.top

scp file user@host:/path/
来源：http://jev.yongpay.top

[R57] 远程执行命令
来源：http://gtw.wangdashe.top

ssh user@host 'uptime'
来源：http://muv.epnwcf.com

[R58] 下载文件
来源：http://vsn.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ztg.cashguo.top

[R59] 发 POST JSON
来源：http://eys.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tsu.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://pht.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mke.ivvv.top

[R61] 磁盘占用
来源：http://zqt.daxiang520.top

df -h;  du -sh *
来源：http://wet.havefunace.top

[R62] 找最占空间的文件
来源：http://fvu.havefunace.top

du -ah . | sort -rh | head -10
来源：http://bqj.iojbl.cn

[R63] 内存与进程
来源：http://cub.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://gik.gogol.net.cn

[R64] 结束进程
来源：http://dgi.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://sim.aizwys.cn

[R65] 查看端口占用
来源：http://iql.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aia.gogol.net.cn

[R66] 定时任务
来源：http://lex.iojbl.cn

crontab -e;  crontab -l
来源：http://vfa.shuidangran.top

[R67] 生成随机十六进制串
来源：http://nni.ydjk.org.cn

openssl rand -hex 16
来源：http://wzg.ctjpmb.com

[R68] 计算文件校验值
来源：http://lmt.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://rqu.zhengqikj.top

[R69] 生成随机密码
来源：http://ysi.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://xbz.zdbjq.cn

[R70] 时间戳与互转
来源：http://ezh.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://wjm.hywenlv.cn

[R71] 日期格式化
来源：http://kzc.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nef.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://qrw.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ftg.sxryk.cn

[R73] 分割大日志
来源：http://dhm.bbcook.cn

split -l 1000 big.log part_
来源：http://mjk.yj20258.top

[R74] 批量重命名
来源：http://nwb.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fzr.hfpthk.cn

[R75] 导出环境变量
来源：http://nzn.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://jsk.nanxuanxn.top

[R76] 使用临时文件
来源：http://mjf.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ouv.cashguo.top

[R77] 读取用户输入
来源：http://oos.yfazqb.com

read -rp "请输入: " ans
来源：http://zka.zycfv.cn

[R78] 交互式菜单
来源：http://uuu.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mzx.hfpthk.cn

[R79] 解析命令行选项
来源：http://idb.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kwm.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://vog.shangyingyoupin.top

time ./run.sh
来源：http://vya.kuanghao11.cn

================================================================================
来源：http://gvm.zdbjq.cn

S. C / C++ 专题
来源：http://ibd.jinqigfzy.top

================================================================================
来源：http://kjl.316326.xyz

[S01] C：Hello World
来源：http://jed.daria6918.cn

#include <stdio.h>
来源：http://uyv.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hsw.yfazqb.com

[S02] C：变量与格式化输出
来源：http://ngm.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://bgy.aizwys.cn

[S03] C：读入整数
来源：http://cqr.aibaodan.cn

int x; scanf("%d", &x);
来源：http://jll.xziqi.cn

[S04] C：字符串复制
来源：http://ypk.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cua.feifeiyinyue.top

[S05] C：字符串长度
来源：http://hml.haohaochexian.top

strlen(s)
来源：http://yka.daxiang520.top

[S06] C：字符串比较
来源：http://ixq.ppjwa.cn

strcmp(a, b) == 0
来源：http://trx.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://fjs.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cal.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://qcd.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://upj.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://xca.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vhg.yuxming.cn

[S10] C：指针与解引用
来源：http://zlb.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://wpe.quarkkingdee.top

[S11] C：逐行读文件
来源：http://fay.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://sci.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lot.zhengqikj.top

fclose(f);
来源：http://vpw.cashguo.top

[S12] C：写文件
来源：http://und.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://esa.cashguo.top

[S13] C：宏定义
来源：http://grm.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvn.aibaodan.cn

[S14] C：枚举
来源：http://ugg.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://bcv.nwbrower.top

[S15] C：类型转换
来源：http://tec.xinyue.icu

(double) a / b
来源：http://rdx.zhijiandao.cn

[S16] C：位操作置位
来源：http://ngd.yj202588.top

x |= (1 << 3);
来源：http://wrw.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://pcf.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iky.hysaishi.cn

[S18] C：命令行参数
来源：http://rwe.guowangkeji.top

int main(int argc, char **argv)
来源：http://qrb.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://clo.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://hae.xylfe.cn

[S20] C：二分查找
来源：http://ppl.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wys.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://rim.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://njw.dashuyun.cn

[S22] C：字符串转数字
来源：http://jda.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://faq.52xcode.cn

[S23] C：随机数
来源：http://pls.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rgs.hcnkem.com

[S24] C：获取本地时间
来源：http://zgo.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xnz.sjlbkw.cn

[S25] C：内存拷贝
来源：http://awv.cashguo.top

memcpy(dst, src, n);
来源：http://qds.nanxinkj.top

[S26] C：内存清零
来源：http://asw.wangdashe.top

memset(a, 0, sizeof a);
来源：http://sby.sjlbkw.cn

[S27] C：定义常量
来源：http://cll.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://zgj.jinqigfzy.top

[S28] C：静态变量
来源：http://jio.zhixingplan.top

static int counter = 0;
来源：http://znj.dashuyun.cn

[S29] C：变参函数
来源：http://hiu.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ctu.shangyingyoupin.top

[S30] C：头文件保护
来源：http://pws.vehdjk.com

#ifndef X_H
来源：http://zma.ywan-chungtsiang.top

#define X_H
来源：http://zmy.ydjk.org.cn

#endif
来源：http://crp.0kj1m.cn

[S31] C++：Hello World
来源：http://usa.0kj1m.cn

#include <iostream>
来源：http://qoy.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://quf.xylfe.cn

[S32] C++：字符串
来源：http://vyh.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://lsu.nanxuanxn.top

[S33] C++：vector 增删
来源：http://xit.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rng.hysaishi.cn

[S34] C++：遍历 vector
来源：http://pju.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://tnp.zdbjq.cn

[S35] C++：map
来源：http://shr.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kcg.yuxming.cn

[S36] C++：unordered_map
来源：http://kmn.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sfq.nanxuanxn.top

[S37] C++：set
来源：http://pds.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tmc.aibaodan.cn

[S38] C++：排序
来源：http://dst.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://ism.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://mek.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://icn.jianghu66.top

[S40] C++：查找元素
来源：http://nsv.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://drs.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://dub.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ste.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://zdw.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://piz.yuxming.cn

[S43] C++：智能指针
来源：http://smk.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://eoa.birdmap.top

[S44] C++：引用传参
来源：http://cjt.birdmap.top

void inc(int &x) { ++x; }
来源：http://mvo.yj20258888.top

[S45] C++：lambda
来源：http://vwd.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://ays.zhongyouzk.top

[S46] C++：函数模板
来源：http://tvx.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lca.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://gyg.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://asc.hnqzz.top

[S48] C++：逐行读文件
来源：http://svv.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mhy.mhx1999.top

while (std::getline(in, line)) { }
来源：http://kew.bjfxy.top

[S49] C++：写文件
来源：http://joj.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uxr.nanxinkj.top

[S50] C++：格式化数字
来源：http://wbd.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhv.ydzc1.top

[S51] C++：显式类型转换
来源：http://div.fzhhl.top

static_cast<double>(a) / b
来源：http://kpm.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://fml.hammf.cn

int size() const noexcept { return n_; }
来源：http://thr.shuidangran.top

[S53] C++：移动语义
来源：http://thw.yj202588.top

std::vector<int> w = std::move(v);
来源：http://wqw.yuxming.cn

[S54] C++：异常处理
来源：http://woa.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pnt.fktsv.cn

[S55] C++：结构化绑定
来源：http://tea.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dcz.sjlbkw.cn

[S56] C++：optional
来源：http://bxv.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oii.zhongyouzk.top

[S57] C++：编译期常量
来源：http://rkj.ehwqpu.com

constexpr int N = 10;
来源：http://ole.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://zhb.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://hwm.bbcook.cn

[S59] C++：静态断言
来源：http://ucw.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://are.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://ksy.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dkn.zhoulong.xyz

================================================================================
来源：http://juh.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wnb.zycfv.cn

================================================================================
来源：http://iuo.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://jeg.sweek.top

println("Hello")
来源：http://vwm.havefunace.top

[T02] Kotlin：变量
来源：http://nti.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vuk.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://fht.yuxming.cn

"值: $b"
来源：http://qwi.sufxvd.cn

[T04] Kotlin：空安全
来源：http://jzz.daxiang520.top

val n: String? = null;  n?.length
来源：http://wgb.birdmap.top

[T05] Kotlin：when 表达式
来源：http://jfz.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pif.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://mrb.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pzn.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://fbs.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ebk.hysaishi.cn

[T08] Kotlin：数据类
来源：http://ych.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://jyw.cheryme.top

[T09] Kotlin：扩展函数
来源：http://yla.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://ner.havefunace.top

[T10] Kotlin：默认参数
来源：http://lff.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vso.shuidangran.top

[T11] Kotlin：协程
来源：http://acf.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fku.zycfv.cn

[T12] Kotlin：解构声明
来源：http://tui.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://uol.cashguo.top

[T13] Kotlin：只读 Map
来源：http://nzu.hesvh.cn

val m = mapOf("a" to 1)
来源：http://omt.uphjek.com

[T14] Kotlin：循环
来源：http://grf.bbcook.cn

for (i in 1..10) println(i)
来源：http://bnr.zhijiandao.cn

[T15] Kotlin：接口
来源：http://lai.wangdashe.top

interface Shape { fun area(): Double }
来源：http://fuj.nanxuanxn.top

[T16] Swift：Hello World
来源：http://ghj.yanxiufei.cn

print("Hello")
来源：http://vri.yongpay.top

[T17] Swift：变量与常量
来源：http://rqv.zhixingplan.top

var a = 1;  let b = 2
来源：http://ywp.xylfe.cn

[T18] Swift：字符串插值
来源：http://kww.gaohongyu789.top

"值: \(b)"
来源：http://azs.ehwqpu.com

[T19] Swift：可选绑定
来源：http://kzl.yanxiufei.cn

if let n = opt { print(n) }
来源：http://mbo.chenlongwang.top

[T20] Swift：数组操作
来源：http://pwp.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://tjf.hammf.cn

[T21] Swift：遍历
来源：http://hfl.yvedp.cn

for x in a { print(x) }
来源：http://akt.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://mxd.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kub.zhongyouzk.top

[T23] Swift：函数
来源：http://zog.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jbm.ydzc1.top

[T24] Swift：闭包
来源：http://isv.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bmk.nanxinkj.top

[T25] Swift：结构体
来源：http://fkz.xylfe.cn

struct P { var x: Int }
来源：http://tnz.nanxuanxn.top

[T26] Swift：类与重写
来源：http://jbi.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://kkt.ydjk.org.cn

[T27] Swift：错误处理
来源：http://zzf.fengsongda.top

do { try f() } catch { print(error) }
来源：http://fsr.yvedp.cn

[T28] Swift：枚举
来源：http://pxy.havefunace.top

enum Color { case red, green }
来源：http://pev.meibo888.top

[T29] Swift：guard 提前返回
来源：http://jeq.ydzc1.top

guard let x = opt else { return }
来源：http://lrb.nanxinkj.top

[T30] Swift：协议
来源：http://vvu.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://jef.xinyue.icu

[T31] Lua：Hello World
来源：http://hml.gogol.net.cn

print("Hello")
来源：http://pfx.sjlbkw.cn

[T32] Lua：局部变量
来源：http://hjb.fengsongda.top

local a = 1
来源：http://whw.hfpthk.cn

[T33] Lua：表（数组）
来源：http://rbf.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ndj.zhijiandao.cn

[T34] Lua：遍历表
来源：http://ima.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bep.yanxiufei.cn

[T35] Lua：字典表
来源：http://opo.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://abj.fktsv.cn

[T36] Lua：函数
来源：http://gvf.yj202588.top

function add(a, b) return a + b end
来源：http://qni.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://wqi.yanxiufei.cn

"a" .. "b"
来源：http://ngz.guowangkeji.top

[T38] Lua：条件
来源：http://wtu.yangfankeji.com

if x > 0 then print("正") end
来源：http://nvr.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://bza.haohaochexian.top

string.find(s, "%d+")
来源：http://saf.yj20258.top

[T40] Lua：元表
来源：http://lcq.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://wns.zhijiandao.cn

[T41] Perl：Hello World
来源：http://ovn.cqqwz.cn

print "Hello\n";
来源：http://xjy.nanxinkj.top

[T42] Perl：变量类型
来源：http://ldy.sjlbkw.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cro.dashuyun.cn

[T43] Perl：字符串插值
来源：http://pbd.aibaodan.cn

"值: $a"
来源：http://nqu.zhoulong.xyz

[T44] Perl：条件
来源：http://dyy.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://qyc.ivvv.top

[T45] Perl：数组遍历
来源：http://fmc.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://vxz.snrcjt.cn

[T46] Perl：哈希操作
来源：http://yvf.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hiw.hesvh.cn

[T47] Perl：正则捕获
来源：http://ykw.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qxx.pycfn.com

[T48] Perl：正则替换
来源：http://rqd.ybcxt.top

$s =~ s/old/new/g;
来源：http://osf.fengsongda.top

[T49] Perl：函数
来源：http://ave.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mcc.yvedp.cn

[T50] Perl：逐行读文件
来源：http://yuy.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://drj.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://vuz.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://kkg.yueranfly.top

println("Hello")
来源：http://eog.yangfankeji.com

[T52] Scala：变量
来源：http://qmw.tarul.cn

val a = 1;  var b = 2
来源：http://qpb.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://lqq.chenzaomai.com

s"值: $b"
来源：http://wpi.zhongyouzk.top

[T54] Scala：集合映射
来源：http://aju.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://mfo.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://ryc.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nnu.pengpengdd.cyou

[T56] Scala：样例类
来源：http://ucn.hcnkem.com

case class User(name: String, age: Int)
来源：http://mjp.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://xbl.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oky.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://igo.yuxming.cn


<!-- 参考信息 -->