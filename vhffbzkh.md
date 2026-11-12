代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://toc.yangfankeji.com

[R52] 统计行数
来源：http://moy.chenzaomai.com

wc -l a.txt
来源：http://uve.tarul.cn

[R53] 查看文件头与实时尾
来源：http://tvn.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zxn.xinyue.icu

[R54] 比较两个文件
来源：http://ffd.vqdsnc.cn

diff a.txt b.txt
来源：http://uec.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://ndy.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kbj.tian-w.cn

[R56] 远程拷贝
来源：http://cgq.daxiang520.top

scp file user@host:/path/
来源：http://yhl.yuanzhike.top

[R57] 远程执行命令
来源：http://otw.yj20258.top

ssh user@host 'uptime'
来源：http://sso.snrcjt.cn

[R58] 下载文件
来源：http://vyj.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lqa.nanxuanxn.top

[R59] 发 POST JSON
来源：http://rzn.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qve.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://wnf.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nie.yangfankeji.com

[R61] 磁盘占用
来源：http://cqv.hesvh.cn

df -h;  du -sh *
来源：http://hro.nwbrower.top

[R62] 找最占空间的文件
来源：http://mre.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://qxe.cdnleiting.top

[R63] 内存与进程
来源：http://suf.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://mvd.yanxiufei.cn

[R64] 结束进程
来源：http://crf.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://soy.chenjidiqi.icu

[R65] 查看端口占用
来源：http://fkl.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ujr.xuetiantiany.cn

[R66] 定时任务
来源：http://cbw.52xcode.cn

crontab -e;  crontab -l
来源：http://lcn.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://jvx.birdmap.top

openssl rand -hex 16
来源：http://mkk.ybcxt.top

[R68] 计算文件校验值
来源：http://cbv.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://hnf.yuanzhike.top

[R69] 生成随机密码
来源：http://wjv.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://bjg.fktsv.cn

[R70] 时间戳与互转
来源：http://ibz.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://snb.cheryme.top

[R71] 日期格式化
来源：http://wfm.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fvr.jlsjyb.cn

[R72] 等待端口就绪
来源：http://loa.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tcz.hywenlv.cn

[R73] 分割大日志
来源：http://ikl.hnxiangtu.top

split -l 1000 big.log part_
来源：http://pic.sjlbkw.cn

[R74] 批量重命名
来源：http://ccb.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yiu.yuxming.cn

[R75] 导出环境变量
来源：http://xku.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://ani.tanke756.top

[R76] 使用临时文件
来源：http://ifz.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wqd.jinqigufen.top

[R77] 读取用户输入
来源：http://mdb.gaohongyu789.top

read -rp "请输入: " ans
来源：http://ths.ivvv.top

[R78] 交互式菜单
来源：http://byu.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gmf.jinqigufen.top

[R79] 解析命令行选项
来源：http://urs.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mfw.pycfn.com

[R80] 查看脚本执行耗时
来源：http://pdt.yuanzhike.top

time ./run.sh
来源：http://jxm.chenlongwang.top

================================================================================
来源：http://dhr.hongshengwenyu.top

S. C / C++ 专题
来源：http://txc.cdnleiting.top

================================================================================
来源：http://zou.yongpay.top

[S01] C：Hello World
来源：http://lom.guowangkeji.top

#include <stdio.h>
来源：http://grl.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vcq.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://eut.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://qhw.tian-w.cn

[S03] C：读入整数
来源：http://kda.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://pma.cucudq.cn

[S04] C：字符串复制
来源：http://jaw.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://uoz.bjfxy.top

[S05] C：字符串长度
来源：http://vqg.vehdjk.com

strlen(s)
来源：http://emq.ybcxt.top

[S06] C：字符串比较
来源：http://ovr.shzxlz.cn

strcmp(a, b) == 0
来源：http://tbm.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://udd.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://igt.hammf.cn

[S08] C：动态内存分配与释放
来源：http://wiv.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ehi.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://pwl.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fnr.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://fjp.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://kfi.jiagoushi.top

[S11] C：逐行读文件
来源：http://trv.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://yiz.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://hmg.gzhubu.top

fclose(f);
来源：http://cbq.zhoulong.xyz

[S12] C：写文件
来源：http://yto.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nuh.zdbjq.cn

[S13] C：宏定义
来源：http://snc.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kgn.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://zfv.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://ufz.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://yft.aibaodan.cn

(double) a / b
来源：http://wor.dashuyun.cn

[S16] C：位操作置位
来源：http://hze.ehwqpu.com

x |= (1 << 3);
来源：http://zas.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://kqy.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://apy.jianghu66.top

[S18] C：命令行参数
来源：http://lqr.zdbjq.cn

int main(int argc, char **argv)
来源：http://ylw.fktsv.cn

[S19] C：快速排序
来源：http://fum.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://abl.hnqzz.top

[S20] C：二分查找
来源：http://vwy.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://byh.cdnleiting.top

[S21] C：字符类别判断
来源：http://zmu.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://psx.gaohongyu789.top

[S22] C：字符串转数字
来源：http://aqy.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://toz.yonumen.top

[S23] C：随机数
来源：http://xro.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nra.316326.xyz

[S24] C：获取本地时间
来源：http://fch.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qdl.yj202588.top

[S25] C：内存拷贝
来源：http://izn.chenlongwang.top

memcpy(dst, src, n);
来源：http://wpz.zhiwuduotai.top

[S26] C：内存清零
来源：http://agm.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://ylc.shuidangran.top

[S27] C：定义常量
来源：http://cpu.zhoulong.xyz

const double PI = 3.14159;
来源：http://exf.shanyushiyangtech.top

[S28] C：静态变量
来源：http://ytg.pengpengdd.cyou

static int counter = 0;
来源：http://qlg.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://lqs.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mwr.zdqjudy.top

[S30] C：头文件保护
来源：http://jef.yangfankeji.com

#ifndef X_H
来源：http://hvh.xylfe.cn

#define X_H
来源：http://whn.vqdsnc.cn

#endif
来源：http://enm.hfpthk.cn

[S31] C++：Hello World
来源：http://tvm.bbcook.cn

#include <iostream>
来源：http://utv.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://xco.cdnleiting.top

[S32] C++：字符串
来源：http://jyi.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://kuq.zhongyouzk.top

[S33] C++：vector 增删
来源：http://nge.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bsl.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://zzg.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://ysn.shangyingyoupin.top

[S35] C++：map
来源：http://bzt.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pvj.jqgufenzy.top

[S36] C++：unordered_map
来源：http://oom.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jee.jianghu66.top

[S37] C++：set
来源：http://pns.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rrr.fengsongda.top

[S38] C++：排序
来源：http://mnx.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://fse.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://jts.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dxj.tarul.cn

[S40] C++：查找元素
来源：http://act.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hve.sweek.top

[S41] C++：类与构造函数
来源：http://dsl.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xxj.nwbrower.top

[S42] C++：继承与虚函数
来源：http://stm.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://usf.hnqzz.top

[S43] C++：智能指针
来源：http://svc.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://lqa.jyoumei.cn

[S44] C++：引用传参
来源：http://pdm.tarul.cn

void inc(int &x) { ++x; }
来源：http://sjm.xuetiantiany.cn

[S45] C++：lambda
来源：http://qlx.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://ans.hcnkem.com

[S46] C++：函数模板
来源：http://wvn.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tad.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://msk.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ejm.aizwys.cn

[S48] C++：逐行读文件
来源：http://akb.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://knf.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://zwz.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://zpk.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nzm.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://kqw.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ntn.yuxming.cn

[S51] C++：显式类型转换
来源：http://xzq.shzxlz.cn

static_cast<double>(a) / b
来源：http://plu.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://tdv.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://qhh.jianghu66.top

[S53] C++：移动语义
来源：http://gmp.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://dry.fengsongda.top

[S54] C++：异常处理
来源：http://sew.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wpc.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://znv.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nce.sjlbkw.cn

[S56] C++：optional
来源：http://ghn.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vso.nwbrower.top

[S57] C++：编译期常量
来源：http://ruh.zycfv.cn

constexpr int N = 10;
来源：http://wtm.sweek.top

[S58] C++：命名空间
来源：http://piu.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://dyu.pengpengdd.cyou

[S59] C++：静态断言
来源：http://xqz.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://txa.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://hbs.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wxo.feifeiyinyue.top

================================================================================
来源：http://cfc.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qrc.jinqigfzy.top

================================================================================
来源：http://hkr.hnqzz.top

[T01] Kotlin：Hello World
来源：http://ckt.52xcode.cn

println("Hello")
来源：http://kns.epnwcf.com

[T02] Kotlin：变量
来源：http://pik.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eil.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://ovg.fanxiaobao.xyz

"值: $b"
来源：http://vtt.hysaishi.cn

[T04] Kotlin：空安全
来源：http://dbk.ybcxt.top

val n: String? = null;  n?.length
来源：http://msm.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://gfn.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ent.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://kbh.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nld.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://ovh.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sko.fengsongda.top

[T08] Kotlin：数据类
来源：http://ked.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://auk.tanke756.top

[T09] Kotlin：扩展函数
来源：http://bgi.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://iur.hnqzz.top

[T10] Kotlin：默认参数
来源：http://lhh.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tso.jiagoushi.top

[T11] Kotlin：协程
来源：http://cxm.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wvo.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://zcq.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://prv.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://arv.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://qhk.ctjpmb.com

[T14] Kotlin：循环
来源：http://vlo.hnqzz.top

for (i in 1..10) println(i)
来源：http://grn.jinqigfzy.top

[T15] Kotlin：接口
来源：http://ezg.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://qzo.0kj1m.cn

[T16] Swift：Hello World
来源：http://evc.ehwqpu.com

print("Hello")
来源：http://hxf.gogol.net.cn

[T17] Swift：变量与常量
来源：http://yaj.zdqjudy.top

var a = 1;  let b = 2
来源：http://hpw.yongpay.top

[T18] Swift：字符串插值
来源：http://tpp.zhaomingkeji.xyz

"值: \(b)"
来源：http://iqq.zhengqikj.top

[T19] Swift：可选绑定
来源：http://jmy.gaohongyu789.top

if let n = opt { print(n) }
来源：http://ejd.aibaodan.cn

[T20] Swift：数组操作
来源：http://vnb.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://cvl.sweek.top

[T21] Swift：遍历
来源：http://uhl.redwolf501.top

for x in a { print(x) }
来源：http://kky.jinqigfzy.top

[T22] Swift：字典
来源：http://eia.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://urs.xylfe.cn

[T23] Swift：函数
来源：http://ipw.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fvr.tian-w.cn

[T24] Swift：闭包
来源：http://yqx.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sfz.sysykeji.top

[T25] Swift：结构体
来源：http://eya.fanxiaobao.xyz

struct P { var x: Int }
来源：http://mqd.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://zfr.jinqigufen.top

class A: Base { override func f() {} }
来源：http://trw.hammf.cn

[T27] Swift：错误处理
来源：http://rbm.redwolf501.top

do { try f() } catch { print(error) }
来源：http://jdy.gzhubu.top

[T28] Swift：枚举
来源：http://wdw.cucudq.cn

enum Color { case red, green }
来源：http://afc.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://znt.yueranfly.top

guard let x = opt else { return }
来源：http://srx.tian-w.cn

[T30] Swift：协议
来源：http://qjj.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://nwy.hywenlv.cn

[T31] Lua：Hello World
来源：http://aio.shanyushiyangtech.top

print("Hello")
来源：http://mpm.aibaodan.cn

[T32] Lua：局部变量
来源：http://lpz.daria6918.cn

local a = 1
来源：http://aru.yj20258.top

[T33] Lua：表（数组）
来源：http://qxx.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ijb.zhengqikj.top

[T34] Lua：遍历表
来源：http://thf.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://uta.snrcjt.cn

[T35] Lua：字典表
来源：http://lzr.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://wwr.yueranfly.top

[T36] Lua：函数
来源：http://ufe.iojbl.cn

function add(a, b) return a + b end
来源：http://yzp.yfazqb.com

[T37] Lua：字符串拼接
来源：http://qfe.jlsjyb.cn

"a" .. "b"
来源：http://usb.cashguo.top

[T38] Lua：条件
来源：http://rfv.sysykeji.top

if x > 0 then print("正") end
来源：http://qlw.hysaishi.cn

[T39] Lua：模式匹配
来源：http://aar.zdbjq.cn

string.find(s, "%d+")
来源：http://ump.birdmap.top

[T40] Lua：元表
来源：http://wgo.yvedp.cn

setmetatable({}, { __index = base })
来源：http://anb.hcnkem.com

[T41] Perl：Hello World
来源：http://xhq.zhengqikj.top

print "Hello\n";
来源：http://bum.guannengcc.top

[T42] Perl：变量类型
来源：http://prp.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cku.zhixingplan.top

[T43] Perl：字符串插值
来源：http://eep.redwolf501.top

"值: $a"
来源：http://bpv.jqgfzy.top

[T44] Perl：条件
来源：http://kum.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://ipt.tanke756.top

[T45] Perl：数组遍历
来源：http://lgz.yj202588.top

for my $x (@arr) { print $x; }
来源：http://oin.guowangkeji.top

[T46] Perl：哈希操作
来源：http://dxu.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mat.xuanzx.com

[T47] Perl：正则捕获
来源：http://yyc.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://djt.kuanghao11.cn

[T48] Perl：正则替换
来源：http://smm.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://nye.quarkkingdee.top

[T49] Perl：函数
来源：http://eez.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://erd.cheryme.top

[T50] Perl：逐行读文件
来源：http://gvw.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wsg.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://ltv.yuxming.cn

[T51] Scala：Hello World
来源：http://jse.hammf.cn

println("Hello")
来源：http://kpo.svipenyu.cn

[T52] Scala：变量
来源：http://hgt.ppjwa.cn

val a = 1;  var b = 2
来源：http://upk.yuxming.cn

[T53] Scala：字符串插值
来源：http://eeo.0kj1m.cn

s"值: $b"
来源：http://ima.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://iqk.sjlbkw.cn


<!-- 参考信息 -->