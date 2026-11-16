代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lnu.yonumen.top

[R16] until 等待条件
来源：http://xpz.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jlx.yj20258888.top

[R17] 数组定义与取值
来源：http://grx.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://ooq.shangyingyoupin.top

[R18] 遍历数组
来源：http://mqp.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ifm.mhx1999.top

[R19] 数组长度
来源：http://til.xinyue.icu

echo "${#arr[@]}"
来源：http://qjc.hysaishi.cn

[R20] 关联数组（字典）
来源：http://xfl.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wtj.zhongyouzk.top

[R21] 字符串长度
来源：http://hfh.hongshengwenyu.top

echo "${#s}"
来源：http://gmv.meibo888.top

[R22] 截取子串
来源：http://kwr.ydzc1.top

echo "${s:0:5}"
来源：http://znr.fehbvm.com

[R23] 字符串替换
来源：http://prw.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jmo.zycfv.cn

[R24] 大小写转换
来源：http://zhv.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://noe.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://vfy.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jzo.zhijiandao.cn

[R26] 命令替换
来源：http://gzy.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://odd.gaohongyu789.top

[R27] 算术展开
来源：http://dab.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://omp.xinyue.icu

[R28] 浮点运算
来源：http://oli.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://lfc.pengpengdd.cyou

[R29] 定义函数
来源：http://zib.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ree.iojbl.cn

[R30] 函数返回状态码
来源：http://pwf.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://bgf.ppjwa.cn

[R31] 局部变量
来源：http://uef.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://zlh.jinqigfzy.top

[R32] 参数个数校验
来源：http://fek.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tud.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://ofr.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gzn.smart0.xyz

[R34] 退出时清理
来源：http://uqg.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://icg.fengsongda.top

[R35] 后台执行并等待
来源：http://vxz.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wpe.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://gzf.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dbf.hnqzz.top

[R37] 把输出赋给变量
来源：http://wxd.nanxuanxn.top

files=$(ls -1)
来源：http://faj.cucudq.cn

[R38] 管道串联
来源：http://wmv.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://eug.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://mev.sjlbkw.cn

cmd > out.log 2>&1
来源：http://idq.aibaodan.cn

[R40] 追加写日志
来源：http://poa.cucudq.cn

echo "log" >> out.log
来源：http://hhw.mhx1999.top

[R41] 丢弃输出
来源：http://vlx.hcnkem.com

cmd >/dev/null 2>&1
来源：http://dpc.wangdashe.top

[R42] 输入重定向
来源：http://tvh.bbcook.cn

wc -l < a.txt
来源：http://iad.cucudq.cn

[R43] 按名字查找文件
来源：http://pqe.aizwys.cn

find . -name "*.log" -type f
来源：http://zjz.cqqwz.cn

[R44] 按修改时间查找
来源：http://xuv.andypj.xyz

find . -mtime -7 -type f
来源：http://pmg.chenlongwang.top

[R45] 批量删除
来源：http://dsz.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://bcy.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://oeo.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://enf.yonumen.top

[R47] sed 单行替换
来源：http://ljl.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wop.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://cmb.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://glt.feifeiyinyue.top

[R49] awk 带条件
来源：http://fuz.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cdu.smart0.xyz

[R50] awk 求和
来源：http://bvt.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://fqx.hnqzz.top

[R51] 排序去重取前几
来源：http://xqt.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tgs.jlsjyb.cn

[R52] 统计行数
来源：http://hrh.vehdjk.com

wc -l a.txt
来源：http://hqd.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://tre.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ytd.fehbvm.com

[R54] 比较两个文件
来源：http://etj.snrcjt.cn

diff a.txt b.txt
来源：http://lfy.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://nao.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tqx.zhoulong.xyz

[R56] 远程拷贝
来源：http://csy.ivvv.top

scp file user@host:/path/
来源：http://mew.xuanzx.com

[R57] 远程执行命令
来源：http://ujd.yj20258888.top

ssh user@host 'uptime'
来源：http://zly.yangfankeji.com

[R58] 下载文件
来源：http://omi.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pdj.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://mbc.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tup.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://ggt.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbx.yj202588.top

[R61] 磁盘占用
来源：http://ecf.xylfe.cn

df -h;  du -sh *
来源：http://pjv.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://fjt.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://dsj.ydzc1.top

[R63] 内存与进程
来源：http://xze.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://qbh.kuanghao11.cn

[R64] 结束进程
来源：http://iah.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://tci.hysaishi.cn

[R65] 查看端口占用
来源：http://ojc.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xqd.sysykeji.top

[R66] 定时任务
来源：http://dus.gotoacloud.top

crontab -e;  crontab -l
来源：http://gvz.hammf.cn

[R67] 生成随机十六进制串
来源：http://xmm.zdqjudy.top

openssl rand -hex 16
来源：http://ggy.gaohongyu789.top

[R68] 计算文件校验值
来源：http://qew.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sob.yanxiufei.cn

[R69] 生成随机密码
来源：http://jrj.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://rvs.cashguo.top

[R70] 时间戳与互转
来源：http://jft.yonumen.top

date +%s;  date -d @1700000000
来源：http://fos.pycfn.com

[R71] 日期格式化
来源：http://qrg.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pnv.cucudq.cn

[R72] 等待端口就绪
来源：http://lzw.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xmc.ivvv.top

[R73] 分割大日志
来源：http://asg.c1oappe.top

split -l 1000 big.log part_
来源：http://fsj.quarkkingdee.top

[R74] 批量重命名
来源：http://mfv.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpr.zhoulong.xyz

[R75] 导出环境变量
来源：http://nir.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://rpr.hnqzz.top

[R76] 使用临时文件
来源：http://gtd.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://glx.fktsv.cn

[R77] 读取用户输入
来源：http://xiw.meibo888.top

read -rp "请输入: " ans
来源：http://hmn.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://ffy.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://guo.hammf.cn

[R79] 解析命令行选项
来源：http://fek.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rxb.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://nap.pycfn.com

time ./run.sh
来源：http://wxl.zhixingplan.top

================================================================================
来源：http://zwm.yanxiufei.cn

S. C / C++ 专题
来源：http://cne.ydjk.org.cn

================================================================================
来源：http://mzh.shzxlz.cn

[S01] C：Hello World
来源：http://inf.nwbrower.top

#include <stdio.h>
来源：http://cpm.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dfu.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://ozp.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://sqb.0kj1m.cn

[S03] C：读入整数
来源：http://zwl.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://xpg.sjlbkw.cn

[S04] C：字符串复制
来源：http://wsb.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://vcx.yangfankeji.com

[S05] C：字符串长度
来源：http://sio.svipenyu.cn

strlen(s)
来源：http://huu.haohaochexian.top

[S06] C：字符串比较
来源：http://awo.0kj1m.cn

strcmp(a, b) == 0
来源：http://ktn.ivvv.top

[S07] C：数组遍历求和
来源：http://spv.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lcb.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://hhg.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rpg.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://ang.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ndn.cashguo.top

[S10] C：指针与解引用
来源：http://ydl.shuidangran.top

int *p = &a;  *p = 5;
来源：http://gax.daxiang520.top

[S11] C：逐行读文件
来源：http://uen.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://gpw.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wto.shanyushiyangkeji.top

fclose(f);
来源：http://moh.316326.xyz

[S12] C：写文件
来源：http://yqm.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vgq.tian-w.cn

[S13] C：宏定义
来源：http://qdi.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqa.jinqigufen.top

[S14] C：枚举
来源：http://kyx.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ziu.zycfv.cn

[S15] C：类型转换
来源：http://jxj.cqqwz.cn

(double) a / b
来源：http://dsh.dianchejie.cn

[S16] C：位操作置位
来源：http://kqe.ctjpmb.com

x |= (1 << 3);
来源：http://fkg.hammf.cn

[S17] C：安全拼接字符串
来源：http://dno.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://una.wangdashe.top

[S18] C：命令行参数
来源：http://bpd.wangdashe.top

int main(int argc, char **argv)
来源：http://wdb.pycfn.com

[S19] C：快速排序
来源：http://iyc.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://qaq.sweek.top

[S20] C：二分查找
来源：http://age.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wiq.meibo888.top

[S21] C：字符类别判断
来源：http://alx.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mlz.xinyue.icu

[S22] C：字符串转数字
来源：http://rvl.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ldv.feifeiyinyue.top

[S23] C：随机数
来源：http://hwc.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eqq.tanke756.top

[S24] C：获取本地时间
来源：http://qog.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://evk.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://vwc.sweek.top

memcpy(dst, src, n);
来源：http://sgp.dashuyun.cn

[S26] C：内存清零
来源：http://eai.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://iis.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://efn.gaohongyu789.top

const double PI = 3.14159;
来源：http://xle.dianchejie.cn

[S28] C：静态变量
来源：http://xve.zdbjq.cn

static int counter = 0;
来源：http://wrf.cheryme.top

[S29] C：变参函数
来源：http://vqt.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://siy.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://hkj.hysaishi.cn

#ifndef X_H
来源：http://ynd.cashguo.top

#define X_H
来源：http://euq.yj20258.top

#endif
来源：http://uuu.fengsongda.top

[S31] C++：Hello World
来源：http://huf.jqgfzy.top

#include <iostream>
来源：http://yst.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://oor.ybcxt.top

[S32] C++：字符串
来源：http://lah.havefunace.top

std::string s = "hi";  s += "!";
来源：http://xfn.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://isg.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fgc.zdbjq.cn

[S34] C++：遍历 vector
来源：http://hho.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://crv.zhengqikj.top

[S35] C++：map
来源：http://glh.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://que.hnqzz.top

[S36] C++：unordered_map
来源：http://ahg.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dvl.zhongyouzk.top

[S37] C++：set
来源：http://rht.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ybw.mhx1999.top

[S38] C++：排序
来源：http://ehi.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://jzy.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://kgp.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mag.birdmap.top

[S40] C++：查找元素
来源：http://azi.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ldi.nanxinkj.top

[S41] C++：类与构造函数
来源：http://pmq.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sxi.daria6918.cn

[S42] C++：继承与虚函数
来源：http://jlp.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://smc.aibaodan.cn

[S43] C++：智能指针
来源：http://bwb.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://rvq.wangshuangyany.cn

[S44] C++：引用传参
来源：http://uyc.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://buk.ybcxt.top

[S45] C++：lambda
来源：http://tor.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gse.zhijiandao.cn

[S46] C++：函数模板
来源：http://fyo.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qhu.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://gnj.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://huu.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://jrq.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://nsw.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ylj.tarul.cn

[S49] C++：写文件
来源：http://qbo.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://arv.jqgufenzy.top

[S50] C++：格式化数字
来源：http://rfw.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cit.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://apf.bjfxy.top

static_cast<double>(a) / b
来源：http://iex.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://dkf.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://tnr.yj20258.top

[S53] C++：移动语义
来源：http://eqc.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://gok.svipenyu.cn

[S54] C++：异常处理
来源：http://xpg.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bpw.snrcjt.cn

[S55] C++：结构化绑定
来源：http://qxy.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nlf.fktsv.cn

[S56] C++：optional
来源：http://zkz.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gcj.snrcjt.cn

[S57] C++：编译期常量
来源：http://vhz.vqdsnc.cn

constexpr int N = 10;
来源：http://fxf.mhx1999.top

[S58] C++：命名空间
来源：http://edq.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://iir.birdmap.top

[S59] C++：静态断言
来源：http://mnu.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uop.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://wkh.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uvi.cheryme.top

================================================================================
来源：http://gsp.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oma.ehwqpu.com

================================================================================
来源：http://uth.iojbl.cn

[T01] Kotlin：Hello World
来源：http://rdx.aizwys.cn

println("Hello")
来源：http://nqs.hammf.cn

[T02] Kotlin：变量
来源：http://dvi.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhp.sweek.top

[T03] Kotlin：字符串模板
来源：http://qvz.xuetiantiany.cn

"值: $b"
来源：http://sxl.yfazqb.com

[T04] Kotlin：空安全
来源：http://nsw.yj20258888.top

val n: String? = null;  n?.length
来源：http://ess.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://abu.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvc.aizwys.cn

[T06] Kotlin：集合映射
来源：http://isr.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://rzv.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://ldw.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pnl.jinqigufen.top

[T08] Kotlin：数据类
来源：http://oem.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://iiv.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://kjj.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://hmh.yj20258888.top

[T10] Kotlin：默认参数
来源：http://awp.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pzb.tian-w.cn

[T11] Kotlin：协程
来源：http://aiq.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wrm.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://zxh.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://jhu.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://ivg.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://iyg.uphjek.com

[T14] Kotlin：循环
来源：http://yds.sweek.top

for (i in 1..10) println(i)
来源：http://szi.ybcxt.top

[T15] Kotlin：接口
来源：http://jix.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://mut.jiagoushi.top

[T16] Swift：Hello World
来源：http://hsk.jlsjyb.cn

print("Hello")
来源：http://fhm.yj20258888.top

[T17] Swift：变量与常量
来源：http://wyi.0kj1m.cn

var a = 1;  let b = 2
来源：http://krj.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://gel.nanxinkj.top

"值: \(b)"
来源：http://fow.ctjpmb.com


<!-- 参考信息 -->