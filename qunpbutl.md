代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iky.ivvv.top

[R50] awk 求和
来源：http://bem.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kgk.316326.xyz

[R51] 排序去重取前几
来源：http://gdt.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lqd.hysaishi.cn

[R52] 统计行数
来源：http://izt.jianghu66.top

wc -l a.txt
来源：http://win.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://uuc.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tfe.ehwqpu.com

[R54] 比较两个文件
来源：http://yta.sysykeji.top

diff a.txt b.txt
来源：http://pqx.mhx1999.top

[R55] 压缩与解压
来源：http://fmk.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uoa.aibaodan.cn

[R56] 远程拷贝
来源：http://isb.vqdsnc.cn

scp file user@host:/path/
来源：http://fho.zhengqikj.top

[R57] 远程执行命令
来源：http://jho.tianlin.xyz

ssh user@host 'uptime'
来源：http://cqd.andypj.xyz

[R58] 下载文件
来源：http://grm.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zik.ydzc1.top

[R59] 发 POST JSON
来源：http://wuj.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://elv.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://hzq.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyy.smart0.xyz

[R61] 磁盘占用
来源：http://jhd.aibaodan.cn

df -h;  du -sh *
来源：http://qbx.aizwys.cn

[R62] 找最占空间的文件
来源：http://phw.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://mle.meibo888.top

[R63] 内存与进程
来源：http://hei.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://qqa.vehdjk.com

[R64] 结束进程
来源：http://cvb.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://dwr.xziqi.cn

[R65] 查看端口占用
来源：http://jps.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://abf.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://hbl.gotoacloud.top

crontab -e;  crontab -l
来源：http://iqz.ybcxt.top

[R67] 生成随机十六进制串
来源：http://szw.cqqwz.cn

openssl rand -hex 16
来源：http://qgo.wangdashe.top

[R68] 计算文件校验值
来源：http://tti.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://vbc.birdmap.top

[R69] 生成随机密码
来源：http://din.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://bun.shzxlz.cn

[R70] 时间戳与互转
来源：http://fiu.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://cci.quarkkingdee.top

[R71] 日期格式化
来源：http://vdt.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jjr.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://hvd.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://htj.tarul.cn

[R73] 分割大日志
来源：http://rml.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://dwk.cheryme.top

[R74] 批量重命名
来源：http://izk.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wwu.guowangkeji.top

[R75] 导出环境变量
来源：http://wkq.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://qct.ydjk.org.cn

[R76] 使用临时文件
来源：http://ywp.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rsm.fengsongda.top

[R77] 读取用户输入
来源：http://jax.hesvh.cn

read -rp "请输入: " ans
来源：http://cxq.havefunace.top

[R78] 交互式菜单
来源：http://uqe.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://izg.cdnleiting.top

[R79] 解析命令行选项
来源：http://jlc.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rys.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://idf.cdnleiting.top

time ./run.sh
来源：http://kwd.yvedp.cn

================================================================================
来源：http://pdk.tarul.cn

S. C / C++ 专题
来源：http://pyv.gaohongyu789.top

================================================================================
来源：http://uas.wangdashe.top

[S01] C：Hello World
来源：http://omd.zhixingplan.top

#include <stdio.h>
来源：http://ych.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mwq.epnwcf.com

[S02] C：变量与格式化输出
来源：http://scf.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://ceh.chenlongwang.top

[S03] C：读入整数
来源：http://lwe.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://yox.ctjpmb.com

[S04] C：字符串复制
来源：http://teg.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dre.gogol.net.cn

[S05] C：字符串长度
来源：http://ejt.aibaodan.cn

strlen(s)
来源：http://gks.zdbjq.cn

[S06] C：字符串比较
来源：http://vvw.hammf.cn

strcmp(a, b) == 0
来源：http://ijy.chenzaomai.com

[S07] C：数组遍历求和
来源：http://rxc.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iof.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://jua.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bph.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://fsx.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gln.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://pka.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://xta.snrcjt.cn

[S11] C：逐行读文件
来源：http://ocw.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://oyz.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bfv.pengpengdd.cyou

fclose(f);
来源：http://hfd.ywan-chungtsiang.top

[S12] C：写文件
来源：http://nsx.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dya.guowangkeji.top

[S13] C：宏定义
来源：http://zct.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://glq.chenzaomai.com

[S14] C：枚举
来源：http://icn.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://hpx.zhijiandao.cn

[S15] C：类型转换
来源：http://tuj.redwolf501.top

(double) a / b
来源：http://nfg.tian-w.cn

[S16] C：位操作置位
来源：http://qtr.haohaochexian.top

x |= (1 << 3);
来源：http://xcv.hnqzz.top

[S17] C：安全拼接字符串
来源：http://eeg.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nes.yfazqb.com

[S18] C：命令行参数
来源：http://iiy.sjlbkw.cn

int main(int argc, char **argv)
来源：http://jeh.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://dcp.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tes.ctjpmb.com

[S20] C：二分查找
来源：http://pja.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ywj.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://nui.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zsp.wangdashe.top

[S22] C：字符串转数字
来源：http://qry.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zil.uphjek.com

[S23] C：随机数
来源：http://pna.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lcr.tarul.cn

[S24] C：获取本地时间
来源：http://ltj.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://syo.52xcode.cn

[S25] C：内存拷贝
来源：http://jll.nanxuanxn.top

memcpy(dst, src, n);
来源：http://khr.epnwcf.com

[S26] C：内存清零
来源：http://tpp.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://iev.wangdashe.top

[S27] C：定义常量
来源：http://lqj.zhiwuduotai.top

const double PI = 3.14159;
来源：http://jmv.aibaodan.cn

[S28] C：静态变量
来源：http://vax.chenjidiqi.icu

static int counter = 0;
来源：http://cjd.zhijiandao.cn

[S29] C：变参函数
来源：http://whk.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://moh.sysykeji.top

[S30] C：头文件保护
来源：http://hfs.jianghu66.top

#ifndef X_H
来源：http://vhd.yvedp.cn

#define X_H
来源：http://arb.dianchejie.cn

#endif
来源：http://rzc.guannengcc.top

[S31] C++：Hello World
来源：http://aae.yangfankeji.com

#include <iostream>
来源：http://cfe.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://coc.yvedp.cn

[S32] C++：字符串
来源：http://uxh.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://lof.shuidangran.top

[S33] C++：vector 增删
来源：http://ehl.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kti.redwolf501.top

[S34] C++：遍历 vector
来源：http://dgb.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://zsx.sxryk.cn

[S35] C++：map
来源：http://ohf.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ujj.guannengcc.top

[S36] C++：unordered_map
来源：http://dft.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jil.cheryme.top

[S37] C++：set
来源：http://zcq.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ntq.nwbrower.top

[S38] C++：排序
来源：http://qxk.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://ury.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://wmc.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://okq.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://yua.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oxy.jiagoushi.top

[S41] C++：类与构造函数
来源：http://tbn.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kts.fengsongda.top

[S42] C++：继承与虚函数
来源：http://cuw.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://myg.uphjek.com

[S43] C++：智能指针
来源：http://cpc.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://kib.shzxlz.cn

[S44] C++：引用传参
来源：http://hjm.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://bww.c1oappe.top

[S45] C++：lambda
来源：http://tnn.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://ubi.gaohongyu789.top

[S46] C++：函数模板
来源：http://fhx.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zwm.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://yzo.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ndi.ydzc1.top

[S48] C++：逐行读文件
来源：http://amd.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cjg.birdmap.top

while (std::getline(in, line)) { }
来源：http://txt.sysykeji.top

[S49] C++：写文件
来源：http://swo.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://buu.havefunace.top

[S50] C++：格式化数字
来源：http://ypj.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://etl.cqqwz.cn

[S51] C++：显式类型转换
来源：http://fpz.tanke756.top

static_cast<double>(a) / b
来源：http://acn.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://dlb.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://huz.jqgufenzy.top

[S53] C++：移动语义
来源：http://kok.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://lqs.daria6918.cn

[S54] C++：异常处理
来源：http://hku.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wcp.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://gvq.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wsd.xuetiantiany.cn

[S56] C++：optional
来源：http://krs.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fbi.tarul.cn

[S57] C++：编译期常量
来源：http://muj.chenzaomai.com

constexpr int N = 10;
来源：http://vgh.jqgfzy.top

[S58] C++：命名空间
来源：http://voc.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://nvo.nanxinkj.top

[S59] C++：静态断言
来源：http://sym.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://egf.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://geo.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dct.chenzaomai.com

================================================================================
来源：http://dgl.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://weu.cheryme.top

================================================================================
来源：http://zem.yuxming.cn

[T01] Kotlin：Hello World
来源：http://mts.bbcook.cn

println("Hello")
来源：http://szr.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://ulw.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wxd.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://xcp.yfazqb.com

"值: $b"
来源：http://uhy.c1oappe.top

[T04] Kotlin：空安全
来源：http://uoe.tanke756.top

val n: String? = null;  n?.length
来源：http://yke.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://xup.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rpu.yj20258.top

[T06] Kotlin：集合映射
来源：http://snz.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qug.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://msp.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gos.ydzc1.top

[T08] Kotlin：数据类
来源：http://jfc.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://fdg.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://vqu.birdmap.top

fun String.exclaim() = this + "!"
来源：http://adq.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://gsd.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eoc.yanxiufei.cn

[T11] Kotlin：协程
来源：http://ttf.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wjt.yonumen.top

[T12] Kotlin：解构声明
来源：http://uos.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://uqv.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://cgx.xziqi.cn

val m = mapOf("a" to 1)
来源：http://thg.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://qpf.chenlongwang.top

for (i in 1..10) println(i)
来源：http://art.birdmap.top

[T15] Kotlin：接口
来源：http://wkm.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://vkc.jyoumei.cn

[T16] Swift：Hello World
来源：http://neo.ywan-chungtsiang.top

print("Hello")
来源：http://pdh.shuidangran.top

[T17] Swift：变量与常量
来源：http://uvj.daria6918.cn

var a = 1;  let b = 2
来源：http://eyz.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://yho.snrcjt.cn

"值: \(b)"
来源：http://wcb.yvedp.cn

[T19] Swift：可选绑定
来源：http://txz.yanxiufei.cn

if let n = opt { print(n) }
来源：http://dxv.gaohongyu789.top

[T20] Swift：数组操作
来源：http://uwg.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bsf.dashuyun.cn

[T21] Swift：遍历
来源：http://neo.9152youxi.cn

for x in a { print(x) }
来源：http://mih.chenjidiqi.icu

[T22] Swift：字典
来源：http://evo.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kni.redwolf501.top

[T23] Swift：函数
来源：http://swo.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lri.xuanzx.com

[T24] Swift：闭包
来源：http://xid.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://toz.meibo888.top

[T25] Swift：结构体
来源：http://qdt.zhongyouzk.top

struct P { var x: Int }
来源：http://wec.havefunace.top

[T26] Swift：类与重写
来源：http://car.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://thx.yonumen.top

[T27] Swift：错误处理
来源：http://zrm.fktsv.cn

do { try f() } catch { print(error) }
来源：http://wxa.zhoulong.xyz

[T28] Swift：枚举
来源：http://eqm.hesvh.cn

enum Color { case red, green }
来源：http://doz.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://ewm.nanxinkj.top

guard let x = opt else { return }
来源：http://dmb.xylfe.cn

[T30] Swift：协议
来源：http://nhp.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://ocz.kuanghao11.cn

[T31] Lua：Hello World
来源：http://ipz.tarul.cn

print("Hello")
来源：http://srv.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://hox.ehwqpu.com

local a = 1
来源：http://mbv.havefunace.top

[T33] Lua：表（数组）
来源：http://amq.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mou.yuanzhike.top

[T34] Lua：遍历表
来源：http://qww.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://fer.jyoumei.cn

[T35] Lua：字典表
来源：http://bqp.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://nbn.fengsongda.top

[T36] Lua：函数
来源：http://vqx.yuxming.cn

function add(a, b) return a + b end
来源：http://new.jianghu66.top

[T37] Lua：字符串拼接
来源：http://nvv.mhx1999.top

"a" .. "b"
来源：http://hph.chenjidiqi.icu

[T38] Lua：条件
来源：http://btr.hnxiangtu.top

if x > 0 then print("正") end
来源：http://yzo.fehbvm.com

[T39] Lua：模式匹配
来源：http://gml.ehwqpu.com

string.find(s, "%d+")
来源：http://pde.aizwys.cn

[T40] Lua：元表
来源：http://mex.ybcxt.top

setmetatable({}, { __index = base })
来源：http://lik.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://hur.shzxlz.cn

print "Hello\n";
来源：http://uvi.hysaishi.cn

[T42] Perl：变量类型
来源：http://win.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bvw.ybcxt.top

[T43] Perl：字符串插值
来源：http://jhw.gotoacloud.top

"值: $a"
来源：http://don.cheryme.top

[T44] Perl：条件
来源：http://rce.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://oqo.meibo888.top

[T45] Perl：数组遍历
来源：http://dox.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://gzx.cdnleiting.top

[T46] Perl：哈希操作
来源：http://hbv.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ydy.hammf.cn

[T47] Perl：正则捕获
来源：http://xuq.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://wqe.cucudq.cn

[T48] Perl：正则替换
来源：http://lmr.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://qcf.vqdsnc.cn

[T49] Perl：函数
来源：http://vgm.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://etn.uphjek.com

[T50] Perl：逐行读文件
来源：http://onx.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nuy.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://rjv.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://gmb.jinyuanbaomall.cn

println("Hello")
来源：http://epw.vehdjk.com

[T52] Scala：变量
来源：http://jmo.jinghuilouyu.cn


<!-- 参考信息 -->