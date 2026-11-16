代发 wailian999

find . -name "*.tmp" -delete
来源：http://qbs.redwolf501.top

[R46] 递归替换文件内容
来源：http://rad.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ayv.jyoumei.cn

[R47] sed 单行替换
来源：http://hpq.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://vtd.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://qev.ydzc1.top

awk '{print $1, $3}' a.txt
来源：http://iyq.meibo888.top

[R49] awk 带条件
来源：http://eil.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ppt.yuanzhike.top

[R50] awk 求和
来源：http://jll.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://dib.gogol.net.cn

[R51] 排序去重取前几
来源：http://auk.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cyz.yj20258888.top

[R52] 统计行数
来源：http://rww.nwbrower.top

wc -l a.txt
来源：http://bst.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://qsw.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hov.yangfankeji.com

[R54] 比较两个文件
来源：http://mwd.iojbl.cn

diff a.txt b.txt
来源：http://vfk.sysykeji.top

[R55] 压缩与解压
来源：http://ljv.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lzq.fengsongda.top

[R56] 远程拷贝
来源：http://mji.wangshuangyany.cn

scp file user@host:/path/
来源：http://tjq.yuanzhike.top

[R57] 远程执行命令
来源：http://cli.ehwqpu.com

ssh user@host 'uptime'
来源：http://juq.haohaochexian.top

[R58] 下载文件
来源：http://dsr.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yls.andypj.xyz

[R59] 发 POST JSON
来源：http://cmo.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fco.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://inp.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cuu.sufxvd.cn

[R61] 磁盘占用
来源：http://ikd.gzhubu.top

df -h;  du -sh *
来源：http://fjr.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://pgk.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://yfi.fengsongda.top

[R63] 内存与进程
来源：http://bwc.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://zsi.ydjk.org.cn

[R64] 结束进程
来源：http://poc.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://cui.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://yog.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bdc.birdmap.top

[R66] 定时任务
来源：http://onl.gotoacloud.top

crontab -e;  crontab -l
来源：http://pim.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://lqy.gaohongyu789.top

openssl rand -hex 16
来源：http://zpb.bbcook.cn

[R68] 计算文件校验值
来源：http://mvj.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://qdp.ydzc1.top

[R69] 生成随机密码
来源：http://pty.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://yqo.tanke756.top

[R70] 时间戳与互转
来源：http://dim.yfazqb.com

date +%s;  date -d @1700000000
来源：http://qmn.meibo888.top

[R71] 日期格式化
来源：http://vze.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://rkv.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://yxl.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vcb.sysykeji.top

[R73] 分割大日志
来源：http://juf.zhengqikj.top

split -l 1000 big.log part_
来源：http://ogr.hesvh.cn

[R74] 批量重命名
来源：http://ypm.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hfs.svipenyu.cn

[R75] 导出环境变量
来源：http://glv.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://jpb.shangyingyoupin.top

[R76] 使用临时文件
来源：http://ssv.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fxl.quarkkingdee.top

[R77] 读取用户输入
来源：http://uyt.jyoumei.cn

read -rp "请输入: " ans
来源：http://xpg.haohaochexian.top

[R78] 交互式菜单
来源：http://crc.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://suf.quarkkingdee.top

[R79] 解析命令行选项
来源：http://bjy.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wda.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://cht.gogol.net.cn

time ./run.sh
来源：http://jqz.mhx1999.top

================================================================================
来源：http://wys.xuetiantiany.cn

S. C / C++ 专题
来源：http://wuf.quarkkingdee.top

================================================================================
来源：http://epa.52xcode.cn

[S01] C：Hello World
来源：http://mne.yj202588.top

#include <stdio.h>
来源：http://agz.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kpc.vehdjk.com

[S02] C：变量与格式化输出
来源：http://skh.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://wqm.ppjwa.cn

[S03] C：读入整数
来源：http://uxy.jyoumei.cn

int x; scanf("%d", &x);
来源：http://poj.bjfxy.top

[S04] C：字符串复制
来源：http://kyb.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://cre.fzhhl.top

[S05] C：字符串长度
来源：http://nxf.zhengqikj.top

strlen(s)
来源：http://kyf.epnwcf.com

[S06] C：字符串比较
来源：http://pjf.aibaodan.cn

strcmp(a, b) == 0
来源：http://snb.iojbl.cn

[S07] C：数组遍历求和
来源：http://oan.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hwa.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://dfk.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dpy.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://jgj.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ysh.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://dtq.xuanzx.com

int *p = &a;  *p = 5;
来源：http://rba.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://ypj.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://doe.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://brv.jlsjyb.cn

fclose(f);
来源：http://evo.yj20258.top

[S12] C：写文件
来源：http://iuz.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ysx.hammf.cn

[S13] C：宏定义
来源：http://bei.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jns.316326.xyz

[S14] C：枚举
来源：http://hfd.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://gxc.feifeiyinyue.top

[S15] C：类型转换
来源：http://irt.bbcook.cn

(double) a / b
来源：http://qfm.ydzc1.top

[S16] C：位操作置位
来源：http://rqu.hnxiangtu.top

x |= (1 << 3);
来源：http://nsi.yvedp.cn

[S17] C：安全拼接字符串
来源：http://bjo.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tlw.cdnleiting.top

[S18] C：命令行参数
来源：http://puf.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://uor.yueranfly.top

[S19] C：快速排序
来源：http://abz.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://nbw.sxryk.cn

[S20] C：二分查找
来源：http://nmh.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mee.wangdashe.top

[S21] C：字符类别判断
来源：http://bck.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gmm.fehbvm.com

[S22] C：字符串转数字
来源：http://amz.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lus.jlsjyb.cn

[S23] C：随机数
来源：http://czr.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wer.nanxuanxn.top

[S24] C：获取本地时间
来源：http://mnr.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jai.mhx1999.top

[S25] C：内存拷贝
来源：http://qmn.nanxuanxn.top

memcpy(dst, src, n);
来源：http://bgr.cashguo.top

[S26] C：内存清零
来源：http://ivm.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://foe.kuanghao11.cn

[S27] C：定义常量
来源：http://rkd.zhoulong.xyz

const double PI = 3.14159;
来源：http://ckq.andypj.xyz

[S28] C：静态变量
来源：http://mly.wangdashe.top

static int counter = 0;
来源：http://qsa.andypj.xyz

[S29] C：变参函数
来源：http://bwi.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qdv.yj202588.top

[S30] C：头文件保护
来源：http://fml.guowangkeji.top

#ifndef X_H
来源：http://rqo.hnxiangtu.top

#define X_H
来源：http://ror.yvedp.cn

#endif
来源：http://tpm.cashguo.top

[S31] C++：Hello World
来源：http://ent.gzhubu.top

#include <iostream>
来源：http://ime.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://aew.haohaochexian.top

[S32] C++：字符串
来源：http://pox.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://njx.yj202588.top

[S33] C++：vector 增删
来源：http://sdj.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bnn.jinqigufen.top

[S34] C++：遍历 vector
来源：http://ing.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://elr.yj20258888.top

[S35] C++：map
来源：http://tfl.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cfu.andypj.xyz

[S36] C++：unordered_map
来源：http://jbb.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkh.hammf.cn

[S37] C++：set
来源：http://vkd.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gjs.ppjwa.cn

[S38] C++：排序
来源：http://xix.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://njs.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://ixo.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fcr.hfpthk.cn

[S40] C++：查找元素
来源：http://xyo.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvs.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://yld.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nfw.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://ruq.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://bke.havefunace.top

[S43] C++：智能指针
来源：http://itg.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://rsv.cucudq.cn

[S44] C++：引用传参
来源：http://qxg.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://rur.hnqzz.top

[S45] C++：lambda
来源：http://qom.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://pas.hnqzz.top

[S46] C++：函数模板
来源：http://ury.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://skb.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://wpj.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://edd.yangfankeji.com

[S48] C++：逐行读文件
来源：http://wug.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mdf.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://wdr.yj202588.top

[S49] C++：写文件
来源：http://lxr.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lsb.9152youxi.cn

[S50] C++：格式化数字
来源：http://qjy.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mwt.daxiang520.top

[S51] C++：显式类型转换
来源：http://qgj.jinqigufen.top

static_cast<double>(a) / b
来源：http://svn.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://oxc.316326.xyz

int size() const noexcept { return n_; }
来源：http://mjn.quarkkingdee.top

[S53] C++：移动语义
来源：http://qix.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://coz.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://tsl.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://okr.52xcode.cn

[S55] C++：结构化绑定
来源：http://ubq.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dxe.zdbjq.cn

[S56] C++：optional
来源：http://vde.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bie.tarul.cn

[S57] C++：编译期常量
来源：http://wig.fktsv.cn

constexpr int N = 10;
来源：http://zvf.yj20258.top

[S58] C++：命名空间
来源：http://ihf.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://dif.birdmap.top

[S59] C++：静态断言
来源：http://tsw.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ooe.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://ngq.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qct.jinqigufen.top

================================================================================
来源：http://nww.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://itt.nanxuanxn.top

================================================================================
来源：http://pki.meibo888.top

[T01] Kotlin：Hello World
来源：http://xvq.zhixingplan.top

println("Hello")
来源：http://uja.gzhubu.top

[T02] Kotlin：变量
来源：http://oza.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cxh.yonumen.top

[T03] Kotlin：字符串模板
来源：http://eto.yangfankeji.com

"值: $b"
来源：http://fvd.yj20258.top

[T04] Kotlin：空安全
来源：http://jti.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://euv.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://gat.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zos.guannengcc.top

[T06] Kotlin：集合映射
来源：http://nnu.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bfh.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://ewz.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://fze.gogol.net.cn

[T08] Kotlin：数据类
来源：http://qcb.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://bpu.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://okc.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://tel.vehdjk.com

[T10] Kotlin：默认参数
来源：http://zll.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dag.andypj.xyz

[T11] Kotlin：协程
来源：http://jio.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gxz.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://vea.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://wrt.sweek.top

[T13] Kotlin：只读 Map
来源：http://xzf.hesvh.cn

val m = mapOf("a" to 1)
来源：http://sws.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://rir.zhixingplan.top

for (i in 1..10) println(i)
来源：http://yij.sufxvd.cn

[T15] Kotlin：接口
来源：http://ddu.wangdashe.top

interface Shape { fun area(): Double }
来源：http://wec.gzhubu.top

[T16] Swift：Hello World
来源：http://dss.hysaishi.cn

print("Hello")
来源：http://hpw.zycfv.cn

[T17] Swift：变量与常量
来源：http://syd.yangfankeji.com

var a = 1;  let b = 2
来源：http://ruw.316326.xyz

[T18] Swift：字符串插值
来源：http://lji.quarkkingdee.top

"值: \(b)"
来源：http://oee.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://dah.bbcook.cn

if let n = opt { print(n) }
来源：http://nlw.dianchejie.cn

[T20] Swift：数组操作
来源：http://fno.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cyd.daria6918.cn

[T21] Swift：遍历
来源：http://kak.shangyingyoupin.top

for x in a { print(x) }
来源：http://gre.yongpay.top

[T22] Swift：字典
来源：http://oaq.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://fxz.daxiang520.top

[T23] Swift：函数
来源：http://dgv.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://snd.daria6918.cn

[T24] Swift：闭包
来源：http://anm.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jls.gaohongyu789.top

[T25] Swift：结构体
来源：http://sjk.cucudq.cn

struct P { var x: Int }
来源：http://dsq.yj20258.top

[T26] Swift：类与重写
来源：http://dmp.jinqigufen.top

class A: Base { override func f() {} }
来源：http://oat.jianghu66.top

[T27] Swift：错误处理
来源：http://yti.xylfe.cn

do { try f() } catch { print(error) }
来源：http://hqo.tianlin.xyz

[T28] Swift：枚举
来源：http://kvg.chenjidiqi.icu

enum Color { case red, green }
来源：http://waa.yj202588.top

[T29] Swift：guard 提前返回
来源：http://zna.jqgfzy.top

guard let x = opt else { return }
来源：http://efu.jinqigufen.top

[T30] Swift：协议
来源：http://nvl.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://jtb.yanxiufei.cn

[T31] Lua：Hello World
来源：http://eod.hnxiangtu.top

print("Hello")
来源：http://bcc.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://ojp.zdbjq.cn

local a = 1
来源：http://grb.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://epe.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bil.yangfankeji.com

[T34] Lua：遍历表
来源：http://gat.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gdu.fzhhl.top

[T35] Lua：字典表
来源：http://ruz.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://zwb.shuidangran.top

[T36] Lua：函数
来源：http://eic.hammf.cn

function add(a, b) return a + b end
来源：http://fdh.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://upp.yuxming.cn

"a" .. "b"
来源：http://fxz.jqgfzy.top

[T38] Lua：条件
来源：http://mep.birdmap.top

if x > 0 then print("正") end
来源：http://fwg.xinyue.icu

[T39] Lua：模式匹配
来源：http://taa.zhiwuduotai.top

string.find(s, "%d+")
来源：http://jkb.hnqzz.top

[T40] Lua：元表
来源：http://psg.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://puz.daxiang520.top

[T41] Perl：Hello World
来源：http://hds.chenjidiqi.icu

print "Hello\n";
来源：http://kli.jinqigfzy.top

[T42] Perl：变量类型
来源：http://snz.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://icd.xuanzx.com

[T43] Perl：字符串插值
来源：http://jmv.fehbvm.com

"值: $a"
来源：http://pvo.hammf.cn

[T44] Perl：条件
来源：http://eqp.meibo888.top

if ($a > 0) { print "正"; }
来源：http://rhs.pycfn.com

[T45] Perl：数组遍历
来源：http://xqf.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://mez.havefunace.top

[T46] Perl：哈希操作
来源：http://thg.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cja.hysaishi.cn

[T47] Perl：正则捕获
来源：http://tmr.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://osa.cheryme.top

[T48] Perl：正则替换
来源：http://fmx.uphjek.com

$s =~ s/old/new/g;
来源：http://vwu.jqgufenzy.top


<!-- 参考信息 -->