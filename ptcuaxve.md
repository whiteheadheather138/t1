代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://xru.yj202588.top

[R18] 遍历数组
来源：http://gld.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qut.vehdjk.com

[R19] 数组长度
来源：http://bug.gaohongyu789.top

echo "${#arr[@]}"
来源：http://ynv.hnqzz.top

[R20] 关联数组（字典）
来源：http://vse.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nms.jinqigufen.top

[R21] 字符串长度
来源：http://xud.ywan-chungtsiang.top

echo "${#s}"
来源：http://xgj.yangfankeji.com

[R22] 截取子串
来源：http://jwh.jinqigfzy.top

echo "${s:0:5}"
来源：http://nlb.yangfankeji.com

[R23] 字符串替换
来源：http://yss.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pve.guannengcc.top

[R24] 大小写转换
来源：http://xdg.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://iuq.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://nda.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://euj.hysaishi.cn

[R26] 命令替换
来源：http://itj.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://xia.cdnleiting.top

[R27] 算术展开
来源：http://wjp.guannengcc.top

echo $((1 + 2 * 3))
来源：http://vpl.bbcook.cn

[R28] 浮点运算
来源：http://yjo.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://xfx.hfpthk.cn

[R29] 定义函数
来源：http://zyp.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://twk.yuxming.cn

[R30] 函数返回状态码
来源：http://vra.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://ezs.shangyingyoupin.top

[R31] 局部变量
来源：http://cmr.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://psa.epnwcf.com

[R32] 参数个数校验
来源：http://aky.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yct.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://ukg.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hgc.zdbjq.cn

[R34] 退出时清理
来源：http://wla.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xtq.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://qvg.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lxc.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://qog.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vey.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://pds.zhongyouzk.top

files=$(ls -1)
来源：http://dsw.feifeiyinyue.top

[R38] 管道串联
来源：http://fcq.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://btm.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://mnl.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://csv.tanke756.top

[R40] 追加写日志
来源：http://wwm.xinyue.icu

echo "log" >> out.log
来源：http://xvi.bjfxy.top

[R41] 丢弃输出
来源：http://xtz.xziqi.cn

cmd >/dev/null 2>&1
来源：http://gpz.ehwqpu.com

[R42] 输入重定向
来源：http://iqo.haohaochexian.top

wc -l < a.txt
来源：http://qbx.zhixingplan.top

[R43] 按名字查找文件
来源：http://dyp.havefunace.top

find . -name "*.log" -type f
来源：http://lwd.hnxiangtu.top

[R44] 按修改时间查找
来源：http://ram.nanxinkj.top

find . -mtime -7 -type f
来源：http://olj.smart0.xyz

[R45] 批量删除
来源：http://pth.xylfe.cn

find . -name "*.tmp" -delete
来源：http://mjy.yj20258.top

[R46] 递归替换文件内容
来源：http://cjx.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bem.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://wzy.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://krr.chenzaomai.com

[R48] awk 取指定列
来源：http://eqo.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://mvm.cdnleiting.top

[R49] awk 带条件
来源：http://qfh.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rqu.haohaochexian.top

[R50] awk 求和
来源：http://yyv.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aty.ybcxt.top

[R51] 排序去重取前几
来源：http://ymw.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vgf.yj202588.top

[R52] 统计行数
来源：http://iwz.chenzaomai.com

wc -l a.txt
来源：http://aot.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://zkh.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tut.pengpengdd.cyou

[R54] 比较两个文件
来源：http://ppf.pengpengdd.cyou

diff a.txt b.txt
来源：http://ips.quarkkingdee.top

[R55] 压缩与解压
来源：http://uak.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kqt.zdbjq.cn

[R56] 远程拷贝
来源：http://rnr.hammf.cn

scp file user@host:/path/
来源：http://ynh.316326.xyz

[R57] 远程执行命令
来源：http://rkg.hywenlv.cn

ssh user@host 'uptime'
来源：http://npn.pycfn.com

[R58] 下载文件
来源：http://oph.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ajk.fengsongda.top

[R59] 发 POST JSON
来源：http://yrr.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://esm.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://qaz.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xhv.cqqwz.cn

[R61] 磁盘占用
来源：http://laq.yongpay.top

df -h;  du -sh *
来源：http://nfv.meibo888.top

[R62] 找最占空间的文件
来源：http://ldb.316326.xyz

du -ah . | sort -rh | head -10
来源：http://koo.tianlin.xyz

[R63] 内存与进程
来源：http://qtw.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://cbp.c1oappe.top

[R64] 结束进程
来源：http://gmd.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://yfx.gaohongyu789.top

[R65] 查看端口占用
来源：http://iyl.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ewg.cucudq.cn

[R66] 定时任务
来源：http://zso.fehbvm.com

crontab -e;  crontab -l
来源：http://unl.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://oey.shzxlz.cn

openssl rand -hex 16
来源：http://uup.jianghu66.top

[R68] 计算文件校验值
来源：http://twj.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mqs.pengpengdd.cyou

[R69] 生成随机密码
来源：http://fro.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://zyt.daxiang520.top

[R70] 时间戳与互转
来源：http://aqw.xinyue.icu

date +%s;  date -d @1700000000
来源：http://hli.hcnkem.com

[R71] 日期格式化
来源：http://csi.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://isw.zdqjudy.top

[R72] 等待端口就绪
来源：http://guu.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lad.feifeiyinyue.top

[R73] 分割大日志
来源：http://fnz.sweek.top

split -l 1000 big.log part_
来源：http://apg.pycfn.com

[R74] 批量重命名
来源：http://fuk.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tvx.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://nee.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://elc.pengpengdd.cyou

[R76] 使用临时文件
来源：http://wru.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ipx.nanxuanxn.top

[R77] 读取用户输入
来源：http://cih.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://cce.yj20258.top

[R78] 交互式菜单
来源：http://uwf.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lbx.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://vcs.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ssh.tarul.cn

[R80] 查看脚本执行耗时
来源：http://xph.birdmap.top

time ./run.sh
来源：http://glx.wangdashe.top

================================================================================
来源：http://orw.pycfn.com

S. C / C++ 专题
来源：http://hpt.jinqigfzy.top

================================================================================
来源：http://plk.nwbrower.top

[S01] C：Hello World
来源：http://bnu.zhixingplan.top

#include <stdio.h>
来源：http://uox.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xek.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://mhe.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://jvj.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://tyl.hesvh.cn

int x; scanf("%d", &x);
来源：http://hsu.zdqjudy.top

[S04] C：字符串复制
来源：http://vdf.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://csk.zycfv.cn

[S05] C：字符串长度
来源：http://avo.guowangkeji.top

strlen(s)
来源：http://khd.sjlbkw.cn

[S06] C：字符串比较
来源：http://qks.tanke756.top

strcmp(a, b) == 0
来源：http://msf.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://dld.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sxm.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://lgs.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ywg.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://qrv.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vmb.gzhubu.top

[S10] C：指针与解引用
来源：http://fgt.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://yuh.52xcode.cn

[S11] C：逐行读文件
来源：http://gkd.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kgt.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://omt.jiagoushi.top

fclose(f);
来源：http://ckm.tanke756.top

[S12] C：写文件
来源：http://vxz.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ncq.ppjwa.cn

[S13] C：宏定义
来源：http://sif.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dzc.xinyue.icu

[S14] C：枚举
来源：http://fmd.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://pqk.hcnkem.com

[S15] C：类型转换
来源：http://rbl.sjlbkw.cn

(double) a / b
来源：http://wel.316326.xyz

[S16] C：位操作置位
来源：http://wor.fzhhl.top

x |= (1 << 3);
来源：http://tis.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://abx.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blw.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://uvq.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://gui.52xcode.cn

[S19] C：快速排序
来源：http://xoj.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://hch.hysaishi.cn

[S20] C：二分查找
来源：http://qtq.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oji.yueranfly.top

[S21] C：字符类别判断
来源：http://bli.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bcv.fengsongda.top

[S22] C：字符串转数字
来源：http://apd.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rdd.pengpengdd.cyou

[S23] C：随机数
来源：http://gfi.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lgo.yj202588.top

[S24] C：获取本地时间
来源：http://yhj.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xsn.guannengcc.top

[S25] C：内存拷贝
来源：http://mxk.chenzaomai.com

memcpy(dst, src, n);
来源：http://rig.sxryk.cn

[S26] C：内存清零
来源：http://hmj.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://giq.yangfankeji.com

[S27] C：定义常量
来源：http://obi.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://jiz.ydzc1.top

[S28] C：静态变量
来源：http://yii.9152youxi.cn

static int counter = 0;
来源：http://ved.sufxvd.cn

[S29] C：变参函数
来源：http://ydf.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cbe.fehbvm.com

[S30] C：头文件保护
来源：http://xlt.bbcook.cn

#ifndef X_H
来源：http://xja.chenjidiqi.icu

#define X_H
来源：http://cgq.meibo888.top

#endif
来源：http://riw.hysaishi.cn

[S31] C++：Hello World
来源：http://cgf.pycfn.com

#include <iostream>
来源：http://xmq.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dmg.gzhubu.top

[S32] C++：字符串
来源：http://amf.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://xax.jiagoushi.top

[S33] C++：vector 增删
来源：http://cmw.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yhm.hfpthk.cn

[S34] C++：遍历 vector
来源：http://gpy.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://oiy.cdnleiting.top

[S35] C++：map
来源：http://glg.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pxd.yj202588.top

[S36] C++：unordered_map
来源：http://jdj.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ulw.sjlbkw.cn

[S37] C++：set
来源：http://oop.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pxo.bbcook.cn

[S38] C++：排序
来源：http://imy.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://fhm.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://yfn.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uqx.nanxuanxn.top

[S40] C++：查找元素
来源：http://qhg.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sgb.ehwqpu.com

[S41] C++：类与构造函数
来源：http://onf.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zvx.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://hjr.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://npy.xylfe.cn

[S43] C++：智能指针
来源：http://tfp.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://aqo.cheryme.top

[S44] C++：引用传参
来源：http://yln.meibo888.top

void inc(int &x) { ++x; }
来源：http://imm.c1oappe.top

[S45] C++：lambda
来源：http://liy.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uhy.hfpthk.cn

[S46] C++：函数模板
来源：http://rrq.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dkv.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://usi.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ghg.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://gvn.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://grj.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://iye.jinghuilouyu.cn

[S49] C++：写文件
来源：http://qcn.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://scv.haohaochexian.top

[S50] C++：格式化数字
来源：http://iun.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wjc.yongpay.top

[S51] C++：显式类型转换
来源：http://cbx.xinyue.icu

static_cast<double>(a) / b
来源：http://djf.havefunace.top

[S52] C++：const 与 noexcept
来源：http://rst.zycfv.cn

int size() const noexcept { return n_; }
来源：http://loq.quarkkingdee.top

[S53] C++：移动语义
来源：http://mug.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://eob.hongshengwenyu.top

[S54] C++：异常处理
来源：http://ntk.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yea.smart0.xyz

[S55] C++：结构化绑定
来源：http://ldf.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tqk.chenlongwang.top

[S56] C++：optional
来源：http://byg.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zhs.daria6918.cn

[S57] C++：编译期常量
来源：http://hqd.smart0.xyz

constexpr int N = 10;
来源：http://jrs.tianlin.xyz

[S58] C++：命名空间
来源：http://qds.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://vym.feifeiyinyue.top

[S59] C++：静态断言
来源：http://ssq.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ern.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://yrt.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wxr.wangshuangyany.cn

================================================================================
来源：http://lfq.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dam.iojbl.cn

================================================================================
来源：http://fst.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://xju.chenlongwang.top

println("Hello")
来源：http://cuf.zdbjq.cn

[T02] Kotlin：变量
来源：http://ksk.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fxf.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://kbp.svipenyu.cn

"值: $b"
来源：http://bhu.cucudq.cn

[T04] Kotlin：空安全
来源：http://lnc.fengsongda.top

val n: String? = null;  n?.length
来源：http://qgf.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://inp.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qhf.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://fwa.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://abg.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://vxe.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ovy.yj20258.top

[T08] Kotlin：数据类
来源：http://nqx.cheryme.top

data class User(val name: String, val age: Int)
来源：http://gru.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://zob.yj20258.top

fun String.exclaim() = this + "!"
来源：http://iuf.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://fzt.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nqp.hnxiangtu.top

[T11] Kotlin：协程
来源：http://pve.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kmm.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://qjo.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://bvy.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://eyw.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://gos.xziqi.cn

[T14] Kotlin：循环
来源：http://vpk.0kj1m.cn

for (i in 1..10) println(i)
来源：http://opr.hammf.cn

[T15] Kotlin：接口
来源：http://zpt.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://lbn.zhixingplan.top

[T16] Swift：Hello World
来源：http://qwo.gogol.net.cn

print("Hello")
来源：http://nll.meibo888.top

[T17] Swift：变量与常量
来源：http://lfa.zdbjq.cn

var a = 1;  let b = 2
来源：http://cas.yj20258.top

[T18] Swift：字符串插值
来源：http://wwj.shangyingyoupin.top

"值: \(b)"
来源：http://oce.nwbrower.top

[T19] Swift：可选绑定
来源：http://lug.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://rmu.jiagoushi.top

[T20] Swift：数组操作
来源：http://vqo.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://lmk.ppjwa.cn


<!-- 参考信息 -->