代发 wailian999

echo "${#s}"
来源：http://oci.zhixingplan.top

[R22] 截取子串
来源：http://vva.smart0.xyz

echo "${s:0:5}"
来源：http://jga.ehwqpu.com

[R23] 字符串替换
来源：http://jez.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zkt.sysykeji.top

[R24] 大小写转换
来源：http://grx.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://vjl.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://syf.hongshengwenyu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gjc.zhengqikj.top

[R26] 命令替换
来源：http://cqm.ivvv.top

now=$(date +%F); echo "$now"
来源：http://jkx.kuanghao11.cn

[R27] 算术展开
来源：http://bec.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://xlu.tianlin.xyz

[R28] 浮点运算
来源：http://poa.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://erv.ehwqpu.com

[R29] 定义函数
来源：http://vbu.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hsq.jiagoushi.top

[R30] 函数返回状态码
来源：http://wyj.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://bqv.52xcode.cn

[R31] 局部变量
来源：http://trb.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://kag.jiagoushi.top

[R32] 参数个数校验
来源：http://tes.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xes.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://uyp.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kxv.jinqigfzy.top

[R34] 退出时清理
来源：http://gev.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gne.vqdsnc.cn

[R35] 后台执行并等待
来源：http://rag.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://llt.birdmap.top

[R36] 并发执行多个任务
来源：http://lpn.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cmm.ybcxt.top

[R37] 把输出赋给变量
来源：http://nwm.sysykeji.top

files=$(ls -1)
来源：http://uzy.gzhubu.top

[R38] 管道串联
来源：http://cln.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://jho.meibo888.top

[R39] 重定向标准输出与错误
来源：http://tsd.jqgfzy.top

cmd > out.log 2>&1
来源：http://iso.nanxinkj.top

[R40] 追加写日志
来源：http://fwf.jyoumei.cn

echo "log" >> out.log
来源：http://hjj.guowangkeji.top

[R41] 丢弃输出
来源：http://kwj.wangdashe.top

cmd >/dev/null 2>&1
来源：http://dte.ydjk.org.cn

[R42] 输入重定向
来源：http://mdd.jinqigufen.top

wc -l < a.txt
来源：http://dym.yj202588.top

[R43] 按名字查找文件
来源：http://xfc.daria6918.cn

find . -name "*.log" -type f
来源：http://agg.ydzc1.top

[R44] 按修改时间查找
来源：http://tpy.aizwys.cn

find . -mtime -7 -type f
来源：http://vrt.wangshuangyany.cn

[R45] 批量删除
来源：http://thv.yonumen.top

find . -name "*.tmp" -delete
来源：http://fcq.cqqwz.cn

[R46] 递归替换文件内容
来源：http://fou.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lcx.fehbvm.com

[R47] sed 单行替换
来源：http://yty.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://szn.feifeiyinyue.top

[R48] awk 取指定列
来源：http://uzt.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://wzg.zhongyouzk.top

[R49] awk 带条件
来源：http://uvl.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://brw.hnxiangtu.top

[R50] awk 求和
来源：http://tgt.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://mwl.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://wnq.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://flq.snrcjt.cn

[R52] 统计行数
来源：http://jom.chenjidiqi.icu

wc -l a.txt
来源：http://goo.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://zvy.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gzc.yueranfly.top

[R54] 比较两个文件
来源：http://sct.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://btb.cucudq.cn

[R55] 压缩与解压
来源：http://vmt.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wil.andypj.xyz

[R56] 远程拷贝
来源：http://ycl.jqgfzy.top

scp file user@host:/path/
来源：http://riw.chenjidiqi.icu

[R57] 远程执行命令
来源：http://ijp.havefunace.top

ssh user@host 'uptime'
来源：http://isw.0kj1m.cn

[R58] 下载文件
来源：http://wur.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cwg.redwolf501.top

[R59] 发 POST JSON
来源：http://qqt.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dcv.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://dkc.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aqq.xziqi.cn

[R61] 磁盘占用
来源：http://hyh.redwolf501.top

df -h;  du -sh *
来源：http://gxa.jinqigufen.top

[R62] 找最占空间的文件
来源：http://kvh.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://ivc.hongshengwenyu.top

[R63] 内存与进程
来源：http://rwt.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://tmk.bbcook.cn

[R64] 结束进程
来源：http://wpm.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://mjr.iojbl.cn

[R65] 查看端口占用
来源：http://ofa.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eyk.guannengcc.top

[R66] 定时任务
来源：http://mud.xuanzx.com

crontab -e;  crontab -l
来源：http://arv.guannengcc.top

[R67] 生成随机十六进制串
来源：http://zli.tianlin.xyz

openssl rand -hex 16
来源：http://odr.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://hwh.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rit.zhengqikj.top

[R69] 生成随机密码
来源：http://ndi.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://niu.birdmap.top

[R70] 时间戳与互转
来源：http://yte.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://xbt.gaohongyu789.top

[R71] 日期格式化
来源：http://rqm.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://amh.fzhhl.top

[R72] 等待端口就绪
来源：http://goy.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qmb.c1oappe.top

[R73] 分割大日志
来源：http://uvk.hammf.cn

split -l 1000 big.log part_
来源：http://arf.smart0.xyz

[R74] 批量重命名
来源：http://zqw.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fbb.chenzaomai.com

[R75] 导出环境变量
来源：http://sau.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://unj.epnwcf.com

[R76] 使用临时文件
来源：http://jns.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jxu.cucudq.cn

[R77] 读取用户输入
来源：http://pby.epnwcf.com

read -rp "请输入: " ans
来源：http://mlu.hnqzz.top

[R78] 交互式菜单
来源：http://rpe.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ohq.hywenlv.cn

[R79] 解析命令行选项
来源：http://mjp.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pug.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://npl.aizwys.cn

time ./run.sh
来源：http://gpb.cucudq.cn

================================================================================
来源：http://uea.havefunace.top

S. C / C++ 专题
来源：http://sxj.tanke756.top

================================================================================
来源：http://aqf.daxiang520.top

[S01] C：Hello World
来源：http://gdy.ppjwa.cn

#include <stdio.h>
来源：http://dxz.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://meb.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://usz.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://nee.guannengcc.top

[S03] C：读入整数
来源：http://rlf.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://caj.yj20258888.top

[S04] C：字符串复制
来源：http://vjv.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://akt.cheryme.top

[S05] C：字符串长度
来源：http://pqh.yj202588.top

strlen(s)
来源：http://itn.yonumen.top

[S06] C：字符串比较
来源：http://mtp.birdmap.top

strcmp(a, b) == 0
来源：http://bcj.mhx1999.top

[S07] C：数组遍历求和
来源：http://nfj.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hog.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://fhp.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ett.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://vpb.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://edc.wangdashe.top

[S10] C：指针与解引用
来源：http://wqr.xylfe.cn

int *p = &a;  *p = 5;
来源：http://tqi.jianghu66.top

[S11] C：逐行读文件
来源：http://yex.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://xbv.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://alq.ywan-chungtsiang.top

fclose(f);
来源：http://uao.vqdsnc.cn

[S12] C：写文件
来源：http://svt.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fkf.smart0.xyz

[S13] C：宏定义
来源：http://syp.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rvy.yongpay.top

[S14] C：枚举
来源：http://muf.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ckp.jqgfzy.top

[S15] C：类型转换
来源：http://muu.316326.xyz

(double) a / b
来源：http://lqt.jiagoushi.top

[S16] C：位操作置位
来源：http://gma.ydjk.org.cn

x |= (1 << 3);
来源：http://kxf.aizwys.cn

[S17] C：安全拼接字符串
来源：http://biw.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bxp.zhengqikj.top

[S18] C：命令行参数
来源：http://eib.zhengqikj.top

int main(int argc, char **argv)
来源：http://oxf.zhiwuduotai.top

[S19] C：快速排序
来源：http://dlj.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iod.hysaishi.cn

[S20] C：二分查找
来源：http://lyl.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jhh.dianchejie.cn

[S21] C：字符类别判断
来源：http://hrx.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rol.sjlbkw.cn

[S22] C：字符串转数字
来源：http://ihd.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://utn.shanyushiyangtech.top

[S23] C：随机数
来源：http://alh.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qom.aibaodan.cn

[S24] C：获取本地时间
来源：http://ehd.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hjk.andypj.xyz

[S25] C：内存拷贝
来源：http://pqb.yj20258.top

memcpy(dst, src, n);
来源：http://yos.ivvv.top

[S26] C：内存清零
来源：http://yyu.bjfxy.top

memset(a, 0, sizeof a);
来源：http://qeh.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://ycu.hammf.cn

const double PI = 3.14159;
来源：http://gyb.redwolf501.top

[S28] C：静态变量
来源：http://iqd.fehbvm.com

static int counter = 0;
来源：http://ifr.aibaodan.cn

[S29] C：变参函数
来源：http://nrm.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vjy.yangfankeji.com

[S30] C：头文件保护
来源：http://msg.havefunace.top

#ifndef X_H
来源：http://xwe.zhongyouzk.top

#define X_H
来源：http://ibe.chenjidiqi.icu

#endif
来源：http://vmx.yfazqb.com

[S31] C++：Hello World
来源：http://het.tian-w.cn

#include <iostream>
来源：http://fky.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://hhd.nanxuanxn.top

[S32] C++：字符串
来源：http://owc.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://lrt.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://cje.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tjv.gotoacloud.top

[S34] C++：遍历 vector
来源：http://bam.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://zcv.haohaochexian.top

[S35] C++：map
来源：http://fur.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xor.jqgfzy.top

[S36] C++：unordered_map
来源：http://xez.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xet.yonumen.top

[S37] C++：set
来源：http://pzl.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mel.sjlbkw.cn

[S38] C++：排序
来源：http://pvx.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://dan.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://wid.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ogk.andypj.xyz

[S40] C++：查找元素
来源：http://hwj.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gqz.hysaishi.cn

[S41] C++：类与构造函数
来源：http://hfk.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxl.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://mgf.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://xpu.chenzaomai.com

[S43] C++：智能指针
来源：http://lfs.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://oqc.xylfe.cn

[S44] C++：引用传参
来源：http://izb.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://kqq.zdqjudy.top

[S45] C++：lambda
来源：http://akx.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aok.xziqi.cn

[S46] C++：函数模板
来源：http://pex.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://atw.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://bqm.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://snp.snrcjt.cn

[S48] C++：逐行读文件
来源：http://upk.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rfn.xuanzx.com

while (std::getline(in, line)) { }
来源：http://swi.chenlongwang.top

[S49] C++：写文件
来源：http://zss.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uvj.yfazqb.com

[S50] C++：格式化数字
来源：http://mew.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xys.ivvv.top

[S51] C++：显式类型转换
来源：http://dky.nanxinkj.top

static_cast<double>(a) / b
来源：http://ubx.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://ywr.hesvh.cn

int size() const noexcept { return n_; }
来源：http://xbr.0kj1m.cn

[S53] C++：移动语义
来源：http://wxj.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://sjc.sxryk.cn

[S54] C++：异常处理
来源：http://vlj.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uzg.epnwcf.com

[S55] C++：结构化绑定
来源：http://neb.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qzu.yanxiufei.cn

[S56] C++：optional
来源：http://xjp.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pnr.guannengcc.top

[S57] C++：编译期常量
来源：http://ylw.jianghu66.top

constexpr int N = 10;
来源：http://cfw.zhiwuduotai.top

[S58] C++：命名空间
来源：http://xch.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://xgr.316326.xyz

[S59] C++：静态断言
来源：http://yoi.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ovk.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://sui.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://huc.jianghu66.top

================================================================================
来源：http://zhs.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lry.bbcook.cn

================================================================================
来源：http://bdx.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://ggh.yfazqb.com

println("Hello")
来源：http://ntm.vehdjk.com

[T02] Kotlin：变量
来源：http://uti.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eul.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://ats.yonumen.top

"值: $b"
来源：http://yni.daria6918.cn

[T04] Kotlin：空安全
来源：http://hrw.mhx1999.top

val n: String? = null;  n?.length
来源：http://ket.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://ztm.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ymd.yonumen.top

[T06] Kotlin：集合映射
来源：http://jje.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jma.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://par.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nzk.yangfankeji.com

[T08] Kotlin：数据类
来源：http://snl.cheryme.top

data class User(val name: String, val age: Int)
来源：http://jqo.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://vwh.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://ilh.tanke756.top

[T10] Kotlin：默认参数
来源：http://kgk.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rbl.gzhubu.top

[T11] Kotlin：协程
来源：http://abr.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qro.nwbrower.top

[T12] Kotlin：解构声明
来源：http://trv.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://jgo.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://niq.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://fyf.jlsjyb.cn

[T14] Kotlin：循环
来源：http://zxd.guowangkeji.top

for (i in 1..10) println(i)
来源：http://vdp.nanxinkj.top

[T15] Kotlin：接口
来源：http://qdy.aizwys.cn

interface Shape { fun area(): Double }
来源：http://vxc.hysaishi.cn

[T16] Swift：Hello World
来源：http://pii.vqdsnc.cn

print("Hello")
来源：http://mqx.xinyue.icu

[T17] Swift：变量与常量
来源：http://fwm.tian-w.cn

var a = 1;  let b = 2
来源：http://brm.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://znr.havefunace.top

"值: \(b)"
来源：http://zps.316326.xyz

[T19] Swift：可选绑定
来源：http://ivv.aibaodan.cn

if let n = opt { print(n) }
来源：http://luw.hnqzz.top

[T20] Swift：数组操作
来源：http://far.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pic.gogol.net.cn

[T21] Swift：遍历
来源：http://udw.ctjpmb.com

for x in a { print(x) }
来源：http://exm.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://cvn.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mzv.xinyue.icu

[T23] Swift：函数
来源：http://xap.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vpk.guannengcc.top

[T24] Swift：闭包
来源：http://fyo.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://qcn.uphjek.com


<!-- 参考信息 -->