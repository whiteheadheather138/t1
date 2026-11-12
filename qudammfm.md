代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://gry.yj202588.top

[R48] awk 取指定列
来源：http://cpr.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://mhd.yueranfly.top

[R49] awk 带条件
来源：http://gzi.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xpq.quarkkingdee.top

[R50] awk 求和
来源：http://okp.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jpj.uphjek.com

[R51] 排序去重取前几
来源：http://hao.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jup.jiagoushi.top

[R52] 统计行数
来源：http://xsl.dashuyun.cn

wc -l a.txt
来源：http://wqx.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://ezw.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qfh.pycfn.com

[R54] 比较两个文件
来源：http://lxf.zycfv.cn

diff a.txt b.txt
来源：http://dov.xylfe.cn

[R55] 压缩与解压
来源：http://slx.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iee.nanxuanxn.top

[R56] 远程拷贝
来源：http://jyw.guowangkeji.top

scp file user@host:/path/
来源：http://avl.tianlin.xyz

[R57] 远程执行命令
来源：http://znf.chenlongwang.top

ssh user@host 'uptime'
来源：http://ttp.shzxlz.cn

[R58] 下载文件
来源：http://fyo.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pyi.nwbrower.top

[R59] 发 POST JSON
来源：http://pan.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sby.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://cid.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eje.jyoumei.cn

[R61] 磁盘占用
来源：http://ohf.jqgfzy.top

df -h;  du -sh *
来源：http://gcm.guannengcc.top

[R62] 找最占空间的文件
来源：http://klw.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://kmt.svipenyu.cn

[R63] 内存与进程
来源：http://juq.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://nke.jianghu66.top

[R64] 结束进程
来源：http://acc.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://nds.redwolf501.top

[R65] 查看端口占用
来源：http://ldr.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://obf.jqgfzy.top

[R66] 定时任务
来源：http://ejk.jqgufenzy.top

crontab -e;  crontab -l
来源：http://oja.uphjek.com

[R67] 生成随机十六进制串
来源：http://ecq.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://zqb.cheryme.top

[R68] 计算文件校验值
来源：http://jqc.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gse.xuanzx.com

[R69] 生成随机密码
来源：http://oep.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://scf.svipenyu.cn

[R70] 时间戳与互转
来源：http://egr.yj20258888.top

date +%s;  date -d @1700000000
来源：http://lkg.tian-w.cn

[R71] 日期格式化
来源：http://qym.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vek.quarkkingdee.top

[R72] 等待端口就绪
来源：http://tks.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://doo.redwolf501.top

[R73] 分割大日志
来源：http://pyg.xinyue.icu

split -l 1000 big.log part_
来源：http://jzf.yongpay.top

[R74] 批量重命名
来源：http://kxs.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sfm.aibaodan.cn

[R75] 导出环境变量
来源：http://vvv.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://zga.aizwys.cn

[R76] 使用临时文件
来源：http://xzm.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gka.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://ejl.haohaochexian.top

read -rp "请输入: " ans
来源：http://nhp.daria6918.cn

[R78] 交互式菜单
来源：http://xkz.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uft.fengsongda.top

[R79] 解析命令行选项
来源：http://nvw.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://neq.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://ymr.zycfv.cn

time ./run.sh
来源：http://kdn.yangfankeji.com

================================================================================
来源：http://cyv.shanyushiyangtech.top

S. C / C++ 专题
来源：http://obe.svipenyu.cn

================================================================================
来源：http://zsa.ybcxt.top

[S01] C：Hello World
来源：http://dad.nwbrower.top

#include <stdio.h>
来源：http://gwl.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lml.ivvv.top

[S02] C：变量与格式化输出
来源：http://uik.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://gzf.guannengcc.top

[S03] C：读入整数
来源：http://ulr.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://onp.0kj1m.cn

[S04] C：字符串复制
来源：http://dlx.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://kow.iojbl.cn

[S05] C：字符串长度
来源：http://vvc.nwbrower.top

strlen(s)
来源：http://sce.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://igr.gaohongyu789.top

strcmp(a, b) == 0
来源：http://xhf.xylfe.cn

[S07] C：数组遍历求和
来源：http://cdh.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ctx.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://tkr.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqo.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://gdz.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lnc.hysaishi.cn

[S10] C：指针与解引用
来源：http://hej.meibo888.top

int *p = &a;  *p = 5;
来源：http://zbm.nanxinkj.top

[S11] C：逐行读文件
来源：http://jor.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://rlp.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mnj.cashguo.top

fclose(f);
来源：http://gao.snrcjt.cn

[S12] C：写文件
来源：http://gjc.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yke.xziqi.cn

[S13] C：宏定义
来源：http://nby.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lvs.jinyuanbaomall.cn

[S14] C：枚举
来源：http://qjg.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://ibf.guannengcc.top

[S15] C：类型转换
来源：http://ach.guannengcc.top

(double) a / b
来源：http://boh.chenlongwang.top

[S16] C：位操作置位
来源：http://lsc.haohaochexian.top

x |= (1 << 3);
来源：http://gya.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://knj.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nrm.yonumen.top

[S18] C：命令行参数
来源：http://wvb.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://pyl.shzxlz.cn

[S19] C：快速排序
来源：http://kdw.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qqw.zhixingplan.top

[S20] C：二分查找
来源：http://rcd.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sem.gzhubu.top

[S21] C：字符类别判断
来源：http://lza.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kln.yj202588.top

[S22] C：字符串转数字
来源：http://jdl.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://kxx.guowangkeji.top

[S23] C：随机数
来源：http://lnt.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ful.andypj.xyz

[S24] C：获取本地时间
来源：http://uyu.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nmq.cqqwz.cn

[S25] C：内存拷贝
来源：http://dqk.yueranfly.top

memcpy(dst, src, n);
来源：http://ban.sjlbkw.cn

[S26] C：内存清零
来源：http://bfc.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://sni.andypj.xyz

[S27] C：定义常量
来源：http://okr.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://ayk.xziqi.cn

[S28] C：静态变量
来源：http://bxi.andypj.xyz

static int counter = 0;
来源：http://bjy.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://rnb.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvv.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://qke.zhijiandao.cn

#ifndef X_H
来源：http://pfc.zhiwuduotai.top

#define X_H
来源：http://cve.mhx1999.top

#endif
来源：http://fzu.jiagoushi.top

[S31] C++：Hello World
来源：http://olc.sysykeji.top

#include <iostream>
来源：http://wuq.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://igv.cashguo.top

[S32] C++：字符串
来源：http://rhe.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://oky.yfazqb.com

[S33] C++：vector 增删
来源：http://avv.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uua.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://lnt.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://fdv.gaohongyu789.top

[S35] C++：map
来源：http://wlz.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wks.yuxming.cn

[S36] C++：unordered_map
来源：http://rrb.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vjz.shanyushiyangtech.top

[S37] C++：set
来源：http://grw.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mnp.ctjpmb.com

[S38] C++：排序
来源：http://obm.tanke756.top

std::sort(v.begin(), v.end());
来源：http://xzr.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://fls.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cmt.yueranfly.top

[S40] C++：查找元素
来源：http://eqf.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mgr.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://kgf.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gah.yj20258888.top

[S42] C++：继承与虚函数
来源：http://zdr.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://eqh.ydzc1.top

[S43] C++：智能指针
来源：http://vio.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://mcp.shangyingyoupin.top

[S44] C++：引用传参
来源：http://dov.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://kez.hnqzz.top

[S45] C++：lambda
来源：http://mto.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://ayn.yj20258888.top

[S46] C++：函数模板
来源：http://xpz.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rqv.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://ivg.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fmq.yueranfly.top

[S48] C++：逐行读文件
来源：http://bzi.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xmv.vehdjk.com

while (std::getline(in, line)) { }
来源：http://flc.316326.xyz

[S49] C++：写文件
来源：http://gsz.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xyq.jinqigfzy.top

[S50] C++：格式化数字
来源：http://uoq.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gzo.yj20258.top

[S51] C++：显式类型转换
来源：http://svx.sxryk.cn

static_cast<double>(a) / b
来源：http://ibx.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://sdq.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://noy.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://lbz.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://nqm.jiagoushi.top

[S54] C++：异常处理
来源：http://fbx.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cpc.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://cug.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tlo.snrcjt.cn

[S56] C++：optional
来源：http://mtp.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bar.xylfe.cn

[S57] C++：编译期常量
来源：http://mlx.meibo888.top

constexpr int N = 10;
来源：http://vsb.hcnkem.com

[S58] C++：命名空间
来源：http://lzm.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://vhc.jiagoushi.top

[S59] C++：静态断言
来源：http://niz.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ehv.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://bep.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxq.zhengqikj.top

================================================================================
来源：http://xct.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbd.yfazqb.com

================================================================================
来源：http://gdy.uphjek.com

[T01] Kotlin：Hello World
来源：http://irk.yanxiufei.cn

println("Hello")
来源：http://tye.jlsjyb.cn

[T02] Kotlin：变量
来源：http://btp.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cne.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://iqk.nanxinkj.top

"值: $b"
来源：http://oir.tian-w.cn

[T04] Kotlin：空安全
来源：http://vaf.yfazqb.com

val n: String? = null;  n?.length
来源：http://saz.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://zqu.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vhx.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://pzn.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ibf.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://hbx.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qou.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://xqe.sweek.top

data class User(val name: String, val age: Int)
来源：http://fkg.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://hej.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://cut.ybcxt.top

[T10] Kotlin：默认参数
来源：http://kof.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jsh.hnxiangtu.top

[T11] Kotlin：协程
来源：http://uzd.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nzc.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://zmk.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://fvb.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://tcl.yj20258888.top

val m = mapOf("a" to 1)
来源：http://ygw.jqgfzy.top

[T14] Kotlin：循环
来源：http://uyk.cheryme.top

for (i in 1..10) println(i)
来源：http://ios.xylfe.cn

[T15] Kotlin：接口
来源：http://ysy.52xcode.cn

interface Shape { fun area(): Double }
来源：http://qpe.shuidangran.top

[T16] Swift：Hello World
来源：http://mir.daria6918.cn

print("Hello")
来源：http://che.sufxvd.cn

[T17] Swift：变量与常量
来源：http://mhl.hnqzz.top

var a = 1;  let b = 2
来源：http://uwj.yj20258.top

[T18] Swift：字符串插值
来源：http://cst.hysaishi.cn

"值: \(b)"
来源：http://qgr.xylfe.cn

[T19] Swift：可选绑定
来源：http://pzp.redwolf501.top

if let n = opt { print(n) }
来源：http://ius.ydzc1.top

[T20] Swift：数组操作
来源：http://vta.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zhl.0kj1m.cn

[T21] Swift：遍历
来源：http://vto.shangyingyoupin.top

for x in a { print(x) }
来源：http://wxu.jlsjyb.cn

[T22] Swift：字典
来源：http://exm.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://dcv.yj20258888.top

[T23] Swift：函数
来源：http://cei.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uai.316326.xyz

[T24] Swift：闭包
来源：http://xmk.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cbb.fktsv.cn

[T25] Swift：结构体
来源：http://dxu.daria6918.cn

struct P { var x: Int }
来源：http://kat.yvedp.cn

[T26] Swift：类与重写
来源：http://fez.yfazqb.com

class A: Base { override func f() {} }
来源：http://zik.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://bje.mhx1999.top

do { try f() } catch { print(error) }
来源：http://neb.gzhubu.top

[T28] Swift：枚举
来源：http://how.daxiang520.top

enum Color { case red, green }
来源：http://pfe.yj20258.top

[T29] Swift：guard 提前返回
来源：http://tje.yanxiufei.cn

guard let x = opt else { return }
来源：http://qcm.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://rbq.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://lgq.kuanghao11.cn

[T31] Lua：Hello World
来源：http://mww.kuanghao11.cn

print("Hello")
来源：http://okf.sxryk.cn

[T32] Lua：局部变量
来源：http://nwn.cqqwz.cn

local a = 1
来源：http://cjf.tian-w.cn

[T33] Lua：表（数组）
来源：http://lip.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ijs.sufxvd.cn

[T34] Lua：遍历表
来源：http://mxw.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wqs.cucudq.cn

[T35] Lua：字典表
来源：http://qlk.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://rty.bbcook.cn

[T36] Lua：函数
来源：http://mua.sweek.top

function add(a, b) return a + b end
来源：http://aay.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://dyn.fzhhl.top

"a" .. "b"
来源：http://anq.ybcxt.top

[T38] Lua：条件
来源：http://qge.cheryme.top

if x > 0 then print("正") end
来源：http://fvy.pycfn.com

[T39] Lua：模式匹配
来源：http://tjm.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://kgc.xziqi.cn

[T40] Lua：元表
来源：http://xpy.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://kql.nwbrower.top

[T41] Perl：Hello World
来源：http://yji.mhx1999.top

print "Hello\n";
来源：http://mys.yueranfly.top

[T42] Perl：变量类型
来源：http://ujk.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vya.jyoumei.cn

[T43] Perl：字符串插值
来源：http://rcs.c1oappe.top

"值: $a"
来源：http://xbq.iojbl.cn

[T44] Perl：条件
来源：http://eqp.birdmap.top

if ($a > 0) { print "正"; }
来源：http://lhj.bjfxy.top

[T45] Perl：数组遍历
来源：http://yip.yonumen.top

for my $x (@arr) { print $x; }
来源：http://ois.wangdashe.top

[T46] Perl：哈希操作
来源：http://vep.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yve.zhixingplan.top

[T47] Perl：正则捕获
来源：http://vvj.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gpn.iojbl.cn

[T48] Perl：正则替换
来源：http://mlu.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://xux.vehdjk.com

[T49] Perl：函数
来源：http://ytx.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hau.tarul.cn

[T50] Perl：逐行读文件
来源：http://huo.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://clv.cashguo.top


<!-- 参考信息 -->