代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://pxh.52xcode.cn

[R14] C 风格 for
来源：http://knw.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ttz.zhijiandao.cn

[R15] while 逐行读文件
来源：http://htv.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ekq.yonumen.top

[R16] until 等待条件
来源：http://hvm.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vcn.shuidangran.top

[R17] 数组定义与取值
来源：http://hng.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vqe.andypj.xyz

[R18] 遍历数组
来源：http://xyy.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://azx.yonumen.top

[R19] 数组长度
来源：http://udw.hnqzz.top

echo "${#arr[@]}"
来源：http://pku.xuanzx.com

[R20] 关联数组（字典）
来源：http://ivt.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://thz.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://rnp.snrcjt.cn

echo "${#s}"
来源：http://fue.gzhubu.top

[R22] 截取子串
来源：http://gkc.yj20258.top

echo "${s:0:5}"
来源：http://sly.jinqigufen.top

[R23] 字符串替换
来源：http://ssw.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dvc.9152youxi.cn

[R24] 大小写转换
来源：http://vyd.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://gyj.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://kca.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hog.yueranfly.top

[R26] 命令替换
来源：http://xjw.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://nhd.ctjpmb.com

[R27] 算术展开
来源：http://oqd.bjfxy.top

echo $((1 + 2 * 3))
来源：http://owj.yangfankeji.com

[R28] 浮点运算
来源：http://yyw.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://fwy.xinyue.icu

[R29] 定义函数
来源：http://bdm.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfj.andypj.xyz

[R30] 函数返回状态码
来源：http://nqz.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://trt.kuanghao11.cn

[R31] 局部变量
来源：http://kis.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://zru.hywenlv.cn

[R32] 参数个数校验
来源：http://sis.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://trb.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://qtm.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://csy.jianghu66.top

[R34] 退出时清理
来源：http://xsm.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://leq.hnqzz.top

[R35] 后台执行并等待
来源：http://rnp.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ujc.ybcxt.top

[R36] 并发执行多个任务
来源：http://oak.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zvy.fzhhl.top

[R37] 把输出赋给变量
来源：http://zdy.uphjek.com

files=$(ls -1)
来源：http://iox.hammf.cn

[R38] 管道串联
来源：http://zqq.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://hhs.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://tct.ybcxt.top

cmd > out.log 2>&1
来源：http://ele.quarkkingdee.top

[R40] 追加写日志
来源：http://bct.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://cbu.hysaishi.cn

[R41] 丢弃输出
来源：http://tjj.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://vxn.kuanghao11.cn

[R42] 输入重定向
来源：http://pgw.yj202588.top

wc -l < a.txt
来源：http://nqa.daria6918.cn

[R43] 按名字查找文件
来源：http://pxq.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://xjm.aibaodan.cn

[R44] 按修改时间查找
来源：http://nnt.zdqjudy.top

find . -mtime -7 -type f
来源：http://ptc.ybcxt.top

[R45] 批量删除
来源：http://hzu.sweek.top

find . -name "*.tmp" -delete
来源：http://qfo.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://kbd.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pur.fehbvm.com

[R47] sed 单行替换
来源：http://str.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://ovy.ybcxt.top

[R48] awk 取指定列
来源：http://yle.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://lpj.yj202588.top

[R49] awk 带条件
来源：http://xsu.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://obi.zdbjq.cn

[R50] awk 求和
来源：http://gxr.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://wmd.hnqzz.top

[R51] 排序去重取前几
来源：http://ada.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ine.0kj1m.cn

[R52] 统计行数
来源：http://zjv.xinyue.icu

wc -l a.txt
来源：http://liq.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://lzl.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sqj.cheryme.top

[R54] 比较两个文件
来源：http://brr.jqgufenzy.top

diff a.txt b.txt
来源：http://tod.bjfxy.top

[R55] 压缩与解压
来源：http://gbx.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ufp.zhoulong.xyz

[R56] 远程拷贝
来源：http://ojx.yj202588.top

scp file user@host:/path/
来源：http://zgy.hongshengwenyu.top

[R57] 远程执行命令
来源：http://gfi.wangdashe.top

ssh user@host 'uptime'
来源：http://qdr.zhijiandao.cn

[R58] 下载文件
来源：http://vdm.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kry.ehwqpu.com

[R59] 发 POST JSON
来源：http://zth.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sdp.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://ejj.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mpv.ydzc1.top

[R61] 磁盘占用
来源：http://oby.jinqigfzy.top

df -h;  du -sh *
来源：http://tvg.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://dik.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://ijf.pengpengdd.cyou

[R63] 内存与进程
来源：http://yal.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://tiw.zhixingplan.top

[R64] 结束进程
来源：http://ahh.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://xpo.bjfxy.top

[R65] 查看端口占用
来源：http://fxz.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://crt.zhengqikj.top

[R66] 定时任务
来源：http://sxe.fengsongda.top

crontab -e;  crontab -l
来源：http://yvi.iojbl.cn

[R67] 生成随机十六进制串
来源：http://phh.zhengqikj.top

openssl rand -hex 16
来源：http://slp.birdmap.top

[R68] 计算文件校验值
来源：http://wfj.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://yme.kuanghao11.cn

[R69] 生成随机密码
来源：http://yxp.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://tzq.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://bge.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://sjt.hesvh.cn

[R71] 日期格式化
来源：http://ntx.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tah.shuidangran.top

[R72] 等待端口就绪
来源：http://jav.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nac.wangdashe.top

[R73] 分割大日志
来源：http://ucg.zdqjudy.top

split -l 1000 big.log part_
来源：http://zuf.zhixingplan.top

[R74] 批量重命名
来源：http://wnn.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uau.gogol.net.cn

[R75] 导出环境变量
来源：http://hdg.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://xlv.dianchejie.cn

[R76] 使用临时文件
来源：http://zol.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fqi.hywenlv.cn

[R77] 读取用户输入
来源：http://dzl.andypj.xyz

read -rp "请输入: " ans
来源：http://ebf.jiagoushi.top

[R78] 交互式菜单
来源：http://yog.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://myl.zhijiandao.cn

[R79] 解析命令行选项
来源：http://vgh.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gus.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://ylu.nanxuanxn.top

time ./run.sh
来源：http://wwo.uphjek.com

================================================================================
来源：http://bps.hnqzz.top

S. C / C++ 专题
来源：http://uss.ywan-chungtsiang.top

================================================================================
来源：http://ary.yongpay.top

[S01] C：Hello World
来源：http://mos.cdnleiting.top

#include <stdio.h>
来源：http://hoq.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://biw.yvedp.cn

[S02] C：变量与格式化输出
来源：http://kgz.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://daa.vqdsnc.cn

[S03] C：读入整数
来源：http://qdk.yfazqb.com

int x; scanf("%d", &x);
来源：http://mkz.sweek.top

[S04] C：字符串复制
来源：http://wvo.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://cey.gaohongyu789.top

[S05] C：字符串长度
来源：http://uij.haohaochexian.top

strlen(s)
来源：http://vyb.guannengcc.top

[S06] C：字符串比较
来源：http://xtq.ehwqpu.com

strcmp(a, b) == 0
来源：http://djp.sweek.top

[S07] C：数组遍历求和
来源：http://lcg.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yey.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://ulb.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nwp.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://chy.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yuh.smart0.xyz

[S10] C：指针与解引用
来源：http://eso.cashguo.top

int *p = &a;  *p = 5;
来源：http://rim.tian-w.cn

[S11] C：逐行读文件
来源：http://kvi.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://obt.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xjr.hysaishi.cn

fclose(f);
来源：http://dhb.jinyuanbaomall.cn

[S12] C：写文件
来源：http://ipe.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cwz.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://wok.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iwt.iojbl.cn

[S14] C：枚举
来源：http://ozn.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://jpf.cashguo.top

[S15] C：类型转换
来源：http://sxz.quarkkingdee.top

(double) a / b
来源：http://kbi.jqgufenzy.top

[S16] C：位操作置位
来源：http://yri.yuanzhike.top

x |= (1 << 3);
来源：http://zzu.hammf.cn

[S17] C：安全拼接字符串
来源：http://gys.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ucp.quarkkingdee.top

[S18] C：命令行参数
来源：http://arj.aibaodan.cn

int main(int argc, char **argv)
来源：http://rbx.tianlin.xyz

[S19] C：快速排序
来源：http://kou.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://pwz.nanxuanxn.top

[S20] C：二分查找
来源：http://vls.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kqj.snrcjt.cn

[S21] C：字符类别判断
来源：http://smm.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://spj.birdmap.top

[S22] C：字符串转数字
来源：http://pug.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://neb.ydjk.org.cn

[S23] C：随机数
来源：http://yjk.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://smf.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://ygj.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mfl.hfpthk.cn

[S25] C：内存拷贝
来源：http://gmc.daria6918.cn

memcpy(dst, src, n);
来源：http://feb.ydzc1.top

[S26] C：内存清零
来源：http://tsf.uphjek.com

memset(a, 0, sizeof a);
来源：http://pvp.bjfxy.top

[S27] C：定义常量
来源：http://icd.hnxiangtu.top

const double PI = 3.14159;
来源：http://ybx.zhengqikj.top

[S28] C：静态变量
来源：http://olw.zhiwuduotai.top

static int counter = 0;
来源：http://lor.sweek.top

[S29] C：变参函数
来源：http://opb.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://agc.smart0.xyz

[S30] C：头文件保护
来源：http://ooy.yj202588.top

#ifndef X_H
来源：http://ytt.52xcode.cn

#define X_H
来源：http://dcf.svipenyu.cn

#endif
来源：http://njn.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://vsx.zdqjudy.top

#include <iostream>
来源：http://tgt.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://jec.chenzaomai.com

[S32] C++：字符串
来源：http://khf.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://fcd.zdbjq.cn

[S33] C++：vector 增删
来源：http://vlp.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vxx.tianlin.xyz

[S34] C++：遍历 vector
来源：http://gdf.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://oam.jinghuilouyu.cn

[S35] C++：map
来源：http://xph.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zyr.chenlongwang.top

[S36] C++：unordered_map
来源：http://osu.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rcn.fanxiaobao.xyz

[S37] C++：set
来源：http://rzk.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgn.jinyuanbaomall.cn

[S38] C++：排序
来源：http://kdt.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://mln.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://lsc.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kub.jqgfzy.top

[S40] C++：查找元素
来源：http://ntn.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xzh.fehbvm.com

[S41] C++：类与构造函数
来源：http://ecv.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oxb.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://rnc.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://rnq.yj20258.top

[S43] C++：智能指针
来源：http://abf.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://rvf.yuxming.cn

[S44] C++：引用传参
来源：http://cyl.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://rvz.iojbl.cn

[S45] C++：lambda
来源：http://lig.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://tpi.sjlbkw.cn

[S46] C++：函数模板
来源：http://smb.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rgx.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://uep.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfh.dashuyun.cn

[S48] C++：逐行读文件
来源：http://ysv.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://cpt.yongpay.top

while (std::getline(in, line)) { }
来源：http://yys.sweek.top

[S49] C++：写文件
来源：http://duc.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pnf.daxiang520.top

[S50] C++：格式化数字
来源：http://kkk.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ekx.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://bsc.9152youxi.cn

static_cast<double>(a) / b
来源：http://wts.yongpay.top

[S52] C++：const 与 noexcept
来源：http://khh.jianghu66.top

int size() const noexcept { return n_; }
来源：http://ncl.yonumen.top

[S53] C++：移动语义
来源：http://qgb.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://hid.ydjk.org.cn

[S54] C++：异常处理
来源：http://lga.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zzc.zycfv.cn

[S55] C++：结构化绑定
来源：http://ean.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://unf.sjlbkw.cn

[S56] C++：optional
来源：http://nlt.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rmm.daxiang520.top

[S57] C++：编译期常量
来源：http://vpz.gogol.net.cn

constexpr int N = 10;
来源：http://ynq.pycfn.com

[S58] C++：命名空间
来源：http://bel.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://obn.wangdashe.top

[S59] C++：静态断言
来源：http://xxt.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vay.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://kso.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isz.pycfn.com

================================================================================
来源：http://xut.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wby.cqqwz.cn

================================================================================
来源：http://glx.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://bbc.ydjk.org.cn

println("Hello")
来源：http://vee.yj20258.top

[T02] Kotlin：变量
来源：http://hzk.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zdl.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://wgm.sysykeji.top

"值: $b"
来源：http://dsx.snrcjt.cn

[T04] Kotlin：空安全
来源：http://lez.zdqjudy.top

val n: String? = null;  n?.length
来源：http://vsw.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://lwt.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zkz.xuanzx.com

[T06] Kotlin：集合映射
来源：http://suj.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rnv.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://wbn.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wim.aizwys.cn

[T08] Kotlin：数据类
来源：http://ryv.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://nzq.sweek.top

[T09] Kotlin：扩展函数
来源：http://oso.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://wpz.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://sya.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://udi.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://sas.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://doc.tarul.cn

[T12] Kotlin：解构声明
来源：http://pgn.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://hxj.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://pbg.yj20258888.top

val m = mapOf("a" to 1)
来源：http://kru.iojbl.cn

[T14] Kotlin：循环
来源：http://fom.c1oappe.top

for (i in 1..10) println(i)
来源：http://tdd.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://lhc.smart0.xyz

interface Shape { fun area(): Double }
来源：http://iko.cashguo.top

[T16] Swift：Hello World
来源：http://foe.jiagoushi.top

print("Hello")
来源：http://ukt.0kj1m.cn


<!-- 参考信息 -->