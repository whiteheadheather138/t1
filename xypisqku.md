代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://tyx.yongpay.top

[R52] 统计行数
来源：http://gfl.sxryk.cn

wc -l a.txt
来源：http://cup.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://laq.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://feo.aizwys.cn

[R54] 比较两个文件
来源：http://qer.cucudq.cn

diff a.txt b.txt
来源：http://rkr.52xcode.cn

[R55] 压缩与解压
来源：http://ymw.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fzs.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://psg.xziqi.cn

scp file user@host:/path/
来源：http://jri.gotoacloud.top

[R57] 远程执行命令
来源：http://nvi.fktsv.cn

ssh user@host 'uptime'
来源：http://epq.hammf.cn

[R58] 下载文件
来源：http://wcl.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eyw.uphjek.com

[R59] 发 POST JSON
来源：http://ftz.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tig.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://lzn.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fde.haohaochexian.top

[R61] 磁盘占用
来源：http://tpm.chenjidiqi.icu

df -h;  du -sh *
来源：http://uka.fzhhl.top

[R62] 找最占空间的文件
来源：http://nlc.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://fkh.jinqigufen.top

[R63] 内存与进程
来源：http://ceh.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://qju.xuanzx.com

[R64] 结束进程
来源：http://fza.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://uqu.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://wce.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sua.jyoumei.cn

[R66] 定时任务
来源：http://ncf.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://lot.meibo888.top

[R67] 生成随机十六进制串
来源：http://fne.tianlin.xyz

openssl rand -hex 16
来源：http://eos.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://umc.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vky.havefunace.top

[R69] 生成随机密码
来源：http://zho.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://hbn.dashuyun.cn

[R70] 时间戳与互转
来源：http://iwn.316326.xyz

date +%s;  date -d @1700000000
来源：http://lnj.cucudq.cn

[R71] 日期格式化
来源：http://ula.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yot.jyoumei.cn

[R72] 等待端口就绪
来源：http://ymg.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eau.svipenyu.cn

[R73] 分割大日志
来源：http://eya.jyoumei.cn

split -l 1000 big.log part_
来源：http://fnk.uphjek.com

[R74] 批量重命名
来源：http://tuf.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vgx.cucudq.cn

[R75] 导出环境变量
来源：http://nzk.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://blk.jyoumei.cn

[R76] 使用临时文件
来源：http://xve.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bnu.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://gfe.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://gpp.shangyingyoupin.top

[R78] 交互式菜单
来源：http://hjj.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://koc.fehbvm.com

[R79] 解析命令行选项
来源：http://ecd.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wpd.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://jgy.hysaishi.cn

time ./run.sh
来源：http://uxn.nanxinkj.top

================================================================================
来源：http://qjo.tian-w.cn

S. C / C++ 专题
来源：http://qtg.tanke756.top

================================================================================
来源：http://qym.0kj1m.cn

[S01] C：Hello World
来源：http://gge.nanxuanxn.top

#include <stdio.h>
来源：http://hex.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cwb.shuidangran.top

[S02] C：变量与格式化输出
来源：http://ioq.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://wfz.0kj1m.cn

[S03] C：读入整数
来源：http://frv.daria6918.cn

int x; scanf("%d", &x);
来源：http://jnq.guowangkeji.top

[S04] C：字符串复制
来源：http://cdy.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yuc.daria6918.cn

[S05] C：字符串长度
来源：http://rjz.vehdjk.com

strlen(s)
来源：http://qgo.tanke756.top

[S06] C：字符串比较
来源：http://dxx.guowangkeji.top

strcmp(a, b) == 0
来源：http://gag.gogol.net.cn

[S07] C：数组遍历求和
来源：http://sae.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oya.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://mdz.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ybd.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://kde.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gmz.xziqi.cn

[S10] C：指针与解引用
来源：http://orh.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://nvv.yvedp.cn

[S11] C：逐行读文件
来源：http://pqh.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://rkg.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cbf.zdqjudy.top

fclose(f);
来源：http://uqh.aizwys.cn

[S12] C：写文件
来源：http://dzp.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gbc.hysaishi.cn

[S13] C：宏定义
来源：http://hqy.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcz.jyoumei.cn

[S14] C：枚举
来源：http://acx.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://mzz.ydzc1.top

[S15] C：类型转换
来源：http://qna.aizwys.cn

(double) a / b
来源：http://xap.xuanzx.com

[S16] C：位操作置位
来源：http://tzn.ydjk.org.cn

x |= (1 << 3);
来源：http://bdm.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://rmp.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rvv.hongshengwenyu.top

[S18] C：命令行参数
来源：http://vea.aizwys.cn

int main(int argc, char **argv)
来源：http://exv.hfpthk.cn

[S19] C：快速排序
来源：http://uan.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://efb.snrcjt.cn

[S20] C：二分查找
来源：http://rqu.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://txq.zhixingplan.top

[S21] C：字符类别判断
来源：http://vhq.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxx.smart0.xyz

[S22] C：字符串转数字
来源：http://zof.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://dux.hfpthk.cn

[S23] C：随机数
来源：http://gqf.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ggp.kuanghao11.cn

[S24] C：获取本地时间
来源：http://icm.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krz.yj202588.top

[S25] C：内存拷贝
来源：http://mbe.pycfn.com

memcpy(dst, src, n);
来源：http://mfz.shangyingyoupin.top

[S26] C：内存清零
来源：http://sqg.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://wgp.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://awp.jyoumei.cn

const double PI = 3.14159;
来源：http://ode.zhoulong.xyz

[S28] C：静态变量
来源：http://heb.hywenlv.cn

static int counter = 0;
来源：http://try.vqdsnc.cn

[S29] C：变参函数
来源：http://xqz.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mjw.aibaodan.cn

[S30] C：头文件保护
来源：http://tfj.guowangkeji.top

#ifndef X_H
来源：http://zaw.gotoacloud.top

#define X_H
来源：http://tyv.gaohongyu789.top

#endif
来源：http://toh.uphjek.com

[S31] C++：Hello World
来源：http://qrf.andypj.xyz

#include <iostream>
来源：http://cnn.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://bfn.zdbjq.cn

[S32] C++：字符串
来源：http://emd.tanke756.top

std::string s = "hi";  s += "!";
来源：http://otk.tianlin.xyz

[S33] C++：vector 增删
来源：http://lgm.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mac.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://ulp.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://pxg.hysaishi.cn

[S35] C++：map
来源：http://cgs.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vhq.gaohongyu789.top

[S36] C++：unordered_map
来源：http://yic.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blm.cucudq.cn

[S37] C++：set
来源：http://dtf.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ski.daria6918.cn

[S38] C++：排序
来源：http://kan.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://agw.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://xay.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fgy.9152youxi.cn

[S40] C++：查找元素
来源：http://kla.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gla.fktsv.cn

[S41] C++：类与构造函数
来源：http://bcc.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qwd.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://gdl.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://sxb.hongshengwenyu.top

[S43] C++：智能指针
来源：http://loa.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://ihx.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://omr.tarul.cn

void inc(int &x) { ++x; }
来源：http://wvm.mhx1999.top

[S45] C++：lambda
来源：http://vic.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://axo.tarul.cn

[S46] C++：函数模板
来源：http://pyf.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kix.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://dhl.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bdq.fzhhl.top

[S48] C++：逐行读文件
来源：http://hnq.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cfn.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://gxr.cucudq.cn

[S49] C++：写文件
来源：http://sol.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dja.fktsv.cn

[S50] C++：格式化数字
来源：http://tgk.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rfb.daxiang520.top

[S51] C++：显式类型转换
来源：http://add.9152youxi.cn

static_cast<double>(a) / b
来源：http://vmf.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://wxg.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://ehu.jinqigufen.top

[S53] C++：移动语义
来源：http://thh.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://zcn.tianlin.xyz

[S54] C++：异常处理
来源：http://gma.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ubt.xziqi.cn

[S55] C++：结构化绑定
来源：http://scd.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xct.pycfn.com

[S56] C++：optional
来源：http://fep.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kzt.gaohongyu789.top

[S57] C++：编译期常量
来源：http://dag.jinqigufen.top

constexpr int N = 10;
来源：http://sdh.epnwcf.com

[S58] C++：命名空间
来源：http://dec.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://rej.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://mso.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fmq.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://yxs.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://joo.xinyue.icu

================================================================================
来源：http://jaj.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xjk.hysaishi.cn

================================================================================
来源：http://dnr.fzhhl.top

[T01] Kotlin：Hello World
来源：http://gae.snrcjt.cn

println("Hello")
来源：http://lfn.xziqi.cn

[T02] Kotlin：变量
来源：http://cod.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kxm.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://xsk.ybcxt.top

"值: $b"
来源：http://pds.cheryme.top

[T04] Kotlin：空安全
来源：http://vdu.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://lav.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://czm.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kzc.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://tyn.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://llm.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://kto.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rge.52xcode.cn

[T08] Kotlin：数据类
来源：http://cjj.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://hax.pycfn.com

[T09] Kotlin：扩展函数
来源：http://vsj.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://qur.pycfn.com

[T10] Kotlin：默认参数
来源：http://out.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kgr.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://hvh.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ztz.hammf.cn

[T12] Kotlin：解构声明
来源：http://kha.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://tjq.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://kog.ivvv.top

val m = mapOf("a" to 1)
来源：http://pyp.hcnkem.com

[T14] Kotlin：循环
来源：http://gxs.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://ffl.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://ckc.yuxming.cn

interface Shape { fun area(): Double }
来源：http://qqc.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://hao.cdnleiting.top

print("Hello")
来源：http://esc.fktsv.cn

[T17] Swift：变量与常量
来源：http://ovz.xziqi.cn

var a = 1;  let b = 2
来源：http://ttr.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://dru.fengsongda.top

"值: \(b)"
来源：http://iee.yongpay.top

[T19] Swift：可选绑定
来源：http://bod.yanxiufei.cn

if let n = opt { print(n) }
来源：http://fyy.jianghu66.top

[T20] Swift：数组操作
来源：http://jap.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ivh.yj202588.top

[T21] Swift：遍历
来源：http://xkr.fanxiaobao.xyz

for x in a { print(x) }
来源：http://zag.bbcook.cn

[T22] Swift：字典
来源：http://yil.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ryg.cashguo.top

[T23] Swift：函数
来源：http://mkh.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xac.guannengcc.top

[T24] Swift：闭包
来源：http://gbc.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zar.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://ugj.cheryme.top

struct P { var x: Int }
来源：http://wpu.redwolf501.top

[T26] Swift：类与重写
来源：http://xvd.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://cts.havefunace.top

[T27] Swift：错误处理
来源：http://wca.316326.xyz

do { try f() } catch { print(error) }
来源：http://hiq.bbcook.cn

[T28] Swift：枚举
来源：http://ukt.uphjek.com

enum Color { case red, green }
来源：http://fyt.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://oqp.shuidangran.top

guard let x = opt else { return }
来源：http://ypg.zhijiandao.cn

[T30] Swift：协议
来源：http://hry.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://cxk.jqgufenzy.top

[T31] Lua：Hello World
来源：http://fpp.andypj.xyz

print("Hello")
来源：http://jsu.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://rhu.xylfe.cn

local a = 1
来源：http://yte.cucudq.cn

[T33] Lua：表（数组）
来源：http://llg.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://igw.yueranfly.top

[T34] Lua：遍历表
来源：http://las.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qie.feifeiyinyue.top

[T35] Lua：字典表
来源：http://vjg.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://sgi.birdmap.top

[T36] Lua：函数
来源：http://img.hnqzz.top

function add(a, b) return a + b end
来源：http://alw.cucudq.cn

[T37] Lua：字符串拼接
来源：http://zvf.jiagoushi.top

"a" .. "b"
来源：http://rqw.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://qlw.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://azz.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://xdh.daria6918.cn

string.find(s, "%d+")
来源：http://aym.sxryk.cn

[T40] Lua：元表
来源：http://eez.tian-w.cn

setmetatable({}, { __index = base })
来源：http://kav.xziqi.cn

[T41] Perl：Hello World
来源：http://ajy.gaohongyu789.top

print "Hello\n";
来源：http://vux.uphjek.com

[T42] Perl：变量类型
来源：http://tee.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qta.xuanzx.com

[T43] Perl：字符串插值
来源：http://epl.smart0.xyz

"值: $a"
来源：http://jpy.gotoacloud.top

[T44] Perl：条件
来源：http://sqx.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://txp.shzxlz.cn

[T45] Perl：数组遍历
来源：http://bfa.tanke756.top

for my $x (@arr) { print $x; }
来源：http://cjt.cashguo.top

[T46] Perl：哈希操作
来源：http://rcj.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hfx.andypj.xyz

[T47] Perl：正则捕获
来源：http://mpz.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mfz.gotoacloud.top

[T48] Perl：正则替换
来源：http://dtl.redwolf501.top

$s =~ s/old/new/g;
来源：http://wbd.vehdjk.com

[T49] Perl：函数
来源：http://szu.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggx.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://cln.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rwn.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://mjl.iojbl.cn

[T51] Scala：Hello World
来源：http://ykb.hysaishi.cn

println("Hello")
来源：http://omw.yj20258.top

[T52] Scala：变量
来源：http://qos.yfazqb.com

val a = 1;  var b = 2
来源：http://jdv.xuanzx.com

[T53] Scala：字符串插值
来源：http://jgg.shuidangran.top

s"值: $b"
来源：http://gok.smart0.xyz

[T54] Scala：集合映射
来源：http://thu.sufxvd.cn


<!-- 参考信息 -->