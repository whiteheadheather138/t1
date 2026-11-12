代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tuw.ctjpmb.com

[R16] until 等待条件
来源：http://lvy.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fcu.yfazqb.com

[R17] 数组定义与取值
来源：http://ypo.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://sgq.ehwqpu.com

[R18] 遍历数组
来源：http://zwl.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kov.guowangkeji.top

[R19] 数组长度
来源：http://dld.zycfv.cn

echo "${#arr[@]}"
来源：http://olu.shzxlz.cn

[R20] 关联数组（字典）
来源：http://ofr.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ivc.haohaochexian.top

[R21] 字符串长度
来源：http://thx.fanxiaobao.xyz

echo "${#s}"
来源：http://pfx.9152youxi.cn

[R22] 截取子串
来源：http://jxb.svipenyu.cn

echo "${s:0:5}"
来源：http://hcu.hfpthk.cn

[R23] 字符串替换
来源：http://nyl.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hli.fanxiaobao.xyz

[R24] 大小写转换
来源：http://lhs.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://glj.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://wmt.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sqq.zycfv.cn

[R26] 命令替换
来源：http://iec.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://dnr.havefunace.top

[R27] 算术展开
来源：http://pmc.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://cbt.ybcxt.top

[R28] 浮点运算
来源：http://lak.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://lyi.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://tuc.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nvw.yuxming.cn

[R30] 函数返回状态码
来源：http://dwi.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://ijx.tanke756.top

[R31] 局部变量
来源：http://mqe.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://pbl.hysaishi.cn

[R32] 参数个数校验
来源：http://emv.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://snp.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://oto.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cbx.ydjk.org.cn

[R34] 退出时清理
来源：http://wdm.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://akc.52xcode.cn

[R35] 后台执行并等待
来源：http://weo.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xif.fengsongda.top

[R36] 并发执行多个任务
来源：http://jai.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tij.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://bdz.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://frd.shuidangran.top

[R38] 管道串联
来源：http://wsl.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://yxj.tanke756.top

[R39] 重定向标准输出与错误
来源：http://mdw.yuanzhike.top

cmd > out.log 2>&1
来源：http://hxf.dashuyun.cn

[R40] 追加写日志
来源：http://adf.zycfv.cn

echo "log" >> out.log
来源：http://ako.smart0.xyz

[R41] 丢弃输出
来源：http://xer.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://avg.wangshuangyany.cn

[R42] 输入重定向
来源：http://ixp.epnwcf.com

wc -l < a.txt
来源：http://mhs.xuanzx.com

[R43] 按名字查找文件
来源：http://eis.zdqjudy.top

find . -name "*.log" -type f
来源：http://ghj.yongpay.top

[R44] 按修改时间查找
来源：http://fwi.zdbjq.cn

find . -mtime -7 -type f
来源：http://egm.tianlin.xyz

[R45] 批量删除
来源：http://gdh.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://bnp.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://vsx.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rgq.daxiang520.top

[R47] sed 单行替换
来源：http://udd.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://gmu.aibaodan.cn

[R48] awk 取指定列
来源：http://gim.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://gnu.nwbrower.top

[R49] awk 带条件
来源：http://iio.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kku.cheryme.top

[R50] awk 求和
来源：http://ocw.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://bdu.gaohongyu789.top

[R51] 排序去重取前几
来源：http://lam.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dig.zhijiandao.cn

[R52] 统计行数
来源：http://omn.gotoacloud.top

wc -l a.txt
来源：http://qrc.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://hcq.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://roo.fzhhl.top

[R54] 比较两个文件
来源：http://ire.shanyushiyangtech.top

diff a.txt b.txt
来源：http://ler.wangdashe.top

[R55] 压缩与解压
来源：http://qck.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zxh.52xcode.cn

[R56] 远程拷贝
来源：http://zaj.ehwqpu.com

scp file user@host:/path/
来源：http://xgk.zhixingplan.top

[R57] 远程执行命令
来源：http://fjx.haohaochexian.top

ssh user@host 'uptime'
来源：http://djo.gogol.net.cn

[R58] 下载文件
来源：http://jor.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ngz.xylfe.cn

[R59] 发 POST JSON
来源：http://rxk.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sdt.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://czd.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hpq.daria6918.cn

[R61] 磁盘占用
来源：http://tfd.sweek.top

df -h;  du -sh *
来源：http://jkp.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://vbs.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://irt.sufxvd.cn

[R63] 内存与进程
来源：http://ogw.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://aih.snrcjt.cn

[R64] 结束进程
来源：http://gag.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://xvl.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://naq.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://typ.xinyue.icu

[R66] 定时任务
来源：http://evr.shuidangran.top

crontab -e;  crontab -l
来源：http://nxz.mhx1999.top

[R67] 生成随机十六进制串
来源：http://uko.yuxming.cn

openssl rand -hex 16
来源：http://twz.snrcjt.cn

[R68] 计算文件校验值
来源：http://lcp.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://lfm.cucudq.cn

[R69] 生成随机密码
来源：http://kaq.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://kmi.yueranfly.top

[R70] 时间戳与互转
来源：http://kxm.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://aio.vehdjk.com

[R71] 日期格式化
来源：http://irw.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://efe.yj20258888.top

[R72] 等待端口就绪
来源：http://fjr.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lmf.shanyushiyangtech.top

[R73] 分割大日志
来源：http://xxd.uphjek.com

split -l 1000 big.log part_
来源：http://vin.xziqi.cn

[R74] 批量重命名
来源：http://fjh.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kry.tianlin.xyz

[R75] 导出环境变量
来源：http://ciu.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://myc.redwolf501.top

[R76] 使用临时文件
来源：http://wkx.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jiu.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://prj.mhx1999.top

read -rp "请输入: " ans
来源：http://stx.hongshengwenyu.top

[R78] 交互式菜单
来源：http://bes.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uqk.vqdsnc.cn

[R79] 解析命令行选项
来源：http://oza.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kne.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://efv.andypj.xyz

time ./run.sh
来源：http://lie.ywan-chungtsiang.top

================================================================================
来源：http://neh.yongpay.top

S. C / C++ 专题
来源：http://hsh.chenlongwang.top

================================================================================
来源：http://lsn.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://elk.xylfe.cn

#include <stdio.h>
来源：http://eus.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://srx.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://jws.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://mkb.52xcode.cn

[S03] C：读入整数
来源：http://avp.52xcode.cn

int x; scanf("%d", &x);
来源：http://jfy.redwolf501.top

[S04] C：字符串复制
来源：http://zda.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wop.sxryk.cn

[S05] C：字符串长度
来源：http://cqx.bjfxy.top

strlen(s)
来源：http://lkn.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://nry.sjlbkw.cn

strcmp(a, b) == 0
来源：http://kzl.yj20258888.top

[S07] C：数组遍历求和
来源：http://wgv.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fpv.havefunace.top

[S08] C：动态内存分配与释放
来源：http://qfc.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jpy.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://slf.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lhj.daria6918.cn

[S10] C：指针与解引用
来源：http://gkr.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://kae.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://pjw.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://qea.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lux.shuidangran.top

fclose(f);
来源：http://rrg.zhongyouzk.top

[S12] C：写文件
来源：http://ars.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qce.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://ozn.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://etr.zdqjudy.top

[S14] C：枚举
来源：http://opn.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://dxb.gzhubu.top

[S15] C：类型转换
来源：http://xle.chenzaomai.com

(double) a / b
来源：http://cid.zdqjudy.top

[S16] C：位操作置位
来源：http://lyf.andypj.xyz

x |= (1 << 3);
来源：http://wdb.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://wxq.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://viq.feifeiyinyue.top

[S18] C：命令行参数
来源：http://rkr.zdbjq.cn

int main(int argc, char **argv)
来源：http://yyc.ctjpmb.com

[S19] C：快速排序
来源：http://pjb.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sqb.daxiang520.top

[S20] C：二分查找
来源：http://fly.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cwr.jyoumei.cn

[S21] C：字符类别判断
来源：http://poa.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pva.vqdsnc.cn

[S22] C：字符串转数字
来源：http://yjl.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://gyj.daxiang520.top

[S23] C：随机数
来源：http://ptp.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ler.gzhubu.top

[S24] C：获取本地时间
来源：http://gya.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gtl.hnqzz.top

[S25] C：内存拷贝
来源：http://tes.uphjek.com

memcpy(dst, src, n);
来源：http://mzx.nanxuanxn.top

[S26] C：内存清零
来源：http://ulo.shuidangran.top

memset(a, 0, sizeof a);
来源：http://lme.jinqigufen.top

[S27] C：定义常量
来源：http://rxn.pengpengdd.cyou

const double PI = 3.14159;
来源：http://sua.fanxiaobao.xyz

[S28] C：静态变量
来源：http://ezj.jqgufenzy.top

static int counter = 0;
来源：http://udb.iojbl.cn

[S29] C：变参函数
来源：http://elg.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cjl.hnqzz.top

[S30] C：头文件保护
来源：http://hor.yj202588.top

#ifndef X_H
来源：http://gvh.shangyingyoupin.top

#define X_H
来源：http://ccq.ybcxt.top

#endif
来源：http://kij.jinqigfzy.top

[S31] C++：Hello World
来源：http://ykw.yuanzhike.top

#include <iostream>
来源：http://xyn.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://bwb.gaohongyu789.top

[S32] C++：字符串
来源：http://zev.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://gyh.zhengqikj.top

[S33] C++：vector 增删
来源：http://fyh.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ywt.ybcxt.top

[S34] C++：遍历 vector
来源：http://wpg.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://bue.vqdsnc.cn

[S35] C++：map
来源：http://fcp.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vpj.daria6918.cn

[S36] C++：unordered_map
来源：http://sxt.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cye.shzxlz.cn

[S37] C++：set
来源：http://ybe.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://flt.c1oappe.top

[S38] C++：排序
来源：http://tth.sweek.top

std::sort(v.begin(), v.end());
来源：http://odc.meibo888.top

[S39] C++：自定义比较器排序
来源：http://qdu.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ezk.bjfxy.top

[S40] C++：查找元素
来源：http://hww.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yxx.chenzaomai.com

[S41] C++：类与构造函数
来源：http://zex.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://elq.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://ija.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://xcq.hywenlv.cn

[S43] C++：智能指针
来源：http://bkq.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://lry.dianchejie.cn

[S44] C++：引用传参
来源：http://qtr.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://zcm.yueranfly.top

[S45] C++：lambda
来源：http://djc.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://azt.ctjpmb.com

[S46] C++：函数模板
来源：http://gkx.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ovd.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://lvx.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zee.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://tup.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qqr.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://yxb.daxiang520.top

[S49] C++：写文件
来源：http://zjw.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ulh.shzxlz.cn

[S50] C++：格式化数字
来源：http://shg.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yai.sxryk.cn

[S51] C++：显式类型转换
来源：http://wtm.ydjk.org.cn

static_cast<double>(a) / b
来源：http://hhp.yj202588.top

[S52] C++：const 与 noexcept
来源：http://vkw.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://ayw.birdmap.top

[S53] C++：移动语义
来源：http://qok.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://qli.guannengcc.top

[S54] C++：异常处理
来源：http://jhr.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jvm.ivvv.top

[S55] C++：结构化绑定
来源：http://nqn.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tjl.quarkkingdee.top

[S56] C++：optional
来源：http://now.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bzs.ydjk.org.cn

[S57] C++：编译期常量
来源：http://coz.redwolf501.top

constexpr int N = 10;
来源：http://mdn.gotoacloud.top

[S58] C++：命名空间
来源：http://sln.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://oya.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://zde.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xnt.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://nxo.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edx.ivvv.top

================================================================================
来源：http://vpg.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://osy.shangyingyoupin.top

================================================================================
来源：http://uxm.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://ofp.zhijiandao.cn

println("Hello")
来源：http://qsx.yvedp.cn

[T02] Kotlin：变量
来源：http://ocv.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bqb.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://fao.gzhubu.top

"值: $b"
来源：http://uvf.gzhubu.top

[T04] Kotlin：空安全
来源：http://oli.hammf.cn

val n: String? = null;  n?.length
来源：http://rix.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://ycl.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hzj.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://abz.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://msy.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://goo.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zuc.jianghu66.top

[T08] Kotlin：数据类
来源：http://rmd.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://dmb.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://hxh.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://jei.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://zpm.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yhi.vehdjk.com

[T11] Kotlin：协程
来源：http://ajb.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rfa.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://vyz.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://sxq.yj202588.top

[T13] Kotlin：只读 Map
来源：http://ded.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://swn.chenlongwang.top

[T14] Kotlin：循环
来源：http://oai.mhx1999.top

for (i in 1..10) println(i)
来源：http://fzr.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://zle.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://zjt.gogol.net.cn

[T16] Swift：Hello World
来源：http://rtj.jinqigufen.top

print("Hello")
来源：http://moi.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://vos.gaohongyu789.top

var a = 1;  let b = 2
来源：http://tat.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://uye.gogol.net.cn

"值: \(b)"
来源：http://qgd.xylfe.cn


<!-- 参考信息 -->