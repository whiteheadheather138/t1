代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://brw.yanxiufei.cn

[R48] awk 取指定列
来源：http://pnv.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://yrq.nwbrower.top

[R49] awk 带条件
来源：http://lzo.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://goc.quarkkingdee.top

[R50] awk 求和
来源：http://nww.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://vum.52xcode.cn

[R51] 排序去重取前几
来源：http://ydh.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://utv.jinqigufen.top

[R52] 统计行数
来源：http://puj.ctjpmb.com

wc -l a.txt
来源：http://bxm.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://xoe.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xmk.yj20258888.top

[R54] 比较两个文件
来源：http://hng.xinyue.icu

diff a.txt b.txt
来源：http://ppc.feifeiyinyue.top

[R55] 压缩与解压
来源：http://pic.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://muh.jiagoushi.top

[R56] 远程拷贝
来源：http://jqz.jianghu66.top

scp file user@host:/path/
来源：http://tlv.jianghu66.top

[R57] 远程执行命令
来源：http://bdt.hcnkem.com

ssh user@host 'uptime'
来源：http://yax.sxryk.cn

[R58] 下载文件
来源：http://zps.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxp.zhixingplan.top

[R59] 发 POST JSON
来源：http://qab.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iqs.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://yps.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mgs.mhx1999.top

[R61] 磁盘占用
来源：http://wmo.ybcxt.top

df -h;  du -sh *
来源：http://vqp.jiagoushi.top

[R62] 找最占空间的文件
来源：http://weg.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://xzx.shangyingyoupin.top

[R63] 内存与进程
来源：http://sba.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://trk.meibo888.top

[R64] 结束进程
来源：http://stv.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://puc.xuetiantiany.cn

[R65] 查看端口占用
来源：http://uvz.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpw.cashguo.top

[R66] 定时任务
来源：http://dgu.cqqwz.cn

crontab -e;  crontab -l
来源：http://oga.uphjek.com

[R67] 生成随机十六进制串
来源：http://fdu.nwbrower.top

openssl rand -hex 16
来源：http://dug.daxiang520.top

[R68] 计算文件校验值
来源：http://slp.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gsm.dianchejie.cn

[R69] 生成随机密码
来源：http://wbd.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://xqs.jqgfzy.top

[R70] 时间戳与互转
来源：http://hsy.xuanzx.com

date +%s;  date -d @1700000000
来源：http://vls.xuetiantiany.cn

[R71] 日期格式化
来源：http://dnd.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bwv.wangdashe.top

[R72] 等待端口就绪
来源：http://txc.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://val.epnwcf.com

[R73] 分割大日志
来源：http://pzs.shuidangran.top

split -l 1000 big.log part_
来源：http://oeu.cqqwz.cn

[R74] 批量重命名
来源：http://giw.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uxl.c1oappe.top

[R75] 导出环境变量
来源：http://ydu.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://req.yonumen.top

[R76] 使用临时文件
来源：http://zco.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lbm.jqgfzy.top

[R77] 读取用户输入
来源：http://nmg.yj202588.top

read -rp "请输入: " ans
来源：http://ido.hcnkem.com

[R78] 交互式菜单
来源：http://xvg.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rag.xuanzx.com

[R79] 解析命令行选项
来源：http://rzn.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xyd.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://rfm.ehwqpu.com

time ./run.sh
来源：http://occ.xingfuxueyuan.xyz

================================================================================
来源：http://pjv.cdnleiting.top

S. C / C++ 专题
来源：http://cuy.zhaomingkeji.xyz

================================================================================
来源：http://liu.nanxuanxn.top

[S01] C：Hello World
来源：http://kxa.xylfe.cn

#include <stdio.h>
来源：http://sfj.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dmr.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://bvn.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://dzj.jyoumei.cn

[S03] C：读入整数
来源：http://utt.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://fjv.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://jxb.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dvf.9152youxi.cn

[S05] C：字符串长度
来源：http://mkx.yangfankeji.com

strlen(s)
来源：http://fzi.sweek.top

[S06] C：字符串比较
来源：http://oit.zhongyouzk.top

strcmp(a, b) == 0
来源：http://pvt.hnqzz.top

[S07] C：数组遍历求和
来源：http://iyy.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hrv.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://yib.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://olv.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://eqr.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lrk.yfazqb.com

[S10] C：指针与解引用
来源：http://qct.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://imf.birdmap.top

[S11] C：逐行读文件
来源：http://ril.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://xlk.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vqr.jqgfzy.top

fclose(f);
来源：http://pwq.hfpthk.cn

[S12] C：写文件
来源：http://zoh.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xen.yj202588.top

[S13] C：宏定义
来源：http://hee.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kic.jinghuilouyu.cn

[S14] C：枚举
来源：http://gdc.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://paj.daxiang520.top

[S15] C：类型转换
来源：http://tis.yuanzhike.top

(double) a / b
来源：http://prc.yonumen.top

[S16] C：位操作置位
来源：http://wab.xylfe.cn

x |= (1 << 3);
来源：http://chp.hammf.cn

[S17] C：安全拼接字符串
来源：http://jcp.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jst.birdmap.top

[S18] C：命令行参数
来源：http://djm.yj20258888.top

int main(int argc, char **argv)
来源：http://utr.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://epd.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://txp.hnqzz.top

[S20] C：二分查找
来源：http://vfv.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ldg.smart0.xyz

[S21] C：字符类别判断
来源：http://knm.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wvl.yvedp.cn

[S22] C：字符串转数字
来源：http://jwi.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iyc.nwbrower.top

[S23] C：随机数
来源：http://wqk.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pch.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://jga.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jdw.bjfxy.top

[S25] C：内存拷贝
来源：http://aye.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://mbl.mhx1999.top

[S26] C：内存清零
来源：http://wqe.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://woq.redwolf501.top

[S27] C：定义常量
来源：http://hgx.yj202588.top

const double PI = 3.14159;
来源：http://qay.hammf.cn

[S28] C：静态变量
来源：http://jbv.cashguo.top

static int counter = 0;
来源：http://qcq.sxryk.cn

[S29] C：变参函数
来源：http://ztv.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkn.zycfv.cn

[S30] C：头文件保护
来源：http://che.wangshuangyany.cn

#ifndef X_H
来源：http://oiu.sufxvd.cn

#define X_H
来源：http://ijp.aizwys.cn

#endif
来源：http://iaj.guowangkeji.top

[S31] C++：Hello World
来源：http://cro.cheryme.top

#include <iostream>
来源：http://wfk.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://and.vehdjk.com

[S32] C++：字符串
来源：http://jju.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://ims.sysykeji.top

[S33] C++：vector 增删
来源：http://zqv.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sgp.cucudq.cn

[S34] C++：遍历 vector
来源：http://xbo.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://lga.hcnkem.com

[S35] C++：map
来源：http://fcs.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zec.52xcode.cn

[S36] C++：unordered_map
来源：http://ulh.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aco.yj202588.top

[S37] C++：set
来源：http://myj.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://stj.cdnleiting.top

[S38] C++：排序
来源：http://yiq.yonumen.top

std::sort(v.begin(), v.end());
来源：http://zfd.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://vgr.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wpj.hywenlv.cn

[S40] C++：查找元素
来源：http://sdn.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ini.xinyue.icu

[S41] C++：类与构造函数
来源：http://arb.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dau.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://ksd.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://klb.zhoulong.xyz

[S43] C++：智能指针
来源：http://zwe.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://ekb.andypj.xyz

[S44] C++：引用传参
来源：http://cgo.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://ayk.sweek.top

[S45] C++：lambda
来源：http://rfp.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jog.fktsv.cn

[S46] C++：函数模板
来源：http://ldz.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yfd.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://kpz.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jim.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://yxn.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pjd.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://qpj.jiagoushi.top

[S49] C++：写文件
来源：http://ovo.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://syt.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://zsa.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kkf.cqqwz.cn

[S51] C++：显式类型转换
来源：http://amx.yongpay.top

static_cast<double>(a) / b
来源：http://gum.uphjek.com

[S52] C++：const 与 noexcept
来源：http://dym.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://ypi.mhx1999.top

[S53] C++：移动语义
来源：http://jur.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://xay.uphjek.com

[S54] C++：异常处理
来源：http://tvg.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tta.bjfxy.top

[S55] C++：结构化绑定
来源：http://fjj.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rei.wangshuangyany.cn

[S56] C++：optional
来源：http://ogb.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://quh.gotoacloud.top

[S57] C++：编译期常量
来源：http://qhj.fzhhl.top

constexpr int N = 10;
来源：http://nmy.svipenyu.cn

[S58] C++：命名空间
来源：http://lhh.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://poh.dashuyun.cn

[S59] C++：静态断言
来源：http://hvl.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hgl.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://ldr.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ewn.zhijiandao.cn

================================================================================
来源：http://zwi.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sji.0kj1m.cn

================================================================================
来源：http://oik.yj202588.top

[T01] Kotlin：Hello World
来源：http://krf.cqqwz.cn

println("Hello")
来源：http://zgt.jiagoushi.top

[T02] Kotlin：变量
来源：http://pxj.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tjo.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://qic.sxryk.cn

"值: $b"
来源：http://tto.cheryme.top

[T04] Kotlin：空安全
来源：http://alt.yonumen.top

val n: String? = null;  n?.length
来源：http://wnu.pycfn.com

[T05] Kotlin：when 表达式
来源：http://shb.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uzu.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://upl.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://taw.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://vmn.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://scw.hysaishi.cn

[T08] Kotlin：数据类
来源：http://ezh.yj20258.top

data class User(val name: String, val age: Int)
来源：http://siz.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://gku.yj20258.top

fun String.exclaim() = this + "!"
来源：http://kgb.fzhhl.top

[T10] Kotlin：默认参数
来源：http://vfd.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rcn.birdmap.top

[T11] Kotlin：协程
来源：http://pvx.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jbn.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://yxg.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://yai.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://tlo.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://dhl.bjfxy.top

[T14] Kotlin：循环
来源：http://iwl.tian-w.cn

for (i in 1..10) println(i)
来源：http://dat.snrcjt.cn

[T15] Kotlin：接口
来源：http://atj.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://adb.yj20258888.top

[T16] Swift：Hello World
来源：http://djf.fehbvm.com

print("Hello")
来源：http://pqd.bbcook.cn

[T17] Swift：变量与常量
来源：http://kfk.gzhubu.top

var a = 1;  let b = 2
来源：http://dfn.bjfxy.top

[T18] Swift：字符串插值
来源：http://zwd.snrcjt.cn

"值: \(b)"
来源：http://gij.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://szx.daxiang520.top

if let n = opt { print(n) }
来源：http://vou.chenzaomai.com

[T20] Swift：数组操作
来源：http://zsm.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://npk.gaohongyu789.top

[T21] Swift：遍历
来源：http://snn.xuetiantiany.cn

for x in a { print(x) }
来源：http://mqa.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://tcc.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gyc.gogol.net.cn

[T23] Swift：函数
来源：http://xqg.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ubk.daria6918.cn

[T24] Swift：闭包
来源：http://oqw.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://lce.sysykeji.top

[T25] Swift：结构体
来源：http://jiu.iojbl.cn

struct P { var x: Int }
来源：http://fro.jiagoushi.top

[T26] Swift：类与重写
来源：http://hzr.tanke756.top

class A: Base { override func f() {} }
来源：http://gvx.zhoulong.xyz

[T27] Swift：错误处理
来源：http://xfq.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://gtv.hysaishi.cn

[T28] Swift：枚举
来源：http://tzd.jinqigufen.top

enum Color { case red, green }
来源：http://irb.tarul.cn

[T29] Swift：guard 提前返回
来源：http://sbv.jlsjyb.cn

guard let x = opt else { return }
来源：http://qoi.tianlin.xyz

[T30] Swift：协议
来源：http://gom.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://ppx.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://qhi.zdbjq.cn

print("Hello")
来源：http://yyu.yj202588.top

[T32] Lua：局部变量
来源：http://vuh.ywan-chungtsiang.top

local a = 1
来源：http://vty.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://sbr.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://faw.xuanzx.com

[T34] Lua：遍历表
来源：http://lfi.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pnk.hfpthk.cn

[T35] Lua：字典表
来源：http://dap.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://ske.jinqigufen.top

[T36] Lua：函数
来源：http://ugr.bjfxy.top

function add(a, b) return a + b end
来源：http://vvu.redwolf501.top

[T37] Lua：字符串拼接
来源：http://zkf.yongpay.top

"a" .. "b"
来源：http://aut.sjlbkw.cn

[T38] Lua：条件
来源：http://lfz.nanxinkj.top

if x > 0 then print("正") end
来源：http://tnc.hcnkem.com

[T39] Lua：模式匹配
来源：http://ehz.uphjek.com

string.find(s, "%d+")
来源：http://hhs.xziqi.cn

[T40] Lua：元表
来源：http://nmq.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://ksp.svipenyu.cn

[T41] Perl：Hello World
来源：http://kvd.yonumen.top

print "Hello\n";
来源：http://rqo.zdqjudy.top

[T42] Perl：变量类型
来源：http://szl.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hdp.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://uqi.feifeiyinyue.top

"值: $a"
来源：http://rqq.jinqigfzy.top

[T44] Perl：条件
来源：http://abf.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://kpt.birdmap.top

[T45] Perl：数组遍历
来源：http://mwc.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://lrh.aibaodan.cn

[T46] Perl：哈希操作
来源：http://cii.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vqh.fengsongda.top

[T47] Perl：正则捕获
来源：http://fmw.sweek.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://num.xuanzx.com

[T48] Perl：正则替换
来源：http://dlv.jiagoushi.top

$s =~ s/old/new/g;
来源：http://sju.xylfe.cn

[T49] Perl：函数
来源：http://jqy.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rvd.shuidangran.top

[T50] Perl：逐行读文件
来源：http://wsl.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://vhb.gotoacloud.top


<!-- 参考信息 -->