代发 wailian999

find . -name "*.tmp" -delete
来源：http://agd.316326.xyz

[R46] 递归替换文件内容
来源：http://yaa.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://til.0kj1m.cn

[R47] sed 单行替换
来源：http://oxi.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jce.yuxming.cn

[R48] awk 取指定列
来源：http://vjw.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://uco.iojbl.cn

[R49] awk 带条件
来源：http://aic.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otp.yonumen.top

[R50] awk 求和
来源：http://edd.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://abi.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://fdw.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hbw.gaohongyu789.top

[R52] 统计行数
来源：http://sns.c1oappe.top

wc -l a.txt
来源：http://kjy.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://hcv.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://liw.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://xya.yuxming.cn

diff a.txt b.txt
来源：http://kzv.yongpay.top

[R55] 压缩与解压
来源：http://jkh.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nsf.sjlbkw.cn

[R56] 远程拷贝
来源：http://xzf.bjfxy.top

scp file user@host:/path/
来源：http://ylp.pycfn.com

[R57] 远程执行命令
来源：http://qmc.meibo888.top

ssh user@host 'uptime'
来源：http://ith.sysykeji.top

[R58] 下载文件
来源：http://lez.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pgl.cheryme.top

[R59] 发 POST JSON
来源：http://fhk.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mwp.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://dsx.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wwy.smart0.xyz

[R61] 磁盘占用
来源：http://sdc.9152youxi.cn

df -h;  du -sh *
来源：http://tyk.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://jeo.yj202588.top

du -ah . | sort -rh | head -10
来源：http://phb.guowangkeji.top

[R63] 内存与进程
来源：http://car.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://iyu.cucudq.cn

[R64] 结束进程
来源：http://aix.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://xla.jlsjyb.cn

[R65] 查看端口占用
来源：http://hnz.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bvf.hywenlv.cn

[R66] 定时任务
来源：http://til.epnwcf.com

crontab -e;  crontab -l
来源：http://pvk.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://gux.zycfv.cn

openssl rand -hex 16
来源：http://kwu.sjlbkw.cn

[R68] 计算文件校验值
来源：http://yet.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iqw.ydjk.org.cn

[R69] 生成随机密码
来源：http://ofp.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://jds.gzhubu.top

[R70] 时间戳与互转
来源：http://lkr.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://hfh.gogol.net.cn

[R71] 日期格式化
来源：http://gua.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ode.tarul.cn

[R72] 等待端口就绪
来源：http://hxf.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://gwz.hammf.cn

[R73] 分割大日志
来源：http://zia.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://tfc.wangdashe.top

[R74] 批量重命名
来源：http://hag.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zza.chenjidiqi.icu

[R75] 导出环境变量
来源：http://btc.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://jvq.zycfv.cn

[R76] 使用临时文件
来源：http://haw.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dks.snrcjt.cn

[R77] 读取用户输入
来源：http://tbs.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://hjh.vehdjk.com

[R78] 交互式菜单
来源：http://lso.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nzj.haohaochexian.top

[R79] 解析命令行选项
来源：http://jnu.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xes.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://inr.tianlin.xyz

time ./run.sh
来源：http://osw.jiagoushi.top

================================================================================
来源：http://rwc.fktsv.cn

S. C / C++ 专题
来源：http://krl.sufxvd.cn

================================================================================
来源：http://luk.9152youxi.cn

[S01] C：Hello World
来源：http://fhd.yj20258888.top

#include <stdio.h>
来源：http://jeb.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://obt.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://jhg.sweek.top

int a = 10; printf("%d\n", a);
来源：http://plb.smart0.xyz

[S03] C：读入整数
来源：http://thi.smart0.xyz

int x; scanf("%d", &x);
来源：http://tmr.xuanzx.com

[S04] C：字符串复制
来源：http://tcj.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://ktt.xylfe.cn

[S05] C：字符串长度
来源：http://ypp.fehbvm.com

strlen(s)
来源：http://cbh.bbcook.cn

[S06] C：字符串比较
来源：http://ijj.daria6918.cn

strcmp(a, b) == 0
来源：http://pec.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://odg.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oeq.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://vqr.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nmt.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://qlx.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kut.cheryme.top

[S10] C：指针与解引用
来源：http://xww.yfazqb.com

int *p = &a;  *p = 5;
来源：http://url.zdqjudy.top

[S11] C：逐行读文件
来源：http://moa.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://nsr.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://ytl.fehbvm.com

fclose(f);
来源：http://zth.ybcxt.top

[S12] C：写文件
来源：http://qpm.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://umz.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://kzv.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jix.dianchejie.cn

[S14] C：枚举
来源：http://ovk.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://fin.yj202588.top

[S15] C：类型转换
来源：http://ccg.jiagoushi.top

(double) a / b
来源：http://hhn.shzxlz.cn

[S16] C：位操作置位
来源：http://ycc.daria6918.cn

x |= (1 << 3);
来源：http://nnn.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://gau.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pxc.sweek.top

[S18] C：命令行参数
来源：http://ihk.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://elo.zhixingplan.top

[S19] C：快速排序
来源：http://zzp.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://jzi.c1oappe.top

[S20] C：二分查找
来源：http://lfj.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kws.ctjpmb.com

[S21] C：字符类别判断
来源：http://vem.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aks.vqdsnc.cn

[S22] C：字符串转数字
来源：http://vxn.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://vjo.jqgufenzy.top

[S23] C：随机数
来源：http://pbq.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sws.uphjek.com

[S24] C：获取本地时间
来源：http://bdg.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fbm.havefunace.top

[S25] C：内存拷贝
来源：http://oqi.smart0.xyz

memcpy(dst, src, n);
来源：http://zmq.hfpthk.cn

[S26] C：内存清零
来源：http://nel.yvedp.cn

memset(a, 0, sizeof a);
来源：http://kqa.hysaishi.cn

[S27] C：定义常量
来源：http://iep.yvedp.cn

const double PI = 3.14159;
来源：http://fgu.sufxvd.cn

[S28] C：静态变量
来源：http://vti.jinqigufen.top

static int counter = 0;
来源：http://ams.hcnkem.com

[S29] C：变参函数
来源：http://wmb.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvu.jlsjyb.cn

[S30] C：头文件保护
来源：http://cuw.shanyushiyangkeji.top

#ifndef X_H
来源：http://lgy.zhijiandao.cn

#define X_H
来源：http://req.yj20258.top

#endif
来源：http://vwc.0kj1m.cn

[S31] C++：Hello World
来源：http://kzm.haohaochexian.top

#include <iostream>
来源：http://ixg.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://foa.fengsongda.top

[S32] C++：字符串
来源：http://ehh.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://zam.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://ryc.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yvj.uphjek.com

[S34] C++：遍历 vector
来源：http://fcl.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://dvo.xingfuxueyuan.xyz

[S35] C++：map
来源：http://usp.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhf.xylfe.cn

[S36] C++：unordered_map
来源：http://vyk.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xyf.hongshengwenyu.top

[S37] C++：set
来源：http://hew.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://krn.yfazqb.com

[S38] C++：排序
来源：http://tme.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://hgt.birdmap.top

[S39] C++：自定义比较器排序
来源：http://sdc.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vrp.hcnkem.com

[S40] C++：查找元素
来源：http://gfk.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://grh.yongpay.top

[S41] C++：类与构造函数
来源：http://qfr.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvc.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://ljx.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://soy.jyoumei.cn

[S43] C++：智能指针
来源：http://wow.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://cgb.yuxming.cn

[S44] C++：引用传参
来源：http://bfa.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://qpc.cashguo.top

[S45] C++：lambda
来源：http://emn.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://lyq.ctjpmb.com

[S46] C++：函数模板
来源：http://ton.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ega.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://oug.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pig.wangdashe.top

[S48] C++：逐行读文件
来源：http://cse.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://zcl.tian-w.cn

while (std::getline(in, line)) { }
来源：http://wgw.aibaodan.cn

[S49] C++：写文件
来源：http://hxm.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jzk.c1oappe.top

[S50] C++：格式化数字
来源：http://joc.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://drm.hywenlv.cn

[S51] C++：显式类型转换
来源：http://ggz.gaohongyu789.top

static_cast<double>(a) / b
来源：http://qaz.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://bla.tanke756.top

int size() const noexcept { return n_; }
来源：http://gbs.jianghu66.top

[S53] C++：移动语义
来源：http://bzn.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://emr.sysykeji.top

[S54] C++：异常处理
来源：http://kry.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://agr.gogol.net.cn

[S55] C++：结构化绑定
来源：http://dst.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nkg.52xcode.cn

[S56] C++：optional
来源：http://hod.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ytf.xuanzx.com

[S57] C++：编译期常量
来源：http://kgb.zhongyouzk.top

constexpr int N = 10;
来源：http://sjw.feifeiyinyue.top

[S58] C++：命名空间
来源：http://whk.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://mtd.yanxiufei.cn

[S59] C++：静态断言
来源：http://wpn.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bhs.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://vti.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://byz.ctjpmb.com

================================================================================
来源：http://saj.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rff.dianchejie.cn

================================================================================
来源：http://nbo.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://pgy.cqqwz.cn

println("Hello")
来源：http://zxu.yfazqb.com

[T02] Kotlin：变量
来源：http://ukf.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hir.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://zyl.zhoulong.xyz

"值: $b"
来源：http://dws.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://koi.52xcode.cn

val n: String? = null;  n?.length
来源：http://vpf.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://kip.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nlz.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://kll.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wrc.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://jat.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gzn.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://hkm.yonumen.top

data class User(val name: String, val age: Int)
来源：http://uib.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://kdh.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://tzt.andypj.xyz

[T10] Kotlin：默认参数
来源：http://afe.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aex.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://qpw.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://mif.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://epg.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://pqr.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://mpe.sweek.top

val m = mapOf("a" to 1)
来源：http://toj.ctjpmb.com

[T14] Kotlin：循环
来源：http://xts.tianlin.xyz

for (i in 1..10) println(i)
来源：http://jfd.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://xpe.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://uuh.jianghu66.top

[T16] Swift：Hello World
来源：http://dyt.sxryk.cn

print("Hello")
来源：http://ohz.hfpthk.cn

[T17] Swift：变量与常量
来源：http://hbr.snrcjt.cn

var a = 1;  let b = 2
来源：http://fte.52xcode.cn

[T18] Swift：字符串插值
来源：http://dsf.fehbvm.com

"值: \(b)"
来源：http://ogu.316326.xyz

[T19] Swift：可选绑定
来源：http://xyb.meibo888.top

if let n = opt { print(n) }
来源：http://zwc.snrcjt.cn

[T20] Swift：数组操作
来源：http://ldn.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://bbx.yvedp.cn

[T21] Swift：遍历
来源：http://xmm.ctjpmb.com

for x in a { print(x) }
来源：http://niu.gaohongyu789.top

[T22] Swift：字典
来源：http://vkm.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://ein.yj20258.top

[T23] Swift：函数
来源：http://nqx.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ror.yanxiufei.cn

[T24] Swift：闭包
来源：http://xep.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfw.hfpthk.cn

[T25] Swift：结构体
来源：http://gqm.chenlongwang.top

struct P { var x: Int }
来源：http://vcj.daria6918.cn

[T26] Swift：类与重写
来源：http://fbb.gotoacloud.top

class A: Base { override func f() {} }
来源：http://iyj.jiagoushi.top

[T27] Swift：错误处理
来源：http://yhs.hammf.cn

do { try f() } catch { print(error) }
来源：http://klc.tarul.cn

[T28] Swift：枚举
来源：http://hai.316326.xyz

enum Color { case red, green }
来源：http://mzh.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://eod.9152youxi.cn

guard let x = opt else { return }
来源：http://mcr.hnqzz.top

[T30] Swift：协议
来源：http://ovi.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://cqm.tian-w.cn

[T31] Lua：Hello World
来源：http://icx.ydjk.org.cn

print("Hello")
来源：http://del.zhengqikj.top

[T32] Lua：局部变量
来源：http://qvq.9152youxi.cn

local a = 1
来源：http://hgf.aizwys.cn

[T33] Lua：表（数组）
来源：http://qom.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mau.sxryk.cn

[T34] Lua：遍历表
来源：http://zwd.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://utn.andypj.xyz

[T35] Lua：字典表
来源：http://fmy.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://afi.yueranfly.top

[T36] Lua：函数
来源：http://cyu.52xcode.cn

function add(a, b) return a + b end
来源：http://ryk.hammf.cn

[T37] Lua：字符串拼接
来源：http://dcy.zhongyouzk.top

"a" .. "b"
来源：http://wgz.aibaodan.cn

[T38] Lua：条件
来源：http://bcl.aizwys.cn

if x > 0 then print("正") end
来源：http://tnp.vehdjk.com

[T39] Lua：模式匹配
来源：http://dje.aibaodan.cn

string.find(s, "%d+")
来源：http://lue.zdbjq.cn

[T40] Lua：元表
来源：http://jxf.redwolf501.top

setmetatable({}, { __index = base })
来源：http://kiu.zdqjudy.top

[T41] Perl：Hello World
来源：http://mkl.xziqi.cn

print "Hello\n";
来源：http://juj.cqqwz.cn

[T42] Perl：变量类型
来源：http://eqw.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jnk.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://eip.shuidangran.top

"值: $a"
来源：http://lhu.shanyushiyangtech.top

[T44] Perl：条件
来源：http://zta.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://jwj.redwolf501.top

[T45] Perl：数组遍历
来源：http://kqd.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://tmh.cucudq.cn

[T46] Perl：哈希操作
来源：http://zuw.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ngi.hcnkem.com

[T47] Perl：正则捕获
来源：http://zhb.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lvy.daria6918.cn

[T48] Perl：正则替换
来源：http://qiw.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://qlb.shuidangran.top


<!-- 参考信息 -->