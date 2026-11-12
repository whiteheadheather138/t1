代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://pvl.zycfv.cn

[R14] C 风格 for
来源：http://qai.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rmf.jinqigufen.top

[R15] while 逐行读文件
来源：http://lmr.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uxs.vqdsnc.cn

[R16] until 等待条件
来源：http://vxh.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oli.nwbrower.top

[R17] 数组定义与取值
来源：http://rxx.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://xcm.jqgfzy.top

[R18] 遍历数组
来源：http://okq.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pni.cheryme.top

[R19] 数组长度
来源：http://nbs.zhongyouzk.top

echo "${#arr[@]}"
来源：http://oxw.jyoumei.cn

[R20] 关联数组（字典）
来源：http://wzs.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcy.birdmap.top

[R21] 字符串长度
来源：http://mqj.smart0.xyz

echo "${#s}"
来源：http://knt.shanyushiyangtech.top

[R22] 截取子串
来源：http://sox.hysaishi.cn

echo "${s:0:5}"
来源：http://bdf.zhoulong.xyz

[R23] 字符串替换
来源：http://qrk.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pbj.hcnkem.com

[R24] 大小写转换
来源：http://dlg.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://khz.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://ozf.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iuz.zhoulong.xyz

[R26] 命令替换
来源：http://usi.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://gvz.dianchejie.cn

[R27] 算术展开
来源：http://gjo.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://ewo.kuanghao11.cn

[R28] 浮点运算
来源：http://gqd.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://nvu.redwolf501.top

[R29] 定义函数
来源：http://qkh.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kgq.sysykeji.top

[R30] 函数返回状态码
来源：http://yro.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://zoz.pengpengdd.cyou

[R31] 局部变量
来源：http://srg.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://uor.guowangkeji.top

[R32] 参数个数校验
来源：http://zym.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aym.cashguo.top

[R33] 捕获错误并提示行号
来源：http://gxz.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vkp.shanyushiyangtech.top

[R34] 退出时清理
来源：http://iiu.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://wxg.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://tco.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ryp.jiagoushi.top

[R36] 并发执行多个任务
来源：http://nvi.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jgb.yfazqb.com

[R37] 把输出赋给变量
来源：http://obn.jinqigfzy.top

files=$(ls -1)
来源：http://iet.wangdashe.top

[R38] 管道串联
来源：http://skq.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://bzp.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://ume.shuidangran.top

cmd > out.log 2>&1
来源：http://etc.hfpthk.cn

[R40] 追加写日志
来源：http://vfs.guannengcc.top

echo "log" >> out.log
来源：http://pkl.shzxlz.cn

[R41] 丢弃输出
来源：http://byg.ydzc1.top

cmd >/dev/null 2>&1
来源：http://ppl.feifeiyinyue.top

[R42] 输入重定向
来源：http://ubd.xinyue.icu

wc -l < a.txt
来源：http://glr.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://uzo.daria6918.cn

find . -name "*.log" -type f
来源：http://nxg.yj202588.top

[R44] 按修改时间查找
来源：http://pwc.ydjk.org.cn

find . -mtime -7 -type f
来源：http://tra.zhengqikj.top

[R45] 批量删除
来源：http://vjt.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://nfy.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://ewe.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xvs.zhengqikj.top

[R47] sed 单行替换
来源：http://slv.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://izr.daria6918.cn

[R48] awk 取指定列
来源：http://kdg.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://twd.wangdashe.top

[R49] awk 带条件
来源：http://pcs.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cge.jlsjyb.cn

[R50] awk 求和
来源：http://kyx.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dza.hysaishi.cn

[R51] 排序去重取前几
来源：http://xkj.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bpj.sufxvd.cn

[R52] 统计行数
来源：http://gyx.jianghu66.top

wc -l a.txt
来源：http://agq.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://xzy.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyv.daria6918.cn

[R54] 比较两个文件
来源：http://puc.316326.xyz

diff a.txt b.txt
来源：http://ocz.jinqigufen.top

[R55] 压缩与解压
来源：http://msp.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oro.quarkkingdee.top

[R56] 远程拷贝
来源：http://het.ctjpmb.com

scp file user@host:/path/
来源：http://pqg.aibaodan.cn

[R57] 远程执行命令
来源：http://idp.guannengcc.top

ssh user@host 'uptime'
来源：http://ook.daria6918.cn

[R58] 下载文件
来源：http://tif.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xhn.fengsongda.top

[R59] 发 POST JSON
来源：http://ary.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ret.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://cxx.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vdo.bjfxy.top

[R61] 磁盘占用
来源：http://gqf.hesvh.cn

df -h;  du -sh *
来源：http://kcg.guowangkeji.top

[R62] 找最占空间的文件
来源：http://sib.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://iqr.hnqzz.top

[R63] 内存与进程
来源：http://qgt.meibo888.top

free -h;  ps aux | grep nginx
来源：http://vpk.shangyingyoupin.top

[R64] 结束进程
来源：http://uno.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://yez.zhijiandao.cn

[R65] 查看端口占用
来源：http://tjc.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yss.ywan-chungtsiang.top

[R66] 定时任务
来源：http://akt.sweek.top

crontab -e;  crontab -l
来源：http://ovc.yj20258888.top

[R67] 生成随机十六进制串
来源：http://nns.chenlongwang.top

openssl rand -hex 16
来源：http://led.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://dpy.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mum.hywenlv.cn

[R69] 生成随机密码
来源：http://sap.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://esp.nanxuanxn.top

[R70] 时间戳与互转
来源：http://xwi.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://aks.fktsv.cn

[R71] 日期格式化
来源：http://wkr.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lbt.yonumen.top

[R72] 等待端口就绪
来源：http://ngd.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mre.xylfe.cn

[R73] 分割大日志
来源：http://ium.xinyue.icu

split -l 1000 big.log part_
来源：http://tbq.fzhhl.top

[R74] 批量重命名
来源：http://hxq.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gbf.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://cut.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://rea.zdqjudy.top

[R76] 使用临时文件
来源：http://mtj.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nli.meibo888.top

[R77] 读取用户输入
来源：http://yla.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://hox.yfazqb.com

[R78] 交互式菜单
来源：http://yan.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wvr.wangdashe.top

[R79] 解析命令行选项
来源：http://wvt.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yyk.yonumen.top

[R80] 查看脚本执行耗时
来源：http://ccx.sysykeji.top

time ./run.sh
来源：http://xut.jinqigufen.top

================================================================================
来源：http://sgu.chenlongwang.top

S. C / C++ 专题
来源：http://agg.dianchejie.cn

================================================================================
来源：http://vcn.tanke756.top

[S01] C：Hello World
来源：http://anm.uphjek.com

#include <stdio.h>
来源：http://min.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://xdg.smart0.xyz

[S02] C：变量与格式化输出
来源：http://eer.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://cnr.wangshuangyany.cn

[S03] C：读入整数
来源：http://wzx.yongpay.top

int x; scanf("%d", &x);
来源：http://iuc.yuxming.cn

[S04] C：字符串复制
来源：http://bgd.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://crs.jlsjyb.cn

[S05] C：字符串长度
来源：http://sau.yongpay.top

strlen(s)
来源：http://tgl.havefunace.top

[S06] C：字符串比较
来源：http://enz.jinqigfzy.top

strcmp(a, b) == 0
来源：http://oqh.cashguo.top

[S07] C：数组遍历求和
来源：http://wum.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://krn.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://owd.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://api.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://vde.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vde.ppjwa.cn

[S10] C：指针与解引用
来源：http://izf.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://rsc.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://sxj.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://xap.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dkp.daria6918.cn

fclose(f);
来源：http://fmo.shuidangran.top

[S12] C：写文件
来源：http://faa.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wzr.tianlin.xyz

[S13] C：宏定义
来源：http://amx.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gth.xziqi.cn

[S14] C：枚举
来源：http://zzz.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://omz.jinghuilouyu.cn

[S15] C：类型转换
来源：http://ewc.dashuyun.cn

(double) a / b
来源：http://kug.aibaodan.cn

[S16] C：位操作置位
来源：http://qiv.zycfv.cn

x |= (1 << 3);
来源：http://jqj.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://xii.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://haa.jlsjyb.cn

[S18] C：命令行参数
来源：http://jkp.chenlongwang.top

int main(int argc, char **argv)
来源：http://ewx.jqgfzy.top

[S19] C：快速排序
来源：http://biq.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://gge.jlsjyb.cn

[S20] C：二分查找
来源：http://izh.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ywo.wangdashe.top

[S21] C：字符类别判断
来源：http://mqd.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ahr.jqgfzy.top

[S22] C：字符串转数字
来源：http://vcu.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bci.nanxuanxn.top

[S23] C：随机数
来源：http://apw.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qvn.tian-w.cn

[S24] C：获取本地时间
来源：http://osa.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kxa.hcnkem.com

[S25] C：内存拷贝
来源：http://jwe.andypj.xyz

memcpy(dst, src, n);
来源：http://qvc.sjlbkw.cn

[S26] C：内存清零
来源：http://wcw.yj20258888.top

memset(a, 0, sizeof a);
来源：http://yim.guowangkeji.top

[S27] C：定义常量
来源：http://vku.yonumen.top

const double PI = 3.14159;
来源：http://yfh.hcnkem.com

[S28] C：静态变量
来源：http://png.aibaodan.cn

static int counter = 0;
来源：http://ziy.ydjk.org.cn

[S29] C：变参函数
来源：http://wbs.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zax.nwbrower.top

[S30] C：头文件保护
来源：http://fmy.jianghu66.top

#ifndef X_H
来源：http://uah.fehbvm.com

#define X_H
来源：http://koq.shanyushiyangkeji.top

#endif
来源：http://mrg.yangfankeji.com

[S31] C++：Hello World
来源：http://dfb.c1oappe.top

#include <iostream>
来源：http://guc.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://hwk.vqdsnc.cn

[S32] C++：字符串
来源：http://tds.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://atc.jiagoushi.top

[S33] C++：vector 增删
来源：http://dvk.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bto.ehwqpu.com

[S34] C++：遍历 vector
来源：http://gbh.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://tqn.tarul.cn

[S35] C++：map
来源：http://lbs.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tav.yfazqb.com

[S36] C++：unordered_map
来源：http://nvj.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qro.aizwys.cn

[S37] C++：set
来源：http://bde.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dik.hywenlv.cn

[S38] C++：排序
来源：http://ndm.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://tvi.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://vhh.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gux.zhixingplan.top

[S40] C++：查找元素
来源：http://yqu.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gzg.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://ode.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fpj.ydzc1.top

[S42] C++：继承与虚函数
来源：http://dwy.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://gux.gogol.net.cn

[S43] C++：智能指针
来源：http://zkm.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://kry.jianghu66.top

[S44] C++：引用传参
来源：http://qsc.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://yjx.xylfe.cn

[S45] C++：lambda
来源：http://cww.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://xya.xuanzx.com

[S46] C++：函数模板
来源：http://uou.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dkf.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://iep.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewv.tian-w.cn

[S48] C++：逐行读文件
来源：http://vxb.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://zhm.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://xug.hnxiangtu.top

[S49] C++：写文件
来源：http://qfd.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fus.yuanzhike.top

[S50] C++：格式化数字
来源：http://sqq.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gsr.chenlongwang.top

[S51] C++：显式类型转换
来源：http://yvw.tanke756.top

static_cast<double>(a) / b
来源：http://ime.cheryme.top

[S52] C++：const 与 noexcept
来源：http://oon.sweek.top

int size() const noexcept { return n_; }
来源：http://ayl.fzhhl.top

[S53] C++：移动语义
来源：http://coz.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://uyr.mhx1999.top

[S54] C++：异常处理
来源：http://laf.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://irj.iojbl.cn

[S55] C++：结构化绑定
来源：http://cck.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ssc.guowangkeji.top

[S56] C++：optional
来源：http://sjw.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eec.yuanzhike.top

[S57] C++：编译期常量
来源：http://rei.zhongyouzk.top

constexpr int N = 10;
来源：http://moy.xylfe.cn

[S58] C++：命名空间
来源：http://lkx.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://lsw.guannengcc.top

[S59] C++：静态断言
来源：http://gwp.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hmd.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://crk.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xfo.chenlongwang.top

================================================================================
来源：http://oal.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ima.tianlin.xyz

================================================================================
来源：http://uhu.xylfe.cn

[T01] Kotlin：Hello World
来源：http://abs.uphjek.com

println("Hello")
来源：http://dms.tianlin.xyz

[T02] Kotlin：变量
来源：http://ofs.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sks.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://dka.yfazqb.com

"值: $b"
来源：http://dzu.jianghu66.top

[T04] Kotlin：空安全
来源：http://ppi.yuanzhike.top

val n: String? = null;  n?.length
来源：http://ggi.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://wyi.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mbh.pycfn.com

[T06] Kotlin：集合映射
来源：http://pbv.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rlj.tanke756.top

[T07] Kotlin：集合过滤
来源：http://wjs.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mzc.yj202588.top

[T08] Kotlin：数据类
来源：http://ali.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://bwd.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://vbp.meibo888.top

fun String.exclaim() = this + "!"
来源：http://rng.hnqzz.top

[T10] Kotlin：默认参数
来源：http://skn.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bfy.meibo888.top

[T11] Kotlin：协程
来源：http://xjo.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pzo.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://kee.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://yib.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://rew.shuidangran.top

val m = mapOf("a" to 1)
来源：http://ryn.sysykeji.top

[T14] Kotlin：循环
来源：http://knd.dashuyun.cn

for (i in 1..10) println(i)
来源：http://jws.fehbvm.com

[T15] Kotlin：接口
来源：http://foo.meibo888.top

interface Shape { fun area(): Double }
来源：http://yjt.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://cji.guannengcc.top

print("Hello")
来源：http://ftk.bjfxy.top


<!-- 参考信息 -->