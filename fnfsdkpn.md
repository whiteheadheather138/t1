代发 wailian999

find . -name "*.log" -type f
来源：http://pxm.ivvv.top

[R44] 按修改时间查找
来源：http://kly.chenzaomai.com

find . -mtime -7 -type f
来源：http://mhy.fanxiaobao.xyz

[R45] 批量删除
来源：http://xjj.tian-w.cn

find . -name "*.tmp" -delete
来源：http://dlk.chenzaomai.com

[R46] 递归替换文件内容
来源：http://xti.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dem.bbcook.cn

[R47] sed 单行替换
来源：http://ojb.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://lal.cdnleiting.top

[R48] awk 取指定列
来源：http://oqy.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://vcn.ehwqpu.com

[R49] awk 带条件
来源：http://vxo.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hdh.chenzaomai.com

[R50] awk 求和
来源：http://yqu.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://ipy.tianlin.xyz

[R51] 排序去重取前几
来源：http://xcd.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://htc.guannengcc.top

[R52] 统计行数
来源：http://iks.feifeiyinyue.top

wc -l a.txt
来源：http://pns.pycfn.com

[R53] 查看文件头与实时尾
来源：http://xmb.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tof.zhixingplan.top

[R54] 比较两个文件
来源：http://awv.fengsongda.top

diff a.txt b.txt
来源：http://osd.meibo888.top

[R55] 压缩与解压
来源：http://cqi.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rol.hongshengwenyu.top

[R56] 远程拷贝
来源：http://tcm.guannengcc.top

scp file user@host:/path/
来源：http://wff.zhengqikj.top

[R57] 远程执行命令
来源：http://gyk.havefunace.top

ssh user@host 'uptime'
来源：http://png.smart0.xyz

[R58] 下载文件
来源：http://fgt.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wrm.ydzc1.top

[R59] 发 POST JSON
来源：http://kno.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ouk.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://lqz.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://imx.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://bos.xinyue.icu

df -h;  du -sh *
来源：http://lsf.gogol.net.cn

[R62] 找最占空间的文件
来源：http://fqx.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://uyq.hysaishi.cn

[R63] 内存与进程
来源：http://fwu.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://qjf.gogol.net.cn

[R64] 结束进程
来源：http://cqp.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://ajs.ppjwa.cn

[R65] 查看端口占用
来源：http://vtn.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tii.wangdashe.top

[R66] 定时任务
来源：http://wgx.aizwys.cn

crontab -e;  crontab -l
来源：http://ptq.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://ggx.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://igs.hcnkem.com

[R68] 计算文件校验值
来源：http://xny.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gjy.meibo888.top

[R69] 生成随机密码
来源：http://qdb.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://fad.fktsv.cn

[R70] 时间戳与互转
来源：http://bam.yfazqb.com

date +%s;  date -d @1700000000
来源：http://wua.cucudq.cn

[R71] 日期格式化
来源：http://unn.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dez.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://uqd.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ilx.zdqjudy.top

[R73] 分割大日志
来源：http://auo.svipenyu.cn

split -l 1000 big.log part_
来源：http://lup.316326.xyz

[R74] 批量重命名
来源：http://jdm.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bgr.zhijiandao.cn

[R75] 导出环境变量
来源：http://cji.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://sjj.tianlin.xyz

[R76] 使用临时文件
来源：http://upt.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tgn.hysaishi.cn

[R77] 读取用户输入
来源：http://plu.shuidangran.top

read -rp "请输入: " ans
来源：http://xdv.xylfe.cn

[R78] 交互式菜单
来源：http://tka.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cir.xinyue.icu

[R79] 解析命令行选项
来源：http://fkk.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufa.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://bot.iojbl.cn

time ./run.sh
来源：http://ora.hammf.cn

================================================================================
来源：http://sfz.hysaishi.cn

S. C / C++ 专题
来源：http://fux.dianchejie.cn

================================================================================
来源：http://ugf.yonumen.top

[S01] C：Hello World
来源：http://lnx.jinyuanbaomall.cn

#include <stdio.h>
来源：http://lny.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://azg.yj20258888.top

[S02] C：变量与格式化输出
来源：http://but.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://fpl.nanxuanxn.top

[S03] C：读入整数
来源：http://ajn.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://vum.yuanzhike.top

[S04] C：字符串复制
来源：http://tps.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dkx.shuidangran.top

[S05] C：字符串长度
来源：http://wfc.epnwcf.com

strlen(s)
来源：http://pxf.tanke756.top

[S06] C：字符串比较
来源：http://psu.zhongyouzk.top

strcmp(a, b) == 0
来源：http://rdd.fengsongda.top

[S07] C：数组遍历求和
来源：http://lyx.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tfc.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://twh.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vpp.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://vhk.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zsl.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://orr.redwolf501.top

int *p = &a;  *p = 5;
来源：http://pqe.sufxvd.cn

[S11] C：逐行读文件
来源：http://lwo.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://ncp.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://xct.zdqjudy.top

fclose(f);
来源：http://igw.yonumen.top

[S12] C：写文件
来源：http://sbe.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xex.zycfv.cn

[S13] C：宏定义
来源：http://zpw.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dqh.ctjpmb.com

[S14] C：枚举
来源：http://uyy.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://cyv.ivvv.top

[S15] C：类型转换
来源：http://dho.ppjwa.cn

(double) a / b
来源：http://pdd.yj20258.top

[S16] C：位操作置位
来源：http://kqq.mhx1999.top

x |= (1 << 3);
来源：http://mtg.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://ybq.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kta.hfpthk.cn

[S18] C：命令行参数
来源：http://iei.zhoulong.xyz

int main(int argc, char **argv)
来源：http://cwx.zhengqikj.top

[S19] C：快速排序
来源：http://qbe.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://rfo.aizwys.cn

[S20] C：二分查找
来源：http://cpb.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kmp.haohaochexian.top

[S21] C：字符类别判断
来源：http://cgd.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gzg.aizwys.cn

[S22] C：字符串转数字
来源：http://cuw.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://qji.dianchejie.cn

[S23] C：随机数
来源：http://ldj.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qir.aizwys.cn

[S24] C：获取本地时间
来源：http://zyn.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yos.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://rhe.uphjek.com

memcpy(dst, src, n);
来源：http://jpo.zhoulong.xyz

[S26] C：内存清零
来源：http://cgw.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://ghz.vehdjk.com

[S27] C：定义常量
来源：http://bpp.ydzc1.top

const double PI = 3.14159;
来源：http://nqh.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://yir.jinyuanbaomall.cn

static int counter = 0;
来源：http://uqo.zhiwuduotai.top

[S29] C：变参函数
来源：http://tzc.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etf.redwolf501.top

[S30] C：头文件保护
来源：http://wsb.jinghuilouyu.cn

#ifndef X_H
来源：http://beq.dashuyun.cn

#define X_H
来源：http://oiu.shanyushiyangkeji.top

#endif
来源：http://yey.gogol.net.cn

[S31] C++：Hello World
来源：http://sta.zycfv.cn

#include <iostream>
来源：http://tqb.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://qpg.ydjk.org.cn

[S32] C++：字符串
来源：http://tpj.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://mrd.shuidangran.top

[S33] C++：vector 增删
来源：http://wtd.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://avq.yj20258.top

[S34] C++：遍历 vector
来源：http://shb.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://gsq.zhixingplan.top

[S35] C++：map
来源：http://zbz.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://upb.52xcode.cn

[S36] C++：unordered_map
来源：http://kiy.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://obg.316326.xyz

[S37] C++：set
来源：http://cvw.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iqc.tanke756.top

[S38] C++：排序
来源：http://zra.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://mts.cheryme.top

[S39] C++：自定义比较器排序
来源：http://zqc.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pkq.jinqigfzy.top

[S40] C++：查找元素
来源：http://xfw.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ckx.zycfv.cn

[S41] C++：类与构造函数
来源：http://mab.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lev.andypj.xyz

[S42] C++：继承与虚函数
来源：http://ytx.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://xff.uphjek.com

[S43] C++：智能指针
来源：http://wfp.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://pvu.ppjwa.cn

[S44] C++：引用传参
来源：http://mpw.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://cwn.jlsjyb.cn

[S45] C++：lambda
来源：http://oud.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://qeb.meibo888.top

[S46] C++：函数模板
来源：http://ixy.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xih.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://rsk.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kcg.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://yis.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://bes.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://elb.ppjwa.cn

[S49] C++：写文件
来源：http://chf.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://shj.jiagoushi.top

[S50] C++：格式化数字
来源：http://csz.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rnv.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://prt.dianchejie.cn

static_cast<double>(a) / b
来源：http://ogt.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://vmj.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://nii.fengsongda.top

[S53] C++：移动语义
来源：http://xnu.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://zzc.cashguo.top

[S54] C++：异常处理
来源：http://kda.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ear.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://shn.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://czm.ivvv.top

[S56] C++：optional
来源：http://zqx.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ueh.jlsjyb.cn

[S57] C++：编译期常量
来源：http://emm.xziqi.cn

constexpr int N = 10;
来源：http://ocu.yonumen.top

[S58] C++：命名空间
来源：http://psy.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://ima.pycfn.com

[S59] C++：静态断言
来源：http://fwm.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cni.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://cgy.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xgd.zhongyouzk.top

================================================================================
来源：http://mbg.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqg.vqdsnc.cn

================================================================================
来源：http://lnr.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://lqi.zhixingplan.top

println("Hello")
来源：http://bgt.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://yrl.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://frj.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://ibm.zhixingplan.top

"值: $b"
来源：http://gcq.hesvh.cn

[T04] Kotlin：空安全
来源：http://ods.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://srq.yj202588.top

[T05] Kotlin：when 表达式
来源：http://fgj.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rzw.316326.xyz

[T06] Kotlin：集合映射
来源：http://hme.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dbi.yj202588.top

[T07] Kotlin：集合过滤
来源：http://tfc.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fbb.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://aco.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://tyh.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://knt.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://pwv.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://bma.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://omz.pycfn.com

[T11] Kotlin：协程
来源：http://rmh.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uog.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://dfk.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://okx.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://urj.316326.xyz

val m = mapOf("a" to 1)
来源：http://fss.guannengcc.top

[T14] Kotlin：循环
来源：http://ijm.birdmap.top

for (i in 1..10) println(i)
来源：http://ztx.yj20258888.top

[T15] Kotlin：接口
来源：http://knm.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://qtd.yvedp.cn

[T16] Swift：Hello World
来源：http://nrw.jyoumei.cn

print("Hello")
来源：http://ttp.meibo888.top

[T17] Swift：变量与常量
来源：http://bnw.aibaodan.cn

var a = 1;  let b = 2
来源：http://ten.meibo888.top

[T18] Swift：字符串插值
来源：http://fyd.xuetiantiany.cn

"值: \(b)"
来源：http://nbh.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://vva.andypj.xyz

if let n = opt { print(n) }
来源：http://vaz.tanke756.top

[T20] Swift：数组操作
来源：http://zhc.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vsq.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://jqd.bjfxy.top

for x in a { print(x) }
来源：http://lnt.svipenyu.cn

[T22] Swift：字典
来源：http://swc.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://wyx.guowangkeji.top

[T23] Swift：函数
来源：http://kwx.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://agy.snrcjt.cn

[T24] Swift：闭包
来源：http://ent.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hpu.shuidangran.top

[T25] Swift：结构体
来源：http://qzq.xuanzx.com

struct P { var x: Int }
来源：http://ocu.jinqigfzy.top

[T26] Swift：类与重写
来源：http://gge.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://sbs.dashuyun.cn

[T27] Swift：错误处理
来源：http://sgr.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://dvs.tian-w.cn

[T28] Swift：枚举
来源：http://ttk.hnxiangtu.top

enum Color { case red, green }
来源：http://mkb.316326.xyz

[T29] Swift：guard 提前返回
来源：http://nfx.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://jmp.wangshuangyany.cn

[T30] Swift：协议
来源：http://fok.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://xuj.daxiang520.top

[T31] Lua：Hello World
来源：http://fwx.jinqigfzy.top

print("Hello")
来源：http://jca.cdnleiting.top

[T32] Lua：局部变量
来源：http://nul.shzxlz.cn

local a = 1
来源：http://xnk.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://jra.svipenyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wsg.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://oca.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sqa.feifeiyinyue.top

[T35] Lua：字典表
来源：http://vbj.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://lal.sysykeji.top

[T36] Lua：函数
来源：http://msl.yuxming.cn

function add(a, b) return a + b end
来源：http://ecu.andypj.xyz

[T37] Lua：字符串拼接
来源：http://pjr.zycfv.cn

"a" .. "b"
来源：http://ktt.fzhhl.top

[T38] Lua：条件
来源：http://htq.fehbvm.com

if x > 0 then print("正") end
来源：http://vuf.sxryk.cn

[T39] Lua：模式匹配
来源：http://tom.yuxming.cn

string.find(s, "%d+")
来源：http://eem.0kj1m.cn

[T40] Lua：元表
来源：http://tpj.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://qvk.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://hoy.hnxiangtu.top

print "Hello\n";
来源：http://alx.hywenlv.cn

[T42] Perl：变量类型
来源：http://mxx.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://flo.snrcjt.cn

[T43] Perl：字符串插值
来源：http://hhk.yuanzhike.top

"值: $a"
来源：http://isj.uphjek.com

[T44] Perl：条件
来源：http://ouh.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://mki.yonumen.top

[T45] Perl：数组遍历
来源：http://seo.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://ayl.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://ztb.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://alm.52xcode.cn


<!-- 参考信息 -->