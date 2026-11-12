代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://cms.yueranfly.top

[R48] awk 取指定列
来源：http://esd.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://cdl.zhixingplan.top

[R49] awk 带条件
来源：http://mtd.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avi.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://tff.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xxz.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://ssm.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iug.yj20258888.top

[R52] 统计行数
来源：http://cgz.svipenyu.cn

wc -l a.txt
来源：http://ndk.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://rez.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fqe.feifeiyinyue.top

[R54] 比较两个文件
来源：http://xtt.dianchejie.cn

diff a.txt b.txt
来源：http://che.snrcjt.cn

[R55] 压缩与解压
来源：http://ipd.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ium.daria6918.cn

[R56] 远程拷贝
来源：http://kvf.fengsongda.top

scp file user@host:/path/
来源：http://rvg.yvedp.cn

[R57] 远程执行命令
来源：http://fea.xziqi.cn

ssh user@host 'uptime'
来源：http://giw.epnwcf.com

[R58] 下载文件
来源：http://dee.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xfq.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://rtn.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://prk.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://nyu.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cjx.yj20258.top

[R61] 磁盘占用
来源：http://htj.feifeiyinyue.top

df -h;  du -sh *
来源：http://qiu.guowangkeji.top

[R62] 找最占空间的文件
来源：http://vzd.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://ero.jyoumei.cn

[R63] 内存与进程
来源：http://sbc.yonumen.top

free -h;  ps aux | grep nginx
来源：http://pov.yfazqb.com

[R64] 结束进程
来源：http://sld.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://kip.sjlbkw.cn

[R65] 查看端口占用
来源：http://gpz.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jpy.tanke756.top

[R66] 定时任务
来源：http://gjn.hnxiangtu.top

crontab -e;  crontab -l
来源：http://lmi.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://usq.haohaochexian.top

openssl rand -hex 16
来源：http://xpb.nanxuanxn.top

[R68] 计算文件校验值
来源：http://diq.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://sds.jinqigufen.top

[R69] 生成随机密码
来源：http://smh.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://ces.yfazqb.com

[R70] 时间戳与互转
来源：http://daq.redwolf501.top

date +%s;  date -d @1700000000
来源：http://dei.316326.xyz

[R71] 日期格式化
来源：http://vsy.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fut.nanxuanxn.top

[R72] 等待端口就绪
来源：http://aua.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wrh.shuidangran.top

[R73] 分割大日志
来源：http://msb.zdqjudy.top

split -l 1000 big.log part_
来源：http://otp.gzhubu.top

[R74] 批量重命名
来源：http://ydw.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zhk.yuanzhike.top

[R75] 导出环境变量
来源：http://iok.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://eqe.yuanzhike.top

[R76] 使用临时文件
来源：http://xgm.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lcq.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://edq.ydzc1.top

read -rp "请输入: " ans
来源：http://dmc.fehbvm.com

[R78] 交互式菜单
来源：http://kgb.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uzi.cucudq.cn

[R79] 解析命令行选项
来源：http://baa.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://daw.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://ixa.meibo888.top

time ./run.sh
来源：http://his.jqgufenzy.top

================================================================================
来源：http://hnq.smart0.xyz

S. C / C++ 专题
来源：http://uzz.pengpengdd.cyou

================================================================================
来源：http://pcl.ybcxt.top

[S01] C：Hello World
来源：http://rzz.jqgufenzy.top

#include <stdio.h>
来源：http://tfq.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nnm.fehbvm.com

[S02] C：变量与格式化输出
来源：http://ovg.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://tfv.pycfn.com

[S03] C：读入整数
来源：http://soq.tanke756.top

int x; scanf("%d", &x);
来源：http://olf.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://zdy.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://vfb.yanxiufei.cn

[S05] C：字符串长度
来源：http://xiq.uphjek.com

strlen(s)
来源：http://xmj.shuidangran.top

[S06] C：字符串比较
来源：http://dpz.jianghu66.top

strcmp(a, b) == 0
来源：http://qkv.cdnleiting.top

[S07] C：数组遍历求和
来源：http://zic.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://khm.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://dud.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://caj.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://sqm.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yqp.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://uuj.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://uku.daria6918.cn

[S11] C：逐行读文件
来源：http://cwq.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://jgo.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zib.sufxvd.cn

fclose(f);
来源：http://kep.zhongyouzk.top

[S12] C：写文件
来源：http://jop.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jee.yfazqb.com

[S13] C：宏定义
来源：http://zou.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wuw.yfazqb.com

[S14] C：枚举
来源：http://sof.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://dqw.smart0.xyz

[S15] C：类型转换
来源：http://oav.zhengqikj.top

(double) a / b
来源：http://kjc.ydjk.org.cn

[S16] C：位操作置位
来源：http://yxr.zhixingplan.top

x |= (1 << 3);
来源：http://sgc.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://wif.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ucy.zhongyouzk.top

[S18] C：命令行参数
来源：http://ekt.jqgufenzy.top

int main(int argc, char **argv)
来源：http://czw.ydzc1.top

[S19] C：快速排序
来源：http://mqm.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://vxd.chenlongwang.top

[S20] C：二分查找
来源：http://wkm.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://emp.sufxvd.cn

[S21] C：字符类别判断
来源：http://zkf.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fsa.shzxlz.cn

[S22] C：字符串转数字
来源：http://mum.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://edp.andypj.xyz

[S23] C：随机数
来源：http://oyd.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://xzt.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://aep.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nrd.fzhhl.top

[S25] C：内存拷贝
来源：http://qjd.hcnkem.com

memcpy(dst, src, n);
来源：http://wat.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://dpx.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://tdw.aizwys.cn

[S27] C：定义常量
来源：http://trx.kuanghao11.cn

const double PI = 3.14159;
来源：http://ykr.yj20258888.top

[S28] C：静态变量
来源：http://nfo.zhixingplan.top

static int counter = 0;
来源：http://npl.hongshengwenyu.top

[S29] C：变参函数
来源：http://wdq.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cip.xinyue.icu

[S30] C：头文件保护
来源：http://rew.hongshengwenyu.top

#ifndef X_H
来源：http://xal.yueranfly.top

#define X_H
来源：http://qfb.dianchejie.cn

#endif
来源：http://lmh.zhixingplan.top

[S31] C++：Hello World
来源：http://xfv.zhixingplan.top

#include <iostream>
来源：http://qgs.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://ngy.redwolf501.top

[S32] C++：字符串
来源：http://jpn.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://pkh.meibo888.top

[S33] C++：vector 增删
来源：http://kaj.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://atm.yuxming.cn

[S34] C++：遍历 vector
来源：http://pqd.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://eia.hesvh.cn

[S35] C++：map
来源：http://veh.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bme.ivvv.top

[S36] C++：unordered_map
来源：http://nrw.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sxm.cheryme.top

[S37] C++：set
来源：http://alk.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ceg.shanyushiyangkeji.top

[S38] C++：排序
来源：http://jpo.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://mwl.pycfn.com

[S39] C++：自定义比较器排序
来源：http://wpr.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iaj.hesvh.cn

[S40] C++：查找元素
来源：http://zjq.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lvh.nanxinkj.top

[S41] C++：类与构造函数
来源：http://yym.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://teh.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://wvg.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://sic.xuetiantiany.cn

[S43] C++：智能指针
来源：http://whf.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://jyr.ehwqpu.com

[S44] C++：引用传参
来源：http://ndi.andypj.xyz

void inc(int &x) { ++x; }
来源：http://izv.mhx1999.top

[S45] C++：lambda
来源：http://sfv.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://hxd.zycfv.cn

[S46] C++：函数模板
来源：http://otb.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cna.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://nfb.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dip.0kj1m.cn

[S48] C++：逐行读文件
来源：http://qae.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://ozb.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://hef.andypj.xyz

[S49] C++：写文件
来源：http://nir.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qzz.gotoacloud.top

[S50] C++：格式化数字
来源：http://sug.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jgc.andypj.xyz

[S51] C++：显式类型转换
来源：http://ijv.hcnkem.com

static_cast<double>(a) / b
来源：http://fri.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://pbb.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://bfy.kuanghao11.cn

[S53] C++：移动语义
来源：http://tyb.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://miu.haohaochexian.top

[S54] C++：异常处理
来源：http://fqf.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tag.hammf.cn

[S55] C++：结构化绑定
来源：http://qra.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pzu.gotoacloud.top

[S56] C++：optional
来源：http://nar.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ndz.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://iel.yj20258888.top

constexpr int N = 10;
来源：http://hsu.sjlbkw.cn

[S58] C++：命名空间
来源：http://sbe.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://ydo.vqdsnc.cn

[S59] C++：静态断言
来源：http://osk.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ssw.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://oko.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vrb.gogol.net.cn

================================================================================
来源：http://uet.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbr.jlsjyb.cn

================================================================================
来源：http://qvr.yj202588.top

[T01] Kotlin：Hello World
来源：http://shh.bjfxy.top

println("Hello")
来源：http://owg.guowangkeji.top

[T02] Kotlin：变量
来源：http://bhh.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lhx.cheryme.top

[T03] Kotlin：字符串模板
来源：http://hig.zhoulong.xyz

"值: $b"
来源：http://qta.zycfv.cn

[T04] Kotlin：空安全
来源：http://uyk.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://xxc.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://tvt.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ifq.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://sfe.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dyv.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://aaj.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tqx.yj20258.top

[T08] Kotlin：数据类
来源：http://guv.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://jkh.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://niu.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://rko.c1oappe.top

[T10] Kotlin：默认参数
来源：http://xki.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://siu.hcnkem.com

[T11] Kotlin：协程
来源：http://whx.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bob.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://ape.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://nwn.ivvv.top

[T13] Kotlin：只读 Map
来源：http://rlh.daria6918.cn

val m = mapOf("a" to 1)
来源：http://myd.zhixingplan.top

[T14] Kotlin：循环
来源：http://wzm.tian-w.cn

for (i in 1..10) println(i)
来源：http://aan.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://ene.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://pbr.sweek.top

[T16] Swift：Hello World
来源：http://xci.chenlongwang.top

print("Hello")
来源：http://oku.c1oappe.top

[T17] Swift：变量与常量
来源：http://gqo.mhx1999.top

var a = 1;  let b = 2
来源：http://bnd.yj20258.top

[T18] Swift：字符串插值
来源：http://lvw.tanke756.top

"值: \(b)"
来源：http://nmg.daria6918.cn

[T19] Swift：可选绑定
来源：http://iwj.yvedp.cn

if let n = opt { print(n) }
来源：http://wor.redwolf501.top

[T20] Swift：数组操作
来源：http://lae.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://niw.iojbl.cn

[T21] Swift：遍历
来源：http://crh.mhx1999.top

for x in a { print(x) }
来源：http://ued.yonumen.top

[T22] Swift：字典
来源：http://vnu.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://pfz.zhongyouzk.top

[T23] Swift：函数
来源：http://npl.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qya.daxiang520.top

[T24] Swift：闭包
来源：http://xsr.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dnv.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://dxs.yanxiufei.cn

struct P { var x: Int }
来源：http://ewk.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://kye.jianghu66.top

class A: Base { override func f() {} }
来源：http://bwo.fktsv.cn

[T27] Swift：错误处理
来源：http://rca.cheryme.top

do { try f() } catch { print(error) }
来源：http://tca.zhengqikj.top

[T28] Swift：枚举
来源：http://dha.shangyingyoupin.top

enum Color { case red, green }
来源：http://pjv.sweek.top

[T29] Swift：guard 提前返回
来源：http://ytc.zhongyouzk.top

guard let x = opt else { return }
来源：http://arr.zhengqikj.top

[T30] Swift：协议
来源：http://aoc.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://dja.fehbvm.com

[T31] Lua：Hello World
来源：http://zxh.cqqwz.cn

print("Hello")
来源：http://wuq.bbcook.cn

[T32] Lua：局部变量
来源：http://oox.dashuyun.cn

local a = 1
来源：http://ttw.xinyue.icu

[T33] Lua：表（数组）
来源：http://ofa.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://prd.sjlbkw.cn

[T34] Lua：遍历表
来源：http://dmb.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dlp.haohaochexian.top

[T35] Lua：字典表
来源：http://xye.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://rli.gaohongyu789.top

[T36] Lua：函数
来源：http://nzq.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://hry.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://jsi.ivvv.top

"a" .. "b"
来源：http://ois.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://lba.cheryme.top

if x > 0 then print("正") end
来源：http://qpt.jqgfzy.top

[T39] Lua：模式匹配
来源：http://bko.jianghu66.top

string.find(s, "%d+")
来源：http://gyb.yonumen.top

[T40] Lua：元表
来源：http://ojo.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://nvx.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://afc.haohaochexian.top

print "Hello\n";
来源：http://vpb.hammf.cn

[T42] Perl：变量类型
来源：http://duo.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ijd.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://eja.316326.xyz

"值: $a"
来源：http://tod.havefunace.top

[T44] Perl：条件
来源：http://vqv.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://rpc.sweek.top

[T45] Perl：数组遍历
来源：http://zit.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://uvn.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://mvb.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zyl.jinqigufen.top

[T47] Perl：正则捕获
来源：http://pnl.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pkm.chenlongwang.top

[T48] Perl：正则替换
来源：http://iqj.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://qba.bjfxy.top

[T49] Perl：函数
来源：http://bpg.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dkm.xuanzx.com

[T50] Perl：逐行读文件
来源：http://kmk.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://onc.meibo888.top


<!-- 参考信息 -->