代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://urp.nwbrower.top

[R34] 退出时清理
来源：http://xuk.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kca.epnwcf.com

[R35] 后台执行并等待
来源：http://xnh.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ydq.uphjek.com

[R36] 并发执行多个任务
来源：http://qsi.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ncv.cdnleiting.top

[R37] 把输出赋给变量
来源：http://bcj.c1oappe.top

files=$(ls -1)
来源：http://jdm.shanyushiyangtech.top

[R38] 管道串联
来源：http://swq.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://iat.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://vjx.yvedp.cn

cmd > out.log 2>&1
来源：http://lky.zycfv.cn

[R40] 追加写日志
来源：http://orh.chenlongwang.top

echo "log" >> out.log
来源：http://swx.hongshengwenyu.top

[R41] 丢弃输出
来源：http://yyb.xziqi.cn

cmd >/dev/null 2>&1
来源：http://rvn.gogol.net.cn

[R42] 输入重定向
来源：http://hah.hysaishi.cn

wc -l < a.txt
来源：http://ddr.hammf.cn

[R43] 按名字查找文件
来源：http://ieu.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://pgp.andypj.xyz

[R44] 按修改时间查找
来源：http://xjg.tanke756.top

find . -mtime -7 -type f
来源：http://pnz.yj20258.top

[R45] 批量删除
来源：http://aom.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://vsm.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://hik.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tpk.chenlongwang.top

[R47] sed 单行替换
来源：http://usq.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tgx.zhengqikj.top

[R48] awk 取指定列
来源：http://bag.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://yma.wangdashe.top

[R49] awk 带条件
来源：http://iem.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qry.fehbvm.com

[R50] awk 求和
来源：http://srn.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hoc.mhx1999.top

[R51] 排序去重取前几
来源：http://hbv.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://vzl.zhaomingkeji.xyz

[R52] 统计行数
来源：http://oqy.jinqigufen.top

wc -l a.txt
来源：http://hyj.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://osu.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://erc.yj202588.top

[R54] 比较两个文件
来源：http://phk.0kj1m.cn

diff a.txt b.txt
来源：http://uao.cheryme.top

[R55] 压缩与解压
来源：http://ikn.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ivt.guowangkeji.top

[R56] 远程拷贝
来源：http://tju.hysaishi.cn

scp file user@host:/path/
来源：http://osv.dianchejie.cn

[R57] 远程执行命令
来源：http://doo.316326.xyz

ssh user@host 'uptime'
来源：http://eaf.ydzc1.top

[R58] 下载文件
来源：http://fam.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cim.sxryk.cn

[R59] 发 POST JSON
来源：http://mxo.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hbi.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://cpj.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://log.pengpengdd.cyou

[R61] 磁盘占用
来源：http://irp.jinqigufen.top

df -h;  du -sh *
来源：http://ebv.sxryk.cn

[R62] 找最占空间的文件
来源：http://jek.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://yfb.aizwys.cn

[R63] 内存与进程
来源：http://kmf.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://kfg.aizwys.cn

[R64] 结束进程
来源：http://bpe.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://pxy.hesvh.cn

[R65] 查看端口占用
来源：http://agv.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qno.aibaodan.cn

[R66] 定时任务
来源：http://yka.ctjpmb.com

crontab -e;  crontab -l
来源：http://kpt.bjfxy.top

[R67] 生成随机十六进制串
来源：http://igb.zhongyouzk.top

openssl rand -hex 16
来源：http://mym.tarul.cn

[R68] 计算文件校验值
来源：http://vxe.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://ndg.fehbvm.com

[R69] 生成随机密码
来源：http://qkc.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://cag.zycfv.cn

[R70] 时间戳与互转
来源：http://vyv.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://oky.yj202588.top

[R71] 日期格式化
来源：http://eic.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gre.meibo888.top

[R72] 等待端口就绪
来源：http://kex.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xio.redwolf501.top

[R73] 分割大日志
来源：http://jyo.yongpay.top

split -l 1000 big.log part_
来源：http://eyx.pycfn.com

[R74] 批量重命名
来源：http://ybx.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cjz.feifeiyinyue.top

[R75] 导出环境变量
来源：http://nid.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://uog.cashguo.top

[R76] 使用临时文件
来源：http://tqs.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yyv.zdqjudy.top

[R77] 读取用户输入
来源：http://rxb.fktsv.cn

read -rp "请输入: " ans
来源：http://fvl.ybcxt.top

[R78] 交互式菜单
来源：http://zjf.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ymi.zhoulong.xyz

[R79] 解析命令行选项
来源：http://ipo.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fwd.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://nuj.gotoacloud.top

time ./run.sh
来源：http://fbf.jianghu66.top

================================================================================
来源：http://ltl.jlsjyb.cn

S. C / C++ 专题
来源：http://pfp.52xcode.cn

================================================================================
来源：http://zoq.tanke756.top

[S01] C：Hello World
来源：http://nfz.jqgufenzy.top

#include <stdio.h>
来源：http://pzn.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vwq.yj20258.top

[S02] C：变量与格式化输出
来源：http://awz.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://zkp.guowangkeji.top

[S03] C：读入整数
来源：http://gib.yj202588.top

int x; scanf("%d", &x);
来源：http://kgb.cqqwz.cn

[S04] C：字符串复制
来源：http://aqp.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hye.sjlbkw.cn

[S05] C：字符串长度
来源：http://lno.yueranfly.top

strlen(s)
来源：http://cnd.chenzaomai.com

[S06] C：字符串比较
来源：http://iqq.sufxvd.cn

strcmp(a, b) == 0
来源：http://orm.ctjpmb.com

[S07] C：数组遍历求和
来源：http://vlq.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xyv.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://mol.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ctm.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://uth.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jib.yuxming.cn

[S10] C：指针与解引用
来源：http://iih.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://yjk.hnxiangtu.top

[S11] C：逐行读文件
来源：http://mie.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://rgg.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hlo.gzhubu.top

fclose(f);
来源：http://pax.wangshuangyany.cn

[S12] C：写文件
来源：http://bgt.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhr.yangfankeji.com

[S13] C：宏定义
来源：http://gvz.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hwp.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://sbg.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://fpo.fehbvm.com

[S15] C：类型转换
来源：http://rog.zdqjudy.top

(double) a / b
来源：http://rdm.gotoacloud.top

[S16] C：位操作置位
来源：http://zyd.cqqwz.cn

x |= (1 << 3);
来源：http://ooh.xziqi.cn

[S17] C：安全拼接字符串
来源：http://eha.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blb.hesvh.cn

[S18] C：命令行参数
来源：http://hin.redwolf501.top

int main(int argc, char **argv)
来源：http://nii.zhongyouzk.top

[S19] C：快速排序
来源：http://rty.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fcc.c1oappe.top

[S20] C：二分查找
来源：http://jhu.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wem.guannengcc.top

[S21] C：字符类别判断
来源：http://yng.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yru.ydzc1.top

[S22] C：字符串转数字
来源：http://sbm.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jsi.0kj1m.cn

[S23] C：随机数
来源：http://tnm.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sks.sweek.top

[S24] C：获取本地时间
来源：http://beg.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iuk.sweek.top

[S25] C：内存拷贝
来源：http://zku.zhijiandao.cn

memcpy(dst, src, n);
来源：http://fht.fzhhl.top

[S26] C：内存清零
来源：http://rnk.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://kpb.gotoacloud.top

[S27] C：定义常量
来源：http://vyo.quarkkingdee.top

const double PI = 3.14159;
来源：http://tbo.zdbjq.cn

[S28] C：静态变量
来源：http://wil.iojbl.cn

static int counter = 0;
来源：http://rke.fehbvm.com

[S29] C：变参函数
来源：http://coc.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pyw.nanxinkj.top

[S30] C：头文件保护
来源：http://zcn.cheryme.top

#ifndef X_H
来源：http://ane.yj202588.top

#define X_H
来源：http://ofn.jianghu66.top

#endif
来源：http://zad.ctjpmb.com

[S31] C++：Hello World
来源：http://vbp.yuanzhike.top

#include <iostream>
来源：http://mmy.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://wuw.shanyushiyangtech.top

[S32] C++：字符串
来源：http://ldv.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://dds.havefunace.top

[S33] C++：vector 增删
来源：http://duy.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mbg.zdqjudy.top

[S34] C++：遍历 vector
来源：http://lzt.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://hxj.zhiwuduotai.top

[S35] C++：map
来源：http://khv.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ayp.0kj1m.cn

[S36] C++：unordered_map
来源：http://bbq.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://grl.mhx1999.top

[S37] C++：set
来源：http://lkq.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tiy.gotoacloud.top

[S38] C++：排序
来源：http://ehg.fanxiaobao.xyz

std::sort(v.begin(), v.end());
来源：http://oce.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://ywh.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rdc.birdmap.top

[S40] C++：查找元素
来源：http://stb.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ndh.cucudq.cn

[S41] C++：类与构造函数
来源：http://ltm.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://exc.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://vrx.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://aeo.mhx1999.top

[S43] C++：智能指针
来源：http://tai.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://cuv.jqgfzy.top

[S44] C++：引用传参
来源：http://vrg.uphjek.com

void inc(int &x) { ++x; }
来源：http://qhz.bbcook.cn

[S45] C++：lambda
来源：http://kja.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://hfp.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://dcv.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jsl.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://lkz.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aap.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://nbe.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://rad.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://med.tianlin.xyz

[S49] C++：写文件
来源：http://ufa.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fns.dianchejie.cn

[S50] C++：格式化数字
来源：http://muj.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://akd.yongpay.top

[S51] C++：显式类型转换
来源：http://trq.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://zww.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://noe.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://qao.gogol.net.cn

[S53] C++：移动语义
来源：http://vmn.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://dnw.snrcjt.cn

[S54] C++：异常处理
来源：http://wiz.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cmu.jyoumei.cn

[S55] C++：结构化绑定
来源：http://dqy.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://piy.andypj.xyz

[S56] C++：optional
来源：http://otf.xuanzx.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nde.xylfe.cn

[S57] C++：编译期常量
来源：http://tyr.hnxiangtu.top

constexpr int N = 10;
来源：http://uam.jyoumei.cn

[S58] C++：命名空间
来源：http://gkg.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://jyq.yuxming.cn

[S59] C++：静态断言
来源：http://grw.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wbj.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://acn.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bjb.zhixingplan.top

================================================================================
来源：http://yqp.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nwt.nanxinkj.top

================================================================================
来源：http://txb.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://tev.ydzc1.top

println("Hello")
来源：http://jwa.yj20258.top

[T02] Kotlin：变量
来源：http://hff.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qfh.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://bqu.jinyuanbaomall.cn

"值: $b"
来源：http://cvg.yvedp.cn

[T04] Kotlin：空安全
来源：http://hsl.sysykeji.top

val n: String? = null;  n?.length
来源：http://bpi.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://gwg.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uhy.pycfn.com

[T06] Kotlin：集合映射
来源：http://jwp.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://odx.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://iyy.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gbn.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://vql.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://rsk.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://awu.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://wub.yonumen.top

[T10] Kotlin：默认参数
来源：http://wyg.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://doq.gotoacloud.top

[T11] Kotlin：协程
来源：http://wgw.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uqi.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://cjj.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://pqy.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://jmv.c1oappe.top

val m = mapOf("a" to 1)
来源：http://tbk.yonumen.top

[T14] Kotlin：循环
来源：http://nwl.guannengcc.top

for (i in 1..10) println(i)
来源：http://nxj.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://phh.tarul.cn

interface Shape { fun area(): Double }
来源：http://sxq.uphjek.com

[T16] Swift：Hello World
来源：http://rvw.fehbvm.com

print("Hello")
来源：http://bfq.fengsongda.top

[T17] Swift：变量与常量
来源：http://kuz.smart0.xyz

var a = 1;  let b = 2
来源：http://zvf.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://zcv.jqgufenzy.top

"值: \(b)"
来源：http://wlu.andypj.xyz

[T19] Swift：可选绑定
来源：http://ewc.cashguo.top

if let n = opt { print(n) }
来源：http://xje.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://jqw.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://ocp.tianlin.xyz

[T21] Swift：遍历
来源：http://qat.xinyue.icu

for x in a { print(x) }
来源：http://art.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://uvm.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://yek.ehwqpu.com

[T23] Swift：函数
来源：http://qja.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvu.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://rjv.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xax.0kj1m.cn

[T25] Swift：结构体
来源：http://dnv.yangfankeji.com

struct P { var x: Int }
来源：http://oda.ydjk.org.cn

[T26] Swift：类与重写
来源：http://oku.guannengcc.top

class A: Base { override func f() {} }
来源：http://mmg.sysykeji.top

[T27] Swift：错误处理
来源：http://duh.daxiang520.top

do { try f() } catch { print(error) }
来源：http://gsi.ehwqpu.com

[T28] Swift：枚举
来源：http://tnb.jinghuilouyu.cn

enum Color { case red, green }
来源：http://umw.cheryme.top

[T29] Swift：guard 提前返回
来源：http://zfk.yangfankeji.com

guard let x = opt else { return }
来源：http://ksg.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://hcd.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://tbh.gogol.net.cn

[T31] Lua：Hello World
来源：http://cxj.shangyingyoupin.top

print("Hello")
来源：http://lss.sxryk.cn

[T32] Lua：局部变量
来源：http://mtj.fktsv.cn

local a = 1
来源：http://hnm.gotoacloud.top

[T33] Lua：表（数组）
来源：http://sra.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://caj.gogol.net.cn

[T34] Lua：遍历表
来源：http://obd.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hxc.tianlin.xyz

[T35] Lua：字典表
来源：http://utw.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://rrn.dashuyun.cn

[T36] Lua：函数
来源：http://ffu.sjlbkw.cn

function add(a, b) return a + b end
来源：http://tdh.zdbjq.cn


<!-- 参考信息 -->