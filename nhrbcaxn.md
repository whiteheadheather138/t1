代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zfh.gzhubu.top

[R16] until 等待条件
来源：http://lii.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vra.jqgufenzy.top

[R17] 数组定义与取值
来源：http://llg.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fpw.fzhhl.top

[R18] 遍历数组
来源：http://axy.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cub.zdqjudy.top

[R19] 数组长度
来源：http://wer.nwbrower.top

echo "${#arr[@]}"
来源：http://rvo.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://lpz.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xpe.fzhhl.top

[R21] 字符串长度
来源：http://cab.yvedp.cn

echo "${#s}"
来源：http://max.ctjpmb.com

[R22] 截取子串
来源：http://qzl.0kj1m.cn

echo "${s:0:5}"
来源：http://uor.cqqwz.cn

[R23] 字符串替换
来源：http://der.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zld.shuidangran.top

[R24] 大小写转换
来源：http://toi.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://pfr.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://nqa.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ndg.shanyushiyangtech.top

[R26] 命令替换
来源：http://gmc.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://efd.hongshengwenyu.top

[R27] 算术展开
来源：http://fwy.fehbvm.com

echo $((1 + 2 * 3))
来源：http://ucm.sweek.top

[R28] 浮点运算
来源：http://zcz.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://qgg.hcnkem.com

[R29] 定义函数
来源：http://sjs.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://riv.nanxinkj.top

[R30] 函数返回状态码
来源：http://lwp.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://qjx.meibo888.top

[R31] 局部变量
来源：http://lvg.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://ppb.epnwcf.com

[R32] 参数个数校验
来源：http://zir.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mvs.ivvv.top

[R33] 捕获错误并提示行号
来源：http://neq.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ooi.fktsv.cn

[R34] 退出时清理
来源：http://ped.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://qfw.epnwcf.com

[R35] 后台执行并等待
来源：http://lxu.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kyo.yueranfly.top

[R36] 并发执行多个任务
来源：http://psm.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://opx.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://qvi.dashuyun.cn

files=$(ls -1)
来源：http://tez.aizwys.cn

[R38] 管道串联
来源：http://ddc.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://gfq.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://act.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://gtl.hnxiangtu.top

[R40] 追加写日志
来源：http://wgl.zycfv.cn

echo "log" >> out.log
来源：http://iid.ydzc1.top

[R41] 丢弃输出
来源：http://egh.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://dny.yonumen.top

[R42] 输入重定向
来源：http://lza.yanxiufei.cn

wc -l < a.txt
来源：http://wnk.yj20258.top

[R43] 按名字查找文件
来源：http://mmd.chenzaomai.com

find . -name "*.log" -type f
来源：http://kwk.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://mya.bjfxy.top

find . -mtime -7 -type f
来源：http://kof.shzxlz.cn

[R45] 批量删除
来源：http://mhy.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://zca.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://lwj.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qam.birdmap.top

[R47] sed 单行替换
来源：http://kdu.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://csg.guowangkeji.top

[R48] awk 取指定列
来源：http://nkd.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://sqz.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://axc.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://snp.epnwcf.com

[R50] awk 求和
来源：http://sgd.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://nea.xylfe.cn

[R51] 排序去重取前几
来源：http://jee.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jow.bbcook.cn

[R52] 统计行数
来源：http://vvf.nwbrower.top

wc -l a.txt
来源：http://ier.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://mob.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://idu.havefunace.top

[R54] 比较两个文件
来源：http://otx.hnxiangtu.top

diff a.txt b.txt
来源：http://pbu.sjlbkw.cn

[R55] 压缩与解压
来源：http://tml.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pnv.ybcxt.top

[R56] 远程拷贝
来源：http://mqq.kuanghao11.cn

scp file user@host:/path/
来源：http://ium.havefunace.top

[R57] 远程执行命令
来源：http://aag.sysykeji.top

ssh user@host 'uptime'
来源：http://urg.hcnkem.com

[R58] 下载文件
来源：http://rxa.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://njr.yongpay.top

[R59] 发 POST JSON
来源：http://nwf.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zoj.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://lob.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mlu.zhiwuduotai.top

[R61] 磁盘占用
来源：http://zjd.shuidangran.top

df -h;  du -sh *
来源：http://wva.yuxming.cn

[R62] 找最占空间的文件
来源：http://grl.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://grb.tian-w.cn

[R63] 内存与进程
来源：http://zyz.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://lwm.yanxiufei.cn

[R64] 结束进程
来源：http://bmi.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://sxc.hnqzz.top

[R65] 查看端口占用
来源：http://xxz.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ohy.vqdsnc.cn

[R66] 定时任务
来源：http://dar.jyoumei.cn

crontab -e;  crontab -l
来源：http://fvq.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://swc.uphjek.com

openssl rand -hex 16
来源：http://coi.svipenyu.cn

[R68] 计算文件校验值
来源：http://pny.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://ngu.yonumen.top

[R69] 生成随机密码
来源：http://mdo.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://yhm.yueranfly.top

[R70] 时间戳与互转
来源：http://nih.mhx1999.top

date +%s;  date -d @1700000000
来源：http://iih.smart0.xyz

[R71] 日期格式化
来源：http://twu.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sal.meibo888.top

[R72] 等待端口就绪
来源：http://gmb.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fau.dianchejie.cn

[R73] 分割大日志
来源：http://oiz.meibo888.top

split -l 1000 big.log part_
来源：http://kfw.c1oappe.top

[R74] 批量重命名
来源：http://txb.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ole.hywenlv.cn

[R75] 导出环境变量
来源：http://qeo.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://bgo.sweek.top

[R76] 使用临时文件
来源：http://aji.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://byf.zhongyouzk.top

[R77] 读取用户输入
来源：http://fof.dashuyun.cn

read -rp "请输入: " ans
来源：http://nxo.sysykeji.top

[R78] 交互式菜单
来源：http://lre.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uhw.0kj1m.cn

[R79] 解析命令行选项
来源：http://zbc.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://unm.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://jcs.ivvv.top

time ./run.sh
来源：http://fps.xuetiantiany.cn

================================================================================
来源：http://tyb.sjlbkw.cn

S. C / C++ 专题
来源：http://wzw.shzxlz.cn

================================================================================
来源：http://vuo.sweek.top

[S01] C：Hello World
来源：http://gsm.ywan-chungtsiang.top

#include <stdio.h>
来源：http://ukp.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tce.iojbl.cn

[S02] C：变量与格式化输出
来源：http://cdw.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://gwk.chenzaomai.com

[S03] C：读入整数
来源：http://trs.fengsongda.top

int x; scanf("%d", &x);
来源：http://aji.tarul.cn

[S04] C：字符串复制
来源：http://xlt.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rjb.hfpthk.cn

[S05] C：字符串长度
来源：http://hnl.tian-w.cn

strlen(s)
来源：http://eiq.birdmap.top

[S06] C：字符串比较
来源：http://nth.chenlongwang.top

strcmp(a, b) == 0
来源：http://nrm.svipenyu.cn

[S07] C：数组遍历求和
来源：http://dkh.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://laj.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://sro.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xyg.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://zke.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bfk.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://pcp.xziqi.cn

int *p = &a;  *p = 5;
来源：http://ovm.sjlbkw.cn

[S11] C：逐行读文件
来源：http://akc.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://lck.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tat.fanxiaobao.xyz

fclose(f);
来源：http://qyn.hnxiangtu.top

[S12] C：写文件
来源：http://ygd.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hwl.aizwys.cn

[S13] C：宏定义
来源：http://szh.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://crk.daria6918.cn

[S14] C：枚举
来源：http://ysh.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://eiu.9152youxi.cn

[S15] C：类型转换
来源：http://ivi.fanxiaobao.xyz

(double) a / b
来源：http://gqh.jiagoushi.top

[S16] C：位操作置位
来源：http://umi.sweek.top

x |= (1 << 3);
来源：http://xij.sxryk.cn

[S17] C：安全拼接字符串
来源：http://ulq.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jir.ivvv.top

[S18] C：命令行参数
来源：http://yfa.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://cfp.cashguo.top

[S19] C：快速排序
来源：http://wqc.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oov.dianchejie.cn

[S20] C：二分查找
来源：http://que.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://srp.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://idt.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qox.dashuyun.cn

[S22] C：字符串转数字
来源：http://mbc.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://emj.sjlbkw.cn

[S23] C：随机数
来源：http://gkq.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mnw.jianghu66.top

[S24] C：获取本地时间
来源：http://cms.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oss.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://cmd.yongpay.top

memcpy(dst, src, n);
来源：http://vgr.zycfv.cn

[S26] C：内存清零
来源：http://pjf.gzhubu.top

memset(a, 0, sizeof a);
来源：http://cex.zhiwuduotai.top

[S27] C：定义常量
来源：http://jea.nwbrower.top

const double PI = 3.14159;
来源：http://sli.cdnleiting.top

[S28] C：静态变量
来源：http://ohw.jlsjyb.cn

static int counter = 0;
来源：http://rlo.pengpengdd.cyou

[S29] C：变参函数
来源：http://pxz.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ngx.9152youxi.cn

[S30] C：头文件保护
来源：http://foe.aibaodan.cn

#ifndef X_H
来源：http://eae.yj20258.top

#define X_H
来源：http://joj.jinyuanbaomall.cn

#endif
来源：http://rer.yuxming.cn

[S31] C++：Hello World
来源：http://lfj.zhixingplan.top

#include <iostream>
来源：http://faq.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://nbl.yvedp.cn

[S32] C++：字符串
来源：http://lfb.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://ixj.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://ric.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lki.c1oappe.top

[S34] C++：遍历 vector
来源：http://rfu.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://mua.wangshuangyany.cn

[S35] C++：map
来源：http://rqa.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hiw.316326.xyz

[S36] C++：unordered_map
来源：http://lwi.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eyf.yfazqb.com

[S37] C++：set
来源：http://gqr.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ame.mhx1999.top

[S38] C++：排序
来源：http://otf.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://ozi.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://uwd.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbh.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://urw.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://scf.smart0.xyz

[S41] C++：类与构造函数
来源：http://veb.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cjv.yfazqb.com

[S42] C++：继承与虚函数
来源：http://knc.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://dvf.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://jad.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://bar.gotoacloud.top

[S44] C++：引用传参
来源：http://awl.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://fiu.tanke756.top

[S45] C++：lambda
来源：http://inm.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://ndy.hfpthk.cn

[S46] C++：函数模板
来源：http://sab.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itt.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://pzt.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bfn.andypj.xyz

[S48] C++：逐行读文件
来源：http://mgu.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://obe.yj20258888.top

while (std::getline(in, line)) { }
来源：http://pvv.hysaishi.cn

[S49] C++：写文件
来源：http://wlo.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fvd.nanxinkj.top

[S50] C++：格式化数字
来源：http://wph.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aqh.9152youxi.cn

[S51] C++：显式类型转换
来源：http://fup.svipenyu.cn

static_cast<double>(a) / b
来源：http://osy.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://wpq.sxryk.cn

int size() const noexcept { return n_; }
来源：http://qgh.vqdsnc.cn

[S53] C++：移动语义
来源：http://ekv.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://sev.haohaochexian.top

[S54] C++：异常处理
来源：http://awp.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tnj.iojbl.cn

[S55] C++：结构化绑定
来源：http://hpz.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vhf.redwolf501.top

[S56] C++：optional
来源：http://etp.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dwu.xinyue.icu

[S57] C++：编译期常量
来源：http://sob.ydzc1.top

constexpr int N = 10;
来源：http://umv.fktsv.cn

[S58] C++：命名空间
来源：http://hmi.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://dcd.bbcook.cn

[S59] C++：静态断言
来源：http://pog.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jze.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://cso.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ysj.iojbl.cn

================================================================================
来源：http://vje.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qun.yj202588.top

================================================================================
来源：http://imm.ybcxt.top

[T01] Kotlin：Hello World
来源：http://zpj.zhixingplan.top

println("Hello")
来源：http://qjj.meibo888.top

[T02] Kotlin：变量
来源：http://eba.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fdj.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://ole.quarkkingdee.top

"值: $b"
来源：http://ezr.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://ouu.bbcook.cn

val n: String? = null;  n?.length
来源：http://axg.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://tcj.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://usr.xinyue.icu

[T06] Kotlin：集合映射
来源：http://ise.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uqq.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://flg.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sui.nwbrower.top

[T08] Kotlin：数据类
来源：http://bzt.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://qpl.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://ift.yongpay.top

fun String.exclaim() = this + "!"
来源：http://ezw.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://dbl.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uax.316326.xyz

[T11] Kotlin：协程
来源：http://zxh.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jbp.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://tqo.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://ybo.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://rjz.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://jww.andypj.xyz

[T14] Kotlin：循环
来源：http://swm.bbcook.cn

for (i in 1..10) println(i)
来源：http://aln.hysaishi.cn

[T15] Kotlin：接口
来源：http://mbt.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://zth.kuanghao11.cn

[T16] Swift：Hello World
来源：http://slw.jyoumei.cn

print("Hello")
来源：http://twu.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://fed.chenzaomai.com

var a = 1;  let b = 2
来源：http://rmg.hfpthk.cn

[T18] Swift：字符串插值
来源：http://bus.316326.xyz

"值: \(b)"
来源：http://sxs.cashguo.top


<!-- 参考信息 -->