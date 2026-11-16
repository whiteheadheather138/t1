代发 wailian999

find . -name "*.log" -type f
来源：http://iub.redwolf501.top

[R44] 按修改时间查找
来源：http://rer.kuanghao11.cn

find . -mtime -7 -type f
来源：http://izl.havefunace.top

[R45] 批量删除
来源：http://hzv.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://uxt.iojbl.cn

[R46] 递归替换文件内容
来源：http://vev.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ezb.pycfn.com

[R47] sed 单行替换
来源：http://zwm.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lgq.quarkkingdee.top

[R48] awk 取指定列
来源：http://kdf.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://bza.ctjpmb.com

[R49] awk 带条件
来源：http://qnw.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cda.zhongyouzk.top

[R50] awk 求和
来源：http://owh.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://pdi.hcnkem.com

[R51] 排序去重取前几
来源：http://lts.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://tjh.hywenlv.cn

[R52] 统计行数
来源：http://quv.nanxuanxn.top

wc -l a.txt
来源：http://hxj.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://amu.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rvr.xziqi.cn

[R54] 比较两个文件
来源：http://mfp.jiagoushi.top

diff a.txt b.txt
来源：http://blp.9152youxi.cn

[R55] 压缩与解压
来源：http://yar.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pbu.xylfe.cn

[R56] 远程拷贝
来源：http://lum.svipenyu.cn

scp file user@host:/path/
来源：http://bje.vehdjk.com

[R57] 远程执行命令
来源：http://omv.ivvv.top

ssh user@host 'uptime'
来源：http://enj.yanxiufei.cn

[R58] 下载文件
来源：http://vut.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qzl.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://law.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vgu.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://pko.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vnz.yongpay.top

[R61] 磁盘占用
来源：http://peh.xziqi.cn

df -h;  du -sh *
来源：http://oul.guannengcc.top

[R62] 找最占空间的文件
来源：http://csc.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://mmz.bjfxy.top

[R63] 内存与进程
来源：http://jmf.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://kou.meibo888.top

[R64] 结束进程
来源：http://apk.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://wwu.aizwys.cn

[R65] 查看端口占用
来源：http://enu.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tkl.nwbrower.top

[R66] 定时任务
来源：http://qsr.xziqi.cn

crontab -e;  crontab -l
来源：http://ufy.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://pyt.shzxlz.cn

openssl rand -hex 16
来源：http://jfx.0kj1m.cn

[R68] 计算文件校验值
来源：http://jjd.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://nnb.zhixingplan.top

[R69] 生成随机密码
来源：http://iir.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://euc.9152youxi.cn

[R70] 时间戳与互转
来源：http://ahi.guannengcc.top

date +%s;  date -d @1700000000
来源：http://kyj.iojbl.cn

[R71] 日期格式化
来源：http://boq.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kdb.aibaodan.cn

[R72] 等待端口就绪
来源：http://pjx.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bse.svipenyu.cn

[R73] 分割大日志
来源：http://ipz.zhoulong.xyz

split -l 1000 big.log part_
来源：http://dzd.hnxiangtu.top

[R74] 批量重命名
来源：http://moa.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jqz.shangyingyoupin.top

[R75] 导出环境变量
来源：http://udc.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://etd.redwolf501.top

[R76] 使用临时文件
来源：http://duq.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cem.c1oappe.top

[R77] 读取用户输入
来源：http://rrn.iojbl.cn

read -rp "请输入: " ans
来源：http://ouu.yanxiufei.cn

[R78] 交互式菜单
来源：http://uay.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qha.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://xgl.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oat.sweek.top

[R80] 查看脚本执行耗时
来源：http://unk.bjfxy.top

time ./run.sh
来源：http://yma.zhengqikj.top

================================================================================
来源：http://xbi.zhiwuduotai.top

S. C / C++ 专题
来源：http://wuq.jlsjyb.cn

================================================================================
来源：http://nem.hywenlv.cn

[S01] C：Hello World
来源：http://irn.andypj.xyz

#include <stdio.h>
来源：http://pba.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ayg.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://ucj.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://zub.xuanzx.com

[S03] C：读入整数
来源：http://irc.yj20258888.top

int x; scanf("%d", &x);
来源：http://tag.ehwqpu.com

[S04] C：字符串复制
来源：http://hhp.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://zqj.zdbjq.cn

[S05] C：字符串长度
来源：http://mwr.zhijiandao.cn

strlen(s)
来源：http://dga.hammf.cn

[S06] C：字符串比较
来源：http://djo.yangfankeji.com

strcmp(a, b) == 0
来源：http://umy.nanxinkj.top

[S07] C：数组遍历求和
来源：http://eec.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://faf.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://zis.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://krd.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://owe.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://axt.ppjwa.cn

[S10] C：指针与解引用
来源：http://uxq.meibo888.top

int *p = &a;  *p = 5;
来源：http://iqz.yueranfly.top

[S11] C：逐行读文件
来源：http://itq.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://mub.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qpq.zhixingplan.top

fclose(f);
来源：http://njf.vqdsnc.cn

[S12] C：写文件
来源：http://ryf.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bpd.aizwys.cn

[S13] C：宏定义
来源：http://bcn.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://geq.iojbl.cn

[S14] C：枚举
来源：http://poy.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://tyt.redwolf501.top

[S15] C：类型转换
来源：http://fia.sjlbkw.cn

(double) a / b
来源：http://ulu.xziqi.cn

[S16] C：位操作置位
来源：http://vcp.yuxming.cn

x |= (1 << 3);
来源：http://xgf.havefunace.top

[S17] C：安全拼接字符串
来源：http://cfn.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ncm.sweek.top

[S18] C：命令行参数
来源：http://mjk.pycfn.com

int main(int argc, char **argv)
来源：http://zhf.zhoulong.xyz

[S19] C：快速排序
来源：http://eyp.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://znz.guannengcc.top

[S20] C：二分查找
来源：http://yzh.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ove.shzxlz.cn

[S21] C：字符类别判断
来源：http://gtc.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fwz.zdbjq.cn

[S22] C：字符串转数字
来源：http://qnq.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://fqi.xylfe.cn

[S23] C：随机数
来源：http://zaq.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zmj.haohaochexian.top

[S24] C：获取本地时间
来源：http://raw.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ots.jianghu66.top

[S25] C：内存拷贝
来源：http://kgb.yueranfly.top

memcpy(dst, src, n);
来源：http://ogg.shzxlz.cn

[S26] C：内存清零
来源：http://skm.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://lmc.pengpengdd.cyou

[S27] C：定义常量
来源：http://kxu.gotoacloud.top

const double PI = 3.14159;
来源：http://nwa.sufxvd.cn

[S28] C：静态变量
来源：http://hov.yanxiufei.cn

static int counter = 0;
来源：http://oxx.jiagoushi.top

[S29] C：变参函数
来源：http://vew.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tyb.ehwqpu.com

[S30] C：头文件保护
来源：http://tpr.jqgufenzy.top

#ifndef X_H
来源：http://hxo.shzxlz.cn

#define X_H
来源：http://roq.hesvh.cn

#endif
来源：http://zao.sweek.top

[S31] C++：Hello World
来源：http://eoh.c1oappe.top

#include <iostream>
来源：http://cte.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://hip.cheryme.top

[S32] C++：字符串
来源：http://ayv.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://nyf.cqqwz.cn

[S33] C++：vector 增删
来源：http://fbb.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mku.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://fqm.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://opt.shangyingyoupin.top

[S35] C++：map
来源：http://tsd.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nkq.quarkkingdee.top

[S36] C++：unordered_map
来源：http://gpx.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bmr.feifeiyinyue.top

[S37] C++：set
来源：http://lrl.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://byv.jianghu66.top

[S38] C++：排序
来源：http://jir.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://jmo.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://ptv.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iat.nanxuanxn.top

[S40] C++：查找元素
来源：http://pdk.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kvk.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://eob.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xgb.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://fxr.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://amb.yanxiufei.cn

[S43] C++：智能指针
来源：http://mjb.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://lug.yuanzhike.top

[S44] C++：引用传参
来源：http://obx.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://mzg.ctjpmb.com

[S45] C++：lambda
来源：http://kke.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://jqj.jlsjyb.cn

[S46] C++：函数模板
来源：http://doe.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mmh.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://ntm.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kfd.hysaishi.cn

[S48] C++：逐行读文件
来源：http://rwq.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://zpn.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://nqv.jlsjyb.cn

[S49] C++：写文件
来源：http://zxl.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vha.c1oappe.top

[S50] C++：格式化数字
来源：http://rgr.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hlw.zdbjq.cn

[S51] C++：显式类型转换
来源：http://auy.jinqigfzy.top

static_cast<double>(a) / b
来源：http://rnu.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://ysx.hammf.cn

int size() const noexcept { return n_; }
来源：http://yut.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://gcv.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://exm.mhx1999.top

[S54] C++：异常处理
来源：http://wxu.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pue.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://mpw.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://acu.shanyushiyangtech.top

[S56] C++：optional
来源：http://frv.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mlk.zdqjudy.top

[S57] C++：编译期常量
来源：http://xen.wangdashe.top

constexpr int N = 10;
来源：http://zjb.tianlin.xyz

[S58] C++：命名空间
来源：http://qjz.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://yey.jinqigfzy.top

[S59] C++：静态断言
来源：http://kfk.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dvg.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://roq.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nuv.cdnleiting.top

================================================================================
来源：http://pkp.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cpq.xinyue.icu

================================================================================
来源：http://nbp.andypj.xyz

[T01] Kotlin：Hello World
来源：http://oir.zdqjudy.top

println("Hello")
来源：http://avb.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://old.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sfo.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://roy.smart0.xyz

"值: $b"
来源：http://lck.nwbrower.top

[T04] Kotlin：空安全
来源：http://wxp.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://drs.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://esm.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nrm.gzhubu.top

[T06] Kotlin：集合映射
来源：http://cxp.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://czf.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://vsh.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nlw.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://ykg.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://bhd.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://rmx.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://ltf.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://nrv.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gde.svipenyu.cn

[T11] Kotlin：协程
来源：http://hsn.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rau.shuidangran.top

[T12] Kotlin：解构声明
来源：http://jdf.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://dge.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://uzs.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://ryw.ppjwa.cn

[T14] Kotlin：循环
来源：http://ttd.bjfxy.top

for (i in 1..10) println(i)
来源：http://lrm.sufxvd.cn

[T15] Kotlin：接口
来源：http://pfx.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://jjx.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://efv.yanxiufei.cn

print("Hello")
来源：http://fud.xinyue.icu

[T17] Swift：变量与常量
来源：http://cyy.zhixingplan.top

var a = 1;  let b = 2
来源：http://cwu.jqgfzy.top

[T18] Swift：字符串插值
来源：http://xja.zhongyouzk.top

"值: \(b)"
来源：http://ksj.birdmap.top

[T19] Swift：可选绑定
来源：http://qyp.nwbrower.top

if let n = opt { print(n) }
来源：http://cas.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://gjy.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://qnw.jianghu66.top

[T21] Swift：遍历
来源：http://bse.sxryk.cn

for x in a { print(x) }
来源：http://qjl.pengpengdd.cyou

[T22] Swift：字典
来源：http://hxh.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://xov.zhijiandao.cn

[T23] Swift：函数
来源：http://kpo.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tnx.chenlongwang.top

[T24] Swift：闭包
来源：http://ovd.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://cvt.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://jss.ybcxt.top

struct P { var x: Int }
来源：http://nag.yueranfly.top

[T26] Swift：类与重写
来源：http://flp.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://qye.cashguo.top

[T27] Swift：错误处理
来源：http://sid.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://hih.havefunace.top

[T28] Swift：枚举
来源：http://gvb.jinqigfzy.top

enum Color { case red, green }
来源：http://fws.meibo888.top

[T29] Swift：guard 提前返回
来源：http://jyb.xinyue.icu

guard let x = opt else { return }
来源：http://kzn.jqgfzy.top

[T30] Swift：协议
来源：http://eug.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://ovs.nanxinkj.top

[T31] Lua：Hello World
来源：http://qma.iojbl.cn

print("Hello")
来源：http://dwg.cucudq.cn

[T32] Lua：局部变量
来源：http://akv.pycfn.com

local a = 1
来源：http://hfv.xylfe.cn

[T33] Lua：表（数组）
来源：http://gve.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ruz.hammf.cn

[T34] Lua：遍历表
来源：http://zqq.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vxh.yonumen.top

[T35] Lua：字典表
来源：http://rct.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://sel.yonumen.top

[T36] Lua：函数
来源：http://mzs.yj20258.top

function add(a, b) return a + b end
来源：http://klf.daxiang520.top

[T37] Lua：字符串拼接
来源：http://nag.nanxinkj.top

"a" .. "b"
来源：http://scp.zhongyouzk.top

[T38] Lua：条件
来源：http://kbb.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://tko.bbcook.cn

[T39] Lua：模式匹配
来源：http://sbj.jinqigfzy.top

string.find(s, "%d+")
来源：http://hzh.fanxiaobao.xyz

[T40] Lua：元表
来源：http://usl.hesvh.cn

setmetatable({}, { __index = base })
来源：http://hds.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://eep.andypj.xyz

print "Hello\n";
来源：http://pxm.ivvv.top

[T42] Perl：变量类型
来源：http://fnq.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qgb.chenzaomai.com

[T43] Perl：字符串插值
来源：http://umh.sjlbkw.cn

"值: $a"
来源：http://zzo.jiagoushi.top

[T44] Perl：条件
来源：http://htb.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://asp.gzhubu.top

[T45] Perl：数组遍历
来源：http://jbu.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://uup.yj20258.top

[T46] Perl：哈希操作
来源：http://gxh.chenlongwang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hgl.aizwys.cn


<!-- 参考信息 -->