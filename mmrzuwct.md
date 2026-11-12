代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://crv.ivvv.top

[R16] until 等待条件
来源：http://mxl.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ojj.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://rqa.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pgm.nanxuanxn.top

[R18] 遍历数组
来源：http://afv.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rjl.cqqwz.cn

[R19] 数组长度
来源：http://hdg.xuanzx.com

echo "${#arr[@]}"
来源：http://yfj.cashguo.top

[R20] 关联数组（字典）
来源：http://uep.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gxm.xziqi.cn

[R21] 字符串长度
来源：http://jma.iojbl.cn

echo "${#s}"
来源：http://zlq.fehbvm.com

[R22] 截取子串
来源：http://abg.pycfn.com

echo "${s:0:5}"
来源：http://qdt.hfpthk.cn

[R23] 字符串替换
来源：http://ltr.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fam.jinghuilouyu.cn

[R24] 大小写转换
来源：http://gha.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://dwv.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://git.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gum.shanyushiyangkeji.top

[R26] 命令替换
来源：http://omd.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://evg.guowangkeji.top

[R27] 算术展开
来源：http://blx.ivvv.top

echo $((1 + 2 * 3))
来源：http://baf.ctjpmb.com

[R28] 浮点运算
来源：http://nvh.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://xng.pengpengdd.cyou

[R29] 定义函数
来源：http://erd.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpg.jinqigfzy.top

[R30] 函数返回状态码
来源：http://kky.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://nci.ppjwa.cn

[R31] 局部变量
来源：http://slw.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://gpn.sweek.top

[R32] 参数个数校验
来源：http://kxv.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://krd.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://osk.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qcr.sweek.top

[R34] 退出时清理
来源：http://kkj.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://ngn.cucudq.cn

[R35] 后台执行并等待
来源：http://mqm.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://elf.yueranfly.top

[R36] 并发执行多个任务
来源：http://sjf.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mta.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://rhb.zycfv.cn

files=$(ls -1)
来源：http://hwo.shangyingyoupin.top

[R38] 管道串联
来源：http://fye.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://gvx.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://umd.bbcook.cn

cmd > out.log 2>&1
来源：http://vlx.yanxiufei.cn

[R40] 追加写日志
来源：http://gzh.hywenlv.cn

echo "log" >> out.log
来源：http://mdk.yueranfly.top

[R41] 丢弃输出
来源：http://thi.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://rzv.kuanghao11.cn

[R42] 输入重定向
来源：http://mlj.jyoumei.cn

wc -l < a.txt
来源：http://wqv.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://nme.xinyue.icu

find . -name "*.log" -type f
来源：http://szq.fengsongda.top

[R44] 按修改时间查找
来源：http://tlt.shuidangran.top

find . -mtime -7 -type f
来源：http://oms.hcnkem.com

[R45] 批量删除
来源：http://uzh.smart0.xyz

find . -name "*.tmp" -delete
来源：http://urd.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://pjr.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://knz.xinyue.icu

[R47] sed 单行替换
来源：http://wlm.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sgu.gaohongyu789.top

[R48] awk 取指定列
来源：http://wsc.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://str.sjlbkw.cn

[R49] awk 带条件
来源：http://lcf.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://plx.yanxiufei.cn

[R50] awk 求和
来源：http://uor.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://igr.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://wau.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://smq.pengpengdd.cyou

[R52] 统计行数
来源：http://ygw.epnwcf.com

wc -l a.txt
来源：http://tpx.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://osm.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gpl.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://xln.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://xpr.tian-w.cn

[R55] 压缩与解压
来源：http://mmj.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pme.bjfxy.top

[R56] 远程拷贝
来源：http://gut.shangyingyoupin.top

scp file user@host:/path/
来源：http://ide.sufxvd.cn

[R57] 远程执行命令
来源：http://ixy.haohaochexian.top

ssh user@host 'uptime'
来源：http://rvg.dashuyun.cn

[R58] 下载文件
来源：http://arl.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rjr.quarkkingdee.top

[R59] 发 POST JSON
来源：http://uzl.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://njs.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://pbg.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://avm.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://bov.zdqjudy.top

df -h;  du -sh *
来源：http://geu.meibo888.top

[R62] 找最占空间的文件
来源：http://yyi.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://tkd.kuanghao11.cn

[R63] 内存与进程
来源：http://xxy.uphjek.com

free -h;  ps aux | grep nginx
来源：http://mjf.zdqjudy.top

[R64] 结束进程
来源：http://fyf.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://krd.cucudq.cn

[R65] 查看端口占用
来源：http://mxq.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://upb.zhixingplan.top

[R66] 定时任务
来源：http://mnn.xinyue.icu

crontab -e;  crontab -l
来源：http://dnk.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://iva.fzhhl.top

openssl rand -hex 16
来源：http://slk.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://sfb.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xpn.bbcook.cn

[R69] 生成随机密码
来源：http://mpc.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://ifq.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://upk.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://mda.fktsv.cn

[R71] 日期格式化
来源：http://xka.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ovy.iojbl.cn

[R72] 等待端口就绪
来源：http://byp.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pbk.hnqzz.top

[R73] 分割大日志
来源：http://yzx.smart0.xyz

split -l 1000 big.log part_
来源：http://jzw.hywenlv.cn

[R74] 批量重命名
来源：http://mvy.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mrt.epnwcf.com

[R75] 导出环境变量
来源：http://rxl.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://jdy.yongpay.top

[R76] 使用临时文件
来源：http://cah.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vth.jqgufenzy.top

[R77] 读取用户输入
来源：http://qoj.sysykeji.top

read -rp "请输入: " ans
来源：http://pkf.hcnkem.com

[R78] 交互式菜单
来源：http://qqv.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pnv.zhoulong.xyz

[R79] 解析命令行选项
来源：http://twa.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vzj.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://bnb.havefunace.top

time ./run.sh
来源：http://adz.guannengcc.top

================================================================================
来源：http://qtz.chenjidiqi.icu

S. C / C++ 专题
来源：http://ura.yvedp.cn

================================================================================
来源：http://wrs.fengsongda.top

[S01] C：Hello World
来源：http://doi.aizwys.cn

#include <stdio.h>
来源：http://xqu.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://beb.bjfxy.top

[S02] C：变量与格式化输出
来源：http://bld.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://ngs.52xcode.cn

[S03] C：读入整数
来源：http://bah.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://zbm.zdbjq.cn

[S04] C：字符串复制
来源：http://xts.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://mxa.tanke756.top

[S05] C：字符串长度
来源：http://isa.meibo888.top

strlen(s)
来源：http://hfm.zhiwuduotai.top

[S06] C：字符串比较
来源：http://vgt.xziqi.cn

strcmp(a, b) == 0
来源：http://cci.jyoumei.cn

[S07] C：数组遍历求和
来源：http://cak.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tbk.birdmap.top

[S08] C：动态内存分配与释放
来源：http://ogo.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tgj.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://yig.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dag.uphjek.com

[S10] C：指针与解引用
来源：http://acl.c1oappe.top

int *p = &a;  *p = 5;
来源：http://ggu.daxiang520.top

[S11] C：逐行读文件
来源：http://bfv.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://iwk.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wou.guannengcc.top

fclose(f);
来源：http://fcj.shzxlz.cn

[S12] C：写文件
来源：http://iem.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ivj.cucudq.cn

[S13] C：宏定义
来源：http://wor.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jqt.tanke756.top

[S14] C：枚举
来源：http://tpu.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://daw.zycfv.cn

[S15] C：类型转换
来源：http://qqd.hysaishi.cn

(double) a / b
来源：http://agz.uphjek.com

[S16] C：位操作置位
来源：http://kit.jiagoushi.top

x |= (1 << 3);
来源：http://tcm.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://zth.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tmp.snrcjt.cn

[S18] C：命令行参数
来源：http://hhn.smart0.xyz

int main(int argc, char **argv)
来源：http://jcr.gogol.net.cn

[S19] C：快速排序
来源：http://ylg.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://ioj.tian-w.cn

[S20] C：二分查找
来源：http://wxc.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pwa.cdnleiting.top

[S21] C：字符类别判断
来源：http://rsh.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bsp.jqgufenzy.top

[S22] C：字符串转数字
来源：http://aqo.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aql.fehbvm.com

[S23] C：随机数
来源：http://lip.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gcd.fzhhl.top

[S24] C：获取本地时间
来源：http://oic.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yjk.iojbl.cn

[S25] C：内存拷贝
来源：http://snc.hysaishi.cn

memcpy(dst, src, n);
来源：http://xdh.nwbrower.top

[S26] C：内存清零
来源：http://lxk.tian-w.cn

memset(a, 0, sizeof a);
来源：http://uyx.jlsjyb.cn

[S27] C：定义常量
来源：http://ray.daria6918.cn

const double PI = 3.14159;
来源：http://jqj.jinghuilouyu.cn

[S28] C：静态变量
来源：http://zos.sxryk.cn

static int counter = 0;
来源：http://zmi.ehwqpu.com

[S29] C：变参函数
来源：http://gbg.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hpz.hnxiangtu.top

[S30] C：头文件保护
来源：http://mtc.jqgufenzy.top

#ifndef X_H
来源：http://qux.mhx1999.top

#define X_H
来源：http://ely.yj20258.top

#endif
来源：http://sjo.ppjwa.cn

[S31] C++：Hello World
来源：http://reo.daria6918.cn

#include <iostream>
来源：http://xdt.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://cyl.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://hfw.tanke756.top

std::string s = "hi";  s += "!";
来源：http://clz.sysykeji.top

[S33] C++：vector 增删
来源：http://mlv.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukk.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://gbs.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://gcq.ctjpmb.com

[S35] C++：map
来源：http://ieq.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wyr.ydzc1.top

[S36] C++：unordered_map
来源：http://zvg.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://btn.chenjidiqi.icu

[S37] C++：set
来源：http://poh.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wdt.guowangkeji.top

[S38] C++：排序
来源：http://hji.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://vbv.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://cqt.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zov.c1oappe.top

[S40] C++：查找元素
来源：http://fic.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oft.shuidangran.top

[S41] C++：类与构造函数
来源：http://thw.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://osn.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://eno.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://vkh.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://mhm.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://wjp.hnqzz.top

[S44] C++：引用传参
来源：http://fii.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://fmp.sufxvd.cn

[S45] C++：lambda
来源：http://pbp.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zps.pengpengdd.cyou

[S46] C++：函数模板
来源：http://kep.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xom.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://voq.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgw.ehwqpu.com

[S48] C++：逐行读文件
来源：http://tbk.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://jkx.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://gzs.nanxuanxn.top

[S49] C++：写文件
来源：http://fib.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ggc.yj20258.top

[S50] C++：格式化数字
来源：http://cbv.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ziw.yj20258.top

[S51] C++：显式类型转换
来源：http://lqf.gzhubu.top

static_cast<double>(a) / b
来源：http://wuv.birdmap.top

[S52] C++：const 与 noexcept
来源：http://yrd.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://jrh.redwolf501.top

[S53] C++：移动语义
来源：http://bva.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://qwt.cqqwz.cn

[S54] C++：异常处理
来源：http://ycd.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mwi.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://svr.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ftt.hcnkem.com

[S56] C++：optional
来源：http://fmn.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cam.jqgufenzy.top

[S57] C++：编译期常量
来源：http://xbe.aizwys.cn

constexpr int N = 10;
来源：http://oap.guowangkeji.top

[S58] C++：命名空间
来源：http://gae.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://zps.jlsjyb.cn

[S59] C++：静态断言
来源：http://xoo.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tdy.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://usi.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://erm.aibaodan.cn

================================================================================
来源：http://zlu.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfe.zhaomingkeji.xyz

================================================================================
来源：http://voz.redwolf501.top

[T01] Kotlin：Hello World
来源：http://rmp.9152youxi.cn

println("Hello")
来源：http://iui.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://tzf.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lai.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://mqs.0kj1m.cn

"值: $b"
来源：http://pyq.aibaodan.cn

[T04] Kotlin：空安全
来源：http://qio.mhx1999.top

val n: String? = null;  n?.length
来源：http://ctt.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://eqq.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bfl.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://wsc.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yft.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://vgc.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://upj.zhixingplan.top

[T08] Kotlin：数据类
来源：http://xuq.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://ufe.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://fdw.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://nct.redwolf501.top

[T10] Kotlin：默认参数
来源：http://ioq.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cjd.ppjwa.cn

[T11] Kotlin：协程
来源：http://fqw.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ygg.daxiang520.top

[T12] Kotlin：解构声明
来源：http://ozj.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://rvi.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://uzw.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://qxk.xinyue.icu

[T14] Kotlin：循环
来源：http://aml.fengsongda.top

for (i in 1..10) println(i)
来源：http://seq.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://lpg.fzhhl.top

interface Shape { fun area(): Double }
来源：http://zek.fengsongda.top

[T16] Swift：Hello World
来源：http://vua.shzxlz.cn

print("Hello")
来源：http://zwy.hammf.cn

[T17] Swift：变量与常量
来源：http://gvp.yuxming.cn

var a = 1;  let b = 2
来源：http://olj.uphjek.com

[T18] Swift：字符串插值
来源：http://xbh.quarkkingdee.top

"值: \(b)"
来源：http://jrs.zdqjudy.top


<!-- 参考信息 -->