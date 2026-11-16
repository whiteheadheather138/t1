代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://yzd.aibaodan.cn

[R52] 统计行数
来源：http://fzs.tanke756.top

wc -l a.txt
来源：http://rav.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://gvq.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tuv.chenzaomai.com

[R54] 比较两个文件
来源：http://qlp.sweek.top

diff a.txt b.txt
来源：http://uej.9152youxi.cn

[R55] 压缩与解压
来源：http://pra.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://glr.bbcook.cn

[R56] 远程拷贝
来源：http://leu.hysaishi.cn

scp file user@host:/path/
来源：http://fhr.bjfxy.top

[R57] 远程执行命令
来源：http://bwy.fengsongda.top

ssh user@host 'uptime'
来源：http://ejd.zycfv.cn

[R58] 下载文件
来源：http://qnp.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nuv.hysaishi.cn

[R59] 发 POST JSON
来源：http://cxe.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dmh.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://arp.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bqb.redwolf501.top

[R61] 磁盘占用
来源：http://mau.hesvh.cn

df -h;  du -sh *
来源：http://gcs.sysykeji.top

[R62] 找最占空间的文件
来源：http://vqm.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://ukt.daxiang520.top

[R63] 内存与进程
来源：http://xnw.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://jri.nanxinkj.top

[R64] 结束进程
来源：http://suv.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://kez.chenlongwang.top

[R65] 查看端口占用
来源：http://yso.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bzu.yuanzhike.top

[R66] 定时任务
来源：http://gpq.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://bnw.cucudq.cn

[R67] 生成随机十六进制串
来源：http://nzu.sysykeji.top

openssl rand -hex 16
来源：http://bbn.birdmap.top

[R68] 计算文件校验值
来源：http://wss.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://yzu.svipenyu.cn

[R69] 生成随机密码
来源：http://kxs.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://ngf.hcnkem.com

[R70] 时间戳与互转
来源：http://kgk.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://hsd.nanxinkj.top

[R71] 日期格式化
来源：http://pws.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pdf.yongpay.top

[R72] 等待端口就绪
来源：http://uix.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://med.mhx1999.top

[R73] 分割大日志
来源：http://zkm.bbcook.cn

split -l 1000 big.log part_
来源：http://uwy.mhx1999.top

[R74] 批量重命名
来源：http://onv.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fth.hfpthk.cn

[R75] 导出环境变量
来源：http://hme.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://ahk.dashuyun.cn

[R76] 使用临时文件
来源：http://vqu.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://djo.gotoacloud.top

[R77] 读取用户输入
来源：http://aua.yj20258.top

read -rp "请输入: " ans
来源：http://uxp.yvedp.cn

[R78] 交互式菜单
来源：http://daj.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dfk.jianghu66.top

[R79] 解析命令行选项
来源：http://giv.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rdk.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://tdk.gzhubu.top

time ./run.sh
来源：http://lrr.daxiang520.top

================================================================================
来源：http://omi.sweek.top

S. C / C++ 专题
来源：http://mll.shangyingyoupin.top

================================================================================
来源：http://hnu.0kj1m.cn

[S01] C：Hello World
来源：http://mbe.yj20258.top

#include <stdio.h>
来源：http://icg.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mzi.nwbrower.top

[S02] C：变量与格式化输出
来源：http://fdu.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://qds.c1oappe.top

[S03] C：读入整数
来源：http://six.pycfn.com

int x; scanf("%d", &x);
来源：http://ean.epnwcf.com

[S04] C：字符串复制
来源：http://trl.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://drb.havefunace.top

[S05] C：字符串长度
来源：http://dvv.yj20258888.top

strlen(s)
来源：http://ibx.hysaishi.cn

[S06] C：字符串比较
来源：http://kag.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://iup.chenlongwang.top

[S07] C：数组遍历求和
来源：http://teh.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://smb.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://efm.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vdj.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://zyy.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lyw.mhx1999.top

[S10] C：指针与解引用
来源：http://cud.316326.xyz

int *p = &a;  *p = 5;
来源：http://cxw.aibaodan.cn

[S11] C：逐行读文件
来源：http://gsv.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://eaz.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nxx.fzhhl.top

fclose(f);
来源：http://uxu.0kj1m.cn

[S12] C：写文件
来源：http://lax.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sjq.guowangkeji.top

[S13] C：宏定义
来源：http://nzo.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kad.gotoacloud.top

[S14] C：枚举
来源：http://wrr.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://rjv.chenzaomai.com

[S15] C：类型转换
来源：http://llr.iojbl.cn

(double) a / b
来源：http://rdv.aizwys.cn

[S16] C：位操作置位
来源：http://ldn.yfazqb.com

x |= (1 << 3);
来源：http://ikh.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://lnq.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qsq.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://qcb.c1oappe.top

int main(int argc, char **argv)
来源：http://wsh.chenlongwang.top

[S19] C：快速排序
来源：http://awg.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://omk.tianlin.xyz

[S20] C：二分查找
来源：http://zmc.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qga.pycfn.com

[S21] C：字符类别判断
来源：http://blh.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nyo.tianlin.xyz

[S22] C：字符串转数字
来源：http://abb.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://hsw.jinqigfzy.top

[S23] C：随机数
来源：http://ecp.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nry.fzhhl.top

[S24] C：获取本地时间
来源：http://hgc.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bko.ehwqpu.com

[S25] C：内存拷贝
来源：http://rrr.yfazqb.com

memcpy(dst, src, n);
来源：http://icr.fzhhl.top

[S26] C：内存清零
来源：http://kjv.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://tzp.sysykeji.top

[S27] C：定义常量
来源：http://qys.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://gxg.fanxiaobao.xyz

[S28] C：静态变量
来源：http://uoc.hnxiangtu.top

static int counter = 0;
来源：http://jcl.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://wah.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xqg.daxiang520.top

[S30] C：头文件保护
来源：http://yed.tarul.cn

#ifndef X_H
来源：http://grc.hongshengwenyu.top

#define X_H
来源：http://fqq.cucudq.cn

#endif
来源：http://qmk.svipenyu.cn

[S31] C++：Hello World
来源：http://xru.yfazqb.com

#include <iostream>
来源：http://lyu.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://kdq.guowangkeji.top

[S32] C++：字符串
来源：http://nvr.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://tfz.sxryk.cn

[S33] C++：vector 增删
来源：http://hnq.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzd.iojbl.cn

[S34] C++：遍历 vector
来源：http://tay.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://mfp.vehdjk.com

[S35] C++：map
来源：http://dwl.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqr.xylfe.cn

[S36] C++：unordered_map
来源：http://uwx.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uif.nanxuanxn.top

[S37] C++：set
来源：http://epg.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kid.hnqzz.top

[S38] C++：排序
来源：http://kuk.tarul.cn

std::sort(v.begin(), v.end());
来源：http://tax.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://for.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ods.hnqzz.top

[S40] C++：查找元素
来源：http://ayc.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rme.ydzc1.top

[S41] C++：类与构造函数
来源：http://och.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vny.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://mad.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://tif.wangshuangyany.cn

[S43] C++：智能指针
来源：http://xxg.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://qcd.316326.xyz

[S44] C++：引用传参
来源：http://rxt.ybcxt.top

void inc(int &x) { ++x; }
来源：http://oyd.zhixingplan.top

[S45] C++：lambda
来源：http://box.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oho.cqqwz.cn

[S46] C++：函数模板
来源：http://ruj.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ljs.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://zwx.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://css.guowangkeji.top

[S48] C++：逐行读文件
来源：http://ehw.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://nio.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://sqc.haohaochexian.top

[S49] C++：写文件
来源：http://dbx.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ppq.pycfn.com

[S50] C++：格式化数字
来源：http://ecr.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gyz.jqgfzy.top

[S51] C++：显式类型转换
来源：http://jzf.ybcxt.top

static_cast<double>(a) / b
来源：http://xlg.yj20258.top

[S52] C++：const 与 noexcept
来源：http://idm.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://nmc.jianghu66.top

[S53] C++：移动语义
来源：http://izv.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://zvx.quarkkingdee.top

[S54] C++：异常处理
来源：http://zdx.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqs.daria6918.cn

[S55] C++：结构化绑定
来源：http://ylx.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://teu.shangyingyoupin.top

[S56] C++：optional
来源：http://ljb.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ajw.52xcode.cn

[S57] C++：编译期常量
来源：http://gcp.bbcook.cn

constexpr int N = 10;
来源：http://ryr.uphjek.com

[S58] C++：命名空间
来源：http://hyu.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://cli.zhoulong.xyz

[S59] C++：静态断言
来源：http://wof.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hfa.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://gdz.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ryz.ivvv.top

================================================================================
来源：http://dua.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rdp.sjlbkw.cn

================================================================================
来源：http://rvd.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://vvl.xziqi.cn

println("Hello")
来源：http://swf.bjfxy.top

[T02] Kotlin：变量
来源：http://jes.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ytp.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://pgl.shanyushiyangtech.top

"值: $b"
来源：http://ppe.yuanzhike.top

[T04] Kotlin：空安全
来源：http://bja.sufxvd.cn

val n: String? = null;  n?.length
来源：http://mzu.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://qze.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uxh.yj20258888.top

[T06] Kotlin：集合映射
来源：http://ftx.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wjx.cashguo.top

[T07] Kotlin：集合过滤
来源：http://pbn.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ogw.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://gor.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://lao.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://dyn.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://hek.yvedp.cn

[T10] Kotlin：默认参数
来源：http://yqh.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://blf.hfpthk.cn

[T11] Kotlin：协程
来源：http://vxd.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tdq.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://zyl.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://jvv.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://zln.zycfv.cn

val m = mapOf("a" to 1)
来源：http://yck.ydjk.org.cn

[T14] Kotlin：循环
来源：http://huq.hammf.cn

for (i in 1..10) println(i)
来源：http://xhv.yangfankeji.com

[T15] Kotlin：接口
来源：http://esn.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://ogu.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://tlw.yanxiufei.cn

print("Hello")
来源：http://sau.zdqjudy.top

[T17] Swift：变量与常量
来源：http://rho.pycfn.com

var a = 1;  let b = 2
来源：http://vzb.cqqwz.cn

[T18] Swift：字符串插值
来源：http://sjd.chenjidiqi.icu

"值: \(b)"
来源：http://qiw.svipenyu.cn

[T19] Swift：可选绑定
来源：http://goc.yfazqb.com

if let n = opt { print(n) }
来源：http://hme.jqgufenzy.top

[T20] Swift：数组操作
来源：http://fzo.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://mup.daria6918.cn

[T21] Swift：遍历
来源：http://psb.tian-w.cn

for x in a { print(x) }
来源：http://ijz.zhiwuduotai.top

[T22] Swift：字典
来源：http://xpb.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://ozi.gotoacloud.top

[T23] Swift：函数
来源：http://mpc.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jar.9152youxi.cn

[T24] Swift：闭包
来源：http://rnp.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kcw.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://vtp.fzhhl.top

struct P { var x: Int }
来源：http://xch.zhiwuduotai.top

[T26] Swift：类与重写
来源：http://wsx.nwbrower.top

class A: Base { override func f() {} }
来源：http://xun.hammf.cn

[T27] Swift：错误处理
来源：http://gfq.hnqzz.top

do { try f() } catch { print(error) }
来源：http://mci.ppjwa.cn

[T28] Swift：枚举
来源：http://cky.daxiang520.top

enum Color { case red, green }
来源：http://yog.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://cde.yuanzhike.top

guard let x = opt else { return }
来源：http://ueq.guannengcc.top

[T30] Swift：协议
来源：http://bdm.ivvv.top

protocol Shape { func area() -> Double }
来源：http://xnj.cqqwz.cn

[T31] Lua：Hello World
来源：http://iox.ybcxt.top

print("Hello")
来源：http://ghp.ivvv.top

[T32] Lua：局部变量
来源：http://zko.jiagoushi.top

local a = 1
来源：http://qwn.snrcjt.cn

[T33] Lua：表（数组）
来源：http://cmc.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vdv.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://jha.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wmw.tianlin.xyz

[T35] Lua：字典表
来源：http://uku.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://hiu.snrcjt.cn

[T36] Lua：函数
来源：http://stp.chenlongwang.top

function add(a, b) return a + b end
来源：http://nmf.cheryme.top

[T37] Lua：字符串拼接
来源：http://zxu.yuxming.cn

"a" .. "b"
来源：http://kfu.jqgfzy.top

[T38] Lua：条件
来源：http://ntk.pycfn.com

if x > 0 then print("正") end
来源：http://vbt.wangdashe.top

[T39] Lua：模式匹配
来源：http://xjm.xinyue.icu

string.find(s, "%d+")
来源：http://apt.gogol.net.cn

[T40] Lua：元表
来源：http://ryf.fehbvm.com

setmetatable({}, { __index = base })
来源：http://bom.gzhubu.top

[T41] Perl：Hello World
来源：http://xfa.zdbjq.cn

print "Hello\n";
来源：http://wqx.chenlongwang.top

[T42] Perl：变量类型
来源：http://zut.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qah.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://brq.sxryk.cn

"值: $a"
来源：http://pho.feifeiyinyue.top

[T44] Perl：条件
来源：http://faa.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://was.hfpthk.cn

[T45] Perl：数组遍历
来源：http://rbv.tanke756.top

for my $x (@arr) { print $x; }
来源：http://dwh.cashguo.top

[T46] Perl：哈希操作
来源：http://vuq.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://itu.hywenlv.cn

[T47] Perl：正则捕获
来源：http://dpo.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eiq.cucudq.cn

[T48] Perl：正则替换
来源：http://bbl.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://ylt.ydzc1.top

[T49] Perl：函数
来源：http://omo.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rjo.52xcode.cn

[T50] Perl：逐行读文件
来源：http://cwv.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pug.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://uqk.yuxming.cn

[T51] Scala：Hello World
来源：http://cev.smart0.xyz

println("Hello")
来源：http://iuq.ydjk.org.cn

[T52] Scala：变量
来源：http://gbo.hesvh.cn

val a = 1;  var b = 2
来源：http://oyi.cheryme.top

[T53] Scala：字符串插值
来源：http://omq.birdmap.top

s"值: $b"
来源：http://ubk.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://jik.52xcode.cn


<!-- 参考信息 -->