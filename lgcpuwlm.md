代发 wailian999

find . -name "*.tmp" -delete
来源：http://vhj.yonumen.top

[R46] 递归替换文件内容
来源：http://ehz.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ifs.yuanzhike.top

[R47] sed 单行替换
来源：http://onp.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ibo.zdqjudy.top

[R48] awk 取指定列
来源：http://scr.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://gar.xylfe.cn

[R49] awk 带条件
来源：http://zyg.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jjk.shangyingyoupin.top

[R50] awk 求和
来源：http://icy.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jkr.jinqigfzy.top

[R51] 排序去重取前几
来源：http://kdz.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ewi.zdbjq.cn

[R52] 统计行数
来源：http://srg.gogol.net.cn

wc -l a.txt
来源：http://eoi.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://ixy.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pss.hcnkem.com

[R54] 比较两个文件
来源：http://kvj.uphjek.com

diff a.txt b.txt
来源：http://xup.nanxuanxn.top

[R55] 压缩与解压
来源：http://apv.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngg.sweek.top

[R56] 远程拷贝
来源：http://wdb.cheryme.top

scp file user@host:/path/
来源：http://wsd.52xcode.cn

[R57] 远程执行命令
来源：http://ieg.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://fwt.birdmap.top

[R58] 下载文件
来源：http://lkd.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kua.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://ecg.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lsn.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://vao.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dbg.c1oappe.top

[R61] 磁盘占用
来源：http://nmi.fanxiaobao.xyz

df -h;  du -sh *
来源：http://muy.tian-w.cn

[R62] 找最占空间的文件
来源：http://yum.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://mnf.jyoumei.cn

[R63] 内存与进程
来源：http://evm.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://tmh.epnwcf.com

[R64] 结束进程
来源：http://xyt.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://tvq.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://fhx.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oco.yuxming.cn

[R66] 定时任务
来源：http://bra.yongpay.top

crontab -e;  crontab -l
来源：http://aju.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://zuc.chenlongwang.top

openssl rand -hex 16
来源：http://hky.c1oappe.top

[R68] 计算文件校验值
来源：http://tnm.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://mrt.guannengcc.top

[R69] 生成随机密码
来源：http://unt.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://int.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://ycz.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://chj.shanyushiyangtech.top

[R71] 日期格式化
来源：http://tfx.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mbc.guannengcc.top

[R72] 等待端口就绪
来源：http://cje.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://afa.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://ygj.yuanzhike.top

split -l 1000 big.log part_
来源：http://zib.gogol.net.cn

[R74] 批量重命名
来源：http://hlx.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://spd.cheryme.top

[R75] 导出环境变量
来源：http://bzo.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://iiq.jiagoushi.top

[R76] 使用临时文件
来源：http://uuq.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jvq.birdmap.top

[R77] 读取用户输入
来源：http://zyl.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://juy.yangfankeji.com

[R78] 交互式菜单
来源：http://gbm.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hrq.yj20258888.top

[R79] 解析命令行选项
来源：http://ehi.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hus.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://ssf.ydzc1.top

time ./run.sh
来源：http://qlh.jqgfzy.top

================================================================================
来源：http://qbf.fzhhl.top

S. C / C++ 专题
来源：http://vpo.jlsjyb.cn

================================================================================
来源：http://knh.chenjidiqi.icu

[S01] C：Hello World
来源：http://wdh.pengpengdd.cyou

#include <stdio.h>
来源：http://cbo.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://imo.yueranfly.top

[S02] C：变量与格式化输出
来源：http://itg.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://eif.xuetiantiany.cn

[S03] C：读入整数
来源：http://cks.gzhubu.top

int x; scanf("%d", &x);
来源：http://rhu.chenlongwang.top

[S04] C：字符串复制
来源：http://czr.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://gzm.epnwcf.com

[S05] C：字符串长度
来源：http://vzw.316326.xyz

strlen(s)
来源：http://yyl.ppjwa.cn

[S06] C：字符串比较
来源：http://zcy.gzhubu.top

strcmp(a, b) == 0
来源：http://tdh.meibo888.top

[S07] C：数组遍历求和
来源：http://bly.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://try.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://raz.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://osd.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://yyo.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ehe.meibo888.top

[S10] C：指针与解引用
来源：http://tws.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://lkn.havefunace.top

[S11] C：逐行读文件
来源：http://ksv.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://hxu.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://xjj.chenzaomai.com

fclose(f);
来源：http://opn.sufxvd.cn

[S12] C：写文件
来源：http://cgu.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jpa.guowangkeji.top

[S13] C：宏定义
来源：http://ail.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qdg.tian-w.cn

[S14] C：枚举
来源：http://etm.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://msa.smart0.xyz

[S15] C：类型转换
来源：http://cfy.9152youxi.cn

(double) a / b
来源：http://khe.ehwqpu.com

[S16] C：位操作置位
来源：http://uwl.jyoumei.cn

x |= (1 << 3);
来源：http://dzr.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://xdj.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mql.tianlin.xyz

[S18] C：命令行参数
来源：http://dce.sufxvd.cn

int main(int argc, char **argv)
来源：http://ctd.fehbvm.com

[S19] C：快速排序
来源：http://nex.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cqi.cheryme.top

[S20] C：二分查找
来源：http://prp.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yqh.jqgufenzy.top

[S21] C：字符类别判断
来源：http://amq.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vpg.jyoumei.cn

[S22] C：字符串转数字
来源：http://bnq.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fjf.yj20258888.top

[S23] C：随机数
来源：http://xkx.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://btz.jinqigufen.top

[S24] C：获取本地时间
来源：http://vcd.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xpj.ybcxt.top

[S25] C：内存拷贝
来源：http://mgh.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://xho.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://grh.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://ovy.yj20258888.top

[S27] C：定义常量
来源：http://ovo.yj20258.top

const double PI = 3.14159;
来源：http://mzs.xinyue.icu

[S28] C：静态变量
来源：http://qds.hcnkem.com

static int counter = 0;
来源：http://squ.hongshengwenyu.top

[S29] C：变参函数
来源：http://dqr.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jhg.xuanzx.com

[S30] C：头文件保护
来源：http://gje.vehdjk.com

#ifndef X_H
来源：http://mst.fktsv.cn

#define X_H
来源：http://khm.tianlin.xyz

#endif
来源：http://ija.zhijiandao.cn

[S31] C++：Hello World
来源：http://nzj.hammf.cn

#include <iostream>
来源：http://ftg.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ycd.sjlbkw.cn

[S32] C++：字符串
来源：http://pei.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://evb.zdqjudy.top

[S33] C++：vector 增删
来源：http://nol.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tts.jiagoushi.top

[S34] C++：遍历 vector
来源：http://oxi.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://mzl.yvedp.cn

[S35] C++：map
来源：http://uta.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rtr.cucudq.cn

[S36] C++：unordered_map
来源：http://lfa.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yxb.dianchejie.cn

[S37] C++：set
来源：http://xyu.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://phx.shanyushiyangkeji.top

[S38] C++：排序
来源：http://kak.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://uui.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://ngf.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wfw.fzhhl.top

[S40] C++：查找元素
来源：http://rwu.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wwj.guannengcc.top

[S41] C++：类与构造函数
来源：http://hsg.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xbz.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://pan.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://vrz.yvedp.cn

[S43] C++：智能指针
来源：http://aqr.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://umn.jinqigufen.top

[S44] C++：引用传参
来源：http://ama.havefunace.top

void inc(int &x) { ++x; }
来源：http://son.hysaishi.cn

[S45] C++：lambda
来源：http://khq.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ugq.ydjk.org.cn

[S46] C++：函数模板
来源：http://cli.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jfn.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://tft.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iuh.yj20258.top

[S48] C++：逐行读文件
来源：http://qgd.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://yqq.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://cdz.zhixingplan.top

[S49] C++：写文件
来源：http://zgm.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spt.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://yhp.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bkd.gzhubu.top

[S51] C++：显式类型转换
来源：http://gnn.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://aub.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://yws.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://lpk.jqgufenzy.top

[S53] C++：移动语义
来源：http://hzg.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://kee.jqgfzy.top

[S54] C++：异常处理
来源：http://hss.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ztm.sufxvd.cn

[S55] C++：结构化绑定
来源：http://lgr.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ixs.yueranfly.top

[S56] C++：optional
来源：http://uiq.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jtf.sweek.top

[S57] C++：编译期常量
来源：http://ces.hcnkem.com

constexpr int N = 10;
来源：http://nvo.xziqi.cn

[S58] C++：命名空间
来源：http://aem.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://zty.yj20258888.top

[S59] C++：静态断言
来源：http://qpb.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hax.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://twh.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rlc.yangfankeji.com

================================================================================
来源：http://amf.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ctz.jinqigfzy.top

================================================================================
来源：http://iny.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://vjz.yj202588.top

println("Hello")
来源：http://tos.ybcxt.top

[T02] Kotlin：变量
来源：http://qgl.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nwv.316326.xyz

[T03] Kotlin：字符串模板
来源：http://cvw.havefunace.top

"值: $b"
来源：http://gye.ctjpmb.com

[T04] Kotlin：空安全
来源：http://fpj.sysykeji.top

val n: String? = null;  n?.length
来源：http://qhq.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://aul.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zjy.hesvh.cn

[T06] Kotlin：集合映射
来源：http://ldy.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://weu.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://ioe.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://che.chenzaomai.com

[T08] Kotlin：数据类
来源：http://gak.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://mcy.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://tiw.sweek.top

fun String.exclaim() = this + "!"
来源：http://dvt.c1oappe.top

[T10] Kotlin：默认参数
来源：http://qep.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://usq.hysaishi.cn

[T11] Kotlin：协程
来源：http://oyy.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zon.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://qag.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://jsh.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://cip.fengsongda.top

val m = mapOf("a" to 1)
来源：http://ydf.vqdsnc.cn

[T14] Kotlin：循环
来源：http://lxv.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://mxi.hysaishi.cn

[T15] Kotlin：接口
来源：http://glq.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://nql.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://zzr.uphjek.com

print("Hello")
来源：http://rna.yuxming.cn

[T17] Swift：变量与常量
来源：http://doq.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://qsh.ybcxt.top

[T18] Swift：字符串插值
来源：http://jqr.nanxuanxn.top

"值: \(b)"
来源：http://mhm.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://uoy.ppjwa.cn

if let n = opt { print(n) }
来源：http://qrl.cdnleiting.top

[T20] Swift：数组操作
来源：http://qdq.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ccn.ydjk.org.cn

[T21] Swift：遍历
来源：http://jgp.zhongyouzk.top

for x in a { print(x) }
来源：http://zln.xinyue.icu

[T22] Swift：字典
来源：http://ekj.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://xvx.chenzaomai.com

[T23] Swift：函数
来源：http://esx.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://elh.zhoulong.xyz

[T24] Swift：闭包
来源：http://glu.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ssa.yongpay.top

[T25] Swift：结构体
来源：http://orb.meibo888.top

struct P { var x: Int }
来源：http://log.nwbrower.top

[T26] Swift：类与重写
来源：http://gmg.meibo888.top

class A: Base { override func f() {} }
来源：http://czt.havefunace.top

[T27] Swift：错误处理
来源：http://cxp.gzhubu.top

do { try f() } catch { print(error) }
来源：http://gpc.kuanghao11.cn

[T28] Swift：枚举
来源：http://mzh.cucudq.cn

enum Color { case red, green }
来源：http://qqt.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://geu.52xcode.cn

guard let x = opt else { return }
来源：http://nak.sysykeji.top

[T30] Swift：协议
来源：http://dqj.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://kzs.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://bzc.nanxuanxn.top

print("Hello")
来源：http://bfc.daxiang520.top

[T32] Lua：局部变量
来源：http://erp.ydzc1.top

local a = 1
来源：http://fnc.xinyue.icu

[T33] Lua：表（数组）
来源：http://svt.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://nsa.sufxvd.cn

[T34] Lua：遍历表
来源：http://uzc.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://huu.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://qhl.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://afl.yongpay.top

[T36] Lua：函数
来源：http://ldo.xziqi.cn

function add(a, b) return a + b end
来源：http://lvp.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://qbb.jinqigufen.top

"a" .. "b"
来源：http://val.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://zsp.hysaishi.cn

if x > 0 then print("正") end
来源：http://cdl.hesvh.cn

[T39] Lua：模式匹配
来源：http://usz.9152youxi.cn

string.find(s, "%d+")
来源：http://tkc.zhixingplan.top

[T40] Lua：元表
来源：http://wfj.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://bhv.nanxinkj.top

[T41] Perl：Hello World
来源：http://ilx.xuanzx.com

print "Hello\n";
来源：http://fhf.hcnkem.com

[T42] Perl：变量类型
来源：http://blg.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://deh.shuidangran.top

[T43] Perl：字符串插值
来源：http://iat.ybcxt.top

"值: $a"
来源：http://zcp.sufxvd.cn

[T44] Perl：条件
来源：http://bol.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://ggq.fehbvm.com

[T45] Perl：数组遍历
来源：http://hbt.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://wlw.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://jjx.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ouc.tarul.cn

[T47] Perl：正则捕获
来源：http://qvt.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://lwa.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://kxp.birdmap.top

$s =~ s/old/new/g;
来源：http://vif.quarkkingdee.top


<!-- 参考信息 -->