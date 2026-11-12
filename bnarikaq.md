代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tfy.feifeiyinyue.top

[R50] awk 求和
来源：http://kah.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nbf.cheryme.top

[R51] 排序去重取前几
来源：http://fxu.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://unt.xinyue.icu

[R52] 统计行数
来源：http://imm.mhx1999.top

wc -l a.txt
来源：http://uos.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://tct.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hvv.yanxiufei.cn

[R54] 比较两个文件
来源：http://tdz.xuetiantiany.cn

diff a.txt b.txt
来源：http://tqu.chenjidiqi.icu

[R55] 压缩与解压
来源：http://utp.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pfg.xinyue.icu

[R56] 远程拷贝
来源：http://lvk.jinqigfzy.top

scp file user@host:/path/
来源：http://ndm.hnqzz.top

[R57] 远程执行命令
来源：http://nci.hnqzz.top

ssh user@host 'uptime'
来源：http://uvs.cheryme.top

[R58] 下载文件
来源：http://bfe.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sgy.zycfv.cn

[R59] 发 POST JSON
来源：http://mtl.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://exe.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://adp.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mwu.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://lqd.ybcxt.top

df -h;  du -sh *
来源：http://kqu.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://aad.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://dgz.tianlin.xyz

[R63] 内存与进程
来源：http://jfr.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://mmv.ydjk.org.cn

[R64] 结束进程
来源：http://hws.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://aty.yangfankeji.com

[R65] 查看端口占用
来源：http://fcz.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zoe.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://bpi.ppjwa.cn

crontab -e;  crontab -l
来源：http://zkp.hesvh.cn

[R67] 生成随机十六进制串
来源：http://fsd.jinqigufen.top

openssl rand -hex 16
来源：http://okd.zhengqikj.top

[R68] 计算文件校验值
来源：http://qgv.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://dpv.zdqjudy.top

[R69] 生成随机密码
来源：http://azt.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://hnq.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://dzv.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://iiz.xziqi.cn

[R71] 日期格式化
来源：http://drb.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uqi.hfpthk.cn

[R72] 等待端口就绪
来源：http://hxs.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ifg.jianghu66.top

[R73] 分割大日志
来源：http://spu.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://rxm.dianchejie.cn

[R74] 批量重命名
来源：http://jjd.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nun.sjlbkw.cn

[R75] 导出环境变量
来源：http://dry.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://oem.xuanzx.com

[R76] 使用临时文件
来源：http://grk.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zbm.zdbjq.cn

[R77] 读取用户输入
来源：http://ewj.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://pbu.pycfn.com

[R78] 交互式菜单
来源：http://vla.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nkn.xinyue.icu

[R79] 解析命令行选项
来源：http://umq.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ulm.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://fii.nanxinkj.top

time ./run.sh
来源：http://fdd.iojbl.cn

================================================================================
来源：http://ghu.vehdjk.com

S. C / C++ 专题
来源：http://ftg.nanxuanxn.top

================================================================================
来源：http://jli.fehbvm.com

[S01] C：Hello World
来源：http://bdb.jyoumei.cn

#include <stdio.h>
来源：http://ifa.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://doe.iojbl.cn

[S02] C：变量与格式化输出
来源：http://qln.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://lfi.shanyushiyangtech.top

[S03] C：读入整数
来源：http://whs.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://dea.jianghu66.top

[S04] C：字符串复制
来源：http://lix.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xde.jqgfzy.top

[S05] C：字符串长度
来源：http://qoa.gaohongyu789.top

strlen(s)
来源：http://okt.havefunace.top

[S06] C：字符串比较
来源：http://uyw.daxiang520.top

strcmp(a, b) == 0
来源：http://fhi.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://zvk.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qns.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://uht.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayv.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://ruo.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://exu.jinqigfzy.top

[S10] C：指针与解引用
来源：http://vgq.xziqi.cn

int *p = &a;  *p = 5;
来源：http://pbn.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://ntr.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://azc.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://svs.bbcook.cn

fclose(f);
来源：http://enq.316326.xyz

[S12] C：写文件
来源：http://pck.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ugx.wangdashe.top

[S13] C：宏定义
来源：http://dnq.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zib.yanxiufei.cn

[S14] C：枚举
来源：http://ctw.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://lex.zhongyouzk.top

[S15] C：类型转换
来源：http://cny.gaohongyu789.top

(double) a / b
来源：http://ivu.9152youxi.cn

[S16] C：位操作置位
来源：http://atz.hysaishi.cn

x |= (1 << 3);
来源：http://vra.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://fio.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpe.jlsjyb.cn

[S18] C：命令行参数
来源：http://zcz.shuidangran.top

int main(int argc, char **argv)
来源：http://glk.bbcook.cn

[S19] C：快速排序
来源：http://tyh.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qmc.hongshengwenyu.top

[S20] C：二分查找
来源：http://wgp.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kqb.jiagoushi.top

[S21] C：字符类别判断
来源：http://xwx.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dgd.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://suf.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://fef.zycfv.cn

[S23] C：随机数
来源：http://egd.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nom.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://eog.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pdm.pycfn.com

[S25] C：内存拷贝
来源：http://wlu.vehdjk.com

memcpy(dst, src, n);
来源：http://nrw.xinyue.icu

[S26] C：内存清零
来源：http://gbe.wangdashe.top

memset(a, 0, sizeof a);
来源：http://zuq.yj202588.top

[S27] C：定义常量
来源：http://dmm.yueranfly.top

const double PI = 3.14159;
来源：http://iks.cucudq.cn

[S28] C：静态变量
来源：http://kkz.wangdashe.top

static int counter = 0;
来源：http://vrl.ctjpmb.com

[S29] C：变参函数
来源：http://joq.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://izm.bbcook.cn

[S30] C：头文件保护
来源：http://kzg.ydjk.org.cn

#ifndef X_H
来源：http://bhx.tianlin.xyz

#define X_H
来源：http://yek.redwolf501.top

#endif
来源：http://tzx.zdbjq.cn

[S31] C++：Hello World
来源：http://usp.yueranfly.top

#include <iostream>
来源：http://bbw.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://cin.zhoulong.xyz

[S32] C++：字符串
来源：http://ecf.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://vvn.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://xxs.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gai.hesvh.cn

[S34] C++：遍历 vector
来源：http://wie.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://qzf.shangyingyoupin.top

[S35] C++：map
来源：http://dnj.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yrh.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://dmn.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eyc.ehwqpu.com

[S37] C++：set
来源：http://kyp.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nzb.nanxuanxn.top

[S38] C++：排序
来源：http://qao.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://vpy.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://uoa.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vij.hysaishi.cn

[S40] C++：查找元素
来源：http://fjx.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sgz.epnwcf.com

[S41] C++：类与构造函数
来源：http://dgo.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvm.uphjek.com

[S42] C++：继承与虚函数
来源：http://eeh.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://qpz.316326.xyz

[S43] C++：智能指针
来源：http://ivb.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://bls.sweek.top

[S44] C++：引用传参
来源：http://oqh.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://kte.haohaochexian.top

[S45] C++：lambda
来源：http://yae.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nft.iojbl.cn

[S46] C++：函数模板
来源：http://vjq.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uyy.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://wkh.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xwg.yj20258.top

[S48] C++：逐行读文件
来源：http://lqm.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://xif.mhx1999.top

while (std::getline(in, line)) { }
来源：http://ptz.hesvh.cn

[S49] C++：写文件
来源：http://wdg.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ihf.quarkkingdee.top

[S50] C++：格式化数字
来源：http://jkq.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ees.epnwcf.com

[S51] C++：显式类型转换
来源：http://smk.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://ebp.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://kzx.shuidangran.top

int size() const noexcept { return n_; }
来源：http://lss.xylfe.cn

[S53] C++：移动语义
来源：http://pew.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://gjs.vqdsnc.cn

[S54] C++：异常处理
来源：http://kkm.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zbb.hammf.cn

[S55] C++：结构化绑定
来源：http://ttn.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dec.nwbrower.top

[S56] C++：optional
来源：http://bcz.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eql.birdmap.top

[S57] C++：编译期常量
来源：http://dnq.chenjidiqi.icu

constexpr int N = 10;
来源：http://sul.aibaodan.cn

[S58] C++：命名空间
来源：http://rho.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://tzk.birdmap.top

[S59] C++：静态断言
来源：http://owd.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zvc.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://bit.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uxc.hfpthk.cn

================================================================================
来源：http://tik.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sie.jinghuilouyu.cn

================================================================================
来源：http://xgu.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://qeg.hnxiangtu.top

println("Hello")
来源：http://qft.meibo888.top

[T02] Kotlin：变量
来源：http://mar.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxv.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://vjx.cashguo.top

"值: $b"
来源：http://qaq.ydzc1.top

[T04] Kotlin：空安全
来源：http://quk.nanxinkj.top

val n: String? = null;  n?.length
来源：http://syg.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://uty.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pdb.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://ftl.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wej.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://vkk.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qok.hywenlv.cn

[T08] Kotlin：数据类
来源：http://sty.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://nqi.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://jvf.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://nji.yueranfly.top

[T10] Kotlin：默认参数
来源：http://lcq.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fud.fzhhl.top

[T11] Kotlin：协程
来源：http://jbf.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lki.yj202588.top

[T12] Kotlin：解构声明
来源：http://hvp.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://qlp.havefunace.top

[T13] Kotlin：只读 Map
来源：http://pdb.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://iwn.jiagoushi.top

[T14] Kotlin：循环
来源：http://pis.andypj.xyz

for (i in 1..10) println(i)
来源：http://wli.cheryme.top

[T15] Kotlin：接口
来源：http://xmf.wangdashe.top

interface Shape { fun area(): Double }
来源：http://mth.haohaochexian.top

[T16] Swift：Hello World
来源：http://hyr.ivvv.top

print("Hello")
来源：http://uuy.daxiang520.top

[T17] Swift：变量与常量
来源：http://nxn.yangfankeji.com

var a = 1;  let b = 2
来源：http://ugk.fktsv.cn

[T18] Swift：字符串插值
来源：http://nrf.xinyue.icu

"值: \(b)"
来源：http://ucf.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://gij.yfazqb.com

if let n = opt { print(n) }
来源：http://mhp.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://zlf.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oev.xylfe.cn

[T21] Swift：遍历
来源：http://kft.chenjidiqi.icu

for x in a { print(x) }
来源：http://xai.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://gss.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rzm.vqdsnc.cn

[T23] Swift：函数
来源：http://nyq.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gqr.hysaishi.cn

[T24] Swift：闭包
来源：http://vwj.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xlr.smart0.xyz

[T25] Swift：结构体
来源：http://uuy.yvedp.cn

struct P { var x: Int }
来源：http://xmm.c1oappe.top

[T26] Swift：类与重写
来源：http://cbj.gotoacloud.top

class A: Base { override func f() {} }
来源：http://bce.birdmap.top

[T27] Swift：错误处理
来源：http://kiy.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://jih.0kj1m.cn

[T28] Swift：枚举
来源：http://glj.xziqi.cn

enum Color { case red, green }
来源：http://vqs.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://zua.daria6918.cn

guard let x = opt else { return }
来源：http://ifr.gogol.net.cn

[T30] Swift：协议
来源：http://xet.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://ooj.pycfn.com

[T31] Lua：Hello World
来源：http://qgf.zhongyouzk.top

print("Hello")
来源：http://rda.bbcook.cn

[T32] Lua：局部变量
来源：http://fhd.xinyue.icu

local a = 1
来源：http://icb.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://tqq.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ogz.zhijiandao.cn

[T34] Lua：遍历表
来源：http://eui.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oob.ivvv.top

[T35] Lua：字典表
来源：http://vgc.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://pyt.iojbl.cn

[T36] Lua：函数
来源：http://ikz.jianghu66.top

function add(a, b) return a + b end
来源：http://uff.shuidangran.top

[T37] Lua：字符串拼接
来源：http://trx.vehdjk.com

"a" .. "b"
来源：http://kmq.jiagoushi.top

[T38] Lua：条件
来源：http://tsu.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://dtp.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://wpv.gaohongyu789.top

string.find(s, "%d+")
来源：http://euw.havefunace.top

[T40] Lua：元表
来源：http://rhv.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://pdx.9152youxi.cn

[T41] Perl：Hello World
来源：http://udr.nanxinkj.top

print "Hello\n";
来源：http://yxs.haohaochexian.top

[T42] Perl：变量类型
来源：http://xyu.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hho.nanxinkj.top

[T43] Perl：字符串插值
来源：http://gqb.fzhhl.top

"值: $a"
来源：http://qcm.zdbjq.cn

[T44] Perl：条件
来源：http://jwy.pycfn.com

if ($a > 0) { print "正"; }
来源：http://gjl.xylfe.cn

[T45] Perl：数组遍历
来源：http://saq.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://pdi.zdqjudy.top

[T46] Perl：哈希操作
来源：http://bos.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://noz.hcnkem.com

[T47] Perl：正则捕获
来源：http://mle.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yex.yuanzhike.top

[T48] Perl：正则替换
来源：http://jpe.yj202588.top

$s =~ s/old/new/g;
来源：http://knj.dianchejie.cn

[T49] Perl：函数
来源：http://iln.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rnw.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://tua.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://knu.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://qfa.zdqjudy.top

[T51] Scala：Hello World
来源：http://wdr.birdmap.top

println("Hello")
来源：http://qwu.redwolf501.top

[T52] Scala：变量
来源：http://ysh.mhx1999.top


<!-- 参考信息 -->