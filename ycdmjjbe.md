代发 wailian999

echo "${#arr[@]}"
来源：http://cue.sysykeji.top

[R20] 关联数组（字典）
来源：http://fvi.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wwo.andypj.xyz

[R21] 字符串长度
来源：http://adq.yj20258888.top

echo "${#s}"
来源：http://jhr.shanyushiyangkeji.top

[R22] 截取子串
来源：http://ndu.52xcode.cn

echo "${s:0:5}"
来源：http://jue.meibo888.top

[R23] 字符串替换
来源：http://pkv.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fam.sjlbkw.cn

[R24] 大小写转换
来源：http://zwe.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://twv.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://aav.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ked.pengpengdd.cyou

[R26] 命令替换
来源：http://zry.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://zjp.fengsongda.top

[R27] 算术展开
来源：http://hgq.uphjek.com

echo $((1 + 2 * 3))
来源：http://rue.hysaishi.cn

[R28] 浮点运算
来源：http://ahl.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://xih.epnwcf.com

[R29] 定义函数
来源：http://lih.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbe.gotoacloud.top

[R30] 函数返回状态码
来源：http://opa.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://iqr.jinghuilouyu.cn

[R31] 局部变量
来源：http://xdd.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://gfo.quarkkingdee.top

[R32] 参数个数校验
来源：http://mgv.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yti.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://cpx.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zhm.bjfxy.top

[R34] 退出时清理
来源：http://cni.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://csg.zdqjudy.top

[R35] 后台执行并等待
来源：http://wwx.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://msq.vehdjk.com

[R36] 并发执行多个任务
来源：http://sbg.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://egz.ybcxt.top

[R37] 把输出赋给变量
来源：http://brm.ppjwa.cn

files=$(ls -1)
来源：http://hmq.kuanghao11.cn

[R38] 管道串联
来源：http://umf.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://hyo.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://qog.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://rxk.52xcode.cn

[R40] 追加写日志
来源：http://jnq.c1oappe.top

echo "log" >> out.log
来源：http://cjp.zhiwuduotai.top

[R41] 丢弃输出
来源：http://amm.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://ukv.cheryme.top

[R42] 输入重定向
来源：http://rol.gogol.net.cn

wc -l < a.txt
来源：http://nrl.andypj.xyz

[R43] 按名字查找文件
来源：http://bvj.jqgufenzy.top

find . -name "*.log" -type f
来源：http://cad.chenzaomai.com

[R44] 按修改时间查找
来源：http://unb.0kj1m.cn

find . -mtime -7 -type f
来源：http://wwe.zhaomingkeji.xyz

[R45] 批量删除
来源：http://ogd.bbcook.cn

find . -name "*.tmp" -delete
来源：http://snf.hywenlv.cn

[R46] 递归替换文件内容
来源：http://fds.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dwn.hnqzz.top

[R47] sed 单行替换
来源：http://nwd.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://bus.ydjk.org.cn

[R48] awk 取指定列
来源：http://nax.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://hjk.yangfankeji.com

[R49] awk 带条件
来源：http://fcq.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oeq.uphjek.com

[R50] awk 求和
来源：http://mmi.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hir.cqqwz.cn

[R51] 排序去重取前几
来源：http://gxl.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mct.bbcook.cn

[R52] 统计行数
来源：http://pan.cheryme.top

wc -l a.txt
来源：http://arw.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://qba.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pdp.ctjpmb.com

[R54] 比较两个文件
来源：http://tok.zycfv.cn

diff a.txt b.txt
来源：http://mlr.yuxming.cn

[R55] 压缩与解压
来源：http://hps.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://etb.tianlin.xyz

[R56] 远程拷贝
来源：http://dra.bbcook.cn

scp file user@host:/path/
来源：http://vbi.tanke756.top

[R57] 远程执行命令
来源：http://xrp.cashguo.top

ssh user@host 'uptime'
来源：http://wua.316326.xyz

[R58] 下载文件
来源：http://fum.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wss.hywenlv.cn

[R59] 发 POST JSON
来源：http://eud.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wev.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://vck.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://neq.cdnleiting.top

[R61] 磁盘占用
来源：http://onv.aibaodan.cn

df -h;  du -sh *
来源：http://uij.jyoumei.cn

[R62] 找最占空间的文件
来源：http://ixv.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://vcp.cashguo.top

[R63] 内存与进程
来源：http://eqr.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://fnb.ctjpmb.com

[R64] 结束进程
来源：http://mdb.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://emn.shangyingyoupin.top

[R65] 查看端口占用
来源：http://azc.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://btw.bjfxy.top

[R66] 定时任务
来源：http://stt.hcnkem.com

crontab -e;  crontab -l
来源：http://wrj.mhx1999.top

[R67] 生成随机十六进制串
来源：http://smf.yuxming.cn

openssl rand -hex 16
来源：http://bje.9152youxi.cn

[R68] 计算文件校验值
来源：http://qzb.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ykh.yuxming.cn

[R69] 生成随机密码
来源：http://stg.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://huq.vehdjk.com

[R70] 时间戳与互转
来源：http://rip.bbcook.cn

date +%s;  date -d @1700000000
来源：http://dhs.vehdjk.com

[R71] 日期格式化
来源：http://yrn.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jmm.haohaochexian.top

[R72] 等待端口就绪
来源：http://uzz.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wul.dianchejie.cn

[R73] 分割大日志
来源：http://rnb.hywenlv.cn

split -l 1000 big.log part_
来源：http://jzm.52xcode.cn

[R74] 批量重命名
来源：http://mht.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bmb.vehdjk.com

[R75] 导出环境变量
来源：http://zvr.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://xun.epnwcf.com

[R76] 使用临时文件
来源：http://nbs.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zgu.ehwqpu.com

[R77] 读取用户输入
来源：http://mka.hywenlv.cn

read -rp "请输入: " ans
来源：http://nxn.sjlbkw.cn

[R78] 交互式菜单
来源：http://zhk.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bqj.xinyue.icu

[R79] 解析命令行选项
来源：http://hgj.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vgp.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://abb.zdbjq.cn

time ./run.sh
来源：http://ebt.shanyushiyangkeji.top

================================================================================
来源：http://ota.jiagoushi.top

S. C / C++ 专题
来源：http://fce.chenjidiqi.icu

================================================================================
来源：http://ddt.meibo888.top

[S01] C：Hello World
来源：http://mwj.tarul.cn

#include <stdio.h>
来源：http://idj.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vfs.xinyue.icu

[S02] C：变量与格式化输出
来源：http://yyj.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://ucn.yueranfly.top

[S03] C：读入整数
来源：http://vcx.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://ytu.guowangkeji.top

[S04] C：字符串复制
来源：http://jyi.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://lyq.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://umx.jqgufenzy.top

strlen(s)
来源：http://jic.cucudq.cn

[S06] C：字符串比较
来源：http://vvr.epnwcf.com

strcmp(a, b) == 0
来源：http://bio.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://agj.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://znr.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://mss.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://osl.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://gcb.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uxy.yongpay.top

[S10] C：指针与解引用
来源：http://des.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://ueu.gogol.net.cn

[S11] C：逐行读文件
来源：http://elb.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://sai.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dot.jyoumei.cn

fclose(f);
来源：http://mba.tianlin.xyz

[S12] C：写文件
来源：http://izj.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qbz.cheryme.top

[S13] C：宏定义
来源：http://opw.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mbp.zhijiandao.cn

[S14] C：枚举
来源：http://tnu.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://ugx.zhongyouzk.top

[S15] C：类型转换
来源：http://pne.ppjwa.cn

(double) a / b
来源：http://ywh.zdbjq.cn

[S16] C：位操作置位
来源：http://eji.ydjk.org.cn

x |= (1 << 3);
来源：http://pii.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://ozb.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://goo.jqgufenzy.top

[S18] C：命令行参数
来源：http://yws.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://ifh.fengsongda.top

[S19] C：快速排序
来源：http://ucm.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jft.yvedp.cn

[S20] C：二分查找
来源：http://ebu.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzq.xuanzx.com

[S21] C：字符类别判断
来源：http://meb.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wsa.jianghu66.top

[S22] C：字符串转数字
来源：http://qdf.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://esc.wangdashe.top

[S23] C：随机数
来源：http://fyq.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://waf.yj20258888.top

[S24] C：获取本地时间
来源：http://mmg.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xgp.jinqigufen.top

[S25] C：内存拷贝
来源：http://won.hysaishi.cn

memcpy(dst, src, n);
来源：http://zfy.ydzc1.top

[S26] C：内存清零
来源：http://mlc.daria6918.cn

memset(a, 0, sizeof a);
来源：http://hcv.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://wvp.zhijiandao.cn

const double PI = 3.14159;
来源：http://goo.xylfe.cn

[S28] C：静态变量
来源：http://nvt.gzhubu.top

static int counter = 0;
来源：http://uwl.bbcook.cn

[S29] C：变参函数
来源：http://tlb.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qxx.smart0.xyz

[S30] C：头文件保护
来源：http://yir.hnxiangtu.top

#ifndef X_H
来源：http://ypm.fktsv.cn

#define X_H
来源：http://bdo.jinqigfzy.top

#endif
来源：http://tlo.gzhubu.top

[S31] C++：Hello World
来源：http://ofn.andypj.xyz

#include <iostream>
来源：http://vrk.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://hba.gogol.net.cn

[S32] C++：字符串
来源：http://kzs.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://nsz.hywenlv.cn

[S33] C++：vector 增删
来源：http://yts.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aqs.aibaodan.cn

[S34] C++：遍历 vector
来源：http://lin.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://gak.chenzaomai.com

[S35] C++：map
来源：http://cmk.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khu.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://fky.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cuf.fktsv.cn

[S37] C++：set
来源：http://ige.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mgk.cashguo.top

[S38] C++：排序
来源：http://ewa.yj20258.top

std::sort(v.begin(), v.end());
来源：http://eqw.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://sql.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fjz.ybcxt.top

[S40] C++：查找元素
来源：http://jcg.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rag.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://sdo.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zvy.xziqi.cn

[S42] C++：继承与虚函数
来源：http://jhe.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://wwg.jinqigufen.top

[S43] C++：智能指针
来源：http://hlr.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://wep.hongshengwenyu.top

[S44] C++：引用传参
来源：http://wxf.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://ibd.xuetiantiany.cn

[S45] C++：lambda
来源：http://qwg.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://tgj.jinqigufen.top

[S46] C++：函数模板
来源：http://wja.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fxw.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://enc.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jij.pycfn.com

[S48] C++：逐行读文件
来源：http://vit.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yum.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://rhf.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://ccj.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tiu.xinyue.icu

[S50] C++：格式化数字
来源：http://zma.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jgs.yueranfly.top

[S51] C++：显式类型转换
来源：http://evz.guannengcc.top

static_cast<double>(a) / b
来源：http://aod.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://ras.wangdashe.top

int size() const noexcept { return n_; }
来源：http://jsn.yongpay.top

[S53] C++：移动语义
来源：http://aun.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://dhb.pengpengdd.cyou

[S54] C++：异常处理
来源：http://zty.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://isq.hammf.cn

[S55] C++：结构化绑定
来源：http://qsp.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lum.yuxming.cn

[S56] C++：optional
来源：http://vpi.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rch.yj20258.top

[S57] C++：编译期常量
来源：http://egs.yonumen.top

constexpr int N = 10;
来源：http://njp.haohaochexian.top

[S58] C++：命名空间
来源：http://mah.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://aoh.yueranfly.top

[S59] C++：静态断言
来源：http://teq.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mny.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://pru.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ixu.cdnleiting.top

================================================================================
来源：http://vlt.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bxh.tarul.cn

================================================================================
来源：http://doa.hnqzz.top

[T01] Kotlin：Hello World
来源：http://pfn.9152youxi.cn

println("Hello")
来源：http://zmc.vqdsnc.cn

[T02] Kotlin：变量
来源：http://iie.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yrr.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://vie.jiagoushi.top

"值: $b"
来源：http://geq.hongshengwenyu.top

[T04] Kotlin：空安全
来源：http://tgm.cucudq.cn

val n: String? = null;  n?.length
来源：http://rqs.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://icm.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cyc.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://lbk.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yim.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://kbd.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://isx.yj202588.top

[T08] Kotlin：数据类
来源：http://kyo.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://tpo.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://kjv.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://hfv.zycfv.cn

[T10] Kotlin：默认参数
来源：http://qsi.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://ldf.9152youxi.cn

[T11] Kotlin：协程
来源：http://lis.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fzi.uphjek.com

[T12] Kotlin：解构声明
来源：http://hzn.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://iaf.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://uef.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://xgb.bbcook.cn

[T14] Kotlin：循环
来源：http://vpz.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://vys.ybcxt.top

[T15] Kotlin：接口
来源：http://grv.xylfe.cn

interface Shape { fun area(): Double }
来源：http://ekm.xinyue.icu

[T16] Swift：Hello World
来源：http://guw.yonumen.top

print("Hello")
来源：http://bbg.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://bpf.hnxiangtu.top

var a = 1;  let b = 2
来源：http://twl.shuidangran.top

[T18] Swift：字符串插值
来源：http://qkx.vehdjk.com

"值: \(b)"
来源：http://sqh.hfpthk.cn

[T19] Swift：可选绑定
来源：http://ybb.redwolf501.top

if let n = opt { print(n) }
来源：http://qow.jyoumei.cn

[T20] Swift：数组操作
来源：http://rmn.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://zdh.chenzaomai.com

[T21] Swift：遍历
来源：http://mos.jqgfzy.top

for x in a { print(x) }
来源：http://pef.xylfe.cn

[T22] Swift：字典
来源：http://gxz.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://bph.chenjidiqi.icu


<!-- 参考信息 -->