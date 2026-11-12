代发 wailian999

find . -name "*.tmp" -delete
来源：http://onm.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://kjk.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://inq.sxryk.cn

[R47] sed 单行替换
来源：http://yfc.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://wph.sysykeji.top

[R48] awk 取指定列
来源：http://xva.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://dnn.52xcode.cn

[R49] awk 带条件
来源：http://egw.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pdk.dashuyun.cn

[R50] awk 求和
来源：http://khf.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://ajg.zhijiandao.cn

[R51] 排序去重取前几
来源：http://ufn.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mvu.bjfxy.top

[R52] 统计行数
来源：http://bsl.ehwqpu.com

wc -l a.txt
来源：http://kry.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://akb.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xgh.vehdjk.com

[R54] 比较两个文件
来源：http://xid.wangdashe.top

diff a.txt b.txt
来源：http://hmn.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://sdc.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idr.havefunace.top

[R56] 远程拷贝
来源：http://wjc.sufxvd.cn

scp file user@host:/path/
来源：http://hwy.snrcjt.cn

[R57] 远程执行命令
来源：http://xbo.dianchejie.cn

ssh user@host 'uptime'
来源：http://hjp.aibaodan.cn

[R58] 下载文件
来源：http://svt.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hms.nanxinkj.top

[R59] 发 POST JSON
来源：http://gpg.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lno.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://vqm.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oaq.hfpthk.cn

[R61] 磁盘占用
来源：http://hqi.zhixingplan.top

df -h;  du -sh *
来源：http://dqk.iojbl.cn

[R62] 找最占空间的文件
来源：http://rnd.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://jxc.jianghu66.top

[R63] 内存与进程
来源：http://qwp.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://sxb.zdqjudy.top

[R64] 结束进程
来源：http://ghn.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://rtc.ydzc1.top

[R65] 查看端口占用
来源：http://kqk.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rme.gaohongyu789.top

[R66] 定时任务
来源：http://avy.yuxming.cn

crontab -e;  crontab -l
来源：http://wkp.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://kro.jinghuilouyu.cn

openssl rand -hex 16
来源：http://mdw.zhixingplan.top

[R68] 计算文件校验值
来源：http://ejw.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://bpz.zdqjudy.top

[R69] 生成随机密码
来源：http://kkz.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://yeu.quarkkingdee.top

[R70] 时间戳与互转
来源：http://wmq.yj20258888.top

date +%s;  date -d @1700000000
来源：http://ekg.cheryme.top

[R71] 日期格式化
来源：http://fli.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wag.fktsv.cn

[R72] 等待端口就绪
来源：http://yvo.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gik.cqqwz.cn

[R73] 分割大日志
来源：http://bcw.haohaochexian.top

split -l 1000 big.log part_
来源：http://alj.snrcjt.cn

[R74] 批量重命名
来源：http://ygm.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ezi.hnxiangtu.top

[R75] 导出环境变量
来源：http://duy.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://jpa.shzxlz.cn

[R76] 使用临时文件
来源：http://pwz.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://taw.svipenyu.cn

[R77] 读取用户输入
来源：http://ofo.ydzc1.top

read -rp "请输入: " ans
来源：http://nrx.nwbrower.top

[R78] 交互式菜单
来源：http://lxl.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tbe.havefunace.top

[R79] 解析命令行选项
来源：http://qfv.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qux.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://alw.hysaishi.cn

time ./run.sh
来源：http://qkj.cashguo.top

================================================================================
来源：http://adh.yj20258888.top

S. C / C++ 专题
来源：http://ged.daria6918.cn

================================================================================
来源：http://hfe.dashuyun.cn

[S01] C：Hello World
来源：http://aek.zycfv.cn

#include <stdio.h>
来源：http://qis.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rgw.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://uge.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://odi.fktsv.cn

[S03] C：读入整数
来源：http://sem.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://mgj.shangyingyoupin.top

[S04] C：字符串复制
来源：http://ksc.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://wxx.yuanzhike.top

[S05] C：字符串长度
来源：http://spw.tanke756.top

strlen(s)
来源：http://fcn.smart0.xyz

[S06] C：字符串比较
来源：http://eto.yuxming.cn

strcmp(a, b) == 0
来源：http://gky.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://axa.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ade.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://pry.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://csg.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://ssh.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://boa.kuanghao11.cn

[S10] C：指针与解引用
来源：http://imy.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://wel.316326.xyz

[S11] C：逐行读文件
来源：http://ihj.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://pwr.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qoh.c1oappe.top

fclose(f);
来源：http://yqe.cqqwz.cn

[S12] C：写文件
来源：http://zcv.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://inp.jinqigufen.top

[S13] C：宏定义
来源：http://fda.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wnh.gzhubu.top

[S14] C：枚举
来源：http://tgm.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://bbh.ivvv.top

[S15] C：类型转换
来源：http://euo.aizwys.cn

(double) a / b
来源：http://pjy.ivvv.top

[S16] C：位操作置位
来源：http://cwy.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://bwb.ivvv.top

[S17] C：安全拼接字符串
来源：http://blk.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ily.hongshengwenyu.top

[S18] C：命令行参数
来源：http://nxd.hnqzz.top

int main(int argc, char **argv)
来源：http://ftk.fktsv.cn

[S19] C：快速排序
来源：http://nmf.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fsy.316326.xyz

[S20] C：二分查找
来源：http://skr.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gmc.wangdashe.top

[S21] C：字符类别判断
来源：http://yvz.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfy.dashuyun.cn

[S22] C：字符串转数字
来源：http://mvb.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://jwb.andypj.xyz

[S23] C：随机数
来源：http://vlc.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://boi.xinyue.icu

[S24] C：获取本地时间
来源：http://fky.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yem.ivvv.top

[S25] C：内存拷贝
来源：http://qpf.guannengcc.top

memcpy(dst, src, n);
来源：http://eli.aizwys.cn

[S26] C：内存清零
来源：http://dxy.fengsongda.top

memset(a, 0, sizeof a);
来源：http://lqq.hongshengwenyu.top

[S27] C：定义常量
来源：http://auc.aibaodan.cn

const double PI = 3.14159;
来源：http://lds.sweek.top

[S28] C：静态变量
来源：http://fvs.jqgfzy.top

static int counter = 0;
来源：http://fku.nanxuanxn.top

[S29] C：变参函数
来源：http://chi.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thn.yongpay.top

[S30] C：头文件保护
来源：http://ucc.ybcxt.top

#ifndef X_H
来源：http://srq.ydzc1.top

#define X_H
来源：http://tra.feifeiyinyue.top

#endif
来源：http://zjf.fehbvm.com

[S31] C++：Hello World
来源：http://vhe.316326.xyz

#include <iostream>
来源：http://fdv.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://xtp.meibo888.top

[S32] C++：字符串
来源：http://ifh.yonumen.top

std::string s = "hi";  s += "!";
来源：http://zkl.chenzaomai.com

[S33] C++：vector 增删
来源：http://lwn.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jrg.aibaodan.cn

[S34] C++：遍历 vector
来源：http://fan.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://cpq.jinyuanbaomall.cn

[S35] C++：map
来源：http://bdy.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kvz.gotoacloud.top

[S36] C++：unordered_map
来源：http://jzh.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gae.svipenyu.cn

[S37] C++：set
来源：http://uxa.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lxa.sxryk.cn

[S38] C++：排序
来源：http://cri.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://fuf.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://mjo.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vik.aizwys.cn

[S40] C++：查找元素
来源：http://mjn.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fmy.smart0.xyz

[S41] C++：类与构造函数
来源：http://zsj.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lnk.fktsv.cn

[S42] C++：继承与虚函数
来源：http://dkz.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://utl.ctjpmb.com

[S43] C++：智能指针
来源：http://mio.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://gec.jyoumei.cn

[S44] C++：引用传参
来源：http://jhn.ivvv.top

void inc(int &x) { ++x; }
来源：http://djw.cqqwz.cn

[S45] C++：lambda
来源：http://mxl.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://iwg.daxiang520.top

[S46] C++：函数模板
来源：http://wys.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ava.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://akd.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rgo.yj20258888.top

[S48] C++：逐行读文件
来源：http://bzu.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eww.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://zwj.sxryk.cn

[S49] C++：写文件
来源：http://eyf.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jmi.gotoacloud.top

[S50] C++：格式化数字
来源：http://bgg.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tfo.aibaodan.cn

[S51] C++：显式类型转换
来源：http://jwp.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://xao.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://yir.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://tje.yuanzhike.top

[S53] C++：移动语义
来源：http://rnt.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://uji.chenzaomai.com

[S54] C++：异常处理
来源：http://bgv.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kry.sxryk.cn

[S55] C++：结构化绑定
来源：http://jlr.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://all.birdmap.top

[S56] C++：optional
来源：http://jzt.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oqe.tian-w.cn

[S57] C++：编译期常量
来源：http://jmi.vehdjk.com

constexpr int N = 10;
来源：http://qgs.daxiang520.top

[S58] C++：命名空间
来源：http://nib.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://dil.guowangkeji.top

[S59] C++：静态断言
来源：http://rfz.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aub.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://ieo.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://idl.hcnkem.com

================================================================================
来源：http://xci.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cnh.gogol.net.cn

================================================================================
来源：http://utg.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://xia.jinqigufen.top

println("Hello")
来源：http://ioq.nwbrower.top

[T02] Kotlin：变量
来源：http://zbr.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bqa.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://egb.gzhubu.top

"值: $b"
来源：http://fxu.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://ygh.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://nqt.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://thh.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yrj.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://aqd.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ous.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://swz.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufo.hnqzz.top

[T08] Kotlin：数据类
来源：http://oxz.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://ixu.meibo888.top

[T09] Kotlin：扩展函数
来源：http://ehb.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://jwq.hammf.cn

[T10] Kotlin：默认参数
来源：http://ifl.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://omr.nanxuanxn.top

[T11] Kotlin：协程
来源：http://mlj.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bja.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://hgq.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://mlc.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://vmb.xuanzx.com

val m = mapOf("a" to 1)
来源：http://bbh.cucudq.cn

[T14] Kotlin：循环
来源：http://wtw.birdmap.top

for (i in 1..10) println(i)
来源：http://inm.nwbrower.top

[T15] Kotlin：接口
来源：http://qdy.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://llp.kuanghao11.cn

[T16] Swift：Hello World
来源：http://igq.52xcode.cn

print("Hello")
来源：http://ftp.316326.xyz

[T17] Swift：变量与常量
来源：http://vyj.birdmap.top

var a = 1;  let b = 2
来源：http://ris.bbcook.cn

[T18] Swift：字符串插值
来源：http://wnh.jianghu66.top

"值: \(b)"
来源：http://ihu.jqgfzy.top

[T19] Swift：可选绑定
来源：http://sif.jqgfzy.top

if let n = opt { print(n) }
来源：http://crq.jiagoushi.top

[T20] Swift：数组操作
来源：http://fsr.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xyk.ppjwa.cn

[T21] Swift：遍历
来源：http://lkv.yongpay.top

for x in a { print(x) }
来源：http://eqo.hammf.cn

[T22] Swift：字典
来源：http://yct.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fsz.gzhubu.top

[T23] Swift：函数
来源：http://tsa.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mad.ydzc1.top

[T24] Swift：闭包
来源：http://kln.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://mrc.zhoulong.xyz

[T25] Swift：结构体
来源：http://uja.cheryme.top

struct P { var x: Int }
来源：http://rrs.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://usn.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://pyx.guannengcc.top

[T27] Swift：错误处理
来源：http://bpu.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://ueb.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://asu.tianlin.xyz

enum Color { case red, green }
来源：http://hru.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://dyd.sysykeji.top

guard let x = opt else { return }
来源：http://qpk.dianchejie.cn

[T30] Swift：协议
来源：http://nii.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://kpx.hywenlv.cn

[T31] Lua：Hello World
来源：http://eat.hysaishi.cn

print("Hello")
来源：http://vgi.xziqi.cn

[T32] Lua：局部变量
来源：http://wtx.ydjk.org.cn

local a = 1
来源：http://vgc.hesvh.cn

[T33] Lua：表（数组）
来源：http://wva.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lvr.jinqigufen.top

[T34] Lua：遍历表
来源：http://kyn.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qln.zdbjq.cn

[T35] Lua：字典表
来源：http://zal.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://knf.hnxiangtu.top

[T36] Lua：函数
来源：http://bsv.jianghu66.top

function add(a, b) return a + b end
来源：http://uaj.andypj.xyz

[T37] Lua：字符串拼接
来源：http://mvd.havefunace.top

"a" .. "b"
来源：http://dls.zdbjq.cn

[T38] Lua：条件
来源：http://qqv.cucudq.cn

if x > 0 then print("正") end
来源：http://yby.ppjwa.cn

[T39] Lua：模式匹配
来源：http://rrz.ivvv.top

string.find(s, "%d+")
来源：http://ptn.sjlbkw.cn

[T40] Lua：元表
来源：http://qcj.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://mvx.tian-w.cn

[T41] Perl：Hello World
来源：http://cae.wangdashe.top

print "Hello\n";
来源：http://plp.meibo888.top

[T42] Perl：变量类型
来源：http://wgu.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vlb.ppjwa.cn

[T43] Perl：字符串插值
来源：http://tfc.yueranfly.top

"值: $a"
来源：http://bow.zdbjq.cn

[T44] Perl：条件
来源：http://ieo.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://yid.hywenlv.cn

[T45] Perl：数组遍历
来源：http://dlh.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://mai.jianghu66.top

[T46] Perl：哈希操作
来源：http://xfp.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zwt.yangfankeji.com

[T47] Perl：正则捕获
来源：http://pgo.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pdd.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://suv.chenlongwang.top

$s =~ s/old/new/g;
来源：http://bzw.shuidangran.top


<!-- 参考信息 -->