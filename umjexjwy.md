代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kap.nwbrower.top

[R16] until 等待条件
来源：http://cop.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xuq.mhx1999.top

[R17] 数组定义与取值
来源：http://you.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://pfk.epnwcf.com

[R18] 遍历数组
来源：http://ynz.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tuy.dianchejie.cn

[R19] 数组长度
来源：http://fdk.sysykeji.top

echo "${#arr[@]}"
来源：http://ltf.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://ntc.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pgm.0kj1m.cn

[R21] 字符串长度
来源：http://eqc.jlsjyb.cn

echo "${#s}"
来源：http://ita.sysykeji.top

[R22] 截取子串
来源：http://dji.yj20258888.top

echo "${s:0:5}"
来源：http://xnw.jianghu66.top

[R23] 字符串替换
来源：http://eek.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pfd.havefunace.top

[R24] 大小写转换
来源：http://nue.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://sbq.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://khp.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hvx.ivvv.top

[R26] 命令替换
来源：http://ebw.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://mjt.wangshuangyany.cn

[R27] 算术展开
来源：http://irq.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://gzu.daxiang520.top

[R28] 浮点运算
来源：http://mqt.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://dlq.havefunace.top

[R29] 定义函数
来源：http://bgv.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rgz.dianchejie.cn

[R30] 函数返回状态码
来源：http://zvj.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://gws.cheryme.top

[R31] 局部变量
来源：http://pfg.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://uqi.tarul.cn

[R32] 参数个数校验
来源：http://qya.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jof.meibo888.top

[R33] 捕获错误并提示行号
来源：http://ibr.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://upg.yonumen.top

[R34] 退出时清理
来源：http://bqa.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://vfq.jlsjyb.cn

[R35] 后台执行并等待
来源：http://foq.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://mra.sufxvd.cn

[R36] 并发执行多个任务
来源：http://mua.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eww.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://sfl.kuanghao11.cn

files=$(ls -1)
来源：http://yip.jinghuilouyu.cn

[R38] 管道串联
来源：http://enk.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://xcd.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://vgt.xinyue.icu

cmd > out.log 2>&1
来源：http://ipw.pycfn.com

[R40] 追加写日志
来源：http://ord.jinqigfzy.top

echo "log" >> out.log
来源：http://wxu.ybcxt.top

[R41] 丢弃输出
来源：http://rnj.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://fnu.guannengcc.top

[R42] 输入重定向
来源：http://qdf.iojbl.cn

wc -l < a.txt
来源：http://cog.hnxiangtu.top

[R43] 按名字查找文件
来源：http://uuu.ehwqpu.com

find . -name "*.log" -type f
来源：http://wkx.chenzaomai.com

[R44] 按修改时间查找
来源：http://nwh.nanxinkj.top

find . -mtime -7 -type f
来源：http://vnu.jinyuanbaomall.cn

[R45] 批量删除
来源：http://wug.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://kby.iojbl.cn

[R46] 递归替换文件内容
来源：http://kpf.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qac.havefunace.top

[R47] sed 单行替换
来源：http://zdz.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://vjj.jyoumei.cn

[R48] awk 取指定列
来源：http://ryl.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://vja.yonumen.top

[R49] awk 带条件
来源：http://zpg.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kjt.shangyingyoupin.top

[R50] awk 求和
来源：http://xyk.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://ckf.jiagoushi.top

[R51] 排序去重取前几
来源：http://zre.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jnv.bjfxy.top

[R52] 统计行数
来源：http://ppl.chenlongwang.top

wc -l a.txt
来源：http://cer.yj20258.top

[R53] 查看文件头与实时尾
来源：http://qvw.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wos.ehwqpu.com

[R54] 比较两个文件
来源：http://ili.nanxinkj.top

diff a.txt b.txt
来源：http://vlp.zhengqikj.top

[R55] 压缩与解压
来源：http://jis.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sea.gogol.net.cn

[R56] 远程拷贝
来源：http://mlj.hnxiangtu.top

scp file user@host:/path/
来源：http://hli.yfazqb.com

[R57] 远程执行命令
来源：http://fmg.chenzaomai.com

ssh user@host 'uptime'
来源：http://udw.yj20258.top

[R58] 下载文件
来源：http://acs.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yhh.epnwcf.com

[R59] 发 POST JSON
来源：http://lsb.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ewl.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://hff.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vgq.gzhubu.top

[R61] 磁盘占用
来源：http://qec.hywenlv.cn

df -h;  du -sh *
来源：http://aox.zdbjq.cn

[R62] 找最占空间的文件
来源：http://hva.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://mur.fanxiaobao.xyz

[R63] 内存与进程
来源：http://pkq.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://sdc.0kj1m.cn

[R64] 结束进程
来源：http://aqv.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://zpr.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://pcr.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mob.shuidangran.top

[R66] 定时任务
来源：http://bbu.sysykeji.top

crontab -e;  crontab -l
来源：http://doy.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://eco.jlsjyb.cn

openssl rand -hex 16
来源：http://kca.52xcode.cn

[R68] 计算文件校验值
来源：http://phi.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://xri.xziqi.cn

[R69] 生成随机密码
来源：http://kdm.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://gll.jinqigfzy.top

[R70] 时间戳与互转
来源：http://zqc.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://wzs.shzxlz.cn

[R71] 日期格式化
来源：http://ypq.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gyr.dianchejie.cn

[R72] 等待端口就绪
来源：http://eib.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vdh.jinghuilouyu.cn

[R73] 分割大日志
来源：http://qhv.pycfn.com

split -l 1000 big.log part_
来源：http://nrb.haohaochexian.top

[R74] 批量重命名
来源：http://vir.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://seq.gaohongyu789.top

[R75] 导出环境变量
来源：http://tly.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://els.hcnkem.com

[R76] 使用临时文件
来源：http://ppv.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dwu.havefunace.top

[R77] 读取用户输入
来源：http://wpe.ydjk.org.cn

read -rp "请输入: " ans
来源：http://win.0kj1m.cn

[R78] 交互式菜单
来源：http://ekq.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iwh.mhx1999.top

[R79] 解析命令行选项
来源：http://ckg.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://spw.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://pwc.tarul.cn

time ./run.sh
来源：http://cuh.nanxinkj.top

================================================================================
来源：http://kzm.bjfxy.top

S. C / C++ 专题
来源：http://vbb.gzhubu.top

================================================================================
来源：http://cgg.yuanzhike.top

[S01] C：Hello World
来源：http://fut.pycfn.com

#include <stdio.h>
来源：http://ctd.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wje.bjfxy.top

[S02] C：变量与格式化输出
来源：http://unw.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://vvv.feifeiyinyue.top

[S03] C：读入整数
来源：http://ktz.daria6918.cn

int x; scanf("%d", &x);
来源：http://bjl.mhx1999.top

[S04] C：字符串复制
来源：http://lac.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://rms.bbcook.cn

[S05] C：字符串长度
来源：http://hft.gaohongyu789.top

strlen(s)
来源：http://igj.yj20258888.top

[S06] C：字符串比较
来源：http://lba.gotoacloud.top

strcmp(a, b) == 0
来源：http://ybf.xuanzx.com

[S07] C：数组遍历求和
来源：http://nrm.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lmy.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://age.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hnp.pycfn.com

[S09] C：结构体定义与初始化
来源：http://ykv.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xlv.mhx1999.top

[S10] C：指针与解引用
来源：http://llo.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://qgj.hfpthk.cn

[S11] C：逐行读文件
来源：http://nce.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://eoo.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://das.haohaochexian.top

fclose(f);
来源：http://xdy.yuanzhike.top

[S12] C：写文件
来源：http://wjs.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cxy.quarkkingdee.top

[S13] C：宏定义
来源：http://ily.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rdt.nanxinkj.top

[S14] C：枚举
来源：http://lss.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://spk.shanyushiyangtech.top

[S15] C：类型转换
来源：http://lct.hnxiangtu.top

(double) a / b
来源：http://rag.gotoacloud.top

[S16] C：位操作置位
来源：http://mtl.fengsongda.top

x |= (1 << 3);
来源：http://nku.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://lnj.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mau.hammf.cn

[S18] C：命令行参数
来源：http://nmz.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://fpj.chenjidiqi.icu

[S19] C：快速排序
来源：http://wmm.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://cbj.ydzc1.top

[S20] C：二分查找
来源：http://zfd.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jyn.ivvv.top

[S21] C：字符类别判断
来源：http://bmv.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://poa.chenlongwang.top

[S22] C：字符串转数字
来源：http://pbp.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://err.sufxvd.cn

[S23] C：随机数
来源：http://oyk.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fgy.jinqigufen.top

[S24] C：获取本地时间
来源：http://jcd.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aij.sweek.top

[S25] C：内存拷贝
来源：http://mlr.gogol.net.cn

memcpy(dst, src, n);
来源：http://qqt.0kj1m.cn

[S26] C：内存清零
来源：http://wsy.ydzc1.top

memset(a, 0, sizeof a);
来源：http://sag.bbcook.cn

[S27] C：定义常量
来源：http://xuv.0kj1m.cn

const double PI = 3.14159;
来源：http://zrv.hnqzz.top

[S28] C：静态变量
来源：http://nfv.zhongyouzk.top

static int counter = 0;
来源：http://thg.quarkkingdee.top

[S29] C：变参函数
来源：http://xhe.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iht.zhengqikj.top

[S30] C：头文件保护
来源：http://oks.xingfuxueyuan.xyz

#ifndef X_H
来源：http://mpp.shangyingyoupin.top

#define X_H
来源：http://iqq.hfpthk.cn

#endif
来源：http://xlz.cqqwz.cn

[S31] C++：Hello World
来源：http://njq.zhiwuduotai.top

#include <iostream>
来源：http://jlf.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://ysn.ctjpmb.com

[S32] C++：字符串
来源：http://nkp.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://amb.yj20258888.top

[S33] C++：vector 增删
来源：http://lee.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ifc.jyoumei.cn

[S34] C++：遍历 vector
来源：http://zgx.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://wzl.bbcook.cn

[S35] C++：map
来源：http://tac.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rrm.gzhubu.top

[S36] C++：unordered_map
来源：http://aam.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lwm.zhengqikj.top

[S37] C++：set
来源：http://ndy.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ntr.yongpay.top

[S38] C++：排序
来源：http://elr.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://tdb.hammf.cn

[S39] C++：自定义比较器排序
来源：http://xct.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mop.yangfankeji.com

[S40] C++：查找元素
来源：http://clv.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ldj.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://wvt.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yyx.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://xlz.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://jem.tianlin.xyz

[S43] C++：智能指针
来源：http://aco.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://knj.yongpay.top

[S44] C++：引用传参
来源：http://fir.epnwcf.com

void inc(int &x) { ++x; }
来源：http://bhu.uphjek.com

[S45] C++：lambda
来源：http://bbb.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eon.wangshuangyany.cn

[S46] C++：函数模板
来源：http://jpq.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mvu.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://rnh.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hsb.redwolf501.top

[S48] C++：逐行读文件
来源：http://luy.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ulv.cucudq.cn

while (std::getline(in, line)) { }
来源：http://hem.jinqigufen.top

[S49] C++：写文件
来源：http://gka.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tly.guowangkeji.top

[S50] C++：格式化数字
来源：http://wrc.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://snz.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://yhq.hammf.cn

static_cast<double>(a) / b
来源：http://mux.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://jjc.hcnkem.com

int size() const noexcept { return n_; }
来源：http://czd.andypj.xyz

[S53] C++：移动语义
来源：http://srn.tarul.cn

std::vector<int> w = std::move(v);
来源：http://scy.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://gec.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dqt.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://eeq.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://upo.birdmap.top

[S56] C++：optional
来源：http://qqc.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://urj.yj20258.top

[S57] C++：编译期常量
来源：http://ate.hongshengwenyu.top

constexpr int N = 10;
来源：http://cfl.yanxiufei.cn

[S58] C++：命名空间
来源：http://aek.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://epe.hongshengwenyu.top

[S59] C++：静态断言
来源：http://nba.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pjr.cheryme.top

[S60] C++：遍历并删除元素
来源：http://bhz.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nyw.ywan-chungtsiang.top

================================================================================
来源：http://jja.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pgs.dashuyun.cn

================================================================================
来源：http://dqr.tanke756.top

[T01] Kotlin：Hello World
来源：http://wgk.316326.xyz

println("Hello")
来源：http://fqt.xziqi.cn

[T02] Kotlin：变量
来源：http://cgd.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hbe.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://eqp.c1oappe.top

"值: $b"
来源：http://roq.jinqigufen.top

[T04] Kotlin：空安全
来源：http://qdv.shzxlz.cn

val n: String? = null;  n?.length
来源：http://hsj.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://wij.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmy.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://ltq.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tvw.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://pur.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qch.fehbvm.com

[T08] Kotlin：数据类
来源：http://ndx.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://qzc.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://cem.tanke756.top

fun String.exclaim() = this + "!"
来源：http://ljb.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://oqg.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fal.hesvh.cn

[T11] Kotlin：协程
来源：http://jdi.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ouc.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://wzr.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://vbl.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://ylu.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://yro.cdnleiting.top

[T14] Kotlin：循环
来源：http://fyr.havefunace.top

for (i in 1..10) println(i)
来源：http://ngh.daxiang520.top

[T15] Kotlin：接口
来源：http://mch.jianghu66.top

interface Shape { fun area(): Double }
来源：http://uxk.zycfv.cn

[T16] Swift：Hello World
来源：http://mgh.jinqigufen.top

print("Hello")
来源：http://iqe.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://ofn.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://pzx.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://vlj.epnwcf.com

"值: \(b)"
来源：http://vyh.yongpay.top


<!-- 参考信息 -->