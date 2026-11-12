代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://xab.birdmap.top

[R14] C 风格 for
来源：http://uds.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hgc.guannengcc.top

[R15] while 逐行读文件
来源：http://yff.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://esa.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://xhr.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dlp.sweek.top

[R17] 数组定义与取值
来源：http://ift.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://yoy.jlsjyb.cn

[R18] 遍历数组
来源：http://uqq.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://evs.hesvh.cn

[R19] 数组长度
来源：http://joz.vehdjk.com

echo "${#arr[@]}"
来源：http://psq.jianghu66.top

[R20] 关联数组（字典）
来源：http://szb.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lfd.havefunace.top

[R21] 字符串长度
来源：http://qno.cqqwz.cn

echo "${#s}"
来源：http://xos.daxiang520.top

[R22] 截取子串
来源：http://ocg.vehdjk.com

echo "${s:0:5}"
来源：http://mrf.zdbjq.cn

[R23] 字符串替换
来源：http://roz.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ten.pycfn.com

[R24] 大小写转换
来源：http://ixd.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://zss.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://and.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lwh.fengsongda.top

[R26] 命令替换
来源：http://ytl.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://hvf.fehbvm.com

[R27] 算术展开
来源：http://idt.ybcxt.top

echo $((1 + 2 * 3))
来源：http://pto.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://vrz.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://kke.epnwcf.com

[R29] 定义函数
来源：http://yjh.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pcg.cheryme.top

[R30] 函数返回状态码
来源：http://sgy.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://gtg.chenlongwang.top

[R31] 局部变量
来源：http://tpl.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://vaf.cashguo.top

[R32] 参数个数校验
来源：http://aon.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gwp.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://rsi.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oxa.svipenyu.cn

[R34] 退出时清理
来源：http://btd.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://jnh.hesvh.cn

[R35] 后台执行并等待
来源：http://onn.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jam.shuidangran.top

[R36] 并发执行多个任务
来源：http://hib.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iwj.smart0.xyz

[R37] 把输出赋给变量
来源：http://tou.yongpay.top

files=$(ls -1)
来源：http://cox.hongshengwenyu.top

[R38] 管道串联
来源：http://nfo.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://xrj.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://kma.xinyue.icu

cmd > out.log 2>&1
来源：http://iec.yangfankeji.com

[R40] 追加写日志
来源：http://gic.fktsv.cn

echo "log" >> out.log
来源：http://jxy.fengsongda.top

[R41] 丢弃输出
来源：http://vud.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://hgq.aizwys.cn

[R42] 输入重定向
来源：http://xlo.jyoumei.cn

wc -l < a.txt
来源：http://ogj.yonumen.top

[R43] 按名字查找文件
来源：http://zql.sweek.top

find . -name "*.log" -type f
来源：http://sjn.yangfankeji.com

[R44] 按修改时间查找
来源：http://uzy.tanke756.top

find . -mtime -7 -type f
来源：http://ivr.svipenyu.cn

[R45] 批量删除
来源：http://ufr.uphjek.com

find . -name "*.tmp" -delete
来源：http://vfz.zdbjq.cn

[R46] 递归替换文件内容
来源：http://uwr.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tzc.xuetiantiany.cn

[R47] sed 单行替换
来源：http://cvh.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ssf.jiagoushi.top

[R48] awk 取指定列
来源：http://hjt.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://xad.tarul.cn

[R49] awk 带条件
来源：http://epc.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zzc.jianghu66.top

[R50] awk 求和
来源：http://aym.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://seb.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://bgl.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://csf.hcnkem.com

[R52] 统计行数
来源：http://mlt.nanxinkj.top

wc -l a.txt
来源：http://piw.yongpay.top

[R53] 查看文件头与实时尾
来源：http://gtg.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://toa.dashuyun.cn

[R54] 比较两个文件
来源：http://val.pycfn.com

diff a.txt b.txt
来源：http://vuc.sweek.top

[R55] 压缩与解压
来源：http://pnv.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://apu.nwbrower.top

[R56] 远程拷贝
来源：http://qys.yanxiufei.cn

scp file user@host:/path/
来源：http://hua.fehbvm.com

[R57] 远程执行命令
来源：http://amt.hywenlv.cn

ssh user@host 'uptime'
来源：http://mjs.yfazqb.com

[R58] 下载文件
来源：http://jlk.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tcc.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://kcn.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbi.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://ljw.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kdl.mhx1999.top

[R61] 磁盘占用
来源：http://rcp.xziqi.cn

df -h;  du -sh *
来源：http://qdf.yangfankeji.com

[R62] 找最占空间的文件
来源：http://ycu.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://qig.iojbl.cn

[R63] 内存与进程
来源：http://lrz.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://iiw.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://vgq.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://hni.sysykeji.top

[R65] 查看端口占用
来源：http://hps.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hui.jianghu66.top

[R66] 定时任务
来源：http://pml.redwolf501.top

crontab -e;  crontab -l
来源：http://zxx.redwolf501.top

[R67] 生成随机十六进制串
来源：http://ngh.nanxuanxn.top

openssl rand -hex 16
来源：http://fxn.yj20258.top

[R68] 计算文件校验值
来源：http://udq.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://xha.ydjk.org.cn

[R69] 生成随机密码
来源：http://kqh.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://jmv.jiagoushi.top

[R70] 时间戳与互转
来源：http://svp.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://lxw.aizwys.cn

[R71] 日期格式化
来源：http://etp.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gor.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://suh.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yvo.zhongyouzk.top

[R73] 分割大日志
来源：http://met.gzhubu.top

split -l 1000 big.log part_
来源：http://ftl.aibaodan.cn

[R74] 批量重命名
来源：http://tlb.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sga.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://axc.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://igx.gzhubu.top

[R76] 使用临时文件
来源：http://zql.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xik.jqgufenzy.top

[R77] 读取用户输入
来源：http://bsn.yj20258888.top

read -rp "请输入: " ans
来源：http://ail.jinqigufen.top

[R78] 交互式菜单
来源：http://vxm.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mgv.hcnkem.com

[R79] 解析命令行选项
来源：http://dwh.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qof.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://cia.yj20258888.top

time ./run.sh
来源：http://yco.haohaochexian.top

================================================================================
来源：http://tku.jinqigfzy.top

S. C / C++ 专题
来源：http://hdu.tarul.cn

================================================================================
来源：http://fls.xinyue.icu

[S01] C：Hello World
来源：http://uvd.yfazqb.com

#include <stdio.h>
来源：http://nya.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mam.cucudq.cn

[S02] C：变量与格式化输出
来源：http://jdg.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://etb.yvedp.cn

[S03] C：读入整数
来源：http://ere.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://stq.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://awq.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://mus.nanxinkj.top

[S05] C：字符串长度
来源：http://ytt.jinqigufen.top

strlen(s)
来源：http://evw.ydzc1.top

[S06] C：字符串比较
来源：http://jdz.yueranfly.top

strcmp(a, b) == 0
来源：http://lwt.gotoacloud.top

[S07] C：数组遍历求和
来源：http://tjr.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yln.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://suw.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wss.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://bcd.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ccf.uphjek.com

[S10] C：指针与解引用
来源：http://vem.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://zlx.daria6918.cn

[S11] C：逐行读文件
来源：http://wfp.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ync.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://vfm.xinyue.icu

fclose(f);
来源：http://ypg.ybcxt.top

[S12] C：写文件
来源：http://wdj.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xwi.sxryk.cn

[S13] C：宏定义
来源：http://mhu.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fcp.ydjk.org.cn

[S14] C：枚举
来源：http://gue.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://pqn.hongshengwenyu.top

[S15] C：类型转换
来源：http://mgc.cdnleiting.top

(double) a / b
来源：http://mux.sweek.top

[S16] C：位操作置位
来源：http://fqy.chenlongwang.top

x |= (1 << 3);
来源：http://pia.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://ugq.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qtu.zycfv.cn

[S18] C：命令行参数
来源：http://pri.andypj.xyz

int main(int argc, char **argv)
来源：http://mak.jqgfzy.top

[S19] C：快速排序
来源：http://fwa.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://czy.gogol.net.cn

[S20] C：二分查找
来源：http://aek.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hht.yuxming.cn

[S21] C：字符类别判断
来源：http://jxa.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jej.hammf.cn

[S22] C：字符串转数字
来源：http://iyi.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rmb.shzxlz.cn

[S23] C：随机数
来源：http://jdc.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eyx.hcnkem.com

[S24] C：获取本地时间
来源：http://wdv.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ayk.c1oappe.top

[S25] C：内存拷贝
来源：http://tsh.cheryme.top

memcpy(dst, src, n);
来源：http://dwf.hysaishi.cn

[S26] C：内存清零
来源：http://elv.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://baq.yuanzhike.top

[S27] C：定义常量
来源：http://evv.nanxuanxn.top

const double PI = 3.14159;
来源：http://qmp.hammf.cn

[S28] C：静态变量
来源：http://gwf.daria6918.cn

static int counter = 0;
来源：http://ryi.sysykeji.top

[S29] C：变参函数
来源：http://dwi.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://byb.smart0.xyz

[S30] C：头文件保护
来源：http://nau.chenzaomai.com

#ifndef X_H
来源：http://ngh.sjlbkw.cn

#define X_H
来源：http://ltd.shuidangran.top

#endif
来源：http://ogz.chenzaomai.com

[S31] C++：Hello World
来源：http://jag.daria6918.cn

#include <iostream>
来源：http://end.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://kkw.sweek.top

[S32] C++：字符串
来源：http://uff.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://csp.vqdsnc.cn

[S33] C++：vector 增删
来源：http://ygj.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://orv.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://xaw.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://jny.gaohongyu789.top

[S35] C++：map
来源：http://oao.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://isl.yongpay.top

[S36] C++：unordered_map
来源：http://bzi.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bej.fktsv.cn

[S37] C++：set
来源：http://kph.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gwm.yvedp.cn

[S38] C++：排序
来源：http://cpz.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://cfk.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://uua.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ubw.ctjpmb.com

[S40] C++：查找元素
来源：http://hgz.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://grj.uphjek.com

[S41] C++：类与构造函数
来源：http://bpz.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zhb.iojbl.cn

[S42] C++：继承与虚函数
来源：http://puy.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://cpx.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://bef.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://rvs.cheryme.top

[S44] C++：引用传参
来源：http://yio.yueranfly.top

void inc(int &x) { ++x; }
来源：http://lpm.zhongyouzk.top

[S45] C++：lambda
来源：http://usm.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pow.yonumen.top

[S46] C++：函数模板
来源：http://lmb.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oiv.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://pbw.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucj.mhx1999.top

[S48] C++：逐行读文件
来源：http://hjk.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://gsa.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://jpy.pengpengdd.cyou

[S49] C++：写文件
来源：http://wuo.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ewu.guannengcc.top

[S50] C++：格式化数字
来源：http://fbp.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yjs.uphjek.com

[S51] C++：显式类型转换
来源：http://gll.quarkkingdee.top

static_cast<double>(a) / b
来源：http://znu.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://dwa.mhx1999.top

int size() const noexcept { return n_; }
来源：http://eje.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://vtb.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://pvn.jianghu66.top

[S54] C++：异常处理
来源：http://wcz.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ztk.cashguo.top

[S55] C++：结构化绑定
来源：http://swj.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://inm.zhijiandao.cn

[S56] C++：optional
来源：http://fel.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yoo.9152youxi.cn

[S57] C++：编译期常量
来源：http://qmy.birdmap.top

constexpr int N = 10;
来源：http://axs.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://hno.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://nfq.yvedp.cn

[S59] C++：静态断言
来源：http://zto.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ieh.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://qie.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhz.jianghu66.top

================================================================================
来源：http://qgo.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dyu.zdqjudy.top

================================================================================
来源：http://rce.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://vdc.zdqjudy.top

println("Hello")
来源：http://bxx.0kj1m.cn

[T02] Kotlin：变量
来源：http://ult.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdm.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://pev.yuxming.cn

"值: $b"
来源：http://xfu.tianlin.xyz

[T04] Kotlin：空安全
来源：http://gab.guowangkeji.top

val n: String? = null;  n?.length
来源：http://hbp.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://rcx.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ezf.yongpay.top

[T06] Kotlin：集合映射
来源：http://faa.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wrm.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://wpo.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://pir.guowangkeji.top

[T08] Kotlin：数据类
来源：http://pgw.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://sja.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://vuq.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://trh.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://lxk.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cxh.daria6918.cn

[T11] Kotlin：协程
来源：http://oew.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tpj.xinyue.icu

[T12] Kotlin：解构声明
来源：http://pqp.sweek.top

val (a, b) = Pair(1, 2)
来源：http://zgq.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://myn.fengsongda.top

val m = mapOf("a" to 1)
来源：http://fgv.yfazqb.com

[T14] Kotlin：循环
来源：http://kbj.ppjwa.cn

for (i in 1..10) println(i)
来源：http://jgt.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://zww.ydzc1.top

interface Shape { fun area(): Double }
来源：http://cpj.redwolf501.top

[T16] Swift：Hello World
来源：http://nux.tianlin.xyz

print("Hello")
来源：http://ess.shanyushiyangkeji.top


<!-- 参考信息 -->