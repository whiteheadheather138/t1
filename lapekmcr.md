代发 wailian999

esac
来源：http://yhh.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://qam.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://byu.sysykeji.top

[R13] for 计数循环
来源：http://rwd.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://uka.zhiwuduotai.top

[R14] C 风格 for
来源：http://lhk.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uxs.yvedp.cn

[R15] while 逐行读文件
来源：http://fxo.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vdj.hywenlv.cn

[R16] until 等待条件
来源：http://mcz.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lec.cheryme.top

[R17] 数组定义与取值
来源：http://xpp.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://uog.zhongyouzk.top

[R18] 遍历数组
来源：http://oyk.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sll.yj20258888.top

[R19] 数组长度
来源：http://sbp.guowangkeji.top

echo "${#arr[@]}"
来源：http://ydz.ydzc1.top

[R20] 关联数组（字典）
来源：http://tbh.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sjk.316326.xyz

[R21] 字符串长度
来源：http://exf.jqgufenzy.top

echo "${#s}"
来源：http://nde.feifeiyinyue.top

[R22] 截取子串
来源：http://kxa.redwolf501.top

echo "${s:0:5}"
来源：http://woa.yangfankeji.com

[R23] 字符串替换
来源：http://prf.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gxr.tarul.cn

[R24] 大小写转换
来源：http://xqs.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fdl.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://fnv.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lnj.svipenyu.cn

[R26] 命令替换
来源：http://nrr.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://teg.fengsongda.top

[R27] 算术展开
来源：http://nqu.xinyue.icu

echo $((1 + 2 * 3))
来源：http://tpe.daxiang520.top

[R28] 浮点运算
来源：http://pym.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://suj.ivvv.top

[R29] 定义函数
来源：http://sql.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dot.yj20258888.top

[R30] 函数返回状态码
来源：http://dht.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://zud.hywenlv.cn

[R31] 局部变量
来源：http://tck.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://dod.ivvv.top

[R32] 参数个数校验
来源：http://qro.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mdh.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://uoo.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nbf.yvedp.cn

[R34] 退出时清理
来源：http://uxu.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://czi.dianchejie.cn

[R35] 后台执行并等待
来源：http://zaf.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mvw.epnwcf.com

[R36] 并发执行多个任务
来源：http://odb.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lrw.nanxinkj.top

[R37] 把输出赋给变量
来源：http://uvd.aibaodan.cn

files=$(ls -1)
来源：http://jmr.zhiwuduotai.top

[R38] 管道串联
来源：http://myl.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://wmp.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://yhg.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://lkl.hysaishi.cn

[R40] 追加写日志
来源：http://qga.bjfxy.top

echo "log" >> out.log
来源：http://qdi.uphjek.com

[R41] 丢弃输出
来源：http://zxn.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://xxw.hcnkem.com

[R42] 输入重定向
来源：http://ieb.fktsv.cn

wc -l < a.txt
来源：http://iee.haohaochexian.top

[R43] 按名字查找文件
来源：http://cty.dashuyun.cn

find . -name "*.log" -type f
来源：http://qyd.jyoumei.cn

[R44] 按修改时间查找
来源：http://kyy.dashuyun.cn

find . -mtime -7 -type f
来源：http://zej.wangdashe.top

[R45] 批量删除
来源：http://swy.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://rnc.yangfankeji.com

[R46] 递归替换文件内容
来源：http://aie.zhengqikj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gtt.yj202588.top

[R47] sed 单行替换
来源：http://ljv.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vym.jlsjyb.cn

[R48] awk 取指定列
来源：http://yyc.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://vxy.xziqi.cn

[R49] awk 带条件
来源：http://bnz.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xxv.redwolf501.top

[R50] awk 求和
来源：http://bqc.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://obm.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://hlr.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fho.nanxinkj.top

[R52] 统计行数
来源：http://ajj.jinyuanbaomall.cn

wc -l a.txt
来源：http://hyj.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://zbu.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://izl.sxryk.cn

[R54] 比较两个文件
来源：http://qww.tarul.cn

diff a.txt b.txt
来源：http://enr.chenjidiqi.icu

[R55] 压缩与解压
来源：http://imc.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dgz.hnqzz.top

[R56] 远程拷贝
来源：http://tyq.52xcode.cn

scp file user@host:/path/
来源：http://frv.yfazqb.com

[R57] 远程执行命令
来源：http://xbu.jinqigufen.top

ssh user@host 'uptime'
来源：http://gbg.316326.xyz

[R58] 下载文件
来源：http://umu.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hhn.gotoacloud.top

[R59] 发 POST JSON
来源：http://gxw.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvu.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://sqw.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eru.zdqjudy.top

[R61] 磁盘占用
来源：http://eup.chenjidiqi.icu

df -h;  du -sh *
来源：http://icq.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://fuo.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://hvc.fanxiaobao.xyz

[R63] 内存与进程
来源：http://dan.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://nkm.cucudq.cn

[R64] 结束进程
来源：http://aky.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://mcf.wangshuangyany.cn

[R65] 查看端口占用
来源：http://lmf.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fan.yuxming.cn

[R66] 定时任务
来源：http://cgw.havefunace.top

crontab -e;  crontab -l
来源：http://hog.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://zkb.yuxming.cn

openssl rand -hex 16
来源：http://xjn.yj20258.top

[R68] 计算文件校验值
来源：http://kcn.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://shz.sufxvd.cn

[R69] 生成随机密码
来源：http://guj.ybcxt.top

head -c 16 /dev/urandom | base64
来源：http://bta.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://jcy.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://joc.aibaodan.cn

[R71] 日期格式化
来源：http://dvh.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wno.tianlin.xyz

[R72] 等待端口就绪
来源：http://dne.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://oce.zhiwuduotai.top

[R73] 分割大日志
来源：http://vlk.zhijiandao.cn

split -l 1000 big.log part_
来源：http://oxd.havefunace.top

[R74] 批量重命名
来源：http://aby.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xeo.zhixingplan.top

[R75] 导出环境变量
来源：http://gor.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://syb.52xcode.cn

[R76] 使用临时文件
来源：http://crz.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jya.hfpthk.cn

[R77] 读取用户输入
来源：http://vvr.gogol.net.cn

read -rp "请输入: " ans
来源：http://rdk.ppjwa.cn

[R78] 交互式菜单
来源：http://tsz.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wdr.hfpthk.cn

[R79] 解析命令行选项
来源：http://xuv.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gib.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://cqm.0kj1m.cn

time ./run.sh
来源：http://lnw.guannengcc.top

================================================================================
来源：http://qpd.cheryme.top

S. C / C++ 专题
来源：http://axk.zhoulong.xyz

================================================================================
来源：http://spr.zhijiandao.cn

[S01] C：Hello World
来源：http://uer.ehwqpu.com

#include <stdio.h>
来源：http://uzo.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ygo.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://kul.sweek.top

int a = 10; printf("%d\n", a);
来源：http://kon.hnqzz.top

[S03] C：读入整数
来源：http://pou.iojbl.cn

int x; scanf("%d", &x);
来源：http://xdq.jyoumei.cn

[S04] C：字符串复制
来源：http://qim.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://jkn.jqgfzy.top

[S05] C：字符串长度
来源：http://gip.sjlbkw.cn

strlen(s)
来源：http://hcx.epnwcf.com

[S06] C：字符串比较
来源：http://olo.andypj.xyz

strcmp(a, b) == 0
来源：http://yoa.iojbl.cn

[S07] C：数组遍历求和
来源：http://qpr.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nmg.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://uwr.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://byg.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://gmi.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nvr.uphjek.com

[S10] C：指针与解引用
来源：http://wje.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://cpv.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://eiu.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://ler.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://asn.c1oappe.top

fclose(f);
来源：http://nme.tian-w.cn

[S12] C：写文件
来源：http://nyi.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tvm.jqgfzy.top

[S13] C：宏定义
来源：http://ojf.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gpv.feifeiyinyue.top

[S14] C：枚举
来源：http://lnn.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://kyk.gaohongyu789.top

[S15] C：类型转换
来源：http://jky.zhixingplan.top

(double) a / b
来源：http://jqi.pycfn.com

[S16] C：位操作置位
来源：http://tmc.havefunace.top

x |= (1 << 3);
来源：http://xdl.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://iyo.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iej.yj202588.top

[S18] C：命令行参数
来源：http://auj.cqqwz.cn

int main(int argc, char **argv)
来源：http://bmo.pengpengdd.cyou

[S19] C：快速排序
来源：http://imm.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://vyn.0kj1m.cn

[S20] C：二分查找
来源：http://jex.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://osi.tian-w.cn

[S21] C：字符类别判断
来源：http://vqo.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://amz.redwolf501.top

[S22] C：字符串转数字
来源：http://kzm.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zjg.birdmap.top

[S23] C：随机数
来源：http://mjw.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ikt.chenzaomai.com

[S24] C：获取本地时间
来源：http://yye.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ztg.cheryme.top

[S25] C：内存拷贝
来源：http://lsb.cashguo.top

memcpy(dst, src, n);
来源：http://bgk.cashguo.top

[S26] C：内存清零
来源：http://woz.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://oye.aibaodan.cn

[S27] C：定义常量
来源：http://nfm.yvedp.cn

const double PI = 3.14159;
来源：http://nsh.aizwys.cn

[S28] C：静态变量
来源：http://zlu.tarul.cn

static int counter = 0;
来源：http://cbp.shangyingyoupin.top

[S29] C：变参函数
来源：http://iue.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ezk.epnwcf.com

[S30] C：头文件保护
来源：http://iwd.xziqi.cn

#ifndef X_H
来源：http://dym.c1oappe.top

#define X_H
来源：http://gkm.birdmap.top

#endif
来源：http://lpo.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://rzi.xingfuxueyuan.xyz

#include <iostream>
来源：http://gcj.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://azk.feifeiyinyue.top

[S32] C++：字符串
来源：http://cgx.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://pnz.zhongyouzk.top

[S33] C++：vector 增删
来源：http://rtq.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yqc.dashuyun.cn

[S34] C++：遍历 vector
来源：http://xvg.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://pfq.shuidangran.top

[S35] C++：map
来源：http://ukn.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bdh.hnqzz.top

[S36] C++：unordered_map
来源：http://hrc.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lim.cqqwz.cn

[S37] C++：set
来源：http://duh.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vkc.wangshuangyany.cn

[S38] C++：排序
来源：http://srz.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://tlz.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://mzn.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nld.cashguo.top

[S40] C++：查找元素
来源：http://nby.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wrd.daria6918.cn

[S41] C++：类与构造函数
来源：http://gkz.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oni.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://lnw.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://wzn.chenjidiqi.icu

[S43] C++：智能指针
来源：http://lio.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://hja.svipenyu.cn

[S44] C++：引用传参
来源：http://zmt.xylfe.cn

void inc(int &x) { ++x; }
来源：http://ekm.zdqjudy.top

[S45] C++：lambda
来源：http://rzs.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tdi.hywenlv.cn

[S46] C++：函数模板
来源：http://yhd.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tin.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://xkq.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqr.pycfn.com

[S48] C++：逐行读文件
来源：http://iic.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://brq.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://lre.vehdjk.com

[S49] C++：写文件
来源：http://kdw.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://exu.bjfxy.top

[S50] C++：格式化数字
来源：http://arp.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://urk.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://ajo.yanxiufei.cn

static_cast<double>(a) / b
来源：http://baz.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://gno.sysykeji.top

int size() const noexcept { return n_; }
来源：http://mif.hysaishi.cn

[S53] C++：移动语义
来源：http://rwv.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://umv.epnwcf.com

[S54] C++：异常处理
来源：http://wab.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://srn.vehdjk.com

[S55] C++：结构化绑定
来源：http://ucu.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://btw.redwolf501.top

[S56] C++：optional
来源：http://pam.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gqe.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://xdx.fengsongda.top

constexpr int N = 10;
来源：http://zlf.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://wcj.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://psp.52xcode.cn

[S59] C++：静态断言
来源：http://pda.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gkz.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://nve.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tke.yj20258888.top

================================================================================
来源：http://uqk.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cgn.ydjk.org.cn

================================================================================
来源：http://ywq.xinyue.icu

[T01] Kotlin：Hello World
来源：http://vyz.bjfxy.top

println("Hello")
来源：http://otx.dashuyun.cn

[T02] Kotlin：变量
来源：http://yxl.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://epr.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://eko.zhixingplan.top

"值: $b"
来源：http://bdt.sysykeji.top

[T04] Kotlin：空安全
来源：http://kgp.hywenlv.cn

val n: String? = null;  n?.length
来源：http://nft.tanke756.top

[T05] Kotlin：when 表达式
来源：http://wdu.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gkb.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://jbi.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://awv.tanke756.top

[T07] Kotlin：集合过滤
来源：http://uve.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://smm.zhixingplan.top

[T08] Kotlin：数据类
来源：http://pae.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://ryr.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://ojq.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://uug.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://ngi.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xmn.ybcxt.top

[T11] Kotlin：协程
来源：http://xam.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oum.aizwys.cn

[T12] Kotlin：解构声明
来源：http://qij.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://pdl.316326.xyz

[T13] Kotlin：只读 Map
来源：http://jre.tanke756.top

val m = mapOf("a" to 1)
来源：http://kul.fzhhl.top

[T14] Kotlin：循环
来源：http://kby.guannengcc.top

for (i in 1..10) println(i)
来源：http://sqc.hfpthk.cn


<!-- 参考信息 -->