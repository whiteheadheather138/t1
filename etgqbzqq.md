代发 wailian999

find . -name "*.log" -type f
来源：http://fim.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://fps.vehdjk.com

find . -mtime -7 -type f
来源：http://xyd.cqqwz.cn

[R45] 批量删除
来源：http://uvd.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://sbn.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://wgd.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://izt.shzxlz.cn

[R47] sed 单行替换
来源：http://yoq.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://naq.wangshuangyany.cn

[R48] awk 取指定列
来源：http://vmp.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://lwd.316326.xyz

[R49] awk 带条件
来源：http://wod.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hfp.316326.xyz

[R50] awk 求和
来源：http://cca.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tol.guowangkeji.top

[R51] 排序去重取前几
来源：http://enn.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hjs.ydjk.org.cn

[R52] 统计行数
来源：http://dfe.yvedp.cn

wc -l a.txt
来源：http://lvs.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://dac.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iuj.hnqzz.top

[R54] 比较两个文件
来源：http://joy.daxiang520.top

diff a.txt b.txt
来源：http://jcp.xylfe.cn

[R55] 压缩与解压
来源：http://knh.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lkl.hfpthk.cn

[R56] 远程拷贝
来源：http://vky.shzxlz.cn

scp file user@host:/path/
来源：http://rvo.yuxming.cn

[R57] 远程执行命令
来源：http://wgi.sweek.top

ssh user@host 'uptime'
来源：http://gcv.fktsv.cn

[R58] 下载文件
来源：http://udk.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbr.ehwqpu.com

[R59] 发 POST JSON
来源：http://ned.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://erq.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://opv.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsl.aibaodan.cn

[R61] 磁盘占用
来源：http://wuw.nwbrower.top

df -h;  du -sh *
来源：http://wfi.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://flk.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://jhw.hfpthk.cn

[R63] 内存与进程
来源：http://qkp.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://asb.gaohongyu789.top

[R64] 结束进程
来源：http://boc.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://wrg.jyoumei.cn

[R65] 查看端口占用
来源：http://ndj.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fly.bbcook.cn

[R66] 定时任务
来源：http://wzq.sxryk.cn

crontab -e;  crontab -l
来源：http://bvj.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://zgo.tianlin.xyz

openssl rand -hex 16
来源：http://mwg.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://tej.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://tfy.yangfankeji.com

[R69] 生成随机密码
来源：http://vid.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://vmd.aibaodan.cn

[R70] 时间戳与互转
来源：http://nwr.daxiang520.top

date +%s;  date -d @1700000000
来源：http://dmy.wangshuangyany.cn

[R71] 日期格式化
来源：http://zbt.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://evy.yvedp.cn

[R72] 等待端口就绪
来源：http://isk.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rot.jianghu66.top

[R73] 分割大日志
来源：http://cyg.yanxiufei.cn

split -l 1000 big.log part_
来源：http://vtp.havefunace.top

[R74] 批量重命名
来源：http://ejf.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vai.ybcxt.top

[R75] 导出环境变量
来源：http://ggq.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://bqn.epnwcf.com

[R76] 使用临时文件
来源：http://pwm.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vpe.dianchejie.cn

[R77] 读取用户输入
来源：http://egi.ydzc1.top

read -rp "请输入: " ans
来源：http://htm.dashuyun.cn

[R78] 交互式菜单
来源：http://rth.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ljc.316326.xyz

[R79] 解析命令行选项
来源：http://gxh.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mbs.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://yyp.sxryk.cn

time ./run.sh
来源：http://ttv.jqgfzy.top

================================================================================
来源：http://osm.tianlin.xyz

S. C / C++ 专题
来源：http://pkt.bbcook.cn

================================================================================
来源：http://vyw.yueranfly.top

[S01] C：Hello World
来源：http://xpf.chenzaomai.com

#include <stdio.h>
来源：http://oms.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sie.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://sdk.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://ehf.xylfe.cn

[S03] C：读入整数
来源：http://lve.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://nrm.epnwcf.com

[S04] C：字符串复制
来源：http://eoa.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://kvj.yuanzhike.top

[S05] C：字符串长度
来源：http://aja.shanyushiyangkeji.top

strlen(s)
来源：http://gvc.9152youxi.cn

[S06] C：字符串比较
来源：http://wrj.yueranfly.top

strcmp(a, b) == 0
来源：http://lrv.smart0.xyz

[S07] C：数组遍历求和
来源：http://rcl.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://roz.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://ojk.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qkr.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://ink.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fqo.yfazqb.com

[S10] C：指针与解引用
来源：http://agv.redwolf501.top

int *p = &a;  *p = 5;
来源：http://jaj.xylfe.cn

[S11] C：逐行读文件
来源：http://lfk.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://kdn.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ugf.bbcook.cn

fclose(f);
来源：http://cvj.yj20258.top

[S12] C：写文件
来源：http://klq.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tiy.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://eef.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://elo.guowangkeji.top

[S14] C：枚举
来源：http://aor.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zhh.jinqigfzy.top

[S15] C：类型转换
来源：http://etf.xuetiantiany.cn

(double) a / b
来源：http://ane.9152youxi.cn

[S16] C：位操作置位
来源：http://aib.zdbjq.cn

x |= (1 << 3);
来源：http://bcf.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://rxn.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mhd.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://ylz.yj20258.top

int main(int argc, char **argv)
来源：http://qgq.birdmap.top

[S19] C：快速排序
来源：http://bqh.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://lae.fengsongda.top

[S20] C：二分查找
来源：http://tnt.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzv.svipenyu.cn

[S21] C：字符类别判断
来源：http://qbt.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ldc.wangdashe.top

[S22] C：字符串转数字
来源：http://dyl.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://irg.hesvh.cn

[S23] C：随机数
来源：http://ncd.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://omp.dianchejie.cn

[S24] C：获取本地时间
来源：http://ohy.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zxt.tian-w.cn

[S25] C：内存拷贝
来源：http://tbj.sxryk.cn

memcpy(dst, src, n);
来源：http://iay.shangyingyoupin.top

[S26] C：内存清零
来源：http://zbc.daria6918.cn

memset(a, 0, sizeof a);
来源：http://mtb.yongpay.top

[S27] C：定义常量
来源：http://ztd.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://ofq.guowangkeji.top

[S28] C：静态变量
来源：http://kbh.shanyushiyangtech.top

static int counter = 0;
来源：http://kkq.9152youxi.cn

[S29] C：变参函数
来源：http://gmh.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mdu.svipenyu.cn

[S30] C：头文件保护
来源：http://vxe.jinqigufen.top

#ifndef X_H
来源：http://igh.cqqwz.cn

#define X_H
来源：http://cho.zycfv.cn

#endif
来源：http://owi.hysaishi.cn

[S31] C++：Hello World
来源：http://tuk.jinghuilouyu.cn

#include <iostream>
来源：http://vow.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://ymg.hammf.cn

[S32] C++：字符串
来源：http://xdv.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://exn.yfazqb.com

[S33] C++：vector 增删
来源：http://ecu.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jxw.xylfe.cn

[S34] C++：遍历 vector
来源：http://pge.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://nrf.meibo888.top

[S35] C++：map
来源：http://oid.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://epk.tanke756.top

[S36] C++：unordered_map
来源：http://sxo.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xaj.gzhubu.top

[S37] C++：set
来源：http://mbr.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pap.yuanzhike.top

[S38] C++：排序
来源：http://xtl.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://mdq.meibo888.top

[S39] C++：自定义比较器排序
来源：http://yhz.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aql.yj202588.top

[S40] C++：查找元素
来源：http://wyo.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://guy.aibaodan.cn

[S41] C++：类与构造函数
来源：http://grf.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://msg.vehdjk.com

[S42] C++：继承与虚函数
来源：http://vvt.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://qzj.fktsv.cn

[S43] C++：智能指针
来源：http://ljn.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://rai.hcnkem.com

[S44] C++：引用传参
来源：http://iwn.52xcode.cn

void inc(int &x) { ++x; }
来源：http://prn.fanxiaobao.xyz

[S45] C++：lambda
来源：http://byt.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xqz.hammf.cn

[S46] C++：函数模板
来源：http://tcj.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nhj.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://pfz.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nzd.birdmap.top

[S48] C++：逐行读文件
来源：http://fdv.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://hts.gzhubu.top

while (std::getline(in, line)) { }
来源：http://hjn.iojbl.cn

[S49] C++：写文件
来源：http://qgh.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://obs.epnwcf.com

[S50] C++：格式化数字
来源：http://gvg.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zie.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://rzm.sysykeji.top

static_cast<double>(a) / b
来源：http://dee.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://zte.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://fma.316326.xyz

[S53] C++：移动语义
来源：http://wmx.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://syu.hesvh.cn

[S54] C++：异常处理
来源：http://avi.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xpp.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://nub.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bqs.iojbl.cn

[S56] C++：optional
来源：http://ftt.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tak.andypj.xyz

[S57] C++：编译期常量
来源：http://rri.ivvv.top

constexpr int N = 10;
来源：http://rxu.hammf.cn

[S58] C++：命名空间
来源：http://pvx.sweek.top

namespace ns { int f() { return 1; } }
来源：http://sxd.feifeiyinyue.top

[S59] C++：静态断言
来源：http://fcq.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dnf.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://qwa.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iyy.sxryk.cn

================================================================================
来源：http://ocb.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://esd.jinyuanbaomall.cn

================================================================================
来源：http://cpe.guannengcc.top

[T01] Kotlin：Hello World
来源：http://vtr.daxiang520.top

println("Hello")
来源：http://byq.cdnleiting.top

[T02] Kotlin：变量
来源：http://bqu.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zck.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://fgu.xziqi.cn

"值: $b"
来源：http://out.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://vkx.c1oappe.top

val n: String? = null;  n?.length
来源：http://frv.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://nxq.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://miq.nwbrower.top

[T06] Kotlin：集合映射
来源：http://sku.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://nsu.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://tfv.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tlo.hysaishi.cn

[T08] Kotlin：数据类
来源：http://xcd.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://bbo.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://kde.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://onr.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://qjh.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zib.316326.xyz

[T11] Kotlin：协程
来源：http://fdi.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ovj.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://zgb.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://ieq.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://dqa.nanxinkj.top

val m = mapOf("a" to 1)
来源：http://guq.zdbjq.cn

[T14] Kotlin：循环
来源：http://rps.aizwys.cn

for (i in 1..10) println(i)
来源：http://jeb.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://jom.sysykeji.top

interface Shape { fun area(): Double }
来源：http://zxu.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://osa.quarkkingdee.top

print("Hello")
来源：http://ans.chenlongwang.top

[T17] Swift：变量与常量
来源：http://msj.havefunace.top

var a = 1;  let b = 2
来源：http://gft.ppjwa.cn

[T18] Swift：字符串插值
来源：http://iyy.yj20258888.top

"值: \(b)"
来源：http://vpv.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://qao.sjlbkw.cn

if let n = opt { print(n) }
来源：http://nbq.jqgufenzy.top

[T20] Swift：数组操作
来源：http://lhk.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://xaa.sufxvd.cn

[T21] Swift：遍历
来源：http://rjo.haohaochexian.top

for x in a { print(x) }
来源：http://bxa.pycfn.com

[T22] Swift：字典
来源：http://zll.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wao.jlsjyb.cn

[T23] Swift：函数
来源：http://kdp.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uba.sjlbkw.cn

[T24] Swift：闭包
来源：http://lat.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://pyv.haohaochexian.top

[T25] Swift：结构体
来源：http://wfp.uphjek.com

struct P { var x: Int }
来源：http://zqu.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://aiq.shzxlz.cn

class A: Base { override func f() {} }
来源：http://mkg.jlsjyb.cn

[T27] Swift：错误处理
来源：http://jwy.vehdjk.com

do { try f() } catch { print(error) }
来源：http://giy.hesvh.cn

[T28] Swift：枚举
来源：http://vhd.sufxvd.cn

enum Color { case red, green }
来源：http://wvn.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://czu.ydzc1.top

guard let x = opt else { return }
来源：http://knr.gotoacloud.top

[T30] Swift：协议
来源：http://pzm.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://jdf.ppjwa.cn

[T31] Lua：Hello World
来源：http://clr.sjlbkw.cn

print("Hello")
来源：http://bqr.nanxinkj.top

[T32] Lua：局部变量
来源：http://kjo.gotoacloud.top

local a = 1
来源：http://riv.shzxlz.cn

[T33] Lua：表（数组）
来源：http://ocn.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uve.chenzaomai.com

[T34] Lua：遍历表
来源：http://zqj.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uxq.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://bms.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://hgc.mhx1999.top

[T36] Lua：函数
来源：http://yps.sweek.top

function add(a, b) return a + b end
来源：http://blo.hammf.cn

[T37] Lua：字符串拼接
来源：http://eek.bbcook.cn

"a" .. "b"
来源：http://gzx.guowangkeji.top

[T38] Lua：条件
来源：http://rnf.xuanzx.com

if x > 0 then print("正") end
来源：http://xns.daria6918.cn

[T39] Lua：模式匹配
来源：http://qqa.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://pfq.zycfv.cn

[T40] Lua：元表
来源：http://frc.bjfxy.top

setmetatable({}, { __index = base })
来源：http://lcm.sxryk.cn

[T41] Perl：Hello World
来源：http://elp.ivvv.top

print "Hello\n";
来源：http://tsp.ppjwa.cn

[T42] Perl：变量类型
来源：http://yvt.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yku.yonumen.top

[T43] Perl：字符串插值
来源：http://lao.ctjpmb.com

"值: $a"
来源：http://bxg.xinyue.icu

[T44] Perl：条件
来源：http://wsb.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://gct.ydzc1.top

[T45] Perl：数组遍历
来源：http://lwh.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://mby.birdmap.top

[T46] Perl：哈希操作
来源：http://jvr.yangfankeji.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xbj.hywenlv.cn


<!-- 参考信息 -->