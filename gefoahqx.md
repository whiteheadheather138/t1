代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://xvj.nanxinkj.top

[R14] C 风格 for
来源：http://teb.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oss.xinyue.icu

[R15] while 逐行读文件
来源：http://lky.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gfw.fengsongda.top

[R16] until 等待条件
来源：http://ipr.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ess.yvedp.cn

[R17] 数组定义与取值
来源：http://xob.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://eec.yangfankeji.com

[R18] 遍历数组
来源：http://dsl.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zzy.hnqzz.top

[R19] 数组长度
来源：http://rvd.ppjwa.cn

echo "${#arr[@]}"
来源：http://lim.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://vfv.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jdt.zycfv.cn

[R21] 字符串长度
来源：http://zrw.zhongyouzk.top

echo "${#s}"
来源：http://lyx.redwolf501.top

[R22] 截取子串
来源：http://bvg.zhiwuduotai.top

echo "${s:0:5}"
来源：http://gpq.yuxming.cn

[R23] 字符串替换
来源：http://ivx.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zdc.gogol.net.cn

[R24] 大小写转换
来源：http://cah.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ckv.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://eao.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qqa.chenjidiqi.icu

[R26] 命令替换
来源：http://yvz.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://kxu.haohaochexian.top

[R27] 算术展开
来源：http://rmn.yueranfly.top

echo $((1 + 2 * 3))
来源：http://lof.xuanzx.com

[R28] 浮点运算
来源：http://rlv.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://bxb.smart0.xyz

[R29] 定义函数
来源：http://ffe.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xur.pycfn.com

[R30] 函数返回状态码
来源：http://fiu.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://qmj.cdnleiting.top

[R31] 局部变量
来源：http://yao.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://snm.yonumen.top

[R32] 参数个数校验
来源：http://wcq.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hha.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://tit.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ene.havefunace.top

[R34] 退出时清理
来源：http://whw.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://rla.jinqigufen.top

[R35] 后台执行并等待
来源：http://irx.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vxl.sysykeji.top

[R36] 并发执行多个任务
来源：http://trt.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvj.chenzaomai.com

[R37] 把输出赋给变量
来源：http://hds.yangfankeji.com

files=$(ls -1)
来源：http://add.xuetiantiany.cn

[R38] 管道串联
来源：http://kxr.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://iox.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://tmu.fktsv.cn

cmd > out.log 2>&1
来源：http://rwo.sxryk.cn

[R40] 追加写日志
来源：http://bmo.ydzc1.top

echo "log" >> out.log
来源：http://pni.gaohongyu789.top

[R41] 丢弃输出
来源：http://esd.xylfe.cn

cmd >/dev/null 2>&1
来源：http://foa.ivvv.top

[R42] 输入重定向
来源：http://cik.sysykeji.top

wc -l < a.txt
来源：http://xgl.daxiang520.top

[R43] 按名字查找文件
来源：http://wix.316326.xyz

find . -name "*.log" -type f
来源：http://gkq.yueranfly.top

[R44] 按修改时间查找
来源：http://qec.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://vfl.dashuyun.cn

[R45] 批量删除
来源：http://ojj.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://pce.dashuyun.cn

[R46] 递归替换文件内容
来源：http://kcd.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://edr.0kj1m.cn

[R47] sed 单行替换
来源：http://com.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://bfk.tarul.cn

[R48] awk 取指定列
来源：http://hwp.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://kcs.chenzaomai.com

[R49] awk 带条件
来源：http://tio.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tim.shanyushiyangtech.top

[R50] awk 求和
来源：http://xrd.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://zqo.tian-w.cn

[R51] 排序去重取前几
来源：http://oev.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mgb.hywenlv.cn

[R52] 统计行数
来源：http://kzn.hysaishi.cn

wc -l a.txt
来源：http://sdp.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://old.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rgf.yj20258.top

[R54] 比较两个文件
来源：http://avb.yj20258.top

diff a.txt b.txt
来源：http://yae.wangshuangyany.cn

[R55] 压缩与解压
来源：http://gkr.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://csz.nwbrower.top

[R56] 远程拷贝
来源：http://jgr.nwbrower.top

scp file user@host:/path/
来源：http://zea.316326.xyz

[R57] 远程执行命令
来源：http://uxu.svipenyu.cn

ssh user@host 'uptime'
来源：http://byy.hammf.cn

[R58] 下载文件
来源：http://oft.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oax.daria6918.cn

[R59] 发 POST JSON
来源：http://jkh.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wto.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://kzl.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tgn.chenlongwang.top

[R61] 磁盘占用
来源：http://kil.jqgufenzy.top

df -h;  du -sh *
来源：http://kfe.daxiang520.top

[R62] 找最占空间的文件
来源：http://dap.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://pyf.uphjek.com

[R63] 内存与进程
来源：http://yhq.tarul.cn

free -h;  ps aux | grep nginx
来源：http://amb.cashguo.top

[R64] 结束进程
来源：http://jck.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://phj.cashguo.top

[R65] 查看端口占用
来源：http://cxp.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pnt.jinghuilouyu.cn

[R66] 定时任务
来源：http://dsh.jinqigufen.top

crontab -e;  crontab -l
来源：http://bms.tanke756.top

[R67] 生成随机十六进制串
来源：http://ilj.hysaishi.cn

openssl rand -hex 16
来源：http://rok.daria6918.cn

[R68] 计算文件校验值
来源：http://oih.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://gtz.shangyingyoupin.top

[R69] 生成随机密码
来源：http://zai.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://vco.bjfxy.top

[R70] 时间戳与互转
来源：http://zns.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://ejx.yfazqb.com

[R71] 日期格式化
来源：http://tft.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cix.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://mrv.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rdf.316326.xyz

[R73] 分割大日志
来源：http://ggx.jinqigfzy.top

split -l 1000 big.log part_
来源：http://ppx.yj20258.top

[R74] 批量重命名
来源：http://htg.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zyc.epnwcf.com

[R75] 导出环境变量
来源：http://ilr.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://syz.yonumen.top

[R76] 使用临时文件
来源：http://krp.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://umm.ybcxt.top

[R77] 读取用户输入
来源：http://czk.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://bol.sweek.top

[R78] 交互式菜单
来源：http://ddz.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://toz.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://oan.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lnp.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://mkz.pengpengdd.cyou

time ./run.sh
来源：http://nvg.gotoacloud.top

================================================================================
来源：http://nsh.hcnkem.com

S. C / C++ 专题
来源：http://kce.pengpengdd.cyou

================================================================================
来源：http://dbh.sufxvd.cn

[S01] C：Hello World
来源：http://qtj.jianghu66.top

#include <stdio.h>
来源：http://rrr.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hhh.ybcxt.top

[S02] C：变量与格式化输出
来源：http://qwm.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://elj.vqdsnc.cn

[S03] C：读入整数
来源：http://kjd.c1oappe.top

int x; scanf("%d", &x);
来源：http://ddq.yvedp.cn

[S04] C：字符串复制
来源：http://ruy.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://try.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://grl.hesvh.cn

strlen(s)
来源：http://ydp.iojbl.cn

[S06] C：字符串比较
来源：http://zcc.ydjk.org.cn

strcmp(a, b) == 0
来源：http://ebw.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://hbp.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pwf.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://yee.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://osg.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://bly.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ssl.wangdashe.top

[S10] C：指针与解引用
来源：http://zov.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://daw.guowangkeji.top

[S11] C：逐行读文件
来源：http://qpo.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://fuz.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xml.shanyushiyangkeji.top

fclose(f);
来源：http://gdl.zhoulong.xyz

[S12] C：写文件
来源：http://dbs.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://stn.xuetiantiany.cn

[S13] C：宏定义
来源：http://qho.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wkg.zdqjudy.top

[S14] C：枚举
来源：http://kry.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://pbo.dashuyun.cn

[S15] C：类型转换
来源：http://uzc.zhongyouzk.top

(double) a / b
来源：http://rba.wangshuangyany.cn

[S16] C：位操作置位
来源：http://zlr.cashguo.top

x |= (1 << 3);
来源：http://unc.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://onv.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zkf.yonumen.top

[S18] C：命令行参数
来源：http://ylz.cqqwz.cn

int main(int argc, char **argv)
来源：http://swd.gaohongyu789.top

[S19] C：快速排序
来源：http://vqq.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://obv.jlsjyb.cn

[S20] C：二分查找
来源：http://wog.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kab.jinqigufen.top

[S21] C：字符类别判断
来源：http://wls.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syn.hywenlv.cn

[S22] C：字符串转数字
来源：http://txy.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://ige.gotoacloud.top

[S23] C：随机数
来源：http://njt.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xfc.smart0.xyz

[S24] C：获取本地时间
来源：http://plc.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rsl.xinyue.icu

[S25] C：内存拷贝
来源：http://boy.sjlbkw.cn

memcpy(dst, src, n);
来源：http://rcu.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://cba.yonumen.top

memset(a, 0, sizeof a);
来源：http://scd.aibaodan.cn

[S27] C：定义常量
来源：http://hzh.bjfxy.top

const double PI = 3.14159;
来源：http://mkj.zhengqikj.top

[S28] C：静态变量
来源：http://pic.gaohongyu789.top

static int counter = 0;
来源：http://jte.zhoulong.xyz

[S29] C：变参函数
来源：http://uoa.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dyu.sysykeji.top

[S30] C：头文件保护
来源：http://xmn.jianghu66.top

#ifndef X_H
来源：http://zpw.zycfv.cn

#define X_H
来源：http://ery.hnxiangtu.top

#endif
来源：http://ykf.haohaochexian.top

[S31] C++：Hello World
来源：http://cyu.chenlongwang.top

#include <iostream>
来源：http://dwh.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://pic.vqdsnc.cn

[S32] C++：字符串
来源：http://ggd.yonumen.top

std::string s = "hi";  s += "!";
来源：http://qyt.ctjpmb.com

[S33] C++：vector 增删
来源：http://xwy.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://csz.fengsongda.top

[S34] C++：遍历 vector
来源：http://mkx.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://ucq.fengsongda.top

[S35] C++：map
来源：http://new.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dtz.jyoumei.cn

[S36] C++：unordered_map
来源：http://tyw.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://slk.haohaochexian.top

[S37] C++：set
来源：http://lme.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zns.kuanghao11.cn

[S38] C++：排序
来源：http://npy.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://swy.ivvv.top

[S39] C++：自定义比较器排序
来源：http://xzj.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://exb.fehbvm.com

[S40] C++：查找元素
来源：http://awt.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fbl.cheryme.top

[S41] C++：类与构造函数
来源：http://ubd.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lqi.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://rku.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://wlk.jyoumei.cn

[S43] C++：智能指针
来源：http://yif.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://iwc.yuanzhike.top

[S44] C++：引用传参
来源：http://gal.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://mpx.daxiang520.top

[S45] C++：lambda
来源：http://aqh.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://kwf.zycfv.cn

[S46] C++：函数模板
来源：http://hfa.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yeb.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://jhq.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dry.shuidangran.top

[S48] C++：逐行读文件
来源：http://qod.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://qeg.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://hkh.jqgufenzy.top

[S49] C++：写文件
来源：http://kkb.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uzq.haohaochexian.top

[S50] C++：格式化数字
来源：http://rwp.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rsi.iojbl.cn

[S51] C++：显式类型转换
来源：http://afg.nanxuanxn.top

static_cast<double>(a) / b
来源：http://zuc.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://yzt.fktsv.cn

int size() const noexcept { return n_; }
来源：http://pqh.yfazqb.com

[S53] C++：移动语义
来源：http://frh.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://ijx.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://rhe.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dsn.guowangkeji.top

[S55] C++：结构化绑定
来源：http://eug.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uhn.redwolf501.top

[S56] C++：optional
来源：http://pwg.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hie.birdmap.top

[S57] C++：编译期常量
来源：http://zsh.yonumen.top

constexpr int N = 10;
来源：http://lwe.jianghu66.top

[S58] C++：命名空间
来源：http://yrn.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://utn.yj20258.top

[S59] C++：静态断言
来源：http://qrl.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sfa.uphjek.com

[S60] C++：遍历并删除元素
来源：http://kvy.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wza.gaohongyu789.top

================================================================================
来源：http://nju.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qgp.shuidangran.top

================================================================================
来源：http://lim.hesvh.cn

[T01] Kotlin：Hello World
来源：http://hsu.0kj1m.cn

println("Hello")
来源：http://pgl.aibaodan.cn

[T02] Kotlin：变量
来源：http://dkz.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kel.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://ktp.dashuyun.cn

"值: $b"
来源：http://cyy.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://azw.yuanzhike.top

val n: String? = null;  n?.length
来源：http://sos.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://ktq.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://puf.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://rfy.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pvr.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://srq.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jan.zycfv.cn

[T08] Kotlin：数据类
来源：http://jfn.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ztt.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://gww.hammf.cn

fun String.exclaim() = this + "!"
来源：http://yjf.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://ltz.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nwg.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://ksw.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://hry.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://jem.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://blp.yonumen.top

[T13] Kotlin：只读 Map
来源：http://rsr.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://yfo.sweek.top

[T14] Kotlin：循环
来源：http://hle.yongpay.top

for (i in 1..10) println(i)
来源：http://xfv.andypj.xyz

[T15] Kotlin：接口
来源：http://fpw.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://gei.pycfn.com

[T16] Swift：Hello World
来源：http://jiv.tarul.cn

print("Hello")
来源：http://lfz.hfpthk.cn


<!-- 参考信息 -->