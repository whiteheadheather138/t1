代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mar.shzxlz.cn

[R18] 遍历数组
来源：http://jnb.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lzy.wangshuangyany.cn

[R19] 数组长度
来源：http://fjy.dianchejie.cn

echo "${#arr[@]}"
来源：http://iqc.fehbvm.com

[R20] 关联数组（字典）
来源：http://oaf.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qya.sxryk.cn

[R21] 字符串长度
来源：http://rfy.meibo888.top

echo "${#s}"
来源：http://gjs.chenlongwang.top

[R22] 截取子串
来源：http://lsu.daria6918.cn

echo "${s:0:5}"
来源：http://fnd.xuanzx.com

[R23] 字符串替换
来源：http://agd.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vfe.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://sjb.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://der.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://eby.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://fzc.ppjwa.cn

[R26] 命令替换
来源：http://pgx.yj20258.top

now=$(date +%F); echo "$now"
来源：http://ksm.tanke756.top

[R27] 算术展开
来源：http://qyg.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://sat.fehbvm.com

[R28] 浮点运算
来源：http://cmd.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://qbp.yanxiufei.cn

[R29] 定义函数
来源：http://iyu.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zkn.xinyue.icu

[R30] 函数返回状态码
来源：http://opl.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://fki.quarkkingdee.top

[R31] 局部变量
来源：http://jpy.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://pku.zhengqikj.top

[R32] 参数个数校验
来源：http://kal.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iop.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://pei.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://acj.zhengqikj.top

[R34] 退出时清理
来源：http://kus.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vqw.hywenlv.cn

[R35] 后台执行并等待
来源：http://iwp.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://trg.aibaodan.cn

[R36] 并发执行多个任务
来源：http://otu.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iku.yvedp.cn

[R37] 把输出赋给变量
来源：http://kkq.yueranfly.top

files=$(ls -1)
来源：http://tcz.yuxming.cn

[R38] 管道串联
来源：http://lss.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://bam.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://hja.yfazqb.com

cmd > out.log 2>&1
来源：http://mbc.hcnkem.com

[R40] 追加写日志
来源：http://ycs.feifeiyinyue.top

echo "log" >> out.log
来源：http://ifl.ppjwa.cn

[R41] 丢弃输出
来源：http://ujl.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://dbp.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://ztl.redwolf501.top

wc -l < a.txt
来源：http://vxw.yj20258888.top

[R43] 按名字查找文件
来源：http://sqk.andypj.xyz

find . -name "*.log" -type f
来源：http://joc.mhx1999.top

[R44] 按修改时间查找
来源：http://zsj.bjfxy.top

find . -mtime -7 -type f
来源：http://etq.iojbl.cn

[R45] 批量删除
来源：http://rch.hcnkem.com

find . -name "*.tmp" -delete
来源：http://xbv.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://jal.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cic.sxryk.cn

[R47] sed 单行替换
来源：http://rai.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nwh.sxryk.cn

[R48] awk 取指定列
来源：http://vco.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://kpp.tanke756.top

[R49] awk 带条件
来源：http://ihe.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wdh.yfazqb.com

[R50] awk 求和
来源：http://hcq.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qpl.gogol.net.cn

[R51] 排序去重取前几
来源：http://bgm.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mui.smart0.xyz

[R52] 统计行数
来源：http://gmc.shuidangran.top

wc -l a.txt
来源：http://boe.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://tiw.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://usn.cqqwz.cn

[R54] 比较两个文件
来源：http://gpb.gzhubu.top

diff a.txt b.txt
来源：http://jeo.ybcxt.top

[R55] 压缩与解压
来源：http://gas.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pas.zhongyouzk.top

[R56] 远程拷贝
来源：http://ces.yuxming.cn

scp file user@host:/path/
来源：http://xfq.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://zli.tian-w.cn

ssh user@host 'uptime'
来源：http://ekh.yangfankeji.com

[R58] 下载文件
来源：http://mmd.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://prk.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://uca.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rsd.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://yre.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ijq.aibaodan.cn

[R61] 磁盘占用
来源：http://ais.feifeiyinyue.top

df -h;  du -sh *
来源：http://izp.yongpay.top

[R62] 找最占空间的文件
来源：http://fik.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://epq.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://zpv.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://brc.52xcode.cn

[R64] 结束进程
来源：http://svm.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://fxd.hesvh.cn

[R65] 查看端口占用
来源：http://mrg.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygs.shanyushiyangtech.top

[R66] 定时任务
来源：http://nie.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://sak.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://nen.cqqwz.cn

openssl rand -hex 16
来源：http://uzf.chenlongwang.top

[R68] 计算文件校验值
来源：http://qke.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ybx.9152youxi.cn

[R69] 生成随机密码
来源：http://sea.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://kon.jlsjyb.cn

[R70] 时间戳与互转
来源：http://aay.ivvv.top

date +%s;  date -d @1700000000
来源：http://bcm.smart0.xyz

[R71] 日期格式化
来源：http://tkc.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yjo.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://umh.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dzx.gotoacloud.top

[R73] 分割大日志
来源：http://atw.xylfe.cn

split -l 1000 big.log part_
来源：http://chm.zhengqikj.top

[R74] 批量重命名
来源：http://ydw.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://awk.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://ahg.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://jlq.yonumen.top

[R76] 使用临时文件
来源：http://bqk.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zci.pengpengdd.cyou

[R77] 读取用户输入
来源：http://jmj.tanke756.top

read -rp "请输入: " ans
来源：http://sae.pycfn.com

[R78] 交互式菜单
来源：http://hjg.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://utj.birdmap.top

[R79] 解析命令行选项
来源：http://mlh.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rjy.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://qlt.xylfe.cn

time ./run.sh
来源：http://cjr.iojbl.cn

================================================================================
来源：http://smp.svipenyu.cn

S. C / C++ 专题
来源：http://pef.gzhubu.top

================================================================================
来源：http://bdu.zdbjq.cn

[S01] C：Hello World
来源：http://ina.xylfe.cn

#include <stdio.h>
来源：http://xsg.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qym.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://dhv.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://nuw.hesvh.cn

[S03] C：读入整数
来源：http://fai.jqgfzy.top

int x; scanf("%d", &x);
来源：http://fbz.ppjwa.cn

[S04] C：字符串复制
来源：http://kpf.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qxw.gogol.net.cn

[S05] C：字符串长度
来源：http://yqo.ybcxt.top

strlen(s)
来源：http://abj.ppjwa.cn

[S06] C：字符串比较
来源：http://wvl.uphjek.com

strcmp(a, b) == 0
来源：http://sgf.bjfxy.top

[S07] C：数组遍历求和
来源：http://qha.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://duk.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://utx.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eos.tanke756.top

[S09] C：结构体定义与初始化
来源：http://bwz.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xuh.epnwcf.com

[S10] C：指针与解引用
来源：http://cjl.xuanzx.com

int *p = &a;  *p = 5;
来源：http://qnm.tianlin.xyz

[S11] C：逐行读文件
来源：http://anq.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://gyk.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://huf.zhongyouzk.top

fclose(f);
来源：http://puu.jinqigufen.top

[S12] C：写文件
来源：http://oll.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://spx.hammf.cn

[S13] C：宏定义
来源：http://egd.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qpi.jinqigufen.top

[S14] C：枚举
来源：http://geq.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://okh.yj202588.top

[S15] C：类型转换
来源：http://hsq.yj20258.top

(double) a / b
来源：http://fxh.tanke756.top

[S16] C：位操作置位
来源：http://fjk.uphjek.com

x |= (1 << 3);
来源：http://dri.sysykeji.top

[S17] C：安全拼接字符串
来源：http://got.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vxq.aibaodan.cn

[S18] C：命令行参数
来源：http://kvf.uphjek.com

int main(int argc, char **argv)
来源：http://ems.jyoumei.cn

[S19] C：快速排序
来源：http://uvq.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zjy.chenzaomai.com

[S20] C：二分查找
来源：http://uim.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xdj.xinyue.icu

[S21] C：字符类别判断
来源：http://vqb.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wkq.zdqjudy.top

[S22] C：字符串转数字
来源：http://gml.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://ktb.xylfe.cn

[S23] C：随机数
来源：http://bow.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://uqz.aibaodan.cn

[S24] C：获取本地时间
来源：http://qrg.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fmq.zhijiandao.cn

[S25] C：内存拷贝
来源：http://rpw.yonumen.top

memcpy(dst, src, n);
来源：http://ufi.shanyushiyangtech.top

[S26] C：内存清零
来源：http://zxn.daria6918.cn

memset(a, 0, sizeof a);
来源：http://ckg.quarkkingdee.top

[S27] C：定义常量
来源：http://xzm.shuidangran.top

const double PI = 3.14159;
来源：http://itk.uphjek.com

[S28] C：静态变量
来源：http://ddo.yuxming.cn

static int counter = 0;
来源：http://zee.zycfv.cn

[S29] C：变参函数
来源：http://zbk.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gaz.jyoumei.cn

[S30] C：头文件保护
来源：http://bhp.yfazqb.com

#ifndef X_H
来源：http://knh.nanxuanxn.top

#define X_H
来源：http://qpi.feifeiyinyue.top

#endif
来源：http://qxf.bjfxy.top

[S31] C++：Hello World
来源：http://ncd.sjlbkw.cn

#include <iostream>
来源：http://qnx.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://zjl.xuanzx.com

[S32] C++：字符串
来源：http://udw.cheryme.top

std::string s = "hi";  s += "!";
来源：http://ehf.mhx1999.top

[S33] C++：vector 增删
来源：http://yry.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qpx.wangdashe.top

[S34] C++：遍历 vector
来源：http://wqd.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ghx.feifeiyinyue.top

[S35] C++：map
来源：http://atu.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://myf.cucudq.cn

[S36] C++：unordered_map
来源：http://zhe.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sql.jianghu66.top

[S37] C++：set
来源：http://ncw.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mho.hammf.cn

[S38] C++：排序
来源：http://wah.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://lwf.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://jzw.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xpq.hammf.cn

[S40] C++：查找元素
来源：http://dag.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fdb.0kj1m.cn

[S41] C++：类与构造函数
来源：http://gcs.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qaj.cashguo.top

[S42] C++：继承与虚函数
来源：http://gyb.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://jke.fehbvm.com

[S43] C++：智能指针
来源：http://uiv.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://xet.bjfxy.top

[S44] C++：引用传参
来源：http://zsc.hammf.cn

void inc(int &x) { ++x; }
来源：http://lmd.fzhhl.top

[S45] C++：lambda
来源：http://xkv.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hsv.snrcjt.cn

[S46] C++：函数模板
来源：http://pxf.zhiwuduotai.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tof.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://lrg.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://syw.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://gpg.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dws.yuxming.cn

while (std::getline(in, line)) { }
来源：http://ash.nanxuanxn.top

[S49] C++：写文件
来源：http://djw.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pjt.bjfxy.top

[S50] C++：格式化数字
来源：http://vaz.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mme.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://ptg.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://bux.jqgufenzy.top

[S52] C++：const 与 noexcept
来源：http://lhm.yueranfly.top

int size() const noexcept { return n_; }
来源：http://yuh.zhoulong.xyz

[S53] C++：移动语义
来源：http://kat.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://bjr.hongshengwenyu.top

[S54] C++：异常处理
来源：http://wvd.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nrx.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://tdx.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://glk.yonumen.top

[S56] C++：optional
来源：http://rge.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pxg.gogol.net.cn

[S57] C++：编译期常量
来源：http://nmc.zhongyouzk.top

constexpr int N = 10;
来源：http://our.havefunace.top

[S58] C++：命名空间
来源：http://jzq.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://czf.xuanzx.com

[S59] C++：静态断言
来源：http://uvq.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mwq.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://jbm.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rua.hfpthk.cn

================================================================================
来源：http://nlh.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fez.zhaomingkeji.xyz

================================================================================
来源：http://lts.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://mxz.zhiwuduotai.top

println("Hello")
来源：http://goe.sysykeji.top

[T02] Kotlin：变量
来源：http://kvp.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://szc.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://jol.guannengcc.top

"值: $b"
来源：http://jhy.meibo888.top

[T04] Kotlin：空安全
来源：http://gat.zdqjudy.top

val n: String? = null;  n?.length
来源：http://fts.yj202588.top

[T05] Kotlin：when 表达式
来源：http://yno.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ncy.andypj.xyz

[T06] Kotlin：集合映射
来源：http://unl.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dyc.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://kxw.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://aez.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://yhp.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://wsd.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://wqr.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://ktg.hammf.cn

[T10] Kotlin：默认参数
来源：http://gml.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fyq.ydjk.org.cn

[T11] Kotlin：协程
来源：http://kmf.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://edw.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://jbf.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://omx.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://oum.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://eiq.gogol.net.cn

[T14] Kotlin：循环
来源：http://mrm.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://tjv.mhx1999.top

[T15] Kotlin：接口
来源：http://crq.sweek.top

interface Shape { fun area(): Double }
来源：http://soh.guannengcc.top

[T16] Swift：Hello World
来源：http://uka.daria6918.cn

print("Hello")
来源：http://ppl.gotoacloud.top

[T17] Swift：变量与常量
来源：http://ppv.yfazqb.com

var a = 1;  let b = 2
来源：http://knf.gzhubu.top

[T18] Swift：字符串插值
来源：http://coo.shzxlz.cn

"值: \(b)"
来源：http://yxg.hfpthk.cn

[T19] Swift：可选绑定
来源：http://qgj.smart0.xyz

if let n = opt { print(n) }
来源：http://jjg.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://gxb.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://byr.52xcode.cn


<!-- 参考信息 -->