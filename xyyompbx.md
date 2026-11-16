代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://xin.nanxinkj.top

[R48] awk 取指定列
来源：http://oak.sweek.top

awk '{print $1, $3}' a.txt
来源：http://bay.xylfe.cn

[R49] awk 带条件
来源：http://zud.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://teq.svipenyu.cn

[R50] awk 求和
来源：http://dfd.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://fxm.svipenyu.cn

[R51] 排序去重取前几
来源：http://amj.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://svj.zhengqikj.top

[R52] 统计行数
来源：http://ulf.nwbrower.top

wc -l a.txt
来源：http://biq.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://fwu.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://itf.xylfe.cn

[R54] 比较两个文件
来源：http://ovv.yonumen.top

diff a.txt b.txt
来源：http://aeh.jianghu66.top

[R55] 压缩与解压
来源：http://zwp.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vlm.guowangkeji.top

[R56] 远程拷贝
来源：http://eip.nanxuanxn.top

scp file user@host:/path/
来源：http://iot.cashguo.top

[R57] 远程执行命令
来源：http://msm.yonumen.top

ssh user@host 'uptime'
来源：http://xsq.jinyuanbaomall.cn

[R58] 下载文件
来源：http://hez.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://okd.gzhubu.top

[R59] 发 POST JSON
来源：http://xwq.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://erl.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://pad.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blp.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://mjp.xinyue.icu

df -h;  du -sh *
来源：http://uhg.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://zdn.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://bza.hcnkem.com

[R63] 内存与进程
来源：http://cne.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://oma.c1oappe.top

[R64] 结束进程
来源：http://epp.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://twn.vqdsnc.cn

[R65] 查看端口占用
来源：http://ppw.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cwh.jinqigufen.top

[R66] 定时任务
来源：http://vje.meibo888.top

crontab -e;  crontab -l
来源：http://ndz.yj20258888.top

[R67] 生成随机十六进制串
来源：http://smy.gzhubu.top

openssl rand -hex 16
来源：http://hps.epnwcf.com

[R68] 计算文件校验值
来源：http://pjg.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://lqd.quarkkingdee.top

[R69] 生成随机密码
来源：http://kvu.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://ksb.hysaishi.cn

[R70] 时间戳与互转
来源：http://rgg.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://zlg.tanke756.top

[R71] 日期格式化
来源：http://rig.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ksk.sjlbkw.cn

[R72] 等待端口就绪
来源：http://xqs.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://msw.zhongyouzk.top

[R73] 分割大日志
来源：http://ccq.hnqzz.top

split -l 1000 big.log part_
来源：http://dwt.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://lqj.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wss.feifeiyinyue.top

[R75] 导出环境变量
来源：http://jnh.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://vaz.hnxiangtu.top

[R76] 使用临时文件
来源：http://qom.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hsl.9152youxi.cn

[R77] 读取用户输入
来源：http://yht.ydzc1.top

read -rp "请输入: " ans
来源：http://cvd.epnwcf.com

[R78] 交互式菜单
来源：http://rvt.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pfa.havefunace.top

[R79] 解析命令行选项
来源：http://mbm.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oyp.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://njd.ywan-chungtsiang.top

time ./run.sh
来源：http://onu.haohaochexian.top

================================================================================
来源：http://nag.cashguo.top

S. C / C++ 专题
来源：http://jjo.fehbvm.com

================================================================================
来源：http://jly.zhiwuduotai.top

[S01] C：Hello World
来源：http://dao.uphjek.com

#include <stdio.h>
来源：http://gqx.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://joo.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://zpc.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://qju.hnqzz.top

[S03] C：读入整数
来源：http://qeq.aibaodan.cn

int x; scanf("%d", &x);
来源：http://tsl.sweek.top

[S04] C：字符串复制
来源：http://tic.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://mku.jqgfzy.top

[S05] C：字符串长度
来源：http://vgn.hongshengwenyu.top

strlen(s)
来源：http://iuv.haohaochexian.top

[S06] C：字符串比较
来源：http://sxu.sjlbkw.cn

strcmp(a, b) == 0
来源：http://ckx.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://yuh.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kqb.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://tfp.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qob.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://hei.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kes.zhengqikj.top

[S10] C：指针与解引用
来源：http://juo.tian-w.cn

int *p = &a;  *p = 5;
来源：http://dsb.kuanghao11.cn

[S11] C：逐行读文件
来源：http://pao.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://kfc.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zkn.shuidangran.top

fclose(f);
来源：http://lrx.chenjidiqi.icu

[S12] C：写文件
来源：http://lup.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sfa.fengsongda.top

[S13] C：宏定义
来源：http://xyq.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nan.jiagoushi.top

[S14] C：枚举
来源：http://aln.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://aju.fengsongda.top

[S15] C：类型转换
来源：http://jlw.shangyingyoupin.top

(double) a / b
来源：http://myh.bbcook.cn

[S16] C：位操作置位
来源：http://ddb.hesvh.cn

x |= (1 << 3);
来源：http://adn.nwbrower.top

[S17] C：安全拼接字符串
来源：http://nca.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dsf.0kj1m.cn

[S18] C：命令行参数
来源：http://bjb.cqqwz.cn

int main(int argc, char **argv)
来源：http://mcp.gogol.net.cn

[S19] C：快速排序
来源：http://dgk.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lsl.nwbrower.top

[S20] C：二分查找
来源：http://rit.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kws.zhoulong.xyz

[S21] C：字符类别判断
来源：http://xaj.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nrg.yuanzhike.top

[S22] C：字符串转数字
来源：http://uiz.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eie.yj202588.top

[S23] C：随机数
来源：http://dae.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rxg.sxryk.cn

[S24] C：获取本地时间
来源：http://jsb.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sel.shuidangran.top

[S25] C：内存拷贝
来源：http://qvd.ehwqpu.com

memcpy(dst, src, n);
来源：http://rqn.tian-w.cn

[S26] C：内存清零
来源：http://hys.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://wfr.zhiwuduotai.top

[S27] C：定义常量
来源：http://xkz.gogol.net.cn

const double PI = 3.14159;
来源：http://cob.jinghuilouyu.cn

[S28] C：静态变量
来源：http://pum.hongshengwenyu.top

static int counter = 0;
来源：http://ijr.0kj1m.cn

[S29] C：变参函数
来源：http://dha.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ljw.xylfe.cn

[S30] C：头文件保护
来源：http://uzf.hammf.cn

#ifndef X_H
来源：http://lmk.ppjwa.cn

#define X_H
来源：http://nbs.cheryme.top

#endif
来源：http://wks.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://ooq.tian-w.cn

#include <iostream>
来源：http://eiy.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ktq.zhoulong.xyz

[S32] C++：字符串
来源：http://nry.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://drk.jyoumei.cn

[S33] C++：vector 增删
来源：http://wzf.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fdu.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://xys.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://yib.xuetiantiany.cn

[S35] C++：map
来源：http://ldt.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dfy.yfazqb.com

[S36] C++：unordered_map
来源：http://eea.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xok.jiagoushi.top

[S37] C++：set
来源：http://zrm.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gqs.zhaomingkeji.xyz

[S38] C++：排序
来源：http://eww.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://yqq.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://qos.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ugd.aibaodan.cn

[S40] C++：查找元素
来源：http://vxx.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qkl.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://zup.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jnv.hammf.cn

[S42] C++：继承与虚函数
来源：http://nmx.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://wnj.jianghu66.top

[S43] C++：智能指针
来源：http://bew.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://zbp.guowangkeji.top

[S44] C++：引用传参
来源：http://fqd.yj20258.top

void inc(int &x) { ++x; }
来源：http://hlp.vehdjk.com

[S45] C++：lambda
来源：http://qya.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://bak.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://biu.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qeu.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://ibw.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gcg.redwolf501.top

[S48] C++：逐行读文件
来源：http://btx.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ztf.sweek.top

while (std::getline(in, line)) { }
来源：http://tam.shanyushiyangtech.top

[S49] C++：写文件
来源：http://ufq.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ovm.jiagoushi.top

[S50] C++：格式化数字
来源：http://jnu.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ehr.chenzaomai.com

[S51] C++：显式类型转换
来源：http://abc.gaohongyu789.top

static_cast<double>(a) / b
来源：http://wju.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://dea.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://nut.pengpengdd.cyou

[S53] C++：移动语义
来源：http://upa.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://zqh.nwbrower.top

[S54] C++：异常处理
来源：http://xxz.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jwb.jinqigufen.top

[S55] C++：结构化绑定
来源：http://fnv.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jir.zhoulong.xyz

[S56] C++：optional
来源：http://pyx.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kxj.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://six.wangdashe.top

constexpr int N = 10;
来源：http://tah.snrcjt.cn

[S58] C++：命名空间
来源：http://ygu.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://wop.chenjidiqi.icu

[S59] C++：静态断言
来源：http://tqn.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ifj.havefunace.top

[S60] C++：遍历并删除元素
来源：http://edr.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hud.cheryme.top

================================================================================
来源：http://ygq.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ocl.aibaodan.cn

================================================================================
来源：http://hic.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://ppt.guowangkeji.top

println("Hello")
来源：http://tby.yueranfly.top

[T02] Kotlin：变量
来源：http://qsn.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://swk.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://bdm.quarkkingdee.top

"值: $b"
来源：http://ydl.meibo888.top

[T04] Kotlin：空安全
来源：http://cra.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://twk.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://lyi.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uob.aizwys.cn

[T06] Kotlin：集合映射
来源：http://ker.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://syz.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://utw.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://txw.gogol.net.cn

[T08] Kotlin：数据类
来源：http://ahe.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://ewu.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://qwc.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://zxx.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://joz.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gtm.yfazqb.com

[T11] Kotlin：协程
来源：http://hsi.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bcu.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://qys.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://fzm.yongpay.top

[T13] Kotlin：只读 Map
来源：http://oin.pycfn.com

val m = mapOf("a" to 1)
来源：http://icg.yongpay.top

[T14] Kotlin：循环
来源：http://uqa.andypj.xyz

for (i in 1..10) println(i)
来源：http://lvc.jiagoushi.top

[T15] Kotlin：接口
来源：http://ijp.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://lcn.jianghu66.top

[T16] Swift：Hello World
来源：http://pla.jinqigfzy.top

print("Hello")
来源：http://ocp.jiagoushi.top

[T17] Swift：变量与常量
来源：http://wpc.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://fsv.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://ohn.fehbvm.com

"值: \(b)"
来源：http://vit.chenzaomai.com

[T19] Swift：可选绑定
来源：http://vku.ydjk.org.cn

if let n = opt { print(n) }
来源：http://nkv.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://urs.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pwz.bjfxy.top

[T21] Swift：遍历
来源：http://cjo.yanxiufei.cn

for x in a { print(x) }
来源：http://eoz.ctjpmb.com

[T22] Swift：字典
来源：http://tbs.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://kjq.yonumen.top

[T23] Swift：函数
来源：http://egd.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aqs.hnqzz.top

[T24] Swift：闭包
来源：http://wfd.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ikm.jinqigufen.top

[T25] Swift：结构体
来源：http://gxz.tianlin.xyz

struct P { var x: Int }
来源：http://woe.316326.xyz

[T26] Swift：类与重写
来源：http://jgr.xziqi.cn

class A: Base { override func f() {} }
来源：http://gar.bjfxy.top

[T27] Swift：错误处理
来源：http://zur.daxiang520.top

do { try f() } catch { print(error) }
来源：http://lya.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://fpu.yongpay.top

enum Color { case red, green }
来源：http://ssf.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://can.ehwqpu.com

guard let x = opt else { return }
来源：http://qan.yonumen.top

[T30] Swift：协议
来源：http://sxd.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://nch.sjlbkw.cn

[T31] Lua：Hello World
来源：http://bml.dashuyun.cn

print("Hello")
来源：http://zky.dashuyun.cn

[T32] Lua：局部变量
来源：http://qer.pycfn.com

local a = 1
来源：http://jbe.bjfxy.top

[T33] Lua：表（数组）
来源：http://rsr.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zud.cheryme.top

[T34] Lua：遍历表
来源：http://ttb.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://flx.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://vpo.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://nrk.yuanzhike.top

[T36] Lua：函数
来源：http://mts.yuanzhike.top

function add(a, b) return a + b end
来源：http://zsp.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://fiy.redwolf501.top

"a" .. "b"
来源：http://xde.ehwqpu.com

[T38] Lua：条件
来源：http://wnz.guannengcc.top

if x > 0 then print("正") end
来源：http://osg.yj202588.top

[T39] Lua：模式匹配
来源：http://mgp.nanxinkj.top

string.find(s, "%d+")
来源：http://sln.0kj1m.cn

[T40] Lua：元表
来源：http://rgm.52xcode.cn

setmetatable({}, { __index = base })
来源：http://oor.cqqwz.cn

[T41] Perl：Hello World
来源：http://ryi.cdnleiting.top

print "Hello\n";
来源：http://fzh.snrcjt.cn

[T42] Perl：变量类型
来源：http://uft.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czu.dashuyun.cn

[T43] Perl：字符串插值
来源：http://pdx.chenjidiqi.icu

"值: $a"
来源：http://taa.sysykeji.top

[T44] Perl：条件
来源：http://yxq.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://cta.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://dkb.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://ayu.hesvh.cn

[T46] Perl：哈希操作
来源：http://twx.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bat.pycfn.com

[T47] Perl：正则捕获
来源：http://joc.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dgj.sxryk.cn

[T48] Perl：正则替换
来源：http://cfo.tian-w.cn

$s =~ s/old/new/g;
来源：http://piz.haohaochexian.top

[T49] Perl：函数
来源：http://eos.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://luu.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://uqt.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://uvw.gotoacloud.top


<!-- 参考信息 -->