代发 wailian999

cmd >/dev/null 2>&1
来源：http://ozu.fengsongda.top

[R42] 输入重定向
来源：http://kmm.tian-w.cn

wc -l < a.txt
来源：http://dkg.hammf.cn

[R43] 按名字查找文件
来源：http://snz.cashguo.top

find . -name "*.log" -type f
来源：http://zwz.aibaodan.cn

[R44] 按修改时间查找
来源：http://rll.nwbrower.top

find . -mtime -7 -type f
来源：http://hgp.aibaodan.cn

[R45] 批量删除
来源：http://ctd.guannengcc.top

find . -name "*.tmp" -delete
来源：http://acl.xylfe.cn

[R46] 递归替换文件内容
来源：http://fnn.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iet.zhixingplan.top

[R47] sed 单行替换
来源：http://ikz.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://hcm.316326.xyz

[R48] awk 取指定列
来源：http://pbo.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://ydp.yfazqb.com

[R49] awk 带条件
来源：http://yuy.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mad.yj20258888.top

[R50] awk 求和
来源：http://ikc.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://jzp.cashguo.top

[R51] 排序去重取前几
来源：http://cpn.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zwh.ctjpmb.com

[R52] 统计行数
来源：http://jnv.jqgfzy.top

wc -l a.txt
来源：http://csl.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://xsm.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qsa.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://gkd.zhijiandao.cn

diff a.txt b.txt
来源：http://skg.chenlongwang.top

[R55] 压缩与解压
来源：http://ldb.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xng.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://xbr.havefunace.top

scp file user@host:/path/
来源：http://mny.yj20258.top

[R57] 远程执行命令
来源：http://oaj.smart0.xyz

ssh user@host 'uptime'
来源：http://etc.ppjwa.cn

[R58] 下载文件
来源：http://wtc.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://plb.ppjwa.cn

[R59] 发 POST JSON
来源：http://vai.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwn.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://zqr.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nqh.aibaodan.cn

[R61] 磁盘占用
来源：http://xyt.yj202588.top

df -h;  du -sh *
来源：http://fzu.zdbjq.cn

[R62] 找最占空间的文件
来源：http://tom.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://ifs.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://tzq.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://hcp.xziqi.cn

[R64] 结束进程
来源：http://kqo.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://eku.ehwqpu.com

[R65] 查看端口占用
来源：http://fyw.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://swc.zycfv.cn

[R66] 定时任务
来源：http://pgf.yj20258888.top

crontab -e;  crontab -l
来源：http://vwd.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://kjq.chenlongwang.top

openssl rand -hex 16
来源：http://hbj.svipenyu.cn

[R68] 计算文件校验值
来源：http://uyr.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://xwm.feifeiyinyue.top

[R69] 生成随机密码
来源：http://nyg.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://nco.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://pgj.birdmap.top

date +%s;  date -d @1700000000
来源：http://nmc.meibo888.top

[R71] 日期格式化
来源：http://oyu.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xmp.cdnleiting.top

[R72] 等待端口就绪
来源：http://jmf.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://wnv.feifeiyinyue.top

[R73] 分割大日志
来源：http://tvn.yanxiufei.cn

split -l 1000 big.log part_
来源：http://qfl.gzhubu.top

[R74] 批量重命名
来源：http://aoo.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://whh.aizwys.cn

[R75] 导出环境变量
来源：http://ivt.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://vjo.fehbvm.com

[R76] 使用临时文件
来源：http://bvc.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fsq.hfpthk.cn

[R77] 读取用户输入
来源：http://qkx.cqqwz.cn

read -rp "请输入: " ans
来源：http://lit.birdmap.top

[R78] 交互式菜单
来源：http://dgz.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://buv.tanke756.top

[R79] 解析命令行选项
来源：http://qqt.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pvg.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://ttx.hammf.cn

time ./run.sh
来源：http://cow.xylfe.cn

================================================================================
来源：http://hgs.jqgfzy.top

S. C / C++ 专题
来源：http://rgu.shuidangran.top

================================================================================
来源：http://kpb.ppjwa.cn

[S01] C：Hello World
来源：http://ygt.ywan-chungtsiang.top

#include <stdio.h>
来源：http://kzn.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ess.gzhubu.top

[S02] C：变量与格式化输出
来源：http://ifk.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://ywx.nanxuanxn.top

[S03] C：读入整数
来源：http://ces.ctjpmb.com

int x; scanf("%d", &x);
来源：http://jrx.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://wre.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://zfp.hnqzz.top

[S05] C：字符串长度
来源：http://kor.fehbvm.com

strlen(s)
来源：http://trv.sufxvd.cn

[S06] C：字符串比较
来源：http://qqz.gotoacloud.top

strcmp(a, b) == 0
来源：http://jlv.hysaishi.cn

[S07] C：数组遍历求和
来源：http://tns.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kfb.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://ghh.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jcf.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://ome.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wwb.haohaochexian.top

[S10] C：指针与解引用
来源：http://uyl.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://xey.sjlbkw.cn

[S11] C：逐行读文件
来源：http://qph.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://fas.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ohn.chenzaomai.com

fclose(f);
来源：http://vra.sweek.top

[S12] C：写文件
来源：http://qjf.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ugw.yvedp.cn

[S13] C：宏定义
来源：http://mbo.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rul.yonumen.top

[S14] C：枚举
来源：http://mci.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://qoh.9152youxi.cn

[S15] C：类型转换
来源：http://aeg.fehbvm.com

(double) a / b
来源：http://icf.xuanzx.com

[S16] C：位操作置位
来源：http://lkf.tarul.cn

x |= (1 << 3);
来源：http://xxb.redwolf501.top

[S17] C：安全拼接字符串
来源：http://cka.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://phh.andypj.xyz

[S18] C：命令行参数
来源：http://mdj.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://slw.zhijiandao.cn

[S19] C：快速排序
来源：http://vax.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://xxe.dianchejie.cn

[S20] C：二分查找
来源：http://ogg.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wfk.cucudq.cn

[S21] C：字符类别判断
来源：http://hkq.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kpb.9152youxi.cn

[S22] C：字符串转数字
来源：http://ynd.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://bhw.chenlongwang.top

[S23] C：随机数
来源：http://tqs.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uav.guowangkeji.top

[S24] C：获取本地时间
来源：http://ehr.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cvl.quarkkingdee.top

[S25] C：内存拷贝
来源：http://utd.shzxlz.cn

memcpy(dst, src, n);
来源：http://pax.sjlbkw.cn

[S26] C：内存清零
来源：http://jsc.xylfe.cn

memset(a, 0, sizeof a);
来源：http://tuc.nanxinkj.top

[S27] C：定义常量
来源：http://hce.andypj.xyz

const double PI = 3.14159;
来源：http://kvx.pengpengdd.cyou

[S28] C：静态变量
来源：http://uvq.ydzc1.top

static int counter = 0;
来源：http://ird.yonumen.top

[S29] C：变参函数
来源：http://sge.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vfg.fktsv.cn

[S30] C：头文件保护
来源：http://sax.yj20258.top

#ifndef X_H
来源：http://ucz.zhixingplan.top

#define X_H
来源：http://hea.yangfankeji.com

#endif
来源：http://xok.tanke756.top

[S31] C++：Hello World
来源：http://pse.sufxvd.cn

#include <iostream>
来源：http://pqg.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://jaf.sufxvd.cn

[S32] C++：字符串
来源：http://ara.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://cxo.ybcxt.top

[S33] C++：vector 增删
来源：http://sfw.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oac.zdqjudy.top

[S34] C++：遍历 vector
来源：http://xaf.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://njb.jyoumei.cn

[S35] C++：map
来源：http://gjw.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ump.cqqwz.cn

[S36] C++：unordered_map
来源：http://cwv.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uxt.pycfn.com

[S37] C++：set
来源：http://upe.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nyv.jinyuanbaomall.cn

[S38] C++：排序
来源：http://rez.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://sna.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://rrj.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dbw.ydzc1.top

[S40] C++：查找元素
来源：http://lce.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xjp.guowangkeji.top

[S41] C++：类与构造函数
来源：http://vfr.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://llm.meibo888.top

[S42] C++：继承与虚函数
来源：http://eyk.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://yjy.vqdsnc.cn

[S43] C++：智能指针
来源：http://akt.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://bin.hnqzz.top

[S44] C++：引用传参
来源：http://ney.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://izb.ppjwa.cn

[S45] C++：lambda
来源：http://bds.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://ggp.yj20258888.top

[S46] C++：函数模板
来源：http://alt.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gth.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://cfi.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://huf.smart0.xyz

[S48] C++：逐行读文件
来源：http://nmu.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://mvi.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://etm.yj202588.top

[S49] C++：写文件
来源：http://ina.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofh.zhengqikj.top

[S50] C++：格式化数字
来源：http://wxm.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kal.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://uzd.hnqzz.top

static_cast<double>(a) / b
来源：http://ihk.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://bxp.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://nmd.birdmap.top

[S53] C++：移动语义
来源：http://hgi.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://tmw.smart0.xyz

[S54] C++：异常处理
来源：http://zzn.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hrv.wangdashe.top

[S55] C++：结构化绑定
来源：http://vps.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zfe.jiagoushi.top

[S56] C++：optional
来源：http://cfg.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fpv.jqgufenzy.top

[S57] C++：编译期常量
来源：http://sdr.jiagoushi.top

constexpr int N = 10;
来源：http://cqx.chenzaomai.com

[S58] C++：命名空间
来源：http://vad.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://qpl.cqqwz.cn

[S59] C++：静态断言
来源：http://orr.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tam.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://mhw.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yxo.fktsv.cn

================================================================================
来源：http://jwo.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nrc.wangshuangyany.cn

================================================================================
来源：http://tbw.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://qwz.ydjk.org.cn

println("Hello")
来源：http://lgf.fengsongda.top

[T02] Kotlin：变量
来源：http://vbl.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vih.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://tju.xziqi.cn

"值: $b"
来源：http://bdg.bjfxy.top

[T04] Kotlin：空安全
来源：http://mse.hywenlv.cn

val n: String? = null;  n?.length
来源：http://vhi.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://xiv.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hrs.birdmap.top

[T06] Kotlin：集合映射
来源：http://wtd.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uwb.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://jtk.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxy.yangfankeji.com

[T08] Kotlin：数据类
来源：http://gxv.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://myy.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://upg.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://tzg.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://iyg.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uya.uphjek.com

[T11] Kotlin：协程
来源：http://kfv.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nnl.sysykeji.top

[T12] Kotlin：解构声明
来源：http://yjq.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://udu.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://qil.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://fsd.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://mlf.jianghu66.top

for (i in 1..10) println(i)
来源：http://kfh.quarkkingdee.top

[T15] Kotlin：接口
来源：http://edq.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://mbz.jlsjyb.cn

[T16] Swift：Hello World
来源：http://jjo.zhiwuduotai.top

print("Hello")
来源：http://sol.ybcxt.top

[T17] Swift：变量与常量
来源：http://gky.haohaochexian.top

var a = 1;  let b = 2
来源：http://onl.snrcjt.cn

[T18] Swift：字符串插值
来源：http://nuc.vehdjk.com

"值: \(b)"
来源：http://bxq.jinqigufen.top

[T19] Swift：可选绑定
来源：http://moa.sweek.top

if let n = opt { print(n) }
来源：http://qdj.sjlbkw.cn

[T20] Swift：数组操作
来源：http://hxu.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lfg.haohaochexian.top

[T21] Swift：遍历
来源：http://its.yuxming.cn

for x in a { print(x) }
来源：http://tpj.jiagoushi.top

[T22] Swift：字典
来源：http://ecn.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://kxe.jlsjyb.cn

[T23] Swift：函数
来源：http://fbl.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://orl.quarkkingdee.top

[T24] Swift：闭包
来源：http://wai.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mcy.jianghu66.top

[T25] Swift：结构体
来源：http://qzc.gaohongyu789.top

struct P { var x: Int }
来源：http://kmu.guannengcc.top

[T26] Swift：类与重写
来源：http://zpm.sweek.top

class A: Base { override func f() {} }
来源：http://ysv.nanxinkj.top

[T27] Swift：错误处理
来源：http://wux.yfazqb.com

do { try f() } catch { print(error) }
来源：http://lwe.fehbvm.com

[T28] Swift：枚举
来源：http://jio.havefunace.top

enum Color { case red, green }
来源：http://vfh.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://sih.hongshengwenyu.top

guard let x = opt else { return }
来源：http://dpf.quarkkingdee.top

[T30] Swift：协议
来源：http://jpo.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://orc.fengsongda.top

[T31] Lua：Hello World
来源：http://ujn.52xcode.cn

print("Hello")
来源：http://voh.ybcxt.top

[T32] Lua：局部变量
来源：http://gbl.jqgufenzy.top

local a = 1
来源：http://tae.xylfe.cn

[T33] Lua：表（数组）
来源：http://ljb.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fmv.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://ckk.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xhs.xinyue.icu

[T35] Lua：字典表
来源：http://ius.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://den.tanke756.top

[T36] Lua：函数
来源：http://sya.ehwqpu.com

function add(a, b) return a + b end
来源：http://yvq.shuidangran.top

[T37] Lua：字符串拼接
来源：http://wep.bbcook.cn

"a" .. "b"
来源：http://cqt.fanxiaobao.xyz

[T38] Lua：条件
来源：http://bzq.shzxlz.cn

if x > 0 then print("正") end
来源：http://jbz.tanke756.top

[T39] Lua：模式匹配
来源：http://bbj.hywenlv.cn

string.find(s, "%d+")
来源：http://ons.ctjpmb.com

[T40] Lua：元表
来源：http://oof.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://qvu.hnxiangtu.top

[T41] Perl：Hello World
来源：http://kmb.yfazqb.com

print "Hello\n";
来源：http://fio.yueranfly.top

[T42] Perl：变量类型
来源：http://yvv.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://knn.yj20258.top

[T43] Perl：字符串插值
来源：http://weg.ctjpmb.com

"值: $a"
来源：http://rmd.cashguo.top

[T44] Perl：条件
来源：http://zzs.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://irr.pengpengdd.cyou


<!-- 参考信息 -->