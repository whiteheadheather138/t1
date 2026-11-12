代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://pyq.cucudq.cn

[R52] 统计行数
来源：http://lhk.jianghu66.top

wc -l a.txt
来源：http://fmv.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://kko.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nrx.c1oappe.top

[R54] 比较两个文件
来源：http://aci.jiagoushi.top

diff a.txt b.txt
来源：http://xhw.yueranfly.top

[R55] 压缩与解压
来源：http://hnw.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sic.zdbjq.cn

[R56] 远程拷贝
来源：http://jcx.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://bph.daxiang520.top

[R57] 远程执行命令
来源：http://xay.yvedp.cn

ssh user@host 'uptime'
来源：http://jdr.cheryme.top

[R58] 下载文件
来源：http://zmm.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kpp.yueranfly.top

[R59] 发 POST JSON
来源：http://yuw.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hdb.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://qzi.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ifr.jqgfzy.top

[R61] 磁盘占用
来源：http://pqb.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://tfy.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://prl.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://nfj.epnwcf.com

[R63] 内存与进程
来源：http://yfk.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://exv.yvedp.cn

[R64] 结束进程
来源：http://tsg.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://cgr.tian-w.cn

[R65] 查看端口占用
来源：http://ddw.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rtw.chenzaomai.com

[R66] 定时任务
来源：http://ski.xuanzx.com

crontab -e;  crontab -l
来源：http://qom.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://ykq.xinyue.icu

openssl rand -hex 16
来源：http://hoa.jlsjyb.cn

[R68] 计算文件校验值
来源：http://rfv.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zto.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://wge.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://had.tarul.cn

[R70] 时间戳与互转
来源：http://rcy.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://rsh.nanxinkj.top

[R71] 日期格式化
来源：http://ggj.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yhk.mhx1999.top

[R72] 等待端口就绪
来源：http://ykh.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mbe.yj202588.top

[R73] 分割大日志
来源：http://kuh.zhoulong.xyz

split -l 1000 big.log part_
来源：http://cov.yfazqb.com

[R74] 批量重命名
来源：http://vkq.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://viv.yuxming.cn

[R75] 导出环境变量
来源：http://gop.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://joh.cashguo.top

[R76] 使用临时文件
来源：http://ymd.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zwi.0kj1m.cn

[R77] 读取用户输入
来源：http://fzu.yueranfly.top

read -rp "请输入: " ans
来源：http://gyg.hammf.cn

[R78] 交互式菜单
来源：http://dbg.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://srw.haohaochexian.top

[R79] 解析命令行选项
来源：http://oeu.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dwy.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://cmf.tian-w.cn

time ./run.sh
来源：http://llg.jqgufenzy.top

================================================================================
来源：http://kkf.sysykeji.top

S. C / C++ 专题
来源：http://ehw.yuxming.cn

================================================================================
来源：http://rcr.meibo888.top

[S01] C：Hello World
来源：http://sxi.jinqigfzy.top

#include <stdio.h>
来源：http://zrq.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwp.sweek.top

[S02] C：变量与格式化输出
来源：http://rmn.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://umq.snrcjt.cn

[S03] C：读入整数
来源：http://gql.ppjwa.cn

int x; scanf("%d", &x);
来源：http://gxq.tianlin.xyz

[S04] C：字符串复制
来源：http://jrr.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ndr.epnwcf.com

[S05] C：字符串长度
来源：http://yfc.zhixingplan.top

strlen(s)
来源：http://hxs.sysykeji.top

[S06] C：字符串比较
来源：http://djn.xuanzx.com

strcmp(a, b) == 0
来源：http://vdr.uphjek.com

[S07] C：数组遍历求和
来源：http://ngb.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tbf.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://ory.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pyk.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://ztt.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hcr.smart0.xyz

[S10] C：指针与解引用
来源：http://tyb.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ays.chenzaomai.com

[S11] C：逐行读文件
来源：http://tpk.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://dxd.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vvd.jiagoushi.top

fclose(f);
来源：http://ydo.nanxinkj.top

[S12] C：写文件
来源：http://gkv.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wok.ehwqpu.com

[S13] C：宏定义
来源：http://ovl.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mrv.shzxlz.cn

[S14] C：枚举
来源：http://nxe.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://kja.jlsjyb.cn

[S15] C：类型转换
来源：http://udj.hesvh.cn

(double) a / b
来源：http://vtq.yuanzhike.top

[S16] C：位操作置位
来源：http://ezv.feifeiyinyue.top

x |= (1 << 3);
来源：http://xqq.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://ydk.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oso.bbcook.cn

[S18] C：命令行参数
来源：http://usl.jlsjyb.cn

int main(int argc, char **argv)
来源：http://wux.hongshengwenyu.top

[S19] C：快速排序
来源：http://hxf.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://huh.birdmap.top

[S20] C：二分查找
来源：http://cpb.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cop.tian-w.cn

[S21] C：字符类别判断
来源：http://lsu.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vcl.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://ahi.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://uva.jqgfzy.top

[S23] C：随机数
来源：http://mmx.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zcf.cqqwz.cn

[S24] C：获取本地时间
来源：http://yqv.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uqj.zycfv.cn

[S25] C：内存拷贝
来源：http://sgq.tian-w.cn

memcpy(dst, src, n);
来源：http://atg.xziqi.cn

[S26] C：内存清零
来源：http://lyi.316326.xyz

memset(a, 0, sizeof a);
来源：http://syu.svipenyu.cn

[S27] C：定义常量
来源：http://txn.mhx1999.top

const double PI = 3.14159;
来源：http://dvb.9152youxi.cn

[S28] C：静态变量
来源：http://inb.dianchejie.cn

static int counter = 0;
来源：http://hxt.hysaishi.cn

[S29] C：变参函数
来源：http://con.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxj.aibaodan.cn

[S30] C：头文件保护
来源：http://dxp.fanxiaobao.xyz

#ifndef X_H
来源：http://ymr.fktsv.cn

#define X_H
来源：http://hvc.chenlongwang.top

#endif
来源：http://exn.ehwqpu.com

[S31] C++：Hello World
来源：http://vbf.zhixingplan.top

#include <iostream>
来源：http://nlq.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://gih.ivvv.top

[S32] C++：字符串
来源：http://kvd.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://snd.gogol.net.cn

[S33] C++：vector 增删
来源：http://rie.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zzp.daria6918.cn

[S34] C++：遍历 vector
来源：http://ihk.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://uvr.jyoumei.cn

[S35] C++：map
来源：http://xye.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vxa.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://sip.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eqb.sxryk.cn

[S37] C++：set
来源：http://dga.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vrk.svipenyu.cn

[S38] C++：排序
来源：http://aoq.tanke756.top

std::sort(v.begin(), v.end());
来源：http://jca.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://wnt.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vhq.sweek.top

[S40] C++：查找元素
来源：http://gfn.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mgf.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://bqn.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jzh.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://pru.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://vhy.cheryme.top

[S43] C++：智能指针
来源：http://ipx.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://wcq.cqqwz.cn

[S44] C++：引用传参
来源：http://wuu.52xcode.cn

void inc(int &x) { ++x; }
来源：http://idn.gogol.net.cn

[S45] C++：lambda
来源：http://owt.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://crx.ybcxt.top

[S46] C++：函数模板
来源：http://udo.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cwg.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://kre.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vrt.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://ohf.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://txt.sxryk.cn

while (std::getline(in, line)) { }
来源：http://apu.fzhhl.top

[S49] C++：写文件
来源：http://dzm.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://loh.dianchejie.cn

[S50] C++：格式化数字
来源：http://sqj.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sxa.redwolf501.top

[S51] C++：显式类型转换
来源：http://kcl.smart0.xyz

static_cast<double>(a) / b
来源：http://mcf.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://noz.yvedp.cn

int size() const noexcept { return n_; }
来源：http://pkd.nanxuanxn.top

[S53] C++：移动语义
来源：http://tmv.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://mif.zhijiandao.cn

[S54] C++：异常处理
来源：http://kwn.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xhn.shuidangran.top

[S55] C++：结构化绑定
来源：http://qkl.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oiz.ctjpmb.com

[S56] C++：optional
来源：http://bnr.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rei.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://rbd.tarul.cn

constexpr int N = 10;
来源：http://qgw.daria6918.cn

[S58] C++：命名空间
来源：http://qrv.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://vlm.yanxiufei.cn

[S59] C++：静态断言
来源：http://hrf.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://miw.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://ojw.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tdv.yj20258.top

================================================================================
来源：http://eis.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://msk.feifeiyinyue.top

================================================================================
来源：http://irs.tian-w.cn

[T01] Kotlin：Hello World
来源：http://pmz.jinyuanbaomall.cn

println("Hello")
来源：http://dgs.cdnleiting.top

[T02] Kotlin：变量
来源：http://bfu.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qwc.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://tcm.wangdashe.top

"值: $b"
来源：http://whf.0kj1m.cn

[T04] Kotlin：空安全
来源：http://jiv.yonumen.top

val n: String? = null;  n?.length
来源：http://diz.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://cjk.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tih.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://bdy.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ghc.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://ves.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://acv.haohaochexian.top

[T08] Kotlin：数据类
来源：http://eoa.uphjek.com

data class User(val name: String, val age: Int)
来源：http://xln.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://clz.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://ear.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://qzh.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nkz.c1oappe.top

[T11] Kotlin：协程
来源：http://ptt.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://swk.nwbrower.top

[T12] Kotlin：解构声明
来源：http://xfp.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://ene.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://hsu.fengsongda.top

val m = mapOf("a" to 1)
来源：http://zgj.daxiang520.top

[T14] Kotlin：循环
来源：http://wlw.hysaishi.cn

for (i in 1..10) println(i)
来源：http://rds.yfazqb.com

[T15] Kotlin：接口
来源：http://shx.andypj.xyz

interface Shape { fun area(): Double }
来源：http://keb.aibaodan.cn

[T16] Swift：Hello World
来源：http://vbj.hesvh.cn

print("Hello")
来源：http://rjo.mhx1999.top

[T17] Swift：变量与常量
来源：http://fbu.0kj1m.cn

var a = 1;  let b = 2
来源：http://umw.hywenlv.cn

[T18] Swift：字符串插值
来源：http://cjy.sxryk.cn

"值: \(b)"
来源：http://rsc.0kj1m.cn

[T19] Swift：可选绑定
来源：http://ckl.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://kym.pycfn.com

[T20] Swift：数组操作
来源：http://quk.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tvo.jyoumei.cn

[T21] Swift：遍历
来源：http://xry.shanyushiyangtech.top

for x in a { print(x) }
来源：http://ngv.xziqi.cn

[T22] Swift：字典
来源：http://vae.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://yxh.zhixingplan.top

[T23] Swift：函数
来源：http://yol.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rix.hnxiangtu.top

[T24] Swift：闭包
来源：http://isp.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqs.jinqigfzy.top

[T25] Swift：结构体
来源：http://iax.cqqwz.cn

struct P { var x: Int }
来源：http://igh.ppjwa.cn

[T26] Swift：类与重写
来源：http://gal.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://exw.fzhhl.top

[T27] Swift：错误处理
来源：http://iwj.ivvv.top

do { try f() } catch { print(error) }
来源：http://gmv.dashuyun.cn

[T28] Swift：枚举
来源：http://qwz.feifeiyinyue.top

enum Color { case red, green }
来源：http://wup.cashguo.top

[T29] Swift：guard 提前返回
来源：http://szi.jqgfzy.top

guard let x = opt else { return }
来源：http://zpf.ehwqpu.com

[T30] Swift：协议
来源：http://yrf.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://dai.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://oem.xziqi.cn

print("Hello")
来源：http://elt.iojbl.cn

[T32] Lua：局部变量
来源：http://drt.xingfuxueyuan.xyz

local a = 1
来源：http://wtt.316326.xyz

[T33] Lua：表（数组）
来源：http://jgr.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xow.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://hif.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kbm.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://ctc.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://nfn.jqgfzy.top

[T36] Lua：函数
来源：http://wpg.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://jee.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://jyr.bjfxy.top

"a" .. "b"
来源：http://pgd.cashguo.top

[T38] Lua：条件
来源：http://noi.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://dhf.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://dac.hysaishi.cn

string.find(s, "%d+")
来源：http://viu.tanke756.top

[T40] Lua：元表
来源：http://wqr.ivvv.top

setmetatable({}, { __index = base })
来源：http://xsn.jlsjyb.cn

[T41] Perl：Hello World
来源：http://mmu.ywan-chungtsiang.top

print "Hello\n";
来源：http://ltz.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://yde.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aed.tanke756.top

[T43] Perl：字符串插值
来源：http://gxi.jyoumei.cn

"值: $a"
来源：http://ipx.hfpthk.cn

[T44] Perl：条件
来源：http://scb.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://jho.chenzaomai.com

[T45] Perl：数组遍历
来源：http://lxx.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://odj.andypj.xyz

[T46] Perl：哈希操作
来源：http://hzx.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://seq.fzhhl.top

[T47] Perl：正则捕获
来源：http://pcw.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iyh.yanxiufei.cn

[T48] Perl：正则替换
来源：http://jar.daria6918.cn

$s =~ s/old/new/g;
来源：http://wfx.xuanzx.com

[T49] Perl：函数
来源：http://mvx.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://phc.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://vfj.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lbc.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://fuk.wangdashe.top

[T51] Scala：Hello World
来源：http://apz.zhoulong.xyz

println("Hello")
来源：http://gqe.guowangkeji.top

[T52] Scala：变量
来源：http://ztr.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://jdz.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://cjl.iojbl.cn

s"值: $b"
来源：http://pkq.zhixingplan.top

[T54] Scala：集合映射
来源：http://hjw.xuetiantiany.cn


<!-- 参考信息 -->