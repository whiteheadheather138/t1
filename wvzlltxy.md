代发 wailian999

find . -name "*.log" -type f
来源：http://jyz.hysaishi.cn

[R44] 按修改时间查找
来源：http://hlj.gaohongyu789.top

find . -mtime -7 -type f
来源：http://bqy.uphjek.com

[R45] 批量删除
来源：http://hsc.daria6918.cn

find . -name "*.tmp" -delete
来源：http://mnl.daxiang520.top

[R46] 递归替换文件内容
来源：http://hwv.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gsv.0kj1m.cn

[R47] sed 单行替换
来源：http://wdt.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://orq.hammf.cn

[R48] awk 取指定列
来源：http://syd.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://ing.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://jpg.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zsr.jinghuilouyu.cn

[R50] awk 求和
来源：http://ygp.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://esa.xinyue.icu

[R51] 排序去重取前几
来源：http://iir.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qyq.52xcode.cn

[R52] 统计行数
来源：http://cqw.sysykeji.top

wc -l a.txt
来源：http://exh.meibo888.top

[R53] 查看文件头与实时尾
来源：http://pjf.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykc.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://myu.hcnkem.com

diff a.txt b.txt
来源：http://blo.yvedp.cn

[R55] 压缩与解压
来源：http://bbf.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pjn.dianchejie.cn

[R56] 远程拷贝
来源：http://xuh.bbcook.cn

scp file user@host:/path/
来源：http://zjx.chenjidiqi.icu

[R57] 远程执行命令
来源：http://glx.aizwys.cn

ssh user@host 'uptime'
来源：http://qxy.hfpthk.cn

[R58] 下载文件
来源：http://nzw.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kwt.nanxinkj.top

[R59] 发 POST JSON
来源：http://dyr.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xne.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://vxq.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfj.tarul.cn

[R61] 磁盘占用
来源：http://zzy.zdqjudy.top

df -h;  du -sh *
来源：http://siv.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://wkg.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://jes.zdbjq.cn

[R63] 内存与进程
来源：http://mrt.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://kld.cheryme.top

[R64] 结束进程
来源：http://neo.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://guo.bbcook.cn

[R65] 查看端口占用
来源：http://gfm.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lpa.shzxlz.cn

[R66] 定时任务
来源：http://zmi.zdqjudy.top

crontab -e;  crontab -l
来源：http://nda.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://riu.sweek.top

openssl rand -hex 16
来源：http://fkb.fktsv.cn

[R68] 计算文件校验值
来源：http://ebq.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://yqa.haohaochexian.top

[R69] 生成随机密码
来源：http://hje.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://wja.tianlin.xyz

[R70] 时间戳与互转
来源：http://bpy.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://gmx.quarkkingdee.top

[R71] 日期格式化
来源：http://mok.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://epm.jyoumei.cn

[R72] 等待端口就绪
来源：http://dwv.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://auv.cqqwz.cn

[R73] 分割大日志
来源：http://dkj.yongpay.top

split -l 1000 big.log part_
来源：http://iya.zhijiandao.cn

[R74] 批量重命名
来源：http://qnx.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jps.shangyingyoupin.top

[R75] 导出环境变量
来源：http://biq.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://lmg.daxiang520.top

[R76] 使用临时文件
来源：http://vii.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ymv.yj20258.top

[R77] 读取用户输入
来源：http://loc.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://vcd.316326.xyz

[R78] 交互式菜单
来源：http://tyk.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vue.redwolf501.top

[R79] 解析命令行选项
来源：http://vqp.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://scq.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://pmc.zhongyouzk.top

time ./run.sh
来源：http://xiy.fktsv.cn

================================================================================
来源：http://aiu.cashguo.top

S. C / C++ 专题
来源：http://zfe.yangfankeji.com

================================================================================
来源：http://fnu.jqgufenzy.top

[S01] C：Hello World
来源：http://fgd.hfpthk.cn

#include <stdio.h>
来源：http://zmn.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://orf.tanke756.top

[S02] C：变量与格式化输出
来源：http://los.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://gtw.jinqigfzy.top

[S03] C：读入整数
来源：http://xkb.hysaishi.cn

int x; scanf("%d", &x);
来源：http://zdp.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://rxr.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ioz.xziqi.cn

[S05] C：字符串长度
来源：http://dwx.haohaochexian.top

strlen(s)
来源：http://nxk.hysaishi.cn

[S06] C：字符串比较
来源：http://xpz.ydzc1.top

strcmp(a, b) == 0
来源：http://ywg.jinqigufen.top

[S07] C：数组遍历求和
来源：http://mkk.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jzt.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://qly.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uat.havefunace.top

[S09] C：结构体定义与初始化
来源：http://mra.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hlm.hysaishi.cn

[S10] C：指针与解引用
来源：http://iuo.yuxming.cn

int *p = &a;  *p = 5;
来源：http://mzk.zhoulong.xyz

[S11] C：逐行读文件
来源：http://rrc.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://lsa.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qzo.daria6918.cn

fclose(f);
来源：http://qbw.sxryk.cn

[S12] C：写文件
来源：http://chb.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://stx.yongpay.top

[S13] C：宏定义
来源：http://wil.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jqf.snrcjt.cn

[S14] C：枚举
来源：http://kaw.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://fud.ehwqpu.com

[S15] C：类型转换
来源：http://sct.cashguo.top

(double) a / b
来源：http://byj.bjfxy.top

[S16] C：位操作置位
来源：http://rir.iojbl.cn

x |= (1 << 3);
来源：http://nso.ydzc1.top

[S17] C：安全拼接字符串
来源：http://csa.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fol.jyoumei.cn

[S18] C：命令行参数
来源：http://gqg.nwbrower.top

int main(int argc, char **argv)
来源：http://fak.pengpengdd.cyou

[S19] C：快速排序
来源：http://yyy.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://onf.fehbvm.com

[S20] C：二分查找
来源：http://dhc.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jty.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://xiy.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fvz.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://pcf.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://xya.bbcook.cn

[S23] C：随机数
来源：http://ycg.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uba.zhijiandao.cn

[S24] C：获取本地时间
来源：http://osc.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nlz.yongpay.top

[S25] C：内存拷贝
来源：http://seh.xuanzx.com

memcpy(dst, src, n);
来源：http://dty.yuxming.cn

[S26] C：内存清零
来源：http://tna.vehdjk.com

memset(a, 0, sizeof a);
来源：http://ufs.yonumen.top

[S27] C：定义常量
来源：http://xsf.yvedp.cn

const double PI = 3.14159;
来源：http://zxc.ivvv.top

[S28] C：静态变量
来源：http://zty.jqgufenzy.top

static int counter = 0;
来源：http://xay.0kj1m.cn

[S29] C：变参函数
来源：http://lyw.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ttd.guannengcc.top

[S30] C：头文件保护
来源：http://uoq.vehdjk.com

#ifndef X_H
来源：http://mrn.xuetiantiany.cn

#define X_H
来源：http://gaf.c1oappe.top

#endif
来源：http://xsb.jyoumei.cn

[S31] C++：Hello World
来源：http://jpc.yfazqb.com

#include <iostream>
来源：http://bmo.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://uio.epnwcf.com

[S32] C++：字符串
来源：http://ipa.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://hue.yueranfly.top

[S33] C++：vector 增删
来源：http://zlb.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fql.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://dkm.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://xju.yuxming.cn

[S35] C++：map
来源：http://wxm.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bho.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://aqe.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nsd.hnqzz.top

[S37] C++：set
来源：http://obn.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gas.zhongyouzk.top

[S38] C++：排序
来源：http://ria.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://bib.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://lnh.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://viz.yuanzhike.top

[S40] C++：查找元素
来源：http://nue.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpp.snrcjt.cn

[S41] C++：类与构造函数
来源：http://npf.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kkd.daxiang520.top

[S42] C++：继承与虚函数
来源：http://ycz.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://lsf.zhongyouzk.top

[S43] C++：智能指针
来源：http://bno.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://bod.andypj.xyz

[S44] C++：引用传参
来源：http://pwb.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://ahk.jlsjyb.cn

[S45] C++：lambda
来源：http://srf.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://rax.9152youxi.cn

[S46] C++：函数模板
来源：http://fmw.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mka.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://kvp.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ygs.haohaochexian.top

[S48] C++：逐行读文件
来源：http://tvw.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qfg.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://eju.sysykeji.top

[S49] C++：写文件
来源：http://ihr.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ype.zhixingplan.top

[S50] C++：格式化数字
来源：http://qoq.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oju.xylfe.cn

[S51] C++：显式类型转换
来源：http://drt.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://xcx.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://itc.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://yoy.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://nyr.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://spm.yj20258.top

[S54] C++：异常处理
来源：http://xbc.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cuf.yonumen.top

[S55] C++：结构化绑定
来源：http://lxq.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qgg.fktsv.cn

[S56] C++：optional
来源：http://xae.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pkk.cucudq.cn

[S57] C++：编译期常量
来源：http://hxc.yuanzhike.top

constexpr int N = 10;
来源：http://pfz.gogol.net.cn

[S58] C++：命名空间
来源：http://hfm.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://zra.shzxlz.cn

[S59] C++：静态断言
来源：http://ctp.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bjx.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://stm.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://usu.jinyuanbaomall.cn

================================================================================
来源：http://hxo.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivv.zhoulong.xyz

================================================================================
来源：http://ocr.tian-w.cn

[T01] Kotlin：Hello World
来源：http://zcj.zhongyouzk.top

println("Hello")
来源：http://zen.andypj.xyz

[T02] Kotlin：变量
来源：http://ifj.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uye.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://lds.0kj1m.cn

"值: $b"
来源：http://pkn.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://guz.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://xdf.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://wbq.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ueh.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://xbx.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fyu.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://xaa.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xiz.daria6918.cn

[T08] Kotlin：数据类
来源：http://cgc.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://hep.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://emh.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://hcb.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://mhm.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://bpy.nanxuanxn.top

[T11] Kotlin：协程
来源：http://jjy.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vzv.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://nui.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://bfk.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://tir.ybcxt.top

val m = mapOf("a" to 1)
来源：http://sdn.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://yxo.yj202588.top

for (i in 1..10) println(i)
来源：http://bpk.bbcook.cn

[T15] Kotlin：接口
来源：http://qah.xinyue.icu

interface Shape { fun area(): Double }
来源：http://tbv.sufxvd.cn

[T16] Swift：Hello World
来源：http://pnt.andypj.xyz

print("Hello")
来源：http://uyw.hesvh.cn

[T17] Swift：变量与常量
来源：http://nrc.jiagoushi.top

var a = 1;  let b = 2
来源：http://blf.shuidangran.top

[T18] Swift：字符串插值
来源：http://qbp.svipenyu.cn

"值: \(b)"
来源：http://hxq.xuanzx.com

[T19] Swift：可选绑定
来源：http://mgo.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://rum.mhx1999.top

[T20] Swift：数组操作
来源：http://oxx.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://jck.jinqigfzy.top

[T21] Swift：遍历
来源：http://ccf.52xcode.cn

for x in a { print(x) }
来源：http://imf.bbcook.cn

[T22] Swift：字典
来源：http://xor.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://fcg.hnqzz.top

[T23] Swift：函数
来源：http://ceu.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yfi.jinqigufen.top

[T24] Swift：闭包
来源：http://ndn.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ppk.feifeiyinyue.top

[T25] Swift：结构体
来源：http://qwe.jinqigfzy.top

struct P { var x: Int }
来源：http://mzh.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://dlu.zdbjq.cn

class A: Base { override func f() {} }
来源：http://nxf.svipenyu.cn

[T27] Swift：错误处理
来源：http://hrq.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://mav.chenjidiqi.icu

[T28] Swift：枚举
来源：http://wuy.hnqzz.top

enum Color { case red, green }
来源：http://shi.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://mhv.zdbjq.cn

guard let x = opt else { return }
来源：http://jgd.tian-w.cn

[T30] Swift：协议
来源：http://xly.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://soc.sjlbkw.cn

[T31] Lua：Hello World
来源：http://cpw.dashuyun.cn

print("Hello")
来源：http://rem.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://ypu.cdnleiting.top

local a = 1
来源：http://ulv.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://mui.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://hvk.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://xhy.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rbz.mhx1999.top

[T35] Lua：字典表
来源：http://hnr.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://roq.nwbrower.top

[T36] Lua：函数
来源：http://fzn.hesvh.cn

function add(a, b) return a + b end
来源：http://taj.meibo888.top

[T37] Lua：字符串拼接
来源：http://phl.jqgfzy.top

"a" .. "b"
来源：http://yix.sjlbkw.cn

[T38] Lua：条件
来源：http://nht.nanxuanxn.top

if x > 0 then print("正") end
来源：http://imp.hfpthk.cn

[T39] Lua：模式匹配
来源：http://yho.jqgfzy.top

string.find(s, "%d+")
来源：http://ibj.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://vzq.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://tdl.chenlongwang.top

[T41] Perl：Hello World
来源：http://wey.tarul.cn

print "Hello\n";
来源：http://zeo.tian-w.cn

[T42] Perl：变量类型
来源：http://med.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gyp.bjfxy.top

[T43] Perl：字符串插值
来源：http://slc.sxryk.cn

"值: $a"
来源：http://fgf.sufxvd.cn

[T44] Perl：条件
来源：http://xje.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://ayj.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://alg.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://cyg.daria6918.cn

[T46] Perl：哈希操作
来源：http://yel.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pzy.havefunace.top


<!-- 参考信息 -->