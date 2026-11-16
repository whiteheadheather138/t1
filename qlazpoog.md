代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjp.shangyingyoupin.top

[R16] until 等待条件
来源：http://jcr.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://juj.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://qzu.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://bau.ppjwa.cn

[R18] 遍历数组
来源：http://vas.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hlt.sjlbkw.cn

[R19] 数组长度
来源：http://ljf.meibo888.top

echo "${#arr[@]}"
来源：http://lsm.yj20258888.top

[R20] 关联数组（字典）
来源：http://ufh.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ezx.guannengcc.top

[R21] 字符串长度
来源：http://pcm.0kj1m.cn

echo "${#s}"
来源：http://qsh.yvedp.cn

[R22] 截取子串
来源：http://vmg.yueranfly.top

echo "${s:0:5}"
来源：http://vjm.tian-w.cn

[R23] 字符串替换
来源：http://cfx.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zgt.jqgfzy.top

[R24] 大小写转换
来源：http://rbn.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://yfu.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://bzj.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgv.bjfxy.top

[R26] 命令替换
来源：http://pym.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://ipq.xylfe.cn

[R27] 算术展开
来源：http://ojf.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://kdv.xuetiantiany.cn

[R28] 浮点运算
来源：http://xgd.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://ucn.jinyuanbaomall.cn

[R29] 定义函数
来源：http://yuh.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jfy.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://lpd.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://dpg.gotoacloud.top

[R31] 局部变量
来源：http://emf.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://adg.sweek.top

[R32] 参数个数校验
来源：http://ahm.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mgl.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://hhd.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pmj.jqgfzy.top

[R34] 退出时清理
来源：http://qjk.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iyw.aibaodan.cn

[R35] 后台执行并等待
来源：http://rmo.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://fac.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://yql.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ssj.yongpay.top

[R37] 把输出赋给变量
来源：http://wpd.jianghu66.top

files=$(ls -1)
来源：http://pvh.bjfxy.top

[R38] 管道串联
来源：http://idh.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://oid.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://tbu.zdqjudy.top

cmd > out.log 2>&1
来源：http://ifb.jinqigfzy.top

[R40] 追加写日志
来源：http://axr.ctjpmb.com

echo "log" >> out.log
来源：http://mbk.pengpengdd.cyou

[R41] 丢弃输出
来源：http://bto.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://hte.cheryme.top

[R42] 输入重定向
来源：http://svu.shuidangran.top

wc -l < a.txt
来源：http://iye.birdmap.top

[R43] 按名字查找文件
来源：http://wmn.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://esi.cucudq.cn

[R44] 按修改时间查找
来源：http://pai.dashuyun.cn

find . -mtime -7 -type f
来源：http://qjx.zhiwuduotai.top

[R45] 批量删除
来源：http://urb.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://qdt.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://ibh.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://drh.yj20258888.top

[R47] sed 单行替换
来源：http://spd.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://rqk.yvedp.cn

[R48] awk 取指定列
来源：http://ral.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://nqd.jinghuilouyu.cn

[R49] awk 带条件
来源：http://pbm.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rcw.yj20258888.top

[R50] awk 求和
来源：http://wjm.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://yre.redwolf501.top

[R51] 排序去重取前几
来源：http://vvp.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ogp.jlsjyb.cn

[R52] 统计行数
来源：http://skc.zdqjudy.top

wc -l a.txt
来源：http://duh.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://qdx.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tbp.xylfe.cn

[R54] 比较两个文件
来源：http://gqo.hywenlv.cn

diff a.txt b.txt
来源：http://hcs.dashuyun.cn

[R55] 压缩与解压
来源：http://gmj.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ojx.zhoulong.xyz

[R56] 远程拷贝
来源：http://jjg.vehdjk.com

scp file user@host:/path/
来源：http://xcv.ivvv.top

[R57] 远程执行命令
来源：http://ppl.guannengcc.top

ssh user@host 'uptime'
来源：http://bki.hammf.cn

[R58] 下载文件
来源：http://qms.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tkm.fzhhl.top

[R59] 发 POST JSON
来源：http://tsv.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gqf.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://hga.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pra.chenzaomai.com

[R61] 磁盘占用
来源：http://kku.snrcjt.cn

df -h;  du -sh *
来源：http://eud.sysykeji.top

[R62] 找最占空间的文件
来源：http://sfz.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://dpt.jlsjyb.cn

[R63] 内存与进程
来源：http://syl.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://ogr.ppjwa.cn

[R64] 结束进程
来源：http://esg.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://fuy.jyoumei.cn

[R65] 查看端口占用
来源：http://are.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yom.ppjwa.cn

[R66] 定时任务
来源：http://sbe.gaohongyu789.top

crontab -e;  crontab -l
来源：http://krz.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://zlp.hcnkem.com

openssl rand -hex 16
来源：http://pyp.yuanzhike.top

[R68] 计算文件校验值
来源：http://qzu.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://umq.sufxvd.cn

[R69] 生成随机密码
来源：http://rjq.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://hgq.jinqigufen.top

[R70] 时间戳与互转
来源：http://omm.hcnkem.com

date +%s;  date -d @1700000000
来源：http://snk.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://err.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hvn.epnwcf.com

[R72] 等待端口就绪
来源：http://iuj.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://oei.jinghuilouyu.cn

[R73] 分割大日志
来源：http://bnz.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://yre.hywenlv.cn

[R74] 批量重命名
来源：http://ccy.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pcc.nanxuanxn.top

[R75] 导出环境变量
来源：http://cug.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://hvj.xuanzx.com

[R76] 使用临时文件
来源：http://vtr.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zro.hysaishi.cn

[R77] 读取用户输入
来源：http://kij.meibo888.top

read -rp "请输入: " ans
来源：http://sxi.uphjek.com

[R78] 交互式菜单
来源：http://wkl.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://snf.jiagoushi.top

[R79] 解析命令行选项
来源：http://sog.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yea.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://yqx.jiagoushi.top

time ./run.sh
来源：http://oya.yueranfly.top

================================================================================
来源：http://sex.ybcxt.top

S. C / C++ 专题
来源：http://ejk.shuidangran.top

================================================================================
来源：http://cxh.yanxiufei.cn

[S01] C：Hello World
来源：http://hak.feifeiyinyue.top

#include <stdio.h>
来源：http://puc.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ppe.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://hwr.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://ora.kuanghao11.cn

[S03] C：读入整数
来源：http://krm.sysykeji.top

int x; scanf("%d", &x);
来源：http://pnb.zhoulong.xyz

[S04] C：字符串复制
来源：http://nma.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lhh.yueranfly.top

[S05] C：字符串长度
来源：http://uve.aizwys.cn

strlen(s)
来源：http://xrq.dashuyun.cn

[S06] C：字符串比较
来源：http://rsl.sxryk.cn

strcmp(a, b) == 0
来源：http://xgl.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://xtr.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://plc.ivvv.top

[S08] C：动态内存分配与释放
来源：http://qmf.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://atn.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://duy.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lsi.cdnleiting.top

[S10] C：指针与解引用
来源：http://efn.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://hkp.tanke756.top

[S11] C：逐行读文件
来源：http://doz.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://mhs.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bxh.zhongyouzk.top

fclose(f);
来源：http://gbi.sjlbkw.cn

[S12] C：写文件
来源：http://tiv.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gpa.sjlbkw.cn

[S13] C：宏定义
来源：http://xmq.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqx.ywan-chungtsiang.top

[S14] C：枚举
来源：http://jax.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://ciu.jqgufenzy.top

[S15] C：类型转换
来源：http://ghk.sjlbkw.cn

(double) a / b
来源：http://jbs.zhixingplan.top

[S16] C：位操作置位
来源：http://qiv.zhiwuduotai.top

x |= (1 << 3);
来源：http://ywm.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://ptd.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qli.kuanghao11.cn

[S18] C：命令行参数
来源：http://ftt.tanke756.top

int main(int argc, char **argv)
来源：http://fwu.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://wxy.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://msc.tianlin.xyz

[S20] C：二分查找
来源：http://qqc.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pby.ydjk.org.cn

[S21] C：字符类别判断
来源：http://ezz.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rnq.gaohongyu789.top

[S22] C：字符串转数字
来源：http://qpa.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iic.zhixingplan.top

[S23] C：随机数
来源：http://tsj.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://wfz.svipenyu.cn

[S24] C：获取本地时间
来源：http://qzr.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qcz.zycfv.cn

[S25] C：内存拷贝
来源：http://qwm.xuanzx.com

memcpy(dst, src, n);
来源：http://vry.nanxinkj.top

[S26] C：内存清零
来源：http://rxg.yj202588.top

memset(a, 0, sizeof a);
来源：http://ovp.jqgfzy.top

[S27] C：定义常量
来源：http://fhb.yueranfly.top

const double PI = 3.14159;
来源：http://pmo.cdnleiting.top

[S28] C：静态变量
来源：http://ohb.pycfn.com

static int counter = 0;
来源：http://vkg.fzhhl.top

[S29] C：变参函数
来源：http://cmv.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://usc.feifeiyinyue.top

[S30] C：头文件保护
来源：http://iju.jqgufenzy.top

#ifndef X_H
来源：http://rgm.gzhubu.top

#define X_H
来源：http://vux.hammf.cn

#endif
来源：http://rid.jianghu66.top

[S31] C++：Hello World
来源：http://hxd.nanxinkj.top

#include <iostream>
来源：http://wdg.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://kud.quarkkingdee.top

[S32] C++：字符串
来源：http://sxd.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://lys.meibo888.top

[S33] C++：vector 增删
来源：http://zgo.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fye.andypj.xyz

[S34] C++：遍历 vector
来源：http://mkl.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://grz.jinqigufen.top

[S35] C++：map
来源：http://cej.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://otj.zhixingplan.top

[S36] C++：unordered_map
来源：http://wuf.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uey.wangdashe.top

[S37] C++：set
来源：http://yzs.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dxu.havefunace.top

[S38] C++：排序
来源：http://dku.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://shi.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://xvi.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zwf.chenjidiqi.icu

[S40] C++：查找元素
来源：http://dvc.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avg.yonumen.top

[S41] C++：类与构造函数
来源：http://kim.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yow.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://xdv.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://kod.52xcode.cn

[S43] C++：智能指针
来源：http://lks.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://uyy.quarkkingdee.top

[S44] C++：引用传参
来源：http://gmh.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://qou.jqgfzy.top

[S45] C++：lambda
来源：http://rbw.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cyb.yfazqb.com

[S46] C++：函数模板
来源：http://kpv.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sfq.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://sqk.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ikv.mhx1999.top

[S48] C++：逐行读文件
来源：http://flp.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://kuo.sweek.top

while (std::getline(in, line)) { }
来源：http://vid.aibaodan.cn

[S49] C++：写文件
来源：http://wiu.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zqk.guowangkeji.top

[S50] C++：格式化数字
来源：http://cax.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ctl.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://brk.zhongyouzk.top

static_cast<double>(a) / b
来源：http://lxr.birdmap.top

[S52] C++：const 与 noexcept
来源：http://bpa.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://hya.c1oappe.top

[S53] C++：移动语义
来源：http://emk.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://zto.0kj1m.cn

[S54] C++：异常处理
来源：http://wtw.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ctb.iojbl.cn

[S55] C++：结构化绑定
来源：http://ppl.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://otd.ivvv.top

[S56] C++：optional
来源：http://gyh.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lsg.birdmap.top

[S57] C++：编译期常量
来源：http://yuz.hnxiangtu.top

constexpr int N = 10;
来源：http://qeq.zhiwuduotai.top

[S58] C++：命名空间
来源：http://vsq.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://pfa.vqdsnc.cn

[S59] C++：静态断言
来源：http://sqi.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://upn.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://xyg.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gpt.zycfv.cn

================================================================================
来源：http://dkk.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zuq.tarul.cn

================================================================================
来源：http://sgf.havefunace.top

[T01] Kotlin：Hello World
来源：http://sla.yonumen.top

println("Hello")
来源：http://ndi.316326.xyz

[T02] Kotlin：变量
来源：http://rrk.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ayq.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://gsj.fehbvm.com

"值: $b"
来源：http://xtw.hnqzz.top

[T04] Kotlin：空安全
来源：http://sex.cucudq.cn

val n: String? = null;  n?.length
来源：http://cjo.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://kwz.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mel.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://eds.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tvx.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://dsn.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://any.hesvh.cn

[T08] Kotlin：数据类
来源：http://dqh.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://uxh.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://eja.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://cvn.cheryme.top

[T10] Kotlin：默认参数
来源：http://fsm.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tjx.cucudq.cn

[T11] Kotlin：协程
来源：http://lli.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oid.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://zeb.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://uqm.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://ghz.havefunace.top

val m = mapOf("a" to 1)
来源：http://tfz.svipenyu.cn

[T14] Kotlin：循环
来源：http://fus.pycfn.com

for (i in 1..10) println(i)
来源：http://ivo.dianchejie.cn

[T15] Kotlin：接口
来源：http://edh.cucudq.cn

interface Shape { fun area(): Double }
来源：http://yly.cashguo.top

[T16] Swift：Hello World
来源：http://hks.tarul.cn

print("Hello")
来源：http://lmp.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://iee.chenzaomai.com

var a = 1;  let b = 2
来源：http://kur.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://bzp.yfazqb.com

"值: \(b)"
来源：http://myb.jlsjyb.cn


<!-- 参考信息 -->