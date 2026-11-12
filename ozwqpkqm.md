代发 wailian999

echo "${#s}"
来源：http://fbr.jlsjyb.cn

[R22] 截取子串
来源：http://ikh.jqgufenzy.top

echo "${s:0:5}"
来源：http://frp.jlsjyb.cn

[R23] 字符串替换
来源：http://cai.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ugs.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://oxc.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://ijp.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://qjq.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsr.tanke756.top

[R26] 命令替换
来源：http://etq.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://btu.hysaishi.cn

[R27] 算术展开
来源：http://rbk.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://bjo.0kj1m.cn

[R28] 浮点运算
来源：http://wvo.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://adi.zdqjudy.top

[R29] 定义函数
来源：http://fgz.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sub.ybcxt.top

[R30] 函数返回状态码
来源：http://zwj.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://rtt.tian-w.cn

[R31] 局部变量
来源：http://aqd.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://mul.pycfn.com

[R32] 参数个数校验
来源：http://vyn.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://asp.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://abk.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sla.ydjk.org.cn

[R34] 退出时清理
来源：http://qlq.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://yjz.nanxuanxn.top

[R35] 后台执行并等待
来源：http://hix.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://veo.hammf.cn

[R36] 并发执行多个任务
来源：http://fzq.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ytt.yangfankeji.com

[R37] 把输出赋给变量
来源：http://ryw.ywan-chungtsiang.top

files=$(ls -1)
来源：http://oar.yueranfly.top

[R38] 管道串联
来源：http://glk.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://cco.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://ygw.epnwcf.com

cmd > out.log 2>&1
来源：http://ors.jyoumei.cn

[R40] 追加写日志
来源：http://kwx.chenjidiqi.icu

echo "log" >> out.log
来源：http://mea.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://lxc.wangdashe.top

cmd >/dev/null 2>&1
来源：http://jou.vehdjk.com

[R42] 输入重定向
来源：http://rgg.zhongyouzk.top

wc -l < a.txt
来源：http://zby.quarkkingdee.top

[R43] 按名字查找文件
来源：http://umw.guannengcc.top

find . -name "*.log" -type f
来源：http://erp.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://xjd.jlsjyb.cn

find . -mtime -7 -type f
来源：http://nwd.xziqi.cn

[R45] 批量删除
来源：http://pjc.mhx1999.top

find . -name "*.tmp" -delete
来源：http://ofl.52xcode.cn

[R46] 递归替换文件内容
来源：http://eod.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oqe.cucudq.cn

[R47] sed 单行替换
来源：http://gys.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://jcu.hesvh.cn

[R48] awk 取指定列
来源：http://ynm.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://hoj.9152youxi.cn

[R49] awk 带条件
来源：http://vyq.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://agr.zhiwuduotai.top

[R50] awk 求和
来源：http://saw.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://njp.jlsjyb.cn

[R51] 排序去重取前几
来源：http://hyl.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://omt.dianchejie.cn

[R52] 统计行数
来源：http://pic.shzxlz.cn

wc -l a.txt
来源：http://rbk.ivvv.top

[R53] 查看文件头与实时尾
来源：http://bao.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://orc.jqgfzy.top

[R54] 比较两个文件
来源：http://woy.haohaochexian.top

diff a.txt b.txt
来源：http://lpg.yvedp.cn

[R55] 压缩与解压
来源：http://rel.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ner.jqgufenzy.top

[R56] 远程拷贝
来源：http://xdn.chenzaomai.com

scp file user@host:/path/
来源：http://tgb.birdmap.top

[R57] 远程执行命令
来源：http://qqx.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://qsa.cashguo.top

[R58] 下载文件
来源：http://kyg.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kjv.xinyue.icu

[R59] 发 POST JSON
来源：http://bcc.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wic.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://iak.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hmd.nanxinkj.top

[R61] 磁盘占用
来源：http://lfk.nanxinkj.top

df -h;  du -sh *
来源：http://zpv.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://mxz.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://sch.ctjpmb.com

[R63] 内存与进程
来源：http://nqh.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://bis.yueranfly.top

[R64] 结束进程
来源：http://dqg.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://pka.uphjek.com

[R65] 查看端口占用
来源：http://ogm.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hmc.tanke756.top

[R66] 定时任务
来源：http://vws.yanxiufei.cn

crontab -e;  crontab -l
来源：http://fyn.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://lok.hywenlv.cn

openssl rand -hex 16
来源：http://zxo.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://jzh.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://rpn.pengpengdd.cyou

[R69] 生成随机密码
来源：http://tlr.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://vmt.gogol.net.cn

[R70] 时间戳与互转
来源：http://jqk.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://ffd.zhoulong.xyz

[R71] 日期格式化
来源：http://mdb.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zhk.fehbvm.com

[R72] 等待端口就绪
来源：http://bwn.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://elf.hcnkem.com

[R73] 分割大日志
来源：http://mxc.zhoulong.xyz

split -l 1000 big.log part_
来源：http://qtg.kuanghao11.cn

[R74] 批量重命名
来源：http://zgu.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://byx.hnqzz.top

[R75] 导出环境变量
来源：http://zcf.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://csi.zhengqikj.top

[R76] 使用临时文件
来源：http://bmx.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zcn.c1oappe.top

[R77] 读取用户输入
来源：http://ujo.yj202588.top

read -rp "请输入: " ans
来源：http://zje.jqgfzy.top

[R78] 交互式菜单
来源：http://fpi.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cei.cdnleiting.top

[R79] 解析命令行选项
来源：http://jgd.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cek.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://jry.mhx1999.top

time ./run.sh
来源：http://myl.feifeiyinyue.top

================================================================================
来源：http://xtd.gotoacloud.top

S. C / C++ 专题
来源：http://dsb.zhoulong.xyz

================================================================================
来源：http://nap.fanxiaobao.xyz

[S01] C：Hello World
来源：http://fyf.nwbrower.top

#include <stdio.h>
来源：http://rzv.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://afo.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://amo.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://tkj.fzhhl.top

[S03] C：读入整数
来源：http://vly.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://fff.fzhhl.top

[S04] C：字符串复制
来源：http://coe.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://zhz.epnwcf.com

[S05] C：字符串长度
来源：http://gnc.chenlongwang.top

strlen(s)
来源：http://rxk.0kj1m.cn

[S06] C：字符串比较
来源：http://ksm.gzhubu.top

strcmp(a, b) == 0
来源：http://ymn.sweek.top

[S07] C：数组遍历求和
来源：http://jrd.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rhp.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://wim.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://htn.birdmap.top

[S09] C：结构体定义与初始化
来源：http://qle.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eet.tarul.cn

[S10] C：指针与解引用
来源：http://pyb.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://uti.birdmap.top

[S11] C：逐行读文件
来源：http://ivs.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://hma.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yod.fzhhl.top

fclose(f);
来源：http://zjm.fzhhl.top

[S12] C：写文件
来源：http://iba.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tno.shangyingyoupin.top

[S13] C：宏定义
来源：http://fsw.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wwv.shuidangran.top

[S14] C：枚举
来源：http://spq.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://ksw.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://zya.fzhhl.top

(double) a / b
来源：http://zkq.yj202588.top

[S16] C：位操作置位
来源：http://jzu.yongpay.top

x |= (1 << 3);
来源：http://atc.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://nck.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slb.yj202588.top

[S18] C：命令行参数
来源：http://uhh.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://tnz.jlsjyb.cn

[S19] C：快速排序
来源：http://lun.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://vzs.yfazqb.com

[S20] C：二分查找
来源：http://jjd.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zfc.hysaishi.cn

[S21] C：字符类别判断
来源：http://ikt.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hto.nanxinkj.top

[S22] C：字符串转数字
来源：http://cfy.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://aok.jqgfzy.top

[S23] C：随机数
来源：http://ldl.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xvk.meibo888.top

[S24] C：获取本地时间
来源：http://ear.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://emb.zhoulong.xyz

[S25] C：内存拷贝
来源：http://ils.xuanzx.com

memcpy(dst, src, n);
来源：http://ydc.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://dov.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://zxl.tianlin.xyz

[S27] C：定义常量
来源：http://zoj.ydzc1.top

const double PI = 3.14159;
来源：http://bqd.sufxvd.cn

[S28] C：静态变量
来源：http://yyv.fktsv.cn

static int counter = 0;
来源：http://hff.jinghuilouyu.cn

[S29] C：变参函数
来源：http://ztm.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hsj.chenjidiqi.icu

[S30] C：头文件保护
来源：http://cqh.52xcode.cn

#ifndef X_H
来源：http://hea.xinyue.icu

#define X_H
来源：http://zjm.zdqjudy.top

#endif
来源：http://dxs.bbcook.cn

[S31] C++：Hello World
来源：http://imi.sxryk.cn

#include <iostream>
来源：http://xiv.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://jfg.chenzaomai.com

[S32] C++：字符串
来源：http://yej.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://cht.iojbl.cn

[S33] C++：vector 增删
来源：http://tti.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sqb.yuxming.cn

[S34] C++：遍历 vector
来源：http://gwv.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://cik.shuidangran.top

[S35] C++：map
来源：http://ciz.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wwb.jianghu66.top

[S36] C++：unordered_map
来源：http://ydu.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlj.yanxiufei.cn

[S37] C++：set
来源：http://gzd.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://daz.jyoumei.cn

[S38] C++：排序
来源：http://hbo.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://deo.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://xay.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xpl.ybcxt.top

[S40] C++：查找元素
来源：http://knq.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kka.snrcjt.cn

[S41] C++：类与构造函数
来源：http://jfn.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ucr.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://qcu.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://neg.redwolf501.top

[S43] C++：智能指针
来源：http://qrw.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://eos.shzxlz.cn

[S44] C++：引用传参
来源：http://hug.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://jjf.svipenyu.cn

[S45] C++：lambda
来源：http://ojx.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://jwp.zdbjq.cn

[S46] C++：函数模板
来源：http://kiu.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://udo.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://ugv.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vkr.uphjek.com

[S48] C++：逐行读文件
来源：http://oib.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fzj.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://lbk.tarul.cn

[S49] C++：写文件
来源：http://pdq.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://swz.birdmap.top

[S50] C++：格式化数字
来源：http://xfh.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://csw.andypj.xyz

[S51] C++：显式类型转换
来源：http://zad.aibaodan.cn

static_cast<double>(a) / b
来源：http://wkm.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://fch.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://hlz.ctjpmb.com

[S53] C++：移动语义
来源：http://dnc.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://vlc.havefunace.top

[S54] C++：异常处理
来源：http://urj.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ift.yj202588.top

[S55] C++：结构化绑定
来源：http://plt.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zyo.xziqi.cn

[S56] C++：optional
来源：http://emz.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hrt.zhongyouzk.top

[S57] C++：编译期常量
来源：http://jyu.nanxuanxn.top

constexpr int N = 10;
来源：http://dfm.zhongyouzk.top

[S58] C++：命名空间
来源：http://jbj.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://osk.ydzc1.top

[S59] C++：静态断言
来源：http://vxy.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://azn.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://mat.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edm.hfpthk.cn

================================================================================
来源：http://uti.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vvy.epnwcf.com

================================================================================
来源：http://sqd.9152youxi.cn

[T01] Kotlin：Hello World
来源：http://dua.c1oappe.top

println("Hello")
来源：http://ekb.cashguo.top

[T02] Kotlin：变量
来源：http://wvi.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rzb.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://flk.svipenyu.cn

"值: $b"
来源：http://wxy.pycfn.com

[T04] Kotlin：空安全
来源：http://jzs.hfpthk.cn

val n: String? = null;  n?.length
来源：http://sho.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://suj.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hrr.ybcxt.top

[T06] Kotlin：集合映射
来源：http://nph.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kpz.yonumen.top

[T07] Kotlin：集合过滤
来源：http://tva.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sxm.yuanzhike.top

[T08] Kotlin：数据类
来源：http://cvd.sweek.top

data class User(val name: String, val age: Int)
来源：http://wex.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://lkk.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://fmu.sweek.top

[T10] Kotlin：默认参数
来源：http://tui.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zsq.zdbjq.cn

[T11] Kotlin：协程
来源：http://tza.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kbe.hcnkem.com

[T12] Kotlin：解构声明
来源：http://riz.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://cme.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://prn.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://qpg.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://cjm.svipenyu.cn

for (i in 1..10) println(i)
来源：http://ozw.gotoacloud.top

[T15] Kotlin：接口
来源：http://qfb.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://icn.xinyue.icu

[T16] Swift：Hello World
来源：http://equ.pycfn.com

print("Hello")
来源：http://qpp.jianghu66.top

[T17] Swift：变量与常量
来源：http://sbf.bjfxy.top

var a = 1;  let b = 2
来源：http://nff.hesvh.cn

[T18] Swift：字符串插值
来源：http://whx.nwbrower.top

"值: \(b)"
来源：http://ewk.sxryk.cn

[T19] Swift：可选绑定
来源：http://yny.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://yhj.kuanghao11.cn

[T20] Swift：数组操作
来源：http://ftv.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://eic.nanxinkj.top

[T21] Swift：遍历
来源：http://zim.jinghuilouyu.cn

for x in a { print(x) }
来源：http://ptx.aibaodan.cn

[T22] Swift：字典
来源：http://hsr.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kbn.yj20258.top

[T23] Swift：函数
来源：http://ind.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qvh.pycfn.com

[T24] Swift：闭包
来源：http://sno.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dbi.xziqi.cn


<!-- 参考信息 -->