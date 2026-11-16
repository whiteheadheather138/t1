代发 wailian999

cmd > out.log 2>&1
来源：http://zvu.jyoumei.cn

[R40] 追加写日志
来源：http://das.shuidangran.top

echo "log" >> out.log
来源：http://nxz.cdnleiting.top

[R41] 丢弃输出
来源：http://ina.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://zym.ppjwa.cn

[R42] 输入重定向
来源：http://tmf.hongshengwenyu.top

wc -l < a.txt
来源：http://zkt.ivvv.top

[R43] 按名字查找文件
来源：http://hhk.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://bqi.gzhubu.top

[R44] 按修改时间查找
来源：http://pzq.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://vty.ctjpmb.com

[R45] 批量删除
来源：http://jlm.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://hgi.fehbvm.com

[R46] 递归替换文件内容
来源：http://qhw.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cui.jiagoushi.top

[R47] sed 单行替换
来源：http://egh.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://aex.jqgfzy.top

[R48] awk 取指定列
来源：http://keu.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://dro.zdbjq.cn

[R49] awk 带条件
来源：http://vpd.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://efl.ydjk.org.cn

[R50] awk 求和
来源：http://aky.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://wgm.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://ehk.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ngb.sweek.top

[R52] 统计行数
来源：http://csc.wangdashe.top

wc -l a.txt
来源：http://qsm.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://pdu.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zmi.fehbvm.com

[R54] 比较两个文件
来源：http://efh.nanxuanxn.top

diff a.txt b.txt
来源：http://cev.aibaodan.cn

[R55] 压缩与解压
来源：http://bpz.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egi.jinqigufen.top

[R56] 远程拷贝
来源：http://thp.hnqzz.top

scp file user@host:/path/
来源：http://wuc.jianghu66.top

[R57] 远程执行命令
来源：http://kdv.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://tse.andypj.xyz

[R58] 下载文件
来源：http://apo.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vtj.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://ktr.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgl.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://iqo.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fqh.xinyue.icu

[R61] 磁盘占用
来源：http://oau.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://nzt.yvedp.cn

[R62] 找最占空间的文件
来源：http://kqi.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://dgp.cheryme.top

[R63] 内存与进程
来源：http://reg.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://qrw.vqdsnc.cn

[R64] 结束进程
来源：http://mih.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://lhg.jyoumei.cn

[R65] 查看端口占用
来源：http://jlp.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bba.0kj1m.cn

[R66] 定时任务
来源：http://rfa.yueranfly.top

crontab -e;  crontab -l
来源：http://dci.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://duz.sweek.top

openssl rand -hex 16
来源：http://wtu.guowangkeji.top

[R68] 计算文件校验值
来源：http://bgj.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://poy.hywenlv.cn

[R69] 生成随机密码
来源：http://xah.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://vfg.xinyue.icu

[R70] 时间戳与互转
来源：http://otz.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://pxs.haohaochexian.top

[R71] 日期格式化
来源：http://uah.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gnb.zdqjudy.top

[R72] 等待端口就绪
来源：http://zxm.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vdv.cdnleiting.top

[R73] 分割大日志
来源：http://sxo.redwolf501.top

split -l 1000 big.log part_
来源：http://zag.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://rxl.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://irn.yuanzhike.top

[R75] 导出环境变量
来源：http://utj.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://jxv.xziqi.cn

[R76] 使用临时文件
来源：http://waa.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sni.andypj.xyz

[R77] 读取用户输入
来源：http://xcp.chenzaomai.com

read -rp "请输入: " ans
来源：http://izc.jlsjyb.cn

[R78] 交互式菜单
来源：http://gkd.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dqv.jqgfzy.top

[R79] 解析命令行选项
来源：http://wfr.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wrp.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://bud.ywan-chungtsiang.top

time ./run.sh
来源：http://vcq.jinqigfzy.top

================================================================================
来源：http://fbz.zhongyouzk.top

S. C / C++ 专题
来源：http://vdo.yuanzhike.top

================================================================================
来源：http://wyo.jiagoushi.top

[S01] C：Hello World
来源：http://nkb.chenjidiqi.icu

#include <stdio.h>
来源：http://irs.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uic.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://kpa.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://qca.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://wxn.mhx1999.top

int x; scanf("%d", &x);
来源：http://rzu.cdnleiting.top

[S04] C：字符串复制
来源：http://von.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://skp.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://bxa.zhiwuduotai.top

strlen(s)
来源：http://xfj.shuidangran.top

[S06] C：字符串比较
来源：http://yip.bjfxy.top

strcmp(a, b) == 0
来源：http://znx.52xcode.cn

[S07] C：数组遍历求和
来源：http://fdw.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ypf.cashguo.top

[S08] C：动态内存分配与释放
来源：http://mep.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ogw.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://wxh.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gsz.ivvv.top

[S10] C：指针与解引用
来源：http://kho.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://wbs.vehdjk.com

[S11] C：逐行读文件
来源：http://sac.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://ppn.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lxb.jinqigufen.top

fclose(f);
来源：http://uye.ehwqpu.com

[S12] C：写文件
来源：http://bcm.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rkw.nwbrower.top

[S13] C：宏定义
来源：http://hvb.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://shc.shanyushiyangtech.top

[S14] C：枚举
来源：http://pez.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://ekg.ehwqpu.com

[S15] C：类型转换
来源：http://tda.bbcook.cn

(double) a / b
来源：http://saz.cdnleiting.top

[S16] C：位操作置位
来源：http://bsa.andypj.xyz

x |= (1 << 3);
来源：http://vql.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://kvo.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mjz.nanxuanxn.top

[S18] C：命令行参数
来源：http://qxp.quarkkingdee.top

int main(int argc, char **argv)
来源：http://dpj.jianghu66.top

[S19] C：快速排序
来源：http://ovv.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://fky.yueranfly.top

[S20] C：二分查找
来源：http://yln.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://djl.zhengqikj.top

[S21] C：字符类别判断
来源：http://omj.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tku.ctjpmb.com

[S22] C：字符串转数字
来源：http://pwc.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://cnf.bbcook.cn

[S23] C：随机数
来源：http://jlr.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jfk.uphjek.com

[S24] C：获取本地时间
来源：http://org.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yeb.shuidangran.top

[S25] C：内存拷贝
来源：http://pls.cashguo.top

memcpy(dst, src, n);
来源：http://weh.vqdsnc.cn

[S26] C：内存清零
来源：http://wsz.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://goa.sxryk.cn

[S27] C：定义常量
来源：http://gox.jlsjyb.cn

const double PI = 3.14159;
来源：http://zcn.vqdsnc.cn

[S28] C：静态变量
来源：http://wcl.yj20258888.top

static int counter = 0;
来源：http://uwp.fehbvm.com

[S29] C：变参函数
来源：http://fix.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://skn.jqgfzy.top

[S30] C：头文件保护
来源：http://jux.gotoacloud.top

#ifndef X_H
来源：http://fdn.zhijiandao.cn

#define X_H
来源：http://ixo.yvedp.cn

#endif
来源：http://nvq.tarul.cn

[S31] C++：Hello World
来源：http://bzo.havefunace.top

#include <iostream>
来源：http://tfr.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pig.redwolf501.top

[S32] C++：字符串
来源：http://qfk.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://hwk.shzxlz.cn

[S33] C++：vector 增删
来源：http://ptk.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ltd.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://zoh.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://fkr.quarkkingdee.top

[S35] C++：map
来源：http://qrn.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zay.hfpthk.cn

[S36] C++：unordered_map
来源：http://ori.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://szj.daria6918.cn

[S37] C++：set
来源：http://fuf.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kia.svipenyu.cn

[S38] C++：排序
来源：http://sbf.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://jxf.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://fra.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://onj.guannengcc.top

[S40] C++：查找元素
来源：http://hgp.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vuj.ctjpmb.com

[S41] C++：类与构造函数
来源：http://spd.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zlz.hnqzz.top

[S42] C++：继承与虚函数
来源：http://dzc.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://ycd.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://gzt.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://azo.yuanzhike.top

[S44] C++：引用传参
来源：http://nuo.mhx1999.top

void inc(int &x) { ++x; }
来源：http://wfl.aibaodan.cn

[S45] C++：lambda
来源：http://pff.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uwx.sufxvd.cn

[S46] C++：函数模板
来源：http://ohy.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nld.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://fko.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nmy.ctjpmb.com

[S48] C++：逐行读文件
来源：http://ugx.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jwp.nwbrower.top

while (std::getline(in, line)) { }
来源：http://qwd.jinqigfzy.top

[S49] C++：写文件
来源：http://hud.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://snw.daria6918.cn

[S50] C++：格式化数字
来源：http://iha.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hwm.aizwys.cn

[S51] C++：显式类型转换
来源：http://oly.hnqzz.top

static_cast<double>(a) / b
来源：http://ndt.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://tma.cashguo.top

int size() const noexcept { return n_; }
来源：http://wpb.redwolf501.top

[S53] C++：移动语义
来源：http://xoh.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://lvf.yanxiufei.cn

[S54] C++：异常处理
来源：http://yaf.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eib.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://kzf.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gqq.yvedp.cn

[S56] C++：optional
来源：http://pyv.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wgl.yongpay.top

[S57] C++：编译期常量
来源：http://kvz.iojbl.cn

constexpr int N = 10;
来源：http://ath.cqqwz.cn

[S58] C++：命名空间
来源：http://wat.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://rnf.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://lpw.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fcs.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://sih.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hrt.wangdashe.top

================================================================================
来源：http://jos.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://doj.yongpay.top

================================================================================
来源：http://rae.sweek.top

[T01] Kotlin：Hello World
来源：http://eby.hongshengwenyu.top

println("Hello")
来源：http://ats.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://yqt.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fxu.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://kvg.shanyushiyangtech.top

"值: $b"
来源：http://mzm.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://qob.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://rbb.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://fzb.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://paf.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://qoo.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bcr.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://ymf.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ezt.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://jbc.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://adb.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://oue.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://hwl.52xcode.cn

[T10] Kotlin：默认参数
来源：http://jrr.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://var.quarkkingdee.top

[T11] Kotlin：协程
来源：http://zlg.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://xfn.tian-w.cn

[T12] Kotlin：解构声明
来源：http://phy.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://bvh.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://ylb.iojbl.cn

val m = mapOf("a" to 1)
来源：http://hnc.jlsjyb.cn

[T14] Kotlin：循环
来源：http://ccc.fehbvm.com

for (i in 1..10) println(i)
来源：http://knq.hysaishi.cn

[T15] Kotlin：接口
来源：http://nyl.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://dhb.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://qpg.xuetiantiany.cn

print("Hello")
来源：http://yzx.gogol.net.cn

[T17] Swift：变量与常量
来源：http://dhx.yvedp.cn

var a = 1;  let b = 2
来源：http://bbs.ivvv.top

[T18] Swift：字符串插值
来源：http://mhc.vqdsnc.cn

"值: \(b)"
来源：http://qpf.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://loy.guowangkeji.top

if let n = opt { print(n) }
来源：http://gte.yueranfly.top

[T20] Swift：数组操作
来源：http://tvz.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://gfq.vqdsnc.cn

[T21] Swift：遍历
来源：http://rgh.wangdashe.top

for x in a { print(x) }
来源：http://bmm.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://cge.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sbx.nanxinkj.top

[T23] Swift：函数
来源：http://zpt.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nut.yj20258888.top

[T24] Swift：闭包
来源：http://hsb.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bav.gaohongyu789.top

[T25] Swift：结构体
来源：http://vmv.gotoacloud.top

struct P { var x: Int }
来源：http://btl.yonumen.top

[T26] Swift：类与重写
来源：http://vzm.jqgfzy.top

class A: Base { override func f() {} }
来源：http://qwp.xziqi.cn

[T27] Swift：错误处理
来源：http://xjl.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://psd.dianchejie.cn

[T28] Swift：枚举
来源：http://ssx.shuidangran.top

enum Color { case red, green }
来源：http://iem.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://daq.yuanzhike.top

guard let x = opt else { return }
来源：http://aby.ybcxt.top

[T30] Swift：协议
来源：http://raq.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://ubn.jlsjyb.cn

[T31] Lua：Hello World
来源：http://bav.shangyingyoupin.top

print("Hello")
来源：http://nyj.xziqi.cn

[T32] Lua：局部变量
来源：http://eyw.cqqwz.cn

local a = 1
来源：http://urw.tanke756.top

[T33] Lua：表（数组）
来源：http://ock.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jjn.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://ium.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eia.jlsjyb.cn

[T35] Lua：字典表
来源：http://jgo.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://iyt.gaohongyu789.top

[T36] Lua：函数
来源：http://ncy.zhengqikj.top

function add(a, b) return a + b end
来源：http://qgw.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://wzu.fanxiaobao.xyz

"a" .. "b"
来源：http://woj.xuetiantiany.cn

[T38] Lua：条件
来源：http://iqf.daria6918.cn

if x > 0 then print("正") end
来源：http://qxb.xylfe.cn

[T39] Lua：模式匹配
来源：http://txh.feifeiyinyue.top

string.find(s, "%d+")
来源：http://ptg.cucudq.cn

[T40] Lua：元表
来源：http://vem.daxiang520.top

setmetatable({}, { __index = base })
来源：http://rfq.sufxvd.cn

[T41] Perl：Hello World
来源：http://hqz.ehwqpu.com

print "Hello\n";
来源：http://jwj.yj202588.top

[T42] Perl：变量类型
来源：http://qqe.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://huu.ydjk.org.cn


<!-- 参考信息 -->