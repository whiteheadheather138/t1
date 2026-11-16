代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://ilz.nanxinkj.top

[R14] C 风格 for
来源：http://mdm.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ydp.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://zje.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jrd.xziqi.cn

[R16] until 等待条件
来源：http://dbi.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fpf.ppjwa.cn

[R17] 数组定义与取值
来源：http://fxc.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dhj.havefunace.top

[R18] 遍历数组
来源：http://kbv.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://von.birdmap.top

[R19] 数组长度
来源：http://mfq.xylfe.cn

echo "${#arr[@]}"
来源：http://dzu.meibo888.top

[R20] 关联数组（字典）
来源：http://gtu.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfm.zhiwuduotai.top

[R21] 字符串长度
来源：http://yps.zhengqikj.top

echo "${#s}"
来源：http://atm.zhoulong.xyz

[R22] 截取子串
来源：http://yij.cqqwz.cn

echo "${s:0:5}"
来源：http://cyc.hcnkem.com

[R23] 字符串替换
来源：http://bcz.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sux.snrcjt.cn

[R24] 大小写转换
来源：http://qdh.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://skr.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://jex.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mbn.dashuyun.cn

[R26] 命令替换
来源：http://nrx.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://odc.gotoacloud.top

[R27] 算术展开
来源：http://ekb.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://gll.sweek.top

[R28] 浮点运算
来源：http://abr.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://nxz.feifeiyinyue.top

[R29] 定义函数
来源：http://xfn.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lil.chenzaomai.com

[R30] 函数返回状态码
来源：http://shd.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://amz.hammf.cn

[R31] 局部变量
来源：http://rqb.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://llg.shangyingyoupin.top

[R32] 参数个数校验
来源：http://mym.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rdj.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://njl.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xli.guannengcc.top

[R34] 退出时清理
来源：http://cwy.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://qkk.tian-w.cn

[R35] 后台执行并等待
来源：http://bxk.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mxy.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://wzm.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pvq.cashguo.top

[R37] 把输出赋给变量
来源：http://ija.zhiwuduotai.top

files=$(ls -1)
来源：http://ukn.hongshengwenyu.top

[R38] 管道串联
来源：http://jgo.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://uui.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://kwa.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://wta.nanxuanxn.top

[R40] 追加写日志
来源：http://psm.hongshengwenyu.top

echo "log" >> out.log
来源：http://quw.dianchejie.cn

[R41] 丢弃输出
来源：http://bjz.yonumen.top

cmd >/dev/null 2>&1
来源：http://bql.sjlbkw.cn

[R42] 输入重定向
来源：http://jry.yonumen.top

wc -l < a.txt
来源：http://kqa.uphjek.com

[R43] 按名字查找文件
来源：http://ygm.xylfe.cn

find . -name "*.log" -type f
来源：http://fdb.yj20258888.top

[R44] 按修改时间查找
来源：http://uhs.ppjwa.cn

find . -mtime -7 -type f
来源：http://aln.zhaomingkeji.xyz

[R45] 批量删除
来源：http://nsf.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://xnz.chenlongwang.top

[R46] 递归替换文件内容
来源：http://kgk.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qod.bbcook.cn

[R47] sed 单行替换
来源：http://ddf.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jom.hysaishi.cn

[R48] awk 取指定列
来源：http://dbg.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://klb.0kj1m.cn

[R49] awk 带条件
来源：http://qut.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qyf.zdqjudy.top

[R50] awk 求和
来源：http://lpp.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://dmo.ctjpmb.com

[R51] 排序去重取前几
来源：http://phf.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://etj.daria6918.cn

[R52] 统计行数
来源：http://zra.smart0.xyz

wc -l a.txt
来源：http://ktn.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://vqf.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mvb.svipenyu.cn

[R54] 比较两个文件
来源：http://vth.jianghu66.top

diff a.txt b.txt
来源：http://fnt.xuanzx.com

[R55] 压缩与解压
来源：http://viu.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ljv.svipenyu.cn

[R56] 远程拷贝
来源：http://hfx.jqgufenzy.top

scp file user@host:/path/
来源：http://ijq.hongshengwenyu.top

[R57] 远程执行命令
来源：http://qdk.yj20258.top

ssh user@host 'uptime'
来源：http://bau.yj20258.top

[R58] 下载文件
来源：http://nax.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iyc.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://nit.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dxl.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://bvg.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eve.ppjwa.cn

[R61] 磁盘占用
来源：http://vgn.xuanzx.com

df -h;  du -sh *
来源：http://jed.guowangkeji.top

[R62] 找最占空间的文件
来源：http://rtq.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://hfm.jinqigfzy.top

[R63] 内存与进程
来源：http://cbi.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://cxi.zhaomingkeji.xyz

[R64] 结束进程
来源：http://ieu.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://jvj.ehwqpu.com

[R65] 查看端口占用
来源：http://efb.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ady.shangyingyoupin.top

[R66] 定时任务
来源：http://asy.smart0.xyz

crontab -e;  crontab -l
来源：http://rvc.316326.xyz

[R67] 生成随机十六进制串
来源：http://svi.yj202588.top

openssl rand -hex 16
来源：http://qul.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://ybc.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tjd.dashuyun.cn

[R69] 生成随机密码
来源：http://fwn.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://cyv.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://jvp.xuanzx.com

date +%s;  date -d @1700000000
来源：http://beq.gaohongyu789.top

[R71] 日期格式化
来源：http://ebx.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hnz.0kj1m.cn

[R72] 等待端口就绪
来源：http://jaa.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rxf.yfazqb.com

[R73] 分割大日志
来源：http://hgl.pycfn.com

split -l 1000 big.log part_
来源：http://sgw.wangshuangyany.cn

[R74] 批量重命名
来源：http://scd.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysv.wangshuangyany.cn

[R75] 导出环境变量
来源：http://var.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://xws.hcnkem.com

[R76] 使用临时文件
来源：http://wdb.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://juw.chenjidiqi.icu

[R77] 读取用户输入
来源：http://syp.vqdsnc.cn

read -rp "请输入: " ans
来源：http://iyz.tarul.cn

[R78] 交互式菜单
来源：http://myl.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rwb.birdmap.top

[R79] 解析命令行选项
来源：http://ahm.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lie.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://uny.xuanzx.com

time ./run.sh
来源：http://iuk.fktsv.cn

================================================================================
来源：http://flo.9152youxi.cn

S. C / C++ 专题
来源：http://mrv.birdmap.top

================================================================================
来源：http://xuu.xuetiantiany.cn

[S01] C：Hello World
来源：http://gky.0kj1m.cn

#include <stdio.h>
来源：http://tbp.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cll.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://yql.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://ots.cucudq.cn

[S03] C：读入整数
来源：http://edb.gogol.net.cn

int x; scanf("%d", &x);
来源：http://sbn.hesvh.cn

[S04] C：字符串复制
来源：http://tll.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bya.jqgufenzy.top

[S05] C：字符串长度
来源：http://krj.bbcook.cn

strlen(s)
来源：http://kod.vehdjk.com

[S06] C：字符串比较
来源：http://zkl.shuidangran.top

strcmp(a, b) == 0
来源：http://upg.nanxinkj.top

[S07] C：数组遍历求和
来源：http://gdw.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qqd.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://kwl.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hof.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://nzo.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xkt.daria6918.cn

[S10] C：指针与解引用
来源：http://jgn.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://wxm.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://diw.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://ofe.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bmn.xuetiantiany.cn

fclose(f);
来源：http://psn.ybcxt.top

[S12] C：写文件
来源：http://xuj.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lun.zhoulong.xyz

[S13] C：宏定义
来源：http://jlo.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xus.yvedp.cn

[S14] C：枚举
来源：http://wde.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://itn.sufxvd.cn

[S15] C：类型转换
来源：http://cvz.hesvh.cn

(double) a / b
来源：http://ccb.zhoulong.xyz

[S16] C：位操作置位
来源：http://sua.cashguo.top

x |= (1 << 3);
来源：http://ncz.sxryk.cn

[S17] C：安全拼接字符串
来源：http://gnf.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cbb.havefunace.top

[S18] C：命令行参数
来源：http://ylu.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://fbb.havefunace.top

[S19] C：快速排序
来源：http://ptz.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vqs.yuxming.cn

[S20] C：二分查找
来源：http://efh.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lhd.fehbvm.com

[S21] C：字符类别判断
来源：http://urj.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://omr.nanxinkj.top

[S22] C：字符串转数字
来源：http://wpm.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://cqk.yueranfly.top

[S23] C：随机数
来源：http://ded.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://leu.jianghu66.top

[S24] C：获取本地时间
来源：http://ayg.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://apu.9152youxi.cn

[S25] C：内存拷贝
来源：http://kti.yongpay.top

memcpy(dst, src, n);
来源：http://pkx.zhiwuduotai.top

[S26] C：内存清零
来源：http://mlb.ivvv.top

memset(a, 0, sizeof a);
来源：http://thw.uphjek.com

[S27] C：定义常量
来源：http://hsl.jinqigfzy.top

const double PI = 3.14159;
来源：http://xun.yongpay.top

[S28] C：静态变量
来源：http://uin.xziqi.cn

static int counter = 0;
来源：http://pev.fanxiaobao.xyz

[S29] C：变参函数
来源：http://uip.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hrz.c1oappe.top

[S30] C：头文件保护
来源：http://wum.svipenyu.cn

#ifndef X_H
来源：http://gim.hnqzz.top

#define X_H
来源：http://sru.0kj1m.cn

#endif
来源：http://rwe.sysykeji.top

[S31] C++：Hello World
来源：http://txj.gaohongyu789.top

#include <iostream>
来源：http://koz.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://jkw.guannengcc.top

[S32] C++：字符串
来源：http://amj.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://ren.chenzaomai.com

[S33] C++：vector 增删
来源：http://aoh.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xvt.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://ibc.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://zhw.svipenyu.cn

[S35] C++：map
来源：http://ihu.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dkh.zhongyouzk.top

[S36] C++：unordered_map
来源：http://ymh.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pln.jqgufenzy.top

[S37] C++：set
来源：http://xyp.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://giw.nanxinkj.top

[S38] C++：排序
来源：http://hxz.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://vrx.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://kel.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fvj.zhongyouzk.top

[S40] C++：查找元素
来源：http://vcd.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://byg.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://kxn.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tdv.aizwys.cn

[S42] C++：继承与虚函数
来源：http://sqb.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://lbq.cashguo.top

[S43] C++：智能指针
来源：http://gag.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://xqn.iojbl.cn

[S44] C++：引用传参
来源：http://xpi.ivvv.top

void inc(int &x) { ++x; }
来源：http://frx.guannengcc.top

[S45] C++：lambda
来源：http://qij.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://ajd.bbcook.cn

[S46] C++：函数模板
来源：http://bbo.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vwb.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://zog.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dho.hywenlv.cn

[S48] C++：逐行读文件
来源：http://klu.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lqw.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://owb.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://drn.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://axm.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://hmk.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uub.yongpay.top

[S51] C++：显式类型转换
来源：http://cbx.sjlbkw.cn

static_cast<double>(a) / b
来源：http://hjb.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://wea.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://kut.dianchejie.cn

[S53] C++：移动语义
来源：http://zfn.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://igk.vqdsnc.cn

[S54] C++：异常处理
来源：http://hog.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mpf.ctjpmb.com

[S55] C++：结构化绑定
来源：http://lmo.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kud.havefunace.top

[S56] C++：optional
来源：http://zix.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://etv.pycfn.com

[S57] C++：编译期常量
来源：http://ujo.nanxuanxn.top

constexpr int N = 10;
来源：http://lge.zhongyouzk.top

[S58] C++：命名空间
来源：http://rrl.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://zxp.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://jww.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://psa.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://ojm.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://prv.fzhhl.top

================================================================================
来源：http://hiu.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jwr.feifeiyinyue.top

================================================================================
来源：http://cas.yueranfly.top

[T01] Kotlin：Hello World
来源：http://abm.smart0.xyz

println("Hello")
来源：http://rbm.uphjek.com

[T02] Kotlin：变量
来源：http://jxl.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jny.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://qvd.gaohongyu789.top

"值: $b"
来源：http://uqi.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://www.jyoumei.cn

val n: String? = null;  n?.length
来源：http://moj.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://syo.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://shg.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://leb.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mca.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://frs.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pqb.chenzaomai.com

[T08] Kotlin：数据类
来源：http://ewp.birdmap.top

data class User(val name: String, val age: Int)
来源：http://sfe.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://toz.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://fdv.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://san.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jzx.redwolf501.top

[T11] Kotlin：协程
来源：http://fve.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uyq.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://vup.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://qyg.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://zuu.yfazqb.com

val m = mapOf("a" to 1)
来源：http://weh.cucudq.cn

[T14] Kotlin：循环
来源：http://ohh.xylfe.cn

for (i in 1..10) println(i)
来源：http://pby.wangdashe.top

[T15] Kotlin：接口
来源：http://hlp.vehdjk.com

interface Shape { fun area(): Double }
来源：http://bwm.hammf.cn

[T16] Swift：Hello World
来源：http://pws.xuetiantiany.cn

print("Hello")
来源：http://vbu.jyoumei.cn


<!-- 参考信息 -->