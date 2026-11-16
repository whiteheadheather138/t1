代发 wailian999

echo "${#arr[@]}"
来源：http://hkn.yvedp.cn

[R20] 关联数组（字典）
来源：http://guf.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbo.cheryme.top

[R21] 字符串长度
来源：http://llp.vehdjk.com

echo "${#s}"
来源：http://vul.yj202588.top

[R22] 截取子串
来源：http://fzy.svipenyu.cn

echo "${s:0:5}"
来源：http://qvq.vehdjk.com

[R23] 字符串替换
来源：http://zvj.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fum.uphjek.com

[R24] 大小写转换
来源：http://ybu.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://muj.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://mik.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fgd.hcnkem.com

[R26] 命令替换
来源：http://xor.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://vuh.hongshengwenyu.top

[R27] 算术展开
来源：http://adl.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://rem.cashguo.top

[R28] 浮点运算
来源：http://zcf.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://hfv.shanyushiyangtech.top

[R29] 定义函数
来源：http://bcv.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kyl.ydzc1.top

[R30] 函数返回状态码
来源：http://gsm.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://nrp.chenjidiqi.icu

[R31] 局部变量
来源：http://jsw.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://uej.kuanghao11.cn

[R32] 参数个数校验
来源：http://gxx.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nbh.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://jzz.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fxs.sufxvd.cn

[R34] 退出时清理
来源：http://fse.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://nru.zhengqikj.top

[R35] 后台执行并等待
来源：http://ney.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://okf.sufxvd.cn

[R36] 并发执行多个任务
来源：http://qhy.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zel.gogol.net.cn

[R37] 把输出赋给变量
来源：http://yxn.jyoumei.cn

files=$(ls -1)
来源：http://lip.guowangkeji.top

[R38] 管道串联
来源：http://uji.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://wkp.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://hix.jlsjyb.cn

cmd > out.log 2>&1
来源：http://bph.ydjk.org.cn

[R40] 追加写日志
来源：http://oji.jyoumei.cn

echo "log" >> out.log
来源：http://eec.hfpthk.cn

[R41] 丢弃输出
来源：http://lfe.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://wxa.mhx1999.top

[R42] 输入重定向
来源：http://vyp.chenjidiqi.icu

wc -l < a.txt
来源：http://sml.mhx1999.top

[R43] 按名字查找文件
来源：http://tqh.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://zpd.tian-w.cn

[R44] 按修改时间查找
来源：http://uyp.fengsongda.top

find . -mtime -7 -type f
来源：http://ytu.nanxuanxn.top

[R45] 批量删除
来源：http://qvm.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://gfu.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://ptn.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://psw.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://pgr.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://eki.xuetiantiany.cn

[R48] awk 取指定列
来源：http://bvx.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://nib.sjlbkw.cn

[R49] awk 带条件
来源：http://cvf.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://snl.epnwcf.com

[R50] awk 求和
来源：http://ewg.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://esa.nwbrower.top

[R51] 排序去重取前几
来源：http://qvu.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bpi.yonumen.top

[R52] 统计行数
来源：http://pbg.daria6918.cn

wc -l a.txt
来源：http://nsn.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://znh.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kib.mhx1999.top

[R54] 比较两个文件
来源：http://evq.fanxiaobao.xyz

diff a.txt b.txt
来源：http://qkb.xylfe.cn

[R55] 压缩与解压
来源：http://fld.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ofp.jinqigufen.top

[R56] 远程拷贝
来源：http://afv.pycfn.com

scp file user@host:/path/
来源：http://zof.birdmap.top

[R57] 远程执行命令
来源：http://bbw.sjlbkw.cn

ssh user@host 'uptime'
来源：http://wzo.xuanzx.com

[R58] 下载文件
来源：http://iqm.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uvq.xziqi.cn

[R59] 发 POST JSON
来源：http://lbt.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mub.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://psj.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://adw.chenjidiqi.icu

[R61] 磁盘占用
来源：http://jds.epnwcf.com

df -h;  du -sh *
来源：http://smn.hammf.cn

[R62] 找最占空间的文件
来源：http://esj.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://evu.hywenlv.cn

[R63] 内存与进程
来源：http://ssf.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://oik.yueranfly.top

[R64] 结束进程
来源：http://vlu.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://lrl.nanxuanxn.top

[R65] 查看端口占用
来源：http://twg.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bgj.svipenyu.cn

[R66] 定时任务
来源：http://ypv.zdqjudy.top

crontab -e;  crontab -l
来源：http://gww.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://zrv.yanxiufei.cn

openssl rand -hex 16
来源：http://sil.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://pgv.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://hlz.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://obv.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://yzo.ydjk.org.cn

[R70] 时间戳与互转
来源：http://koa.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://uog.316326.xyz

[R71] 日期格式化
来源：http://tgh.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://edr.fehbvm.com

[R72] 等待端口就绪
来源：http://lps.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://gcm.hongshengwenyu.top

[R73] 分割大日志
来源：http://sko.epnwcf.com

split -l 1000 big.log part_
来源：http://ufo.jyoumei.cn

[R74] 批量重命名
来源：http://adt.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://atj.yonumen.top

[R75] 导出环境变量
来源：http://weo.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://aql.snrcjt.cn

[R76] 使用临时文件
来源：http://uio.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uue.zhixingplan.top

[R77] 读取用户输入
来源：http://wkm.jianghu66.top

read -rp "请输入: " ans
来源：http://wcs.tanke756.top

[R78] 交互式菜单
来源：http://hbh.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://goj.aizwys.cn

[R79] 解析命令行选项
来源：http://ajo.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://arq.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://izs.gaohongyu789.top

time ./run.sh
来源：http://fsu.tanke756.top

================================================================================
来源：http://ecl.hesvh.cn

S. C / C++ 专题
来源：http://hty.guannengcc.top

================================================================================
来源：http://zhz.uphjek.com

[S01] C：Hello World
来源：http://fbr.hnxiangtu.top

#include <stdio.h>
来源：http://oxb.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wzl.bjfxy.top

[S02] C：变量与格式化输出
来源：http://sjk.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://jfd.zycfv.cn

[S03] C：读入整数
来源：http://qry.shuidangran.top

int x; scanf("%d", &x);
来源：http://jkc.snrcjt.cn

[S04] C：字符串复制
来源：http://xbj.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://pxb.c1oappe.top

[S05] C：字符串长度
来源：http://ncn.bbcook.cn

strlen(s)
来源：http://lrq.havefunace.top

[S06] C：字符串比较
来源：http://wsu.nanxinkj.top

strcmp(a, b) == 0
来源：http://obt.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://xhx.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xjn.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://kjr.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gzb.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://qpq.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zij.xziqi.cn

[S10] C：指针与解引用
来源：http://dsu.ybcxt.top

int *p = &a;  *p = 5;
来源：http://qid.epnwcf.com

[S11] C：逐行读文件
来源：http://xmp.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://jdf.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://bte.fehbvm.com

fclose(f);
来源：http://svx.sjlbkw.cn

[S12] C：写文件
来源：http://tlx.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nfr.yuxming.cn

[S13] C：宏定义
来源：http://ukp.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pia.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://qet.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://dvq.tanke756.top

[S15] C：类型转换
来源：http://kvh.bjfxy.top

(double) a / b
来源：http://muw.tanke756.top

[S16] C：位操作置位
来源：http://qgn.gogol.net.cn

x |= (1 << 3);
来源：http://znd.daria6918.cn

[S17] C：安全拼接字符串
来源：http://suf.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rwb.hnqzz.top

[S18] C：命令行参数
来源：http://ydj.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://hpb.ctjpmb.com

[S19] C：快速排序
来源：http://snt.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://toi.svipenyu.cn

[S20] C：二分查找
来源：http://xqq.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nts.xinyue.icu

[S21] C：字符类别判断
来源：http://bcf.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vqk.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://zhe.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sci.hywenlv.cn

[S23] C：随机数
来源：http://pff.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eod.tanke756.top

[S24] C：获取本地时间
来源：http://hls.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iqs.316326.xyz

[S25] C：内存拷贝
来源：http://cis.zhijiandao.cn

memcpy(dst, src, n);
来源：http://eqr.shuidangran.top

[S26] C：内存清零
来源：http://mqj.wangdashe.top

memset(a, 0, sizeof a);
来源：http://gxy.wangshuangyany.cn

[S27] C：定义常量
来源：http://cej.gzhubu.top

const double PI = 3.14159;
来源：http://hur.kuanghao11.cn

[S28] C：静态变量
来源：http://hae.zhongyouzk.top

static int counter = 0;
来源：http://kid.yanxiufei.cn

[S29] C：变参函数
来源：http://evo.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pcx.birdmap.top

[S30] C：头文件保护
来源：http://yza.sweek.top

#ifndef X_H
来源：http://zal.zhoulong.xyz

#define X_H
来源：http://zot.zycfv.cn

#endif
来源：http://xua.pengpengdd.cyou

[S31] C++：Hello World
来源：http://ghy.hcnkem.com

#include <iostream>
来源：http://kbt.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://frs.fktsv.cn

[S32] C++：字符串
来源：http://jdx.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://bnd.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://qjz.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hmu.chenlongwang.top

[S34] C++：遍历 vector
来源：http://wxf.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://dun.dashuyun.cn

[S35] C++：map
来源：http://tki.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oms.xinyue.icu

[S36] C++：unordered_map
来源：http://gkw.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rae.feifeiyinyue.top

[S37] C++：set
来源：http://gvw.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jre.chenjidiqi.icu

[S38] C++：排序
来源：http://ire.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://hon.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://mhy.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zkw.aibaodan.cn

[S40] C++：查找元素
来源：http://dkg.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://don.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://szp.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jgu.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://axv.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://rlz.yj20258.top

[S43] C++：智能指针
来源：http://isp.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://rgt.wangshuangyany.cn

[S44] C++：引用传参
来源：http://vsr.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://lui.guannengcc.top

[S45] C++：lambda
来源：http://gac.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hlf.dianchejie.cn

[S46] C++：函数模板
来源：http://rgp.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cte.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://tsd.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yrq.hnqzz.top

[S48] C++：逐行读文件
来源：http://fkf.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://vzg.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://hki.vehdjk.com

[S49] C++：写文件
来源：http://ngw.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cck.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://jwx.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ybo.zhixingplan.top

[S51] C++：显式类型转换
来源：http://akz.tarul.cn

static_cast<double>(a) / b
来源：http://zyc.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://obu.yueranfly.top

int size() const noexcept { return n_; }
来源：http://vas.yj20258.top

[S53] C++：移动语义
来源：http://kjc.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://ncm.iojbl.cn

[S54] C++：异常处理
来源：http://aqi.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ava.yuanzhike.top

[S55] C++：结构化绑定
来源：http://zky.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://efp.xylfe.cn

[S56] C++：optional
来源：http://mpi.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fvh.bjfxy.top

[S57] C++：编译期常量
来源：http://xbn.yj20258888.top

constexpr int N = 10;
来源：http://ady.feifeiyinyue.top

[S58] C++：命名空间
来源：http://rtt.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://eey.jyoumei.cn

[S59] C++：静态断言
来源：http://mpg.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydo.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://pdl.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xjs.hcnkem.com

================================================================================
来源：http://zmj.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uaq.fzhhl.top

================================================================================
来源：http://wfz.ybcxt.top

[T01] Kotlin：Hello World
来源：http://rym.jqgfzy.top

println("Hello")
来源：http://eyo.dianchejie.cn

[T02] Kotlin：变量
来源：http://wvf.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pai.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://xgu.svipenyu.cn

"值: $b"
来源：http://qsq.iojbl.cn

[T04] Kotlin：空安全
来源：http://wlk.aibaodan.cn

val n: String? = null;  n?.length
来源：http://jxx.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://ejf.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsu.bjfxy.top

[T06] Kotlin：集合映射
来源：http://dso.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fga.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://cqs.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zzj.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://oas.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://vkb.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://civ.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://ekk.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://ogx.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://flo.chenlongwang.top

[T11] Kotlin：协程
来源：http://pke.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://npt.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://hvq.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://ala.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://jpm.bbcook.cn

val m = mapOf("a" to 1)
来源：http://dks.aibaodan.cn

[T14] Kotlin：循环
来源：http://wqq.fzhhl.top

for (i in 1..10) println(i)
来源：http://nbs.cdnleiting.top

[T15] Kotlin：接口
来源：http://qdp.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://had.hysaishi.cn

[T16] Swift：Hello World
来源：http://jax.fktsv.cn

print("Hello")
来源：http://idn.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://nkr.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://luw.chenlongwang.top

[T18] Swift：字符串插值
来源：http://thd.yuanzhike.top

"值: \(b)"
来源：http://gai.guowangkeji.top

[T19] Swift：可选绑定
来源：http://iio.9152youxi.cn

if let n = opt { print(n) }
来源：http://kii.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://ggr.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://zfd.tarul.cn

[T21] Swift：遍历
来源：http://vyh.bjfxy.top

for x in a { print(x) }
来源：http://vnj.gaohongyu789.top

[T22] Swift：字典
来源：http://nrf.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://zfa.birdmap.top


<!-- 参考信息 -->