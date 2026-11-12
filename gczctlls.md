代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://yqy.yj20258.top

[R48] awk 取指定列
来源：http://btb.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://fqz.shangyingyoupin.top

[R49] awk 带条件
来源：http://hho.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bms.jlsjyb.cn

[R50] awk 求和
来源：http://xqu.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://hga.yongpay.top

[R51] 排序去重取前几
来源：http://jun.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://lii.chenzaomai.com

[R52] 统计行数
来源：http://izi.wangdashe.top

wc -l a.txt
来源：http://bxb.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://ofk.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fkp.nanxuanxn.top

[R54] 比较两个文件
来源：http://eym.hywenlv.cn

diff a.txt b.txt
来源：http://urq.c1oappe.top

[R55] 压缩与解压
来源：http://mzh.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xzo.hongshengwenyu.top

[R56] 远程拷贝
来源：http://gqi.xinyue.icu

scp file user@host:/path/
来源：http://klk.yuanzhike.top

[R57] 远程执行命令
来源：http://ufs.zycfv.cn

ssh user@host 'uptime'
来源：http://qtk.jinqigfzy.top

[R58] 下载文件
来源：http://gxu.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hfc.sjlbkw.cn

[R59] 发 POST JSON
来源：http://ken.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jgx.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://rcx.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vme.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://koe.zhoulong.xyz

df -h;  du -sh *
来源：http://wyv.uphjek.com

[R62] 找最占空间的文件
来源：http://wxg.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://jdk.cdnleiting.top

[R63] 内存与进程
来源：http://uxe.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://exw.sjlbkw.cn

[R64] 结束进程
来源：http://dny.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://fan.cashguo.top

[R65] 查看端口占用
来源：http://lqm.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bsk.shzxlz.cn

[R66] 定时任务
来源：http://qer.zhijiandao.cn

crontab -e;  crontab -l
来源：http://hux.vehdjk.com

[R67] 生成随机十六进制串
来源：http://dmy.dianchejie.cn

openssl rand -hex 16
来源：http://oor.sysykeji.top

[R68] 计算文件校验值
来源：http://yiy.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vyo.sxryk.cn

[R69] 生成随机密码
来源：http://zsu.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://zcu.quarkkingdee.top

[R70] 时间戳与互转
来源：http://rmy.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://opj.zhiwuduotai.top

[R71] 日期格式化
来源：http://mkz.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybw.zdqjudy.top

[R72] 等待端口就绪
来源：http://ott.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wyk.snrcjt.cn

[R73] 分割大日志
来源：http://afv.316326.xyz

split -l 1000 big.log part_
来源：http://xkn.kuanghao11.cn

[R74] 批量重命名
来源：http://sye.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bdm.redwolf501.top

[R75] 导出环境变量
来源：http://yvw.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://nxf.yanxiufei.cn

[R76] 使用临时文件
来源：http://bav.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pja.daria6918.cn

[R77] 读取用户输入
来源：http://rsh.fzhhl.top

read -rp "请输入: " ans
来源：http://vpw.mhx1999.top

[R78] 交互式菜单
来源：http://ges.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://afn.nanxinkj.top

[R79] 解析命令行选项
来源：http://lyg.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nyd.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://zmv.sysykeji.top

time ./run.sh
来源：http://sbl.gzhubu.top

================================================================================
来源：http://jhf.jianghu66.top

S. C / C++ 专题
来源：http://bol.sjlbkw.cn

================================================================================
来源：http://nrh.pengpengdd.cyou

[S01] C：Hello World
来源：http://uth.zhoulong.xyz

#include <stdio.h>
来源：http://gcj.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uiw.fktsv.cn

[S02] C：变量与格式化输出
来源：http://sya.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://ull.snrcjt.cn

[S03] C：读入整数
来源：http://txx.hysaishi.cn

int x; scanf("%d", &x);
来源：http://aqn.sysykeji.top

[S04] C：字符串复制
来源：http://yod.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://tjz.svipenyu.cn

[S05] C：字符串长度
来源：http://mga.sweek.top

strlen(s)
来源：http://tow.chenjidiqi.icu

[S06] C：字符串比较
来源：http://lvi.haohaochexian.top

strcmp(a, b) == 0
来源：http://xow.redwolf501.top

[S07] C：数组遍历求和
来源：http://izm.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdu.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://hqn.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://anl.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://ylf.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uwb.yj20258888.top

[S10] C：指针与解引用
来源：http://rob.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://rdn.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://ztc.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://ryz.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jgi.9152youxi.cn

fclose(f);
来源：http://dup.yuanzhike.top

[S12] C：写文件
来源：http://ouz.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ujh.sxryk.cn

[S13] C：宏定义
来源：http://anz.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvu.fehbvm.com

[S14] C：枚举
来源：http://hcx.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://xpy.yanxiufei.cn

[S15] C：类型转换
来源：http://cre.feifeiyinyue.top

(double) a / b
来源：http://hko.meibo888.top

[S16] C：位操作置位
来源：http://zva.cashguo.top

x |= (1 << 3);
来源：http://auu.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://lue.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://huo.chenzaomai.com

[S18] C：命令行参数
来源：http://row.zhijiandao.cn

int main(int argc, char **argv)
来源：http://zpg.9152youxi.cn

[S19] C：快速排序
来源：http://ngz.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ped.quarkkingdee.top

[S20] C：二分查找
来源：http://ebn.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sbe.iojbl.cn

[S21] C：字符类别判断
来源：http://rdh.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hhk.hammf.cn

[S22] C：字符串转数字
来源：http://nxe.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ctq.wangshuangyany.cn

[S23] C：随机数
来源：http://hza.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ugr.jqgufenzy.top

[S24] C：获取本地时间
来源：http://wba.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dkw.meibo888.top

[S25] C：内存拷贝
来源：http://hrt.gaohongyu789.top

memcpy(dst, src, n);
来源：http://hkz.zhongyouzk.top

[S26] C：内存清零
来源：http://bnq.yj20258888.top

memset(a, 0, sizeof a);
来源：http://wtc.hongshengwenyu.top

[S27] C：定义常量
来源：http://lyo.hysaishi.cn

const double PI = 3.14159;
来源：http://cbm.ydzc1.top

[S28] C：静态变量
来源：http://xgw.iojbl.cn

static int counter = 0;
来源：http://qfe.pycfn.com

[S29] C：变参函数
来源：http://iyd.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nkl.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://tii.smart0.xyz

#ifndef X_H
来源：http://kpz.zycfv.cn

#define X_H
来源：http://yzu.yangfankeji.com

#endif
来源：http://ziz.xziqi.cn

[S31] C++：Hello World
来源：http://ujl.shangyingyoupin.top

#include <iostream>
来源：http://mry.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://szb.epnwcf.com

[S32] C++：字符串
来源：http://hhp.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://pgt.xinyue.icu

[S33] C++：vector 增删
来源：http://fcb.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xpn.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://cgu.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://tiv.shangyingyoupin.top

[S35] C++：map
来源：http://rks.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gdb.cucudq.cn

[S36] C++：unordered_map
来源：http://vkt.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwx.sysykeji.top

[S37] C++：set
来源：http://qrj.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xhz.pengpengdd.cyou

[S38] C++：排序
来源：http://iss.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://fle.uphjek.com

[S39] C++：自定义比较器排序
来源：http://rom.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ump.tian-w.cn

[S40] C++：查找元素
来源：http://vyf.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://krt.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://ezr.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dhk.smart0.xyz

[S42] C++：继承与虚函数
来源：http://hzd.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://zda.ehwqpu.com

[S43] C++：智能指针
来源：http://dju.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://aoe.jinqigufen.top

[S44] C++：引用传参
来源：http://evu.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://xed.9152youxi.cn

[S45] C++：lambda
来源：http://byk.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://thg.kuanghao11.cn

[S46] C++：函数模板
来源：http://ydb.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oif.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://bjc.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vnv.hnqzz.top

[S48] C++：逐行读文件
来源：http://wkt.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://shc.fktsv.cn

while (std::getline(in, line)) { }
来源：http://upx.vehdjk.com

[S49] C++：写文件
来源：http://bwo.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ijd.yuanzhike.top

[S50] C++：格式化数字
来源：http://ide.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oom.aibaodan.cn

[S51] C++：显式类型转换
来源：http://osq.quarkkingdee.top

static_cast<double>(a) / b
来源：http://mvk.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://slr.fktsv.cn

int size() const noexcept { return n_; }
来源：http://zws.jinqigufen.top

[S53] C++：移动语义
来源：http://dph.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://ndv.yueranfly.top

[S54] C++：异常处理
来源：http://gex.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mzf.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://kkv.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rht.iojbl.cn

[S56] C++：optional
来源：http://lmo.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rmc.shzxlz.cn

[S57] C++：编译期常量
来源：http://rii.yfazqb.com

constexpr int N = 10;
来源：http://dub.316326.xyz

[S58] C++：命名空间
来源：http://ruo.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://kpg.hammf.cn

[S59] C++：静态断言
来源：http://shg.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nph.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://fpy.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zar.xuanzx.com

================================================================================
来源：http://zhg.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://red.feifeiyinyue.top

================================================================================
来源：http://jxc.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://iib.epnwcf.com

println("Hello")
来源：http://ygt.epnwcf.com

[T02] Kotlin：变量
来源：http://vgl.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgd.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://eyc.zycfv.cn

"值: $b"
来源：http://qhp.ppjwa.cn

[T04] Kotlin：空安全
来源：http://hft.chenzaomai.com

val n: String? = null;  n?.length
来源：http://qfo.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://bta.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aix.bbcook.cn

[T06] Kotlin：集合映射
来源：http://pmm.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hos.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://bri.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgu.hnqzz.top

[T08] Kotlin：数据类
来源：http://lab.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://pno.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://qfi.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://znz.tanke756.top

[T10] Kotlin：默认参数
来源：http://qqt.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mbc.daria6918.cn

[T11] Kotlin：协程
来源：http://elb.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ovd.yueranfly.top

[T12] Kotlin：解构声明
来源：http://auk.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://rgm.meibo888.top

[T13] Kotlin：只读 Map
来源：http://wwt.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://wyr.yvedp.cn

[T14] Kotlin：循环
来源：http://zlp.sxryk.cn

for (i in 1..10) println(i)
来源：http://jbt.zhijiandao.cn

[T15] Kotlin：接口
来源：http://wca.cheryme.top

interface Shape { fun area(): Double }
来源：http://dhe.hywenlv.cn

[T16] Swift：Hello World
来源：http://oet.xuetiantiany.cn

print("Hello")
来源：http://kwi.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://kzf.hnqzz.top

var a = 1;  let b = 2
来源：http://uhv.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://wnz.jyoumei.cn

"值: \(b)"
来源：http://dpp.havefunace.top

[T19] Swift：可选绑定
来源：http://vfw.chenlongwang.top

if let n = opt { print(n) }
来源：http://uwp.yuanzhike.top

[T20] Swift：数组操作
来源：http://jly.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://nkk.shzxlz.cn

[T21] Swift：遍历
来源：http://wmq.sufxvd.cn

for x in a { print(x) }
来源：http://bki.aizwys.cn

[T22] Swift：字典
来源：http://nll.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rgh.wangdashe.top

[T23] Swift：函数
来源：http://oxt.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://syw.zhoulong.xyz

[T24] Swift：闭包
来源：http://rso.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mqp.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://xtz.cheryme.top

struct P { var x: Int }
来源：http://mfr.guannengcc.top

[T26] Swift：类与重写
来源：http://vvn.sufxvd.cn

class A: Base { override func f() {} }
来源：http://yii.andypj.xyz

[T27] Swift：错误处理
来源：http://xib.yj20258.top

do { try f() } catch { print(error) }
来源：http://osp.fzhhl.top

[T28] Swift：枚举
来源：http://qev.havefunace.top

enum Color { case red, green }
来源：http://orv.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://agr.bjfxy.top

guard let x = opt else { return }
来源：http://gse.fengsongda.top

[T30] Swift：协议
来源：http://rtd.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://qrs.c1oappe.top

[T31] Lua：Hello World
来源：http://xhf.hesvh.cn

print("Hello")
来源：http://ztc.sysykeji.top

[T32] Lua：局部变量
来源：http://vld.guowangkeji.top

local a = 1
来源：http://knm.cheryme.top

[T33] Lua：表（数组）
来源：http://rje.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dna.pycfn.com

[T34] Lua：遍历表
来源：http://iqp.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xjl.shuidangran.top

[T35] Lua：字典表
来源：http://sqh.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://nvc.chenzaomai.com

[T36] Lua：函数
来源：http://ewz.dianchejie.cn

function add(a, b) return a + b end
来源：http://jze.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://clz.yongpay.top

"a" .. "b"
来源：http://fuj.birdmap.top

[T38] Lua：条件
来源：http://dou.xziqi.cn

if x > 0 then print("正") end
来源：http://ddf.epnwcf.com

[T39] Lua：模式匹配
来源：http://ksi.jlsjyb.cn

string.find(s, "%d+")
来源：http://fxf.chenlongwang.top

[T40] Lua：元表
来源：http://drz.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://jma.yj20258.top

[T41] Perl：Hello World
来源：http://pyn.gaohongyu789.top

print "Hello\n";
来源：http://iqa.hfpthk.cn

[T42] Perl：变量类型
来源：http://ykt.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzp.fzhhl.top

[T43] Perl：字符串插值
来源：http://ppx.yuanzhike.top

"值: $a"
来源：http://por.zhoulong.xyz

[T44] Perl：条件
来源：http://hho.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://jgm.uphjek.com

[T45] Perl：数组遍历
来源：http://riu.cheryme.top

for my $x (@arr) { print $x; }
来源：http://ptx.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://gja.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fpl.cashguo.top

[T47] Perl：正则捕获
来源：http://elo.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xyv.pycfn.com

[T48] Perl：正则替换
来源：http://gcj.guannengcc.top

$s =~ s/old/new/g;
来源：http://pbo.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://ydb.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hgf.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://ipu.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lyc.fktsv.cn


<!-- 参考信息 -->