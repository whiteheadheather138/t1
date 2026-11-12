代发 wailian999

cmd >/dev/null 2>&1
来源：http://ghw.chenzaomai.com

[R42] 输入重定向
来源：http://ugi.sxryk.cn

wc -l < a.txt
来源：http://xmj.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://tvp.sweek.top

find . -name "*.log" -type f
来源：http://qxp.zdqjudy.top

[R44] 按修改时间查找
来源：http://tzl.svipenyu.cn

find . -mtime -7 -type f
来源：http://fuh.uphjek.com

[R45] 批量删除
来源：http://ilf.daxiang520.top

find . -name "*.tmp" -delete
来源：http://uac.redwolf501.top

[R46] 递归替换文件内容
来源：http://sby.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pus.chenlongwang.top

[R47] sed 单行替换
来源：http://anx.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://tup.yuanzhike.top

[R48] awk 取指定列
来源：http://omf.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ymz.guowangkeji.top

[R49] awk 带条件
来源：http://hwa.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cxc.gzhubu.top

[R50] awk 求和
来源：http://thf.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://egm.guowangkeji.top

[R51] 排序去重取前几
来源：http://gzn.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ohv.meibo888.top

[R52] 统计行数
来源：http://yzz.jlsjyb.cn

wc -l a.txt
来源：http://jui.yj202588.top

[R53] 查看文件头与实时尾
来源：http://gkf.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tmy.kuanghao11.cn

[R54] 比较两个文件
来源：http://dcw.ppjwa.cn

diff a.txt b.txt
来源：http://wed.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://mtj.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lxq.chenlongwang.top

[R56] 远程拷贝
来源：http://zmf.smart0.xyz

scp file user@host:/path/
来源：http://uuc.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://qsq.aibaodan.cn

ssh user@host 'uptime'
来源：http://aof.xylfe.cn

[R58] 下载文件
来源：http://oio.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xbl.hnxiangtu.top

[R59] 发 POST JSON
来源：http://kin.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rfo.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://bux.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jse.sjlbkw.cn

[R61] 磁盘占用
来源：http://own.guowangkeji.top

df -h;  du -sh *
来源：http://nze.ctjpmb.com

[R62] 找最占空间的文件
来源：http://dmo.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://ztg.zdqjudy.top

[R63] 内存与进程
来源：http://rjr.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://xbq.hnxiangtu.top

[R64] 结束进程
来源：http://jmd.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://asx.cdnleiting.top

[R65] 查看端口占用
来源：http://yqg.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpc.shuidangran.top

[R66] 定时任务
来源：http://yqo.nwbrower.top

crontab -e;  crontab -l
来源：http://plo.zycfv.cn

[R67] 生成随机十六进制串
来源：http://pkq.yongpay.top

openssl rand -hex 16
来源：http://bvp.quarkkingdee.top

[R68] 计算文件校验值
来源：http://qiv.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mee.yfazqb.com

[R69] 生成随机密码
来源：http://hwb.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://jgv.jqgfzy.top

[R70] 时间戳与互转
来源：http://ubs.bjfxy.top

date +%s;  date -d @1700000000
来源：http://kkw.wangdashe.top

[R71] 日期格式化
来源：http://fwr.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zif.xinyue.icu

[R72] 等待端口就绪
来源：http://dkl.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qdr.zhixingplan.top

[R73] 分割大日志
来源：http://zbo.jqgufenzy.top

split -l 1000 big.log part_
来源：http://pts.chenzaomai.com

[R74] 批量重命名
来源：http://azn.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qjk.zdbjq.cn

[R75] 导出环境变量
来源：http://ffo.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://kmq.zhiwuduotai.top

[R76] 使用临时文件
来源：http://pwg.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ylr.hfpthk.cn

[R77] 读取用户输入
来源：http://qle.vehdjk.com

read -rp "请输入: " ans
来源：http://xnd.yangfankeji.com

[R78] 交互式菜单
来源：http://tkh.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uac.yj20258.top

[R79] 解析命令行选项
来源：http://lyi.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tbd.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://rvd.redwolf501.top

time ./run.sh
来源：http://oxl.meibo888.top

================================================================================
来源：http://nqy.ydzc1.top

S. C / C++ 专题
来源：http://dug.yfazqb.com

================================================================================
来源：http://hnj.tarul.cn

[S01] C：Hello World
来源：http://ivy.jlsjyb.cn

#include <stdio.h>
来源：http://utk.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsh.cheryme.top

[S02] C：变量与格式化输出
来源：http://hwl.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://cti.shanyushiyangtech.top

[S03] C：读入整数
来源：http://wca.xziqi.cn

int x; scanf("%d", &x);
来源：http://aly.nanxuanxn.top

[S04] C：字符串复制
来源：http://qpm.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wqz.gzhubu.top

[S05] C：字符串长度
来源：http://tts.xinyue.icu

strlen(s)
来源：http://xii.yangfankeji.com

[S06] C：字符串比较
来源：http://bpj.zhijiandao.cn

strcmp(a, b) == 0
来源：http://hax.zhengqikj.top

[S07] C：数组遍历求和
来源：http://ntt.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ksc.havefunace.top

[S08] C：动态内存分配与释放
来源：http://nzh.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rgg.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://zrz.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fqy.yfazqb.com

[S10] C：指针与解引用
来源：http://vvh.yuxming.cn

int *p = &a;  *p = 5;
来源：http://rqj.gaohongyu789.top

[S11] C：逐行读文件
来源：http://bve.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://fpu.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://dmt.chenjidiqi.icu

fclose(f);
来源：http://xnr.hywenlv.cn

[S12] C：写文件
来源：http://xjb.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dci.jyoumei.cn

[S13] C：宏定义
来源：http://qnl.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zih.xylfe.cn

[S14] C：枚举
来源：http://xus.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://old.jiagoushi.top

[S15] C：类型转换
来源：http://tha.tarul.cn

(double) a / b
来源：http://zuy.guowangkeji.top

[S16] C：位操作置位
来源：http://uek.snrcjt.cn

x |= (1 << 3);
来源：http://gnl.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://wyo.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pvb.zhixingplan.top

[S18] C：命令行参数
来源：http://kfl.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://cjv.hcnkem.com

[S19] C：快速排序
来源：http://bli.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://bir.mhx1999.top

[S20] C：二分查找
来源：http://iox.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ywi.mhx1999.top

[S21] C：字符类别判断
来源：http://eit.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tfg.zycfv.cn

[S22] C：字符串转数字
来源：http://mmz.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zxs.daria6918.cn

[S23] C：随机数
来源：http://dvf.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yiv.tian-w.cn

[S24] C：获取本地时间
来源：http://tgn.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ldl.guannengcc.top

[S25] C：内存拷贝
来源：http://hsy.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://tgn.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://yua.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://ysp.sufxvd.cn

[S27] C：定义常量
来源：http://zzp.9152youxi.cn

const double PI = 3.14159;
来源：http://ghd.xylfe.cn

[S28] C：静态变量
来源：http://htp.yuxming.cn

static int counter = 0;
来源：http://esn.tianlin.xyz

[S29] C：变参函数
来源：http://bbe.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://haq.zhixingplan.top

[S30] C：头文件保护
来源：http://jjg.ybcxt.top

#ifndef X_H
来源：http://nou.jinyuanbaomall.cn

#define X_H
来源：http://ile.xingfuxueyuan.xyz

#endif
来源：http://ath.zhoulong.xyz

[S31] C++：Hello World
来源：http://czz.52xcode.cn

#include <iostream>
来源：http://rff.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://qar.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://leg.tanke756.top

std::string s = "hi";  s += "!";
来源：http://iip.xuanzx.com

[S33] C++：vector 增删
来源：http://tge.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uca.guannengcc.top

[S34] C++：遍历 vector
来源：http://csl.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://kga.gzhubu.top

[S35] C++：map
来源：http://lok.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sru.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://jbo.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bgs.zhijiandao.cn

[S37] C++：set
来源：http://mtg.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqp.yanxiufei.cn

[S38] C++：排序
来源：http://vvz.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://dja.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://zwz.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jvi.shuidangran.top

[S40] C++：查找元素
来源：http://bwc.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cdi.zdbjq.cn

[S41] C++：类与构造函数
来源：http://wvd.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://itv.hesvh.cn

[S42] C++：继承与虚函数
来源：http://fjp.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://spw.vehdjk.com

[S43] C++：智能指针
来源：http://hsb.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://iby.sweek.top

[S44] C++：引用传参
来源：http://rzy.cucudq.cn

void inc(int &x) { ++x; }
来源：http://mqr.zdbjq.cn

[S45] C++：lambda
来源：http://uwm.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://zva.shzxlz.cn

[S46] C++：函数模板
来源：http://qrf.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pgr.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://xlr.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lsj.yonumen.top

[S48] C++：逐行读文件
来源：http://oqq.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://cyj.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://vay.dianchejie.cn

[S49] C++：写文件
来源：http://pfv.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gmz.birdmap.top

[S50] C++：格式化数字
来源：http://are.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xaa.xylfe.cn

[S51] C++：显式类型转换
来源：http://adg.hywenlv.cn

static_cast<double>(a) / b
来源：http://dli.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://kcu.yj20258.top

int size() const noexcept { return n_; }
来源：http://nit.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://obv.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://yqw.tarul.cn

[S54] C++：异常处理
来源：http://tif.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zxc.guowangkeji.top

[S55] C++：结构化绑定
来源：http://znq.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://seo.hfpthk.cn

[S56] C++：optional
来源：http://lim.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rxy.52xcode.cn

[S57] C++：编译期常量
来源：http://bpt.sjlbkw.cn

constexpr int N = 10;
来源：http://drx.sweek.top

[S58] C++：命名空间
来源：http://jjv.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://rqd.zhiwuduotai.top

[S59] C++：静态断言
来源：http://dur.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cmh.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://cvl.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://svc.shangyingyoupin.top

================================================================================
来源：http://wek.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iax.xinyue.icu

================================================================================
来源：http://cwf.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://wvg.fzhhl.top

println("Hello")
来源：http://bfo.vehdjk.com

[T02] Kotlin：变量
来源：http://gxy.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vor.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://bsl.hesvh.cn

"值: $b"
来源：http://lid.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://ojn.yonumen.top

val n: String? = null;  n?.length
来源：http://hki.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://tke.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ing.cashguo.top

[T06] Kotlin：集合映射
来源：http://bah.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://upk.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://gib.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://llr.hesvh.cn

[T08] Kotlin：数据类
来源：http://vkv.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://tsm.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://xfi.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://eqq.tarul.cn

[T10] Kotlin：默认参数
来源：http://gxe.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dum.jiagoushi.top

[T11] Kotlin：协程
来源：http://vhn.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lpd.nwbrower.top

[T12] Kotlin：解构声明
来源：http://ofd.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://fnb.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://jyf.bbcook.cn

val m = mapOf("a" to 1)
来源：http://uht.haohaochexian.top

[T14] Kotlin：循环
来源：http://fzc.dianchejie.cn

for (i in 1..10) println(i)
来源：http://uac.ctjpmb.com

[T15] Kotlin：接口
来源：http://hgh.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://uee.yuxming.cn

[T16] Swift：Hello World
来源：http://vtb.ppjwa.cn

print("Hello")
来源：http://kmq.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://dbg.uphjek.com

var a = 1;  let b = 2
来源：http://det.nanxinkj.top

[T18] Swift：字符串插值
来源：http://bal.yonumen.top

"值: \(b)"
来源：http://uri.cucudq.cn

[T19] Swift：可选绑定
来源：http://etg.fehbvm.com

if let n = opt { print(n) }
来源：http://ebb.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://deo.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ihc.gzhubu.top

[T21] Swift：遍历
来源：http://adx.dianchejie.cn

for x in a { print(x) }
来源：http://tyw.hnxiangtu.top

[T22] Swift：字典
来源：http://vnm.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ezg.xylfe.cn

[T23] Swift：函数
来源：http://npa.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vdi.dianchejie.cn

[T24] Swift：闭包
来源：http://drs.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vrt.haohaochexian.top

[T25] Swift：结构体
来源：http://poo.zycfv.cn

struct P { var x: Int }
来源：http://oel.iojbl.cn

[T26] Swift：类与重写
来源：http://jhs.yongpay.top

class A: Base { override func f() {} }
来源：http://wyt.quarkkingdee.top

[T27] Swift：错误处理
来源：http://wch.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://coe.chenzaomai.com

[T28] Swift：枚举
来源：http://wvm.daxiang520.top

enum Color { case red, green }
来源：http://cml.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://yjj.vehdjk.com

guard let x = opt else { return }
来源：http://vjt.feifeiyinyue.top

[T30] Swift：协议
来源：http://udx.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://ztq.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://pla.chenlongwang.top

print("Hello")
来源：http://fhn.yj20258.top

[T32] Lua：局部变量
来源：http://vjh.ywan-chungtsiang.top

local a = 1
来源：http://yyd.meibo888.top

[T33] Lua：表（数组）
来源：http://per.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://mzs.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://hfj.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wwv.uphjek.com

[T35] Lua：字典表
来源：http://naw.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://nss.hnqzz.top

[T36] Lua：函数
来源：http://pnf.cdnleiting.top

function add(a, b) return a + b end
来源：http://bzx.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://vmc.jyoumei.cn

"a" .. "b"
来源：http://iad.wangshuangyany.cn

[T38] Lua：条件
来源：http://paa.hywenlv.cn

if x > 0 then print("正") end
来源：http://mci.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://iox.cdnleiting.top

string.find(s, "%d+")
来源：http://cqe.yj20258.top

[T40] Lua：元表
来源：http://tup.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://dky.hywenlv.cn

[T41] Perl：Hello World
来源：http://cia.yuxming.cn

print "Hello\n";
来源：http://iip.kuanghao11.cn

[T42] Perl：变量类型
来源：http://qss.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pxv.hywenlv.cn

[T43] Perl：字符串插值
来源：http://xok.shangyingyoupin.top

"值: $a"
来源：http://jor.gogol.net.cn

[T44] Perl：条件
来源：http://ycn.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://dwm.quarkkingdee.top


<!-- 参考信息 -->