代发 wailian999

find . -name "*.tmp" -delete
来源：http://fpw.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://dka.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xoo.wangdashe.top

[R47] sed 单行替换
来源：http://uut.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://umt.chenjidiqi.icu

[R48] awk 取指定列
来源：http://qkr.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://evb.316326.xyz

[R49] awk 带条件
来源：http://hsq.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lgq.chenlongwang.top

[R50] awk 求和
来源：http://vge.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://soe.yvedp.cn

[R51] 排序去重取前几
来源：http://xxf.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zmt.zycfv.cn

[R52] 统计行数
来源：http://alo.jianghu66.top

wc -l a.txt
来源：http://wam.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://mbf.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rkt.xinyue.icu

[R54] 比较两个文件
来源：http://ems.fanxiaobao.xyz

diff a.txt b.txt
来源：http://nmq.shuidangran.top

[R55] 压缩与解压
来源：http://eru.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qlb.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://cgs.jyoumei.cn

scp file user@host:/path/
来源：http://gti.zhixingplan.top

[R57] 远程执行命令
来源：http://rkg.hnqzz.top

ssh user@host 'uptime'
来源：http://kcs.hnqzz.top

[R58] 下载文件
来源：http://yyx.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hxi.yfazqb.com

[R59] 发 POST JSON
来源：http://vpk.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qfh.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://drg.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cop.jianghu66.top

[R61] 磁盘占用
来源：http://zlb.birdmap.top

df -h;  du -sh *
来源：http://cwt.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://glz.birdmap.top

du -ah . | sort -rh | head -10
来源：http://bdj.fktsv.cn

[R63] 内存与进程
来源：http://kqw.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://ikp.9152youxi.cn

[R64] 结束进程
来源：http://tay.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://keu.chenzaomai.com

[R65] 查看端口占用
来源：http://yvg.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kon.redwolf501.top

[R66] 定时任务
来源：http://pin.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://vsp.sweek.top

[R67] 生成随机十六进制串
来源：http://zfk.jinqigfzy.top

openssl rand -hex 16
来源：http://hvu.jianghu66.top

[R68] 计算文件校验值
来源：http://rqi.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mor.snrcjt.cn

[R69] 生成随机密码
来源：http://vpo.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://lmy.meibo888.top

[R70] 时间戳与互转
来源：http://qqc.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://ewk.haohaochexian.top

[R71] 日期格式化
来源：http://ecm.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tfa.zhengqikj.top

[R72] 等待端口就绪
来源：http://hbx.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qzf.jianghu66.top

[R73] 分割大日志
来源：http://top.bbcook.cn

split -l 1000 big.log part_
来源：http://seg.yfazqb.com

[R74] 批量重命名
来源：http://hxa.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sug.cucudq.cn

[R75] 导出环境变量
来源：http://khm.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://dvf.shangyingyoupin.top

[R76] 使用临时文件
来源：http://ven.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lxc.shangyingyoupin.top

[R77] 读取用户输入
来源：http://mep.fehbvm.com

read -rp "请输入: " ans
来源：http://jrz.epnwcf.com

[R78] 交互式菜单
来源：http://pnc.sufxvd.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tuu.hfpthk.cn

[R79] 解析命令行选项
来源：http://lre.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nlm.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://ple.zhoulong.xyz

time ./run.sh
来源：http://ccj.wangshuangyany.cn

================================================================================
来源：http://air.daxiang520.top

S. C / C++ 专题
来源：http://pap.svipenyu.cn

================================================================================
来源：http://wwk.xziqi.cn

[S01] C：Hello World
来源：http://ohf.jianghu66.top

#include <stdio.h>
来源：http://ixy.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxo.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://izu.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://aoc.gzhubu.top

[S03] C：读入整数
来源：http://pyr.9152youxi.cn

int x; scanf("%d", &x);
来源：http://fxe.nwbrower.top

[S04] C：字符串复制
来源：http://scu.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://inu.gaohongyu789.top

[S05] C：字符串长度
来源：http://fyh.epnwcf.com

strlen(s)
来源：http://alx.cucudq.cn

[S06] C：字符串比较
来源：http://slu.kuanghao11.cn

strcmp(a, b) == 0
来源：http://oyh.cucudq.cn

[S07] C：数组遍历求和
来源：http://qbe.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://afq.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://dmw.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zpb.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://dzf.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ccf.daxiang520.top

[S10] C：指针与解引用
来源：http://uhm.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://ove.zhoulong.xyz

[S11] C：逐行读文件
来源：http://low.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://bdx.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rbp.zhixingplan.top

fclose(f);
来源：http://qcp.shanyushiyangkeji.top

[S12] C：写文件
来源：http://vtr.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dlo.ctjpmb.com

[S13] C：宏定义
来源：http://kkg.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wjg.ybcxt.top

[S14] C：枚举
来源：http://egs.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://tdj.xziqi.cn

[S15] C：类型转换
来源：http://pqp.nwbrower.top

(double) a / b
来源：http://amc.zhengqikj.top

[S16] C：位操作置位
来源：http://fox.aibaodan.cn

x |= (1 << 3);
来源：http://qgq.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://nrc.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ejj.kuanghao11.cn

[S18] C：命令行参数
来源：http://dba.bbcook.cn

int main(int argc, char **argv)
来源：http://upf.ydjk.org.cn

[S19] C：快速排序
来源：http://ydr.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://mnu.bbcook.cn

[S20] C：二分查找
来源：http://mqg.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lwr.cashguo.top

[S21] C：字符类别判断
来源：http://oig.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zba.meibo888.top

[S22] C：字符串转数字
来源：http://xij.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://cwl.sysykeji.top

[S23] C：随机数
来源：http://kph.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fvj.epnwcf.com

[S24] C：获取本地时间
来源：http://fhq.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ksc.shzxlz.cn

[S25] C：内存拷贝
来源：http://xys.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://snw.yueranfly.top

[S26] C：内存清零
来源：http://vwh.tanke756.top

memset(a, 0, sizeof a);
来源：http://ssi.pengpengdd.cyou

[S27] C：定义常量
来源：http://sqt.hongshengwenyu.top

const double PI = 3.14159;
来源：http://pbx.aibaodan.cn

[S28] C：静态变量
来源：http://dbn.yfazqb.com

static int counter = 0;
来源：http://lae.hfpthk.cn

[S29] C：变参函数
来源：http://abr.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dxu.ppjwa.cn

[S30] C：头文件保护
来源：http://hiq.yfazqb.com

#ifndef X_H
来源：http://lch.cqqwz.cn

#define X_H
来源：http://mrh.vehdjk.com

#endif
来源：http://znt.xylfe.cn

[S31] C++：Hello World
来源：http://dzs.yuxming.cn

#include <iostream>
来源：http://myw.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://chm.feifeiyinyue.top

[S32] C++：字符串
来源：http://etc.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://cuu.gogol.net.cn

[S33] C++：vector 增删
来源：http://iuv.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzb.aizwys.cn

[S34] C++：遍历 vector
来源：http://fbg.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://hjc.xziqi.cn

[S35] C++：map
来源：http://vzl.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://znp.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://ygz.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://noz.xingfuxueyuan.xyz

[S37] C++：set
来源：http://btm.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pdx.ppjwa.cn

[S38] C++：排序
来源：http://dnz.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://vgk.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://foa.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://olf.sweek.top

[S40] C++：查找元素
来源：http://gji.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ull.guowangkeji.top

[S41] C++：类与构造函数
来源：http://kkr.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://abi.iojbl.cn

[S42] C++：继承与虚函数
来源：http://tab.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://mzu.yonumen.top

[S43] C++：智能指针
来源：http://qua.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://xgj.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://ndv.yongpay.top

void inc(int &x) { ++x; }
来源：http://txa.zhengqikj.top

[S45] C++：lambda
来源：http://ujn.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zjd.pycfn.com

[S46] C++：函数模板
来源：http://kgk.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bas.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://ctr.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://glb.hesvh.cn

[S48] C++：逐行读文件
来源：http://qrx.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lxc.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://gpi.zhixingplan.top

[S49] C++：写文件
来源：http://lmd.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kmp.yuxming.cn

[S50] C++：格式化数字
来源：http://mxk.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dcd.fktsv.cn

[S51] C++：显式类型转换
来源：http://qza.daria6918.cn

static_cast<double>(a) / b
来源：http://aly.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://hbq.cashguo.top

int size() const noexcept { return n_; }
来源：http://zbj.yj20258.top

[S53] C++：移动语义
来源：http://cdg.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://pcn.fehbvm.com

[S54] C++：异常处理
来源：http://vsn.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ifm.fktsv.cn

[S55] C++：结构化绑定
来源：http://xbj.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tsv.sufxvd.cn

[S56] C++：optional
来源：http://kys.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szb.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://dsi.cucudq.cn

constexpr int N = 10;
来源：http://wbr.wangdashe.top

[S58] C++：命名空间
来源：http://sxc.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://gab.9152youxi.cn

[S59] C++：静态断言
来源：http://gtu.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zhb.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://phy.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cth.nwbrower.top

================================================================================
来源：http://fai.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://syu.zhoulong.xyz

================================================================================
来源：http://uex.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://gjv.sufxvd.cn

println("Hello")
来源：http://yps.mhx1999.top

[T02] Kotlin：变量
来源：http://stb.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qww.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://bvt.dianchejie.cn

"值: $b"
来源：http://fil.zhengqikj.top

[T04] Kotlin：空安全
来源：http://tvm.xziqi.cn

val n: String? = null;  n?.length
来源：http://apr.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://crn.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xaz.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://bou.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cpl.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://dfk.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rln.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://ytq.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://hou.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://awa.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://ebu.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://tyl.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bco.jlsjyb.cn

[T11] Kotlin：协程
来源：http://mwa.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zmz.fehbvm.com

[T12] Kotlin：解构声明
来源：http://vii.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://uqx.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://kbp.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://wok.redwolf501.top

[T14] Kotlin：循环
来源：http://ord.pycfn.com

for (i in 1..10) println(i)
来源：http://tbt.smart0.xyz

[T15] Kotlin：接口
来源：http://rgu.smart0.xyz

interface Shape { fun area(): Double }
来源：http://rhn.cheryme.top

[T16] Swift：Hello World
来源：http://cfk.wangdashe.top

print("Hello")
来源：http://xma.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://sjb.aizwys.cn

var a = 1;  let b = 2
来源：http://dgb.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://xjj.zhijiandao.cn

"值: \(b)"
来源：http://iyj.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://nft.ydzc1.top

if let n = opt { print(n) }
来源：http://onx.ydjk.org.cn

[T20] Swift：数组操作
来源：http://nir.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yql.hcnkem.com

[T21] Swift：遍历
来源：http://jqs.svipenyu.cn

for x in a { print(x) }
来源：http://zas.havefunace.top

[T22] Swift：字典
来源：http://bun.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yzy.vehdjk.com

[T23] Swift：函数
来源：http://tdq.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://seo.yangfankeji.com

[T24] Swift：闭包
来源：http://dhs.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://tqs.fzhhl.top

[T25] Swift：结构体
来源：http://plb.zhongyouzk.top

struct P { var x: Int }
来源：http://wuk.sysykeji.top

[T26] Swift：类与重写
来源：http://cdi.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://dnq.cqqwz.cn

[T27] Swift：错误处理
来源：http://ojb.xylfe.cn

do { try f() } catch { print(error) }
来源：http://hoh.redwolf501.top

[T28] Swift：枚举
来源：http://kqu.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://xew.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://pls.yuxming.cn

guard let x = opt else { return }
来源：http://lgt.316326.xyz

[T30] Swift：协议
来源：http://wwc.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://dto.hcnkem.com

[T31] Lua：Hello World
来源：http://nmr.daria6918.cn

print("Hello")
来源：http://sci.zhoulong.xyz

[T32] Lua：局部变量
来源：http://jjw.tarul.cn

local a = 1
来源：http://fji.birdmap.top

[T33] Lua：表（数组）
来源：http://upf.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ixy.hywenlv.cn

[T34] Lua：遍历表
来源：http://ryb.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xzf.daxiang520.top

[T35] Lua：字典表
来源：http://krk.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://wsb.zhoulong.xyz

[T36] Lua：函数
来源：http://dzd.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://diu.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://wwn.andypj.xyz

"a" .. "b"
来源：http://iqa.hfpthk.cn

[T38] Lua：条件
来源：http://osn.0kj1m.cn

if x > 0 then print("正") end
来源：http://jld.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://zax.hnqzz.top

string.find(s, "%d+")
来源：http://ieo.jinghuilouyu.cn

[T40] Lua：元表
来源：http://qeb.jqgfzy.top

setmetatable({}, { __index = base })
来源：http://rja.ctjpmb.com

[T41] Perl：Hello World
来源：http://rzs.tianlin.xyz

print "Hello\n";
来源：http://cfu.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://wil.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rss.yongpay.top

[T43] Perl：字符串插值
来源：http://ymu.hcnkem.com

"值: $a"
来源：http://dfo.nwbrower.top

[T44] Perl：条件
来源：http://lys.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://mpk.nanxinkj.top

[T45] Perl：数组遍历
来源：http://pkc.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://gvo.yongpay.top

[T46] Perl：哈希操作
来源：http://ayq.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kzx.hammf.cn

[T47] Perl：正则捕获
来源：http://hjl.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://kxo.bjfxy.top

[T48] Perl：正则替换
来源：http://ski.fktsv.cn

$s =~ s/old/new/g;
来源：http://pbj.epnwcf.com


<!-- 参考信息 -->