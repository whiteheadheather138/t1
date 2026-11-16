代发 wailian999

files=$(ls -1)
来源：http://gks.sysykeji.top

[R38] 管道串联
来源：http://udw.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://dul.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://ppl.jinqigfzy.top

cmd > out.log 2>&1
来源：http://cbt.shanyushiyangtech.top

[R40] 追加写日志
来源：http://fod.ivvv.top

echo "log" >> out.log
来源：http://row.zdqjudy.top

[R41] 丢弃输出
来源：http://kdw.iojbl.cn

cmd >/dev/null 2>&1
来源：http://sxr.chenzaomai.com

[R42] 输入重定向
来源：http://qgy.mhx1999.top

wc -l < a.txt
来源：http://tqd.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://qyg.bjfxy.top

find . -name "*.log" -type f
来源：http://cxc.zycfv.cn

[R44] 按修改时间查找
来源：http://jtn.yuanzhike.top

find . -mtime -7 -type f
来源：http://eoy.9152youxi.cn

[R45] 批量删除
来源：http://tbu.gzhubu.top

find . -name "*.tmp" -delete
来源：http://bbr.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://vkj.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zah.chenzaomai.com

[R47] sed 单行替换
来源：http://vod.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://bum.aibaodan.cn

[R48] awk 取指定列
来源：http://rdf.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://ovy.dashuyun.cn

[R49] awk 带条件
来源：http://yfb.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dgz.ppjwa.cn

[R50] awk 求和
来源：http://slc.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://tcy.fzhhl.top

[R51] 排序去重取前几
来源：http://rir.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cmr.vehdjk.com

[R52] 统计行数
来源：http://ehk.c1oappe.top

wc -l a.txt
来源：http://btr.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://vuo.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xqt.zdqjudy.top

[R54] 比较两个文件
来源：http://baa.hysaishi.cn

diff a.txt b.txt
来源：http://nkh.xuanzx.com

[R55] 压缩与解压
来源：http://byi.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yde.tarul.cn

[R56] 远程拷贝
来源：http://eeg.jlsjyb.cn

scp file user@host:/path/
来源：http://nie.aizwys.cn

[R57] 远程执行命令
来源：http://igl.ivvv.top

ssh user@host 'uptime'
来源：http://vik.meibo888.top

[R58] 下载文件
来源：http://dbt.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sah.ehwqpu.com

[R59] 发 POST JSON
来源：http://rvu.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jum.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://uex.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ysn.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://uwj.birdmap.top

df -h;  du -sh *
来源：http://lle.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://wmh.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://mzv.jyoumei.cn

[R63] 内存与进程
来源：http://nju.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://kbe.9152youxi.cn

[R64] 结束进程
来源：http://ows.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://mfc.sysykeji.top

[R65] 查看端口占用
来源：http://sqb.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ndv.cheryme.top

[R66] 定时任务
来源：http://xxy.jiagoushi.top

crontab -e;  crontab -l
来源：http://amg.xziqi.cn

[R67] 生成随机十六进制串
来源：http://ssj.aizwys.cn

openssl rand -hex 16
来源：http://apc.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://mdl.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://vfz.yueranfly.top

[R69] 生成随机密码
来源：http://prb.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://org.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://fyi.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://jzs.ydzc1.top

[R71] 日期格式化
来源：http://lbh.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gvg.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://jgo.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nav.gzhubu.top

[R73] 分割大日志
来源：http://zmx.0kj1m.cn

split -l 1000 big.log part_
来源：http://obw.fktsv.cn

[R74] 批量重命名
来源：http://wyj.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://afl.mhx1999.top

[R75] 导出环境变量
来源：http://ecm.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://dex.xuanzx.com

[R76] 使用临时文件
来源：http://olx.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ggv.gzhubu.top

[R77] 读取用户输入
来源：http://sfm.hesvh.cn

read -rp "请输入: " ans
来源：http://suk.daria6918.cn

[R78] 交互式菜单
来源：http://ffv.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kvi.daxiang520.top

[R79] 解析命令行选项
来源：http://drp.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mzo.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://pqk.zhongyouzk.top

time ./run.sh
来源：http://pfb.aizwys.cn

================================================================================
来源：http://fje.zdbjq.cn

S. C / C++ 专题
来源：http://hub.jinyuanbaomall.cn

================================================================================
来源：http://uyu.daria6918.cn

[S01] C：Hello World
来源：http://nsm.gogol.net.cn

#include <stdio.h>
来源：http://azw.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://isc.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://ocx.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://hui.jyoumei.cn

[S03] C：读入整数
来源：http://lbt.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://mfa.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://jbm.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://elw.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://ddy.xuanzx.com

strlen(s)
来源：http://wki.havefunace.top

[S06] C：字符串比较
来源：http://nly.yj202588.top

strcmp(a, b) == 0
来源：http://ljo.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://pfw.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gse.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://nhg.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gjp.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://zqh.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jsa.epnwcf.com

[S10] C：指针与解引用
来源：http://oey.wangdashe.top

int *p = &a;  *p = 5;
来源：http://ngz.hesvh.cn

[S11] C：逐行读文件
来源：http://hgx.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://cbp.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dku.jqgfzy.top

fclose(f);
来源：http://hrl.fehbvm.com

[S12] C：写文件
来源：http://nbj.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://loo.ydzc1.top

[S13] C：宏定义
来源：http://wpz.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://amc.feifeiyinyue.top

[S14] C：枚举
来源：http://mzm.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://ogm.ydzc1.top

[S15] C：类型转换
来源：http://wvb.zdqjudy.top

(double) a / b
来源：http://sez.fzhhl.top

[S16] C：位操作置位
来源：http://itr.zhiwuduotai.top

x |= (1 << 3);
来源：http://pts.vehdjk.com

[S17] C：安全拼接字符串
来源：http://iyx.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://foj.hesvh.cn

[S18] C：命令行参数
来源：http://wiv.tianlin.xyz

int main(int argc, char **argv)
来源：http://gas.sjlbkw.cn

[S19] C：快速排序
来源：http://vnl.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://yat.xuetiantiany.cn

[S20] C：二分查找
来源：http://sya.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dew.zdbjq.cn

[S21] C：字符类别判断
来源：http://bwx.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wlc.jiagoushi.top

[S22] C：字符串转数字
来源：http://zdv.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://rcs.svipenyu.cn

[S23] C：随机数
来源：http://btk.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lam.sysykeji.top

[S24] C：获取本地时间
来源：http://fkj.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fcv.yanxiufei.cn

[S25] C：内存拷贝
来源：http://myg.hnxiangtu.top

memcpy(dst, src, n);
来源：http://oci.yvedp.cn

[S26] C：内存清零
来源：http://rus.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://drp.sjlbkw.cn

[S27] C：定义常量
来源：http://cbp.quarkkingdee.top

const double PI = 3.14159;
来源：http://vwz.aibaodan.cn

[S28] C：静态变量
来源：http://lbe.daxiang520.top

static int counter = 0;
来源：http://tmt.316326.xyz

[S29] C：变参函数
来源：http://kdh.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nmy.chenjidiqi.icu

[S30] C：头文件保护
来源：http://ukx.yangfankeji.com

#ifndef X_H
来源：http://fdx.chenzaomai.com

#define X_H
来源：http://ijl.pycfn.com

#endif
来源：http://npf.wangdashe.top

[S31] C++：Hello World
来源：http://fuz.xylfe.cn

#include <iostream>
来源：http://twa.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://mvq.yangfankeji.com

[S32] C++：字符串
来源：http://jwq.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://ihe.zhixingplan.top

[S33] C++：vector 增删
来源：http://guf.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ltm.tanke756.top

[S34] C++：遍历 vector
来源：http://jyt.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://qsd.sysykeji.top

[S35] C++：map
来源：http://dsn.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://imc.xuanzx.com

[S36] C++：unordered_map
来源：http://wdq.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eyp.pycfn.com

[S37] C++：set
来源：http://kgq.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://drm.ctjpmb.com

[S38] C++：排序
来源：http://uwa.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://rra.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://uuf.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lox.ydzc1.top

[S40] C++：查找元素
来源：http://jnw.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bli.sufxvd.cn

[S41] C++：类与构造函数
来源：http://mey.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vhh.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://jsn.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://wxf.aibaodan.cn

[S43] C++：智能指针
来源：http://cfv.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://xya.tarul.cn

[S44] C++：引用传参
来源：http://fyn.hammf.cn

void inc(int &x) { ++x; }
来源：http://vkk.cheryme.top

[S45] C++：lambda
来源：http://bic.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://pix.andypj.xyz

[S46] C++：函数模板
来源：http://agl.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kjr.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://ado.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xks.epnwcf.com

[S48] C++：逐行读文件
来源：http://dbu.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rdm.guannengcc.top

while (std::getline(in, line)) { }
来源：http://ljm.52xcode.cn

[S49] C++：写文件
来源：http://ztc.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofg.chenzaomai.com

[S50] C++：格式化数字
来源：http://yhk.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aef.hesvh.cn

[S51] C++：显式类型转换
来源：http://nkh.jiagoushi.top

static_cast<double>(a) / b
来源：http://znp.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://eyj.tanke756.top

int size() const noexcept { return n_; }
来源：http://iyv.mhx1999.top

[S53] C++：移动语义
来源：http://wzg.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://zvf.xinyue.icu

[S54] C++：异常处理
来源：http://ape.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://evt.yuxming.cn

[S55] C++：结构化绑定
来源：http://uva.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lug.gzhubu.top

[S56] C++：optional
来源：http://pyz.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fwv.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://soy.jyoumei.cn

constexpr int N = 10;
来源：http://nbd.bbcook.cn

[S58] C++：命名空间
来源：http://ngq.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://bih.mhx1999.top

[S59] C++：静态断言
来源：http://pzc.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rvr.hammf.cn

[S60] C++：遍历并删除元素
来源：http://mdz.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qrs.quarkkingdee.top

================================================================================
来源：http://pek.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxo.hywenlv.cn

================================================================================
来源：http://pug.jianghu66.top

[T01] Kotlin：Hello World
来源：http://fip.meibo888.top

println("Hello")
来源：http://bmh.mhx1999.top

[T02] Kotlin：变量
来源：http://hdu.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wud.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://yry.dianchejie.cn

"值: $b"
来源：http://vaa.xuanzx.com

[T04] Kotlin：空安全
来源：http://oom.tarul.cn

val n: String? = null;  n?.length
来源：http://qhc.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://hph.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qob.vehdjk.com

[T06] Kotlin：集合映射
来源：http://vxu.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ncx.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://qky.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://awj.0kj1m.cn

[T08] Kotlin：数据类
来源：http://ohx.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://yuu.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://tou.hammf.cn

fun String.exclaim() = this + "!"
来源：http://xsx.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://naf.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tzj.hammf.cn

[T11] Kotlin：协程
来源：http://aun.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://udr.yfazqb.com

[T12] Kotlin：解构声明
来源：http://dhq.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://qdo.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://skc.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://tpz.jianghu66.top

[T14] Kotlin：循环
来源：http://dmv.fehbvm.com

for (i in 1..10) println(i)
来源：http://tsz.ybcxt.top

[T15] Kotlin：接口
来源：http://rpu.xinyue.icu

interface Shape { fun area(): Double }
来源：http://xwt.andypj.xyz

[T16] Swift：Hello World
来源：http://xkz.gotoacloud.top

print("Hello")
来源：http://iqh.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://sat.epnwcf.com

var a = 1;  let b = 2
来源：http://rua.ehwqpu.com

[T18] Swift：字符串插值
来源：http://hnn.aizwys.cn

"值: \(b)"
来源：http://vep.9152youxi.cn

[T19] Swift：可选绑定
来源：http://yrj.daria6918.cn

if let n = opt { print(n) }
来源：http://ihx.jlsjyb.cn

[T20] Swift：数组操作
来源：http://fhb.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hwl.c1oappe.top

[T21] Swift：遍历
来源：http://izq.nwbrower.top

for x in a { print(x) }
来源：http://ylr.bbcook.cn

[T22] Swift：字典
来源：http://jye.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://msl.zhijiandao.cn

[T23] Swift：函数
来源：http://jlu.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://idc.feifeiyinyue.top

[T24] Swift：闭包
来源：http://feb.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fwz.cashguo.top

[T25] Swift：结构体
来源：http://nzc.bjfxy.top

struct P { var x: Int }
来源：http://cly.shzxlz.cn

[T26] Swift：类与重写
来源：http://fpj.aibaodan.cn

class A: Base { override func f() {} }
来源：http://bwt.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://xib.yvedp.cn

do { try f() } catch { print(error) }
来源：http://ubi.tanke756.top

[T28] Swift：枚举
来源：http://kde.andypj.xyz

enum Color { case red, green }
来源：http://yjt.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://tpg.yuxming.cn

guard let x = opt else { return }
来源：http://fbm.hongshengwenyu.top

[T30] Swift：协议
来源：http://ucq.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://tjd.havefunace.top

[T31] Lua：Hello World
来源：http://txw.tian-w.cn

print("Hello")
来源：http://ewi.0kj1m.cn

[T32] Lua：局部变量
来源：http://dhg.gzhubu.top

local a = 1
来源：http://hmf.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://hcb.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bih.dianchejie.cn

[T34] Lua：遍历表
来源：http://slo.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vrm.snrcjt.cn

[T35] Lua：字典表
来源：http://ggt.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://ivj.yj20258.top

[T36] Lua：函数
来源：http://cmj.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://prc.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://lpc.9152youxi.cn

"a" .. "b"
来源：http://vkr.jinqigufen.top

[T38] Lua：条件
来源：http://npq.hammf.cn

if x > 0 then print("正") end
来源：http://zyv.xuanzx.com

[T39] Lua：模式匹配
来源：http://pjf.xuanzx.com

string.find(s, "%d+")
来源：http://wyn.jianghu66.top

[T40] Lua：元表
来源：http://zsw.fehbvm.com

setmetatable({}, { __index = base })
来源：http://qih.zhiwuduotai.top


<!-- 参考信息 -->