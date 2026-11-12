代发 wailian999

find . -name "*.log" -type f
来源：http://umi.hnxiangtu.top

[R44] 按修改时间查找
来源：http://vnh.chenzaomai.com

find . -mtime -7 -type f
来源：http://ogg.jqgfzy.top

[R45] 批量删除
来源：http://ame.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://ymo.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://fzj.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zoa.haohaochexian.top

[R47] sed 单行替换
来源：http://eyj.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://tmy.zhixingplan.top

[R48] awk 取指定列
来源：http://qyc.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://hgk.epnwcf.com

[R49] awk 带条件
来源：http://qof.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zza.shzxlz.cn

[R50] awk 求和
来源：http://pcs.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wtk.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://kbf.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ttj.guowangkeji.top

[R52] 统计行数
来源：http://xlo.smart0.xyz

wc -l a.txt
来源：http://wkj.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://yry.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yiq.ehwqpu.com

[R54] 比较两个文件
来源：http://uex.smart0.xyz

diff a.txt b.txt
来源：http://rmz.jinqigufen.top

[R55] 压缩与解压
来源：http://riw.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oik.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://qsl.redwolf501.top

scp file user@host:/path/
来源：http://gtb.vqdsnc.cn

[R57] 远程执行命令
来源：http://oyl.sysykeji.top

ssh user@host 'uptime'
来源：http://zhx.yvedp.cn

[R58] 下载文件
来源：http://ssy.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vxo.jyoumei.cn

[R59] 发 POST JSON
来源：http://mof.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ggx.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://ndb.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivo.shangyingyoupin.top

[R61] 磁盘占用
来源：http://quw.c1oappe.top

df -h;  du -sh *
来源：http://hwo.0kj1m.cn

[R62] 找最占空间的文件
来源：http://imd.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://gcp.daria6918.cn

[R63] 内存与进程
来源：http://yqt.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://trb.tianlin.xyz

[R64] 结束进程
来源：http://dlg.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://pis.yvedp.cn

[R65] 查看端口占用
来源：http://oxh.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rsy.uphjek.com

[R66] 定时任务
来源：http://zpi.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://irb.sysykeji.top

[R67] 生成随机十六进制串
来源：http://kdp.yonumen.top

openssl rand -hex 16
来源：http://rpi.nanxuanxn.top

[R68] 计算文件校验值
来源：http://zlj.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cor.yongpay.top

[R69] 生成随机密码
来源：http://sgh.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://ohx.nwbrower.top

[R70] 时间戳与互转
来源：http://dfs.uphjek.com

date +%s;  date -d @1700000000
来源：http://kit.hnxiangtu.top

[R71] 日期格式化
来源：http://tmg.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rui.daria6918.cn

[R72] 等待端口就绪
来源：http://crl.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ddg.aizwys.cn

[R73] 分割大日志
来源：http://qnr.fehbvm.com

split -l 1000 big.log part_
来源：http://cqc.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://jda.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pvf.ydjk.org.cn

[R75] 导出环境变量
来源：http://nfz.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://zyz.ehwqpu.com

[R76] 使用临时文件
来源：http://clu.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qdm.andypj.xyz

[R77] 读取用户输入
来源：http://rer.0kj1m.cn

read -rp "请输入: " ans
来源：http://una.xuanzx.com

[R78] 交互式菜单
来源：http://wzy.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wqu.yangfankeji.com

[R79] 解析命令行选项
来源：http://axw.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qoy.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://nyl.yongpay.top

time ./run.sh
来源：http://ego.gotoacloud.top

================================================================================
来源：http://vuz.ydzc1.top

S. C / C++ 专题
来源：http://qds.ywan-chungtsiang.top

================================================================================
来源：http://kgh.jqgfzy.top

[S01] C：Hello World
来源：http://uux.chenzaomai.com

#include <stdio.h>
来源：http://djn.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ktn.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://rcz.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://iiq.birdmap.top

[S03] C：读入整数
来源：http://pfm.52xcode.cn

int x; scanf("%d", &x);
来源：http://xsv.pengpengdd.cyou

[S04] C：字符串复制
来源：http://vxr.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uko.yuxming.cn

[S05] C：字符串长度
来源：http://dwb.sweek.top

strlen(s)
来源：http://ndo.guowangkeji.top

[S06] C：字符串比较
来源：http://gnr.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://etu.dianchejie.cn

[S07] C：数组遍历求和
来源：http://dmf.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mep.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://mjr.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iur.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://guh.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zpj.meibo888.top

[S10] C：指针与解引用
来源：http://kwp.tarul.cn

int *p = &a;  *p = 5;
来源：http://qzf.jianghu66.top

[S11] C：逐行读文件
来源：http://bvs.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://uva.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ebu.gzhubu.top

fclose(f);
来源：http://mhw.quarkkingdee.top

[S12] C：写文件
来源：http://ntk.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hzx.yongpay.top

[S13] C：宏定义
来源：http://gew.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kmq.wangshuangyany.cn

[S14] C：枚举
来源：http://uge.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://tal.redwolf501.top

[S15] C：类型转换
来源：http://zms.sysykeji.top

(double) a / b
来源：http://qto.yj20258888.top

[S16] C：位操作置位
来源：http://zcv.jinghuilouyu.cn

x |= (1 << 3);
来源：http://kvl.yj202588.top

[S17] C：安全拼接字符串
来源：http://rds.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qjz.zhijiandao.cn

[S18] C：命令行参数
来源：http://ttf.uphjek.com

int main(int argc, char **argv)
来源：http://kgd.nanxinkj.top

[S19] C：快速排序
来源：http://fnj.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bbv.jqgufenzy.top

[S20] C：二分查找
来源：http://pee.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://byx.gzhubu.top

[S21] C：字符类别判断
来源：http://cje.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ikg.yueranfly.top

[S22] C：字符串转数字
来源：http://lpm.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://plc.feifeiyinyue.top

[S23] C：随机数
来源：http://aje.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mcr.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://cjn.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://znr.zhongyouzk.top

[S25] C：内存拷贝
来源：http://bls.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://xiz.epnwcf.com

[S26] C：内存清零
来源：http://pef.fehbvm.com

memset(a, 0, sizeof a);
来源：http://ust.gaohongyu789.top

[S27] C：定义常量
来源：http://jmo.xuetiantiany.cn

const double PI = 3.14159;
来源：http://gyn.iojbl.cn

[S28] C：静态变量
来源：http://bkm.daxiang520.top

static int counter = 0;
来源：http://qxn.hnxiangtu.top

[S29] C：变参函数
来源：http://yjv.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pne.cashguo.top

[S30] C：头文件保护
来源：http://xlw.0kj1m.cn

#ifndef X_H
来源：http://jwy.ctjpmb.com

#define X_H
来源：http://wwf.hysaishi.cn

#endif
来源：http://nxg.yongpay.top

[S31] C++：Hello World
来源：http://ygz.zycfv.cn

#include <iostream>
来源：http://zcq.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://fbh.cashguo.top

[S32] C++：字符串
来源：http://ouk.tarul.cn

std::string s = "hi";  s += "!";
来源：http://lzw.jlsjyb.cn

[S33] C++：vector 增删
来源：http://rjd.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kev.yj202588.top

[S34] C++：遍历 vector
来源：http://cyi.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://hxx.yfazqb.com

[S35] C++：map
来源：http://qoz.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fri.shzxlz.cn

[S36] C++：unordered_map
来源：http://gma.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kjw.hammf.cn

[S37] C++：set
来源：http://vgt.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://utc.shuidangran.top

[S38] C++：排序
来源：http://xxr.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://qmv.ivvv.top

[S39] C++：自定义比较器排序
来源：http://akw.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kew.zhengqikj.top

[S40] C++：查找元素
来源：http://yww.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lpk.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://fpd.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ljv.ydzc1.top

[S42] C++：继承与虚函数
来源：http://xzp.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://igl.iojbl.cn

[S43] C++：智能指针
来源：http://gxg.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://eue.meibo888.top

[S44] C++：引用传参
来源：http://cgz.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://wtc.zhongyouzk.top

[S45] C++：lambda
来源：http://xzv.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://ooj.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://vus.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ihw.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://yhx.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uxf.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://ext.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ivp.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://rdt.yj202588.top

[S49] C++：写文件
来源：http://brh.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://noc.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://nfx.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lcm.yvedp.cn

[S51] C++：显式类型转换
来源：http://xqm.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://rsb.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://ila.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://fmd.jyoumei.cn

[S53] C++：移动语义
来源：http://vkk.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://dvl.jlsjyb.cn

[S54] C++：异常处理
来源：http://jyx.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kow.hcnkem.com

[S55] C++：结构化绑定
来源：http://wti.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rlg.birdmap.top

[S56] C++：optional
来源：http://dth.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bhc.birdmap.top

[S57] C++：编译期常量
来源：http://vmq.jinqigufen.top

constexpr int N = 10;
来源：http://qvu.9152youxi.cn

[S58] C++：命名空间
来源：http://gdp.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://gih.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://amh.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fvd.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://inp.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nmz.ybcxt.top

================================================================================
来源：http://oya.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zeh.chenlongwang.top

================================================================================
来源：http://yss.yvedp.cn

[T01] Kotlin：Hello World
来源：http://rmt.chenjidiqi.icu

println("Hello")
来源：http://qhc.hnxiangtu.top

[T02] Kotlin：变量
来源：http://fcf.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xaj.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://nkh.bjfxy.top

"值: $b"
来源：http://gqz.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://hay.nanxinkj.top

val n: String? = null;  n?.length
来源：http://jqj.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://xmq.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hfy.fengsongda.top

[T06] Kotlin：集合映射
来源：http://lhu.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dhe.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://nzw.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nwe.pycfn.com

[T08] Kotlin：数据类
来源：http://crb.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://lzi.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://vmp.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://byx.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://cal.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nfy.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://zex.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://svn.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://vrq.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://upw.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://pia.bjfxy.top

val m = mapOf("a" to 1)
来源：http://tou.fengsongda.top

[T14] Kotlin：循环
来源：http://dar.dashuyun.cn

for (i in 1..10) println(i)
来源：http://psb.cqqwz.cn

[T15] Kotlin：接口
来源：http://ajt.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://mws.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://ljj.yangfankeji.com

print("Hello")
来源：http://oay.hywenlv.cn

[T17] Swift：变量与常量
来源：http://nkc.316326.xyz

var a = 1;  let b = 2
来源：http://oar.jyoumei.cn

[T18] Swift：字符串插值
来源：http://wsx.yongpay.top

"值: \(b)"
来源：http://fle.smart0.xyz

[T19] Swift：可选绑定
来源：http://uhl.hfpthk.cn

if let n = opt { print(n) }
来源：http://nvq.zhengqikj.top

[T20] Swift：数组操作
来源：http://liz.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://uau.quarkkingdee.top

[T21] Swift：遍历
来源：http://giv.jqgufenzy.top

for x in a { print(x) }
来源：http://pzo.yj20258.top

[T22] Swift：字典
来源：http://gpf.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://pfx.yanxiufei.cn

[T23] Swift：函数
来源：http://ivq.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ibp.zhixingplan.top

[T24] Swift：闭包
来源：http://eud.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgt.wangdashe.top

[T25] Swift：结构体
来源：http://apf.gogol.net.cn

struct P { var x: Int }
来源：http://tzh.sxryk.cn

[T26] Swift：类与重写
来源：http://jzr.fehbvm.com

class A: Base { override func f() {} }
来源：http://tlz.xuanzx.com

[T27] Swift：错误处理
来源：http://pnn.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://vsp.kuanghao11.cn

[T28] Swift：枚举
来源：http://dlo.ehwqpu.com

enum Color { case red, green }
来源：http://ski.cheryme.top

[T29] Swift：guard 提前返回
来源：http://kxv.sjlbkw.cn

guard let x = opt else { return }
来源：http://jlc.zhongyouzk.top

[T30] Swift：协议
来源：http://shj.yj202588.top

protocol Shape { func area() -> Double }
来源：http://zjg.daxiang520.top

[T31] Lua：Hello World
来源：http://inz.hesvh.cn

print("Hello")
来源：http://rqu.bbcook.cn

[T32] Lua：局部变量
来源：http://yfv.shanyushiyangtech.top

local a = 1
来源：http://rbc.smart0.xyz

[T33] Lua：表（数组）
来源：http://nvw.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://irf.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://dmx.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zdw.jyoumei.cn

[T35] Lua：字典表
来源：http://rug.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://izn.jinqigfzy.top

[T36] Lua：函数
来源：http://scs.guowangkeji.top

function add(a, b) return a + b end
来源：http://nem.smart0.xyz

[T37] Lua：字符串拼接
来源：http://xbe.jyoumei.cn

"a" .. "b"
来源：http://xfc.hongshengwenyu.top

[T38] Lua：条件
来源：http://dax.shuidangran.top

if x > 0 then print("正") end
来源：http://pmr.guowangkeji.top

[T39] Lua：模式匹配
来源：http://uvb.jqgfzy.top

string.find(s, "%d+")
来源：http://bhw.sweek.top

[T40] Lua：元表
来源：http://chk.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://mue.wangdashe.top

[T41] Perl：Hello World
来源：http://gtc.wangshuangyany.cn

print "Hello\n";
来源：http://xaf.smart0.xyz

[T42] Perl：变量类型
来源：http://wtn.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wzq.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://rbt.epnwcf.com

"值: $a"
来源：http://dit.nanxinkj.top

[T44] Perl：条件
来源：http://aat.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://mbe.tianlin.xyz

[T45] Perl：数组遍历
来源：http://jfy.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://bxh.hammf.cn

[T46] Perl：哈希操作
来源：http://pff.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dce.tarul.cn


<!-- 参考信息 -->