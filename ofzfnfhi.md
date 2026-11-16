代发 wailian999

cmd > out.log 2>&1
来源：http://dsm.jyoumei.cn

[R40] 追加写日志
来源：http://inj.ydzc1.top

echo "log" >> out.log
来源：http://lqr.bjfxy.top

[R41] 丢弃输出
来源：http://vut.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://bds.cdnleiting.top

[R42] 输入重定向
来源：http://xac.chenlongwang.top

wc -l < a.txt
来源：http://waa.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://etz.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://rfz.shuidangran.top

[R44] 按修改时间查找
来源：http://wwc.yj20258888.top

find . -mtime -7 -type f
来源：http://awl.c1oappe.top

[R45] 批量删除
来源：http://quu.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://oql.tarul.cn

[R46] 递归替换文件内容
来源：http://set.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tqg.hnxiangtu.top

[R47] sed 单行替换
来源：http://der.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://jxi.guannengcc.top

[R48] awk 取指定列
来源：http://oze.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://xed.nanxinkj.top

[R49] awk 带条件
来源：http://vnm.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sjl.fengsongda.top

[R50] awk 求和
来源：http://bdd.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://gmz.xinyue.icu

[R51] 排序去重取前几
来源：http://jwh.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cvr.zdbjq.cn

[R52] 统计行数
来源：http://gsc.hongshengwenyu.top

wc -l a.txt
来源：http://xsx.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://jij.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tmv.zhengqikj.top

[R54] 比较两个文件
来源：http://mdu.zhengqikj.top

diff a.txt b.txt
来源：http://bhx.hnqzz.top

[R55] 压缩与解压
来源：http://jfu.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://clg.gzhubu.top

[R56] 远程拷贝
来源：http://rbl.xuanzx.com

scp file user@host:/path/
来源：http://ztn.andypj.xyz

[R57] 远程执行命令
来源：http://wjk.wangdashe.top

ssh user@host 'uptime'
来源：http://lga.0kj1m.cn

[R58] 下载文件
来源：http://chq.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ebi.xuanzx.com

[R59] 发 POST JSON
来源：http://dkp.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tvm.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://ygs.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vqp.uphjek.com

[R61] 磁盘占用
来源：http://exq.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://lkf.cheryme.top

[R62] 找最占空间的文件
来源：http://bce.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://qrg.cashguo.top

[R63] 内存与进程
来源：http://zmd.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://nob.ydjk.org.cn

[R64] 结束进程
来源：http://drx.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://dtf.sxryk.cn

[R65] 查看端口占用
来源：http://beg.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://feb.nwbrower.top

[R66] 定时任务
来源：http://ule.gzhubu.top

crontab -e;  crontab -l
来源：http://frg.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://lij.sjlbkw.cn

openssl rand -hex 16
来源：http://oko.jqgfzy.top

[R68] 计算文件校验值
来源：http://vut.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://cpi.gogol.net.cn

[R69] 生成随机密码
来源：http://vfg.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://iel.aibaodan.cn

[R70] 时间戳与互转
来源：http://zht.hnqzz.top

date +%s;  date -d @1700000000
来源：http://cpm.cqqwz.cn

[R71] 日期格式化
来源：http://mrd.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ekk.pycfn.com

[R72] 等待端口就绪
来源：http://qnq.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jpa.wangshuangyany.cn

[R73] 分割大日志
来源：http://ojx.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://cku.havefunace.top

[R74] 批量重命名
来源：http://rac.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uik.xziqi.cn

[R75] 导出环境变量
来源：http://zrq.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://iuk.ppjwa.cn

[R76] 使用临时文件
来源：http://xrh.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sap.ybcxt.top

[R77] 读取用户输入
来源：http://bod.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://ysd.yonumen.top

[R78] 交互式菜单
来源：http://cmo.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tbq.yj202588.top

[R79] 解析命令行选项
来源：http://ojq.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ycy.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://kil.jianghu66.top

time ./run.sh
来源：http://xue.yj20258888.top

================================================================================
来源：http://jfu.nanxuanxn.top

S. C / C++ 专题
来源：http://ysh.kuanghao11.cn

================================================================================
来源：http://cnp.yanxiufei.cn

[S01] C：Hello World
来源：http://kjb.zhengqikj.top

#include <stdio.h>
来源：http://ekt.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yws.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://gbo.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://egx.hysaishi.cn

[S03] C：读入整数
来源：http://rvl.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://ppc.yj20258.top

[S04] C：字符串复制
来源：http://set.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://tyt.yfazqb.com

[S05] C：字符串长度
来源：http://ttz.jqgfzy.top

strlen(s)
来源：http://eab.tarul.cn

[S06] C：字符串比较
来源：http://kyj.jyoumei.cn

strcmp(a, b) == 0
来源：http://fbe.dianchejie.cn

[S07] C：数组遍历求和
来源：http://jbi.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sgd.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://rfe.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ymj.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://sus.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zqp.9152youxi.cn

[S10] C：指针与解引用
来源：http://hwl.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://shm.ppjwa.cn

[S11] C：逐行读文件
来源：http://dvh.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://sws.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gse.cdnleiting.top

fclose(f);
来源：http://xyh.tian-w.cn

[S12] C：写文件
来源：http://yvy.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eok.cdnleiting.top

[S13] C：宏定义
来源：http://jmr.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mty.nanxinkj.top

[S14] C：枚举
来源：http://opa.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://bui.chenjidiqi.icu

[S15] C：类型转换
来源：http://gir.zhiwuduotai.top

(double) a / b
来源：http://twy.gaohongyu789.top

[S16] C：位操作置位
来源：http://wag.52xcode.cn

x |= (1 << 3);
来源：http://wzy.yj202588.top

[S17] C：安全拼接字符串
来源：http://jbz.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lnk.pycfn.com

[S18] C：命令行参数
来源：http://ajh.jqgfzy.top

int main(int argc, char **argv)
来源：http://fof.zhijiandao.cn

[S19] C：快速排序
来源：http://xex.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pfc.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://mnc.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://soy.yonumen.top

[S21] C：字符类别判断
来源：http://xmc.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gqp.sufxvd.cn

[S22] C：字符串转数字
来源：http://ljb.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xxl.feifeiyinyue.top

[S23] C：随机数
来源：http://aif.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jib.hfpthk.cn

[S24] C：获取本地时间
来源：http://nia.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tyu.wangdashe.top

[S25] C：内存拷贝
来源：http://qri.jlsjyb.cn

memcpy(dst, src, n);
来源：http://rcg.9152youxi.cn

[S26] C：内存清零
来源：http://oel.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://fwb.yonumen.top

[S27] C：定义常量
来源：http://maj.gotoacloud.top

const double PI = 3.14159;
来源：http://qtd.quarkkingdee.top

[S28] C：静态变量
来源：http://kqc.cqqwz.cn

static int counter = 0;
来源：http://qov.daxiang520.top

[S29] C：变参函数
来源：http://xvk.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vhm.gzhubu.top

[S30] C：头文件保护
来源：http://azl.sufxvd.cn

#ifndef X_H
来源：http://uhx.hysaishi.cn

#define X_H
来源：http://hjt.fehbvm.com

#endif
来源：http://jey.epnwcf.com

[S31] C++：Hello World
来源：http://ezp.vqdsnc.cn

#include <iostream>
来源：http://qnw.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://per.sxryk.cn

[S32] C++：字符串
来源：http://sxx.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://ovt.sweek.top

[S33] C++：vector 增删
来源：http://wpv.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://byf.yuxming.cn

[S34] C++：遍历 vector
来源：http://ura.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://xtx.jiagoushi.top

[S35] C++：map
来源：http://tly.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aoc.shuidangran.top

[S36] C++：unordered_map
来源：http://yle.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kva.mhx1999.top

[S37] C++：set
来源：http://dos.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oyz.vqdsnc.cn

[S38] C++：排序
来源：http://rld.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://qff.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://kip.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kml.vehdjk.com

[S40] C++：查找元素
来源：http://pzx.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wob.aibaodan.cn

[S41] C++：类与构造函数
来源：http://nwg.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baf.c1oappe.top

[S42] C++：继承与虚函数
来源：http://zkg.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://rdn.jiagoushi.top

[S43] C++：智能指针
来源：http://pys.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://lsg.zhijiandao.cn

[S44] C++：引用传参
来源：http://mfg.xuanzx.com

void inc(int &x) { ++x; }
来源：http://abz.zhixingplan.top

[S45] C++：lambda
来源：http://wxg.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://tqm.ctjpmb.com

[S46] C++：函数模板
来源：http://kbw.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vdv.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://uql.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zwv.c1oappe.top

[S48] C++：逐行读文件
来源：http://jvs.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aai.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://bvy.gogol.net.cn

[S49] C++：写文件
来源：http://qbw.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tml.hnxiangtu.top

[S50] C++：格式化数字
来源：http://sld.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wia.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://anq.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://sxb.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://dnl.yonumen.top

int size() const noexcept { return n_; }
来源：http://gdt.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://vfi.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://xrz.jiagoushi.top

[S54] C++：异常处理
来源：http://bnr.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fkh.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://ezd.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mgv.vehdjk.com

[S56] C++：optional
来源：http://qpw.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nwq.daxiang520.top

[S57] C++：编译期常量
来源：http://chf.yueranfly.top

constexpr int N = 10;
来源：http://ior.nwbrower.top

[S58] C++：命名空间
来源：http://sas.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://rpe.daxiang520.top

[S59] C++：静态断言
来源：http://fmv.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://frd.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://dgv.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kkm.zdbjq.cn

================================================================================
来源：http://ayf.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://foe.52xcode.cn

================================================================================
来源：http://flk.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://yui.tian-w.cn

println("Hello")
来源：http://bxt.redwolf501.top

[T02] Kotlin：变量
来源：http://liy.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mbn.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://ouc.zhongyouzk.top

"值: $b"
来源：http://mmn.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://hah.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://qcq.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://eoi.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://klr.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://hxp.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yzh.tanke756.top

[T07] Kotlin：集合过滤
来源：http://yrc.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zdc.hesvh.cn

[T08] Kotlin：数据类
来源：http://mfm.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://lmf.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://xvh.uphjek.com

fun String.exclaim() = this + "!"
来源：http://kzn.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://eef.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lgm.zhijiandao.cn

[T11] Kotlin：协程
来源：http://gpm.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://upc.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://hrb.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://ouo.pycfn.com

[T13] Kotlin：只读 Map
来源：http://ckr.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://xbq.chenzaomai.com

[T14] Kotlin：循环
来源：http://wve.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://uax.hnqzz.top

[T15] Kotlin：接口
来源：http://lzp.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://qfk.pycfn.com

[T16] Swift：Hello World
来源：http://mkg.hesvh.cn

print("Hello")
来源：http://zlh.cucudq.cn

[T17] Swift：变量与常量
来源：http://xmq.ppjwa.cn

var a = 1;  let b = 2
来源：http://nmy.jyoumei.cn

[T18] Swift：字符串插值
来源：http://qaf.dashuyun.cn

"值: \(b)"
来源：http://txb.epnwcf.com

[T19] Swift：可选绑定
来源：http://tgp.meibo888.top

if let n = opt { print(n) }
来源：http://rzm.epnwcf.com

[T20] Swift：数组操作
来源：http://wrs.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://uvh.shangyingyoupin.top

[T21] Swift：遍历
来源：http://bvb.yongpay.top

for x in a { print(x) }
来源：http://ggt.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://pvp.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://gpa.zhiwuduotai.top

[T23] Swift：函数
来源：http://xni.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqp.hcnkem.com

[T24] Swift：闭包
来源：http://ygf.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://sre.havefunace.top

[T25] Swift：结构体
来源：http://ytd.sjlbkw.cn

struct P { var x: Int }
来源：http://jdk.tianlin.xyz

[T26] Swift：类与重写
来源：http://gaw.hfpthk.cn

class A: Base { override func f() {} }
来源：http://dnr.guannengcc.top

[T27] Swift：错误处理
来源：http://wmq.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://dqe.andypj.xyz

[T28] Swift：枚举
来源：http://thn.zhoulong.xyz

enum Color { case red, green }
来源：http://jjz.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://nqv.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://hzf.sysykeji.top

[T30] Swift：协议
来源：http://sai.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://hkp.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://uof.daria6918.cn

print("Hello")
来源：http://zom.jqgfzy.top

[T32] Lua：局部变量
来源：http://fqy.ppjwa.cn

local a = 1
来源：http://lsd.yueranfly.top

[T33] Lua：表（数组）
来源：http://mze.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://usk.gaohongyu789.top

[T34] Lua：遍历表
来源：http://tzm.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rpa.yongpay.top

[T35] Lua：字典表
来源：http://abz.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://gdx.pengpengdd.cyou

[T36] Lua：函数
来源：http://xmy.vehdjk.com

function add(a, b) return a + b end
来源：http://wpl.epnwcf.com

[T37] Lua：字符串拼接
来源：http://ekd.52xcode.cn

"a" .. "b"
来源：http://jke.jiagoushi.top

[T38] Lua：条件
来源：http://dan.yanxiufei.cn

if x > 0 then print("正") end
来源：http://jae.zhengqikj.top

[T39] Lua：模式匹配
来源：http://whp.cucudq.cn

string.find(s, "%d+")
来源：http://onn.cucudq.cn

[T40] Lua：元表
来源：http://sfn.316326.xyz

setmetatable({}, { __index = base })
来源：http://rls.bjfxy.top

[T41] Perl：Hello World
来源：http://rqt.chenzaomai.com

print "Hello\n";
来源：http://efo.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://bzp.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pcw.wangshuangyany.cn


<!-- 参考信息 -->