代发 wailian999

cmd >/dev/null 2>&1
来源：http://zql.fzhhl.top

[R42] 输入重定向
来源：http://kww.tanke756.top

wc -l < a.txt
来源：http://bxo.zhixingplan.top

[R43] 按名字查找文件
来源：http://ogf.tanke756.top

find . -name "*.log" -type f
来源：http://aqc.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://xrz.ivvv.top

find . -mtime -7 -type f
来源：http://zce.hnxiangtu.top

[R45] 批量删除
来源：http://avx.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://tra.daria6918.cn

[R46] 递归替换文件内容
来源：http://rhm.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cqh.shangyingyoupin.top

[R47] sed 单行替换
来源：http://jqv.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://usz.gogol.net.cn

[R48] awk 取指定列
来源：http://cxk.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://hbo.hesvh.cn

[R49] awk 带条件
来源：http://tiz.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dwt.shzxlz.cn

[R50] awk 求和
来源：http://nfy.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wmq.gotoacloud.top

[R51] 排序去重取前几
来源：http://hai.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://siv.yuxming.cn

[R52] 统计行数
来源：http://uqj.yj202588.top

wc -l a.txt
来源：http://ymu.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://mtw.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qja.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://lco.gotoacloud.top

diff a.txt b.txt
来源：http://fid.zdbjq.cn

[R55] 压缩与解压
来源：http://lvs.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rwx.hesvh.cn

[R56] 远程拷贝
来源：http://cgb.ybcxt.top

scp file user@host:/path/
来源：http://kyf.tianlin.xyz

[R57] 远程执行命令
来源：http://xmm.nanxuanxn.top

ssh user@host 'uptime'
来源：http://vyw.jiagoushi.top

[R58] 下载文件
来源：http://jui.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kwr.0kj1m.cn

[R59] 发 POST JSON
来源：http://flg.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iau.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://ypx.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pqy.zhixingplan.top

[R61] 磁盘占用
来源：http://qdd.zdbjq.cn

df -h;  du -sh *
来源：http://qgy.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://xff.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://rex.tian-w.cn

[R63] 内存与进程
来源：http://gql.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://wbv.iojbl.cn

[R64] 结束进程
来源：http://ziq.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://fua.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://ven.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vlh.yangfankeji.com

[R66] 定时任务
来源：http://hxs.snrcjt.cn

crontab -e;  crontab -l
来源：http://uvz.fehbvm.com

[R67] 生成随机十六进制串
来源：http://onq.andypj.xyz

openssl rand -hex 16
来源：http://age.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://dzo.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://lpp.sxryk.cn

[R69] 生成随机密码
来源：http://ylk.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://scq.ybcxt.top

[R70] 时间戳与互转
来源：http://ejf.ydzc1.top

date +%s;  date -d @1700000000
来源：http://ywm.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://wry.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dat.yvedp.cn

[R72] 等待端口就绪
来源：http://szz.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pmk.uphjek.com

[R73] 分割大日志
来源：http://kvs.gaohongyu789.top

split -l 1000 big.log part_
来源：http://jzl.yangfankeji.com

[R74] 批量重命名
来源：http://npv.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zxo.ydzc1.top

[R75] 导出环境变量
来源：http://xvg.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://qjv.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://bpt.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cdi.yj20258888.top

[R77] 读取用户输入
来源：http://fxx.316326.xyz

read -rp "请输入: " ans
来源：http://qmo.hfpthk.cn

[R78] 交互式菜单
来源：http://dwm.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gvk.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://pjm.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qap.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wwx.zhongyouzk.top

time ./run.sh
来源：http://oog.smart0.xyz

================================================================================
来源：http://lxm.hnqzz.top

S. C / C++ 专题
来源：http://vut.sufxvd.cn

================================================================================
来源：http://sap.ydzc1.top

[S01] C：Hello World
来源：http://ekc.xylfe.cn

#include <stdio.h>
来源：http://ffl.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gct.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://uxb.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://gnl.yonumen.top

[S03] C：读入整数
来源：http://nkn.yuanzhike.top

int x; scanf("%d", &x);
来源：http://uzv.yj20258.top

[S04] C：字符串复制
来源：http://slb.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://seg.aibaodan.cn

[S05] C：字符串长度
来源：http://rag.redwolf501.top

strlen(s)
来源：http://lec.tian-w.cn

[S06] C：字符串比较
来源：http://dne.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://zgr.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://ede.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wox.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://sdi.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vpf.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://oew.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qcl.hywenlv.cn

[S10] C：指针与解引用
来源：http://mfz.mhx1999.top

int *p = &a;  *p = 5;
来源：http://byf.meibo888.top

[S11] C：逐行读文件
来源：http://yzf.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://aij.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hlw.cdnleiting.top

fclose(f);
来源：http://ktp.andypj.xyz

[S12] C：写文件
来源：http://xgx.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bhl.gogol.net.cn

[S13] C：宏定义
来源：http://wje.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jim.cucudq.cn

[S14] C：枚举
来源：http://ffx.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://far.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://kss.xylfe.cn

(double) a / b
来源：http://fcl.yuanzhike.top

[S16] C：位操作置位
来源：http://tvz.yvedp.cn

x |= (1 << 3);
来源：http://rrj.xziqi.cn

[S17] C：安全拼接字符串
来源：http://nqp.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hkc.daria6918.cn

[S18] C：命令行参数
来源：http://vhr.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://bch.tianlin.xyz

[S19] C：快速排序
来源：http://wbn.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://pfy.zhixingplan.top

[S20] C：二分查找
来源：http://klg.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tli.uphjek.com

[S21] C：字符类别判断
来源：http://qsn.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jcn.hfpthk.cn

[S22] C：字符串转数字
来源：http://ykd.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://exf.bjfxy.top

[S23] C：随机数
来源：http://ump.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://alk.ppjwa.cn

[S24] C：获取本地时间
来源：http://bqx.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://trk.ehwqpu.com

[S25] C：内存拷贝
来源：http://wfb.haohaochexian.top

memcpy(dst, src, n);
来源：http://odm.hnxiangtu.top

[S26] C：内存清零
来源：http://xfv.sweek.top

memset(a, 0, sizeof a);
来源：http://ibn.ybcxt.top

[S27] C：定义常量
来源：http://kau.zhiwuduotai.top

const double PI = 3.14159;
来源：http://jrl.redwolf501.top

[S28] C：静态变量
来源：http://fem.yanxiufei.cn

static int counter = 0;
来源：http://hgm.sxryk.cn

[S29] C：变参函数
来源：http://rex.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://chf.jinqigfzy.top

[S30] C：头文件保护
来源：http://zff.gogol.net.cn

#ifndef X_H
来源：http://huq.nanxinkj.top

#define X_H
来源：http://sft.mhx1999.top

#endif
来源：http://ptw.yuxming.cn

[S31] C++：Hello World
来源：http://njn.hesvh.cn

#include <iostream>
来源：http://ome.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://hsg.zhongyouzk.top

[S32] C++：字符串
来源：http://nad.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://ots.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://xjg.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hbu.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://cld.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://ohq.hysaishi.cn

[S35] C++：map
来源：http://myj.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://elg.yfazqb.com

[S36] C++：unordered_map
来源：http://pqd.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://axu.zhaomingkeji.xyz

[S37] C++：set
来源：http://zuv.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zxg.jyoumei.cn

[S38] C++：排序
来源：http://xqa.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://wvq.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://krq.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://phv.haohaochexian.top

[S40] C++：查找元素
来源：http://iqx.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cme.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://vho.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fwi.cheryme.top

[S42] C++：继承与虚函数
来源：http://gaz.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://kri.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://srz.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://wxq.quarkkingdee.top

[S44] C++：引用传参
来源：http://xcx.meibo888.top

void inc(int &x) { ++x; }
来源：http://bqa.jianghu66.top

[S45] C++：lambda
来源：http://zwc.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://etg.nanxuanxn.top

[S46] C++：函数模板
来源：http://jap.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://odd.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://bfp.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hgb.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://kco.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzq.tian-w.cn

while (std::getline(in, line)) { }
来源：http://cqh.dianchejie.cn

[S49] C++：写文件
来源：http://qjt.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cvz.vehdjk.com

[S50] C++：格式化数字
来源：http://hdk.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fma.zdbjq.cn

[S51] C++：显式类型转换
来源：http://xyr.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://kpu.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://vpn.yj20258.top

int size() const noexcept { return n_; }
来源：http://wdi.xinyue.icu

[S53] C++：移动语义
来源：http://cwy.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://ssp.yuxming.cn

[S54] C++：异常处理
来源：http://ocq.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lqn.aibaodan.cn

[S55] C++：结构化绑定
来源：http://nkt.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://idn.haohaochexian.top

[S56] C++：optional
来源：http://evu.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hbj.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://lgp.svipenyu.cn

constexpr int N = 10;
来源：http://ose.feifeiyinyue.top

[S58] C++：命名空间
来源：http://tvr.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://tqo.dashuyun.cn

[S59] C++：静态断言
来源：http://evu.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ooh.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://uzf.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mnj.chenzaomai.com

================================================================================
来源：http://bnc.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://muq.gotoacloud.top

================================================================================
来源：http://ojn.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://hys.jianghu66.top

println("Hello")
来源：http://djd.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://rwv.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cdx.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://usj.pycfn.com

"值: $b"
来源：http://ipx.sysykeji.top

[T04] Kotlin：空安全
来源：http://qmb.hysaishi.cn

val n: String? = null;  n?.length
来源：http://bja.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://fqb.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://glt.mhx1999.top

[T06] Kotlin：集合映射
来源：http://uro.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pdf.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://axx.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://dap.xinyue.icu

[T08] Kotlin：数据类
来源：http://ras.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://ygh.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://lrh.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://hsk.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://gnj.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qny.xinyue.icu

[T11] Kotlin：协程
来源：http://bcx.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wmf.birdmap.top

[T12] Kotlin：解构声明
来源：http://lmr.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://jpg.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://vcv.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://dqj.hammf.cn

[T14] Kotlin：循环
来源：http://fpj.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://acb.hywenlv.cn

[T15] Kotlin：接口
来源：http://rbm.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://vme.wangdashe.top

[T16] Swift：Hello World
来源：http://arl.sufxvd.cn

print("Hello")
来源：http://aro.shuidangran.top

[T17] Swift：变量与常量
来源：http://uyp.snrcjt.cn

var a = 1;  let b = 2
来源：http://god.ybcxt.top

[T18] Swift：字符串插值
来源：http://mpv.shanyushiyangkeji.top

"值: \(b)"
来源：http://ysm.yueranfly.top

[T19] Swift：可选绑定
来源：http://tox.shuidangran.top

if let n = opt { print(n) }
来源：http://hic.fengsongda.top

[T20] Swift：数组操作
来源：http://zgs.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rxl.hongshengwenyu.top

[T21] Swift：遍历
来源：http://gbw.hysaishi.cn

for x in a { print(x) }
来源：http://wuw.jianghu66.top

[T22] Swift：字典
来源：http://hjv.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://szo.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://efh.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hwr.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://ylg.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://fqx.xziqi.cn

[T25] Swift：结构体
来源：http://nhi.bbcook.cn

struct P { var x: Int }
来源：http://zas.vehdjk.com

[T26] Swift：类与重写
来源：http://bti.jyoumei.cn

class A: Base { override func f() {} }
来源：http://nao.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://wnp.andypj.xyz

do { try f() } catch { print(error) }
来源：http://rtx.dianchejie.cn

[T28] Swift：枚举
来源：http://alu.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://tgv.cheryme.top

[T29] Swift：guard 提前返回
来源：http://qkg.xuanzx.com

guard let x = opt else { return }
来源：http://ewt.hfpthk.cn

[T30] Swift：协议
来源：http://nli.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://wio.nanxuanxn.top

[T31] Lua：Hello World
来源：http://obq.shanyushiyangkeji.top

print("Hello")
来源：http://tks.aibaodan.cn

[T32] Lua：局部变量
来源：http://vea.fehbvm.com

local a = 1
来源：http://put.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://pov.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nek.hesvh.cn

[T34] Lua：遍历表
来源：http://zis.tanke756.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ezn.daxiang520.top

[T35] Lua：字典表
来源：http://nts.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://aux.cashguo.top

[T36] Lua：函数
来源：http://lag.wangdashe.top

function add(a, b) return a + b end
来源：http://kgq.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://cwn.yj20258888.top

"a" .. "b"
来源：http://kjn.tanke756.top

[T38] Lua：条件
来源：http://dvz.iojbl.cn

if x > 0 then print("正") end
来源：http://arf.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://npt.haohaochexian.top

string.find(s, "%d+")
来源：http://lox.tian-w.cn

[T40] Lua：元表
来源：http://ytk.tian-w.cn

setmetatable({}, { __index = base })
来源：http://jdy.yj20258888.top

[T41] Perl：Hello World
来源：http://all.zycfv.cn

print "Hello\n";
来源：http://cgp.cashguo.top

[T42] Perl：变量类型
来源：http://qxq.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://izy.yuanzhike.top

[T43] Perl：字符串插值
来源：http://urq.shuidangran.top

"值: $a"
来源：http://fin.hfpthk.cn

[T44] Perl：条件
来源：http://ndj.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://hwo.meibo888.top


<!-- 参考信息 -->