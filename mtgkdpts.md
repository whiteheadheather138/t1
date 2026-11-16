代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqs.nanxinkj.top

[R16] until 等待条件
来源：http://ggc.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://syg.havefunace.top

[R17] 数组定义与取值
来源：http://qal.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://lgj.pengpengdd.cyou

[R18] 遍历数组
来源：http://mnq.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vla.shangyingyoupin.top

[R19] 数组长度
来源：http://pjb.zdqjudy.top

echo "${#arr[@]}"
来源：http://etn.fengsongda.top

[R20] 关联数组（字典）
来源：http://gtd.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vej.ivvv.top

[R21] 字符串长度
来源：http://vqc.quarkkingdee.top

echo "${#s}"
来源：http://ecp.gzhubu.top

[R22] 截取子串
来源：http://yty.feifeiyinyue.top

echo "${s:0:5}"
来源：http://hlj.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://cdh.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://klc.uphjek.com

[R24] 大小写转换
来源：http://ttd.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dpp.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://aja.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://woh.gaohongyu789.top

[R26] 命令替换
来源：http://rbs.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://wcs.chenlongwang.top

[R27] 算术展开
来源：http://fqw.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://zit.bjfxy.top

[R28] 浮点运算
来源：http://kyb.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://oez.hcnkem.com

[R29] 定义函数
来源：http://zam.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uim.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://ilp.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://wjm.hcnkem.com

[R31] 局部变量
来源：http://rak.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://ixr.hysaishi.cn

[R32] 参数个数校验
来源：http://jie.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://suu.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://ehe.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jnw.hammf.cn

[R34] 退出时清理
来源：http://qlw.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pfq.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://bfk.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://nqt.iojbl.cn

[R36] 并发执行多个任务
来源：http://yck.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nys.chenlongwang.top

[R37] 把输出赋给变量
来源：http://myr.yuxming.cn

files=$(ls -1)
来源：http://pfd.tarul.cn

[R38] 管道串联
来源：http://oor.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://rkh.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://izc.tanke756.top

cmd > out.log 2>&1
来源：http://xnr.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://ici.fktsv.cn

echo "log" >> out.log
来源：http://xxx.fengsongda.top

[R41] 丢弃输出
来源：http://hgz.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://dwn.yongpay.top

[R42] 输入重定向
来源：http://jgo.fzhhl.top

wc -l < a.txt
来源：http://dcw.fktsv.cn

[R43] 按名字查找文件
来源：http://lba.dianchejie.cn

find . -name "*.log" -type f
来源：http://wol.sufxvd.cn

[R44] 按修改时间查找
来源：http://bkc.jqgfzy.top

find . -mtime -7 -type f
来源：http://cza.sysykeji.top

[R45] 批量删除
来源：http://qby.xuanzx.com

find . -name "*.tmp" -delete
来源：http://eah.haohaochexian.top

[R46] 递归替换文件内容
来源：http://gdr.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cbz.snrcjt.cn

[R47] sed 单行替换
来源：http://ika.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://may.svipenyu.cn

[R48] awk 取指定列
来源：http://wsq.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://zmh.nanxuanxn.top

[R49] awk 带条件
来源：http://btw.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qin.xziqi.cn

[R50] awk 求和
来源：http://ouc.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gcs.birdmap.top

[R51] 排序去重取前几
来源：http://vdn.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wxy.jiagoushi.top

[R52] 统计行数
来源：http://pdh.chenlongwang.top

wc -l a.txt
来源：http://erf.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://kfn.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxb.ehwqpu.com

[R54] 比较两个文件
来源：http://gdu.fzhhl.top

diff a.txt b.txt
来源：http://mhb.yuxming.cn

[R55] 压缩与解压
来源：http://njy.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lqf.smart0.xyz

[R56] 远程拷贝
来源：http://ryn.tianlin.xyz

scp file user@host:/path/
来源：http://gji.jqgufenzy.top

[R57] 远程执行命令
来源：http://bzd.jinqigfzy.top

ssh user@host 'uptime'
来源：http://eyk.dianchejie.cn

[R58] 下载文件
来源：http://hqx.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lmo.fktsv.cn

[R59] 发 POST JSON
来源：http://xyq.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://udj.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://wpa.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://whs.smart0.xyz

[R61] 磁盘占用
来源：http://maz.chenlongwang.top

df -h;  du -sh *
来源：http://vvg.yuxming.cn

[R62] 找最占空间的文件
来源：http://eio.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://lov.gzhubu.top

[R63] 内存与进程
来源：http://oqv.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://nuw.birdmap.top

[R64] 结束进程
来源：http://dto.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://mlz.smart0.xyz

[R65] 查看端口占用
来源：http://wgx.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oic.quarkkingdee.top

[R66] 定时任务
来源：http://zsz.fehbvm.com

crontab -e;  crontab -l
来源：http://oxf.gzhubu.top

[R67] 生成随机十六进制串
来源：http://uhj.gzhubu.top

openssl rand -hex 16
来源：http://aei.hnqzz.top

[R68] 计算文件校验值
来源：http://jub.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yev.fzhhl.top

[R69] 生成随机密码
来源：http://vit.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://pae.tanke756.top

[R70] 时间戳与互转
来源：http://hny.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://vbr.aizwys.cn

[R71] 日期格式化
来源：http://fhb.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://thf.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://buo.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zdp.dashuyun.cn

[R73] 分割大日志
来源：http://ezp.tanke756.top

split -l 1000 big.log part_
来源：http://qmv.hammf.cn

[R74] 批量重命名
来源：http://sqo.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://prd.52xcode.cn

[R75] 导出环境变量
来源：http://qdf.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://kfx.zhixingplan.top

[R76] 使用临时文件
来源：http://fek.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://scx.yuxming.cn

[R77] 读取用户输入
来源：http://fkb.yuanzhike.top

read -rp "请输入: " ans
来源：http://ebz.guowangkeji.top

[R78] 交互式菜单
来源：http://xjp.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rbv.yfazqb.com

[R79] 解析命令行选项
来源：http://xze.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://icp.birdmap.top

[R80] 查看脚本执行耗时
来源：http://ziq.cashguo.top

time ./run.sh
来源：http://jla.smart0.xyz

================================================================================
来源：http://qww.52xcode.cn

S. C / C++ 专题
来源：http://eyn.cqqwz.cn

================================================================================
来源：http://igh.sweek.top

[S01] C：Hello World
来源：http://axp.yj20258.top

#include <stdio.h>
来源：http://ajp.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rxc.gzhubu.top

[S02] C：变量与格式化输出
来源：http://jzk.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://lzs.sysykeji.top

[S03] C：读入整数
来源：http://wgz.ctjpmb.com

int x; scanf("%d", &x);
来源：http://jtt.quarkkingdee.top

[S04] C：字符串复制
来源：http://ina.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://wdd.xziqi.cn

[S05] C：字符串长度
来源：http://rgk.shzxlz.cn

strlen(s)
来源：http://fsx.yueranfly.top

[S06] C：字符串比较
来源：http://vev.gzhubu.top

strcmp(a, b) == 0
来源：http://zvs.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://woa.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://otw.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://zff.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rsy.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://kox.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzb.yanxiufei.cn

[S10] C：指针与解引用
来源：http://vlu.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://hyu.pycfn.com

[S11] C：逐行读文件
来源：http://gvc.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://xtc.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://yau.yongpay.top

fclose(f);
来源：http://hzq.zycfv.cn

[S12] C：写文件
来源：http://gjj.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://asm.jinghuilouyu.cn

[S13] C：宏定义
来源：http://wct.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pwz.hnqzz.top

[S14] C：枚举
来源：http://gbt.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://ado.shuidangran.top

[S15] C：类型转换
来源：http://hyq.ydjk.org.cn

(double) a / b
来源：http://lki.birdmap.top

[S16] C：位操作置位
来源：http://rus.52xcode.cn

x |= (1 << 3);
来源：http://rdq.guannengcc.top

[S17] C：安全拼接字符串
来源：http://cmp.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xnn.yuxming.cn

[S18] C：命令行参数
来源：http://zvf.yuxming.cn

int main(int argc, char **argv)
来源：http://sua.sweek.top

[S19] C：快速排序
来源：http://ccr.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://xkx.chenjidiqi.icu

[S20] C：二分查找
来源：http://ixd.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://awf.cucudq.cn

[S21] C：字符类别判断
来源：http://ejr.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fay.fzhhl.top

[S22] C：字符串转数字
来源：http://aby.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://twh.daxiang520.top

[S23] C：随机数
来源：http://liu.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://hda.tian-w.cn

[S24] C：获取本地时间
来源：http://ool.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fpy.ybcxt.top

[S25] C：内存拷贝
来源：http://sxt.chenlongwang.top

memcpy(dst, src, n);
来源：http://lxz.hywenlv.cn

[S26] C：内存清零
来源：http://slz.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://vjl.zdqjudy.top

[S27] C：定义常量
来源：http://qpr.yj202588.top

const double PI = 3.14159;
来源：http://etp.feifeiyinyue.top

[S28] C：静态变量
来源：http://wzy.zdbjq.cn

static int counter = 0;
来源：http://yha.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://ily.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jpp.daria6918.cn

[S30] C：头文件保护
来源：http://ltf.chenjidiqi.icu

#ifndef X_H
来源：http://hjw.bbcook.cn

#define X_H
来源：http://dtn.daria6918.cn

#endif
来源：http://avy.xziqi.cn

[S31] C++：Hello World
来源：http://jjb.zdqjudy.top

#include <iostream>
来源：http://uap.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://ezu.chenjidiqi.icu

[S32] C++：字符串
来源：http://uwz.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://nnf.vqdsnc.cn

[S33] C++：vector 增删
来源：http://syw.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yox.nwbrower.top

[S34] C++：遍历 vector
来源：http://hgb.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://eqa.iojbl.cn

[S35] C++：map
来源：http://jbj.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qxu.smart0.xyz

[S36] C++：unordered_map
来源：http://kzy.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bpk.svipenyu.cn

[S37] C++：set
来源：http://sor.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zyu.guowangkeji.top

[S38] C++：排序
来源：http://mqg.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://ijg.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://jpt.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hjo.yonumen.top

[S40] C++：查找元素
来源：http://nik.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jow.yfazqb.com

[S41] C++：类与构造函数
来源：http://wrk.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sjo.yuxming.cn

[S42] C++：继承与虚函数
来源：http://uon.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://oya.hongshengwenyu.top

[S43] C++：智能指针
来源：http://zvm.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://ruw.hesvh.cn

[S44] C++：引用传参
来源：http://jir.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://qrj.hesvh.cn

[S45] C++：lambda
来源：http://deh.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rqb.sufxvd.cn

[S46] C++：函数模板
来源：http://ihm.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pdx.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://qwf.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ldv.guannengcc.top

[S48] C++：逐行读文件
来源：http://hqi.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://crt.iojbl.cn

while (std::getline(in, line)) { }
来源：http://pyi.yongpay.top

[S49] C++：写文件
来源：http://sks.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dbt.zhengqikj.top

[S50] C++：格式化数字
来源：http://fqr.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gov.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://wgq.jiagoushi.top

static_cast<double>(a) / b
来源：http://vmi.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://ajz.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://pct.yfazqb.com

[S53] C++：移动语义
来源：http://dkp.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://mkx.nanxuanxn.top

[S54] C++：异常处理
来源：http://yha.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dan.birdmap.top

[S55] C++：结构化绑定
来源：http://hyr.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://etg.fktsv.cn

[S56] C++：optional
来源：http://adu.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://asw.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://wgq.haohaochexian.top

constexpr int N = 10;
来源：http://jvp.redwolf501.top

[S58] C++：命名空间
来源：http://kgl.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://gne.andypj.xyz

[S59] C++：静态断言
来源：http://vmy.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://svb.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://nmy.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://puw.cashguo.top

================================================================================
来源：http://vkc.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztz.zhaomingkeji.xyz

================================================================================
来源：http://yqn.xinyue.icu

[T01] Kotlin：Hello World
来源：http://dvu.tanke756.top

println("Hello")
来源：http://hmy.jqgufenzy.top

[T02] Kotlin：变量
来源：http://ypw.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rgz.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://zvn.sjlbkw.cn

"值: $b"
来源：http://wiz.hesvh.cn

[T04] Kotlin：空安全
来源：http://fhs.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://tkq.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://bgh.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nfy.tanke756.top

[T06] Kotlin：集合映射
来源：http://ngn.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zbf.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://tjo.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykz.smart0.xyz

[T08] Kotlin：数据类
来源：http://sem.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://dyo.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://hbs.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://wvw.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://bjn.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://skk.birdmap.top

[T11] Kotlin：协程
来源：http://ucr.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mxj.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://ggk.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://ymw.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://vxm.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://zbe.cdnleiting.top

[T14] Kotlin：循环
来源：http://izy.52xcode.cn

for (i in 1..10) println(i)
来源：http://vum.sufxvd.cn

[T15] Kotlin：接口
来源：http://vuj.xuanzx.com

interface Shape { fun area(): Double }
来源：http://qti.gaohongyu789.top

[T16] Swift：Hello World
来源：http://yim.jianghu66.top

print("Hello")
来源：http://hmi.hesvh.cn

[T17] Swift：变量与常量
来源：http://ltp.hammf.cn

var a = 1;  let b = 2
来源：http://ueu.xylfe.cn

[T18] Swift：字符串插值
来源：http://dvc.0kj1m.cn

"值: \(b)"
来源：http://jwz.xingfuxueyuan.xyz


<!-- 参考信息 -->