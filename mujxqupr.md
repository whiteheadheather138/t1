代发 wailian999

cmd >/dev/null 2>&1
来源：http://ixr.hywenlv.cn

[R42] 输入重定向
来源：http://lfk.svipenyu.cn

wc -l < a.txt
来源：http://mvd.yuanzhike.top

[R43] 按名字查找文件
来源：http://muv.ivvv.top

find . -name "*.log" -type f
来源：http://ajt.bbcook.cn

[R44] 按修改时间查找
来源：http://izb.daxiang520.top

find . -mtime -7 -type f
来源：http://mer.sjlbkw.cn

[R45] 批量删除
来源：http://nqs.xuanzx.com

find . -name "*.tmp" -delete
来源：http://oxg.9152youxi.cn

[R46] 递归替换文件内容
来源：http://rju.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uou.fehbvm.com

[R47] sed 单行替换
来源：http://exm.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wja.0kj1m.cn

[R48] awk 取指定列
来源：http://ess.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://gam.cucudq.cn

[R49] awk 带条件
来源：http://kux.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ahz.zhongyouzk.top

[R50] awk 求和
来源：http://qvz.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://bxe.yongpay.top

[R51] 排序去重取前几
来源：http://xwo.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ttz.fehbvm.com

[R52] 统计行数
来源：http://upd.nanxuanxn.top

wc -l a.txt
来源：http://icf.yj20258.top

[R53] 查看文件头与实时尾
来源：http://jys.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hmg.hywenlv.cn

[R54] 比较两个文件
来源：http://ore.nwbrower.top

diff a.txt b.txt
来源：http://pkt.c1oappe.top

[R55] 压缩与解压
来源：http://ozi.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qzb.ydzc1.top

[R56] 远程拷贝
来源：http://hnw.hfpthk.cn

scp file user@host:/path/
来源：http://kfa.yuxming.cn

[R57] 远程执行命令
来源：http://yeg.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://snp.birdmap.top

[R58] 下载文件
来源：http://ymm.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://htv.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://unt.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sat.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://oaz.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vuh.epnwcf.com

[R61] 磁盘占用
来源：http://ats.zhongyouzk.top

df -h;  du -sh *
来源：http://lvo.aibaodan.cn

[R62] 找最占空间的文件
来源：http://zwm.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://fzj.yuanzhike.top

[R63] 内存与进程
来源：http://ekr.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://nxj.jinqigufen.top

[R64] 结束进程
来源：http://rci.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://yry.tanke756.top

[R65] 查看端口占用
来源：http://dup.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nzf.hammf.cn

[R66] 定时任务
来源：http://zwr.tianlin.xyz

crontab -e;  crontab -l
来源：http://qnv.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://dyx.hongshengwenyu.top

openssl rand -hex 16
来源：http://ayr.ybcxt.top

[R68] 计算文件校验值
来源：http://oyh.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dam.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://bxz.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://qec.epnwcf.com

[R70] 时间戳与互转
来源：http://plq.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://yya.vqdsnc.cn

[R71] 日期格式化
来源：http://ovp.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybi.jinqigufen.top

[R72] 等待端口就绪
来源：http://fml.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shl.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://yyj.ppjwa.cn

split -l 1000 big.log part_
来源：http://zth.tanke756.top

[R74] 批量重命名
来源：http://tvg.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnw.wangshuangyany.cn

[R75] 导出环境变量
来源：http://car.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rwz.dashuyun.cn

[R76] 使用临时文件
来源：http://ftf.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://icu.cheryme.top

[R77] 读取用户输入
来源：http://avn.jinqigfzy.top

read -rp "请输入: " ans
来源：http://hca.xylfe.cn

[R78] 交互式菜单
来源：http://wyj.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hum.0kj1m.cn

[R79] 解析命令行选项
来源：http://tun.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wqh.ivvv.top

[R80] 查看脚本执行耗时
来源：http://hhk.ydzc1.top

time ./run.sh
来源：http://eev.nanxuanxn.top

================================================================================
来源：http://bkx.guowangkeji.top

S. C / C++ 专题
来源：http://zvp.zhiwuduotai.top

================================================================================
来源：http://tzs.nwbrower.top

[S01] C：Hello World
来源：http://fff.dashuyun.cn

#include <stdio.h>
来源：http://yte.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zko.iojbl.cn

[S02] C：变量与格式化输出
来源：http://imb.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://rvt.zdqjudy.top

[S03] C：读入整数
来源：http://oqd.ybcxt.top

int x; scanf("%d", &x);
来源：http://ols.jqgufenzy.top

[S04] C：字符串复制
来源：http://wbf.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://poh.hywenlv.cn

[S05] C：字符串长度
来源：http://xgp.316326.xyz

strlen(s)
来源：http://rrl.wangshuangyany.cn

[S06] C：字符串比较
来源：http://fbo.zdqjudy.top

strcmp(a, b) == 0
来源：http://qmp.epnwcf.com

[S07] C：数组遍历求和
来源：http://axc.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ikm.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://nmh.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vaj.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://trb.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wcc.xuetiantiany.cn

[S10] C：指针与解引用
来源：http://kgn.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://uuo.yongpay.top

[S11] C：逐行读文件
来源：http://csc.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://gal.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qlh.sysykeji.top

fclose(f);
来源：http://cky.yangfankeji.com

[S12] C：写文件
来源：http://wob.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uhc.jianghu66.top

[S13] C：宏定义
来源：http://qds.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hwu.cdnleiting.top

[S14] C：枚举
来源：http://kyv.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://mid.hywenlv.cn

[S15] C：类型转换
来源：http://vbb.chenjidiqi.icu

(double) a / b
来源：http://dhn.chenjidiqi.icu

[S16] C：位操作置位
来源：http://edv.jqgufenzy.top

x |= (1 << 3);
来源：http://psw.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://pso.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dch.redwolf501.top

[S18] C：命令行参数
来源：http://ihx.zdqjudy.top

int main(int argc, char **argv)
来源：http://kvu.shangyingyoupin.top

[S19] C：快速排序
来源：http://qov.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ocr.316326.xyz

[S20] C：二分查找
来源：http://gdm.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pim.nanxuanxn.top

[S21] C：字符类别判断
来源：http://itn.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eip.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://phc.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://blw.wangdashe.top

[S23] C：随机数
来源：http://tfl.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ffq.hcnkem.com

[S24] C：获取本地时间
来源：http://uap.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ahy.sufxvd.cn

[S25] C：内存拷贝
来源：http://mqt.fktsv.cn

memcpy(dst, src, n);
来源：http://qjh.zhijiandao.cn

[S26] C：内存清零
来源：http://wka.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://idf.vqdsnc.cn

[S27] C：定义常量
来源：http://dci.tianlin.xyz

const double PI = 3.14159;
来源：http://glg.ehwqpu.com

[S28] C：静态变量
来源：http://euh.wangshuangyany.cn

static int counter = 0;
来源：http://suc.andypj.xyz

[S29] C：变参函数
来源：http://hnh.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://euk.hammf.cn

[S30] C：头文件保护
来源：http://urt.xinyue.icu

#ifndef X_H
来源：http://boe.havefunace.top

#define X_H
来源：http://fhf.zycfv.cn

#endif
来源：http://ujj.xinyue.icu

[S31] C++：Hello World
来源：http://lfh.xuanzx.com

#include <iostream>
来源：http://iub.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://pmv.bbcook.cn

[S32] C++：字符串
来源：http://wxj.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://sql.gaohongyu789.top

[S33] C++：vector 增删
来源：http://kcd.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ulm.52xcode.cn

[S34] C++：遍历 vector
来源：http://bwc.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://mpl.ydzc1.top

[S35] C++：map
来源：http://yfb.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvz.shuidangran.top

[S36] C++：unordered_map
来源：http://fwg.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qps.jiagoushi.top

[S37] C++：set
来源：http://mcy.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mcp.xinyue.icu

[S38] C++：排序
来源：http://hgb.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://men.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://pfa.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gss.jqgufenzy.top

[S40] C++：查找元素
来源：http://hia.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dsp.xylfe.cn

[S41] C++：类与构造函数
来源：http://ucb.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eei.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://ved.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://var.cdnleiting.top

[S43] C++：智能指针
来源：http://klk.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://qwt.zycfv.cn

[S44] C++：引用传参
来源：http://dyb.hcnkem.com

void inc(int &x) { ++x; }
来源：http://peg.yj202588.top

[S45] C++：lambda
来源：http://zzt.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bpv.zhijiandao.cn

[S46] C++：函数模板
来源：http://kjc.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kkw.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://ppx.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wib.sxryk.cn

[S48] C++：逐行读文件
来源：http://mzj.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://gel.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://osd.ydjk.org.cn

[S49] C++：写文件
来源：http://zsw.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://doy.jyoumei.cn

[S50] C++：格式化数字
来源：http://uyb.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hgq.ehwqpu.com

[S51] C++：显式类型转换
来源：http://pfb.sweek.top

static_cast<double>(a) / b
来源：http://kqs.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://krk.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://kby.gaohongyu789.top

[S53] C++：移动语义
来源：http://laz.hammf.cn

std::vector<int> w = std::move(v);
来源：http://ick.yvedp.cn

[S54] C++：异常处理
来源：http://chi.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jbr.9152youxi.cn

[S55] C++：结构化绑定
来源：http://sbf.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mqr.zhijiandao.cn

[S56] C++：optional
来源：http://zyn.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ngk.ydjk.org.cn

[S57] C++：编译期常量
来源：http://qxm.xuanzx.com

constexpr int N = 10;
来源：http://gcm.cdnleiting.top

[S58] C++：命名空间
来源：http://mxh.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://ogm.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://xyk.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://giy.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://gye.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pvb.sysykeji.top

================================================================================
来源：http://int.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nzl.jinghuilouyu.cn

================================================================================
来源：http://vnx.hesvh.cn

[T01] Kotlin：Hello World
来源：http://qxs.guowangkeji.top

println("Hello")
来源：http://tbc.hnxiangtu.top

[T02] Kotlin：变量
来源：http://swh.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fzd.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://ble.gotoacloud.top

"值: $b"
来源：http://ctg.gzhubu.top

[T04] Kotlin：空安全
来源：http://dvf.sysykeji.top

val n: String? = null;  n?.length
来源：http://phg.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://ibc.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rhj.guannengcc.top

[T06] Kotlin：集合映射
来源：http://qgb.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://czr.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://bql.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ksv.tanke756.top

[T08] Kotlin：数据类
来源：http://oki.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://igd.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://eop.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://afi.fengsongda.top

[T10] Kotlin：默认参数
来源：http://cne.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cfr.bjfxy.top

[T11] Kotlin：协程
来源：http://oyu.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://msq.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://bde.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://ews.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://bcb.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://jyr.ivvv.top

[T14] Kotlin：循环
来源：http://dvn.9152youxi.cn

for (i in 1..10) println(i)
来源：http://kjr.ydzc1.top

[T15] Kotlin：接口
来源：http://man.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://ydu.jyoumei.cn

[T16] Swift：Hello World
来源：http://ehp.yonumen.top

print("Hello")
来源：http://gzi.ppjwa.cn

[T17] Swift：变量与常量
来源：http://hin.vehdjk.com

var a = 1;  let b = 2
来源：http://not.zdbjq.cn

[T18] Swift：字符串插值
来源：http://zky.jqgfzy.top

"值: \(b)"
来源：http://pgz.andypj.xyz

[T19] Swift：可选绑定
来源：http://xac.gogol.net.cn

if let n = opt { print(n) }
来源：http://qru.yj20258.top

[T20] Swift：数组操作
来源：http://yqz.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ufh.ppjwa.cn

[T21] Swift：遍历
来源：http://uhl.zhijiandao.cn

for x in a { print(x) }
来源：http://erc.daxiang520.top

[T22] Swift：字典
来源：http://vri.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://bdw.nanxinkj.top

[T23] Swift：函数
来源：http://wnu.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cwm.yvedp.cn

[T24] Swift：闭包
来源：http://cfe.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://gsy.zhixingplan.top

[T25] Swift：结构体
来源：http://ogs.ehwqpu.com

struct P { var x: Int }
来源：http://gkz.yanxiufei.cn

[T26] Swift：类与重写
来源：http://trr.ivvv.top

class A: Base { override func f() {} }
来源：http://zlv.yonumen.top

[T27] Swift：错误处理
来源：http://qoi.guannengcc.top

do { try f() } catch { print(error) }
来源：http://kxn.ybcxt.top

[T28] Swift：枚举
来源：http://fet.shuidangran.top

enum Color { case red, green }
来源：http://wcs.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://wkk.zdbjq.cn

guard let x = opt else { return }
来源：http://drw.aibaodan.cn

[T30] Swift：协议
来源：http://qao.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://ufu.yanxiufei.cn

[T31] Lua：Hello World
来源：http://fta.fzhhl.top

print("Hello")
来源：http://mmd.gogol.net.cn

[T32] Lua：局部变量
来源：http://rio.fengsongda.top

local a = 1
来源：http://qmm.wangdashe.top

[T33] Lua：表（数组）
来源：http://tvt.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wuq.nanxuanxn.top

[T34] Lua：遍历表
来源：http://tzi.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wtd.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://pvq.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://hvg.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://mgl.meibo888.top

function add(a, b) return a + b end
来源：http://bts.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://vtv.hammf.cn

"a" .. "b"
来源：http://zfi.ppjwa.cn

[T38] Lua：条件
来源：http://lce.xylfe.cn

if x > 0 then print("正") end
来源：http://xsy.sweek.top

[T39] Lua：模式匹配
来源：http://yii.havefunace.top

string.find(s, "%d+")
来源：http://coz.hfpthk.cn

[T40] Lua：元表
来源：http://njx.gzhubu.top

setmetatable({}, { __index = base })
来源：http://yzc.vqdsnc.cn

[T41] Perl：Hello World
来源：http://oas.fanxiaobao.xyz

print "Hello\n";
来源：http://bhy.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://hvs.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ffi.dianchejie.cn

[T43] Perl：字符串插值
来源：http://tck.316326.xyz

"值: $a"
来源：http://xbe.shangyingyoupin.top

[T44] Perl：条件
来源：http://jgz.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://yla.fktsv.cn


<!-- 参考信息 -->