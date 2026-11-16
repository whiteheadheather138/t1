代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://aaw.chenlongwang.top

[R14] C 风格 for
来源：http://qco.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://haf.dashuyun.cn

[R15] while 逐行读文件
来源：http://eir.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hma.tarul.cn

[R16] until 等待条件
来源：http://zlo.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bwb.cashguo.top

[R17] 数组定义与取值
来源：http://yvo.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mcr.redwolf501.top

[R18] 遍历数组
来源：http://uys.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tzv.haohaochexian.top

[R19] 数组长度
来源：http://dhw.52xcode.cn

echo "${#arr[@]}"
来源：http://edt.hnqzz.top

[R20] 关联数组（字典）
来源：http://tya.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxt.xziqi.cn

[R21] 字符串长度
来源：http://fbe.xuanzx.com

echo "${#s}"
来源：http://rzk.tarul.cn

[R22] 截取子串
来源：http://xfl.zhoulong.xyz

echo "${s:0:5}"
来源：http://okn.jqgfzy.top

[R23] 字符串替换
来源：http://xoq.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ufh.haohaochexian.top

[R24] 大小写转换
来源：http://lvi.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://chn.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://hmp.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bnr.haohaochexian.top

[R26] 命令替换
来源：http://ild.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://nfw.andypj.xyz

[R27] 算术展开
来源：http://fni.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://dzv.mhx1999.top

[R28] 浮点运算
来源：http://ein.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://met.hesvh.cn

[R29] 定义函数
来源：http://jss.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rxk.xuanzx.com

[R30] 函数返回状态码
来源：http://gtf.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://hyd.sysykeji.top

[R31] 局部变量
来源：http://qwi.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://lra.yongpay.top

[R32] 参数个数校验
来源：http://bcr.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kcf.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://mnh.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqs.cqqwz.cn

[R34] 退出时清理
来源：http://edm.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://cag.zhixingplan.top

[R35] 后台执行并等待
来源：http://caa.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dgc.zhixingplan.top

[R36] 并发执行多个任务
来源：http://gzg.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vpd.zhengqikj.top

[R37] 把输出赋给变量
来源：http://qok.yangfankeji.com

files=$(ls -1)
来源：http://lzm.pycfn.com

[R38] 管道串联
来源：http://nmw.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://tdv.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://qqi.jianghu66.top

cmd > out.log 2>&1
来源：http://gby.cheryme.top

[R40] 追加写日志
来源：http://jvp.fanxiaobao.xyz

echo "log" >> out.log
来源：http://vwn.jianghu66.top

[R41] 丢弃输出
来源：http://zmx.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://soo.chenjidiqi.icu

[R42] 输入重定向
来源：http://iem.316326.xyz

wc -l < a.txt
来源：http://fnd.zdbjq.cn

[R43] 按名字查找文件
来源：http://rwk.jqgfzy.top

find . -name "*.log" -type f
来源：http://gdl.cucudq.cn

[R44] 按修改时间查找
来源：http://skh.yangfankeji.com

find . -mtime -7 -type f
来源：http://xbu.daxiang520.top

[R45] 批量删除
来源：http://whl.fzhhl.top

find . -name "*.tmp" -delete
来源：http://cwq.fzhhl.top

[R46] 递归替换文件内容
来源：http://vsk.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rqg.sufxvd.cn

[R47] sed 单行替换
来源：http://qqj.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://wfv.yfazqb.com

[R48] awk 取指定列
来源：http://pny.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://yqf.zycfv.cn

[R49] awk 带条件
来源：http://bja.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dfa.hfpthk.cn

[R50] awk 求和
来源：http://hdx.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://gci.c1oappe.top

[R51] 排序去重取前几
来源：http://rpu.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://izd.hcnkem.com

[R52] 统计行数
来源：http://jwg.birdmap.top

wc -l a.txt
来源：http://hyc.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://kam.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://grn.dianchejie.cn

[R54] 比较两个文件
来源：http://kqp.daria6918.cn

diff a.txt b.txt
来源：http://yum.iojbl.cn

[R55] 压缩与解压
来源：http://qyu.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kfs.hesvh.cn

[R56] 远程拷贝
来源：http://ulw.cdnleiting.top

scp file user@host:/path/
来源：http://kcj.snrcjt.cn

[R57] 远程执行命令
来源：http://xvz.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://dsd.yj20258.top

[R58] 下载文件
来源：http://tcf.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jbi.nanxuanxn.top

[R59] 发 POST JSON
来源：http://aic.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tbj.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://ytf.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://anh.dashuyun.cn

[R61] 磁盘占用
来源：http://vrp.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://wqm.hfpthk.cn

[R62] 找最占空间的文件
来源：http://fhr.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://uow.yongpay.top

[R63] 内存与进程
来源：http://qfa.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://cxm.hysaishi.cn

[R64] 结束进程
来源：http://bng.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://jlg.chenzaomai.com

[R65] 查看端口占用
来源：http://odq.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://npo.yangfankeji.com

[R66] 定时任务
来源：http://voa.zhengqikj.top

crontab -e;  crontab -l
来源：http://nna.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://qcl.andypj.xyz

openssl rand -hex 16
来源：http://nrr.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://kpm.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uft.haohaochexian.top

[R69] 生成随机密码
来源：http://fky.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://lzt.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://mnc.bjfxy.top

date +%s;  date -d @1700000000
来源：http://emw.nanxuanxn.top

[R71] 日期格式化
来源：http://nly.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uvj.shzxlz.cn

[R72] 等待端口就绪
来源：http://fyu.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dhi.kuanghao11.cn

[R73] 分割大日志
来源：http://pqw.jqgufenzy.top

split -l 1000 big.log part_
来源：http://ifm.ydzc1.top

[R74] 批量重命名
来源：http://woh.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hly.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://qfj.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://dbd.havefunace.top

[R76] 使用临时文件
来源：http://ekw.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dvl.uphjek.com

[R77] 读取用户输入
来源：http://bbl.hnqzz.top

read -rp "请输入: " ans
来源：http://mdj.pengpengdd.cyou

[R78] 交互式菜单
来源：http://mip.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yrv.vehdjk.com

[R79] 解析命令行选项
来源：http://ywa.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nsq.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://pem.jinqigufen.top

time ./run.sh
来源：http://jrp.zycfv.cn

================================================================================
来源：http://xkq.yueranfly.top

S. C / C++ 专题
来源：http://mym.iojbl.cn

================================================================================
来源：http://cnw.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://wjm.chenlongwang.top

#include <stdio.h>
来源：http://igh.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hof.bbcook.cn

[S02] C：变量与格式化输出
来源：http://ram.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://okg.hongshengwenyu.top

[S03] C：读入整数
来源：http://cek.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://mat.redwolf501.top

[S04] C：字符串复制
来源：http://zlu.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pgq.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://qvp.yfazqb.com

strlen(s)
来源：http://yxh.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://egv.smart0.xyz

strcmp(a, b) == 0
来源：http://wia.cucudq.cn

[S07] C：数组遍历求和
来源：http://tid.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fid.ivvv.top

[S08] C：动态内存分配与释放
来源：http://gxj.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mhv.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://kfe.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wel.dianchejie.cn

[S10] C：指针与解引用
来源：http://aey.yuxming.cn

int *p = &a;  *p = 5;
来源：http://ira.zdbjq.cn

[S11] C：逐行读文件
来源：http://luy.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://clo.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://roy.aibaodan.cn

fclose(f);
来源：http://ufp.jinqigfzy.top

[S12] C：写文件
来源：http://hde.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lid.jiagoushi.top

[S13] C：宏定义
来源：http://giv.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wle.gaohongyu789.top

[S14] C：枚举
来源：http://dou.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://slw.shangyingyoupin.top

[S15] C：类型转换
来源：http://rbi.gogol.net.cn

(double) a / b
来源：http://gsc.yj202588.top

[S16] C：位操作置位
来源：http://hru.guannengcc.top

x |= (1 << 3);
来源：http://ynq.fzhhl.top

[S17] C：安全拼接字符串
来源：http://ahl.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://esz.haohaochexian.top

[S18] C：命令行参数
来源：http://idv.redwolf501.top

int main(int argc, char **argv)
来源：http://qgz.hywenlv.cn

[S19] C：快速排序
来源：http://guk.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://stt.jiagoushi.top

[S20] C：二分查找
来源：http://kvk.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rdw.zhongyouzk.top

[S21] C：字符类别判断
来源：http://bjz.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gsv.hfpthk.cn

[S22] C：字符串转数字
来源：http://wog.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://fad.wangshuangyany.cn

[S23] C：随机数
来源：http://mit.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kjt.birdmap.top

[S24] C：获取本地时间
来源：http://ekc.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qlk.tianlin.xyz

[S25] C：内存拷贝
来源：http://rsg.9152youxi.cn

memcpy(dst, src, n);
来源：http://cqq.sjlbkw.cn

[S26] C：内存清零
来源：http://tuj.fehbvm.com

memset(a, 0, sizeof a);
来源：http://wlu.ivvv.top

[S27] C：定义常量
来源：http://rbc.shuidangran.top

const double PI = 3.14159;
来源：http://fcg.aibaodan.cn

[S28] C：静态变量
来源：http://dva.gaohongyu789.top

static int counter = 0;
来源：http://htu.daria6918.cn

[S29] C：变参函数
来源：http://lph.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://euy.zhijiandao.cn

[S30] C：头文件保护
来源：http://xzh.52xcode.cn

#ifndef X_H
来源：http://jcg.zhengqikj.top

#define X_H
来源：http://pbm.ehwqpu.com

#endif
来源：http://qfg.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://nia.cashguo.top

#include <iostream>
来源：http://ocy.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://cil.chenzaomai.com

[S32] C++：字符串
来源：http://apo.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://osu.316326.xyz

[S33] C++：vector 增删
来源：http://ein.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://szo.yuanzhike.top

[S34] C++：遍历 vector
来源：http://cle.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://ghx.zhijiandao.cn

[S35] C++：map
来源：http://ree.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rmx.zycfv.cn

[S36] C++：unordered_map
来源：http://ukb.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lmh.uphjek.com

[S37] C++：set
来源：http://vaa.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hvc.cheryme.top

[S38] C++：排序
来源：http://ldk.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://eom.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://qoh.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://phe.yuanzhike.top

[S40] C++：查找元素
来源：http://glj.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dvc.aizwys.cn

[S41] C++：类与构造函数
来源：http://luf.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gni.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://eid.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://unr.yonumen.top

[S43] C++：智能指针
来源：http://qus.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://wji.bjfxy.top

[S44] C++：引用传参
来源：http://uuw.mhx1999.top

void inc(int &x) { ++x; }
来源：http://byo.ydjk.org.cn

[S45] C++：lambda
来源：http://pjd.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jsd.wangshuangyany.cn

[S46] C++：函数模板
来源：http://kxp.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gig.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://auy.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ehi.gzhubu.top

[S48] C++：逐行读文件
来源：http://kei.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rkf.xylfe.cn

while (std::getline(in, line)) { }
来源：http://mnf.nanxinkj.top

[S49] C++：写文件
来源：http://ntl.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zpv.jinqigufen.top

[S50] C++：格式化数字
来源：http://bve.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kjo.guannengcc.top

[S51] C++：显式类型转换
来源：http://ezc.yangfankeji.com

static_cast<double>(a) / b
来源：http://ful.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://nxl.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://zah.pengpengdd.cyou

[S53] C++：移动语义
来源：http://gsk.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://ojq.pengpengdd.cyou

[S54] C++：异常处理
来源：http://vle.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aet.ppjwa.cn

[S55] C++：结构化绑定
来源：http://bbc.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vac.sweek.top

[S56] C++：optional
来源：http://csl.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qaz.gzhubu.top

[S57] C++：编译期常量
来源：http://xeb.zhongyouzk.top

constexpr int N = 10;
来源：http://ocq.hywenlv.cn

[S58] C++：命名空间
来源：http://ypg.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://glm.bbcook.cn

[S59] C++：静态断言
来源：http://fqw.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rxu.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://hxr.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tce.bjfxy.top

================================================================================
来源：http://hht.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fsx.yuxming.cn

================================================================================
来源：http://ans.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://lmr.sweek.top

println("Hello")
来源：http://akm.bjfxy.top

[T02] Kotlin：变量
来源：http://zqj.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yvn.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://dez.fktsv.cn

"值: $b"
来源：http://pyn.meibo888.top

[T04] Kotlin：空安全
来源：http://vfs.sxryk.cn

val n: String? = null;  n?.length
来源：http://xev.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://vbd.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://isi.ydzc1.top

[T06] Kotlin：集合映射
来源：http://jqq.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://adu.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://ava.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vsc.sufxvd.cn

[T08] Kotlin：数据类
来源：http://ken.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://wev.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://hrr.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://cvw.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://gnm.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hpy.cheryme.top

[T11] Kotlin：协程
来源：http://pcc.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hjp.52xcode.cn

[T12] Kotlin：解构声明
来源：http://dvt.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://sdi.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://cup.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://ngj.haohaochexian.top

[T14] Kotlin：循环
来源：http://wio.zdqjudy.top

for (i in 1..10) println(i)
来源：http://dos.tian-w.cn

[T15] Kotlin：接口
来源：http://ncc.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://xes.nanxinkj.top

[T16] Swift：Hello World
来源：http://gdc.uphjek.com

print("Hello")
来源：http://bvm.jqgfzy.top


<!-- 参考信息 -->