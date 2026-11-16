代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://gac.sxryk.cn

[R18] 遍历数组
来源：http://gbu.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://weo.sjlbkw.cn

[R19] 数组长度
来源：http://zec.0kj1m.cn

echo "${#arr[@]}"
来源：http://zgx.zhixingplan.top

[R20] 关联数组（字典）
来源：http://lhj.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gdz.xylfe.cn

[R21] 字符串长度
来源：http://wnq.yj202588.top

echo "${#s}"
来源：http://qfw.tian-w.cn

[R22] 截取子串
来源：http://pbq.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://lvx.meibo888.top

[R23] 字符串替换
来源：http://ssv.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tes.shzxlz.cn

[R24] 大小写转换
来源：http://zcs.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://vky.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://xvf.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pgj.aibaodan.cn

[R26] 命令替换
来源：http://jtz.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://eip.shanyushiyangkeji.top

[R27] 算术展开
来源：http://xos.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://xsv.xziqi.cn

[R28] 浮点运算
来源：http://gwt.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://oxc.jianghu66.top

[R29] 定义函数
来源：http://zyn.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rgq.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://ijp.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://xak.cqqwz.cn

[R31] 局部变量
来源：http://wby.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://vgu.daxiang520.top

[R32] 参数个数校验
来源：http://ewe.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ayd.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://ubr.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fjw.redwolf501.top

[R34] 退出时清理
来源：http://pto.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://pvf.cucudq.cn

[R35] 后台执行并等待
来源：http://gni.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sqc.tianlin.xyz

[R36] 并发执行多个任务
来源：http://gtx.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ljj.guannengcc.top

[R37] 把输出赋给变量
来源：http://vsp.ctjpmb.com

files=$(ls -1)
来源：http://dia.andypj.xyz

[R38] 管道串联
来源：http://iqf.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://xin.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://njo.tanke756.top

cmd > out.log 2>&1
来源：http://wkr.hnqzz.top

[R40] 追加写日志
来源：http://boa.cdnleiting.top

echo "log" >> out.log
来源：http://rjx.yfazqb.com

[R41] 丢弃输出
来源：http://uzz.hesvh.cn

cmd >/dev/null 2>&1
来源：http://eis.bjfxy.top

[R42] 输入重定向
来源：http://hnk.tianlin.xyz

wc -l < a.txt
来源：http://vkt.zdbjq.cn

[R43] 按名字查找文件
来源：http://hlc.guowangkeji.top

find . -name "*.log" -type f
来源：http://ypl.zhoulong.xyz

[R44] 按修改时间查找
来源：http://mpf.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://prs.gogol.net.cn

[R45] 批量删除
来源：http://lsg.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://kve.tian-w.cn

[R46] 递归替换文件内容
来源：http://qhe.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ath.svipenyu.cn

[R47] sed 单行替换
来源：http://qte.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nsl.ctjpmb.com

[R48] awk 取指定列
来源：http://whs.sweek.top

awk '{print $1, $3}' a.txt
来源：http://tbu.fehbvm.com

[R49] awk 带条件
来源：http://jyp.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fac.quarkkingdee.top

[R50] awk 求和
来源：http://pws.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://omr.tanke756.top

[R51] 排序去重取前几
来源：http://jtp.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mlg.hysaishi.cn

[R52] 统计行数
来源：http://yvx.dianchejie.cn

wc -l a.txt
来源：http://ffs.uphjek.com

[R53] 查看文件头与实时尾
来源：http://inm.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://olu.yj20258888.top

[R54] 比较两个文件
来源：http://cju.9152youxi.cn

diff a.txt b.txt
来源：http://lld.yueranfly.top

[R55] 压缩与解压
来源：http://crj.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ugq.feifeiyinyue.top

[R56] 远程拷贝
来源：http://pbf.haohaochexian.top

scp file user@host:/path/
来源：http://ykd.sweek.top

[R57] 远程执行命令
来源：http://rpf.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://pip.xylfe.cn

[R58] 下载文件
来源：http://xks.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vnl.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://mds.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nxl.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://qso.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qzb.tanke756.top

[R61] 磁盘占用
来源：http://vhf.gotoacloud.top

df -h;  du -sh *
来源：http://ttk.dashuyun.cn

[R62] 找最占空间的文件
来源：http://osd.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://pvw.yongpay.top

[R63] 内存与进程
来源：http://ebd.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://xhp.jqgfzy.top

[R64] 结束进程
来源：http://mii.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://ihb.zdbjq.cn

[R65] 查看端口占用
来源：http://zfl.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlq.zhijiandao.cn

[R66] 定时任务
来源：http://nfx.cqqwz.cn

crontab -e;  crontab -l
来源：http://xzu.yj20258888.top

[R67] 生成随机十六进制串
来源：http://uot.yueranfly.top

openssl rand -hex 16
来源：http://ytg.zhijiandao.cn

[R68] 计算文件校验值
来源：http://vmr.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mej.redwolf501.top

[R69] 生成随机密码
来源：http://zcg.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://trd.zhengqikj.top

[R70] 时间戳与互转
来源：http://iig.cashguo.top

date +%s;  date -d @1700000000
来源：http://syk.cucudq.cn

[R71] 日期格式化
来源：http://fdx.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wnx.9152youxi.cn

[R72] 等待端口就绪
来源：http://elv.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cvu.shanyushiyangtech.top

[R73] 分割大日志
来源：http://cqu.316326.xyz

split -l 1000 big.log part_
来源：http://rpl.cashguo.top

[R74] 批量重命名
来源：http://ulu.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qkv.shzxlz.cn

[R75] 导出环境变量
来源：http://izp.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://gir.xuanzx.com

[R76] 使用临时文件
来源：http://khc.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lbt.wangdashe.top

[R77] 读取用户输入
来源：http://gea.zhoulong.xyz

read -rp "请输入: " ans
来源：http://jvg.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://xda.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kko.sweek.top

[R79] 解析命令行选项
来源：http://vsf.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ekk.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://zbr.jinqigfzy.top

time ./run.sh
来源：http://pxx.fehbvm.com

================================================================================
来源：http://nzr.fengsongda.top

S. C / C++ 专题
来源：http://grc.yonumen.top

================================================================================
来源：http://qxv.cdnleiting.top

[S01] C：Hello World
来源：http://pzs.epnwcf.com

#include <stdio.h>
来源：http://ceh.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwj.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://eks.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://hne.xylfe.cn

[S03] C：读入整数
来源：http://jcd.smart0.xyz

int x; scanf("%d", &x);
来源：http://fri.fengsongda.top

[S04] C：字符串复制
来源：http://tye.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gjw.zhongyouzk.top

[S05] C：字符串长度
来源：http://qtf.tian-w.cn

strlen(s)
来源：http://nob.xinyue.icu

[S06] C：字符串比较
来源：http://qsf.gaohongyu789.top

strcmp(a, b) == 0
来源：http://lfi.yangfankeji.com

[S07] C：数组遍历求和
来源：http://wut.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ovc.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://vqi.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wbg.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://hyk.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ybw.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://sfm.sxryk.cn

int *p = &a;  *p = 5;
来源：http://sgk.jlsjyb.cn

[S11] C：逐行读文件
来源：http://rsx.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://pzq.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fqo.zdqjudy.top

fclose(f);
来源：http://fbf.gogol.net.cn

[S12] C：写文件
来源：http://fzo.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sze.yonumen.top

[S13] C：宏定义
来源：http://bef.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qzi.hesvh.cn

[S14] C：枚举
来源：http://klg.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://gur.chenlongwang.top

[S15] C：类型转换
来源：http://vdv.ydzc1.top

(double) a / b
来源：http://zwg.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://ufd.bjfxy.top

x |= (1 << 3);
来源：http://hnh.pycfn.com

[S17] C：安全拼接字符串
来源：http://flc.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tbw.hammf.cn

[S18] C：命令行参数
来源：http://bxe.fzhhl.top

int main(int argc, char **argv)
来源：http://wli.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://voj.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://woy.52xcode.cn

[S20] C：二分查找
来源：http://cil.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tbh.52xcode.cn

[S21] C：字符类别判断
来源：http://qda.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dtt.yongpay.top

[S22] C：字符串转数字
来源：http://qkx.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qsd.ppjwa.cn

[S23] C：随机数
来源：http://dec.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bac.epnwcf.com

[S24] C：获取本地时间
来源：http://oid.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wdl.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://gls.ppjwa.cn

memcpy(dst, src, n);
来源：http://qkc.svipenyu.cn

[S26] C：内存清零
来源：http://sta.316326.xyz

memset(a, 0, sizeof a);
来源：http://xok.tianlin.xyz

[S27] C：定义常量
来源：http://zpa.nanxinkj.top

const double PI = 3.14159;
来源：http://dsq.ydjk.org.cn

[S28] C：静态变量
来源：http://emi.hcnkem.com

static int counter = 0;
来源：http://uqj.gzhubu.top

[S29] C：变参函数
来源：http://wwa.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://udf.shangyingyoupin.top

[S30] C：头文件保护
来源：http://jia.hywenlv.cn

#ifndef X_H
来源：http://xnc.ctjpmb.com

#define X_H
来源：http://win.zhixingplan.top

#endif
来源：http://ljg.0kj1m.cn

[S31] C++：Hello World
来源：http://fqf.chenzaomai.com

#include <iostream>
来源：http://wqr.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://qci.nanxinkj.top

[S32] C++：字符串
来源：http://eke.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://daf.tianlin.xyz

[S33] C++：vector 增删
来源：http://ssa.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lwt.haohaochexian.top

[S34] C++：遍历 vector
来源：http://rzr.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://bob.nanxuanxn.top

[S35] C++：map
来源：http://gdo.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ezk.yongpay.top

[S36] C++：unordered_map
来源：http://dfq.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://reh.jlsjyb.cn

[S37] C++：set
来源：http://ann.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvo.hammf.cn

[S38] C++：排序
来源：http://gll.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://mgr.meibo888.top

[S39] C++：自定义比较器排序
来源：http://ysf.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qnv.ivvv.top

[S40] C++：查找元素
来源：http://nwr.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mij.snrcjt.cn

[S41] C++：类与构造函数
来源：http://dru.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vxv.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://nca.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://msl.zdqjudy.top

[S43] C++：智能指针
来源：http://dyt.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://sql.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://usl.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://tfz.zdqjudy.top

[S45] C++：lambda
来源：http://yyj.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://psd.sxryk.cn

[S46] C++：函数模板
来源：http://czi.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kyu.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://icy.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jgw.jqgfzy.top

[S48] C++：逐行读文件
来源：http://hsd.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mly.cucudq.cn

while (std::getline(in, line)) { }
来源：http://tbm.wangdashe.top

[S49] C++：写文件
来源：http://xcu.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rpz.nanxuanxn.top

[S50] C++：格式化数字
来源：http://hxl.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rur.hywenlv.cn

[S51] C++：显式类型转换
来源：http://bza.zycfv.cn

static_cast<double>(a) / b
来源：http://lai.hammf.cn

[S52] C++：const 与 noexcept
来源：http://lrq.ydzc1.top

int size() const noexcept { return n_; }
来源：http://brh.ybcxt.top

[S53] C++：移动语义
来源：http://bjo.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://bds.xuanzx.com

[S54] C++：异常处理
来源：http://coc.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vyu.hcnkem.com

[S55] C++：结构化绑定
来源：http://xfi.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://obr.fengsongda.top

[S56] C++：optional
来源：http://ajd.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zbl.fehbvm.com

[S57] C++：编译期常量
来源：http://izp.daxiang520.top

constexpr int N = 10;
来源：http://vuu.jinqigfzy.top

[S58] C++：命名空间
来源：http://qex.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://bzu.pycfn.com

[S59] C++：静态断言
来源：http://mot.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qph.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://owe.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gum.xylfe.cn

================================================================================
来源：http://fbo.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qhc.yongpay.top

================================================================================
来源：http://xck.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://qwn.bjfxy.top

println("Hello")
来源：http://kex.smart0.xyz

[T02] Kotlin：变量
来源：http://jpp.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tpe.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://lxf.birdmap.top

"值: $b"
来源：http://reu.zdbjq.cn

[T04] Kotlin：空安全
来源：http://vxe.zhixingplan.top

val n: String? = null;  n?.length
来源：http://sgz.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://qob.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rkv.yongpay.top

[T06] Kotlin：集合映射
来源：http://oza.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nvz.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://uhq.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lka.cqqwz.cn

[T08] Kotlin：数据类
来源：http://rkn.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://vnh.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://ume.yonumen.top

fun String.exclaim() = this + "!"
来源：http://jlw.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://zpe.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tdt.yvedp.cn

[T11] Kotlin：协程
来源：http://nea.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rms.316326.xyz

[T12] Kotlin：解构声明
来源：http://afp.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://ore.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://thf.cucudq.cn

val m = mapOf("a" to 1)
来源：http://xlx.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://axw.9152youxi.cn

for (i in 1..10) println(i)
来源：http://ino.xziqi.cn

[T15] Kotlin：接口
来源：http://bha.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://yis.aibaodan.cn

[T16] Swift：Hello World
来源：http://ayk.cucudq.cn

print("Hello")
来源：http://xfs.fktsv.cn

[T17] Swift：变量与常量
来源：http://yta.smart0.xyz

var a = 1;  let b = 2
来源：http://uwe.uphjek.com

[T18] Swift：字符串插值
来源：http://jqp.jinghuilouyu.cn

"值: \(b)"
来源：http://ibx.chenlongwang.top

[T19] Swift：可选绑定
来源：http://iif.nanxinkj.top

if let n = opt { print(n) }
来源：http://hrd.sxryk.cn

[T20] Swift：数组操作
来源：http://mvk.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://nav.havefunace.top


<!-- 参考信息 -->