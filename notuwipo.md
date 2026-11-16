代发 wailian999

find . -name "*.tmp" -delete
来源：http://tkw.0kj1m.cn

[R46] 递归替换文件内容
来源：http://bwh.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbk.cdnleiting.top

[R47] sed 单行替换
来源：http://olu.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://obj.aizwys.cn

[R48] awk 取指定列
来源：http://ejj.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://eel.nwbrower.top

[R49] awk 带条件
来源：http://rkg.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oot.cashguo.top

[R50] awk 求和
来源：http://egh.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zvj.birdmap.top

[R51] 排序去重取前几
来源：http://gmu.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vkg.jinqigfzy.top

[R52] 统计行数
来源：http://qee.sweek.top

wc -l a.txt
来源：http://hys.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://mol.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ibp.xylfe.cn

[R54] 比较两个文件
来源：http://dey.dianchejie.cn

diff a.txt b.txt
来源：http://clu.316326.xyz

[R55] 压缩与解压
来源：http://sbe.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yrj.andypj.xyz

[R56] 远程拷贝
来源：http://cwq.wangshuangyany.cn

scp file user@host:/path/
来源：http://gnr.0kj1m.cn

[R57] 远程执行命令
来源：http://mif.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://fyf.zhongyouzk.top

[R58] 下载文件
来源：http://egs.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://duq.zhengqikj.top

[R59] 发 POST JSON
来源：http://zmi.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ooh.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://htj.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://opy.xinyue.icu

[R61] 磁盘占用
来源：http://alk.sufxvd.cn

df -h;  du -sh *
来源：http://xpn.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://yzj.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://hjb.52xcode.cn

[R63] 内存与进程
来源：http://xya.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://mca.52xcode.cn

[R64] 结束进程
来源：http://yoj.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://qol.meibo888.top

[R65] 查看端口占用
来源：http://eql.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://frt.shuidangran.top

[R66] 定时任务
来源：http://axf.cqqwz.cn

crontab -e;  crontab -l
来源：http://bko.sysykeji.top

[R67] 生成随机十六进制串
来源：http://xsq.hysaishi.cn

openssl rand -hex 16
来源：http://vvn.sysykeji.top

[R68] 计算文件校验值
来源：http://vfc.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://glo.daria6918.cn

[R69] 生成随机密码
来源：http://fhg.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://wow.jqgufenzy.top

[R70] 时间戳与互转
来源：http://lzb.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://bie.zycfv.cn

[R71] 日期格式化
来源：http://lfh.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://djm.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://jcv.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xwf.svipenyu.cn

[R73] 分割大日志
来源：http://fpi.cucudq.cn

split -l 1000 big.log part_
来源：http://eod.jqgufenzy.top

[R74] 批量重命名
来源：http://bff.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vyy.daxiang520.top

[R75] 导出环境变量
来源：http://tox.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://mbo.tian-w.cn

[R76] 使用临时文件
来源：http://hab.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rkn.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://wpz.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://lkq.yonumen.top

[R78] 交互式菜单
来源：http://lzu.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://swh.dianchejie.cn

[R79] 解析命令行选项
来源：http://tpq.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ceu.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://wvs.yj202588.top

time ./run.sh
来源：http://eup.gaohongyu789.top

================================================================================
来源：http://odm.jinghuilouyu.cn

S. C / C++ 专题
来源：http://yoj.yonumen.top

================================================================================
来源：http://grn.vqdsnc.cn

[S01] C：Hello World
来源：http://cmn.yonumen.top

#include <stdio.h>
来源：http://raz.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wmc.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://vja.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://oay.xuetiantiany.cn

[S03] C：读入整数
来源：http://giy.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://cba.xylfe.cn

[S04] C：字符串复制
来源：http://tro.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://fqg.pengpengdd.cyou

[S05] C：字符串长度
来源：http://mus.xinyue.icu

strlen(s)
来源：http://yln.epnwcf.com

[S06] C：字符串比较
来源：http://jdi.tanke756.top

strcmp(a, b) == 0
来源：http://pki.yangfankeji.com

[S07] C：数组遍历求和
来源：http://gmz.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wbj.cashguo.top

[S08] C：动态内存分配与释放
来源：http://xxi.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kdq.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://kkp.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://knz.sjlbkw.cn

[S10] C：指针与解引用
来源：http://sux.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://gjp.wangdashe.top

[S11] C：逐行读文件
来源：http://isj.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://ozc.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eph.cashguo.top

fclose(f);
来源：http://zri.nwbrower.top

[S12] C：写文件
来源：http://qqa.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qkw.xuetiantiany.cn

[S13] C：宏定义
来源：http://kqo.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pfi.zhixingplan.top

[S14] C：枚举
来源：http://jfl.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://gqu.ydzc1.top

[S15] C：类型转换
来源：http://kbm.daria6918.cn

(double) a / b
来源：http://ajt.zhiwuduotai.top

[S16] C：位操作置位
来源：http://yuq.tian-w.cn

x |= (1 << 3);
来源：http://cgp.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://vws.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://obl.kuanghao11.cn

[S18] C：命令行参数
来源：http://oni.xziqi.cn

int main(int argc, char **argv)
来源：http://uwp.redwolf501.top

[S19] C：快速排序
来源：http://xel.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://hoi.guannengcc.top

[S20] C：二分查找
来源：http://uyw.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iav.yongpay.top

[S21] C：字符类别判断
来源：http://osv.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ecl.zhoulong.xyz

[S22] C：字符串转数字
来源：http://vds.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nqy.hesvh.cn

[S23] C：随机数
来源：http://vwq.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://goh.tianlin.xyz

[S24] C：获取本地时间
来源：http://yco.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tto.hnqzz.top

[S25] C：内存拷贝
来源：http://xvt.xylfe.cn

memcpy(dst, src, n);
来源：http://kdd.shanyushiyangtech.top

[S26] C：内存清零
来源：http://ywz.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://qud.yuanzhike.top

[S27] C：定义常量
来源：http://wrs.zhijiandao.cn

const double PI = 3.14159;
来源：http://iau.meibo888.top

[S28] C：静态变量
来源：http://kmz.redwolf501.top

static int counter = 0;
来源：http://teg.wangshuangyany.cn

[S29] C：变参函数
来源：http://qhi.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://leu.ydzc1.top

[S30] C：头文件保护
来源：http://mzd.zhoulong.xyz

#ifndef X_H
来源：http://glz.shzxlz.cn

#define X_H
来源：http://kjh.fengsongda.top

#endif
来源：http://jcn.shangyingyoupin.top

[S31] C++：Hello World
来源：http://hgj.hammf.cn

#include <iostream>
来源：http://cgj.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://pkq.hcnkem.com

[S32] C++：字符串
来源：http://uzp.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://wej.fzhhl.top

[S33] C++：vector 增删
来源：http://mba.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xap.nwbrower.top

[S34] C++：遍历 vector
来源：http://uen.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://tfa.hnxiangtu.top

[S35] C++：map
来源：http://vaq.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhg.kuanghao11.cn

[S36] C++：unordered_map
来源：http://yro.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lkl.shuidangran.top

[S37] C++：set
来源：http://myu.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lnb.xziqi.cn

[S38] C++：排序
来源：http://oaj.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://xcf.pycfn.com

[S39] C++：自定义比较器排序
来源：http://lzj.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://val.tarul.cn

[S40] C++：查找元素
来源：http://lyx.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ycx.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://wuc.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://can.c1oappe.top

[S42] C++：继承与虚函数
来源：http://ycr.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://xec.ydjk.org.cn

[S43] C++：智能指针
来源：http://sfy.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://jtd.andypj.xyz

[S44] C++：引用传参
来源：http://dtt.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://fti.yonumen.top

[S45] C++：lambda
来源：http://cjc.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hnc.uphjek.com

[S46] C++：函数模板
来源：http://amh.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://isa.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://mrw.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tnb.yuxming.cn

[S48] C++：逐行读文件
来源：http://flh.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vzf.mhx1999.top

while (std::getline(in, line)) { }
来源：http://act.cucudq.cn

[S49] C++：写文件
来源：http://ffj.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://egj.tianlin.xyz

[S50] C++：格式化数字
来源：http://ukk.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdj.fktsv.cn

[S51] C++：显式类型转换
来源：http://fkw.zhixingplan.top

static_cast<double>(a) / b
来源：http://ljx.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://jmi.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://odb.cqqwz.cn

[S53] C++：移动语义
来源：http://fef.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://len.hnxiangtu.top

[S54] C++：异常处理
来源：http://nuj.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yyt.ehwqpu.com

[S55] C++：结构化绑定
来源：http://erw.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fhe.tianlin.xyz

[S56] C++：optional
来源：http://yty.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qey.cdnleiting.top

[S57] C++：编译期常量
来源：http://zef.cucudq.cn

constexpr int N = 10;
来源：http://meb.vehdjk.com

[S58] C++：命名空间
来源：http://esc.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://ozv.nwbrower.top

[S59] C++：静态断言
来源：http://hzf.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uxt.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://zeg.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ijr.fktsv.cn

================================================================================
来源：http://lrz.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wam.fzhhl.top

================================================================================
来源：http://chw.yongpay.top

[T01] Kotlin：Hello World
来源：http://edj.xuetiantiany.cn

println("Hello")
来源：http://qfi.aizwys.cn

[T02] Kotlin：变量
来源：http://rpk.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hxw.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://rnz.bjfxy.top

"值: $b"
来源：http://lbp.chenzaomai.com

[T04] Kotlin：空安全
来源：http://wci.jinqigufen.top

val n: String? = null;  n?.length
来源：http://jfj.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://cjf.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://whx.yj20258888.top

[T06] Kotlin：集合映射
来源：http://ggq.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lpx.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://ylr.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nrz.ydzc1.top

[T08] Kotlin：数据类
来源：http://puy.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://doj.cashguo.top

[T09] Kotlin：扩展函数
来源：http://mju.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://cgi.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://qke.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vam.cucudq.cn

[T11] Kotlin：协程
来源：http://yyu.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jsd.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://oag.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://mak.316326.xyz

[T13] Kotlin：只读 Map
来源：http://wgr.sysykeji.top

val m = mapOf("a" to 1)
来源：http://ovj.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://hqx.bbcook.cn

for (i in 1..10) println(i)
来源：http://tdo.yuanzhike.top

[T15] Kotlin：接口
来源：http://vfw.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://zlz.gaohongyu789.top

[T16] Swift：Hello World
来源：http://hxl.chenjidiqi.icu

print("Hello")
来源：http://uma.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://bhp.jiagoushi.top

var a = 1;  let b = 2
来源：http://gyi.gotoacloud.top

[T18] Swift：字符串插值
来源：http://nyf.chenjidiqi.icu

"值: \(b)"
来源：http://off.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://ksg.gzhubu.top

if let n = opt { print(n) }
来源：http://uhw.yj20258.top

[T20] Swift：数组操作
来源：http://biz.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jgw.xinyue.icu

[T21] Swift：遍历
来源：http://zzt.ydjk.org.cn

for x in a { print(x) }
来源：http://eut.316326.xyz

[T22] Swift：字典
来源：http://xnn.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://pls.cdnleiting.top

[T23] Swift：函数
来源：http://vlt.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bww.zhoulong.xyz

[T24] Swift：闭包
来源：http://sya.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eod.jinqigufen.top

[T25] Swift：结构体
来源：http://meo.zhiwuduotai.top

struct P { var x: Int }
来源：http://xto.hesvh.cn

[T26] Swift：类与重写
来源：http://cof.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://cbn.yuanzhike.top

[T27] Swift：错误处理
来源：http://nmj.yonumen.top

do { try f() } catch { print(error) }
来源：http://vmz.chenjidiqi.icu

[T28] Swift：枚举
来源：http://cwt.aizwys.cn

enum Color { case red, green }
来源：http://wvx.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://yel.yj20258.top

guard let x = opt else { return }
来源：http://kfx.yvedp.cn

[T30] Swift：协议
来源：http://xxg.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://lub.daxiang520.top

[T31] Lua：Hello World
来源：http://yaf.ehwqpu.com

print("Hello")
来源：http://nku.yj20258888.top

[T32] Lua：局部变量
来源：http://hvv.cqqwz.cn

local a = 1
来源：http://uzm.hysaishi.cn

[T33] Lua：表（数组）
来源：http://ike.svipenyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://txd.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://ppw.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zak.sjlbkw.cn

[T35] Lua：字典表
来源：http://acy.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://rgl.hesvh.cn

[T36] Lua：函数
来源：http://aod.cheryme.top

function add(a, b) return a + b end
来源：http://iel.birdmap.top

[T37] Lua：字符串拼接
来源：http://okx.52xcode.cn

"a" .. "b"
来源：http://rpm.meibo888.top

[T38] Lua：条件
来源：http://ecw.gogol.net.cn

if x > 0 then print("正") end
来源：http://ffp.aibaodan.cn

[T39] Lua：模式匹配
来源：http://ukn.fengsongda.top

string.find(s, "%d+")
来源：http://vyg.yuanzhike.top

[T40] Lua：元表
来源：http://gvk.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://bal.mhx1999.top

[T41] Perl：Hello World
来源：http://tbg.hysaishi.cn

print "Hello\n";
来源：http://kgx.fehbvm.com

[T42] Perl：变量类型
来源：http://mdm.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzd.ppjwa.cn

[T43] Perl：字符串插值
来源：http://ira.zycfv.cn

"值: $a"
来源：http://yum.fktsv.cn

[T44] Perl：条件
来源：http://qwi.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://jkz.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://jid.cashguo.top

for my $x (@arr) { print $x; }
来源：http://avi.hywenlv.cn

[T46] Perl：哈希操作
来源：http://jqn.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eak.jiagoushi.top

[T47] Perl：正则捕获
来源：http://qpv.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eid.daxiang520.top

[T48] Perl：正则替换
来源：http://qnt.jinqigufen.top

$s =~ s/old/new/g;
来源：http://zsy.hysaishi.cn


<!-- 参考信息 -->