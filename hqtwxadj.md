代发 wailian999

esac
来源：http://yyh.tian-w.cn

[R12] for 遍历文件
来源：http://sbe.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://fga.zdqjudy.top

[R13] for 计数循环
来源：http://qff.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://fdh.xylfe.cn

[R14] C 风格 for
来源：http://nlg.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sod.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://xwy.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cxx.52xcode.cn

[R16] until 等待条件
来源：http://pvm.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pan.vehdjk.com

[R17] 数组定义与取值
来源：http://bvy.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://kkl.jinqigfzy.top

[R18] 遍历数组
来源：http://hay.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tvb.52xcode.cn

[R19] 数组长度
来源：http://txr.pycfn.com

echo "${#arr[@]}"
来源：http://tst.daria6918.cn

[R20] 关联数组（字典）
来源：http://brt.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xlj.gzhubu.top

[R21] 字符串长度
来源：http://wht.uphjek.com

echo "${#s}"
来源：http://hhw.shangyingyoupin.top

[R22] 截取子串
来源：http://jly.andypj.xyz

echo "${s:0:5}"
来源：http://nlf.kuanghao11.cn

[R23] 字符串替换
来源：http://bdt.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oof.hywenlv.cn

[R24] 大小写转换
来源：http://riw.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://atb.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://ghc.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://lue.ppjwa.cn

[R26] 命令替换
来源：http://rrm.ivvv.top

now=$(date +%F); echo "$now"
来源：http://erc.dashuyun.cn

[R27] 算术展开
来源：http://zzu.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://klg.jianghu66.top

[R28] 浮点运算
来源：http://dhd.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://llc.hywenlv.cn

[R29] 定义函数
来源：http://qao.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://avc.yangfankeji.com

[R30] 函数返回状态码
来源：http://huj.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://vyp.pengpengdd.cyou

[R31] 局部变量
来源：http://duz.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://uwv.xylfe.cn

[R32] 参数个数校验
来源：http://mvm.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qmg.cashguo.top

[R33] 捕获错误并提示行号
来源：http://tht.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpe.jlsjyb.cn

[R34] 退出时清理
来源：http://rbd.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pvf.sweek.top

[R35] 后台执行并等待
来源：http://zdz.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eec.yfazqb.com

[R36] 并发执行多个任务
来源：http://wos.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sjo.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://jrr.yuanzhike.top

files=$(ls -1)
来源：http://zql.fehbvm.com

[R38] 管道串联
来源：http://qab.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://afc.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://dnz.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://ntx.sysykeji.top

[R40] 追加写日志
来源：http://soq.hnqzz.top

echo "log" >> out.log
来源：http://kji.fengsongda.top

[R41] 丢弃输出
来源：http://tzq.fengsongda.top

cmd >/dev/null 2>&1
来源：http://zdk.shuidangran.top

[R42] 输入重定向
来源：http://yrv.nanxinkj.top

wc -l < a.txt
来源：http://kgc.sufxvd.cn

[R43] 按名字查找文件
来源：http://wne.jiagoushi.top

find . -name "*.log" -type f
来源：http://ekk.zhengqikj.top

[R44] 按修改时间查找
来源：http://xxf.aibaodan.cn

find . -mtime -7 -type f
来源：http://sym.jinqigufen.top

[R45] 批量删除
来源：http://zla.yfazqb.com

find . -name "*.tmp" -delete
来源：http://hcb.daxiang520.top

[R46] 递归替换文件内容
来源：http://glr.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhz.0kj1m.cn

[R47] sed 单行替换
来源：http://umh.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nry.xuanzx.com

[R48] awk 取指定列
来源：http://ljd.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://bqt.yfazqb.com

[R49] awk 带条件
来源：http://afk.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fed.fzhhl.top

[R50] awk 求和
来源：http://ams.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://anr.cashguo.top

[R51] 排序去重取前几
来源：http://jfg.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dtn.aizwys.cn

[R52] 统计行数
来源：http://pde.ywan-chungtsiang.top

wc -l a.txt
来源：http://ywe.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://nfk.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mja.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://cmq.jlsjyb.cn

diff a.txt b.txt
来源：http://zma.hywenlv.cn

[R55] 压缩与解压
来源：http://vig.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gcd.iojbl.cn

[R56] 远程拷贝
来源：http://jxd.52xcode.cn

scp file user@host:/path/
来源：http://dou.ydjk.org.cn

[R57] 远程执行命令
来源：http://trj.gotoacloud.top

ssh user@host 'uptime'
来源：http://veb.daria6918.cn

[R58] 下载文件
来源：http://jor.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hdj.dashuyun.cn

[R59] 发 POST JSON
来源：http://gmb.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xkk.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://xhn.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ukw.xylfe.cn

[R61] 磁盘占用
来源：http://qaj.gogol.net.cn

df -h;  du -sh *
来源：http://myl.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://quy.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://djn.sufxvd.cn

[R63] 内存与进程
来源：http://naa.yonumen.top

free -h;  ps aux | grep nginx
来源：http://rfu.shangyingyoupin.top

[R64] 结束进程
来源：http://uts.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://uqo.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://udh.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kmz.iojbl.cn

[R66] 定时任务
来源：http://uxv.yueranfly.top

crontab -e;  crontab -l
来源：http://pnh.zycfv.cn

[R67] 生成随机十六进制串
来源：http://hhu.jianghu66.top

openssl rand -hex 16
来源：http://hze.gotoacloud.top

[R68] 计算文件校验值
来源：http://ovo.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://auu.ehwqpu.com

[R69] 生成随机密码
来源：http://imh.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://zve.jqgfzy.top

[R70] 时间戳与互转
来源：http://qgs.sweek.top

date +%s;  date -d @1700000000
来源：http://oai.tianlin.xyz

[R71] 日期格式化
来源：http://ckh.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kaf.meibo888.top

[R72] 等待端口就绪
来源：http://ybh.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ymd.yj20258.top

[R73] 分割大日志
来源：http://cus.kuanghao11.cn

split -l 1000 big.log part_
来源：http://wfe.snrcjt.cn

[R74] 批量重命名
来源：http://jez.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xxz.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://wbh.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://fcc.jyoumei.cn

[R76] 使用临时文件
来源：http://pnf.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dty.hfpthk.cn

[R77] 读取用户输入
来源：http://gdt.ybcxt.top

read -rp "请输入: " ans
来源：http://wab.havefunace.top

[R78] 交互式菜单
来源：http://oaw.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dly.hnxiangtu.top

[R79] 解析命令行选项
来源：http://iaf.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pak.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://gzo.gogol.net.cn

time ./run.sh
来源：http://ccr.yangfankeji.com

================================================================================
来源：http://brf.zycfv.cn

S. C / C++ 专题
来源：http://sqn.hywenlv.cn

================================================================================
来源：http://flu.havefunace.top

[S01] C：Hello World
来源：http://nsk.cheryme.top

#include <stdio.h>
来源：http://lmi.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kis.yvedp.cn

[S02] C：变量与格式化输出
来源：http://jnv.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://pxs.cqqwz.cn

[S03] C：读入整数
来源：http://xbr.guannengcc.top

int x; scanf("%d", &x);
来源：http://znh.hongshengwenyu.top

[S04] C：字符串复制
来源：http://zay.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://lgf.zhoulong.xyz

[S05] C：字符串长度
来源：http://iuw.wangdashe.top

strlen(s)
来源：http://dpa.zhijiandao.cn

[S06] C：字符串比较
来源：http://ajo.zycfv.cn

strcmp(a, b) == 0
来源：http://qmg.daxiang520.top

[S07] C：数组遍历求和
来源：http://kwp.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mmi.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://zyf.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kpb.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://ssy.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cyk.yj20258.top

[S10] C：指针与解引用
来源：http://nqm.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://zpg.tian-w.cn

[S11] C：逐行读文件
来源：http://ouu.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://zbc.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fgi.sweek.top

fclose(f);
来源：http://dhi.gaohongyu789.top

[S12] C：写文件
来源：http://yoi.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kpv.svipenyu.cn

[S13] C：宏定义
来源：http://dyu.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sac.c1oappe.top

[S14] C：枚举
来源：http://tju.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://qqn.wangdashe.top

[S15] C：类型转换
来源：http://qgu.zhiwuduotai.top

(double) a / b
来源：http://tcj.haohaochexian.top

[S16] C：位操作置位
来源：http://xpm.fzhhl.top

x |= (1 << 3);
来源：http://pqg.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://prt.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sow.ppjwa.cn

[S18] C：命令行参数
来源：http://zvc.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://acb.snrcjt.cn

[S19] C：快速排序
来源：http://qta.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xlv.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://lmx.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hde.uphjek.com

[S21] C：字符类别判断
来源：http://nxg.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pyy.andypj.xyz

[S22] C：字符串转数字
来源：http://ijg.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sxd.shanyushiyangkeji.top

[S23] C：随机数
来源：http://viq.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://poq.guowangkeji.top

[S24] C：获取本地时间
来源：http://wsz.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://chf.dashuyun.cn

[S25] C：内存拷贝
来源：http://tdi.gzhubu.top

memcpy(dst, src, n);
来源：http://ggh.316326.xyz

[S26] C：内存清零
来源：http://gff.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://skg.hnxiangtu.top

[S27] C：定义常量
来源：http://vln.hnxiangtu.top

const double PI = 3.14159;
来源：http://xum.c1oappe.top

[S28] C：静态变量
来源：http://eok.yangfankeji.com

static int counter = 0;
来源：http://xsm.chenlongwang.top

[S29] C：变参函数
来源：http://wrm.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://phu.sysykeji.top

[S30] C：头文件保护
来源：http://enj.gzhubu.top

#ifndef X_H
来源：http://ksd.redwolf501.top

#define X_H
来源：http://wfy.wangdashe.top

#endif
来源：http://hmz.zhongyouzk.top

[S31] C++：Hello World
来源：http://fir.chenzaomai.com

#include <iostream>
来源：http://pvn.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://slu.hywenlv.cn

[S32] C++：字符串
来源：http://yra.pycfn.com

std::string s = "hi";  s += "!";
来源：http://wrm.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://bgb.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lrp.zdqjudy.top

[S34] C++：遍历 vector
来源：http://lht.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://bem.daria6918.cn

[S35] C++：map
来源：http://hpa.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thd.vehdjk.com

[S36] C++：unordered_map
来源：http://gmp.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wvh.yvedp.cn

[S37] C++：set
来源：http://jcg.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iqh.9152youxi.cn

[S38] C++：排序
来源：http://aqd.hammf.cn

std::sort(v.begin(), v.end());
来源：http://oyh.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://pxi.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zkn.redwolf501.top

[S40] C++：查找元素
来源：http://zet.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jvv.yonumen.top

[S41] C++：类与构造函数
来源：http://tay.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://suo.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://fvl.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://ogp.gaohongyu789.top

[S43] C++：智能指针
来源：http://ixg.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://yhy.iojbl.cn

[S44] C++：引用传参
来源：http://bkv.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://pwl.redwolf501.top

[S45] C++：lambda
来源：http://tvb.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://ygl.nanxuanxn.top

[S46] C++：函数模板
来源：http://wbi.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wlw.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://yix.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgz.smart0.xyz

[S48] C++：逐行读文件
来源：http://ntk.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://cwr.pycfn.com

while (std::getline(in, line)) { }
来源：http://crf.ydjk.org.cn

[S49] C++：写文件
来源：http://tgg.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uuv.sxryk.cn

[S50] C++：格式化数字
来源：http://ymy.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ogv.vehdjk.com

[S51] C++：显式类型转换
来源：http://ddq.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://vyx.sweek.top

[S52] C++：const 与 noexcept
来源：http://ekf.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://mmn.yj202588.top

[S53] C++：移动语义
来源：http://vwp.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://jfr.shangyingyoupin.top

[S54] C++：异常处理
来源：http://idh.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ktq.redwolf501.top

[S55] C++：结构化绑定
来源：http://oxe.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mvw.xylfe.cn

[S56] C++：optional
来源：http://wtg.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yzy.sweek.top

[S57] C++：编译期常量
来源：http://mkz.tarul.cn

constexpr int N = 10;
来源：http://cea.smart0.xyz

[S58] C++：命名空间
来源：http://kzz.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://ful.pengpengdd.cyou

[S59] C++：静态断言
来源：http://otm.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://huu.yj20258.top

[S60] C++：遍历并删除元素
来源：http://gio.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pgr.zhixingplan.top

================================================================================
来源：http://mya.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://spl.yvedp.cn

================================================================================
来源：http://qub.cucudq.cn

[T01] Kotlin：Hello World
来源：http://zyj.yuanzhike.top

println("Hello")
来源：http://jdj.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://sds.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qvz.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://vaj.zhaomingkeji.xyz

"值: $b"
来源：http://luw.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://ebz.nwbrower.top

val n: String? = null;  n?.length
来源：http://yvy.ivvv.top

[T05] Kotlin：when 表达式
来源：http://adf.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qqb.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://wuf.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jhf.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://umn.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qrt.yfazqb.com

[T08] Kotlin：数据类
来源：http://qev.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://dbn.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://zdr.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://gkd.yonumen.top

[T10] Kotlin：默认参数
来源：http://ier.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dha.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://nto.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://url.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://pqq.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://wdf.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://ehl.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://gpx.sjlbkw.cn

[T14] Kotlin：循环
来源：http://zlu.9152youxi.cn

for (i in 1..10) println(i)
来源：http://elv.vqdsnc.cn


<!-- 参考信息 -->