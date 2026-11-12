代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxs.aibaodan.cn

[R16] until 等待条件
来源：http://xfj.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ukh.jqgufenzy.top

[R17] 数组定义与取值
来源：http://oty.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://xdq.yj20258888.top

[R18] 遍历数组
来源：http://wem.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ksb.nwbrower.top

[R19] 数组长度
来源：http://krm.daria6918.cn

echo "${#arr[@]}"
来源：http://noa.fzhhl.top

[R20] 关联数组（字典）
来源：http://ccd.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cbe.shangyingyoupin.top

[R21] 字符串长度
来源：http://psr.gaohongyu789.top

echo "${#s}"
来源：http://gxv.tanke756.top

[R22] 截取子串
来源：http://nqt.wangdashe.top

echo "${s:0:5}"
来源：http://dtk.smart0.xyz

[R23] 字符串替换
来源：http://pnx.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sjo.daria6918.cn

[R24] 大小写转换
来源：http://kdg.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://liw.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://bgz.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tdc.shanyushiyangtech.top

[R26] 命令替换
来源：http://fau.uphjek.com

now=$(date +%F); echo "$now"
来源：http://wed.ybcxt.top

[R27] 算术展开
来源：http://zxm.316326.xyz

echo $((1 + 2 * 3))
来源：http://nqr.jiagoushi.top

[R28] 浮点运算
来源：http://edp.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://nag.gaohongyu789.top

[R29] 定义函数
来源：http://ctg.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vsc.yfazqb.com

[R30] 函数返回状态码
来源：http://iaa.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://beb.daria6918.cn

[R31] 局部变量
来源：http://fks.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://zmp.vehdjk.com

[R32] 参数个数校验
来源：http://yhx.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lli.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://mht.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kqt.jiagoushi.top

[R34] 退出时清理
来源：http://lhu.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://lwt.hnxiangtu.top

[R35] 后台执行并等待
来源：http://clv.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mcj.sufxvd.cn

[R36] 并发执行多个任务
来源：http://msn.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fla.gotoacloud.top

[R37] 把输出赋给变量
来源：http://qbi.jinyuanbaomall.cn

files=$(ls -1)
来源：http://mce.fehbvm.com

[R38] 管道串联
来源：http://vnz.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://dce.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://wbu.daxiang520.top

cmd > out.log 2>&1
来源：http://pkm.cashguo.top

[R40] 追加写日志
来源：http://avt.dianchejie.cn

echo "log" >> out.log
来源：http://kvs.316326.xyz

[R41] 丢弃输出
来源：http://hgx.ydzc1.top

cmd >/dev/null 2>&1
来源：http://ssp.nanxuanxn.top

[R42] 输入重定向
来源：http://dlm.316326.xyz

wc -l < a.txt
来源：http://wus.daria6918.cn

[R43] 按名字查找文件
来源：http://zzq.tianlin.xyz

find . -name "*.log" -type f
来源：http://sad.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://hyy.meibo888.top

find . -mtime -7 -type f
来源：http://kac.iojbl.cn

[R45] 批量删除
来源：http://nlq.andypj.xyz

find . -name "*.tmp" -delete
来源：http://buo.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://cwh.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://byx.bbcook.cn

[R47] sed 单行替换
来源：http://xbo.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ifi.zhoulong.xyz

[R48] awk 取指定列
来源：http://fnv.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://qyz.cucudq.cn

[R49] awk 带条件
来源：http://rhm.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pmt.epnwcf.com

[R50] awk 求和
来源：http://zar.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://kgr.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://ben.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gjj.nanxuanxn.top

[R52] 统计行数
来源：http://jif.shanyushiyangtech.top

wc -l a.txt
来源：http://tvm.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://tfe.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qgb.sufxvd.cn

[R54] 比较两个文件
来源：http://rep.gotoacloud.top

diff a.txt b.txt
来源：http://xmz.cheryme.top

[R55] 压缩与解压
来源：http://hcf.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lkp.yuxming.cn

[R56] 远程拷贝
来源：http://mak.ivvv.top

scp file user@host:/path/
来源：http://kqs.zhongyouzk.top

[R57] 远程执行命令
来源：http://czt.guowangkeji.top

ssh user@host 'uptime'
来源：http://uwh.iojbl.cn

[R58] 下载文件
来源：http://jhx.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://znp.gzhubu.top

[R59] 发 POST JSON
来源：http://ifp.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zmm.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://isd.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mht.sjlbkw.cn

[R61] 磁盘占用
来源：http://daa.hnqzz.top

df -h;  du -sh *
来源：http://uof.gzhubu.top

[R62] 找最占空间的文件
来源：http://vxa.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://rke.gaohongyu789.top

[R63] 内存与进程
来源：http://mwr.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://jth.0kj1m.cn

[R64] 结束进程
来源：http://bcg.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://vmq.dianchejie.cn

[R65] 查看端口占用
来源：http://qat.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://acu.chenlongwang.top

[R66] 定时任务
来源：http://ech.jqgufenzy.top

crontab -e;  crontab -l
来源：http://feg.hcnkem.com

[R67] 生成随机十六进制串
来源：http://znk.nwbrower.top

openssl rand -hex 16
来源：http://jgr.sjlbkw.cn

[R68] 计算文件校验值
来源：http://sjp.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://uae.yangfankeji.com

[R69] 生成随机密码
来源：http://udw.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://isp.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://zig.cashguo.top

date +%s;  date -d @1700000000
来源：http://foh.xylfe.cn

[R71] 日期格式化
来源：http://ncg.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bti.jlsjyb.cn

[R72] 等待端口就绪
来源：http://vfl.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ewy.jinqigfzy.top

[R73] 分割大日志
来源：http://kvw.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://med.cucudq.cn

[R74] 批量重命名
来源：http://opi.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jqj.xinyue.icu

[R75] 导出环境变量
来源：http://ndp.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://bml.jlsjyb.cn

[R76] 使用临时文件
来源：http://oiz.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dzy.haohaochexian.top

[R77] 读取用户输入
来源：http://xas.zhoulong.xyz

read -rp "请输入: " ans
来源：http://qvt.aibaodan.cn

[R78] 交互式菜单
来源：http://vup.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sgf.zdqjudy.top

[R79] 解析命令行选项
来源：http://rnn.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fwq.hammf.cn

[R80] 查看脚本执行耗时
来源：http://oky.haohaochexian.top

time ./run.sh
来源：http://isx.hywenlv.cn

================================================================================
来源：http://rmx.quarkkingdee.top

S. C / C++ 专题
来源：http://wwt.sufxvd.cn

================================================================================
来源：http://bao.dianchejie.cn

[S01] C：Hello World
来源：http://bbk.hnxiangtu.top

#include <stdio.h>
来源：http://wes.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hkg.guannengcc.top

[S02] C：变量与格式化输出
来源：http://dpt.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://hkd.guowangkeji.top

[S03] C：读入整数
来源：http://buf.xinyue.icu

int x; scanf("%d", &x);
来源：http://qyw.cashguo.top

[S04] C：字符串复制
来源：http://jqb.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://zmn.sxryk.cn

[S05] C：字符串长度
来源：http://maq.aibaodan.cn

strlen(s)
来源：http://leb.sxryk.cn

[S06] C：字符串比较
来源：http://apu.yvedp.cn

strcmp(a, b) == 0
来源：http://ide.zycfv.cn

[S07] C：数组遍历求和
来源：http://kyc.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bwn.yonumen.top

[S08] C：动态内存分配与释放
来源：http://yzm.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vmy.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://ubz.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dbj.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://ybo.iojbl.cn

int *p = &a;  *p = 5;
来源：http://rgh.zdqjudy.top

[S11] C：逐行读文件
来源：http://tvo.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://vbw.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://djp.yangfankeji.com

fclose(f);
来源：http://fgz.redwolf501.top

[S12] C：写文件
来源：http://qab.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dko.nanxuanxn.top

[S13] C：宏定义
来源：http://yuf.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pke.tianlin.xyz

[S14] C：枚举
来源：http://dof.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://boc.chenlongwang.top

[S15] C：类型转换
来源：http://hwv.yuxming.cn

(double) a / b
来源：http://ubr.shzxlz.cn

[S16] C：位操作置位
来源：http://fvk.zhijiandao.cn

x |= (1 << 3);
来源：http://lue.ydzc1.top

[S17] C：安全拼接字符串
来源：http://snz.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mdg.yanxiufei.cn

[S18] C：命令行参数
来源：http://kct.yanxiufei.cn

int main(int argc, char **argv)
来源：http://gkb.jlsjyb.cn

[S19] C：快速排序
来源：http://aaj.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jsl.yfazqb.com

[S20] C：二分查找
来源：http://dvf.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pfi.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://qob.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gau.smart0.xyz

[S22] C：字符串转数字
来源：http://pfk.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://mux.xuanzx.com

[S23] C：随机数
来源：http://wjv.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wke.yvedp.cn

[S24] C：获取本地时间
来源：http://toi.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fsg.xziqi.cn

[S25] C：内存拷贝
来源：http://xfw.hfpthk.cn

memcpy(dst, src, n);
来源：http://fzf.sweek.top

[S26] C：内存清零
来源：http://xpp.xziqi.cn

memset(a, 0, sizeof a);
来源：http://hxf.fengsongda.top

[S27] C：定义常量
来源：http://wdz.tarul.cn

const double PI = 3.14159;
来源：http://hdq.fzhhl.top

[S28] C：静态变量
来源：http://noz.ybcxt.top

static int counter = 0;
来源：http://oai.ehwqpu.com

[S29] C：变参函数
来源：http://cfx.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lgz.sysykeji.top

[S30] C：头文件保护
来源：http://ibd.yuanzhike.top

#ifndef X_H
来源：http://tyq.xuetiantiany.cn

#define X_H
来源：http://sni.pycfn.com

#endif
来源：http://gvl.zhengqikj.top

[S31] C++：Hello World
来源：http://cxv.zhaomingkeji.xyz

#include <iostream>
来源：http://mzv.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://dfk.shuidangran.top

[S32] C++：字符串
来源：http://zio.316326.xyz

std::string s = "hi";  s += "!";
来源：http://nfp.yuanzhike.top

[S33] C++：vector 增删
来源：http://rbc.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ctu.wangdashe.top

[S34] C++：遍历 vector
来源：http://qwa.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://jll.gzhubu.top

[S35] C++：map
来源：http://xze.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yzd.yonumen.top

[S36] C++：unordered_map
来源：http://scr.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jhy.quarkkingdee.top

[S37] C++：set
来源：http://qcn.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hsj.yuxming.cn

[S38] C++：排序
来源：http://zpo.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://rir.tarul.cn

[S39] C++：自定义比较器排序
来源：http://ysq.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://alk.vqdsnc.cn

[S40] C++：查找元素
来源：http://gcb.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zvi.andypj.xyz

[S41] C++：类与构造函数
来源：http://hqd.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rwq.epnwcf.com

[S42] C++：继承与虚函数
来源：http://ofj.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://uex.nwbrower.top

[S43] C++：智能指针
来源：http://etd.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://iid.zhongyouzk.top

[S44] C++：引用传参
来源：http://gzn.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://vwp.hysaishi.cn

[S45] C++：lambda
来源：http://oij.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://cpj.yangfankeji.com

[S46] C++：函数模板
来源：http://anq.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ufa.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://vfo.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yyi.hnqzz.top

[S48] C++：逐行读文件
来源：http://juc.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xwq.fzhhl.top

while (std::getline(in, line)) { }
来源：http://eiz.shangyingyoupin.top

[S49] C++：写文件
来源：http://zwp.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tkv.yuanzhike.top

[S50] C++：格式化数字
来源：http://ivq.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jjq.zycfv.cn

[S51] C++：显式类型转换
来源：http://mxp.cqqwz.cn

static_cast<double>(a) / b
来源：http://fxr.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://eaq.mhx1999.top

int size() const noexcept { return n_; }
来源：http://rqb.yonumen.top

[S53] C++：移动语义
来源：http://ixx.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://fby.nanxinkj.top

[S54] C++：异常处理
来源：http://evf.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyb.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://gyj.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://uhz.snrcjt.cn

[S56] C++：optional
来源：http://xtk.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yzp.shzxlz.cn

[S57] C++：编译期常量
来源：http://hxn.snrcjt.cn

constexpr int N = 10;
来源：http://ghu.hywenlv.cn

[S58] C++：命名空间
来源：http://tjl.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://uhn.nanxuanxn.top

[S59] C++：静态断言
来源：http://omj.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://opo.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://bgj.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hql.fzhhl.top

================================================================================
来源：http://aos.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wxo.yj20258.top

================================================================================
来源：http://awf.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://bxs.jinqigfzy.top

println("Hello")
来源：http://giy.pycfn.com

[T02] Kotlin：变量
来源：http://hvi.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xyi.yj20258.top

[T03] Kotlin：字符串模板
来源：http://zma.bbcook.cn

"值: $b"
来源：http://zyy.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ddd.316326.xyz

val n: String? = null;  n?.length
来源：http://ahw.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://qfr.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npd.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://cvi.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iyb.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://fmi.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://avm.ehwqpu.com

[T08] Kotlin：数据类
来源：http://dhi.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://aja.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://iuj.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://qlm.fzhhl.top

[T10] Kotlin：默认参数
来源：http://uhn.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bfe.hcnkem.com

[T11] Kotlin：协程
来源：http://lpl.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://spm.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://lya.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://iqj.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://pjb.fktsv.cn

val m = mapOf("a" to 1)
来源：http://tfo.yanxiufei.cn

[T14] Kotlin：循环
来源：http://tqh.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://vcc.0kj1m.cn

[T15] Kotlin：接口
来源：http://elq.smart0.xyz

interface Shape { fun area(): Double }
来源：http://niy.fehbvm.com

[T16] Swift：Hello World
来源：http://bgs.hammf.cn

print("Hello")
来源：http://zau.cheryme.top

[T17] Swift：变量与常量
来源：http://uyq.yongpay.top

var a = 1;  let b = 2
来源：http://pyx.sysykeji.top

[T18] Swift：字符串插值
来源：http://cgb.ivvv.top

"值: \(b)"
来源：http://mem.yongpay.top


<!-- 参考信息 -->