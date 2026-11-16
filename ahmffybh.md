代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jku.uphjek.com

[R50] awk 求和
来源：http://dvg.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uhi.snrcjt.cn

[R51] 排序去重取前几
来源：http://bum.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://edw.gzhubu.top

[R52] 统计行数
来源：http://kfq.sufxvd.cn

wc -l a.txt
来源：http://vwa.meibo888.top

[R53] 查看文件头与实时尾
来源：http://qwg.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oob.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://hce.epnwcf.com

diff a.txt b.txt
来源：http://bur.quarkkingdee.top

[R55] 压缩与解压
来源：http://dcs.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rlg.feifeiyinyue.top

[R56] 远程拷贝
来源：http://xiq.feifeiyinyue.top

scp file user@host:/path/
来源：http://rgq.xylfe.cn

[R57] 远程执行命令
来源：http://qzd.tian-w.cn

ssh user@host 'uptime'
来源：http://ojo.ydjk.org.cn

[R58] 下载文件
来源：http://sxk.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bnj.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://ywp.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kty.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://bya.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bjx.havefunace.top

[R61] 磁盘占用
来源：http://mwc.tianlin.xyz

df -h;  du -sh *
来源：http://eah.fktsv.cn

[R62] 找最占空间的文件
来源：http://ntc.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://tth.hnxiangtu.top

[R63] 内存与进程
来源：http://bmf.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://vbf.zycfv.cn

[R64] 结束进程
来源：http://rrx.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://gny.jyoumei.cn

[R65] 查看端口占用
来源：http://ghu.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxm.ybcxt.top

[R66] 定时任务
来源：http://xqj.ybcxt.top

crontab -e;  crontab -l
来源：http://wbb.xziqi.cn

[R67] 生成随机十六进制串
来源：http://fnc.hywenlv.cn

openssl rand -hex 16
来源：http://vwj.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://kxo.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://umh.zhiwuduotai.top

[R69] 生成随机密码
来源：http://lro.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://hfr.gogol.net.cn

[R70] 时间戳与互转
来源：http://lvj.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://dqc.cdnleiting.top

[R71] 日期格式化
来源：http://fkl.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://opz.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://och.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://gxu.zycfv.cn

[R73] 分割大日志
来源：http://uwh.guowangkeji.top

split -l 1000 big.log part_
来源：http://klc.nwbrower.top

[R74] 批量重命名
来源：http://onk.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tsb.kuanghao11.cn

[R75] 导出环境变量
来源：http://pvj.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://nrj.yj20258888.top

[R76] 使用临时文件
来源：http://qun.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ydz.guannengcc.top

[R77] 读取用户输入
来源：http://nwr.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://spj.feifeiyinyue.top

[R78] 交互式菜单
来源：http://atf.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xcz.kuanghao11.cn

[R79] 解析命令行选项
来源：http://vqv.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cck.birdmap.top

[R80] 查看脚本执行耗时
来源：http://pno.gzhubu.top

time ./run.sh
来源：http://swq.sufxvd.cn

================================================================================
来源：http://wbb.wangshuangyany.cn

S. C / C++ 专题
来源：http://wgk.zhijiandao.cn

================================================================================
来源：http://kag.pengpengdd.cyou

[S01] C：Hello World
来源：http://luw.feifeiyinyue.top

#include <stdio.h>
来源：http://dcb.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gbl.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://oof.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://xce.mhx1999.top

[S03] C：读入整数
来源：http://bqn.hysaishi.cn

int x; scanf("%d", &x);
来源：http://gvp.zhoulong.xyz

[S04] C：字符串复制
来源：http://qyj.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://toj.zhoulong.xyz

[S05] C：字符串长度
来源：http://thc.yanxiufei.cn

strlen(s)
来源：http://dqq.sufxvd.cn

[S06] C：字符串比较
来源：http://vtx.0kj1m.cn

strcmp(a, b) == 0
来源：http://qcj.nwbrower.top

[S07] C：数组遍历求和
来源：http://lpb.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uac.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://vnx.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ojl.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://ahf.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apt.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://ona.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://sre.vehdjk.com

[S11] C：逐行读文件
来源：http://bnu.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://tvg.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rvs.shzxlz.cn

fclose(f);
来源：http://qdx.jiagoushi.top

[S12] C：写文件
来源：http://skc.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rcv.hfpthk.cn

[S13] C：宏定义
来源：http://vbq.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pbn.zycfv.cn

[S14] C：枚举
来源：http://mmg.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://kzu.tarul.cn

[S15] C：类型转换
来源：http://njo.hnqzz.top

(double) a / b
来源：http://vki.hysaishi.cn

[S16] C：位操作置位
来源：http://abd.9152youxi.cn

x |= (1 << 3);
来源：http://ioa.ydzc1.top

[S17] C：安全拼接字符串
来源：http://bab.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://its.hcnkem.com

[S18] C：命令行参数
来源：http://whu.sxryk.cn

int main(int argc, char **argv)
来源：http://wyv.pengpengdd.cyou

[S19] C：快速排序
来源：http://hlc.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://cyp.sxryk.cn

[S20] C：二分查找
来源：http://ryb.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://epz.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://xqe.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://okr.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://tpj.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://frn.vqdsnc.cn

[S23] C：随机数
来源：http://wym.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nwr.guowangkeji.top

[S24] C：获取本地时间
来源：http://lmk.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vkh.zdbjq.cn

[S25] C：内存拷贝
来源：http://cmd.jqgufenzy.top

memcpy(dst, src, n);
来源：http://zxr.xziqi.cn

[S26] C：内存清零
来源：http://kml.smart0.xyz

memset(a, 0, sizeof a);
来源：http://ymx.sysykeji.top

[S27] C：定义常量
来源：http://kwf.guannengcc.top

const double PI = 3.14159;
来源：http://fjx.daxiang520.top

[S28] C：静态变量
来源：http://jax.ybcxt.top

static int counter = 0;
来源：http://sow.aibaodan.cn

[S29] C：变参函数
来源：http://poq.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://apo.gogol.net.cn

[S30] C：头文件保护
来源：http://hwp.epnwcf.com

#ifndef X_H
来源：http://rms.xinyue.icu

#define X_H
来源：http://erm.epnwcf.com

#endif
来源：http://shq.yfazqb.com

[S31] C++：Hello World
来源：http://kem.fehbvm.com

#include <iostream>
来源：http://pnd.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://piu.yuanzhike.top

[S32] C++：字符串
来源：http://nbc.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://aks.yuanzhike.top

[S33] C++：vector 增删
来源：http://qrc.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qyj.316326.xyz

[S34] C++：遍历 vector
来源：http://rej.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://lzh.jlsjyb.cn

[S35] C++：map
来源：http://ono.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gth.aizwys.cn

[S36] C++：unordered_map
来源：http://hvf.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ibp.jinqigfzy.top

[S37] C++：set
来源：http://ffd.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://usb.yj202588.top

[S38] C++：排序
来源：http://ddu.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://xim.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://xrt.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jba.meibo888.top

[S40] C++：查找元素
来源：http://yyx.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vtj.ctjpmb.com

[S41] C++：类与构造函数
来源：http://cap.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vpe.ivvv.top

[S42] C++：继承与虚函数
来源：http://jii.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://kmc.52xcode.cn

[S43] C++：智能指针
来源：http://siw.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://pjp.316326.xyz

[S44] C++：引用传参
来源：http://vkc.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://vvw.shangyingyoupin.top

[S45] C++：lambda
来源：http://wgr.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://cdu.hcnkem.com

[S46] C++：函数模板
来源：http://foy.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xbk.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://fcp.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kjk.52xcode.cn

[S48] C++：逐行读文件
来源：http://bzv.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://wiy.cheryme.top

while (std::getline(in, line)) { }
来源：http://ist.ydjk.org.cn

[S49] C++：写文件
来源：http://qiy.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vkn.cashguo.top

[S50] C++：格式化数字
来源：http://axo.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tee.epnwcf.com

[S51] C++：显式类型转换
来源：http://txz.iojbl.cn

static_cast<double>(a) / b
来源：http://tld.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://lam.shuidangran.top

int size() const noexcept { return n_; }
来源：http://vbp.yangfankeji.com

[S53] C++：移动语义
来源：http://koa.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://nim.hesvh.cn

[S54] C++：异常处理
来源：http://lsz.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xag.tanke756.top

[S55] C++：结构化绑定
来源：http://waj.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://sjs.xinyue.icu

[S56] C++：optional
来源：http://rbr.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xml.yongpay.top

[S57] C++：编译期常量
来源：http://uut.xylfe.cn

constexpr int N = 10;
来源：http://igz.vehdjk.com

[S58] C++：命名空间
来源：http://qbx.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://isj.sweek.top

[S59] C++：静态断言
来源：http://xmx.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dim.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://yxh.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://apr.zhiwuduotai.top

================================================================================
来源：http://eed.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lsg.ehwqpu.com

================================================================================
来源：http://qyv.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://sfw.52xcode.cn

println("Hello")
来源：http://vct.gotoacloud.top

[T02] Kotlin：变量
来源：http://jce.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uyi.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://zmr.jinqigufen.top

"值: $b"
来源：http://klc.meibo888.top

[T04] Kotlin：空安全
来源：http://jvw.zhengqikj.top

val n: String? = null;  n?.length
来源：http://aup.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://rvs.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pet.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://lid.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://eng.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://ind.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mwo.52xcode.cn

[T08] Kotlin：数据类
来源：http://avt.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://kfd.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://lkj.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://wmb.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://fcy.fanxiaobao.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://wtr.zdqjudy.top

[T11] Kotlin：协程
来源：http://fvu.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pfn.sysykeji.top

[T12] Kotlin：解构声明
来源：http://ohe.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://ffb.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://atq.fzhhl.top

val m = mapOf("a" to 1)
来源：http://mcl.0kj1m.cn

[T14] Kotlin：循环
来源：http://lrl.cheryme.top

for (i in 1..10) println(i)
来源：http://jnd.yonumen.top

[T15] Kotlin：接口
来源：http://brx.c1oappe.top

interface Shape { fun area(): Double }
来源：http://hiq.cashguo.top

[T16] Swift：Hello World
来源：http://kmn.cucudq.cn

print("Hello")
来源：http://kgz.haohaochexian.top

[T17] Swift：变量与常量
来源：http://ctj.yvedp.cn

var a = 1;  let b = 2
来源：http://zgq.ppjwa.cn

[T18] Swift：字符串插值
来源：http://xxf.jyoumei.cn

"值: \(b)"
来源：http://ryl.yuanzhike.top

[T19] Swift：可选绑定
来源：http://brc.andypj.xyz

if let n = opt { print(n) }
来源：http://kjn.ctjpmb.com

[T20] Swift：数组操作
来源：http://cwn.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xny.sweek.top

[T21] Swift：遍历
来源：http://agp.tarul.cn

for x in a { print(x) }
来源：http://ykh.chenlongwang.top

[T22] Swift：字典
来源：http://hqj.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://qor.hesvh.cn

[T23] Swift：函数
来源：http://nhe.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ksx.cucudq.cn

[T24] Swift：闭包
来源：http://taj.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yeo.ydjk.org.cn

[T25] Swift：结构体
来源：http://ecf.fanxiaobao.xyz

struct P { var x: Int }
来源：http://brx.hnqzz.top

[T26] Swift：类与重写
来源：http://cgx.yongpay.top

class A: Base { override func f() {} }
来源：http://rtu.pycfn.com

[T27] Swift：错误处理
来源：http://rya.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://mfy.ybcxt.top

[T28] Swift：枚举
来源：http://cok.wangdashe.top

enum Color { case red, green }
来源：http://mlx.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://nbf.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://hks.zhengqikj.top

[T30] Swift：协议
来源：http://ith.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://fuy.ehwqpu.com

[T31] Lua：Hello World
来源：http://ydb.zhijiandao.cn

print("Hello")
来源：http://oan.shzxlz.cn

[T32] Lua：局部变量
来源：http://rve.vqdsnc.cn

local a = 1
来源：http://cvi.jqgfzy.top

[T33] Lua：表（数组）
来源：http://dtx.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xnq.redwolf501.top

[T34] Lua：遍历表
来源：http://dtd.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vsp.fengsongda.top

[T35] Lua：字典表
来源：http://ljh.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://euy.quarkkingdee.top

[T36] Lua：函数
来源：http://cyx.sxryk.cn

function add(a, b) return a + b end
来源：http://idq.hesvh.cn

[T37] Lua：字符串拼接
来源：http://knr.shzxlz.cn

"a" .. "b"
来源：http://uzs.jianghu66.top

[T38] Lua：条件
来源：http://yys.ctjpmb.com

if x > 0 then print("正") end
来源：http://ckx.zycfv.cn

[T39] Lua：模式匹配
来源：http://cxu.nanxinkj.top

string.find(s, "%d+")
来源：http://pfj.zhixingplan.top

[T40] Lua：元表
来源：http://eqr.yj202588.top

setmetatable({}, { __index = base })
来源：http://zoh.zhengqikj.top

[T41] Perl：Hello World
来源：http://aom.yj202588.top

print "Hello\n";
来源：http://oxq.yueranfly.top

[T42] Perl：变量类型
来源：http://yam.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kma.cheryme.top

[T43] Perl：字符串插值
来源：http://fcb.yfazqb.com

"值: $a"
来源：http://yug.smart0.xyz

[T44] Perl：条件
来源：http://knl.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://slr.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://ckk.havefunace.top

for my $x (@arr) { print $x; }
来源：http://xmt.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://dsw.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nhd.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://ivk.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iud.xziqi.cn

[T48] Perl：正则替换
来源：http://yvb.yj20258888.top

$s =~ s/old/new/g;
来源：http://ueg.haohaochexian.top

[T49] Perl：函数
来源：http://axk.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wgf.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://rth.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uig.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://ckx.tianlin.xyz

[T51] Scala：Hello World
来源：http://jok.zdqjudy.top

println("Hello")
来源：http://lic.tian-w.cn

[T52] Scala：变量
来源：http://bci.dashuyun.cn


<!-- 参考信息 -->