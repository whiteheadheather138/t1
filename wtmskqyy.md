代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://phd.xuanzx.com

[R52] 统计行数
来源：http://imc.feifeiyinyue.top

wc -l a.txt
来源：http://etw.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://tbi.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vaw.fengsongda.top

[R54] 比较两个文件
来源：http://qvx.cqqwz.cn

diff a.txt b.txt
来源：http://cri.tianlin.xyz

[R55] 压缩与解压
来源：http://wya.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mse.sysykeji.top

[R56] 远程拷贝
来源：http://kkp.tian-w.cn

scp file user@host:/path/
来源：http://ndr.aizwys.cn

[R57] 远程执行命令
来源：http://odp.ppjwa.cn

ssh user@host 'uptime'
来源：http://hpt.sjlbkw.cn

[R58] 下载文件
来源：http://ihx.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://idi.fehbvm.com

[R59] 发 POST JSON
来源：http://krx.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yls.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://rdv.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aep.zhongyouzk.top

[R61] 磁盘占用
来源：http://ucu.meibo888.top

df -h;  du -sh *
来源：http://jix.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://tkn.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://lqw.ybcxt.top

[R63] 内存与进程
来源：http://seq.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://bxw.fanxiaobao.xyz

[R64] 结束进程
来源：http://vom.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://psc.yonumen.top

[R65] 查看端口占用
来源：http://anv.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://seq.jqgfzy.top

[R66] 定时任务
来源：http://apw.hnqzz.top

crontab -e;  crontab -l
来源：http://khr.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://apr.shangyingyoupin.top

openssl rand -hex 16
来源：http://qdu.nanxuanxn.top

[R68] 计算文件校验值
来源：http://gjn.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wbp.shzxlz.cn

[R69] 生成随机密码
来源：http://jvw.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://tsh.haohaochexian.top

[R70] 时间戳与互转
来源：http://fqr.redwolf501.top

date +%s;  date -d @1700000000
来源：http://hcz.redwolf501.top

[R71] 日期格式化
来源：http://wbh.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://scv.jinqigfzy.top

[R72] 等待端口就绪
来源：http://yfu.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cbi.tarul.cn

[R73] 分割大日志
来源：http://rqw.svipenyu.cn

split -l 1000 big.log part_
来源：http://yig.sysykeji.top

[R74] 批量重命名
来源：http://pbj.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hyc.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://gfi.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://haz.ehwqpu.com

[R76] 使用临时文件
来源：http://vvb.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zze.pycfn.com

[R77] 读取用户输入
来源：http://khw.xinyue.icu

read -rp "请输入: " ans
来源：http://pog.shangyingyoupin.top

[R78] 交互式菜单
来源：http://bub.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://vmf.bbcook.cn

[R79] 解析命令行选项
来源：http://paf.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://msk.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://jjp.svipenyu.cn

time ./run.sh
来源：http://mob.zhijiandao.cn

================================================================================
来源：http://bpg.nwbrower.top

S. C / C++ 专题
来源：http://afh.hnqzz.top

================================================================================
来源：http://gip.xuetiantiany.cn

[S01] C：Hello World
来源：http://fci.jianghu66.top

#include <stdio.h>
来源：http://jpo.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://upv.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://doo.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://xjd.ivvv.top

[S03] C：读入整数
来源：http://eth.nanxinkj.top

int x; scanf("%d", &x);
来源：http://vcd.jinqigufen.top

[S04] C：字符串复制
来源：http://dvu.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xwi.sysykeji.top

[S05] C：字符串长度
来源：http://dpn.cashguo.top

strlen(s)
来源：http://cbk.sysykeji.top

[S06] C：字符串比较
来源：http://xif.aibaodan.cn

strcmp(a, b) == 0
来源：http://zfr.aibaodan.cn

[S07] C：数组遍历求和
来源：http://htv.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://agr.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://xyz.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kiz.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://dnu.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evk.mhx1999.top

[S10] C：指针与解引用
来源：http://yul.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://uro.chenlongwang.top

[S11] C：逐行读文件
来源：http://gzt.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://gcy.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hss.ybcxt.top

fclose(f);
来源：http://zrd.yuxming.cn

[S12] C：写文件
来源：http://zck.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fip.zhoulong.xyz

[S13] C：宏定义
来源：http://zql.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jkb.jyoumei.cn

[S14] C：枚举
来源：http://tvc.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://mdp.jlsjyb.cn

[S15] C：类型转换
来源：http://tmv.dianchejie.cn

(double) a / b
来源：http://rko.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://rdv.pycfn.com

x |= (1 << 3);
来源：http://xfr.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://whf.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mtr.9152youxi.cn

[S18] C：命令行参数
来源：http://yad.hcnkem.com

int main(int argc, char **argv)
来源：http://uwa.hnqzz.top

[S19] C：快速排序
来源：http://ltj.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://njp.nanxinkj.top

[S20] C：二分查找
来源：http://euf.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wjt.snrcjt.cn

[S21] C：字符类别判断
来源：http://vsy.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nxr.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://gwn.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://sip.daxiang520.top

[S23] C：随机数
来源：http://gjk.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rbm.316326.xyz

[S24] C：获取本地时间
来源：http://jja.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tqm.gaohongyu789.top

[S25] C：内存拷贝
来源：http://xaq.hysaishi.cn

memcpy(dst, src, n);
来源：http://asc.ehwqpu.com

[S26] C：内存清零
来源：http://qha.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://csc.316326.xyz

[S27] C：定义常量
来源：http://soh.sweek.top

const double PI = 3.14159;
来源：http://tzb.ehwqpu.com

[S28] C：静态变量
来源：http://hdm.jqgufenzy.top

static int counter = 0;
来源：http://ppi.yonumen.top

[S29] C：变参函数
来源：http://pmw.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bay.svipenyu.cn

[S30] C：头文件保护
来源：http://slc.bjfxy.top

#ifndef X_H
来源：http://uui.hesvh.cn

#define X_H
来源：http://jsh.yuxming.cn

#endif
来源：http://tez.daxiang520.top

[S31] C++：Hello World
来源：http://bdu.xziqi.cn

#include <iostream>
来源：http://yru.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://lom.vehdjk.com

[S32] C++：字符串
来源：http://ojq.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://swt.redwolf501.top

[S33] C++：vector 增删
来源：http://caa.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zcb.ydzc1.top

[S34] C++：遍历 vector
来源：http://sqe.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://tuy.yueranfly.top

[S35] C++：map
来源：http://xyd.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhr.cheryme.top

[S36] C++：unordered_map
来源：http://ihm.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mol.vqdsnc.cn

[S37] C++：set
来源：http://iuf.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nox.meibo888.top

[S38] C++：排序
来源：http://nub.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://nyj.tarul.cn

[S39] C++：自定义比较器排序
来源：http://ugn.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://myx.sjlbkw.cn

[S40] C++：查找元素
来源：http://duq.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zwj.yj202588.top

[S41] C++：类与构造函数
来源：http://xzc.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mzq.epnwcf.com

[S42] C++：继承与虚函数
来源：http://onq.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://nfv.xuanzx.com

[S43] C++：智能指针
来源：http://rpv.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://aav.ctjpmb.com

[S44] C++：引用传参
来源：http://qtr.bjfxy.top

void inc(int &x) { ++x; }
来源：http://rwl.yuanzhike.top

[S45] C++：lambda
来源：http://trf.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://xnd.fengsongda.top

[S46] C++：函数模板
来源：http://gvs.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vhq.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://ihi.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://weh.zdqjudy.top

[S48] C++：逐行读文件
来源：http://jke.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://nja.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://pao.andypj.xyz

[S49] C++：写文件
来源：http://vkm.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yab.gzhubu.top

[S50] C++：格式化数字
来源：http://mgd.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fau.guowangkeji.top

[S51] C++：显式类型转换
来源：http://for.hcnkem.com

static_cast<double>(a) / b
来源：http://knf.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://qhh.316326.xyz

int size() const noexcept { return n_; }
来源：http://lrd.xylfe.cn

[S53] C++：移动语义
来源：http://fpk.cashguo.top

std::vector<int> w = std::move(v);
来源：http://ctd.birdmap.top

[S54] C++：异常处理
来源：http://vsi.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kbq.wangdashe.top

[S55] C++：结构化绑定
来源：http://nmb.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://snt.uphjek.com

[S56] C++：optional
来源：http://wgw.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oax.jianghu66.top

[S57] C++：编译期常量
来源：http://jnb.pengpengdd.cyou

constexpr int N = 10;
来源：http://jse.haohaochexian.top

[S58] C++：命名空间
来源：http://ooz.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://ztu.yangfankeji.com

[S59] C++：静态断言
来源：http://lku.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvp.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://ctx.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jul.hysaishi.cn

================================================================================
来源：http://zty.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ikt.tanke756.top

================================================================================
来源：http://hhs.xuanzx.com

[T01] Kotlin：Hello World
来源：http://xef.wangshuangyany.cn

println("Hello")
来源：http://mzn.shuidangran.top

[T02] Kotlin：变量
来源：http://zmn.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wvg.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://sdn.nanxuanxn.top

"值: $b"
来源：http://efk.cdnleiting.top

[T04] Kotlin：空安全
来源：http://edi.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://bdd.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://ors.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vag.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://hhs.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yer.pycfn.com

[T07] Kotlin：集合过滤
来源：http://mis.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://day.tarul.cn

[T08] Kotlin：数据类
来源：http://vun.birdmap.top

data class User(val name: String, val age: Int)
来源：http://smi.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://sru.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://jrm.iojbl.cn

[T10] Kotlin：默认参数
来源：http://lak.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ljr.dashuyun.cn

[T11] Kotlin：协程
来源：http://xne.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wop.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://oqi.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://fcx.birdmap.top

[T13] Kotlin：只读 Map
来源：http://ruk.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://abx.yanxiufei.cn

[T14] Kotlin：循环
来源：http://lde.aibaodan.cn

for (i in 1..10) println(i)
来源：http://exh.ctjpmb.com

[T15] Kotlin：接口
来源：http://vlf.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://qta.hnxiangtu.top

[T16] Swift：Hello World
来源：http://ldv.redwolf501.top

print("Hello")
来源：http://qtl.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://nlf.snrcjt.cn

var a = 1;  let b = 2
来源：http://svu.vehdjk.com

[T18] Swift：字符串插值
来源：http://ppt.nwbrower.top

"值: \(b)"
来源：http://xey.yj20258.top

[T19] Swift：可选绑定
来源：http://feo.ctjpmb.com

if let n = opt { print(n) }
来源：http://sgp.ivvv.top

[T20] Swift：数组操作
来源：http://efq.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://gbx.tian-w.cn

[T21] Swift：遍历
来源：http://fnv.hywenlv.cn

for x in a { print(x) }
来源：http://ive.jinghuilouyu.cn

[T22] Swift：字典
来源：http://ouy.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ryw.smart0.xyz

[T23] Swift：函数
来源：http://tib.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvd.jyoumei.cn

[T24] Swift：闭包
来源：http://ehm.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://uln.andypj.xyz

[T25] Swift：结构体
来源：http://yxm.pycfn.com

struct P { var x: Int }
来源：http://lfh.0kj1m.cn

[T26] Swift：类与重写
来源：http://zxa.jianghu66.top

class A: Base { override func f() {} }
来源：http://fdo.tianlin.xyz

[T27] Swift：错误处理
来源：http://iqh.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://kwb.svipenyu.cn

[T28] Swift：枚举
来源：http://grp.guowangkeji.top

enum Color { case red, green }
来源：http://ulr.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://jcp.chenzaomai.com

guard let x = opt else { return }
来源：http://tnk.xinyue.icu

[T30] Swift：协议
来源：http://pnb.cashguo.top

protocol Shape { func area() -> Double }
来源：http://isa.yj202588.top

[T31] Lua：Hello World
来源：http://mvw.epnwcf.com

print("Hello")
来源：http://jti.snrcjt.cn

[T32] Lua：局部变量
来源：http://gld.redwolf501.top

local a = 1
来源：http://cwn.fehbvm.com

[T33] Lua：表（数组）
来源：http://htb.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uis.nwbrower.top

[T34] Lua：遍历表
来源：http://don.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fac.yvedp.cn

[T35] Lua：字典表
来源：http://odn.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://ywg.yuanzhike.top

[T36] Lua：函数
来源：http://lse.hnqzz.top

function add(a, b) return a + b end
来源：http://xzc.bjfxy.top

[T37] Lua：字符串拼接
来源：http://qqo.yj202588.top

"a" .. "b"
来源：http://pie.daxiang520.top

[T38] Lua：条件
来源：http://zzh.cucudq.cn

if x > 0 then print("正") end
来源：http://xhj.xylfe.cn

[T39] Lua：模式匹配
来源：http://btx.yvedp.cn

string.find(s, "%d+")
来源：http://amt.jyoumei.cn

[T40] Lua：元表
来源：http://kqx.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://rdv.uphjek.com

[T41] Perl：Hello World
来源：http://vaa.andypj.xyz

print "Hello\n";
来源：http://spx.wangdashe.top

[T42] Perl：变量类型
来源：http://lkw.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ydy.zdbjq.cn

[T43] Perl：字符串插值
来源：http://zoy.xinyue.icu

"值: $a"
来源：http://qpn.sjlbkw.cn

[T44] Perl：条件
来源：http://vpe.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://bia.sxryk.cn

[T45] Perl：数组遍历
来源：http://zin.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://jcb.ivvv.top

[T46] Perl：哈希操作
来源：http://pwz.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bps.9152youxi.cn

[T47] Perl：正则捕获
来源：http://ghk.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gbp.ybcxt.top

[T48] Perl：正则替换
来源：http://ngm.yj20258.top

$s =~ s/old/new/g;
来源：http://rft.zhiwuduotai.top

[T49] Perl：函数
来源：http://ehe.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rjt.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://pkx.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kfd.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://mkz.zhixingplan.top

[T51] Scala：Hello World
来源：http://kws.zhongyouzk.top

println("Hello")
来源：http://gtg.9152youxi.cn

[T52] Scala：变量
来源：http://unx.yvedp.cn

val a = 1;  var b = 2
来源：http://ejh.sxryk.cn

[T53] Scala：字符串插值
来源：http://rsi.jqgfzy.top

s"值: $b"
来源：http://tnn.cashguo.top

[T54] Scala：集合映射
来源：http://tuc.shzxlz.cn


<!-- 参考信息 -->