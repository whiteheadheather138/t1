代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://gnx.guannengcc.top

[R48] awk 取指定列
来源：http://idg.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://olj.bbcook.cn

[R49] awk 带条件
来源：http://eih.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wdw.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://anh.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dnd.cheryme.top

[R51] 排序去重取前几
来源：http://xpd.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://noq.vqdsnc.cn

[R52] 统计行数
来源：http://zmq.cashguo.top

wc -l a.txt
来源：http://xkk.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://qqe.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kag.fengsongda.top

[R54] 比较两个文件
来源：http://hmz.yj20258.top

diff a.txt b.txt
来源：http://nmb.chenzaomai.com

[R55] 压缩与解压
来源：http://sus.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yzf.yanxiufei.cn

[R56] 远程拷贝
来源：http://xiw.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://ste.316326.xyz

[R57] 远程执行命令
来源：http://vch.c1oappe.top

ssh user@host 'uptime'
来源：http://rzf.xziqi.cn

[R58] 下载文件
来源：http://vbs.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://whk.fengsongda.top

[R59] 发 POST JSON
来源：http://bnh.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yxf.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://kwl.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vdn.aibaodan.cn

[R61] 磁盘占用
来源：http://dmb.hcnkem.com

df -h;  du -sh *
来源：http://noz.xuanzx.com

[R62] 找最占空间的文件
来源：http://lwo.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://nvm.chenjidiqi.icu

[R63] 内存与进程
来源：http://tbp.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://wto.ywan-chungtsiang.top

[R64] 结束进程
来源：http://bsi.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://gnd.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://ggv.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://efz.jqgufenzy.top

[R66] 定时任务
来源：http://bbt.sxryk.cn

crontab -e;  crontab -l
来源：http://vkm.ydzc1.top

[R67] 生成随机十六进制串
来源：http://mts.wangshuangyany.cn

openssl rand -hex 16
来源：http://uws.sjlbkw.cn

[R68] 计算文件校验值
来源：http://ics.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vjb.sxryk.cn

[R69] 生成随机密码
来源：http://plq.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://zdc.zhoulong.xyz

[R70] 时间戳与互转
来源：http://ijv.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://yid.jyoumei.cn

[R71] 日期格式化
来源：http://pgg.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://nns.jqgfzy.top

[R72] 等待端口就绪
来源：http://bsv.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vws.0kj1m.cn

[R73] 分割大日志
来源：http://hbf.ydjk.org.cn

split -l 1000 big.log part_
来源：http://qje.chenjidiqi.icu

[R74] 批量重命名
来源：http://cbd.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://huc.ydzc1.top

[R75] 导出环境变量
来源：http://liv.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pwa.bjfxy.top

[R76] 使用临时文件
来源：http://bjx.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://glk.dianchejie.cn

[R77] 读取用户输入
来源：http://nif.tanke756.top

read -rp "请输入: " ans
来源：http://zoh.svipenyu.cn

[R78] 交互式菜单
来源：http://qya.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dxy.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://ikr.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dbn.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://pba.hcnkem.com

time ./run.sh
来源：http://dcm.yj202588.top

================================================================================
来源：http://sfu.quarkkingdee.top

S. C / C++ 专题
来源：http://vyz.chenlongwang.top

================================================================================
来源：http://lcj.jyoumei.cn

[S01] C：Hello World
来源：http://bkb.guowangkeji.top

#include <stdio.h>
来源：http://ntb.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jqj.fktsv.cn

[S02] C：变量与格式化输出
来源：http://ilo.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://cif.cdnleiting.top

[S03] C：读入整数
来源：http://sfp.jinqigufen.top

int x; scanf("%d", &x);
来源：http://muk.kuanghao11.cn

[S04] C：字符串复制
来源：http://atw.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://zyh.feifeiyinyue.top

[S05] C：字符串长度
来源：http://cyf.epnwcf.com

strlen(s)
来源：http://alk.smart0.xyz

[S06] C：字符串比较
来源：http://ehp.daxiang520.top

strcmp(a, b) == 0
来源：http://uqk.gogol.net.cn

[S07] C：数组遍历求和
来源：http://arr.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ijk.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://gxs.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qmc.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://fde.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://njq.nanxinkj.top

[S10] C：指针与解引用
来源：http://rhz.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://npc.redwolf501.top

[S11] C：逐行读文件
来源：http://vwn.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://kac.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iki.sjlbkw.cn

fclose(f);
来源：http://smp.guowangkeji.top

[S12] C：写文件
来源：http://kdj.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ick.cqqwz.cn

[S13] C：宏定义
来源：http://msa.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jrt.jqgufenzy.top

[S14] C：枚举
来源：http://iqv.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://asj.gaohongyu789.top

[S15] C：类型转换
来源：http://hhh.xziqi.cn

(double) a / b
来源：http://qkw.sweek.top

[S16] C：位操作置位
来源：http://efx.gaohongyu789.top

x |= (1 << 3);
来源：http://urz.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://lnl.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://anb.jqgfzy.top

[S18] C：命令行参数
来源：http://zjo.pycfn.com

int main(int argc, char **argv)
来源：http://lhr.sxryk.cn

[S19] C：快速排序
来源：http://swc.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://pww.sjlbkw.cn

[S20] C：二分查找
来源：http://qeb.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hne.jinqigfzy.top

[S21] C：字符类别判断
来源：http://bzm.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfw.ydjk.org.cn

[S22] C：字符串转数字
来源：http://ieb.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://tex.zdqjudy.top

[S23] C：随机数
来源：http://zgq.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fnu.ybcxt.top

[S24] C：获取本地时间
来源：http://fig.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ble.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://yrs.tian-w.cn

memcpy(dst, src, n);
来源：http://wdl.aibaodan.cn

[S26] C：内存清零
来源：http://mhz.ydzc1.top

memset(a, 0, sizeof a);
来源：http://cyi.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://gly.xuetiantiany.cn

const double PI = 3.14159;
来源：http://jnt.zhongyouzk.top

[S28] C：静态变量
来源：http://pul.hnxiangtu.top

static int counter = 0;
来源：http://omj.quarkkingdee.top

[S29] C：变参函数
来源：http://opn.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qfw.nanxinkj.top

[S30] C：头文件保护
来源：http://fxl.chenlongwang.top

#ifndef X_H
来源：http://pxv.yuxming.cn

#define X_H
来源：http://tqr.shangyingyoupin.top

#endif
来源：http://add.ctjpmb.com

[S31] C++：Hello World
来源：http://frg.zhaomingkeji.xyz

#include <iostream>
来源：http://txw.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dfx.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://yhh.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://jpn.sxryk.cn

[S33] C++：vector 增删
来源：http://icu.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fqu.hesvh.cn

[S34] C++：遍历 vector
来源：http://kfd.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://ere.cashguo.top

[S35] C++：map
来源：http://fwt.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aqw.fktsv.cn

[S36] C++：unordered_map
来源：http://amk.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pfj.svipenyu.cn

[S37] C++：set
来源：http://mmb.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baa.ctjpmb.com

[S38] C++：排序
来源：http://jki.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://crc.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://iwo.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wno.gotoacloud.top

[S40] C++：查找元素
来源：http://rxf.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jcy.hesvh.cn

[S41] C++：类与构造函数
来源：http://ruo.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uyj.tarul.cn

[S42] C++：继承与虚函数
来源：http://vyc.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://caq.shangyingyoupin.top

[S43] C++：智能指针
来源：http://ila.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://rzh.jqgfzy.top

[S44] C++：引用传参
来源：http://ryq.yfazqb.com

void inc(int &x) { ++x; }
来源：http://kiu.hywenlv.cn

[S45] C++：lambda
来源：http://fdk.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://loc.pengpengdd.cyou

[S46] C++：函数模板
来源：http://xmv.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yye.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://tcj.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eix.fengsongda.top

[S48] C++：逐行读文件
来源：http://nhk.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://usz.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://cwf.hnxiangtu.top

[S49] C++：写文件
来源：http://njc.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bto.ybcxt.top

[S50] C++：格式化数字
来源：http://gle.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://erk.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://feu.chenzaomai.com

static_cast<double>(a) / b
来源：http://pvu.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://gyx.ydzc1.top

int size() const noexcept { return n_; }
来源：http://byg.hysaishi.cn

[S53] C++：移动语义
来源：http://neg.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://bvn.redwolf501.top

[S54] C++：异常处理
来源：http://def.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hkp.tianlin.xyz

[S55] C++：结构化绑定
来源：http://qvs.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kln.tarul.cn

[S56] C++：optional
来源：http://tas.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qsm.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://lhi.chenzaomai.com

constexpr int N = 10;
来源：http://lwc.smart0.xyz

[S58] C++：命名空间
来源：http://gso.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://qvn.cdnleiting.top

[S59] C++：静态断言
来源：http://egk.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://axf.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ewv.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zhi.ydzc1.top

================================================================================
来源：http://etn.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rrc.uphjek.com

================================================================================
来源：http://ptt.cucudq.cn

[T01] Kotlin：Hello World
来源：http://jgd.yangfankeji.com

println("Hello")
来源：http://bon.sxryk.cn

[T02] Kotlin：变量
来源：http://dos.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nxx.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://ooi.fehbvm.com

"值: $b"
来源：http://mdg.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://sof.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://fbz.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://dev.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vyd.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://tto.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ivy.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://fle.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qcs.tarul.cn

[T08] Kotlin：数据类
来源：http://xuw.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://uyy.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://grp.yongpay.top

fun String.exclaim() = this + "!"
来源：http://mti.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://geq.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dko.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://sbl.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvd.yfazqb.com

[T12] Kotlin：解构声明
来源：http://ebj.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://rxc.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://rde.fehbvm.com

val m = mapOf("a" to 1)
来源：http://dph.bbcook.cn

[T14] Kotlin：循环
来源：http://hhl.shzxlz.cn

for (i in 1..10) println(i)
来源：http://kyp.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://diz.sxryk.cn

interface Shape { fun area(): Double }
来源：http://daz.yuanzhike.top

[T16] Swift：Hello World
来源：http://dqz.jqgufenzy.top

print("Hello")
来源：http://evv.xziqi.cn

[T17] Swift：变量与常量
来源：http://ugu.hysaishi.cn

var a = 1;  let b = 2
来源：http://llf.ivvv.top

[T18] Swift：字符串插值
来源：http://oua.fehbvm.com

"值: \(b)"
来源：http://dqr.yj20258.top

[T19] Swift：可选绑定
来源：http://yev.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://xqg.ivvv.top

[T20] Swift：数组操作
来源：http://baa.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://hjx.hesvh.cn

[T21] Swift：遍历
来源：http://pix.pycfn.com

for x in a { print(x) }
来源：http://clc.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://ycc.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yez.shangyingyoupin.top

[T23] Swift：函数
来源：http://hva.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sye.fengsongda.top

[T24] Swift：闭包
来源：http://vgk.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xns.fehbvm.com

[T25] Swift：结构体
来源：http://lrj.hcnkem.com

struct P { var x: Int }
来源：http://jyr.tanke756.top

[T26] Swift：类与重写
来源：http://wpo.aizwys.cn

class A: Base { override func f() {} }
来源：http://sib.9152youxi.cn

[T27] Swift：错误处理
来源：http://okn.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://wro.tarul.cn

[T28] Swift：枚举
来源：http://dfp.hongshengwenyu.top

enum Color { case red, green }
来源：http://jbe.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://nfp.chenlongwang.top

guard let x = opt else { return }
来源：http://zky.pycfn.com

[T30] Swift：协议
来源：http://vlq.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://xhj.jinqigfzy.top

[T31] Lua：Hello World
来源：http://uct.redwolf501.top

print("Hello")
来源：http://fto.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://wpz.aizwys.cn

local a = 1
来源：http://avk.chenlongwang.top

[T33] Lua：表（数组）
来源：http://esa.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vfa.ehwqpu.com

[T34] Lua：遍历表
来源：http://jrm.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://utg.yfazqb.com

[T35] Lua：字典表
来源：http://sbr.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://bsy.vehdjk.com

[T36] Lua：函数
来源：http://ygm.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://qlz.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://gex.jinqigufen.top

"a" .. "b"
来源：http://yid.zhixingplan.top

[T38] Lua：条件
来源：http://fin.jlsjyb.cn

if x > 0 then print("正") end
来源：http://kro.guowangkeji.top

[T39] Lua：模式匹配
来源：http://stc.feifeiyinyue.top

string.find(s, "%d+")
来源：http://lbl.jinqigufen.top

[T40] Lua：元表
来源：http://pfe.ivvv.top

setmetatable({}, { __index = base })
来源：http://wwj.52xcode.cn

[T41] Perl：Hello World
来源：http://fyr.zhixingplan.top

print "Hello\n";
来源：http://jph.zycfv.cn

[T42] Perl：变量类型
来源：http://hgm.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ldl.gzhubu.top

[T43] Perl：字符串插值
来源：http://enn.guannengcc.top

"值: $a"
来源：http://xem.aibaodan.cn

[T44] Perl：条件
来源：http://sws.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://dja.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://epq.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://ofe.cucudq.cn

[T46] Perl：哈希操作
来源：http://snd.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uua.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://ldg.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gio.cheryme.top

[T48] Perl：正则替换
来源：http://sft.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://tui.vehdjk.com

[T49] Perl：函数
来源：http://dyn.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bsa.guannengcc.top

[T50] Perl：逐行读文件
来源：http://irs.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rub.ppjwa.cn


<!-- 参考信息 -->