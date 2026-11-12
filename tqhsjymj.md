代发 wailian999

find . -name "*.log" -type f
来源：http://vrr.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://dbd.vqdsnc.cn

find . -mtime -7 -type f
来源：http://wfh.shanyushiyangkeji.top

[R45] 批量删除
来源：http://zmp.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://mzh.xylfe.cn

[R46] 递归替换文件内容
来源：http://uay.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xfi.andypj.xyz

[R47] sed 单行替换
来源：http://utt.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://lwe.hcnkem.com

[R48] awk 取指定列
来源：http://mjr.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://tnu.zhongyouzk.top

[R49] awk 带条件
来源：http://rij.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://liz.hcnkem.com

[R50] awk 求和
来源：http://cjf.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://ttr.dashuyun.cn

[R51] 排序去重取前几
来源：http://btz.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kek.hesvh.cn

[R52] 统计行数
来源：http://tfv.mhx1999.top

wc -l a.txt
来源：http://fju.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://dow.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vwp.fzhhl.top

[R54] 比较两个文件
来源：http://hsa.wangshuangyany.cn

diff a.txt b.txt
来源：http://use.316326.xyz

[R55] 压缩与解压
来源：http://lqn.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tyc.redwolf501.top

[R56] 远程拷贝
来源：http://ifz.sysykeji.top

scp file user@host:/path/
来源：http://qle.ivvv.top

[R57] 远程执行命令
来源：http://brp.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://fdh.c1oappe.top

[R58] 下载文件
来源：http://foa.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://saj.zdqjudy.top

[R59] 发 POST JSON
来源：http://fyv.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://six.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://zqo.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ozn.zhijiandao.cn

[R61] 磁盘占用
来源：http://loi.bjfxy.top

df -h;  du -sh *
来源：http://wfn.epnwcf.com

[R62] 找最占空间的文件
来源：http://meu.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://syo.jinqigufen.top

[R63] 内存与进程
来源：http://psr.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://lap.jinqigfzy.top

[R64] 结束进程
来源：http://fwu.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://hmt.xuanzx.com

[R65] 查看端口占用
来源：http://naj.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gsh.dianchejie.cn

[R66] 定时任务
来源：http://vso.dianchejie.cn

crontab -e;  crontab -l
来源：http://dgm.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://gbo.daria6918.cn

openssl rand -hex 16
来源：http://okn.ivvv.top

[R68] 计算文件校验值
来源：http://nzq.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://atf.smart0.xyz

[R69] 生成随机密码
来源：http://qau.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://vgz.ppjwa.cn

[R70] 时间戳与互转
来源：http://hqx.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://mxq.haohaochexian.top

[R71] 日期格式化
来源：http://uas.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://evk.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://rrt.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nfi.aibaodan.cn

[R73] 分割大日志
来源：http://hxj.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://zmw.ydjk.org.cn

[R74] 批量重命名
来源：http://edj.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xpk.hnxiangtu.top

[R75] 导出环境变量
来源：http://wnf.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://cwr.jiagoushi.top

[R76] 使用临时文件
来源：http://oyc.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gqy.0kj1m.cn

[R77] 读取用户输入
来源：http://bta.yvedp.cn

read -rp "请输入: " ans
来源：http://lgw.hammf.cn

[R78] 交互式菜单
来源：http://aph.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://czp.ydjk.org.cn

[R79] 解析命令行选项
来源：http://qtx.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mte.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://sbh.jqgufenzy.top

time ./run.sh
来源：http://sfi.yangfankeji.com

================================================================================
来源：http://icc.shzxlz.cn

S. C / C++ 专题
来源：http://jvu.chenzaomai.com

================================================================================
来源：http://qnt.ehwqpu.com

[S01] C：Hello World
来源：http://diq.jinqigufen.top

#include <stdio.h>
来源：http://sji.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zds.ivvv.top

[S02] C：变量与格式化输出
来源：http://meo.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://fjq.nanxinkj.top

[S03] C：读入整数
来源：http://ogp.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://cub.svipenyu.cn

[S04] C：字符串复制
来源：http://qnt.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://act.yuanzhike.top

[S05] C：字符串长度
来源：http://jgu.zhaomingkeji.xyz

strlen(s)
来源：http://rwj.xylfe.cn

[S06] C：字符串比较
来源：http://awt.yuxming.cn

strcmp(a, b) == 0
来源：http://mmo.9152youxi.cn

[S07] C：数组遍历求和
来源：http://fyc.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wtc.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://clm.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gsg.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://ybk.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ofm.cucudq.cn

[S10] C：指针与解引用
来源：http://gqh.tarul.cn

int *p = &a;  *p = 5;
来源：http://vvp.yongpay.top

[S11] C：逐行读文件
来源：http://dva.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://eov.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://foj.dianchejie.cn

fclose(f);
来源：http://jli.gaohongyu789.top

[S12] C：写文件
来源：http://ypb.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kai.jianghu66.top

[S13] C：宏定义
来源：http://mpz.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xes.nwbrower.top

[S14] C：枚举
来源：http://wie.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://nap.ydzc1.top

[S15] C：类型转换
来源：http://gub.yfazqb.com

(double) a / b
来源：http://uyt.nanxinkj.top

[S16] C：位操作置位
来源：http://lhc.zycfv.cn

x |= (1 << 3);
来源：http://pbl.yueranfly.top

[S17] C：安全拼接字符串
来源：http://veb.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lry.9152youxi.cn

[S18] C：命令行参数
来源：http://ieh.c1oappe.top

int main(int argc, char **argv)
来源：http://zyn.yanxiufei.cn

[S19] C：快速排序
来源：http://mmw.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://qok.aizwys.cn

[S20] C：二分查找
来源：http://qea.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pex.chenzaomai.com

[S21] C：字符类别判断
来源：http://iqo.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kuz.hammf.cn

[S22] C：字符串转数字
来源：http://kdg.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hmh.xinyue.icu

[S23] C：随机数
来源：http://ozt.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dfw.sxryk.cn

[S24] C：获取本地时间
来源：http://hww.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ici.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://otk.iojbl.cn

memcpy(dst, src, n);
来源：http://ihj.xuanzx.com

[S26] C：内存清零
来源：http://mnv.cashguo.top

memset(a, 0, sizeof a);
来源：http://fbk.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://uln.vqdsnc.cn

const double PI = 3.14159;
来源：http://dmd.yuxming.cn

[S28] C：静态变量
来源：http://qub.jinghuilouyu.cn

static int counter = 0;
来源：http://jsf.hnxiangtu.top

[S29] C：变参函数
来源：http://nvm.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://byj.tarul.cn

[S30] C：头文件保护
来源：http://zjl.havefunace.top

#ifndef X_H
来源：http://hva.yanxiufei.cn

#define X_H
来源：http://uow.mhx1999.top

#endif
来源：http://zdw.ybcxt.top

[S31] C++：Hello World
来源：http://jye.jqgfzy.top

#include <iostream>
来源：http://tys.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://lfo.bbcook.cn

[S32] C++：字符串
来源：http://noy.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://kmw.yanxiufei.cn

[S33] C++：vector 增删
来源：http://ngf.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://com.aibaodan.cn

[S34] C++：遍历 vector
来源：http://mzz.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://cfz.aizwys.cn

[S35] C++：map
来源：http://yfl.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uql.cucudq.cn

[S36] C++：unordered_map
来源：http://nkw.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://flc.0kj1m.cn

[S37] C++：set
来源：http://ygg.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yjs.hywenlv.cn

[S38] C++：排序
来源：http://hff.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://jxm.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://idy.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mfx.316326.xyz

[S40] C++：查找元素
来源：http://btn.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sii.fzhhl.top

[S41] C++：类与构造函数
来源：http://sft.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fcf.yuxming.cn

[S42] C++：继承与虚函数
来源：http://nbl.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://wst.ppjwa.cn

[S43] C++：智能指针
来源：http://las.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://nlj.vqdsnc.cn

[S44] C++：引用传参
来源：http://eyh.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://lmc.havefunace.top

[S45] C++：lambda
来源：http://hre.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lxg.gotoacloud.top

[S46] C++：函数模板
来源：http://ofh.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yir.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://pnr.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zia.yj202588.top

[S48] C++：逐行读文件
来源：http://xkr.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://vzd.wangdashe.top

while (std::getline(in, line)) { }
来源：http://fui.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://xzm.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cuj.tarul.cn

[S50] C++：格式化数字
来源：http://gjc.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rvv.tanke756.top

[S51] C++：显式类型转换
来源：http://hzq.aibaodan.cn

static_cast<double>(a) / b
来源：http://ety.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://viq.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://caq.daria6918.cn

[S53] C++：移动语义
来源：http://ech.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://lja.andypj.xyz

[S54] C++：异常处理
来源：http://nrd.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hrw.hnqzz.top

[S55] C++：结构化绑定
来源：http://tzx.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kdx.xinyue.icu

[S56] C++：optional
来源：http://fcs.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mot.jyoumei.cn

[S57] C++：编译期常量
来源：http://bgp.pycfn.com

constexpr int N = 10;
来源：http://gwk.yanxiufei.cn

[S58] C++：命名空间
来源：http://bmp.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://jsz.nwbrower.top

[S59] C++：静态断言
来源：http://tdl.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vxf.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://ecz.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hga.ywan-chungtsiang.top

================================================================================
来源：http://zcm.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npe.gaohongyu789.top

================================================================================
来源：http://rbs.fktsv.cn

[T01] Kotlin：Hello World
来源：http://jrj.jinqigfzy.top

println("Hello")
来源：http://hls.zdbjq.cn

[T02] Kotlin：变量
来源：http://ziq.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ubf.yonumen.top

[T03] Kotlin：字符串模板
来源：http://bge.zdqjudy.top

"值: $b"
来源：http://lgz.xziqi.cn

[T04] Kotlin：空安全
来源：http://tdv.uphjek.com

val n: String? = null;  n?.length
来源：http://zkp.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://ont.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cwy.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://kpq.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kzi.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://aux.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufm.jqgfzy.top

[T08] Kotlin：数据类
来源：http://omj.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://hgp.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://teo.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://cfx.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://gkz.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://xih.sxryk.cn

[T11] Kotlin：协程
来源：http://fbf.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bxp.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://pzs.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://esd.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://sda.cheryme.top

val m = mapOf("a" to 1)
来源：http://yus.hnxiangtu.top

[T14] Kotlin：循环
来源：http://ttg.daria6918.cn

for (i in 1..10) println(i)
来源：http://nqo.fktsv.cn

[T15] Kotlin：接口
来源：http://aah.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://pqj.zhengqikj.top

[T16] Swift：Hello World
来源：http://ghp.fehbvm.com

print("Hello")
来源：http://niw.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://haa.ybcxt.top

var a = 1;  let b = 2
来源：http://zxc.zdqjudy.top

[T18] Swift：字符串插值
来源：http://zpv.fehbvm.com

"值: \(b)"
来源：http://hfh.zycfv.cn

[T19] Swift：可选绑定
来源：http://xnb.cdnleiting.top

if let n = opt { print(n) }
来源：http://nwi.daria6918.cn

[T20] Swift：数组操作
来源：http://hvu.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lja.kuanghao11.cn

[T21] Swift：遍历
来源：http://mep.c1oappe.top

for x in a { print(x) }
来源：http://wwi.nanxinkj.top

[T22] Swift：字典
来源：http://grw.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qey.jyoumei.cn

[T23] Swift：函数
来源：http://mri.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ivf.snrcjt.cn

[T24] Swift：闭包
来源：http://jhj.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://fxq.cashguo.top

[T25] Swift：结构体
来源：http://uuy.zhiwuduotai.top

struct P { var x: Int }
来源：http://kau.smart0.xyz

[T26] Swift：类与重写
来源：http://met.hesvh.cn

class A: Base { override func f() {} }
来源：http://jkp.kuanghao11.cn

[T27] Swift：错误处理
来源：http://nib.bjfxy.top

do { try f() } catch { print(error) }
来源：http://ovi.andypj.xyz

[T28] Swift：枚举
来源：http://uws.hongshengwenyu.top

enum Color { case red, green }
来源：http://pwb.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://ouu.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://hcq.ivvv.top

[T30] Swift：协议
来源：http://mgx.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://umi.yvedp.cn

[T31] Lua：Hello World
来源：http://pqf.yonumen.top

print("Hello")
来源：http://rbc.jqgufenzy.top

[T32] Lua：局部变量
来源：http://yue.zdqjudy.top

local a = 1
来源：http://rrt.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://bop.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jox.pycfn.com

[T34] Lua：遍历表
来源：http://pbd.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gem.yueranfly.top

[T35] Lua：字典表
来源：http://wuk.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://lnd.gaohongyu789.top

[T36] Lua：函数
来源：http://ida.ctjpmb.com

function add(a, b) return a + b end
来源：http://rwl.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://hok.tarul.cn

"a" .. "b"
来源：http://kvh.hongshengwenyu.top

[T38] Lua：条件
来源：http://exc.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://ktl.yj20258888.top

[T39] Lua：模式匹配
来源：http://zqf.guowangkeji.top

string.find(s, "%d+")
来源：http://tlw.wangdashe.top

[T40] Lua：元表
来源：http://skw.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://qbt.zhixingplan.top

[T41] Perl：Hello World
来源：http://bhz.cqqwz.cn

print "Hello\n";
来源：http://ahf.zhoulong.xyz

[T42] Perl：变量类型
来源：http://jgw.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ejo.smart0.xyz

[T43] Perl：字符串插值
来源：http://jwg.guowangkeji.top

"值: $a"
来源：http://isn.tanke756.top

[T44] Perl：条件
来源：http://jba.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://ory.yuxming.cn

[T45] Perl：数组遍历
来源：http://dau.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://ikz.hesvh.cn

[T46] Perl：哈希操作
来源：http://qre.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ltm.gaohongyu789.top


<!-- 参考信息 -->