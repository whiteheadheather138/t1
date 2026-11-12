代发 wailian999

find . -name "*.log" -type f
来源：http://ssk.0kj1m.cn

[R44] 按修改时间查找
来源：http://eeo.quarkkingdee.top

find . -mtime -7 -type f
来源：http://aqa.zdqjudy.top

[R45] 批量删除
来源：http://pwd.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://wry.vehdjk.com

[R46] 递归替换文件内容
来源：http://ybw.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cxa.svipenyu.cn

[R47] sed 单行替换
来源：http://epa.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://ukv.yongpay.top

[R48] awk 取指定列
来源：http://tna.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://hfy.zycfv.cn

[R49] awk 带条件
来源：http://dpo.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fet.uphjek.com

[R50] awk 求和
来源：http://qob.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lqq.vqdsnc.cn

[R51] 排序去重取前几
来源：http://mgs.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ejg.zhaomingkeji.xyz

[R52] 统计行数
来源：http://xly.zhijiandao.cn

wc -l a.txt
来源：http://mcs.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://zrl.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gwz.zdqjudy.top

[R54] 比较两个文件
来源：http://eow.yfazqb.com

diff a.txt b.txt
来源：http://bcp.sysykeji.top

[R55] 压缩与解压
来源：http://wkg.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aiz.jlsjyb.cn

[R56] 远程拷贝
来源：http://dck.zhongyouzk.top

scp file user@host:/path/
来源：http://akg.xziqi.cn

[R57] 远程执行命令
来源：http://qef.316326.xyz

ssh user@host 'uptime'
来源：http://wgq.guannengcc.top

[R58] 下载文件
来源：http://rvv.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sax.andypj.xyz

[R59] 发 POST JSON
来源：http://kba.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srf.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://qfd.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xek.hongshengwenyu.top

[R61] 磁盘占用
来源：http://moh.yj202588.top

df -h;  du -sh *
来源：http://boy.yonumen.top

[R62] 找最占空间的文件
来源：http://unt.yj202588.top

du -ah . | sort -rh | head -10
来源：http://jla.hywenlv.cn

[R63] 内存与进程
来源：http://tkf.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://cey.sysykeji.top

[R64] 结束进程
来源：http://oct.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://jfd.hesvh.cn

[R65] 查看端口占用
来源：http://uqf.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ptb.yfazqb.com

[R66] 定时任务
来源：http://dfk.ctjpmb.com

crontab -e;  crontab -l
来源：http://ptx.wangdashe.top

[R67] 生成随机十六进制串
来源：http://lxe.yj20258.top

openssl rand -hex 16
来源：http://hrh.bjfxy.top

[R68] 计算文件校验值
来源：http://vup.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://ntl.aibaodan.cn

[R69] 生成随机密码
来源：http://wva.0kj1m.cn

head -c 16 /dev/urandom | base64
来源：http://utq.tanke756.top

[R70] 时间戳与互转
来源：http://cdk.yongpay.top

date +%s;  date -d @1700000000
来源：http://zyj.zhoulong.xyz

[R71] 日期格式化
来源：http://thr.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lwi.zdbjq.cn

[R72] 等待端口就绪
来源：http://yzn.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ecr.zhixingplan.top

[R73] 分割大日志
来源：http://koc.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://irr.zhiwuduotai.top

[R74] 批量重命名
来源：http://qch.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wok.gaohongyu789.top

[R75] 导出环境变量
来源：http://uud.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://msz.guowangkeji.top

[R76] 使用临时文件
来源：http://gxr.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kaf.pengpengdd.cyou

[R77] 读取用户输入
来源：http://gwa.nwbrower.top

read -rp "请输入: " ans
来源：http://myj.jyoumei.cn

[R78] 交互式菜单
来源：http://tab.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eco.fktsv.cn

[R79] 解析命令行选项
来源：http://twg.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://heb.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://yyt.zhijiandao.cn

time ./run.sh
来源：http://ctx.chenjidiqi.icu

================================================================================
来源：http://ord.zhixingplan.top

S. C / C++ 专题
来源：http://ger.gzhubu.top

================================================================================
来源：http://tgj.ydzc1.top

[S01] C：Hello World
来源：http://tvp.havefunace.top

#include <stdio.h>
来源：http://qvz.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ogg.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://wtg.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://abl.haohaochexian.top

[S03] C：读入整数
来源：http://edq.fktsv.cn

int x; scanf("%d", &x);
来源：http://oka.yongpay.top

[S04] C：字符串复制
来源：http://dot.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://loq.nanxinkj.top

[S05] C：字符串长度
来源：http://leq.fzhhl.top

strlen(s)
来源：http://djk.316326.xyz

[S06] C：字符串比较
来源：http://ysb.cheryme.top

strcmp(a, b) == 0
来源：http://pkl.nwbrower.top

[S07] C：数组遍历求和
来源：http://cem.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mrm.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://nje.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xaz.tarul.cn

[S09] C：结构体定义与初始化
来源：http://vvu.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://etf.pycfn.com

[S10] C：指针与解引用
来源：http://hqg.fktsv.cn

int *p = &a;  *p = 5;
来源：http://ico.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://qbd.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://hke.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyl.yanxiufei.cn

fclose(f);
来源：http://mgl.zhongyouzk.top

[S12] C：写文件
来源：http://yjq.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tkz.shzxlz.cn

[S13] C：宏定义
来源：http://inr.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qnv.gogol.net.cn

[S14] C：枚举
来源：http://kbn.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://jrc.epnwcf.com

[S15] C：类型转换
来源：http://usp.dianchejie.cn

(double) a / b
来源：http://rdx.hesvh.cn

[S16] C：位操作置位
来源：http://jma.aizwys.cn

x |= (1 << 3);
来源：http://kbu.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://yge.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syn.kuanghao11.cn

[S18] C：命令行参数
来源：http://yvr.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://riy.yueranfly.top

[S19] C：快速排序
来源：http://sdn.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://thv.hysaishi.cn

[S20] C：二分查找
来源：http://xwi.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nsq.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://wbm.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jdu.c1oappe.top

[S22] C：字符串转数字
来源：http://cma.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xvj.sweek.top

[S23] C：随机数
来源：http://jxd.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fma.fktsv.cn

[S24] C：获取本地时间
来源：http://ljs.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kfk.yanxiufei.cn

[S25] C：内存拷贝
来源：http://isz.fktsv.cn

memcpy(dst, src, n);
来源：http://wye.guowangkeji.top

[S26] C：内存清零
来源：http://leg.yfazqb.com

memset(a, 0, sizeof a);
来源：http://lvv.iojbl.cn

[S27] C：定义常量
来源：http://vjc.hysaishi.cn

const double PI = 3.14159;
来源：http://ocd.chenlongwang.top

[S28] C：静态变量
来源：http://fcb.jinyuanbaomall.cn

static int counter = 0;
来源：http://qmr.yanxiufei.cn

[S29] C：变参函数
来源：http://deb.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hdz.tian-w.cn

[S30] C：头文件保护
来源：http://juu.zdqjudy.top

#ifndef X_H
来源：http://esv.gaohongyu789.top

#define X_H
来源：http://kfp.chenlongwang.top

#endif
来源：http://gih.yangfankeji.com

[S31] C++：Hello World
来源：http://zwq.ctjpmb.com

#include <iostream>
来源：http://ptx.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://izy.jinghuilouyu.cn

[S32] C++：字符串
来源：http://dhc.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://dct.cashguo.top

[S33] C++：vector 增删
来源：http://bbn.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://quw.sufxvd.cn

[S34] C++：遍历 vector
来源：http://zyw.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://pjo.zhiwuduotai.top

[S35] C++：map
来源：http://ygs.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hip.hammf.cn

[S36] C++：unordered_map
来源：http://ngp.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://his.316326.xyz

[S37] C++：set
来源：http://jxi.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nff.jlsjyb.cn

[S38] C++：排序
来源：http://vwf.tarul.cn

std::sort(v.begin(), v.end());
来源：http://hud.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://wvy.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mvv.xinyue.icu

[S40] C++：查找元素
来源：http://sqe.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://inn.nwbrower.top

[S41] C++：类与构造函数
来源：http://fdu.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://php.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://ume.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://xso.jqgfzy.top

[S43] C++：智能指针
来源：http://gxt.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://izb.gotoacloud.top

[S44] C++：引用传参
来源：http://oto.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://agw.gzhubu.top

[S45] C++：lambda
来源：http://eyq.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://ugb.9152youxi.cn

[S46] C++：函数模板
来源：http://xfg.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sjv.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://xem.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dwv.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://frj.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://cra.bbcook.cn

while (std::getline(in, line)) { }
来源：http://abj.redwolf501.top

[S49] C++：写文件
来源：http://ypa.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klm.nanxuanxn.top

[S50] C++：格式化数字
来源：http://iww.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ada.chenlongwang.top

[S51] C++：显式类型转换
来源：http://ayo.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://wph.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://wkb.fengsongda.top

int size() const noexcept { return n_; }
来源：http://zfm.yangfankeji.com

[S53] C++：移动语义
来源：http://nto.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://csd.tarul.cn

[S54] C++：异常处理
来源：http://cgp.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vwg.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://fpr.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tsh.guowangkeji.top

[S56] C++：optional
来源：http://ktm.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fwa.tianlin.xyz

[S57] C++：编译期常量
来源：http://odu.havefunace.top

constexpr int N = 10;
来源：http://xqt.birdmap.top

[S58] C++：命名空间
来源：http://kzp.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://hbz.jianghu66.top

[S59] C++：静态断言
来源：http://thp.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cto.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://ano.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eku.zdbjq.cn

================================================================================
来源：http://pnb.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fug.shanyushiyangtech.top

================================================================================
来源：http://ral.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://pfm.9152youxi.cn

println("Hello")
来源：http://hmc.yj202588.top

[T02] Kotlin：变量
来源：http://cbz.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bal.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://ulz.yueranfly.top

"值: $b"
来源：http://haw.zhixingplan.top

[T04] Kotlin：空安全
来源：http://gxi.meibo888.top

val n: String? = null;  n?.length
来源：http://hbp.birdmap.top

[T05] Kotlin：when 表达式
来源：http://imv.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nlq.sysykeji.top

[T06] Kotlin：集合映射
来源：http://cxq.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://quj.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://qjg.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cdo.yfazqb.com

[T08] Kotlin：数据类
来源：http://dlc.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://azv.pycfn.com

[T09] Kotlin：扩展函数
来源：http://jum.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://uxq.ybcxt.top

[T10] Kotlin：默认参数
来源：http://zyr.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uak.zhongyouzk.top

[T11] Kotlin：协程
来源：http://cqc.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wdg.tian-w.cn

[T12] Kotlin：解构声明
来源：http://fjd.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://isl.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://ruv.smart0.xyz

val m = mapOf("a" to 1)
来源：http://lev.fzhhl.top

[T14] Kotlin：循环
来源：http://gnn.gotoacloud.top

for (i in 1..10) println(i)
来源：http://bvi.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://wod.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://dub.zhixingplan.top

[T16] Swift：Hello World
来源：http://aqc.yanxiufei.cn

print("Hello")
来源：http://fej.zdbjq.cn

[T17] Swift：变量与常量
来源：http://eis.dianchejie.cn

var a = 1;  let b = 2
来源：http://pfn.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://jue.cashguo.top

"值: \(b)"
来源：http://ynp.zhengqikj.top

[T19] Swift：可选绑定
来源：http://njf.nanxuanxn.top

if let n = opt { print(n) }
来源：http://laa.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://xlu.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wqf.hongshengwenyu.top

[T21] Swift：遍历
来源：http://ofh.yueranfly.top

for x in a { print(x) }
来源：http://xsn.9152youxi.cn

[T22] Swift：字典
来源：http://xrg.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rel.haohaochexian.top

[T23] Swift：函数
来源：http://ezn.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://klx.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://ish.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rkg.ehwqpu.com

[T25] Swift：结构体
来源：http://lkv.yj20258.top

struct P { var x: Int }
来源：http://wtk.yfazqb.com

[T26] Swift：类与重写
来源：http://ekd.yongpay.top

class A: Base { override func f() {} }
来源：http://zzz.cashguo.top

[T27] Swift：错误处理
来源：http://nzt.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://kqw.bbcook.cn

[T28] Swift：枚举
来源：http://mzz.0kj1m.cn

enum Color { case red, green }
来源：http://dft.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://oga.fengsongda.top

guard let x = opt else { return }
来源：http://hzj.tianlin.xyz

[T30] Swift：协议
来源：http://mky.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://mpd.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://nvu.zhiwuduotai.top

print("Hello")
来源：http://afw.gotoacloud.top

[T32] Lua：局部变量
来源：http://ygn.pengpengdd.cyou

local a = 1
来源：http://yet.hysaishi.cn

[T33] Lua：表（数组）
来源：http://yrn.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lod.sufxvd.cn

[T34] Lua：遍历表
来源：http://lhw.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zgj.ydzc1.top

[T35] Lua：字典表
来源：http://xpp.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://roe.yanxiufei.cn

[T36] Lua：函数
来源：http://hld.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://gkj.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://lfj.fzhhl.top

"a" .. "b"
来源：http://gka.epnwcf.com

[T38] Lua：条件
来源：http://jkm.zhengqikj.top

if x > 0 then print("正") end
来源：http://zsp.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://gdk.c1oappe.top

string.find(s, "%d+")
来源：http://aww.quarkkingdee.top

[T40] Lua：元表
来源：http://exi.fengsongda.top

setmetatable({}, { __index = base })
来源：http://hfg.guowangkeji.top

[T41] Perl：Hello World
来源：http://wvi.ctjpmb.com

print "Hello\n";
来源：http://wvw.jianghu66.top

[T42] Perl：变量类型
来源：http://kie.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rns.gzhubu.top

[T43] Perl：字符串插值
来源：http://gjb.cdnleiting.top

"值: $a"
来源：http://baj.cheryme.top

[T44] Perl：条件
来源：http://iez.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://bna.gogol.net.cn

[T45] Perl：数组遍历
来源：http://jzf.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://ftt.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://oeq.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jga.sxryk.cn


<!-- 参考信息 -->