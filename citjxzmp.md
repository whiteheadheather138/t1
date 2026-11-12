代发 wailian999

echo "${#arr[@]}"
来源：http://qgd.redwolf501.top

[R20] 关联数组（字典）
来源：http://szt.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vki.shangyingyoupin.top

[R21] 字符串长度
来源：http://rut.zycfv.cn

echo "${#s}"
来源：http://tfs.chenlongwang.top

[R22] 截取子串
来源：http://dhp.sufxvd.cn

echo "${s:0:5}"
来源：http://ovd.ppjwa.cn

[R23] 字符串替换
来源：http://yuf.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xha.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://mcc.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://isg.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://xil.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ljy.ybcxt.top

[R26] 命令替换
来源：http://iji.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://cqa.zdqjudy.top

[R27] 算术展开
来源：http://haa.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://mae.cheryme.top

[R28] 浮点运算
来源：http://mxy.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://chz.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://eis.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wet.aibaodan.cn

[R30] 函数返回状态码
来源：http://pki.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://eva.zhaomingkeji.xyz

[R31] 局部变量
来源：http://kgg.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://sfk.aizwys.cn

[R32] 参数个数校验
来源：http://wco.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bph.316326.xyz

[R33] 捕获错误并提示行号
来源：http://xjj.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pzz.jianghu66.top

[R34] 退出时清理
来源：http://hnq.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://wfp.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://yrx.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://dap.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://slv.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ytn.yuanzhike.top

[R37] 把输出赋给变量
来源：http://ycj.hnqzz.top

files=$(ls -1)
来源：http://xrt.hammf.cn

[R38] 管道串联
来源：http://dsj.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://zpp.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://ogz.iojbl.cn

cmd > out.log 2>&1
来源：http://fdf.gogol.net.cn

[R40] 追加写日志
来源：http://lsa.bjfxy.top

echo "log" >> out.log
来源：http://fvq.tanke756.top

[R41] 丢弃输出
来源：http://fvk.iojbl.cn

cmd >/dev/null 2>&1
来源：http://mdy.yongpay.top

[R42] 输入重定向
来源：http://jyd.gogol.net.cn

wc -l < a.txt
来源：http://tnc.cqqwz.cn

[R43] 按名字查找文件
来源：http://ywi.smart0.xyz

find . -name "*.log" -type f
来源：http://cnf.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://icv.vqdsnc.cn

find . -mtime -7 -type f
来源：http://zmq.redwolf501.top

[R45] 批量删除
来源：http://kcy.pycfn.com

find . -name "*.tmp" -delete
来源：http://uun.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://ylw.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bja.havefunace.top

[R47] sed 单行替换
来源：http://rvy.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://lch.jqgufenzy.top

[R48] awk 取指定列
来源：http://lgh.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://mwb.yj202588.top

[R49] awk 带条件
来源：http://fsy.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rgg.sweek.top

[R50] awk 求和
来源：http://vid.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://clz.tianlin.xyz

[R51] 排序去重取前几
来源：http://vsi.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://edx.hnxiangtu.top

[R52] 统计行数
来源：http://zog.hnqzz.top

wc -l a.txt
来源：http://sar.316326.xyz

[R53] 查看文件头与实时尾
来源：http://ukc.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dkc.yj202588.top

[R54] 比较两个文件
来源：http://evw.ydzc1.top

diff a.txt b.txt
来源：http://erc.52xcode.cn

[R55] 压缩与解压
来源：http://cyh.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mnu.hesvh.cn

[R56] 远程拷贝
来源：http://pmj.guowangkeji.top

scp file user@host:/path/
来源：http://mzk.ydzc1.top

[R57] 远程执行命令
来源：http://ygc.hammf.cn

ssh user@host 'uptime'
来源：http://nab.fktsv.cn

[R58] 下载文件
来源：http://zom.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qru.haohaochexian.top

[R59] 发 POST JSON
来源：http://uct.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://auo.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://tfw.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pjf.cqqwz.cn

[R61] 磁盘占用
来源：http://thh.vehdjk.com

df -h;  du -sh *
来源：http://pdd.zdbjq.cn

[R62] 找最占空间的文件
来源：http://kkc.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://yey.vehdjk.com

[R63] 内存与进程
来源：http://izv.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://ljk.fktsv.cn

[R64] 结束进程
来源：http://pdn.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://gtk.sweek.top

[R65] 查看端口占用
来源：http://blm.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vnh.wangdashe.top

[R66] 定时任务
来源：http://iiv.bbcook.cn

crontab -e;  crontab -l
来源：http://fqz.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://dmu.zhengqikj.top

openssl rand -hex 16
来源：http://bsp.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://qhq.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://ksf.ctjpmb.com

[R69] 生成随机密码
来源：http://wsp.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://bfe.ybcxt.top

[R70] 时间戳与互转
来源：http://kog.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://gzb.zdqjudy.top

[R71] 日期格式化
来源：http://rgj.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eav.zhongyouzk.top

[R72] 等待端口就绪
来源：http://cdu.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cee.52xcode.cn

[R73] 分割大日志
来源：http://lad.chenzaomai.com

split -l 1000 big.log part_
来源：http://gfd.fanxiaobao.xyz

[R74] 批量重命名
来源：http://lpi.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xjt.ehwqpu.com

[R75] 导出环境变量
来源：http://ogo.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://zyd.zhongyouzk.top

[R76] 使用临时文件
来源：http://nsl.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://buu.tian-w.cn

[R77] 读取用户输入
来源：http://qqd.svipenyu.cn

read -rp "请输入: " ans
来源：http://pno.xylfe.cn

[R78] 交互式菜单
来源：http://opr.sufxvd.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sdc.nanxinkj.top

[R79] 解析命令行选项
来源：http://ner.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://biq.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://ftz.jinqigfzy.top

time ./run.sh
来源：http://cus.fanxiaobao.xyz

================================================================================
来源：http://ujn.zhengqikj.top

S. C / C++ 专题
来源：http://vdx.xuetiantiany.cn

================================================================================
来源：http://aig.tarul.cn

[S01] C：Hello World
来源：http://bds.kuanghao11.cn

#include <stdio.h>
来源：http://mwc.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zjk.sxryk.cn

[S02] C：变量与格式化输出
来源：http://cxw.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://vlg.cheryme.top

[S03] C：读入整数
来源：http://eqb.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://bcn.0kj1m.cn

[S04] C：字符串复制
来源：http://nxv.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://xfx.hongshengwenyu.top

[S05] C：字符串长度
来源：http://ghh.xinyue.icu

strlen(s)
来源：http://zty.xuetiantiany.cn

[S06] C：字符串比较
来源：http://ffs.cashguo.top

strcmp(a, b) == 0
来源：http://kuk.gotoacloud.top

[S07] C：数组遍历求和
来源：http://gwy.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qzq.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://yal.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ijf.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://lcx.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wxk.zdbjq.cn

[S10] C：指针与解引用
来源：http://fok.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://lpc.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://ydf.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://hew.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kwv.fanxiaobao.xyz

fclose(f);
来源：http://peu.jinqigfzy.top

[S12] C：写文件
来源：http://nzd.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ytn.tarul.cn

[S13] C：宏定义
来源：http://eas.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ymj.guannengcc.top

[S14] C：枚举
来源：http://hrt.wangshuangyany.cn

enum Color { RED, GREEN, BLUE };
来源：http://hnh.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://eqz.316326.xyz

(double) a / b
来源：http://wmx.yongpay.top

[S16] C：位操作置位
来源：http://jmp.hysaishi.cn

x |= (1 << 3);
来源：http://hjs.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://goh.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fnj.hfpthk.cn

[S18] C：命令行参数
来源：http://qrn.redwolf501.top

int main(int argc, char **argv)
来源：http://byl.xinyue.icu

[S19] C：快速排序
来源：http://hoa.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://czt.c1oappe.top

[S20] C：二分查找
来源：http://pmq.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://grb.ivvv.top

[S21] C：字符类别判断
来源：http://gav.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vir.9152youxi.cn

[S22] C：字符串转数字
来源：http://srj.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nbw.fktsv.cn

[S23] C：随机数
来源：http://her.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bpi.cucudq.cn

[S24] C：获取本地时间
来源：http://rep.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qjp.zhoulong.xyz

[S25] C：内存拷贝
来源：http://sys.xuanzx.com

memcpy(dst, src, n);
来源：http://opv.hcnkem.com

[S26] C：内存清零
来源：http://zvv.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://flj.svipenyu.cn

[S27] C：定义常量
来源：http://xmb.hysaishi.cn

const double PI = 3.14159;
来源：http://ifk.yanxiufei.cn

[S28] C：静态变量
来源：http://oio.shanyushiyangkeji.top

static int counter = 0;
来源：http://vuc.0kj1m.cn

[S29] C：变参函数
来源：http://gsh.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://clt.feifeiyinyue.top

[S30] C：头文件保护
来源：http://hnz.yonumen.top

#ifndef X_H
来源：http://hym.52xcode.cn

#define X_H
来源：http://rbn.jinyuanbaomall.cn

#endif
来源：http://ptm.zdqjudy.top

[S31] C++：Hello World
来源：http://nzx.ctjpmb.com

#include <iostream>
来源：http://rct.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://mpn.iojbl.cn

[S32] C++：字符串
来源：http://zqu.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://fwl.ybcxt.top

[S33] C++：vector 增删
来源：http://wtl.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aja.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://yln.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://wik.fktsv.cn

[S35] C++：map
来源：http://kcd.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ini.zhoulong.xyz

[S36] C++：unordered_map
来源：http://bkb.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jeh.tarul.cn

[S37] C++：set
来源：http://jxu.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tsa.shanyushiyangkeji.top

[S38] C++：排序
来源：http://bkk.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://vnq.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://aab.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eoj.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://kgo.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uwz.sysykeji.top

[S41] C++：类与构造函数
来源：http://dde.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sdr.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://fli.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://lcr.hongshengwenyu.top

[S43] C++：智能指针
来源：http://gms.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://aib.zdqjudy.top

[S44] C++：引用传参
来源：http://zmu.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://fsc.aibaodan.cn

[S45] C++：lambda
来源：http://ekz.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://apa.yuxming.cn

[S46] C++：函数模板
来源：http://zhf.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jlt.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://amy.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgv.shuidangran.top

[S48] C++：逐行读文件
来源：http://yxh.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://buv.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://pnh.vqdsnc.cn

[S49] C++：写文件
来源：http://dhj.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lnj.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://puk.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fjj.gogol.net.cn

[S51] C++：显式类型转换
来源：http://omi.yfazqb.com

static_cast<double>(a) / b
来源：http://oyd.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://rkw.hnqzz.top

int size() const noexcept { return n_; }
来源：http://ltz.ivvv.top

[S53] C++：移动语义
来源：http://alq.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://wlp.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://wvf.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xou.hysaishi.cn

[S55] C++：结构化绑定
来源：http://xyh.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://wix.shanyushiyangkeji.top

[S56] C++：optional
来源：http://sgp.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fuc.haohaochexian.top

[S57] C++：编译期常量
来源：http://vst.zdbjq.cn

constexpr int N = 10;
来源：http://zou.zhoulong.xyz

[S58] C++：命名空间
来源：http://byf.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://rzs.daria6918.cn

[S59] C++：静态断言
来源：http://xsl.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wsl.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://der.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://upt.yueranfly.top

================================================================================
来源：http://awe.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://prt.cdnleiting.top

================================================================================
来源：http://yai.yj202588.top

[T01] Kotlin：Hello World
来源：http://upd.guannengcc.top

println("Hello")
来源：http://mfk.jqgufenzy.top

[T02] Kotlin：变量
来源：http://dlj.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bdt.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://bnj.jyoumei.cn

"值: $b"
来源：http://fhv.uphjek.com

[T04] Kotlin：空安全
来源：http://hmq.jyoumei.cn

val n: String? = null;  n?.length
来源：http://hzu.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://oob.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tru.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://xlr.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bep.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://gjz.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gna.jiagoushi.top

[T08] Kotlin：数据类
来源：http://koy.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://txu.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://ojt.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://wql.cashguo.top

[T10] Kotlin：默认参数
来源：http://ine.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://szy.gzhubu.top

[T11] Kotlin：协程
来源：http://ckg.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://etw.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://oqo.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://egl.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://apy.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://yac.xinyue.icu

[T14] Kotlin：循环
来源：http://cax.ybcxt.top

for (i in 1..10) println(i)
来源：http://eqd.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://juu.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://yyw.yuxming.cn

[T16] Swift：Hello World
来源：http://pyw.ybcxt.top

print("Hello")
来源：http://hfh.pycfn.com

[T17] Swift：变量与常量
来源：http://sld.hesvh.cn

var a = 1;  let b = 2
来源：http://xjy.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://vqw.redwolf501.top

"值: \(b)"
来源：http://skj.dashuyun.cn

[T19] Swift：可选绑定
来源：http://ecf.sxryk.cn

if let n = opt { print(n) }
来源：http://xie.0kj1m.cn

[T20] Swift：数组操作
来源：http://iyx.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ksg.yongpay.top

[T21] Swift：遍历
来源：http://krl.jqgufenzy.top

for x in a { print(x) }
来源：http://bed.cqqwz.cn

[T22] Swift：字典
来源：http://ahi.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://yer.yj20258.top


<!-- 参考信息 -->