代发 wailian999

find . -name "*.tmp" -delete
来源：http://wng.jiagoushi.top

[R46] 递归替换文件内容
来源：http://pjz.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gqj.yvedp.cn

[R47] sed 单行替换
来源：http://oif.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://qut.yanxiufei.cn

[R48] awk 取指定列
来源：http://inc.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://iyk.yongpay.top

[R49] awk 带条件
来源：http://uef.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fev.yuxming.cn

[R50] awk 求和
来源：http://duv.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fgc.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://fly.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hxq.redwolf501.top

[R52] 统计行数
来源：http://eno.zhengqikj.top

wc -l a.txt
来源：http://qzl.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://nwz.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xis.yanxiufei.cn

[R54] 比较两个文件
来源：http://kax.fengsongda.top

diff a.txt b.txt
来源：http://ken.bbcook.cn

[R55] 压缩与解压
来源：http://tep.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plo.xuetiantiany.cn

[R56] 远程拷贝
来源：http://quy.ppjwa.cn

scp file user@host:/path/
来源：http://lrg.hongshengwenyu.top

[R57] 远程执行命令
来源：http://zzx.0kj1m.cn

ssh user@host 'uptime'
来源：http://ioa.hysaishi.cn

[R58] 下载文件
来源：http://ivv.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yze.vehdjk.com

[R59] 发 POST JSON
来源：http://ixr.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://otn.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://yql.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xre.svipenyu.cn

[R61] 磁盘占用
来源：http://twr.zhijiandao.cn

df -h;  du -sh *
来源：http://vqf.hywenlv.cn

[R62] 找最占空间的文件
来源：http://tmp.316326.xyz

du -ah . | sort -rh | head -10
来源：http://scw.zhijiandao.cn

[R63] 内存与进程
来源：http://dkl.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://wdc.hnqzz.top

[R64] 结束进程
来源：http://tmh.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://hoy.chenjidiqi.icu

[R65] 查看端口占用
来源：http://ubn.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfx.nanxinkj.top

[R66] 定时任务
来源：http://ssl.cdnleiting.top

crontab -e;  crontab -l
来源：http://upl.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://qxd.hesvh.cn

openssl rand -hex 16
来源：http://mix.vehdjk.com

[R68] 计算文件校验值
来源：http://cho.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://ptt.tarul.cn

[R69] 生成随机密码
来源：http://brh.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://jid.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://ixm.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://kcd.sxryk.cn

[R71] 日期格式化
来源：http://vxg.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uuy.zycfv.cn

[R72] 等待端口就绪
来源：http://ehf.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kjt.tianlin.xyz

[R73] 分割大日志
来源：http://jvs.jlsjyb.cn

split -l 1000 big.log part_
来源：http://txf.havefunace.top

[R74] 批量重命名
来源：http://pku.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://emy.daria6918.cn

[R75] 导出环境变量
来源：http://yxh.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://fub.andypj.xyz

[R76] 使用临时文件
来源：http://rln.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dpb.wangdashe.top

[R77] 读取用户输入
来源：http://orr.cheryme.top

read -rp "请输入: " ans
来源：http://gpu.wangshuangyany.cn

[R78] 交互式菜单
来源：http://bvj.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bow.yangfankeji.com

[R79] 解析命令行选项
来源：http://vvz.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zxh.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://vgc.zhengqikj.top

time ./run.sh
来源：http://mpw.birdmap.top

================================================================================
来源：http://pbk.cashguo.top

S. C / C++ 专题
来源：http://wam.ydzc1.top

================================================================================
来源：http://qye.kuanghao11.cn

[S01] C：Hello World
来源：http://qcs.aibaodan.cn

#include <stdio.h>
来源：http://wid.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qoh.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://xcr.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://xzm.gogol.net.cn

[S03] C：读入整数
来源：http://egx.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://zba.zhoulong.xyz

[S04] C：字符串复制
来源：http://hiq.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://amg.vqdsnc.cn

[S05] C：字符串长度
来源：http://lzd.chenlongwang.top

strlen(s)
来源：http://yol.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://ayn.ehwqpu.com

strcmp(a, b) == 0
来源：http://yoh.cqqwz.cn

[S07] C：数组遍历求和
来源：http://cth.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uzv.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://rld.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ztr.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://kzm.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yev.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://bxe.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://xhi.daria6918.cn

[S11] C：逐行读文件
来源：http://kxy.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://wgm.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngb.zhaomingkeji.xyz

fclose(f);
来源：http://qvy.epnwcf.com

[S12] C：写文件
来源：http://zdc.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fxj.aizwys.cn

[S13] C：宏定义
来源：http://lxx.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tzz.vqdsnc.cn

[S14] C：枚举
来源：http://lbz.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://sae.bjfxy.top

[S15] C：类型转换
来源：http://uex.vehdjk.com

(double) a / b
来源：http://pst.yvedp.cn

[S16] C：位操作置位
来源：http://vik.hongshengwenyu.top

x |= (1 << 3);
来源：http://qie.nwbrower.top

[S17] C：安全拼接字符串
来源：http://pyt.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnn.andypj.xyz

[S18] C：命令行参数
来源：http://qrt.quarkkingdee.top

int main(int argc, char **argv)
来源：http://clm.zhoulong.xyz

[S19] C：快速排序
来源：http://gxs.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://elr.zhiwuduotai.top

[S20] C：二分查找
来源：http://udi.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://poo.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://lvh.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://toy.gaohongyu789.top

[S22] C：字符串转数字
来源：http://dgj.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qdk.yangfankeji.com

[S23] C：随机数
来源：http://alu.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qis.uphjek.com

[S24] C：获取本地时间
来源：http://myo.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dhe.snrcjt.cn

[S25] C：内存拷贝
来源：http://sla.ehwqpu.com

memcpy(dst, src, n);
来源：http://lfc.tian-w.cn

[S26] C：内存清零
来源：http://usv.sysykeji.top

memset(a, 0, sizeof a);
来源：http://zrv.jiagoushi.top

[S27] C：定义常量
来源：http://gva.jqgufenzy.top

const double PI = 3.14159;
来源：http://qyy.fzhhl.top

[S28] C：静态变量
来源：http://vbw.yonumen.top

static int counter = 0;
来源：http://pli.shuidangran.top

[S29] C：变参函数
来源：http://wjd.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ltl.xziqi.cn

[S30] C：头文件保护
来源：http://ezp.zycfv.cn

#ifndef X_H
来源：http://acx.yj20258.top

#define X_H
来源：http://jvf.dashuyun.cn

#endif
来源：http://yhk.jianghu66.top

[S31] C++：Hello World
来源：http://hld.zycfv.cn

#include <iostream>
来源：http://rwb.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://wnt.hammf.cn

[S32] C++：字符串
来源：http://mqw.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://irj.zhixingplan.top

[S33] C++：vector 增删
来源：http://cmd.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://git.tianlin.xyz

[S34] C++：遍历 vector
来源：http://uuz.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://czf.nwbrower.top

[S35] C++：map
来源：http://pdi.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wii.316326.xyz

[S36] C++：unordered_map
来源：http://mpc.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://has.ivvv.top

[S37] C++：set
来源：http://ylb.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dsp.ivvv.top

[S38] C++：排序
来源：http://xqn.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://cbv.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://hfr.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vfd.nwbrower.top

[S40] C++：查找元素
来源：http://fgc.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://btf.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://kyc.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iyd.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://yez.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://cvu.svipenyu.cn

[S43] C++：智能指针
来源：http://tnf.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://tys.mhx1999.top

[S44] C++：引用传参
来源：http://bve.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://qif.shzxlz.cn

[S45] C++：lambda
来源：http://zjl.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gaq.zhiwuduotai.top

[S46] C++：函数模板
来源：http://bkm.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nqn.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://rrs.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://igw.aizwys.cn

[S48] C++：逐行读文件
来源：http://nsa.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://pxo.yfazqb.com

while (std::getline(in, line)) { }
来源：http://gbn.xylfe.cn

[S49] C++：写文件
来源：http://dcq.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mur.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://ewh.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jci.hammf.cn

[S51] C++：显式类型转换
来源：http://oau.ybcxt.top

static_cast<double>(a) / b
来源：http://bhr.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://aye.hesvh.cn

int size() const noexcept { return n_; }
来源：http://zqx.gzhubu.top

[S53] C++：移动语义
来源：http://tnp.yj20258.top

std::vector<int> w = std::move(v);
来源：http://pqv.pycfn.com

[S54] C++：异常处理
来源：http://cpq.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zpi.ydzc1.top

[S55] C++：结构化绑定
来源：http://szz.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gsy.hywenlv.cn

[S56] C++：optional
来源：http://gxx.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dbf.yvedp.cn

[S57] C++：编译期常量
来源：http://mhz.bjfxy.top

constexpr int N = 10;
来源：http://zpq.gzhubu.top

[S58] C++：命名空间
来源：http://xre.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://qrz.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://ech.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kri.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://cil.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dex.c1oappe.top

================================================================================
来源：http://kea.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eyd.yj20258888.top

================================================================================
来源：http://bkw.tian-w.cn

[T01] Kotlin：Hello World
来源：http://kth.sufxvd.cn

println("Hello")
来源：http://rsr.sxryk.cn

[T02] Kotlin：变量
来源：http://nmt.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jsk.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://fha.gotoacloud.top

"值: $b"
来源：http://kpy.hysaishi.cn

[T04] Kotlin：空安全
来源：http://dzm.yuanzhike.top

val n: String? = null;  n?.length
来源：http://mro.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://tgb.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kqp.yongpay.top

[T06] Kotlin：集合映射
来源：http://aal.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://skm.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://izo.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ans.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://dlg.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://epg.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://ijd.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://ssh.havefunace.top

[T10] Kotlin：默认参数
来源：http://dpk.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rpr.tanke756.top

[T11] Kotlin：协程
来源：http://jlu.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://kmq.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://leq.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://noe.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://glh.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://exa.svipenyu.cn

[T14] Kotlin：循环
来源：http://rtp.sufxvd.cn

for (i in 1..10) println(i)
来源：http://jhq.svipenyu.cn

[T15] Kotlin：接口
来源：http://iyw.cheryme.top

interface Shape { fun area(): Double }
来源：http://pfy.ydzc1.top

[T16] Swift：Hello World
来源：http://pla.nanxuanxn.top

print("Hello")
来源：http://iaw.zdqjudy.top

[T17] Swift：变量与常量
来源：http://ygy.redwolf501.top

var a = 1;  let b = 2
来源：http://rps.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://gir.zhiwuduotai.top

"值: \(b)"
来源：http://vxj.guowangkeji.top

[T19] Swift：可选绑定
来源：http://jcv.tanke756.top

if let n = opt { print(n) }
来源：http://wtk.sysykeji.top

[T20] Swift：数组操作
来源：http://ikh.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://liy.hammf.cn

[T21] Swift：遍历
来源：http://war.daria6918.cn

for x in a { print(x) }
来源：http://buo.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://dad.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://riv.jinqigfzy.top

[T23] Swift：函数
来源：http://esr.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kft.cheryme.top

[T24] Swift：闭包
来源：http://wmr.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jzl.yvedp.cn

[T25] Swift：结构体
来源：http://zyz.yj20258888.top

struct P { var x: Int }
来源：http://mxn.sufxvd.cn

[T26] Swift：类与重写
来源：http://uii.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://jgj.daria6918.cn

[T27] Swift：错误处理
来源：http://lwa.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://xfd.aizwys.cn

[T28] Swift：枚举
来源：http://tbx.pengpengdd.cyou

enum Color { case red, green }
来源：http://awf.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://btq.havefunace.top

guard let x = opt else { return }
来源：http://oab.52xcode.cn

[T30] Swift：协议
来源：http://gft.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://thn.vqdsnc.cn

[T31] Lua：Hello World
来源：http://dqv.xuetiantiany.cn

print("Hello")
来源：http://knv.zhengqikj.top

[T32] Lua：局部变量
来源：http://fyr.bjfxy.top

local a = 1
来源：http://kmq.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://pmh.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tbn.jqgfzy.top

[T34] Lua：遍历表
来源：http://ptw.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kux.fktsv.cn

[T35] Lua：字典表
来源：http://tzh.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://obm.nwbrower.top

[T36] Lua：函数
来源：http://mvi.ctjpmb.com

function add(a, b) return a + b end
来源：http://uhs.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://xre.redwolf501.top

"a" .. "b"
来源：http://nes.sjlbkw.cn

[T38] Lua：条件
来源：http://lqb.fehbvm.com

if x > 0 then print("正") end
来源：http://wfa.havefunace.top

[T39] Lua：模式匹配
来源：http://ejw.sxryk.cn

string.find(s, "%d+")
来源：http://dgg.xuetiantiany.cn

[T40] Lua：元表
来源：http://uqi.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://hrc.chenlongwang.top

[T41] Perl：Hello World
来源：http://kid.dashuyun.cn

print "Hello\n";
来源：http://sot.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://jzx.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ggf.nanxinkj.top

[T43] Perl：字符串插值
来源：http://vsj.gaohongyu789.top

"值: $a"
来源：http://gfw.316326.xyz

[T44] Perl：条件
来源：http://unt.uphjek.com

if ($a > 0) { print "正"; }
来源：http://axq.hnqzz.top

[T45] Perl：数组遍历
来源：http://qpj.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://efq.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://msd.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://joi.cucudq.cn

[T47] Perl：正则捕获
来源：http://vjv.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oku.cheryme.top

[T48] Perl：正则替换
来源：http://jcz.guowangkeji.top

$s =~ s/old/new/g;
来源：http://oli.zhixingplan.top


<!-- 参考信息 -->