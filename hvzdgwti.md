代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://xyc.yj202588.top

[R18] 遍历数组
来源：http://zpd.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mrn.jianghu66.top

[R19] 数组长度
来源：http://uvt.meibo888.top

echo "${#arr[@]}"
来源：http://gxs.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://aol.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kem.tianlin.xyz

[R21] 字符串长度
来源：http://vfz.ehwqpu.com

echo "${#s}"
来源：http://vmv.ehwqpu.com

[R22] 截取子串
来源：http://wzl.feifeiyinyue.top

echo "${s:0:5}"
来源：http://pcg.smart0.xyz

[R23] 字符串替换
来源：http://adz.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hbp.nwbrower.top

[R24] 大小写转换
来源：http://sjk.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://uef.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://wrl.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wbk.jianghu66.top

[R26] 命令替换
来源：http://lav.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://alu.shanyushiyangtech.top

[R27] 算术展开
来源：http://kxw.gzhubu.top

echo $((1 + 2 * 3))
来源：http://jkv.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://whc.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://lim.xuanzx.com

[R29] 定义函数
来源：http://cgy.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xlc.xziqi.cn

[R30] 函数返回状态码
来源：http://xim.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://ypa.nanxinkj.top

[R31] 局部变量
来源：http://iah.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://yqx.ctjpmb.com

[R32] 参数个数校验
来源：http://tgu.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wzi.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://ign.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kuh.yj202588.top

[R34] 退出时清理
来源：http://oco.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://soh.jinqigfzy.top

[R35] 后台执行并等待
来源：http://pfd.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vjw.tian-w.cn

[R36] 并发执行多个任务
来源：http://ozk.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://geq.yfazqb.com

[R37] 把输出赋给变量
来源：http://zqu.gaohongyu789.top

files=$(ls -1)
来源：http://vwb.hammf.cn

[R38] 管道串联
来源：http://osx.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://pla.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://cqy.cashguo.top

cmd > out.log 2>&1
来源：http://npl.snrcjt.cn

[R40] 追加写日志
来源：http://llp.yuxming.cn

echo "log" >> out.log
来源：http://nun.zhongyouzk.top

[R41] 丢弃输出
来源：http://vwn.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://zjf.tanke756.top

[R42] 输入重定向
来源：http://dak.jyoumei.cn

wc -l < a.txt
来源：http://zol.kuanghao11.cn

[R43] 按名字查找文件
来源：http://rbp.cqqwz.cn

find . -name "*.log" -type f
来源：http://ovk.birdmap.top

[R44] 按修改时间查找
来源：http://nvb.gotoacloud.top

find . -mtime -7 -type f
来源：http://esq.iojbl.cn

[R45] 批量删除
来源：http://ypy.jianghu66.top

find . -name "*.tmp" -delete
来源：http://hrz.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://ver.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxi.hnqzz.top

[R47] sed 单行替换
来源：http://snc.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vta.ydjk.org.cn

[R48] awk 取指定列
来源：http://ftd.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://qcv.fktsv.cn

[R49] awk 带条件
来源：http://ked.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lnh.316326.xyz

[R50] awk 求和
来源：http://mvr.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://qom.yangfankeji.com

[R51] 排序去重取前几
来源：http://psh.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mda.jyoumei.cn

[R52] 统计行数
来源：http://jnu.gogol.net.cn

wc -l a.txt
来源：http://dlj.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://fug.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdh.fzhhl.top

[R54] 比较两个文件
来源：http://uxu.jyoumei.cn

diff a.txt b.txt
来源：http://alx.xinyue.icu

[R55] 压缩与解压
来源：http://xfh.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zsj.shangyingyoupin.top

[R56] 远程拷贝
来源：http://daa.cdnleiting.top

scp file user@host:/path/
来源：http://gxk.mhx1999.top

[R57] 远程执行命令
来源：http://bkg.jianghu66.top

ssh user@host 'uptime'
来源：http://wfs.smart0.xyz

[R58] 下载文件
来源：http://jls.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ont.bbcook.cn

[R59] 发 POST JSON
来源：http://aur.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ejr.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://xtn.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpt.xinyue.icu

[R61] 磁盘占用
来源：http://kjv.quarkkingdee.top

df -h;  du -sh *
来源：http://nqk.yvedp.cn

[R62] 找最占空间的文件
来源：http://pjw.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://jcn.chenzaomai.com

[R63] 内存与进程
来源：http://jgn.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://kbf.feifeiyinyue.top

[R64] 结束进程
来源：http://uuh.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://smb.ppjwa.cn

[R65] 查看端口占用
来源：http://cew.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jvh.redwolf501.top

[R66] 定时任务
来源：http://wmx.haohaochexian.top

crontab -e;  crontab -l
来源：http://ymz.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://tsn.bjfxy.top

openssl rand -hex 16
来源：http://fam.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://ypc.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cyz.ctjpmb.com

[R69] 生成随机密码
来源：http://hyc.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://idl.guowangkeji.top

[R70] 时间戳与互转
来源：http://eog.cucudq.cn

date +%s;  date -d @1700000000
来源：http://lxe.316326.xyz

[R71] 日期格式化
来源：http://kix.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://luu.yj20258888.top

[R72] 等待端口就绪
来源：http://nds.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rzk.zdbjq.cn

[R73] 分割大日志
来源：http://lnp.yuxming.cn

split -l 1000 big.log part_
来源：http://rgn.jiagoushi.top

[R74] 批量重命名
来源：http://mkv.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://omx.snrcjt.cn

[R75] 导出环境变量
来源：http://ufg.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://ivr.cheryme.top

[R76] 使用临时文件
来源：http://xtm.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eoq.nanxuanxn.top

[R77] 读取用户输入
来源：http://tut.daxiang520.top

read -rp "请输入: " ans
来源：http://gpg.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://ekl.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xpt.mhx1999.top

[R79] 解析命令行选项
来源：http://pjc.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsg.pycfn.com

[R80] 查看脚本执行耗时
来源：http://odl.0kj1m.cn

time ./run.sh
来源：http://kbm.shanyushiyangkeji.top

================================================================================
来源：http://sak.hysaishi.cn

S. C / C++ 专题
来源：http://axs.sweek.top

================================================================================
来源：http://pvi.birdmap.top

[S01] C：Hello World
来源：http://ocl.yonumen.top

#include <stdio.h>
来源：http://xdh.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lrn.daria6918.cn

[S02] C：变量与格式化输出
来源：http://rvd.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://msa.yj202588.top

[S03] C：读入整数
来源：http://mum.meibo888.top

int x; scanf("%d", &x);
来源：http://ixg.jiagoushi.top

[S04] C：字符串复制
来源：http://okg.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uil.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://uep.meibo888.top

strlen(s)
来源：http://byq.sweek.top

[S06] C：字符串比较
来源：http://tvc.fehbvm.com

strcmp(a, b) == 0
来源：http://war.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://nfh.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://veq.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://ooy.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wnx.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://xnf.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pdz.sufxvd.cn

[S10] C：指针与解引用
来源：http://hji.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://drc.gzhubu.top

[S11] C：逐行读文件
来源：http://feo.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://maf.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ojs.aibaodan.cn

fclose(f);
来源：http://nyh.ybcxt.top

[S12] C：写文件
来源：http://chx.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ndp.pengpengdd.cyou

[S13] C：宏定义
来源：http://yyg.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pws.zhiwuduotai.top

[S14] C：枚举
来源：http://jcz.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://lhz.tanke756.top

[S15] C：类型转换
来源：http://gbl.jyoumei.cn

(double) a / b
来源：http://hwb.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://bom.quarkkingdee.top

x |= (1 << 3);
来源：http://giz.havefunace.top

[S17] C：安全拼接字符串
来源：http://bls.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fbb.chenjidiqi.icu

[S18] C：命令行参数
来源：http://ahx.snrcjt.cn

int main(int argc, char **argv)
来源：http://diz.shuidangran.top

[S19] C：快速排序
来源：http://sbm.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nwe.jianghu66.top

[S20] C：二分查找
来源：http://abk.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zhu.c1oappe.top

[S21] C：字符类别判断
来源：http://ejv.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vot.mhx1999.top

[S22] C：字符串转数字
来源：http://swu.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://dwx.0kj1m.cn

[S23] C：随机数
来源：http://dum.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mxb.sxryk.cn

[S24] C：获取本地时间
来源：http://laf.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xaf.zhijiandao.cn

[S25] C：内存拷贝
来源：http://blx.yueranfly.top

memcpy(dst, src, n);
来源：http://odq.jinqigfzy.top

[S26] C：内存清零
来源：http://uip.fktsv.cn

memset(a, 0, sizeof a);
来源：http://fyl.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://kcs.hnxiangtu.top

const double PI = 3.14159;
来源：http://vjz.xziqi.cn

[S28] C：静态变量
来源：http://exh.jinqigfzy.top

static int counter = 0;
来源：http://zye.yangfankeji.com

[S29] C：变参函数
来源：http://oeh.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bma.fehbvm.com

[S30] C：头文件保护
来源：http://knj.zycfv.cn

#ifndef X_H
来源：http://rcb.fengsongda.top

#define X_H
来源：http://pio.sjlbkw.cn

#endif
来源：http://yow.ppjwa.cn

[S31] C++：Hello World
来源：http://suo.zhixingplan.top

#include <iostream>
来源：http://iya.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://whx.quarkkingdee.top

[S32] C++：字符串
来源：http://irk.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://vof.zdqjudy.top

[S33] C++：vector 增删
来源：http://kse.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zqp.cdnleiting.top

[S34] C++：遍历 vector
来源：http://fol.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://err.hesvh.cn

[S35] C++：map
来源：http://jln.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mtc.jianghu66.top

[S36] C++：unordered_map
来源：http://zqp.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://foa.jianghu66.top

[S37] C++：set
来源：http://oyk.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xzl.hnxiangtu.top

[S38] C++：排序
来源：http://zos.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://sep.316326.xyz

[S39] C++：自定义比较器排序
来源：http://syp.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cdl.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://awz.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qcq.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://cvt.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ikz.316326.xyz

[S42] C++：继承与虚函数
来源：http://sdp.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://etf.mhx1999.top

[S43] C++：智能指针
来源：http://ltt.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://his.wangshuangyany.cn

[S44] C++：引用传参
来源：http://gxu.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://ulw.ctjpmb.com

[S45] C++：lambda
来源：http://apt.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://sdh.cashguo.top

[S46] C++：函数模板
来源：http://yqu.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kao.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://wav.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pyi.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://pfy.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lki.meibo888.top

while (std::getline(in, line)) { }
来源：http://kpi.hfpthk.cn

[S49] C++：写文件
来源：http://oye.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://phj.yfazqb.com

[S50] C++：格式化数字
来源：http://qqb.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gcf.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://hvb.zhongyouzk.top

static_cast<double>(a) / b
来源：http://jfo.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://jhu.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://ykq.9152youxi.cn

[S53] C++：移动语义
来源：http://ofe.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://zjc.jinqigufen.top

[S54] C++：异常处理
来源：http://gri.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxk.cheryme.top

[S55] C++：结构化绑定
来源：http://tyt.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://okd.dianchejie.cn

[S56] C++：optional
来源：http://sob.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sfd.hywenlv.cn

[S57] C++：编译期常量
来源：http://gqb.zhiwuduotai.top

constexpr int N = 10;
来源：http://vnk.yfazqb.com

[S58] C++：命名空间
来源：http://ele.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://dsq.jianghu66.top

[S59] C++：静态断言
来源：http://hxi.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfz.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://aia.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ral.cashguo.top

================================================================================
来源：http://zdf.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fyr.meibo888.top

================================================================================
来源：http://odo.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://ahg.hnxiangtu.top

println("Hello")
来源：http://nai.guannengcc.top

[T02] Kotlin：变量
来源：http://icn.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmz.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://drd.xylfe.cn

"值: $b"
来源：http://bfl.yj202588.top

[T04] Kotlin：空安全
来源：http://gga.sxryk.cn

val n: String? = null;  n?.length
来源：http://xag.sweek.top

[T05] Kotlin：when 表达式
来源：http://ezk.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jxo.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://fgm.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://snw.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://zfy.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xyn.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://myh.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://lmv.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://azi.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://loo.sweek.top

[T10] Kotlin：默认参数
来源：http://qbv.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lqe.svipenyu.cn

[T11] Kotlin：协程
来源：http://tyt.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mrg.xinyue.icu

[T12] Kotlin：解构声明
来源：http://hyy.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://dmp.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://moh.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://wfu.sufxvd.cn

[T14] Kotlin：循环
来源：http://ngy.yj202588.top

for (i in 1..10) println(i)
来源：http://anb.ehwqpu.com

[T15] Kotlin：接口
来源：http://rmc.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://igg.c1oappe.top

[T16] Swift：Hello World
来源：http://dlq.jinyuanbaomall.cn

print("Hello")
来源：http://yhe.yonumen.top

[T17] Swift：变量与常量
来源：http://qik.fengsongda.top

var a = 1;  let b = 2
来源：http://bcg.xziqi.cn

[T18] Swift：字符串插值
来源：http://inz.vehdjk.com

"值: \(b)"
来源：http://vvw.tanke756.top

[T19] Swift：可选绑定
来源：http://dor.sxryk.cn

if let n = opt { print(n) }
来源：http://tdq.yj20258.top

[T20] Swift：数组操作
来源：http://tem.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://abw.fzhhl.top


<!-- 参考信息 -->