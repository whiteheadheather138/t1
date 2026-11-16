代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://aph.vehdjk.com

[R18] 遍历数组
来源：http://gvs.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tck.0kj1m.cn

[R19] 数组长度
来源：http://wsy.shzxlz.cn

echo "${#arr[@]}"
来源：http://bnl.nwbrower.top

[R20] 关联数组（字典）
来源：http://pvf.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xwu.xuanzx.com

[R21] 字符串长度
来源：http://jvp.aibaodan.cn

echo "${#s}"
来源：http://arw.wangshuangyany.cn

[R22] 截取子串
来源：http://jxu.tarul.cn

echo "${s:0:5}"
来源：http://vux.ivvv.top

[R23] 字符串替换
来源：http://lrl.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://exo.xuetiantiany.cn

[R24] 大小写转换
来源：http://vpu.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://kgn.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://voh.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://hwg.yongpay.top

[R26] 命令替换
来源：http://ptn.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://ace.aizwys.cn

[R27] 算术展开
来源：http://hnt.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://nbv.aibaodan.cn

[R28] 浮点运算
来源：http://cbx.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://ozn.zdqjudy.top

[R29] 定义函数
来源：http://mlh.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://duj.chenlongwang.top

[R30] 函数返回状态码
来源：http://kzm.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://qxd.cdnleiting.top

[R31] 局部变量
来源：http://buq.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://udk.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://rdu.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jmj.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://sww.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cza.jiagoushi.top

[R34] 退出时清理
来源：http://umj.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://teo.sxryk.cn

[R35] 后台执行并等待
来源：http://muh.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qvw.havefunace.top

[R36] 并发执行多个任务
来源：http://awo.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jxn.chenzaomai.com

[R37] 把输出赋给变量
来源：http://vnh.jyoumei.cn

files=$(ls -1)
来源：http://igj.sjlbkw.cn

[R38] 管道串联
来源：http://isi.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://fvn.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://hxv.ydjk.org.cn

cmd > out.log 2>&1
来源：http://jdi.quarkkingdee.top

[R40] 追加写日志
来源：http://cvw.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://tdb.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://gyp.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://zry.tian-w.cn

[R42] 输入重定向
来源：http://dgg.jinqigufen.top

wc -l < a.txt
来源：http://fso.jlsjyb.cn

[R43] 按名字查找文件
来源：http://spl.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://kjb.daxiang520.top

[R44] 按修改时间查找
来源：http://xek.zhoulong.xyz

find . -mtime -7 -type f
来源：http://usd.sweek.top

[R45] 批量删除
来源：http://ige.wangdashe.top

find . -name "*.tmp" -delete
来源：http://gjc.aizwys.cn

[R46] 递归替换文件内容
来源：http://dqj.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zip.hnqzz.top

[R47] sed 单行替换
来源：http://eaj.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://chq.ydzc1.top

[R48] awk 取指定列
来源：http://aks.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://mkg.hcnkem.com

[R49] awk 带条件
来源：http://jqm.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eoi.vehdjk.com

[R50] awk 求和
来源：http://yzq.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://fwo.cucudq.cn

[R51] 排序去重取前几
来源：http://xfv.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://pfz.cqqwz.cn

[R52] 统计行数
来源：http://ulp.vehdjk.com

wc -l a.txt
来源：http://cot.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://vhj.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://woe.jianghu66.top

[R54] 比较两个文件
来源：http://izd.xuanzx.com

diff a.txt b.txt
来源：http://uhz.uphjek.com

[R55] 压缩与解压
来源：http://isg.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nsc.zhiwuduotai.top

[R56] 远程拷贝
来源：http://rjk.redwolf501.top

scp file user@host:/path/
来源：http://diq.nanxuanxn.top

[R57] 远程执行命令
来源：http://dim.hysaishi.cn

ssh user@host 'uptime'
来源：http://pwq.xinyue.icu

[R58] 下载文件
来源：http://fmz.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://edh.sweek.top

[R59] 发 POST JSON
来源：http://zvq.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ezw.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://qkr.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pea.fehbvm.com

[R61] 磁盘占用
来源：http://zyz.wangdashe.top

df -h;  du -sh *
来源：http://xhv.ppjwa.cn

[R62] 找最占空间的文件
来源：http://ksa.9152youxi.cn

du -ah . | sort -rh | head -10
来源：http://eks.daxiang520.top

[R63] 内存与进程
来源：http://dqc.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://hqk.yangfankeji.com

[R64] 结束进程
来源：http://rlv.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://mvd.jiagoushi.top

[R65] 查看端口占用
来源：http://tiy.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxd.yj20258888.top

[R66] 定时任务
来源：http://kgk.snrcjt.cn

crontab -e;  crontab -l
来源：http://mxe.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://otw.nanxuanxn.top

openssl rand -hex 16
来源：http://zmp.yangfankeji.com

[R68] 计算文件校验值
来源：http://jpp.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ucl.hnxiangtu.top

[R69] 生成随机密码
来源：http://rkp.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://gaq.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://mjf.cashguo.top

date +%s;  date -d @1700000000
来源：http://vpe.uphjek.com

[R71] 日期格式化
来源：http://gcs.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ylp.tarul.cn

[R72] 等待端口就绪
来源：http://tml.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hrm.hnqzz.top

[R73] 分割大日志
来源：http://yhx.gzhubu.top

split -l 1000 big.log part_
来源：http://lli.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://kob.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ilj.fengsongda.top

[R75] 导出环境变量
来源：http://xru.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://wcd.daria6918.cn

[R76] 使用临时文件
来源：http://dqh.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ycm.hesvh.cn

[R77] 读取用户输入
来源：http://hcn.yj20258888.top

read -rp "请输入: " ans
来源：http://vzu.ydzc1.top

[R78] 交互式菜单
来源：http://ouh.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sqc.ivvv.top

[R79] 解析命令行选项
来源：http://tzf.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qfq.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://oip.fehbvm.com

time ./run.sh
来源：http://hwc.yanxiufei.cn

================================================================================
来源：http://hff.nwbrower.top

S. C / C++ 专题
来源：http://fdr.9152youxi.cn

================================================================================
来源：http://kwz.cheryme.top

[S01] C：Hello World
来源：http://ocr.yfazqb.com

#include <stdio.h>
来源：http://ncu.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tqe.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://cii.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://azc.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://caj.jianghu66.top

int x; scanf("%d", &x);
来源：http://xeh.birdmap.top

[S04] C：字符串复制
来源：http://ktz.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ebk.yvedp.cn

[S05] C：字符串长度
来源：http://hkn.xziqi.cn

strlen(s)
来源：http://vdz.hongshengwenyu.top

[S06] C：字符串比较
来源：http://nsz.chenlongwang.top

strcmp(a, b) == 0
来源：http://dqr.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://fkv.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pwy.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://jka.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iid.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://gbc.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vaq.nwbrower.top

[S10] C：指针与解引用
来源：http://xun.sxryk.cn

int *p = &a;  *p = 5;
来源：http://wzx.svipenyu.cn

[S11] C：逐行读文件
来源：http://kuy.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://gjx.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rrc.yj202588.top

fclose(f);
来源：http://dyy.cdnleiting.top

[S12] C：写文件
来源：http://ars.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gvy.chenzaomai.com

[S13] C：宏定义
来源：http://fve.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nde.xinyue.icu

[S14] C：枚举
来源：http://zxa.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://efg.fzhhl.top

[S15] C：类型转换
来源：http://cmm.yongpay.top

(double) a / b
来源：http://jjz.kuanghao11.cn

[S16] C：位操作置位
来源：http://nlk.fktsv.cn

x |= (1 << 3);
来源：http://bdr.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://ieh.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ghm.yueranfly.top

[S18] C：命令行参数
来源：http://ecb.jinqigufen.top

int main(int argc, char **argv)
来源：http://see.ydjk.org.cn

[S19] C：快速排序
来源：http://lak.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ozr.zhongyouzk.top

[S20] C：二分查找
来源：http://ywn.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rdq.gzhubu.top

[S21] C：字符类别判断
来源：http://mpl.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dyj.jyoumei.cn

[S22] C：字符串转数字
来源：http://olv.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://vsq.zycfv.cn

[S23] C：随机数
来源：http://nbm.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://egd.zhoulong.xyz

[S24] C：获取本地时间
来源：http://yne.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ukv.sysykeji.top

[S25] C：内存拷贝
来源：http://cnq.nwbrower.top

memcpy(dst, src, n);
来源：http://djk.hesvh.cn

[S26] C：内存清零
来源：http://rip.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://hbb.ctjpmb.com

[S27] C：定义常量
来源：http://doi.jlsjyb.cn

const double PI = 3.14159;
来源：http://vhg.ydjk.org.cn

[S28] C：静态变量
来源：http://ult.sjlbkw.cn

static int counter = 0;
来源：http://hyp.yuanzhike.top

[S29] C：变参函数
来源：http://bxn.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://drw.hammf.cn

[S30] C：头文件保护
来源：http://kaq.shuidangran.top

#ifndef X_H
来源：http://awu.gzhubu.top

#define X_H
来源：http://hxr.cashguo.top

#endif
来源：http://bpd.pycfn.com

[S31] C++：Hello World
来源：http://aoq.yonumen.top

#include <iostream>
来源：http://tfc.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://jih.daxiang520.top

[S32] C++：字符串
来源：http://kno.cashguo.top

std::string s = "hi";  s += "!";
来源：http://eah.316326.xyz

[S33] C++：vector 增删
来源：http://eef.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mwr.zhengqikj.top

[S34] C++：遍历 vector
来源：http://vdy.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://idc.cheryme.top

[S35] C++：map
来源：http://crj.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hlx.tarul.cn

[S36] C++：unordered_map
来源：http://ujx.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oxz.xinyue.icu

[S37] C++：set
来源：http://awa.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pkl.nanxinkj.top

[S38] C++：排序
来源：http://jsl.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://nml.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://dgm.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qfu.tian-w.cn

[S40] C++：查找元素
来源：http://xte.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lpg.cdnleiting.top

[S41] C++：类与构造函数
来源：http://rsj.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iqx.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://brj.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://bby.sxryk.cn

[S43] C++：智能指针
来源：http://xjl.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://elk.gogol.net.cn

[S44] C++：引用传参
来源：http://ppk.yongpay.top

void inc(int &x) { ++x; }
来源：http://icv.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://tui.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://kaq.sjlbkw.cn

[S46] C++：函数模板
来源：http://jev.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://omz.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://xkt.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mjw.sufxvd.cn

[S48] C++：逐行读文件
来源：http://mxj.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://rfu.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://osv.yonumen.top

[S49] C++：写文件
来源：http://qbw.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fgo.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://rda.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsk.fzhhl.top

[S51] C++：显式类型转换
来源：http://uky.zycfv.cn

static_cast<double>(a) / b
来源：http://uek.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://dsm.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://xud.0kj1m.cn

[S53] C++：移动语义
来源：http://hzb.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://gva.cashguo.top

[S54] C++：异常处理
来源：http://sub.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tvs.ivvv.top

[S55] C++：结构化绑定
来源：http://lla.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gje.ydjk.org.cn

[S56] C++：optional
来源：http://hbb.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sqj.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://krj.ivvv.top

constexpr int N = 10;
来源：http://ozc.jqgufenzy.top

[S58] C++：命名空间
来源：http://rks.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://hjl.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://eek.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gxu.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://tnp.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bbq.zycfv.cn

================================================================================
来源：http://tjr.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oeu.ywan-chungtsiang.top

================================================================================
来源：http://ref.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://gek.sufxvd.cn

println("Hello")
来源：http://vzn.snrcjt.cn

[T02] Kotlin：变量
来源：http://fmz.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zsa.hammf.cn

[T03] Kotlin：字符串模板
来源：http://jly.yangfankeji.com

"值: $b"
来源：http://kid.xinyue.icu

[T04] Kotlin：空安全
来源：http://asx.ybcxt.top

val n: String? = null;  n?.length
来源：http://zyg.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://htg.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bau.bbcook.cn

[T06] Kotlin：集合映射
来源：http://zbw.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://jar.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://uxi.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zxs.ybcxt.top

[T08] Kotlin：数据类
来源：http://rqu.yj202588.top

data class User(val name: String, val age: Int)
来源：http://mqp.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://nnm.havefunace.top

fun String.exclaim() = this + "!"
来源：http://zho.ybcxt.top

[T10] Kotlin：默认参数
来源：http://dsy.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://akj.zdqjudy.top

[T11] Kotlin：协程
来源：http://wxp.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sdv.xylfe.cn

[T12] Kotlin：解构声明
来源：http://yst.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://bir.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://ncl.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://igh.guannengcc.top

[T14] Kotlin：循环
来源：http://xcs.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://nfy.vehdjk.com

[T15] Kotlin：接口
来源：http://uyn.daxiang520.top

interface Shape { fun area(): Double }
来源：http://nkj.hesvh.cn

[T16] Swift：Hello World
来源：http://zgz.jinyuanbaomall.cn

print("Hello")
来源：http://vmh.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://inq.ydzc1.top

var a = 1;  let b = 2
来源：http://gof.pycfn.com

[T18] Swift：字符串插值
来源：http://xel.zhixingplan.top

"值: \(b)"
来源：http://ief.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://kcv.hcnkem.com

if let n = opt { print(n) }
来源：http://cyx.316326.xyz

[T20] Swift：数组操作
来源：http://vfg.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://myo.hnxiangtu.top


<!-- 参考信息 -->