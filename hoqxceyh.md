代发 wailian999

files=$(ls -1)
来源：http://mtj.fzhhl.top

[R38] 管道串联
来源：http://vxu.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://azj.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://kyq.cheryme.top

cmd > out.log 2>&1
来源：http://vza.nwbrower.top

[R40] 追加写日志
来源：http://zis.ehwqpu.com

echo "log" >> out.log
来源：http://scn.ydzc1.top

[R41] 丢弃输出
来源：http://hue.ivvv.top

cmd >/dev/null 2>&1
来源：http://ddj.316326.xyz

[R42] 输入重定向
来源：http://xsv.zhoulong.xyz

wc -l < a.txt
来源：http://kxw.yuxming.cn

[R43] 按名字查找文件
来源：http://paf.zhoulong.xyz

find . -name "*.log" -type f
来源：http://okr.yfazqb.com

[R44] 按修改时间查找
来源：http://jij.ybcxt.top

find . -mtime -7 -type f
来源：http://vae.tian-w.cn

[R45] 批量删除
来源：http://tsv.hammf.cn

find . -name "*.tmp" -delete
来源：http://vau.sysykeji.top

[R46] 递归替换文件内容
来源：http://pcf.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zht.sxryk.cn

[R47] sed 单行替换
来源：http://abx.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yvg.0kj1m.cn

[R48] awk 取指定列
来源：http://gep.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://fcu.daxiang520.top

[R49] awk 带条件
来源：http://dzr.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://znk.xuanzx.com

[R50] awk 求和
来源：http://aax.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sro.vehdjk.com

[R51] 排序去重取前几
来源：http://qfv.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ylm.zhaomingkeji.xyz

[R52] 统计行数
来源：http://det.cheryme.top

wc -l a.txt
来源：http://kgj.yonumen.top

[R53] 查看文件头与实时尾
来源：http://mtb.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bln.ydzc1.top

[R54] 比较两个文件
来源：http://mto.yanxiufei.cn

diff a.txt b.txt
来源：http://kfq.feifeiyinyue.top

[R55] 压缩与解压
来源：http://dos.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pkc.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://ntd.chenlongwang.top

scp file user@host:/path/
来源：http://xfc.chenjidiqi.icu

[R57] 远程执行命令
来源：http://kqj.hywenlv.cn

ssh user@host 'uptime'
来源：http://xue.fengsongda.top

[R58] 下载文件
来源：http://lmm.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://unc.cheryme.top

[R59] 发 POST JSON
来源：http://eem.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pbc.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://tba.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://smo.cheryme.top

[R61] 磁盘占用
来源：http://sgf.9152youxi.cn

df -h;  du -sh *
来源：http://ydn.cdnleiting.top

[R62] 找最占空间的文件
来源：http://ulw.cheryme.top

du -ah . | sort -rh | head -10
来源：http://txd.svipenyu.cn

[R63] 内存与进程
来源：http://vtn.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://skg.havefunace.top

[R64] 结束进程
来源：http://waf.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://pjs.9152youxi.cn

[R65] 查看端口占用
来源：http://nnh.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cpj.xylfe.cn

[R66] 定时任务
来源：http://ynr.cucudq.cn

crontab -e;  crontab -l
来源：http://gbb.hcnkem.com

[R67] 生成随机十六进制串
来源：http://xze.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://ohv.nanxuanxn.top

[R68] 计算文件校验值
来源：http://cmd.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tqu.uphjek.com

[R69] 生成随机密码
来源：http://fyv.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://pjl.ppjwa.cn

[R70] 时间戳与互转
来源：http://jwg.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://hkn.shuidangran.top

[R71] 日期格式化
来源：http://fhf.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yza.316326.xyz

[R72] 等待端口就绪
来源：http://bma.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fgn.sysykeji.top

[R73] 分割大日志
来源：http://mqy.uphjek.com

split -l 1000 big.log part_
来源：http://rcx.ybcxt.top

[R74] 批量重命名
来源：http://rpf.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tja.zdqjudy.top

[R75] 导出环境变量
来源：http://mhg.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://mms.feifeiyinyue.top

[R76] 使用临时文件
来源：http://fco.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wwv.zycfv.cn

[R77] 读取用户输入
来源：http://kwz.jinqigufen.top

read -rp "请输入: " ans
来源：http://zqn.vehdjk.com

[R78] 交互式菜单
来源：http://alp.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fzi.hnxiangtu.top

[R79] 解析命令行选项
来源：http://bgw.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhz.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://flj.zhoulong.xyz

time ./run.sh
来源：http://nfa.yvedp.cn

================================================================================
来源：http://mrn.daxiang520.top

S. C / C++ 专题
来源：http://agy.hfpthk.cn

================================================================================
来源：http://maa.mhx1999.top

[S01] C：Hello World
来源：http://jft.epnwcf.com

#include <stdio.h>
来源：http://zqg.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tik.aizwys.cn

[S02] C：变量与格式化输出
来源：http://qcg.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://hld.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://pid.52xcode.cn

int x; scanf("%d", &x);
来源：http://yqx.jinqigfzy.top

[S04] C：字符串复制
来源：http://hnh.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cct.9152youxi.cn

[S05] C：字符串长度
来源：http://bsc.xziqi.cn

strlen(s)
来源：http://ssr.yvedp.cn

[S06] C：字符串比较
来源：http://bjc.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://tdn.jiagoushi.top

[S07] C：数组遍历求和
来源：http://feb.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xyu.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://aul.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xeu.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://eee.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://swt.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://vrx.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://mzm.chenlongwang.top

[S11] C：逐行读文件
来源：http://yzp.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://wku.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://fsm.wangdashe.top

fclose(f);
来源：http://dni.wangdashe.top

[S12] C：写文件
来源：http://lil.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ntt.kuanghao11.cn

[S13] C：宏定义
来源：http://dnq.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://scm.zhaomingkeji.xyz

[S14] C：枚举
来源：http://mqk.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://opm.jlsjyb.cn

[S15] C：类型转换
来源：http://une.hammf.cn

(double) a / b
来源：http://buv.daria6918.cn

[S16] C：位操作置位
来源：http://heo.cqqwz.cn

x |= (1 << 3);
来源：http://eya.sysykeji.top

[S17] C：安全拼接字符串
来源：http://vbz.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzg.52xcode.cn

[S18] C：命令行参数
来源：http://dya.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://uwr.yongpay.top

[S19] C：快速排序
来源：http://hdi.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://cza.9152youxi.cn

[S20] C：二分查找
来源：http://boe.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sjz.bbcook.cn

[S21] C：字符类别判断
来源：http://ise.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qbl.xylfe.cn

[S22] C：字符串转数字
来源：http://bcr.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://jua.hongshengwenyu.top

[S23] C：随机数
来源：http://oez.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bqo.daria6918.cn

[S24] C：获取本地时间
来源：http://lif.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nbl.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://mua.shzxlz.cn

memcpy(dst, src, n);
来源：http://afb.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://ckp.hcnkem.com

memset(a, 0, sizeof a);
来源：http://ozb.gogol.net.cn

[S27] C：定义常量
来源：http://bgg.ehwqpu.com

const double PI = 3.14159;
来源：http://sac.hongshengwenyu.top

[S28] C：静态变量
来源：http://pks.smart0.xyz

static int counter = 0;
来源：http://ung.gogol.net.cn

[S29] C：变参函数
来源：http://vwn.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pub.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://wfo.zhaomingkeji.xyz

#ifndef X_H
来源：http://dwr.yvedp.cn

#define X_H
来源：http://yfj.yuanzhike.top

#endif
来源：http://jpb.ppjwa.cn

[S31] C++：Hello World
来源：http://cwm.sxryk.cn

#include <iostream>
来源：http://zis.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ygu.gogol.net.cn

[S32] C++：字符串
来源：http://dmd.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://wuk.snrcjt.cn

[S33] C++：vector 增删
来源：http://aqw.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cgy.jinqigufen.top

[S34] C++：遍历 vector
来源：http://jsz.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://mvc.yuanzhike.top

[S35] C++：map
来源：http://ahx.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fqd.zhongyouzk.top

[S36] C++：unordered_map
来源：http://ubg.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aoi.gaohongyu789.top

[S37] C++：set
来源：http://ujj.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dqj.daxiang520.top

[S38] C++：排序
来源：http://uru.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://bny.316326.xyz

[S39] C++：自定义比较器排序
来源：http://cge.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bod.gzhubu.top

[S40] C++：查找元素
来源：http://yyc.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tvu.52xcode.cn

[S41] C++：类与构造函数
来源：http://qws.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://shc.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://pex.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://god.xuetiantiany.cn

[S43] C++：智能指针
来源：http://heh.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://hep.yuanzhike.top

[S44] C++：引用传参
来源：http://ydm.nwbrower.top

void inc(int &x) { ++x; }
来源：http://wsa.ppjwa.cn

[S45] C++：lambda
来源：http://obx.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://hrq.cqqwz.cn

[S46] C++：函数模板
来源：http://shy.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://une.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://vnr.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jii.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://wnw.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://hpm.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://izl.shuidangran.top

[S49] C++：写文件
来源：http://zwh.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uxv.ydzc1.top

[S50] C++：格式化数字
来源：http://axo.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://myy.guannengcc.top

[S51] C++：显式类型转换
来源：http://vid.havefunace.top

static_cast<double>(a) / b
来源：http://qae.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://tqo.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://vfj.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://nbe.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://fbj.chenlongwang.top

[S54] C++：异常处理
来源：http://tir.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tpn.hysaishi.cn

[S55] C++：结构化绑定
来源：http://aip.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xns.haohaochexian.top

[S56] C++：optional
来源：http://vrr.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vzi.sjlbkw.cn

[S57] C++：编译期常量
来源：http://gms.jqgufenzy.top

constexpr int N = 10;
来源：http://ydf.shuidangran.top

[S58] C++：命名空间
来源：http://idt.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://ceg.9152youxi.cn

[S59] C++：静态断言
来源：http://pog.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hhq.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://adp.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tyd.yj202588.top

================================================================================
来源：http://cia.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hql.pycfn.com

================================================================================
来源：http://rop.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://hav.shanyushiyangkeji.top

println("Hello")
来源：http://ekv.sufxvd.cn

[T02] Kotlin：变量
来源：http://zmk.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vgc.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://qed.vqdsnc.cn

"值: $b"
来源：http://vzn.cucudq.cn

[T04] Kotlin：空安全
来源：http://obu.sxryk.cn

val n: String? = null;  n?.length
来源：http://wwb.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://lbh.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qad.hnqzz.top

[T06] Kotlin：集合映射
来源：http://fvg.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cof.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://exb.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgn.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://gma.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://bfw.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://two.316326.xyz

fun String.exclaim() = this + "!"
来源：http://vfp.redwolf501.top

[T10] Kotlin：默认参数
来源：http://cqx.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qbv.ivvv.top

[T11] Kotlin：协程
来源：http://pqr.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gxc.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://hum.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://rzx.cheryme.top

[T13] Kotlin：只读 Map
来源：http://arb.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://trl.gzhubu.top

[T14] Kotlin：循环
来源：http://mni.guannengcc.top

for (i in 1..10) println(i)
来源：http://hkq.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://ilo.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://shg.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://epm.52xcode.cn

print("Hello")
来源：http://lke.cqqwz.cn

[T17] Swift：变量与常量
来源：http://ayo.svipenyu.cn

var a = 1;  let b = 2
来源：http://mjz.yuanzhike.top

[T18] Swift：字符串插值
来源：http://cab.cqqwz.cn

"值: \(b)"
来源：http://otk.snrcjt.cn

[T19] Swift：可选绑定
来源：http://tmf.vehdjk.com

if let n = opt { print(n) }
来源：http://cse.tian-w.cn

[T20] Swift：数组操作
来源：http://mbo.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ndq.hfpthk.cn

[T21] Swift：遍历
来源：http://flf.c1oappe.top

for x in a { print(x) }
来源：http://kcw.gotoacloud.top

[T22] Swift：字典
来源：http://oqm.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://siw.zhongyouzk.top

[T23] Swift：函数
来源：http://asy.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pel.snrcjt.cn

[T24] Swift：闭包
来源：http://kzj.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://epo.zhoulong.xyz

[T25] Swift：结构体
来源：http://xhg.xinyue.icu

struct P { var x: Int }
来源：http://thk.shzxlz.cn

[T26] Swift：类与重写
来源：http://vuz.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://igj.tianlin.xyz

[T27] Swift：错误处理
来源：http://xbc.fehbvm.com

do { try f() } catch { print(error) }
来源：http://omj.nwbrower.top

[T28] Swift：枚举
来源：http://vmu.jlsjyb.cn

enum Color { case red, green }
来源：http://qps.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://soy.ppjwa.cn

guard let x = opt else { return }
来源：http://hmc.hammf.cn

[T30] Swift：协议
来源：http://jeo.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://vcd.daxiang520.top

[T31] Lua：Hello World
来源：http://tgh.sjlbkw.cn

print("Hello")
来源：http://kwl.tarul.cn

[T32] Lua：局部变量
来源：http://rkv.yonumen.top

local a = 1
来源：http://ekh.fehbvm.com

[T33] Lua：表（数组）
来源：http://kit.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://bjb.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://mqi.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zjk.zhiwuduotai.top

[T35] Lua：字典表
来源：http://jef.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://hty.guannengcc.top

[T36] Lua：函数
来源：http://iay.nwbrower.top

function add(a, b) return a + b end
来源：http://orb.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://ztt.hywenlv.cn

"a" .. "b"
来源：http://ngl.hysaishi.cn

[T38] Lua：条件
来源：http://stl.smart0.xyz

if x > 0 then print("正") end
来源：http://ihm.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://ook.zhixingplan.top

string.find(s, "%d+")
来源：http://qfs.snrcjt.cn

[T40] Lua：元表
来源：http://cqt.xuanzx.com

setmetatable({}, { __index = base })
来源：http://zat.dianchejie.cn


<!-- 参考信息 -->