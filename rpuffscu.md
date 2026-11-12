代发 wailian999

case "$1" in
来源：http://tdj.cdnleiting.top

start) echo "启动" ;;
来源：http://ele.chenlongwang.top

stop)  echo "停止" ;;
来源：http://xdk.nwbrower.top

*)     echo "未知命令" ;;
来源：http://oyk.yj20258.top

esac
来源：http://hsz.dianchejie.cn

[R12] for 遍历文件
来源：http://sjb.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://him.hywenlv.cn

[R13] for 计数循环
来源：http://jvl.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://nwx.hesvh.cn

[R14] C 风格 for
来源：http://kod.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pgd.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://omz.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pkl.jinqigfzy.top

[R16] until 等待条件
来源：http://otq.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tch.cheryme.top

[R17] 数组定义与取值
来源：http://xlm.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vzf.quarkkingdee.top

[R18] 遍历数组
来源：http://ntr.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://llt.shzxlz.cn

[R19] 数组长度
来源：http://uzz.pycfn.com

echo "${#arr[@]}"
来源：http://aix.yj202588.top

[R20] 关联数组（字典）
来源：http://gab.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yxp.shzxlz.cn

[R21] 字符串长度
来源：http://oti.yonumen.top

echo "${#s}"
来源：http://hca.bjfxy.top

[R22] 截取子串
来源：http://azf.zhiwuduotai.top

echo "${s:0:5}"
来源：http://aby.xuanzx.com

[R23] 字符串替换
来源：http://fir.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ksr.zhengqikj.top

[R24] 大小写转换
来源：http://nji.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vvf.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://bii.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rgx.wangdashe.top

[R26] 命令替换
来源：http://mmf.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://sxe.hammf.cn

[R27] 算术展开
来源：http://tzl.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://oge.nanxinkj.top

[R28] 浮点运算
来源：http://uke.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://ltd.sysykeji.top

[R29] 定义函数
来源：http://vga.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xgu.gzhubu.top

[R30] 函数返回状态码
来源：http://fvd.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://coo.ybcxt.top

[R31] 局部变量
来源：http://lhz.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://yoc.vehdjk.com

[R32] 参数个数校验
来源：http://qds.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ipv.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://uyq.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aws.jqgufenzy.top

[R34] 退出时清理
来源：http://yxt.bjfxy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ccq.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://goo.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vzv.wangdashe.top

[R36] 并发执行多个任务
来源：http://nrs.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbm.birdmap.top

[R37] 把输出赋给变量
来源：http://zqw.daxiang520.top

files=$(ls -1)
来源：http://lhs.tian-w.cn

[R38] 管道串联
来源：http://kfb.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://foa.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://pcs.xziqi.cn

cmd > out.log 2>&1
来源：http://nmv.wangshuangyany.cn

[R40] 追加写日志
来源：http://nyd.gotoacloud.top

echo "log" >> out.log
来源：http://cey.hesvh.cn

[R41] 丢弃输出
来源：http://zdi.vehdjk.com

cmd >/dev/null 2>&1
来源：http://tig.ppjwa.cn

[R42] 输入重定向
来源：http://uxg.yanxiufei.cn

wc -l < a.txt
来源：http://vzc.meibo888.top

[R43] 按名字查找文件
来源：http://nsg.hcnkem.com

find . -name "*.log" -type f
来源：http://gea.bbcook.cn

[R44] 按修改时间查找
来源：http://thb.dashuyun.cn

find . -mtime -7 -type f
来源：http://rys.ywan-chungtsiang.top

[R45] 批量删除
来源：http://bzw.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://fhx.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://odk.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gkm.jiagoushi.top

[R47] sed 单行替换
来源：http://rcw.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://jdj.ybcxt.top

[R48] awk 取指定列
来源：http://num.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://sos.andypj.xyz

[R49] awk 带条件
来源：http://sdt.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://adj.xziqi.cn

[R50] awk 求和
来源：http://qyc.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pck.zhijiandao.cn

[R51] 排序去重取前几
来源：http://kzt.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://psk.chenlongwang.top

[R52] 统计行数
来源：http://bhb.svipenyu.cn

wc -l a.txt
来源：http://app.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://cpb.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sah.jqgufenzy.top

[R54] 比较两个文件
来源：http://hwy.bbcook.cn

diff a.txt b.txt
来源：http://avp.shzxlz.cn

[R55] 压缩与解压
来源：http://oft.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tuz.zhoulong.xyz

[R56] 远程拷贝
来源：http://elj.zhijiandao.cn

scp file user@host:/path/
来源：http://lha.epnwcf.com

[R57] 远程执行命令
来源：http://rsu.jqgfzy.top

ssh user@host 'uptime'
来源：http://kcg.nanxuanxn.top

[R58] 下载文件
来源：http://afv.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vpz.sweek.top

[R59] 发 POST JSON
来源：http://daz.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vic.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://vlg.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qmi.zycfv.cn

[R61] 磁盘占用
来源：http://frh.shangyingyoupin.top

df -h;  du -sh *
来源：http://feo.hysaishi.cn

[R62] 找最占空间的文件
来源：http://wvu.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://upm.wangshuangyany.cn

[R63] 内存与进程
来源：http://qtx.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://iwr.yfazqb.com

[R64] 结束进程
来源：http://beh.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://crc.c1oappe.top

[R65] 查看端口占用
来源：http://bae.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vrr.yj20258.top

[R66] 定时任务
来源：http://jyx.redwolf501.top

crontab -e;  crontab -l
来源：http://jqt.yfazqb.com

[R67] 生成随机十六进制串
来源：http://dwj.316326.xyz

openssl rand -hex 16
来源：http://hai.ybcxt.top

[R68] 计算文件校验值
来源：http://kwj.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://ydw.wangshuangyany.cn

[R69] 生成随机密码
来源：http://lgm.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://wmg.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://ady.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://zgk.aizwys.cn

[R71] 日期格式化
来源：http://tkp.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ojv.guowangkeji.top

[R72] 等待端口就绪
来源：http://hbb.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yup.jyoumei.cn

[R73] 分割大日志
来源：http://cbw.fengsongda.top

split -l 1000 big.log part_
来源：http://rln.xinyue.icu

[R74] 批量重命名
来源：http://spf.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mgu.9152youxi.cn

[R75] 导出环境变量
来源：http://dna.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://qss.zhijiandao.cn

[R76] 使用临时文件
来源：http://ggn.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fms.hywenlv.cn

[R77] 读取用户输入
来源：http://hft.zdqjudy.top

read -rp "请输入: " ans
来源：http://www.c1oappe.top

[R78] 交互式菜单
来源：http://woe.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sdu.zhoulong.xyz

[R79] 解析命令行选项
来源：http://saa.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oln.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://ksk.yvedp.cn

time ./run.sh
来源：http://tpc.birdmap.top

================================================================================
来源：http://kpv.gotoacloud.top

S. C / C++ 专题
来源：http://ego.ctjpmb.com

================================================================================
来源：http://uqw.vehdjk.com

[S01] C：Hello World
来源：http://zio.aizwys.cn

#include <stdio.h>
来源：http://mgf.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hok.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://nmj.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://ynu.c1oappe.top

[S03] C：读入整数
来源：http://dpf.bbcook.cn

int x; scanf("%d", &x);
来源：http://ygz.xuetiantiany.cn

[S04] C：字符串复制
来源：http://cru.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ade.quarkkingdee.top

[S05] C：字符串长度
来源：http://dzr.zycfv.cn

strlen(s)
来源：http://nwz.svipenyu.cn

[S06] C：字符串比较
来源：http://xjn.ybcxt.top

strcmp(a, b) == 0
来源：http://rdj.zycfv.cn

[S07] C：数组遍历求和
来源：http://oes.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vcj.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://gad.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ukk.cheryme.top

[S09] C：结构体定义与初始化
来源：http://wdr.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qma.xuetiantiany.cn

[S10] C：指针与解引用
来源：http://div.meibo888.top

int *p = &a;  *p = 5;
来源：http://zcd.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://gsh.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://xdo.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://cmd.andypj.xyz

fclose(f);
来源：http://kxp.uphjek.com

[S12] C：写文件
来源：http://nxd.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hxa.fzhhl.top

[S13] C：宏定义
来源：http://nhr.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hcx.zhiwuduotai.top

[S14] C：枚举
来源：http://svj.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://nli.yj20258.top

[S15] C：类型转换
来源：http://cal.hywenlv.cn

(double) a / b
来源：http://iio.0kj1m.cn

[S16] C：位操作置位
来源：http://rnl.yonumen.top

x |= (1 << 3);
来源：http://xcl.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://fce.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sfz.zycfv.cn

[S18] C：命令行参数
来源：http://imv.yj202588.top

int main(int argc, char **argv)
来源：http://zst.yj20258.top

[S19] C：快速排序
来源：http://bjq.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://cnf.hnxiangtu.top

[S20] C：二分查找
来源：http://znt.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zet.aibaodan.cn

[S21] C：字符类别判断
来源：http://vlu.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gqa.yvedp.cn

[S22] C：字符串转数字
来源：http://wla.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://okw.uphjek.com

[S23] C：随机数
来源：http://ssi.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ssr.yonumen.top

[S24] C：获取本地时间
来源：http://grr.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dmb.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://nsy.yongpay.top

memcpy(dst, src, n);
来源：http://qxj.jlsjyb.cn

[S26] C：内存清零
来源：http://pgw.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://uvg.nanxuanxn.top

[S27] C：定义常量
来源：http://ill.pycfn.com

const double PI = 3.14159;
来源：http://snw.ivvv.top

[S28] C：静态变量
来源：http://vhi.tanke756.top

static int counter = 0;
来源：http://zgi.ybcxt.top

[S29] C：变参函数
来源：http://uqx.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sxr.redwolf501.top

[S30] C：头文件保护
来源：http://sug.zhaomingkeji.xyz

#ifndef X_H
来源：http://gzq.nwbrower.top

#define X_H
来源：http://xmk.quarkkingdee.top

#endif
来源：http://ffs.jiagoushi.top

[S31] C++：Hello World
来源：http://pdu.ctjpmb.com

#include <iostream>
来源：http://exo.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://sow.dianchejie.cn

[S32] C++：字符串
来源：http://jmm.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://uhs.nwbrower.top

[S33] C++：vector 增删
来源：http://edp.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://phi.yj20258888.top

[S34] C++：遍历 vector
来源：http://iwb.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://zqs.iojbl.cn

[S35] C++：map
来源：http://qvr.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nib.jinqigfzy.top

[S36] C++：unordered_map
来源：http://qal.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zsc.shzxlz.cn

[S37] C++：set
来源：http://zhc.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mvf.cqqwz.cn

[S38] C++：排序
来源：http://bjr.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://brr.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://ncm.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://itr.gaohongyu789.top

[S40] C++：查找元素
来源：http://mgf.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bsd.nwbrower.top

[S41] C++：类与构造函数
来源：http://klg.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lse.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://dar.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://ehi.tian-w.cn

[S43] C++：智能指针
来源：http://jwv.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://vmx.chenjidiqi.icu

[S44] C++：引用传参
来源：http://tka.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://zjy.kuanghao11.cn

[S45] C++：lambda
来源：http://ejk.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://khc.hywenlv.cn

[S46] C++：函数模板
来源：http://xkv.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://twx.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://ppt.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dxm.gzhubu.top

[S48] C++：逐行读文件
来源：http://uxt.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qcs.smart0.xyz

while (std::getline(in, line)) { }
来源：http://lab.fehbvm.com

[S49] C++：写文件
来源：http://akz.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xau.hnxiangtu.top

[S50] C++：格式化数字
来源：http://bzq.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yaq.svipenyu.cn

[S51] C++：显式类型转换
来源：http://alk.fehbvm.com

static_cast<double>(a) / b
来源：http://jyb.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://tvb.cucudq.cn

int size() const noexcept { return n_; }
来源：http://fzz.zdqjudy.top

[S53] C++：移动语义
来源：http://bpb.tarul.cn

std::vector<int> w = std::move(v);
来源：http://atc.jqgufenzy.top

[S54] C++：异常处理
来源：http://slz.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eeh.cdnleiting.top

[S55] C++：结构化绑定
来源：http://dcw.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kvj.yuanzhike.top

[S56] C++：optional
来源：http://kpa.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ziv.zhijiandao.cn

[S57] C++：编译期常量
来源：http://vfb.hesvh.cn

constexpr int N = 10;
来源：http://pch.yangfankeji.com

[S58] C++：命名空间
来源：http://lru.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://gct.ehwqpu.com

[S59] C++：静态断言
来源：http://opw.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fxd.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://hnu.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vut.feifeiyinyue.top

================================================================================
来源：http://zqq.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wgg.yj202588.top

================================================================================
来源：http://qqy.yonumen.top

[T01] Kotlin：Hello World
来源：http://olk.jqgfzy.top

println("Hello")
来源：http://itk.zycfv.cn

[T02] Kotlin：变量
来源：http://rmn.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pzn.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://htk.zdqjudy.top

"值: $b"
来源：http://afa.iojbl.cn

[T04] Kotlin：空安全
来源：http://lby.tianlin.xyz

val n: String? = null;  n?.length
来源：http://ent.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://yus.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kdx.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://yco.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pbp.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://iyi.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://blo.guowangkeji.top

[T08] Kotlin：数据类
来源：http://slz.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://cvm.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://aaa.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://ylb.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://atz.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://faz.jqgfzy.top

[T11] Kotlin：协程
来源：http://gnk.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jea.mhx1999.top

[T12] Kotlin：解构声明
来源：http://whs.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://pna.vehdjk.com


<!-- 参考信息 -->