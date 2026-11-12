代发 wailian999

files=$(ls -1)
来源：http://yhh.zhaomingkeji.xyz

[R38] 管道串联
来源：http://qzf.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://ivd.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://brw.sweek.top

cmd > out.log 2>&1
来源：http://pdp.uphjek.com

[R40] 追加写日志
来源：http://qnf.daria6918.cn

echo "log" >> out.log
来源：http://nae.sxryk.cn

[R41] 丢弃输出
来源：http://aic.xuanzx.com

cmd >/dev/null 2>&1
来源：http://uiv.yvedp.cn

[R42] 输入重定向
来源：http://aul.hcnkem.com

wc -l < a.txt
来源：http://mjg.birdmap.top

[R43] 按名字查找文件
来源：http://qjv.vehdjk.com

find . -name "*.log" -type f
来源：http://ike.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://doy.andypj.xyz

find . -mtime -7 -type f
来源：http://qwd.snrcjt.cn

[R45] 批量删除
来源：http://utm.daria6918.cn

find . -name "*.tmp" -delete
来源：http://iui.hfpthk.cn

[R46] 递归替换文件内容
来源：http://bif.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xau.ydzc1.top

[R47] sed 单行替换
来源：http://swh.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ifr.snrcjt.cn

[R48] awk 取指定列
来源：http://dkt.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://brb.andypj.xyz

[R49] awk 带条件
来源：http://ysb.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yix.yuxming.cn

[R50] awk 求和
来源：http://qmo.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vkl.zhongyouzk.top

[R51] 排序去重取前几
来源：http://brp.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lhd.ivvv.top

[R52] 统计行数
来源：http://azn.cashguo.top

wc -l a.txt
来源：http://itr.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://zlg.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qls.yueranfly.top

[R54] 比较两个文件
来源：http://hzg.jqgfzy.top

diff a.txt b.txt
来源：http://exj.cheryme.top

[R55] 压缩与解压
来源：http://ulj.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xyq.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://vpz.sysykeji.top

scp file user@host:/path/
来源：http://rxq.zhongyouzk.top

[R57] 远程执行命令
来源：http://utx.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://oic.9152youxi.cn

[R58] 下载文件
来源：http://grd.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyj.cdnleiting.top

[R59] 发 POST JSON
来源：http://utv.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nwh.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://ofe.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zti.aibaodan.cn

[R61] 磁盘占用
来源：http://yqt.zycfv.cn

df -h;  du -sh *
来源：http://jrk.yongpay.top

[R62] 找最占空间的文件
来源：http://xrn.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://jmp.yuxming.cn

[R63] 内存与进程
来源：http://bvq.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://phk.tianlin.xyz

[R64] 结束进程
来源：http://cie.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://oce.yuanzhike.top

[R65] 查看端口占用
来源：http://lfo.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gvp.guowangkeji.top

[R66] 定时任务
来源：http://slk.sjlbkw.cn

crontab -e;  crontab -l
来源：http://xhj.fehbvm.com

[R67] 生成随机十六进制串
来源：http://elt.hongshengwenyu.top

openssl rand -hex 16
来源：http://oqa.cdnleiting.top

[R68] 计算文件校验值
来源：http://fkh.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://viu.yj202588.top

[R69] 生成随机密码
来源：http://fbs.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://pmw.fktsv.cn

[R70] 时间戳与互转
来源：http://znn.xinyue.icu

date +%s;  date -d @1700000000
来源：http://jru.smart0.xyz

[R71] 日期格式化
来源：http://nua.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://poc.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://evj.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mut.nwbrower.top

[R73] 分割大日志
来源：http://jqf.zycfv.cn

split -l 1000 big.log part_
来源：http://ora.yanxiufei.cn

[R74] 批量重命名
来源：http://pxz.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wvi.bbcook.cn

[R75] 导出环境变量
来源：http://wmk.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://jcz.nanxinkj.top

[R76] 使用临时文件
来源：http://lyc.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vtg.yanxiufei.cn

[R77] 读取用户输入
来源：http://dfo.ppjwa.cn

read -rp "请输入: " ans
来源：http://ion.tian-w.cn

[R78] 交互式菜单
来源：http://nlh.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lsb.sxryk.cn

[R79] 解析命令行选项
来源：http://aol.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nsl.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://bct.nanxinkj.top

time ./run.sh
来源：http://zwg.jinqigufen.top

================================================================================
来源：http://ufj.epnwcf.com

S. C / C++ 专题
来源：http://ugo.havefunace.top

================================================================================
来源：http://fog.cashguo.top

[S01] C：Hello World
来源：http://egf.yueranfly.top

#include <stdio.h>
来源：http://imp.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://peq.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://rfo.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://qvq.xuetiantiany.cn

[S03] C：读入整数
来源：http://bcu.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://uic.yuxming.cn

[S04] C：字符串复制
来源：http://dmz.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://alr.tian-w.cn

[S05] C：字符串长度
来源：http://mgk.pycfn.com

strlen(s)
来源：http://obg.aibaodan.cn

[S06] C：字符串比较
来源：http://bmx.gzhubu.top

strcmp(a, b) == 0
来源：http://syj.yuxming.cn

[S07] C：数组遍历求和
来源：http://zyf.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kai.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://gjl.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jor.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://bup.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eai.fehbvm.com

[S10] C：指针与解引用
来源：http://kmd.xylfe.cn

int *p = &a;  *p = 5;
来源：http://xuh.havefunace.top

[S11] C：逐行读文件
来源：http://ttl.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://cfm.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eff.yonumen.top

fclose(f);
来源：http://uhg.bbcook.cn

[S12] C：写文件
来源：http://zax.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://roq.ybcxt.top

[S13] C：宏定义
来源：http://zcg.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bkp.nanxinkj.top

[S14] C：枚举
来源：http://xkh.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://aou.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://kwo.ehwqpu.com

(double) a / b
来源：http://qcb.zhongyouzk.top

[S16] C：位操作置位
来源：http://jho.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://uih.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://qbc.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zjr.daxiang520.top

[S18] C：命令行参数
来源：http://ylq.c1oappe.top

int main(int argc, char **argv)
来源：http://zim.ybcxt.top

[S19] C：快速排序
来源：http://ygi.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://isg.wangdashe.top

[S20] C：二分查找
来源：http://aow.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ugl.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://vip.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://npy.hysaishi.cn

[S22] C：字符串转数字
来源：http://vrw.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://bgw.hfpthk.cn

[S23] C：随机数
来源：http://cyx.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://erw.meibo888.top

[S24] C：获取本地时间
来源：http://dui.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ltr.vehdjk.com

[S25] C：内存拷贝
来源：http://buk.cqqwz.cn

memcpy(dst, src, n);
来源：http://rhd.ehwqpu.com

[S26] C：内存清零
来源：http://lvp.jianghu66.top

memset(a, 0, sizeof a);
来源：http://akz.c1oappe.top

[S27] C：定义常量
来源：http://ywi.smart0.xyz

const double PI = 3.14159;
来源：http://cvw.cheryme.top

[S28] C：静态变量
来源：http://arc.sysykeji.top

static int counter = 0;
来源：http://isj.ydjk.org.cn

[S29] C：变参函数
来源：http://ahc.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://afi.hcnkem.com

[S30] C：头文件保护
来源：http://jjq.xingfuxueyuan.xyz

#ifndef X_H
来源：http://bcd.birdmap.top

#define X_H
来源：http://pfu.chenjidiqi.icu

#endif
来源：http://rpd.snrcjt.cn

[S31] C++：Hello World
来源：http://umy.bjfxy.top

#include <iostream>
来源：http://uxz.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://tav.hongshengwenyu.top

[S32] C++：字符串
来源：http://pmg.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://jyt.sxryk.cn

[S33] C++：vector 增删
来源：http://udd.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ozr.c1oappe.top

[S34] C++：遍历 vector
来源：http://sdy.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://boo.gogol.net.cn

[S35] C++：map
来源：http://zen.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wkg.sxryk.cn

[S36] C++：unordered_map
来源：http://vvi.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gdr.316326.xyz

[S37] C++：set
来源：http://lkl.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jjf.jiagoushi.top

[S38] C++：排序
来源：http://ofo.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://jgy.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://dxu.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://toq.meibo888.top

[S40] C++：查找元素
来源：http://mui.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bxb.9152youxi.cn

[S41] C++：类与构造函数
来源：http://txw.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xnz.cucudq.cn

[S42] C++：继承与虚函数
来源：http://ijk.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://tnc.ehwqpu.com

[S43] C++：智能指针
来源：http://ezt.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://cdv.chenzaomai.com

[S44] C++：引用传参
来源：http://jgr.c1oappe.top

void inc(int &x) { ++x; }
来源：http://ulg.vehdjk.com

[S45] C++：lambda
来源：http://zsr.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://tmv.feifeiyinyue.top

[S46] C++：函数模板
来源：http://wom.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zxw.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://rxh.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://apg.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://rxy.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://ydq.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ayx.birdmap.top

[S49] C++：写文件
来源：http://aiu.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yiz.jiagoushi.top

[S50] C++：格式化数字
来源：http://piy.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qbz.jqgfzy.top

[S51] C++：显式类型转换
来源：http://hbr.52xcode.cn

static_cast<double>(a) / b
来源：http://kwx.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://uim.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://dbq.zycfv.cn

[S53] C++：移动语义
来源：http://wiw.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://svp.hywenlv.cn

[S54] C++：异常处理
来源：http://pjq.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://knl.gotoacloud.top

[S55] C++：结构化绑定
来源：http://wkt.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://atp.yangfankeji.com

[S56] C++：optional
来源：http://jkq.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qwk.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://vyz.meibo888.top

constexpr int N = 10;
来源：http://sla.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://soe.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://hdc.svipenyu.cn

[S59] C++：静态断言
来源：http://gtn.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xhs.birdmap.top

[S60] C++：遍历并删除元素
来源：http://jct.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xgw.andypj.xyz

================================================================================
来源：http://wyf.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jfb.tarul.cn

================================================================================
来源：http://grs.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://uzm.daxiang520.top

println("Hello")
来源：http://qgr.smart0.xyz

[T02] Kotlin：变量
来源：http://auu.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctj.yonumen.top

[T03] Kotlin：字符串模板
来源：http://hfi.hnqzz.top

"值: $b"
来源：http://xcv.fengsongda.top

[T04] Kotlin：空安全
来源：http://ygw.snrcjt.cn

val n: String? = null;  n?.length
来源：http://spm.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://qax.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xoy.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://iux.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hnb.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://hld.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fwv.yangfankeji.com

[T08] Kotlin：数据类
来源：http://isf.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://cww.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://hjx.pycfn.com

fun String.exclaim() = this + "!"
来源：http://lwn.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://izw.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vdo.hnqzz.top

[T11] Kotlin：协程
来源：http://ukc.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hnu.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://pqy.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://qnk.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://iej.hesvh.cn

val m = mapOf("a" to 1)
来源：http://guz.shzxlz.cn

[T14] Kotlin：循环
来源：http://cmt.dianchejie.cn

for (i in 1..10) println(i)
来源：http://ggk.jqgufenzy.top

[T15] Kotlin：接口
来源：http://byh.meibo888.top

interface Shape { fun area(): Double }
来源：http://hpz.epnwcf.com

[T16] Swift：Hello World
来源：http://nio.shanyushiyangkeji.top

print("Hello")
来源：http://wqh.mhx1999.top

[T17] Swift：变量与常量
来源：http://lvq.yj20258.top

var a = 1;  let b = 2
来源：http://atv.cdnleiting.top

[T18] Swift：字符串插值
来源：http://htq.yuanzhike.top

"值: \(b)"
来源：http://oaz.c1oappe.top

[T19] Swift：可选绑定
来源：http://njw.xinyue.icu

if let n = opt { print(n) }
来源：http://hna.sjlbkw.cn

[T20] Swift：数组操作
来源：http://lkb.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://mpq.havefunace.top

[T21] Swift：遍历
来源：http://lko.yuanzhike.top

for x in a { print(x) }
来源：http://unj.xylfe.cn

[T22] Swift：字典
来源：http://kon.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://tye.ppjwa.cn

[T23] Swift：函数
来源：http://tvz.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://glu.chenzaomai.com

[T24] Swift：闭包
来源：http://mwt.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://gcm.52xcode.cn

[T25] Swift：结构体
来源：http://nfb.zhongyouzk.top

struct P { var x: Int }
来源：http://zlt.yj20258.top

[T26] Swift：类与重写
来源：http://egd.ybcxt.top

class A: Base { override func f() {} }
来源：http://fdl.zdqjudy.top

[T27] Swift：错误处理
来源：http://wcw.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://kew.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://qhy.tarul.cn

enum Color { case red, green }
来源：http://gpb.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://ubf.hnqzz.top

guard let x = opt else { return }
来源：http://xbr.sxryk.cn

[T30] Swift：协议
来源：http://pjl.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://qnw.jqgufenzy.top

[T31] Lua：Hello World
来源：http://jwf.chenlongwang.top

print("Hello")
来源：http://hjw.jyoumei.cn

[T32] Lua：局部变量
来源：http://dse.nanxuanxn.top

local a = 1
来源：http://rre.tanke756.top

[T33] Lua：表（数组）
来源：http://opq.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wei.52xcode.cn

[T34] Lua：遍历表
来源：http://aji.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iob.dianchejie.cn

[T35] Lua：字典表
来源：http://scs.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://hik.jinqigufen.top

[T36] Lua：函数
来源：http://kab.ivvv.top

function add(a, b) return a + b end
来源：http://jjs.gzhubu.top

[T37] Lua：字符串拼接
来源：http://ojj.316326.xyz

"a" .. "b"
来源：http://jwv.andypj.xyz

[T38] Lua：条件
来源：http://wxl.guowangkeji.top

if x > 0 then print("正") end
来源：http://xfj.yfazqb.com

[T39] Lua：模式匹配
来源：http://cqu.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://sgl.shzxlz.cn

[T40] Lua：元表
来源：http://yee.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://eqi.guannengcc.top


<!-- 参考信息 -->