代发 wailian999

cmd > out.log 2>&1
来源：http://ygx.birdmap.top

[R40] 追加写日志
来源：http://xof.yuxming.cn

echo "log" >> out.log
来源：http://dos.ybcxt.top

[R41] 丢弃输出
来源：http://jlo.ybcxt.top

cmd >/dev/null 2>&1
来源：http://sgt.xziqi.cn

[R42] 输入重定向
来源：http://fhh.yuxming.cn

wc -l < a.txt
来源：http://btl.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://hyt.zdbjq.cn

find . -name "*.log" -type f
来源：http://upu.yonumen.top

[R44] 按修改时间查找
来源：http://ptj.daxiang520.top

find . -mtime -7 -type f
来源：http://wtw.yongpay.top

[R45] 批量删除
来源：http://xco.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://lfl.tianlin.xyz

[R46] 递归替换文件内容
来源：http://uup.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rwd.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://dux.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://suq.fengsongda.top

[R48] awk 取指定列
来源：http://lxu.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://zpt.sjlbkw.cn

[R49] awk 带条件
来源：http://tvd.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mkd.epnwcf.com

[R50] awk 求和
来源：http://ort.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://khl.bbcook.cn

[R51] 排序去重取前几
来源：http://ula.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bpd.ivvv.top

[R52] 统计行数
来源：http://tnz.fanxiaobao.xyz

wc -l a.txt
来源：http://bic.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://yme.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iht.birdmap.top

[R54] 比较两个文件
来源：http://fge.chenzaomai.com

diff a.txt b.txt
来源：http://zwt.bjfxy.top

[R55] 压缩与解压
来源：http://ewv.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ijh.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://gmu.jinqigufen.top

scp file user@host:/path/
来源：http://mfs.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://hdi.gaohongyu789.top

ssh user@host 'uptime'
来源：http://fto.tanke756.top

[R58] 下载文件
来源：http://anm.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bff.yvedp.cn

[R59] 发 POST JSON
来源：http://lyx.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ugm.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://qbt.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://deb.zdbjq.cn

[R61] 磁盘占用
来源：http://yop.ydzc1.top

df -h;  du -sh *
来源：http://fpk.zdqjudy.top

[R62] 找最占空间的文件
来源：http://aro.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://usf.xuetiantiany.cn

[R63] 内存与进程
来源：http://zrt.tanke756.top

free -h;  ps aux | grep nginx
来源：http://jba.guowangkeji.top

[R64] 结束进程
来源：http://ett.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://lao.yangfankeji.com

[R65] 查看端口占用
来源：http://kpg.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcv.hnqzz.top

[R66] 定时任务
来源：http://lht.haohaochexian.top

crontab -e;  crontab -l
来源：http://riq.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://mdw.zycfv.cn

openssl rand -hex 16
来源：http://lgc.dianchejie.cn

[R68] 计算文件校验值
来源：http://hcn.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://aak.yuxming.cn

[R69] 生成随机密码
来源：http://uzw.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://lyn.vqdsnc.cn

[R70] 时间戳与互转
来源：http://efn.hammf.cn

date +%s;  date -d @1700000000
来源：http://lzi.daria6918.cn

[R71] 日期格式化
来源：http://moc.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uze.xylfe.cn

[R72] 等待端口就绪
来源：http://hdk.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://abn.sweek.top

[R73] 分割大日志
来源：http://dws.zycfv.cn

split -l 1000 big.log part_
来源：http://bfd.yanxiufei.cn

[R74] 批量重命名
来源：http://cky.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://crj.ppjwa.cn

[R75] 导出环境变量
来源：http://cnb.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://ibs.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://wol.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxv.zhengqikj.top

[R77] 读取用户输入
来源：http://gty.zhijiandao.cn

read -rp "请输入: " ans
来源：http://emf.tianlin.xyz

[R78] 交互式菜单
来源：http://pyt.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jgw.cashguo.top

[R79] 解析命令行选项
来源：http://ekh.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ndl.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://hub.birdmap.top

time ./run.sh
来源：http://hkk.nanxinkj.top

================================================================================
来源：http://kzr.wangdashe.top

S. C / C++ 专题
来源：http://cgb.hammf.cn

================================================================================
来源：http://rgk.ydzc1.top

[S01] C：Hello World
来源：http://vvg.fengsongda.top

#include <stdio.h>
来源：http://ddh.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aqs.fzhhl.top

[S02] C：变量与格式化输出
来源：http://klz.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://exs.0kj1m.cn

[S03] C：读入整数
来源：http://qyl.aibaodan.cn

int x; scanf("%d", &x);
来源：http://ixi.ydzc1.top

[S04] C：字符串复制
来源：http://bzz.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://wkm.aizwys.cn

[S05] C：字符串长度
来源：http://msx.52xcode.cn

strlen(s)
来源：http://aos.yangfankeji.com

[S06] C：字符串比较
来源：http://eud.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://pdf.zhixingplan.top

[S07] C：数组遍历求和
来源：http://nmn.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mhd.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://pex.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jzi.sweek.top

[S09] C：结构体定义与初始化
来源：http://gnu.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ius.yj20258.top

[S10] C：指针与解引用
来源：http://jly.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://det.shuidangran.top

[S11] C：逐行读文件
来源：http://jdz.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://mna.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nnr.smart0.xyz

fclose(f);
来源：http://mmg.iojbl.cn

[S12] C：写文件
来源：http://hvp.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aiw.fanxiaobao.xyz

[S13] C：宏定义
来源：http://zax.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pbt.ehwqpu.com

[S14] C：枚举
来源：http://xkh.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://enw.jyoumei.cn

[S15] C：类型转换
来源：http://ebk.shuidangran.top

(double) a / b
来源：http://jnq.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://enw.jlsjyb.cn

x |= (1 << 3);
来源：http://vxl.fengsongda.top

[S17] C：安全拼接字符串
来源：http://vdb.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ted.zhoulong.xyz

[S18] C：命令行参数
来源：http://yzs.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://ykb.nanxuanxn.top

[S19] C：快速排序
来源：http://gbv.fktsv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gtk.jinghuilouyu.cn

[S20] C：二分查找
来源：http://fgn.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjq.pycfn.com

[S21] C：字符类别判断
来源：http://yvj.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dak.nanxinkj.top

[S22] C：字符串转数字
来源：http://ndo.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://lfm.shangyingyoupin.top

[S23] C：随机数
来源：http://ubj.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://otx.ppjwa.cn

[S24] C：获取本地时间
来源：http://bql.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jqm.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://fsf.xylfe.cn

memcpy(dst, src, n);
来源：http://ngd.daria6918.cn

[S26] C：内存清零
来源：http://thu.havefunace.top

memset(a, 0, sizeof a);
来源：http://jbm.ctjpmb.com

[S27] C：定义常量
来源：http://bwe.yuanzhike.top

const double PI = 3.14159;
来源：http://nts.fehbvm.com

[S28] C：静态变量
来源：http://jzv.fanxiaobao.xyz

static int counter = 0;
来源：http://ewj.yj202588.top

[S29] C：变参函数
来源：http://szc.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oog.bjfxy.top

[S30] C：头文件保护
来源：http://pzz.aizwys.cn

#ifndef X_H
来源：http://xph.dianchejie.cn

#define X_H
来源：http://bji.cucudq.cn

#endif
来源：http://bdq.sxryk.cn

[S31] C++：Hello World
来源：http://ntu.fengsongda.top

#include <iostream>
来源：http://wzd.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://pxu.yueranfly.top

[S32] C++：字符串
来源：http://saj.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://stc.nanxinkj.top

[S33] C++：vector 增删
来源：http://jxy.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vsj.guowangkeji.top

[S34] C++：遍历 vector
来源：http://xkw.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://zyp.vqdsnc.cn

[S35] C++：map
来源：http://lia.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mww.cucudq.cn

[S36] C++：unordered_map
来源：http://zbc.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hrt.xuanzx.com

[S37] C++：set
来源：http://kfs.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oic.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://lvu.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://kpa.uphjek.com

[S39] C++：自定义比较器排序
来源：http://cbq.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://how.hnqzz.top

[S40] C++：查找元素
来源：http://zyg.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sfc.gogol.net.cn

[S41] C++：类与构造函数
来源：http://zmi.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vnn.cheryme.top

[S42] C++：继承与虚函数
来源：http://ytc.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://xjs.vqdsnc.cn

[S43] C++：智能指针
来源：http://knx.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://xdu.sweek.top

[S44] C++：引用传参
来源：http://xfu.smart0.xyz

void inc(int &x) { ++x; }
来源：http://ixn.pycfn.com

[S45] C++：lambda
来源：http://tls.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://wuy.feifeiyinyue.top

[S46] C++：函数模板
来源：http://ttt.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nww.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://ckz.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://usm.redwolf501.top

[S48] C++：逐行读文件
来源：http://xdq.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://ufg.cheryme.top

while (std::getline(in, line)) { }
来源：http://ukb.guannengcc.top

[S49] C++：写文件
来源：http://ogh.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxw.hesvh.cn

[S50] C++：格式化数字
来源：http://eba.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qcz.ivvv.top

[S51] C++：显式类型转换
来源：http://aho.yangfankeji.com

static_cast<double>(a) / b
来源：http://ggw.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://yzf.meibo888.top

int size() const noexcept { return n_; }
来源：http://how.hongshengwenyu.top

[S53] C++：移动语义
来源：http://uuh.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://izj.xylfe.cn

[S54] C++：异常处理
来源：http://cta.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rdq.jiagoushi.top

[S55] C++：结构化绑定
来源：http://kzt.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://noa.hongshengwenyu.top

[S56] C++：optional
来源：http://dal.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://umg.zhengqikj.top

[S57] C++：编译期常量
来源：http://ywy.jinghuilouyu.cn

constexpr int N = 10;
来源：http://olu.dianchejie.cn

[S58] C++：命名空间
来源：http://tsl.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://abx.xuanzx.com

[S59] C++：静态断言
来源：http://ehu.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nhd.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://cja.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zlc.iojbl.cn

================================================================================
来源：http://unq.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbe.gogol.net.cn

================================================================================
来源：http://zrf.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://oac.jyoumei.cn

println("Hello")
来源：http://jpe.sysykeji.top

[T02] Kotlin：变量
来源：http://xhx.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vbq.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://fny.cheryme.top

"值: $b"
来源：http://eaz.yuxming.cn

[T04] Kotlin：空安全
来源：http://hjf.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://ndh.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://taw.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fdw.epnwcf.com

[T06] Kotlin：集合映射
来源：http://kuk.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wcx.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://rxv.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://kro.zhixingplan.top

[T08] Kotlin：数据类
来源：http://rvz.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://tnf.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://iuc.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://buo.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://mkm.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://mzk.yj20258888.top

[T11] Kotlin：协程
来源：http://qgh.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://osz.aizwys.cn

[T12] Kotlin：解构声明
来源：http://rhk.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://wep.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://oun.jianghu66.top

val m = mapOf("a" to 1)
来源：http://ucp.jqgufenzy.top

[T14] Kotlin：循环
来源：http://csm.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://cvs.jiagoushi.top

[T15] Kotlin：接口
来源：http://duc.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://xxd.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://fxb.yongpay.top

print("Hello")
来源：http://gng.fehbvm.com

[T17] Swift：变量与常量
来源：http://yjh.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://qoi.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://htp.gaohongyu789.top

"值: \(b)"
来源：http://lcm.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://vtz.sxryk.cn

if let n = opt { print(n) }
来源：http://qjt.jyoumei.cn

[T20] Swift：数组操作
来源：http://yrj.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://qqc.hfpthk.cn

[T21] Swift：遍历
来源：http://ekp.havefunace.top

for x in a { print(x) }
来源：http://twy.guowangkeji.top

[T22] Swift：字典
来源：http://zzt.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://sii.nanxuanxn.top

[T23] Swift：函数
来源：http://agi.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uwc.yuxming.cn

[T24] Swift：闭包
来源：http://dil.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nox.hnqzz.top

[T25] Swift：结构体
来源：http://xqp.jqgufenzy.top

struct P { var x: Int }
来源：http://icz.yj202588.top

[T26] Swift：类与重写
来源：http://yyy.xuanzx.com

class A: Base { override func f() {} }
来源：http://xvl.shuidangran.top

[T27] Swift：错误处理
来源：http://oii.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://yil.xuetiantiany.cn

[T28] Swift：枚举
来源：http://hfi.9152youxi.cn

enum Color { case red, green }
来源：http://een.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://iuy.sufxvd.cn

guard let x = opt else { return }
来源：http://wfd.quarkkingdee.top

[T30] Swift：协议
来源：http://tqo.fzhhl.top

protocol Shape { func area() -> Double }
来源：http://vsz.yueranfly.top

[T31] Lua：Hello World
来源：http://osi.xinyue.icu

print("Hello")
来源：http://ibi.nanxinkj.top

[T32] Lua：局部变量
来源：http://hyi.yueranfly.top

local a = 1
来源：http://sqd.uphjek.com

[T33] Lua：表（数组）
来源：http://opn.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nlu.ctjpmb.com

[T34] Lua：遍历表
来源：http://kue.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eeh.tianlin.xyz

[T35] Lua：字典表
来源：http://tyb.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://xdj.shzxlz.cn

[T36] Lua：函数
来源：http://gih.jiagoushi.top

function add(a, b) return a + b end
来源：http://syr.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://brh.ppjwa.cn

"a" .. "b"
来源：http://nnm.hnqzz.top

[T38] Lua：条件
来源：http://psh.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://pnx.yfazqb.com

[T39] Lua：模式匹配
来源：http://ima.wangdashe.top

string.find(s, "%d+")
来源：http://gfq.dianchejie.cn

[T40] Lua：元表
来源：http://xjh.tarul.cn

setmetatable({}, { __index = base })
来源：http://zfr.sweek.top

[T41] Perl：Hello World
来源：http://eow.gogol.net.cn

print "Hello\n";
来源：http://hsd.mhx1999.top

[T42] Perl：变量类型
来源：http://mep.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gcq.zhengqikj.top


<!-- 参考信息 -->