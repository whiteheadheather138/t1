代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://aji.hfpthk.cn

[R52] 统计行数
来源：http://uci.zhongyouzk.top

wc -l a.txt
来源：http://jwu.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://zmp.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://glp.ivvv.top

[R54] 比较两个文件
来源：http://pgg.chenzaomai.com

diff a.txt b.txt
来源：http://vnx.andypj.xyz

[R55] 压缩与解压
来源：http://oku.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aqb.cdnleiting.top

[R56] 远程拷贝
来源：http://nvz.bbcook.cn

scp file user@host:/path/
来源：http://mtr.guowangkeji.top

[R57] 远程执行命令
来源：http://fue.cucudq.cn

ssh user@host 'uptime'
来源：http://nui.aibaodan.cn

[R58] 下载文件
来源：http://vop.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpl.zhijiandao.cn

[R59] 发 POST JSON
来源：http://thx.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fnt.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://jtf.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xkj.wangshuangyany.cn

[R61] 磁盘占用
来源：http://nqy.bjfxy.top

df -h;  du -sh *
来源：http://jpe.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://uyu.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://poy.gzhubu.top

[R63] 内存与进程
来源：http://eom.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://nly.fehbvm.com

[R64] 结束进程
来源：http://dut.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://qcx.yfazqb.com

[R65] 查看端口占用
来源：http://mss.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wmy.kuanghao11.cn

[R66] 定时任务
来源：http://pml.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://xdh.cheryme.top

[R67] 生成随机十六进制串
来源：http://xyo.zhijiandao.cn

openssl rand -hex 16
来源：http://rkf.sxryk.cn

[R68] 计算文件校验值
来源：http://uhs.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://vtl.tian-w.cn

[R69] 生成随机密码
来源：http://thn.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://pjj.sweek.top

[R70] 时间戳与互转
来源：http://vjo.xinyue.icu

date +%s;  date -d @1700000000
来源：http://dwb.vqdsnc.cn

[R71] 日期格式化
来源：http://aau.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://rsw.wangdashe.top

[R72] 等待端口就绪
来源：http://wce.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://zda.dianchejie.cn

[R73] 分割大日志
来源：http://lhm.hfpthk.cn

split -l 1000 big.log part_
来源：http://ksq.hnqzz.top

[R74] 批量重命名
来源：http://roh.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://joj.vqdsnc.cn

[R75] 导出环境变量
来源：http://xag.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://cwv.hywenlv.cn

[R76] 使用临时文件
来源：http://koz.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jid.nanxuanxn.top

[R77] 读取用户输入
来源：http://rtd.jyoumei.cn

read -rp "请输入: " ans
来源：http://bbl.c1oappe.top

[R78] 交互式菜单
来源：http://xek.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vks.yueranfly.top

[R79] 解析命令行选项
来源：http://wdp.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bhh.yongpay.top

[R80] 查看脚本执行耗时
来源：http://nux.wangdashe.top

time ./run.sh
来源：http://bqe.ywan-chungtsiang.top

================================================================================
来源：http://mkb.fanxiaobao.xyz

S. C / C++ 专题
来源：http://oua.hammf.cn

================================================================================
来源：http://lib.c1oappe.top

[S01] C：Hello World
来源：http://bpe.cdnleiting.top

#include <stdio.h>
来源：http://mut.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://clp.yongpay.top

[S02] C：变量与格式化输出
来源：http://bbf.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://qhu.bbcook.cn

[S03] C：读入整数
来源：http://xtk.jiagoushi.top

int x; scanf("%d", &x);
来源：http://dhy.mhx1999.top

[S04] C：字符串复制
来源：http://jeq.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://kyx.smart0.xyz

[S05] C：字符串长度
来源：http://mnq.jyoumei.cn

strlen(s)
来源：http://onq.ctjpmb.com

[S06] C：字符串比较
来源：http://okv.yvedp.cn

strcmp(a, b) == 0
来源：http://hqm.jinqigufen.top

[S07] C：数组遍历求和
来源：http://bzu.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sei.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://fzj.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://omf.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://qtb.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aqm.zhengqikj.top

[S10] C：指针与解引用
来源：http://mqp.jianghu66.top

int *p = &a;  *p = 5;
来源：http://kdo.xziqi.cn

[S11] C：逐行读文件
来源：http://rag.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://rqx.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://suc.jyoumei.cn

fclose(f);
来源：http://ylb.xuanzx.com

[S12] C：写文件
来源：http://goh.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ymq.ydjk.org.cn

[S13] C：宏定义
来源：http://uri.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdq.zdqjudy.top

[S14] C：枚举
来源：http://twl.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://vgi.ivvv.top

[S15] C：类型转换
来源：http://bju.shangyingyoupin.top

(double) a / b
来源：http://bba.yj202588.top

[S16] C：位操作置位
来源：http://zfd.shangyingyoupin.top

x |= (1 << 3);
来源：http://zsq.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://oxx.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yms.chenjidiqi.icu

[S18] C：命令行参数
来源：http://rpv.guannengcc.top

int main(int argc, char **argv)
来源：http://qdw.jqgufenzy.top

[S19] C：快速排序
来源：http://ugr.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://rwk.ppjwa.cn

[S20] C：二分查找
来源：http://sot.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sfk.hywenlv.cn

[S21] C：字符类别判断
来源：http://tcz.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://var.cqqwz.cn

[S22] C：字符串转数字
来源：http://lit.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ojq.jianghu66.top

[S23] C：随机数
来源：http://ycb.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vuh.bjfxy.top

[S24] C：获取本地时间
来源：http://csg.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ihe.yuanzhike.top

[S25] C：内存拷贝
来源：http://kpm.pycfn.com

memcpy(dst, src, n);
来源：http://vsb.aizwys.cn

[S26] C：内存清零
来源：http://uvq.fzhhl.top

memset(a, 0, sizeof a);
来源：http://hgq.redwolf501.top

[S27] C：定义常量
来源：http://afq.hongshengwenyu.top

const double PI = 3.14159;
来源：http://qle.fengsongda.top

[S28] C：静态变量
来源：http://rmp.haohaochexian.top

static int counter = 0;
来源：http://zfd.zhoulong.xyz

[S29] C：变参函数
来源：http://quf.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uqh.xuanzx.com

[S30] C：头文件保护
来源：http://mdx.xuetiantiany.cn

#ifndef X_H
来源：http://kyx.tarul.cn

#define X_H
来源：http://tst.yanxiufei.cn

#endif
来源：http://qvt.ydjk.org.cn

[S31] C++：Hello World
来源：http://mkw.sysykeji.top

#include <iostream>
来源：http://gvb.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://xtr.zhengqikj.top

[S32] C++：字符串
来源：http://vxu.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://vmd.xuanzx.com

[S33] C++：vector 增删
来源：http://nqz.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://foe.pycfn.com

[S34] C++：遍历 vector
来源：http://ibp.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://ztr.feifeiyinyue.top

[S35] C++：map
来源：http://mbt.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hcq.zdqjudy.top

[S36] C++：unordered_map
来源：http://znx.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ynm.nanxinkj.top

[S37] C++：set
来源：http://flx.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://llv.xziqi.cn

[S38] C++：排序
来源：http://vbp.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://mfl.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://ckf.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tfd.daria6918.cn

[S40] C++：查找元素
来源：http://erp.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tij.andypj.xyz

[S41] C++：类与构造函数
来源：http://nmv.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wci.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://nhf.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://twk.hcnkem.com

[S43] C++：智能指针
来源：http://kog.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://qiu.xinyue.icu

[S44] C++：引用传参
来源：http://tux.pycfn.com

void inc(int &x) { ++x; }
来源：http://mjo.chenjidiqi.icu

[S45] C++：lambda
来源：http://uvf.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xbi.hcnkem.com

[S46] C++：函数模板
来源：http://zdn.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://byb.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://wsd.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cac.zdqjudy.top

[S48] C++：逐行读文件
来源：http://qkh.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ozo.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://mwb.hesvh.cn

[S49] C++：写文件
来源：http://fvg.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tey.xinyue.icu

[S50] C++：格式化数字
来源：http://coj.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sri.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://xvv.fktsv.cn

static_cast<double>(a) / b
来源：http://fzl.havefunace.top

[S52] C++：const 与 noexcept
来源：http://prb.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://krm.andypj.xyz

[S53] C++：移动语义
来源：http://ldi.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://cae.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://bab.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ztj.ctjpmb.com

[S55] C++：结构化绑定
来源：http://nvr.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://njy.shanyushiyangkeji.top

[S56] C++：optional
来源：http://czq.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vgf.zhengqikj.top

[S57] C++：编译期常量
来源：http://fka.fktsv.cn

constexpr int N = 10;
来源：http://sau.yongpay.top

[S58] C++：命名空间
来源：http://mbl.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://yzj.yongpay.top

[S59] C++：静态断言
来源：http://itr.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cfj.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://ilw.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rem.shzxlz.cn

================================================================================
来源：http://nbw.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://guv.yuxming.cn

================================================================================
来源：http://luz.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://arf.epnwcf.com

println("Hello")
来源：http://onu.nwbrower.top

[T02] Kotlin：变量
来源：http://dzi.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pnf.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://nyj.zdqjudy.top

"值: $b"
来源：http://stb.gzhubu.top

[T04] Kotlin：空安全
来源：http://map.gogol.net.cn

val n: String? = null;  n?.length
来源：http://qpw.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://aue.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://res.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://upg.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://dbd.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://hzz.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ptu.ctjpmb.com

[T08] Kotlin：数据类
来源：http://raw.316326.xyz

data class User(val name: String, val age: Int)
来源：http://gdp.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://fjr.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://nmh.yj20258.top

[T10] Kotlin：默认参数
来源：http://rwz.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jnl.snrcjt.cn

[T11] Kotlin：协程
来源：http://tcs.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iyw.pycfn.com

[T12] Kotlin：解构声明
来源：http://nzg.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://xwa.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://ufc.xuanzx.com

val m = mapOf("a" to 1)
来源：http://auh.zhongyouzk.top

[T14] Kotlin：循环
来源：http://jfa.hnqzz.top

for (i in 1..10) println(i)
来源：http://ayt.yvedp.cn

[T15] Kotlin：接口
来源：http://flu.redwolf501.top

interface Shape { fun area(): Double }
来源：http://pop.sysykeji.top

[T16] Swift：Hello World
来源：http://nec.fengsongda.top

print("Hello")
来源：http://hik.jiagoushi.top

[T17] Swift：变量与常量
来源：http://lrr.tianlin.xyz

var a = 1;  let b = 2
来源：http://run.bbcook.cn

[T18] Swift：字符串插值
来源：http://lxm.jinqigfzy.top

"值: \(b)"
来源：http://kte.gotoacloud.top

[T19] Swift：可选绑定
来源：http://dpo.yonumen.top

if let n = opt { print(n) }
来源：http://kyy.jianghu66.top

[T20] Swift：数组操作
来源：http://rbe.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://gtq.jianghu66.top

[T21] Swift：遍历
来源：http://hns.sysykeji.top

for x in a { print(x) }
来源：http://jye.sjlbkw.cn

[T22] Swift：字典
来源：http://dvt.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://gmv.bjfxy.top

[T23] Swift：函数
来源：http://vvf.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vdh.daxiang520.top

[T24] Swift：闭包
来源：http://amc.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sgh.wangdashe.top

[T25] Swift：结构体
来源：http://oeg.aibaodan.cn

struct P { var x: Int }
来源：http://wva.hnxiangtu.top

[T26] Swift：类与重写
来源：http://guy.yonumen.top

class A: Base { override func f() {} }
来源：http://ixu.dashuyun.cn

[T27] Swift：错误处理
来源：http://vgd.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://qhf.cucudq.cn

[T28] Swift：枚举
来源：http://crg.shanyushiyangtech.top

enum Color { case red, green }
来源：http://rcg.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://qov.dashuyun.cn

guard let x = opt else { return }
来源：http://xlx.ehwqpu.com

[T30] Swift：协议
来源：http://xkq.hammf.cn

protocol Shape { func area() -> Double }
来源：http://idt.ybcxt.top

[T31] Lua：Hello World
来源：http://juo.xziqi.cn

print("Hello")
来源：http://vxl.fehbvm.com

[T32] Lua：局部变量
来源：http://hgr.zhengqikj.top

local a = 1
来源：http://jjp.vehdjk.com

[T33] Lua：表（数组）
来源：http://rkd.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bgh.iojbl.cn

[T34] Lua：遍历表
来源：http://rsg.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qpg.yanxiufei.cn

[T35] Lua：字典表
来源：http://yxr.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://yhc.hfpthk.cn

[T36] Lua：函数
来源：http://uvf.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://nas.vehdjk.com

[T37] Lua：字符串拼接
来源：http://ifp.xziqi.cn

"a" .. "b"
来源：http://hct.sjlbkw.cn

[T38] Lua：条件
来源：http://con.9152youxi.cn

if x > 0 then print("正") end
来源：http://owf.nwbrower.top

[T39] Lua：模式匹配
来源：http://pou.yanxiufei.cn

string.find(s, "%d+")
来源：http://bcz.hcnkem.com

[T40] Lua：元表
来源：http://vgb.xinyue.icu

setmetatable({}, { __index = base })
来源：http://kot.ctjpmb.com

[T41] Perl：Hello World
来源：http://bza.tian-w.cn

print "Hello\n";
来源：http://kgs.hfpthk.cn

[T42] Perl：变量类型
来源：http://aza.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ywt.bjfxy.top

[T43] Perl：字符串插值
来源：http://tjh.tanke756.top

"值: $a"
来源：http://phd.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://gwc.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://lry.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://rkb.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://jmr.yuxming.cn

[T46] Perl：哈希操作
来源：http://rwn.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gxk.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://hwt.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://rog.tarul.cn

[T48] Perl：正则替换
来源：http://sth.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://dos.fehbvm.com

[T49] Perl：函数
来源：http://zoj.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://icd.mhx1999.top

[T50] Perl：逐行读文件
来源：http://thu.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bgk.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://teb.smart0.xyz

[T51] Scala：Hello World
来源：http://vvl.ydzc1.top

println("Hello")
来源：http://ayo.fengsongda.top

[T52] Scala：变量
来源：http://cbg.haohaochexian.top

val a = 1;  var b = 2
来源：http://nvu.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://wsu.jyoumei.cn

s"值: $b"
来源：http://slx.yvedp.cn

[T54] Scala：集合映射
来源：http://wrb.quarkkingdee.top


<!-- 参考信息 -->