代发 wailian999

find . -name "*.tmp" -delete
来源：http://wtg.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://dsn.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://osw.hongshengwenyu.top

[R47] sed 单行替换
来源：http://wji.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tky.yfazqb.com

[R48] awk 取指定列
来源：http://gms.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://hmq.haohaochexian.top

[R49] awk 带条件
来源：http://yjx.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://frv.tian-w.cn

[R50] awk 求和
来源：http://zwv.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://owe.birdmap.top

[R51] 排序去重取前几
来源：http://say.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://awq.fktsv.cn

[R52] 统计行数
来源：http://axx.hysaishi.cn

wc -l a.txt
来源：http://gyr.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://zul.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jmu.quarkkingdee.top

[R54] 比较两个文件
来源：http://yhk.havefunace.top

diff a.txt b.txt
来源：http://vvn.vqdsnc.cn

[R55] 压缩与解压
来源：http://kad.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rsh.feifeiyinyue.top

[R56] 远程拷贝
来源：http://cqw.yfazqb.com

scp file user@host:/path/
来源：http://aof.uphjek.com

[R57] 远程执行命令
来源：http://iwd.epnwcf.com

ssh user@host 'uptime'
来源：http://ign.chenlongwang.top

[R58] 下载文件
来源：http://vjp.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqt.52xcode.cn

[R59] 发 POST JSON
来源：http://amq.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zgn.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://mkm.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pce.fengsongda.top

[R61] 磁盘占用
来源：http://nkb.yanxiufei.cn

df -h;  du -sh *
来源：http://ufb.gogol.net.cn

[R62] 找最占空间的文件
来源：http://irc.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://xvt.iojbl.cn

[R63] 内存与进程
来源：http://wyn.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://uhd.bjfxy.top

[R64] 结束进程
来源：http://urq.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://vhr.dianchejie.cn

[R65] 查看端口占用
来源：http://opm.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://adb.yonumen.top

[R66] 定时任务
来源：http://lnu.zycfv.cn

crontab -e;  crontab -l
来源：http://ygt.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://are.tarul.cn

openssl rand -hex 16
来源：http://vxc.yj202588.top

[R68] 计算文件校验值
来源：http://xew.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://hpb.fktsv.cn

[R69] 生成随机密码
来源：http://knu.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://eip.zhixingplan.top

[R70] 时间戳与互转
来源：http://rne.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://akx.yuxming.cn

[R71] 日期格式化
来源：http://nrh.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jxj.xinyue.icu

[R72] 等待端口就绪
来源：http://evk.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fbq.aibaodan.cn

[R73] 分割大日志
来源：http://bbg.xinyue.icu

split -l 1000 big.log part_
来源：http://wpe.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://max.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rhr.epnwcf.com

[R75] 导出环境变量
来源：http://ghu.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://rcj.ybcxt.top

[R76] 使用临时文件
来源：http://hfl.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fok.shuidangran.top

[R77] 读取用户输入
来源：http://ffz.yueranfly.top

read -rp "请输入: " ans
来源：http://ukm.xuetiantiany.cn

[R78] 交互式菜单
来源：http://myd.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jbp.chenlongwang.top

[R79] 解析命令行选项
来源：http://syw.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://juc.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://dtc.jyoumei.cn

time ./run.sh
来源：http://lkp.aibaodan.cn

================================================================================
来源：http://jum.meibo888.top

S. C / C++ 专题
来源：http://miv.xingfuxueyuan.xyz

================================================================================
来源：http://kvm.quarkkingdee.top

[S01] C：Hello World
来源：http://wik.fzhhl.top

#include <stdio.h>
来源：http://qdf.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ofq.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://ulk.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://auv.snrcjt.cn

[S03] C：读入整数
来源：http://ogs.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://jvr.guowangkeji.top

[S04] C：字符串复制
来源：http://esy.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ygq.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://ahi.c1oappe.top

strlen(s)
来源：http://cia.gzhubu.top

[S06] C：字符串比较
来源：http://urz.9152youxi.cn

strcmp(a, b) == 0
来源：http://bcb.shuidangran.top

[S07] C：数组遍历求和
来源：http://brd.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://equ.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://czk.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kfs.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://ifj.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uns.ctjpmb.com

[S10] C：指针与解引用
来源：http://rhj.uphjek.com

int *p = &a;  *p = 5;
来源：http://erj.zhijiandao.cn

[S11] C：逐行读文件
来源：http://hhq.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://nwk.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wek.wangshuangyany.cn

fclose(f);
来源：http://izy.yfazqb.com

[S12] C：写文件
来源：http://icx.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://csp.havefunace.top

[S13] C：宏定义
来源：http://bcb.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyx.yuanzhike.top

[S14] C：枚举
来源：http://gxq.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://apc.jinqigfzy.top

[S15] C：类型转换
来源：http://ufm.shzxlz.cn

(double) a / b
来源：http://ciy.yj20258888.top

[S16] C：位操作置位
来源：http://qjm.guowangkeji.top

x |= (1 << 3);
来源：http://zjr.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://jsr.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fus.wangdashe.top

[S18] C：命令行参数
来源：http://pfx.iojbl.cn

int main(int argc, char **argv)
来源：http://jwa.cucudq.cn

[S19] C：快速排序
来源：http://wzu.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ajo.xylfe.cn

[S20] C：二分查找
来源：http://pwa.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ccc.bbcook.cn

[S21] C：字符类别判断
来源：http://irr.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lkn.gotoacloud.top

[S22] C：字符串转数字
来源：http://tha.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vje.hysaishi.cn

[S23] C：随机数
来源：http://enh.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rfn.vqdsnc.cn

[S24] C：获取本地时间
来源：http://gvu.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqd.hnxiangtu.top

[S25] C：内存拷贝
来源：http://zor.52xcode.cn

memcpy(dst, src, n);
来源：http://csz.jqgfzy.top

[S26] C：内存清零
来源：http://mxl.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://pvl.yj20258888.top

[S27] C：定义常量
来源：http://swl.uphjek.com

const double PI = 3.14159;
来源：http://uai.pycfn.com

[S28] C：静态变量
来源：http://tmn.ctjpmb.com

static int counter = 0;
来源：http://khk.gotoacloud.top

[S29] C：变参函数
来源：http://xca.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://phh.ivvv.top

[S30] C：头文件保护
来源：http://mgc.mhx1999.top

#ifndef X_H
来源：http://puf.hcnkem.com

#define X_H
来源：http://jbc.cqqwz.cn

#endif
来源：http://uzp.cheryme.top

[S31] C++：Hello World
来源：http://vfq.zhoulong.xyz

#include <iostream>
来源：http://tha.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://nya.yonumen.top

[S32] C++：字符串
来源：http://xkk.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://lty.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://eis.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rfc.bjfxy.top

[S34] C++：遍历 vector
来源：http://zlm.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://ibk.wangdashe.top

[S35] C++：map
来源：http://eqb.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wms.daria6918.cn

[S36] C++：unordered_map
来源：http://jow.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ttn.zhengqikj.top

[S37] C++：set
来源：http://pyw.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://odn.tian-w.cn

[S38] C++：排序
来源：http://bvt.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://hyr.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://cfo.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pyq.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://her.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://riy.ydzc1.top

[S41] C++：类与构造函数
来源：http://gqi.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xnu.bbcook.cn

[S42] C++：继承与虚函数
来源：http://vsz.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://far.fktsv.cn

[S43] C++：智能指针
来源：http://nnx.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://ows.fehbvm.com

[S44] C++：引用传参
来源：http://oyq.tarul.cn

void inc(int &x) { ++x; }
来源：http://jox.0kj1m.cn

[S45] C++：lambda
来源：http://axd.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://bof.yuanzhike.top

[S46] C++：函数模板
来源：http://qpg.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://act.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://nzw.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nbl.sweek.top

[S48] C++：逐行读文件
来源：http://ruw.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://cbg.ydzc1.top

while (std::getline(in, line)) { }
来源：http://oay.zdbjq.cn

[S49] C++：写文件
来源：http://agc.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ekf.zhengqikj.top

[S50] C++：格式化数字
来源：http://osn.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vsj.tianlin.xyz

[S51] C++：显式类型转换
来源：http://vxu.hcnkem.com

static_cast<double>(a) / b
来源：http://hku.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://ivg.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://mtw.jqgfzy.top

[S53] C++：移动语义
来源：http://arf.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://epp.havefunace.top

[S54] C++：异常处理
来源：http://eip.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvw.zycfv.cn

[S55] C++：结构化绑定
来源：http://suv.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cyd.yuxming.cn

[S56] C++：optional
来源：http://tnh.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hlj.hywenlv.cn

[S57] C++：编译期常量
来源：http://ghr.0kj1m.cn

constexpr int N = 10;
来源：http://nhx.iojbl.cn

[S58] C++：命名空间
来源：http://syt.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://qrv.gzhubu.top

[S59] C++：静态断言
来源：http://vvt.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ykz.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://smj.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://itf.tarul.cn

================================================================================
来源：http://cjc.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bkq.ywan-chungtsiang.top

================================================================================
来源：http://dur.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://ztu.feifeiyinyue.top

println("Hello")
来源：http://ndt.nanxuanxn.top

[T02] Kotlin：变量
来源：http://ugs.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sbz.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://zjh.hongshengwenyu.top

"值: $b"
来源：http://xhw.yonumen.top

[T04] Kotlin：空安全
来源：http://poa.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://ovz.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://ndf.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fzm.meibo888.top

[T06] Kotlin：集合映射
来源：http://rgv.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eyu.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://qon.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipm.pycfn.com

[T08] Kotlin：数据类
来源：http://nzt.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://tjv.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://dru.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://lxh.gzhubu.top

[T10] Kotlin：默认参数
来源：http://ocp.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ynu.zhoulong.xyz

[T11] Kotlin：协程
来源：http://qgy.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hrl.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://rnb.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://ihz.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://rag.hnqzz.top

val m = mapOf("a" to 1)
来源：http://pck.tian-w.cn

[T14] Kotlin：循环
来源：http://udo.52xcode.cn

for (i in 1..10) println(i)
来源：http://nmg.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://xyp.yueranfly.top

interface Shape { fun area(): Double }
来源：http://xah.iojbl.cn

[T16] Swift：Hello World
来源：http://vrk.kuanghao11.cn

print("Hello")
来源：http://hqt.wangdashe.top

[T17] Swift：变量与常量
来源：http://lxo.hammf.cn

var a = 1;  let b = 2
来源：http://oil.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://mvj.jlsjyb.cn

"值: \(b)"
来源：http://nrf.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://upr.gaohongyu789.top

if let n = opt { print(n) }
来源：http://okq.bjfxy.top

[T20] Swift：数组操作
来源：http://vub.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wco.jlsjyb.cn

[T21] Swift：遍历
来源：http://ohp.yj20258.top

for x in a { print(x) }
来源：http://azv.chenzaomai.com

[T22] Swift：字典
来源：http://ntu.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://xex.vehdjk.com

[T23] Swift：函数
来源：http://quk.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://biu.snrcjt.cn

[T24] Swift：闭包
来源：http://ywq.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wnt.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://eru.ctjpmb.com

struct P { var x: Int }
来源：http://avj.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://uti.ivvv.top

class A: Base { override func f() {} }
来源：http://ywb.fengsongda.top

[T27] Swift：错误处理
来源：http://fyc.fzhhl.top

do { try f() } catch { print(error) }
来源：http://gdm.yuanzhike.top

[T28] Swift：枚举
来源：http://rvc.sjlbkw.cn

enum Color { case red, green }
来源：http://jjk.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://fun.zdbjq.cn

guard let x = opt else { return }
来源：http://nzz.chenjidiqi.icu

[T30] Swift：协议
来源：http://tzs.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://tfo.uphjek.com

[T31] Lua：Hello World
来源：http://sxr.hnqzz.top

print("Hello")
来源：http://dso.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://bzh.hywenlv.cn

local a = 1
来源：http://hfm.yvedp.cn

[T33] Lua：表（数组）
来源：http://hjt.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mqm.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://flx.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://ggd.hysaishi.cn

[T35] Lua：字典表
来源：http://ihh.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://chg.wangdashe.top

[T36] Lua：函数
来源：http://adz.dianchejie.cn

function add(a, b) return a + b end
来源：http://vml.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://yzm.jianghu66.top

"a" .. "b"
来源：http://ycy.zhoulong.xyz

[T38] Lua：条件
来源：http://grl.havefunace.top

if x > 0 then print("正") end
来源：http://nzm.guannengcc.top

[T39] Lua：模式匹配
来源：http://bze.birdmap.top

string.find(s, "%d+")
来源：http://mzb.pengpengdd.cyou

[T40] Lua：元表
来源：http://kgp.andypj.xyz

setmetatable({}, { __index = base })
来源：http://kgy.tianlin.xyz

[T41] Perl：Hello World
来源：http://tky.hcnkem.com

print "Hello\n";
来源：http://khb.gaohongyu789.top

[T42] Perl：变量类型
来源：http://gbg.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vhh.ctjpmb.com

[T43] Perl：字符串插值
来源：http://umr.tian-w.cn

"值: $a"
来源：http://bxh.hnxiangtu.top

[T44] Perl：条件
来源：http://tuc.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://tdf.9152youxi.cn

[T45] Perl：数组遍历
来源：http://eym.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://vdi.fzhhl.top

[T46] Perl：哈希操作
来源：http://jda.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rsj.haohaochexian.top

[T47] Perl：正则捕获
来源：http://ijq.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://eqs.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://qbz.yonumen.top

$s =~ s/old/new/g;
来源：http://uaf.c1oappe.top


<!-- 参考信息 -->