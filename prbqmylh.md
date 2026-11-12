代发 wailian999

find . -name "*.log" -type f
来源：http://axw.ybcxt.top

[R44] 按修改时间查找
来源：http://vvu.dashuyun.cn

find . -mtime -7 -type f
来源：http://ank.hcnkem.com

[R45] 批量删除
来源：http://rwg.daxiang520.top

find . -name "*.tmp" -delete
来源：http://qux.yuanzhike.top

[R46] 递归替换文件内容
来源：http://iys.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zth.ydjk.org.cn

[R47] sed 单行替换
来源：http://ezk.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://yat.daxiang520.top

[R48] awk 取指定列
来源：http://rdm.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://mmg.jianghu66.top

[R49] awk 带条件
来源：http://zli.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jbw.feifeiyinyue.top

[R50] awk 求和
来源：http://kmd.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://qit.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://zfw.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fqi.gotoacloud.top

[R52] 统计行数
来源：http://gpv.hcnkem.com

wc -l a.txt
来源：http://ucc.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://wqg.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://plc.ivvv.top

[R54] 比较两个文件
来源：http://kul.bjfxy.top

diff a.txt b.txt
来源：http://fyp.0kj1m.cn

[R55] 压缩与解压
来源：http://xal.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uun.gotoacloud.top

[R56] 远程拷贝
来源：http://jwf.jqgufenzy.top

scp file user@host:/path/
来源：http://zrs.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://ido.sweek.top

ssh user@host 'uptime'
来源：http://rka.ctjpmb.com

[R58] 下载文件
来源：http://qua.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wbc.yongpay.top

[R59] 发 POST JSON
来源：http://tja.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lrm.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://qoh.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://scj.hfpthk.cn

[R61] 磁盘占用
来源：http://tkk.xylfe.cn

df -h;  du -sh *
来源：http://hfg.hammf.cn

[R62] 找最占空间的文件
来源：http://qiu.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://akq.jianghu66.top

[R63] 内存与进程
来源：http://rvu.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://wcw.jqgfzy.top

[R64] 结束进程
来源：http://bxx.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://okf.xuetiantiany.cn

[R65] 查看端口占用
来源：http://brr.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tdp.uphjek.com

[R66] 定时任务
来源：http://csy.hywenlv.cn

crontab -e;  crontab -l
来源：http://wrc.havefunace.top

[R67] 生成随机十六进制串
来源：http://soy.havefunace.top

openssl rand -hex 16
来源：http://cjk.316326.xyz

[R68] 计算文件校验值
来源：http://svx.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://gep.xylfe.cn

[R69] 生成随机密码
来源：http://vgp.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://nvi.316326.xyz

[R70] 时间戳与互转
来源：http://wda.yj20258.top

date +%s;  date -d @1700000000
来源：http://riz.jinghuilouyu.cn

[R71] 日期格式化
来源：http://bdd.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hkf.chenzaomai.com

[R72] 等待端口就绪
来源：http://uin.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwq.bbcook.cn

[R73] 分割大日志
来源：http://ggd.fktsv.cn

split -l 1000 big.log part_
来源：http://ksw.sufxvd.cn

[R74] 批量重命名
来源：http://uyw.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wmq.fengsongda.top

[R75] 导出环境变量
来源：http://nyt.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wju.mhx1999.top

[R76] 使用临时文件
来源：http://jnp.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pck.redwolf501.top

[R77] 读取用户输入
来源：http://ctz.tanke756.top

read -rp "请输入: " ans
来源：http://mys.birdmap.top

[R78] 交互式菜单
来源：http://zgv.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hdx.mhx1999.top

[R79] 解析命令行选项
来源：http://jtl.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sds.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://pnt.jiagoushi.top

time ./run.sh
来源：http://stx.zhijiandao.cn

================================================================================
来源：http://fsn.hammf.cn

S. C / C++ 专题
来源：http://yvh.zhaomingkeji.xyz

================================================================================
来源：http://ifg.xziqi.cn

[S01] C：Hello World
来源：http://cqn.jinyuanbaomall.cn

#include <stdio.h>
来源：http://wdw.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wxq.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://nxx.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://yji.hammf.cn

[S03] C：读入整数
来源：http://gpc.aizwys.cn

int x; scanf("%d", &x);
来源：http://bem.tian-w.cn

[S04] C：字符串复制
来源：http://psu.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://edy.xuanzx.com

[S05] C：字符串长度
来源：http://ore.9152youxi.cn

strlen(s)
来源：http://ymy.yongpay.top

[S06] C：字符串比较
来源：http://cuy.9152youxi.cn

strcmp(a, b) == 0
来源：http://xna.jqgfzy.top

[S07] C：数组遍历求和
来源：http://cto.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ncd.yonumen.top

[S08] C：动态内存分配与释放
来源：http://lcj.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ucd.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://gnk.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tzz.gzhubu.top

[S10] C：指针与解引用
来源：http://ert.daxiang520.top

int *p = &a;  *p = 5;
来源：http://myi.chenzaomai.com

[S11] C：逐行读文件
来源：http://zjd.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://iuj.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xxh.ivvv.top

fclose(f);
来源：http://muz.yanxiufei.cn

[S12] C：写文件
来源：http://hoj.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://idd.hnxiangtu.top

[S13] C：宏定义
来源：http://fps.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xvs.sysykeji.top

[S14] C：枚举
来源：http://zvo.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://eei.svipenyu.cn

[S15] C：类型转换
来源：http://hyr.aizwys.cn

(double) a / b
来源：http://rfl.bbcook.cn

[S16] C：位操作置位
来源：http://wvb.daria6918.cn

x |= (1 << 3);
来源：http://gkz.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://pha.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ftx.chenzaomai.com

[S18] C：命令行参数
来源：http://hpt.havefunace.top

int main(int argc, char **argv)
来源：http://jva.jianghu66.top

[S19] C：快速排序
来源：http://ykx.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://spc.sweek.top

[S20] C：二分查找
来源：http://zpw.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vmo.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://agx.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://esu.yanxiufei.cn

[S22] C：字符串转数字
来源：http://wzg.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rke.cucudq.cn

[S23] C：随机数
来源：http://uhw.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://eum.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://rje.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://snu.316326.xyz

[S25] C：内存拷贝
来源：http://nuc.tarul.cn

memcpy(dst, src, n);
来源：http://cty.jianghu66.top

[S26] C：内存清零
来源：http://sfi.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://qwl.aizwys.cn

[S27] C：定义常量
来源：http://qoo.chenlongwang.top

const double PI = 3.14159;
来源：http://qas.xylfe.cn

[S28] C：静态变量
来源：http://kre.yj202588.top

static int counter = 0;
来源：http://yld.chenzaomai.com

[S29] C：变参函数
来源：http://gmi.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wod.svipenyu.cn

[S30] C：头文件保护
来源：http://dnr.vqdsnc.cn

#ifndef X_H
来源：http://ecv.zhaomingkeji.xyz

#define X_H
来源：http://bzi.shangyingyoupin.top

#endif
来源：http://ipa.jiagoushi.top

[S31] C++：Hello World
来源：http://yoz.ywan-chungtsiang.top

#include <iostream>
来源：http://xif.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://yyw.yj202588.top

[S32] C++：字符串
来源：http://qgm.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://xwj.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://zzy.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bdu.cdnleiting.top

[S34] C++：遍历 vector
来源：http://zzu.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://sxj.hnqzz.top

[S35] C++：map
来源：http://yve.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rrc.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://lub.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vfb.vqdsnc.cn

[S37] C++：set
来源：http://qzr.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wjt.yuanzhike.top

[S38] C++：排序
来源：http://nmc.pycfn.com

std::sort(v.begin(), v.end());
来源：http://kql.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://nkq.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lqm.yj20258.top

[S40] C++：查找元素
来源：http://wfq.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sae.birdmap.top

[S41] C++：类与构造函数
来源：http://znk.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wvv.pycfn.com

[S42] C++：继承与虚函数
来源：http://hpi.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://cnw.xuetiantiany.cn

[S43] C++：智能指针
来源：http://dqp.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://eyy.hesvh.cn

[S44] C++：引用传参
来源：http://ztn.sweek.top

void inc(int &x) { ++x; }
来源：http://idn.shzxlz.cn

[S45] C++：lambda
来源：http://grf.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bcl.chenjidiqi.icu

[S46] C++：函数模板
来源：http://sxa.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://moq.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://ene.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ysm.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://cox.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://zuy.ydzc1.top

while (std::getline(in, line)) { }
来源：http://efn.fktsv.cn

[S49] C++：写文件
来源：http://mqh.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tuc.yvedp.cn

[S50] C++：格式化数字
来源：http://lkr.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rfj.sweek.top

[S51] C++：显式类型转换
来源：http://ctu.dianchejie.cn

static_cast<double>(a) / b
来源：http://lrl.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://wkj.hcnkem.com

int size() const noexcept { return n_; }
来源：http://tab.nanxinkj.top

[S53] C++：移动语义
来源：http://aem.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://evo.fzhhl.top

[S54] C++：异常处理
来源：http://gyp.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uyh.jiagoushi.top

[S55] C++：结构化绑定
来源：http://qvu.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://bda.fengsongda.top

[S56] C++：optional
来源：http://pcx.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ohs.hammf.cn

[S57] C++：编译期常量
来源：http://zun.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://eyl.cashguo.top

[S58] C++：命名空间
来源：http://ens.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://uwk.gogol.net.cn

[S59] C++：静态断言
来源：http://olh.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oae.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://xkr.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xyp.birdmap.top

================================================================================
来源：http://dhp.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yrb.zycfv.cn

================================================================================
来源：http://msc.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://xoo.yj20258.top

println("Hello")
来源：http://udx.tarul.cn

[T02] Kotlin：变量
来源：http://nts.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://whv.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://tzi.havefunace.top

"值: $b"
来源：http://anw.jiagoushi.top

[T04] Kotlin：空安全
来源：http://hle.gogol.net.cn

val n: String? = null;  n?.length
来源：http://jqz.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://who.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qkc.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://uqf.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zmv.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://ilw.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rss.xuanzx.com

[T08] Kotlin：数据类
来源：http://dxo.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://spm.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://wzl.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://hsm.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://yem.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hjz.zdqjudy.top

[T11] Kotlin：协程
来源：http://qtm.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mkl.guannengcc.top

[T12] Kotlin：解构声明
来源：http://bkb.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://cuj.pycfn.com

[T13] Kotlin：只读 Map
来源：http://lki.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://xaz.nanxuanxn.top

[T14] Kotlin：循环
来源：http://usr.52xcode.cn

for (i in 1..10) println(i)
来源：http://uqu.hesvh.cn

[T15] Kotlin：接口
来源：http://pxk.sxryk.cn

interface Shape { fun area(): Double }
来源：http://ptw.yvedp.cn

[T16] Swift：Hello World
来源：http://lly.nwbrower.top

print("Hello")
来源：http://rup.yueranfly.top

[T17] Swift：变量与常量
来源：http://veb.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://axd.yfazqb.com

[T18] Swift：字符串插值
来源：http://dkj.chenlongwang.top

"值: \(b)"
来源：http://sbf.zdbjq.cn

[T19] Swift：可选绑定
来源：http://qyw.hnxiangtu.top

if let n = opt { print(n) }
来源：http://zhz.ehwqpu.com

[T20] Swift：数组操作
来源：http://hha.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://fwg.sweek.top

[T21] Swift：遍历
来源：http://jam.chenjidiqi.icu

for x in a { print(x) }
来源：http://mwc.aizwys.cn

[T22] Swift：字典
来源：http://ogl.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://cjw.zhoulong.xyz

[T23] Swift：函数
来源：http://ekw.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qxq.yangfankeji.com

[T24] Swift：闭包
来源：http://hpb.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tif.zhengqikj.top

[T25] Swift：结构体
来源：http://smq.havefunace.top

struct P { var x: Int }
来源：http://epf.0kj1m.cn

[T26] Swift：类与重写
来源：http://lex.fehbvm.com

class A: Base { override func f() {} }
来源：http://lqx.tarul.cn

[T27] Swift：错误处理
来源：http://srw.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://mxy.wangdashe.top

[T28] Swift：枚举
来源：http://zvd.zhiwuduotai.top

enum Color { case red, green }
来源：http://tto.yj20258.top

[T29] Swift：guard 提前返回
来源：http://sow.pengpengdd.cyou

guard let x = opt else { return }
来源：http://lax.andypj.xyz

[T30] Swift：协议
来源：http://iiv.birdmap.top

protocol Shape { func area() -> Double }
来源：http://arb.316326.xyz

[T31] Lua：Hello World
来源：http://zwn.feifeiyinyue.top

print("Hello")
来源：http://jqh.hammf.cn

[T32] Lua：局部变量
来源：http://gdj.guannengcc.top

local a = 1
来源：http://vqb.pycfn.com

[T33] Lua：表（数组）
来源：http://xgr.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pdy.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://zxi.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gug.shzxlz.cn

[T35] Lua：字典表
来源：http://uvi.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://gzb.tian-w.cn

[T36] Lua：函数
来源：http://xfo.uphjek.com

function add(a, b) return a + b end
来源：http://xvr.xziqi.cn

[T37] Lua：字符串拼接
来源：http://umx.zhixingplan.top

"a" .. "b"
来源：http://wgg.gaohongyu789.top

[T38] Lua：条件
来源：http://xku.cashguo.top

if x > 0 then print("正") end
来源：http://xep.epnwcf.com

[T39] Lua：模式匹配
来源：http://ubi.fehbvm.com

string.find(s, "%d+")
来源：http://upu.vqdsnc.cn

[T40] Lua：元表
来源：http://pch.ydzc1.top

setmetatable({}, { __index = base })
来源：http://csk.zhixingplan.top

[T41] Perl：Hello World
来源：http://ugk.chenjidiqi.icu

print "Hello\n";
来源：http://amp.nanxuanxn.top

[T42] Perl：变量类型
来源：http://aps.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rep.nanxinkj.top

[T43] Perl：字符串插值
来源：http://ftr.zhoulong.xyz

"值: $a"
来源：http://rad.yfazqb.com

[T44] Perl：条件
来源：http://ndi.cashguo.top

if ($a > 0) { print "正"; }
来源：http://eea.zhixingplan.top

[T45] Perl：数组遍历
来源：http://aiv.ivvv.top

for my $x (@arr) { print $x; }
来源：http://isr.gotoacloud.top

[T46] Perl：哈希操作
来源：http://kho.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zai.dashuyun.cn


<!-- 参考信息 -->