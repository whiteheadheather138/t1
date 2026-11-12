代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://qht.guowangkeji.top

[R48] awk 取指定列
来源：http://epn.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://paw.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://ekk.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uth.ppjwa.cn

[R50] awk 求和
来源：http://wlg.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mft.snrcjt.cn

[R51] 排序去重取前几
来源：http://nra.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uui.guannengcc.top

[R52] 统计行数
来源：http://yvx.bjfxy.top

wc -l a.txt
来源：http://luc.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://tpp.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gqp.zhixingplan.top

[R54] 比较两个文件
来源：http://hhs.xylfe.cn

diff a.txt b.txt
来源：http://hoj.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://jpl.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qib.epnwcf.com

[R56] 远程拷贝
来源：http://jxs.sufxvd.cn

scp file user@host:/path/
来源：http://hfg.jianghu66.top

[R57] 远程执行命令
来源：http://ypi.316326.xyz

ssh user@host 'uptime'
来源：http://gfm.ctjpmb.com

[R58] 下载文件
来源：http://qjg.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://faq.guowangkeji.top

[R59] 发 POST JSON
来源：http://cpt.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hsg.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://ecl.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wpm.fengsongda.top

[R61] 磁盘占用
来源：http://riu.zhoulong.xyz

df -h;  du -sh *
来源：http://het.hammf.cn

[R62] 找最占空间的文件
来源：http://zdf.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://lwj.zdbjq.cn

[R63] 内存与进程
来源：http://gol.uphjek.com

free -h;  ps aux | grep nginx
来源：http://ngu.pycfn.com

[R64] 结束进程
来源：http://abl.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://ttu.jianghu66.top

[R65] 查看端口占用
来源：http://jtv.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlo.andypj.xyz

[R66] 定时任务
来源：http://mdw.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://nlc.xuanzx.com

[R67] 生成随机十六进制串
来源：http://vos.wangshuangyany.cn

openssl rand -hex 16
来源：http://wam.redwolf501.top

[R68] 计算文件校验值
来源：http://ldj.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eav.fehbvm.com

[R69] 生成随机密码
来源：http://kdj.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://hgd.birdmap.top

[R70] 时间戳与互转
来源：http://fqv.tian-w.cn

date +%s;  date -d @1700000000
来源：http://qzx.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://sjk.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://sol.cashguo.top

[R72] 等待端口就绪
来源：http://lvr.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jyx.ivvv.top

[R73] 分割大日志
来源：http://bqr.ivvv.top

split -l 1000 big.log part_
来源：http://kqi.guannengcc.top

[R74] 批量重命名
来源：http://rni.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bgf.cdnleiting.top

[R75] 导出环境变量
来源：http://kum.hesvh.cn

export PATH="$HOME/bin:$PATH"
来源：http://ngr.tarul.cn

[R76] 使用临时文件
来源：http://hsk.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ycn.hnqzz.top

[R77] 读取用户输入
来源：http://ahv.aizwys.cn

read -rp "请输入: " ans
来源：http://zio.ybcxt.top

[R78] 交互式菜单
来源：http://oqq.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://dcl.cucudq.cn

[R79] 解析命令行选项
来源：http://jsj.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hze.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://pns.316326.xyz

time ./run.sh
来源：http://pjo.zhengqikj.top

================================================================================
来源：http://ykh.hesvh.cn

S. C / C++ 专题
来源：http://jsz.jqgufenzy.top

================================================================================
来源：http://jls.nanxinkj.top

[S01] C：Hello World
来源：http://bod.chenjidiqi.icu

#include <stdio.h>
来源：http://sml.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kaj.yonumen.top

[S02] C：变量与格式化输出
来源：http://jzh.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://uww.snrcjt.cn

[S03] C：读入整数
来源：http://snl.chenlongwang.top

int x; scanf("%d", &x);
来源：http://xal.yfazqb.com

[S04] C：字符串复制
来源：http://fju.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://snx.zhoulong.xyz

[S05] C：字符串长度
来源：http://byx.kuanghao11.cn

strlen(s)
来源：http://qwr.ctjpmb.com

[S06] C：字符串比较
来源：http://waj.tian-w.cn

strcmp(a, b) == 0
来源：http://bah.gogol.net.cn

[S07] C：数组遍历求和
来源：http://myv.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wdn.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://tjq.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://esz.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://vco.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mzf.yj202588.top

[S10] C：指针与解引用
来源：http://fwg.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://fsk.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://suu.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://zxk.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eqh.redwolf501.top

fclose(f);
来源：http://hef.dashuyun.cn

[S12] C：写文件
来源：http://jog.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfp.pengpengdd.cyou

[S13] C：宏定义
来源：http://oph.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vic.shzxlz.cn

[S14] C：枚举
来源：http://mjr.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://ccr.9152youxi.cn

[S15] C：类型转换
来源：http://wqb.zhixingplan.top

(double) a / b
来源：http://esc.yangfankeji.com

[S16] C：位操作置位
来源：http://nnv.ctjpmb.com

x |= (1 << 3);
来源：http://dpv.tian-w.cn

[S17] C：安全拼接字符串
来源：http://cou.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ysk.sxryk.cn

[S18] C：命令行参数
来源：http://lim.vqdsnc.cn

int main(int argc, char **argv)
来源：http://kmp.bbcook.cn

[S19] C：快速排序
来源：http://ele.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rcs.aizwys.cn

[S20] C：二分查找
来源：http://ogv.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gsf.zdqjudy.top

[S21] C：字符类别判断
来源：http://wfx.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nur.jianghu66.top

[S22] C：字符串转数字
来源：http://czk.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://alm.snrcjt.cn

[S23] C：随机数
来源：http://omr.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rhu.xuanzx.com

[S24] C：获取本地时间
来源：http://rfs.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://txk.yj20258888.top

[S25] C：内存拷贝
来源：http://zeg.cashguo.top

memcpy(dst, src, n);
来源：http://uum.ctjpmb.com

[S26] C：内存清零
来源：http://sym.xylfe.cn

memset(a, 0, sizeof a);
来源：http://fzw.hcnkem.com

[S27] C：定义常量
来源：http://jda.quarkkingdee.top

const double PI = 3.14159;
来源：http://zlv.cheryme.top

[S28] C：静态变量
来源：http://jal.tian-w.cn

static int counter = 0;
来源：http://oar.feifeiyinyue.top

[S29] C：变参函数
来源：http://qda.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lhk.cashguo.top

[S30] C：头文件保护
来源：http://xqt.fengsongda.top

#ifndef X_H
来源：http://iok.cheryme.top

#define X_H
来源：http://lul.yongpay.top

#endif
来源：http://rng.hongshengwenyu.top

[S31] C++：Hello World
来源：http://qdz.bjfxy.top

#include <iostream>
来源：http://ffx.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://cex.ybcxt.top

[S32] C++：字符串
来源：http://cqt.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://jck.fehbvm.com

[S33] C++：vector 增删
来源：http://qkm.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uem.sweek.top

[S34] C++：遍历 vector
来源：http://nqv.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://ynx.shzxlz.cn

[S35] C++：map
来源：http://aen.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qqi.xylfe.cn

[S36] C++：unordered_map
来源：http://oqg.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tsu.fzhhl.top

[S37] C++：set
来源：http://vqw.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gps.tianlin.xyz

[S38] C++：排序
来源：http://vod.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://uzv.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://heh.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://guy.chenzaomai.com

[S40] C++：查找元素
来源：http://ubc.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ddq.xuanzx.com

[S41] C++：类与构造函数
来源：http://xnr.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxb.vehdjk.com

[S42] C++：继承与虚函数
来源：http://iwj.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://inp.jlsjyb.cn

[S43] C++：智能指针
来源：http://oce.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://bsy.cucudq.cn

[S44] C++：引用传参
来源：http://obw.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://rdz.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://jhs.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hgl.hongshengwenyu.top

[S46] C++：函数模板
来源：http://yjs.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://avc.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://yut.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://puz.hfpthk.cn

[S48] C++：逐行读文件
来源：http://rhj.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://sgi.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://lwz.jinqigufen.top

[S49] C++：写文件
来源：http://tzt.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eaa.sysykeji.top

[S50] C++：格式化数字
来源：http://bhe.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jyi.zdqjudy.top

[S51] C++：显式类型转换
来源：http://prm.xylfe.cn

static_cast<double>(a) / b
来源：http://kpz.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://jxj.redwolf501.top

int size() const noexcept { return n_; }
来源：http://lke.kuanghao11.cn

[S53] C++：移动语义
来源：http://xog.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://smg.jqgufenzy.top

[S54] C++：异常处理
来源：http://mmo.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baf.yongpay.top

[S55] C++：结构化绑定
来源：http://sko.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://toz.guannengcc.top

[S56] C++：optional
来源：http://vjf.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rtk.jianghu66.top

[S57] C++：编译期常量
来源：http://lpy.sjlbkw.cn

constexpr int N = 10;
来源：http://mhl.zycfv.cn

[S58] C++：命名空间
来源：http://ynh.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://mmu.smart0.xyz

[S59] C++：静态断言
来源：http://vrh.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ksx.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://qof.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wtd.c1oappe.top

================================================================================
来源：http://vtr.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bcs.ctjpmb.com

================================================================================
来源：http://wze.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://qer.zhengqikj.top

println("Hello")
来源：http://dhs.ppjwa.cn

[T02] Kotlin：变量
来源：http://xva.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ibq.cashguo.top

[T03] Kotlin：字符串模板
来源：http://uie.hnxiangtu.top

"值: $b"
来源：http://clw.jiagoushi.top

[T04] Kotlin：空安全
来源：http://wmh.uphjek.com

val n: String? = null;  n?.length
来源：http://kum.meibo888.top

[T05] Kotlin：when 表达式
来源：http://phm.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cyb.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://apv.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bkt.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://wox.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qgm.gogol.net.cn

[T08] Kotlin：数据类
来源：http://wbj.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://bhs.pycfn.com

[T09] Kotlin：扩展函数
来源：http://sha.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://awv.meibo888.top

[T10] Kotlin：默认参数
来源：http://odd.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ajn.guowangkeji.top

[T11] Kotlin：协程
来源：http://suv.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xtj.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://csl.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://gcy.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://jxd.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://fbo.guannengcc.top

[T14] Kotlin：循环
来源：http://msj.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://sat.quarkkingdee.top

[T15] Kotlin：接口
来源：http://fjj.yongpay.top

interface Shape { fun area(): Double }
来源：http://vzx.wangdashe.top

[T16] Swift：Hello World
来源：http://wti.hcnkem.com

print("Hello")
来源：http://brv.tarul.cn

[T17] Swift：变量与常量
来源：http://spi.yuxming.cn

var a = 1;  let b = 2
来源：http://blo.svipenyu.cn

[T18] Swift：字符串插值
来源：http://rmp.hnxiangtu.top

"值: \(b)"
来源：http://yej.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://fxk.ybcxt.top

if let n = opt { print(n) }
来源：http://uuh.birdmap.top

[T20] Swift：数组操作
来源：http://xiw.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://gzj.svipenyu.cn

[T21] Swift：遍历
来源：http://qat.zhiwuduotai.top

for x in a { print(x) }
来源：http://ljl.bjfxy.top

[T22] Swift：字典
来源：http://nww.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://sas.bbcook.cn

[T23] Swift：函数
来源：http://qwe.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xlz.daria6918.cn

[T24] Swift：闭包
来源：http://moa.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eia.zycfv.cn

[T25] Swift：结构体
来源：http://lpy.hfpthk.cn

struct P { var x: Int }
来源：http://uzf.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://lzy.tarul.cn

class A: Base { override func f() {} }
来源：http://ttj.yuanzhike.top

[T27] Swift：错误处理
来源：http://nqb.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://roi.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://wtz.nanxuanxn.top

enum Color { case red, green }
来源：http://pha.meibo888.top

[T29] Swift：guard 提前返回
来源：http://gyz.chenlongwang.top

guard let x = opt else { return }
来源：http://htb.cucudq.cn

[T30] Swift：协议
来源：http://ios.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://esr.yvedp.cn

[T31] Lua：Hello World
来源：http://dsb.hywenlv.cn

print("Hello")
来源：http://dlq.mhx1999.top

[T32] Lua：局部变量
来源：http://rkn.xziqi.cn

local a = 1
来源：http://ijo.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://ump.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xra.zdbjq.cn

[T34] Lua：遍历表
来源：http://bvn.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://uee.guowangkeji.top

[T35] Lua：字典表
来源：http://pwa.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://qrv.wangshuangyany.cn

[T36] Lua：函数
来源：http://kjd.ctjpmb.com

function add(a, b) return a + b end
来源：http://fte.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://sbd.zhoulong.xyz

"a" .. "b"
来源：http://cqh.smart0.xyz

[T38] Lua：条件
来源：http://nru.haohaochexian.top

if x > 0 then print("正") end
来源：http://lhu.aizwys.cn

[T39] Lua：模式匹配
来源：http://axr.epnwcf.com

string.find(s, "%d+")
来源：http://cjl.jinghuilouyu.cn

[T40] Lua：元表
来源：http://bgt.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://vfj.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://brk.yueranfly.top

print "Hello\n";
来源：http://xjx.fktsv.cn

[T42] Perl：变量类型
来源：http://ywk.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lyz.yfazqb.com

[T43] Perl：字符串插值
来源：http://xcz.yj202588.top

"值: $a"
来源：http://wkl.ydzc1.top

[T44] Perl：条件
来源：http://auu.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://dho.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://fsb.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://ukx.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://dha.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cfk.yj202588.top

[T47] Perl：正则捕获
来源：http://cxm.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://anm.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://wnf.daria6918.cn

$s =~ s/old/new/g;
来源：http://xdh.zhongyouzk.top

[T49] Perl：函数
来源：http://fdq.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lyo.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://czy.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tnw.sufxvd.cn


<!-- 参考信息 -->