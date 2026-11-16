代发 wailian999

find . -name "*.tmp" -delete
来源：http://yea.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://osg.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eau.guannengcc.top

[R47] sed 单行替换
来源：http://dti.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://ahw.cqqwz.cn

[R48] awk 取指定列
来源：http://wdh.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://mfd.ppjwa.cn

[R49] awk 带条件
来源：http://zhl.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qty.wangdashe.top

[R50] awk 求和
来源：http://szz.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://yxk.zhijiandao.cn

[R51] 排序去重取前几
来源：http://shg.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pbp.pycfn.com

[R52] 统计行数
来源：http://dut.yuanzhike.top

wc -l a.txt
来源：http://ybo.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://zel.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ofu.cucudq.cn

[R54] 比较两个文件
来源：http://kul.daxiang520.top

diff a.txt b.txt
来源：http://anp.tanke756.top

[R55] 压缩与解压
来源：http://oaa.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nbw.yanxiufei.cn

[R56] 远程拷贝
来源：http://acc.xziqi.cn

scp file user@host:/path/
来源：http://lon.yongpay.top

[R57] 远程执行命令
来源：http://ttb.fehbvm.com

ssh user@host 'uptime'
来源：http://xyw.sjlbkw.cn

[R58] 下载文件
来源：http://jjm.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qgz.haohaochexian.top

[R59] 发 POST JSON
来源：http://lpl.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://odw.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://xbx.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nqm.mhx1999.top

[R61] 磁盘占用
来源：http://jvu.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://qdm.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://rjw.hammf.cn

du -ah . | sort -rh | head -10
来源：http://ana.pycfn.com

[R63] 内存与进程
来源：http://lgw.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://xtr.gaohongyu789.top

[R64] 结束进程
来源：http://emr.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://qmk.nanxinkj.top

[R65] 查看端口占用
来源：http://rfi.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blz.zhengqikj.top

[R66] 定时任务
来源：http://tvq.havefunace.top

crontab -e;  crontab -l
来源：http://kvq.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://uuc.svipenyu.cn

openssl rand -hex 16
来源：http://boj.fehbvm.com

[R68] 计算文件校验值
来源：http://tik.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ttw.chenjidiqi.icu

[R69] 生成随机密码
来源：http://sjr.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://yky.epnwcf.com

[R70] 时间戳与互转
来源：http://nmk.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://jks.hongshengwenyu.top

[R71] 日期格式化
来源：http://kwl.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://elw.jiagoushi.top

[R72] 等待端口就绪
来源：http://iuq.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rad.yongpay.top

[R73] 分割大日志
来源：http://yzi.guannengcc.top

split -l 1000 big.log part_
来源：http://ytw.jinqigufen.top

[R74] 批量重命名
来源：http://fow.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nyc.jinqigufen.top

[R75] 导出环境变量
来源：http://spg.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://zfx.9152youxi.cn

[R76] 使用临时文件
来源：http://pvu.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jga.tarul.cn

[R77] 读取用户输入
来源：http://xtl.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://ezw.xuetiantiany.cn

[R78] 交互式菜单
来源：http://qig.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sjs.yj20258888.top

[R79] 解析命令行选项
来源：http://sxn.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nni.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://vfi.zdbjq.cn

time ./run.sh
来源：http://myl.xuetiantiany.cn

================================================================================
来源：http://ejk.tian-w.cn

S. C / C++ 专题
来源：http://zav.daria6918.cn

================================================================================
来源：http://rmf.gzhubu.top

[S01] C：Hello World
来源：http://ipv.shangyingyoupin.top

#include <stdio.h>
来源：http://sbo.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vsu.pycfn.com

[S02] C：变量与格式化输出
来源：http://gqz.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://bie.jyoumei.cn

[S03] C：读入整数
来源：http://rev.ppjwa.cn

int x; scanf("%d", &x);
来源：http://htm.vqdsnc.cn

[S04] C：字符串复制
来源：http://gnt.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://dxv.tianlin.xyz

[S05] C：字符串长度
来源：http://aae.sysykeji.top

strlen(s)
来源：http://ymn.bjfxy.top

[S06] C：字符串比较
来源：http://gcj.jiagoushi.top

strcmp(a, b) == 0
来源：http://zxa.ppjwa.cn

[S07] C：数组遍历求和
来源：http://grb.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pcj.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://nrz.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gst.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://blm.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tta.fehbvm.com

[S10] C：指针与解引用
来源：http://qpb.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://iya.zhixingplan.top

[S11] C：逐行读文件
来源：http://ket.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://bby.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vrz.shuidangran.top

fclose(f);
来源：http://wed.xuetiantiany.cn

[S12] C：写文件
来源：http://xsq.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oko.zhiwuduotai.top

[S13] C：宏定义
来源：http://wgo.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agu.yvedp.cn

[S14] C：枚举
来源：http://wlq.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://yzn.kuanghao11.cn

[S15] C：类型转换
来源：http://kba.hnxiangtu.top

(double) a / b
来源：http://jxt.hysaishi.cn

[S16] C：位操作置位
来源：http://dlb.316326.xyz

x |= (1 << 3);
来源：http://lum.xuanzx.com

[S17] C：安全拼接字符串
来源：http://yuz.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ywt.xylfe.cn

[S18] C：命令行参数
来源：http://pqj.hammf.cn

int main(int argc, char **argv)
来源：http://inx.yueranfly.top

[S19] C：快速排序
来源：http://lye.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ziq.cqqwz.cn

[S20] C：二分查找
来源：http://vpq.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://utb.fzhhl.top

[S21] C：字符类别判断
来源：http://tsp.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fhs.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://xuz.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qut.cqqwz.cn

[S23] C：随机数
来源：http://nob.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xas.hnqzz.top

[S24] C：获取本地时间
来源：http://jdi.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tsj.yfazqb.com

[S25] C：内存拷贝
来源：http://cvj.yj20258888.top

memcpy(dst, src, n);
来源：http://lrf.sysykeji.top

[S26] C：内存清零
来源：http://eui.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://tkz.fengsongda.top

[S27] C：定义常量
来源：http://omx.shzxlz.cn

const double PI = 3.14159;
来源：http://xqi.zdqjudy.top

[S28] C：静态变量
来源：http://zbw.yuanzhike.top

static int counter = 0;
来源：http://elb.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://rwr.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kch.uphjek.com

[S30] C：头文件保护
来源：http://cia.hysaishi.cn

#ifndef X_H
来源：http://ric.snrcjt.cn

#define X_H
来源：http://uhz.ehwqpu.com

#endif
来源：http://srm.xziqi.cn

[S31] C++：Hello World
来源：http://crk.sufxvd.cn

#include <iostream>
来源：http://slt.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://kop.iojbl.cn

[S32] C++：字符串
来源：http://oqf.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://akt.tarul.cn

[S33] C++：vector 增删
来源：http://lnb.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bid.ehwqpu.com

[S34] C++：遍历 vector
来源：http://zvm.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://ezk.ywan-chungtsiang.top

[S35] C++：map
来源：http://ukr.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mqg.smart0.xyz

[S36] C++：unordered_map
来源：http://biu.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nth.redwolf501.top

[S37] C++：set
来源：http://yya.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fqr.smart0.xyz

[S38] C++：排序
来源：http://meq.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://wel.yonumen.top

[S39] C++：自定义比较器排序
来源：http://tmj.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://npc.jianghu66.top

[S40] C++：查找元素
来源：http://zlq.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bsm.redwolf501.top

[S41] C++：类与构造函数
来源：http://fjd.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nvb.xinyue.icu

[S42] C++：继承与虚函数
来源：http://rog.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://vxz.ydjk.org.cn

[S43] C++：智能指针
来源：http://nau.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://zyt.shangyingyoupin.top

[S44] C++：引用传参
来源：http://lhd.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://xwj.wangdashe.top

[S45] C++：lambda
来源：http://tml.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lrk.cdnleiting.top

[S46] C++：函数模板
来源：http://npe.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mhf.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://kwv.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sts.shuidangran.top

[S48] C++：逐行读文件
来源：http://iot.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yxt.xinyue.icu

while (std::getline(in, line)) { }
来源：http://brv.0kj1m.cn

[S49] C++：写文件
来源：http://ids.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ydl.xylfe.cn

[S50] C++：格式化数字
来源：http://tgk.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://odv.cucudq.cn

[S51] C++：显式类型转换
来源：http://fzo.fengsongda.top

static_cast<double>(a) / b
来源：http://gpd.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://vhz.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://pma.zhoulong.xyz

[S53] C++：移动语义
来源：http://lil.tanke756.top

std::vector<int> w = std::move(v);
来源：http://qdy.havefunace.top

[S54] C++：异常处理
来源：http://gdz.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbd.ivvv.top

[S55] C++：结构化绑定
来源：http://qoj.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ztw.yuxming.cn

[S56] C++：optional
来源：http://laq.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vmj.xuanzx.com

[S57] C++：编译期常量
来源：http://par.cdnleiting.top

constexpr int N = 10;
来源：http://off.fktsv.cn

[S58] C++：命名空间
来源：http://ssh.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://shh.wangshuangyany.cn

[S59] C++：静态断言
来源：http://nhd.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sco.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://hks.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yyh.snrcjt.cn

================================================================================
来源：http://bzv.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ctc.zhaomingkeji.xyz

================================================================================
来源：http://uhk.ybcxt.top

[T01] Kotlin：Hello World
来源：http://boc.jinghuilouyu.cn

println("Hello")
来源：http://gdo.epnwcf.com

[T02] Kotlin：变量
来源：http://bzd.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lxj.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://btk.jqgfzy.top

"值: $b"
来源：http://wbb.daxiang520.top

[T04] Kotlin：空安全
来源：http://enp.jianghu66.top

val n: String? = null;  n?.length
来源：http://ysk.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://duc.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rfk.52xcode.cn

[T06] Kotlin：集合映射
来源：http://qjh.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vew.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://ijx.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tny.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://xcu.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://jnr.ivvv.top

[T09] Kotlin：扩展函数
来源：http://cfs.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://uoy.yj20258888.top

[T10] Kotlin：默认参数
来源：http://ane.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cos.hfpthk.cn

[T11] Kotlin：协程
来源：http://etx.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ujc.yj202588.top

[T12] Kotlin：解构声明
来源：http://fvq.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://hhj.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://llo.yonumen.top

val m = mapOf("a" to 1)
来源：http://jxa.sysykeji.top

[T14] Kotlin：循环
来源：http://fec.wangdashe.top

for (i in 1..10) println(i)
来源：http://gah.xuanzx.com

[T15] Kotlin：接口
来源：http://key.gzhubu.top

interface Shape { fun area(): Double }
来源：http://qlr.jlsjyb.cn

[T16] Swift：Hello World
来源：http://gej.nwbrower.top

print("Hello")
来源：http://uxy.tianlin.xyz

[T17] Swift：变量与常量
来源：http://zok.yuanzhike.top

var a = 1;  let b = 2
来源：http://yxb.bbcook.cn

[T18] Swift：字符串插值
来源：http://jbc.shanyushiyangtech.top

"值: \(b)"
来源：http://yga.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://inf.fehbvm.com

if let n = opt { print(n) }
来源：http://fdj.hfpthk.cn

[T20] Swift：数组操作
来源：http://bwv.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://ylp.xuanzx.com

[T21] Swift：遍历
来源：http://mfl.pengpengdd.cyou

for x in a { print(x) }
来源：http://bkw.jinghuilouyu.cn

[T22] Swift：字典
来源：http://gss.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://oyd.yj202588.top

[T23] Swift：函数
来源：http://ddg.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pqh.shangyingyoupin.top

[T24] Swift：闭包
来源：http://ssx.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bog.dashuyun.cn

[T25] Swift：结构体
来源：http://bcg.fengsongda.top

struct P { var x: Int }
来源：http://yrl.yonumen.top

[T26] Swift：类与重写
来源：http://mxj.uphjek.com

class A: Base { override func f() {} }
来源：http://ypu.jinqigfzy.top

[T27] Swift：错误处理
来源：http://xwi.andypj.xyz

do { try f() } catch { print(error) }
来源：http://gcg.shuidangran.top

[T28] Swift：枚举
来源：http://xel.daria6918.cn

enum Color { case red, green }
来源：http://svo.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://doq.yj20258.top

guard let x = opt else { return }
来源：http://nuf.hnqzz.top

[T30] Swift：协议
来源：http://uap.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://ukc.svipenyu.cn

[T31] Lua：Hello World
来源：http://pst.chenzaomai.com

print("Hello")
来源：http://qce.ydjk.org.cn

[T32] Lua：局部变量
来源：http://mat.zhongyouzk.top

local a = 1
来源：http://qwe.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://rpt.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://rlu.snrcjt.cn

[T34] Lua：遍历表
来源：http://trc.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bzy.hongshengwenyu.top

[T35] Lua：字典表
来源：http://gct.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://tvi.wangshuangyany.cn

[T36] Lua：函数
来源：http://vmu.c1oappe.top

function add(a, b) return a + b end
来源：http://ydj.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://rhl.sufxvd.cn

"a" .. "b"
来源：http://ltt.c1oappe.top

[T38] Lua：条件
来源：http://ebf.yj20258.top

if x > 0 then print("正") end
来源：http://ruu.chenlongwang.top

[T39] Lua：模式匹配
来源：http://fie.yj20258888.top

string.find(s, "%d+")
来源：http://jfr.iojbl.cn

[T40] Lua：元表
来源：http://rhu.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://gkl.52xcode.cn

[T41] Perl：Hello World
来源：http://qzd.ydjk.org.cn

print "Hello\n";
来源：http://uts.yueranfly.top

[T42] Perl：变量类型
来源：http://tpb.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zkq.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://oqf.aizwys.cn

"值: $a"
来源：http://xhd.mhx1999.top

[T44] Perl：条件
来源：http://frs.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://hmu.jyoumei.cn

[T45] Perl：数组遍历
来源：http://qaf.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://xmy.epnwcf.com

[T46] Perl：哈希操作
来源：http://iag.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bej.haohaochexian.top

[T47] Perl：正则捕获
来源：http://ymz.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xky.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://yuo.yuxming.cn

$s =~ s/old/new/g;
来源：http://weo.aizwys.cn


<!-- 参考信息 -->