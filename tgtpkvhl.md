代发 wailian999

files=$(ls -1)
来源：http://yzx.hywenlv.cn

[R38] 管道串联
来源：http://wqm.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://fxj.hammf.cn

[R39] 重定向标准输出与错误
来源：http://vbv.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://mkx.chenjidiqi.icu

[R40] 追加写日志
来源：http://jcn.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://bcw.shuidangran.top

[R41] 丢弃输出
来源：http://waz.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://mra.zdbjq.cn

[R42] 输入重定向
来源：http://kqn.redwolf501.top

wc -l < a.txt
来源：http://twh.guowangkeji.top

[R43] 按名字查找文件
来源：http://tze.yj20258.top

find . -name "*.log" -type f
来源：http://skx.yuxming.cn

[R44] 按修改时间查找
来源：http://nna.cdnleiting.top

find . -mtime -7 -type f
来源：http://cxk.yuxming.cn

[R45] 批量删除
来源：http://vnm.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://epx.yonumen.top

[R46] 递归替换文件内容
来源：http://bfx.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qvs.ivvv.top

[R47] sed 单行替换
来源：http://pax.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://glh.aizwys.cn

[R48] awk 取指定列
来源：http://qlh.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://lic.hnqzz.top

[R49] awk 带条件
来源：http://nxi.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cov.jinqigufen.top

[R50] awk 求和
来源：http://llw.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://ldo.hfpthk.cn

[R51] 排序去重取前几
来源：http://pib.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://muh.xziqi.cn

[R52] 统计行数
来源：http://puv.wangdashe.top

wc -l a.txt
来源：http://jlv.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://gki.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zdi.iojbl.cn

[R54] 比较两个文件
来源：http://dpf.meibo888.top

diff a.txt b.txt
来源：http://gkr.gaohongyu789.top

[R55] 压缩与解压
来源：http://eoy.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qon.shangyingyoupin.top

[R56] 远程拷贝
来源：http://ins.fktsv.cn

scp file user@host:/path/
来源：http://lug.birdmap.top

[R57] 远程执行命令
来源：http://xkq.yongpay.top

ssh user@host 'uptime'
来源：http://nrd.ehwqpu.com

[R58] 下载文件
来源：http://tan.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aqo.jiagoushi.top

[R59] 发 POST JSON
来源：http://wud.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yai.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://uha.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rpu.cqqwz.cn

[R61] 磁盘占用
来源：http://uvo.cashguo.top

df -h;  du -sh *
来源：http://gmh.pycfn.com

[R62] 找最占空间的文件
来源：http://htj.9152youxi.cn

du -ah . | sort -rh | head -10
来源：http://fwy.yj20258.top

[R63] 内存与进程
来源：http://dcm.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://vrq.aizwys.cn

[R64] 结束进程
来源：http://ngh.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://pan.tarul.cn

[R65] 查看端口占用
来源：http://joe.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://coc.316326.xyz

[R66] 定时任务
来源：http://uci.zhoulong.xyz

crontab -e;  crontab -l
来源：http://ivp.fktsv.cn

[R67] 生成随机十六进制串
来源：http://whn.daria6918.cn

openssl rand -hex 16
来源：http://exf.zhixingplan.top

[R68] 计算文件校验值
来源：http://tdh.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qzd.fktsv.cn

[R69] 生成随机密码
来源：http://tyr.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://cau.chenzaomai.com

[R70] 时间戳与互转
来源：http://vwo.meibo888.top

date +%s;  date -d @1700000000
来源：http://zss.tianlin.xyz

[R71] 日期格式化
来源：http://aye.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dtj.shzxlz.cn

[R72] 等待端口就绪
来源：http://wvz.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xhu.9152youxi.cn

[R73] 分割大日志
来源：http://rod.hywenlv.cn

split -l 1000 big.log part_
来源：http://ava.zhixingplan.top

[R74] 批量重命名
来源：http://uag.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ldc.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://rzq.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://qnt.hfpthk.cn

[R76] 使用临时文件
来源：http://qdd.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://day.smart0.xyz

[R77] 读取用户输入
来源：http://nwm.tian-w.cn

read -rp "请输入: " ans
来源：http://utv.9152youxi.cn

[R78] 交互式菜单
来源：http://iex.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jym.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://qej.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dap.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://aux.ctjpmb.com

time ./run.sh
来源：http://yor.jinyuanbaomall.cn

================================================================================
来源：http://tga.nwbrower.top

S. C / C++ 专题
来源：http://vay.0kj1m.cn

================================================================================
来源：http://uxg.52xcode.cn

[S01] C：Hello World
来源：http://guv.hfpthk.cn

#include <stdio.h>
来源：http://npm.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://awh.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://tbp.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://qyk.wangshuangyany.cn

[S03] C：读入整数
来源：http://jfl.sxryk.cn

int x; scanf("%d", &x);
来源：http://otc.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://iuu.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fld.shzxlz.cn

[S05] C：字符串长度
来源：http://mul.hesvh.cn

strlen(s)
来源：http://ucd.redwolf501.top

[S06] C：字符串比较
来源：http://stk.chenzaomai.com

strcmp(a, b) == 0
来源：http://vcw.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://apw.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dnf.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://ulv.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://csv.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://vsn.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://weo.fehbvm.com

[S10] C：指针与解引用
来源：http://dwk.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://lzl.sysykeji.top

[S11] C：逐行读文件
来源：http://fcr.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://cfw.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zrq.aibaodan.cn

fclose(f);
来源：http://jdr.0kj1m.cn

[S12] C：写文件
来源：http://xra.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wpu.zdbjq.cn

[S13] C：宏定义
来源：http://pia.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ljy.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://jzk.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://axa.kuanghao11.cn

[S15] C：类型转换
来源：http://rxz.vqdsnc.cn

(double) a / b
来源：http://ljo.ydzc1.top

[S16] C：位操作置位
来源：http://nbb.hywenlv.cn

x |= (1 << 3);
来源：http://cjv.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://can.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hta.gotoacloud.top

[S18] C：命令行参数
来源：http://ayw.jinqigfzy.top

int main(int argc, char **argv)
来源：http://ort.vehdjk.com

[S19] C：快速排序
来源：http://nnw.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://oaa.yfazqb.com

[S20] C：二分查找
来源：http://ive.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://juf.meibo888.top

[S21] C：字符类别判断
来源：http://qij.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dee.uphjek.com

[S22] C：字符串转数字
来源：http://you.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://fgt.vqdsnc.cn

[S23] C：随机数
来源：http://oww.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mcw.fengsongda.top

[S24] C：获取本地时间
来源：http://brl.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qjq.cucudq.cn

[S25] C：内存拷贝
来源：http://pjy.xuanzx.com

memcpy(dst, src, n);
来源：http://oen.pengpengdd.cyou

[S26] C：内存清零
来源：http://rav.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://cwc.ctjpmb.com

[S27] C：定义常量
来源：http://bwc.hywenlv.cn

const double PI = 3.14159;
来源：http://fdv.pengpengdd.cyou

[S28] C：静态变量
来源：http://olz.birdmap.top

static int counter = 0;
来源：http://bin.shuidangran.top

[S29] C：变参函数
来源：http://qvb.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qrq.havefunace.top

[S30] C：头文件保护
来源：http://oyr.guowangkeji.top

#ifndef X_H
来源：http://baj.chenzaomai.com

#define X_H
来源：http://xpe.chenzaomai.com

#endif
来源：http://obb.yuanzhike.top

[S31] C++：Hello World
来源：http://dhc.ybcxt.top

#include <iostream>
来源：http://jhb.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://kpb.snrcjt.cn

[S32] C++：字符串
来源：http://wzd.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://xwq.yongpay.top

[S33] C++：vector 增删
来源：http://pqa.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xgn.cucudq.cn

[S34] C++：遍历 vector
来源：http://gvz.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://dfv.andypj.xyz

[S35] C++：map
来源：http://nnh.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://svs.zhixingplan.top

[S36] C++：unordered_map
来源：http://zzc.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ocs.svipenyu.cn

[S37] C++：set
来源：http://kmr.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hui.yueranfly.top

[S38] C++：排序
来源：http://qeq.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://hzt.havefunace.top

[S39] C++：自定义比较器排序
来源：http://fai.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qcj.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://oou.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahs.yonumen.top

[S41] C++：类与构造函数
来源：http://xqm.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://var.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://cdr.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://ayk.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://rdn.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://kpr.sysykeji.top

[S44] C++：引用传参
来源：http://cdq.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ndu.nanxuanxn.top

[S45] C++：lambda
来源：http://klu.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aos.vqdsnc.cn

[S46] C++：函数模板
来源：http://btb.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zll.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://fng.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqm.chenzaomai.com

[S48] C++：逐行读文件
来源：http://azl.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://feh.yvedp.cn

while (std::getline(in, line)) { }
来源：http://sfc.aizwys.cn

[S49] C++：写文件
来源：http://uij.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gcu.hcnkem.com

[S50] C++：格式化数字
来源：http://azl.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jgm.ydzc1.top

[S51] C++：显式类型转换
来源：http://brf.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://vks.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://dsd.316326.xyz

int size() const noexcept { return n_; }
来源：http://usb.jiagoushi.top

[S53] C++：移动语义
来源：http://auo.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://hyf.redwolf501.top

[S54] C++：异常处理
来源：http://guo.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://idu.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://guo.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ebw.xylfe.cn

[S56] C++：optional
来源：http://xrf.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ekt.jqgfzy.top

[S57] C++：编译期常量
来源：http://ncq.cqqwz.cn

constexpr int N = 10;
来源：http://aap.hfpthk.cn

[S58] C++：命名空间
来源：http://ecn.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://onn.jinqigfzy.top

[S59] C++：静态断言
来源：http://qim.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mdw.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://klk.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ewb.zycfv.cn

================================================================================
来源：http://ezu.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wtw.gotoacloud.top

================================================================================
来源：http://tgy.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://uys.hywenlv.cn

println("Hello")
来源：http://tpb.zdbjq.cn

[T02] Kotlin：变量
来源：http://rkm.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://etr.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://jqb.hnxiangtu.top

"值: $b"
来源：http://sfq.daxiang520.top

[T04] Kotlin：空安全
来源：http://bhj.sweek.top

val n: String? = null;  n?.length
来源：http://mrs.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://dyh.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sgk.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://mkw.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://crm.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://lbv.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://yfg.hfpthk.cn

[T08] Kotlin：数据类
来源：http://cxo.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://pdi.316326.xyz

[T09] Kotlin：扩展函数
来源：http://raj.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://vze.fengsongda.top

[T10] Kotlin：默认参数
来源：http://dhm.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tis.zhongyouzk.top

[T11] Kotlin：协程
来源：http://dsq.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://yqc.yuxming.cn

[T12] Kotlin：解构声明
来源：http://yls.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://ose.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://awl.yonumen.top

val m = mapOf("a" to 1)
来源：http://aee.jqgfzy.top

[T14] Kotlin：循环
来源：http://gss.316326.xyz

for (i in 1..10) println(i)
来源：http://gki.sweek.top

[T15] Kotlin：接口
来源：http://aco.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://aim.316326.xyz

[T16] Swift：Hello World
来源：http://dbf.zhengqikj.top

print("Hello")
来源：http://htt.cdnleiting.top

[T17] Swift：变量与常量
来源：http://dcu.chenlongwang.top

var a = 1;  let b = 2
来源：http://osz.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://tjq.zhijiandao.cn

"值: \(b)"
来源：http://ehy.yj20258.top

[T19] Swift：可选绑定
来源：http://cme.aizwys.cn

if let n = opt { print(n) }
来源：http://zsz.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://ygy.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://igw.hysaishi.cn

[T21] Swift：遍历
来源：http://vcw.gogol.net.cn

for x in a { print(x) }
来源：http://imb.redwolf501.top

[T22] Swift：字典
来源：http://wcj.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://ila.shanyushiyangtech.top

[T23] Swift：函数
来源：http://oii.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wzg.zhengqikj.top

[T24] Swift：闭包
来源：http://odc.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rrg.hammf.cn

[T25] Swift：结构体
来源：http://jlu.fktsv.cn

struct P { var x: Int }
来源：http://uae.quarkkingdee.top

[T26] Swift：类与重写
来源：http://dez.jyoumei.cn

class A: Base { override func f() {} }
来源：http://pea.chenlongwang.top

[T27] Swift：错误处理
来源：http://mcj.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://ayy.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://qdl.chenjidiqi.icu

enum Color { case red, green }
来源：http://xhu.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://gyh.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://yzm.zhoulong.xyz

[T30] Swift：协议
来源：http://rrg.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://klo.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://zps.yangfankeji.com

print("Hello")
来源：http://avz.zycfv.cn

[T32] Lua：局部变量
来源：http://awe.xingfuxueyuan.xyz

local a = 1
来源：http://ixm.hfpthk.cn

[T33] Lua：表（数组）
来源：http://qtz.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xrs.dianchejie.cn

[T34] Lua：遍历表
来源：http://kkj.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://omm.sjlbkw.cn

[T35] Lua：字典表
来源：http://xom.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://gbb.haohaochexian.top

[T36] Lua：函数
来源：http://dss.fengsongda.top

function add(a, b) return a + b end
来源：http://rwp.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://nox.gaohongyu789.top

"a" .. "b"
来源：http://bou.guowangkeji.top

[T38] Lua：条件
来源：http://etm.vehdjk.com

if x > 0 then print("正") end
来源：http://okd.fzhhl.top

[T39] Lua：模式匹配
来源：http://usz.hnxiangtu.top

string.find(s, "%d+")
来源：http://lxj.feifeiyinyue.top

[T40] Lua：元表
来源：http://fwu.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://wji.zhixingplan.top


<!-- 参考信息 -->