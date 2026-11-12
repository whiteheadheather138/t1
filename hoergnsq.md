代发 wailian999

cmd >/dev/null 2>&1
来源：http://rnb.zhixingplan.top

[R42] 输入重定向
来源：http://mnn.zhiwuduotai.top

wc -l < a.txt
来源：http://ueq.chenlongwang.top

[R43] 按名字查找文件
来源：http://col.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://zuh.andypj.xyz

[R44] 按修改时间查找
来源：http://srz.smart0.xyz

find . -mtime -7 -type f
来源：http://zpy.xziqi.cn

[R45] 批量删除
来源：http://wlk.c1oappe.top

find . -name "*.tmp" -delete
来源：http://pvw.svipenyu.cn

[R46] 递归替换文件内容
来源：http://dhw.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vuz.feifeiyinyue.top

[R47] sed 单行替换
来源：http://pdu.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://qea.jianghu66.top

[R48] awk 取指定列
来源：http://vmm.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://psm.jinghuilouyu.cn

[R49] awk 带条件
来源：http://lah.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://spu.cheryme.top

[R50] awk 求和
来源：http://ijt.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fzb.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://hgq.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://auc.zhiwuduotai.top

[R52] 统计行数
来源：http://jcy.ybcxt.top

wc -l a.txt
来源：http://qjh.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://bte.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fjs.yuanzhike.top

[R54] 比较两个文件
来源：http://sxf.bjfxy.top

diff a.txt b.txt
来源：http://tkw.hywenlv.cn

[R55] 压缩与解压
来源：http://kdq.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vcv.hnqzz.top

[R56] 远程拷贝
来源：http://rzz.chenzaomai.com

scp file user@host:/path/
来源：http://fpb.quarkkingdee.top

[R57] 远程执行命令
来源：http://ruo.jyoumei.cn

ssh user@host 'uptime'
来源：http://npw.hcnkem.com

[R58] 下载文件
来源：http://jxv.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wmo.jinqigfzy.top

[R59] 发 POST JSON
来源：http://bqa.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iic.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://cul.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dbx.yonumen.top

[R61] 磁盘占用
来源：http://mwy.smart0.xyz

df -h;  du -sh *
来源：http://lng.yueranfly.top

[R62] 找最占空间的文件
来源：http://sjo.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://upw.wangshuangyany.cn

[R63] 内存与进程
来源：http://rbm.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://sqv.gaohongyu789.top

[R64] 结束进程
来源：http://lgq.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://goz.yj20258888.top

[R65] 查看端口占用
来源：http://xdf.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cjh.cdnleiting.top

[R66] 定时任务
来源：http://dsk.uphjek.com

crontab -e;  crontab -l
来源：http://shi.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://vqu.guannengcc.top

openssl rand -hex 16
来源：http://dqm.daxiang520.top

[R68] 计算文件校验值
来源：http://teh.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://gur.birdmap.top

[R69] 生成随机密码
来源：http://sky.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://cvu.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://xdy.cashguo.top

date +%s;  date -d @1700000000
来源：http://tcm.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://axh.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ukx.snrcjt.cn

[R72] 等待端口就绪
来源：http://eys.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dje.zycfv.cn

[R73] 分割大日志
来源：http://smq.jqgfzy.top

split -l 1000 big.log part_
来源：http://oxq.jinqigfzy.top

[R74] 批量重命名
来源：http://exb.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://adf.iojbl.cn

[R75] 导出环境变量
来源：http://zux.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://qsd.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://jbj.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://feu.gotoacloud.top

[R77] 读取用户输入
来源：http://edf.316326.xyz

read -rp "请输入: " ans
来源：http://tdj.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://jtt.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ydn.zdbjq.cn

[R79] 解析命令行选项
来源：http://ndf.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bfa.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://svf.ehwqpu.com

time ./run.sh
来源：http://pjk.ctjpmb.com

================================================================================
来源：http://fpk.xinyue.icu

S. C / C++ 专题
来源：http://blm.gogol.net.cn

================================================================================
来源：http://unz.jyoumei.cn

[S01] C：Hello World
来源：http://ial.haohaochexian.top

#include <stdio.h>
来源：http://tzu.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://awr.pycfn.com

[S02] C：变量与格式化输出
来源：http://pdf.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://jyz.tian-w.cn

[S03] C：读入整数
来源：http://muo.bjfxy.top

int x; scanf("%d", &x);
来源：http://mdc.jinqigfzy.top

[S04] C：字符串复制
来源：http://dza.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://wlg.hnxiangtu.top

[S05] C：字符串长度
来源：http://ewx.quarkkingdee.top

strlen(s)
来源：http://lyh.aizwys.cn

[S06] C：字符串比较
来源：http://hsu.hysaishi.cn

strcmp(a, b) == 0
来源：http://ppd.pycfn.com

[S07] C：数组遍历求和
来源：http://wph.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lxw.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://pnk.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jvv.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://vtd.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cae.yuxming.cn

[S10] C：指针与解引用
来源：http://kec.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://kjn.havefunace.top

[S11] C：逐行读文件
来源：http://znq.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://tbg.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hum.ehwqpu.com

fclose(f);
来源：http://wjd.chenlongwang.top

[S12] C：写文件
来源：http://jss.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://irw.chenzaomai.com

[S13] C：宏定义
来源：http://bar.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jyo.vehdjk.com

[S14] C：枚举
来源：http://bhw.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://yau.tian-w.cn

[S15] C：类型转换
来源：http://jno.jinyuanbaomall.cn

(double) a / b
来源：http://dvk.daxiang520.top

[S16] C：位操作置位
来源：http://ssn.tarul.cn

x |= (1 << 3);
来源：http://ohe.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://cbf.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tka.ybcxt.top

[S18] C：命令行参数
来源：http://lsm.sjlbkw.cn

int main(int argc, char **argv)
来源：http://wvz.hammf.cn

[S19] C：快速排序
来源：http://bbd.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mly.wangshuangyany.cn

[S20] C：二分查找
来源：http://nck.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gez.sufxvd.cn

[S21] C：字符类别判断
来源：http://ola.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pvu.0kj1m.cn

[S22] C：字符串转数字
来源：http://hmc.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jqe.shuidangran.top

[S23] C：随机数
来源：http://gmz.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xrv.jlsjyb.cn

[S24] C：获取本地时间
来源：http://isk.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ahq.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://vmh.316326.xyz

memcpy(dst, src, n);
来源：http://fmi.fzhhl.top

[S26] C：内存清零
来源：http://wwp.xylfe.cn

memset(a, 0, sizeof a);
来源：http://rdx.fengsongda.top

[S27] C：定义常量
来源：http://vzp.yangfankeji.com

const double PI = 3.14159;
来源：http://zev.ehwqpu.com

[S28] C：静态变量
来源：http://rht.svipenyu.cn

static int counter = 0;
来源：http://eay.hcnkem.com

[S29] C：变参函数
来源：http://dka.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://siw.quarkkingdee.top

[S30] C：头文件保护
来源：http://dpv.cucudq.cn

#ifndef X_H
来源：http://ofh.hcnkem.com

#define X_H
来源：http://lbp.jyoumei.cn

#endif
来源：http://yxq.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://ian.gotoacloud.top

#include <iostream>
来源：http://gcu.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://poe.iojbl.cn

[S32] C++：字符串
来源：http://hrx.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://ajk.ppjwa.cn

[S33] C++：vector 增删
来源：http://nmy.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mbt.zdqjudy.top

[S34] C++：遍历 vector
来源：http://hzi.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://wbz.vqdsnc.cn

[S35] C++：map
来源：http://lwa.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qwt.c1oappe.top

[S36] C++：unordered_map
来源：http://uby.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yju.zhixingplan.top

[S37] C++：set
来源：http://iyl.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tgi.sufxvd.cn

[S38] C++：排序
来源：http://htg.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://aqw.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://bft.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://avz.yvedp.cn

[S40] C++：查找元素
来源：http://yvf.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bua.jyoumei.cn

[S41] C++：类与构造函数
来源：http://rtw.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://osm.nwbrower.top

[S42] C++：继承与虚函数
来源：http://gbo.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://pzc.yj20258888.top

[S43] C++：智能指针
来源：http://slc.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://edh.jiagoushi.top

[S44] C++：引用传参
来源：http://sap.havefunace.top

void inc(int &x) { ++x; }
来源：http://fnt.zhoulong.xyz

[S45] C++：lambda
来源：http://dhc.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://pbp.wangdashe.top

[S46] C++：函数模板
来源：http://ojg.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jbm.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://dta.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://muy.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://wrg.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://zmq.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://zwr.hysaishi.cn

[S49] C++：写文件
来源：http://ebb.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qsm.hywenlv.cn

[S50] C++：格式化数字
来源：http://zdi.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ynt.52xcode.cn

[S51] C++：显式类型转换
来源：http://zmp.jianghu66.top

static_cast<double>(a) / b
来源：http://kzz.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://cue.316326.xyz

int size() const noexcept { return n_; }
来源：http://vui.zhijiandao.cn

[S53] C++：移动语义
来源：http://oqa.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://lju.wangdashe.top

[S54] C++：异常处理
来源：http://ekb.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jsl.birdmap.top

[S55] C++：结构化绑定
来源：http://aie.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jec.xuanzx.com

[S56] C++：optional
来源：http://sqz.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jwb.vqdsnc.cn

[S57] C++：编译期常量
来源：http://dru.yueranfly.top

constexpr int N = 10;
来源：http://zvy.ybcxt.top

[S58] C++：命名空间
来源：http://eix.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://gxp.jqgufenzy.top

[S59] C++：静态断言
来源：http://jjf.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jsa.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://yfm.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://chf.shangyingyoupin.top

================================================================================
来源：http://soy.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bjj.aibaodan.cn

================================================================================
来源：http://uip.yuxming.cn

[T01] Kotlin：Hello World
来源：http://qae.316326.xyz

println("Hello")
来源：http://jfn.kuanghao11.cn

[T02] Kotlin：变量
来源：http://bsp.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cmy.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://gyy.quarkkingdee.top

"值: $b"
来源：http://eri.cucudq.cn

[T04] Kotlin：空安全
来源：http://uuu.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://ogc.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://wqi.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fcg.sysykeji.top

[T06] Kotlin：集合映射
来源：http://fys.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://evn.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://gwk.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ckc.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://xrg.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://rmx.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://zbi.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://lxa.yj20258.top

[T10] Kotlin：默认参数
来源：http://tgu.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lod.zhixingplan.top

[T11] Kotlin：协程
来源：http://syo.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bzf.xziqi.cn

[T12] Kotlin：解构声明
来源：http://zxw.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://ykc.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://vir.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://cst.jyoumei.cn

[T14] Kotlin：循环
来源：http://ser.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://nou.svipenyu.cn

[T15] Kotlin：接口
来源：http://anp.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://jah.jlsjyb.cn

[T16] Swift：Hello World
来源：http://soo.cdnleiting.top

print("Hello")
来源：http://gca.bjfxy.top

[T17] Swift：变量与常量
来源：http://pcg.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://mep.jiagoushi.top

[T18] Swift：字符串插值
来源：http://kpu.guowangkeji.top

"值: \(b)"
来源：http://bjq.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://lvh.zdbjq.cn

if let n = opt { print(n) }
来源：http://jic.zhixingplan.top

[T20] Swift：数组操作
来源：http://svl.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://sbw.birdmap.top

[T21] Swift：遍历
来源：http://akn.dianchejie.cn

for x in a { print(x) }
来源：http://zdr.shuidangran.top

[T22] Swift：字典
来源：http://knf.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qqf.yueranfly.top

[T23] Swift：函数
来源：http://umk.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dez.hfpthk.cn

[T24] Swift：闭包
来源：http://dem.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ybw.ppjwa.cn

[T25] Swift：结构体
来源：http://pzj.hnxiangtu.top

struct P { var x: Int }
来源：http://okh.fktsv.cn

[T26] Swift：类与重写
来源：http://btn.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://cxs.guowangkeji.top

[T27] Swift：错误处理
来源：http://hqg.xuanzx.com

do { try f() } catch { print(error) }
来源：http://jko.316326.xyz

[T28] Swift：枚举
来源：http://muc.cheryme.top

enum Color { case red, green }
来源：http://amz.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://yls.nanxuanxn.top

guard let x = opt else { return }
来源：http://yno.yonumen.top

[T30] Swift：协议
来源：http://qii.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://fhg.hnqzz.top

[T31] Lua：Hello World
来源：http://zqt.yuxming.cn

print("Hello")
来源：http://zvv.sysykeji.top

[T32] Lua：局部变量
来源：http://srj.jinqigufen.top

local a = 1
来源：http://dzz.ctjpmb.com

[T33] Lua：表（数组）
来源：http://kee.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ygl.yangfankeji.com

[T34] Lua：遍历表
来源：http://bjc.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rea.jqgfzy.top

[T35] Lua：字典表
来源：http://kqm.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://yyr.zhongyouzk.top

[T36] Lua：函数
来源：http://jvp.xylfe.cn

function add(a, b) return a + b end
来源：http://nyc.redwolf501.top

[T37] Lua：字符串拼接
来源：http://iwz.xuanzx.com

"a" .. "b"
来源：http://dgb.cheryme.top

[T38] Lua：条件
来源：http://ztc.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://wnl.xylfe.cn

[T39] Lua：模式匹配
来源：http://ivh.gzhubu.top

string.find(s, "%d+")
来源：http://stb.bbcook.cn

[T40] Lua：元表
来源：http://wtg.tanke756.top

setmetatable({}, { __index = base })
来源：http://zxv.ydjk.org.cn

[T41] Perl：Hello World
来源：http://kpl.shuidangran.top

print "Hello\n";
来源：http://jsk.hysaishi.cn

[T42] Perl：变量类型
来源：http://csk.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://omt.yvedp.cn

[T43] Perl：字符串插值
来源：http://crp.sufxvd.cn

"值: $a"
来源：http://cza.aibaodan.cn

[T44] Perl：条件
来源：http://pew.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://gra.epnwcf.com


<!-- 参考信息 -->