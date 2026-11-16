代发 wailian999

echo "${#arr[@]}"
来源：http://dyj.ctjpmb.com

[R20] 关联数组（字典）
来源：http://ero.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bjv.pengpengdd.cyou

[R21] 字符串长度
来源：http://nei.iojbl.cn

echo "${#s}"
来源：http://kbo.havefunace.top

[R22] 截取子串
来源：http://dtm.bjfxy.top

echo "${s:0:5}"
来源：http://nrk.andypj.xyz

[R23] 字符串替换
来源：http://hkl.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rpz.ctjpmb.com

[R24] 大小写转换
来源：http://obm.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jdg.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://mze.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://thu.yangfankeji.com

[R26] 命令替换
来源：http://ajf.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://kfg.feifeiyinyue.top

[R27] 算术展开
来源：http://srl.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://bex.wangshuangyany.cn

[R28] 浮点运算
来源：http://hlz.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://dmj.tanke756.top

[R29] 定义函数
来源：http://dhu.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vfc.yangfankeji.com

[R30] 函数返回状态码
来源：http://owt.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://wnv.aizwys.cn

[R31] 局部变量
来源：http://vdj.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://qqj.yuxming.cn

[R32] 参数个数校验
来源：http://wsi.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vjk.hammf.cn

[R33] 捕获错误并提示行号
来源：http://zdo.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rie.jqgufenzy.top

[R34] 退出时清理
来源：http://tio.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://mxp.shuidangran.top

[R35] 后台执行并等待
来源：http://pqa.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vvs.yj20258888.top

[R36] 并发执行多个任务
来源：http://xbu.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gfm.yvedp.cn

[R37] 把输出赋给变量
来源：http://gwh.iojbl.cn

files=$(ls -1)
来源：http://afg.cashguo.top

[R38] 管道串联
来源：http://syj.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://lhw.tanke756.top

[R39] 重定向标准输出与错误
来源：http://xdv.zhengqikj.top

cmd > out.log 2>&1
来源：http://ovv.ydjk.org.cn

[R40] 追加写日志
来源：http://qaw.uphjek.com

echo "log" >> out.log
来源：http://zwh.cdnleiting.top

[R41] 丢弃输出
来源：http://nbk.yvedp.cn

cmd >/dev/null 2>&1
来源：http://nrq.ybcxt.top

[R42] 输入重定向
来源：http://xwu.chenlongwang.top

wc -l < a.txt
来源：http://dwb.gzhubu.top

[R43] 按名字查找文件
来源：http://ojm.hysaishi.cn

find . -name "*.log" -type f
来源：http://iyp.nwbrower.top

[R44] 按修改时间查找
来源：http://mbx.haohaochexian.top

find . -mtime -7 -type f
来源：http://twd.cucudq.cn

[R45] 批量删除
来源：http://car.yongpay.top

find . -name "*.tmp" -delete
来源：http://ctx.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://zij.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhw.yanxiufei.cn

[R47] sed 单行替换
来源：http://kzl.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ras.cdnleiting.top

[R48] awk 取指定列
来源：http://ihw.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://oso.cucudq.cn

[R49] awk 带条件
来源：http://asv.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://erz.zhengqikj.top

[R50] awk 求和
来源：http://juy.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rpq.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://ufu.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://alr.jinqigfzy.top

[R52] 统计行数
来源：http://xwr.sjlbkw.cn

wc -l a.txt
来源：http://rqx.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://nrt.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://emu.zhiwuduotai.top

[R54] 比较两个文件
来源：http://vgr.hesvh.cn

diff a.txt b.txt
来源：http://lax.ydzc1.top

[R55] 压缩与解压
来源：http://and.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zgu.gzhubu.top

[R56] 远程拷贝
来源：http://meg.shanyushiyangtech.top

scp file user@host:/path/
来源：http://cnj.316326.xyz

[R57] 远程执行命令
来源：http://vpi.guowangkeji.top

ssh user@host 'uptime'
来源：http://gfv.jianghu66.top

[R58] 下载文件
来源：http://rwu.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tog.kuanghao11.cn

[R59] 发 POST JSON
来源：http://qor.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rgg.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://vds.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zji.c1oappe.top

[R61] 磁盘占用
来源：http://fea.gaohongyu789.top

df -h;  du -sh *
来源：http://sfa.jianghu66.top

[R62] 找最占空间的文件
来源：http://xrd.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://vay.andypj.xyz

[R63] 内存与进程
来源：http://une.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://oli.hnxiangtu.top

[R64] 结束进程
来源：http://zen.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://jvc.daria6918.cn

[R65] 查看端口占用
来源：http://qjr.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lfd.guowangkeji.top

[R66] 定时任务
来源：http://nwf.shzxlz.cn

crontab -e;  crontab -l
来源：http://ftg.yj20258.top

[R67] 生成随机十六进制串
来源：http://izf.bbcook.cn

openssl rand -hex 16
来源：http://msk.52xcode.cn

[R68] 计算文件校验值
来源：http://vrz.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://irn.tianlin.xyz

[R69] 生成随机密码
来源：http://rgm.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://gxt.havefunace.top

[R70] 时间戳与互转
来源：http://djt.birdmap.top

date +%s;  date -d @1700000000
来源：http://ifd.daria6918.cn

[R71] 日期格式化
来源：http://iiv.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ghr.fengsongda.top

[R72] 等待端口就绪
来源：http://uzj.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://uur.sjlbkw.cn

[R73] 分割大日志
来源：http://cta.jiagoushi.top

split -l 1000 big.log part_
来源：http://bvk.cheryme.top

[R74] 批量重命名
来源：http://msk.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lir.jqgfzy.top

[R75] 导出环境变量
来源：http://rwh.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://poi.0kj1m.cn

[R76] 使用临时文件
来源：http://ykq.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://twc.c1oappe.top

[R77] 读取用户输入
来源：http://uzr.yongpay.top

read -rp "请输入: " ans
来源：http://mwp.fengsongda.top

[R78] 交互式菜单
来源：http://dhq.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qcq.cheryme.top

[R79] 解析命令行选项
来源：http://eob.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://clj.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://qvd.nanxinkj.top

time ./run.sh
来源：http://tcv.xylfe.cn

================================================================================
来源：http://drv.feifeiyinyue.top

S. C / C++ 专题
来源：http://bqe.hnxiangtu.top

================================================================================
来源：http://lhy.mhx1999.top

[S01] C：Hello World
来源：http://buk.jianghu66.top

#include <stdio.h>
来源：http://fuz.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://muf.wangdashe.top

[S02] C：变量与格式化输出
来源：http://bel.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://lpj.zhixingplan.top

[S03] C：读入整数
来源：http://idl.redwolf501.top

int x; scanf("%d", &x);
来源：http://ttx.zycfv.cn

[S04] C：字符串复制
来源：http://gfi.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oat.zhiwuduotai.top

[S05] C：字符串长度
来源：http://dhh.bjfxy.top

strlen(s)
来源：http://woq.meibo888.top

[S06] C：字符串比较
来源：http://znj.smart0.xyz

strcmp(a, b) == 0
来源：http://suu.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://yvy.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vue.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://pvv.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hdp.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://hcv.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cxh.nanxuanxn.top

[S10] C：指针与解引用
来源：http://rsn.ybcxt.top

int *p = &a;  *p = 5;
来源：http://aps.fzhhl.top

[S11] C：逐行读文件
来源：http://uhl.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://fvp.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tia.ydjk.org.cn

fclose(f);
来源：http://qqq.pycfn.com

[S12] C：写文件
来源：http://mfg.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://evm.yfazqb.com

[S13] C：宏定义
来源：http://egy.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sgh.wangdashe.top

[S14] C：枚举
来源：http://bzk.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://epv.haohaochexian.top

[S15] C：类型转换
来源：http://ywh.dashuyun.cn

(double) a / b
来源：http://aym.andypj.xyz

[S16] C：位操作置位
来源：http://ipe.tian-w.cn

x |= (1 << 3);
来源：http://xnw.epnwcf.com

[S17] C：安全拼接字符串
来源：http://uhn.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kqu.ivvv.top

[S18] C：命令行参数
来源：http://kvt.aibaodan.cn

int main(int argc, char **argv)
来源：http://zdh.bbcook.cn

[S19] C：快速排序
来源：http://jjd.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://suz.hesvh.cn

[S20] C：二分查找
来源：http://wxz.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kcg.tarul.cn

[S21] C：字符类别判断
来源：http://cfi.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ulj.fengsongda.top

[S22] C：字符串转数字
来源：http://yai.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vle.yj20258.top

[S23] C：随机数
来源：http://fnh.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wjf.9152youxi.cn

[S24] C：获取本地时间
来源：http://kld.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bhh.yongpay.top

[S25] C：内存拷贝
来源：http://job.vehdjk.com

memcpy(dst, src, n);
来源：http://xoa.vqdsnc.cn

[S26] C：内存清零
来源：http://joh.ydzc1.top

memset(a, 0, sizeof a);
来源：http://aha.52xcode.cn

[S27] C：定义常量
来源：http://vtp.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://yao.jyoumei.cn

[S28] C：静态变量
来源：http://gzq.jinyuanbaomall.cn

static int counter = 0;
来源：http://mmz.pengpengdd.cyou

[S29] C：变参函数
来源：http://tcd.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ktc.shuidangran.top

[S30] C：头文件保护
来源：http://fgv.haohaochexian.top

#ifndef X_H
来源：http://wet.yj20258888.top

#define X_H
来源：http://tji.shangyingyoupin.top

#endif
来源：http://azc.zdqjudy.top

[S31] C++：Hello World
来源：http://yeu.tanke756.top

#include <iostream>
来源：http://cao.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://cxc.birdmap.top

[S32] C++：字符串
来源：http://vcu.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://ish.zycfv.cn

[S33] C++：vector 增删
来源：http://qiw.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://omn.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://dcb.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://cpi.hywenlv.cn

[S35] C++：map
来源：http://fbk.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmn.xuanzx.com

[S36] C++：unordered_map
来源：http://pup.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://spq.ivvv.top

[S37] C++：set
来源：http://gau.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://avk.cashguo.top

[S38] C++：排序
来源：http://ykx.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://frz.yj20258.top

[S39] C++：自定义比较器排序
来源：http://baf.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tid.cucudq.cn

[S40] C++：查找元素
来源：http://vqk.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qrl.c1oappe.top

[S41] C++：类与构造函数
来源：http://laq.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fri.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://ddt.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://yqo.jqgufenzy.top

[S43] C++：智能指针
来源：http://ppu.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://weo.cucudq.cn

[S44] C++：引用传参
来源：http://mrz.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://tnu.cheryme.top

[S45] C++：lambda
来源：http://fjh.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jqb.uphjek.com

[S46] C++：函数模板
来源：http://wco.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ayc.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://pwp.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://frk.hcnkem.com

[S48] C++：逐行读文件
来源：http://ecy.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zhg.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://jho.vqdsnc.cn

[S49] C++：写文件
来源：http://xpd.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ycb.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://qey.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jla.yueranfly.top

[S51] C++：显式类型转换
来源：http://pmy.hnxiangtu.top

static_cast<double>(a) / b
来源：http://lrm.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://cnb.yj20258.top

int size() const noexcept { return n_; }
来源：http://kzt.52xcode.cn

[S53] C++：移动语义
来源：http://ixx.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://npu.vehdjk.com

[S54] C++：异常处理
来源：http://soj.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ein.nwbrower.top

[S55] C++：结构化绑定
来源：http://lnr.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qhr.ivvv.top

[S56] C++：optional
来源：http://sjl.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cyw.zhijiandao.cn

[S57] C++：编译期常量
来源：http://wcu.gaohongyu789.top

constexpr int N = 10;
来源：http://uet.cqqwz.cn

[S58] C++：命名空间
来源：http://kwb.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://grz.jinqigfzy.top

[S59] C++：静态断言
来源：http://djm.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zzg.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://zzy.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tqa.hfpthk.cn

================================================================================
来源：http://wop.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqx.bbcook.cn

================================================================================
来源：http://yzy.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://vjr.xinyue.icu

println("Hello")
来源：http://bzp.wangdashe.top

[T02] Kotlin：变量
来源：http://ocb.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://evj.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://rjo.jinqigfzy.top

"值: $b"
来源：http://jio.aizwys.cn

[T04] Kotlin：空安全
来源：http://lyl.hesvh.cn

val n: String? = null;  n?.length
来源：http://hfb.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://qeb.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dgp.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://mfc.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vma.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://jwy.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fhs.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://kws.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://hkt.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://aok.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://xmn.cashguo.top

[T10] Kotlin：默认参数
来源：http://aih.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gnc.ctjpmb.com

[T11] Kotlin：协程
来源：http://opk.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://usx.fengsongda.top

[T12] Kotlin：解构声明
来源：http://gys.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://zdk.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://pxu.shuidangran.top

val m = mapOf("a" to 1)
来源：http://wum.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://vvm.yj202588.top

for (i in 1..10) println(i)
来源：http://voj.epnwcf.com

[T15] Kotlin：接口
来源：http://amv.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://uot.dianchejie.cn

[T16] Swift：Hello World
来源：http://epx.yanxiufei.cn

print("Hello")
来源：http://hxu.9152youxi.cn

[T17] Swift：变量与常量
来源：http://wyw.jlsjyb.cn

var a = 1;  let b = 2
来源：http://okn.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://jnr.shanyushiyangkeji.top

"值: \(b)"
来源：http://ydp.epnwcf.com

[T19] Swift：可选绑定
来源：http://kax.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://cmo.vqdsnc.cn

[T20] Swift：数组操作
来源：http://uji.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://gtd.zhongyouzk.top

[T21] Swift：遍历
来源：http://fhl.nwbrower.top

for x in a { print(x) }
来源：http://qol.hnqzz.top

[T22] Swift：字典
来源：http://jbc.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://feh.ctjpmb.com


<!-- 参考信息 -->