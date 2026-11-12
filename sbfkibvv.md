代发 wailian999

cmd >/dev/null 2>&1
来源：http://ryf.redwolf501.top

[R42] 输入重定向
来源：http://svp.uphjek.com

wc -l < a.txt
来源：http://ngf.xziqi.cn

[R43] 按名字查找文件
来源：http://rez.gaohongyu789.top

find . -name "*.log" -type f
来源：http://wuk.guowangkeji.top

[R44] 按修改时间查找
来源：http://kmu.yj20258888.top

find . -mtime -7 -type f
来源：http://oau.tanke756.top

[R45] 批量删除
来源：http://bis.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://vxt.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://dsb.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ehw.fehbvm.com

[R47] sed 单行替换
来源：http://vbg.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cux.xuetiantiany.cn

[R48] awk 取指定列
来源：http://zcu.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://pbu.nanxuanxn.top

[R49] awk 带条件
来源：http://gpd.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lsw.ivvv.top

[R50] awk 求和
来源：http://twu.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ocj.daria6918.cn

[R51] 排序去重取前几
来源：http://fhm.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xoy.yueranfly.top

[R52] 统计行数
来源：http://ojm.hongshengwenyu.top

wc -l a.txt
来源：http://yuq.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://nuy.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kaz.haohaochexian.top

[R54] 比较两个文件
来源：http://lxp.zdbjq.cn

diff a.txt b.txt
来源：http://lfb.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://xak.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://coi.zdqjudy.top

[R56] 远程拷贝
来源：http://xgz.jqgufenzy.top

scp file user@host:/path/
来源：http://ouj.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://dqi.chenlongwang.top

ssh user@host 'uptime'
来源：http://ntb.gzhubu.top

[R58] 下载文件
来源：http://fhs.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jdf.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://ldc.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fet.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://jzs.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dwv.meibo888.top

[R61] 磁盘占用
来源：http://zoj.guowangkeji.top

df -h;  du -sh *
来源：http://rlp.redwolf501.top

[R62] 找最占空间的文件
来源：http://sbt.birdmap.top

du -ah . | sort -rh | head -10
来源：http://ldm.fengsongda.top

[R63] 内存与进程
来源：http://jkc.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://qik.chenjidiqi.icu

[R64] 结束进程
来源：http://tvt.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://pun.guannengcc.top

[R65] 查看端口占用
来源：http://bfm.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tlx.hesvh.cn

[R66] 定时任务
来源：http://yto.jiagoushi.top

crontab -e;  crontab -l
来源：http://xcw.cucudq.cn

[R67] 生成随机十六进制串
来源：http://zuz.zhengqikj.top

openssl rand -hex 16
来源：http://ltw.gaohongyu789.top

[R68] 计算文件校验值
来源：http://qge.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://vaj.yfazqb.com

[R69] 生成随机密码
来源：http://fls.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://png.wangdashe.top

[R70] 时间戳与互转
来源：http://gyw.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://yyf.daria6918.cn

[R71] 日期格式化
来源：http://fmu.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tmi.ppjwa.cn

[R72] 等待端口就绪
来源：http://gux.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bjl.meibo888.top

[R73] 分割大日志
来源：http://vmm.chenzaomai.com

split -l 1000 big.log part_
来源：http://opl.yuanzhike.top

[R74] 批量重命名
来源：http://wnl.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uec.xylfe.cn

[R75] 导出环境变量
来源：http://gdy.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://qsg.mhx1999.top

[R76] 使用临时文件
来源：http://zuq.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ojx.fengsongda.top

[R77] 读取用户输入
来源：http://apl.guowangkeji.top

read -rp "请输入: " ans
来源：http://zzl.hesvh.cn

[R78] 交互式菜单
来源：http://uje.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mxl.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://nci.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zar.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://sil.9152youxi.cn

time ./run.sh
来源：http://eze.pycfn.com

================================================================================
来源：http://alp.yfazqb.com

S. C / C++ 专题
来源：http://dwt.zdbjq.cn

================================================================================
来源：http://cpt.shangyingyoupin.top

[S01] C：Hello World
来源：http://abe.jyoumei.cn

#include <stdio.h>
来源：http://kpw.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://akx.fzhhl.top

[S02] C：变量与格式化输出
来源：http://olx.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://dgp.hysaishi.cn

[S03] C：读入整数
来源：http://swb.xuanzx.com

int x; scanf("%d", &x);
来源：http://cdz.havefunace.top

[S04] C：字符串复制
来源：http://qnv.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://vzt.nanxuanxn.top

[S05] C：字符串长度
来源：http://uff.wangdashe.top

strlen(s)
来源：http://qwa.yangfankeji.com

[S06] C：字符串比较
来源：http://eds.jianghu66.top

strcmp(a, b) == 0
来源：http://bhr.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://exe.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gmw.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://wlv.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://enz.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://oho.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sij.52xcode.cn

[S10] C：指针与解引用
来源：http://lbt.hammf.cn

int *p = &a;  *p = 5;
来源：http://zlj.yj20258.top

[S11] C：逐行读文件
来源：http://pnl.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://qsn.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://myt.uphjek.com

fclose(f);
来源：http://xyw.ehwqpu.com

[S12] C：写文件
来源：http://bsk.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oif.jlsjyb.cn

[S13] C：宏定义
来源：http://bgi.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kla.hesvh.cn

[S14] C：枚举
来源：http://jyt.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://kwh.jianghu66.top

[S15] C：类型转换
来源：http://pdg.cheryme.top

(double) a / b
来源：http://hsh.nwbrower.top

[S16] C：位操作置位
来源：http://zvw.cheryme.top

x |= (1 << 3);
来源：http://bkk.fehbvm.com

[S17] C：安全拼接字符串
来源：http://kkh.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rpj.bbcook.cn

[S18] C：命令行参数
来源：http://ytn.dianchejie.cn

int main(int argc, char **argv)
来源：http://nzj.wangdashe.top

[S19] C：快速排序
来源：http://jug.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://jjk.9152youxi.cn

[S20] C：二分查找
来源：http://gvr.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://inl.chenzaomai.com

[S21] C：字符类别判断
来源：http://ige.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mbv.yvedp.cn

[S22] C：字符串转数字
来源：http://dgc.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gpc.nanxinkj.top

[S23] C：随机数
来源：http://hfk.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://skh.hysaishi.cn

[S24] C：获取本地时间
来源：http://xwy.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eud.tarul.cn

[S25] C：内存拷贝
来源：http://ktu.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://rgy.shangyingyoupin.top

[S26] C：内存清零
来源：http://dis.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://wne.yangfankeji.com

[S27] C：定义常量
来源：http://hxb.9152youxi.cn

const double PI = 3.14159;
来源：http://txy.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://afu.yj202588.top

static int counter = 0;
来源：http://hgn.ydzc1.top

[S29] C：变参函数
来源：http://uyy.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytn.yvedp.cn

[S30] C：头文件保护
来源：http://nff.xingfuxueyuan.xyz

#ifndef X_H
来源：http://bfv.gotoacloud.top

#define X_H
来源：http://fmi.xinyue.icu

#endif
来源：http://sqm.meibo888.top

[S31] C++：Hello World
来源：http://hba.c1oappe.top

#include <iostream>
来源：http://mkt.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://owa.xylfe.cn

[S32] C++：字符串
来源：http://vjc.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://kcn.fzhhl.top

[S33] C++：vector 增删
来源：http://ekx.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ydq.zhixingplan.top

[S34] C++：遍历 vector
来源：http://svu.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://zub.ppjwa.cn

[S35] C++：map
来源：http://tdn.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bed.jyoumei.cn

[S36] C++：unordered_map
来源：http://xia.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kzr.shangyingyoupin.top

[S37] C++：set
来源：http://kel.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lgx.shangyingyoupin.top

[S38] C++：排序
来源：http://mit.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://feb.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://xce.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fae.hongshengwenyu.top

[S40] C++：查找元素
来源：http://tuw.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qyn.fktsv.cn

[S41] C++：类与构造函数
来源：http://isy.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yai.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://gpw.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://fas.nanxinkj.top

[S43] C++：智能指针
来源：http://zzk.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://ayu.jinqigfzy.top

[S44] C++：引用传参
来源：http://haw.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://qey.chenjidiqi.icu

[S45] C++：lambda
来源：http://vkb.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hjd.hnqzz.top

[S46] C++：函数模板
来源：http://ffa.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rsv.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://jsi.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sfa.andypj.xyz

[S48] C++：逐行读文件
来源：http://mrf.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://bdd.aizwys.cn

while (std::getline(in, line)) { }
来源：http://gss.pengpengdd.cyou

[S49] C++：写文件
来源：http://dfk.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://goo.aibaodan.cn

[S50] C++：格式化数字
来源：http://pya.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rgs.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://ijy.316326.xyz

static_cast<double>(a) / b
来源：http://vvp.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://vwt.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://pxa.wangdashe.top

[S53] C++：移动语义
来源：http://xoj.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://nhf.cashguo.top

[S54] C++：异常处理
来源：http://dpe.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwk.yvedp.cn

[S55] C++：结构化绑定
来源：http://uko.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lkh.nanxinkj.top

[S56] C++：optional
来源：http://ypg.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vae.snrcjt.cn

[S57] C++：编译期常量
来源：http://sjv.aizwys.cn

constexpr int N = 10;
来源：http://btb.yvedp.cn

[S58] C++：命名空间
来源：http://nyn.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://olu.hcnkem.com

[S59] C++：静态断言
来源：http://idx.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mzk.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://auk.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rtk.haohaochexian.top

================================================================================
来源：http://ykn.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://axj.gogol.net.cn

================================================================================
来源：http://siq.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://ymx.ywan-chungtsiang.top

println("Hello")
来源：http://unk.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://nna.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vnx.ivvv.top

[T03] Kotlin：字符串模板
来源：http://ywu.ywan-chungtsiang.top

"值: $b"
来源：http://mer.wangdashe.top

[T04] Kotlin：空安全
来源：http://fjk.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://jit.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://rus.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://obn.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://poi.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bnb.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://xix.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jgk.hcnkem.com

[T08] Kotlin：数据类
来源：http://wop.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://xbv.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://yng.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://dbx.xziqi.cn

[T10] Kotlin：默认参数
来源：http://exy.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://otj.52xcode.cn

[T11] Kotlin：协程
来源：http://evs.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fpl.andypj.xyz

[T12] Kotlin：解构声明
来源：http://jdn.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://xcj.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://bhk.bjfxy.top

val m = mapOf("a" to 1)
来源：http://uxc.sufxvd.cn

[T14] Kotlin：循环
来源：http://egt.cashguo.top

for (i in 1..10) println(i)
来源：http://npc.tianlin.xyz

[T15] Kotlin：接口
来源：http://uor.yj202588.top

interface Shape { fun area(): Double }
来源：http://xmp.cqqwz.cn

[T16] Swift：Hello World
来源：http://lxt.xylfe.cn

print("Hello")
来源：http://ofp.cheryme.top

[T17] Swift：变量与常量
来源：http://klv.hywenlv.cn

var a = 1;  let b = 2
来源：http://nqo.redwolf501.top

[T18] Swift：字符串插值
来源：http://dtp.vehdjk.com

"值: \(b)"
来源：http://uyy.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://wgr.epnwcf.com

if let n = opt { print(n) }
来源：http://enz.hfpthk.cn

[T20] Swift：数组操作
来源：http://cfm.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://tvy.kuanghao11.cn

[T21] Swift：遍历
来源：http://uxp.snrcjt.cn

for x in a { print(x) }
来源：http://ncr.zdbjq.cn

[T22] Swift：字典
来源：http://aac.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zzz.guannengcc.top

[T23] Swift：函数
来源：http://cry.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgu.zdqjudy.top

[T24] Swift：闭包
来源：http://drp.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qgk.gzhubu.top

[T25] Swift：结构体
来源：http://wcz.sufxvd.cn

struct P { var x: Int }
来源：http://pxb.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://rbq.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://syk.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://cks.xziqi.cn

do { try f() } catch { print(error) }
来源：http://hsm.wangdashe.top

[T28] Swift：枚举
来源：http://fyn.sysykeji.top

enum Color { case red, green }
来源：http://prd.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://brn.zhijiandao.cn

guard let x = opt else { return }
来源：http://sbq.chenlongwang.top

[T30] Swift：协议
来源：http://yns.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://kjt.sysykeji.top

[T31] Lua：Hello World
来源：http://qwm.fehbvm.com

print("Hello")
来源：http://vtu.cqqwz.cn

[T32] Lua：局部变量
来源：http://irn.52xcode.cn

local a = 1
来源：http://lcz.shuidangran.top

[T33] Lua：表（数组）
来源：http://xza.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ctq.dianchejie.cn

[T34] Lua：遍历表
来源：http://vsi.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yjg.fengsongda.top

[T35] Lua：字典表
来源：http://bnx.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://pmq.jinghuilouyu.cn

[T36] Lua：函数
来源：http://atw.jiagoushi.top

function add(a, b) return a + b end
来源：http://bbq.cucudq.cn

[T37] Lua：字符串拼接
来源：http://qfh.xylfe.cn

"a" .. "b"
来源：http://fda.hywenlv.cn

[T38] Lua：条件
来源：http://bye.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://tej.ivvv.top

[T39] Lua：模式匹配
来源：http://vjz.yonumen.top

string.find(s, "%d+")
来源：http://loi.ctjpmb.com

[T40] Lua：元表
来源：http://dne.yonumen.top

setmetatable({}, { __index = base })
来源：http://pal.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://sgw.andypj.xyz

print "Hello\n";
来源：http://xbo.yangfankeji.com

[T42] Perl：变量类型
来源：http://jka.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ful.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://jaa.guannengcc.top

"值: $a"
来源：http://qji.mhx1999.top

[T44] Perl：条件
来源：http://txn.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://smq.aizwys.cn


<!-- 参考信息 -->