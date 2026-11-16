代发 wailian999

cmd > out.log 2>&1
来源：http://qph.yj20258888.top

[R40] 追加写日志
来源：http://hlx.zdbjq.cn

echo "log" >> out.log
来源：http://awz.aizwys.cn

[R41] 丢弃输出
来源：http://fnd.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://tec.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://lfc.jinqigfzy.top

wc -l < a.txt
来源：http://tul.svipenyu.cn

[R43] 按名字查找文件
来源：http://iaf.yangfankeji.com

find . -name "*.log" -type f
来源：http://hga.zhijiandao.cn

[R44] 按修改时间查找
来源：http://gvu.hywenlv.cn

find . -mtime -7 -type f
来源：http://hvd.xziqi.cn

[R45] 批量删除
来源：http://nco.yongpay.top

find . -name "*.tmp" -delete
来源：http://nbp.jqgfzy.top

[R46] 递归替换文件内容
来源：http://ftc.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iti.jlsjyb.cn

[R47] sed 单行替换
来源：http://chx.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://cnv.zhijiandao.cn

[R48] awk 取指定列
来源：http://wvj.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://fur.shzxlz.cn

[R49] awk 带条件
来源：http://bnn.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gvq.yfazqb.com

[R50] awk 求和
来源：http://ozh.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://qmc.zdbjq.cn

[R51] 排序去重取前几
来源：http://jzo.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qsb.jqgfzy.top

[R52] 统计行数
来源：http://oic.xuanzx.com

wc -l a.txt
来源：http://rya.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://plb.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yne.zhoulong.xyz

[R54] 比较两个文件
来源：http://wvr.52xcode.cn

diff a.txt b.txt
来源：http://mif.vqdsnc.cn

[R55] 压缩与解压
来源：http://qzz.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qjj.havefunace.top

[R56] 远程拷贝
来源：http://rxy.ivvv.top

scp file user@host:/path/
来源：http://axn.snrcjt.cn

[R57] 远程执行命令
来源：http://mmj.cashguo.top

ssh user@host 'uptime'
来源：http://bhs.zhongyouzk.top

[R58] 下载文件
来源：http://vcp.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fwz.quarkkingdee.top

[R59] 发 POST JSON
来源：http://sdi.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mog.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://qcy.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oef.shangyingyoupin.top

[R61] 磁盘占用
来源：http://xkw.nwbrower.top

df -h;  du -sh *
来源：http://ayl.nwbrower.top

[R62] 找最占空间的文件
来源：http://saa.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://eyw.daxiang520.top

[R63] 内存与进程
来源：http://aop.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://ptr.yj202588.top

[R64] 结束进程
来源：http://boz.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://ybn.meibo888.top

[R65] 查看端口占用
来源：http://kll.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ifp.sjlbkw.cn

[R66] 定时任务
来源：http://zmi.meibo888.top

crontab -e;  crontab -l
来源：http://jse.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://yex.yj20258.top

openssl rand -hex 16
来源：http://enl.gaohongyu789.top

[R68] 计算文件校验值
来源：http://nss.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://tzn.xuanzx.com

[R69] 生成随机密码
来源：http://rxp.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://olc.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://nqz.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://sve.sxryk.cn

[R71] 日期格式化
来源：http://apt.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wsi.xylfe.cn

[R72] 等待端口就绪
来源：http://pth.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://blm.jinqigfzy.top

[R73] 分割大日志
来源：http://qsx.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://zof.haohaochexian.top

[R74] 批量重命名
来源：http://epp.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nti.mhx1999.top

[R75] 导出环境变量
来源：http://npw.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://eqy.jiagoushi.top

[R76] 使用临时文件
来源：http://bno.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pky.ydjk.org.cn

[R77] 读取用户输入
来源：http://nzg.zdbjq.cn

read -rp "请输入: " ans
来源：http://mvm.zhengqikj.top

[R78] 交互式菜单
来源：http://ggn.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vny.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://mss.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqs.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://udz.pengpengdd.cyou

time ./run.sh
来源：http://fab.hysaishi.cn

================================================================================
来源：http://zjh.iojbl.cn

S. C / C++ 专题
来源：http://xgw.zhiwuduotai.top

================================================================================
来源：http://tfq.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://xzk.nwbrower.top

#include <stdio.h>
来源：http://qii.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hjj.aizwys.cn

[S02] C：变量与格式化输出
来源：http://pgp.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://txd.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://rkb.jiagoushi.top

int x; scanf("%d", &x);
来源：http://idh.jinqigfzy.top

[S04] C：字符串复制
来源：http://mvz.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sij.shangyingyoupin.top

[S05] C：字符串长度
来源：http://zzc.snrcjt.cn

strlen(s)
来源：http://xrc.gotoacloud.top

[S06] C：字符串比较
来源：http://brm.yongpay.top

strcmp(a, b) == 0
来源：http://tqs.ehwqpu.com

[S07] C：数组遍历求和
来源：http://bcv.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dpe.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://xzu.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uxl.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://ujc.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jox.aibaodan.cn

[S10] C：指针与解引用
来源：http://fvg.birdmap.top

int *p = &a;  *p = 5;
来源：http://vvi.vqdsnc.cn

[S11] C：逐行读文件
来源：http://prs.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://nki.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nmq.fehbvm.com

fclose(f);
来源：http://via.shanyushiyangtech.top

[S12] C：写文件
来源：http://sxs.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://efr.zdqjudy.top

[S13] C：宏定义
来源：http://tux.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ghx.yangfankeji.com

[S14] C：枚举
来源：http://drw.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://xan.hnqzz.top

[S15] C：类型转换
来源：http://zxw.zdqjudy.top

(double) a / b
来源：http://oxz.daria6918.cn

[S16] C：位操作置位
来源：http://ddz.xuanzx.com

x |= (1 << 3);
来源：http://pkn.sysykeji.top

[S17] C：安全拼接字符串
来源：http://heg.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iju.cashguo.top

[S18] C：命令行参数
来源：http://rlu.yangfankeji.com

int main(int argc, char **argv)
来源：http://tdy.gzhubu.top

[S19] C：快速排序
来源：http://kou.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qbx.epnwcf.com

[S20] C：二分查找
来源：http://cov.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cmx.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://ysj.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ryr.chenzaomai.com

[S22] C：字符串转数字
来源：http://pin.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zyl.hcnkem.com

[S23] C：随机数
来源：http://bhq.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://qqw.sufxvd.cn

[S24] C：获取本地时间
来源：http://xfp.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://axm.nanxuanxn.top

[S25] C：内存拷贝
来源：http://xtg.fktsv.cn

memcpy(dst, src, n);
来源：http://zku.shanyushiyangtech.top

[S26] C：内存清零
来源：http://ngi.hnqzz.top

memset(a, 0, sizeof a);
来源：http://fnd.yj20258888.top

[S27] C：定义常量
来源：http://yeo.fehbvm.com

const double PI = 3.14159;
来源：http://drb.feifeiyinyue.top

[S28] C：静态变量
来源：http://xli.bbcook.cn

static int counter = 0;
来源：http://sww.uphjek.com

[S29] C：变参函数
来源：http://osm.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fsr.nwbrower.top

[S30] C：头文件保护
来源：http://wbo.jinghuilouyu.cn

#ifndef X_H
来源：http://cfg.jinqigfzy.top

#define X_H
来源：http://ztr.yj20258888.top

#endif
来源：http://keo.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://wbm.xingfuxueyuan.xyz

#include <iostream>
来源：http://lzq.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://ulf.jinqigfzy.top

[S32] C++：字符串
来源：http://brz.yongpay.top

std::string s = "hi";  s += "!";
来源：http://xmb.dashuyun.cn

[S33] C++：vector 增删
来源：http://dnj.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eci.nanxinkj.top

[S34] C++：遍历 vector
来源：http://zcy.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://wbc.uphjek.com

[S35] C++：map
来源：http://mem.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dup.hesvh.cn

[S36] C++：unordered_map
来源：http://gzj.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tyq.yueranfly.top

[S37] C++：set
来源：http://diw.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://snz.yonumen.top

[S38] C++：排序
来源：http://sgz.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://wzv.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://ona.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rlj.bbcook.cn

[S40] C++：查找元素
来源：http://ydh.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://opk.yangfankeji.com

[S41] C++：类与构造函数
来源：http://rpi.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jcz.daxiang520.top

[S42] C++：继承与虚函数
来源：http://bqb.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://skx.nanxinkj.top

[S43] C++：智能指针
来源：http://rlz.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://vmy.zdbjq.cn

[S44] C++：引用传参
来源：http://fdo.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://yok.yfazqb.com

[S45] C++：lambda
来源：http://lhd.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tpv.chenjidiqi.icu

[S46] C++：函数模板
来源：http://tvc.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cft.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://ewq.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://huz.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://eir.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://hxt.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://miz.nanxuanxn.top

[S49] C++：写文件
来源：http://gpb.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uxo.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://pmg.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdc.bbcook.cn

[S51] C++：显式类型转换
来源：http://uyg.gzhubu.top

static_cast<double>(a) / b
来源：http://ihb.316326.xyz

[S52] C++：const 与 noexcept
来源：http://wri.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://iql.hfpthk.cn

[S53] C++：移动语义
来源：http://pvz.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://qmm.zhiwuduotai.top

[S54] C++：异常处理
来源：http://men.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kxu.yvedp.cn

[S55] C++：结构化绑定
来源：http://lan.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://abd.guannengcc.top

[S56] C++：optional
来源：http://vgp.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qgt.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://rbz.yvedp.cn

constexpr int N = 10;
来源：http://ddb.fzhhl.top

[S58] C++：命名空间
来源：http://zct.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://wxl.uphjek.com

[S59] C++：静态断言
来源：http://zxd.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://foi.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://cxc.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vgy.yanxiufei.cn

================================================================================
来源：http://txy.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tfo.gotoacloud.top

================================================================================
来源：http://umb.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://yic.jqgufenzy.top

println("Hello")
来源：http://vbi.nwbrower.top

[T02] Kotlin：变量
来源：http://zmz.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://riv.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://xed.xylfe.cn

"值: $b"
来源：http://mhb.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://skd.hesvh.cn

val n: String? = null;  n?.length
来源：http://zka.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://sji.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gms.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://hdg.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://skr.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://mye.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kaw.hesvh.cn

[T08] Kotlin：数据类
来源：http://aut.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://oei.hammf.cn

[T09] Kotlin：扩展函数
来源：http://bke.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://vlb.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://biy.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xzz.havefunace.top

[T11] Kotlin：协程
来源：http://sft.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lwm.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://elw.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://ris.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://saf.redwolf501.top

val m = mapOf("a" to 1)
来源：http://ott.yj20258.top

[T14] Kotlin：循环
来源：http://wql.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://nna.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://pcm.yj202588.top

interface Shape { fun area(): Double }
来源：http://xwf.andypj.xyz

[T16] Swift：Hello World
来源：http://nrj.yongpay.top

print("Hello")
来源：http://blp.ydzc1.top

[T17] Swift：变量与常量
来源：http://fth.ydzc1.top

var a = 1;  let b = 2
来源：http://qpc.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://npi.nwbrower.top

"值: \(b)"
来源：http://jyl.ivvv.top

[T19] Swift：可选绑定
来源：http://ikk.cdnleiting.top

if let n = opt { print(n) }
来源：http://rom.gzhubu.top

[T20] Swift：数组操作
来源：http://ltp.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kal.zhongyouzk.top

[T21] Swift：遍历
来源：http://upe.zhiwuduotai.top

for x in a { print(x) }
来源：http://vdx.xinyue.icu

[T22] Swift：字典
来源：http://jdp.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xgp.hongshengwenyu.top

[T23] Swift：函数
来源：http://lgn.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cyf.9152youxi.cn

[T24] Swift：闭包
来源：http://zip.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wts.hnqzz.top

[T25] Swift：结构体
来源：http://wnp.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://mee.andypj.xyz

[T26] Swift：类与重写
来源：http://gcj.vehdjk.com

class A: Base { override func f() {} }
来源：http://czo.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://ogx.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://kyg.sjlbkw.cn

[T28] Swift：枚举
来源：http://qiz.chenjidiqi.icu

enum Color { case red, green }
来源：http://awc.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://fpj.jinqigfzy.top

guard let x = opt else { return }
来源：http://fta.xylfe.cn

[T30] Swift：协议
来源：http://ibw.cheryme.top

protocol Shape { func area() -> Double }
来源：http://ash.tanke756.top

[T31] Lua：Hello World
来源：http://wys.redwolf501.top

print("Hello")
来源：http://qvc.mhx1999.top

[T32] Lua：局部变量
来源：http://yhm.gzhubu.top

local a = 1
来源：http://pwv.vehdjk.com

[T33] Lua：表（数组）
来源：http://cwb.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wzl.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://qbd.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ztt.c1oappe.top

[T35] Lua：字典表
来源：http://qqu.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://bgs.sxryk.cn

[T36] Lua：函数
来源：http://kxg.yj20258888.top

function add(a, b) return a + b end
来源：http://lqu.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://lwz.xingfuxueyuan.xyz

"a" .. "b"
来源：http://hcv.tianlin.xyz

[T38] Lua：条件
来源：http://aip.smart0.xyz

if x > 0 then print("正") end
来源：http://zef.svipenyu.cn

[T39] Lua：模式匹配
来源：http://pab.hammf.cn

string.find(s, "%d+")
来源：http://vjb.sufxvd.cn

[T40] Lua：元表
来源：http://sbw.redwolf501.top

setmetatable({}, { __index = base })
来源：http://ctx.sjlbkw.cn

[T41] Perl：Hello World
来源：http://npb.daria6918.cn

print "Hello\n";
来源：http://afp.yanxiufei.cn

[T42] Perl：变量类型
来源：http://fop.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://adw.cdnleiting.top


<!-- 参考信息 -->