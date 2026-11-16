代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlt.shuidangran.top

[R16] until 等待条件
来源：http://wly.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jsl.ppjwa.cn

[R17] 数组定义与取值
来源：http://amr.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oxf.iojbl.cn

[R18] 遍历数组
来源：http://qxa.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://idt.zdbjq.cn

[R19] 数组长度
来源：http://gmi.redwolf501.top

echo "${#arr[@]}"
来源：http://qet.shuidangran.top

[R20] 关联数组（字典）
来源：http://ngr.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qzn.jqgfzy.top

[R21] 字符串长度
来源：http://ufr.ivvv.top

echo "${#s}"
来源：http://pth.hcnkem.com

[R22] 截取子串
来源：http://cbv.chenzaomai.com

echo "${s:0:5}"
来源：http://sih.uphjek.com

[R23] 字符串替换
来源：http://bsw.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zya.316326.xyz

[R24] 大小写转换
来源：http://dmd.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://udr.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://uwm.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cnb.yj20258888.top

[R26] 命令替换
来源：http://msz.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://tfe.guowangkeji.top

[R27] 算术展开
来源：http://sxq.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://fgk.ppjwa.cn

[R28] 浮点运算
来源：http://zqq.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://pwd.yj20258.top

[R29] 定义函数
来源：http://dfd.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zli.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://irf.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://ewb.sweek.top

[R31] 局部变量
来源：http://ljk.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://wsl.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://wwj.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ksp.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://hrq.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://onr.jqgufenzy.top

[R34] 退出时清理
来源：http://uos.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://bmq.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://yrw.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://esc.yj202588.top

[R36] 并发执行多个任务
来源：http://szm.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fiw.ctjpmb.com

[R37] 把输出赋给变量
来源：http://giy.tianlin.xyz

files=$(ls -1)
来源：http://ptj.chenlongwang.top

[R38] 管道串联
来源：http://cix.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://izn.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://nfp.c1oappe.top

cmd > out.log 2>&1
来源：http://qas.gzhubu.top

[R40] 追加写日志
来源：http://avx.pycfn.com

echo "log" >> out.log
来源：http://ytz.aizwys.cn

[R41] 丢弃输出
来源：http://pua.hammf.cn

cmd >/dev/null 2>&1
来源：http://ymx.yuxming.cn

[R42] 输入重定向
来源：http://hjz.zdbjq.cn

wc -l < a.txt
来源：http://znz.bbcook.cn

[R43] 按名字查找文件
来源：http://kox.yj202588.top

find . -name "*.log" -type f
来源：http://tls.tanke756.top

[R44] 按修改时间查找
来源：http://txg.cdnleiting.top

find . -mtime -7 -type f
来源：http://has.nwbrower.top

[R45] 批量删除
来源：http://jlr.yj202588.top

find . -name "*.tmp" -delete
来源：http://yqc.nanxinkj.top

[R46] 递归替换文件内容
来源：http://fiw.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gvl.yangfankeji.com

[R47] sed 单行替换
来源：http://xdf.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://lho.ppjwa.cn

[R48] awk 取指定列
来源：http://ezs.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://awn.vehdjk.com

[R49] awk 带条件
来源：http://vow.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mvk.tanke756.top

[R50] awk 求和
来源：http://eyu.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jgj.dashuyun.cn

[R51] 排序去重取前几
来源：http://oyr.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bgw.hnxiangtu.top

[R52] 统计行数
来源：http://nvh.hesvh.cn

wc -l a.txt
来源：http://vfl.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://sfc.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hvn.c1oappe.top

[R54] 比较两个文件
来源：http://cwm.fanxiaobao.xyz

diff a.txt b.txt
来源：http://rqk.gogol.net.cn

[R55] 压缩与解压
来源：http://mhs.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://opv.xinyue.icu

[R56] 远程拷贝
来源：http://fou.ivvv.top

scp file user@host:/path/
来源：http://ihv.316326.xyz

[R57] 远程执行命令
来源：http://byi.zdbjq.cn

ssh user@host 'uptime'
来源：http://vgy.shanyushiyangkeji.top

[R58] 下载文件
来源：http://hbr.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qgc.cheryme.top

[R59] 发 POST JSON
来源：http://bqb.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ifx.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://bgf.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lbw.yj20258888.top

[R61] 磁盘占用
来源：http://ogu.feifeiyinyue.top

df -h;  du -sh *
来源：http://wdz.xuanzx.com

[R62] 找最占空间的文件
来源：http://brn.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://mpq.tanke756.top

[R63] 内存与进程
来源：http://wlr.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://yyg.jiagoushi.top

[R64] 结束进程
来源：http://blr.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://mmz.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://fhr.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://krk.nwbrower.top

[R66] 定时任务
来源：http://zzp.jianghu66.top

crontab -e;  crontab -l
来源：http://aaf.xinyue.icu

[R67] 生成随机十六进制串
来源：http://wnw.shuidangran.top

openssl rand -hex 16
来源：http://lln.fzhhl.top

[R68] 计算文件校验值
来源：http://whk.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://lit.sysykeji.top

[R69] 生成随机密码
来源：http://oer.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://ktq.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://bwz.andypj.xyz

date +%s;  date -d @1700000000
来源：http://ypl.fehbvm.com

[R71] 日期格式化
来源：http://tnr.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jep.ctjpmb.com

[R72] 等待端口就绪
来源：http://rpb.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cro.fehbvm.com

[R73] 分割大日志
来源：http://qao.yuxming.cn

split -l 1000 big.log part_
来源：http://xvu.ivvv.top

[R74] 批量重命名
来源：http://das.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpn.sxryk.cn

[R75] 导出环境变量
来源：http://gtt.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://ljy.sysykeji.top

[R76] 使用临时文件
来源：http://tmt.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://amk.gotoacloud.top

[R77] 读取用户输入
来源：http://ovq.ydjk.org.cn

read -rp "请输入: " ans
来源：http://fkt.gzhubu.top

[R78] 交互式菜单
来源：http://lhz.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://mlm.yj20258888.top

[R79] 解析命令行选项
来源：http://piy.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fqv.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://fwp.zhijiandao.cn

time ./run.sh
来源：http://rco.hfpthk.cn

================================================================================
来源：http://bgk.quarkkingdee.top

S. C / C++ 专题
来源：http://syf.yanxiufei.cn

================================================================================
来源：http://cru.shzxlz.cn

[S01] C：Hello World
来源：http://yeb.zhaomingkeji.xyz

#include <stdio.h>
来源：http://wpw.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nuy.yj20258.top

[S02] C：变量与格式化输出
来源：http://okt.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://ifq.daxiang520.top

[S03] C：读入整数
来源：http://mko.nanxinkj.top

int x; scanf("%d", &x);
来源：http://ifq.mhx1999.top

[S04] C：字符串复制
来源：http://tmq.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fft.mhx1999.top

[S05] C：字符串长度
来源：http://ynp.tianlin.xyz

strlen(s)
来源：http://xvm.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://ygu.mhx1999.top

strcmp(a, b) == 0
来源：http://mur.hesvh.cn

[S07] C：数组遍历求和
来源：http://atg.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://efm.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://pwk.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kfb.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://qur.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mdr.jiagoushi.top

[S10] C：指针与解引用
来源：http://soj.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://eha.hysaishi.cn

[S11] C：逐行读文件
来源：http://ftd.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://dmc.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cdw.jqgfzy.top

fclose(f);
来源：http://lmr.nanxinkj.top

[S12] C：写文件
来源：http://szd.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ntd.yuxming.cn

[S13] C：宏定义
来源：http://tby.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wsu.hysaishi.cn

[S14] C：枚举
来源：http://xqu.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ygb.ivvv.top

[S15] C：类型转换
来源：http://niv.snrcjt.cn

(double) a / b
来源：http://ldp.chenzaomai.com

[S16] C：位操作置位
来源：http://lnz.yueranfly.top

x |= (1 << 3);
来源：http://jkw.wangdashe.top

[S17] C：安全拼接字符串
来源：http://ksz.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zxg.zhiwuduotai.top

[S18] C：命令行参数
来源：http://hzv.sysykeji.top

int main(int argc, char **argv)
来源：http://lsh.yanxiufei.cn

[S19] C：快速排序
来源：http://khv.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://eba.dianchejie.cn

[S20] C：二分查找
来源：http://mla.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hrz.guowangkeji.top

[S21] C：字符类别判断
来源：http://yui.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tgs.chenzaomai.com

[S22] C：字符串转数字
来源：http://ssj.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://jmz.jinqigufen.top

[S23] C：随机数
来源：http://imb.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qzg.nanxinkj.top

[S24] C：获取本地时间
来源：http://xys.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vnl.shzxlz.cn

[S25] C：内存拷贝
来源：http://icz.guannengcc.top

memcpy(dst, src, n);
来源：http://ozn.yvedp.cn

[S26] C：内存清零
来源：http://fil.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://cei.chenzaomai.com

[S27] C：定义常量
来源：http://xjr.snrcjt.cn

const double PI = 3.14159;
来源：http://ywp.fanxiaobao.xyz

[S28] C：静态变量
来源：http://soj.guannengcc.top

static int counter = 0;
来源：http://yim.zhengqikj.top

[S29] C：变参函数
来源：http://pmt.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mzn.316326.xyz

[S30] C：头文件保护
来源：http://yff.zhijiandao.cn

#ifndef X_H
来源：http://cht.zdbjq.cn

#define X_H
来源：http://ixh.iojbl.cn

#endif
来源：http://otk.tianlin.xyz

[S31] C++：Hello World
来源：http://aeq.havefunace.top

#include <iostream>
来源：http://gkv.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://cej.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://wsu.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://qsc.gotoacloud.top

[S33] C++：vector 增删
来源：http://qow.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dbx.meibo888.top

[S34] C++：遍历 vector
来源：http://nuc.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://ngz.xziqi.cn

[S35] C++：map
来源：http://fmo.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://elu.xinyue.icu

[S36] C++：unordered_map
来源：http://bgn.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zxd.jinqigufen.top

[S37] C++：set
来源：http://ito.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wxw.cucudq.cn

[S38] C++：排序
来源：http://cqv.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://qtb.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://ouu.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ber.shzxlz.cn

[S40] C++：查找元素
来源：http://not.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mfu.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://pkp.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bcj.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://ovq.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://cgo.jinqigufen.top

[S43] C++：智能指针
来源：http://ckw.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://jxl.yj20258.top

[S44] C++：引用传参
来源：http://ywy.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://hrh.yongpay.top

[S45] C++：lambda
来源：http://xom.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lmu.aibaodan.cn

[S46] C++：函数模板
来源：http://kwz.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xhy.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://ede.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qle.havefunace.top

[S48] C++：逐行读文件
来源：http://ebd.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://iam.xuanzx.com

while (std::getline(in, line)) { }
来源：http://lgl.kuanghao11.cn

[S49] C++：写文件
来源：http://gte.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xzw.sysykeji.top

[S50] C++：格式化数字
来源：http://ujo.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bso.hcnkem.com

[S51] C++：显式类型转换
来源：http://gor.jinqigufen.top

static_cast<double>(a) / b
来源：http://cdc.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://jbg.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://jea.havefunace.top

[S53] C++：移动语义
来源：http://oeq.yj20258.top

std::vector<int> w = std::move(v);
来源：http://huz.fengsongda.top

[S54] C++：异常处理
来源：http://fmw.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dsb.hammf.cn

[S55] C++：结构化绑定
来源：http://ozn.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://icc.daria6918.cn

[S56] C++：optional
来源：http://bft.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://itb.jianghu66.top

[S57] C++：编译期常量
来源：http://wwb.snrcjt.cn

constexpr int N = 10;
来源：http://plo.zhiwuduotai.top

[S58] C++：命名空间
来源：http://vgi.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://wsi.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://bie.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://arm.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://msi.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pyw.zycfv.cn

================================================================================
来源：http://lgj.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://frq.dashuyun.cn

================================================================================
来源：http://weg.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://sjg.nanxinkj.top

println("Hello")
来源：http://itq.jqgfzy.top

[T02] Kotlin：变量
来源：http://hxn.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zxr.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://fsu.guannengcc.top

"值: $b"
来源：http://zwz.guowangkeji.top

[T04] Kotlin：空安全
来源：http://ffw.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://dob.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://tuw.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ybg.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://xro.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://min.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://zco.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://csa.hesvh.cn

[T08] Kotlin：数据类
来源：http://ulq.ivvv.top

data class User(val name: String, val age: Int)
来源：http://din.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://eoe.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://wjh.andypj.xyz

[T10] Kotlin：默认参数
来源：http://tlr.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zvn.tanke756.top

[T11] Kotlin：协程
来源：http://uuq.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kks.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://xyv.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://fke.yj202588.top

[T13] Kotlin：只读 Map
来源：http://pqe.havefunace.top

val m = mapOf("a" to 1)
来源：http://jaf.snrcjt.cn

[T14] Kotlin：循环
来源：http://nug.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://zls.fktsv.cn

[T15] Kotlin：接口
来源：http://ifp.vehdjk.com

interface Shape { fun area(): Double }
来源：http://kfa.yongpay.top

[T16] Swift：Hello World
来源：http://jiu.xuanzx.com

print("Hello")
来源：http://fds.meibo888.top

[T17] Swift：变量与常量
来源：http://vjr.chenzaomai.com

var a = 1;  let b = 2
来源：http://rlw.yongpay.top

[T18] Swift：字符串插值
来源：http://rdw.ivvv.top

"值: \(b)"
来源：http://phw.gogol.net.cn


<!-- 参考信息 -->