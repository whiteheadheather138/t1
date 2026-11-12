代发 wailian999

case "$1" in
来源：http://jvp.birdmap.top

start) echo "启动" ;;
来源：http://nsz.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://lsd.yj202588.top

*)     echo "未知命令" ;;
来源：http://agl.fengsongda.top

esac
来源：http://vvm.ydzc1.top

[R12] for 遍历文件
来源：http://pkl.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://gqi.aizwys.cn

[R13] for 计数循环
来源：http://odm.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://dsi.uphjek.com

[R14] C 风格 for
来源：http://llt.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zce.hysaishi.cn

[R15] while 逐行读文件
来源：http://yfc.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dtq.yanxiufei.cn

[R16] until 等待条件
来源：http://jbc.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oxm.hysaishi.cn

[R17] 数组定义与取值
来源：http://fol.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qmi.vehdjk.com

[R18] 遍历数组
来源：http://dfm.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nyy.redwolf501.top

[R19] 数组长度
来源：http://ode.vehdjk.com

echo "${#arr[@]}"
来源：http://rcz.wangdashe.top

[R20] 关联数组（字典）
来源：http://ruj.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tyn.shuidangran.top

[R21] 字符串长度
来源：http://msa.xuanzx.com

echo "${#s}"
来源：http://jpp.yanxiufei.cn

[R22] 截取子串
来源：http://jvx.zhongyouzk.top

echo "${s:0:5}"
来源：http://gnv.smart0.xyz

[R23] 字符串替换
来源：http://ujj.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jod.hfpthk.cn

[R24] 大小写转换
来源：http://rth.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://dep.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://tpd.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cia.cucudq.cn

[R26] 命令替换
来源：http://bwp.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://pcv.xziqi.cn

[R27] 算术展开
来源：http://wbu.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://cap.smart0.xyz

[R28] 浮点运算
来源：http://xhd.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://jgm.sweek.top

[R29] 定义函数
来源：http://uxf.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ico.jiagoushi.top

[R30] 函数返回状态码
来源：http://xiv.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://hnf.vqdsnc.cn

[R31] 局部变量
来源：http://amn.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://dbx.jinqigfzy.top

[R32] 参数个数校验
来源：http://hoj.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zoo.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://sfs.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xvm.yj202588.top

[R34] 退出时清理
来源：http://tdi.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://aqg.bjfxy.top

[R35] 后台执行并等待
来源：http://llz.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://nsb.dashuyun.cn

[R36] 并发执行多个任务
来源：http://xgl.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://das.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://bwm.sweek.top

files=$(ls -1)
来源：http://rml.ctjpmb.com

[R38] 管道串联
来源：http://jmc.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://ver.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://jgg.316326.xyz

cmd > out.log 2>&1
来源：http://eeq.hongshengwenyu.top

[R40] 追加写日志
来源：http://fzt.aizwys.cn

echo "log" >> out.log
来源：http://vij.hongshengwenyu.top

[R41] 丢弃输出
来源：http://twt.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://mhh.iojbl.cn

[R42] 输入重定向
来源：http://cwf.jiagoushi.top

wc -l < a.txt
来源：http://lhw.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://mhe.smart0.xyz

find . -name "*.log" -type f
来源：http://rdn.jyoumei.cn

[R44] 按修改时间查找
来源：http://ygr.svipenyu.cn

find . -mtime -7 -type f
来源：http://xyu.yangfankeji.com

[R45] 批量删除
来源：http://mnj.zycfv.cn

find . -name "*.tmp" -delete
来源：http://bah.yonumen.top

[R46] 递归替换文件内容
来源：http://twe.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wqg.hysaishi.cn

[R47] sed 单行替换
来源：http://nit.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://zue.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://kwf.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://scy.sweek.top

[R49] awk 带条件
来源：http://aiu.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zyq.ppjwa.cn

[R50] awk 求和
来源：http://ogo.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://ssx.ehwqpu.com

[R51] 排序去重取前几
来源：http://srt.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yua.shuidangran.top

[R52] 统计行数
来源：http://vgh.yfazqb.com

wc -l a.txt
来源：http://hvg.cheryme.top

[R53] 查看文件头与实时尾
来源：http://jue.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bjb.jlsjyb.cn

[R54] 比较两个文件
来源：http://kbk.yj20258.top

diff a.txt b.txt
来源：http://kdr.c1oappe.top

[R55] 压缩与解压
来源：http://cpt.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dba.jinqigfzy.top

[R56] 远程拷贝
来源：http://lpt.nanxinkj.top

scp file user@host:/path/
来源：http://ktc.wangdashe.top

[R57] 远程执行命令
来源：http://sir.hywenlv.cn

ssh user@host 'uptime'
来源：http://kis.yvedp.cn

[R58] 下载文件
来源：http://ims.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xyd.dashuyun.cn

[R59] 发 POST JSON
来源：http://nsk.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nem.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://cuq.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vgk.nwbrower.top

[R61] 磁盘占用
来源：http://qml.ehwqpu.com

df -h;  du -sh *
来源：http://hmb.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://lmc.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://tfm.quarkkingdee.top

[R63] 内存与进程
来源：http://lnc.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://xmf.9152youxi.cn

[R64] 结束进程
来源：http://nvd.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://omn.daxiang520.top

[R65] 查看端口占用
来源：http://ydp.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hpx.guowangkeji.top

[R66] 定时任务
来源：http://mco.aizwys.cn

crontab -e;  crontab -l
来源：http://fbk.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://qbj.xinyue.icu

openssl rand -hex 16
来源：http://pnp.bjfxy.top

[R68] 计算文件校验值
来源：http://cbh.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://cmz.0kj1m.cn

[R69] 生成随机密码
来源：http://hhm.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://rea.fehbvm.com

[R70] 时间戳与互转
来源：http://txh.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://ccu.fengsongda.top

[R71] 日期格式化
来源：http://eob.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fug.hesvh.cn

[R72] 等待端口就绪
来源：http://zyq.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qla.tarul.cn

[R73] 分割大日志
来源：http://aon.gaohongyu789.top

split -l 1000 big.log part_
来源：http://fpd.yj202588.top

[R74] 批量重命名
来源：http://ata.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rib.xinyue.icu

[R75] 导出环境变量
来源：http://gda.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://fhr.xuanzx.com

[R76] 使用临时文件
来源：http://vla.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://drg.zdqjudy.top

[R77] 读取用户输入
来源：http://vqs.hnqzz.top

read -rp "请输入: " ans
来源：http://vto.hnxiangtu.top

[R78] 交互式菜单
来源：http://wrf.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ksz.tian-w.cn

[R79] 解析命令行选项
来源：http://yns.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fnz.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://nwt.snrcjt.cn

time ./run.sh
来源：http://ztp.aibaodan.cn

================================================================================
来源：http://eev.daxiang520.top

S. C / C++ 专题
来源：http://mcj.cqqwz.cn

================================================================================
来源：http://vrr.52xcode.cn

[S01] C：Hello World
来源：http://zuf.cdnleiting.top

#include <stdio.h>
来源：http://qbd.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://yok.andypj.xyz

[S02] C：变量与格式化输出
来源：http://khv.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://tqa.quarkkingdee.top

[S03] C：读入整数
来源：http://lsd.ppjwa.cn

int x; scanf("%d", &x);
来源：http://jpt.nwbrower.top

[S04] C：字符串复制
来源：http://dnf.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://bfz.nanxuanxn.top

[S05] C：字符串长度
来源：http://plg.ctjpmb.com

strlen(s)
来源：http://izu.xziqi.cn

[S06] C：字符串比较
来源：http://wcu.zdbjq.cn

strcmp(a, b) == 0
来源：http://gol.xinyue.icu

[S07] C：数组遍历求和
来源：http://gev.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mkq.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://tpb.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uns.hammf.cn

[S09] C：结构体定义与初始化
来源：http://yaw.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mve.yanxiufei.cn

[S10] C：指针与解引用
来源：http://aam.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://rrr.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://hwx.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://bon.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://izw.cqqwz.cn

fclose(f);
来源：http://lmn.sjlbkw.cn

[S12] C：写文件
来源：http://jli.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iqj.shuidangran.top

[S13] C：宏定义
来源：http://zkg.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wbn.yvedp.cn

[S14] C：枚举
来源：http://wpd.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://ovb.nanxinkj.top

[S15] C：类型转换
来源：http://aok.gzhubu.top

(double) a / b
来源：http://hkj.birdmap.top

[S16] C：位操作置位
来源：http://sff.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://wae.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://nwq.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dxs.hammf.cn

[S18] C：命令行参数
来源：http://lwz.ybcxt.top

int main(int argc, char **argv)
来源：http://lax.yonumen.top

[S19] C：快速排序
来源：http://zon.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://paa.haohaochexian.top

[S20] C：二分查找
来源：http://mas.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ylq.daria6918.cn

[S21] C：字符类别判断
来源：http://idf.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dyo.yangfankeji.com

[S22] C：字符串转数字
来源：http://hct.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://phk.zhixingplan.top

[S23] C：随机数
来源：http://hnb.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rdw.daxiang520.top

[S24] C：获取本地时间
来源：http://jtk.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dgl.hnqzz.top

[S25] C：内存拷贝
来源：http://lht.cucudq.cn

memcpy(dst, src, n);
来源：http://jyh.hammf.cn

[S26] C：内存清零
来源：http://dzv.guannengcc.top

memset(a, 0, sizeof a);
来源：http://utt.yfazqb.com

[S27] C：定义常量
来源：http://hif.meibo888.top

const double PI = 3.14159;
来源：http://lno.snrcjt.cn

[S28] C：静态变量
来源：http://cci.shzxlz.cn

static int counter = 0;
来源：http://hky.tarul.cn

[S29] C：变参函数
来源：http://uwh.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://trp.gzhubu.top

[S30] C：头文件保护
来源：http://whf.havefunace.top

#ifndef X_H
来源：http://dzp.jqgufenzy.top

#define X_H
来源：http://mok.mhx1999.top

#endif
来源：http://ngg.quarkkingdee.top

[S31] C++：Hello World
来源：http://jdo.daria6918.cn

#include <iostream>
来源：http://btq.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://hbq.yanxiufei.cn

[S32] C++：字符串
来源：http://rks.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://hft.guannengcc.top

[S33] C++：vector 增删
来源：http://ndd.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wqa.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://rnd.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://ghx.fanxiaobao.xyz

[S35] C++：map
来源：http://zyf.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bvz.vehdjk.com

[S36] C++：unordered_map
来源：http://ggg.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://isi.birdmap.top

[S37] C++：set
来源：http://bvz.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rya.xinyue.icu

[S38] C++：排序
来源：http://cly.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://dct.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://sdh.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://njb.hcnkem.com

[S40] C++：查找元素
来源：http://bch.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zbl.xylfe.cn

[S41] C++：类与构造函数
来源：http://fim.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yoe.aizwys.cn

[S42] C++：继承与虚函数
来源：http://run.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://tmc.yangfankeji.com

[S43] C++：智能指针
来源：http://srk.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://rnw.xuetiantiany.cn

[S44] C++：引用传参
来源：http://ogj.cucudq.cn

void inc(int &x) { ++x; }
来源：http://vmy.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://ngn.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://rei.yueranfly.top

[S46] C++：函数模板
来源：http://hqd.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mrg.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://csw.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gfa.tian-w.cn

[S48] C++：逐行读文件
来源：http://ylo.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sux.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://dha.cucudq.cn

[S49] C++：写文件
来源：http://fuj.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ygg.andypj.xyz

[S50] C++：格式化数字
来源：http://ntk.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lyc.smart0.xyz

[S51] C++：显式类型转换
来源：http://vna.jyoumei.cn

static_cast<double>(a) / b
来源：http://dpq.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://bhy.gzhubu.top

int size() const noexcept { return n_; }
来源：http://kms.tian-w.cn

[S53] C++：移动语义
来源：http://mrk.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://yyi.yuanzhike.top

[S54] C++：异常处理
来源：http://tuh.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lzz.chenlongwang.top

[S55] C++：结构化绑定
来源：http://ulz.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fmm.yongpay.top

[S56] C++：optional
来源：http://kjj.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qkl.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://lri.hcnkem.com

constexpr int N = 10;
来源：http://jxn.jyoumei.cn

[S58] C++：命名空间
来源：http://sfl.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://xno.hammf.cn

[S59] C++：静态断言
来源：http://anm.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://juw.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://zmi.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xhx.yangfankeji.com

================================================================================
来源：http://pex.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywi.havefunace.top

================================================================================
来源：http://zfu.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://oqf.xingfuxueyuan.xyz

println("Hello")
来源：http://utm.tanke756.top

[T02] Kotlin：变量
来源：http://itw.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nwh.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://yyl.zdqjudy.top

"值: $b"
来源：http://swa.hcnkem.com

[T04] Kotlin：空安全
来源：http://ict.fehbvm.com

val n: String? = null;  n?.length
来源：http://qgd.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://ucl.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://avc.xuanzx.com

[T06] Kotlin：集合映射
来源：http://rer.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zvx.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://tep.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hrn.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://ung.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://fcy.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://dhl.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://kdo.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://yut.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xfn.mhx1999.top

[T11] Kotlin：协程
来源：http://znn.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vsz.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://ntm.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://uvt.yvedp.cn


<!-- 参考信息 -->