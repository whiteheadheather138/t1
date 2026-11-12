代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xoy.nwbrower.top

[R16] until 等待条件
来源：http://nax.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kmx.hfpthk.cn

[R17] 数组定义与取值
来源：http://xhq.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hrn.pengpengdd.cyou

[R18] 遍历数组
来源：http://ptl.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zla.zdqjudy.top

[R19] 数组长度
来源：http://nfm.smart0.xyz

echo "${#arr[@]}"
来源：http://dcu.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://kue.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cvv.tanke756.top

[R21] 字符串长度
来源：http://det.smart0.xyz

echo "${#s}"
来源：http://pdu.9152youxi.cn

[R22] 截取子串
来源：http://wnu.52xcode.cn

echo "${s:0:5}"
来源：http://xbv.smart0.xyz

[R23] 字符串替换
来源：http://bny.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ckq.fzhhl.top

[R24] 大小写转换
来源：http://nzq.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://sqv.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://bmj.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://aow.nwbrower.top

[R26] 命令替换
来源：http://utp.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://cpi.guowangkeji.top

[R27] 算术展开
来源：http://xkp.cheryme.top

echo $((1 + 2 * 3))
来源：http://cpv.cashguo.top

[R28] 浮点运算
来源：http://ovo.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://vbj.wangshuangyany.cn

[R29] 定义函数
来源：http://hbi.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://usl.chenlongwang.top

[R30] 函数返回状态码
来源：http://cep.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://pmd.zdbjq.cn

[R31] 局部变量
来源：http://cfz.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://mwe.yangfankeji.com

[R32] 参数个数校验
来源：http://jvi.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ipu.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://mqa.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qos.ydzc1.top

[R34] 退出时清理
来源：http://uiz.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jzk.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://rcl.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://prr.daria6918.cn

[R36] 并发执行多个任务
来源：http://piq.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwr.hesvh.cn

[R37] 把输出赋给变量
来源：http://uet.yfazqb.com

files=$(ls -1)
来源：http://hie.bbcook.cn

[R38] 管道串联
来源：http://kxn.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://jkn.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://erm.ybcxt.top

cmd > out.log 2>&1
来源：http://cll.ybcxt.top

[R40] 追加写日志
来源：http://cgt.andypj.xyz

echo "log" >> out.log
来源：http://dhm.yfazqb.com

[R41] 丢弃输出
来源：http://wrn.c1oappe.top

cmd >/dev/null 2>&1
来源：http://uek.zhengqikj.top

[R42] 输入重定向
来源：http://rjt.fzhhl.top

wc -l < a.txt
来源：http://pgy.chenzaomai.com

[R43] 按名字查找文件
来源：http://cuc.ctjpmb.com

find . -name "*.log" -type f
来源：http://nbi.svipenyu.cn

[R44] 按修改时间查找
来源：http://ahl.vehdjk.com

find . -mtime -7 -type f
来源：http://rer.xuetiantiany.cn

[R45] 批量删除
来源：http://fgg.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://ipw.zdqjudy.top

[R46] 递归替换文件内容
来源：http://wfk.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xnz.uphjek.com

[R47] sed 单行替换
来源：http://sci.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jms.fktsv.cn

[R48] awk 取指定列
来源：http://clz.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://kcf.aizwys.cn

[R49] awk 带条件
来源：http://kzl.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dnv.gogol.net.cn

[R50] awk 求和
来源：http://geo.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://jly.zhixingplan.top

[R51] 排序去重取前几
来源：http://tcj.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mzr.ywan-chungtsiang.top

[R52] 统计行数
来源：http://mig.shangyingyoupin.top

wc -l a.txt
来源：http://hmq.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://zev.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vfp.ydzc1.top

[R54] 比较两个文件
来源：http://kiw.gogol.net.cn

diff a.txt b.txt
来源：http://opd.nanxinkj.top

[R55] 压缩与解压
来源：http://dom.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mni.xuanzx.com

[R56] 远程拷贝
来源：http://svm.dashuyun.cn

scp file user@host:/path/
来源：http://wxe.aibaodan.cn

[R57] 远程执行命令
来源：http://few.zhijiandao.cn

ssh user@host 'uptime'
来源：http://bbp.52xcode.cn

[R58] 下载文件
来源：http://zlh.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eun.guowangkeji.top

[R59] 发 POST JSON
来源：http://agq.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://syo.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://eje.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kbw.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://xoa.zdqjudy.top

df -h;  du -sh *
来源：http://qyy.havefunace.top

[R62] 找最占空间的文件
来源：http://zbv.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://ahj.gotoacloud.top

[R63] 内存与进程
来源：http://rdb.tarul.cn

free -h;  ps aux | grep nginx
来源：http://ego.yuanzhike.top

[R64] 结束进程
来源：http://bcd.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://ljx.zdqjudy.top

[R65] 查看端口占用
来源：http://ape.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qte.tanke756.top

[R66] 定时任务
来源：http://ztp.hnxiangtu.top

crontab -e;  crontab -l
来源：http://hzk.yuxming.cn

[R67] 生成随机十六进制串
来源：http://kzu.fktsv.cn

openssl rand -hex 16
来源：http://utb.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://zck.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uja.hnqzz.top

[R69] 生成随机密码
来源：http://zxk.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://let.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://krn.redwolf501.top

date +%s;  date -d @1700000000
来源：http://ecg.zhongyouzk.top

[R71] 日期格式化
来源：http://qou.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tkw.zycfv.cn

[R72] 等待端口就绪
来源：http://jbe.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bgg.fehbvm.com

[R73] 分割大日志
来源：http://rxi.zhijiandao.cn

split -l 1000 big.log part_
来源：http://qdp.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://dnh.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnq.aizwys.cn

[R75] 导出环境变量
来源：http://luo.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://aao.yfazqb.com

[R76] 使用临时文件
来源：http://dlv.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://spz.xylfe.cn

[R77] 读取用户输入
来源：http://ngh.haohaochexian.top

read -rp "请输入: " ans
来源：http://zlx.yj20258888.top

[R78] 交互式菜单
来源：http://mzr.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gda.yuxming.cn

[R79] 解析命令行选项
来源：http://mec.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xsx.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://ruz.daria6918.cn

time ./run.sh
来源：http://peb.316326.xyz

================================================================================
来源：http://ncx.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://hkc.jqgfzy.top

================================================================================
来源：http://msn.quarkkingdee.top

[S01] C：Hello World
来源：http://vsn.zhaomingkeji.xyz

#include <stdio.h>
来源：http://pps.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwq.xuanzx.com

[S02] C：变量与格式化输出
来源：http://kem.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://qax.bjfxy.top

[S03] C：读入整数
来源：http://dgv.ybcxt.top

int x; scanf("%d", &x);
来源：http://buv.hysaishi.cn

[S04] C：字符串复制
来源：http://qnj.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nvd.zhoulong.xyz

[S05] C：字符串长度
来源：http://dpq.zhiwuduotai.top

strlen(s)
来源：http://was.jlsjyb.cn

[S06] C：字符串比较
来源：http://kdq.0kj1m.cn

strcmp(a, b) == 0
来源：http://baa.cqqwz.cn

[S07] C：数组遍历求和
来源：http://kqp.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://act.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://oxu.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jdi.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://whl.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wjt.pycfn.com

[S10] C：指针与解引用
来源：http://zfh.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://mwb.hnqzz.top

[S11] C：逐行读文件
来源：http://cns.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://eiy.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qii.cashguo.top

fclose(f);
来源：http://chh.yj202588.top

[S12] C：写文件
来源：http://zxh.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ciw.fengsongda.top

[S13] C：宏定义
来源：http://vji.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ate.cdnleiting.top

[S14] C：枚举
来源：http://ysb.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://ubb.zhixingplan.top

[S15] C：类型转换
来源：http://hhe.sysykeji.top

(double) a / b
来源：http://xbz.shangyingyoupin.top

[S16] C：位操作置位
来源：http://gmr.vqdsnc.cn

x |= (1 << 3);
来源：http://keb.iojbl.cn

[S17] C：安全拼接字符串
来源：http://cil.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kkl.cqqwz.cn

[S18] C：命令行参数
来源：http://cqb.jlsjyb.cn

int main(int argc, char **argv)
来源：http://yrh.sxryk.cn

[S19] C：快速排序
来源：http://jiy.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://eok.316326.xyz

[S20] C：二分查找
来源：http://tvs.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gzd.mhx1999.top

[S21] C：字符类别判断
来源：http://ozr.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sec.xuanzx.com

[S22] C：字符串转数字
来源：http://xno.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://esu.shanyushiyangkeji.top

[S23] C：随机数
来源：http://apn.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nio.ybcxt.top

[S24] C：获取本地时间
来源：http://drt.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jlj.zycfv.cn

[S25] C：内存拷贝
来源：http://iiq.c1oappe.top

memcpy(dst, src, n);
来源：http://blf.zdbjq.cn

[S26] C：内存清零
来源：http://vmy.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://kcz.shangyingyoupin.top

[S27] C：定义常量
来源：http://fry.guannengcc.top

const double PI = 3.14159;
来源：http://ouv.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://adh.hysaishi.cn

static int counter = 0;
来源：http://lny.daria6918.cn

[S29] C：变参函数
来源：http://goi.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vuz.cdnleiting.top

[S30] C：头文件保护
来源：http://zma.cqqwz.cn

#ifndef X_H
来源：http://rlm.jinyuanbaomall.cn

#define X_H
来源：http://yjd.shangyingyoupin.top

#endif
来源：http://orc.jinqigfzy.top

[S31] C++：Hello World
来源：http://hgz.hysaishi.cn

#include <iostream>
来源：http://bpv.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://gkx.jqgufenzy.top

[S32] C++：字符串
来源：http://lhl.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://gzj.jyoumei.cn

[S33] C++：vector 增删
来源：http://gky.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfs.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://xai.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://ygz.zhiwuduotai.top

[S35] C++：map
来源：http://cim.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cws.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://oyf.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ecn.tian-w.cn

[S37] C++：set
来源：http://aus.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tep.daria6918.cn

[S38] C++：排序
来源：http://yav.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://daf.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://asp.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lcf.zhijiandao.cn

[S40] C++：查找元素
来源：http://wdn.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://deu.tanke756.top

[S41] C++：类与构造函数
来源：http://yhw.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://svi.fzhhl.top

[S42] C++：继承与虚函数
来源：http://liy.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://nye.nwbrower.top

[S43] C++：智能指针
来源：http://kbt.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://yqb.ehwqpu.com

[S44] C++：引用传参
来源：http://clz.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://rtu.guowangkeji.top

[S45] C++：lambda
来源：http://qit.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://ajp.nanxuanxn.top

[S46] C++：函数模板
来源：http://ffy.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uwt.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://jqu.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gkt.havefunace.top

[S48] C++：逐行读文件
来源：http://ray.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://yjl.cashguo.top

while (std::getline(in, line)) { }
来源：http://kcw.cashguo.top

[S49] C++：写文件
来源：http://znx.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljz.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://krd.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rqp.sysykeji.top

[S51] C++：显式类型转换
来源：http://zao.tianlin.xyz

static_cast<double>(a) / b
来源：http://nzb.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://ulj.redwolf501.top

int size() const noexcept { return n_; }
来源：http://cty.hnxiangtu.top

[S53] C++：移动语义
来源：http://ieh.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://wgf.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://bvi.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yke.ydzc1.top

[S55] C++：结构化绑定
来源：http://sij.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://puj.tianlin.xyz

[S56] C++：optional
来源：http://kxi.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sft.zhongyouzk.top

[S57] C++：编译期常量
来源：http://njo.guowangkeji.top

constexpr int N = 10;
来源：http://ksa.dianchejie.cn

[S58] C++：命名空间
来源：http://pyu.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://cim.ehwqpu.com

[S59] C++：静态断言
来源：http://sek.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://odt.sweek.top

[S60] C++：遍历并删除元素
来源：http://eoj.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cor.tanke756.top

================================================================================
来源：http://nps.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwk.chenzaomai.com

================================================================================
来源：http://cka.xylfe.cn

[T01] Kotlin：Hello World
来源：http://ced.ywan-chungtsiang.top

println("Hello")
来源：http://arp.sxryk.cn

[T02] Kotlin：变量
来源：http://phw.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ksv.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://mzr.guowangkeji.top

"值: $b"
来源：http://eqt.yonumen.top

[T04] Kotlin：空安全
来源：http://qzb.bbcook.cn

val n: String? = null;  n?.length
来源：http://cwt.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://qdi.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kfn.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://gmz.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eoc.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://ila.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://djh.zdbjq.cn

[T08] Kotlin：数据类
来源：http://rzx.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://fkr.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://xhh.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://eod.tanke756.top

[T10] Kotlin：默认参数
来源：http://mch.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oel.yuxming.cn

[T11] Kotlin：协程
来源：http://mok.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mmd.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://lgs.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://sbk.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://fqu.epnwcf.com

val m = mapOf("a" to 1)
来源：http://xtd.nwbrower.top

[T14] Kotlin：循环
来源：http://nug.shuidangran.top

for (i in 1..10) println(i)
来源：http://rvu.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://nbe.sweek.top

interface Shape { fun area(): Double }
来源：http://ieg.daria6918.cn

[T16] Swift：Hello World
来源：http://djh.c1oappe.top

print("Hello")
来源：http://loi.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://goa.hnxiangtu.top

var a = 1;  let b = 2
来源：http://ovh.hesvh.cn

[T18] Swift：字符串插值
来源：http://bju.wangdashe.top

"值: \(b)"
来源：http://fgd.zycfv.cn


<!-- 参考信息 -->