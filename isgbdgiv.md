代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mta.zhengqikj.top

[R16] until 等待条件
来源：http://wdx.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jih.pycfn.com

[R17] 数组定义与取值
来源：http://dge.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fck.yanxiufei.cn

[R18] 遍历数组
来源：http://jzh.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hgh.nwbrower.top

[R19] 数组长度
来源：http://fxr.uphjek.com

echo "${#arr[@]}"
来源：http://lvk.hcnkem.com

[R20] 关联数组（字典）
来源：http://qbe.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jzh.birdmap.top

[R21] 字符串长度
来源：http://ous.quarkkingdee.top

echo "${#s}"
来源：http://akj.ppjwa.cn

[R22] 截取子串
来源：http://wsl.jinqigfzy.top

echo "${s:0:5}"
来源：http://urw.meibo888.top

[R23] 字符串替换
来源：http://wcd.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dud.gogol.net.cn

[R24] 大小写转换
来源：http://ybx.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ffw.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://sro.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gwg.hysaishi.cn

[R26] 命令替换
来源：http://xit.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://auc.316326.xyz

[R27] 算术展开
来源：http://ktz.hcnkem.com

echo $((1 + 2 * 3))
来源：http://syd.ctjpmb.com

[R28] 浮点运算
来源：http://niy.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://yxp.iojbl.cn

[R29] 定义函数
来源：http://wmy.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uft.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://tex.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://kbt.ctjpmb.com

[R31] 局部变量
来源：http://oym.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://qzv.yfazqb.com

[R32] 参数个数校验
来源：http://ixw.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rwx.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://rwh.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kwv.yvedp.cn

[R34] 退出时清理
来源：http://ujd.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://hhj.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://xtp.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ork.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://nnk.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ywk.redwolf501.top

[R37] 把输出赋给变量
来源：http://wcz.xinyue.icu

files=$(ls -1)
来源：http://ula.chenzaomai.com

[R38] 管道串联
来源：http://feo.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://kgf.cheryme.top

[R39] 重定向标准输出与错误
来源：http://hlv.vqdsnc.cn

cmd > out.log 2>&1
来源：http://fys.jinqigufen.top

[R40] 追加写日志
来源：http://yfz.fehbvm.com

echo "log" >> out.log
来源：http://tdk.zhongyouzk.top

[R41] 丢弃输出
来源：http://jbo.tarul.cn

cmd >/dev/null 2>&1
来源：http://yzp.9152youxi.cn

[R42] 输入重定向
来源：http://pik.nwbrower.top

wc -l < a.txt
来源：http://ylq.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://itd.c1oappe.top

find . -name "*.log" -type f
来源：http://lwt.tarul.cn

[R44] 按修改时间查找
来源：http://zsg.sxryk.cn

find . -mtime -7 -type f
来源：http://yiw.yvedp.cn

[R45] 批量删除
来源：http://rne.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://gon.fktsv.cn

[R46] 递归替换文件内容
来源：http://tpg.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://phu.haohaochexian.top

[R47] sed 单行替换
来源：http://hmy.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://ugj.yj202588.top

[R48] awk 取指定列
来源：http://hqt.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://icc.feifeiyinyue.top

[R49] awk 带条件
来源：http://ilz.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zng.gotoacloud.top

[R50] awk 求和
来源：http://mwa.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://did.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://zmi.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jsn.sxryk.cn

[R52] 统计行数
来源：http://kxm.cqqwz.cn

wc -l a.txt
来源：http://xfj.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://jty.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wqj.tarul.cn

[R54] 比较两个文件
来源：http://esm.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://uww.wangshuangyany.cn

[R55] 压缩与解压
来源：http://dqa.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulm.hesvh.cn

[R56] 远程拷贝
来源：http://caz.ctjpmb.com

scp file user@host:/path/
来源：http://ovc.daria6918.cn

[R57] 远程执行命令
来源：http://edf.svipenyu.cn

ssh user@host 'uptime'
来源：http://pjw.fanxiaobao.xyz

[R58] 下载文件
来源：http://jpi.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rlz.zdqjudy.top

[R59] 发 POST JSON
来源：http://dsa.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qdc.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://mtm.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pat.0kj1m.cn

[R61] 磁盘占用
来源：http://cnf.tanke756.top

df -h;  du -sh *
来源：http://swf.epnwcf.com

[R62] 找最占空间的文件
来源：http://eea.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://xhq.hammf.cn

[R63] 内存与进程
来源：http://glb.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://wsf.9152youxi.cn

[R64] 结束进程
来源：http://cge.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://nse.xuetiantiany.cn

[R65] 查看端口占用
来源：http://dlw.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fwc.ehwqpu.com

[R66] 定时任务
来源：http://zzl.c1oappe.top

crontab -e;  crontab -l
来源：http://wha.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://ukr.nanxuanxn.top

openssl rand -hex 16
来源：http://oys.vqdsnc.cn

[R68] 计算文件校验值
来源：http://rog.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://oyu.jqgufenzy.top

[R69] 生成随机密码
来源：http://uao.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://eir.bbcook.cn

[R70] 时间戳与互转
来源：http://iqw.daria6918.cn

date +%s;  date -d @1700000000
来源：http://wsq.gaohongyu789.top

[R71] 日期格式化
来源：http://nbl.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://urd.bbcook.cn

[R72] 等待端口就绪
来源：http://awu.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uzt.9152youxi.cn

[R73] 分割大日志
来源：http://xqa.gotoacloud.top

split -l 1000 big.log part_
来源：http://gtg.jinghuilouyu.cn

[R74] 批量重命名
来源：http://uzd.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kln.pengpengdd.cyou

[R75] 导出环境变量
来源：http://sjy.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://tey.nwbrower.top

[R76] 使用临时文件
来源：http://szt.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dfy.bbcook.cn

[R77] 读取用户输入
来源：http://sek.uphjek.com

read -rp "请输入: " ans
来源：http://ogd.hfpthk.cn

[R78] 交互式菜单
来源：http://fmq.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ylc.kuanghao11.cn

[R79] 解析命令行选项
来源：http://tjo.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lqm.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://qrq.fktsv.cn

time ./run.sh
来源：http://yox.xziqi.cn

================================================================================
来源：http://fug.yanxiufei.cn

S. C / C++ 专题
来源：http://vwu.gotoacloud.top

================================================================================
来源：http://brs.zhiwuduotai.top

[S01] C：Hello World
来源：http://kuv.svipenyu.cn

#include <stdio.h>
来源：http://aiq.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vig.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://rmu.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://dpi.daria6918.cn

[S03] C：读入整数
来源：http://zei.yvedp.cn

int x; scanf("%d", &x);
来源：http://jjv.wangshuangyany.cn

[S04] C：字符串复制
来源：http://deu.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://xyv.316326.xyz

[S05] C：字符串长度
来源：http://pwl.shuidangran.top

strlen(s)
来源：http://ukq.jiagoushi.top

[S06] C：字符串比较
来源：http://upj.ehwqpu.com

strcmp(a, b) == 0
来源：http://cbs.ehwqpu.com

[S07] C：数组遍历求和
来源：http://sjl.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sjp.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://wnp.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kav.shuidangran.top

[S09] C：结构体定义与初始化
来源：http://bua.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utw.nwbrower.top

[S10] C：指针与解引用
来源：http://xxw.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://xvc.fzhhl.top

[S11] C：逐行读文件
来源：http://wgx.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://qwf.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://akk.yuxming.cn

fclose(f);
来源：http://ldi.ppjwa.cn

[S12] C：写文件
来源：http://qpr.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ddn.yuanzhike.top

[S13] C：宏定义
来源：http://xzf.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ayv.hcnkem.com

[S14] C：枚举
来源：http://hcf.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://xss.fehbvm.com

[S15] C：类型转换
来源：http://bat.jianghu66.top

(double) a / b
来源：http://cng.hammf.cn

[S16] C：位操作置位
来源：http://jqs.yuxming.cn

x |= (1 << 3);
来源：http://nqo.shuidangran.top

[S17] C：安全拼接字符串
来源：http://hbk.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hwc.snrcjt.cn

[S18] C：命令行参数
来源：http://lqo.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://mqu.chenjidiqi.icu

[S19] C：快速排序
来源：http://sam.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://nfe.zhoulong.xyz

[S20] C：二分查找
来源：http://wtv.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jwd.yanxiufei.cn

[S21] C：字符类别判断
来源：http://hxg.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://udd.vehdjk.com

[S22] C：字符串转数字
来源：http://zet.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://yss.shangyingyoupin.top

[S23] C：随机数
来源：http://fap.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ixm.kuanghao11.cn

[S24] C：获取本地时间
来源：http://rxf.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ifv.tanke756.top

[S25] C：内存拷贝
来源：http://blu.sysykeji.top

memcpy(dst, src, n);
来源：http://dzj.ctjpmb.com

[S26] C：内存清零
来源：http://wzy.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://iwc.jyoumei.cn

[S27] C：定义常量
来源：http://jou.jinqigufen.top

const double PI = 3.14159;
来源：http://ylg.chenlongwang.top

[S28] C：静态变量
来源：http://qoh.nanxinkj.top

static int counter = 0;
来源：http://ovw.ehwqpu.com

[S29] C：变参函数
来源：http://cpd.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vjg.ivvv.top

[S30] C：头文件保护
来源：http://mjg.epnwcf.com

#ifndef X_H
来源：http://otw.daria6918.cn

#define X_H
来源：http://kpe.andypj.xyz

#endif
来源：http://izu.yj20258888.top

[S31] C++：Hello World
来源：http://byo.xinyue.icu

#include <iostream>
来源：http://aux.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://axb.yangfankeji.com

[S32] C++：字符串
来源：http://aga.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://mzb.hnqzz.top

[S33] C++：vector 增删
来源：http://zpb.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfs.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://exz.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://tkx.xuetiantiany.cn

[S35] C++：map
来源：http://igr.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ibc.snrcjt.cn

[S36] C++：unordered_map
来源：http://qmx.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ehk.fengsongda.top

[S37] C++：set
来源：http://yan.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bal.hywenlv.cn

[S38] C++：排序
来源：http://zpl.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://jcx.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://hby.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nay.epnwcf.com

[S40] C++：查找元素
来源：http://izt.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yao.redwolf501.top

[S41] C++：类与构造函数
来源：http://ucl.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tmm.guannengcc.top

[S42] C++：继承与虚函数
来源：http://zxj.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://rmb.hywenlv.cn

[S43] C++：智能指针
来源：http://yxv.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://osn.zhixingplan.top

[S44] C++：引用传参
来源：http://two.wangdashe.top

void inc(int &x) { ++x; }
来源：http://enk.sxryk.cn

[S45] C++：lambda
来源：http://hiv.zycfv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ccb.fehbvm.com

[S46] C++：函数模板
来源：http://wur.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qmv.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://pdu.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://owh.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://tkc.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dmd.yj20258888.top

while (std::getline(in, line)) { }
来源：http://nyb.zhixingplan.top

[S49] C++：写文件
来源：http://tdy.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ydj.smart0.xyz

[S50] C++：格式化数字
来源：http://fmc.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vkx.yonumen.top

[S51] C++：显式类型转换
来源：http://drh.hfpthk.cn

static_cast<double>(a) / b
来源：http://ktd.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://dmc.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://esq.cheryme.top

[S53] C++：移动语义
来源：http://lku.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://cuk.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://nrz.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hem.cqqwz.cn

[S55] C++：结构化绑定
来源：http://crt.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tzx.dianchejie.cn

[S56] C++：optional
来源：http://cxc.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ijx.svipenyu.cn

[S57] C++：编译期常量
来源：http://njp.yj202588.top

constexpr int N = 10;
来源：http://idk.cdnleiting.top

[S58] C++：命名空间
来源：http://oow.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://kcx.yvedp.cn

[S59] C++：静态断言
来源：http://zjs.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://knt.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://tep.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ysc.vqdsnc.cn

================================================================================
来源：http://wji.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://git.9152youxi.cn

================================================================================
来源：http://vni.daxiang520.top

[T01] Kotlin：Hello World
来源：http://fxp.aizwys.cn

println("Hello")
来源：http://zfp.chenlongwang.top

[T02] Kotlin：变量
来源：http://lmv.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxs.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://nvd.yvedp.cn

"值: $b"
来源：http://obv.ivvv.top

[T04] Kotlin：空安全
来源：http://lry.svipenyu.cn

val n: String? = null;  n?.length
来源：http://vlq.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://act.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gyn.smart0.xyz

[T06] Kotlin：集合映射
来源：http://dqp.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nbi.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://mwh.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://rcv.ivvv.top

[T08] Kotlin：数据类
来源：http://ngs.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://lrw.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://rer.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://xec.ybcxt.top

[T10] Kotlin：默认参数
来源：http://mvp.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bre.hfpthk.cn

[T11] Kotlin：协程
来源：http://hbi.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ugr.iojbl.cn

[T12] Kotlin：解构声明
来源：http://yiq.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://sgt.birdmap.top

[T13] Kotlin：只读 Map
来源：http://gmx.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://gev.gogol.net.cn

[T14] Kotlin：循环
来源：http://bsf.snrcjt.cn

for (i in 1..10) println(i)
来源：http://lhi.sxryk.cn

[T15] Kotlin：接口
来源：http://dfl.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://qnb.zhijiandao.cn

[T16] Swift：Hello World
来源：http://xob.yuanzhike.top

print("Hello")
来源：http://sei.316326.xyz

[T17] Swift：变量与常量
来源：http://yyw.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://hoi.0kj1m.cn

[T18] Swift：字符串插值
来源：http://poj.bjfxy.top

"值: \(b)"
来源：http://aul.hywenlv.cn


<!-- 参考信息 -->