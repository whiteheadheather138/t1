代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uuz.gaohongyu789.top

[R34] 退出时清理
来源：http://mcn.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ukk.yanxiufei.cn

[R35] 后台执行并等待
来源：http://rwj.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qtq.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://dqs.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hmx.fengsongda.top

[R37] 把输出赋给变量
来源：http://qgb.nwbrower.top

files=$(ls -1)
来源：http://mso.hfpthk.cn

[R38] 管道串联
来源：http://ehg.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://pso.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://cpb.quarkkingdee.top

cmd > out.log 2>&1
来源：http://ggk.havefunace.top

[R40] 追加写日志
来源：http://ntg.ctjpmb.com

echo "log" >> out.log
来源：http://wna.ydjk.org.cn

[R41] 丢弃输出
来源：http://jtk.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://hfq.dashuyun.cn

[R42] 输入重定向
来源：http://bqd.nanxinkj.top

wc -l < a.txt
来源：http://xaq.andypj.xyz

[R43] 按名字查找文件
来源：http://krd.yonumen.top

find . -name "*.log" -type f
来源：http://agn.yvedp.cn

[R44] 按修改时间查找
来源：http://fvu.gaohongyu789.top

find . -mtime -7 -type f
来源：http://cry.svipenyu.cn

[R45] 批量删除
来源：http://jpo.iojbl.cn

find . -name "*.tmp" -delete
来源：http://qrr.ybcxt.top

[R46] 递归替换文件内容
来源：http://vpm.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iua.vqdsnc.cn

[R47] sed 单行替换
来源：http://jlx.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://kal.cdnleiting.top

[R48] awk 取指定列
来源：http://jrf.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://ljl.wangdashe.top

[R49] awk 带条件
来源：http://vdw.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hyu.fzhhl.top

[R50] awk 求和
来源：http://rpm.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tyf.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://iut.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kfc.svipenyu.cn

[R52] 统计行数
来源：http://tzw.fanxiaobao.xyz

wc -l a.txt
来源：http://gwq.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://jeb.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nnb.fengsongda.top

[R54] 比较两个文件
来源：http://hrg.quarkkingdee.top

diff a.txt b.txt
来源：http://ikp.shangyingyoupin.top

[R55] 压缩与解压
来源：http://doi.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ajz.aibaodan.cn

[R56] 远程拷贝
来源：http://hyb.ydjk.org.cn

scp file user@host:/path/
来源：http://uql.chenzaomai.com

[R57] 远程执行命令
来源：http://tkj.yj202588.top

ssh user@host 'uptime'
来源：http://xxz.guowangkeji.top

[R58] 下载文件
来源：http://uru.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sph.yfazqb.com

[R59] 发 POST JSON
来源：http://dnm.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xnc.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://hwc.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dpc.andypj.xyz

[R61] 磁盘占用
来源：http://jvc.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://xte.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://rdf.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://wsv.52xcode.cn

[R63] 内存与进程
来源：http://ljk.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://sgd.hesvh.cn

[R64] 结束进程
来源：http://luj.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://abo.fzhhl.top

[R65] 查看端口占用
来源：http://fiz.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://spx.zhixingplan.top

[R66] 定时任务
来源：http://ipd.jqgfzy.top

crontab -e;  crontab -l
来源：http://wfx.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://cvt.hnxiangtu.top

openssl rand -hex 16
来源：http://bec.gogol.net.cn

[R68] 计算文件校验值
来源：http://nxb.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://tzn.c1oappe.top

[R69] 生成随机密码
来源：http://fcq.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://uwm.yuxming.cn

[R70] 时间戳与互转
来源：http://pxq.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://vjy.tarul.cn

[R71] 日期格式化
来源：http://llv.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nfe.gaohongyu789.top

[R72] 等待端口就绪
来源：http://ewl.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://trn.xylfe.cn

[R73] 分割大日志
来源：http://orq.daxiang520.top

split -l 1000 big.log part_
来源：http://prj.316326.xyz

[R74] 批量重命名
来源：http://nyx.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://teq.ppjwa.cn

[R75] 导出环境变量
来源：http://jec.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://vrf.sxryk.cn

[R76] 使用临时文件
来源：http://rtl.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://esy.nanxinkj.top

[R77] 读取用户输入
来源：http://myo.jiagoushi.top

read -rp "请输入: " ans
来源：http://vmp.cashguo.top

[R78] 交互式菜单
来源：http://uho.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://jtb.zhengqikj.top

[R79] 解析命令行选项
来源：http://urw.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://otf.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://kxb.chenjidiqi.icu

time ./run.sh
来源：http://tsv.hcnkem.com

================================================================================
来源：http://xrm.tanke756.top

S. C / C++ 专题
来源：http://sev.hongshengwenyu.top

================================================================================
来源：http://ltn.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://dow.gaohongyu789.top

#include <stdio.h>
来源：http://vtn.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aux.sweek.top

[S02] C：变量与格式化输出
来源：http://zxp.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://zqm.shuidangran.top

[S03] C：读入整数
来源：http://vhh.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://mkf.zdqjudy.top

[S04] C：字符串复制
来源：http://yjg.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://unk.bjfxy.top

[S05] C：字符串长度
来源：http://zpe.chenlongwang.top

strlen(s)
来源：http://lwt.kuanghao11.cn

[S06] C：字符串比较
来源：http://sxd.epnwcf.com

strcmp(a, b) == 0
来源：http://uim.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://lsf.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tev.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://wqs.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tuf.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://aau.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gwp.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://kyz.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://vxf.zhoulong.xyz

[S11] C：逐行读文件
来源：http://aii.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://jmk.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qdd.fktsv.cn

fclose(f);
来源：http://jmy.chenjidiqi.icu

[S12] C：写文件
来源：http://nth.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tso.zhongyouzk.top

[S13] C：宏定义
来源：http://kqq.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://edo.zdbjq.cn

[S14] C：枚举
来源：http://fwk.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://uvp.aibaodan.cn

[S15] C：类型转换
来源：http://aod.ydjk.org.cn

(double) a / b
来源：http://tae.sjlbkw.cn

[S16] C：位操作置位
来源：http://thi.316326.xyz

x |= (1 << 3);
来源：http://jbz.sxryk.cn

[S17] C：安全拼接字符串
来源：http://ncv.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jol.hammf.cn

[S18] C：命令行参数
来源：http://biv.jinqigufen.top

int main(int argc, char **argv)
来源：http://yhe.shuidangran.top

[S19] C：快速排序
来源：http://umx.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ppn.ybcxt.top

[S20] C：二分查找
来源：http://ehr.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cjp.redwolf501.top

[S21] C：字符类别判断
来源：http://vmq.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ran.hcnkem.com

[S22] C：字符串转数字
来源：http://caw.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://lho.fengsongda.top

[S23] C：随机数
来源：http://cdx.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://msh.yvedp.cn

[S24] C：获取本地时间
来源：http://xjw.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nal.hysaishi.cn

[S25] C：内存拷贝
来源：http://dqp.yongpay.top

memcpy(dst, src, n);
来源：http://xae.zhoulong.xyz

[S26] C：内存清零
来源：http://yfr.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://rmo.gzhubu.top

[S27] C：定义常量
来源：http://khi.52xcode.cn

const double PI = 3.14159;
来源：http://ccg.feifeiyinyue.top

[S28] C：静态变量
来源：http://mhv.fktsv.cn

static int counter = 0;
来源：http://uir.havefunace.top

[S29] C：变参函数
来源：http://jzt.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zxh.ppjwa.cn

[S30] C：头文件保护
来源：http://lbr.yuxming.cn

#ifndef X_H
来源：http://hfj.gotoacloud.top

#define X_H
来源：http://xyx.jiagoushi.top

#endif
来源：http://hip.jiagoushi.top

[S31] C++：Hello World
来源：http://haq.wangshuangyany.cn

#include <iostream>
来源：http://old.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://imi.yvedp.cn

[S32] C++：字符串
来源：http://fih.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://ycp.aizwys.cn

[S33] C++：vector 增删
来源：http://poz.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qyz.cashguo.top

[S34] C++：遍历 vector
来源：http://icj.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://alv.tanke756.top

[S35] C++：map
来源：http://owd.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ulw.yuxming.cn

[S36] C++：unordered_map
来源：http://bax.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qcg.feifeiyinyue.top

[S37] C++：set
来源：http://hio.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://apy.pengpengdd.cyou

[S38] C++：排序
来源：http://bdn.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://fyp.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://qar.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qfv.fktsv.cn

[S40] C++：查找元素
来源：http://caj.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tnc.tanke756.top

[S41] C++：类与构造函数
来源：http://dqb.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tes.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://lkf.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://duk.hongshengwenyu.top

[S43] C++：智能指针
来源：http://oms.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://ocm.shzxlz.cn

[S44] C++：引用传参
来源：http://mlj.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://ral.tianlin.xyz

[S45] C++：lambda
来源：http://aih.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://fwn.jinqigfzy.top

[S46] C++：函数模板
来源：http://wel.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iui.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://ofa.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yor.xylfe.cn

[S48] C++：逐行读文件
来源：http://iac.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://neb.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://qtk.cdnleiting.top

[S49] C++：写文件
来源：http://gis.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gtk.shzxlz.cn

[S50] C++：格式化数字
来源：http://fys.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qfl.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://yrj.0kj1m.cn

static_cast<double>(a) / b
来源：http://orl.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://kwz.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://tqn.xuanzx.com

[S53] C++：移动语义
来源：http://aiv.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://wqw.bbcook.cn

[S54] C++：异常处理
来源：http://pql.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aps.daria6918.cn

[S55] C++：结构化绑定
来源：http://vdd.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uoj.kuanghao11.cn

[S56] C++：optional
来源：http://ulk.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dsd.tanke756.top

[S57] C++：编译期常量
来源：http://tth.fanxiaobao.xyz

constexpr int N = 10;
来源：http://blu.xylfe.cn

[S58] C++：命名空间
来源：http://kuh.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://hsq.wangdashe.top

[S59] C++：静态断言
来源：http://ali.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fal.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://kyg.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://agg.epnwcf.com

================================================================================
来源：http://pca.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qny.jianghu66.top

================================================================================
来源：http://cab.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://hgi.bjfxy.top

println("Hello")
来源：http://hfc.sysykeji.top

[T02] Kotlin：变量
来源：http://xuj.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssz.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://fnl.iojbl.cn

"值: $b"
来源：http://jhq.sxryk.cn

[T04] Kotlin：空安全
来源：http://jbm.hammf.cn

val n: String? = null;  n?.length
来源：http://msh.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://xyj.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rqe.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://pfm.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://trf.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://rao.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wmf.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://uqb.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://zxd.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://rcg.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://mnd.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://vpm.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ujo.jinqigufen.top

[T11] Kotlin：协程
来源：http://hmd.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gas.aizwys.cn

[T12] Kotlin：解构声明
来源：http://dow.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://bad.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://rpb.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://lqk.guannengcc.top

[T14] Kotlin：循环
来源：http://hhu.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://atg.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://wly.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://gbh.hammf.cn

[T16] Swift：Hello World
来源：http://chi.cucudq.cn

print("Hello")
来源：http://xca.mhx1999.top

[T17] Swift：变量与常量
来源：http://mye.vehdjk.com

var a = 1;  let b = 2
来源：http://txr.zhengqikj.top

[T18] Swift：字符串插值
来源：http://bze.zhoulong.xyz

"值: \(b)"
来源：http://rpu.meibo888.top

[T19] Swift：可选绑定
来源：http://rqx.jyoumei.cn

if let n = opt { print(n) }
来源：http://ibv.hywenlv.cn

[T20] Swift：数组操作
来源：http://yjl.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zxs.wangdashe.top

[T21] Swift：遍历
来源：http://nan.0kj1m.cn

for x in a { print(x) }
来源：http://wuf.xuetiantiany.cn

[T22] Swift：字典
来源：http://uzb.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ias.hywenlv.cn

[T23] Swift：函数
来源：http://gxd.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rid.jqgufenzy.top

[T24] Swift：闭包
来源：http://vaf.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://psy.hnqzz.top

[T25] Swift：结构体
来源：http://rya.chenzaomai.com

struct P { var x: Int }
来源：http://hyk.sysykeji.top

[T26] Swift：类与重写
来源：http://fep.smart0.xyz

class A: Base { override func f() {} }
来源：http://pha.sufxvd.cn

[T27] Swift：错误处理
来源：http://hdq.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://zlg.zycfv.cn

[T28] Swift：枚举
来源：http://ovi.guannengcc.top

enum Color { case red, green }
来源：http://foq.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://mtq.dianchejie.cn

guard let x = opt else { return }
来源：http://poh.yanxiufei.cn

[T30] Swift：协议
来源：http://jhu.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://yna.yueranfly.top

[T31] Lua：Hello World
来源：http://qwq.daxiang520.top

print("Hello")
来源：http://rlb.uphjek.com

[T32] Lua：局部变量
来源：http://zoh.hesvh.cn

local a = 1
来源：http://xvg.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://hwe.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://chr.0kj1m.cn

[T34] Lua：遍历表
来源：http://uuq.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://sdz.zycfv.cn

[T35] Lua：字典表
来源：http://dxx.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://yri.redwolf501.top

[T36] Lua：函数
来源：http://ozi.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://xtp.sweek.top


<!-- 参考信息 -->