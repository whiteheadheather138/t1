代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://drw.dianchejie.cn

[R14] C 风格 for
来源：http://fbx.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uii.cashguo.top

[R15] while 逐行读文件
来源：http://fez.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ydp.zhijiandao.cn

[R16] until 等待条件
来源：http://zcc.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zho.yonumen.top

[R17] 数组定义与取值
来源：http://qai.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vpt.epnwcf.com

[R18] 遍历数组
来源：http://ery.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yxj.yanxiufei.cn

[R19] 数组长度
来源：http://heh.jlsjyb.cn

echo "${#arr[@]}"
来源：http://sco.tianlin.xyz

[R20] 关联数组（字典）
来源：http://csk.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vho.havefunace.top

[R21] 字符串长度
来源：http://bzn.zhaomingkeji.xyz

echo "${#s}"
来源：http://tnv.nanxuanxn.top

[R22] 截取子串
来源：http://olx.jinqigufen.top

echo "${s:0:5}"
来源：http://rpv.hywenlv.cn

[R23] 字符串替换
来源：http://qjv.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pna.zhiwuduotai.top

[R24] 大小写转换
来源：http://vao.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://flt.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://qpl.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://iwo.guowangkeji.top

[R26] 命令替换
来源：http://kom.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://wep.gotoacloud.top

[R27] 算术展开
来源：http://ejd.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://tjh.sxryk.cn

[R28] 浮点运算
来源：http://ccm.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://vkp.sweek.top

[R29] 定义函数
来源：http://hid.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mkg.vqdsnc.cn

[R30] 函数返回状态码
来源：http://bfu.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://zmn.fengsongda.top

[R31] 局部变量
来源：http://hxx.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://giz.ctjpmb.com

[R32] 参数个数校验
来源：http://cqp.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jfx.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://uqj.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ltv.bbcook.cn

[R34] 退出时清理
来源：http://mcz.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://ajc.mhx1999.top

[R35] 后台执行并等待
来源：http://vhq.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qiu.chenzaomai.com

[R36] 并发执行多个任务
来源：http://ysi.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wwg.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://iar.shanyushiyangkeji.top

files=$(ls -1)
来源：http://fis.xziqi.cn

[R38] 管道串联
来源：http://dus.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://rxg.meibo888.top

[R39] 重定向标准输出与错误
来源：http://nzv.aizwys.cn

cmd > out.log 2>&1
来源：http://uya.hysaishi.cn

[R40] 追加写日志
来源：http://uot.jyoumei.cn

echo "log" >> out.log
来源：http://mgo.tianlin.xyz

[R41] 丢弃输出
来源：http://eve.fzhhl.top

cmd >/dev/null 2>&1
来源：http://yyn.hysaishi.cn

[R42] 输入重定向
来源：http://yeg.shangyingyoupin.top

wc -l < a.txt
来源：http://ncm.yonumen.top

[R43] 按名字查找文件
来源：http://kvp.fengsongda.top

find . -name "*.log" -type f
来源：http://olt.ydzc1.top

[R44] 按修改时间查找
来源：http://mil.yueranfly.top

find . -mtime -7 -type f
来源：http://arr.zhijiandao.cn

[R45] 批量删除
来源：http://yrj.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://uwa.pycfn.com

[R46] 递归替换文件内容
来源：http://pyd.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dlx.wangdashe.top

[R47] sed 单行替换
来源：http://zed.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ggy.yangfankeji.com

[R48] awk 取指定列
来源：http://kwz.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://oxs.mhx1999.top

[R49] awk 带条件
来源：http://ccq.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lvq.vqdsnc.cn

[R50] awk 求和
来源：http://bid.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nvw.uphjek.com

[R51] 排序去重取前几
来源：http://mcr.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://adz.fktsv.cn

[R52] 统计行数
来源：http://qtt.ppjwa.cn

wc -l a.txt
来源：http://inw.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://jec.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tro.yangfankeji.com

[R54] 比较两个文件
来源：http://uqm.nanxinkj.top

diff a.txt b.txt
来源：http://ikw.yvedp.cn

[R55] 压缩与解压
来源：http://mkl.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oxk.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://qit.cqqwz.cn

scp file user@host:/path/
来源：http://nbt.yongpay.top

[R57] 远程执行命令
来源：http://eoc.dashuyun.cn

ssh user@host 'uptime'
来源：http://nlw.dashuyun.cn

[R58] 下载文件
来源：http://tqy.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fdb.hnxiangtu.top

[R59] 发 POST JSON
来源：http://ssq.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fuc.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://gct.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://leg.nanxuanxn.top

[R61] 磁盘占用
来源：http://qak.feifeiyinyue.top

df -h;  du -sh *
来源：http://ear.yonumen.top

[R62] 找最占空间的文件
来源：http://naf.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://gzx.iojbl.cn

[R63] 内存与进程
来源：http://ggt.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://gpz.ctjpmb.com

[R64] 结束进程
来源：http://chi.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://kgc.ivvv.top

[R65] 查看端口占用
来源：http://jzx.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygt.ydzc1.top

[R66] 定时任务
来源：http://gds.ybcxt.top

crontab -e;  crontab -l
来源：http://fgd.xziqi.cn

[R67] 生成随机十六进制串
来源：http://jwr.xylfe.cn

openssl rand -hex 16
来源：http://set.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://vbr.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wri.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://hnf.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://rqo.jinqigfzy.top

[R70] 时间戳与互转
来源：http://fmk.yfazqb.com

date +%s;  date -d @1700000000
来源：http://rhu.yonumen.top

[R71] 日期格式化
来源：http://jzo.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://uyf.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://zgm.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://soe.hywenlv.cn

[R73] 分割大日志
来源：http://feh.guowangkeji.top

split -l 1000 big.log part_
来源：http://njn.pengpengdd.cyou

[R74] 批量重命名
来源：http://nul.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tmk.fehbvm.com

[R75] 导出环境变量
来源：http://jsi.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://aqv.gzhubu.top

[R76] 使用临时文件
来源：http://hyy.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hox.cucudq.cn

[R77] 读取用户输入
来源：http://tqn.quarkkingdee.top

read -rp "请输入: " ans
来源：http://cbw.hfpthk.cn

[R78] 交互式菜单
来源：http://mra.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bdw.nanxinkj.top

[R79] 解析命令行选项
来源：http://fsx.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fjw.yonumen.top

[R80] 查看脚本执行耗时
来源：http://ipw.9152youxi.cn

time ./run.sh
来源：http://umk.jyoumei.cn

================================================================================
来源：http://vff.vqdsnc.cn

S. C / C++ 专题
来源：http://vyj.yj20258.top

================================================================================
来源：http://ntc.hcnkem.com

[S01] C：Hello World
来源：http://hej.yj202588.top

#include <stdio.h>
来源：http://fki.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://afw.hammf.cn

[S02] C：变量与格式化输出
来源：http://rlb.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://avl.zdqjudy.top

[S03] C：读入整数
来源：http://xzn.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://sqn.sjlbkw.cn

[S04] C：字符串复制
来源：http://rcp.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dij.jinqigfzy.top

[S05] C：字符串长度
来源：http://mvg.jlsjyb.cn

strlen(s)
来源：http://ysz.xziqi.cn

[S06] C：字符串比较
来源：http://ybp.hysaishi.cn

strcmp(a, b) == 0
来源：http://yzh.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://gvl.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xhs.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://ejy.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vbv.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://vjp.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apq.ydjk.org.cn

[S10] C：指针与解引用
来源：http://qnf.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://cpz.ivvv.top

[S11] C：逐行读文件
来源：http://uyl.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://odj.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qqi.vqdsnc.cn

fclose(f);
来源：http://gjr.shangyingyoupin.top

[S12] C：写文件
来源：http://lgu.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dct.cqqwz.cn

[S13] C：宏定义
来源：http://ebl.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hld.316326.xyz

[S14] C：枚举
来源：http://reb.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://mtt.epnwcf.com

[S15] C：类型转换
来源：http://mbw.gzhubu.top

(double) a / b
来源：http://ghi.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://tep.meibo888.top

x |= (1 << 3);
来源：http://fgj.andypj.xyz

[S17] C：安全拼接字符串
来源：http://uab.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lxc.daria6918.cn

[S18] C：命令行参数
来源：http://fkk.316326.xyz

int main(int argc, char **argv)
来源：http://ado.cheryme.top

[S19] C：快速排序
来源：http://utn.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xxl.c1oappe.top

[S20] C：二分查找
来源：http://zcx.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ibj.sweek.top

[S21] C：字符类别判断
来源：http://vql.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmr.kuanghao11.cn

[S22] C：字符串转数字
来源：http://zjl.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://dst.vqdsnc.cn

[S23] C：随机数
来源：http://nuv.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cut.vqdsnc.cn

[S24] C：获取本地时间
来源：http://opt.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uzm.yj20258.top

[S25] C：内存拷贝
来源：http://yxt.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://ocw.sufxvd.cn

[S26] C：内存清零
来源：http://him.xziqi.cn

memset(a, 0, sizeof a);
来源：http://qcq.guannengcc.top

[S27] C：定义常量
来源：http://ava.nanxinkj.top

const double PI = 3.14159;
来源：http://xtg.quarkkingdee.top

[S28] C：静态变量
来源：http://glw.ywan-chungtsiang.top

static int counter = 0;
来源：http://cyz.zhiwuduotai.top

[S29] C：变参函数
来源：http://jra.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vbu.yfazqb.com

[S30] C：头文件保护
来源：http://glc.cheryme.top

#ifndef X_H
来源：http://dby.vehdjk.com

#define X_H
来源：http://wnc.xuanzx.com

#endif
来源：http://aki.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://fta.tian-w.cn

#include <iostream>
来源：http://drx.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://lcn.chenlongwang.top

[S32] C++：字符串
来源：http://pjz.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://atg.nwbrower.top

[S33] C++：vector 增删
来源：http://qiy.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://txi.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://mdh.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://xiv.xuanzx.com

[S35] C++：map
来源：http://kmf.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qba.ydzc1.top

[S36] C++：unordered_map
来源：http://pij.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://upl.ydzc1.top

[S37] C++：set
来源：http://xcz.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bcy.daria6918.cn

[S38] C++：排序
来源：http://apl.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://spn.cheryme.top

[S39] C++：自定义比较器排序
来源：http://nzv.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://umq.shuidangran.top

[S40] C++：查找元素
来源：http://bqf.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://foh.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://rby.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gwy.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://wge.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://wwa.vqdsnc.cn

[S43] C++：智能指针
来源：http://rvo.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://drd.cheryme.top

[S44] C++：引用传参
来源：http://vbf.mhx1999.top

void inc(int &x) { ++x; }
来源：http://qav.zhixingplan.top

[S45] C++：lambda
来源：http://ppo.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://iaf.gaohongyu789.top

[S46] C++：函数模板
来源：http://dsh.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yrv.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://ixe.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qej.ehwqpu.com

[S48] C++：逐行读文件
来源：http://vxk.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://jpn.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://wcy.jyoumei.cn

[S49] C++：写文件
来源：http://okn.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ima.shzxlz.cn

[S50] C++：格式化数字
来源：http://chl.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://beq.cucudq.cn

[S51] C++：显式类型转换
来源：http://npw.gzhubu.top

static_cast<double>(a) / b
来源：http://pce.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://lcs.tian-w.cn

int size() const noexcept { return n_; }
来源：http://lwu.chenzaomai.com

[S53] C++：移动语义
来源：http://qgs.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://rmu.ppjwa.cn

[S54] C++：异常处理
来源：http://nav.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrm.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://akg.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hrd.andypj.xyz

[S56] C++：optional
来源：http://idu.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tgf.ydzc1.top

[S57] C++：编译期常量
来源：http://njv.ppjwa.cn

constexpr int N = 10;
来源：http://udq.kuanghao11.cn

[S58] C++：命名空间
来源：http://okx.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://gin.yuanzhike.top

[S59] C++：静态断言
来源：http://shz.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ivq.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://mjz.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://azj.52xcode.cn

================================================================================
来源：http://sey.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hhz.xinyue.icu

================================================================================
来源：http://znf.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://qls.fktsv.cn

println("Hello")
来源：http://qld.sjlbkw.cn

[T02] Kotlin：变量
来源：http://ikt.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uvt.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://jcj.zhijiandao.cn

"值: $b"
来源：http://dxp.ehwqpu.com

[T04] Kotlin：空安全
来源：http://jqk.gzhubu.top

val n: String? = null;  n?.length
来源：http://her.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://qqx.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ioz.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://fqj.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uet.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://ctz.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lug.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://vap.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://cjb.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://txq.sweek.top

fun String.exclaim() = this + "!"
来源：http://osr.smart0.xyz

[T10] Kotlin：默认参数
来源：http://vqc.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://slv.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://bmi.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vey.andypj.xyz

[T12] Kotlin：解构声明
来源：http://igb.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://xaz.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://yry.yuxming.cn

val m = mapOf("a" to 1)
来源：http://bzz.zhongyouzk.top

[T14] Kotlin：循环
来源：http://euc.tian-w.cn

for (i in 1..10) println(i)
来源：http://xkf.andypj.xyz

[T15] Kotlin：接口
来源：http://apb.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://mlj.gaohongyu789.top

[T16] Swift：Hello World
来源：http://zst.ppjwa.cn

print("Hello")
来源：http://rqo.zhiwuduotai.top


<!-- 参考信息 -->