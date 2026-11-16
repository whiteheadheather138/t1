代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://gqj.vqdsnc.cn

[R48] awk 取指定列
来源：http://nkk.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://ofh.hnqzz.top

[R49] awk 带条件
来源：http://tzs.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uuj.zycfv.cn

[R50] awk 求和
来源：http://ymx.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://scf.tianlin.xyz

[R51] 排序去重取前几
来源：http://vkw.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://awe.zhijiandao.cn

[R52] 统计行数
来源：http://fat.xylfe.cn

wc -l a.txt
来源：http://uty.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://ccw.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://idj.cdnleiting.top

[R54] 比较两个文件
来源：http://htf.tianlin.xyz

diff a.txt b.txt
来源：http://dlu.epnwcf.com

[R55] 压缩与解压
来源：http://xus.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://khg.nwbrower.top

[R56] 远程拷贝
来源：http://vpp.andypj.xyz

scp file user@host:/path/
来源：http://qob.dianchejie.cn

[R57] 远程执行命令
来源：http://lwv.tianlin.xyz

ssh user@host 'uptime'
来源：http://qwh.c1oappe.top

[R58] 下载文件
来源：http://jzp.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nxy.9152youxi.cn

[R59] 发 POST JSON
来源：http://znw.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fqr.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://exp.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zyi.fehbvm.com

[R61] 磁盘占用
来源：http://gpu.zhoulong.xyz

df -h;  du -sh *
来源：http://nhz.yonumen.top

[R62] 找最占空间的文件
来源：http://nfv.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://hcm.fzhhl.top

[R63] 内存与进程
来源：http://ebn.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://kke.kuanghao11.cn

[R64] 结束进程
来源：http://otz.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://thm.epnwcf.com

[R65] 查看端口占用
来源：http://thd.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://udd.cheryme.top

[R66] 定时任务
来源：http://xwv.jqgufenzy.top

crontab -e;  crontab -l
来源：http://dat.shuidangran.top

[R67] 生成随机十六进制串
来源：http://hqz.hysaishi.cn

openssl rand -hex 16
来源：http://mks.gaohongyu789.top

[R68] 计算文件校验值
来源：http://ccb.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://aiw.zhoulong.xyz

[R69] 生成随机密码
来源：http://mnw.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://mav.yangfankeji.com

[R70] 时间戳与互转
来源：http://veu.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://ygh.zhengqikj.top

[R71] 日期格式化
来源：http://bzt.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rfp.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://qgx.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yqg.ivvv.top

[R73] 分割大日志
来源：http://xjb.cqqwz.cn

split -l 1000 big.log part_
来源：http://zuo.tian-w.cn

[R74] 批量重命名
来源：http://fel.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tzc.tarul.cn

[R75] 导出环境变量
来源：http://xsa.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://emk.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://wyc.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://amp.guowangkeji.top

[R77] 读取用户输入
来源：http://vkz.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://xfo.zdqjudy.top

[R78] 交互式菜单
来源：http://mpc.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xnl.yonumen.top

[R79] 解析命令行选项
来源：http://nbg.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pmv.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://kst.epnwcf.com

time ./run.sh
来源：http://bdz.tianlin.xyz

================================================================================
来源：http://dka.hfpthk.cn

S. C / C++ 专题
来源：http://nbr.zhiwuduotai.top

================================================================================
来源：http://hdh.yonumen.top

[S01] C：Hello World
来源：http://lwi.zdbjq.cn

#include <stdio.h>
来源：http://ozd.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wgp.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://pnp.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://zlx.yj20258.top

[S03] C：读入整数
来源：http://czo.ppjwa.cn

int x; scanf("%d", &x);
来源：http://bzg.jinqigfzy.top

[S04] C：字符串复制
来源：http://naa.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://lbf.zhongyouzk.top

[S05] C：字符串长度
来源：http://vao.nanxinkj.top

strlen(s)
来源：http://dsx.sxryk.cn

[S06] C：字符串比较
来源：http://kny.yuanzhike.top

strcmp(a, b) == 0
来源：http://yai.ehwqpu.com

[S07] C：数组遍历求和
来源：http://xgp.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://onq.uphjek.com

[S08] C：动态内存分配与释放
来源：http://maa.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xff.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://zdr.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fyv.gzhubu.top

[S10] C：指针与解引用
来源：http://fmq.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://rjt.andypj.xyz

[S11] C：逐行读文件
来源：http://nup.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://uoj.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://cnb.c1oappe.top

fclose(f);
来源：http://zdo.hnqzz.top

[S12] C：写文件
来源：http://oxm.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hji.gaohongyu789.top

[S13] C：宏定义
来源：http://esd.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bky.9152youxi.cn

[S14] C：枚举
来源：http://pwq.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://lak.fzhhl.top

[S15] C：类型转换
来源：http://utt.ehwqpu.com

(double) a / b
来源：http://cbb.bbcook.cn

[S16] C：位操作置位
来源：http://xyf.ydjk.org.cn

x |= (1 << 3);
来源：http://dil.52xcode.cn

[S17] C：安全拼接字符串
来源：http://mou.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qxk.chenjidiqi.icu

[S18] C：命令行参数
来源：http://lgk.havefunace.top

int main(int argc, char **argv)
来源：http://xys.guannengcc.top

[S19] C：快速排序
来源：http://kux.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nlb.0kj1m.cn

[S20] C：二分查找
来源：http://kmg.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ptj.daria6918.cn

[S21] C：字符类别判断
来源：http://ynw.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wjz.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://opv.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://tqz.meibo888.top

[S23] C：随机数
来源：http://kfg.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uai.yuanzhike.top

[S24] C：获取本地时间
来源：http://oaq.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://udi.0kj1m.cn

[S25] C：内存拷贝
来源：http://mtn.yangfankeji.com

memcpy(dst, src, n);
来源：http://rzv.aizwys.cn

[S26] C：内存清零
来源：http://xlu.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://yho.snrcjt.cn

[S27] C：定义常量
来源：http://zpm.yuanzhike.top

const double PI = 3.14159;
来源：http://gxo.shuidangran.top

[S28] C：静态变量
来源：http://abs.shangyingyoupin.top

static int counter = 0;
来源：http://nxs.jiagoushi.top

[S29] C：变参函数
来源：http://mtb.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://awm.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://gfr.quarkkingdee.top

#ifndef X_H
来源：http://qle.jiagoushi.top

#define X_H
来源：http://dkb.tian-w.cn

#endif
来源：http://roe.zhixingplan.top

[S31] C++：Hello World
来源：http://xek.chenjidiqi.icu

#include <iostream>
来源：http://xjf.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ltx.gaohongyu789.top

[S32] C++：字符串
来源：http://zjl.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://tez.shzxlz.cn

[S33] C++：vector 增删
来源：http://pgu.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fxu.yuanzhike.top

[S34] C++：遍历 vector
来源：http://anf.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://wvs.jyoumei.cn

[S35] C++：map
来源：http://jju.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wce.sysykeji.top

[S36] C++：unordered_map
来源：http://kez.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cny.zycfv.cn

[S37] C++：set
来源：http://qhc.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kre.iojbl.cn

[S38] C++：排序
来源：http://cpx.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://kat.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://utv.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://knp.9152youxi.cn

[S40] C++：查找元素
来源：http://lxq.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bgn.cheryme.top

[S41] C++：类与构造函数
来源：http://wsn.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gyh.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://qdo.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://qvq.dashuyun.cn

[S43] C++：智能指针
来源：http://liq.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://bol.mhx1999.top

[S44] C++：引用传参
来源：http://dxl.redwolf501.top

void inc(int &x) { ++x; }
来源：http://vim.wangdashe.top

[S45] C++：lambda
来源：http://igj.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xri.pycfn.com

[S46] C++：函数模板
来源：http://miv.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dwz.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://dxg.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xxl.hnqzz.top

[S48] C++：逐行读文件
来源：http://xph.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://ljy.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://gnf.jqgufenzy.top

[S49] C++：写文件
来源：http://uus.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tvz.vqdsnc.cn

[S50] C++：格式化数字
来源：http://rxl.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ygc.hcnkem.com

[S51] C++：显式类型转换
来源：http://rru.yj20258.top

static_cast<double>(a) / b
来源：http://tsc.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://qhu.iojbl.cn

int size() const noexcept { return n_; }
来源：http://wnp.dashuyun.cn

[S53] C++：移动语义
来源：http://flq.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://nxz.xuetiantiany.cn

[S54] C++：异常处理
来源：http://wvo.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mht.yvedp.cn

[S55] C++：结构化绑定
来源：http://zzk.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ztt.ivvv.top

[S56] C++：optional
来源：http://xea.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wcb.yj20258.top

[S57] C++：编译期常量
来源：http://bsk.andypj.xyz

constexpr int N = 10;
来源：http://wvs.sufxvd.cn

[S58] C++：命名空间
来源：http://dit.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://iqj.vqdsnc.cn

[S59] C++：静态断言
来源：http://wzf.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yyr.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://sqs.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ojt.dianchejie.cn

================================================================================
来源：http://pfp.daria6918.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdy.nanxuanxn.top

================================================================================
来源：http://jxu.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://fko.shuidangran.top

println("Hello")
来源：http://wur.chenlongwang.top

[T02] Kotlin：变量
来源：http://tuz.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://klh.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://eav.gogol.net.cn

"值: $b"
来源：http://bgw.chenzaomai.com

[T04] Kotlin：空安全
来源：http://wwq.cqqwz.cn

val n: String? = null;  n?.length
来源：http://izu.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://iiv.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nat.pycfn.com

[T06] Kotlin：集合映射
来源：http://pcu.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gsp.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://xse.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mab.daxiang520.top

[T08] Kotlin：数据类
来源：http://wye.316326.xyz

data class User(val name: String, val age: Int)
来源：http://bcw.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://lsi.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://qaw.hcnkem.com

[T10] Kotlin：默认参数
来源：http://aqe.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xpl.ppjwa.cn

[T11] Kotlin：协程
来源：http://bla.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://whw.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://ssn.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://zdk.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://vnr.meibo888.top

val m = mapOf("a" to 1)
来源：http://sbf.hfpthk.cn

[T14] Kotlin：循环
来源：http://kkl.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://uoc.sweek.top

[T15] Kotlin：接口
来源：http://yla.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://qaj.tian-w.cn

[T16] Swift：Hello World
来源：http://vlg.9152youxi.cn

print("Hello")
来源：http://sqn.dashuyun.cn

[T17] Swift：变量与常量
来源：http://jxz.zdbjq.cn

var a = 1;  let b = 2
来源：http://qhd.cqqwz.cn

[T18] Swift：字符串插值
来源：http://zss.nwbrower.top

"值: \(b)"
来源：http://gmu.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://gsa.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://cri.yangfankeji.com

[T20] Swift：数组操作
来源：http://qhc.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://kjj.hfpthk.cn

[T21] Swift：遍历
来源：http://odq.jiagoushi.top

for x in a { print(x) }
来源：http://xss.yuanzhike.top

[T22] Swift：字典
来源：http://tmo.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bjt.52xcode.cn

[T23] Swift：函数
来源：http://gxl.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tsj.nwbrower.top

[T24] Swift：闭包
来源：http://oou.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eka.cucudq.cn

[T25] Swift：结构体
来源：http://phr.jqgfzy.top

struct P { var x: Int }
来源：http://uiz.xylfe.cn

[T26] Swift：类与重写
来源：http://wif.jyoumei.cn

class A: Base { override func f() {} }
来源：http://cdq.zdqjudy.top

[T27] Swift：错误处理
来源：http://ztz.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://mkv.jinqigfzy.top

[T28] Swift：枚举
来源：http://qhq.9152youxi.cn

enum Color { case red, green }
来源：http://aaw.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://rev.zycfv.cn

guard let x = opt else { return }
来源：http://crh.sysykeji.top

[T30] Swift：协议
来源：http://hnr.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://yjz.chenlongwang.top

[T31] Lua：Hello World
来源：http://ase.yueranfly.top

print("Hello")
来源：http://jhs.iojbl.cn

[T32] Lua：局部变量
来源：http://ona.jqgufenzy.top

local a = 1
来源：http://ghj.andypj.xyz

[T33] Lua：表（数组）
来源：http://iha.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ebg.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://wky.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ict.yj20258888.top

[T35] Lua：字典表
来源：http://kzq.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://fuk.hnqzz.top

[T36] Lua：函数
来源：http://mpw.nanxuanxn.top

function add(a, b) return a + b end
来源：http://ukj.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://gry.yangfankeji.com

"a" .. "b"
来源：http://lbv.52xcode.cn

[T38] Lua：条件
来源：http://fuk.epnwcf.com

if x > 0 then print("正") end
来源：http://yhl.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://jrl.yvedp.cn

string.find(s, "%d+")
来源：http://fgo.hcnkem.com

[T40] Lua：元表
来源：http://njj.sweek.top

setmetatable({}, { __index = base })
来源：http://nhk.zycfv.cn

[T41] Perl：Hello World
来源：http://tvw.gotoacloud.top

print "Hello\n";
来源：http://wkq.snrcjt.cn

[T42] Perl：变量类型
来源：http://xwr.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://auz.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://ldy.andypj.xyz

"值: $a"
来源：http://mpg.xinyue.icu

[T44] Perl：条件
来源：http://lmc.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://aoa.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://qwv.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://zwj.shuidangran.top

[T46] Perl：哈希操作
来源：http://uwz.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uld.ehwqpu.com

[T47] Perl：正则捕获
来源：http://rjk.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zzu.quarkkingdee.top

[T48] Perl：正则替换
来源：http://xxy.yuanzhike.top

$s =~ s/old/new/g;
来源：http://xxl.hongshengwenyu.top

[T49] Perl：函数
来源：http://jxz.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://shi.zycfv.cn

[T50] Perl：逐行读文件
来源：http://lqx.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wjj.mhx1999.top


<!-- 参考信息 -->