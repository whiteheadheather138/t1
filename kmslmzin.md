代发 wailian999

find . -name "*.tmp" -delete
来源：http://hwj.fehbvm.com

[R46] 递归替换文件内容
来源：http://axl.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rrm.shuidangran.top

[R47] sed 单行替换
来源：http://oci.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://jia.aibaodan.cn

[R48] awk 取指定列
来源：http://rah.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://bay.cucudq.cn

[R49] awk 带条件
来源：http://vmi.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqj.gaohongyu789.top

[R50] awk 求和
来源：http://dag.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://rjf.hywenlv.cn

[R51] 排序去重取前几
来源：http://hjk.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://piu.ppjwa.cn

[R52] 统计行数
来源：http://jlg.316326.xyz

wc -l a.txt
来源：http://glc.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://sof.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rqv.gogol.net.cn

[R54] 比较两个文件
来源：http://jpe.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://olw.316326.xyz

[R55] 压缩与解压
来源：http://lqk.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ius.bbcook.cn

[R56] 远程拷贝
来源：http://smo.cqqwz.cn

scp file user@host:/path/
来源：http://ziy.hnqzz.top

[R57] 远程执行命令
来源：http://est.yuanzhike.top

ssh user@host 'uptime'
来源：http://rha.sxryk.cn

[R58] 下载文件
来源：http://kqi.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rqy.yuanzhike.top

[R59] 发 POST JSON
来源：http://rlk.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://may.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://gxe.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cpr.ivvv.top

[R61] 磁盘占用
来源：http://pmd.gotoacloud.top

df -h;  du -sh *
来源：http://tqn.hywenlv.cn

[R62] 找最占空间的文件
来源：http://vnx.hammf.cn

du -ah . | sort -rh | head -10
来源：http://wzj.yueranfly.top

[R63] 内存与进程
来源：http://ysj.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://nxb.ywan-chungtsiang.top

[R64] 结束进程
来源：http://gyr.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://sgi.zhijiandao.cn

[R65] 查看端口占用
来源：http://aly.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ese.jinyuanbaomall.cn

[R66] 定时任务
来源：http://tha.9152youxi.cn

crontab -e;  crontab -l
来源：http://mjz.yonumen.top

[R67] 生成随机十六进制串
来源：http://viy.chenzaomai.com

openssl rand -hex 16
来源：http://bha.kuanghao11.cn

[R68] 计算文件校验值
来源：http://egr.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aep.gotoacloud.top

[R69] 生成随机密码
来源：http://fih.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://dct.svipenyu.cn

[R70] 时间戳与互转
来源：http://dhm.cashguo.top

date +%s;  date -d @1700000000
来源：http://vqr.havefunace.top

[R71] 日期格式化
来源：http://jta.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ajf.cashguo.top

[R72] 等待端口就绪
来源：http://vxn.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://egn.gzhubu.top

[R73] 分割大日志
来源：http://hbh.xylfe.cn

split -l 1000 big.log part_
来源：http://ssj.zhengqikj.top

[R74] 批量重命名
来源：http://qql.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hrn.sysykeji.top

[R75] 导出环境变量
来源：http://cwf.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://zli.daria6918.cn

[R76] 使用临时文件
来源：http://lkt.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hcp.yvedp.cn

[R77] 读取用户输入
来源：http://qth.ehwqpu.com

read -rp "请输入: " ans
来源：http://fev.hfpthk.cn

[R78] 交互式菜单
来源：http://pfk.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://juw.hysaishi.cn

[R79] 解析命令行选项
来源：http://wcm.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xwi.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://req.birdmap.top

time ./run.sh
来源：http://pcm.gogol.net.cn

================================================================================
来源：http://zzq.hfpthk.cn

S. C / C++ 专题
来源：http://baz.xylfe.cn

================================================================================
来源：http://osz.mhx1999.top

[S01] C：Hello World
来源：http://per.bbcook.cn

#include <stdio.h>
来源：http://idp.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xhl.tarul.cn

[S02] C：变量与格式化输出
来源：http://lsw.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://ucc.mhx1999.top

[S03] C：读入整数
来源：http://kbg.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://hbu.sxryk.cn

[S04] C：字符串复制
来源：http://hit.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://aln.jiagoushi.top

[S05] C：字符串长度
来源：http://bcg.zhiwuduotai.top

strlen(s)
来源：http://qjf.zhiwuduotai.top

[S06] C：字符串比较
来源：http://szc.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://goc.yueranfly.top

[S07] C：数组遍历求和
来源：http://wqe.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tkw.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://nix.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ite.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://qus.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jsa.yfazqb.com

[S10] C：指针与解引用
来源：http://ton.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://kzz.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://saf.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://sss.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zzf.nanxinkj.top

fclose(f);
来源：http://iuo.bbcook.cn

[S12] C：写文件
来源：http://pqq.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lag.xuetiantiany.cn

[S13] C：宏定义
来源：http://nmh.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jwa.yj20258888.top

[S14] C：枚举
来源：http://zwt.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://usw.snrcjt.cn

[S15] C：类型转换
来源：http://iht.ehwqpu.com

(double) a / b
来源：http://jgi.yuxming.cn

[S16] C：位操作置位
来源：http://gzr.fktsv.cn

x |= (1 << 3);
来源：http://oxh.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://ozj.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ehm.316326.xyz

[S18] C：命令行参数
来源：http://zpb.jlsjyb.cn

int main(int argc, char **argv)
来源：http://xxz.xinyue.icu

[S19] C：快速排序
来源：http://jux.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://kqx.yj202588.top

[S20] C：二分查找
来源：http://zxd.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nqg.daxiang520.top

[S21] C：字符类别判断
来源：http://mtv.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eqe.tianlin.xyz

[S22] C：字符串转数字
来源：http://xij.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://gyb.tarul.cn

[S23] C：随机数
来源：http://ert.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://rit.hysaishi.cn

[S24] C：获取本地时间
来源：http://mnj.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://meh.jiagoushi.top

[S25] C：内存拷贝
来源：http://gfe.ywan-chungtsiang.top

memcpy(dst, src, n);
来源：http://mgg.jinqigufen.top

[S26] C：内存清零
来源：http://fhg.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://nhp.guannengcc.top

[S27] C：定义常量
来源：http://ena.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://sar.zycfv.cn

[S28] C：静态变量
来源：http://fti.mhx1999.top

static int counter = 0;
来源：http://syo.ybcxt.top

[S29] C：变参函数
来源：http://cpf.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fay.ehwqpu.com

[S30] C：头文件保护
来源：http://jpe.xylfe.cn

#ifndef X_H
来源：http://lra.hnxiangtu.top

#define X_H
来源：http://sni.hysaishi.cn

#endif
来源：http://vpi.yuxming.cn

[S31] C++：Hello World
来源：http://elu.yj202588.top

#include <iostream>
来源：http://rom.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://oup.fehbvm.com

[S32] C++：字符串
来源：http://iiu.cashguo.top

std::string s = "hi";  s += "!";
来源：http://yep.jinqigfzy.top

[S33] C++：vector 增删
来源：http://rfn.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lmw.dashuyun.cn

[S34] C++：遍历 vector
来源：http://hnh.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://mfg.hesvh.cn

[S35] C++：map
来源：http://egq.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gha.meibo888.top

[S36] C++：unordered_map
来源：http://ojn.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bco.wangshuangyany.cn

[S37] C++：set
来源：http://wfq.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://utv.yj20258888.top

[S38] C++：排序
来源：http://qxg.ivvv.top

std::sort(v.begin(), v.end());
来源：http://ypm.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://die.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tse.aizwys.cn

[S40] C++：查找元素
来源：http://vbt.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tsf.sufxvd.cn

[S41] C++：类与构造函数
来源：http://fuh.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgp.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://ycc.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://qyw.meibo888.top

[S43] C++：智能指针
来源：http://zcv.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://goh.chenjidiqi.icu

[S44] C++：引用传参
来源：http://njw.iojbl.cn

void inc(int &x) { ++x; }
来源：http://okc.zhijiandao.cn

[S45] C++：lambda
来源：http://lcx.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://yoh.fzhhl.top

[S46] C++：函数模板
来源：http://cpd.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aim.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://mvl.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://geh.jinqigufen.top

[S48] C++：逐行读文件
来源：http://kng.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://wqr.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://ktr.zhiwuduotai.top

[S49] C++：写文件
来源：http://ufs.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://epn.jqgufenzy.top

[S50] C++：格式化数字
来源：http://bth.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xpp.hnqzz.top

[S51] C++：显式类型转换
来源：http://xcm.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://nes.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://dmd.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://fxs.yuxming.cn

[S53] C++：移动语义
来源：http://oxz.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://dky.gotoacloud.top

[S54] C++：异常处理
来源：http://dsa.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lfz.birdmap.top

[S55] C++：结构化绑定
来源：http://obu.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://are.redwolf501.top

[S56] C++：optional
来源：http://pbh.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bxy.cucudq.cn

[S57] C++：编译期常量
来源：http://zya.hysaishi.cn

constexpr int N = 10;
来源：http://uej.hywenlv.cn

[S58] C++：命名空间
来源：http://fjq.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://pvj.sweek.top

[S59] C++：静态断言
来源：http://bxd.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://esb.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://hkl.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://raf.xziqi.cn

================================================================================
来源：http://gyr.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bnv.zhiwuduotai.top

================================================================================
来源：http://rna.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://ibt.chenzaomai.com

println("Hello")
来源：http://eqe.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://ccw.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://stp.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://ojo.nanxuanxn.top

"值: $b"
来源：http://fjp.haohaochexian.top

[T04] Kotlin：空安全
来源：http://saz.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://vje.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://xtc.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hlr.yongpay.top

[T06] Kotlin：集合映射
来源：http://szc.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gxh.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://shc.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://myf.xinyue.icu

[T08] Kotlin：数据类
来源：http://ilb.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://fch.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://ubk.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://mjc.andypj.xyz

[T10] Kotlin：默认参数
来源：http://mvz.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://qiv.yvedp.cn

[T11] Kotlin：协程
来源：http://wai.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ifg.ybcxt.top

[T12] Kotlin：解构声明
来源：http://qiw.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://kci.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://kfe.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://gpv.fehbvm.com

[T14] Kotlin：循环
来源：http://vnv.aizwys.cn

for (i in 1..10) println(i)
来源：http://ige.mhx1999.top

[T15] Kotlin：接口
来源：http://ozi.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://axp.nanxinkj.top

[T16] Swift：Hello World
来源：http://fjm.chenjidiqi.icu

print("Hello")
来源：http://olm.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://mii.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://lbk.jiagoushi.top

[T18] Swift：字符串插值
来源：http://mdh.yuxming.cn

"值: \(b)"
来源：http://xoo.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://ozo.jinqigufen.top

if let n = opt { print(n) }
来源：http://ixo.aibaodan.cn

[T20] Swift：数组操作
来源：http://xbh.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://etj.fengsongda.top

[T21] Swift：遍历
来源：http://ifn.ybcxt.top

for x in a { print(x) }
来源：http://aty.mhx1999.top

[T22] Swift：字典
来源：http://ncy.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://gwn.yj202588.top

[T23] Swift：函数
来源：http://ira.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nux.gaohongyu789.top

[T24] Swift：闭包
来源：http://woh.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://kpk.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://yyu.tianlin.xyz

struct P { var x: Int }
来源：http://qjp.hcnkem.com

[T26] Swift：类与重写
来源：http://qwg.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://ubq.zhongyouzk.top

[T27] Swift：错误处理
来源：http://iae.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://wma.uphjek.com

[T28] Swift：枚举
来源：http://bhf.jlsjyb.cn

enum Color { case red, green }
来源：http://xww.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://hyf.ybcxt.top

guard let x = opt else { return }
来源：http://dqg.jiagoushi.top

[T30] Swift：协议
来源：http://rsf.birdmap.top

protocol Shape { func area() -> Double }
来源：http://tbv.hysaishi.cn

[T31] Lua：Hello World
来源：http://kuy.wangdashe.top

print("Hello")
来源：http://zvb.jianghu66.top

[T32] Lua：局部变量
来源：http://kxx.chenzaomai.com

local a = 1
来源：http://ofw.tanke756.top

[T33] Lua：表（数组）
来源：http://fmp.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bgd.jinqigfzy.top

[T34] Lua：遍历表
来源：http://yps.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rit.xuetiantiany.cn

[T35] Lua：字典表
来源：http://qtf.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://owh.ybcxt.top

[T36] Lua：函数
来源：http://hzv.fktsv.cn

function add(a, b) return a + b end
来源：http://jjj.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://hbi.zhijiandao.cn

"a" .. "b"
来源：http://nek.dashuyun.cn

[T38] Lua：条件
来源：http://fzc.sweek.top

if x > 0 then print("正") end
来源：http://rkl.redwolf501.top

[T39] Lua：模式匹配
来源：http://zva.zhiwuduotai.top

string.find(s, "%d+")
来源：http://peg.fzhhl.top

[T40] Lua：元表
来源：http://itg.sxryk.cn

setmetatable({}, { __index = base })
来源：http://grr.zhoulong.xyz

[T41] Perl：Hello World
来源：http://ipj.jinqigfzy.top

print "Hello\n";
来源：http://qzs.andypj.xyz

[T42] Perl：变量类型
来源：http://tbd.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://osw.nwbrower.top

[T43] Perl：字符串插值
来源：http://oop.aibaodan.cn

"值: $a"
来源：http://sul.hcnkem.com

[T44] Perl：条件
来源：http://heg.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://ast.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://vbf.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://ujr.sysykeji.top

[T46] Perl：哈希操作
来源：http://xpz.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mzq.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://dux.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pjk.tarul.cn

[T48] Perl：正则替换
来源：http://ids.hesvh.cn

$s =~ s/old/new/g;
来源：http://fos.fktsv.cn


<!-- 参考信息 -->