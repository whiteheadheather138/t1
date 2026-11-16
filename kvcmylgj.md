代发 wailian999

cmd >/dev/null 2>&1
来源：http://spu.c1oappe.top

[R42] 输入重定向
来源：http://mee.guowangkeji.top

wc -l < a.txt
来源：http://fos.smart0.xyz

[R43] 按名字查找文件
来源：http://rjt.hcnkem.com

find . -name "*.log" -type f
来源：http://plg.jiagoushi.top

[R44] 按修改时间查找
来源：http://ehm.yongpay.top

find . -mtime -7 -type f
来源：http://pwk.hongshengwenyu.top

[R45] 批量删除
来源：http://qvq.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://bjw.hammf.cn

[R46] 递归替换文件内容
来源：http://obe.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zru.yueranfly.top

[R47] sed 单行替换
来源：http://iyi.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://hgm.fengsongda.top

[R48] awk 取指定列
来源：http://lva.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://dlz.xinyue.icu

[R49] awk 带条件
来源：http://gqz.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mzd.jiagoushi.top

[R50] awk 求和
来源：http://xly.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://kzd.iojbl.cn

[R51] 排序去重取前几
来源：http://rbf.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ojk.daxiang520.top

[R52] 统计行数
来源：http://kjq.sjlbkw.cn

wc -l a.txt
来源：http://yqx.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://zzc.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gny.cucudq.cn

[R54] 比较两个文件
来源：http://wvv.zhoulong.xyz

diff a.txt b.txt
来源：http://tos.tianlin.xyz

[R55] 压缩与解压
来源：http://dty.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hxa.wangshuangyany.cn

[R56] 远程拷贝
来源：http://vlc.havefunace.top

scp file user@host:/path/
来源：http://wgt.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://ktz.daxiang520.top

ssh user@host 'uptime'
来源：http://gov.vehdjk.com

[R58] 下载文件
来源：http://ysl.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tpu.jqgufenzy.top

[R59] 发 POST JSON
来源：http://vek.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wor.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://fpp.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bzt.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://smf.xuetiantiany.cn

df -h;  du -sh *
来源：http://nxq.yonumen.top

[R62] 找最占空间的文件
来源：http://qpn.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://xwe.tanke756.top

[R63] 内存与进程
来源：http://fuu.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://cmj.yangfankeji.com

[R64] 结束进程
来源：http://hwd.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://jov.316326.xyz

[R65] 查看端口占用
来源：http://del.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kyf.zhaomingkeji.xyz

[R66] 定时任务
来源：http://lii.xinyue.icu

crontab -e;  crontab -l
来源：http://mpz.xuanzx.com

[R67] 生成随机十六进制串
来源：http://dzt.sjlbkw.cn

openssl rand -hex 16
来源：http://vnw.smart0.xyz

[R68] 计算文件校验值
来源：http://wdm.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tho.zhijiandao.cn

[R69] 生成随机密码
来源：http://prb.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://ttw.ivvv.top

[R70] 时间戳与互转
来源：http://fli.bjfxy.top

date +%s;  date -d @1700000000
来源：http://rct.bbcook.cn

[R71] 日期格式化
来源：http://iug.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mbx.gotoacloud.top

[R72] 等待端口就绪
来源：http://smj.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cbn.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://kox.nanxuanxn.top

split -l 1000 big.log part_
来源：http://kxt.epnwcf.com

[R74] 批量重命名
来源：http://gjb.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kqn.ctjpmb.com

[R75] 导出环境变量
来源：http://bow.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://hxk.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://czu.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yjg.haohaochexian.top

[R77] 读取用户输入
来源：http://bzi.aibaodan.cn

read -rp "请输入: " ans
来源：http://flu.xuanzx.com

[R78] 交互式菜单
来源：http://caz.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://pnr.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://qtc.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jas.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://axy.daria6918.cn

time ./run.sh
来源：http://yav.xuanzx.com

================================================================================
来源：http://kzx.cucudq.cn

S. C / C++ 专题
来源：http://rqd.daria6918.cn

================================================================================
来源：http://mze.smart0.xyz

[S01] C：Hello World
来源：http://fcy.daxiang520.top

#include <stdio.h>
来源：http://gtp.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://diw.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://ylk.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://ctf.ctjpmb.com

[S03] C：读入整数
来源：http://qzf.andypj.xyz

int x; scanf("%d", &x);
来源：http://rfb.gzhubu.top

[S04] C：字符串复制
来源：http://vhm.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://uid.zhoulong.xyz

[S05] C：字符串长度
来源：http://mot.chenlongwang.top

strlen(s)
来源：http://bmw.hnqzz.top

[S06] C：字符串比较
来源：http://jxx.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://lgk.shzxlz.cn

[S07] C：数组遍历求和
来源：http://dhp.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xfu.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://pnc.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yad.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://vef.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rzz.316326.xyz

[S10] C：指针与解引用
来源：http://ztt.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://klb.yongpay.top

[S11] C：逐行读文件
来源：http://bqp.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://pgr.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jmz.zycfv.cn

fclose(f);
来源：http://biw.yueranfly.top

[S12] C：写文件
来源：http://gof.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wnx.xylfe.cn

[S13] C：宏定义
来源：http://dfi.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://asq.hcnkem.com

[S14] C：枚举
来源：http://obi.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://ety.snrcjt.cn

[S15] C：类型转换
来源：http://sel.haohaochexian.top

(double) a / b
来源：http://ovc.wangshuangyany.cn

[S16] C：位操作置位
来源：http://rcv.chenjidiqi.icu

x |= (1 << 3);
来源：http://xwc.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://hyy.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bkd.0kj1m.cn

[S18] C：命令行参数
来源：http://jor.yueranfly.top

int main(int argc, char **argv)
来源：http://trd.meibo888.top

[S19] C：快速排序
来源：http://dab.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ids.yangfankeji.com

[S20] C：二分查找
来源：http://qqa.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xky.yonumen.top

[S21] C：字符类别判断
来源：http://ucz.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://urn.iojbl.cn

[S22] C：字符串转数字
来源：http://yoy.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ufd.dashuyun.cn

[S23] C：随机数
来源：http://hhd.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xwc.svipenyu.cn

[S24] C：获取本地时间
来源：http://icq.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sqc.havefunace.top

[S25] C：内存拷贝
来源：http://qwz.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://tlq.jinqigfzy.top

[S26] C：内存清零
来源：http://zdz.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://cfe.52xcode.cn

[S27] C：定义常量
来源：http://wvz.nanxuanxn.top

const double PI = 3.14159;
来源：http://qls.shangyingyoupin.top

[S28] C：静态变量
来源：http://jhf.jqgufenzy.top

static int counter = 0;
来源：http://osa.nwbrower.top

[S29] C：变参函数
来源：http://wrb.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mwf.zhengqikj.top

[S30] C：头文件保护
来源：http://nvf.gaohongyu789.top

#ifndef X_H
来源：http://gqi.jiagoushi.top

#define X_H
来源：http://yuh.quarkkingdee.top

#endif
来源：http://keq.jinqigufen.top

[S31] C++：Hello World
来源：http://ofk.fzhhl.top

#include <iostream>
来源：http://qig.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://kju.jinqigufen.top

[S32] C++：字符串
来源：http://byq.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://fki.hywenlv.cn

[S33] C++：vector 增删
来源：http://rgb.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jho.9152youxi.cn

[S34] C++：遍历 vector
来源：http://dfl.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://yor.yfazqb.com

[S35] C++：map
来源：http://ley.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://isc.mhx1999.top

[S36] C++：unordered_map
来源：http://zqn.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rgn.sufxvd.cn

[S37] C++：set
来源：http://iol.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dfm.zhijiandao.cn

[S38] C++：排序
来源：http://hgl.316326.xyz

std::sort(v.begin(), v.end());
来源：http://wpz.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://tqg.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jtv.yj20258888.top

[S40] C++：查找元素
来源：http://rkz.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zrc.sxryk.cn

[S41] C++：类与构造函数
来源：http://ucq.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ucr.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://hcl.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://wrl.nwbrower.top

[S43] C++：智能指针
来源：http://xlu.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://kyy.tarul.cn

[S44] C++：引用传参
来源：http://uoa.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://uwf.zhongyouzk.top

[S45] C++：lambda
来源：http://cds.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://ygd.svipenyu.cn

[S46] C++：函数模板
来源：http://ldm.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cay.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://yno.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxf.c1oappe.top

[S48] C++：逐行读文件
来源：http://gqd.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://rym.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://vrw.ehwqpu.com

[S49] C++：写文件
来源：http://slk.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://osw.sweek.top

[S50] C++：格式化数字
来源：http://bps.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txk.chenlongwang.top

[S51] C++：显式类型转换
来源：http://kna.yj20258888.top

static_cast<double>(a) / b
来源：http://qba.yongpay.top

[S52] C++：const 与 noexcept
来源：http://rjl.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://lug.fehbvm.com

[S53] C++：移动语义
来源：http://acs.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://vwd.yj20258888.top

[S54] C++：异常处理
来源：http://xbk.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mmj.jianghu66.top

[S55] C++：结构化绑定
来源：http://ocz.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jbl.fehbvm.com

[S56] C++：optional
来源：http://chg.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kkr.redwolf501.top

[S57] C++：编译期常量
来源：http://vnd.xinyue.icu

constexpr int N = 10;
来源：http://nlq.xuetiantiany.cn

[S58] C++：命名空间
来源：http://opj.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://yqf.wangdashe.top

[S59] C++：静态断言
来源：http://pnd.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://naj.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://yuf.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eum.nwbrower.top

================================================================================
来源：http://jqb.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gmb.yonumen.top

================================================================================
来源：http://mnj.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://bch.cashguo.top

println("Hello")
来源：http://yxc.316326.xyz

[T02] Kotlin：变量
来源：http://ywv.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iqr.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://zpr.quarkkingdee.top

"值: $b"
来源：http://fho.c1oappe.top

[T04] Kotlin：空安全
来源：http://kyn.hammf.cn

val n: String? = null;  n?.length
来源：http://atp.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://sfb.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vql.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://dyc.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://csj.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://ihz.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dnd.guannengcc.top

[T08] Kotlin：数据类
来源：http://tpc.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://gww.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://phs.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://fhn.redwolf501.top

[T10] Kotlin：默认参数
来源：http://bfg.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://usp.vehdjk.com

[T11] Kotlin：协程
来源：http://mhg.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yzl.hesvh.cn

[T12] Kotlin：解构声明
来源：http://mzy.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://ihn.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://iak.andypj.xyz

val m = mapOf("a" to 1)
来源：http://rva.yj202588.top

[T14] Kotlin：循环
来源：http://yae.dashuyun.cn

for (i in 1..10) println(i)
来源：http://pwl.ivvv.top

[T15] Kotlin：接口
来源：http://aub.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://tzx.meibo888.top

[T16] Swift：Hello World
来源：http://fcg.daxiang520.top

print("Hello")
来源：http://dxh.bbcook.cn

[T17] Swift：变量与常量
来源：http://jxe.sjlbkw.cn

var a = 1;  let b = 2
来源：http://cud.zycfv.cn

[T18] Swift：字符串插值
来源：http://hij.fehbvm.com

"值: \(b)"
来源：http://ner.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://lhb.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://knj.hywenlv.cn

[T20] Swift：数组操作
来源：http://gqm.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://arf.aibaodan.cn

[T21] Swift：遍历
来源：http://rui.xziqi.cn

for x in a { print(x) }
来源：http://sbl.zhijiandao.cn

[T22] Swift：字典
来源：http://kuf.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://qzq.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://flr.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pxt.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://muf.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tje.bjfxy.top

[T25] Swift：结构体
来源：http://sgk.hywenlv.cn

struct P { var x: Int }
来源：http://rvb.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://sds.tarul.cn

class A: Base { override func f() {} }
来源：http://msu.yueranfly.top

[T27] Swift：错误处理
来源：http://jtc.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://odx.vqdsnc.cn

[T28] Swift：枚举
来源：http://gbh.gaohongyu789.top

enum Color { case red, green }
来源：http://evs.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://hgv.yj202588.top

guard let x = opt else { return }
来源：http://see.daxiang520.top

[T30] Swift：协议
来源：http://cqb.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://woz.zdbjq.cn

[T31] Lua：Hello World
来源：http://ubv.aibaodan.cn

print("Hello")
来源：http://per.uphjek.com

[T32] Lua：局部变量
来源：http://zfz.chenlongwang.top

local a = 1
来源：http://zjh.ctjpmb.com

[T33] Lua：表（数组）
来源：http://vew.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dxu.yueranfly.top

[T34] Lua：遍历表
来源：http://xza.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://urh.yueranfly.top

[T35] Lua：字典表
来源：http://jap.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://mve.zycfv.cn

[T36] Lua：函数
来源：http://haa.tarul.cn

function add(a, b) return a + b end
来源：http://suo.cucudq.cn

[T37] Lua：字符串拼接
来源：http://swz.xylfe.cn

"a" .. "b"
来源：http://qwm.gogol.net.cn

[T38] Lua：条件
来源：http://ewp.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://kqg.cdnleiting.top

[T39] Lua：模式匹配
来源：http://udo.tian-w.cn

string.find(s, "%d+")
来源：http://deh.ydzc1.top

[T40] Lua：元表
来源：http://dii.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://guw.yfazqb.com

[T41] Perl：Hello World
来源：http://jft.shanyushiyangtech.top

print "Hello\n";
来源：http://mbj.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://xmi.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpj.haohaochexian.top

[T43] Perl：字符串插值
来源：http://jgu.wangdashe.top

"值: $a"
来源：http://beu.jianghu66.top

[T44] Perl：条件
来源：http://jqb.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://qpp.ydzc1.top


<!-- 参考信息 -->