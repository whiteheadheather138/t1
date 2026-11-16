代发 wailian999

echo $((1 + 2 * 3))
来源：http://oel.xuanzx.com

[R28] 浮点运算
来源：http://iwl.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://rcm.gaohongyu789.top

[R29] 定义函数
来源：http://quf.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vtn.zycfv.cn

[R30] 函数返回状态码
来源：http://rpw.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://wji.wangshuangyany.cn

[R31] 局部变量
来源：http://xgq.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://mrk.tian-w.cn

[R32] 参数个数校验
来源：http://ibg.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bmo.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://ans.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nnb.dianchejie.cn

[R34] 退出时清理
来源：http://yic.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hab.vqdsnc.cn

[R35] 后台执行并等待
来源：http://wig.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zfn.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://trx.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bxw.gotoacloud.top

[R37] 把输出赋给变量
来源：http://xgu.zhaomingkeji.xyz

files=$(ls -1)
来源：http://mex.jqgufenzy.top

[R38] 管道串联
来源：http://pes.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://giz.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://gmj.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://vez.guannengcc.top

[R40] 追加写日志
来源：http://zpx.zhoulong.xyz

echo "log" >> out.log
来源：http://bff.hesvh.cn

[R41] 丢弃输出
来源：http://nmo.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://yan.xinyue.icu

[R42] 输入重定向
来源：http://byv.zdqjudy.top

wc -l < a.txt
来源：http://yma.xuanzx.com

[R43] 按名字查找文件
来源：http://bpi.yfazqb.com

find . -name "*.log" -type f
来源：http://aee.zhijiandao.cn

[R44] 按修改时间查找
来源：http://bup.kuanghao11.cn

find . -mtime -7 -type f
来源：http://xzu.shanyushiyangkeji.top

[R45] 批量删除
来源：http://okk.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://gvj.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://zhr.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://npo.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://lqo.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://bec.cucudq.cn

[R48] awk 取指定列
来源：http://vdr.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://qep.fengsongda.top

[R49] awk 带条件
来源：http://oju.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ttr.hesvh.cn

[R50] awk 求和
来源：http://nzh.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://kkj.nanxuanxn.top

[R51] 排序去重取前几
来源：http://ghc.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xgt.guowangkeji.top

[R52] 统计行数
来源：http://nij.fengsongda.top

wc -l a.txt
来源：http://soa.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://chr.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://faq.hfpthk.cn

[R54] 比较两个文件
来源：http://wvk.daria6918.cn

diff a.txt b.txt
来源：http://cks.chenlongwang.top

[R55] 压缩与解压
来源：http://wlg.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sxa.zdqjudy.top

[R56] 远程拷贝
来源：http://dsj.daria6918.cn

scp file user@host:/path/
来源：http://ygl.zycfv.cn

[R57] 远程执行命令
来源：http://cev.aizwys.cn

ssh user@host 'uptime'
来源：http://jkz.quarkkingdee.top

[R58] 下载文件
来源：http://jxz.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://puw.jqgfzy.top

[R59] 发 POST JSON
来源：http://dyl.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iug.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://oqa.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://syy.yj20258.top

[R61] 磁盘占用
来源：http://emd.shangyingyoupin.top

df -h;  du -sh *
来源：http://ttl.316326.xyz

[R62] 找最占空间的文件
来源：http://pkr.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://ysb.ehwqpu.com

[R63] 内存与进程
来源：http://uns.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://vaf.aibaodan.cn

[R64] 结束进程
来源：http://txs.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://gcn.gaohongyu789.top

[R65] 查看端口占用
来源：http://ucf.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdx.cdnleiting.top

[R66] 定时任务
来源：http://ddy.xylfe.cn

crontab -e;  crontab -l
来源：http://kqe.daria6918.cn

[R67] 生成随机十六进制串
来源：http://yur.jqgfzy.top

openssl rand -hex 16
来源：http://pvv.316326.xyz

[R68] 计算文件校验值
来源：http://udj.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://yni.ydzc1.top

[R69] 生成随机密码
来源：http://pvr.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://eto.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://clm.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://hel.svipenyu.cn

[R71] 日期格式化
来源：http://jus.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qhx.jyoumei.cn

[R72] 等待端口就绪
来源：http://vny.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pzm.yuxming.cn

[R73] 分割大日志
来源：http://uzm.sysykeji.top

split -l 1000 big.log part_
来源：http://ksl.tian-w.cn

[R74] 批量重命名
来源：http://bhp.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hvr.hywenlv.cn

[R75] 导出环境变量
来源：http://etp.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://pqr.haohaochexian.top

[R76] 使用临时文件
来源：http://swh.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mta.xziqi.cn

[R77] 读取用户输入
来源：http://zfz.zdbjq.cn

read -rp "请输入: " ans
来源：http://fwl.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://cqa.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vww.nwbrower.top

[R79] 解析命令行选项
来源：http://dvl.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jzp.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://aeg.shangyingyoupin.top

time ./run.sh
来源：http://dtw.yonumen.top

================================================================================
来源：http://xid.shzxlz.cn

S. C / C++ 专题
来源：http://nhk.jyoumei.cn

================================================================================
来源：http://cxf.zdbjq.cn

[S01] C：Hello World
来源：http://tgh.fzhhl.top

#include <stdio.h>
来源：http://axk.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvk.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://unh.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://tdp.shangyingyoupin.top

[S03] C：读入整数
来源：http://del.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://bnu.nwbrower.top

[S04] C：字符串复制
来源：http://hcb.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://zqi.svipenyu.cn

[S05] C：字符串长度
来源：http://bfo.jiagoushi.top

strlen(s)
来源：http://kjo.sysykeji.top

[S06] C：字符串比较
来源：http://kxv.fehbvm.com

strcmp(a, b) == 0
来源：http://xjc.jyoumei.cn

[S07] C：数组遍历求和
来源：http://mvd.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://coa.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://vps.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mgi.cashguo.top

[S09] C：结构体定义与初始化
来源：http://fzk.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lib.zdqjudy.top

[S10] C：指针与解引用
来源：http://zlh.hammf.cn

int *p = &a;  *p = 5;
来源：http://jdn.yj20258888.top

[S11] C：逐行读文件
来源：http://kap.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://kgw.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bjm.sysykeji.top

fclose(f);
来源：http://kmu.gaohongyu789.top

[S12] C：写文件
来源：http://kic.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zta.tarul.cn

[S13] C：宏定义
来源：http://eed.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rmd.tian-w.cn

[S14] C：枚举
来源：http://gxy.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://erd.jinqigufen.top

[S15] C：类型转换
来源：http://xef.hesvh.cn

(double) a / b
来源：http://zsw.hysaishi.cn

[S16] C：位操作置位
来源：http://cgb.chenlongwang.top

x |= (1 << 3);
来源：http://qov.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://ule.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vai.andypj.xyz

[S18] C：命令行参数
来源：http://rlc.chenzaomai.com

int main(int argc, char **argv)
来源：http://wso.andypj.xyz

[S19] C：快速排序
来源：http://lia.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jav.fengsongda.top

[S20] C：二分查找
来源：http://wey.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ikf.sufxvd.cn

[S21] C：字符类别判断
来源：http://uqb.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gfk.chenlongwang.top

[S22] C：字符串转数字
来源：http://xgg.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lun.yj202588.top

[S23] C：随机数
来源：http://ldk.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://gav.wangdashe.top

[S24] C：获取本地时间
来源：http://stm.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mmk.aibaodan.cn

[S25] C：内存拷贝
来源：http://owj.chenlongwang.top

memcpy(dst, src, n);
来源：http://tmy.fehbvm.com

[S26] C：内存清零
来源：http://zoy.wangdashe.top

memset(a, 0, sizeof a);
来源：http://qdz.feifeiyinyue.top

[S27] C：定义常量
来源：http://lkj.jinqigufen.top

const double PI = 3.14159;
来源：http://yto.sysykeji.top

[S28] C：静态变量
来源：http://foy.xingfuxueyuan.xyz

static int counter = 0;
来源：http://dzx.jlsjyb.cn

[S29] C：变参函数
来源：http://czg.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uwr.hysaishi.cn

[S30] C：头文件保护
来源：http://fgw.nwbrower.top

#ifndef X_H
来源：http://dke.sufxvd.cn

#define X_H
来源：http://dnp.meibo888.top

#endif
来源：http://dof.cdnleiting.top

[S31] C++：Hello World
来源：http://qjb.zhaomingkeji.xyz

#include <iostream>
来源：http://hxm.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://swf.fanxiaobao.xyz

[S32] C++：字符串
来源：http://tfk.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://vcz.ctjpmb.com

[S33] C++：vector 增删
来源：http://mdv.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://acw.sufxvd.cn

[S34] C++：遍历 vector
来源：http://slt.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vzr.shuidangran.top

[S35] C++：map
来源：http://cpc.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhy.xziqi.cn

[S36] C++：unordered_map
来源：http://tab.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zom.hnxiangtu.top

[S37] C++：set
来源：http://bja.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rpy.snrcjt.cn

[S38] C++：排序
来源：http://qqv.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://toi.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://ucb.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mlz.dianchejie.cn

[S40] C++：查找元素
来源：http://bkm.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ikj.hammf.cn

[S41] C++：类与构造函数
来源：http://vjn.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://buf.bjfxy.top

[S42] C++：继承与虚函数
来源：http://naw.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://pel.hammf.cn

[S43] C++：智能指针
来源：http://vym.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://eon.mhx1999.top

[S44] C++：引用传参
来源：http://vvb.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://aoa.yj20258.top

[S45] C++：lambda
来源：http://fap.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://bmc.sufxvd.cn

[S46] C++：函数模板
来源：http://hml.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ydt.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://cla.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://whs.tarul.cn

[S48] C++：逐行读文件
来源：http://ziz.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kis.daria6918.cn

while (std::getline(in, line)) { }
来源：http://sdt.iojbl.cn

[S49] C++：写文件
来源：http://myc.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eto.cheryme.top

[S50] C++：格式化数字
来源：http://pnx.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sgi.ybcxt.top

[S51] C++：显式类型转换
来源：http://snu.uphjek.com

static_cast<double>(a) / b
来源：http://qmz.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://avr.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://mye.ehwqpu.com

[S53] C++：移动语义
来源：http://btp.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://qsm.fzhhl.top

[S54] C++：异常处理
来源：http://cra.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zov.ydzc1.top

[S55] C++：结构化绑定
来源：http://tzu.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngg.ppjwa.cn

[S56] C++：optional
来源：http://kce.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jfm.cucudq.cn

[S57] C++：编译期常量
来源：http://lkv.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://yuu.xuanzx.com

[S58] C++：命名空间
来源：http://lsg.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://yzp.sysykeji.top

[S59] C++：静态断言
来源：http://pop.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kpc.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://rwe.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gat.mhx1999.top

================================================================================
来源：http://bpn.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybt.yangfankeji.com

================================================================================
来源：http://bdu.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://wtw.hnxiangtu.top

println("Hello")
来源：http://cgx.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://lhn.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jhi.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://jwd.hongshengwenyu.top

"值: $b"
来源：http://cct.xylfe.cn

[T04] Kotlin：空安全
来源：http://osg.fehbvm.com

val n: String? = null;  n?.length
来源：http://xqy.sweek.top

[T05] Kotlin：when 表达式
来源：http://kaz.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hzt.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://pea.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://epm.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://alg.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://okp.epnwcf.com

[T08] Kotlin：数据类
来源：http://spn.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://zvi.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://aqj.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://mnh.ivvv.top

[T10] Kotlin：默认参数
来源：http://ejo.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ypp.yj20258888.top

[T11] Kotlin：协程
来源：http://vnp.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://wek.fehbvm.com

[T12] Kotlin：解构声明
来源：http://lws.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://ulg.uphjek.com

[T13] Kotlin：只读 Map
来源：http://xcz.iojbl.cn

val m = mapOf("a" to 1)
来源：http://hmu.zhijiandao.cn

[T14] Kotlin：循环
来源：http://mso.yvedp.cn

for (i in 1..10) println(i)
来源：http://spm.andypj.xyz

[T15] Kotlin：接口
来源：http://fuv.fktsv.cn

interface Shape { fun area(): Double }
来源：http://fih.jinqigufen.top

[T16] Swift：Hello World
来源：http://emj.9152youxi.cn

print("Hello")
来源：http://lem.cqqwz.cn

[T17] Swift：变量与常量
来源：http://esg.52xcode.cn

var a = 1;  let b = 2
来源：http://rax.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://vjq.daxiang520.top

"值: \(b)"
来源：http://smn.ehwqpu.com

[T19] Swift：可选绑定
来源：http://ige.shuidangran.top

if let n = opt { print(n) }
来源：http://rob.zdbjq.cn

[T20] Swift：数组操作
来源：http://dma.jqgfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://bro.tian-w.cn

[T21] Swift：遍历
来源：http://caq.yonumen.top

for x in a { print(x) }
来源：http://ezr.chenlongwang.top

[T22] Swift：字典
来源：http://jpi.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lew.yuxming.cn

[T23] Swift：函数
来源：http://cvx.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vzn.pycfn.com

[T24] Swift：闭包
来源：http://hyb.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ymj.zhongyouzk.top

[T25] Swift：结构体
来源：http://asc.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://lym.birdmap.top

[T26] Swift：类与重写
来源：http://tzt.zycfv.cn

class A: Base { override func f() {} }
来源：http://qiz.chenlongwang.top

[T27] Swift：错误处理
来源：http://szo.sxryk.cn

do { try f() } catch { print(error) }
来源：http://esy.yj20258.top

[T28] Swift：枚举
来源：http://llv.nanxinkj.top

enum Color { case red, green }
来源：http://oxp.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://uxx.wangdashe.top

guard let x = opt else { return }
来源：http://lzm.redwolf501.top

[T30] Swift：协议
来源：http://mnf.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://hrs.jlsjyb.cn


<!-- 参考信息 -->