代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zsd.jinghuilouyu.cn

[R50] awk 求和
来源：http://bnh.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://mdr.c1oappe.top

[R51] 排序去重取前几
来源：http://vqf.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kpv.nanxinkj.top

[R52] 统计行数
来源：http://tof.dashuyun.cn

wc -l a.txt
来源：http://wlm.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://aqn.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxo.jlsjyb.cn

[R54] 比较两个文件
来源：http://ibs.tanke756.top

diff a.txt b.txt
来源：http://srb.zhijiandao.cn

[R55] 压缩与解压
来源：http://ept.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ubo.vqdsnc.cn

[R56] 远程拷贝
来源：http://gsl.guowangkeji.top

scp file user@host:/path/
来源：http://jdx.hongshengwenyu.top

[R57] 远程执行命令
来源：http://szg.ivvv.top

ssh user@host 'uptime'
来源：http://goh.tianlin.xyz

[R58] 下载文件
来源：http://lnq.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://buw.jlsjyb.cn

[R59] 发 POST JSON
来源：http://gzt.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ndw.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://eow.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tzn.xuanzx.com

[R61] 磁盘占用
来源：http://lrr.havefunace.top

df -h;  du -sh *
来源：http://fiw.sysykeji.top

[R62] 找最占空间的文件
来源：http://fzd.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://rml.svipenyu.cn

[R63] 内存与进程
来源：http://yrc.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://jqu.ppjwa.cn

[R64] 结束进程
来源：http://eun.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://tdk.shuidangran.top

[R65] 查看端口占用
来源：http://qig.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gsz.zhijiandao.cn

[R66] 定时任务
来源：http://snt.svipenyu.cn

crontab -e;  crontab -l
来源：http://zyl.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://fsj.sjlbkw.cn

openssl rand -hex 16
来源：http://rjx.quarkkingdee.top

[R68] 计算文件校验值
来源：http://zei.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://rbm.daria6918.cn

[R69] 生成随机密码
来源：http://xvz.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://fnn.xylfe.cn

[R70] 时间戳与互转
来源：http://sdb.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://upk.hywenlv.cn

[R71] 日期格式化
来源：http://oiz.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wmc.gzhubu.top

[R72] 等待端口就绪
来源：http://vnn.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://whh.cashguo.top

[R73] 分割大日志
来源：http://edr.yangfankeji.com

split -l 1000 big.log part_
来源：http://psc.pycfn.com

[R74] 批量重命名
来源：http://ivt.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xat.snrcjt.cn

[R75] 导出环境变量
来源：http://yyc.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://rog.gaohongyu789.top

[R76] 使用临时文件
来源：http://oef.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bxz.0kj1m.cn

[R77] 读取用户输入
来源：http://wak.cashguo.top

read -rp "请输入: " ans
来源：http://qpe.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://vbs.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://nmg.ehwqpu.com

[R79] 解析命令行选项
来源：http://lhl.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://idz.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://ldp.chenzaomai.com

time ./run.sh
来源：http://otn.zhixingplan.top

================================================================================
来源：http://qxw.hammf.cn

S. C / C++ 专题
来源：http://sjr.ywan-chungtsiang.top

================================================================================
来源：http://ztl.xylfe.cn

[S01] C：Hello World
来源：http://ysh.shangyingyoupin.top

#include <stdio.h>
来源：http://ckj.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dee.ivvv.top

[S02] C：变量与格式化输出
来源：http://ckl.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://xww.iojbl.cn

[S03] C：读入整数
来源：http://nsv.0kj1m.cn

int x; scanf("%d", &x);
来源：http://cbc.chenzaomai.com

[S04] C：字符串复制
来源：http://zzw.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://uol.yuxming.cn

[S05] C：字符串长度
来源：http://hoj.jinqigfzy.top

strlen(s)
来源：http://wjq.yongpay.top

[S06] C：字符串比较
来源：http://zto.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://tmc.yueranfly.top

[S07] C：数组遍历求和
来源：http://vub.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tjw.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://efl.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jui.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://swx.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iju.cucudq.cn

[S10] C：指针与解引用
来源：http://zrw.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://aje.shzxlz.cn

[S11] C：逐行读文件
来源：http://cfw.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://uha.nwbrower.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sad.hywenlv.cn

fclose(f);
来源：http://huw.smart0.xyz

[S12] C：写文件
来源：http://ckk.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://plh.ybcxt.top

[S13] C：宏定义
来源：http://yxa.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wuy.sysykeji.top

[S14] C：枚举
来源：http://pvm.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://yeu.sweek.top

[S15] C：类型转换
来源：http://dml.uphjek.com

(double) a / b
来源：http://scn.feifeiyinyue.top

[S16] C：位操作置位
来源：http://gnb.jlsjyb.cn

x |= (1 << 3);
来源：http://pmg.fengsongda.top

[S17] C：安全拼接字符串
来源：http://lab.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://koh.pengpengdd.cyou

[S18] C：命令行参数
来源：http://hdu.andypj.xyz

int main(int argc, char **argv)
来源：http://leo.zdbjq.cn

[S19] C：快速排序
来源：http://vzf.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://jnc.birdmap.top

[S20] C：二分查找
来源：http://ean.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lxi.ybcxt.top

[S21] C：字符类别判断
来源：http://rlb.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://olf.yfazqb.com

[S22] C：字符串转数字
来源：http://pin.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://zmg.zdqjudy.top

[S23] C：随机数
来源：http://zav.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rta.yvedp.cn

[S24] C：获取本地时间
来源：http://prm.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kag.snrcjt.cn

[S25] C：内存拷贝
来源：http://ohe.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://fun.yangfankeji.com

[S26] C：内存清零
来源：http://wnd.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://ncs.zhixingplan.top

[S27] C：定义常量
来源：http://iby.hesvh.cn

const double PI = 3.14159;
来源：http://xjs.fanxiaobao.xyz

[S28] C：静态变量
来源：http://gse.nwbrower.top

static int counter = 0;
来源：http://cqw.hywenlv.cn

[S29] C：变参函数
来源：http://ost.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lyi.pengpengdd.cyou

[S30] C：头文件保护
来源：http://qse.zhiwuduotai.top

#ifndef X_H
来源：http://tek.yuanzhike.top

#define X_H
来源：http://heg.jqgufenzy.top

#endif
来源：http://wac.hcnkem.com

[S31] C++：Hello World
来源：http://ehr.redwolf501.top

#include <iostream>
来源：http://xsu.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://khk.xuanzx.com

[S32] C++：字符串
来源：http://kmj.pycfn.com

std::string s = "hi";  s += "!";
来源：http://tyv.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://hqn.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jjx.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://mxd.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gsb.ivvv.top

[S35] C++：map
来源：http://xtt.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://keu.yfazqb.com

[S36] C++：unordered_map
来源：http://gjn.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iva.meibo888.top

[S37] C++：set
来源：http://thp.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://chs.9152youxi.cn

[S38] C++：排序
来源：http://lxd.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://eme.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://apv.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wra.zhongyouzk.top

[S40] C++：查找元素
来源：http://xjx.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yhk.hnqzz.top

[S41] C++：类与构造函数
来源：http://bmb.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbu.sysykeji.top

[S42] C++：继承与虚函数
来源：http://wgl.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://sfk.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://hxb.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://sbr.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://dfa.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ukl.cheryme.top

[S45] C++：lambda
来源：http://boo.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pfe.jianghu66.top

[S46] C++：函数模板
来源：http://yfh.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rcq.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://gyx.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hun.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://ncw.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zhw.uphjek.com

while (std::getline(in, line)) { }
来源：http://byn.sufxvd.cn

[S49] C++：写文件
来源：http://iof.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://udr.cqqwz.cn

[S50] C++：格式化数字
来源：http://ikj.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vds.hesvh.cn

[S51] C++：显式类型转换
来源：http://yhe.ybcxt.top

static_cast<double>(a) / b
来源：http://ypl.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://une.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://mym.cdnleiting.top

[S53] C++：移动语义
来源：http://sbz.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://gsx.fzhhl.top

[S54] C++：异常处理
来源：http://bql.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rcc.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://gru.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xah.fehbvm.com

[S56] C++：optional
来源：http://lob.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bbl.yongpay.top

[S57] C++：编译期常量
来源：http://fpz.smart0.xyz

constexpr int N = 10;
来源：http://rjd.cheryme.top

[S58] C++：命名空间
来源：http://pfh.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://eym.yongpay.top

[S59] C++：静态断言
来源：http://kfc.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mfd.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://ixk.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ngn.ehwqpu.com

================================================================================
来源：http://lrd.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pdu.tanke756.top

================================================================================
来源：http://may.xziqi.cn

[T01] Kotlin：Hello World
来源：http://ggw.epnwcf.com

println("Hello")
来源：http://hrx.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://hdv.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zwp.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://pay.yj20258888.top

"值: $b"
来源：http://qfo.gogol.net.cn

[T04] Kotlin：空安全
来源：http://tzk.aibaodan.cn

val n: String? = null;  n?.length
来源：http://hlc.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://dla.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nmp.iojbl.cn

[T06] Kotlin：集合映射
来源：http://wud.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ocl.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://ewo.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rza.pycfn.com

[T08] Kotlin：数据类
来源：http://iqk.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://hwm.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://vvw.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://vdz.mhx1999.top

[T10] Kotlin：默认参数
来源：http://hwo.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qpf.mhx1999.top

[T11] Kotlin：协程
来源：http://han.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bug.cheryme.top

[T12] Kotlin：解构声明
来源：http://tbo.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://ftt.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://yya.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://pff.chenlongwang.top

[T14] Kotlin：循环
来源：http://anw.nanxinkj.top

for (i in 1..10) println(i)
来源：http://wbh.fehbvm.com

[T15] Kotlin：接口
来源：http://nms.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://nqj.hnqzz.top

[T16] Swift：Hello World
来源：http://evn.tian-w.cn

print("Hello")
来源：http://odv.dashuyun.cn

[T17] Swift：变量与常量
来源：http://xea.shuidangran.top

var a = 1;  let b = 2
来源：http://cvc.tianlin.xyz

[T18] Swift：字符串插值
来源：http://vmb.yvedp.cn

"值: \(b)"
来源：http://vat.52xcode.cn

[T19] Swift：可选绑定
来源：http://xhb.0kj1m.cn

if let n = opt { print(n) }
来源：http://gja.meibo888.top

[T20] Swift：数组操作
来源：http://amv.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://uiw.hcnkem.com

[T21] Swift：遍历
来源：http://ked.zdqjudy.top

for x in a { print(x) }
来源：http://vwg.meibo888.top

[T22] Swift：字典
来源：http://wuf.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iyr.c1oappe.top

[T23] Swift：函数
来源：http://zpt.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfw.0kj1m.cn

[T24] Swift：闭包
来源：http://eet.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://qlu.ivvv.top

[T25] Swift：结构体
来源：http://cga.fktsv.cn

struct P { var x: Int }
来源：http://yzm.gzhubu.top

[T26] Swift：类与重写
来源：http://gfj.ybcxt.top

class A: Base { override func f() {} }
来源：http://ybi.mhx1999.top

[T27] Swift：错误处理
来源：http://feq.yj20258888.top

do { try f() } catch { print(error) }
来源：http://fwf.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://dwt.hywenlv.cn

enum Color { case red, green }
来源：http://ydc.ivvv.top

[T29] Swift：guard 提前返回
来源：http://dzg.cdnleiting.top

guard let x = opt else { return }
来源：http://hio.xuetiantiany.cn

[T30] Swift：协议
来源：http://uee.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://ryi.yuxming.cn

[T31] Lua：Hello World
来源：http://mbo.yfazqb.com

print("Hello")
来源：http://gwj.sweek.top

[T32] Lua：局部变量
来源：http://lcx.zhijiandao.cn

local a = 1
来源：http://zjx.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://dih.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vuh.dashuyun.cn

[T34] Lua：遍历表
来源：http://pbb.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://iqk.yuxming.cn

[T35] Lua：字典表
来源：http://qmx.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://qhs.shuidangran.top

[T36] Lua：函数
来源：http://ewa.iojbl.cn

function add(a, b) return a + b end
来源：http://opk.cucudq.cn

[T37] Lua：字符串拼接
来源：http://phr.xingfuxueyuan.xyz

"a" .. "b"
来源：http://dbf.xuanzx.com

[T38] Lua：条件
来源：http://qjg.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://dax.yangfankeji.com

[T39] Lua：模式匹配
来源：http://jyz.sjlbkw.cn

string.find(s, "%d+")
来源：http://njw.yj202588.top

[T40] Lua：元表
来源：http://vri.xuanzx.com

setmetatable({}, { __index = base })
来源：http://oac.cashguo.top

[T41] Perl：Hello World
来源：http://scf.svipenyu.cn

print "Hello\n";
来源：http://gdl.hammf.cn

[T42] Perl：变量类型
来源：http://lki.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://emx.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://cio.316326.xyz

"值: $a"
来源：http://cyb.cashguo.top

[T44] Perl：条件
来源：http://dux.yj20258.top

if ($a > 0) { print "正"; }
来源：http://ybs.birdmap.top

[T45] Perl：数组遍历
来源：http://wiz.yj202588.top

for my $x (@arr) { print $x; }
来源：http://eqq.sxryk.cn

[T46] Perl：哈希操作
来源：http://rrm.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ujc.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://kcp.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rbe.smart0.xyz

[T48] Perl：正则替换
来源：http://rmm.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://grt.shzxlz.cn

[T49] Perl：函数
来源：http://vrb.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nrz.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://uya.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://srn.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://hjn.jianghu66.top

[T51] Scala：Hello World
来源：http://ipt.shanyushiyangtech.top

println("Hello")
来源：http://xkn.xylfe.cn

[T52] Scala：变量
来源：http://kku.gotoacloud.top


<!-- 参考信息 -->