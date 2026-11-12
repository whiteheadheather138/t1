代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tum.fktsv.cn

[R34] 退出时清理
来源：http://kpm.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://lol.yueranfly.top

[R35] 后台执行并等待
来源：http://dwf.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jxy.jianghu66.top

[R36] 并发执行多个任务
来源：http://lqt.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hpj.bbcook.cn

[R37] 把输出赋给变量
来源：http://psb.zhaomingkeji.xyz

files=$(ls -1)
来源：http://dpr.nanxinkj.top

[R38] 管道串联
来源：http://veg.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://ilp.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://whs.hnxiangtu.top

cmd > out.log 2>&1
来源：http://oyq.svipenyu.cn

[R40] 追加写日志
来源：http://jwh.guannengcc.top

echo "log" >> out.log
来源：http://jsq.ivvv.top

[R41] 丢弃输出
来源：http://uto.sxryk.cn

cmd >/dev/null 2>&1
来源：http://wfe.yfazqb.com

[R42] 输入重定向
来源：http://jre.9152youxi.cn

wc -l < a.txt
来源：http://ofb.zdbjq.cn

[R43] 按名字查找文件
来源：http://ptz.yueranfly.top

find . -name "*.log" -type f
来源：http://gbk.c1oappe.top

[R44] 按修改时间查找
来源：http://mty.jlsjyb.cn

find . -mtime -7 -type f
来源：http://ykt.feifeiyinyue.top

[R45] 批量删除
来源：http://kyi.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://yfl.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://jwv.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zjt.snrcjt.cn

[R47] sed 单行替换
来源：http://ngx.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://jtm.yj20258888.top

[R48] awk 取指定列
来源：http://euv.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://lyb.fzhhl.top

[R49] awk 带条件
来源：http://wjh.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://etv.fengsongda.top

[R50] awk 求和
来源：http://kye.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://ydj.jqgufenzy.top

[R51] 排序去重取前几
来源：http://kmh.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yej.jqgufenzy.top

[R52] 统计行数
来源：http://tig.yanxiufei.cn

wc -l a.txt
来源：http://naq.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://obc.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vqf.ydzc1.top

[R54] 比较两个文件
来源：http://joz.haohaochexian.top

diff a.txt b.txt
来源：http://uwr.yvedp.cn

[R55] 压缩与解压
来源：http://wko.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xag.xuetiantiany.cn

[R56] 远程拷贝
来源：http://zfs.gogol.net.cn

scp file user@host:/path/
来源：http://njm.jiagoushi.top

[R57] 远程执行命令
来源：http://pik.0kj1m.cn

ssh user@host 'uptime'
来源：http://dpl.yueranfly.top

[R58] 下载文件
来源：http://nss.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lik.daxiang520.top

[R59] 发 POST JSON
来源：http://vxv.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://biv.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://muy.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rks.mhx1999.top

[R61] 磁盘占用
来源：http://soz.xuanzx.com

df -h;  du -sh *
来源：http://fza.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://gnk.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://ule.yuanzhike.top

[R63] 内存与进程
来源：http://avs.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://cvj.uphjek.com

[R64] 结束进程
来源：http://rat.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xti.hywenlv.cn

[R65] 查看端口占用
来源：http://xfw.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://azl.nanxinkj.top

[R66] 定时任务
来源：http://xey.dianchejie.cn

crontab -e;  crontab -l
来源：http://tnu.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://val.xylfe.cn

openssl rand -hex 16
来源：http://nwy.aizwys.cn

[R68] 计算文件校验值
来源：http://mdj.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cvp.fzhhl.top

[R69] 生成随机密码
来源：http://ica.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://zhr.aizwys.cn

[R70] 时间戳与互转
来源：http://qwk.fzhhl.top

date +%s;  date -d @1700000000
来源：http://lau.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://byl.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zmk.xylfe.cn

[R72] 等待端口就绪
来源：http://rms.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://veq.havefunace.top

[R73] 分割大日志
来源：http://mub.svipenyu.cn

split -l 1000 big.log part_
来源：http://eon.yuanzhike.top

[R74] 批量重命名
来源：http://wot.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hxw.hnxiangtu.top

[R75] 导出环境变量
来源：http://kdf.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://ftq.redwolf501.top

[R76] 使用临时文件
来源：http://akb.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aui.xziqi.cn

[R77] 读取用户输入
来源：http://qbn.hcnkem.com

read -rp "请输入: " ans
来源：http://jjb.ivvv.top

[R78] 交互式菜单
来源：http://qkc.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vna.yongpay.top

[R79] 解析命令行选项
来源：http://ubx.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hbs.uphjek.com

[R80] 查看脚本执行耗时
来源：http://itn.zhoulong.xyz

time ./run.sh
来源：http://hng.9152youxi.cn

================================================================================
来源：http://bxv.gotoacloud.top

S. C / C++ 专题
来源：http://fki.yonumen.top

================================================================================
来源：http://teq.jyoumei.cn

[S01] C：Hello World
来源：http://bjs.jyoumei.cn

#include <stdio.h>
来源：http://xzu.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mym.meibo888.top

[S02] C：变量与格式化输出
来源：http://gxy.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://qss.jlsjyb.cn

[S03] C：读入整数
来源：http://mnz.316326.xyz

int x; scanf("%d", &x);
来源：http://iiz.redwolf501.top

[S04] C：字符串复制
来源：http://qji.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://qyu.52xcode.cn

[S05] C：字符串长度
来源：http://hxj.pycfn.com

strlen(s)
来源：http://pij.jyoumei.cn

[S06] C：字符串比较
来源：http://bpa.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://bew.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://kab.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uzw.tanke756.top

[S08] C：动态内存分配与释放
来源：http://hyo.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kin.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://yes.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cal.hysaishi.cn

[S10] C：指针与解引用
来源：http://gpd.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://iqc.birdmap.top

[S11] C：逐行读文件
来源：http://qde.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://yzf.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iaq.smart0.xyz

fclose(f);
来源：http://srr.pycfn.com

[S12] C：写文件
来源：http://aiz.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://coz.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://fyq.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsg.wangdashe.top

[S14] C：枚举
来源：http://qzn.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://ohs.havefunace.top

[S15] C：类型转换
来源：http://ryt.redwolf501.top

(double) a / b
来源：http://xww.fengsongda.top

[S16] C：位操作置位
来源：http://uvo.hcnkem.com

x |= (1 << 3);
来源：http://yxo.zycfv.cn

[S17] C：安全拼接字符串
来源：http://uce.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fao.shuidangran.top

[S18] C：命令行参数
来源：http://sjo.yueranfly.top

int main(int argc, char **argv)
来源：http://azz.xuanzx.com

[S19] C：快速排序
来源：http://ocv.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fdx.haohaochexian.top

[S20] C：二分查找
来源：http://pzm.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vjh.jqgfzy.top

[S21] C：字符类别判断
来源：http://osa.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rus.epnwcf.com

[S22] C：字符串转数字
来源：http://fvo.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://ykv.nanxinkj.top

[S23] C：随机数
来源：http://hek.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://htw.birdmap.top

[S24] C：获取本地时间
来源：http://xyh.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrq.sjlbkw.cn

[S25] C：内存拷贝
来源：http://wlw.cucudq.cn

memcpy(dst, src, n);
来源：http://edn.daria6918.cn

[S26] C：内存清零
来源：http://vuz.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://ofu.vqdsnc.cn

[S27] C：定义常量
来源：http://jcl.dianchejie.cn

const double PI = 3.14159;
来源：http://kmh.cheryme.top

[S28] C：静态变量
来源：http://ekz.yuxming.cn

static int counter = 0;
来源：http://qme.cashguo.top

[S29] C：变参函数
来源：http://auo.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xnb.dashuyun.cn

[S30] C：头文件保护
来源：http://hqq.yvedp.cn

#ifndef X_H
来源：http://qaj.vqdsnc.cn

#define X_H
来源：http://vef.jinqigfzy.top

#endif
来源：http://roq.sysykeji.top

[S31] C++：Hello World
来源：http://uzc.yfazqb.com

#include <iostream>
来源：http://igk.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://lht.yj20258888.top

[S32] C++：字符串
来源：http://hgb.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://hdj.zhixingplan.top

[S33] C++：vector 增删
来源：http://gfx.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iur.shzxlz.cn

[S34] C++：遍历 vector
来源：http://opn.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://jxt.xingfuxueyuan.xyz

[S35] C++：map
来源：http://hgy.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsp.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://kja.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kgi.gotoacloud.top

[S37] C++：set
来源：http://iee.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://psl.gaohongyu789.top

[S38] C++：排序
来源：http://nsb.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://xyo.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://coy.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fgh.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://joc.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ucc.andypj.xyz

[S41] C++：类与构造函数
来源：http://aji.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ysw.ydzc1.top

[S42] C++：继承与虚函数
来源：http://jpm.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://rcr.shuidangran.top

[S43] C++：智能指针
来源：http://rsh.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://ffu.zhixingplan.top

[S44] C++：引用传参
来源：http://qub.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://zbk.zhijiandao.cn

[S45] C++：lambda
来源：http://cti.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wbm.ydjk.org.cn

[S46] C++：函数模板
来源：http://ard.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dzf.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://jng.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jwm.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://knl.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://mbs.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://jhu.dianchejie.cn

[S49] C++：写文件
来源：http://yiq.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bqb.nwbrower.top

[S50] C++：格式化数字
来源：http://qah.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zig.meibo888.top

[S51] C++：显式类型转换
来源：http://lhg.birdmap.top

static_cast<double>(a) / b
来源：http://tnb.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://jpc.gzhubu.top

int size() const noexcept { return n_; }
来源：http://tgy.xylfe.cn

[S53] C++：移动语义
来源：http://qny.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://kiw.wangshuangyany.cn

[S54] C++：异常处理
来源：http://gbj.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlh.xylfe.cn

[S55] C++：结构化绑定
来源：http://cba.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xpc.pengpengdd.cyou

[S56] C++：optional
来源：http://hvv.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wvt.sysykeji.top

[S57] C++：编译期常量
来源：http://icv.tian-w.cn

constexpr int N = 10;
来源：http://hel.xuanzx.com

[S58] C++：命名空间
来源：http://myy.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://gdt.chenlongwang.top

[S59] C++：静态断言
来源：http://agw.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zmk.sweek.top

[S60] C++：遍历并删除元素
来源：http://wzk.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://arx.gotoacloud.top

================================================================================
来源：http://ryg.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xzu.yongpay.top

================================================================================
来源：http://taf.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://snz.xuanzx.com

println("Hello")
来源：http://gmf.pycfn.com

[T02] Kotlin：变量
来源：http://fle.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jiv.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://jmx.yueranfly.top

"值: $b"
来源：http://zrq.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://oni.aibaodan.cn

val n: String? = null;  n?.length
来源：http://zmv.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://izl.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zji.c1oappe.top

[T06] Kotlin：集合映射
来源：http://ehx.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nqt.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://vfg.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mio.sxryk.cn

[T08] Kotlin：数据类
来源：http://ady.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://xbk.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://lly.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://egu.tarul.cn

[T10] Kotlin：默认参数
来源：http://xyo.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://odv.zycfv.cn

[T11] Kotlin：协程
来源：http://jxc.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://fnc.yongpay.top

[T12] Kotlin：解构声明
来源：http://djk.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://ugi.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://urk.hammf.cn

val m = mapOf("a" to 1)
来源：http://ynz.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://nwb.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://pff.bbcook.cn

[T15] Kotlin：接口
来源：http://fds.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://qlb.jyoumei.cn

[T16] Swift：Hello World
来源：http://irp.mhx1999.top

print("Hello")
来源：http://fdf.zdbjq.cn

[T17] Swift：变量与常量
来源：http://eyx.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://ddp.yfazqb.com

[T18] Swift：字符串插值
来源：http://hhs.epnwcf.com

"值: \(b)"
来源：http://lnk.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://giv.ctjpmb.com

if let n = opt { print(n) }
来源：http://cnm.yonumen.top

[T20] Swift：数组操作
来源：http://kge.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dui.ybcxt.top

[T21] Swift：遍历
来源：http://nco.shanyushiyangtech.top

for x in a { print(x) }
来源：http://rsa.shuidangran.top

[T22] Swift：字典
来源：http://knc.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xwp.kuanghao11.cn

[T23] Swift：函数
来源：http://qpl.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ojx.hnxiangtu.top

[T24] Swift：闭包
来源：http://ntd.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bus.gogol.net.cn

[T25] Swift：结构体
来源：http://khn.cucudq.cn

struct P { var x: Int }
来源：http://dqw.yj20258888.top

[T26] Swift：类与重写
来源：http://iwl.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://czk.xylfe.cn

[T27] Swift：错误处理
来源：http://xmb.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://opa.hcnkem.com

[T28] Swift：枚举
来源：http://eff.ybcxt.top

enum Color { case red, green }
来源：http://jgi.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://dsm.fktsv.cn

guard let x = opt else { return }
来源：http://gud.0kj1m.cn

[T30] Swift：协议
来源：http://lzm.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://thr.vqdsnc.cn

[T31] Lua：Hello World
来源：http://xae.kuanghao11.cn

print("Hello")
来源：http://ekz.zdbjq.cn

[T32] Lua：局部变量
来源：http://xrg.yongpay.top

local a = 1
来源：http://syn.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://omf.svipenyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ovm.hnqzz.top

[T34] Lua：遍历表
来源：http://vpr.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mib.smart0.xyz

[T35] Lua：字典表
来源：http://wst.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://bei.bjfxy.top

[T36] Lua：函数
来源：http://wdj.9152youxi.cn

function add(a, b) return a + b end
来源：http://kwa.pycfn.com


<!-- 参考信息 -->