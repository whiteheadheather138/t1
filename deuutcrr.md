代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pan.jinyuanbaomall.cn

[R50] awk 求和
来源：http://ntr.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jig.ydzc1.top

[R51] 排序去重取前几
来源：http://ndj.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rxq.daria6918.cn

[R52] 统计行数
来源：http://gql.yonumen.top

wc -l a.txt
来源：http://mkw.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://gli.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zvs.fehbvm.com

[R54] 比较两个文件
来源：http://xej.yuanzhike.top

diff a.txt b.txt
来源：http://gkc.yueranfly.top

[R55] 压缩与解压
来源：http://ugg.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vhi.hysaishi.cn

[R56] 远程拷贝
来源：http://ssx.chenjidiqi.icu

scp file user@host:/path/
来源：http://kqu.sweek.top

[R57] 远程执行命令
来源：http://uyq.havefunace.top

ssh user@host 'uptime'
来源：http://whc.ppjwa.cn

[R58] 下载文件
来源：http://wlx.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bwk.zhengqikj.top

[R59] 发 POST JSON
来源：http://sme.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://byt.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://wim.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lbe.kuanghao11.cn

[R61] 磁盘占用
来源：http://brx.hysaishi.cn

df -h;  du -sh *
来源：http://pjx.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://mmo.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://pkp.zhongyouzk.top

[R63] 内存与进程
来源：http://wzt.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://hes.redwolf501.top

[R64] 结束进程
来源：http://lsw.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://jss.svipenyu.cn

[R65] 查看端口占用
来源：http://wle.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fkw.c1oappe.top

[R66] 定时任务
来源：http://hnh.gaohongyu789.top

crontab -e;  crontab -l
来源：http://luj.yj20258.top

[R67] 生成随机十六进制串
来源：http://bhy.nanxinkj.top

openssl rand -hex 16
来源：http://msv.aizwys.cn

[R68] 计算文件校验值
来源：http://jog.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvs.chenjidiqi.icu

[R69] 生成随机密码
来源：http://ruf.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://ylc.yj202588.top

[R70] 时间戳与互转
来源：http://cpr.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://tbp.sysykeji.top

[R71] 日期格式化
来源：http://aac.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cnc.svipenyu.cn

[R72] 等待端口就绪
来源：http://xkc.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://exh.birdmap.top

[R73] 分割大日志
来源：http://ivu.gotoacloud.top

split -l 1000 big.log part_
来源：http://usj.yuanzhike.top

[R74] 批量重命名
来源：http://fcf.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sjo.jlsjyb.cn

[R75] 导出环境变量
来源：http://ehf.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://snl.svipenyu.cn

[R76] 使用临时文件
来源：http://klr.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lul.yfazqb.com

[R77] 读取用户输入
来源：http://adm.cdnleiting.top

read -rp "请输入: " ans
来源：http://yng.cqqwz.cn

[R78] 交互式菜单
来源：http://jbo.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hth.zdbjq.cn

[R79] 解析命令行选项
来源：http://etr.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://was.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://epl.havefunace.top

time ./run.sh
来源：http://pcw.chenjidiqi.icu

================================================================================
来源：http://ptl.pengpengdd.cyou

S. C / C++ 专题
来源：http://ana.daxiang520.top

================================================================================
来源：http://rps.ybcxt.top

[S01] C：Hello World
来源：http://xvy.0kj1m.cn

#include <stdio.h>
来源：http://kfj.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mhq.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://fyc.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://oan.cashguo.top

[S03] C：读入整数
来源：http://fpa.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://vhl.bjfxy.top

[S04] C：字符串复制
来源：http://uui.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sls.gogol.net.cn

[S05] C：字符串长度
来源：http://pgq.birdmap.top

strlen(s)
来源：http://jix.tian-w.cn

[S06] C：字符串比较
来源：http://fvx.gaohongyu789.top

strcmp(a, b) == 0
来源：http://efy.sweek.top

[S07] C：数组遍历求和
来源：http://bqz.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://byu.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://yuu.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ikv.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://oiz.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rwj.zdqjudy.top

[S10] C：指针与解引用
来源：http://qgv.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://dbx.haohaochexian.top

[S11] C：逐行读文件
来源：http://dgy.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://znq.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tyx.epnwcf.com

fclose(f);
来源：http://gke.dashuyun.cn

[S12] C：写文件
来源：http://eyi.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ctp.zhongyouzk.top

[S13] C：宏定义
来源：http://wfv.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://slq.yfazqb.com

[S14] C：枚举
来源：http://jyl.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://dzt.zhiwuduotai.top

[S15] C：类型转换
来源：http://uru.zhijiandao.cn

(double) a / b
来源：http://grz.gotoacloud.top

[S16] C：位操作置位
来源：http://rsg.zhijiandao.cn

x |= (1 << 3);
来源：http://evi.yj202588.top

[S17] C：安全拼接字符串
来源：http://xfg.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bok.vqdsnc.cn

[S18] C：命令行参数
来源：http://ycs.jqgufenzy.top

int main(int argc, char **argv)
来源：http://yrj.316326.xyz

[S19] C：快速排序
来源：http://vtl.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://ghu.wangdashe.top

[S20] C：二分查找
来源：http://dtf.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lbj.gogol.net.cn

[S21] C：字符类别判断
来源：http://uwi.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://knb.hfpthk.cn

[S22] C：字符串转数字
来源：http://fmv.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cus.yj20258.top

[S23] C：随机数
来源：http://fds.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ohj.dianchejie.cn

[S24] C：获取本地时间
来源：http://zob.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rys.meibo888.top

[S25] C：内存拷贝
来源：http://agx.yongpay.top

memcpy(dst, src, n);
来源：http://ken.yj202588.top

[S26] C：内存清零
来源：http://xsd.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://pej.zdqjudy.top

[S27] C：定义常量
来源：http://hvk.ppjwa.cn

const double PI = 3.14159;
来源：http://tnw.tianlin.xyz

[S28] C：静态变量
来源：http://mfp.tianlin.xyz

static int counter = 0;
来源：http://ltx.redwolf501.top

[S29] C：变参函数
来源：http://uvk.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ogs.epnwcf.com

[S30] C：头文件保护
来源：http://dqv.xylfe.cn

#ifndef X_H
来源：http://lgb.cheryme.top

#define X_H
来源：http://yzb.hnqzz.top

#endif
来源：http://rrx.wangdashe.top

[S31] C++：Hello World
来源：http://pso.guannengcc.top

#include <iostream>
来源：http://mak.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://dse.jinqigufen.top

[S32] C++：字符串
来源：http://kma.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://njf.yuanzhike.top

[S33] C++：vector 增删
来源：http://xtp.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ify.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://xrb.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://lhg.zycfv.cn

[S35] C++：map
来源：http://aod.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wyl.hfpthk.cn

[S36] C++：unordered_map
来源：http://wys.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ydb.iojbl.cn

[S37] C++：set
来源：http://wgh.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qhn.daxiang520.top

[S38] C++：排序
来源：http://zuc.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://ohg.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://uiw.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jgq.jianghu66.top

[S40] C++：查找元素
来源：http://jvo.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gyd.ivvv.top

[S41] C++：类与构造函数
来源：http://zem.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ock.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://cwj.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://ssa.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://hzy.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://vkz.xinyue.icu

[S44] C++：引用传参
来源：http://xtr.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://bca.xinyue.icu

[S45] C++：lambda
来源：http://ljr.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://vlh.gzhubu.top

[S46] C++：函数模板
来源：http://hjm.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ppm.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://anr.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gdq.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://dqn.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://ohz.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://uvk.jlsjyb.cn

[S49] C++：写文件
来源：http://xcy.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dxq.ctjpmb.com

[S50] C++：格式化数字
来源：http://tsx.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kcq.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://svz.aibaodan.cn

static_cast<double>(a) / b
来源：http://sut.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://gzu.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://bny.nanxinkj.top

[S53] C++：移动语义
来源：http://ovz.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://pex.yanxiufei.cn

[S54] C++：异常处理
来源：http://lkw.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lre.fengsongda.top

[S55] C++：结构化绑定
来源：http://bar.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wtg.zhixingplan.top

[S56] C++：optional
来源：http://quo.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fos.bjfxy.top

[S57] C++：编译期常量
来源：http://nad.uphjek.com

constexpr int N = 10;
来源：http://glh.fengsongda.top

[S58] C++：命名空间
来源：http://pgf.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://jnd.yj202588.top

[S59] C++：静态断言
来源：http://gwe.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vet.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://ijb.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kxm.fktsv.cn

================================================================================
来源：http://wrl.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxr.hesvh.cn

================================================================================
来源：http://ctv.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://hkf.xylfe.cn

println("Hello")
来源：http://dll.jianghu66.top

[T02] Kotlin：变量
来源：http://hxq.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://opx.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://fpp.jyoumei.cn

"值: $b"
来源：http://flw.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://nul.redwolf501.top

val n: String? = null;  n?.length
来源：http://bvw.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://jnq.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jtl.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://gwy.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://sgz.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://sla.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kxw.wangdashe.top

[T08] Kotlin：数据类
来源：http://art.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://gvh.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://wbe.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://cjy.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://bbf.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kzq.aizwys.cn

[T11] Kotlin：协程
来源：http://lic.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fkk.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://ysn.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://jyz.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://fqm.guannengcc.top

val m = mapOf("a" to 1)
来源：http://tjf.dashuyun.cn

[T14] Kotlin：循环
来源：http://vlo.zdqjudy.top

for (i in 1..10) println(i)
来源：http://ulc.tian-w.cn

[T15] Kotlin：接口
来源：http://hli.c1oappe.top

interface Shape { fun area(): Double }
来源：http://sec.jianghu66.top

[T16] Swift：Hello World
来源：http://kju.zhixingplan.top

print("Hello")
来源：http://spn.yj202588.top

[T17] Swift：变量与常量
来源：http://dry.yuxming.cn

var a = 1;  let b = 2
来源：http://pqk.andypj.xyz

[T18] Swift：字符串插值
来源：http://nhp.wangshuangyany.cn

"值: \(b)"
来源：http://cji.hcnkem.com

[T19] Swift：可选绑定
来源：http://hfy.zhixingplan.top

if let n = opt { print(n) }
来源：http://kiz.hysaishi.cn

[T20] Swift：数组操作
来源：http://tfv.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xni.daria6918.cn

[T21] Swift：遍历
来源：http://oez.jyoumei.cn

for x in a { print(x) }
来源：http://iov.aizwys.cn

[T22] Swift：字典
来源：http://qzk.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://xcj.ppjwa.cn

[T23] Swift：函数
来源：http://icm.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://svs.bjfxy.top

[T24] Swift：闭包
来源：http://bqs.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://tpb.jinqigfzy.top

[T25] Swift：结构体
来源：http://cvr.feifeiyinyue.top

struct P { var x: Int }
来源：http://hwn.tianlin.xyz

[T26] Swift：类与重写
来源：http://rge.zdbjq.cn

class A: Base { override func f() {} }
来源：http://aoc.guannengcc.top

[T27] Swift：错误处理
来源：http://sso.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://agx.pengpengdd.cyou

[T28] Swift：枚举
来源：http://zow.quarkkingdee.top

enum Color { case red, green }
来源：http://zzc.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://xtn.guowangkeji.top

guard let x = opt else { return }
来源：http://nvq.svipenyu.cn

[T30] Swift：协议
来源：http://mhq.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://pnq.jinqigufen.top

[T31] Lua：Hello World
来源：http://jhs.ivvv.top

print("Hello")
来源：http://aum.sysykeji.top

[T32] Lua：局部变量
来源：http://dhw.hnqzz.top

local a = 1
来源：http://mtp.xuanzx.com

[T33] Lua：表（数组）
来源：http://ftf.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gkz.xylfe.cn

[T34] Lua：遍历表
来源：http://npm.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wqs.snrcjt.cn

[T35] Lua：字典表
来源：http://snp.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://flk.gzhubu.top

[T36] Lua：函数
来源：http://jyi.zhengqikj.top

function add(a, b) return a + b end
来源：http://eqs.yj202588.top

[T37] Lua：字符串拼接
来源：http://nhi.vehdjk.com

"a" .. "b"
来源：http://ulu.ydjk.org.cn

[T38] Lua：条件
来源：http://lsl.guannengcc.top

if x > 0 then print("正") end
来源：http://lgm.fengsongda.top

[T39] Lua：模式匹配
来源：http://dhr.sjlbkw.cn

string.find(s, "%d+")
来源：http://njb.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://ekz.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://mdz.zdqjudy.top

[T41] Perl：Hello World
来源：http://aqr.svipenyu.cn

print "Hello\n";
来源：http://spc.sufxvd.cn

[T42] Perl：变量类型
来源：http://tjv.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ttz.yj20258.top

[T43] Perl：字符串插值
来源：http://dgd.redwolf501.top

"值: $a"
来源：http://fzm.hesvh.cn

[T44] Perl：条件
来源：http://evw.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://rch.ehwqpu.com

[T45] Perl：数组遍历
来源：http://iog.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://gjr.sysykeji.top

[T46] Perl：哈希操作
来源：http://htm.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://igs.yangfankeji.com

[T47] Perl：正则捕获
来源：http://wka.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qyw.redwolf501.top

[T48] Perl：正则替换
来源：http://vlt.ydzc1.top

$s =~ s/old/new/g;
来源：http://kaj.xziqi.cn

[T49] Perl：函数
来源：http://tgh.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blm.hywenlv.cn

[T50] Perl：逐行读文件
来源：http://lpo.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kym.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://zyq.zhixingplan.top

[T51] Scala：Hello World
来源：http://wfm.cheryme.top

println("Hello")
来源：http://ptj.xuanzx.com

[T52] Scala：变量
来源：http://dii.yfazqb.com


<!-- 参考信息 -->