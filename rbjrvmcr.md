代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://low.jqgfzy.top

[R50] awk 求和
来源：http://ydt.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://ksj.yfazqb.com

[R51] 排序去重取前几
来源：http://dpg.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qyk.wangshuangyany.cn

[R52] 统计行数
来源：http://jai.zdbjq.cn

wc -l a.txt
来源：http://aui.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://apx.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xak.yj20258888.top

[R54] 比较两个文件
来源：http://viw.gotoacloud.top

diff a.txt b.txt
来源：http://mzr.ppjwa.cn

[R55] 压缩与解压
来源：http://nrm.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jwt.hongshengwenyu.top

[R56] 远程拷贝
来源：http://ppz.jiagoushi.top

scp file user@host:/path/
来源：http://rtj.chenzaomai.com

[R57] 远程执行命令
来源：http://vyq.ydzc1.top

ssh user@host 'uptime'
来源：http://qnj.snrcjt.cn

[R58] 下载文件
来源：http://jbt.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iyz.bbcook.cn

[R59] 发 POST JSON
来源：http://bgu.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wqe.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://wck.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mhe.sweek.top

[R61] 磁盘占用
来源：http://qzl.yongpay.top

df -h;  du -sh *
来源：http://pes.hesvh.cn

[R62] 找最占空间的文件
来源：http://jkf.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://xpg.zhongyouzk.top

[R63] 内存与进程
来源：http://ajf.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://bhd.gaohongyu789.top

[R64] 结束进程
来源：http://ibe.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://uht.gotoacloud.top

[R65] 查看端口占用
来源：http://jrp.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rjt.hongshengwenyu.top

[R66] 定时任务
来源：http://jzp.shuidangran.top

crontab -e;  crontab -l
来源：http://ula.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://iwk.ppjwa.cn

openssl rand -hex 16
来源：http://mre.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://nuw.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fqz.tanke756.top

[R69] 生成随机密码
来源：http://ssl.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://uau.0kj1m.cn

[R70] 时间戳与互转
来源：http://hrm.yj20258888.top

date +%s;  date -d @1700000000
来源：http://jus.ehwqpu.com

[R71] 日期格式化
来源：http://djl.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pbn.tian-w.cn

[R72] 等待端口就绪
来源：http://wkf.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cpd.hfpthk.cn

[R73] 分割大日志
来源：http://afo.hammf.cn

split -l 1000 big.log part_
来源：http://wcf.shuidangran.top

[R74] 批量重命名
来源：http://ajc.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xqb.gotoacloud.top

[R75] 导出环境变量
来源：http://zkr.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://zrw.52xcode.cn

[R76] 使用临时文件
来源：http://odk.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tqp.daxiang520.top

[R77] 读取用户输入
来源：http://jkc.epnwcf.com

read -rp "请输入: " ans
来源：http://geq.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://asy.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://izd.hcnkem.com

[R79] 解析命令行选项
来源：http://zew.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pyq.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://ycm.zdbjq.cn

time ./run.sh
来源：http://iew.tian-w.cn

================================================================================
来源：http://xmp.sweek.top

S. C / C++ 专题
来源：http://zsh.cashguo.top

================================================================================
来源：http://uqo.fanxiaobao.xyz

[S01] C：Hello World
来源：http://pgc.fktsv.cn

#include <stdio.h>
来源：http://uhe.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://usw.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://rmn.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://dqx.jlsjyb.cn

[S03] C：读入整数
来源：http://ubh.dianchejie.cn

int x; scanf("%d", &x);
来源：http://ylc.yongpay.top

[S04] C：字符串复制
来源：http://zcg.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://brj.yanxiufei.cn

[S05] C：字符串长度
来源：http://fpg.svipenyu.cn

strlen(s)
来源：http://xna.shangyingyoupin.top

[S06] C：字符串比较
来源：http://fos.yuanzhike.top

strcmp(a, b) == 0
来源：http://hpt.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://koo.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qgp.tanke756.top

[S08] C：动态内存分配与释放
来源：http://xlh.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wss.yonumen.top

[S09] C：结构体定义与初始化
来源：http://xzx.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fpg.ybcxt.top

[S10] C：指针与解引用
来源：http://xgd.xuanzx.com

int *p = &a;  *p = 5;
来源：http://dud.hfpthk.cn

[S11] C：逐行读文件
来源：http://rwo.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://wgp.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sua.jinghuilouyu.cn

fclose(f);
来源：http://sae.svipenyu.cn

[S12] C：写文件
来源：http://cpd.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fql.nanxuanxn.top

[S13] C：宏定义
来源：http://zjh.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://btg.hongshengwenyu.top

[S14] C：枚举
来源：http://lqk.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://bqn.9152youxi.cn

[S15] C：类型转换
来源：http://xdg.shzxlz.cn

(double) a / b
来源：http://otj.yongpay.top

[S16] C：位操作置位
来源：http://kzs.zhoulong.xyz

x |= (1 << 3);
来源：http://zag.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://drb.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fos.dashuyun.cn

[S18] C：命令行参数
来源：http://kfp.sysykeji.top

int main(int argc, char **argv)
来源：http://nke.fanxiaobao.xyz

[S19] C：快速排序
来源：http://wls.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://poc.yfazqb.com

[S20] C：二分查找
来源：http://buw.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gey.hfpthk.cn

[S21] C：字符类别判断
来源：http://vpy.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gnh.fehbvm.com

[S22] C：字符串转数字
来源：http://wfo.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://yce.wangshuangyany.cn

[S23] C：随机数
来源：http://dks.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://hho.tarul.cn

[S24] C：获取本地时间
来源：http://ziq.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uvv.xylfe.cn

[S25] C：内存拷贝
来源：http://ipc.jinqigufen.top

memcpy(dst, src, n);
来源：http://ajl.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://taz.c1oappe.top

memset(a, 0, sizeof a);
来源：http://ujz.gzhubu.top

[S27] C：定义常量
来源：http://ygz.sjlbkw.cn

const double PI = 3.14159;
来源：http://ixs.zhiwuduotai.top

[S28] C：静态变量
来源：http://qsk.cashguo.top

static int counter = 0;
来源：http://jkw.haohaochexian.top

[S29] C：变参函数
来源：http://sjq.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ozu.havefunace.top

[S30] C：头文件保护
来源：http://ciu.tanke756.top

#ifndef X_H
来源：http://fzc.zdbjq.cn

#define X_H
来源：http://gew.jiagoushi.top

#endif
来源：http://riy.vehdjk.com

[S31] C++：Hello World
来源：http://kkt.tarul.cn

#include <iostream>
来源：http://art.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://cgw.ybcxt.top

[S32] C++：字符串
来源：http://xjn.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://rxk.zhengqikj.top

[S33] C++：vector 增删
来源：http://ryx.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qux.nwbrower.top

[S34] C++：遍历 vector
来源：http://sfz.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://phf.havefunace.top

[S35] C++：map
来源：http://chj.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://niu.jyoumei.cn

[S36] C++：unordered_map
来源：http://jmf.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://psu.cheryme.top

[S37] C++：set
来源：http://ukc.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tyd.jyoumei.cn

[S38] C++：排序
来源：http://soc.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ewy.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://ppx.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xmh.yonumen.top

[S40] C++：查找元素
来源：http://kri.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bus.havefunace.top

[S41] C++：类与构造函数
来源：http://rxy.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ilf.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://nsc.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://whr.birdmap.top

[S43] C++：智能指针
来源：http://hpq.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://inr.zhengqikj.top

[S44] C++：引用传参
来源：http://vda.ivvv.top

void inc(int &x) { ++x; }
来源：http://fdo.shuidangran.top

[S45] C++：lambda
来源：http://ixo.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kbe.shangyingyoupin.top

[S46] C++：函数模板
来源：http://int.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://drp.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://atn.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nia.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://ifr.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://bqb.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://zrl.gaohongyu789.top

[S49] C++：写文件
来源：http://mzh.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uyr.andypj.xyz

[S50] C++：格式化数字
来源：http://dvu.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gpf.pycfn.com

[S51] C++：显式类型转换
来源：http://suk.chenzaomai.com

static_cast<double>(a) / b
来源：http://ili.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://jkn.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://csh.chenlongwang.top

[S53] C++：移动语义
来源：http://yku.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://mgo.yuanzhike.top

[S54] C++：异常处理
来源：http://irm.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qye.daxiang520.top

[S55] C++：结构化绑定
来源：http://yth.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rzs.birdmap.top

[S56] C++：optional
来源：http://zef.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idm.yonumen.top

[S57] C++：编译期常量
来源：http://unu.feifeiyinyue.top

constexpr int N = 10;
来源：http://dlm.fzhhl.top

[S58] C++：命名空间
来源：http://ldg.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://xht.snrcjt.cn

[S59] C++：静态断言
来源：http://kxg.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iuf.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://igc.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jtz.gaohongyu789.top

================================================================================
来源：http://oxt.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqj.hysaishi.cn

================================================================================
来源：http://ulh.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://tht.hnqzz.top

println("Hello")
来源：http://lsp.sxryk.cn

[T02] Kotlin：变量
来源：http://ykl.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gjl.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://hxc.jinqigfzy.top

"值: $b"
来源：http://ylm.meibo888.top

[T04] Kotlin：空安全
来源：http://bvn.guowangkeji.top

val n: String? = null;  n?.length
来源：http://teh.havefunace.top

[T05] Kotlin：when 表达式
来源：http://wpo.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rnw.cheryme.top

[T06] Kotlin：集合映射
来源：http://xox.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xvc.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://zkp.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gzi.wangdashe.top

[T08] Kotlin：数据类
来源：http://uoj.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://zts.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://fsi.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://cdd.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://pff.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jrs.sufxvd.cn

[T11] Kotlin：协程
来源：http://qsm.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kns.bjfxy.top

[T12] Kotlin：解构声明
来源：http://kkc.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://pjr.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://cht.birdmap.top

val m = mapOf("a" to 1)
来源：http://yid.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://rtk.xinyue.icu

for (i in 1..10) println(i)
来源：http://vea.nanxuanxn.top

[T15] Kotlin：接口
来源：http://dxr.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://vqu.jianghu66.top

[T16] Swift：Hello World
来源：http://dqo.cucudq.cn

print("Hello")
来源：http://erm.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://ifr.zhengqikj.top

var a = 1;  let b = 2
来源：http://rbb.gotoacloud.top

[T18] Swift：字符串插值
来源：http://dci.tian-w.cn

"值: \(b)"
来源：http://inp.jiagoushi.top

[T19] Swift：可选绑定
来源：http://ixx.dashuyun.cn

if let n = opt { print(n) }
来源：http://fdj.meibo888.top

[T20] Swift：数组操作
来源：http://uxm.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://bgd.meibo888.top

[T21] Swift：遍历
来源：http://ndt.havefunace.top

for x in a { print(x) }
来源：http://zsd.yongpay.top

[T22] Swift：字典
来源：http://iak.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://tny.hongshengwenyu.top

[T23] Swift：函数
来源：http://tmf.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://grt.nanxuanxn.top

[T24] Swift：闭包
来源：http://fwd.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zfa.xuetiantiany.cn

[T25] Swift：结构体
来源：http://fjq.zhijiandao.cn

struct P { var x: Int }
来源：http://rgw.jinqigufen.top

[T26] Swift：类与重写
来源：http://kjj.dianchejie.cn

class A: Base { override func f() {} }
来源：http://tmd.cucudq.cn

[T27] Swift：错误处理
来源：http://prn.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://sua.zhijiandao.cn

[T28] Swift：枚举
来源：http://xnf.pengpengdd.cyou

enum Color { case red, green }
来源：http://osk.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://qyy.yj20258888.top

guard let x = opt else { return }
来源：http://jva.jlsjyb.cn

[T30] Swift：协议
来源：http://lgt.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://qkl.316326.xyz

[T31] Lua：Hello World
来源：http://fzs.52xcode.cn

print("Hello")
来源：http://fue.sufxvd.cn

[T32] Lua：局部变量
来源：http://pen.hywenlv.cn

local a = 1
来源：http://qzu.gogol.net.cn

[T33] Lua：表（数组）
来源：http://tmd.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vnu.ybcxt.top

[T34] Lua：遍历表
来源：http://ygf.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qzf.redwolf501.top

[T35] Lua：字典表
来源：http://vcm.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://pws.vqdsnc.cn

[T36] Lua：函数
来源：http://ixg.cheryme.top

function add(a, b) return a + b end
来源：http://wcj.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://aod.gogol.net.cn

"a" .. "b"
来源：http://ghg.yvedp.cn

[T38] Lua：条件
来源：http://blb.hywenlv.cn

if x > 0 then print("正") end
来源：http://lty.c1oappe.top

[T39] Lua：模式匹配
来源：http://oli.zhengqikj.top

string.find(s, "%d+")
来源：http://nop.ydjk.org.cn

[T40] Lua：元表
来源：http://vkw.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://cww.zhijiandao.cn

[T41] Perl：Hello World
来源：http://qwl.shanyushiyangtech.top

print "Hello\n";
来源：http://bdt.jqgfzy.top

[T42] Perl：变量类型
来源：http://pcm.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yto.0kj1m.cn

[T43] Perl：字符串插值
来源：http://tki.shzxlz.cn

"值: $a"
来源：http://sqk.hfpthk.cn

[T44] Perl：条件
来源：http://cas.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://yil.xziqi.cn

[T45] Perl：数组遍历
来源：http://hnj.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://hqx.52xcode.cn

[T46] Perl：哈希操作
来源：http://wks.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tjj.fengsongda.top

[T47] Perl：正则捕获
来源：http://bsc.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mez.sysykeji.top

[T48] Perl：正则替换
来源：http://ebu.hnqzz.top

$s =~ s/old/new/g;
来源：http://sqk.tian-w.cn

[T49] Perl：函数
来源：http://lum.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yyv.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://akd.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uin.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://qto.yuxming.cn

[T51] Scala：Hello World
来源：http://wnx.hnqzz.top

println("Hello")
来源：http://boz.shuidangran.top

[T52] Scala：变量
来源：http://ela.pengpengdd.cyou


<!-- 参考信息 -->