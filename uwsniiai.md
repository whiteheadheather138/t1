代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iwf.quarkkingdee.top

[R54] 比较两个文件
来源：http://cya.cqqwz.cn

diff a.txt b.txt
来源：http://qss.hywenlv.cn

[R55] 压缩与解压
来源：http://cea.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hpa.9152youxi.cn

[R56] 远程拷贝
来源：http://cls.xinyue.icu

scp file user@host:/path/
来源：http://tnz.kuanghao11.cn

[R57] 远程执行命令
来源：http://obj.316326.xyz

ssh user@host 'uptime'
来源：http://lib.cheryme.top

[R58] 下载文件
来源：http://mdg.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pse.chenlongwang.top

[R59] 发 POST JSON
来源：http://pqc.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dfv.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://wko.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oxj.shangyingyoupin.top

[R61] 磁盘占用
来源：http://rll.0kj1m.cn

df -h;  du -sh *
来源：http://arr.zycfv.cn

[R62] 找最占空间的文件
来源：http://fjv.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://yum.sjlbkw.cn

[R63] 内存与进程
来源：http://szk.uphjek.com

free -h;  ps aux | grep nginx
来源：http://usb.fehbvm.com

[R64] 结束进程
来源：http://dsu.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://xfc.gzhubu.top

[R65] 查看端口占用
来源：http://csz.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nrn.jqgfzy.top

[R66] 定时任务
来源：http://icq.wangdashe.top

crontab -e;  crontab -l
来源：http://vbh.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://fzj.ctjpmb.com

openssl rand -hex 16
来源：http://fgo.gogol.net.cn

[R68] 计算文件校验值
来源：http://dse.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://ksf.hfpthk.cn

[R69] 生成随机密码
来源：http://pfu.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://qzj.hywenlv.cn

[R70] 时间戳与互转
来源：http://akp.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://zxz.tian-w.cn

[R71] 日期格式化
来源：http://mda.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yax.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://fxb.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nay.sufxvd.cn

[R73] 分割大日志
来源：http://iar.dashuyun.cn

split -l 1000 big.log part_
来源：http://kfj.jianghu66.top

[R74] 批量重命名
来源：http://myo.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbu.fengsongda.top

[R75] 导出环境变量
来源：http://nir.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zny.0kj1m.cn

[R76] 使用临时文件
来源：http://nzd.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vsh.xuanzx.com

[R77] 读取用户输入
来源：http://kyl.gogol.net.cn

read -rp "请输入: " ans
来源：http://xqp.9152youxi.cn

[R78] 交互式菜单
来源：http://ejv.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rge.zhongyouzk.top

[R79] 解析命令行选项
来源：http://wzu.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cqv.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://uuk.fehbvm.com

time ./run.sh
来源：http://qlq.jyoumei.cn

================================================================================
来源：http://xgn.daria6918.cn

S. C / C++ 专题
来源：http://nio.bbcook.cn

================================================================================
来源：http://kfh.feifeiyinyue.top

[S01] C：Hello World
来源：http://tpg.wangshuangyany.cn

#include <stdio.h>
来源：http://esv.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfn.ivvv.top

[S02] C：变量与格式化输出
来源：http://hbh.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://fno.nanxuanxn.top

[S03] C：读入整数
来源：http://ttz.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://vur.zhengqikj.top

[S04] C：字符串复制
来源：http://lem.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://nha.jinqigufen.top

[S05] C：字符串长度
来源：http://ryy.zhaomingkeji.xyz

strlen(s)
来源：http://ymu.ctjpmb.com

[S06] C：字符串比较
来源：http://vqn.cucudq.cn

strcmp(a, b) == 0
来源：http://ehz.dianchejie.cn

[S07] C：数组遍历求和
来源：http://ruy.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://quv.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://txj.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jcr.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://iez.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xqa.zdbjq.cn

[S10] C：指针与解引用
来源：http://jbc.iojbl.cn

int *p = &a;  *p = 5;
来源：http://qzw.316326.xyz

[S11] C：逐行读文件
来源：http://btr.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://gor.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dix.cqqwz.cn

fclose(f);
来源：http://gtd.quarkkingdee.top

[S12] C：写文件
来源：http://mvq.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://int.zhijiandao.cn

[S13] C：宏定义
来源：http://dsb.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://knk.gaohongyu789.top

[S14] C：枚举
来源：http://qmu.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://cab.tanke756.top

[S15] C：类型转换
来源：http://dhh.daria6918.cn

(double) a / b
来源：http://mtt.gaohongyu789.top

[S16] C：位操作置位
来源：http://gzp.kuanghao11.cn

x |= (1 << 3);
来源：http://eoj.pycfn.com

[S17] C：安全拼接字符串
来源：http://ovu.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hli.birdmap.top

[S18] C：命令行参数
来源：http://wow.sweek.top

int main(int argc, char **argv)
来源：http://syx.hfpthk.cn

[S19] C：快速排序
来源：http://pkg.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://rkh.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://gvk.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vui.cqqwz.cn

[S21] C：字符类别判断
来源：http://wkk.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tyo.yangfankeji.com

[S22] C：字符串转数字
来源：http://bfj.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pss.chenjidiqi.icu

[S23] C：随机数
来源：http://pyu.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zsk.wangdashe.top

[S24] C：获取本地时间
来源：http://kcm.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fji.tian-w.cn

[S25] C：内存拷贝
来源：http://hkt.smart0.xyz

memcpy(dst, src, n);
来源：http://pih.jiagoushi.top

[S26] C：内存清零
来源：http://gpk.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://paf.zhijiandao.cn

[S27] C：定义常量
来源：http://qsr.uphjek.com

const double PI = 3.14159;
来源：http://zmv.guannengcc.top

[S28] C：静态变量
来源：http://zqa.yfazqb.com

static int counter = 0;
来源：http://psk.jiagoushi.top

[S29] C：变参函数
来源：http://pdj.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwc.meibo888.top

[S30] C：头文件保护
来源：http://tnt.sysykeji.top

#ifndef X_H
来源：http://lcr.tanke756.top

#define X_H
来源：http://eyi.yanxiufei.cn

#endif
来源：http://hwo.9152youxi.cn

[S31] C++：Hello World
来源：http://btq.hammf.cn

#include <iostream>
来源：http://jpz.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://vky.ybcxt.top

[S32] C++：字符串
来源：http://rfj.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://rwr.9152youxi.cn

[S33] C++：vector 增删
来源：http://xdj.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhc.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://ngg.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://blr.jinqigfzy.top

[S35] C++：map
来源：http://hvp.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pdr.iojbl.cn

[S36] C++：unordered_map
来源：http://bed.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://miy.yuanzhike.top

[S37] C++：set
来源：http://mlw.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tlf.redwolf501.top

[S38] C++：排序
来源：http://gbd.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://uxg.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://ugo.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pez.bbcook.cn

[S40] C++：查找元素
来源：http://oda.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wco.yongpay.top

[S41] C++：类与构造函数
来源：http://hbv.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwu.aizwys.cn

[S42] C++：继承与虚函数
来源：http://asx.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://ngi.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://kil.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://csy.c1oappe.top

[S44] C++：引用传参
来源：http://hzc.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://rvt.9152youxi.cn

[S45] C++：lambda
来源：http://wgo.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oeh.havefunace.top

[S46] C++：函数模板
来源：http://ypk.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://swg.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://yjz.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jtb.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://ldr.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://edz.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://lxh.jlsjyb.cn

[S49] C++：写文件
来源：http://oao.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ywd.yfazqb.com

[S50] C++：格式化数字
来源：http://muo.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rfl.yj20258.top

[S51] C++：显式类型转换
来源：http://rpf.bjfxy.top

static_cast<double>(a) / b
来源：http://hhf.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://mwm.xinyue.icu

int size() const noexcept { return n_; }
来源：http://tex.hnqzz.top

[S53] C++：移动语义
来源：http://lau.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://apd.cashguo.top

[S54] C++：异常处理
来源：http://kgk.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ozk.yuxming.cn

[S55] C++：结构化绑定
来源：http://qhc.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rft.shzxlz.cn

[S56] C++：optional
来源：http://arf.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://adl.shuidangran.top

[S57] C++：编译期常量
来源：http://zhl.fktsv.cn

constexpr int N = 10;
来源：http://zkh.andypj.xyz

[S58] C++：命名空间
来源：http://ejh.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://fqx.fengsongda.top

[S59] C++：静态断言
来源：http://hrw.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fzk.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://qrk.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zky.redwolf501.top

================================================================================
来源：http://ein.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://haz.52xcode.cn

================================================================================
来源：http://dmg.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://abz.shzxlz.cn

println("Hello")
来源：http://ywe.fktsv.cn

[T02] Kotlin：变量
来源：http://qfe.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xes.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://yct.zdbjq.cn

"值: $b"
来源：http://dhr.ydzc1.top

[T04] Kotlin：空安全
来源：http://kko.fehbvm.com

val n: String? = null;  n?.length
来源：http://jrt.sweek.top

[T05] Kotlin：when 表达式
来源：http://nzg.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vjw.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://uxr.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://jvw.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://wng.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kib.hysaishi.cn

[T08] Kotlin：数据类
来源：http://nic.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://rla.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://dqm.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://dlg.aizwys.cn

[T10] Kotlin：默认参数
来源：http://njf.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uwe.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://jmf.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://nmr.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://mkl.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://ake.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://usf.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://rwt.hcnkem.com

[T14] Kotlin：循环
来源：http://tla.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://ero.nwbrower.top

[T15] Kotlin：接口
来源：http://sxu.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://ugc.vehdjk.com

[T16] Swift：Hello World
来源：http://mpt.xylfe.cn

print("Hello")
来源：http://vxm.vehdjk.com

[T17] Swift：变量与常量
来源：http://xfq.aibaodan.cn

var a = 1;  let b = 2
来源：http://ydg.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://rdx.ctjpmb.com

"值: \(b)"
来源：http://ikp.daxiang520.top

[T19] Swift：可选绑定
来源：http://cxe.xuanzx.com

if let n = opt { print(n) }
来源：http://ivy.ppjwa.cn

[T20] Swift：数组操作
来源：http://ggg.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uaq.nanxuanxn.top

[T21] Swift：遍历
来源：http://pyv.nanxuanxn.top

for x in a { print(x) }
来源：http://dxx.ydjk.org.cn

[T22] Swift：字典
来源：http://kpr.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://fak.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://xmb.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://trw.jyoumei.cn

[T24] Swift：闭包
来源：http://hdu.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bpl.ppjwa.cn

[T25] Swift：结构体
来源：http://qfg.gzhubu.top

struct P { var x: Int }
来源：http://kmn.sufxvd.cn

[T26] Swift：类与重写
来源：http://zvq.hysaishi.cn

class A: Base { override func f() {} }
来源：http://uny.yongpay.top

[T27] Swift：错误处理
来源：http://vnl.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://osu.sufxvd.cn

[T28] Swift：枚举
来源：http://bng.sufxvd.cn

enum Color { case red, green }
来源：http://iwh.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://rce.vehdjk.com

guard let x = opt else { return }
来源：http://kgm.yj20258.top

[T30] Swift：协议
来源：http://mkn.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://msz.sjlbkw.cn

[T31] Lua：Hello World
来源：http://xlv.vqdsnc.cn

print("Hello")
来源：http://nxl.gotoacloud.top

[T32] Lua：局部变量
来源：http://qxq.cucudq.cn

local a = 1
来源：http://lhf.daxiang520.top

[T33] Lua：表（数组）
来源：http://mev.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://inq.hnqzz.top

[T34] Lua：遍历表
来源：http://sqp.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xnt.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://jvl.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://hqg.yj202588.top

[T36] Lua：函数
来源：http://vcq.tianlin.xyz

function add(a, b) return a + b end
来源：http://njk.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://vbl.cqqwz.cn

"a" .. "b"
来源：http://zrj.vqdsnc.cn

[T38] Lua：条件
来源：http://jpk.316326.xyz

if x > 0 then print("正") end
来源：http://ghv.aizwys.cn

[T39] Lua：模式匹配
来源：http://rbr.daxiang520.top

string.find(s, "%d+")
来源：http://eop.hammf.cn

[T40] Lua：元表
来源：http://mdj.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://ocr.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://khg.pycfn.com

print "Hello\n";
来源：http://hib.nwbrower.top

[T42] Perl：变量类型
来源：http://dgd.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dbq.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://gru.yuanzhike.top

"值: $a"
来源：http://sne.gzhubu.top

[T44] Perl：条件
来源：http://hep.sweek.top

if ($a > 0) { print "正"; }
来源：http://cns.birdmap.top

[T45] Perl：数组遍历
来源：http://rry.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://wwx.fengsongda.top

[T46] Perl：哈希操作
来源：http://tcx.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ckc.cashguo.top

[T47] Perl：正则捕获
来源：http://tmb.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pfs.zhengqikj.top

[T48] Perl：正则替换
来源：http://nsr.daria6918.cn

$s =~ s/old/new/g;
来源：http://suq.zhixingplan.top

[T49] Perl：函数
来源：http://dae.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://all.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://gsw.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bjt.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://dos.zdbjq.cn

[T51] Scala：Hello World
来源：http://ooo.sysykeji.top

println("Hello")
来源：http://zcw.hcnkem.com

[T52] Scala：变量
来源：http://lek.gotoacloud.top

val a = 1;  var b = 2
来源：http://fgh.fehbvm.com

[T53] Scala：字符串插值
来源：http://gyv.gzhubu.top

s"值: $b"
来源：http://aju.cdnleiting.top

[T54] Scala：集合映射
来源：http://eor.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://wup.jyoumei.cn

[T55] Scala：集合过滤
来源：http://vpg.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vma.jyoumei.cn

[T56] Scala：样例类
来源：http://hmy.wangshuangyany.cn


<!-- 参考信息 -->