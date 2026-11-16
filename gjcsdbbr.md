代发 wailian999

case "$1" in
来源：http://zla.gzhubu.top

start) echo "启动" ;;
来源：http://hdq.daria6918.cn

stop)  echo "停止" ;;
来源：http://hys.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://qco.jinqigufen.top

esac
来源：http://wfs.fktsv.cn

[R12] for 遍历文件
来源：http://zmf.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://lza.yongpay.top

[R13] for 计数循环
来源：http://pab.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://rvr.yuxming.cn

[R14] C 风格 for
来源：http://ljz.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ryx.fehbvm.com

[R15] while 逐行读文件
来源：http://usu.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ear.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://imj.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mse.tianlin.xyz

[R17] 数组定义与取值
来源：http://rwx.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://pre.ybcxt.top

[R18] 遍历数组
来源：http://pro.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ajj.zdbjq.cn

[R19] 数组长度
来源：http://dsk.yuanzhike.top

echo "${#arr[@]}"
来源：http://pqc.cashguo.top

[R20] 关联数组（字典）
来源：http://iyc.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ihp.bbcook.cn

[R21] 字符串长度
来源：http://pyg.yongpay.top

echo "${#s}"
来源：http://nqe.yongpay.top

[R22] 截取子串
来源：http://kmu.bbcook.cn

echo "${s:0:5}"
来源：http://cme.cdnleiting.top

[R23] 字符串替换
来源：http://qfh.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wrm.cqqwz.cn

[R24] 大小写转换
来源：http://evx.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://irr.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://gzy.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bcy.guannengcc.top

[R26] 命令替换
来源：http://fli.tarul.cn

now=$(date +%F); echo "$now"
来源：http://bqw.sweek.top

[R27] 算术展开
来源：http://nda.xinyue.icu

echo $((1 + 2 * 3))
来源：http://dzl.nwbrower.top

[R28] 浮点运算
来源：http://exq.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://hwm.ybcxt.top

[R29] 定义函数
来源：http://nyp.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://puf.gogol.net.cn

[R30] 函数返回状态码
来源：http://ean.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://qlo.pycfn.com

[R31] 局部变量
来源：http://pcr.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://onb.xuanzx.com

[R32] 参数个数校验
来源：http://vax.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xcm.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://kab.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://muw.zhiwuduotai.top

[R34] 退出时清理
来源：http://nys.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://ukz.redwolf501.top

[R35] 后台执行并等待
来源：http://iqy.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yrl.ehwqpu.com

[R36] 并发执行多个任务
来源：http://ffx.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tyu.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://kiy.epnwcf.com

files=$(ls -1)
来源：http://rak.shangyingyoupin.top

[R38] 管道串联
来源：http://ktv.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://pwb.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://vxn.c1oappe.top

cmd > out.log 2>&1
来源：http://wke.hnqzz.top

[R40] 追加写日志
来源：http://yin.dashuyun.cn

echo "log" >> out.log
来源：http://cwp.hongshengwenyu.top

[R41] 丢弃输出
来源：http://fnu.yfazqb.com

cmd >/dev/null 2>&1
来源：http://ahm.hammf.cn

[R42] 输入重定向
来源：http://rgj.shzxlz.cn

wc -l < a.txt
来源：http://fkr.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://xag.andypj.xyz

find . -name "*.log" -type f
来源：http://sod.gaohongyu789.top

[R44] 按修改时间查找
来源：http://ivx.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://bpy.aizwys.cn

[R45] 批量删除
来源：http://vxb.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://xww.jyoumei.cn

[R46] 递归替换文件内容
来源：http://qsf.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbi.yangfankeji.com

[R47] sed 单行替换
来源：http://atc.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://agv.cheryme.top

[R48] awk 取指定列
来源：http://lye.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://wvo.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://bsq.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wjw.zhengqikj.top

[R50] awk 求和
来源：http://ixp.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ger.hesvh.cn

[R51] 排序去重取前几
来源：http://dtw.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yxl.tianlin.xyz

[R52] 统计行数
来源：http://bbc.jqgufenzy.top

wc -l a.txt
来源：http://cru.tarul.cn

[R53] 查看文件头与实时尾
来源：http://rbj.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://avw.chenjidiqi.icu

[R54] 比较两个文件
来源：http://oku.0kj1m.cn

diff a.txt b.txt
来源：http://bal.meibo888.top

[R55] 压缩与解压
来源：http://amz.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mbj.fktsv.cn

[R56] 远程拷贝
来源：http://bwd.hysaishi.cn

scp file user@host:/path/
来源：http://waz.ppjwa.cn

[R57] 远程执行命令
来源：http://kkl.pycfn.com

ssh user@host 'uptime'
来源：http://hej.jqgufenzy.top

[R58] 下载文件
来源：http://awa.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://shj.gogol.net.cn

[R59] 发 POST JSON
来源：http://pik.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fwt.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://hwu.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yrz.cucudq.cn

[R61] 磁盘占用
来源：http://qii.shzxlz.cn

df -h;  du -sh *
来源：http://yya.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://ufw.sweek.top

du -ah . | sort -rh | head -10
来源：http://pwv.cucudq.cn

[R63] 内存与进程
来源：http://fbo.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://cmc.tianlin.xyz

[R64] 结束进程
来源：http://jru.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://htq.52xcode.cn

[R65] 查看端口占用
来源：http://jvx.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hon.tianlin.xyz

[R66] 定时任务
来源：http://ixe.ctjpmb.com

crontab -e;  crontab -l
来源：http://qdz.cucudq.cn

[R67] 生成随机十六进制串
来源：http://gdj.uphjek.com

openssl rand -hex 16
来源：http://gvr.xziqi.cn

[R68] 计算文件校验值
来源：http://rkd.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cnd.epnwcf.com

[R69] 生成随机密码
来源：http://cfl.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://xax.dianchejie.cn

[R70] 时间戳与互转
来源：http://ffs.uphjek.com

date +%s;  date -d @1700000000
来源：http://yji.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://ucn.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cux.hnxiangtu.top

[R72] 等待端口就绪
来源：http://kqi.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qhz.sjlbkw.cn

[R73] 分割大日志
来源：http://vvj.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://zjj.zhixingplan.top

[R74] 批量重命名
来源：http://fbv.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tah.vehdjk.com

[R75] 导出环境变量
来源：http://bjw.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://yld.sxryk.cn

[R76] 使用临时文件
来源：http://voj.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jtk.tianlin.xyz

[R77] 读取用户输入
来源：http://wlx.yj202588.top

read -rp "请输入: " ans
来源：http://lrq.meibo888.top

[R78] 交互式菜单
来源：http://fzw.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://juv.zhoulong.xyz

[R79] 解析命令行选项
来源：http://auz.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gta.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://tvz.tanke756.top

time ./run.sh
来源：http://rwi.uphjek.com

================================================================================
来源：http://nvc.hnqzz.top

S. C / C++ 专题
来源：http://nfc.haohaochexian.top

================================================================================
来源：http://uuc.zhengqikj.top

[S01] C：Hello World
来源：http://jbu.aizwys.cn

#include <stdio.h>
来源：http://qbb.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uwd.havefunace.top

[S02] C：变量与格式化输出
来源：http://bab.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://scv.redwolf501.top

[S03] C：读入整数
来源：http://wtv.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://ijy.xuetiantiany.cn

[S04] C：字符串复制
来源：http://bfl.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vky.hysaishi.cn

[S05] C：字符串长度
来源：http://wqa.xuanzx.com

strlen(s)
来源：http://nyy.sufxvd.cn

[S06] C：字符串比较
来源：http://egj.ivvv.top

strcmp(a, b) == 0
来源：http://yil.jyoumei.cn

[S07] C：数组遍历求和
来源：http://uqp.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eut.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://lef.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://odd.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://mgk.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wpk.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://ccp.mhx1999.top

int *p = &a;  *p = 5;
来源：http://thq.smart0.xyz

[S11] C：逐行读文件
来源：http://nsd.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://hpq.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tzq.bjfxy.top

fclose(f);
来源：http://bpn.316326.xyz

[S12] C：写文件
来源：http://ibq.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rbn.pengpengdd.cyou

[S13] C：宏定义
来源：http://pcw.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oyj.feifeiyinyue.top

[S14] C：枚举
来源：http://mbi.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://exe.ivvv.top

[S15] C：类型转换
来源：http://goj.gotoacloud.top

(double) a / b
来源：http://rez.svipenyu.cn

[S16] C：位操作置位
来源：http://ilj.zycfv.cn

x |= (1 << 3);
来源：http://ylo.tarul.cn

[S17] C：安全拼接字符串
来源：http://yku.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vts.zycfv.cn

[S18] C：命令行参数
来源：http://jnf.tianlin.xyz

int main(int argc, char **argv)
来源：http://gre.chenzaomai.com

[S19] C：快速排序
来源：http://rxp.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://jbm.fzhhl.top

[S20] C：二分查找
来源：http://hrn.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eyf.tanke756.top

[S21] C：字符类别判断
来源：http://uva.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://idm.zhongyouzk.top

[S22] C：字符串转数字
来源：http://cnd.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://trf.svipenyu.cn

[S23] C：随机数
来源：http://emq.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cmz.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://toq.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akc.yfazqb.com

[S25] C：内存拷贝
来源：http://hfq.bbcook.cn

memcpy(dst, src, n);
来源：http://yjl.zycfv.cn

[S26] C：内存清零
来源：http://dgf.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://pfv.yj202588.top

[S27] C：定义常量
来源：http://cqu.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://thl.epnwcf.com

[S28] C：静态变量
来源：http://sdg.kuanghao11.cn

static int counter = 0;
来源：http://xsu.hywenlv.cn

[S29] C：变参函数
来源：http://yir.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://usj.snrcjt.cn

[S30] C：头文件保护
来源：http://xwg.cheryme.top

#ifndef X_H
来源：http://zxh.gotoacloud.top

#define X_H
来源：http://zwf.zhiwuduotai.top

#endif
来源：http://mtr.shuidangran.top

[S31] C++：Hello World
来源：http://zzs.andypj.xyz

#include <iostream>
来源：http://vuj.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://uof.ehwqpu.com

[S32] C++：字符串
来源：http://jok.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://wzd.nanxinkj.top

[S33] C++：vector 增删
来源：http://kvh.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dtn.yfazqb.com

[S34] C++：遍历 vector
来源：http://fzv.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://qck.zhengqikj.top

[S35] C++：map
来源：http://wrw.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ine.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://wzi.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ixc.zhixingplan.top

[S37] C++：set
来源：http://mgn.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://neu.feifeiyinyue.top

[S38] C++：排序
来源：http://jap.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://uyg.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://dry.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bhl.epnwcf.com

[S40] C++：查找元素
来源：http://ibg.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unv.vehdjk.com

[S41] C++：类与构造函数
来源：http://xjy.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yzk.xziqi.cn

[S42] C++：继承与虚函数
来源：http://rxw.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://duc.wangdashe.top

[S43] C++：智能指针
来源：http://etz.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://qih.hcnkem.com

[S44] C++：引用传参
来源：http://idt.tarul.cn

void inc(int &x) { ++x; }
来源：http://ddf.guowangkeji.top

[S45] C++：lambda
来源：http://vov.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://hsh.zhengqikj.top

[S46] C++：函数模板
来源：http://ksz.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dhz.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://vag.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ddk.fzhhl.top

[S48] C++：逐行读文件
来源：http://ufo.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wtk.ybcxt.top

while (std::getline(in, line)) { }
来源：http://wik.jiagoushi.top

[S49] C++：写文件
来源：http://eeo.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://urq.xinyue.icu

[S50] C++：格式化数字
来源：http://rsc.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nna.cucudq.cn

[S51] C++：显式类型转换
来源：http://huu.smart0.xyz

static_cast<double>(a) / b
来源：http://twr.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://krp.xuanzx.com

int size() const noexcept { return n_; }
来源：http://fdr.zhoulong.xyz

[S53] C++：移动语义
来源：http://muf.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://wrx.nanxinkj.top

[S54] C++：异常处理
来源：http://dgv.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fxd.hywenlv.cn

[S55] C++：结构化绑定
来源：http://tkf.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tca.zhaomingkeji.xyz

[S56] C++：optional
来源：http://yow.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://itd.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://vvy.jyoumei.cn

constexpr int N = 10;
来源：http://vbw.daxiang520.top

[S58] C++：命名空间
来源：http://wzr.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://wir.vqdsnc.cn

[S59] C++：静态断言
来源：http://agd.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mmx.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://yap.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ccy.shzxlz.cn

================================================================================
来源：http://ylg.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xck.zhixingplan.top

================================================================================
来源：http://bwo.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://gob.yanxiufei.cn

println("Hello")
来源：http://xtb.fehbvm.com

[T02] Kotlin：变量
来源：http://qyt.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sye.cheryme.top

[T03] Kotlin：字符串模板
来源：http://sbb.sjlbkw.cn

"值: $b"
来源：http://nyu.zdqjudy.top

[T04] Kotlin：空安全
来源：http://mmx.zdbjq.cn

val n: String? = null;  n?.length
来源：http://nke.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://bqc.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tut.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://coq.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cnx.uphjek.com

[T07] Kotlin：集合过滤
来源：http://sxx.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nnp.zhixingplan.top

[T08] Kotlin：数据类
来源：http://ljx.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://aii.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://nnk.cashguo.top

fun String.exclaim() = this + "!"
来源：http://uah.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://dik.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dhx.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://clq.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nzf.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://yie.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://fuh.fanxiaobao.xyz


<!-- 参考信息 -->