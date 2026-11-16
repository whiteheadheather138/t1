代发 wailian999

find . -name "*.tmp" -delete
来源：http://int.chenzaomai.com

[R46] 递归替换文件内容
来源：http://cgu.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hra.daria6918.cn

[R47] sed 单行替换
来源：http://pjd.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ddf.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://lak.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://ptr.yangfankeji.com

[R49] awk 带条件
来源：http://wqi.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ifw.feifeiyinyue.top

[R50] awk 求和
来源：http://oym.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oig.yj20258.top

[R51] 排序去重取前几
来源：http://tem.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dzs.zhiwuduotai.top

[R52] 统计行数
来源：http://bvg.gzhubu.top

wc -l a.txt
来源：http://uie.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://mam.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cho.fzhhl.top

[R54] 比较两个文件
来源：http://nde.wangshuangyany.cn

diff a.txt b.txt
来源：http://eyg.aizwys.cn

[R55] 压缩与解压
来源：http://ylf.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jrv.cashguo.top

[R56] 远程拷贝
来源：http://voc.pycfn.com

scp file user@host:/path/
来源：http://yry.ctjpmb.com

[R57] 远程执行命令
来源：http://rnj.cheryme.top

ssh user@host 'uptime'
来源：http://jzs.zhengqikj.top

[R58] 下载文件
来源：http://cyo.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zwm.shzxlz.cn

[R59] 发 POST JSON
来源：http://jmd.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vew.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://wvj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yrh.aibaodan.cn

[R61] 磁盘占用
来源：http://umq.shuidangran.top

df -h;  du -sh *
来源：http://gjh.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://box.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://hhc.aizwys.cn

[R63] 内存与进程
来源：http://rwp.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://tqx.shanyushiyangkeji.top

[R64] 结束进程
来源：http://cuf.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://bcu.cashguo.top

[R65] 查看端口占用
来源：http://eba.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vnw.shanyushiyangkeji.top

[R66] 定时任务
来源：http://mxb.ppjwa.cn

crontab -e;  crontab -l
来源：http://rpi.fzhhl.top

[R67] 生成随机十六进制串
来源：http://uxo.jlsjyb.cn

openssl rand -hex 16
来源：http://xbv.yongpay.top

[R68] 计算文件校验值
来源：http://ido.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bvz.gotoacloud.top

[R69] 生成随机密码
来源：http://rwc.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://yno.fengsongda.top

[R70] 时间戳与互转
来源：http://gci.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://zvo.shzxlz.cn

[R71] 日期格式化
来源：http://gcw.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kxc.pycfn.com

[R72] 等待端口就绪
来源：http://zoj.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jxx.pengpengdd.cyou

[R73] 分割大日志
来源：http://pos.hnqzz.top

split -l 1000 big.log part_
来源：http://anj.hnqzz.top

[R74] 批量重命名
来源：http://ign.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zmw.andypj.xyz

[R75] 导出环境变量
来源：http://qjv.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://ebj.jqgfzy.top

[R76] 使用临时文件
来源：http://rvz.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://smj.jlsjyb.cn

[R77] 读取用户输入
来源：http://kxm.yvedp.cn

read -rp "请输入: " ans
来源：http://lyg.xuanzx.com

[R78] 交互式菜单
来源：http://ryy.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oqw.mhx1999.top

[R79] 解析命令行选项
来源：http://rdo.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hlz.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://prt.jinyuanbaomall.cn

time ./run.sh
来源：http://lht.birdmap.top

================================================================================
来源：http://zer.chenzaomai.com

S. C / C++ 专题
来源：http://bvm.jyoumei.cn

================================================================================
来源：http://kfj.fzhhl.top

[S01] C：Hello World
来源：http://uub.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://txg.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jgf.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://xps.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://fxi.yfazqb.com

[S03] C：读入整数
来源：http://kgw.cdnleiting.top

int x; scanf("%d", &x);
来源：http://tny.cucudq.cn

[S04] C：字符串复制
来源：http://vwb.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://ytl.vehdjk.com

[S05] C：字符串长度
来源：http://qon.uphjek.com

strlen(s)
来源：http://qqc.9152youxi.cn

[S06] C：字符串比较
来源：http://xki.zhoulong.xyz

strcmp(a, b) == 0
来源：http://msc.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://cea.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bpb.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://gux.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jbf.uphjek.com

[S09] C：结构体定义与初始化
来源：http://qvz.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wyk.cashguo.top

[S10] C：指针与解引用
来源：http://mkj.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://ieh.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://dyr.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://koh.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mdg.fktsv.cn

fclose(f);
来源：http://qht.sufxvd.cn

[S12] C：写文件
来源：http://nck.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://awx.shanyushiyangtech.top

[S13] C：宏定义
来源：http://iel.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ste.bbcook.cn

[S14] C：枚举
来源：http://jph.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://brn.tarul.cn

[S15] C：类型转换
来源：http://wpf.xingfuxueyuan.xyz

(double) a / b
来源：http://rmx.zhixingplan.top

[S16] C：位操作置位
来源：http://zwr.nanxinkj.top

x |= (1 << 3);
来源：http://nag.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://wrx.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lus.redwolf501.top

[S18] C：命令行参数
来源：http://ubn.epnwcf.com

int main(int argc, char **argv)
来源：http://zea.jinghuilouyu.cn

[S19] C：快速排序
来源：http://qid.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://kqx.cheryme.top

[S20] C：二分查找
来源：http://ptg.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bse.hfpthk.cn

[S21] C：字符类别判断
来源：http://qrc.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oli.daxiang520.top

[S22] C：字符串转数字
来源：http://lop.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vey.tanke756.top

[S23] C：随机数
来源：http://zeb.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://omi.ivvv.top

[S24] C：获取本地时间
来源：http://bmo.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xnh.xylfe.cn

[S25] C：内存拷贝
来源：http://xpd.tian-w.cn

memcpy(dst, src, n);
来源：http://dow.hnxiangtu.top

[S26] C：内存清零
来源：http://tvx.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://voh.feifeiyinyue.top

[S27] C：定义常量
来源：http://kvm.chenzaomai.com

const double PI = 3.14159;
来源：http://izx.ybcxt.top

[S28] C：静态变量
来源：http://cxt.aizwys.cn

static int counter = 0;
来源：http://bdf.ctjpmb.com

[S29] C：变参函数
来源：http://kxa.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxg.9152youxi.cn

[S30] C：头文件保护
来源：http://vbv.hongshengwenyu.top

#ifndef X_H
来源：http://hjo.yangfankeji.com

#define X_H
来源：http://iao.uphjek.com

#endif
来源：http://nqq.yueranfly.top

[S31] C++：Hello World
来源：http://hxd.hfpthk.cn

#include <iostream>
来源：http://vri.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://rcy.yanxiufei.cn

[S32] C++：字符串
来源：http://vvo.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://iqt.ydzc1.top

[S33] C++：vector 增删
来源：http://rfn.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mns.xinyue.icu

[S34] C++：遍历 vector
来源：http://qog.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://yky.jinyuanbaomall.cn

[S35] C++：map
来源：http://xzp.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zbv.snrcjt.cn

[S36] C++：unordered_map
来源：http://khx.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ftn.hongshengwenyu.top

[S37] C++：set
来源：http://dqk.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nbd.ppjwa.cn

[S38] C++：排序
来源：http://zfs.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://ifm.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://kdt.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vmv.xziqi.cn

[S40] C++：查找元素
来源：http://wev.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hrp.yueranfly.top

[S41] C++：类与构造函数
来源：http://aru.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pby.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://rcy.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://ste.chenjidiqi.icu

[S43] C++：智能指针
来源：http://cao.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://jqw.sxryk.cn

[S44] C++：引用传参
来源：http://vtu.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://xnk.shangyingyoupin.top

[S45] C++：lambda
来源：http://iss.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://nwe.yuanzhike.top

[S46] C++：函数模板
来源：http://anm.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vei.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://mfr.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hjz.cqqwz.cn

[S48] C++：逐行读文件
来源：http://xjb.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pmp.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://pih.yuanzhike.top

[S49] C++：写文件
来源：http://tbo.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wvn.aizwys.cn

[S50] C++：格式化数字
来源：http://kkr.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qwu.aibaodan.cn

[S51] C++：显式类型转换
来源：http://lap.pycfn.com

static_cast<double>(a) / b
来源：http://ofp.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://rrf.havefunace.top

int size() const noexcept { return n_; }
来源：http://fdw.xziqi.cn

[S53] C++：移动语义
来源：http://uwx.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://spu.gzhubu.top

[S54] C++：异常处理
来源：http://qnr.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yrm.haohaochexian.top

[S55] C++：结构化绑定
来源：http://dhm.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jlo.ppjwa.cn

[S56] C++：optional
来源：http://pjt.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://avy.cdnleiting.top

[S57] C++：编译期常量
来源：http://qeh.52xcode.cn

constexpr int N = 10;
来源：http://yqn.zdbjq.cn

[S58] C++：命名空间
来源：http://cye.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://wzq.guowangkeji.top

[S59] C++：静态断言
来源：http://wiq.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sfi.havefunace.top

[S60] C++：遍历并删除元素
来源：http://pbv.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sfc.shzxlz.cn

================================================================================
来源：http://syq.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ris.gogol.net.cn

================================================================================
来源：http://pcc.yj20258888.top

[T01] Kotlin：Hello World
来源：http://pok.xylfe.cn

println("Hello")
来源：http://uil.shuidangran.top

[T02] Kotlin：变量
来源：http://yes.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yif.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://vrp.bbcook.cn

"值: $b"
来源：http://gio.sxryk.cn

[T04] Kotlin：空安全
来源：http://gnn.redwolf501.top

val n: String? = null;  n?.length
来源：http://fwk.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://lkz.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://adh.cheryme.top

[T06] Kotlin：集合映射
来源：http://mrs.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rdf.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://qtp.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fyf.yj202588.top

[T08] Kotlin：数据类
来源：http://lrs.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://hcj.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://xwe.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://fhp.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://gbl.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://mxt.bjfxy.top

[T11] Kotlin：协程
来源：http://ooa.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vyz.c1oappe.top

[T12] Kotlin：解构声明
来源：http://sbs.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://jzb.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://gwo.yj20258888.top

val m = mapOf("a" to 1)
来源：http://plz.zhijiandao.cn

[T14] Kotlin：循环
来源：http://dhh.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://llp.cucudq.cn

[T15] Kotlin：接口
来源：http://jla.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://cyl.yuxming.cn

[T16] Swift：Hello World
来源：http://bph.bbcook.cn

print("Hello")
来源：http://ppu.bjfxy.top

[T17] Swift：变量与常量
来源：http://yoa.tarul.cn

var a = 1;  let b = 2
来源：http://aqb.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://nts.yangfankeji.com

"值: \(b)"
来源：http://fzc.aizwys.cn

[T19] Swift：可选绑定
来源：http://wvi.fengsongda.top

if let n = opt { print(n) }
来源：http://myz.nanxinkj.top

[T20] Swift：数组操作
来源：http://bst.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jpd.shuidangran.top

[T21] Swift：遍历
来源：http://mbi.zhiwuduotai.top

for x in a { print(x) }
来源：http://eoc.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://ten.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://unf.zhiwuduotai.top

[T23] Swift：函数
来源：http://fme.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xrd.cashguo.top

[T24] Swift：闭包
来源：http://aiz.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yec.yangfankeji.com

[T25] Swift：结构体
来源：http://xtg.fanxiaobao.xyz

struct P { var x: Int }
来源：http://fps.zdqjudy.top

[T26] Swift：类与重写
来源：http://buq.0kj1m.cn

class A: Base { override func f() {} }
来源：http://dbp.sufxvd.cn

[T27] Swift：错误处理
来源：http://fjo.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://qxx.hfpthk.cn

[T28] Swift：枚举
来源：http://wnd.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://tvp.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://znz.gogol.net.cn

guard let x = opt else { return }
来源：http://fzy.zdqjudy.top

[T30] Swift：协议
来源：http://gjw.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://rlj.yanxiufei.cn

[T31] Lua：Hello World
来源：http://cgk.ppjwa.cn

print("Hello")
来源：http://vri.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://mop.bbcook.cn

local a = 1
来源：http://qlv.meibo888.top

[T33] Lua：表（数组）
来源：http://hkk.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ctl.nanxinkj.top

[T34] Lua：遍历表
来源：http://sla.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vas.nanxuanxn.top

[T35] Lua：字典表
来源：http://sdf.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://ftj.hnxiangtu.top

[T36] Lua：函数
来源：http://lmh.fzhhl.top

function add(a, b) return a + b end
来源：http://zjf.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://jub.xylfe.cn

"a" .. "b"
来源：http://pjw.yuxming.cn

[T38] Lua：条件
来源：http://tdp.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://dks.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://xju.chenlongwang.top

string.find(s, "%d+")
来源：http://vah.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://ljf.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://kjd.hnqzz.top

[T41] Perl：Hello World
来源：http://inl.zhijiandao.cn

print "Hello\n";
来源：http://xia.smart0.xyz

[T42] Perl：变量类型
来源：http://ejc.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ajj.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://mfd.c1oappe.top

"值: $a"
来源：http://xca.yuxming.cn

[T44] Perl：条件
来源：http://bbp.sweek.top

if ($a > 0) { print "正"; }
来源：http://akn.dashuyun.cn

[T45] Perl：数组遍历
来源：http://vzu.316326.xyz

for my $x (@arr) { print $x; }
来源：http://rst.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://cxw.cqqwz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://etg.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://abo.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pyb.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://fuv.cdnleiting.top

$s =~ s/old/new/g;
来源：http://yli.xuetiantiany.cn


<!-- 参考信息 -->