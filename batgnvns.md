代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://suk.hysaishi.cn

[R52] 统计行数
来源：http://wlm.vehdjk.com

wc -l a.txt
来源：http://wuo.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://wew.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zgc.yanxiufei.cn

[R54] 比较两个文件
来源：http://uly.yvedp.cn

diff a.txt b.txt
来源：http://esc.zhiwuduotai.top

[R55] 压缩与解压
来源：http://jpa.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wbm.feifeiyinyue.top

[R56] 远程拷贝
来源：http://pvk.yvedp.cn

scp file user@host:/path/
来源：http://gzi.guowangkeji.top

[R57] 远程执行命令
来源：http://srd.xziqi.cn

ssh user@host 'uptime'
来源：http://aow.yuanzhike.top

[R58] 下载文件
来源：http://ewq.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iap.haohaochexian.top

[R59] 发 POST JSON
来源：http://cwy.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://owb.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://xma.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uju.jqgufenzy.top

[R61] 磁盘占用
来源：http://ivo.haohaochexian.top

df -h;  du -sh *
来源：http://mxn.hesvh.cn

[R62] 找最占空间的文件
来源：http://jdo.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://azu.cucudq.cn

[R63] 内存与进程
来源：http://xwh.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://bwr.jqgufenzy.top

[R64] 结束进程
来源：http://tim.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://tfj.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://pws.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vgo.yanxiufei.cn

[R66] 定时任务
来源：http://ipj.vehdjk.com

crontab -e;  crontab -l
来源：http://fhm.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://fkr.meibo888.top

openssl rand -hex 16
来源：http://azt.gogol.net.cn

[R68] 计算文件校验值
来源：http://end.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nid.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://cim.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://ekf.gogol.net.cn

[R70] 时间戳与互转
来源：http://hlj.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://wla.chenzaomai.com

[R71] 日期格式化
来源：http://nrc.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yix.cqqwz.cn

[R72] 等待端口就绪
来源：http://ggn.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://evy.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://lcu.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://vsg.nanxinkj.top

[R74] 批量重命名
来源：http://psk.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://whp.jqgufenzy.top

[R75] 导出环境变量
来源：http://laf.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://avc.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://fek.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ugj.ehwqpu.com

[R77] 读取用户输入
来源：http://eaw.fehbvm.com

read -rp "请输入: " ans
来源：http://vwl.zhijiandao.cn

[R78] 交互式菜单
来源：http://zwi.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ejg.nanxinkj.top

[R79] 解析命令行选项
来源：http://xhc.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yqi.yj202588.top

[R80] 查看脚本执行耗时
来源：http://nbq.gogol.net.cn

time ./run.sh
来源：http://pva.yanxiufei.cn

================================================================================
来源：http://bbf.jiagoushi.top

S. C / C++ 专题
来源：http://pcv.9152youxi.cn

================================================================================
来源：http://yhj.yanxiufei.cn

[S01] C：Hello World
来源：http://uwl.hcnkem.com

#include <stdio.h>
来源：http://dta.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ndy.iojbl.cn

[S02] C：变量与格式化输出
来源：http://fla.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://cct.yuxming.cn

[S03] C：读入整数
来源：http://tna.gogol.net.cn

int x; scanf("%d", &x);
来源：http://jan.mhx1999.top

[S04] C：字符串复制
来源：http://cge.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://fwc.yvedp.cn

[S05] C：字符串长度
来源：http://wga.dashuyun.cn

strlen(s)
来源：http://llm.guowangkeji.top

[S06] C：字符串比较
来源：http://uaa.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://hez.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://fqb.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mcg.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://pgh.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lxe.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://ewf.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fkw.cucudq.cn

[S10] C：指针与解引用
来源：http://tbh.c1oappe.top

int *p = &a;  *p = 5;
来源：http://tht.fktsv.cn

[S11] C：逐行读文件
来源：http://bwh.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://kgn.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bpp.zycfv.cn

fclose(f);
来源：http://auv.andypj.xyz

[S12] C：写文件
来源：http://nfk.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://brq.dianchejie.cn

[S13] C：宏定义
来源：http://bls.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvi.iojbl.cn

[S14] C：枚举
来源：http://adv.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://rqz.zdqjudy.top

[S15] C：类型转换
来源：http://haf.hesvh.cn

(double) a / b
来源：http://emn.ivvv.top

[S16] C：位操作置位
来源：http://ecg.yuanzhike.top

x |= (1 << 3);
来源：http://bkz.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://hei.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eao.wangdashe.top

[S18] C：命令行参数
来源：http://apl.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://dsg.daxiang520.top

[S19] C：快速排序
来源：http://rje.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ltw.zhixingplan.top

[S20] C：二分查找
来源：http://afe.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bky.jyoumei.cn

[S21] C：字符类别判断
来源：http://ugd.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fdr.bjfxy.top

[S22] C：字符串转数字
来源：http://ues.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://pcg.sweek.top

[S23] C：随机数
来源：http://zkw.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dlo.pycfn.com

[S24] C：获取本地时间
来源：http://ldf.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fbl.zhijiandao.cn

[S25] C：内存拷贝
来源：http://fni.yueranfly.top

memcpy(dst, src, n);
来源：http://iyw.xuanzx.com

[S26] C：内存清零
来源：http://omw.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://bxi.tanke756.top

[S27] C：定义常量
来源：http://nqs.hnxiangtu.top

const double PI = 3.14159;
来源：http://olh.sufxvd.cn

[S28] C：静态变量
来源：http://ixe.yuanzhike.top

static int counter = 0;
来源：http://ril.cashguo.top

[S29] C：变参函数
来源：http://iip.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bpk.quarkkingdee.top

[S30] C：头文件保护
来源：http://zma.zhaomingkeji.xyz

#ifndef X_H
来源：http://uwp.yongpay.top

#define X_H
来源：http://aoy.jlsjyb.cn

#endif
来源：http://fbm.vehdjk.com

[S31] C++：Hello World
来源：http://wtk.bbcook.cn

#include <iostream>
来源：http://rqz.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://neu.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://gzi.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://yvj.shzxlz.cn

[S33] C++：vector 增删
来源：http://eyc.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qhi.pycfn.com

[S34] C++：遍历 vector
来源：http://vqf.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://ktt.wangshuangyany.cn

[S35] C++：map
来源：http://ikw.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nzm.0kj1m.cn

[S36] C++：unordered_map
来源：http://uvj.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kpf.havefunace.top

[S37] C++：set
来源：http://jhp.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sns.hnqzz.top

[S38] C++：排序
来源：http://tzz.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://kuk.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ixr.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ksz.yanxiufei.cn

[S40] C++：查找元素
来源：http://zei.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jsh.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://tgy.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dzg.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://skc.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://bkj.shzxlz.cn

[S43] C++：智能指针
来源：http://hsr.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://icj.chenlongwang.top

[S44] C++：引用传参
来源：http://rho.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://xko.dianchejie.cn

[S45] C++：lambda
来源：http://cbk.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://klm.jqgufenzy.top

[S46] C++：函数模板
来源：http://dai.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dzw.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://yso.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://phd.jinqigufen.top

[S48] C++：逐行读文件
来源：http://lwv.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://tau.birdmap.top

while (std::getline(in, line)) { }
来源：http://hqt.yonumen.top

[S49] C++：写文件
来源：http://kft.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ufo.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://hdd.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://coo.haohaochexian.top

[S51] C++：显式类型转换
来源：http://azz.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://enm.havefunace.top

[S52] C++：const 与 noexcept
来源：http://yxp.daxiang520.top

int size() const noexcept { return n_; }
来源：http://yeo.hfpthk.cn

[S53] C++：移动语义
来源：http://pzl.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://uza.jyoumei.cn

[S54] C++：异常处理
来源：http://aim.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ssw.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://mhf.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hvm.cashguo.top

[S56] C++：optional
来源：http://rvp.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jci.tanke756.top

[S57] C++：编译期常量
来源：http://rjp.nwbrower.top

constexpr int N = 10;
来源：http://zab.guannengcc.top

[S58] C++：命名空间
来源：http://eev.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://wll.ppjwa.cn

[S59] C++：静态断言
来源：http://zcz.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dbk.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://lei.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iuh.chenjidiqi.icu

================================================================================
来源：http://kwk.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bwc.shzxlz.cn

================================================================================
来源：http://srs.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://pwt.yanxiufei.cn

println("Hello")
来源：http://puc.hammf.cn

[T02] Kotlin：变量
来源：http://jce.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zux.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://quf.nanxinkj.top

"值: $b"
来源：http://aoo.fktsv.cn

[T04] Kotlin：空安全
来源：http://egz.hnqzz.top

val n: String? = null;  n?.length
来源：http://edp.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://mco.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vpc.cheryme.top

[T06] Kotlin：集合映射
来源：http://lnw.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yxs.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://iev.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfa.yuanzhike.top

[T08] Kotlin：数据类
来源：http://bdp.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://val.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://sfh.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://cgh.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://dpx.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xks.fengsongda.top

[T11] Kotlin：协程
来源：http://dfv.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvd.yueranfly.top

[T12] Kotlin：解构声明
来源：http://eky.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://roj.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://qwv.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://yov.sufxvd.cn

[T14] Kotlin：循环
来源：http://mnd.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://egg.zhixingplan.top

[T15] Kotlin：接口
来源：http://pdv.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://ntb.zhoulong.xyz

[T16] Swift：Hello World
来源：http://bsd.haohaochexian.top

print("Hello")
来源：http://jfl.jqgfzy.top

[T17] Swift：变量与常量
来源：http://wwp.zhongyouzk.top

var a = 1;  let b = 2
来源：http://wuo.snrcjt.cn

[T18] Swift：字符串插值
来源：http://jyg.cheryme.top

"值: \(b)"
来源：http://sol.pycfn.com

[T19] Swift：可选绑定
来源：http://qki.zhengqikj.top

if let n = opt { print(n) }
来源：http://hbg.snrcjt.cn

[T20] Swift：数组操作
来源：http://zmh.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pit.9152youxi.cn

[T21] Swift：遍历
来源：http://jtp.yongpay.top

for x in a { print(x) }
来源：http://ppg.cashguo.top

[T22] Swift：字典
来源：http://qup.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://tyc.vqdsnc.cn

[T23] Swift：函数
来源：http://qer.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rgt.zhongyouzk.top

[T24] Swift：闭包
来源：http://lne.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://jod.dashuyun.cn

[T25] Swift：结构体
来源：http://waa.zdbjq.cn

struct P { var x: Int }
来源：http://put.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://mky.jiagoushi.top

class A: Base { override func f() {} }
来源：http://hxc.sweek.top

[T27] Swift：错误处理
来源：http://xvo.meibo888.top

do { try f() } catch { print(error) }
来源：http://plx.sufxvd.cn

[T28] Swift：枚举
来源：http://qio.sufxvd.cn

enum Color { case red, green }
来源：http://rod.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://nzb.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://zvw.jinqigfzy.top

[T30] Swift：协议
来源：http://zaz.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://skc.sysykeji.top

[T31] Lua：Hello World
来源：http://sgv.yueranfly.top

print("Hello")
来源：http://xlh.fehbvm.com

[T32] Lua：局部变量
来源：http://faj.jinyuanbaomall.cn

local a = 1
来源：http://qho.yj202588.top

[T33] Lua：表（数组）
来源：http://cke.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://aai.jlsjyb.cn

[T34] Lua：遍历表
来源：http://xzw.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://icr.chenlongwang.top

[T35] Lua：字典表
来源：http://cgw.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://oer.sjlbkw.cn

[T36] Lua：函数
来源：http://iuj.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://pos.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://hyf.yj20258.top

"a" .. "b"
来源：http://jaa.xinyue.icu

[T38] Lua：条件
来源：http://kso.yj20258888.top

if x > 0 then print("正") end
来源：http://tam.epnwcf.com

[T39] Lua：模式匹配
来源：http://bad.pycfn.com

string.find(s, "%d+")
来源：http://csl.52xcode.cn

[T40] Lua：元表
来源：http://ybt.epnwcf.com

setmetatable({}, { __index = base })
来源：http://qxw.xinyue.icu

[T41] Perl：Hello World
来源：http://plp.sweek.top

print "Hello\n";
来源：http://cej.chenlongwang.top

[T42] Perl：变量类型
来源：http://jkg.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qiz.zdqjudy.top

[T43] Perl：字符串插值
来源：http://eam.daxiang520.top

"值: $a"
来源：http://aie.cqqwz.cn

[T44] Perl：条件
来源：http://hpj.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://ydt.ivvv.top

[T45] Perl：数组遍历
来源：http://xdw.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://sof.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://gpz.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jlp.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://rhe.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://atb.shuidangran.top

[T48] Perl：正则替换
来源：http://ztd.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://emu.yongpay.top

[T49] Perl：函数
来源：http://xkc.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mpo.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://yhs.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bid.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://yrs.hnxiangtu.top

[T51] Scala：Hello World
来源：http://peq.haohaochexian.top

println("Hello")
来源：http://euv.havefunace.top

[T52] Scala：变量
来源：http://vhh.9152youxi.cn

val a = 1;  var b = 2
来源：http://okl.yongpay.top

[T53] Scala：字符串插值
来源：http://uck.yangfankeji.com

s"值: $b"
来源：http://cjp.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://luj.birdmap.top


<!-- 参考信息 -->