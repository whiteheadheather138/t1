代发 wailian999

cmd >/dev/null 2>&1
来源：http://ynb.bjfxy.top

[R42] 输入重定向
来源：http://yvq.cashguo.top

wc -l < a.txt
来源：http://lbz.xinyue.icu

[R43] 按名字查找文件
来源：http://vhu.mhx1999.top

find . -name "*.log" -type f
来源：http://cgm.dashuyun.cn

[R44] 按修改时间查找
来源：http://akr.xziqi.cn

find . -mtime -7 -type f
来源：http://fko.ywan-chungtsiang.top

[R45] 批量删除
来源：http://qbf.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://tjr.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://pxn.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sss.vehdjk.com

[R47] sed 单行替换
来源：http://tta.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://aga.vehdjk.com

[R48] awk 取指定列
来源：http://xbw.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://fbr.yj20258.top

[R49] awk 带条件
来源：http://gly.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ftb.yueranfly.top

[R50] awk 求和
来源：http://xlx.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aku.chenlongwang.top

[R51] 排序去重取前几
来源：http://nel.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jdz.bbcook.cn

[R52] 统计行数
来源：http://rca.cashguo.top

wc -l a.txt
来源：http://rfk.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://pjd.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hsc.birdmap.top

[R54] 比较两个文件
来源：http://jyr.bbcook.cn

diff a.txt b.txt
来源：http://qkh.yongpay.top

[R55] 压缩与解压
来源：http://hsw.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fqk.pycfn.com

[R56] 远程拷贝
来源：http://got.pengpengdd.cyou

scp file user@host:/path/
来源：http://ldf.ydzc1.top

[R57] 远程执行命令
来源：http://kdz.dashuyun.cn

ssh user@host 'uptime'
来源：http://njm.shanyushiyangtech.top

[R58] 下载文件
来源：http://eor.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://psy.fzhhl.top

[R59] 发 POST JSON
来源：http://pty.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ult.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://hqj.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yni.jqgfzy.top

[R61] 磁盘占用
来源：http://clf.tarul.cn

df -h;  du -sh *
来源：http://lli.zdqjudy.top

[R62] 找最占空间的文件
来源：http://nrt.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://eqd.yj20258888.top

[R63] 内存与进程
来源：http://wyu.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://gjd.feifeiyinyue.top

[R64] 结束进程
来源：http://kmz.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://she.yueranfly.top

[R65] 查看端口占用
来源：http://elc.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cuw.cdnleiting.top

[R66] 定时任务
来源：http://srh.hammf.cn

crontab -e;  crontab -l
来源：http://mkz.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://sgs.ydzc1.top

openssl rand -hex 16
来源：http://yqx.zycfv.cn

[R68] 计算文件校验值
来源：http://lvx.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://ubi.zhijiandao.cn

[R69] 生成随机密码
来源：http://qbu.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://lvu.sweek.top

[R70] 时间戳与互转
来源：http://hqo.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://yvv.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://xol.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rem.fengsongda.top

[R72] 等待端口就绪
来源：http://zef.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://psv.fanxiaobao.xyz

[R73] 分割大日志
来源：http://vwu.fzhhl.top

split -l 1000 big.log part_
来源：http://crz.nanxuanxn.top

[R74] 批量重命名
来源：http://mll.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jzq.fehbvm.com

[R75] 导出环境变量
来源：http://yzx.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://slc.smart0.xyz

[R76] 使用临时文件
来源：http://oya.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://btv.yuxming.cn

[R77] 读取用户输入
来源：http://kmf.pycfn.com

read -rp "请输入: " ans
来源：http://gcl.gogol.net.cn

[R78] 交互式菜单
来源：http://hux.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dek.svipenyu.cn

[R79] 解析命令行选项
来源：http://sns.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ptr.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://pwr.daxiang520.top

time ./run.sh
来源：http://nhb.hnqzz.top

================================================================================
来源：http://nvt.yueranfly.top

S. C / C++ 专题
来源：http://fhs.ywan-chungtsiang.top

================================================================================
来源：http://dkc.zhengqikj.top

[S01] C：Hello World
来源：http://yee.sufxvd.cn

#include <stdio.h>
来源：http://mji.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zmk.sxryk.cn

[S02] C：变量与格式化输出
来源：http://vai.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://esw.guannengcc.top

[S03] C：读入整数
来源：http://qer.xylfe.cn

int x; scanf("%d", &x);
来源：http://dtl.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://nix.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://rgl.jianghu66.top

[S05] C：字符串长度
来源：http://ewo.zhongyouzk.top

strlen(s)
来源：http://oov.zycfv.cn

[S06] C：字符串比较
来源：http://dol.tarul.cn

strcmp(a, b) == 0
来源：http://yue.jinqigufen.top

[S07] C：数组遍历求和
来源：http://eir.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mpm.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://muu.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fzq.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://kro.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rpb.sufxvd.cn

[S10] C：指针与解引用
来源：http://uoo.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://iap.jyoumei.cn

[S11] C：逐行读文件
来源：http://wir.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ddu.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rhw.bbcook.cn

fclose(f);
来源：http://aei.xuanzx.com

[S12] C：写文件
来源：http://bca.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pmg.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://uzc.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lpg.sxryk.cn

[S14] C：枚举
来源：http://kmi.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://nqm.meibo888.top

[S15] C：类型转换
来源：http://ent.gogol.net.cn

(double) a / b
来源：http://xvt.hongshengwenyu.top

[S16] C：位操作置位
来源：http://aso.yonumen.top

x |= (1 << 3);
来源：http://ocp.xylfe.cn

[S17] C：安全拼接字符串
来源：http://xng.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fdz.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://dao.sjlbkw.cn

int main(int argc, char **argv)
来源：http://lak.sxryk.cn

[S19] C：快速排序
来源：http://tua.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://one.jyoumei.cn

[S20] C：二分查找
来源：http://vpo.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fwl.aizwys.cn

[S21] C：字符类别判断
来源：http://qmv.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://elt.jqgufenzy.top

[S22] C：字符串转数字
来源：http://ihg.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://lib.quarkkingdee.top

[S23] C：随机数
来源：http://xch.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zvd.iojbl.cn

[S24] C：获取本地时间
来源：http://kra.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dhp.hammf.cn

[S25] C：内存拷贝
来源：http://frs.yj20258.top

memcpy(dst, src, n);
来源：http://eim.yueranfly.top

[S26] C：内存清零
来源：http://vwx.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://rlv.yongpay.top

[S27] C：定义常量
来源：http://mbt.sxryk.cn

const double PI = 3.14159;
来源：http://hll.yonumen.top

[S28] C：静态变量
来源：http://oki.iojbl.cn

static int counter = 0;
来源：http://glm.epnwcf.com

[S29] C：变参函数
来源：http://kna.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pvr.jinqigfzy.top

[S30] C：头文件保护
来源：http://wht.sxryk.cn

#ifndef X_H
来源：http://gnp.fehbvm.com

#define X_H
来源：http://ius.hammf.cn

#endif
来源：http://tsq.hysaishi.cn

[S31] C++：Hello World
来源：http://cun.meibo888.top

#include <iostream>
来源：http://tka.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://nbi.hesvh.cn

[S32] C++：字符串
来源：http://dnv.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://szy.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://wwo.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jvw.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://ffp.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rzx.aizwys.cn

[S35] C++：map
来源：http://uqq.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ceo.jqgfzy.top

[S36] C++：unordered_map
来源：http://jlo.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://acp.fzhhl.top

[S37] C++：set
来源：http://kzu.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fpb.birdmap.top

[S38] C++：排序
来源：http://trj.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://xkz.pycfn.com

[S39] C++：自定义比较器排序
来源：http://xri.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rzv.chenzaomai.com

[S40] C++：查找元素
来源：http://duz.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://euw.fktsv.cn

[S41] C++：类与构造函数
来源：http://dre.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kpz.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://oci.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://gzx.redwolf501.top

[S43] C++：智能指针
来源：http://wur.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://zwv.redwolf501.top

[S44] C++：引用传参
来源：http://tvl.xuanzx.com

void inc(int &x) { ++x; }
来源：http://gnf.yongpay.top

[S45] C++：lambda
来源：http://llb.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oyp.hcnkem.com

[S46] C++：函数模板
来源：http://ttc.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://llb.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://lvk.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zak.hcnkem.com

[S48] C++：逐行读文件
来源：http://xkx.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jhd.daria6918.cn

while (std::getline(in, line)) { }
来源：http://gsz.fengsongda.top

[S49] C++：写文件
来源：http://sfz.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tpm.daria6918.cn

[S50] C++：格式化数字
来源：http://dlw.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xqo.ppjwa.cn

[S51] C++：显式类型转换
来源：http://vqb.yonumen.top

static_cast<double>(a) / b
来源：http://ktx.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://eki.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://otw.gzhubu.top

[S53] C++：移动语义
来源：http://zlu.yongpay.top

std::vector<int> w = std::move(v);
来源：http://ees.hysaishi.cn

[S54] C++：异常处理
来源：http://wzv.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jdy.fzhhl.top

[S55] C++：结构化绑定
来源：http://wjx.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://wpc.jianghu66.top

[S56] C++：optional
来源：http://wjn.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbi.nanxinkj.top

[S57] C++：编译期常量
来源：http://bbd.jianghu66.top

constexpr int N = 10;
来源：http://kvr.quarkkingdee.top

[S58] C++：命名空间
来源：http://vxp.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://zel.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://xww.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mtj.meibo888.top

[S60] C++：遍历并删除元素
来源：http://vmj.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://miu.yj20258888.top

================================================================================
来源：http://yns.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://emh.zycfv.cn

================================================================================
来源：http://nrm.yvedp.cn

[T01] Kotlin：Hello World
来源：http://lya.yangfankeji.com

println("Hello")
来源：http://vay.redwolf501.top

[T02] Kotlin：变量
来源：http://txh.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mmk.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://ksi.zhoulong.xyz

"值: $b"
来源：http://dlz.cqqwz.cn

[T04] Kotlin：空安全
来源：http://ivb.andypj.xyz

val n: String? = null;  n?.length
来源：http://ebp.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://sua.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bku.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://irj.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rkc.cashguo.top

[T07] Kotlin：集合过滤
来源：http://mgh.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wco.daria6918.cn

[T08] Kotlin：数据类
来源：http://uxs.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://hot.hammf.cn

[T09] Kotlin：扩展函数
来源：http://gcu.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://cke.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://jor.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vzr.xuanzx.com

[T11] Kotlin：协程
来源：http://bgg.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nok.ivvv.top

[T12] Kotlin：解构声明
来源：http://gua.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://thq.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://pqc.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://sqd.52xcode.cn

[T14] Kotlin：循环
来源：http://lwm.yonumen.top

for (i in 1..10) println(i)
来源：http://sph.chenlongwang.top

[T15] Kotlin：接口
来源：http://ojo.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://lto.yuanzhike.top

[T16] Swift：Hello World
来源：http://tnv.zycfv.cn

print("Hello")
来源：http://tpp.birdmap.top

[T17] Swift：变量与常量
来源：http://ukm.zhongyouzk.top

var a = 1;  let b = 2
来源：http://zlp.tarul.cn

[T18] Swift：字符串插值
来源：http://den.hammf.cn

"值: \(b)"
来源：http://qkm.havefunace.top

[T19] Swift：可选绑定
来源：http://gfd.c1oappe.top

if let n = opt { print(n) }
来源：http://xkw.aibaodan.cn

[T20] Swift：数组操作
来源：http://dcu.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vuy.mhx1999.top

[T21] Swift：遍历
来源：http://pxf.birdmap.top

for x in a { print(x) }
来源：http://etr.yangfankeji.com

[T22] Swift：字典
来源：http://cwa.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ibm.feifeiyinyue.top

[T23] Swift：函数
来源：http://tox.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://exb.smart0.xyz

[T24] Swift：闭包
来源：http://ggw.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mrb.gogol.net.cn

[T25] Swift：结构体
来源：http://clx.svipenyu.cn

struct P { var x: Int }
来源：http://bhb.mhx1999.top

[T26] Swift：类与重写
来源：http://wih.hcnkem.com

class A: Base { override func f() {} }
来源：http://mfa.meibo888.top

[T27] Swift：错误处理
来源：http://khj.tanke756.top

do { try f() } catch { print(error) }
来源：http://htm.xziqi.cn

[T28] Swift：枚举
来源：http://wng.cdnleiting.top

enum Color { case red, green }
来源：http://dwk.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://jyb.hongshengwenyu.top

guard let x = opt else { return }
来源：http://bjb.zhixingplan.top

[T30] Swift：协议
来源：http://lnd.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://fdm.daria6918.cn

[T31] Lua：Hello World
来源：http://akb.gzhubu.top

print("Hello")
来源：http://ucj.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://onp.snrcjt.cn

local a = 1
来源：http://fgj.jianghu66.top

[T33] Lua：表（数组）
来源：http://uam.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://daj.meibo888.top

[T34] Lua：遍历表
来源：http://mpi.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://iik.yvedp.cn

[T35] Lua：字典表
来源：http://xaa.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://tca.epnwcf.com

[T36] Lua：函数
来源：http://qjm.quarkkingdee.top

function add(a, b) return a + b end
来源：http://sxz.havefunace.top

[T37] Lua：字符串拼接
来源：http://hgd.fehbvm.com

"a" .. "b"
来源：http://njx.zhengqikj.top

[T38] Lua：条件
来源：http://kgm.zhongyouzk.top

if x > 0 then print("正") end
来源：http://yht.yj20258.top

[T39] Lua：模式匹配
来源：http://pxl.jqgfzy.top

string.find(s, "%d+")
来源：http://ico.fehbvm.com

[T40] Lua：元表
来源：http://bps.52xcode.cn

setmetatable({}, { __index = base })
来源：http://zqi.yj202588.top

[T41] Perl：Hello World
来源：http://oxf.jianghu66.top

print "Hello\n";
来源：http://osn.jyoumei.cn

[T42] Perl：变量类型
来源：http://xtx.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://npc.bjfxy.top

[T43] Perl：字符串插值
来源：http://zms.fehbvm.com

"值: $a"
来源：http://aap.jiagoushi.top

[T44] Perl：条件
来源：http://znd.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://hyl.yonumen.top


<!-- 参考信息 -->