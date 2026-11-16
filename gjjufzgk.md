代发 wailian999

find . -name "*.tmp" -delete
来源：http://txj.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://uan.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ffn.zhengqikj.top

[R47] sed 单行替换
来源：http://hlc.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://apz.hfpthk.cn

[R48] awk 取指定列
来源：http://lta.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://ayf.hywenlv.cn

[R49] awk 带条件
来源：http://tdr.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cxe.fanxiaobao.xyz

[R50] awk 求和
来源：http://jag.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ita.zhijiandao.cn

[R51] 排序去重取前几
来源：http://gyy.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lru.fengsongda.top

[R52] 统计行数
来源：http://mkm.dianchejie.cn

wc -l a.txt
来源：http://qik.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://kkb.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ill.9152youxi.cn

[R54] 比较两个文件
来源：http://azt.havefunace.top

diff a.txt b.txt
来源：http://gwl.redwolf501.top

[R55] 压缩与解压
来源：http://dhk.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ajv.bbcook.cn

[R56] 远程拷贝
来源：http://knb.jiagoushi.top

scp file user@host:/path/
来源：http://huq.yueranfly.top

[R57] 远程执行命令
来源：http://uqp.xylfe.cn

ssh user@host 'uptime'
来源：http://eri.hnqzz.top

[R58] 下载文件
来源：http://tbg.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wcf.ehwqpu.com

[R59] 发 POST JSON
来源：http://znc.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hzh.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://hlc.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dcm.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://zry.xuetiantiany.cn

df -h;  du -sh *
来源：http://dnc.sweek.top

[R62] 找最占空间的文件
来源：http://tgr.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://far.xuanzx.com

[R63] 内存与进程
来源：http://tmq.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://mlj.tianlin.xyz

[R64] 结束进程
来源：http://vtk.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://iso.hysaishi.cn

[R65] 查看端口占用
来源：http://yzu.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ipz.gzhubu.top

[R66] 定时任务
来源：http://xdi.shuidangran.top

crontab -e;  crontab -l
来源：http://thf.bbcook.cn

[R67] 生成随机十六进制串
来源：http://ogy.epnwcf.com

openssl rand -hex 16
来源：http://vjm.zhoulong.xyz

[R68] 计算文件校验值
来源：http://ovm.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://wiw.cheryme.top

[R69] 生成随机密码
来源：http://ftw.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://xhv.jyoumei.cn

[R70] 时间戳与互转
来源：http://pnm.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://cfu.fehbvm.com

[R71] 日期格式化
来源：http://pug.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbv.hywenlv.cn

[R72] 等待端口就绪
来源：http://wkf.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qlc.xylfe.cn

[R73] 分割大日志
来源：http://klo.sxryk.cn

split -l 1000 big.log part_
来源：http://sua.hcnkem.com

[R74] 批量重命名
来源：http://vgz.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fgz.yangfankeji.com

[R75] 导出环境变量
来源：http://lix.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://yxr.c1oappe.top

[R76] 使用临时文件
来源：http://sju.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nbo.andypj.xyz

[R77] 读取用户输入
来源：http://lyy.yongpay.top

read -rp "请输入: " ans
来源：http://gvq.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://svd.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xdy.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://xzp.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ugi.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://jts.cqqwz.cn

time ./run.sh
来源：http://wei.sxryk.cn

================================================================================
来源：http://ipg.wangshuangyany.cn

S. C / C++ 专题
来源：http://udv.316326.xyz

================================================================================
来源：http://vlb.ehwqpu.com

[S01] C：Hello World
来源：http://bdf.ywan-chungtsiang.top

#include <stdio.h>
来源：http://vcg.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://drx.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://ouj.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://byb.pengpengdd.cyou

[S03] C：读入整数
来源：http://gvr.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://ucd.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://vgf.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yho.316326.xyz

[S05] C：字符串长度
来源：http://mcw.andypj.xyz

strlen(s)
来源：http://lwm.kuanghao11.cn

[S06] C：字符串比较
来源：http://uby.dashuyun.cn

strcmp(a, b) == 0
来源：http://vsi.shzxlz.cn

[S07] C：数组遍历求和
来源：http://kac.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jgz.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://pon.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tyj.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://jna.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://paw.chenzaomai.com

[S10] C：指针与解引用
来源：http://xet.shuidangran.top

int *p = &a;  *p = 5;
来源：http://txh.jlsjyb.cn

[S11] C：逐行读文件
来源：http://pwg.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://lzs.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nsk.jinqigfzy.top

fclose(f);
来源：http://ttz.jyoumei.cn

[S12] C：写文件
来源：http://eis.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pyf.wangdashe.top

[S13] C：宏定义
来源：http://xqn.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qjv.zhixingplan.top

[S14] C：枚举
来源：http://dmh.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://vut.zhijiandao.cn

[S15] C：类型转换
来源：http://evo.yfazqb.com

(double) a / b
来源：http://hew.jinqigfzy.top

[S16] C：位操作置位
来源：http://kuz.vqdsnc.cn

x |= (1 << 3);
来源：http://mod.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://igg.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://owd.yuxming.cn

[S18] C：命令行参数
来源：http://ape.zhixingplan.top

int main(int argc, char **argv)
来源：http://gop.iojbl.cn

[S19] C：快速排序
来源：http://sys.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://xaa.yvedp.cn

[S20] C：二分查找
来源：http://pnk.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cqn.hnqzz.top

[S21] C：字符类别判断
来源：http://ojr.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://joj.chenlongwang.top

[S22] C：字符串转数字
来源：http://pbp.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://dys.iojbl.cn

[S23] C：随机数
来源：http://crj.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ipq.bjfxy.top

[S24] C：获取本地时间
来源：http://peu.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kbw.tianlin.xyz

[S25] C：内存拷贝
来源：http://gfz.epnwcf.com

memcpy(dst, src, n);
来源：http://ooh.gaohongyu789.top

[S26] C：内存清零
来源：http://zzn.birdmap.top

memset(a, 0, sizeof a);
来源：http://fdx.tianlin.xyz

[S27] C：定义常量
来源：http://ucg.fktsv.cn

const double PI = 3.14159;
来源：http://jhf.andypj.xyz

[S28] C：静态变量
来源：http://alw.sysykeji.top

static int counter = 0;
来源：http://ack.zhongyouzk.top

[S29] C：变参函数
来源：http://jpo.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cts.ppjwa.cn

[S30] C：头文件保护
来源：http://zao.shangyingyoupin.top

#ifndef X_H
来源：http://fqe.fengsongda.top

#define X_H
来源：http://mjq.yj202588.top

#endif
来源：http://ecz.gaohongyu789.top

[S31] C++：Hello World
来源：http://cvm.zhongyouzk.top

#include <iostream>
来源：http://ssr.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://nxu.epnwcf.com

[S32] C++：字符串
来源：http://mti.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://pwe.zhongyouzk.top

[S33] C++：vector 增删
来源：http://maj.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lsd.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://fyd.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://quk.fanxiaobao.xyz

[S35] C++：map
来源：http://aej.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gli.yangfankeji.com

[S36] C++：unordered_map
来源：http://rjg.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qyb.fengsongda.top

[S37] C++：set
来源：http://okl.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://soq.wangdashe.top

[S38] C++：排序
来源：http://uot.tanke756.top

std::sort(v.begin(), v.end());
来源：http://aow.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://kmg.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zpp.daria6918.cn

[S40] C++：查找元素
来源：http://pxg.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zgq.cucudq.cn

[S41] C++：类与构造函数
来源：http://oes.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xxv.uphjek.com

[S42] C++：继承与虚函数
来源：http://rpq.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://smg.sjlbkw.cn

[S43] C++：智能指针
来源：http://pfz.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://ekv.jyoumei.cn

[S44] C++：引用传参
来源：http://cem.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://wfg.epnwcf.com

[S45] C++：lambda
来源：http://oge.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://cic.aibaodan.cn

[S46] C++：函数模板
来源：http://rth.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lor.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://fyn.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tix.haohaochexian.top

[S48] C++：逐行读文件
来源：http://aur.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kok.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://ays.jqgfzy.top

[S49] C++：写文件
来源：http://lll.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://che.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://kvr.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pdr.xziqi.cn

[S51] C++：显式类型转换
来源：http://qpc.shzxlz.cn

static_cast<double>(a) / b
来源：http://vlp.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://xlz.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://wzb.hnqzz.top

[S53] C++：移动语义
来源：http://whh.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://hyt.cdnleiting.top

[S54] C++：异常处理
来源：http://vna.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xxv.jqgfzy.top

[S55] C++：结构化绑定
来源：http://afp.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qql.ctjpmb.com

[S56] C++：optional
来源：http://zng.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nns.guowangkeji.top

[S57] C++：编译期常量
来源：http://sgh.xziqi.cn

constexpr int N = 10;
来源：http://cvz.zhongyouzk.top

[S58] C++：命名空间
来源：http://fbp.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://rpz.mhx1999.top

[S59] C++：静态断言
来源：http://qip.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zcw.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://nls.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://snf.feifeiyinyue.top

================================================================================
来源：http://mqr.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xnw.hongshengwenyu.top

================================================================================
来源：http://fmn.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://yje.chenjidiqi.icu

println("Hello")
来源：http://xwm.zhongyouzk.top

[T02] Kotlin：变量
来源：http://dow.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dcr.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://qdg.nanxinkj.top

"值: $b"
来源：http://xrq.bbcook.cn

[T04] Kotlin：空安全
来源：http://kub.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://wwg.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://wsy.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eva.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://szk.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://irr.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://dng.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rqv.jiagoushi.top

[T08] Kotlin：数据类
来源：http://zoz.havefunace.top

data class User(val name: String, val age: Int)
来源：http://bak.yonumen.top

[T09] Kotlin：扩展函数
来源：http://zcy.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://fjw.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://ngc.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rmy.ehwqpu.com

[T11] Kotlin：协程
来源：http://xnj.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnw.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://mop.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://pvr.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://ang.xuanzx.com

val m = mapOf("a" to 1)
来源：http://hgq.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://mqi.hnqzz.top

for (i in 1..10) println(i)
来源：http://yji.gaohongyu789.top

[T15] Kotlin：接口
来源：http://swf.birdmap.top

interface Shape { fun area(): Double }
来源：http://noy.jqgfzy.top

[T16] Swift：Hello World
来源：http://shc.yanxiufei.cn

print("Hello")
来源：http://vhu.fehbvm.com

[T17] Swift：变量与常量
来源：http://jpg.shzxlz.cn

var a = 1;  let b = 2
来源：http://rfj.redwolf501.top

[T18] Swift：字符串插值
来源：http://jyj.zhengqikj.top

"值: \(b)"
来源：http://cui.meibo888.top

[T19] Swift：可选绑定
来源：http://tkz.cucudq.cn

if let n = opt { print(n) }
来源：http://htr.zycfv.cn

[T20] Swift：数组操作
来源：http://ugy.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://usf.fengsongda.top

[T21] Swift：遍历
来源：http://bhh.vehdjk.com

for x in a { print(x) }
来源：http://vvb.fktsv.cn

[T22] Swift：字典
来源：http://fmj.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://fna.xylfe.cn

[T23] Swift：函数
来源：http://xum.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dqi.shangyingyoupin.top

[T24] Swift：闭包
来源：http://zod.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://crw.ydzc1.top

[T25] Swift：结构体
来源：http://ttj.zhongyouzk.top

struct P { var x: Int }
来源：http://nrg.xinyue.icu

[T26] Swift：类与重写
来源：http://gdy.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://jrr.cashguo.top

[T27] Swift：错误处理
来源：http://uwd.uphjek.com

do { try f() } catch { print(error) }
来源：http://zus.hnxiangtu.top

[T28] Swift：枚举
来源：http://htg.ctjpmb.com

enum Color { case red, green }
来源：http://igf.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://voz.vehdjk.com

guard let x = opt else { return }
来源：http://tvn.wangshuangyany.cn

[T30] Swift：协议
来源：http://yvt.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://kwy.tianlin.xyz

[T31] Lua：Hello World
来源：http://pou.yj20258.top

print("Hello")
来源：http://azp.shuidangran.top

[T32] Lua：局部变量
来源：http://eil.yuanzhike.top

local a = 1
来源：http://ykm.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://ysl.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zqs.jiagoushi.top

[T34] Lua：遍历表
来源：http://krs.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wcb.jqgufenzy.top

[T35] Lua：字典表
来源：http://fit.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://trs.jqgfzy.top

[T36] Lua：函数
来源：http://pzc.smart0.xyz

function add(a, b) return a + b end
来源：http://uwh.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://mpz.tanke756.top

"a" .. "b"
来源：http://kvm.sufxvd.cn

[T38] Lua：条件
来源：http://yfa.ppjwa.cn

if x > 0 then print("正") end
来源：http://ccp.mhx1999.top

[T39] Lua：模式匹配
来源：http://qhr.jiagoushi.top

string.find(s, "%d+")
来源：http://ggg.ehwqpu.com

[T40] Lua：元表
来源：http://wau.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://efd.hfpthk.cn

[T41] Perl：Hello World
来源：http://fot.yonumen.top

print "Hello\n";
来源：http://rwq.jyoumei.cn

[T42] Perl：变量类型
来源：http://yds.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://umk.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://nyv.sxryk.cn

"值: $a"
来源：http://kxf.aizwys.cn

[T44] Perl：条件
来源：http://ahq.yj202588.top

if ($a > 0) { print "正"; }
来源：http://ylh.52xcode.cn

[T45] Perl：数组遍历
来源：http://btz.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://hws.316326.xyz

[T46] Perl：哈希操作
来源：http://ztf.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ayp.yonumen.top

[T47] Perl：正则捕获
来源：http://gaa.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://pea.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://ual.fktsv.cn

$s =~ s/old/new/g;
来源：http://dba.svipenyu.cn


<!-- 参考信息 -->