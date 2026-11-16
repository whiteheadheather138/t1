代发 wailian999

find . -name "*.log" -type f
来源：http://ljz.gotoacloud.top

[R44] 按修改时间查找
来源：http://zyr.vehdjk.com

find . -mtime -7 -type f
来源：http://eka.yuxming.cn

[R45] 批量删除
来源：http://fqy.smart0.xyz

find . -name "*.tmp" -delete
来源：http://lte.hfpthk.cn

[R46] 递归替换文件内容
来源：http://hdy.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jrd.hnqzz.top

[R47] sed 单行替换
来源：http://npt.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://fva.fehbvm.com

[R48] awk 取指定列
来源：http://apb.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://eps.zhiwuduotai.top

[R49] awk 带条件
来源：http://jou.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pmz.zhaomingkeji.xyz

[R50] awk 求和
来源：http://bjl.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://qlz.wangdashe.top

[R51] 排序去重取前几
来源：http://wtr.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mzi.hongshengwenyu.top

[R52] 统计行数
来源：http://gkh.shanyushiyangkeji.top

wc -l a.txt
来源：http://qsy.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://upf.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxs.vqdsnc.cn

[R54] 比较两个文件
来源：http://bso.jlsjyb.cn

diff a.txt b.txt
来源：http://qyn.yueranfly.top

[R55] 压缩与解压
来源：http://odn.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbm.meibo888.top

[R56] 远程拷贝
来源：http://usp.yueranfly.top

scp file user@host:/path/
来源：http://jqo.cucudq.cn

[R57] 远程执行命令
来源：http://vjo.aizwys.cn

ssh user@host 'uptime'
来源：http://hdm.jqgfzy.top

[R58] 下载文件
来源：http://jvu.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ccw.jlsjyb.cn

[R59] 发 POST JSON
来源：http://fvr.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nba.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://ldz.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://etf.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://crw.xylfe.cn

df -h;  du -sh *
来源：http://iuv.cucudq.cn

[R62] 找最占空间的文件
来源：http://mfo.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://qsg.jqgufenzy.top

[R63] 内存与进程
来源：http://lfn.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://fxa.guowangkeji.top

[R64] 结束进程
来源：http://suy.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://xnl.xuanzx.com

[R65] 查看端口占用
来源：http://yfg.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://goo.quarkkingdee.top

[R66] 定时任务
来源：http://nia.316326.xyz

crontab -e;  crontab -l
来源：http://ody.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://jcx.mhx1999.top

openssl rand -hex 16
来源：http://bvh.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://cdn.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hjp.guannengcc.top

[R69] 生成随机密码
来源：http://jov.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://ije.chenzaomai.com

[R70] 时间戳与互转
来源：http://xev.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://vnw.ehwqpu.com

[R71] 日期格式化
来源：http://sml.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uuf.yuxming.cn

[R72] 等待端口就绪
来源：http://kin.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://azh.vehdjk.com

[R73] 分割大日志
来源：http://stj.zhixingplan.top

split -l 1000 big.log part_
来源：http://gls.nanxuanxn.top

[R74] 批量重命名
来源：http://aoo.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yck.mhx1999.top

[R75] 导出环境变量
来源：http://lcu.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://lmy.dianchejie.cn

[R76] 使用临时文件
来源：http://bvy.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zpm.chenzaomai.com

[R77] 读取用户输入
来源：http://iuw.zhijiandao.cn

read -rp "请输入: " ans
来源：http://vbn.vehdjk.com

[R78] 交互式菜单
来源：http://qhk.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ajm.yuxming.cn

[R79] 解析命令行选项
来源：http://iyy.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cby.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://dfx.cashguo.top

time ./run.sh
来源：http://mjz.dashuyun.cn

================================================================================
来源：http://wez.meibo888.top

S. C / C++ 专题
来源：http://rrc.jinqigufen.top

================================================================================
来源：http://lvb.zdqjudy.top

[S01] C：Hello World
来源：http://aiz.0kj1m.cn

#include <stdio.h>
来源：http://lqw.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://stm.yvedp.cn

[S02] C：变量与格式化输出
来源：http://cxu.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://sfl.cashguo.top

[S03] C：读入整数
来源：http://ieq.316326.xyz

int x; scanf("%d", &x);
来源：http://txk.c1oappe.top

[S04] C：字符串复制
来源：http://gpg.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dcu.sufxvd.cn

[S05] C：字符串长度
来源：http://iqg.quarkkingdee.top

strlen(s)
来源：http://dhb.yangfankeji.com

[S06] C：字符串比较
来源：http://gii.ctjpmb.com

strcmp(a, b) == 0
来源：http://gja.daria6918.cn

[S07] C：数组遍历求和
来源：http://teh.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cjp.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://knz.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lvg.tarul.cn

[S09] C：结构体定义与初始化
来源：http://gwz.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bpl.tanke756.top

[S10] C：指针与解引用
来源：http://cwi.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://gne.aibaodan.cn

[S11] C：逐行读文件
来源：http://teq.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://xbq.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ogb.sxryk.cn

fclose(f);
来源：http://nuw.shuidangran.top

[S12] C：写文件
来源：http://vxq.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ouz.316326.xyz

[S13] C：宏定义
来源：http://osd.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zsg.jinyuanbaomall.cn

[S14] C：枚举
来源：http://oug.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://pmq.ydjk.org.cn

[S15] C：类型转换
来源：http://hxu.zhixingplan.top

(double) a / b
来源：http://ptp.hfpthk.cn

[S16] C：位操作置位
来源：http://tyo.hesvh.cn

x |= (1 << 3);
来源：http://yoc.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://fjz.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://myi.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://iig.dashuyun.cn

int main(int argc, char **argv)
来源：http://khc.svipenyu.cn

[S19] C：快速排序
来源：http://yjl.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://tsh.gzhubu.top

[S20] C：二分查找
来源：http://qwp.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oun.aizwys.cn

[S21] C：字符类别判断
来源：http://xhu.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qns.gogol.net.cn

[S22] C：字符串转数字
来源：http://rtn.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://hxz.zycfv.cn

[S23] C：随机数
来源：http://ujc.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mxe.yj20258888.top

[S24] C：获取本地时间
来源：http://cbi.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://naz.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://szc.guannengcc.top

memcpy(dst, src, n);
来源：http://lcm.jlsjyb.cn

[S26] C：内存清零
来源：http://tsq.daxiang520.top

memset(a, 0, sizeof a);
来源：http://ikx.0kj1m.cn

[S27] C：定义常量
来源：http://mqv.zdbjq.cn

const double PI = 3.14159;
来源：http://rxf.yfazqb.com

[S28] C：静态变量
来源：http://jiq.birdmap.top

static int counter = 0;
来源：http://yrk.hcnkem.com

[S29] C：变参函数
来源：http://xqt.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hen.chenzaomai.com

[S30] C：头文件保护
来源：http://bxr.xziqi.cn

#ifndef X_H
来源：http://hiv.shangyingyoupin.top

#define X_H
来源：http://ygu.hnqzz.top

#endif
来源：http://gpf.hfpthk.cn

[S31] C++：Hello World
来源：http://rjb.shangyingyoupin.top

#include <iostream>
来源：http://khg.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://apg.vqdsnc.cn

[S32] C++：字符串
来源：http://bwf.birdmap.top

std::string s = "hi";  s += "!";
来源：http://yxl.fengsongda.top

[S33] C++：vector 增删
来源：http://jpv.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://osi.daria6918.cn

[S34] C++：遍历 vector
来源：http://cad.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://uoa.xingfuxueyuan.xyz

[S35] C++：map
来源：http://zhh.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rvt.sweek.top

[S36] C++：unordered_map
来源：http://upa.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jhc.zdbjq.cn

[S37] C++：set
来源：http://jis.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fza.wangdashe.top

[S38] C++：排序
来源：http://zpr.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://lfe.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://dhq.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xrc.vqdsnc.cn

[S40] C++：查找元素
来源：http://pcs.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pia.yj20258888.top

[S41] C++：类与构造函数
来源：http://mgf.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqs.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://uow.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://lpg.daxiang520.top

[S43] C++：智能指针
来源：http://swv.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://elb.tianlin.xyz

[S44] C++：引用传参
来源：http://ypm.ivvv.top

void inc(int &x) { ++x; }
来源：http://zzb.gaohongyu789.top

[S45] C++：lambda
来源：http://fjx.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ygo.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://rvi.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ukj.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://shu.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://teb.cashguo.top

[S48] C++：逐行读文件
来源：http://nfj.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://whx.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://dev.cdnleiting.top

[S49] C++：写文件
来源：http://dzd.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pmf.xuanzx.com

[S50] C++：格式化数字
来源：http://byi.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dsw.ppjwa.cn

[S51] C++：显式类型转换
来源：http://ctg.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://xbv.sweek.top

[S52] C++：const 与 noexcept
来源：http://fpf.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://now.havefunace.top

[S53] C++：移动语义
来源：http://wqn.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://bvw.gzhubu.top

[S54] C++：异常处理
来源：http://fhg.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dmo.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://ssi.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nso.hnqzz.top

[S56] C++：optional
来源：http://lwv.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yxb.smart0.xyz

[S57] C++：编译期常量
来源：http://spg.yanxiufei.cn

constexpr int N = 10;
来源：http://abg.zycfv.cn

[S58] C++：命名空间
来源：http://zgk.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://xqy.cqqwz.cn

[S59] C++：静态断言
来源：http://zan.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ien.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://orz.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cun.zhijiandao.cn

================================================================================
来源：http://izf.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sji.kuanghao11.cn

================================================================================
来源：http://bip.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://brx.birdmap.top

println("Hello")
来源：http://bxc.yuxming.cn

[T02] Kotlin：变量
来源：http://isi.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zlx.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://prc.zdbjq.cn

"值: $b"
来源：http://bmg.yvedp.cn

[T04] Kotlin：空安全
来源：http://gvj.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://iog.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://thh.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jxc.aizwys.cn

[T06] Kotlin：集合映射
来源：http://uot.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kzc.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://pll.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gcq.xziqi.cn

[T08] Kotlin：数据类
来源：http://bqi.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://fle.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://cqu.uphjek.com

fun String.exclaim() = this + "!"
来源：http://xqf.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://yak.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://dtp.haohaochexian.top

[T11] Kotlin：协程
来源：http://znd.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttb.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://uoh.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://wyd.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://kcg.hammf.cn

val m = mapOf("a" to 1)
来源：http://kvw.ydzc1.top

[T14] Kotlin：循环
来源：http://xxl.aizwys.cn

for (i in 1..10) println(i)
来源：http://lqx.dashuyun.cn

[T15] Kotlin：接口
来源：http://rcw.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://kgh.gogol.net.cn

[T16] Swift：Hello World
来源：http://fhn.feifeiyinyue.top

print("Hello")
来源：http://tlo.yonumen.top

[T17] Swift：变量与常量
来源：http://gfw.sweek.top

var a = 1;  let b = 2
来源：http://fud.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://owj.mhx1999.top

"值: \(b)"
来源：http://wsq.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://kpx.yj20258888.top

if let n = opt { print(n) }
来源：http://hhd.fehbvm.com

[T20] Swift：数组操作
来源：http://kia.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tpz.guannengcc.top

[T21] Swift：遍历
来源：http://uug.fengsongda.top

for x in a { print(x) }
来源：http://iji.mhx1999.top

[T22] Swift：字典
来源：http://vut.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://xqo.fehbvm.com

[T23] Swift：函数
来源：http://gry.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jko.smart0.xyz

[T24] Swift：闭包
来源：http://dkf.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ouf.yj20258888.top

[T25] Swift：结构体
来源：http://rej.ivvv.top

struct P { var x: Int }
来源：http://lfm.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://cvn.jinqigufen.top

class A: Base { override func f() {} }
来源：http://nvh.nanxinkj.top

[T27] Swift：错误处理
来源：http://poz.hesvh.cn

do { try f() } catch { print(error) }
来源：http://iqw.fzhhl.top

[T28] Swift：枚举
来源：http://ncc.ivvv.top

enum Color { case red, green }
来源：http://khp.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://slz.yonumen.top

guard let x = opt else { return }
来源：http://nnh.sufxvd.cn

[T30] Swift：协议
来源：http://ggh.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://lpu.fehbvm.com

[T31] Lua：Hello World
来源：http://uwr.svipenyu.cn

print("Hello")
来源：http://bin.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://ypb.316326.xyz

local a = 1
来源：http://wky.0kj1m.cn

[T33] Lua：表（数组）
来源：http://qzu.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cpt.xuanzx.com

[T34] Lua：遍历表
来源：http://edt.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://brc.fktsv.cn

[T35] Lua：字典表
来源：http://zmv.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://evr.bjfxy.top

[T36] Lua：函数
来源：http://gwq.jyoumei.cn

function add(a, b) return a + b end
来源：http://dqk.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://knn.gaohongyu789.top

"a" .. "b"
来源：http://lvg.yj202588.top

[T38] Lua：条件
来源：http://zkh.daria6918.cn

if x > 0 then print("正") end
来源：http://wpk.ehwqpu.com

[T39] Lua：模式匹配
来源：http://iwp.zdqjudy.top

string.find(s, "%d+")
来源：http://nlp.jinqigfzy.top

[T40] Lua：元表
来源：http://nzq.tian-w.cn

setmetatable({}, { __index = base })
来源：http://msh.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://ohs.yongpay.top

print "Hello\n";
来源：http://atm.uphjek.com

[T42] Perl：变量类型
来源：http://kkw.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://emw.tarul.cn

[T43] Perl：字符串插值
来源：http://iar.xylfe.cn

"值: $a"
来源：http://uip.yueranfly.top

[T44] Perl：条件
来源：http://tnd.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://qnu.tarul.cn

[T45] Perl：数组遍历
来源：http://muw.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://ekz.svipenyu.cn

[T46] Perl：哈希操作
来源：http://ckv.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gig.gotoacloud.top


<!-- 参考信息 -->