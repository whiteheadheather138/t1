代发 wailian999

cmd >/dev/null 2>&1
来源：http://hgk.snrcjt.cn

[R42] 输入重定向
来源：http://wce.yongpay.top

wc -l < a.txt
来源：http://yns.zdqjudy.top

[R43] 按名字查找文件
来源：http://xhx.xuanzx.com

find . -name "*.log" -type f
来源：http://yhg.9152youxi.cn

[R44] 按修改时间查找
来源：http://oib.aizwys.cn

find . -mtime -7 -type f
来源：http://lqi.iojbl.cn

[R45] 批量删除
来源：http://ooh.yj202588.top

find . -name "*.tmp" -delete
来源：http://pid.dashuyun.cn

[R46] 递归替换文件内容
来源：http://saw.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ybm.sufxvd.cn

[R47] sed 单行替换
来源：http://uxn.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tvz.yonumen.top

[R48] awk 取指定列
来源：http://ehr.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://aqv.hesvh.cn

[R49] awk 带条件
来源：http://qpf.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bbi.tarul.cn

[R50] awk 求和
来源：http://suq.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://nxh.zycfv.cn

[R51] 排序去重取前几
来源：http://ohs.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fgh.quarkkingdee.top

[R52] 统计行数
来源：http://gaz.jianghu66.top

wc -l a.txt
来源：http://wlj.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://img.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pxb.guannengcc.top

[R54] 比较两个文件
来源：http://llg.yj20258.top

diff a.txt b.txt
来源：http://tsg.sysykeji.top

[R55] 压缩与解压
来源：http://jgt.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fkc.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://bwo.nwbrower.top

scp file user@host:/path/
来源：http://fec.zhongyouzk.top

[R57] 远程执行命令
来源：http://stf.yonumen.top

ssh user@host 'uptime'
来源：http://xae.hnxiangtu.top

[R58] 下载文件
来源：http://hpu.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aae.316326.xyz

[R59] 发 POST JSON
来源：http://nyt.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rea.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://oek.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nbf.aibaodan.cn

[R61] 磁盘占用
来源：http://rpv.havefunace.top

df -h;  du -sh *
来源：http://sim.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://baf.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://eti.sweek.top

[R63] 内存与进程
来源：http://mfk.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://dnj.zdbjq.cn

[R64] 结束进程
来源：http://jns.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://emv.sweek.top

[R65] 查看端口占用
来源：http://jmc.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tst.epnwcf.com

[R66] 定时任务
来源：http://wsm.sufxvd.cn

crontab -e;  crontab -l
来源：http://eqf.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://xnb.xuetiantiany.cn

openssl rand -hex 16
来源：http://ptz.vqdsnc.cn

[R68] 计算文件校验值
来源：http://our.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yjg.zhoulong.xyz

[R69] 生成随机密码
来源：http://rgu.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://yri.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://yql.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://eus.jyoumei.cn

[R71] 日期格式化
来源：http://kii.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pfd.tian-w.cn

[R72] 等待端口就绪
来源：http://jdl.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zir.hfpthk.cn

[R73] 分割大日志
来源：http://wry.meibo888.top

split -l 1000 big.log part_
来源：http://hvy.52xcode.cn

[R74] 批量重命名
来源：http://pay.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ptm.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://exm.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://xoa.ydzc1.top

[R76] 使用临时文件
来源：http://fuv.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iqo.gzhubu.top

[R77] 读取用户输入
来源：http://bsv.ehwqpu.com

read -rp "请输入: " ans
来源：http://usm.52xcode.cn

[R78] 交互式菜单
来源：http://mjc.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tce.aizwys.cn

[R79] 解析命令行选项
来源：http://dus.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rmp.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://mji.c1oappe.top

time ./run.sh
来源：http://oww.chenzaomai.com

================================================================================
来源：http://lhh.ehwqpu.com

S. C / C++ 专题
来源：http://fvv.yonumen.top

================================================================================
来源：http://mlj.xuetiantiany.cn

[S01] C：Hello World
来源：http://mzh.jinghuilouyu.cn

#include <stdio.h>
来源：http://diy.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://amp.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://jxr.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://mbu.havefunace.top

[S03] C：读入整数
来源：http://kpa.0kj1m.cn

int x; scanf("%d", &x);
来源：http://ppy.cqqwz.cn

[S04] C：字符串复制
来源：http://mco.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://uyz.uphjek.com

[S05] C：字符串长度
来源：http://hgl.shzxlz.cn

strlen(s)
来源：http://ijg.xuanzx.com

[S06] C：字符串比较
来源：http://ehz.hesvh.cn

strcmp(a, b) == 0
来源：http://shh.cqqwz.cn

[S07] C：数组遍历求和
来源：http://frp.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fbf.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://pfo.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hks.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://roj.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hrx.guowangkeji.top

[S10] C：指针与解引用
来源：http://fon.mhx1999.top

int *p = &a;  *p = 5;
来源：http://uhd.jinqigufen.top

[S11] C：逐行读文件
来源：http://ygr.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://fwk.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://tje.haohaochexian.top

fclose(f);
来源：http://obw.ywan-chungtsiang.top

[S12] C：写文件
来源：http://gue.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qve.yanxiufei.cn

[S13] C：宏定义
来源：http://zjs.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qnu.pycfn.com

[S14] C：枚举
来源：http://lhr.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://xkg.mhx1999.top

[S15] C：类型转换
来源：http://coj.svipenyu.cn

(double) a / b
来源：http://zzo.zycfv.cn

[S16] C：位操作置位
来源：http://yyc.hongshengwenyu.top

x |= (1 << 3);
来源：http://uor.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://ves.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xcd.birdmap.top

[S18] C：命令行参数
来源：http://odz.hfpthk.cn

int main(int argc, char **argv)
来源：http://lnz.ydjk.org.cn

[S19] C：快速排序
来源：http://dfp.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://bpn.tarul.cn

[S20] C：二分查找
来源：http://sas.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qsu.jinqigfzy.top

[S21] C：字符类别判断
来源：http://amx.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://npk.yuanzhike.top

[S22] C：字符串转数字
来源：http://biu.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://shx.jinqigufen.top

[S23] C：随机数
来源：http://uch.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ena.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://exn.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sqi.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://hnr.xinyue.icu

memcpy(dst, src, n);
来源：http://qbf.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://cdx.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://hfo.nanxinkj.top

[S27] C：定义常量
来源：http://rtf.daria6918.cn

const double PI = 3.14159;
来源：http://ouw.zhongyouzk.top

[S28] C：静态变量
来源：http://fph.fanxiaobao.xyz

static int counter = 0;
来源：http://nqy.shanyushiyangtech.top

[S29] C：变参函数
来源：http://lih.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://put.xuetiantiany.cn

[S30] C：头文件保护
来源：http://bsz.ydjk.org.cn

#ifndef X_H
来源：http://ydg.hesvh.cn

#define X_H
来源：http://fpe.zhoulong.xyz

#endif
来源：http://cmz.mhx1999.top

[S31] C++：Hello World
来源：http://neh.chenjidiqi.icu

#include <iostream>
来源：http://xlh.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://ptt.hongshengwenyu.top

[S32] C++：字符串
来源：http://dya.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://cmo.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://fab.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://auj.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://sup.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://crc.chenlongwang.top

[S35] C++：map
来源：http://jsr.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eci.gogol.net.cn

[S36] C++：unordered_map
来源：http://vkx.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bmw.yj20258888.top

[S37] C++：set
来源：http://ctd.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yon.zhongyouzk.top

[S38] C++：排序
来源：http://yvt.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://rht.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://spy.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tpy.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://acn.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://far.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://tqh.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zug.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://tgm.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://pif.shangyingyoupin.top

[S43] C++：智能指针
来源：http://hdn.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://eui.wangshuangyany.cn

[S44] C++：引用传参
来源：http://bpr.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://edm.hfpthk.cn

[S45] C++：lambda
来源：http://qrr.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jcr.hongshengwenyu.top

[S46] C++：函数模板
来源：http://ela.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kkf.sweek.top

[S47] C++：结构化绑定遍历
来源：http://wxv.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wwo.yj20258.top

[S48] C++：逐行读文件
来源：http://hid.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://xde.yongpay.top

while (std::getline(in, line)) { }
来源：http://mos.nwbrower.top

[S49] C++：写文件
来源：http://hth.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kmn.jianghu66.top

[S50] C++：格式化数字
来源：http://trn.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ovd.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://hdn.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://wbk.ivvv.top

[S52] C++：const 与 noexcept
来源：http://thz.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://vgl.ehwqpu.com

[S53] C++：移动语义
来源：http://tiw.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://uly.xinyue.icu

[S54] C++：异常处理
来源：http://wrr.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oyt.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://xhz.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://prx.fzhhl.top

[S56] C++：optional
来源：http://ush.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://csg.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://lsv.tarul.cn

constexpr int N = 10;
来源：http://hgu.zhiwuduotai.top

[S58] C++：命名空间
来源：http://ojq.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://hik.cqqwz.cn

[S59] C++：静态断言
来源：http://eos.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://csf.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://mig.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ksi.shanyushiyangtech.top

================================================================================
来源：http://hsk.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oez.snrcjt.cn

================================================================================
来源：http://khc.fktsv.cn

[T01] Kotlin：Hello World
来源：http://bst.nwbrower.top

println("Hello")
来源：http://cvv.nanxinkj.top

[T02] Kotlin：变量
来源：http://ehj.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zlq.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://kzw.fzhhl.top

"值: $b"
来源：http://fmi.yonumen.top

[T04] Kotlin：空安全
来源：http://srp.bbcook.cn

val n: String? = null;  n?.length
来源：http://nhi.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://hrh.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nci.xylfe.cn

[T06] Kotlin：集合映射
来源：http://ctd.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nyd.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://wuo.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zdm.xylfe.cn

[T08] Kotlin：数据类
来源：http://hgg.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://nqv.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://ljz.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://fan.vehdjk.com

[T10] Kotlin：默认参数
来源：http://off.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mxs.hysaishi.cn

[T11] Kotlin：协程
来源：http://jvx.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zha.ivvv.top

[T12] Kotlin：解构声明
来源：http://yzj.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://vbz.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://amg.wangdashe.top

val m = mapOf("a" to 1)
来源：http://gny.xuanzx.com

[T14] Kotlin：循环
来源：http://ovt.guowangkeji.top

for (i in 1..10) println(i)
来源：http://xtx.meibo888.top

[T15] Kotlin：接口
来源：http://sal.iojbl.cn

interface Shape { fun area(): Double }
来源：http://ery.52xcode.cn

[T16] Swift：Hello World
来源：http://yvb.pycfn.com

print("Hello")
来源：http://lsq.hysaishi.cn

[T17] Swift：变量与常量
来源：http://nfp.fengsongda.top

var a = 1;  let b = 2
来源：http://zdv.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://nuy.jinghuilouyu.cn

"值: \(b)"
来源：http://cdz.cheryme.top

[T19] Swift：可选绑定
来源：http://fhv.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://jpo.ybcxt.top

[T20] Swift：数组操作
来源：http://ytc.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://nqh.cdnleiting.top

[T21] Swift：遍历
来源：http://dbz.wangdashe.top

for x in a { print(x) }
来源：http://hvx.hywenlv.cn

[T22] Swift：字典
来源：http://vug.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://bmv.dianchejie.cn

[T23] Swift：函数
来源：http://mhr.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kbp.9152youxi.cn

[T24] Swift：闭包
来源：http://uwv.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ukd.cheryme.top

[T25] Swift：结构体
来源：http://lri.mhx1999.top

struct P { var x: Int }
来源：http://cyz.nanxinkj.top

[T26] Swift：类与重写
来源：http://lts.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://tzi.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://wna.daria6918.cn

do { try f() } catch { print(error) }
来源：http://syh.shuidangran.top

[T28] Swift：枚举
来源：http://mvi.ppjwa.cn

enum Color { case red, green }
来源：http://tjn.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://gki.chenlongwang.top

guard let x = opt else { return }
来源：http://kvf.jqgfzy.top

[T30] Swift：协议
来源：http://bpm.ydjk.org.cn

protocol Shape { func area() -> Double }
来源：http://mbi.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://nqx.xziqi.cn

print("Hello")
来源：http://ksz.yanxiufei.cn

[T32] Lua：局部变量
来源：http://jts.jinqigufen.top

local a = 1
来源：http://ylm.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://fbm.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mkd.yangfankeji.com

[T34] Lua：遍历表
来源：http://fkx.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://apt.hnqzz.top

[T35] Lua：字典表
来源：http://djj.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://agc.gzhubu.top

[T36] Lua：函数
来源：http://drg.daxiang520.top

function add(a, b) return a + b end
来源：http://wur.hesvh.cn

[T37] Lua：字符串拼接
来源：http://juj.jlsjyb.cn

"a" .. "b"
来源：http://hxc.yfazqb.com

[T38] Lua：条件
来源：http://fpy.meibo888.top

if x > 0 then print("正") end
来源：http://wel.zycfv.cn

[T39] Lua：模式匹配
来源：http://lbh.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://tuc.feifeiyinyue.top

[T40] Lua：元表
来源：http://ynu.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://eft.aizwys.cn

[T41] Perl：Hello World
来源：http://kmj.52xcode.cn

print "Hello\n";
来源：http://eip.yangfankeji.com

[T42] Perl：变量类型
来源：http://vfh.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kgq.wangdashe.top

[T43] Perl：字符串插值
来源：http://rot.ctjpmb.com

"值: $a"
来源：http://zzz.feifeiyinyue.top

[T44] Perl：条件
来源：http://mqy.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://fyn.nanxuanxn.top


<!-- 参考信息 -->