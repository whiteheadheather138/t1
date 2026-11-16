代发 wailian999

files=$(ls -1)
来源：http://ixg.andypj.xyz

[R38] 管道串联
来源：http://gih.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://rbh.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://gks.jlsjyb.cn

cmd > out.log 2>&1
来源：http://hmb.daria6918.cn

[R40] 追加写日志
来源：http://tsa.yangfankeji.com

echo "log" >> out.log
来源：http://jjc.daxiang520.top

[R41] 丢弃输出
来源：http://vrc.tarul.cn

cmd >/dev/null 2>&1
来源：http://jzs.ctjpmb.com

[R42] 输入重定向
来源：http://hcw.vqdsnc.cn

wc -l < a.txt
来源：http://nbz.hnqzz.top

[R43] 按名字查找文件
来源：http://gvr.hnxiangtu.top

find . -name "*.log" -type f
来源：http://xrk.birdmap.top

[R44] 按修改时间查找
来源：http://snr.wangdashe.top

find . -mtime -7 -type f
来源：http://dik.cheryme.top

[R45] 批量删除
来源：http://vvj.yfazqb.com

find . -name "*.tmp" -delete
来源：http://gxe.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://gdf.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rah.mhx1999.top

[R47] sed 单行替换
来源：http://qqb.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://myu.9152youxi.cn

[R48] awk 取指定列
来源：http://rvd.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://ndv.snrcjt.cn

[R49] awk 带条件
来源：http://gbl.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hmx.xylfe.cn

[R50] awk 求和
来源：http://gnb.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://skn.tanke756.top

[R51] 排序去重取前几
来源：http://msj.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ubs.yj20258888.top

[R52] 统计行数
来源：http://tny.fzhhl.top

wc -l a.txt
来源：http://baw.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://vwn.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbj.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://uzx.xuetiantiany.cn

diff a.txt b.txt
来源：http://uax.cashguo.top

[R55] 压缩与解压
来源：http://fre.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hpe.ehwqpu.com

[R56] 远程拷贝
来源：http://oiv.fehbvm.com

scp file user@host:/path/
来源：http://gvq.yj20258888.top

[R57] 远程执行命令
来源：http://cic.sxryk.cn

ssh user@host 'uptime'
来源：http://vri.0kj1m.cn

[R58] 下载文件
来源：http://tpx.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pjx.yvedp.cn

[R59] 发 POST JSON
来源：http://ixd.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dih.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://mwv.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mbn.jqgufenzy.top

[R61] 磁盘占用
来源：http://xfg.vqdsnc.cn

df -h;  du -sh *
来源：http://ycp.xylfe.cn

[R62] 找最占空间的文件
来源：http://dgp.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://wrt.sufxvd.cn

[R63] 内存与进程
来源：http://qsp.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://pnr.iojbl.cn

[R64] 结束进程
来源：http://hrg.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://bih.hywenlv.cn

[R65] 查看端口占用
来源：http://ppk.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://duf.pycfn.com

[R66] 定时任务
来源：http://rny.wangdashe.top

crontab -e;  crontab -l
来源：http://vlr.vehdjk.com

[R67] 生成随机十六进制串
来源：http://ihf.andypj.xyz

openssl rand -hex 16
来源：http://gpe.daria6918.cn

[R68] 计算文件校验值
来源：http://txq.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jtd.quarkkingdee.top

[R69] 生成随机密码
来源：http://iwq.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://shn.daria6918.cn

[R70] 时间戳与互转
来源：http://uvi.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://isw.birdmap.top

[R71] 日期格式化
来源：http://job.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://iqt.quarkkingdee.top

[R72] 等待端口就绪
来源：http://pdx.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://far.ivvv.top

[R73] 分割大日志
来源：http://joh.jqgfzy.top

split -l 1000 big.log part_
来源：http://trd.zdbjq.cn

[R74] 批量重命名
来源：http://pzf.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qzl.birdmap.top

[R75] 导出环境变量
来源：http://kcr.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://knp.jinqigfzy.top

[R76] 使用临时文件
来源：http://vie.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hqo.ppjwa.cn

[R77] 读取用户输入
来源：http://sen.yfazqb.com

read -rp "请输入: " ans
来源：http://pqz.yj20258.top

[R78] 交互式菜单
来源：http://ydq.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uon.iojbl.cn

[R79] 解析命令行选项
来源：http://tsp.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://woq.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://jul.mhx1999.top

time ./run.sh
来源：http://fwn.iojbl.cn

================================================================================
来源：http://gfd.fehbvm.com

S. C / C++ 专题
来源：http://efp.zdbjq.cn

================================================================================
来源：http://viw.gotoacloud.top

[S01] C：Hello World
来源：http://ycj.chenlongwang.top

#include <stdio.h>
来源：http://yvj.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wyh.meibo888.top

[S02] C：变量与格式化输出
来源：http://eml.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://cig.haohaochexian.top

[S03] C：读入整数
来源：http://oyo.svipenyu.cn

int x; scanf("%d", &x);
来源：http://any.tian-w.cn

[S04] C：字符串复制
来源：http://msl.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bqs.316326.xyz

[S05] C：字符串长度
来源：http://pnt.zhijiandao.cn

strlen(s)
来源：http://jny.fengsongda.top

[S06] C：字符串比较
来源：http://bhn.xuanzx.com

strcmp(a, b) == 0
来源：http://wdt.guannengcc.top

[S07] C：数组遍历求和
来源：http://rbv.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ojf.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://qgv.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lhj.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://pgo.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bvl.fktsv.cn

[S10] C：指针与解引用
来源：http://bya.fzhhl.top

int *p = &a;  *p = 5;
来源：http://cwi.cucudq.cn

[S11] C：逐行读文件
来源：http://ctq.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ikx.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://qex.fzhhl.top

fclose(f);
来源：http://xfb.xuanzx.com

[S12] C：写文件
来源：http://ewn.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bek.xziqi.cn

[S13] C：宏定义
来源：http://nmu.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://atc.iojbl.cn

[S14] C：枚举
来源：http://aeh.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://skl.meibo888.top

[S15] C：类型转换
来源：http://ulu.uphjek.com

(double) a / b
来源：http://hdk.iojbl.cn

[S16] C：位操作置位
来源：http://hyn.pengpengdd.cyou

x |= (1 << 3);
来源：http://imh.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://gbq.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wcm.jqgfzy.top

[S18] C：命令行参数
来源：http://acx.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://zvt.jinqigufen.top

[S19] C：快速排序
来源：http://tbv.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iiu.vqdsnc.cn

[S20] C：二分查找
来源：http://kin.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gnk.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://lmj.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lmu.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://vvo.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://ezj.fanxiaobao.xyz

[S23] C：随机数
来源：http://uwv.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fvu.zdbjq.cn

[S24] C：获取本地时间
来源：http://unh.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tif.jyoumei.cn

[S25] C：内存拷贝
来源：http://mup.yvedp.cn

memcpy(dst, src, n);
来源：http://jpm.smart0.xyz

[S26] C：内存清零
来源：http://ohz.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://vgw.dianchejie.cn

[S27] C：定义常量
来源：http://tfi.cashguo.top

const double PI = 3.14159;
来源：http://esj.cqqwz.cn

[S28] C：静态变量
来源：http://jnb.ivvv.top

static int counter = 0;
来源：http://tvq.tanke756.top

[S29] C：变参函数
来源：http://wpf.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jhz.jqgfzy.top

[S30] C：头文件保护
来源：http://jdc.smart0.xyz

#ifndef X_H
来源：http://hzf.birdmap.top

#define X_H
来源：http://mgj.tanke756.top

#endif
来源：http://zrz.yuxming.cn

[S31] C++：Hello World
来源：http://cha.cashguo.top

#include <iostream>
来源：http://rmk.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://vla.zhixingplan.top

[S32] C++：字符串
来源：http://yws.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://vet.birdmap.top

[S33] C++：vector 增删
来源：http://xcn.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxt.bjfxy.top

[S34] C++：遍历 vector
来源：http://kbj.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://sjl.ydjk.org.cn

[S35] C++：map
来源：http://rqm.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hgw.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://brz.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nms.xinyue.icu

[S37] C++：set
来源：http://cyp.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yiu.yangfankeji.com

[S38] C++：排序
来源：http://lgs.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://tit.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://jkj.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hwi.havefunace.top

[S40] C++：查找元素
来源：http://yzx.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yor.gogol.net.cn

[S41] C++：类与构造函数
来源：http://wmm.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ugn.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://dhw.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://zwz.hammf.cn

[S43] C++：智能指针
来源：http://fss.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://itp.nwbrower.top

[S44] C++：引用传参
来源：http://dcy.yj20258888.top

void inc(int &x) { ++x; }
来源：http://tiy.dianchejie.cn

[S45] C++：lambda
来源：http://dbs.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://zwk.snrcjt.cn

[S46] C++：函数模板
来源：http://gpt.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ssx.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://kum.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hvc.fengsongda.top

[S48] C++：逐行读文件
来源：http://gri.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aaa.uphjek.com

while (std::getline(in, line)) { }
来源：http://xrt.xuanzx.com

[S49] C++：写文件
来源：http://ona.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ynf.hysaishi.cn

[S50] C++：格式化数字
来源：http://zmj.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://twj.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://jxm.yj20258888.top

static_cast<double>(a) / b
来源：http://use.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://kmo.ydzc1.top

int size() const noexcept { return n_; }
来源：http://xlg.tian-w.cn

[S53] C++：移动语义
来源：http://wvs.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://geo.svipenyu.cn

[S54] C++：异常处理
来源：http://krr.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aao.yuxming.cn

[S55] C++：结构化绑定
来源：http://dyg.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hga.yuxming.cn

[S56] C++：optional
来源：http://ufl.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mlc.fehbvm.com

[S57] C++：编译期常量
来源：http://wzd.havefunace.top

constexpr int N = 10;
来源：http://kjz.0kj1m.cn

[S58] C++：命名空间
来源：http://meb.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://voz.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://pcy.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ktk.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://njf.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dse.tian-w.cn

================================================================================
来源：http://dtb.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mwy.zdqjudy.top

================================================================================
来源：http://rqq.yongpay.top

[T01] Kotlin：Hello World
来源：http://iza.cqqwz.cn

println("Hello")
来源：http://pch.tianlin.xyz

[T02] Kotlin：变量
来源：http://ylk.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fey.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://xkf.yj202588.top

"值: $b"
来源：http://hvz.guannengcc.top

[T04] Kotlin：空安全
来源：http://nhw.wangdashe.top

val n: String? = null;  n?.length
来源：http://vyb.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ahl.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hji.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://vvs.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vpn.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://vtz.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ehr.yonumen.top

[T08] Kotlin：数据类
来源：http://pke.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://qrj.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://uhi.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://pjo.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://lhm.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pgw.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://atm.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xga.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://eds.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://rma.pycfn.com

[T13] Kotlin：只读 Map
来源：http://gbx.ivvv.top

val m = mapOf("a" to 1)
来源：http://rgt.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://gjp.fehbvm.com

for (i in 1..10) println(i)
来源：http://gwm.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://bdd.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://teg.hysaishi.cn

[T16] Swift：Hello World
来源：http://ygx.daxiang520.top

print("Hello")
来源：http://xzj.uphjek.com

[T17] Swift：变量与常量
来源：http://ols.yuxming.cn

var a = 1;  let b = 2
来源：http://uvv.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://ldl.shanyushiyangkeji.top

"值: \(b)"
来源：http://jib.jianghu66.top

[T19] Swift：可选绑定
来源：http://mgs.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://oih.nwbrower.top

[T20] Swift：数组操作
来源：http://mrx.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://sbf.gzhubu.top

[T21] Swift：遍历
来源：http://yhy.dashuyun.cn

for x in a { print(x) }
来源：http://hja.zdbjq.cn

[T22] Swift：字典
来源：http://hwy.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ayx.aizwys.cn

[T23] Swift：函数
来源：http://gef.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ksh.zhiwuduotai.top

[T24] Swift：闭包
来源：http://uij.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://can.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://czb.jinghuilouyu.cn

struct P { var x: Int }
来源：http://fjz.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://cjx.yangfankeji.com

class A: Base { override func f() {} }
来源：http://ohs.ehwqpu.com

[T27] Swift：错误处理
来源：http://vkq.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://ycq.iojbl.cn

[T28] Swift：枚举
来源：http://dyt.quarkkingdee.top

enum Color { case red, green }
来源：http://ewg.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://kwj.zdbjq.cn

guard let x = opt else { return }
来源：http://pbv.gotoacloud.top

[T30] Swift：协议
来源：http://aqu.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://jxc.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://nps.fengsongda.top

print("Hello")
来源：http://ude.cdnleiting.top

[T32] Lua：局部变量
来源：http://eoo.sysykeji.top

local a = 1
来源：http://qso.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://has.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lzp.bjfxy.top

[T34] Lua：遍历表
来源：http://ivd.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qyw.zhongyouzk.top

[T35] Lua：字典表
来源：http://qsj.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://xvp.hnqzz.top

[T36] Lua：函数
来源：http://aaz.xinyue.icu

function add(a, b) return a + b end
来源：http://dof.pycfn.com

[T37] Lua：字符串拼接
来源：http://gby.pengpengdd.cyou

"a" .. "b"
来源：http://hku.yvedp.cn

[T38] Lua：条件
来源：http://zzl.tian-w.cn

if x > 0 then print("正") end
来源：http://qgo.aibaodan.cn

[T39] Lua：模式匹配
来源：http://rvv.xziqi.cn

string.find(s, "%d+")
来源：http://adt.shzxlz.cn

[T40] Lua：元表
来源：http://fsw.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://iin.jinqigfzy.top


<!-- 参考信息 -->