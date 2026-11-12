代发 wailian999

esac
来源：http://pop.fehbvm.com

[R12] for 遍历文件
来源：http://ybm.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://kgm.ydjk.org.cn

[R13] for 计数循环
来源：http://rkc.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://fdk.nanxinkj.top

[R14] C 风格 for
来源：http://dwj.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://abf.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://ruj.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nuh.havefunace.top

[R16] until 等待条件
来源：http://zql.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hbg.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://udg.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wsa.shuidangran.top

[R18] 遍历数组
来源：http://vgj.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ipm.xziqi.cn

[R19] 数组长度
来源：http://tzo.sufxvd.cn

echo "${#arr[@]}"
来源：http://lec.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://ciy.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lgn.redwolf501.top

[R21] 字符串长度
来源：http://ufo.zycfv.cn

echo "${#s}"
来源：http://uhn.fktsv.cn

[R22] 截取子串
来源：http://ebj.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://box.epnwcf.com

[R23] 字符串替换
来源：http://ucb.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hvh.wangdashe.top

[R24] 大小写转换
来源：http://pcb.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hlt.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://lhn.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://zyn.xylfe.cn

[R26] 命令替换
来源：http://zmt.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://cwf.nanxinkj.top

[R27] 算术展开
来源：http://qwm.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://iof.hnxiangtu.top

[R28] 浮点运算
来源：http://qaa.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://rkq.52xcode.cn

[R29] 定义函数
来源：http://ydh.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfv.yj20258888.top

[R30] 函数返回状态码
来源：http://vyp.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://srd.aibaodan.cn

[R31] 局部变量
来源：http://vhc.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://tuh.redwolf501.top

[R32] 参数个数校验
来源：http://lsv.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://enz.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://joz.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ohe.vqdsnc.cn

[R34] 退出时清理
来源：http://mde.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://drc.yangfankeji.com

[R35] 后台执行并等待
来源：http://kfg.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rft.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://lcw.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://npa.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://xxn.aizwys.cn

files=$(ls -1)
来源：http://rdf.zhijiandao.cn

[R38] 管道串联
来源：http://nxh.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://zuy.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://ebs.yongpay.top

cmd > out.log 2>&1
来源：http://lwh.xuetiantiany.cn

[R40] 追加写日志
来源：http://rsz.shangyingyoupin.top

echo "log" >> out.log
来源：http://zbi.ivvv.top

[R41] 丢弃输出
来源：http://yci.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://yup.0kj1m.cn

[R42] 输入重定向
来源：http://kaz.9152youxi.cn

wc -l < a.txt
来源：http://fok.yonumen.top

[R43] 按名字查找文件
来源：http://zkq.shuidangran.top

find . -name "*.log" -type f
来源：http://nej.sjlbkw.cn

[R44] 按修改时间查找
来源：http://ada.hnqzz.top

find . -mtime -7 -type f
来源：http://pyz.ivvv.top

[R45] 批量删除
来源：http://yhq.c1oappe.top

find . -name "*.tmp" -delete
来源：http://kwj.chenlongwang.top

[R46] 递归替换文件内容
来源：http://vxd.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://etw.0kj1m.cn

[R47] sed 单行替换
来源：http://kuy.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://xej.sjlbkw.cn

[R48] awk 取指定列
来源：http://yjb.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://zrq.yongpay.top

[R49] awk 带条件
来源：http://big.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kom.uphjek.com

[R50] awk 求和
来源：http://ulq.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://sha.mhx1999.top

[R51] 排序去重取前几
来源：http://ofc.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://lno.svipenyu.cn

[R52] 统计行数
来源：http://yyo.tian-w.cn

wc -l a.txt
来源：http://qxc.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://qqy.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dbq.zhengqikj.top

[R54] 比较两个文件
来源：http://ugz.snrcjt.cn

diff a.txt b.txt
来源：http://xli.tian-w.cn

[R55] 压缩与解压
来源：http://qdm.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bxl.zycfv.cn

[R56] 远程拷贝
来源：http://zwa.hysaishi.cn

scp file user@host:/path/
来源：http://rjh.jqgfzy.top

[R57] 远程执行命令
来源：http://jem.gzhubu.top

ssh user@host 'uptime'
来源：http://vym.gzhubu.top

[R58] 下载文件
来源：http://wcl.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ars.vqdsnc.cn

[R59] 发 POST JSON
来源：http://sxq.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qjt.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://ezt.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xsd.xylfe.cn

[R61] 磁盘占用
来源：http://bty.chenlongwang.top

df -h;  du -sh *
来源：http://txa.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://aws.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://syb.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://wfz.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://pvb.tianlin.xyz

[R64] 结束进程
来源：http://acl.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://gcb.cucudq.cn

[R65] 查看端口占用
来源：http://ojl.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nvt.9152youxi.cn

[R66] 定时任务
来源：http://ivk.yj20258.top

crontab -e;  crontab -l
来源：http://dch.epnwcf.com

[R67] 生成随机十六进制串
来源：http://cik.quarkkingdee.top

openssl rand -hex 16
来源：http://mex.cucudq.cn

[R68] 计算文件校验值
来源：http://qzd.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ehb.chenjidiqi.icu

[R69] 生成随机密码
来源：http://bus.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://cwe.sysykeji.top

[R70] 时间戳与互转
来源：http://mel.daxiang520.top

date +%s;  date -d @1700000000
来源：http://sle.ivvv.top

[R71] 日期格式化
来源：http://jdd.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://boe.ppjwa.cn

[R72] 等待端口就绪
来源：http://ncj.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dnt.jianghu66.top

[R73] 分割大日志
来源：http://pzc.jqgufenzy.top

split -l 1000 big.log part_
来源：http://vfm.hesvh.cn

[R74] 批量重命名
来源：http://iiw.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://seq.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://lsb.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://uro.hnqzz.top

[R76] 使用临时文件
来源：http://gon.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kbi.52xcode.cn

[R77] 读取用户输入
来源：http://xnb.chenlongwang.top

read -rp "请输入: " ans
来源：http://umg.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://trv.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eyc.nwbrower.top

[R79] 解析命令行选项
来源：http://kag.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ars.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://bah.zhengqikj.top

time ./run.sh
来源：http://xaz.yj202588.top

================================================================================
来源：http://ace.ydzc1.top

S. C / C++ 专题
来源：http://ccb.c1oappe.top

================================================================================
来源：http://ngi.tarul.cn

[S01] C：Hello World
来源：http://zqg.haohaochexian.top

#include <stdio.h>
来源：http://vhl.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://noi.tanke756.top

[S02] C：变量与格式化输出
来源：http://lgn.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://afe.sysykeji.top

[S03] C：读入整数
来源：http://qfu.sufxvd.cn

int x; scanf("%d", &x);
来源：http://cga.fzhhl.top

[S04] C：字符串复制
来源：http://ees.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hjs.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://nxk.hammf.cn

strlen(s)
来源：http://bxj.birdmap.top

[S06] C：字符串比较
来源：http://gbk.yongpay.top

strcmp(a, b) == 0
来源：http://mit.yongpay.top

[S07] C：数组遍历求和
来源：http://ive.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fsq.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://zwb.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ixv.pycfn.com

[S09] C：结构体定义与初始化
来源：http://gxx.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://frh.jlsjyb.cn

[S10] C：指针与解引用
来源：http://ehr.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://ici.aibaodan.cn

[S11] C：逐行读文件
来源：http://ezd.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://ejn.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ybj.pengpengdd.cyou

fclose(f);
来源：http://prv.ehwqpu.com

[S12] C：写文件
来源：http://nfo.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mom.xuetiantiany.cn

[S13] C：宏定义
来源：http://ysw.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdl.xinyue.icu

[S14] C：枚举
来源：http://bgr.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://ejc.havefunace.top

[S15] C：类型转换
来源：http://qvq.cucudq.cn

(double) a / b
来源：http://pco.tanke756.top

[S16] C：位操作置位
来源：http://vvi.c1oappe.top

x |= (1 << 3);
来源：http://wye.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://uks.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uym.pengpengdd.cyou

[S18] C：命令行参数
来源：http://vst.daria6918.cn

int main(int argc, char **argv)
来源：http://dnl.iojbl.cn

[S19] C：快速排序
来源：http://who.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://rtl.jinqigufen.top

[S20] C：二分查找
来源：http://bqa.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://abn.haohaochexian.top

[S21] C：字符类别判断
来源：http://ohy.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xpr.sufxvd.cn

[S22] C：字符串转数字
来源：http://mag.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://wii.iojbl.cn

[S23] C：随机数
来源：http://ygr.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xdl.daxiang520.top

[S24] C：获取本地时间
来源：http://xlo.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sup.yonumen.top

[S25] C：内存拷贝
来源：http://ncv.ydzc1.top

memcpy(dst, src, n);
来源：http://iop.epnwcf.com

[S26] C：内存清零
来源：http://aod.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://tkn.aibaodan.cn

[S27] C：定义常量
来源：http://cmt.dashuyun.cn

const double PI = 3.14159;
来源：http://ftw.daria6918.cn

[S28] C：静态变量
来源：http://ixo.yueranfly.top

static int counter = 0;
来源：http://qhj.haohaochexian.top

[S29] C：变参函数
来源：http://ckz.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sjf.daria6918.cn

[S30] C：头文件保护
来源：http://pep.zdbjq.cn

#ifndef X_H
来源：http://xmm.jlsjyb.cn

#define X_H
来源：http://ziq.ywan-chungtsiang.top

#endif
来源：http://xcx.cucudq.cn

[S31] C++：Hello World
来源：http://tbn.yongpay.top

#include <iostream>
来源：http://dgo.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://tdj.gaohongyu789.top

[S32] C++：字符串
来源：http://hrh.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://eqc.xylfe.cn

[S33] C++：vector 增删
来源：http://mba.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukb.fzhhl.top

[S34] C++：遍历 vector
来源：http://msv.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://gdk.birdmap.top

[S35] C++：map
来源：http://lbq.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpx.hammf.cn

[S36] C++：unordered_map
来源：http://cvx.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://thh.ivvv.top

[S37] C++：set
来源：http://zdv.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgi.bjfxy.top

[S38] C++：排序
来源：http://ekm.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://xwz.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://drk.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://opx.hesvh.cn

[S40] C++：查找元素
来源：http://bxj.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyw.cdnleiting.top

[S41] C++：类与构造函数
来源：http://qns.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbr.hesvh.cn

[S42] C++：继承与虚函数
来源：http://qhx.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://xkr.cdnleiting.top

[S43] C++：智能指针
来源：http://may.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://ehc.feifeiyinyue.top

[S44] C++：引用传参
来源：http://oqa.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://jif.smart0.xyz

[S45] C++：lambda
来源：http://cjr.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lua.tianlin.xyz

[S46] C++：函数模板
来源：http://hew.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xwo.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://hul.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gbi.chenlongwang.top

[S48] C++：逐行读文件
来源：http://dds.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://dbj.ivvv.top

while (std::getline(in, line)) { }
来源：http://qlw.iojbl.cn

[S49] C++：写文件
来源：http://qmb.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dni.yj202588.top

[S50] C++：格式化数字
来源：http://rds.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rsa.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://cmg.chenzaomai.com

static_cast<double>(a) / b
来源：http://dej.tarul.cn

[S52] C++：const 与 noexcept
来源：http://nlf.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://hkr.birdmap.top

[S53] C++：移动语义
来源：http://uwm.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://spf.xylfe.cn

[S54] C++：异常处理
来源：http://wwj.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mho.haohaochexian.top

[S55] C++：结构化绑定
来源：http://sjn.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ble.quarkkingdee.top

[S56] C++：optional
来源：http://pfg.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wkc.jianghu66.top

[S57] C++：编译期常量
来源：http://mua.316326.xyz

constexpr int N = 10;
来源：http://ayn.jinqigufen.top

[S58] C++：命名空间
来源：http://azy.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://xzg.vqdsnc.cn

[S59] C++：静态断言
来源：http://xeg.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iho.tarul.cn

[S60] C++：遍历并删除元素
来源：http://rjh.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jvf.jinqigfzy.top

================================================================================
来源：http://iwa.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sqv.jyoumei.cn

================================================================================
来源：http://dtl.yj202588.top

[T01] Kotlin：Hello World
来源：http://eec.chenlongwang.top

println("Hello")
来源：http://gyt.9152youxi.cn

[T02] Kotlin：变量
来源：http://mar.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aut.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://vsk.aibaodan.cn

"值: $b"
来源：http://noh.hesvh.cn

[T04] Kotlin：空安全
来源：http://prf.zdbjq.cn

val n: String? = null;  n?.length
来源：http://dpa.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://fnn.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qsm.shuidangran.top

[T06] Kotlin：集合映射
来源：http://dgr.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eje.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://yfa.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://don.vehdjk.com

[T08] Kotlin：数据类
来源：http://jzo.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://hut.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://urg.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://ded.yuxming.cn

[T10] Kotlin：默认参数
来源：http://vyn.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://abr.zdbjq.cn

[T11] Kotlin：协程
来源：http://wtb.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jlq.xinyue.icu

[T12] Kotlin：解构声明
来源：http://mbm.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://acp.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://xom.daxiang520.top

val m = mapOf("a" to 1)
来源：http://mys.cheryme.top

[T14] Kotlin：循环
来源：http://gxo.snrcjt.cn

for (i in 1..10) println(i)
来源：http://xuf.vqdsnc.cn


<!-- 参考信息 -->