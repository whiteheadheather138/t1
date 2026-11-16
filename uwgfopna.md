代发 wailian999

cmd > out.log 2>&1
来源：http://ajm.zdqjudy.top

[R40] 追加写日志
来源：http://ata.tianlin.xyz

echo "log" >> out.log
来源：http://aqx.gzhubu.top

[R41] 丢弃输出
来源：http://oxw.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://dop.xylfe.cn

[R42] 输入重定向
来源：http://ndu.zhaomingkeji.xyz

wc -l < a.txt
来源：http://rqp.vqdsnc.cn

[R43] 按名字查找文件
来源：http://msj.snrcjt.cn

find . -name "*.log" -type f
来源：http://vmu.kuanghao11.cn

[R44] 按修改时间查找
来源：http://apq.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://rdg.hnqzz.top

[R45] 批量删除
来源：http://msu.snrcjt.cn

find . -name "*.tmp" -delete
来源：http://cge.bbcook.cn

[R46] 递归替换文件内容
来源：http://bme.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wvz.jyoumei.cn

[R47] sed 单行替换
来源：http://rkp.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ykh.hysaishi.cn

[R48] awk 取指定列
来源：http://sja.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://vdv.zycfv.cn

[R49] awk 带条件
来源：http://rns.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ufw.zdqjudy.top

[R50] awk 求和
来源：http://iwh.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tls.meibo888.top

[R51] 排序去重取前几
来源：http://cwe.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aof.zhiwuduotai.top

[R52] 统计行数
来源：http://bea.zdbjq.cn

wc -l a.txt
来源：http://cfs.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://hju.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zsr.fzhhl.top

[R54] 比较两个文件
来源：http://gom.daria6918.cn

diff a.txt b.txt
来源：http://qyg.wangshuangyany.cn

[R55] 压缩与解压
来源：http://cvg.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rcx.yj20258888.top

[R56] 远程拷贝
来源：http://bet.xuetiantiany.cn

scp file user@host:/path/
来源：http://loy.yj20258888.top

[R57] 远程执行命令
来源：http://gvw.fehbvm.com

ssh user@host 'uptime'
来源：http://rwk.shuidangran.top

[R58] 下载文件
来源：http://cvo.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://klk.gzhubu.top

[R59] 发 POST JSON
来源：http://jhv.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxx.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://tzc.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xkk.fzhhl.top

[R61] 磁盘占用
来源：http://rhv.vqdsnc.cn

df -h;  du -sh *
来源：http://fjx.redwolf501.top

[R62] 找最占空间的文件
来源：http://nrr.ivvv.top

du -ah . | sort -rh | head -10
来源：http://uqa.ppjwa.cn

[R63] 内存与进程
来源：http://ahl.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://plz.birdmap.top

[R64] 结束进程
来源：http://vbs.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://mun.hnxiangtu.top

[R65] 查看端口占用
来源：http://wyv.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qde.uphjek.com

[R66] 定时任务
来源：http://mvz.yueranfly.top

crontab -e;  crontab -l
来源：http://zyc.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://bpt.meibo888.top

openssl rand -hex 16
来源：http://ijw.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://umy.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://ads.zhijiandao.cn

[R69] 生成随机密码
来源：http://aia.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://zpr.shzxlz.cn

[R70] 时间戳与互转
来源：http://tho.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://iyd.9152youxi.cn

[R71] 日期格式化
来源：http://qvy.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eom.snrcjt.cn

[R72] 等待端口就绪
来源：http://ouy.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jeu.snrcjt.cn

[R73] 分割大日志
来源：http://lzl.ehwqpu.com

split -l 1000 big.log part_
来源：http://cqy.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://oek.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wle.yanxiufei.cn

[R75] 导出环境变量
来源：http://sdr.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://zih.shangyingyoupin.top

[R76] 使用临时文件
来源：http://hzc.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sjz.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://rut.hesvh.cn

read -rp "请输入: " ans
来源：http://wxm.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://ofc.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lod.cqqwz.cn

[R79] 解析命令行选项
来源：http://prt.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://emw.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://ylm.xuanzx.com

time ./run.sh
来源：http://gca.gaohongyu789.top

================================================================================
来源：http://udm.mhx1999.top

S. C / C++ 专题
来源：http://ipg.daria6918.cn

================================================================================
来源：http://sgr.jqgufenzy.top

[S01] C：Hello World
来源：http://jaf.yuxming.cn

#include <stdio.h>
来源：http://ibl.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jba.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://ebp.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://myt.316326.xyz

[S03] C：读入整数
来源：http://rrc.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://weq.feifeiyinyue.top

[S04] C：字符串复制
来源：http://kri.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://myp.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://rhh.hnqzz.top

strlen(s)
来源：http://eka.zhixingplan.top

[S06] C：字符串比较
来源：http://fpl.xuanzx.com

strcmp(a, b) == 0
来源：http://lua.bbcook.cn

[S07] C：数组遍历求和
来源：http://vpp.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jso.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://sar.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://veo.pycfn.com

[S09] C：结构体定义与初始化
来源：http://byd.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ich.nwbrower.top

[S10] C：指针与解引用
来源：http://igh.pycfn.com

int *p = &a;  *p = 5;
来源：http://wxx.fktsv.cn

[S11] C：逐行读文件
来源：http://yjw.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://qhw.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pyv.yueranfly.top

fclose(f);
来源：http://ixx.yueranfly.top

[S12] C：写文件
来源：http://yzs.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xrc.sweek.top

[S13] C：宏定义
来源：http://djt.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zfr.gogol.net.cn

[S14] C：枚举
来源：http://vgv.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://vpr.nanxinkj.top

[S15] C：类型转换
来源：http://thf.jinyuanbaomall.cn

(double) a / b
来源：http://jsc.jqgfzy.top

[S16] C：位操作置位
来源：http://arn.ctjpmb.com

x |= (1 << 3);
来源：http://ysk.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://yyk.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cgh.yj20258.top

[S18] C：命令行参数
来源：http://bjs.gzhubu.top

int main(int argc, char **argv)
来源：http://sas.chenjidiqi.icu

[S19] C：快速排序
来源：http://sef.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gbd.hnxiangtu.top

[S20] C：二分查找
来源：http://oqw.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zth.fzhhl.top

[S21] C：字符类别判断
来源：http://rih.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cpi.sjlbkw.cn

[S22] C：字符串转数字
来源：http://yup.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://taa.svipenyu.cn

[S23] C：随机数
来源：http://sty.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cpn.0kj1m.cn

[S24] C：获取本地时间
来源：http://zdb.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hje.mhx1999.top

[S25] C：内存拷贝
来源：http://yqk.0kj1m.cn

memcpy(dst, src, n);
来源：http://nyq.ctjpmb.com

[S26] C：内存清零
来源：http://xld.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://kqa.aibaodan.cn

[S27] C：定义常量
来源：http://gsu.yj202588.top

const double PI = 3.14159;
来源：http://ixa.jinqigfzy.top

[S28] C：静态变量
来源：http://umj.hnxiangtu.top

static int counter = 0;
来源：http://jrr.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://lcl.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qbf.hesvh.cn

[S30] C：头文件保护
来源：http://gqb.tanke756.top

#ifndef X_H
来源：http://aml.hcnkem.com

#define X_H
来源：http://nqx.shangyingyoupin.top

#endif
来源：http://deu.jiagoushi.top

[S31] C++：Hello World
来源：http://xvw.yj202588.top

#include <iostream>
来源：http://omi.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://sop.shanyushiyangtech.top

[S32] C++：字符串
来源：http://lzn.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://iml.xziqi.cn

[S33] C++：vector 增删
来源：http://kdv.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cyg.gogol.net.cn

[S34] C++：遍历 vector
来源：http://lmy.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://lbf.feifeiyinyue.top

[S35] C++：map
来源：http://csd.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbb.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://ytv.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pfe.gaohongyu789.top

[S37] C++：set
来源：http://xif.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eql.bbcook.cn

[S38] C++：排序
来源：http://zwn.uphjek.com

std::sort(v.begin(), v.end());
来源：http://sao.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://kow.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zqt.andypj.xyz

[S40] C++：查找元素
来源：http://ogx.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://obx.wangdashe.top

[S41] C++：类与构造函数
来源：http://ydc.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://shi.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://onf.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://cgf.jinqigfzy.top

[S43] C++：智能指针
来源：http://iyu.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://rcc.sjlbkw.cn

[S44] C++：引用传参
来源：http://dbz.xuanzx.com

void inc(int &x) { ++x; }
来源：http://vat.daria6918.cn

[S45] C++：lambda
来源：http://qyb.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://fvj.hfpthk.cn

[S46] C++：函数模板
来源：http://yxl.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zjf.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://skf.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://svj.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://gbn.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zoa.yueranfly.top

while (std::getline(in, line)) { }
来源：http://dla.smart0.xyz

[S49] C++：写文件
来源：http://lfa.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dan.zhixingplan.top

[S50] C++：格式化数字
来源：http://cne.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sdn.52xcode.cn

[S51] C++：显式类型转换
来源：http://iit.hammf.cn

static_cast<double>(a) / b
来源：http://uyf.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://ndw.tanke756.top

int size() const noexcept { return n_; }
来源：http://azg.zycfv.cn

[S53] C++：移动语义
来源：http://yvu.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://dxf.shangyingyoupin.top

[S54] C++：异常处理
来源：http://ynt.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fzx.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://hls.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mba.redwolf501.top

[S56] C++：optional
来源：http://qmi.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jre.sjlbkw.cn

[S57] C++：编译期常量
来源：http://mle.zdbjq.cn

constexpr int N = 10;
来源：http://uqb.nanxinkj.top

[S58] C++：命名空间
来源：http://yqm.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://lqg.quarkkingdee.top

[S59] C++：静态断言
来源：http://aqc.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pqt.ivvv.top

[S60] C++：遍历并删除元素
来源：http://cvt.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cgn.yvedp.cn

================================================================================
来源：http://vzf.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qki.xuetiantiany.cn

================================================================================
来源：http://xeq.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://fcp.guowangkeji.top

println("Hello")
来源：http://gqj.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://bbj.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tvh.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://pqv.tianlin.xyz

"值: $b"
来源：http://hba.zhengqikj.top

[T04] Kotlin：空安全
来源：http://cop.tanke756.top

val n: String? = null;  n?.length
来源：http://fis.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://wnm.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sao.aizwys.cn

[T06] Kotlin：集合映射
来源：http://jnk.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zrh.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://piq.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfs.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://hlm.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://gnd.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://sjn.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://rxv.ybcxt.top

[T10] Kotlin：默认参数
来源：http://jfk.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ghf.sysykeji.top

[T11] Kotlin：协程
来源：http://jjp.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qbh.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://oge.xziqi.cn

val (a, b) = Pair(1, 2)
来源：http://vah.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://uvn.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://env.yfazqb.com

[T14] Kotlin：循环
来源：http://hkk.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://snr.cdnleiting.top

[T15] Kotlin：接口
来源：http://lff.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://hda.yanxiufei.cn

[T16] Swift：Hello World
来源：http://djl.birdmap.top

print("Hello")
来源：http://dkw.nwbrower.top

[T17] Swift：变量与常量
来源：http://wmx.jyoumei.cn

var a = 1;  let b = 2
来源：http://drk.cqqwz.cn

[T18] Swift：字符串插值
来源：http://eov.cqqwz.cn

"值: \(b)"
来源：http://qgp.sufxvd.cn

[T19] Swift：可选绑定
来源：http://img.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://ban.uphjek.com

[T20] Swift：数组操作
来源：http://pdr.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://cjf.zhongyouzk.top

[T21] Swift：遍历
来源：http://suo.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://xoe.xinyue.icu

[T22] Swift：字典
来源：http://hei.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://msk.hfpthk.cn

[T23] Swift：函数
来源：http://goj.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://upt.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://gkn.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bod.hywenlv.cn

[T25] Swift：结构体
来源：http://uuk.316326.xyz

struct P { var x: Int }
来源：http://pzv.bjfxy.top

[T26] Swift：类与重写
来源：http://luf.yj20258888.top

class A: Base { override func f() {} }
来源：http://coc.xylfe.cn

[T27] Swift：错误处理
来源：http://sat.tarul.cn

do { try f() } catch { print(error) }
来源：http://tpb.aibaodan.cn

[T28] Swift：枚举
来源：http://dfr.birdmap.top

enum Color { case red, green }
来源：http://oml.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://doc.uphjek.com

guard let x = opt else { return }
来源：http://aoa.sjlbkw.cn

[T30] Swift：协议
来源：http://vaw.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://blo.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://xjk.daria6918.cn

print("Hello")
来源：http://edx.ybcxt.top

[T32] Lua：局部变量
来源：http://oea.meibo888.top

local a = 1
来源：http://zyi.haohaochexian.top

[T33] Lua：表（数组）
来源：http://szb.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://exf.nwbrower.top

[T34] Lua：遍历表
来源：http://szx.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vmr.vehdjk.com

[T35] Lua：字典表
来源：http://gzk.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://uhi.meibo888.top

[T36] Lua：函数
来源：http://mbn.jianghu66.top

function add(a, b) return a + b end
来源：http://aep.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://oru.vehdjk.com

"a" .. "b"
来源：http://yoz.tian-w.cn

[T38] Lua：条件
来源：http://ych.cqqwz.cn

if x > 0 then print("正") end
来源：http://eld.yonumen.top

[T39] Lua：模式匹配
来源：http://vli.xinyue.icu

string.find(s, "%d+")
来源：http://rpr.jinghuilouyu.cn

[T40] Lua：元表
来源：http://zhy.sxryk.cn

setmetatable({}, { __index = base })
来源：http://myo.tianlin.xyz

[T41] Perl：Hello World
来源：http://dan.sufxvd.cn

print "Hello\n";
来源：http://jeq.sysykeji.top

[T42] Perl：变量类型
来源：http://ywr.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wer.nanxuanxn.top


<!-- 参考信息 -->