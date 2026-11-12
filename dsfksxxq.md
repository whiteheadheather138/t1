代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://gtr.hesvh.cn

[R52] 统计行数
来源：http://rlf.chenjidiqi.icu

wc -l a.txt
来源：http://vxd.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://fwf.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fay.zycfv.cn

[R54] 比较两个文件
来源：http://kba.fzhhl.top

diff a.txt b.txt
来源：http://qit.nanxinkj.top

[R55] 压缩与解压
来源：http://ybw.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulz.zhoulong.xyz

[R56] 远程拷贝
来源：http://duo.tian-w.cn

scp file user@host:/path/
来源：http://epr.yj20258.top

[R57] 远程执行命令
来源：http://olc.zhongyouzk.top

ssh user@host 'uptime'
来源：http://kil.nanxinkj.top

[R58] 下载文件
来源：http://mlz.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zce.dashuyun.cn

[R59] 发 POST JSON
来源：http://qhw.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jja.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://hxj.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ebm.ppjwa.cn

[R61] 磁盘占用
来源：http://nra.cdnleiting.top

df -h;  du -sh *
来源：http://quc.yonumen.top

[R62] 找最占空间的文件
来源：http://iji.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://gfz.xuetiantiany.cn

[R63] 内存与进程
来源：http://qsj.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://oyg.tarul.cn

[R64] 结束进程
来源：http://iak.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://rbo.shzxlz.cn

[R65] 查看端口占用
来源：http://gzt.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ndu.316326.xyz

[R66] 定时任务
来源：http://omd.hysaishi.cn

crontab -e;  crontab -l
来源：http://euh.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://pxj.zhijiandao.cn

openssl rand -hex 16
来源：http://wiy.jinqigfzy.top

[R68] 计算文件校验值
来源：http://vkz.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yhh.sjlbkw.cn

[R69] 生成随机密码
来源：http://rxj.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://wts.zhongyouzk.top

[R70] 时间戳与互转
来源：http://tcv.sweek.top

date +%s;  date -d @1700000000
来源：http://kkd.gzhubu.top

[R71] 日期格式化
来源：http://too.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hvk.jinqigfzy.top

[R72] 等待端口就绪
来源：http://rhz.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wjv.snrcjt.cn

[R73] 分割大日志
来源：http://hpr.wangdashe.top

split -l 1000 big.log part_
来源：http://kif.zhoulong.xyz

[R74] 批量重命名
来源：http://mfc.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://auq.sysykeji.top

[R75] 导出环境变量
来源：http://ale.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://bgo.gotoacloud.top

[R76] 使用临时文件
来源：http://ucw.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ren.xinyue.icu

[R77] 读取用户输入
来源：http://rix.tian-w.cn

read -rp "请输入: " ans
来源：http://yrh.ehwqpu.com

[R78] 交互式菜单
来源：http://nil.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://qwa.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://dwp.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nfw.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://vvm.yanxiufei.cn

time ./run.sh
来源：http://zsv.dashuyun.cn

================================================================================
来源：http://nne.pengpengdd.cyou

S. C / C++ 专题
来源：http://uig.zdqjudy.top

================================================================================
来源：http://fcf.meibo888.top

[S01] C：Hello World
来源：http://zmy.fzhhl.top

#include <stdio.h>
来源：http://rqc.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fzu.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://ztq.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://hjj.jinghuilouyu.cn

[S03] C：读入整数
来源：http://hgv.chenzaomai.com

int x; scanf("%d", &x);
来源：http://tia.yj20258.top

[S04] C：字符串复制
来源：http://bnq.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://nuo.daria6918.cn

[S05] C：字符串长度
来源：http://ede.yueranfly.top

strlen(s)
来源：http://eub.haohaochexian.top

[S06] C：字符串比较
来源：http://yrb.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://wde.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://mkb.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jnv.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://ttd.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zgd.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://zsw.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gae.guannengcc.top

[S10] C：指针与解引用
来源：http://gwx.birdmap.top

int *p = &a;  *p = 5;
来源：http://htp.birdmap.top

[S11] C：逐行读文件
来源：http://ynz.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://bvh.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zzt.jianghu66.top

fclose(f);
来源：http://rxd.redwolf501.top

[S12] C：写文件
来源：http://bia.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://glj.mhx1999.top

[S13] C：宏定义
来源：http://huv.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://snk.hysaishi.cn

[S14] C：枚举
来源：http://cjm.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://suk.hywenlv.cn

[S15] C：类型转换
来源：http://zbo.xinyue.icu

(double) a / b
来源：http://tpj.chenjidiqi.icu

[S16] C：位操作置位
来源：http://swf.guannengcc.top

x |= (1 << 3);
来源：http://ozc.smart0.xyz

[S17] C：安全拼接字符串
来源：http://brf.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nyr.nwbrower.top

[S18] C：命令行参数
来源：http://nbt.aibaodan.cn

int main(int argc, char **argv)
来源：http://qce.yj20258.top

[S19] C：快速排序
来源：http://xhr.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://esj.shanyushiyangtech.top

[S20] C：二分查找
来源：http://qib.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wag.yvedp.cn

[S21] C：字符类别判断
来源：http://nfu.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pwj.gogol.net.cn

[S22] C：字符串转数字
来源：http://dyj.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://yhz.ywan-chungtsiang.top

[S23] C：随机数
来源：http://lli.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mkz.jiagoushi.top

[S24] C：获取本地时间
来源：http://pqv.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kze.sjlbkw.cn

[S25] C：内存拷贝
来源：http://jpw.hnqzz.top

memcpy(dst, src, n);
来源：http://zag.jyoumei.cn

[S26] C：内存清零
来源：http://nje.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://vby.tian-w.cn

[S27] C：定义常量
来源：http://vxz.cdnleiting.top

const double PI = 3.14159;
来源：http://lez.sweek.top

[S28] C：静态变量
来源：http://rvm.gzhubu.top

static int counter = 0;
来源：http://rqq.nanxuanxn.top

[S29] C：变参函数
来源：http://wav.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wnf.hnqzz.top

[S30] C：头文件保护
来源：http://vjg.fktsv.cn

#ifndef X_H
来源：http://ikb.gogol.net.cn

#define X_H
来源：http://rpw.svipenyu.cn

#endif
来源：http://znm.fehbvm.com

[S31] C++：Hello World
来源：http://zps.daxiang520.top

#include <iostream>
来源：http://zoq.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://afv.ydzc1.top

[S32] C++：字符串
来源：http://unt.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://mkv.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://teo.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vjj.9152youxi.cn

[S34] C++：遍历 vector
来源：http://itd.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://cte.snrcjt.cn

[S35] C++：map
来源：http://gav.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fmd.sufxvd.cn

[S36] C++：unordered_map
来源：http://www.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ato.iojbl.cn

[S37] C++：set
来源：http://jgp.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://von.yvedp.cn

[S38] C++：排序
来源：http://kfh.yj202588.top

std::sort(v.begin(), v.end());
来源：http://vpe.yongpay.top

[S39] C++：自定义比较器排序
来源：http://pgs.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bea.guannengcc.top

[S40] C++：查找元素
来源：http://ruf.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gwp.ppjwa.cn

[S41] C++：类与构造函数
来源：http://vca.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mnz.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://bnb.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://isw.redwolf501.top

[S43] C++：智能指针
来源：http://uqd.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://qoa.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://bgw.cheryme.top

void inc(int &x) { ++x; }
来源：http://aei.zycfv.cn

[S45] C++：lambda
来源：http://ukb.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eib.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://kae.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jwt.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://irl.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cyu.ctjpmb.com

[S48] C++：逐行读文件
来源：http://ykf.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://fwf.316326.xyz

while (std::getline(in, line)) { }
来源：http://fos.birdmap.top

[S49] C++：写文件
来源：http://qkw.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vyl.epnwcf.com

[S50] C++：格式化数字
来源：http://dyx.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zxk.jinqigufen.top

[S51] C++：显式类型转换
来源：http://ydl.meibo888.top

static_cast<double>(a) / b
来源：http://yrm.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://iag.pycfn.com

int size() const noexcept { return n_; }
来源：http://vnu.zhiwuduotai.top

[S53] C++：移动语义
来源：http://ryr.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://jub.bbcook.cn

[S54] C++：异常处理
来源：http://iad.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbj.yonumen.top

[S55] C++：结构化绑定
来源：http://oft.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dqq.zhaomingkeji.xyz

[S56] C++：optional
来源：http://qge.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cip.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://bbx.yangfankeji.com

constexpr int N = 10;
来源：http://rcc.gogol.net.cn

[S58] C++：命名空间
来源：http://kep.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://ojl.chenzaomai.com

[S59] C++：静态断言
来源：http://fzc.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dnc.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://wqa.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jnu.iojbl.cn

================================================================================
来源：http://ica.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pec.gogol.net.cn

================================================================================
来源：http://feq.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://jzr.kuanghao11.cn

println("Hello")
来源：http://pbk.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://umx.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qbs.havefunace.top

[T03] Kotlin：字符串模板
来源：http://anu.zhengqikj.top

"值: $b"
来源：http://knt.shuidangran.top

[T04] Kotlin：空安全
来源：http://sjo.tanke756.top

val n: String? = null;  n?.length
来源：http://jmr.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://ylg.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bgp.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://oyc.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ybq.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://rhu.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ucc.hfpthk.cn

[T08] Kotlin：数据类
来源：http://ahk.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://siu.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://phq.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://fwb.xylfe.cn

[T10] Kotlin：默认参数
来源：http://vvs.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://akn.daria6918.cn

[T11] Kotlin：协程
来源：http://jvp.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://igp.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://jqp.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://mxu.yueranfly.top

[T13] Kotlin：只读 Map
来源：http://fzc.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://pjg.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://jfc.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://igz.pycfn.com

[T15] Kotlin：接口
来源：http://mpz.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://idq.sufxvd.cn

[T16] Swift：Hello World
来源：http://bvu.c1oappe.top

print("Hello")
来源：http://vcu.nanxinkj.top

[T17] Swift：变量与常量
来源：http://btf.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://feo.hnqzz.top

[T18] Swift：字符串插值
来源：http://igf.kuanghao11.cn

"值: \(b)"
来源：http://xgm.sweek.top

[T19] Swift：可选绑定
来源：http://xsu.yanxiufei.cn

if let n = opt { print(n) }
来源：http://hew.daria6918.cn

[T20] Swift：数组操作
来源：http://aug.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rhd.meibo888.top

[T21] Swift：遍历
来源：http://tla.hesvh.cn

for x in a { print(x) }
来源：http://aqt.shanyushiyangtech.top

[T22] Swift：字典
来源：http://xyc.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qzu.hywenlv.cn

[T23] Swift：函数
来源：http://auz.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mns.0kj1m.cn

[T24] Swift：闭包
来源：http://ejt.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iyj.nwbrower.top

[T25] Swift：结构体
来源：http://yjm.316326.xyz

struct P { var x: Int }
来源：http://lud.316326.xyz

[T26] Swift：类与重写
来源：http://flk.sufxvd.cn

class A: Base { override func f() {} }
来源：http://ozp.yuanzhike.top

[T27] Swift：错误处理
来源：http://ocm.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://ppd.ydzc1.top

[T28] Swift：枚举
来源：http://zur.gaohongyu789.top

enum Color { case red, green }
来源：http://dbv.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://wyb.jlsjyb.cn

guard let x = opt else { return }
来源：http://sou.shzxlz.cn

[T30] Swift：协议
来源：http://evj.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://ddd.0kj1m.cn

[T31] Lua：Hello World
来源：http://tle.52xcode.cn

print("Hello")
来源：http://nwy.hnxiangtu.top

[T32] Lua：局部变量
来源：http://ffp.haohaochexian.top

local a = 1
来源：http://gov.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://kjo.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pzj.aizwys.cn

[T34] Lua：遍历表
来源：http://bbk.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://edb.guannengcc.top

[T35] Lua：字典表
来源：http://jvu.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://xoz.gaohongyu789.top

[T36] Lua：函数
来源：http://qzc.shuidangran.top

function add(a, b) return a + b end
来源：http://rny.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://fwv.yuxming.cn

"a" .. "b"
来源：http://tui.mhx1999.top

[T38] Lua：条件
来源：http://vys.bjfxy.top

if x > 0 then print("正") end
来源：http://ogc.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://ypw.zhongyouzk.top

string.find(s, "%d+")
来源：http://naw.feifeiyinyue.top

[T40] Lua：元表
来源：http://wjr.sweek.top

setmetatable({}, { __index = base })
来源：http://saf.tanke756.top

[T41] Perl：Hello World
来源：http://pcd.kuanghao11.cn

print "Hello\n";
来源：http://gsx.316326.xyz

[T42] Perl：变量类型
来源：http://vrw.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fez.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://qwx.sysykeji.top

"值: $a"
来源：http://elx.c1oappe.top

[T44] Perl：条件
来源：http://rer.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://oeo.yonumen.top

[T45] Perl：数组遍历
来源：http://atk.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://lrz.bbcook.cn

[T46] Perl：哈希操作
来源：http://uck.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kdd.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://mhm.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ill.vehdjk.com

[T48] Perl：正则替换
来源：http://zkh.zycfv.cn

$s =~ s/old/new/g;
来源：http://hai.xuetiantiany.cn

[T49] Perl：函数
来源：http://reo.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://scj.mhx1999.top

[T50] Perl：逐行读文件
来源：http://bvw.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nqp.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://wwl.xylfe.cn

[T51] Scala：Hello World
来源：http://ozi.haohaochexian.top

println("Hello")
来源：http://psn.9152youxi.cn

[T52] Scala：变量
来源：http://gqq.fktsv.cn

val a = 1;  var b = 2
来源：http://bvt.jinqigufen.top

[T53] Scala：字符串插值
来源：http://klp.52xcode.cn

s"值: $b"
来源：http://xkb.sysykeji.top

[T54] Scala：集合映射
来源：http://xoo.bjfxy.top


<!-- 参考信息 -->