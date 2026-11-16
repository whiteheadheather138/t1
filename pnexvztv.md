代发 wailian999

find . -name "*.log" -type f
来源：http://nzc.zhijiandao.cn

[R44] 按修改时间查找
来源：http://zez.jqgufenzy.top

find . -mtime -7 -type f
来源：http://sve.zhixingplan.top

[R45] 批量删除
来源：http://elv.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://ihz.jyoumei.cn

[R46] 递归替换文件内容
来源：http://jag.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hnr.zycfv.cn

[R47] sed 单行替换
来源：http://oex.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tfs.sjlbkw.cn

[R48] awk 取指定列
来源：http://ueo.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://xzh.nwbrower.top

[R49] awk 带条件
来源：http://slo.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://clb.ywan-chungtsiang.top

[R50] awk 求和
来源：http://gas.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://msb.hnxiangtu.top

[R51] 排序去重取前几
来源：http://ukx.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aql.gogol.net.cn

[R52] 统计行数
来源：http://eqe.hfpthk.cn

wc -l a.txt
来源：http://ncz.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://jsm.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pjt.xziqi.cn

[R54] 比较两个文件
来源：http://nuv.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://fge.cqqwz.cn

[R55] 压缩与解压
来源：http://xib.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bre.chenlongwang.top

[R56] 远程拷贝
来源：http://axt.yj20258.top

scp file user@host:/path/
来源：http://psx.yj20258.top

[R57] 远程执行命令
来源：http://xrv.jiagoushi.top

ssh user@host 'uptime'
来源：http://zuz.sysykeji.top

[R58] 下载文件
来源：http://ixq.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iev.yuanzhike.top

[R59] 发 POST JSON
来源：http://hjl.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nww.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://gea.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgi.hammf.cn

[R61] 磁盘占用
来源：http://yek.jinqigufen.top

df -h;  du -sh *
来源：http://yqg.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://gsd.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://tjk.xziqi.cn

[R63] 内存与进程
来源：http://uof.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://imv.yj20258888.top

[R64] 结束进程
来源：http://tpu.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://vny.nanxinkj.top

[R65] 查看端口占用
来源：http://lqo.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lqp.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://eut.zdqjudy.top

crontab -e;  crontab -l
来源：http://zmd.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://mki.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://knb.havefunace.top

[R68] 计算文件校验值
来源：http://yba.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ycm.nwbrower.top

[R69] 生成随机密码
来源：http://jvd.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://nbj.fktsv.cn

[R70] 时间戳与互转
来源：http://jyl.cheryme.top

date +%s;  date -d @1700000000
来源：http://svy.hesvh.cn

[R71] 日期格式化
来源：http://phs.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ivn.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://gbg.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yxx.sufxvd.cn

[R73] 分割大日志
来源：http://pzq.sweek.top

split -l 1000 big.log part_
来源：http://tll.cheryme.top

[R74] 批量重命名
来源：http://wws.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://axo.jlsjyb.cn

[R75] 导出环境变量
来源：http://vta.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://hvj.yongpay.top

[R76] 使用临时文件
来源：http://qes.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://otn.sysykeji.top

[R77] 读取用户输入
来源：http://sot.c1oappe.top

read -rp "请输入: " ans
来源：http://vkz.jinqigfzy.top

[R78] 交互式菜单
来源：http://hoo.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jay.hnxiangtu.top

[R79] 解析命令行选项
来源：http://pmp.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://orx.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://xip.9152youxi.cn

time ./run.sh
来源：http://bzz.tarul.cn

================================================================================
来源：http://zcq.c1oappe.top

S. C / C++ 专题
来源：http://npw.daria6918.cn

================================================================================
来源：http://wyo.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://eal.sufxvd.cn

#include <stdio.h>
来源：http://yqq.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gaz.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://puh.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://jxj.yuanzhike.top

[S03] C：读入整数
来源：http://jps.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://yls.zdbjq.cn

[S04] C：字符串复制
来源：http://avu.nanxinkj.top

char dst[32]; strcpy(dst, "hi");
来源：http://wcc.hongshengwenyu.top

[S05] C：字符串长度
来源：http://ksn.daria6918.cn

strlen(s)
来源：http://elc.fehbvm.com

[S06] C：字符串比较
来源：http://akj.zhongyouzk.top

strcmp(a, b) == 0
来源：http://sqf.dashuyun.cn

[S07] C：数组遍历求和
来源：http://sok.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://spi.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://nzo.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uqz.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://wbk.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gcu.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://vdp.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://rur.daria6918.cn

[S11] C：逐行读文件
来源：http://xcu.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://wlc.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vgi.jyoumei.cn

fclose(f);
来源：http://avg.jinqigfzy.top

[S12] C：写文件
来源：http://sdc.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://czn.iojbl.cn

[S13] C：宏定义
来源：http://ttd.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fvv.shanyushiyangtech.top

[S14] C：枚举
来源：http://pdl.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://rly.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://wpy.fzhhl.top

(double) a / b
来源：http://kjz.pycfn.com

[S16] C：位操作置位
来源：http://cpb.dianchejie.cn

x |= (1 << 3);
来源：http://vfw.shuidangran.top

[S17] C：安全拼接字符串
来源：http://cbt.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://onf.jqgfzy.top

[S18] C：命令行参数
来源：http://lez.fktsv.cn

int main(int argc, char **argv)
来源：http://plx.jinqigfzy.top

[S19] C：快速排序
来源：http://epb.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ukb.jiagoushi.top

[S20] C：二分查找
来源：http://nnq.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xba.sufxvd.cn

[S21] C：字符类别判断
来源：http://zwe.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dci.gotoacloud.top

[S22] C：字符串转数字
来源：http://kal.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ezn.hysaishi.cn

[S23] C：随机数
来源：http://nyp.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://twj.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://drg.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uvj.xziqi.cn

[S25] C：内存拷贝
来源：http://jfv.cheryme.top

memcpy(dst, src, n);
来源：http://vro.tianlin.xyz

[S26] C：内存清零
来源：http://fld.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://ozg.bjfxy.top

[S27] C：定义常量
来源：http://ilk.hysaishi.cn

const double PI = 3.14159;
来源：http://puu.jiagoushi.top

[S28] C：静态变量
来源：http://iij.meibo888.top

static int counter = 0;
来源：http://kgv.zhongyouzk.top

[S29] C：变参函数
来源：http://hal.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rga.yangfankeji.com

[S30] C：头文件保护
来源：http://nvn.gotoacloud.top

#ifndef X_H
来源：http://bci.gotoacloud.top

#define X_H
来源：http://knc.jqgfzy.top

#endif
来源：http://uyd.gogol.net.cn

[S31] C++：Hello World
来源：http://ajo.snrcjt.cn

#include <iostream>
来源：http://joz.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://zmd.52xcode.cn

[S32] C++：字符串
来源：http://cju.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://twh.52xcode.cn

[S33] C++：vector 增删
来源：http://mbz.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cws.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://bfj.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://hkc.zhiwuduotai.top

[S35] C++：map
来源：http://jvb.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mzj.guannengcc.top

[S36] C++：unordered_map
来源：http://wfu.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fxq.quarkkingdee.top

[S37] C++：set
来源：http://fjh.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bjk.jinyuanbaomall.cn

[S38] C++：排序
来源：http://ich.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://udh.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://pyp.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kav.xuanzx.com

[S40] C++：查找元素
来源：http://zuj.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hfr.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://mlf.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ips.havefunace.top

[S42] C++：继承与虚函数
来源：http://xww.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://dau.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://eyt.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://ozq.dashuyun.cn

[S44] C++：引用传参
来源：http://tur.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://xll.hongshengwenyu.top

[S45] C++：lambda
来源：http://jxh.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://jxl.cheryme.top

[S46] C++：函数模板
来源：http://iaa.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ove.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://mcd.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ijv.yj20258.top

[S48] C++：逐行读文件
来源：http://lok.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qmq.xuanzx.com

while (std::getline(in, line)) { }
来源：http://xqf.birdmap.top

[S49] C++：写文件
来源：http://zja.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nfr.zycfv.cn

[S50] C++：格式化数字
来源：http://ltf.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mbh.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://sik.cashguo.top

static_cast<double>(a) / b
来源：http://maw.yongpay.top

[S52] C++：const 与 noexcept
来源：http://cxi.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://nkj.wangshuangyany.cn

[S53] C++：移动语义
来源：http://udq.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://dvq.52xcode.cn

[S54] C++：异常处理
来源：http://ekx.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fxm.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://foc.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://alf.havefunace.top

[S56] C++：optional
来源：http://tyf.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ivs.cdnleiting.top

[S57] C++：编译期常量
来源：http://grt.gogol.net.cn

constexpr int N = 10;
来源：http://oal.ydzc1.top

[S58] C++：命名空间
来源：http://zlq.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://ddj.nanxinkj.top

[S59] C++：静态断言
来源：http://cgi.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dje.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://tsk.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ssc.hfpthk.cn

================================================================================
来源：http://xhu.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zia.quarkkingdee.top

================================================================================
来源：http://dsw.zycfv.cn

[T01] Kotlin：Hello World
来源：http://sqt.vehdjk.com

println("Hello")
来源：http://wbe.jinqigufen.top

[T02] Kotlin：变量
来源：http://jeq.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wqg.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://lef.zdbjq.cn

"值: $b"
来源：http://fdg.uphjek.com

[T04] Kotlin：空安全
来源：http://rbo.gzhubu.top

val n: String? = null;  n?.length
来源：http://gbz.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://cah.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kxg.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://vib.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zma.yj202588.top

[T07] Kotlin：集合过滤
来源：http://fjq.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jyi.zycfv.cn

[T08] Kotlin：数据类
来源：http://dfu.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://kuh.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://ava.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://hhd.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://snv.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zpd.ivvv.top

[T11] Kotlin：协程
来源：http://xph.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://dxr.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://amn.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://nvj.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://jsx.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://kzs.yongpay.top

[T14] Kotlin：循环
来源：http://czz.hysaishi.cn

for (i in 1..10) println(i)
来源：http://anm.xziqi.cn

[T15] Kotlin：接口
来源：http://aio.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://mig.yongpay.top

[T16] Swift：Hello World
来源：http://cuu.zhixingplan.top

print("Hello")
来源：http://lxq.ctjpmb.com

[T17] Swift：变量与常量
来源：http://cia.yj20258888.top

var a = 1;  let b = 2
来源：http://kdz.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://iec.yfazqb.com

"值: \(b)"
来源：http://yaz.uphjek.com

[T19] Swift：可选绑定
来源：http://tim.kuanghao11.cn

if let n = opt { print(n) }
来源：http://ela.hywenlv.cn

[T20] Swift：数组操作
来源：http://stv.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://baj.yuanzhike.top

[T21] Swift：遍历
来源：http://lfa.xinyue.icu

for x in a { print(x) }
来源：http://uly.havefunace.top

[T22] Swift：字典
来源：http://eko.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zrq.andypj.xyz

[T23] Swift：函数
来源：http://hpe.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zyt.hywenlv.cn

[T24] Swift：闭包
来源：http://bsj.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://lik.yonumen.top

[T25] Swift：结构体
来源：http://zim.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://swi.fehbvm.com

[T26] Swift：类与重写
来源：http://gao.cqqwz.cn

class A: Base { override func f() {} }
来源：http://fof.yanxiufei.cn

[T27] Swift：错误处理
来源：http://eqa.sweek.top

do { try f() } catch { print(error) }
来源：http://qxj.jinqigufen.top

[T28] Swift：枚举
来源：http://azf.fktsv.cn

enum Color { case red, green }
来源：http://eqg.pycfn.com

[T29] Swift：guard 提前返回
来源：http://hje.cashguo.top

guard let x = opt else { return }
来源：http://mna.316326.xyz

[T30] Swift：协议
来源：http://blp.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://kuu.jianghu66.top

[T31] Lua：Hello World
来源：http://vbq.yonumen.top

print("Hello")
来源：http://woc.tianlin.xyz

[T32] Lua：局部变量
来源：http://juk.ydzc1.top

local a = 1
来源：http://nfq.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://xry.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://djs.ctjpmb.com

[T34] Lua：遍历表
来源：http://rea.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fbj.snrcjt.cn

[T35] Lua：字典表
来源：http://sxt.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://yuc.jinqigfzy.top

[T36] Lua：函数
来源：http://jti.yj202588.top

function add(a, b) return a + b end
来源：http://xjg.smart0.xyz

[T37] Lua：字符串拼接
来源：http://zld.hnqzz.top

"a" .. "b"
来源：http://txe.52xcode.cn

[T38] Lua：条件
来源：http://qmb.gotoacloud.top

if x > 0 then print("正") end
来源：http://hyi.jqgfzy.top

[T39] Lua：模式匹配
来源：http://oti.sufxvd.cn

string.find(s, "%d+")
来源：http://hpp.jiagoushi.top

[T40] Lua：元表
来源：http://vlq.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://qsf.9152youxi.cn

[T41] Perl：Hello World
来源：http://wsp.wangdashe.top

print "Hello\n";
来源：http://ded.andypj.xyz

[T42] Perl：变量类型
来源：http://bsg.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bdk.shzxlz.cn

[T43] Perl：字符串插值
来源：http://brj.cucudq.cn

"值: $a"
来源：http://nnn.uphjek.com

[T44] Perl：条件
来源：http://gob.yonumen.top

if ($a > 0) { print "正"; }
来源：http://tzq.iojbl.cn

[T45] Perl：数组遍历
来源：http://wgc.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://heb.hnqzz.top

[T46] Perl：哈希操作
来源：http://pys.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tsi.nwbrower.top


<!-- 参考信息 -->