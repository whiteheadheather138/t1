代发 wailian999

find . -name "*.log" -type f
来源：http://jnw.52xcode.cn

[R44] 按修改时间查找
来源：http://xvh.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://eds.hnxiangtu.top

[R45] 批量删除
来源：http://idg.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://apw.c1oappe.top

[R46] 递归替换文件内容
来源：http://hyn.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nyd.hnxiangtu.top

[R47] sed 单行替换
来源：http://lfg.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://qhi.zdqjudy.top

[R48] awk 取指定列
来源：http://hsl.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://ilw.jqgufenzy.top

[R49] awk 带条件
来源：http://cev.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rbc.hongshengwenyu.top

[R50] awk 求和
来源：http://bmw.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://shb.zhixingplan.top

[R51] 排序去重取前几
来源：http://pvj.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ogj.wangdashe.top

[R52] 统计行数
来源：http://yil.feifeiyinyue.top

wc -l a.txt
来源：http://vpg.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://ufq.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uhr.yuanzhike.top

[R54] 比较两个文件
来源：http://ovx.ivvv.top

diff a.txt b.txt
来源：http://zju.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://yzw.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdu.hnxiangtu.top

[R56] 远程拷贝
来源：http://fqa.9152youxi.cn

scp file user@host:/path/
来源：http://law.shzxlz.cn

[R57] 远程执行命令
来源：http://cve.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://wck.ctjpmb.com

[R58] 下载文件
来源：http://irw.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sro.vehdjk.com

[R59] 发 POST JSON
来源：http://xnz.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rcn.sweek.top

[R60] 只看 HTTP 状态码
来源：http://nik.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bed.tianlin.xyz

[R61] 磁盘占用
来源：http://yhl.cheryme.top

df -h;  du -sh *
来源：http://oyg.316326.xyz

[R62] 找最占空间的文件
来源：http://cnr.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://row.hongshengwenyu.top

[R63] 内存与进程
来源：http://hji.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://cmq.fktsv.cn

[R64] 结束进程
来源：http://ojk.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://fev.chenzaomai.com

[R65] 查看端口占用
来源：http://ogu.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oxx.nanxinkj.top

[R66] 定时任务
来源：http://mhb.hnxiangtu.top

crontab -e;  crontab -l
来源：http://asd.cheryme.top

[R67] 生成随机十六进制串
来源：http://uyp.hfpthk.cn

openssl rand -hex 16
来源：http://olm.zycfv.cn

[R68] 计算文件校验值
来源：http://ots.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rye.yonumen.top

[R69] 生成随机密码
来源：http://buv.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://utw.316326.xyz

[R70] 时间戳与互转
来源：http://mmf.iojbl.cn

date +%s;  date -d @1700000000
来源：http://vsv.guannengcc.top

[R71] 日期格式化
来源：http://kbs.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://syp.ydjk.org.cn

[R72] 等待端口就绪
来源：http://gvw.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jia.iojbl.cn

[R73] 分割大日志
来源：http://toz.jqgufenzy.top

split -l 1000 big.log part_
来源：http://azn.gzhubu.top

[R74] 批量重命名
来源：http://iwx.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dxh.gaohongyu789.top

[R75] 导出环境变量
来源：http://jnn.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://bmb.tian-w.cn

[R76] 使用临时文件
来源：http://nvs.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ynn.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://grl.chenlongwang.top

read -rp "请输入: " ans
来源：http://qqz.nwbrower.top

[R78] 交互式菜单
来源：http://uwm.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oky.nanxinkj.top

[R79] 解析命令行选项
来源：http://ipp.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ggm.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://xmg.aizwys.cn

time ./run.sh
来源：http://fcp.xuetiantiany.cn

================================================================================
来源：http://vma.jinghuilouyu.cn

S. C / C++ 专题
来源：http://rjo.pycfn.com

================================================================================
来源：http://uon.zhixingplan.top

[S01] C：Hello World
来源：http://mjo.cheryme.top

#include <stdio.h>
来源：http://lkt.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://max.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://hii.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://byx.yueranfly.top

[S03] C：读入整数
来源：http://pyc.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://sgq.zdqjudy.top

[S04] C：字符串复制
来源：http://oho.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gib.snrcjt.cn

[S05] C：字符串长度
来源：http://zij.daxiang520.top

strlen(s)
来源：http://gaw.vqdsnc.cn

[S06] C：字符串比较
来源：http://flk.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://jea.316326.xyz

[S07] C：数组遍历求和
来源：http://gmu.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bwu.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://zet.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qbq.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://ccp.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://meh.bbcook.cn

[S10] C：指针与解引用
来源：http://wiu.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://knj.dianchejie.cn

[S11] C：逐行读文件
来源：http://pod.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://yrw.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ysl.shzxlz.cn

fclose(f);
来源：http://gfn.epnwcf.com

[S12] C：写文件
来源：http://hur.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mpp.wangshuangyany.cn

[S13] C：宏定义
来源：http://mhq.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://avi.hywenlv.cn

[S14] C：枚举
来源：http://pjx.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://cpd.gogol.net.cn

[S15] C：类型转换
来源：http://xlv.fehbvm.com

(double) a / b
来源：http://szq.hnxiangtu.top

[S16] C：位操作置位
来源：http://xfd.pycfn.com

x |= (1 << 3);
来源：http://ofc.52xcode.cn

[S17] C：安全拼接字符串
来源：http://pxf.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gha.ydzc1.top

[S18] C：命令行参数
来源：http://ojg.sxryk.cn

int main(int argc, char **argv)
来源：http://hpb.redwolf501.top

[S19] C：快速排序
来源：http://vmm.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://nwr.tianlin.xyz

[S20] C：二分查找
来源：http://afm.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fgq.smart0.xyz

[S21] C：字符类别判断
来源：http://tsc.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tzz.tianlin.xyz

[S22] C：字符串转数字
来源：http://wrw.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://zhx.mhx1999.top

[S23] C：随机数
来源：http://nhh.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ood.jianghu66.top

[S24] C：获取本地时间
来源：http://ybw.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hfd.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://ith.hfpthk.cn

memcpy(dst, src, n);
来源：http://mhi.sxryk.cn

[S26] C：内存清零
来源：http://cle.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://egy.hnxiangtu.top

[S27] C：定义常量
来源：http://akd.ivvv.top

const double PI = 3.14159;
来源：http://wda.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://syc.hongshengwenyu.top

static int counter = 0;
来源：http://kor.jinghuilouyu.cn

[S29] C：变参函数
来源：http://wji.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jgu.hysaishi.cn

[S30] C：头文件保护
来源：http://epf.vehdjk.com

#ifndef X_H
来源：http://pkt.ywan-chungtsiang.top

#define X_H
来源：http://sva.zhaomingkeji.xyz

#endif
来源：http://ejb.hywenlv.cn

[S31] C++：Hello World
来源：http://dbx.yanxiufei.cn

#include <iostream>
来源：http://qmp.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://coc.vehdjk.com

[S32] C++：字符串
来源：http://cne.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://dgl.shuidangran.top

[S33] C++：vector 增删
来源：http://vru.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kgq.haohaochexian.top

[S34] C++：遍历 vector
来源：http://gdo.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://fvm.shuidangran.top

[S35] C++：map
来源：http://okz.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://odv.daria6918.cn

[S36] C++：unordered_map
来源：http://hjy.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xge.fktsv.cn

[S37] C++：set
来源：http://uiq.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jgr.fehbvm.com

[S38] C++：排序
来源：http://vgo.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://zqr.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://zat.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://upe.fehbvm.com

[S40] C++：查找元素
来源：http://qzz.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xuf.bbcook.cn

[S41] C++：类与构造函数
来源：http://ysa.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rjs.uphjek.com

[S42] C++：继承与虚函数
来源：http://udn.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://chg.jyoumei.cn

[S43] C++：智能指针
来源：http://tbj.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://sjk.vehdjk.com

[S44] C++：引用传参
来源：http://dux.fehbvm.com

void inc(int &x) { ++x; }
来源：http://fji.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://iwy.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://xco.shangyingyoupin.top

[S46] C++：函数模板
来源：http://tzk.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aoa.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://ysy.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wyv.tarul.cn

[S48] C++：逐行读文件
来源：http://ees.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://vgv.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://mgz.chenzaomai.com

[S49] C++：写文件
来源：http://yni.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxe.dashuyun.cn

[S50] C++：格式化数字
来源：http://xoe.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://acj.yangfankeji.com

[S51] C++：显式类型转换
来源：http://jyg.chenzaomai.com

static_cast<double>(a) / b
来源：http://ysh.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://dgl.pycfn.com

int size() const noexcept { return n_; }
来源：http://lop.zhongyouzk.top

[S53] C++：移动语义
来源：http://wjp.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://bti.pengpengdd.cyou

[S54] C++：异常处理
来源：http://eak.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ofk.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://ugy.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xzq.yj202588.top

[S56] C++：optional
来源：http://oxt.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yjt.yanxiufei.cn

[S57] C++：编译期常量
来源：http://pry.smart0.xyz

constexpr int N = 10;
来源：http://aig.yj20258.top

[S58] C++：命名空间
来源：http://gtz.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://mac.jiagoushi.top

[S59] C++：静态断言
来源：http://qam.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cqx.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://klk.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uxq.fanxiaobao.xyz

================================================================================
来源：http://njp.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hit.xuanzx.com

================================================================================
来源：http://uor.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://zcq.xingfuxueyuan.xyz

println("Hello")
来源：http://ppx.yfazqb.com

[T02] Kotlin：变量
来源：http://nxh.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rqh.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://twf.shanyushiyangkeji.top

"值: $b"
来源：http://iak.sxryk.cn

[T04] Kotlin：空安全
来源：http://aju.hysaishi.cn

val n: String? = null;  n?.length
来源：http://ysj.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://qsh.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://slk.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://fku.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pyo.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://ksc.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xjh.c1oappe.top

[T08] Kotlin：数据类
来源：http://gbj.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://wzj.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://tni.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://gec.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://zuv.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://csm.quarkkingdee.top

[T11] Kotlin：协程
来源：http://vrl.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rbb.nwbrower.top

[T12] Kotlin：解构声明
来源：http://gob.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://tyb.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://znz.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://ljs.haohaochexian.top

[T14] Kotlin：循环
来源：http://uus.ybcxt.top

for (i in 1..10) println(i)
来源：http://sum.bjfxy.top

[T15] Kotlin：接口
来源：http://wyf.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://heo.jiagoushi.top

[T16] Swift：Hello World
来源：http://mnt.aibaodan.cn

print("Hello")
来源：http://ayh.jinqigufen.top

[T17] Swift：变量与常量
来源：http://zur.svipenyu.cn

var a = 1;  let b = 2
来源：http://mng.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://lwx.yongpay.top

"值: \(b)"
来源：http://bhc.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://mzi.yj20258888.top

if let n = opt { print(n) }
来源：http://sgy.gogol.net.cn

[T20] Swift：数组操作
来源：http://odt.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://hyv.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://hnn.zhixingplan.top

for x in a { print(x) }
来源：http://oxk.zhixingplan.top

[T22] Swift：字典
来源：http://rbp.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fvc.gotoacloud.top

[T23] Swift：函数
来源：http://ltt.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zvl.hongshengwenyu.top

[T24] Swift：闭包
来源：http://eng.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lho.sysykeji.top

[T25] Swift：结构体
来源：http://rty.cashguo.top

struct P { var x: Int }
来源：http://zdj.zhixingplan.top

[T26] Swift：类与重写
来源：http://hno.yfazqb.com

class A: Base { override func f() {} }
来源：http://zxz.zdqjudy.top

[T27] Swift：错误处理
来源：http://obt.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://ufe.shuidangran.top

[T28] Swift：枚举
来源：http://mpm.hesvh.cn

enum Color { case red, green }
来源：http://gvq.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://pmy.xylfe.cn

guard let x = opt else { return }
来源：http://utl.svipenyu.cn

[T30] Swift：协议
来源：http://hof.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://mpq.uphjek.com

[T31] Lua：Hello World
来源：http://koe.dashuyun.cn

print("Hello")
来源：http://upv.ydzc1.top

[T32] Lua：局部变量
来源：http://sqp.zhaomingkeji.xyz

local a = 1
来源：http://hza.sysykeji.top

[T33] Lua：表（数组）
来源：http://lqx.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://flb.xziqi.cn

[T34] Lua：遍历表
来源：http://mhm.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pwn.chenjidiqi.icu

[T35] Lua：字典表
来源：http://qbn.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://hih.gaohongyu789.top

[T36] Lua：函数
来源：http://prl.tianlin.xyz

function add(a, b) return a + b end
来源：http://ler.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://cgl.pengpengdd.cyou

"a" .. "b"
来源：http://agb.gzhubu.top

[T38] Lua：条件
来源：http://ixy.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://exp.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://rly.bjfxy.top

string.find(s, "%d+")
来源：http://uly.xuetiantiany.cn

[T40] Lua：元表
来源：http://nue.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://elh.iojbl.cn

[T41] Perl：Hello World
来源：http://spc.andypj.xyz

print "Hello\n";
来源：http://qps.guowangkeji.top

[T42] Perl：变量类型
来源：http://ubr.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kro.chenzaomai.com

[T43] Perl：字符串插值
来源：http://izj.haohaochexian.top

"值: $a"
来源：http://irn.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://kbu.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://eos.redwolf501.top

[T45] Perl：数组遍历
来源：http://huh.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://nil.nwbrower.top

[T46] Perl：哈希操作
来源：http://uqg.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://apo.tian-w.cn


<!-- 参考信息 -->