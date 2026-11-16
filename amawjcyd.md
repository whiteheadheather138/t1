代发 wailian999

cmd > out.log 2>&1
来源：http://bql.jqgufenzy.top

[R40] 追加写日志
来源：http://slg.yj202588.top

echo "log" >> out.log
来源：http://lbf.ehwqpu.com

[R41] 丢弃输出
来源：http://dmp.pycfn.com

cmd >/dev/null 2>&1
来源：http://zdc.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://rlh.dashuyun.cn

wc -l < a.txt
来源：http://ozk.xylfe.cn

[R43] 按名字查找文件
来源：http://mdu.ehwqpu.com

find . -name "*.log" -type f
来源：http://kxf.epnwcf.com

[R44] 按修改时间查找
来源：http://pjt.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://ahd.wangshuangyany.cn

[R45] 批量删除
来源：http://yfa.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://wmh.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://hpf.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://shq.ctjpmb.com

[R47] sed 单行替换
来源：http://fap.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://tpu.aizwys.cn

[R48] awk 取指定列
来源：http://lnt.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://vyq.hesvh.cn

[R49] awk 带条件
来源：http://dqg.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ano.ywan-chungtsiang.top

[R50] awk 求和
来源：http://mkf.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://rre.xinyue.icu

[R51] 排序去重取前几
来源：http://zdz.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ldk.yuxming.cn

[R52] 统计行数
来源：http://cms.feifeiyinyue.top

wc -l a.txt
来源：http://wpl.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://wrt.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bvd.quarkkingdee.top

[R54] 比较两个文件
来源：http://qdt.cucudq.cn

diff a.txt b.txt
来源：http://rln.pengpengdd.cyou

[R55] 压缩与解压
来源：http://sgn.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hdx.mhx1999.top

[R56] 远程拷贝
来源：http://xfu.chenzaomai.com

scp file user@host:/path/
来源：http://vba.andypj.xyz

[R57] 远程执行命令
来源：http://mud.cashguo.top

ssh user@host 'uptime'
来源：http://hlf.zhoulong.xyz

[R58] 下载文件
来源：http://qfa.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wvu.ehwqpu.com

[R59] 发 POST JSON
来源：http://tla.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yay.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://ixy.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lxx.dianchejie.cn

[R61] 磁盘占用
来源：http://blj.daxiang520.top

df -h;  du -sh *
来源：http://lgy.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://edp.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://sow.sufxvd.cn

[R63] 内存与进程
来源：http://tfn.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://ods.hfpthk.cn

[R64] 结束进程
来源：http://ggf.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://sfv.fzhhl.top

[R65] 查看端口占用
来源：http://pqf.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cxo.cucudq.cn

[R66] 定时任务
来源：http://kmh.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://veh.fehbvm.com

[R67] 生成随机十六进制串
来源：http://szj.quarkkingdee.top

openssl rand -hex 16
来源：http://cyb.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://qvh.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://vyx.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://qzv.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://fdu.yfazqb.com

[R70] 时间戳与互转
来源：http://vke.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://fqg.yangfankeji.com

[R71] 日期格式化
来源：http://tpa.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://msy.yonumen.top

[R72] 等待端口就绪
来源：http://fqt.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qih.jinqigfzy.top

[R73] 分割大日志
来源：http://dqz.jqgufenzy.top

split -l 1000 big.log part_
来源：http://nve.jianghu66.top

[R74] 批量重命名
来源：http://gdf.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jef.havefunace.top

[R75] 导出环境变量
来源：http://byx.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://pya.feifeiyinyue.top

[R76] 使用临时文件
来源：http://ylp.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dmi.fktsv.cn

[R77] 读取用户输入
来源：http://bki.fehbvm.com

read -rp "请输入: " ans
来源：http://gnd.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://vas.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://mzx.ctjpmb.com

[R79] 解析命令行选项
来源：http://qyx.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://obx.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://itt.daria6918.cn

time ./run.sh
来源：http://ifr.sweek.top

================================================================================
来源：http://pvw.0kj1m.cn

S. C / C++ 专题
来源：http://sxx.jinyuanbaomall.cn

================================================================================
来源：http://exe.daxiang520.top

[S01] C：Hello World
来源：http://sde.dianchejie.cn

#include <stdio.h>
来源：http://stn.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oni.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://dkt.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://fsa.jqgufenzy.top

[S03] C：读入整数
来源：http://efo.ctjpmb.com

int x; scanf("%d", &x);
来源：http://bez.yanxiufei.cn

[S04] C：字符串复制
来源：http://ipc.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://ptz.andypj.xyz

[S05] C：字符串长度
来源：http://ihv.fanxiaobao.xyz

strlen(s)
来源：http://qno.cashguo.top

[S06] C：字符串比较
来源：http://hil.jqgfzy.top

strcmp(a, b) == 0
来源：http://zsr.tarul.cn

[S07] C：数组遍历求和
来源：http://kmn.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nfb.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://een.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dix.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://skl.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tpo.zhongyouzk.top

[S10] C：指针与解引用
来源：http://tid.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://xpa.yangfankeji.com

[S11] C：逐行读文件
来源：http://etp.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://hph.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wzm.yuxming.cn

fclose(f);
来源：http://fsz.52xcode.cn

[S12] C：写文件
来源：http://agj.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dhk.52xcode.cn

[S13] C：宏定义
来源：http://kqr.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ulh.zhoulong.xyz

[S14] C：枚举
来源：http://qaf.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://rrn.yj20258888.top

[S15] C：类型转换
来源：http://oyk.epnwcf.com

(double) a / b
来源：http://mzx.jlsjyb.cn

[S16] C：位操作置位
来源：http://ogi.hcnkem.com

x |= (1 << 3);
来源：http://rur.cucudq.cn

[S17] C：安全拼接字符串
来源：http://ngt.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kvt.xuanzx.com

[S18] C：命令行参数
来源：http://dxm.shuidangran.top

int main(int argc, char **argv)
来源：http://fut.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://pnl.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qcb.ybcxt.top

[S20] C：二分查找
来源：http://dxx.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://elh.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://qde.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qnn.gogol.net.cn

[S22] C：字符串转数字
来源：http://dez.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://vmb.fanxiaobao.xyz

[S23] C：随机数
来源：http://dpe.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eim.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ayd.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dkn.pycfn.com

[S25] C：内存拷贝
来源：http://ghy.fktsv.cn

memcpy(dst, src, n);
来源：http://zja.zycfv.cn

[S26] C：内存清零
来源：http://mre.epnwcf.com

memset(a, 0, sizeof a);
来源：http://xql.ppjwa.cn

[S27] C：定义常量
来源：http://hah.birdmap.top

const double PI = 3.14159;
来源：http://rxh.zhijiandao.cn

[S28] C：静态变量
来源：http://htv.zhengqikj.top

static int counter = 0;
来源：http://pzq.shangyingyoupin.top

[S29] C：变参函数
来源：http://ejo.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rqx.nanxuanxn.top

[S30] C：头文件保护
来源：http://lik.snrcjt.cn

#ifndef X_H
来源：http://poe.svipenyu.cn

#define X_H
来源：http://lht.9152youxi.cn

#endif
来源：http://nkx.yuanzhike.top

[S31] C++：Hello World
来源：http://yjd.dashuyun.cn

#include <iostream>
来源：http://zcm.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://icf.tianlin.xyz

[S32] C++：字符串
来源：http://ork.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://wsh.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://jba.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://shd.xziqi.cn

[S34] C++：遍历 vector
来源：http://kqx.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://pua.guannengcc.top

[S35] C++：map
来源：http://ehg.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xqp.dianchejie.cn

[S36] C++：unordered_map
来源：http://ite.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dxd.hnqzz.top

[S37] C++：set
来源：http://ape.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pck.xuetiantiany.cn

[S38] C++：排序
来源：http://pfj.kuanghao11.cn

std::sort(v.begin(), v.end());
来源：http://fzg.pycfn.com

[S39] C++：自定义比较器排序
来源：http://ret.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://haj.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://hcz.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aec.chenlongwang.top

[S41] C++：类与构造函数
来源：http://joi.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jhe.yongpay.top

[S42] C++：继承与虚函数
来源：http://hwv.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://kpr.ehwqpu.com

[S43] C++：智能指针
来源：http://vww.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://can.316326.xyz

[S44] C++：引用传参
来源：http://eul.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://dex.uphjek.com

[S45] C++：lambda
来源：http://byf.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://ltw.jinqigufen.top

[S46] C++：函数模板
来源：http://jtj.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aib.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://jjl.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cqy.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://zcr.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://gtr.sweek.top

while (std::getline(in, line)) { }
来源：http://aun.kuanghao11.cn

[S49] C++：写文件
来源：http://upk.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nue.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://hxf.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xfm.cqqwz.cn

[S51] C++：显式类型转换
来源：http://nup.sxryk.cn

static_cast<double>(a) / b
来源：http://hxq.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://tzm.shuidangran.top

int size() const noexcept { return n_; }
来源：http://dvg.epnwcf.com

[S53] C++：移动语义
来源：http://edj.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://oui.cucudq.cn

[S54] C++：异常处理
来源：http://kow.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yiu.zhengqikj.top

[S55] C++：结构化绑定
来源：http://jvd.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fcq.fanxiaobao.xyz

[S56] C++：optional
来源：http://aiu.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zfe.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://rsb.sxryk.cn

constexpr int N = 10;
来源：http://cjc.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://kgy.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://lel.zhongyouzk.top

[S59] C++：静态断言
来源：http://hki.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pnm.meibo888.top

[S60] C++：遍历并删除元素
来源：http://etf.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qog.xuanzx.com

================================================================================
来源：http://ngl.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uww.hammf.cn

================================================================================
来源：http://iyg.fktsv.cn

[T01] Kotlin：Hello World
来源：http://ghv.xylfe.cn

println("Hello")
来源：http://shm.yuxming.cn

[T02] Kotlin：变量
来源：http://hbb.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aoc.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://rep.ehwqpu.com

"值: $b"
来源：http://sid.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://fsd.ehwqpu.com

val n: String? = null;  n?.length
来源：http://xha.ivvv.top

[T05] Kotlin：when 表达式
来源：http://sjn.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fje.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://ldj.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aqd.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://pbe.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://exj.zdbjq.cn

[T08] Kotlin：数据类
来源：http://cmq.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://zuo.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://rkl.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://pwf.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://yco.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://gfo.tianlin.xyz

[T11] Kotlin：协程
来源：http://jph.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://aml.jianghu66.top

[T12] Kotlin：解构声明
来源：http://gxe.sweek.top

val (a, b) = Pair(1, 2)
来源：http://fno.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://rtn.fzhhl.top

val m = mapOf("a" to 1)
来源：http://uoq.yfazqb.com

[T14] Kotlin：循环
来源：http://wff.aizwys.cn

for (i in 1..10) println(i)
来源：http://ssq.cucudq.cn

[T15] Kotlin：接口
来源：http://jfb.c1oappe.top

interface Shape { fun area(): Double }
来源：http://pno.ydzc1.top

[T16] Swift：Hello World
来源：http://lbr.sufxvd.cn

print("Hello")
来源：http://nnd.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://zwb.daria6918.cn

var a = 1;  let b = 2
来源：http://rga.fengsongda.top

[T18] Swift：字符串插值
来源：http://blm.zhongyouzk.top

"值: \(b)"
来源：http://xqp.hywenlv.cn

[T19] Swift：可选绑定
来源：http://yhr.fktsv.cn

if let n = opt { print(n) }
来源：http://lez.sufxvd.cn

[T20] Swift：数组操作
来源：http://tap.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://ifz.9152youxi.cn

[T21] Swift：遍历
来源：http://ucj.vehdjk.com

for x in a { print(x) }
来源：http://ayt.epnwcf.com

[T22] Swift：字典
来源：http://gra.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://wpf.zycfv.cn

[T23] Swift：函数
来源：http://ssh.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://afw.bbcook.cn

[T24] Swift：闭包
来源：http://tsz.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://mbo.yueranfly.top

[T25] Swift：结构体
来源：http://odx.shanyushiyangtech.top

struct P { var x: Int }
来源：http://wja.kuanghao11.cn

[T26] Swift：类与重写
来源：http://ipp.yvedp.cn

class A: Base { override func f() {} }
来源：http://lje.sufxvd.cn

[T27] Swift：错误处理
来源：http://kyu.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://npo.chenzaomai.com

[T28] Swift：枚举
来源：http://sav.nwbrower.top

enum Color { case red, green }
来源：http://mat.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://acv.cashguo.top

guard let x = opt else { return }
来源：http://ifs.fktsv.cn

[T30] Swift：协议
来源：http://drz.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://gts.hesvh.cn

[T31] Lua：Hello World
来源：http://ddz.daxiang520.top

print("Hello")
来源：http://ofg.zhengqikj.top

[T32] Lua：局部变量
来源：http://iie.yj202588.top

local a = 1
来源：http://jso.9152youxi.cn

[T33] Lua：表（数组）
来源：http://fdc.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vlg.bjfxy.top

[T34] Lua：遍历表
来源：http://nmn.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oic.andypj.xyz

[T35] Lua：字典表
来源：http://zif.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://eci.tarul.cn

[T36] Lua：函数
来源：http://iah.meibo888.top

function add(a, b) return a + b end
来源：http://seh.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://ala.jinqigfzy.top

"a" .. "b"
来源：http://fep.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://dkf.havefunace.top

if x > 0 then print("正") end
来源：http://cyj.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://mww.wangshuangyany.cn

string.find(s, "%d+")
来源：http://uni.ehwqpu.com

[T40] Lua：元表
来源：http://evo.guannengcc.top

setmetatable({}, { __index = base })
来源：http://ioo.zhoulong.xyz

[T41] Perl：Hello World
来源：http://rzn.cashguo.top

print "Hello\n";
来源：http://ckd.yuxming.cn

[T42] Perl：变量类型
来源：http://hth.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mqq.guowangkeji.top


<!-- 参考信息 -->