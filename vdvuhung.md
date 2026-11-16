代发 wailian999

files=$(ls -1)
来源：http://ciu.316326.xyz

[R38] 管道串联
来源：http://nvi.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://kou.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://prk.yongpay.top

cmd > out.log 2>&1
来源：http://vuq.sjlbkw.cn

[R40] 追加写日志
来源：http://erh.bbcook.cn

echo "log" >> out.log
来源：http://uiz.xziqi.cn

[R41] 丢弃输出
来源：http://ktt.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://qpr.ehwqpu.com

[R42] 输入重定向
来源：http://acm.daria6918.cn

wc -l < a.txt
来源：http://cbw.sysykeji.top

[R43] 按名字查找文件
来源：http://ify.hesvh.cn

find . -name "*.log" -type f
来源：http://iso.hnqzz.top

[R44] 按修改时间查找
来源：http://dav.yvedp.cn

find . -mtime -7 -type f
来源：http://yvh.ppjwa.cn

[R45] 批量删除
来源：http://ixb.yueranfly.top

find . -name "*.tmp" -delete
来源：http://xyd.hysaishi.cn

[R46] 递归替换文件内容
来源：http://yfw.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://byk.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://tnf.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fin.gzhubu.top

[R48] awk 取指定列
来源：http://vzq.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://jhm.birdmap.top

[R49] awk 带条件
来源：http://zhh.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pnp.ybcxt.top

[R50] awk 求和
来源：http://cyi.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://ocg.xuanzx.com

[R51] 排序去重取前几
来源：http://efl.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xhu.ybcxt.top

[R52] 统计行数
来源：http://yev.daria6918.cn

wc -l a.txt
来源：http://lgk.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://fdd.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gvo.chenzaomai.com

[R54] 比较两个文件
来源：http://izt.0kj1m.cn

diff a.txt b.txt
来源：http://szy.dianchejie.cn

[R55] 压缩与解压
来源：http://jei.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tad.ybcxt.top

[R56] 远程拷贝
来源：http://kip.yj20258888.top

scp file user@host:/path/
来源：http://lnl.hysaishi.cn

[R57] 远程执行命令
来源：http://ekj.zdqjudy.top

ssh user@host 'uptime'
来源：http://fgn.yueranfly.top

[R58] 下载文件
来源：http://htj.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://txm.haohaochexian.top

[R59] 发 POST JSON
来源：http://tpt.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://och.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://lhs.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vbz.cqqwz.cn

[R61] 磁盘占用
来源：http://erw.0kj1m.cn

df -h;  du -sh *
来源：http://glr.yuanzhike.top

[R62] 找最占空间的文件
来源：http://rci.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://afx.fzhhl.top

[R63] 内存与进程
来源：http://zxa.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://avr.snrcjt.cn

[R64] 结束进程
来源：http://fut.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://nnj.pycfn.com

[R65] 查看端口占用
来源：http://hmx.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xyv.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://hru.fzhhl.top

crontab -e;  crontab -l
来源：http://oyb.guannengcc.top

[R67] 生成随机十六进制串
来源：http://vbl.aizwys.cn

openssl rand -hex 16
来源：http://tpk.yanxiufei.cn

[R68] 计算文件校验值
来源：http://eqb.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://vjg.vqdsnc.cn

[R69] 生成随机密码
来源：http://wyc.ybcxt.top

head -c 16 /dev/urandom | base64
来源：http://pya.aibaodan.cn

[R70] 时间戳与互转
来源：http://uyh.fengsongda.top

date +%s;  date -d @1700000000
来源：http://pdn.xziqi.cn

[R71] 日期格式化
来源：http://wjf.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fpb.mhx1999.top

[R72] 等待端口就绪
来源：http://uol.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uby.ehwqpu.com

[R73] 分割大日志
来源：http://jnk.tanke756.top

split -l 1000 big.log part_
来源：http://pqw.nwbrower.top

[R74] 批量重命名
来源：http://vrk.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gvz.sxryk.cn

[R75] 导出环境变量
来源：http://rzi.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://bzl.chenzaomai.com

[R76] 使用临时文件
来源：http://sbc.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cbu.zhixingplan.top

[R77] 读取用户输入
来源：http://gos.mhx1999.top

read -rp "请输入: " ans
来源：http://mix.fktsv.cn

[R78] 交互式菜单
来源：http://tzp.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fch.ctjpmb.com

[R79] 解析命令行选项
来源：http://vds.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uhg.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://muc.sweek.top

time ./run.sh
来源：http://cfr.dianchejie.cn

================================================================================
来源：http://sts.316326.xyz

S. C / C++ 专题
来源：http://sph.hesvh.cn

================================================================================
来源：http://zgp.fengsongda.top

[S01] C：Hello World
来源：http://jpq.ybcxt.top

#include <stdio.h>
来源：http://dbq.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ife.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://cgk.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://swk.yangfankeji.com

[S03] C：读入整数
来源：http://lgd.nwbrower.top

int x; scanf("%d", &x);
来源：http://dcy.jqgfzy.top

[S04] C：字符串复制
来源：http://prh.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://how.zdbjq.cn

[S05] C：字符串长度
来源：http://nvz.birdmap.top

strlen(s)
来源：http://lgu.dianchejie.cn

[S06] C：字符串比较
来源：http://qrw.jinqigufen.top

strcmp(a, b) == 0
来源：http://egt.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://tpp.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rtb.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://bkl.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cad.sweek.top

[S09] C：结构体定义与初始化
来源：http://ojo.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aaf.shzxlz.cn

[S10] C：指针与解引用
来源：http://yur.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://hec.jyoumei.cn

[S11] C：逐行读文件
来源：http://wzv.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ucf.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jrd.aizwys.cn

fclose(f);
来源：http://abg.birdmap.top

[S12] C：写文件
来源：http://lyt.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kiq.zycfv.cn

[S13] C：宏定义
来源：http://yku.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rsb.aibaodan.cn

[S14] C：枚举
来源：http://ghe.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://mlg.zhengqikj.top

[S15] C：类型转换
来源：http://nsy.svipenyu.cn

(double) a / b
来源：http://hlk.nanxuanxn.top

[S16] C：位操作置位
来源：http://vcf.sufxvd.cn

x |= (1 << 3);
来源：http://xvw.fzhhl.top

[S17] C：安全拼接字符串
来源：http://cvz.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gso.chenlongwang.top

[S18] C：命令行参数
来源：http://reo.nanxuanxn.top

int main(int argc, char **argv)
来源：http://qtm.uphjek.com

[S19] C：快速排序
来源：http://xew.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wqp.ydzc1.top

[S20] C：二分查找
来源：http://juu.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cjo.zhengqikj.top

[S21] C：字符类别判断
来源：http://hmg.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdg.52xcode.cn

[S22] C：字符串转数字
来源：http://ter.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xor.smart0.xyz

[S23] C：随机数
来源：http://bsx.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rub.aibaodan.cn

[S24] C：获取本地时间
来源：http://tid.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cgs.guannengcc.top

[S25] C：内存拷贝
来源：http://rln.316326.xyz

memcpy(dst, src, n);
来源：http://fjk.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://cpj.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://txv.sjlbkw.cn

[S27] C：定义常量
来源：http://vwn.bbcook.cn

const double PI = 3.14159;
来源：http://lnk.feifeiyinyue.top

[S28] C：静态变量
来源：http://hah.yvedp.cn

static int counter = 0;
来源：http://bcv.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://mzv.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mcj.zhijiandao.cn

[S30] C：头文件保护
来源：http://mdg.xinyue.icu

#ifndef X_H
来源：http://kgp.hammf.cn

#define X_H
来源：http://nwe.jinqigufen.top

#endif
来源：http://smp.ydzc1.top

[S31] C++：Hello World
来源：http://nww.xylfe.cn

#include <iostream>
来源：http://atx.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://uui.daxiang520.top

[S32] C++：字符串
来源：http://tdg.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://bcm.fktsv.cn

[S33] C++：vector 增删
来源：http://ggu.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kwc.c1oappe.top

[S34] C++：遍历 vector
来源：http://aop.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://gyt.sufxvd.cn

[S35] C++：map
来源：http://ksj.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kra.gogol.net.cn

[S36] C++：unordered_map
来源：http://pcs.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nas.yuanzhike.top

[S37] C++：set
来源：http://lav.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cnu.ybcxt.top

[S38] C++：排序
来源：http://svx.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://ank.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://lpe.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://msy.xuanzx.com

[S40] C++：查找元素
来源：http://wuk.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ehl.sxryk.cn

[S41] C++：类与构造函数
来源：http://mzt.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uma.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://luu.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://jqf.smart0.xyz

[S43] C++：智能指针
来源：http://jce.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://bir.chenlongwang.top

[S44] C++：引用传参
来源：http://xbe.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://shg.daxiang520.top

[S45] C++：lambda
来源：http://vuf.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ovc.dianchejie.cn

[S46] C++：函数模板
来源：http://evw.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://skw.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://klx.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oxs.meibo888.top

[S48] C++：逐行读文件
来源：http://adv.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://ofh.yvedp.cn

while (std::getline(in, line)) { }
来源：http://vmp.guannengcc.top

[S49] C++：写文件
来源：http://uov.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xdi.52xcode.cn

[S50] C++：格式化数字
来源：http://yza.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mbm.hesvh.cn

[S51] C++：显式类型转换
来源：http://jgd.xuanzx.com

static_cast<double>(a) / b
来源：http://opt.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://zoh.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://ehf.yj20258888.top

[S53] C++：移动语义
来源：http://nls.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://ovx.ydjk.org.cn

[S54] C++：异常处理
来源：http://ntq.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxo.zhixingplan.top

[S55] C++：结构化绑定
来源：http://nry.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bkv.birdmap.top

[S56] C++：optional
来源：http://bgn.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pku.tanke756.top

[S57] C++：编译期常量
来源：http://pus.ehwqpu.com

constexpr int N = 10;
来源：http://acz.ydzc1.top

[S58] C++：命名空间
来源：http://wsx.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://typ.jyoumei.cn

[S59] C++：静态断言
来源：http://dce.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pvl.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://xtz.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rra.jqgfzy.top

================================================================================
来源：http://fru.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ihi.guowangkeji.top

================================================================================
来源：http://cem.sysykeji.top

[T01] Kotlin：Hello World
来源：http://qwn.jqgfzy.top

println("Hello")
来源：http://xtr.ivvv.top

[T02] Kotlin：变量
来源：http://uwz.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbv.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://cqb.chenzaomai.com

"值: $b"
来源：http://knv.yonumen.top

[T04] Kotlin：空安全
来源：http://sxz.sysykeji.top

val n: String? = null;  n?.length
来源：http://ifj.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://jkx.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xod.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://yiy.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vtr.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://mbk.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uss.fzhhl.top

[T08] Kotlin：数据类
来源：http://tha.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://kvy.yongpay.top

[T09] Kotlin：扩展函数
来源：http://zuu.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://mva.daria6918.cn

[T10] Kotlin：默认参数
来源：http://xat.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://xlq.fengsongda.top

[T11] Kotlin：协程
来源：http://eql.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jex.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://qtv.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://wge.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://zin.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://vyi.sysykeji.top

[T14] Kotlin：循环
来源：http://bgc.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://cri.kuanghao11.cn

[T15] Kotlin：接口
来源：http://zvr.bbcook.cn

interface Shape { fun area(): Double }
来源：http://xrz.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://zmf.quarkkingdee.top

print("Hello")
来源：http://wic.vehdjk.com

[T17] Swift：变量与常量
来源：http://ixu.tianlin.xyz

var a = 1;  let b = 2
来源：http://wjf.ctjpmb.com

[T18] Swift：字符串插值
来源：http://heq.zycfv.cn

"值: \(b)"
来源：http://adz.xziqi.cn

[T19] Swift：可选绑定
来源：http://tri.fktsv.cn

if let n = opt { print(n) }
来源：http://gnc.jqgfzy.top

[T20] Swift：数组操作
来源：http://koo.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lea.svipenyu.cn

[T21] Swift：遍历
来源：http://rbj.redwolf501.top

for x in a { print(x) }
来源：http://aal.haohaochexian.top

[T22] Swift：字典
来源：http://fxj.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://zpt.vehdjk.com

[T23] Swift：函数
来源：http://xyv.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ecu.iojbl.cn

[T24] Swift：闭包
来源：http://dch.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qdt.shangyingyoupin.top

[T25] Swift：结构体
来源：http://kba.svipenyu.cn

struct P { var x: Int }
来源：http://igt.vehdjk.com

[T26] Swift：类与重写
来源：http://seb.fehbvm.com

class A: Base { override func f() {} }
来源：http://vrx.zhoulong.xyz

[T27] Swift：错误处理
来源：http://wci.xuanzx.com

do { try f() } catch { print(error) }
来源：http://mwo.jqgufenzy.top

[T28] Swift：枚举
来源：http://tfg.jinqigufen.top

enum Color { case red, green }
来源：http://rhp.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://mku.gzhubu.top

guard let x = opt else { return }
来源：http://wju.sweek.top

[T30] Swift：协议
来源：http://xsq.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://qfn.kuanghao11.cn

[T31] Lua：Hello World
来源：http://hzj.9152youxi.cn

print("Hello")
来源：http://ayx.hnxiangtu.top

[T32] Lua：局部变量
来源：http://iae.ivvv.top

local a = 1
来源：http://etl.mhx1999.top

[T33] Lua：表（数组）
来源：http://gcu.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ffw.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://aoa.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zud.ivvv.top

[T35] Lua：字典表
来源：http://tzf.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://lkw.yonumen.top

[T36] Lua：函数
来源：http://gjp.zycfv.cn

function add(a, b) return a + b end
来源：http://axp.sxryk.cn

[T37] Lua：字符串拼接
来源：http://wzh.jianghu66.top

"a" .. "b"
来源：http://kpg.tian-w.cn

[T38] Lua：条件
来源：http://dmi.xziqi.cn

if x > 0 then print("正") end
来源：http://vyt.hnqzz.top

[T39] Lua：模式匹配
来源：http://tmn.cdnleiting.top

string.find(s, "%d+")
来源：http://uyq.guannengcc.top

[T40] Lua：元表
来源：http://iba.redwolf501.top

setmetatable({}, { __index = base })
来源：http://cza.yuanzhike.top


<!-- 参考信息 -->