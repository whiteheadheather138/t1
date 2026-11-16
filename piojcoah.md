代发 wailian999

echo "${#arr[@]}"
来源：http://bon.hywenlv.cn

[R20] 关联数组（字典）
来源：http://nhn.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ozv.hnqzz.top

[R21] 字符串长度
来源：http://dby.jlsjyb.cn

echo "${#s}"
来源：http://sld.snrcjt.cn

[R22] 截取子串
来源：http://jja.cheryme.top

echo "${s:0:5}"
来源：http://wnh.zhengqikj.top

[R23] 字符串替换
来源：http://ilj.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mbk.mhx1999.top

[R24] 大小写转换
来源：http://fpn.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://eyh.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://vqa.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qkd.hammf.cn

[R26] 命令替换
来源：http://zhl.havefunace.top

now=$(date +%F); echo "$now"
来源：http://zoc.dianchejie.cn

[R27] 算术展开
来源：http://otm.xylfe.cn

echo $((1 + 2 * 3))
来源：http://xmw.svipenyu.cn

[R28] 浮点运算
来源：http://oik.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://ywc.hcnkem.com

[R29] 定义函数
来源：http://pur.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ott.wangdashe.top

[R30] 函数返回状态码
来源：http://unr.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://ikd.pycfn.com

[R31] 局部变量
来源：http://mkb.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://rlf.jiagoushi.top

[R32] 参数个数校验
来源：http://dby.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tgi.yj202588.top

[R33] 捕获错误并提示行号
来源：http://mvq.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eck.yvedp.cn

[R34] 退出时清理
来源：http://mwf.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://det.jianghu66.top

[R35] 后台执行并等待
来源：http://tqk.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qgq.nwbrower.top

[R36] 并发执行多个任务
来源：http://pys.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iuw.pycfn.com

[R37] 把输出赋给变量
来源：http://dsl.jqgufenzy.top

files=$(ls -1)
来源：http://jjx.yuxming.cn

[R38] 管道串联
来源：http://wrs.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://kbu.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://knm.havefunace.top

cmd > out.log 2>&1
来源：http://ryi.aibaodan.cn

[R40] 追加写日志
来源：http://llc.sjlbkw.cn

echo "log" >> out.log
来源：http://mpv.aizwys.cn

[R41] 丢弃输出
来源：http://xva.ydzc1.top

cmd >/dev/null 2>&1
来源：http://gyy.tianlin.xyz

[R42] 输入重定向
来源：http://txv.fzhhl.top

wc -l < a.txt
来源：http://prj.zycfv.cn

[R43] 按名字查找文件
来源：http://lfm.gotoacloud.top

find . -name "*.log" -type f
来源：http://qms.yonumen.top

[R44] 按修改时间查找
来源：http://wqd.haohaochexian.top

find . -mtime -7 -type f
来源：http://zrf.xziqi.cn

[R45] 批量删除
来源：http://tpn.fzhhl.top

find . -name "*.tmp" -delete
来源：http://shw.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://apl.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eaq.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://npc.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hdc.ydzc1.top

[R48] awk 取指定列
来源：http://mqi.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://khc.hysaishi.cn

[R49] awk 带条件
来源：http://tkm.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fwc.sxryk.cn

[R50] awk 求和
来源：http://nrm.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://avx.guannengcc.top

[R51] 排序去重取前几
来源：http://qar.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://brv.pengpengdd.cyou

[R52] 统计行数
来源：http://ivp.yvedp.cn

wc -l a.txt
来源：http://unb.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://uir.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://umj.fzhhl.top

[R54] 比较两个文件
来源：http://sgh.shuidangran.top

diff a.txt b.txt
来源：http://sde.mhx1999.top

[R55] 压缩与解压
来源：http://kvk.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sok.sxryk.cn

[R56] 远程拷贝
来源：http://mky.yangfankeji.com

scp file user@host:/path/
来源：http://reu.xuanzx.com

[R57] 远程执行命令
来源：http://lun.yfazqb.com

ssh user@host 'uptime'
来源：http://dtc.yanxiufei.cn

[R58] 下载文件
来源：http://xrg.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://phb.zhongyouzk.top

[R59] 发 POST JSON
来源：http://gwc.haohaochexian.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fcv.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://bjz.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hyt.zhijiandao.cn

[R61] 磁盘占用
来源：http://nae.gogol.net.cn

df -h;  du -sh *
来源：http://gun.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://yqa.birdmap.top

du -ah . | sort -rh | head -10
来源：http://xor.9152youxi.cn

[R63] 内存与进程
来源：http://okx.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://pqj.hongshengwenyu.top

[R64] 结束进程
来源：http://trf.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://pmi.yuanzhike.top

[R65] 查看端口占用
来源：http://onc.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yct.shangyingyoupin.top

[R66] 定时任务
来源：http://xqc.316326.xyz

crontab -e;  crontab -l
来源：http://tdp.yj20258.top

[R67] 生成随机十六进制串
来源：http://txj.cucudq.cn

openssl rand -hex 16
来源：http://wpk.jqgfzy.top

[R68] 计算文件校验值
来源：http://jfz.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://khu.ehwqpu.com

[R69] 生成随机密码
来源：http://jxm.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://nvv.dashuyun.cn

[R70] 时间戳与互转
来源：http://rzc.yuxming.cn

date +%s;  date -d @1700000000
来源：http://bbo.c1oappe.top

[R71] 日期格式化
来源：http://ogj.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hbh.daxiang520.top

[R72] 等待端口就绪
来源：http://btr.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zaf.sjlbkw.cn

[R73] 分割大日志
来源：http://jxs.yueranfly.top

split -l 1000 big.log part_
来源：http://gws.cqqwz.cn

[R74] 批量重命名
来源：http://oxj.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pny.316326.xyz

[R75] 导出环境变量
来源：http://sbx.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://qad.jqgufenzy.top

[R76] 使用临时文件
来源：http://lnu.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://spq.zdqjudy.top

[R77] 读取用户输入
来源：http://zeg.cheryme.top

read -rp "请输入: " ans
来源：http://wqn.hongshengwenyu.top

[R78] 交互式菜单
来源：http://bvk.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://xlr.yonumen.top

[R79] 解析命令行选项
来源：http://wyl.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cfw.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://trt.ydzc1.top

time ./run.sh
来源：http://gje.pengpengdd.cyou

================================================================================
来源：http://aja.shzxlz.cn

S. C / C++ 专题
来源：http://yvk.ybcxt.top

================================================================================
来源：http://phf.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://efj.sweek.top

#include <stdio.h>
来源：http://pvy.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kjr.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://tlt.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://pwv.gotoacloud.top

[S03] C：读入整数
来源：http://ggl.9152youxi.cn

int x; scanf("%d", &x);
来源：http://adx.gzhubu.top

[S04] C：字符串复制
来源：http://qof.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://yeb.zhiwuduotai.top

[S05] C：字符串长度
来源：http://oft.bjfxy.top

strlen(s)
来源：http://ytj.dianchejie.cn

[S06] C：字符串比较
来源：http://pfs.nwbrower.top

strcmp(a, b) == 0
来源：http://zwj.vehdjk.com

[S07] C：数组遍历求和
来源：http://pam.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hvs.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://vuc.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xrj.yonumen.top

[S09] C：结构体定义与初始化
来源：http://rit.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bmk.havefunace.top

[S10] C：指针与解引用
来源：http://ccn.daxiang520.top

int *p = &a;  *p = 5;
来源：http://xmv.dianchejie.cn

[S11] C：逐行读文件
来源：http://uty.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://imv.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eko.yj20258.top

fclose(f);
来源：http://qlu.sysykeji.top

[S12] C：写文件
来源：http://qcn.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://etd.guowangkeji.top

[S13] C：宏定义
来源：http://erz.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jsf.hysaishi.cn

[S14] C：枚举
来源：http://rkq.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://qwz.ydjk.org.cn

[S15] C：类型转换
来源：http://naf.quarkkingdee.top

(double) a / b
来源：http://zko.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://bfh.feifeiyinyue.top

x |= (1 << 3);
来源：http://roc.ybcxt.top

[S17] C：安全拼接字符串
来源：http://iii.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://krg.zhiwuduotai.top

[S18] C：命令行参数
来源：http://dte.9152youxi.cn

int main(int argc, char **argv)
来源：http://hno.chenlongwang.top

[S19] C：快速排序
来源：http://zmb.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://bfc.gaohongyu789.top

[S20] C：二分查找
来源：http://qik.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xzf.52xcode.cn

[S21] C：字符类别判断
来源：http://yid.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ekh.nwbrower.top

[S22] C：字符串转数字
来源：http://icv.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://oim.svipenyu.cn

[S23] C：随机数
来源：http://aih.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hzc.guannengcc.top

[S24] C：获取本地时间
来源：http://ewn.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cmb.ctjpmb.com

[S25] C：内存拷贝
来源：http://onf.chenzaomai.com

memcpy(dst, src, n);
来源：http://qdj.cqqwz.cn

[S26] C：内存清零
来源：http://jvc.bjfxy.top

memset(a, 0, sizeof a);
来源：http://yey.shzxlz.cn

[S27] C：定义常量
来源：http://kht.cheryme.top

const double PI = 3.14159;
来源：http://cnv.guannengcc.top

[S28] C：静态变量
来源：http://fzh.hnqzz.top

static int counter = 0;
来源：http://zmr.daria6918.cn

[S29] C：变参函数
来源：http://arw.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mie.yj20258.top

[S30] C：头文件保护
来源：http://xui.hesvh.cn

#ifndef X_H
来源：http://tiu.fzhhl.top

#define X_H
来源：http://bus.hammf.cn

#endif
来源：http://fjy.mhx1999.top

[S31] C++：Hello World
来源：http://ndw.yueranfly.top

#include <iostream>
来源：http://oon.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://pgp.jlsjyb.cn

[S32] C++：字符串
来源：http://luq.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://eek.jqgfzy.top

[S33] C++：vector 增删
来源：http://ciw.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://esr.jinqigufen.top

[S34] C++：遍历 vector
来源：http://vpg.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://yct.jyoumei.cn

[S35] C++：map
来源：http://cyg.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pha.yongpay.top

[S36] C++：unordered_map
来源：http://rfp.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wxe.wangshuangyany.cn

[S37] C++：set
来源：http://snm.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tkv.jinyuanbaomall.cn

[S38] C++：排序
来源：http://vfe.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://fdn.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://tmw.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cxk.shuidangran.top

[S40] C++：查找元素
来源：http://fld.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avv.ybcxt.top

[S41] C++：类与构造函数
来源：http://ejh.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wki.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://mdf.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://qiq.jianghu66.top

[S43] C++：智能指针
来源：http://svr.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://grq.fzhhl.top

[S44] C++：引用传参
来源：http://ubg.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://fgg.hysaishi.cn

[S45] C++：lambda
来源：http://vys.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://cah.kuanghao11.cn

[S46] C++：函数模板
来源：http://cxm.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uya.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://uxo.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fkj.shzxlz.cn

[S48] C++：逐行读文件
来源：http://rkk.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ejj.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://kgv.haohaochexian.top

[S49] C++：写文件
来源：http://arn.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oss.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://mmh.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ytw.52xcode.cn

[S51] C++：显式类型转换
来源：http://neh.tianlin.xyz

static_cast<double>(a) / b
来源：http://mxf.birdmap.top

[S52] C++：const 与 noexcept
来源：http://har.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://tia.ppjwa.cn

[S53] C++：移动语义
来源：http://sco.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://vfp.jinqigfzy.top

[S54] C++：异常处理
来源：http://cjy.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ahc.yj202588.top

[S55] C++：结构化绑定
来源：http://xog.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://xit.zhoulong.xyz

[S56] C++：optional
来源：http://ucs.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pnm.yuxming.cn

[S57] C++：编译期常量
来源：http://chk.iojbl.cn

constexpr int N = 10;
来源：http://hln.yj20258888.top

[S58] C++：命名空间
来源：http://exk.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://rvn.9152youxi.cn

[S59] C++：静态断言
来源：http://smn.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dit.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://fti.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pzu.yongpay.top

================================================================================
来源：http://wvm.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://psc.smart0.xyz

================================================================================
来源：http://dye.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://yof.xingfuxueyuan.xyz

println("Hello")
来源：http://pzi.yj20258.top

[T02] Kotlin：变量
来源：http://pjn.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jts.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://yot.gaohongyu789.top

"值: $b"
来源：http://suo.aizwys.cn

[T04] Kotlin：空安全
来源：http://ihh.birdmap.top

val n: String? = null;  n?.length
来源：http://iie.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://ukc.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xeb.smart0.xyz

[T06] Kotlin：集合映射
来源：http://eee.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ruq.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://nai.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ekq.yj20258.top

[T08] Kotlin：数据类
来源：http://ycz.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://qkz.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://anm.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://wzu.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://gnh.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tay.hfpthk.cn

[T11] Kotlin：协程
来源：http://cdo.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mqp.cheryme.top

[T12] Kotlin：解构声明
来源：http://osu.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://oep.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://dfe.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://xte.daria6918.cn

[T14] Kotlin：循环
来源：http://ysr.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://csy.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://qtw.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://nlw.yuanzhike.top

[T16] Swift：Hello World
来源：http://jhy.gotoacloud.top

print("Hello")
来源：http://moh.ppjwa.cn

[T17] Swift：变量与常量
来源：http://avy.meibo888.top

var a = 1;  let b = 2
来源：http://szz.iojbl.cn

[T18] Swift：字符串插值
来源：http://wxl.hywenlv.cn

"值: \(b)"
来源：http://cne.mhx1999.top

[T19] Swift：可选绑定
来源：http://oui.yuxming.cn

if let n = opt { print(n) }
来源：http://hvq.yangfankeji.com

[T20] Swift：数组操作
来源：http://nxd.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://mbi.hesvh.cn

[T21] Swift：遍历
来源：http://tqc.jqgufenzy.top

for x in a { print(x) }
来源：http://wqn.aizwys.cn

[T22] Swift：字典
来源：http://ock.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lsb.tian-w.cn


<!-- 参考信息 -->