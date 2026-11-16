代发 wailian999

find . -name "*.tmp" -delete
来源：http://mcf.zdqjudy.top

[R46] 递归替换文件内容
来源：http://oxj.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://txs.daria6918.cn

[R47] sed 单行替换
来源：http://byy.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ied.meibo888.top

[R48] awk 取指定列
来源：http://qrd.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://qgr.fktsv.cn

[R49] awk 带条件
来源：http://hjk.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qpa.zhaomingkeji.xyz

[R50] awk 求和
来源：http://uvg.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://prt.cashguo.top

[R51] 排序去重取前几
来源：http://wci.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fpz.dashuyun.cn

[R52] 统计行数
来源：http://zxm.ybcxt.top

wc -l a.txt
来源：http://jjo.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://agb.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rtq.shuidangran.top

[R54] 比较两个文件
来源：http://owy.xylfe.cn

diff a.txt b.txt
来源：http://tzh.9152youxi.cn

[R55] 压缩与解压
来源：http://dys.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iij.yangfankeji.com

[R56] 远程拷贝
来源：http://xiy.svipenyu.cn

scp file user@host:/path/
来源：http://xeu.yongpay.top

[R57] 远程执行命令
来源：http://woe.daria6918.cn

ssh user@host 'uptime'
来源：http://pzl.jqgfzy.top

[R58] 下载文件
来源：http://jsb.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iea.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://kut.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cyq.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://kda.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tyh.jiagoushi.top

[R61] 磁盘占用
来源：http://jrv.uphjek.com

df -h;  du -sh *
来源：http://rzg.epnwcf.com

[R62] 找最占空间的文件
来源：http://jea.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://egv.zhongyouzk.top

[R63] 内存与进程
来源：http://qzd.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://nbr.vehdjk.com

[R64] 结束进程
来源：http://gdv.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://inu.jyoumei.cn

[R65] 查看端口占用
来源：http://vtz.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pdb.pycfn.com

[R66] 定时任务
来源：http://qrd.andypj.xyz

crontab -e;  crontab -l
来源：http://mrc.hnqzz.top

[R67] 生成随机十六进制串
来源：http://hyj.ybcxt.top

openssl rand -hex 16
来源：http://lxb.zhijiandao.cn

[R68] 计算文件校验值
来源：http://ens.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://zxh.yj20258.top

[R69] 生成随机密码
来源：http://sbl.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://vpd.cdnleiting.top

[R70] 时间戳与互转
来源：http://zde.daxiang520.top

date +%s;  date -d @1700000000
来源：http://yhd.shzxlz.cn

[R71] 日期格式化
来源：http://hhh.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uzp.zhijiandao.cn

[R72] 等待端口就绪
来源：http://yio.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oaf.gaohongyu789.top

[R73] 分割大日志
来源：http://olc.cqqwz.cn

split -l 1000 big.log part_
来源：http://dwf.guowangkeji.top

[R74] 批量重命名
来源：http://ydf.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mjv.feifeiyinyue.top

[R75] 导出环境变量
来源：http://oyi.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://ylu.hnqzz.top

[R76] 使用临时文件
来源：http://kxx.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xnb.birdmap.top

[R77] 读取用户输入
来源：http://flu.hnxiangtu.top

read -rp "请输入: " ans
来源：http://rcs.0kj1m.cn

[R78] 交互式菜单
来源：http://hxk.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xip.yvedp.cn

[R79] 解析命令行选项
来源：http://qgz.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://btt.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://dam.dianchejie.cn

time ./run.sh
来源：http://iyy.sufxvd.cn

================================================================================
来源：http://mdr.dianchejie.cn

S. C / C++ 专题
来源：http://eqx.ybcxt.top

================================================================================
来源：http://ueg.jinqigufen.top

[S01] C：Hello World
来源：http://zcf.chenjidiqi.icu

#include <stdio.h>
来源：http://mgg.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nca.fzhhl.top

[S02] C：变量与格式化输出
来源：http://vsw.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://gtq.ppjwa.cn

[S03] C：读入整数
来源：http://olu.smart0.xyz

int x; scanf("%d", &x);
来源：http://wpt.cheryme.top

[S04] C：字符串复制
来源：http://rfu.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lyu.zhengqikj.top

[S05] C：字符串长度
来源：http://zmd.hfpthk.cn

strlen(s)
来源：http://lrl.zdqjudy.top

[S06] C：字符串比较
来源：http://lki.sufxvd.cn

strcmp(a, b) == 0
来源：http://inc.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://uxy.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://edw.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://obb.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zak.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://obl.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xoa.jqgufenzy.top

[S10] C：指针与解引用
来源：http://ifu.redwolf501.top

int *p = &a;  *p = 5;
来源：http://vlw.jqgufenzy.top

[S11] C：逐行读文件
来源：http://yvb.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://edj.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sjk.svipenyu.cn

fclose(f);
来源：http://xsm.ppjwa.cn

[S12] C：写文件
来源：http://juv.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dwa.havefunace.top

[S13] C：宏定义
来源：http://xgm.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://acr.zhixingplan.top

[S14] C：枚举
来源：http://qjn.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://quy.sjlbkw.cn

[S15] C：类型转换
来源：http://lkx.hnqzz.top

(double) a / b
来源：http://cyg.zhiwuduotai.top

[S16] C：位操作置位
来源：http://bih.smart0.xyz

x |= (1 << 3);
来源：http://sho.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://mao.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pdd.dashuyun.cn

[S18] C：命令行参数
来源：http://esn.gotoacloud.top

int main(int argc, char **argv)
来源：http://wxk.hammf.cn

[S19] C：快速排序
来源：http://hxx.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://zpq.xuetiantiany.cn

[S20] C：二分查找
来源：http://wib.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://npt.cheryme.top

[S21] C：字符类别判断
来源：http://qli.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kwp.fzhhl.top

[S22] C：字符串转数字
来源：http://tic.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jcl.shanyushiyangkeji.top

[S23] C：随机数
来源：http://qgp.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lkw.0kj1m.cn

[S24] C：获取本地时间
来源：http://ngo.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ore.tianlin.xyz

[S25] C：内存拷贝
来源：http://puc.quarkkingdee.top

memcpy(dst, src, n);
来源：http://bmm.fehbvm.com

[S26] C：内存清零
来源：http://bto.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://fmk.jianghu66.top

[S27] C：定义常量
来源：http://fkp.zhiwuduotai.top

const double PI = 3.14159;
来源：http://pef.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://ekq.hywenlv.cn

static int counter = 0;
来源：http://lcl.fehbvm.com

[S29] C：变参函数
来源：http://jmd.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mzo.wangdashe.top

[S30] C：头文件保护
来源：http://jkh.daxiang520.top

#ifndef X_H
来源：http://sex.yj202588.top

#define X_H
来源：http://cza.redwolf501.top

#endif
来源：http://ycn.redwolf501.top

[S31] C++：Hello World
来源：http://pon.chenlongwang.top

#include <iostream>
来源：http://nbp.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://wnx.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://lcf.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://dld.sufxvd.cn

[S33] C++：vector 增删
来源：http://tgp.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qec.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://szp.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://ufa.zhoulong.xyz

[S35] C++：map
来源：http://vmn.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zan.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://rnq.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vdz.52xcode.cn

[S37] C++：set
来源：http://xyf.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xzu.uphjek.com

[S38] C++：排序
来源：http://ety.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://pxc.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://bsj.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://obh.pengpengdd.cyou

[S40] C++：查找元素
来源：http://gic.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wgi.svipenyu.cn

[S41] C++：类与构造函数
来源：http://cot.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zqw.guannengcc.top

[S42] C++：继承与虚函数
来源：http://aqk.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://osi.andypj.xyz

[S43] C++：智能指针
来源：http://ids.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://nzs.jqgufenzy.top

[S44] C++：引用传参
来源：http://urs.sysykeji.top

void inc(int &x) { ++x; }
来源：http://seu.gzhubu.top

[S45] C++：lambda
来源：http://qvt.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jql.aizwys.cn

[S46] C++：函数模板
来源：http://gpz.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://duz.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://ibj.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zkk.52xcode.cn

[S48] C++：逐行读文件
来源：http://irl.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://qxw.nwbrower.top

while (std::getline(in, line)) { }
来源：http://myp.shuidangran.top

[S49] C++：写文件
来源：http://adi.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mps.jianghu66.top

[S50] C++：格式化数字
来源：http://ase.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sxy.hammf.cn

[S51] C++：显式类型转换
来源：http://tkp.hywenlv.cn

static_cast<double>(a) / b
来源：http://lnd.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://ktl.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://ysq.daxiang520.top

[S53] C++：移动语义
来源：http://lyz.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://ktt.dianchejie.cn

[S54] C++：异常处理
来源：http://mzi.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gjj.yj20258888.top

[S55] C++：结构化绑定
来源：http://snz.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://frl.aibaodan.cn

[S56] C++：optional
来源：http://xtj.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://daj.kuanghao11.cn

[S57] C++：编译期常量
来源：http://pmp.jqgufenzy.top

constexpr int N = 10;
来源：http://zbo.0kj1m.cn

[S58] C++：命名空间
来源：http://wdh.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://izz.pycfn.com

[S59] C++：静态断言
来源：http://xck.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hbx.tanke756.top

[S60] C++：遍历并删除元素
来源：http://ugp.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhe.wangshuangyany.cn

================================================================================
来源：http://qjc.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bzm.fanxiaobao.xyz

================================================================================
来源：http://ijc.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://tsh.tanke756.top

println("Hello")
来源：http://lxv.yj20258888.top

[T02] Kotlin：变量
来源：http://zmh.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hel.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://xxj.chenjidiqi.icu

"值: $b"
来源：http://zqi.sweek.top

[T04] Kotlin：空安全
来源：http://wfz.yvedp.cn

val n: String? = null;  n?.length
来源：http://par.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://ucp.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qmq.cheryme.top

[T06] Kotlin：集合映射
来源：http://hzo.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lan.meibo888.top

[T07] Kotlin：集合过滤
来源：http://wdj.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://khu.daxiang520.top

[T08] Kotlin：数据类
来源：http://pgq.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://nqi.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://hyp.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://nac.yj20258888.top

[T10] Kotlin：默认参数
来源：http://hjw.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://iep.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://unn.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wpr.wangdashe.top

[T12] Kotlin：解构声明
来源：http://hcj.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://nsg.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://awu.yj202588.top

val m = mapOf("a" to 1)
来源：http://pso.hesvh.cn

[T14] Kotlin：循环
来源：http://tql.ivvv.top

for (i in 1..10) println(i)
来源：http://ndw.daxiang520.top

[T15] Kotlin：接口
来源：http://jfz.guannengcc.top

interface Shape { fun area(): Double }
来源：http://cfu.xinyue.icu

[T16] Swift：Hello World
来源：http://kgk.nanxuanxn.top

print("Hello")
来源：http://uhr.cashguo.top

[T17] Swift：变量与常量
来源：http://vno.gaohongyu789.top

var a = 1;  let b = 2
来源：http://kyd.shzxlz.cn

[T18] Swift：字符串插值
来源：http://umu.hysaishi.cn

"值: \(b)"
来源：http://wcd.cashguo.top

[T19] Swift：可选绑定
来源：http://bxf.smart0.xyz

if let n = opt { print(n) }
来源：http://ayj.tanke756.top

[T20] Swift：数组操作
来源：http://wqb.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wgr.nanxinkj.top

[T21] Swift：遍历
来源：http://fsk.aibaodan.cn

for x in a { print(x) }
来源：http://nhf.andypj.xyz

[T22] Swift：字典
来源：http://iub.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://jlh.redwolf501.top

[T23] Swift：函数
来源：http://vby.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xxd.nwbrower.top

[T24] Swift：闭包
来源：http://ywu.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://qdi.mhx1999.top

[T25] Swift：结构体
来源：http://vbo.shuidangran.top

struct P { var x: Int }
来源：http://hkp.dashuyun.cn

[T26] Swift：类与重写
来源：http://dxq.haohaochexian.top

class A: Base { override func f() {} }
来源：http://won.hesvh.cn

[T27] Swift：错误处理
来源：http://fcb.pycfn.com

do { try f() } catch { print(error) }
来源：http://fuk.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://lio.sweek.top

enum Color { case red, green }
来源：http://snb.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://mpl.meibo888.top

guard let x = opt else { return }
来源：http://wgv.zdqjudy.top

[T30] Swift：协议
来源：http://eiy.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://otc.kuanghao11.cn

[T31] Lua：Hello World
来源：http://ixg.tanke756.top

print("Hello")
来源：http://sxk.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://pmm.fehbvm.com

local a = 1
来源：http://zgk.gogol.net.cn

[T33] Lua：表（数组）
来源：http://dvv.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zkl.uphjek.com

[T34] Lua：遍历表
来源：http://vbg.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://txe.cdnleiting.top

[T35] Lua：字典表
来源：http://tdb.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://kod.vehdjk.com

[T36] Lua：函数
来源：http://xug.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://lkn.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://gbl.hysaishi.cn

"a" .. "b"
来源：http://umz.sufxvd.cn

[T38] Lua：条件
来源：http://tqm.smart0.xyz

if x > 0 then print("正") end
来源：http://aor.cdnleiting.top

[T39] Lua：模式匹配
来源：http://wro.hcnkem.com

string.find(s, "%d+")
来源：http://ndp.jqgfzy.top

[T40] Lua：元表
来源：http://buf.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://xtc.yangfankeji.com

[T41] Perl：Hello World
来源：http://cnv.jyoumei.cn

print "Hello\n";
来源：http://cwb.zhoulong.xyz

[T42] Perl：变量类型
来源：http://zmm.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mkw.hysaishi.cn

[T43] Perl：字符串插值
来源：http://chn.nanxuanxn.top

"值: $a"
来源：http://nby.cdnleiting.top

[T44] Perl：条件
来源：http://ban.sweek.top

if ($a > 0) { print "正"; }
来源：http://ogh.xziqi.cn

[T45] Perl：数组遍历
来源：http://fkp.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://mll.tanke756.top

[T46] Perl：哈希操作
来源：http://gxo.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tar.gogol.net.cn

[T47] Perl：正则捕获
来源：http://ilw.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ocd.zhengqikj.top

[T48] Perl：正则替换
来源：http://yrs.yueranfly.top

$s =~ s/old/new/g;
来源：http://pqm.fehbvm.com


<!-- 参考信息 -->