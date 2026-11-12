代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rvp.daxiang520.top

[R10] 正则匹配
来源：http://fmh.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kpn.uphjek.com

[R11] case 多分支
来源：http://sha.gaohongyu789.top

case "$1" in
来源：http://uyk.9152youxi.cn

start) echo "启动" ;;
来源：http://ibv.ehwqpu.com

stop)  echo "停止" ;;
来源：http://mqg.yj202588.top

*)     echo "未知命令" ;;
来源：http://sbu.sweek.top

esac
来源：http://ngz.yangfankeji.com

[R12] for 遍历文件
来源：http://jvm.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://kvp.shangyingyoupin.top

[R13] for 计数循环
来源：http://lui.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://gxf.jqgufenzy.top

[R14] C 风格 for
来源：http://ews.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hyp.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://zik.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hum.daxiang520.top

[R16] until 等待条件
来源：http://vhf.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zpt.yanxiufei.cn

[R17] 数组定义与取值
来源：http://bln.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mfu.chenlongwang.top

[R18] 遍历数组
来源：http://ynw.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpx.yangfankeji.com

[R19] 数组长度
来源：http://moj.kuanghao11.cn

echo "${#arr[@]}"
来源：http://ffj.chenlongwang.top

[R20] 关联数组（字典）
来源：http://nuj.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lcq.havefunace.top

[R21] 字符串长度
来源：http://pzo.316326.xyz

echo "${#s}"
来源：http://kal.shzxlz.cn

[R22] 截取子串
来源：http://hmd.jyoumei.cn

echo "${s:0:5}"
来源：http://iyo.ybcxt.top

[R23] 字符串替换
来源：http://aqe.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hvh.cashguo.top

[R24] 大小写转换
来源：http://rqh.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sav.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://ihh.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://grb.smart0.xyz

[R26] 命令替换
来源：http://usm.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://xip.jinqigufen.top

[R27] 算术展开
来源：http://hay.fehbvm.com

echo $((1 + 2 * 3))
来源：http://nol.gogol.net.cn

[R28] 浮点运算
来源：http://etx.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://adn.pengpengdd.cyou

[R29] 定义函数
来源：http://kjh.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vwq.iojbl.cn

[R30] 函数返回状态码
来源：http://mdc.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://dui.cqqwz.cn

[R31] 局部变量
来源：http://xkt.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://god.jinqigufen.top

[R32] 参数个数校验
来源：http://ues.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yad.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://mdr.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjp.vehdjk.com

[R34] 退出时清理
来源：http://itw.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://uoh.gaohongyu789.top

[R35] 后台执行并等待
来源：http://tnw.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hfg.ivvv.top

[R36] 并发执行多个任务
来源：http://dsh.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sfn.cqqwz.cn

[R37] 把输出赋给变量
来源：http://muc.zhongyouzk.top

files=$(ls -1)
来源：http://vvm.fengsongda.top

[R38] 管道串联
来源：http://cru.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://vrl.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://uwx.havefunace.top

cmd > out.log 2>&1
来源：http://upg.dianchejie.cn

[R40] 追加写日志
来源：http://ztp.xuanzx.com

echo "log" >> out.log
来源：http://qwh.guannengcc.top

[R41] 丢弃输出
来源：http://fsm.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://jae.c1oappe.top

[R42] 输入重定向
来源：http://omm.chenjidiqi.icu

wc -l < a.txt
来源：http://rfn.hysaishi.cn

[R43] 按名字查找文件
来源：http://ruq.zhixingplan.top

find . -name "*.log" -type f
来源：http://joi.xziqi.cn

[R44] 按修改时间查找
来源：http://llx.uphjek.com

find . -mtime -7 -type f
来源：http://dtx.tianlin.xyz

[R45] 批量删除
来源：http://myd.uphjek.com

find . -name "*.tmp" -delete
来源：http://srs.ctjpmb.com

[R46] 递归替换文件内容
来源：http://rqm.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fgx.ppjwa.cn

[R47] sed 单行替换
来源：http://xhu.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://gto.yj20258888.top

[R48] awk 取指定列
来源：http://jad.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://idc.yj202588.top

[R49] awk 带条件
来源：http://zdm.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rho.c1oappe.top

[R50] awk 求和
来源：http://hxm.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://wpe.jiagoushi.top

[R51] 排序去重取前几
来源：http://inn.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gzj.ivvv.top

[R52] 统计行数
来源：http://maf.xinyue.icu

wc -l a.txt
来源：http://fai.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://ryg.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kih.yonumen.top

[R54] 比较两个文件
来源：http://cly.jqgufenzy.top

diff a.txt b.txt
来源：http://mzc.gotoacloud.top

[R55] 压缩与解压
来源：http://kwu.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hzm.pycfn.com

[R56] 远程拷贝
来源：http://qrf.52xcode.cn

scp file user@host:/path/
来源：http://qbe.cqqwz.cn

[R57] 远程执行命令
来源：http://anr.zdqjudy.top

ssh user@host 'uptime'
来源：http://npz.yonumen.top

[R58] 下载文件
来源：http://sjh.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xpz.hcnkem.com

[R59] 发 POST JSON
来源：http://rhe.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://drt.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://uxz.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jam.shuidangran.top

[R61] 磁盘占用
来源：http://cvu.fktsv.cn

df -h;  du -sh *
来源：http://rtf.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://qbb.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://aew.cucudq.cn

[R63] 内存与进程
来源：http://lkx.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://kmp.hesvh.cn

[R64] 结束进程
来源：http://ssu.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://lnz.fengsongda.top

[R65] 查看端口占用
来源：http://qua.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wbe.redwolf501.top

[R66] 定时任务
来源：http://ayd.shzxlz.cn

crontab -e;  crontab -l
来源：http://pyc.uphjek.com

[R67] 生成随机十六进制串
来源：http://gbn.hnqzz.top

openssl rand -hex 16
来源：http://tjb.nanxuanxn.top

[R68] 计算文件校验值
来源：http://xlg.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pwj.tarul.cn

[R69] 生成随机密码
来源：http://zbh.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://wgi.yvedp.cn

[R70] 时间戳与互转
来源：http://tpm.yj20258.top

date +%s;  date -d @1700000000
来源：http://mzl.kuanghao11.cn

[R71] 日期格式化
来源：http://nqm.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvl.hywenlv.cn

[R72] 等待端口就绪
来源：http://rbk.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uto.hnxiangtu.top

[R73] 分割大日志
来源：http://lif.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://ivm.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://snm.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://byy.zhijiandao.cn

[R75] 导出环境变量
来源：http://fsv.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://zzv.9152youxi.cn

[R76] 使用临时文件
来源：http://arz.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yqo.cheryme.top

[R77] 读取用户输入
来源：http://foy.ydjk.org.cn

read -rp "请输入: " ans
来源：http://tum.yonumen.top

[R78] 交互式菜单
来源：http://jxa.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tjt.xuanzx.com

[R79] 解析命令行选项
来源：http://zri.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mpe.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://who.tanke756.top

time ./run.sh
来源：http://wqv.cdnleiting.top

================================================================================
来源：http://smc.haohaochexian.top

S. C / C++ 专题
来源：http://wak.iojbl.cn

================================================================================
来源：http://bys.ppjwa.cn

[S01] C：Hello World
来源：http://hca.ctjpmb.com

#include <stdio.h>
来源：http://grt.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mjf.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://exw.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://pvj.yuxming.cn

[S03] C：读入整数
来源：http://jae.smart0.xyz

int x; scanf("%d", &x);
来源：http://fra.daria6918.cn

[S04] C：字符串复制
来源：http://cuo.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wjx.chenlongwang.top

[S05] C：字符串长度
来源：http://qdv.tianlin.xyz

strlen(s)
来源：http://mip.quarkkingdee.top

[S06] C：字符串比较
来源：http://tmj.cheryme.top

strcmp(a, b) == 0
来源：http://rlb.yvedp.cn

[S07] C：数组遍历求和
来源：http://ijx.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bxe.cashguo.top

[S08] C：动态内存分配与释放
来源：http://urk.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://obm.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://viw.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vyw.guannengcc.top

[S10] C：指针与解引用
来源：http://gge.hnqzz.top

int *p = &a;  *p = 5;
来源：http://inc.chenlongwang.top

[S11] C：逐行读文件
来源：http://eca.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://rjy.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xef.sweek.top

fclose(f);
来源：http://ipj.fktsv.cn

[S12] C：写文件
来源：http://dtc.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rlh.shuidangran.top

[S13] C：宏定义
来源：http://dzp.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cfi.hfpthk.cn

[S14] C：枚举
来源：http://ktu.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://iao.sufxvd.cn

[S15] C：类型转换
来源：http://bzx.vqdsnc.cn

(double) a / b
来源：http://nlq.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://yfl.yanxiufei.cn

x |= (1 << 3);
来源：http://znh.zycfv.cn

[S17] C：安全拼接字符串
来源：http://tcr.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uxh.zdbjq.cn

[S18] C：命令行参数
来源：http://ogu.guowangkeji.top

int main(int argc, char **argv)
来源：http://xif.chenzaomai.com

[S19] C：快速排序
来源：http://sbu.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://okd.fzhhl.top

[S20] C：二分查找
来源：http://ork.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://flc.yuanzhike.top

[S21] C：字符类别判断
来源：http://zwf.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://toi.mhx1999.top

[S22] C：字符串转数字
来源：http://lll.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kmy.iojbl.cn

[S23] C：随机数
来源：http://qrs.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://prj.birdmap.top

[S24] C：获取本地时间
来源：http://acu.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xbw.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://sfv.snrcjt.cn

memcpy(dst, src, n);
来源：http://wsi.nanxinkj.top

[S26] C：内存清零
来源：http://mjr.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://ruz.zhoulong.xyz

[S27] C：定义常量
来源：http://knj.xziqi.cn

const double PI = 3.14159;
来源：http://cuf.guowangkeji.top

[S28] C：静态变量
来源：http://jdr.yj20258.top

static int counter = 0;
来源：http://djt.meibo888.top

[S29] C：变参函数
来源：http://nln.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kgz.yj202588.top

[S30] C：头文件保护
来源：http://hmt.ydjk.org.cn

#ifndef X_H
来源：http://tnt.jqgufenzy.top

#define X_H
来源：http://yjj.daxiang520.top

#endif
来源：http://lfe.sysykeji.top

[S31] C++：Hello World
来源：http://jgz.yj20258888.top

#include <iostream>
来源：http://xnb.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://ovu.mhx1999.top

[S32] C++：字符串
来源：http://ssp.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://xsk.jiagoushi.top

[S33] C++：vector 增删
来源：http://ami.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xxb.gogol.net.cn

[S34] C++：遍历 vector
来源：http://wmo.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://qib.xuetiantiany.cn

[S35] C++：map
来源：http://qdt.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xob.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://piu.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://erk.fehbvm.com

[S37] C++：set
来源：http://tum.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://srz.jinyuanbaomall.cn

[S38] C++：排序
来源：http://gnh.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://vig.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://wgn.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qaz.jianghu66.top

[S40] C++：查找元素
来源：http://nfy.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bqs.yongpay.top

[S41] C++：类与构造函数
来源：http://ipz.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dhk.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://peh.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://fsj.zhengqikj.top

[S43] C++：智能指针
来源：http://zbu.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://dsb.meibo888.top

[S44] C++：引用传参
来源：http://dpn.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://wkn.chenzaomai.com

[S45] C++：lambda
来源：http://zbu.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gtd.aizwys.cn

[S46] C++：函数模板
来源：http://oix.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://akk.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://vhz.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://djt.hammf.cn

[S48] C++：逐行读文件
来源：http://pzi.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://imw.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://qnr.fehbvm.com

[S49] C++：写文件
来源：http://cxb.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pyy.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://snt.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vay.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://wre.sysykeji.top

static_cast<double>(a) / b
来源：http://dso.tanke756.top

[S52] C++：const 与 noexcept
来源：http://bgc.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://eng.yj20258.top

[S53] C++：移动语义
来源：http://unr.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://tgn.yvedp.cn

[S54] C++：异常处理
来源：http://orw.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qry.smart0.xyz

[S55] C++：结构化绑定
来源：http://wki.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hxl.zycfv.cn

[S56] C++：optional
来源：http://yya.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hse.mhx1999.top

[S57] C++：编译期常量
来源：http://uwh.zhijiandao.cn

constexpr int N = 10;
来源：http://skg.shuidangran.top

[S58] C++：命名空间
来源：http://tgs.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://apg.xinyue.icu

[S59] C++：静态断言
来源：http://yhw.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qfv.meibo888.top

[S60] C++：遍历并删除元素
来源：http://rdf.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lwc.cdnleiting.top

================================================================================
来源：http://qqj.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cmc.jinyuanbaomall.cn

================================================================================
来源：http://bbb.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://vdl.tianlin.xyz

println("Hello")
来源：http://wls.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://tck.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://adc.sweek.top

[T03] Kotlin：字符串模板
来源：http://ufe.shanyushiyangtech.top

"值: $b"
来源：http://nil.316326.xyz

[T04] Kotlin：空安全
来源：http://mdh.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://ukc.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://zqy.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://smp.shuidangran.top

[T06] Kotlin：集合映射
来源：http://kms.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://ryb.tanke756.top

[T07] Kotlin：集合过滤
来源：http://hkv.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://owa.yuanzhike.top

[T08] Kotlin：数据类
来源：http://yok.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://poa.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://hii.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://lyi.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://mue.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rbg.xziqi.cn


<!-- 参考信息 -->