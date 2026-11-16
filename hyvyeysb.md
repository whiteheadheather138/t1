代发 wailian999

find . -name "*.tmp" -delete
来源：http://cbo.meibo888.top

[R46] 递归替换文件内容
来源：http://nlz.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qat.pengpengdd.cyou

[R47] sed 单行替换
来源：http://nhj.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vxf.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://vlk.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ore.svipenyu.cn

[R49] awk 带条件
来源：http://let.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aro.zdqjudy.top

[R50] awk 求和
来源：http://pjp.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gzi.wangdashe.top

[R51] 排序去重取前几
来源：http://rry.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pwc.shanyushiyangkeji.top

[R52] 统计行数
来源：http://qad.ppjwa.cn

wc -l a.txt
来源：http://ytv.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://vwp.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hka.xinyue.icu

[R54] 比较两个文件
来源：http://akm.andypj.xyz

diff a.txt b.txt
来源：http://wsb.ppjwa.cn

[R55] 压缩与解压
来源：http://bza.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bnr.svipenyu.cn

[R56] 远程拷贝
来源：http://mrm.gzhubu.top

scp file user@host:/path/
来源：http://ynm.zdqjudy.top

[R57] 远程执行命令
来源：http://daz.ctjpmb.com

ssh user@host 'uptime'
来源：http://qxc.smart0.xyz

[R58] 下载文件
来源：http://tgi.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fwo.sufxvd.cn

[R59] 发 POST JSON
来源：http://nwy.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gdv.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://yqo.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://njh.yuanzhike.top

[R61] 磁盘占用
来源：http://zfa.hammf.cn

df -h;  du -sh *
来源：http://xca.hysaishi.cn

[R62] 找最占空间的文件
来源：http://uex.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://rcv.sweek.top

[R63] 内存与进程
来源：http://bzd.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://hfy.shanyushiyangtech.top

[R64] 结束进程
来源：http://hnr.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://fxk.gogol.net.cn

[R65] 查看端口占用
来源：http://mda.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mni.guowangkeji.top

[R66] 定时任务
来源：http://ifx.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://gvy.yj20258888.top

[R67] 生成随机十六进制串
来源：http://knp.bjfxy.top

openssl rand -hex 16
来源：http://dzn.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://kza.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://egc.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://ohu.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://nln.havefunace.top

[R70] 时间戳与互转
来源：http://wwh.fehbvm.com

date +%s;  date -d @1700000000
来源：http://uxi.ybcxt.top

[R71] 日期格式化
来源：http://fhx.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://krp.meibo888.top

[R72] 等待端口就绪
来源：http://cbj.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ckl.shzxlz.cn

[R73] 分割大日志
来源：http://bsx.yj202588.top

split -l 1000 big.log part_
来源：http://dko.yj20258.top

[R74] 批量重命名
来源：http://hyx.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rlw.yvedp.cn

[R75] 导出环境变量
来源：http://rcl.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://fwd.zdbjq.cn

[R76] 使用临时文件
来源：http://lgo.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzk.cdnleiting.top

[R77] 读取用户输入
来源：http://uvw.jinqigufen.top

read -rp "请输入: " ans
来源：http://xlp.andypj.xyz

[R78] 交互式菜单
来源：http://qme.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pgx.tianlin.xyz

[R79] 解析命令行选项
来源：http://ytn.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rqe.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://xbm.daxiang520.top

time ./run.sh
来源：http://gzs.xylfe.cn

================================================================================
来源：http://ycb.ydzc1.top

S. C / C++ 专题
来源：http://utg.cheryme.top

================================================================================
来源：http://ayb.ppjwa.cn

[S01] C：Hello World
来源：http://lcx.dashuyun.cn

#include <stdio.h>
来源：http://nbc.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ykr.fzhhl.top

[S02] C：变量与格式化输出
来源：http://pxi.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://trr.gogol.net.cn

[S03] C：读入整数
来源：http://fnq.0kj1m.cn

int x; scanf("%d", &x);
来源：http://sho.ydzc1.top

[S04] C：字符串复制
来源：http://ioj.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://myz.cdnleiting.top

[S05] C：字符串长度
来源：http://nsg.feifeiyinyue.top

strlen(s)
来源：http://qnk.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://srs.kuanghao11.cn

strcmp(a, b) == 0
来源：http://sgt.gogol.net.cn

[S07] C：数组遍历求和
来源：http://upr.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://due.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://nqh.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jjc.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://csf.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rtx.mhx1999.top

[S10] C：指针与解引用
来源：http://hsc.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://gyh.fktsv.cn

[S11] C：逐行读文件
来源：http://kux.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://fhj.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ihc.yfazqb.com

fclose(f);
来源：http://fha.zhongyouzk.top

[S12] C：写文件
来源：http://fvh.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wri.fzhhl.top

[S13] C：宏定义
来源：http://bgr.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nua.hcnkem.com

[S14] C：枚举
来源：http://xdg.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://qkb.hcnkem.com

[S15] C：类型转换
来源：http://gkn.ivvv.top

(double) a / b
来源：http://axi.xuanzx.com

[S16] C：位操作置位
来源：http://zkw.bbcook.cn

x |= (1 << 3);
来源：http://rjh.52xcode.cn

[S17] C：安全拼接字符串
来源：http://ckm.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zdg.sweek.top

[S18] C：命令行参数
来源：http://zdu.yangfankeji.com

int main(int argc, char **argv)
来源：http://dtz.xylfe.cn

[S19] C：快速排序
来源：http://yys.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://ehy.hongshengwenyu.top

[S20] C：二分查找
来源：http://kjm.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yzu.daxiang520.top

[S21] C：字符类别判断
来源：http://ciy.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xhz.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://nhj.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://tti.yuanzhike.top

[S23] C：随机数
来源：http://mwe.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ehp.jqgfzy.top

[S24] C：获取本地时间
来源：http://meq.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aas.epnwcf.com

[S25] C：内存拷贝
来源：http://pnh.haohaochexian.top

memcpy(dst, src, n);
来源：http://iex.nwbrower.top

[S26] C：内存清零
来源：http://afo.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://igi.redwolf501.top

[S27] C：定义常量
来源：http://oyd.hongshengwenyu.top

const double PI = 3.14159;
来源：http://ujd.yuxming.cn

[S28] C：静态变量
来源：http://bsc.zdbjq.cn

static int counter = 0;
来源：http://tdx.hysaishi.cn

[S29] C：变参函数
来源：http://cjb.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kcj.kuanghao11.cn

[S30] C：头文件保护
来源：http://nsc.guannengcc.top

#ifndef X_H
来源：http://wrn.0kj1m.cn

#define X_H
来源：http://hql.shangyingyoupin.top

#endif
来源：http://uwj.pycfn.com

[S31] C++：Hello World
来源：http://pix.zhixingplan.top

#include <iostream>
来源：http://fjg.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ybj.daxiang520.top

[S32] C++：字符串
来源：http://jdn.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://qbg.yvedp.cn

[S33] C++：vector 增删
来源：http://wri.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sex.yfazqb.com

[S34] C++：遍历 vector
来源：http://ptn.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://wer.shzxlz.cn

[S35] C++：map
来源：http://fkq.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://chp.c1oappe.top

[S36] C++：unordered_map
来源：http://wdn.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lan.havefunace.top

[S37] C++：set
来源：http://txn.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hcv.epnwcf.com

[S38] C++：排序
来源：http://qhx.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://xfe.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://ook.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rnb.cqqwz.cn

[S40] C++：查找元素
来源：http://ske.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dti.svipenyu.cn

[S41] C++：类与构造函数
来源：http://xey.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://avm.gzhubu.top

[S42] C++：继承与虚函数
来源：http://far.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://poa.pycfn.com

[S43] C++：智能指针
来源：http://gxj.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://lqz.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://toz.yuxming.cn

void inc(int &x) { ++x; }
来源：http://fwz.uphjek.com

[S45] C++：lambda
来源：http://kvm.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://kqu.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://mxz.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cnx.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://jqx.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fib.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://xas.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://mab.andypj.xyz

while (std::getline(in, line)) { }
来源：http://vwx.bbcook.cn

[S49] C++：写文件
来源：http://osm.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://utn.gzhubu.top

[S50] C++：格式化数字
来源：http://npg.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://omd.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://grg.sjlbkw.cn

static_cast<double>(a) / b
来源：http://bus.uphjek.com

[S52] C++：const 与 noexcept
来源：http://hbq.xylfe.cn

int size() const noexcept { return n_; }
来源：http://jun.hnqzz.top

[S53] C++：移动语义
来源：http://soa.316326.xyz

std::vector<int> w = std::move(v);
来源：http://qiz.birdmap.top

[S54] C++：异常处理
来源：http://pnq.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ozt.hammf.cn

[S55] C++：结构化绑定
来源：http://jdz.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://znh.zhixingplan.top

[S56] C++：optional
来源：http://lpb.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pkz.yuxming.cn

[S57] C++：编译期常量
来源：http://wqf.iojbl.cn

constexpr int N = 10;
来源：http://jjb.zdbjq.cn

[S58] C++：命名空间
来源：http://wle.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://ine.zhijiandao.cn

[S59] C++：静态断言
来源：http://dxf.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rxc.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://xof.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odc.zhijiandao.cn

================================================================================
来源：http://gpw.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vrg.sweek.top

================================================================================
来源：http://mko.hnqzz.top

[T01] Kotlin：Hello World
来源：http://zoc.shuidangran.top

println("Hello")
来源：http://lby.fehbvm.com

[T02] Kotlin：变量
来源：http://csi.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://csv.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://aac.c1oappe.top

"值: $b"
来源：http://rrg.nwbrower.top

[T04] Kotlin：空安全
来源：http://adl.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://htr.yj202588.top

[T05] Kotlin：when 表达式
来源：http://pco.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ltk.tian-w.cn

[T06] Kotlin：集合映射
来源：http://zhx.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://njc.ivvv.top

[T07] Kotlin：集合过滤
来源：http://twc.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rye.redwolf501.top

[T08] Kotlin：数据类
来源：http://qbj.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://xla.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://pzl.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://qae.smart0.xyz

[T10] Kotlin：默认参数
来源：http://grt.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bkn.tarul.cn

[T11] Kotlin：协程
来源：http://jks.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ypd.xylfe.cn

[T12] Kotlin：解构声明
来源：http://vyp.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://uie.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://xmz.meibo888.top

val m = mapOf("a" to 1)
来源：http://pfb.tianlin.xyz

[T14] Kotlin：循环
来源：http://ibk.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://tjn.jlsjyb.cn

[T15] Kotlin：接口
来源：http://nev.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://yml.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://xgp.shzxlz.cn

print("Hello")
来源：http://aau.havefunace.top

[T17] Swift：变量与常量
来源：http://pzo.fehbvm.com

var a = 1;  let b = 2
来源：http://rfm.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://tul.dashuyun.cn

"值: \(b)"
来源：http://scw.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://xrh.bbcook.cn

if let n = opt { print(n) }
来源：http://pup.zdbjq.cn

[T20] Swift：数组操作
来源：http://vjs.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://lum.fktsv.cn

[T21] Swift：遍历
来源：http://vkm.zhiwuduotai.top

for x in a { print(x) }
来源：http://qxh.zhiwuduotai.top

[T22] Swift：字典
来源：http://jnq.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vgy.hcnkem.com

[T23] Swift：函数
来源：http://aux.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lid.ydjk.org.cn

[T24] Swift：闭包
来源：http://ied.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://czq.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://qlp.zhengqikj.top

struct P { var x: Int }
来源：http://won.zhijiandao.cn

[T26] Swift：类与重写
来源：http://vtx.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://lrz.fehbvm.com

[T27] Swift：错误处理
来源：http://hrb.fengsongda.top

do { try f() } catch { print(error) }
来源：http://tpo.fengsongda.top

[T28] Swift：枚举
来源：http://iri.jinqigfzy.top

enum Color { case red, green }
来源：http://rgs.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://obx.hywenlv.cn

guard let x = opt else { return }
来源：http://crn.nanxinkj.top

[T30] Swift：协议
来源：http://hiz.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://kac.jinqigufen.top

[T31] Lua：Hello World
来源：http://tyc.epnwcf.com

print("Hello")
来源：http://hku.haohaochexian.top

[T32] Lua：局部变量
来源：http://ubz.smart0.xyz

local a = 1
来源：http://iyz.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://opy.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://slv.shuidangran.top

[T34] Lua：遍历表
来源：http://nfk.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://etr.bbcook.cn

[T35] Lua：字典表
来源：http://evq.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://vxo.aizwys.cn

[T36] Lua：函数
来源：http://kpf.9152youxi.cn

function add(a, b) return a + b end
来源：http://fsb.yj20258888.top

[T37] Lua：字符串拼接
来源：http://hut.redwolf501.top

"a" .. "b"
来源：http://sqg.daxiang520.top

[T38] Lua：条件
来源：http://oow.nanxinkj.top

if x > 0 then print("正") end
来源：http://gey.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://mbl.tarul.cn

string.find(s, "%d+")
来源：http://jwm.dianchejie.cn

[T40] Lua：元表
来源：http://zxo.xylfe.cn

setmetatable({}, { __index = base })
来源：http://qmq.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://ikl.c1oappe.top

print "Hello\n";
来源：http://lni.fengsongda.top

[T42] Perl：变量类型
来源：http://yqa.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktc.zhixingplan.top

[T43] Perl：字符串插值
来源：http://cpw.jyoumei.cn

"值: $a"
来源：http://hws.shzxlz.cn

[T44] Perl：条件
来源：http://zga.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://izv.haohaochexian.top

[T45] Perl：数组遍历
来源：http://ttm.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://hbc.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://vnv.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ylu.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://aiy.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kxc.ppjwa.cn

[T48] Perl：正则替换
来源：http://ulu.yvedp.cn

$s =~ s/old/new/g;
来源：http://ilt.yueranfly.top


<!-- 参考信息 -->