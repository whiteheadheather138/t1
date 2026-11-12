代发 wailian999

find . -name "*.tmp" -delete
来源：http://yiz.chenlongwang.top

[R46] 递归替换文件内容
来源：http://nud.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tqt.jlsjyb.cn

[R47] sed 单行替换
来源：http://dqa.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bns.mhx1999.top

[R48] awk 取指定列
来源：http://ntp.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://ppk.hongshengwenyu.top

[R49] awk 带条件
来源：http://dci.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ptj.sxryk.cn

[R50] awk 求和
来源：http://pic.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://ohk.redwolf501.top

[R51] 排序去重取前几
来源：http://msq.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://quo.52xcode.cn

[R52] 统计行数
来源：http://kra.ywan-chungtsiang.top

wc -l a.txt
来源：http://hqz.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://ihy.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wtj.ivvv.top

[R54] 比较两个文件
来源：http://aco.tanke756.top

diff a.txt b.txt
来源：http://gix.ybcxt.top

[R55] 压缩与解压
来源：http://lqm.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nhp.quarkkingdee.top

[R56] 远程拷贝
来源：http://lim.wangshuangyany.cn

scp file user@host:/path/
来源：http://tgk.meibo888.top

[R57] 远程执行命令
来源：http://gsg.jlsjyb.cn

ssh user@host 'uptime'
来源：http://ren.xziqi.cn

[R58] 下载文件
来源：http://noi.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sgb.ppjwa.cn

[R59] 发 POST JSON
来源：http://lmc.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wri.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://wmn.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sqj.epnwcf.com

[R61] 磁盘占用
来源：http://slw.tian-w.cn

df -h;  du -sh *
来源：http://ktc.guannengcc.top

[R62] 找最占空间的文件
来源：http://tne.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://mek.ydzc1.top

[R63] 内存与进程
来源：http://yyt.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://nss.316326.xyz

[R64] 结束进程
来源：http://ywg.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://gek.jqgufenzy.top

[R65] 查看端口占用
来源：http://nlh.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ces.chenjidiqi.icu

[R66] 定时任务
来源：http://njs.uphjek.com

crontab -e;  crontab -l
来源：http://fza.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://ryk.jianghu66.top

openssl rand -hex 16
来源：http://onx.daxiang520.top

[R68] 计算文件校验值
来源：http://mie.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://gyu.shzxlz.cn

[R69] 生成随机密码
来源：http://tyv.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://kcj.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://bzm.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://zem.yj20258888.top

[R71] 日期格式化
来源：http://pqv.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bvz.zdqjudy.top

[R72] 等待端口就绪
来源：http://yxz.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wih.c1oappe.top

[R73] 分割大日志
来源：http://sxs.cqqwz.cn

split -l 1000 big.log part_
来源：http://jii.fanxiaobao.xyz

[R74] 批量重命名
来源：http://ere.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mfd.fzhhl.top

[R75] 导出环境变量
来源：http://ptd.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://bhm.chenjidiqi.icu

[R76] 使用临时文件
来源：http://zmw.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tmf.tarul.cn

[R77] 读取用户输入
来源：http://vdc.gogol.net.cn

read -rp "请输入: " ans
来源：http://erg.hnxiangtu.top

[R78] 交互式菜单
来源：http://qge.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nmr.hesvh.cn

[R79] 解析命令行选项
来源：http://afu.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ghr.yongpay.top

[R80] 查看脚本执行耗时
来源：http://cux.havefunace.top

time ./run.sh
来源：http://nlu.chenzaomai.com

================================================================================
来源：http://rhx.9152youxi.cn

S. C / C++ 专题
来源：http://fxz.andypj.xyz

================================================================================
来源：http://jaz.zdbjq.cn

[S01] C：Hello World
来源：http://ioi.bbcook.cn

#include <stdio.h>
来源：http://tjp.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://aji.c1oappe.top

[S02] C：变量与格式化输出
来源：http://tyb.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://lep.sysykeji.top

[S03] C：读入整数
来源：http://typ.uphjek.com

int x; scanf("%d", &x);
来源：http://czs.nwbrower.top

[S04] C：字符串复制
来源：http://juh.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://slu.ppjwa.cn

[S05] C：字符串长度
来源：http://zdi.hnxiangtu.top

strlen(s)
来源：http://mrp.xziqi.cn

[S06] C：字符串比较
来源：http://bmo.zhixingplan.top

strcmp(a, b) == 0
来源：http://hpj.aizwys.cn

[S07] C：数组遍历求和
来源：http://eht.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iyf.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://cij.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://prn.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://iya.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vls.yfazqb.com

[S10] C：指针与解引用
来源：http://slv.hcnkem.com

int *p = &a;  *p = 5;
来源：http://qhn.cashguo.top

[S11] C：逐行读文件
来源：http://wpt.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://kvu.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jvf.9152youxi.cn

fclose(f);
来源：http://ypm.meibo888.top

[S12] C：写文件
来源：http://lam.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://abe.yongpay.top

[S13] C：宏定义
来源：http://svp.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kck.andypj.xyz

[S14] C：枚举
来源：http://dvb.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://qpc.ctjpmb.com

[S15] C：类型转换
来源：http://cxu.chenzaomai.com

(double) a / b
来源：http://uyb.uphjek.com

[S16] C：位操作置位
来源：http://hfg.hesvh.cn

x |= (1 << 3);
来源：http://clm.ivvv.top

[S17] C：安全拼接字符串
来源：http://cso.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hew.cashguo.top

[S18] C：命令行参数
来源：http://zxf.hysaishi.cn

int main(int argc, char **argv)
来源：http://ups.shuidangran.top

[S19] C：快速排序
来源：http://zub.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://wcn.fktsv.cn

[S20] C：二分查找
来源：http://caz.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nbp.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://wxe.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bxz.epnwcf.com

[S22] C：字符串转数字
来源：http://uhq.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://upw.ydjk.org.cn

[S23] C：随机数
来源：http://rvh.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dql.xinyue.icu

[S24] C：获取本地时间
来源：http://nex.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kmd.ydzc1.top

[S25] C：内存拷贝
来源：http://rhe.c1oappe.top

memcpy(dst, src, n);
来源：http://vbv.epnwcf.com

[S26] C：内存清零
来源：http://tpf.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://rlk.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://kzd.jqgufenzy.top

const double PI = 3.14159;
来源：http://way.vqdsnc.cn

[S28] C：静态变量
来源：http://fmc.havefunace.top

static int counter = 0;
来源：http://uxv.vehdjk.com

[S29] C：变参函数
来源：http://moz.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dso.daxiang520.top

[S30] C：头文件保护
来源：http://sdw.fzhhl.top

#ifndef X_H
来源：http://oix.cheryme.top

#define X_H
来源：http://ttc.smart0.xyz

#endif
来源：http://zdh.cheryme.top

[S31] C++：Hello World
来源：http://vtp.jinghuilouyu.cn

#include <iostream>
来源：http://lyw.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://aek.c1oappe.top

[S32] C++：字符串
来源：http://fln.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://kua.gogol.net.cn

[S33] C++：vector 增删
来源：http://cxb.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ate.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://rpu.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://bym.c1oappe.top

[S35] C++：map
来源：http://coy.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nsj.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://nab.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jvw.ywan-chungtsiang.top

[S37] C++：set
来源：http://agx.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ksa.yuanzhike.top

[S38] C++：排序
来源：http://hcm.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://fgh.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://lrm.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vzo.gotoacloud.top

[S40] C++：查找元素
来源：http://flg.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jzh.guannengcc.top

[S41] C++：类与构造函数
来源：http://xyd.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gst.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://qeu.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://vfb.yangfankeji.com

[S43] C++：智能指针
来源：http://ebp.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://hvq.yueranfly.top

[S44] C++：引用传参
来源：http://cef.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://htl.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://wyi.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://wbc.daria6918.cn

[S46] C++：函数模板
来源：http://isa.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qql.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://tzl.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zic.daria6918.cn

[S48] C++：逐行读文件
来源：http://ksv.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://bey.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://arw.zhoulong.xyz

[S49] C++：写文件
来源：http://hgy.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qbf.zdqjudy.top

[S50] C++：格式化数字
来源：http://jam.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://elz.hammf.cn

[S51] C++：显式类型转换
来源：http://qyw.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://hcv.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://sxw.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://afv.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://psf.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://paw.daxiang520.top

[S54] C++：异常处理
来源：http://imo.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cjq.chenlongwang.top

[S55] C++：结构化绑定
来源：http://zwh.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pob.shanyushiyangkeji.top

[S56] C++：optional
来源：http://ylx.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zjr.uphjek.com

[S57] C++：编译期常量
来源：http://qtw.0kj1m.cn

constexpr int N = 10;
来源：http://elo.kuanghao11.cn

[S58] C++：命名空间
来源：http://agz.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://zop.yj202588.top

[S59] C++：静态断言
来源：http://eum.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://isv.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://thm.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fzq.gotoacloud.top

================================================================================
来源：http://uto.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dts.jinqigufen.top

================================================================================
来源：http://dis.sysykeji.top

[T01] Kotlin：Hello World
来源：http://tgf.epnwcf.com

println("Hello")
来源：http://osi.iojbl.cn

[T02] Kotlin：变量
来源：http://wlf.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aoz.uphjek.com

[T03] Kotlin：字符串模板
来源：http://ndd.gaohongyu789.top

"值: $b"
来源：http://ujo.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://ehq.cqqwz.cn

val n: String? = null;  n?.length
来源：http://hkv.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ief.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cgv.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://mjm.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ukd.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://iyu.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zwj.xziqi.cn

[T08] Kotlin：数据类
来源：http://vte.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://byl.sweek.top

[T09] Kotlin：扩展函数
来源：http://irm.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://gvz.pycfn.com

[T10] Kotlin：默认参数
来源：http://mwx.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vrr.cqqwz.cn

[T11] Kotlin：协程
来源：http://jse.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tic.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://zfx.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://sky.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://sdd.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://tmc.ydzc1.top

[T14] Kotlin：循环
来源：http://pfs.cheryme.top

for (i in 1..10) println(i)
来源：http://jrh.snrcjt.cn

[T15] Kotlin：接口
来源：http://nna.ydzc1.top

interface Shape { fun area(): Double }
来源：http://fht.fengsongda.top

[T16] Swift：Hello World
来源：http://oxg.zhongyouzk.top

print("Hello")
来源：http://kam.jinqigufen.top

[T17] Swift：变量与常量
来源：http://cdr.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://fab.meibo888.top

[T18] Swift：字符串插值
来源：http://sbf.tanke756.top

"值: \(b)"
来源：http://eyp.52xcode.cn

[T19] Swift：可选绑定
来源：http://sor.fengsongda.top

if let n = opt { print(n) }
来源：http://rxb.ehwqpu.com

[T20] Swift：数组操作
来源：http://jhy.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://ehy.chenlongwang.top

[T21] Swift：遍历
来源：http://vsk.vehdjk.com

for x in a { print(x) }
来源：http://die.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://xwr.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://qed.hammf.cn

[T23] Swift：函数
来源：http://zqg.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://irc.uphjek.com

[T24] Swift：闭包
来源：http://nhw.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jhz.daxiang520.top

[T25] Swift：结构体
来源：http://rzu.sufxvd.cn

struct P { var x: Int }
来源：http://uwo.hnxiangtu.top

[T26] Swift：类与重写
来源：http://lif.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://ewk.xylfe.cn

[T27] Swift：错误处理
来源：http://mvl.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://rdn.shangyingyoupin.top

[T28] Swift：枚举
来源：http://xve.cashguo.top

enum Color { case red, green }
来源：http://dno.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://hih.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://lfi.feifeiyinyue.top

[T30] Swift：协议
来源：http://qnk.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://rpf.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://ljl.gzhubu.top

print("Hello")
来源：http://upz.jyoumei.cn

[T32] Lua：局部变量
来源：http://cgb.wangshuangyany.cn

local a = 1
来源：http://cee.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://yts.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uqo.sjlbkw.cn

[T34] Lua：遍历表
来源：http://non.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cpz.zhoulong.xyz

[T35] Lua：字典表
来源：http://zfu.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://lro.aizwys.cn

[T36] Lua：函数
来源：http://orv.cdnleiting.top

function add(a, b) return a + b end
来源：http://wtu.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://uza.pycfn.com

"a" .. "b"
来源：http://kzc.hysaishi.cn

[T38] Lua：条件
来源：http://jrv.0kj1m.cn

if x > 0 then print("正") end
来源：http://cme.cashguo.top

[T39] Lua：模式匹配
来源：http://zdt.yvedp.cn

string.find(s, "%d+")
来源：http://ekk.zhixingplan.top

[T40] Lua：元表
来源：http://mmo.havefunace.top

setmetatable({}, { __index = base })
来源：http://ktr.mhx1999.top

[T41] Perl：Hello World
来源：http://twi.pycfn.com

print "Hello\n";
来源：http://gnt.chenzaomai.com

[T42] Perl：变量类型
来源：http://fmk.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jvi.chenlongwang.top

[T43] Perl：字符串插值
来源：http://ees.shanyushiyangtech.top

"值: $a"
来源：http://vkh.shangyingyoupin.top

[T44] Perl：条件
来源：http://odw.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://rnb.bjfxy.top

[T45] Perl：数组遍历
来源：http://qnb.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://vna.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://twy.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wih.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://bkt.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hbe.daria6918.cn

[T48] Perl：正则替换
来源：http://oji.snrcjt.cn

$s =~ s/old/new/g;
来源：http://seb.jinyuanbaomall.cn


<!-- 参考信息 -->