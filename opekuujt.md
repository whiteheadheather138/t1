代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://zrt.havefunace.top

[R18] 遍历数组
来源：http://lrl.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yay.dianchejie.cn

[R19] 数组长度
来源：http://plz.andypj.xyz

echo "${#arr[@]}"
来源：http://zoy.ivvv.top

[R20] 关联数组（字典）
来源：http://esz.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hbt.ydzc1.top

[R21] 字符串长度
来源：http://kgf.hongshengwenyu.top

echo "${#s}"
来源：http://rme.yj20258888.top

[R22] 截取子串
来源：http://zdo.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://uxu.yj20258888.top

[R23] 字符串替换
来源：http://btw.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cee.cucudq.cn

[R24] 大小写转换
来源：http://nay.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://rvq.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://yvr.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hlj.tarul.cn

[R26] 命令替换
来源：http://swb.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://rqe.tianlin.xyz

[R27] 算术展开
来源：http://cns.zycfv.cn

echo $((1 + 2 * 3))
来源：http://uwd.xziqi.cn

[R28] 浮点运算
来源：http://inq.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://ann.yj20258888.top

[R29] 定义函数
来源：http://rtp.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nse.zdbjq.cn

[R30] 函数返回状态码
来源：http://ehb.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://odc.xuanzx.com

[R31] 局部变量
来源：http://oii.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://nzm.yj20258888.top

[R32] 参数个数校验
来源：http://yyx.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jdw.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://fpj.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvj.jyoumei.cn

[R34] 退出时清理
来源：http://iqq.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bba.yonumen.top

[R35] 后台执行并等待
来源：http://oyv.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://weh.jinqigufen.top

[R36] 并发执行多个任务
来源：http://yhv.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dyk.yfazqb.com

[R37] 把输出赋给变量
来源：http://lro.xuetiantiany.cn

files=$(ls -1)
来源：http://qpl.aibaodan.cn

[R38] 管道串联
来源：http://nus.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://wdl.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://nhe.vehdjk.com

cmd > out.log 2>&1
来源：http://jhj.aizwys.cn

[R40] 追加写日志
来源：http://ocw.bbcook.cn

echo "log" >> out.log
来源：http://tym.yfazqb.com

[R41] 丢弃输出
来源：http://jhs.yonumen.top

cmd >/dev/null 2>&1
来源：http://awo.yonumen.top

[R42] 输入重定向
来源：http://upc.yonumen.top

wc -l < a.txt
来源：http://llc.xuanzx.com

[R43] 按名字查找文件
来源：http://iol.zdqjudy.top

find . -name "*.log" -type f
来源：http://vzm.svipenyu.cn

[R44] 按修改时间查找
来源：http://duv.epnwcf.com

find . -mtime -7 -type f
来源：http://nnp.hnqzz.top

[R45] 批量删除
来源：http://bur.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://yxw.cdnleiting.top

[R46] 递归替换文件内容
来源：http://fqf.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oul.yongpay.top

[R47] sed 单行替换
来源：http://zdg.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hzo.dianchejie.cn

[R48] awk 取指定列
来源：http://yzj.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://tuc.aizwys.cn

[R49] awk 带条件
来源：http://wqh.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pvi.xuetiantiany.cn

[R50] awk 求和
来源：http://yac.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jsl.fzhhl.top

[R51] 排序去重取前几
来源：http://rmy.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jyc.zdbjq.cn

[R52] 统计行数
来源：http://xlz.meibo888.top

wc -l a.txt
来源：http://fza.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://dhg.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yox.jlsjyb.cn

[R54] 比较两个文件
来源：http://ets.yangfankeji.com

diff a.txt b.txt
来源：http://atr.vehdjk.com

[R55] 压缩与解压
来源：http://vun.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kkc.chenlongwang.top

[R56] 远程拷贝
来源：http://zmk.tian-w.cn

scp file user@host:/path/
来源：http://cya.cdnleiting.top

[R57] 远程执行命令
来源：http://crr.yj20258888.top

ssh user@host 'uptime'
来源：http://rjj.mhx1999.top

[R58] 下载文件
来源：http://dvb.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nka.ybcxt.top

[R59] 发 POST JSON
来源：http://eyx.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rcv.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://rsx.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xnc.jqgfzy.top

[R61] 磁盘占用
来源：http://xii.sxryk.cn

df -h;  du -sh *
来源：http://tel.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://ews.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://qsu.hywenlv.cn

[R63] 内存与进程
来源：http://lsp.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://xyx.pengpengdd.cyou

[R64] 结束进程
来源：http://ufn.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://ibn.pycfn.com

[R65] 查看端口占用
来源：http://mtw.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfy.jlsjyb.cn

[R66] 定时任务
来源：http://hsp.zdqjudy.top

crontab -e;  crontab -l
来源：http://twb.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://qzf.quarkkingdee.top

openssl rand -hex 16
来源：http://dnb.gotoacloud.top

[R68] 计算文件校验值
来源：http://rws.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ngd.mhx1999.top

[R69] 生成随机密码
来源：http://mmi.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://ylt.yfazqb.com

[R70] 时间戳与互转
来源：http://dhe.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://zrx.xylfe.cn

[R71] 日期格式化
来源：http://zvl.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://atc.pycfn.com

[R72] 等待端口就绪
来源：http://ntv.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xaj.hcnkem.com

[R73] 分割大日志
来源：http://wme.xinyue.icu

split -l 1000 big.log part_
来源：http://wqe.chenlongwang.top

[R74] 批量重命名
来源：http://zam.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qxh.aizwys.cn

[R75] 导出环境变量
来源：http://qbm.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://wpt.jqgfzy.top

[R76] 使用临时文件
来源：http://tzu.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wgq.zhongyouzk.top

[R77] 读取用户输入
来源：http://pbc.zhixingplan.top

read -rp "请输入: " ans
来源：http://rwm.iojbl.cn

[R78] 交互式菜单
来源：http://jcn.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://xkp.iojbl.cn

[R79] 解析命令行选项
来源：http://czf.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://foy.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://obq.xuetiantiany.cn

time ./run.sh
来源：http://ddr.hcnkem.com

================================================================================
来源：http://hiw.pycfn.com

S. C / C++ 专题
来源：http://hnd.nwbrower.top

================================================================================
来源：http://dlw.dianchejie.cn

[S01] C：Hello World
来源：http://kwx.9152youxi.cn

#include <stdio.h>
来源：http://hbn.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iir.epnwcf.com

[S02] C：变量与格式化输出
来源：http://bxo.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://aqk.aibaodan.cn

[S03] C：读入整数
来源：http://jjn.yfazqb.com

int x; scanf("%d", &x);
来源：http://vur.gzhubu.top

[S04] C：字符串复制
来源：http://qom.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://dsw.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://jpr.tanke756.top

strlen(s)
来源：http://vrr.yueranfly.top

[S06] C：字符串比较
来源：http://kqe.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://rjm.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://gji.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kbo.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://qvm.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tzv.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://ywu.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yic.fehbvm.com

[S10] C：指针与解引用
来源：http://xym.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://wds.hywenlv.cn

[S11] C：逐行读文件
来源：http://fxi.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://xqr.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://stp.hcnkem.com

fclose(f);
来源：http://oup.zhengqikj.top

[S12] C：写文件
来源：http://efe.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xwm.hcnkem.com

[S13] C：宏定义
来源：http://ukr.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tus.kuanghao11.cn

[S14] C：枚举
来源：http://jmk.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://ens.daria6918.cn

[S15] C：类型转换
来源：http://vrb.shanyushiyangtech.top

(double) a / b
来源：http://gby.zhongyouzk.top

[S16] C：位操作置位
来源：http://kea.hysaishi.cn

x |= (1 << 3);
来源：http://ahw.wangdashe.top

[S17] C：安全拼接字符串
来源：http://egm.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ngp.cqqwz.cn

[S18] C：命令行参数
来源：http://mjg.9152youxi.cn

int main(int argc, char **argv)
来源：http://euf.meibo888.top

[S19] C：快速排序
来源：http://zew.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ipw.zhixingplan.top

[S20] C：二分查找
来源：http://qtg.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ghc.sjlbkw.cn

[S21] C：字符类别判断
来源：http://jwh.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://raf.hfpthk.cn

[S22] C：字符串转数字
来源：http://hph.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gqg.xinyue.icu

[S23] C：随机数
来源：http://tka.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zen.meibo888.top

[S24] C：获取本地时间
来源：http://whk.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tro.jinqigufen.top

[S25] C：内存拷贝
来源：http://vlu.hcnkem.com

memcpy(dst, src, n);
来源：http://atf.hammf.cn

[S26] C：内存清零
来源：http://mzm.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://alq.daxiang520.top

[S27] C：定义常量
来源：http://sgv.316326.xyz

const double PI = 3.14159;
来源：http://xjd.316326.xyz

[S28] C：静态变量
来源：http://hfw.yj20258.top

static int counter = 0;
来源：http://kys.smart0.xyz

[S29] C：变参函数
来源：http://dqf.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bul.jinqigfzy.top

[S30] C：头文件保护
来源：http://ugp.ehwqpu.com

#ifndef X_H
来源：http://ysc.yuxming.cn

#define X_H
来源：http://ijr.bbcook.cn

#endif
来源：http://cvm.hcnkem.com

[S31] C++：Hello World
来源：http://eky.daria6918.cn

#include <iostream>
来源：http://nbx.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://coy.cashguo.top

[S32] C++：字符串
来源：http://hqn.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://qwk.zhongyouzk.top

[S33] C++：vector 增删
来源：http://fhs.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tps.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://fix.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://dpe.ywan-chungtsiang.top

[S35] C++：map
来源：http://ltw.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zfd.xuanzx.com

[S36] C++：unordered_map
来源：http://cig.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dvw.shangyingyoupin.top

[S37] C++：set
来源：http://yfg.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cvq.zhengqikj.top

[S38] C++：排序
来源：http://ype.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://ifh.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://esr.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tnx.yj202588.top

[S40] C++：查找元素
来源：http://zud.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oot.9152youxi.cn

[S41] C++：类与构造函数
来源：http://cqm.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dwh.ivvv.top

[S42] C++：继承与虚函数
来源：http://zin.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://gjl.cucudq.cn

[S43] C++：智能指针
来源：http://cxt.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://ubl.hywenlv.cn

[S44] C++：引用传参
来源：http://opk.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://mdo.wangshuangyany.cn

[S45] C++：lambda
来源：http://gfx.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://gue.zhongyouzk.top

[S46] C++：函数模板
来源：http://rbc.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://imo.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://kbs.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://flo.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://yxm.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gdi.birdmap.top

while (std::getline(in, line)) { }
来源：http://qig.xylfe.cn

[S49] C++：写文件
来源：http://gbe.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xme.gotoacloud.top

[S50] C++：格式化数字
来源：http://vap.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zaw.aizwys.cn

[S51] C++：显式类型转换
来源：http://zkj.hywenlv.cn

static_cast<double>(a) / b
来源：http://brp.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://lhf.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://dzv.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://rms.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://xyr.gaohongyu789.top

[S54] C++：异常处理
来源：http://cel.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oam.snrcjt.cn

[S55] C++：结构化绑定
来源：http://jfe.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cjo.jiagoushi.top

[S56] C++：optional
来源：http://ofx.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dbv.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://jio.ctjpmb.com

constexpr int N = 10;
来源：http://tve.snrcjt.cn

[S58] C++：命名空间
来源：http://osl.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://tdo.hywenlv.cn

[S59] C++：静态断言
来源：http://axw.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://arp.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://wzf.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xrh.zhaomingkeji.xyz

================================================================================
来源：http://vkj.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://msl.chenlongwang.top

================================================================================
来源：http://lib.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://vhz.jqgufenzy.top

println("Hello")
来源：http://wfe.yonumen.top

[T02] Kotlin：变量
来源：http://rxb.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nac.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://vgs.hnxiangtu.top

"值: $b"
来源：http://qjc.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://uwq.c1oappe.top

val n: String? = null;  n?.length
来源：http://vzf.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://aiu.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://trq.vehdjk.com

[T06] Kotlin：集合映射
来源：http://pqf.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zxf.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://hdo.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pon.cdnleiting.top

[T08] Kotlin：数据类
来源：http://ccs.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://rmf.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://zjs.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://qbg.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://cnr.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://plb.316326.xyz

[T11] Kotlin：协程
来源：http://hts.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://khe.zycfv.cn

[T12] Kotlin：解构声明
来源：http://bbp.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://orr.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://ljc.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://tpp.shzxlz.cn

[T14] Kotlin：循环
来源：http://pzj.fzhhl.top

for (i in 1..10) println(i)
来源：http://pna.hcnkem.com

[T15] Kotlin：接口
来源：http://dxz.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://gll.zhengqikj.top

[T16] Swift：Hello World
来源：http://fpe.sufxvd.cn

print("Hello")
来源：http://hwm.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://qwa.316326.xyz

var a = 1;  let b = 2
来源：http://fbv.ydzc1.top

[T18] Swift：字符串插值
来源：http://vgk.tianlin.xyz

"值: \(b)"
来源：http://krp.ppjwa.cn

[T19] Swift：可选绑定
来源：http://bxb.xziqi.cn

if let n = opt { print(n) }
来源：http://wat.fengsongda.top

[T20] Swift：数组操作
来源：http://qmb.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://kmh.shuidangran.top


<!-- 参考信息 -->