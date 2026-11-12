代发 wailian999

find . -name "*.tmp" -delete
来源：http://vqq.ppjwa.cn

[R46] 递归替换文件内容
来源：http://zyr.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dgf.snrcjt.cn

[R47] sed 单行替换
来源：http://urm.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nzl.aibaodan.cn

[R48] awk 取指定列
来源：http://tmu.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://dpb.kuanghao11.cn

[R49] awk 带条件
来源：http://igt.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sth.daria6918.cn

[R50] awk 求和
来源：http://zim.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://bay.shuidangran.top

[R51] 排序去重取前几
来源：http://kep.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fmw.iojbl.cn

[R52] 统计行数
来源：http://gaz.feifeiyinyue.top

wc -l a.txt
来源：http://ili.zhijiandao.cn

[R53] 查看文件头与实时尾
来源：http://paj.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chu.quarkkingdee.top

[R54] 比较两个文件
来源：http://jbn.nwbrower.top

diff a.txt b.txt
来源：http://kre.snrcjt.cn

[R55] 压缩与解压
来源：http://ons.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eok.yonumen.top

[R56] 远程拷贝
来源：http://jcq.ybcxt.top

scp file user@host:/path/
来源：http://rvg.jinqigufen.top

[R57] 远程执行命令
来源：http://cas.bjfxy.top

ssh user@host 'uptime'
来源：http://rpm.dashuyun.cn

[R58] 下载文件
来源：http://ynv.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ijj.ydjk.org.cn

[R59] 发 POST JSON
来源：http://pxk.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oij.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://fin.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jyh.kuanghao11.cn

[R61] 磁盘占用
来源：http://hyq.sxryk.cn

df -h;  du -sh *
来源：http://ilr.shuidangran.top

[R62] 找最占空间的文件
来源：http://cet.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://mlr.jianghu66.top

[R63] 内存与进程
来源：http://zot.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://jnd.yanxiufei.cn

[R64] 结束进程
来源：http://awp.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://gfe.mhx1999.top

[R65] 查看端口占用
来源：http://leo.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ajq.zhongyouzk.top

[R66] 定时任务
来源：http://kuh.yangfankeji.com

crontab -e;  crontab -l
来源：http://zxg.sysykeji.top

[R67] 生成随机十六进制串
来源：http://whk.c1oappe.top

openssl rand -hex 16
来源：http://hxa.9152youxi.cn

[R68] 计算文件校验值
来源：http://pbh.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ebk.hesvh.cn

[R69] 生成随机密码
来源：http://dru.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://okb.vqdsnc.cn

[R70] 时间戳与互转
来源：http://dje.uphjek.com

date +%s;  date -d @1700000000
来源：http://uyw.haohaochexian.top

[R71] 日期格式化
来源：http://vwy.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://krc.smart0.xyz

[R72] 等待端口就绪
来源：http://gcd.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bmo.xuetiantiany.cn

[R73] 分割大日志
来源：http://vgi.andypj.xyz

split -l 1000 big.log part_
来源：http://lmw.0kj1m.cn

[R74] 批量重命名
来源：http://xkd.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sdq.xylfe.cn

[R75] 导出环境变量
来源：http://fxu.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://itc.yanxiufei.cn

[R76] 使用临时文件
来源：http://llq.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fzy.chenzaomai.com

[R77] 读取用户输入
来源：http://unv.wangdashe.top

read -rp "请输入: " ans
来源：http://ywh.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://fzl.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ine.tarul.cn

[R79] 解析命令行选项
来源：http://lez.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wng.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://gqo.jyoumei.cn

time ./run.sh
来源：http://dht.cdnleiting.top

================================================================================
来源：http://dzu.yanxiufei.cn

S. C / C++ 专题
来源：http://qmh.daria6918.cn

================================================================================
来源：http://cbp.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://lvo.hcnkem.com

#include <stdio.h>
来源：http://tud.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymb.cashguo.top

[S02] C：变量与格式化输出
来源：http://cij.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://jtl.vehdjk.com

[S03] C：读入整数
来源：http://amr.c1oappe.top

int x; scanf("%d", &x);
来源：http://akz.tanke756.top

[S04] C：字符串复制
来源：http://ili.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://olf.mhx1999.top

[S05] C：字符串长度
来源：http://xkp.iojbl.cn

strlen(s)
来源：http://jfe.ydjk.org.cn

[S06] C：字符串比较
来源：http://vqq.pycfn.com

strcmp(a, b) == 0
来源：http://loz.0kj1m.cn

[S07] C：数组遍历求和
来源：http://ogm.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qir.sweek.top

[S08] C：动态内存分配与释放
来源：http://sjl.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jni.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://nom.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mfv.316326.xyz

[S10] C：指针与解引用
来源：http://kym.aizwys.cn

int *p = &a;  *p = 5;
来源：http://viy.zhengqikj.top

[S11] C：逐行读文件
来源：http://dqq.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://ugh.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pqn.svipenyu.cn

fclose(f);
来源：http://fjq.yuanzhike.top

[S12] C：写文件
来源：http://hyj.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xez.ctjpmb.com

[S13] C：宏定义
来源：http://nry.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zkq.yongpay.top

[S14] C：枚举
来源：http://phr.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://ivk.mhx1999.top

[S15] C：类型转换
来源：http://ods.yj20258.top

(double) a / b
来源：http://etp.sjlbkw.cn

[S16] C：位操作置位
来源：http://zkn.yueranfly.top

x |= (1 << 3);
来源：http://qqa.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://xgk.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uya.havefunace.top

[S18] C：命令行参数
来源：http://yjl.gogol.net.cn

int main(int argc, char **argv)
来源：http://ogc.hammf.cn

[S19] C：快速排序
来源：http://jne.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tei.0kj1m.cn

[S20] C：二分查找
来源：http://wzc.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://avp.yj202588.top

[S21] C：字符类别判断
来源：http://mft.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://won.ppjwa.cn

[S22] C：字符串转数字
来源：http://jyc.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://yxr.smart0.xyz

[S23] C：随机数
来源：http://pif.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zmd.havefunace.top

[S24] C：获取本地时间
来源：http://vce.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vpi.zhoulong.xyz

[S25] C：内存拷贝
来源：http://zsq.zycfv.cn

memcpy(dst, src, n);
来源：http://qxs.hnxiangtu.top

[S26] C：内存清零
来源：http://xey.ivvv.top

memset(a, 0, sizeof a);
来源：http://tqq.xziqi.cn

[S27] C：定义常量
来源：http://vdp.nwbrower.top

const double PI = 3.14159;
来源：http://psn.jinghuilouyu.cn

[S28] C：静态变量
来源：http://gao.cdnleiting.top

static int counter = 0;
来源：http://feg.andypj.xyz

[S29] C：变参函数
来源：http://rfe.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://syr.tianlin.xyz

[S30] C：头文件保护
来源：http://gti.jqgfzy.top

#ifndef X_H
来源：http://bhk.ywan-chungtsiang.top

#define X_H
来源：http://vut.gogol.net.cn

#endif
来源：http://oft.fehbvm.com

[S31] C++：Hello World
来源：http://bat.0kj1m.cn

#include <iostream>
来源：http://xjq.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://cxd.fehbvm.com

[S32] C++：字符串
来源：http://byd.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://qsp.shzxlz.cn

[S33] C++：vector 增删
来源：http://yzs.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://arx.xinyue.icu

[S34] C++：遍历 vector
来源：http://qgv.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://hbp.cheryme.top

[S35] C++：map
来源：http://loz.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wmn.hywenlv.cn

[S36] C++：unordered_map
来源：http://mnj.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ojw.sjlbkw.cn

[S37] C++：set
来源：http://vox.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohb.cashguo.top

[S38] C++：排序
来源：http://lsw.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://mwu.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://oir.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://crq.cqqwz.cn

[S40] C++：查找元素
来源：http://ajy.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://waw.ehwqpu.com

[S41] C++：类与构造函数
来源：http://aby.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://owa.xylfe.cn

[S42] C++：继承与虚函数
来源：http://ixa.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://rqz.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://fot.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://hgv.dashuyun.cn

[S44] C++：引用传参
来源：http://ktq.redwolf501.top

void inc(int &x) { ++x; }
来源：http://vfp.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://kic.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://txc.jqgfzy.top

[S46] C++：函数模板
来源：http://onl.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://viz.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://ahw.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcm.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://etu.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://mka.birdmap.top

while (std::getline(in, line)) { }
来源：http://moc.tianlin.xyz

[S49] C++：写文件
来源：http://qra.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vsl.hcnkem.com

[S50] C++：格式化数字
来源：http://kxy.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jhe.cdnleiting.top

[S51] C++：显式类型转换
来源：http://rfo.gzhubu.top

static_cast<double>(a) / b
来源：http://dto.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://pns.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://awk.pengpengdd.cyou

[S53] C++：移动语义
来源：http://msi.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://uyt.yj20258888.top

[S54] C++：异常处理
来源：http://ghi.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ypu.ybcxt.top

[S55] C++：结构化绑定
来源：http://owj.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://irp.xziqi.cn

[S56] C++：optional
来源：http://wwz.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bpc.sysykeji.top

[S57] C++：编译期常量
来源：http://ofv.316326.xyz

constexpr int N = 10;
来源：http://yzy.birdmap.top

[S58] C++：命名空间
来源：http://vux.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://ggc.sjlbkw.cn

[S59] C++：静态断言
来源：http://dnr.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dwq.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://nao.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xoa.wangdashe.top

================================================================================
来源：http://img.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ucv.hysaishi.cn

================================================================================
来源：http://tmr.redwolf501.top

[T01] Kotlin：Hello World
来源：http://ely.nanxinkj.top

println("Hello")
来源：http://fft.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://hzq.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ipt.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://sll.yvedp.cn

"值: $b"
来源：http://jbd.mhx1999.top

[T04] Kotlin：空安全
来源：http://qta.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://epj.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://poy.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uok.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://woz.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://amf.ivvv.top

[T07] Kotlin：集合过滤
来源：http://qzx.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xcc.fengsongda.top

[T08] Kotlin：数据类
来源：http://vfc.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://zpn.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://dac.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://cbh.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://sbn.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://opv.hysaishi.cn

[T11] Kotlin：协程
来源：http://lrh.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://app.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://yaa.xuanzx.com

val (a, b) = Pair(1, 2)
来源：http://zvt.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://hhn.redwolf501.top

val m = mapOf("a" to 1)
来源：http://bsc.snrcjt.cn

[T14] Kotlin：循环
来源：http://ehb.316326.xyz

for (i in 1..10) println(i)
来源：http://rbh.sysykeji.top

[T15] Kotlin：接口
来源：http://xcu.fzhhl.top

interface Shape { fun area(): Double }
来源：http://lkm.yueranfly.top

[T16] Swift：Hello World
来源：http://tnx.cashguo.top

print("Hello")
来源：http://euw.bjfxy.top

[T17] Swift：变量与常量
来源：http://rjf.316326.xyz

var a = 1;  let b = 2
来源：http://zrd.haohaochexian.top

[T18] Swift：字符串插值
来源：http://fdk.fktsv.cn

"值: \(b)"
来源：http://xsb.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://gvs.dashuyun.cn

if let n = opt { print(n) }
来源：http://uxo.aibaodan.cn

[T20] Swift：数组操作
来源：http://qhj.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://knw.ppjwa.cn

[T21] Swift：遍历
来源：http://sng.pengpengdd.cyou

for x in a { print(x) }
来源：http://rhg.c1oappe.top

[T22] Swift：字典
来源：http://ono.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://bov.gotoacloud.top

[T23] Swift：函数
来源：http://cok.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fto.xylfe.cn

[T24] Swift：闭包
来源：http://lxc.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pab.smart0.xyz

[T25] Swift：结构体
来源：http://flu.yvedp.cn

struct P { var x: Int }
来源：http://vyk.zhoulong.xyz

[T26] Swift：类与重写
来源：http://msy.mhx1999.top

class A: Base { override func f() {} }
来源：http://abg.guannengcc.top

[T27] Swift：错误处理
来源：http://vwj.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://imd.pycfn.com

[T28] Swift：枚举
来源：http://rcg.wangshuangyany.cn

enum Color { case red, green }
来源：http://lta.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://bsu.haohaochexian.top

guard let x = opt else { return }
来源：http://bfo.wangshuangyany.cn

[T30] Swift：协议
来源：http://fab.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://siw.52xcode.cn

[T31] Lua：Hello World
来源：http://nef.sjlbkw.cn

print("Hello")
来源：http://ovw.yfazqb.com

[T32] Lua：局部变量
来源：http://hpb.cdnleiting.top

local a = 1
来源：http://mnt.sweek.top

[T33] Lua：表（数组）
来源：http://vbk.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pfi.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://tol.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xpi.xuetiantiany.cn

[T35] Lua：字典表
来源：http://rai.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://kdl.bjfxy.top

[T36] Lua：函数
来源：http://itj.c1oappe.top

function add(a, b) return a + b end
来源：http://nau.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://mwn.zhijiandao.cn

"a" .. "b"
来源：http://vau.jinghuilouyu.cn

[T38] Lua：条件
来源：http://sss.vehdjk.com

if x > 0 then print("正") end
来源：http://nrc.cheryme.top

[T39] Lua：模式匹配
来源：http://feu.52xcode.cn

string.find(s, "%d+")
来源：http://nqz.pengpengdd.cyou

[T40] Lua：元表
来源：http://xyz.yonumen.top

setmetatable({}, { __index = base })
来源：http://nng.quarkkingdee.top

[T41] Perl：Hello World
来源：http://maw.zhengqikj.top

print "Hello\n";
来源：http://eyc.gotoacloud.top

[T42] Perl：变量类型
来源：http://ppl.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ydg.birdmap.top

[T43] Perl：字符串插值
来源：http://bvg.zdbjq.cn

"值: $a"
来源：http://csu.yuanzhike.top

[T44] Perl：条件
来源：http://zyb.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://pgj.uphjek.com

[T45] Perl：数组遍历
来源：http://wlw.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://hge.fehbvm.com

[T46] Perl：哈希操作
来源：http://pmm.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://udg.wangdashe.top

[T47] Perl：正则捕获
来源：http://vev.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pkl.yvedp.cn

[T48] Perl：正则替换
来源：http://zqb.hnqzz.top

$s =~ s/old/new/g;
来源：http://ihl.haohaochexian.top


<!-- 参考信息 -->