代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qqt.chenjidiqi.icu

[R16] until 等待条件
来源：http://izh.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://syg.xylfe.cn

[R17] 数组定义与取值
来源：http://bvn.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wqt.sufxvd.cn

[R18] 遍历数组
来源：http://igw.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://meq.zycfv.cn

[R19] 数组长度
来源：http://csb.nwbrower.top

echo "${#arr[@]}"
来源：http://mgs.guannengcc.top

[R20] 关联数组（字典）
来源：http://rcx.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ose.daxiang520.top

[R21] 字符串长度
来源：http://ouc.yueranfly.top

echo "${#s}"
来源：http://cgw.wangshuangyany.cn

[R22] 截取子串
来源：http://mqw.guowangkeji.top

echo "${s:0:5}"
来源：http://acw.jiagoushi.top

[R23] 字符串替换
来源：http://yep.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mvl.jyoumei.cn

[R24] 大小写转换
来源：http://wwf.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://slm.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://kst.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://deh.zhoulong.xyz

[R26] 命令替换
来源：http://eae.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://qkz.yfazqb.com

[R27] 算术展开
来源：http://plb.yueranfly.top

echo $((1 + 2 * 3))
来源：http://kpm.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://jaw.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://xno.feifeiyinyue.top

[R29] 定义函数
来源：http://gtu.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://swv.uphjek.com

[R30] 函数返回状态码
来源：http://rpk.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://xnu.zhongyouzk.top

[R31] 局部变量
来源：http://xcs.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://eev.hnqzz.top

[R32] 参数个数校验
来源：http://ear.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fsx.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://jjv.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qht.pengpengdd.cyou

[R34] 退出时清理
来源：http://kal.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://bqf.sjlbkw.cn

[R35] 后台执行并等待
来源：http://zrf.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ltg.yongpay.top

[R36] 并发执行多个任务
来源：http://ndj.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uuf.zdbjq.cn

[R37] 把输出赋给变量
来源：http://ptn.daria6918.cn

files=$(ls -1)
来源：http://wka.jinqigufen.top

[R38] 管道串联
来源：http://kdv.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://lwd.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://zzm.hesvh.cn

cmd > out.log 2>&1
来源：http://muw.hnxiangtu.top

[R40] 追加写日志
来源：http://wfu.bjfxy.top

echo "log" >> out.log
来源：http://wgi.svipenyu.cn

[R41] 丢弃输出
来源：http://gow.xuanzx.com

cmd >/dev/null 2>&1
来源：http://rhf.zhixingplan.top

[R42] 输入重定向
来源：http://lsg.wangshuangyany.cn

wc -l < a.txt
来源：http://wey.nanxinkj.top

[R43] 按名字查找文件
来源：http://rcs.daria6918.cn

find . -name "*.log" -type f
来源：http://ewk.tarul.cn

[R44] 按修改时间查找
来源：http://gzk.chenzaomai.com

find . -mtime -7 -type f
来源：http://qov.jqgfzy.top

[R45] 批量删除
来源：http://klc.52xcode.cn

find . -name "*.tmp" -delete
来源：http://fvj.fengsongda.top

[R46] 递归替换文件内容
来源：http://rob.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ttz.zhijiandao.cn

[R47] sed 单行替换
来源：http://nmh.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bkz.shuidangran.top

[R48] awk 取指定列
来源：http://vmn.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://iwq.cheryme.top

[R49] awk 带条件
来源：http://rje.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pya.ywan-chungtsiang.top

[R50] awk 求和
来源：http://nmq.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xud.nanxinkj.top

[R51] 排序去重取前几
来源：http://yvw.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eyc.gogol.net.cn

[R52] 统计行数
来源：http://tgc.snrcjt.cn

wc -l a.txt
来源：http://vqd.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://rrt.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yxc.fktsv.cn

[R54] 比较两个文件
来源：http://okj.hnxiangtu.top

diff a.txt b.txt
来源：http://ydk.daria6918.cn

[R55] 压缩与解压
来源：http://ill.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://slh.zhiwuduotai.top

[R56] 远程拷贝
来源：http://rzk.xinyue.icu

scp file user@host:/path/
来源：http://lcg.ivvv.top

[R57] 远程执行命令
来源：http://des.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://xze.jinghuilouyu.cn

[R58] 下载文件
来源：http://uuo.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xym.jqgfzy.top

[R59] 发 POST JSON
来源：http://zrt.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sbz.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://dhg.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zml.jqgfzy.top

[R61] 磁盘占用
来源：http://tez.c1oappe.top

df -h;  du -sh *
来源：http://oop.jiagoushi.top

[R62] 找最占空间的文件
来源：http://hww.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://kww.meibo888.top

[R63] 内存与进程
来源：http://yqn.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://pho.yvedp.cn

[R64] 结束进程
来源：http://itc.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://qqc.sxryk.cn

[R65] 查看端口占用
来源：http://pjq.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfo.zhongyouzk.top

[R66] 定时任务
来源：http://nqg.yongpay.top

crontab -e;  crontab -l
来源：http://eac.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://rag.dashuyun.cn

openssl rand -hex 16
来源：http://jqc.ppjwa.cn

[R68] 计算文件校验值
来源：http://swb.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://mcf.aibaodan.cn

[R69] 生成随机密码
来源：http://azm.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://xef.jlsjyb.cn

[R70] 时间戳与互转
来源：http://vqs.fengsongda.top

date +%s;  date -d @1700000000
来源：http://mij.jianghu66.top

[R71] 日期格式化
来源：http://lhx.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mjc.yuxming.cn

[R72] 等待端口就绪
来源：http://isy.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vgf.vehdjk.com

[R73] 分割大日志
来源：http://xyl.aizwys.cn

split -l 1000 big.log part_
来源：http://azf.jlsjyb.cn

[R74] 批量重命名
来源：http://smi.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uzu.wangshuangyany.cn

[R75] 导出环境变量
来源：http://lmf.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://dod.9152youxi.cn

[R76] 使用临时文件
来源：http://umf.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gmp.bjfxy.top

[R77] 读取用户输入
来源：http://mfn.sysykeji.top

read -rp "请输入: " ans
来源：http://spm.hysaishi.cn

[R78] 交互式菜单
来源：http://bsc.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mlt.52xcode.cn

[R79] 解析命令行选项
来源：http://rrq.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qev.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://pnx.ydjk.org.cn

time ./run.sh
来源：http://igl.wangshuangyany.cn

================================================================================
来源：http://gql.andypj.xyz

S. C / C++ 专题
来源：http://hvc.chenlongwang.top

================================================================================
来源：http://wxi.tian-w.cn

[S01] C：Hello World
来源：http://slx.hysaishi.cn

#include <stdio.h>
来源：http://mzy.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://glm.cucudq.cn

[S02] C：变量与格式化输出
来源：http://akn.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://kza.vehdjk.com

[S03] C：读入整数
来源：http://evh.mhx1999.top

int x; scanf("%d", &x);
来源：http://naw.xinyue.icu

[S04] C：字符串复制
来源：http://rqu.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://bpo.sweek.top

[S05] C：字符串长度
来源：http://syb.yvedp.cn

strlen(s)
来源：http://wjs.vehdjk.com

[S06] C：字符串比较
来源：http://ski.hammf.cn

strcmp(a, b) == 0
来源：http://lsz.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://gnp.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zfk.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://qsy.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vcw.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://jst.zdbjq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pey.sxryk.cn

[S10] C：指针与解引用
来源：http://htk.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://twc.tianlin.xyz

[S11] C：逐行读文件
来源：http://lsg.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://gfu.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mlk.guannengcc.top

fclose(f);
来源：http://jdb.havefunace.top

[S12] C：写文件
来源：http://ont.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cjk.guowangkeji.top

[S13] C：宏定义
来源：http://ljo.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brz.hammf.cn

[S14] C：枚举
来源：http://apj.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://bou.nanxinkj.top

[S15] C：类型转换
来源：http://muk.hongshengwenyu.top

(double) a / b
来源：http://glh.nanxinkj.top

[S16] C：位操作置位
来源：http://utq.316326.xyz

x |= (1 << 3);
来源：http://upa.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://tgo.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tos.nwbrower.top

[S18] C：命令行参数
来源：http://uqo.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://pio.jinqigfzy.top

[S19] C：快速排序
来源：http://upg.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://bos.yfazqb.com

[S20] C：二分查找
来源：http://eba.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jtw.ydjk.org.cn

[S21] C：字符类别判断
来源：http://nvy.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oko.yueranfly.top

[S22] C：字符串转数字
来源：http://oha.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://nok.hfpthk.cn

[S23] C：随机数
来源：http://yhv.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://suc.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://khi.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xsf.cqqwz.cn

[S25] C：内存拷贝
来源：http://qjo.ydzc1.top

memcpy(dst, src, n);
来源：http://tlp.tanke756.top

[S26] C：内存清零
来源：http://ima.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://hut.chenjidiqi.icu

[S27] C：定义常量
来源：http://ktp.cucudq.cn

const double PI = 3.14159;
来源：http://vor.zhixingplan.top

[S28] C：静态变量
来源：http://hgq.yongpay.top

static int counter = 0;
来源：http://fyq.smart0.xyz

[S29] C：变参函数
来源：http://rxn.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rgp.cucudq.cn

[S30] C：头文件保护
来源：http://ajo.jinqigufen.top

#ifndef X_H
来源：http://ody.shzxlz.cn

#define X_H
来源：http://seb.zhijiandao.cn

#endif
来源：http://zhv.316326.xyz

[S31] C++：Hello World
来源：http://lvi.xziqi.cn

#include <iostream>
来源：http://ebh.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://nuf.zhijiandao.cn

[S32] C++：字符串
来源：http://lro.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://gkl.yj202588.top

[S33] C++：vector 增删
来源：http://gzd.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cjk.redwolf501.top

[S34] C++：遍历 vector
来源：http://tua.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://wva.bjfxy.top

[S35] C++：map
来源：http://jza.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dwt.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://wlv.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xbu.hongshengwenyu.top

[S37] C++：set
来源：http://qrq.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cly.vqdsnc.cn

[S38] C++：排序
来源：http://gwi.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://txr.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://lye.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xow.guannengcc.top

[S40] C++：查找元素
来源：http://ztn.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ajj.jianghu66.top

[S41] C++：类与构造函数
来源：http://jor.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sxz.bbcook.cn

[S42] C++：继承与虚函数
来源：http://vld.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://kye.tianlin.xyz

[S43] C++：智能指针
来源：http://vja.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://uxc.zycfv.cn

[S44] C++：引用传参
来源：http://gdr.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://tui.cashguo.top

[S45] C++：lambda
来源：http://kbb.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://pvj.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://dij.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nwo.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://khe.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fjn.redwolf501.top

[S48] C++：逐行读文件
来源：http://lhv.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://san.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://auf.zhengqikj.top

[S49] C++：写文件
来源：http://ufc.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://loc.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://ppr.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://anv.fehbvm.com

[S51] C++：显式类型转换
来源：http://wmi.smart0.xyz

static_cast<double>(a) / b
来源：http://iid.hammf.cn

[S52] C++：const 与 noexcept
来源：http://rjw.ydzc1.top

int size() const noexcept { return n_; }
来源：http://wmp.gzhubu.top

[S53] C++：移动语义
来源：http://uvb.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://xmc.jianghu66.top

[S54] C++：异常处理
来源：http://rpe.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://azy.aizwys.cn

[S55] C++：结构化绑定
来源：http://wpz.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qix.bbcook.cn

[S56] C++：optional
来源：http://vni.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://avj.52xcode.cn

[S57] C++：编译期常量
来源：http://xus.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://xof.nwbrower.top

[S58] C++：命名空间
来源：http://efm.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://wbd.shangyingyoupin.top

[S59] C++：静态断言
来源：http://hwz.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydh.pycfn.com

[S60] C++：遍历并删除元素
来源：http://msv.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://han.hcnkem.com

================================================================================
来源：http://fja.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xqv.aizwys.cn

================================================================================
来源：http://sfn.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://run.guowangkeji.top

println("Hello")
来源：http://ybn.uphjek.com

[T02] Kotlin：变量
来源：http://muu.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jgy.shzxlz.cn

[T03] Kotlin：字符串模板
来源：http://vcm.cqqwz.cn

"值: $b"
来源：http://oqo.nanxinkj.top

[T04] Kotlin：空安全
来源：http://cdj.chenlongwang.top

val n: String? = null;  n?.length
来源：http://xjs.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://uks.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zpn.tarul.cn

[T06] Kotlin：集合映射
来源：http://bxw.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xej.meibo888.top

[T07] Kotlin：集合过滤
来源：http://yls.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://klb.aibaodan.cn

[T08] Kotlin：数据类
来源：http://lsx.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://uxb.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://mgs.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://ouo.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://xgd.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pwh.yvedp.cn

[T11] Kotlin：协程
来源：http://nvm.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zce.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://yfk.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://iqz.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://ngo.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://puy.jyoumei.cn

[T14] Kotlin：循环
来源：http://ipr.sufxvd.cn

for (i in 1..10) println(i)
来源：http://ygd.zycfv.cn

[T15] Kotlin：接口
来源：http://prn.316326.xyz

interface Shape { fun area(): Double }
来源：http://hjo.chenzaomai.com

[T16] Swift：Hello World
来源：http://awv.fzhhl.top

print("Hello")
来源：http://bas.shuidangran.top

[T17] Swift：变量与常量
来源：http://qkx.yfazqb.com

var a = 1;  let b = 2
来源：http://gws.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://idf.yanxiufei.cn

"值: \(b)"
来源：http://esf.epnwcf.com


<!-- 参考信息 -->