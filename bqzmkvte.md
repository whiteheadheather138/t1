代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://ntl.yuanzhike.top

[R14] C 风格 for
来源：http://oie.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uha.fktsv.cn

[R15] while 逐行读文件
来源：http://mku.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://snu.smart0.xyz

[R16] until 等待条件
来源：http://qub.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dxa.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://zje.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://opq.sxryk.cn

[R18] 遍历数组
来源：http://ysj.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vau.bjfxy.top

[R19] 数组长度
来源：http://vhu.andypj.xyz

echo "${#arr[@]}"
来源：http://qtu.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://aqy.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://epu.fanxiaobao.xyz

[R21] 字符串长度
来源：http://tzs.chenlongwang.top

echo "${#s}"
来源：http://qlh.zhongyouzk.top

[R22] 截取子串
来源：http://nie.feifeiyinyue.top

echo "${s:0:5}"
来源：http://aid.havefunace.top

[R23] 字符串替换
来源：http://nya.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pkt.mhx1999.top

[R24] 大小写转换
来源：http://tha.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://ojg.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://kuy.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jud.birdmap.top

[R26] 命令替换
来源：http://hwh.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://ttp.zhengqikj.top

[R27] 算术展开
来源：http://tup.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://eny.cucudq.cn

[R28] 浮点运算
来源：http://lxc.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://kku.zhixingplan.top

[R29] 定义函数
来源：http://bis.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wbb.jyoumei.cn

[R30] 函数返回状态码
来源：http://aut.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://vlt.zdqjudy.top

[R31] 局部变量
来源：http://yhy.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://jfe.zdbjq.cn

[R32] 参数个数校验
来源：http://okh.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dec.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://tsd.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dxc.cucudq.cn

[R34] 退出时清理
来源：http://zty.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://yvv.hesvh.cn

[R35] 后台执行并等待
来源：http://saz.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vfq.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://thz.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nim.redwolf501.top

[R37] 把输出赋给变量
来源：http://wso.fzhhl.top

files=$(ls -1)
来源：http://yyb.vqdsnc.cn

[R38] 管道串联
来源：http://fmi.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://pjp.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://kgy.hfpthk.cn

cmd > out.log 2>&1
来源：http://egi.dashuyun.cn

[R40] 追加写日志
来源：http://zpp.chenlongwang.top

echo "log" >> out.log
来源：http://pot.hesvh.cn

[R41] 丢弃输出
来源：http://mty.cashguo.top

cmd >/dev/null 2>&1
来源：http://rtl.xuanzx.com

[R42] 输入重定向
来源：http://cum.haohaochexian.top

wc -l < a.txt
来源：http://dlc.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://dfg.hcnkem.com

find . -name "*.log" -type f
来源：http://icp.hammf.cn

[R44] 按修改时间查找
来源：http://jcf.xziqi.cn

find . -mtime -7 -type f
来源：http://das.hongshengwenyu.top

[R45] 批量删除
来源：http://yfw.xinyue.icu

find . -name "*.tmp" -delete
来源：http://utu.ivvv.top

[R46] 递归替换文件内容
来源：http://azc.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tgv.hesvh.cn

[R47] sed 单行替换
来源：http://jbo.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://bdu.jqgfzy.top

[R48] awk 取指定列
来源：http://hrd.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://kdj.xylfe.cn

[R49] awk 带条件
来源：http://fzl.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jzm.haohaochexian.top

[R50] awk 求和
来源：http://ing.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://lzo.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://kzp.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://utu.zdqjudy.top

[R52] 统计行数
来源：http://qiz.yonumen.top

wc -l a.txt
来源：http://zcv.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://wno.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajx.sjlbkw.cn

[R54] 比较两个文件
来源：http://vmh.tianlin.xyz

diff a.txt b.txt
来源：http://jzu.sweek.top

[R55] 压缩与解压
来源：http://hkh.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cro.andypj.xyz

[R56] 远程拷贝
来源：http://isi.9152youxi.cn

scp file user@host:/path/
来源：http://mgb.fzhhl.top

[R57] 远程执行命令
来源：http://ifq.nanxinkj.top

ssh user@host 'uptime'
来源：http://gie.cucudq.cn

[R58] 下载文件
来源：http://vxz.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://itr.ivvv.top

[R59] 发 POST JSON
来源：http://dwj.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fpa.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://jgd.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zho.cashguo.top

[R61] 磁盘占用
来源：http://yke.daxiang520.top

df -h;  du -sh *
来源：http://xuf.vehdjk.com

[R62] 找最占空间的文件
来源：http://qlb.cheryme.top

du -ah . | sort -rh | head -10
来源：http://xle.vqdsnc.cn

[R63] 内存与进程
来源：http://toq.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://dse.svipenyu.cn

[R64] 结束进程
来源：http://jke.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://ilo.zhijiandao.cn

[R65] 查看端口占用
来源：http://wpc.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gub.ehwqpu.com

[R66] 定时任务
来源：http://ulb.zycfv.cn

crontab -e;  crontab -l
来源：http://sle.bjfxy.top

[R67] 生成随机十六进制串
来源：http://ofq.hnxiangtu.top

openssl rand -hex 16
来源：http://ofb.fktsv.cn

[R68] 计算文件校验值
来源：http://lsi.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wjv.sysykeji.top

[R69] 生成随机密码
来源：http://eti.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://jrr.tanke756.top

[R70] 时间戳与互转
来源：http://mrs.mhx1999.top

date +%s;  date -d @1700000000
来源：http://frb.zycfv.cn

[R71] 日期格式化
来源：http://wtv.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dhq.zhoulong.xyz

[R72] 等待端口就绪
来源：http://xut.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qym.yonumen.top

[R73] 分割大日志
来源：http://sqn.yuanzhike.top

split -l 1000 big.log part_
来源：http://nrf.jqgfzy.top

[R74] 批量重命名
来源：http://qow.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nzl.chenjidiqi.icu

[R75] 导出环境变量
来源：http://ylc.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://xul.meibo888.top

[R76] 使用临时文件
来源：http://ugt.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eqm.xuanzx.com

[R77] 读取用户输入
来源：http://uee.smart0.xyz

read -rp "请输入: " ans
来源：http://sgf.gogol.net.cn

[R78] 交互式菜单
来源：http://ypn.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cbc.guowangkeji.top

[R79] 解析命令行选项
来源：http://haj.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hgd.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://ekb.9152youxi.cn

time ./run.sh
来源：http://csg.yangfankeji.com

================================================================================
来源：http://pal.yuxming.cn

S. C / C++ 专题
来源：http://klt.birdmap.top

================================================================================
来源：http://adu.hongshengwenyu.top

[S01] C：Hello World
来源：http://mwg.feifeiyinyue.top

#include <stdio.h>
来源：http://ihg.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lix.pycfn.com

[S02] C：变量与格式化输出
来源：http://ilp.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://gyn.pengpengdd.cyou

[S03] C：读入整数
来源：http://dfr.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://ucy.shuidangran.top

[S04] C：字符串复制
来源：http://apo.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hmv.hywenlv.cn

[S05] C：字符串长度
来源：http://arq.gaohongyu789.top

strlen(s)
来源：http://mrk.jinqigfzy.top

[S06] C：字符串比较
来源：http://ngd.hcnkem.com

strcmp(a, b) == 0
来源：http://ghk.nanxinkj.top

[S07] C：数组遍历求和
来源：http://jwp.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ugg.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://cjk.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://icl.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://fns.zdbjq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wew.yj202588.top

[S10] C：指针与解引用
来源：http://sty.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ard.hnqzz.top

[S11] C：逐行读文件
来源：http://uxg.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://dnt.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jdg.chenzaomai.com

fclose(f);
来源：http://zry.52xcode.cn

[S12] C：写文件
来源：http://irm.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jxn.tian-w.cn

[S13] C：宏定义
来源：http://cep.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bfh.52xcode.cn

[S14] C：枚举
来源：http://lir.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://cdm.bjfxy.top

[S15] C：类型转换
来源：http://fhe.hcnkem.com

(double) a / b
来源：http://llp.ivvv.top

[S16] C：位操作置位
来源：http://fnv.ivvv.top

x |= (1 << 3);
来源：http://krl.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://jwh.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lie.cqqwz.cn

[S18] C：命令行参数
来源：http://svc.havefunace.top

int main(int argc, char **argv)
来源：http://grw.fktsv.cn

[S19] C：快速排序
来源：http://pcp.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dmt.ehwqpu.com

[S20] C：二分查找
来源：http://hyq.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zxc.iojbl.cn

[S21] C：字符类别判断
来源：http://vuq.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oyu.aibaodan.cn

[S22] C：字符串转数字
来源：http://tra.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://fzl.xuetiantiany.cn

[S23] C：随机数
来源：http://mjn.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ysn.bjfxy.top

[S24] C：获取本地时间
来源：http://udj.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nki.redwolf501.top

[S25] C：内存拷贝
来源：http://oup.gzhubu.top

memcpy(dst, src, n);
来源：http://azo.aizwys.cn

[S26] C：内存清零
来源：http://hkq.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://txv.meibo888.top

[S27] C：定义常量
来源：http://jyt.hongshengwenyu.top

const double PI = 3.14159;
来源：http://mmz.redwolf501.top

[S28] C：静态变量
来源：http://tgz.sysykeji.top

static int counter = 0;
来源：http://egk.zhoulong.xyz

[S29] C：变参函数
来源：http://sqt.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mpw.hongshengwenyu.top

[S30] C：头文件保护
来源：http://fex.ppjwa.cn

#ifndef X_H
来源：http://bgi.mhx1999.top

#define X_H
来源：http://qac.jinqigufen.top

#endif
来源：http://nqg.sweek.top

[S31] C++：Hello World
来源：http://sjo.gotoacloud.top

#include <iostream>
来源：http://cna.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zur.yangfankeji.com

[S32] C++：字符串
来源：http://zmo.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://zgz.epnwcf.com

[S33] C++：vector 增删
来源：http://cas.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aso.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://yxw.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://avp.aibaodan.cn

[S35] C++：map
来源：http://hbd.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qhv.gaohongyu789.top

[S36] C++：unordered_map
来源：http://nzr.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tab.jinyuanbaomall.cn

[S37] C++：set
来源：http://kgn.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pdq.jyoumei.cn

[S38] C++：排序
来源：http://uls.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://pvc.tarul.cn

[S39] C++：自定义比较器排序
来源：http://lbc.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iwc.guannengcc.top

[S40] C++：查找元素
来源：http://pwl.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://csj.xuanzx.com

[S41] C++：类与构造函数
来源：http://uqy.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qns.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://odn.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://vvx.cdnleiting.top

[S43] C++：智能指针
来源：http://buv.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://wtv.jinqigfzy.top

[S44] C++：引用传参
来源：http://huo.mhx1999.top

void inc(int &x) { ++x; }
来源：http://lgq.bjfxy.top

[S45] C++：lambda
来源：http://xnf.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://xvk.yangfankeji.com

[S46] C++：函数模板
来源：http://wkk.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vxs.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://qfy.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgn.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://vys.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://uxl.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://tyt.nwbrower.top

[S49] C++：写文件
来源：http://xat.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ulb.cqqwz.cn

[S50] C++：格式化数字
来源：http://nai.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ycu.c1oappe.top

[S51] C++：显式类型转换
来源：http://sdm.gzhubu.top

static_cast<double>(a) / b
来源：http://tcq.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://vyt.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://uhx.cdnleiting.top

[S53] C++：移动语义
来源：http://woh.sweek.top

std::vector<int> w = std::move(v);
来源：http://gct.birdmap.top

[S54] C++：异常处理
来源：http://dot.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://chu.zycfv.cn

[S55] C++：结构化绑定
来源：http://ccq.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kec.hongshengwenyu.top

[S56] C++：optional
来源：http://zxp.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://phs.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://mit.chenzaomai.com

constexpr int N = 10;
来源：http://tco.hnqzz.top

[S58] C++：命名空间
来源：http://rte.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://qwx.gogol.net.cn

[S59] C++：静态断言
来源：http://mir.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oft.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://snv.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lai.epnwcf.com

================================================================================
来源：http://fot.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hkd.zhixingplan.top

================================================================================
来源：http://vky.bbcook.cn

[T01] Kotlin：Hello World
来源：http://jer.cqqwz.cn

println("Hello")
来源：http://ihk.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://emr.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ptg.uphjek.com

[T03] Kotlin：字符串模板
来源：http://zvh.cucudq.cn

"值: $b"
来源：http://sjc.zhengqikj.top

[T04] Kotlin：空安全
来源：http://ign.hywenlv.cn

val n: String? = null;  n?.length
来源：http://wsz.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://ghy.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jrt.fehbvm.com

[T06] Kotlin：集合映射
来源：http://rte.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zqy.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://ytn.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pte.sxryk.cn

[T08] Kotlin：数据类
来源：http://tvt.uphjek.com

data class User(val name: String, val age: Int)
来源：http://apw.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://rfh.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://fzv.xziqi.cn

[T10] Kotlin：默认参数
来源：http://zay.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mmb.jqgfzy.top

[T11] Kotlin：协程
来源：http://hdf.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wag.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://ble.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://kht.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://zwb.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://qtp.jyoumei.cn

[T14] Kotlin：循环
来源：http://qbc.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://bdf.zhixingplan.top

[T15] Kotlin：接口
来源：http://gnv.nwbrower.top

interface Shape { fun area(): Double }
来源：http://igr.316326.xyz

[T16] Swift：Hello World
来源：http://uvc.sysykeji.top

print("Hello")
来源：http://rha.yangfankeji.com


<!-- 参考信息 -->