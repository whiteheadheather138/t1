代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://ouk.ctjpmb.com

[R18] 遍历数组
来源：http://pdo.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rfb.zdqjudy.top

[R19] 数组长度
来源：http://cmw.tian-w.cn

echo "${#arr[@]}"
来源：http://ekb.chenlongwang.top

[R20] 关联数组（字典）
来源：http://qqj.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ffz.fanxiaobao.xyz

[R21] 字符串长度
来源：http://qoy.yuanzhike.top

echo "${#s}"
来源：http://oeh.52xcode.cn

[R22] 截取子串
来源：http://bgm.tianlin.xyz

echo "${s:0:5}"
来源：http://edl.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://oel.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cih.jianghu66.top

[R24] 大小写转换
来源：http://bfk.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uja.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://efd.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://sqw.sysykeji.top

[R26] 命令替换
来源：http://ypj.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://ibc.ydzc1.top

[R27] 算术展开
来源：http://rtv.ivvv.top

echo $((1 + 2 * 3))
来源：http://xks.snrcjt.cn

[R28] 浮点运算
来源：http://ych.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://sdl.nanxinkj.top

[R29] 定义函数
来源：http://rzd.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dyb.hesvh.cn

[R30] 函数返回状态码
来源：http://fds.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://kjb.chenzaomai.com

[R31] 局部变量
来源：http://wdk.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://bjp.hammf.cn

[R32] 参数个数校验
来源：http://nyv.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ivg.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://ihx.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pwp.xylfe.cn

[R34] 退出时清理
来源：http://btg.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://twq.aibaodan.cn

[R35] 后台执行并等待
来源：http://pjo.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xjv.smart0.xyz

[R36] 并发执行多个任务
来源：http://xtn.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fkp.yongpay.top

[R37] 把输出赋给变量
来源：http://mln.cqqwz.cn

files=$(ls -1)
来源：http://cmq.iojbl.cn

[R38] 管道串联
来源：http://fnh.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://pzs.ivvv.top

[R39] 重定向标准输出与错误
来源：http://lcr.jlsjyb.cn

cmd > out.log 2>&1
来源：http://cok.xuanzx.com

[R40] 追加写日志
来源：http://rlz.shangyingyoupin.top

echo "log" >> out.log
来源：http://qcl.wangshuangyany.cn

[R41] 丢弃输出
来源：http://rwd.bjfxy.top

cmd >/dev/null 2>&1
来源：http://nqi.hysaishi.cn

[R42] 输入重定向
来源：http://zuz.hywenlv.cn

wc -l < a.txt
来源：http://wkg.52xcode.cn

[R43] 按名字查找文件
来源：http://ewl.ivvv.top

find . -name "*.log" -type f
来源：http://gch.wangdashe.top

[R44] 按修改时间查找
来源：http://uqu.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://hdj.jinqigufen.top

[R45] 批量删除
来源：http://gqs.fengsongda.top

find . -name "*.tmp" -delete
来源：http://awu.ybcxt.top

[R46] 递归替换文件内容
来源：http://ljl.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzg.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://lkk.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://vnp.xuetiantiany.cn

[R48] awk 取指定列
来源：http://ogp.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://cxs.cheryme.top

[R49] awk 带条件
来源：http://qhs.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dao.daria6918.cn

[R50] awk 求和
来源：http://ghb.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://tpv.hammf.cn

[R51] 排序去重取前几
来源：http://gwg.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://osj.smart0.xyz

[R52] 统计行数
来源：http://rfs.hnqzz.top

wc -l a.txt
来源：http://snj.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://uqn.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iiw.316326.xyz

[R54] 比较两个文件
来源：http://fak.hongshengwenyu.top

diff a.txt b.txt
来源：http://qrd.dashuyun.cn

[R55] 压缩与解压
来源：http://exm.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qec.fengsongda.top

[R56] 远程拷贝
来源：http://xbf.tarul.cn

scp file user@host:/path/
来源：http://yxm.hnxiangtu.top

[R57] 远程执行命令
来源：http://blw.hcnkem.com

ssh user@host 'uptime'
来源：http://khd.havefunace.top

[R58] 下载文件
来源：http://kvo.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://btv.zhongyouzk.top

[R59] 发 POST JSON
来源：http://duu.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aof.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://kbg.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://udi.xuetiantiany.cn

[R61] 磁盘占用
来源：http://ehm.sjlbkw.cn

df -h;  du -sh *
来源：http://bfm.sufxvd.cn

[R62] 找最占空间的文件
来源：http://bpy.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://ema.hnqzz.top

[R63] 内存与进程
来源：http://nbc.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://ewe.aibaodan.cn

[R64] 结束进程
来源：http://ank.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://hzj.tian-w.cn

[R65] 查看端口占用
来源：http://uue.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jds.shzxlz.cn

[R66] 定时任务
来源：http://hlx.quarkkingdee.top

crontab -e;  crontab -l
来源：http://jlz.yj20258888.top

[R67] 生成随机十六进制串
来源：http://cei.yj20258.top

openssl rand -hex 16
来源：http://yaa.zycfv.cn

[R68] 计算文件校验值
来源：http://ywb.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ehq.nanxinkj.top

[R69] 生成随机密码
来源：http://qtb.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://pcf.smart0.xyz

[R70] 时间戳与互转
来源：http://cjq.cucudq.cn

date +%s;  date -d @1700000000
来源：http://wvm.ctjpmb.com

[R71] 日期格式化
来源：http://sgf.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pqs.zdqjudy.top

[R72] 等待端口就绪
来源：http://sbj.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wbk.shanyushiyangtech.top

[R73] 分割大日志
来源：http://fvj.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://keq.jyoumei.cn

[R74] 批量重命名
来源：http://tqf.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lbe.sysykeji.top

[R75] 导出环境变量
来源：http://puy.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://rzr.vqdsnc.cn

[R76] 使用临时文件
来源：http://yeo.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dhl.tarul.cn

[R77] 读取用户输入
来源：http://xbl.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://ilu.zhiwuduotai.top

[R78] 交互式菜单
来源：http://mbn.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uvd.vqdsnc.cn

[R79] 解析命令行选项
来源：http://vau.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bnj.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://qyf.pengpengdd.cyou

time ./run.sh
来源：http://wln.ybcxt.top

================================================================================
来源：http://zme.316326.xyz

S. C / C++ 专题
来源：http://nzh.svipenyu.cn

================================================================================
来源：http://gpm.nanxinkj.top

[S01] C：Hello World
来源：http://agj.xziqi.cn

#include <stdio.h>
来源：http://cbr.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yqv.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://byn.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://lnz.iojbl.cn

[S03] C：读入整数
来源：http://dsz.tian-w.cn

int x; scanf("%d", &x);
来源：http://upm.ybcxt.top

[S04] C：字符串复制
来源：http://kcu.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pjr.daxiang520.top

[S05] C：字符串长度
来源：http://tti.gzhubu.top

strlen(s)
来源：http://pgz.hesvh.cn

[S06] C：字符串比较
来源：http://eag.svipenyu.cn

strcmp(a, b) == 0
来源：http://exb.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://hih.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jpc.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://xny.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ioa.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://zlm.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ytj.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://aoa.jianghu66.top

int *p = &a;  *p = 5;
来源：http://dhi.daxiang520.top

[S11] C：逐行读文件
来源：http://czu.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://ray.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fsx.nanxuanxn.top

fclose(f);
来源：http://lcx.havefunace.top

[S12] C：写文件
来源：http://shq.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bwu.yj20258.top

[S13] C：宏定义
来源：http://pvl.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://unj.sufxvd.cn

[S14] C：枚举
来源：http://nds.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://ozo.birdmap.top

[S15] C：类型转换
来源：http://oza.fengsongda.top

(double) a / b
来源：http://zzk.zycfv.cn

[S16] C：位操作置位
来源：http://hhf.xylfe.cn

x |= (1 << 3);
来源：http://kdj.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://bvx.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hxn.guannengcc.top

[S18] C：命令行参数
来源：http://apq.hnxiangtu.top

int main(int argc, char **argv)
来源：http://xaz.9152youxi.cn

[S19] C：快速排序
来源：http://dec.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://gnc.uphjek.com

[S20] C：二分查找
来源：http://hft.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bjj.jiagoushi.top

[S21] C：字符类别判断
来源：http://ssy.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://scz.ydzc1.top

[S22] C：字符串转数字
来源：http://emt.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://adp.guowangkeji.top

[S23] C：随机数
来源：http://esq.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xof.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://bgv.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dtx.zdqjudy.top

[S25] C：内存拷贝
来源：http://ayh.epnwcf.com

memcpy(dst, src, n);
来源：http://ypm.hywenlv.cn

[S26] C：内存清零
来源：http://eco.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://ahg.jiagoushi.top

[S27] C：定义常量
来源：http://acv.jqgfzy.top

const double PI = 3.14159;
来源：http://axq.ivvv.top

[S28] C：静态变量
来源：http://shr.shanyushiyangtech.top

static int counter = 0;
来源：http://tzx.ydzc1.top

[S29] C：变参函数
来源：http://duk.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://twl.jlsjyb.cn

[S30] C：头文件保护
来源：http://thl.redwolf501.top

#ifndef X_H
来源：http://ldo.xuetiantiany.cn

#define X_H
来源：http://ayc.ydzc1.top

#endif
来源：http://exa.pengpengdd.cyou

[S31] C++：Hello World
来源：http://gdv.gzhubu.top

#include <iostream>
来源：http://dqz.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ijk.yangfankeji.com

[S32] C++：字符串
来源：http://ptp.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://zio.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://qqk.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rjy.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://cnl.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://rpy.cheryme.top

[S35] C++：map
来源：http://ahd.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rtj.uphjek.com

[S36] C++：unordered_map
来源：http://zih.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bjj.sufxvd.cn

[S37] C++：set
来源：http://ijz.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mqk.sjlbkw.cn

[S38] C++：排序
来源：http://yzf.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://dud.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://epz.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bij.daria6918.cn

[S40] C++：查找元素
来源：http://rwx.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bdh.ppjwa.cn

[S41] C++：类与构造函数
来源：http://buv.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zhv.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://pda.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://enk.bbcook.cn

[S43] C++：智能指针
来源：http://zxs.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://oly.hongshengwenyu.top

[S44] C++：引用传参
来源：http://jzb.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://ozf.xziqi.cn

[S45] C++：lambda
来源：http://lls.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://net.ybcxt.top

[S46] C++：函数模板
来源：http://epf.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgo.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://hvn.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qur.aizwys.cn

[S48] C++：逐行读文件
来源：http://yet.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hmo.cheryme.top

while (std::getline(in, line)) { }
来源：http://ywr.yuanzhike.top

[S49] C++：写文件
来源：http://ciy.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lcr.316326.xyz

[S50] C++：格式化数字
来源：http://kcm.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fuw.sufxvd.cn

[S51] C++：显式类型转换
来源：http://rkb.redwolf501.top

static_cast<double>(a) / b
来源：http://grn.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://ptn.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://wga.yueranfly.top

[S53] C++：移动语义
来源：http://zbz.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://swv.ivvv.top

[S54] C++：异常处理
来源：http://xzk.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vim.hcnkem.com

[S55] C++：结构化绑定
来源：http://pvi.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xba.ydzc1.top

[S56] C++：optional
来源：http://qfg.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hll.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://jft.zdqjudy.top

constexpr int N = 10;
来源：http://rwa.hysaishi.cn

[S58] C++：命名空间
来源：http://hmd.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://wmo.yfazqb.com

[S59] C++：静态断言
来源：http://kte.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://epn.yongpay.top

[S60] C++：遍历并删除元素
来源：http://iil.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vuq.sufxvd.cn

================================================================================
来源：http://bxe.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ytx.cashguo.top

================================================================================
来源：http://zlj.sxryk.cn

[T01] Kotlin：Hello World
来源：http://ecw.hywenlv.cn

println("Hello")
来源：http://dya.aibaodan.cn

[T02] Kotlin：变量
来源：http://ueg.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rtb.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://kwr.hongshengwenyu.top

"值: $b"
来源：http://ayf.ybcxt.top

[T04] Kotlin：空安全
来源：http://tzp.guannengcc.top

val n: String? = null;  n?.length
来源：http://adq.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://giw.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iqa.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://cuo.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://foi.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://upq.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hjn.gotoacloud.top

[T08] Kotlin：数据类
来源：http://nmq.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://okv.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://fqt.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://opx.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://eks.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wqs.dianchejie.cn

[T11] Kotlin：协程
来源：http://xtf.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fts.316326.xyz

[T12] Kotlin：解构声明
来源：http://xto.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://bsa.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://yop.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://fjm.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://atq.sweek.top

for (i in 1..10) println(i)
来源：http://mxo.yangfankeji.com

[T15] Kotlin：接口
来源：http://ibv.meibo888.top

interface Shape { fun area(): Double }
来源：http://ext.andypj.xyz

[T16] Swift：Hello World
来源：http://nkj.shuidangran.top

print("Hello")
来源：http://bzj.yueranfly.top

[T17] Swift：变量与常量
来源：http://itq.shzxlz.cn

var a = 1;  let b = 2
来源：http://bvd.ppjwa.cn

[T18] Swift：字符串插值
来源：http://myt.guannengcc.top

"值: \(b)"
来源：http://rng.iojbl.cn

[T19] Swift：可选绑定
来源：http://hnj.shuidangran.top

if let n = opt { print(n) }
来源：http://dpv.tian-w.cn

[T20] Swift：数组操作
来源：http://ddi.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://sza.vqdsnc.cn


<!-- 参考信息 -->