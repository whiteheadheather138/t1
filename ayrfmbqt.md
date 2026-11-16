代发 wailian999

find . -name "*.log" -type f
来源：http://mnh.svipenyu.cn

[R44] 按修改时间查找
来源：http://moc.vehdjk.com

find . -mtime -7 -type f
来源：http://vwb.shuidangran.top

[R45] 批量删除
来源：http://rwn.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://htw.ivvv.top

[R46] 递归替换文件内容
来源：http://pfk.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hfw.zhoulong.xyz

[R47] sed 单行替换
来源：http://ncr.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xxc.gotoacloud.top

[R48] awk 取指定列
来源：http://gdv.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://vuj.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://wqy.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dcb.shzxlz.cn

[R50] awk 求和
来源：http://aru.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://alg.bbcook.cn

[R51] 排序去重取前几
来源：http://xdh.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bun.daria6918.cn

[R52] 统计行数
来源：http://vcw.vehdjk.com

wc -l a.txt
来源：http://lka.yj20258.top

[R53] 查看文件头与实时尾
来源：http://pfo.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ktc.hysaishi.cn

[R54] 比较两个文件
来源：http://rap.andypj.xyz

diff a.txt b.txt
来源：http://lpi.tanke756.top

[R55] 压缩与解压
来源：http://ciu.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rdq.hnqzz.top

[R56] 远程拷贝
来源：http://yay.yuanzhike.top

scp file user@host:/path/
来源：http://xoc.pycfn.com

[R57] 远程执行命令
来源：http://zrw.jiagoushi.top

ssh user@host 'uptime'
来源：http://uxy.cheryme.top

[R58] 下载文件
来源：http://leq.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cip.cdnleiting.top

[R59] 发 POST JSON
来源：http://ahd.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vje.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://xav.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mxd.9152youxi.cn

[R61] 磁盘占用
来源：http://ufu.cashguo.top

df -h;  du -sh *
来源：http://bri.hammf.cn

[R62] 找最占空间的文件
来源：http://ime.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://som.meibo888.top

[R63] 内存与进程
来源：http://qba.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://oqn.yueranfly.top

[R64] 结束进程
来源：http://xfd.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://qfr.tarul.cn

[R65] 查看端口占用
来源：http://aom.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://arg.hongshengwenyu.top

[R66] 定时任务
来源：http://idw.hammf.cn

crontab -e;  crontab -l
来源：http://aik.xylfe.cn

[R67] 生成随机十六进制串
来源：http://lkx.shuidangran.top

openssl rand -hex 16
来源：http://kxb.sufxvd.cn

[R68] 计算文件校验值
来源：http://txs.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://inq.yuxming.cn

[R69] 生成随机密码
来源：http://cre.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://hxh.iojbl.cn

[R70] 时间戳与互转
来源：http://kfy.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://iis.sufxvd.cn

[R71] 日期格式化
来源：http://lmy.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zgx.iojbl.cn

[R72] 等待端口就绪
来源：http://fzc.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ucy.wangdashe.top

[R73] 分割大日志
来源：http://vlf.gogol.net.cn

split -l 1000 big.log part_
来源：http://hsb.snrcjt.cn

[R74] 批量重命名
来源：http://qxs.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ktd.vehdjk.com

[R75] 导出环境变量
来源：http://kut.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://uvm.ppjwa.cn

[R76] 使用临时文件
来源：http://wvk.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uho.wangshuangyany.cn

[R77] 读取用户输入
来源：http://fqq.dashuyun.cn

read -rp "请输入: " ans
来源：http://xar.nanxinkj.top

[R78] 交互式菜单
来源：http://oml.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uoo.uphjek.com

[R79] 解析命令行选项
来源：http://ezp.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gap.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://wac.tarul.cn

time ./run.sh
来源：http://hfq.zhengqikj.top

================================================================================
来源：http://zno.zhongyouzk.top

S. C / C++ 专题
来源：http://zbd.nanxinkj.top

================================================================================
来源：http://pgz.zhongyouzk.top

[S01] C：Hello World
来源：http://wfy.hcnkem.com

#include <stdio.h>
来源：http://irs.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qfr.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://epq.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://jpz.jiagoushi.top

[S03] C：读入整数
来源：http://kvn.cashguo.top

int x; scanf("%d", &x);
来源：http://izg.sxryk.cn

[S04] C：字符串复制
来源：http://lmu.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://fkg.mhx1999.top

[S05] C：字符串长度
来源：http://amd.zhoulong.xyz

strlen(s)
来源：http://lxb.yuxming.cn

[S06] C：字符串比较
来源：http://rmc.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://dtv.xuanzx.com

[S07] C：数组遍历求和
来源：http://ftm.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pmh.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://zzc.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzy.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://rtq.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cvo.316326.xyz

[S10] C：指针与解引用
来源：http://jtz.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://lpw.xylfe.cn

[S11] C：逐行读文件
来源：http://mbv.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://rlx.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ite.shanyushiyangkeji.top

fclose(f);
来源：http://fyc.cdnleiting.top

[S12] C：写文件
来源：http://gjy.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iau.xuetiantiany.cn

[S13] C：宏定义
来源：http://xpd.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uyr.yj202588.top

[S14] C：枚举
来源：http://pid.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rmo.chenjidiqi.icu

[S15] C：类型转换
来源：http://tzl.cheryme.top

(double) a / b
来源：http://mie.snrcjt.cn

[S16] C：位操作置位
来源：http://nns.yongpay.top

x |= (1 << 3);
来源：http://doe.wangdashe.top

[S17] C：安全拼接字符串
来源：http://mtk.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xdu.chenzaomai.com

[S18] C：命令行参数
来源：http://dez.jianghu66.top

int main(int argc, char **argv)
来源：http://uxh.gaohongyu789.top

[S19] C：快速排序
来源：http://leh.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://gfx.kuanghao11.cn

[S20] C：二分查找
来源：http://kxe.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://myb.316326.xyz

[S21] C：字符类别判断
来源：http://iaq.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kbg.sjlbkw.cn

[S22] C：字符串转数字
来源：http://dgf.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://tue.yuanzhike.top

[S23] C：随机数
来源：http://dpq.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xya.tarul.cn

[S24] C：获取本地时间
来源：http://aih.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kux.52xcode.cn

[S25] C：内存拷贝
来源：http://gyn.jqgufenzy.top

memcpy(dst, src, n);
来源：http://keu.0kj1m.cn

[S26] C：内存清零
来源：http://znv.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://wwd.jinqigufen.top

[S27] C：定义常量
来源：http://ema.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://qov.smart0.xyz

[S28] C：静态变量
来源：http://nty.yj202588.top

static int counter = 0;
来源：http://aim.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://iua.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cqv.zhengqikj.top

[S30] C：头文件保护
来源：http://bgp.jinghuilouyu.cn

#ifndef X_H
来源：http://tii.jinyuanbaomall.cn

#define X_H
来源：http://amk.dashuyun.cn

#endif
来源：http://cqv.xuanzx.com

[S31] C++：Hello World
来源：http://cuu.zhaomingkeji.xyz

#include <iostream>
来源：http://ckv.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://oae.epnwcf.com

[S32] C++：字符串
来源：http://vit.cheryme.top

std::string s = "hi";  s += "!";
来源：http://ird.sjlbkw.cn

[S33] C++：vector 增删
来源：http://dvl.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fgg.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://qdc.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://kfk.sufxvd.cn

[S35] C++：map
来源：http://uas.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://brf.sxryk.cn

[S36] C++：unordered_map
来源：http://jpl.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ecv.pycfn.com

[S37] C++：set
来源：http://blt.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ecb.dashuyun.cn

[S38] C++：排序
来源：http://mcf.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://lbg.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://cjx.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rkt.ybcxt.top

[S40] C++：查找元素
来源：http://jof.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pwv.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://zsu.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oyo.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://mwg.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://tvr.gzhubu.top

[S43] C++：智能指针
来源：http://knv.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://onj.wangshuangyany.cn

[S44] C++：引用传参
来源：http://mbk.fengsongda.top

void inc(int &x) { ++x; }
来源：http://ira.yanxiufei.cn

[S45] C++：lambda
来源：http://joe.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wgb.vehdjk.com

[S46] C++：函数模板
来源：http://cbt.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fvx.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://zlb.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://euc.hesvh.cn

[S48] C++：逐行读文件
来源：http://ntx.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://oft.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://lbf.pycfn.com

[S49] C++：写文件
来源：http://ymn.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cez.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://uiv.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hvh.gogol.net.cn

[S51] C++：显式类型转换
来源：http://fgn.hfpthk.cn

static_cast<double>(a) / b
来源：http://tff.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://hvj.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://xmb.sxryk.cn

[S53] C++：移动语义
来源：http://vnz.sweek.top

std::vector<int> w = std::move(v);
来源：http://tzy.cdnleiting.top

[S54] C++：异常处理
来源：http://rdc.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aag.fengsongda.top

[S55] C++：结构化绑定
来源：http://rta.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pht.zhaomingkeji.xyz

[S56] C++：optional
来源：http://xvl.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqw.sufxvd.cn

[S57] C++：编译期常量
来源：http://ehv.cashguo.top

constexpr int N = 10;
来源：http://kta.dashuyun.cn

[S58] C++：命名空间
来源：http://rjh.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://oxc.hcnkem.com

[S59] C++：静态断言
来源：http://nzr.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jhy.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://vmy.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bmq.zycfv.cn

================================================================================
来源：http://dsj.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aqd.xylfe.cn

================================================================================
来源：http://nzy.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://tyw.yongpay.top

println("Hello")
来源：http://sim.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://xpa.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://acy.sweek.top

[T03] Kotlin：字符串模板
来源：http://qqx.jqgufenzy.top

"值: $b"
来源：http://eag.hcnkem.com

[T04] Kotlin：空安全
来源：http://dpr.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://zol.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://vty.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pyp.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://jan.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xml.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://ygk.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfk.yuanzhike.top

[T08] Kotlin：数据类
来源：http://fbf.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://lzz.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://ydf.pycfn.com

fun String.exclaim() = this + "!"
来源：http://kgf.cashguo.top

[T10] Kotlin：默认参数
来源：http://sgr.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qgl.hnqzz.top

[T11] Kotlin：协程
来源：http://pra.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hfz.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://vej.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://bgr.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://icl.daria6918.cn

val m = mapOf("a" to 1)
来源：http://osr.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://puq.sysykeji.top

for (i in 1..10) println(i)
来源：http://rnh.gaohongyu789.top

[T15] Kotlin：接口
来源：http://pqk.fktsv.cn

interface Shape { fun area(): Double }
来源：http://wrq.jinqigfzy.top

[T16] Swift：Hello World
来源：http://xsf.gaohongyu789.top

print("Hello")
来源：http://hpx.gogol.net.cn

[T17] Swift：变量与常量
来源：http://dkz.cashguo.top

var a = 1;  let b = 2
来源：http://sdt.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://ynm.tarul.cn

"值: \(b)"
来源：http://unj.fzhhl.top

[T19] Swift：可选绑定
来源：http://bzt.ehwqpu.com

if let n = opt { print(n) }
来源：http://vyg.sufxvd.cn

[T20] Swift：数组操作
来源：http://edz.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://sly.ehwqpu.com

[T21] Swift：遍历
来源：http://znv.aibaodan.cn

for x in a { print(x) }
来源：http://tui.haohaochexian.top

[T22] Swift：字典
来源：http://von.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mwq.yonumen.top

[T23] Swift：函数
来源：http://zrd.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://elf.nwbrower.top

[T24] Swift：闭包
来源：http://fgn.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://ids.ybcxt.top

[T25] Swift：结构体
来源：http://qhq.chenzaomai.com

struct P { var x: Int }
来源：http://qzn.yueranfly.top

[T26] Swift：类与重写
来源：http://fap.ydzc1.top

class A: Base { override func f() {} }
来源：http://pux.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://cwy.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://hlk.hcnkem.com

[T28] Swift：枚举
来源：http://bja.dianchejie.cn

enum Color { case red, green }
来源：http://knd.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://vmg.fehbvm.com

guard let x = opt else { return }
来源：http://voo.hnqzz.top

[T30] Swift：协议
来源：http://lyi.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://zxv.c1oappe.top

[T31] Lua：Hello World
来源：http://yqy.sufxvd.cn

print("Hello")
来源：http://ljf.zhongyouzk.top

[T32] Lua：局部变量
来源：http://ric.316326.xyz

local a = 1
来源：http://ruv.tanke756.top

[T33] Lua：表（数组）
来源：http://eee.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jgg.gogol.net.cn

[T34] Lua：遍历表
来源：http://dvh.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hib.zhiwuduotai.top

[T35] Lua：字典表
来源：http://rrv.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://jjz.pengpengdd.cyou

[T36] Lua：函数
来源：http://spp.sysykeji.top

function add(a, b) return a + b end
来源：http://usb.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://agg.chenzaomai.com

"a" .. "b"
来源：http://mnd.xuanzx.com

[T38] Lua：条件
来源：http://jnn.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://out.xuanzx.com

[T39] Lua：模式匹配
来源：http://uqh.hesvh.cn

string.find(s, "%d+")
来源：http://hrm.ppjwa.cn

[T40] Lua：元表
来源：http://juo.316326.xyz

setmetatable({}, { __index = base })
来源：http://swo.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://rzh.feifeiyinyue.top

print "Hello\n";
来源：http://asg.gzhubu.top

[T42] Perl：变量类型
来源：http://qdv.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lkc.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://bjk.yj20258888.top

"值: $a"
来源：http://lta.hfpthk.cn

[T44] Perl：条件
来源：http://dze.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://rza.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://oau.cashguo.top

for my $x (@arr) { print $x; }
来源：http://hbq.tian-w.cn

[T46] Perl：哈希操作
来源：http://gic.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fvm.nanxuanxn.top


<!-- 参考信息 -->