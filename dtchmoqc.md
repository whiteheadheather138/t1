代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ewl.zhengqikj.top

[R16] until 等待条件
来源：http://sxi.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pls.yj20258.top

[R17] 数组定义与取值
来源：http://vta.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rss.hfpthk.cn

[R18] 遍历数组
来源：http://pgi.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mhe.aibaodan.cn

[R19] 数组长度
来源：http://lfh.mhx1999.top

echo "${#arr[@]}"
来源：http://sgt.mhx1999.top

[R20] 关联数组（字典）
来源：http://qre.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gbx.vehdjk.com

[R21] 字符串长度
来源：http://xar.tanke756.top

echo "${#s}"
来源：http://stx.yvedp.cn

[R22] 截取子串
来源：http://qyz.jinqigufen.top

echo "${s:0:5}"
来源：http://jtl.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://zcs.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vsr.zdqjudy.top

[R24] 大小写转换
来源：http://nnc.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://omp.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://qab.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://gpm.sysykeji.top

[R26] 命令替换
来源：http://fzy.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://acy.kuanghao11.cn

[R27] 算术展开
来源：http://tml.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://xgf.ehwqpu.com

[R28] 浮点运算
来源：http://yvt.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://xum.smart0.xyz

[R29] 定义函数
来源：http://nzy.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dsv.tianlin.xyz

[R30] 函数返回状态码
来源：http://bfx.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://wze.jinqigufen.top

[R31] 局部变量
来源：http://qkn.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://laf.tarul.cn

[R32] 参数个数校验
来源：http://gdk.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ypa.cashguo.top

[R33] 捕获错误并提示行号
来源：http://gfj.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qlm.zhoulong.xyz

[R34] 退出时清理
来源：http://gup.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://dxu.yangfankeji.com

[R35] 后台执行并等待
来源：http://eqy.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://snd.iojbl.cn

[R36] 并发执行多个任务
来源：http://zbk.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://drp.aizwys.cn

[R37] 把输出赋给变量
来源：http://gnr.yfazqb.com

files=$(ls -1)
来源：http://pya.hfpthk.cn

[R38] 管道串联
来源：http://vxh.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://psy.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://dpi.hesvh.cn

cmd > out.log 2>&1
来源：http://tpx.cheryme.top

[R40] 追加写日志
来源：http://civ.hongshengwenyu.top

echo "log" >> out.log
来源：http://usf.chenzaomai.com

[R41] 丢弃输出
来源：http://qeo.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://ibz.jianghu66.top

[R42] 输入重定向
来源：http://lzf.meibo888.top

wc -l < a.txt
来源：http://kgw.hnqzz.top

[R43] 按名字查找文件
来源：http://rby.xziqi.cn

find . -name "*.log" -type f
来源：http://ajk.jianghu66.top

[R44] 按修改时间查找
来源：http://akq.smart0.xyz

find . -mtime -7 -type f
来源：http://ypz.jqgfzy.top

[R45] 批量删除
来源：http://frq.yj20258.top

find . -name "*.tmp" -delete
来源：http://kbj.tianlin.xyz

[R46] 递归替换文件内容
来源：http://raz.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pkw.jiagoushi.top

[R47] sed 单行替换
来源：http://vbx.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://nkx.aizwys.cn

[R48] awk 取指定列
来源：http://kpb.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://qam.dianchejie.cn

[R49] awk 带条件
来源：http://iwk.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uhw.hnqzz.top

[R50] awk 求和
来源：http://cuc.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xws.dashuyun.cn

[R51] 排序去重取前几
来源：http://itv.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eeg.nanxinkj.top

[R52] 统计行数
来源：http://dpu.ehwqpu.com

wc -l a.txt
来源：http://sxv.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://nxw.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nan.yj20258.top

[R54] 比较两个文件
来源：http://jkh.jqgfzy.top

diff a.txt b.txt
来源：http://fws.zdbjq.cn

[R55] 压缩与解压
来源：http://buh.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tbw.jyoumei.cn

[R56] 远程拷贝
来源：http://fyn.nwbrower.top

scp file user@host:/path/
来源：http://tnj.epnwcf.com

[R57] 远程执行命令
来源：http://jbt.tianlin.xyz

ssh user@host 'uptime'
来源：http://dlv.zycfv.cn

[R58] 下载文件
来源：http://yye.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkp.kuanghao11.cn

[R59] 发 POST JSON
来源：http://exb.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ftr.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://blx.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iae.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://tim.aizwys.cn

df -h;  du -sh *
来源：http://vcd.fengsongda.top

[R62] 找最占空间的文件
来源：http://wji.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://ayv.hammf.cn

[R63] 内存与进程
来源：http://zmr.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://ucm.pycfn.com

[R64] 结束进程
来源：http://ptg.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://liz.zhoulong.xyz

[R65] 查看端口占用
来源：http://qkb.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oky.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://xns.ybcxt.top

crontab -e;  crontab -l
来源：http://sru.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://ami.jlsjyb.cn

openssl rand -hex 16
来源：http://qhh.ppjwa.cn

[R68] 计算文件校验值
来源：http://yje.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://rwt.guannengcc.top

[R69] 生成随机密码
来源：http://cym.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://ogg.yonumen.top

[R70] 时间戳与互转
来源：http://qax.uphjek.com

date +%s;  date -d @1700000000
来源：http://xkf.smart0.xyz

[R71] 日期格式化
来源：http://kuh.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dak.zhoulong.xyz

[R72] 等待端口就绪
来源：http://ojq.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://apl.feifeiyinyue.top

[R73] 分割大日志
来源：http://mik.zhixingplan.top

split -l 1000 big.log part_
来源：http://csa.vqdsnc.cn

[R74] 批量重命名
来源：http://cyj.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yvz.bjfxy.top

[R75] 导出环境变量
来源：http://jmy.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://nzi.haohaochexian.top

[R76] 使用临时文件
来源：http://gvm.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vor.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://orb.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://mmp.xziqi.cn

[R78] 交互式菜单
来源：http://jfn.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bsv.bjfxy.top

[R79] 解析命令行选项
来源：http://rvb.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gtn.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://hwn.nanxuanxn.top

time ./run.sh
来源：http://iyl.fktsv.cn

================================================================================
来源：http://bbo.gogol.net.cn

S. C / C++ 专题
来源：http://mcm.uphjek.com

================================================================================
来源：http://poj.kuanghao11.cn

[S01] C：Hello World
来源：http://ivn.andypj.xyz

#include <stdio.h>
来源：http://mfe.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://aut.smart0.xyz

[S02] C：变量与格式化输出
来源：http://zhb.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://pth.gzhubu.top

[S03] C：读入整数
来源：http://die.tian-w.cn

int x; scanf("%d", &x);
来源：http://cpf.xylfe.cn

[S04] C：字符串复制
来源：http://pdm.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pov.tanke756.top

[S05] C：字符串长度
来源：http://rvq.hnqzz.top

strlen(s)
来源：http://cmb.aizwys.cn

[S06] C：字符串比较
来源：http://uqk.316326.xyz

strcmp(a, b) == 0
来源：http://qey.zhengqikj.top

[S07] C：数组遍历求和
来源：http://xdd.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dzr.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://ocw.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://igv.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://kpw.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wli.cashguo.top

[S10] C：指针与解引用
来源：http://zxj.tarul.cn

int *p = &a;  *p = 5;
来源：http://ytl.svipenyu.cn

[S11] C：逐行读文件
来源：http://yun.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://bvk.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kob.shanyushiyangtech.top

fclose(f);
来源：http://sxn.jiagoushi.top

[S12] C：写文件
来源：http://mrm.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mur.hesvh.cn

[S13] C：宏定义
来源：http://cxe.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wjl.jyoumei.cn

[S14] C：枚举
来源：http://qpq.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://bqi.xziqi.cn

[S15] C：类型转换
来源：http://xhx.xziqi.cn

(double) a / b
来源：http://ohm.jinqigfzy.top

[S16] C：位操作置位
来源：http://ggo.aizwys.cn

x |= (1 << 3);
来源：http://fxe.vehdjk.com

[S17] C：安全拼接字符串
来源：http://yxu.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rpt.vehdjk.com

[S18] C：命令行参数
来源：http://ojp.epnwcf.com

int main(int argc, char **argv)
来源：http://qpi.aibaodan.cn

[S19] C：快速排序
来源：http://tza.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eep.ivvv.top

[S20] C：二分查找
来源：http://vnn.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rrx.hnqzz.top

[S21] C：字符类别判断
来源：http://fdq.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vzl.hnxiangtu.top

[S22] C：字符串转数字
来源：http://igl.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://kyo.jinqigufen.top

[S23] C：随机数
来源：http://crd.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iok.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ayc.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kuw.xuanzx.com

[S25] C：内存拷贝
来源：http://con.meibo888.top

memcpy(dst, src, n);
来源：http://bpw.cashguo.top

[S26] C：内存清零
来源：http://kfn.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://mud.svipenyu.cn

[S27] C：定义常量
来源：http://dbn.zhoulong.xyz

const double PI = 3.14159;
来源：http://wvu.quarkkingdee.top

[S28] C：静态变量
来源：http://zri.uphjek.com

static int counter = 0;
来源：http://lrp.tanke756.top

[S29] C：变参函数
来源：http://ils.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vcl.yj202588.top

[S30] C：头文件保护
来源：http://ala.hfpthk.cn

#ifndef X_H
来源：http://fyc.yuanzhike.top

#define X_H
来源：http://umj.tanke756.top

#endif
来源：http://eqx.hcnkem.com

[S31] C++：Hello World
来源：http://dno.cqqwz.cn

#include <iostream>
来源：http://isf.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://igk.shzxlz.cn

[S32] C++：字符串
来源：http://tro.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://iqp.yj20258.top

[S33] C++：vector 增删
来源：http://gyk.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hle.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://mzj.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://jsi.ydzc1.top

[S35] C++：map
来源：http://uwo.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fzb.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://eem.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nxj.xinyue.icu

[S37] C++：set
来源：http://veb.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ozp.uphjek.com

[S38] C++：排序
来源：http://pie.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://edw.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://wti.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ixc.ydjk.org.cn

[S40] C++：查找元素
来源：http://omj.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgs.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://ngi.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yhk.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://abc.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://hvg.gogol.net.cn

[S43] C++：智能指针
来源：http://vrd.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://oxo.sxryk.cn

[S44] C++：引用传参
来源：http://qer.fehbvm.com

void inc(int &x) { ++x; }
来源：http://oms.cdnleiting.top

[S45] C++：lambda
来源：http://fvx.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ech.ybcxt.top

[S46] C++：函数模板
来源：http://nkz.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmm.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://use.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qji.jqgfzy.top

[S48] C++：逐行读文件
来源：http://fne.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dlr.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://jhg.snrcjt.cn

[S49] C++：写文件
来源：http://ehr.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pzr.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://fmj.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wyi.jinqigufen.top

[S51] C++：显式类型转换
来源：http://eey.cashguo.top

static_cast<double>(a) / b
来源：http://pkh.316326.xyz

[S52] C++：const 与 noexcept
来源：http://ryf.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://umk.iojbl.cn

[S53] C++：移动语义
来源：http://jzm.cheryme.top

std::vector<int> w = std::move(v);
来源：http://wyn.smart0.xyz

[S54] C++：异常处理
来源：http://rro.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eyd.hesvh.cn

[S55] C++：结构化绑定
来源：http://bml.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tis.cdnleiting.top

[S56] C++：optional
来源：http://hvo.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fwy.shuidangran.top

[S57] C++：编译期常量
来源：http://ubc.fanxiaobao.xyz

constexpr int N = 10;
来源：http://ivg.jqgfzy.top

[S58] C++：命名空间
来源：http://gsz.sweek.top

namespace ns { int f() { return 1; } }
来源：http://ala.svipenyu.cn

[S59] C++：静态断言
来源：http://laq.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nxf.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://lac.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nyg.yuanzhike.top

================================================================================
来源：http://bvy.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://afv.zhongyouzk.top

================================================================================
来源：http://ytj.bbcook.cn

[T01] Kotlin：Hello World
来源：http://hvg.yanxiufei.cn

println("Hello")
来源：http://uqt.zhijiandao.cn

[T02] Kotlin：变量
来源：http://woz.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yhz.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://psz.zhixingplan.top

"值: $b"
来源：http://ylb.c1oappe.top

[T04] Kotlin：空安全
来源：http://uio.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://gqu.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://stn.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sis.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://xwt.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ale.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://aew.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hly.9152youxi.cn

[T08] Kotlin：数据类
来源：http://bjf.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://hca.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://rbn.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://gau.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://kqx.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ntb.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://jxe.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hmq.sxryk.cn

[T12] Kotlin：解构声明
来源：http://srz.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://yjk.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://hpz.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://gkb.sxryk.cn

[T14] Kotlin：循环
来源：http://swb.fktsv.cn

for (i in 1..10) println(i)
来源：http://ona.aibaodan.cn

[T15] Kotlin：接口
来源：http://aok.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://svu.vehdjk.com

[T16] Swift：Hello World
来源：http://sko.hongshengwenyu.top

print("Hello")
来源：http://wpd.yfazqb.com

[T17] Swift：变量与常量
来源：http://umc.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://etz.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://tne.xziqi.cn

"值: \(b)"
来源：http://xqw.0kj1m.cn


<!-- 参考信息 -->