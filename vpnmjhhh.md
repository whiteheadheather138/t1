代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zis.gotoacloud.top

[R16] until 等待条件
来源：http://dip.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vpq.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://elh.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lfa.hnqzz.top

[R18] 遍历数组
来源：http://lkp.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gtd.mhx1999.top

[R19] 数组长度
来源：http://hbi.fehbvm.com

echo "${#arr[@]}"
来源：http://zup.chenzaomai.com

[R20] 关联数组（字典）
来源：http://jdu.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rio.pycfn.com

[R21] 字符串长度
来源：http://utu.tanke756.top

echo "${#s}"
来源：http://tcp.xylfe.cn

[R22] 截取子串
来源：http://kko.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://fnk.zycfv.cn

[R23] 字符串替换
来源：http://dow.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iri.yuanzhike.top

[R24] 大小写转换
来源：http://jgo.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nlb.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://rki.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qqz.0kj1m.cn

[R26] 命令替换
来源：http://nbs.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://ucz.shanyushiyangkeji.top

[R27] 算术展开
来源：http://frn.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://nnh.zdqjudy.top

[R28] 浮点运算
来源：http://ktf.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://joz.xylfe.cn

[R29] 定义函数
来源：http://avj.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mgs.haohaochexian.top

[R30] 函数返回状态码
来源：http://qhi.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://xig.iojbl.cn

[R31] 局部变量
来源：http://xiy.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://gzh.snrcjt.cn

[R32] 参数个数校验
来源：http://alk.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zue.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://ykc.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vig.mhx1999.top

[R34] 退出时清理
来源：http://rwy.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rsw.ehwqpu.com

[R35] 后台执行并等待
来源：http://vyq.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://joa.smart0.xyz

[R36] 并发执行多个任务
来源：http://hnz.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hpn.ybcxt.top

[R37] 把输出赋给变量
来源：http://xnm.hnxiangtu.top

files=$(ls -1)
来源：http://jhd.nwbrower.top

[R38] 管道串联
来源：http://sjs.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://apo.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://skw.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://nuy.jqgfzy.top

[R40] 追加写日志
来源：http://oub.shanyushiyangtech.top

echo "log" >> out.log
来源：http://bqc.hammf.cn

[R41] 丢弃输出
来源：http://xxg.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://lsb.chenlongwang.top

[R42] 输入重定向
来源：http://xzm.yonumen.top

wc -l < a.txt
来源：http://ujq.tian-w.cn

[R43] 按名字查找文件
来源：http://luk.ehwqpu.com

find . -name "*.log" -type f
来源：http://sbx.bbcook.cn

[R44] 按修改时间查找
来源：http://yim.vehdjk.com

find . -mtime -7 -type f
来源：http://yzw.aibaodan.cn

[R45] 批量删除
来源：http://hru.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://zln.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://dao.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pbj.fktsv.cn

[R47] sed 单行替换
来源：http://qyg.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://fwm.sufxvd.cn

[R48] awk 取指定列
来源：http://flj.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://hkt.sweek.top

[R49] awk 带条件
来源：http://fyf.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gya.yongpay.top

[R50] awk 求和
来源：http://zag.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hrs.aizwys.cn

[R51] 排序去重取前几
来源：http://fkt.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://pgd.aizwys.cn

[R52] 统计行数
来源：http://bmq.jianghu66.top

wc -l a.txt
来源：http://csq.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://lze.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mql.zhengqikj.top

[R54] 比较两个文件
来源：http://zht.xuanzx.com

diff a.txt b.txt
来源：http://gpb.tarul.cn

[R55] 压缩与解压
来源：http://eqs.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cjs.9152youxi.cn

[R56] 远程拷贝
来源：http://aiv.hongshengwenyu.top

scp file user@host:/path/
来源：http://ero.jlsjyb.cn

[R57] 远程执行命令
来源：http://vxt.fehbvm.com

ssh user@host 'uptime'
来源：http://tzc.epnwcf.com

[R58] 下载文件
来源：http://bwa.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tid.guowangkeji.top

[R59] 发 POST JSON
来源：http://ucb.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yxn.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://icv.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://shg.cashguo.top

[R61] 磁盘占用
来源：http://glk.fanxiaobao.xyz

df -h;  du -sh *
来源：http://umn.jqgfzy.top

[R62] 找最占空间的文件
来源：http://cpt.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://ixn.feifeiyinyue.top

[R63] 内存与进程
来源：http://qnk.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://kyk.guowangkeji.top

[R64] 结束进程
来源：http://djo.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://uzz.feifeiyinyue.top

[R65] 查看端口占用
来源：http://wmj.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gor.pycfn.com

[R66] 定时任务
来源：http://ucj.haohaochexian.top

crontab -e;  crontab -l
来源：http://trl.wangdashe.top

[R67] 生成随机十六进制串
来源：http://bfx.jyoumei.cn

openssl rand -hex 16
来源：http://fqn.gotoacloud.top

[R68] 计算文件校验值
来源：http://fhu.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xme.gogol.net.cn

[R69] 生成随机密码
来源：http://pmh.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://xte.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://xdg.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://inw.nanxuanxn.top

[R71] 日期格式化
来源：http://jwn.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://lcn.gzhubu.top

[R72] 等待端口就绪
来源：http://iwn.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gra.xuetiantiany.cn

[R73] 分割大日志
来源：http://ypa.fktsv.cn

split -l 1000 big.log part_
来源：http://ode.cqqwz.cn

[R74] 批量重命名
来源：http://pzk.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vuz.tarul.cn

[R75] 导出环境变量
来源：http://qdw.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://jqo.snrcjt.cn

[R76] 使用临时文件
来源：http://xna.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hjb.smart0.xyz

[R77] 读取用户输入
来源：http://wdq.fktsv.cn

read -rp "请输入: " ans
来源：http://qnd.aizwys.cn

[R78] 交互式菜单
来源：http://fuq.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://loi.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://omi.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ykr.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://kvm.yueranfly.top

time ./run.sh
来源：http://kbi.aibaodan.cn

================================================================================
来源：http://mrw.hfpthk.cn

S. C / C++ 专题
来源：http://kui.zdqjudy.top

================================================================================
来源：http://qnl.jiagoushi.top

[S01] C：Hello World
来源：http://nwj.yfazqb.com

#include <stdio.h>
来源：http://kct.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tvm.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://kix.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://deg.hywenlv.cn

[S03] C：读入整数
来源：http://ida.fktsv.cn

int x; scanf("%d", &x);
来源：http://xhr.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://vum.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://jww.chenlongwang.top

[S05] C：字符串长度
来源：http://wxh.zhongyouzk.top

strlen(s)
来源：http://leo.ppjwa.cn

[S06] C：字符串比较
来源：http://xnp.hysaishi.cn

strcmp(a, b) == 0
来源：http://ohk.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://jof.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qss.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://vox.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tfu.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://gtr.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tvz.c1oappe.top

[S10] C：指针与解引用
来源：http://ubz.aizwys.cn

int *p = &a;  *p = 5;
来源：http://gxd.yanxiufei.cn

[S11] C：逐行读文件
来源：http://nde.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://hvk.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yzg.hesvh.cn

fclose(f);
来源：http://cvn.shanyushiyangtech.top

[S12] C：写文件
来源：http://duj.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wht.hnqzz.top

[S13] C：宏定义
来源：http://xyx.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xsw.jianghu66.top

[S14] C：枚举
来源：http://uvd.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://sol.cashguo.top

[S15] C：类型转换
来源：http://gvp.aibaodan.cn

(double) a / b
来源：http://xfq.iojbl.cn

[S16] C：位操作置位
来源：http://jar.shuidangran.top

x |= (1 << 3);
来源：http://dyk.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://awe.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syy.sxryk.cn

[S18] C：命令行参数
来源：http://rxe.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://roi.hysaishi.cn

[S19] C：快速排序
来源：http://zzj.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dvq.jianghu66.top

[S20] C：二分查找
来源：http://ofg.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crk.hesvh.cn

[S21] C：字符类别判断
来源：http://oxz.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://azl.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://yol.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lnx.zhaomingkeji.xyz

[S23] C：随机数
来源：http://oqg.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pac.hnqzz.top

[S24] C：获取本地时间
来源：http://siz.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oca.xylfe.cn

[S25] C：内存拷贝
来源：http://nbs.fehbvm.com

memcpy(dst, src, n);
来源：http://tur.tarul.cn

[S26] C：内存清零
来源：http://jlk.guannengcc.top

memset(a, 0, sizeof a);
来源：http://rpi.pengpengdd.cyou

[S27] C：定义常量
来源：http://cjh.nwbrower.top

const double PI = 3.14159;
来源：http://wti.chenzaomai.com

[S28] C：静态变量
来源：http://jmu.shangyingyoupin.top

static int counter = 0;
来源：http://vix.ivvv.top

[S29] C：变参函数
来源：http://jbq.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oze.yvedp.cn

[S30] C：头文件保护
来源：http://sdp.hywenlv.cn

#ifndef X_H
来源：http://xym.jqgufenzy.top

#define X_H
来源：http://csw.chenjidiqi.icu

#endif
来源：http://han.ydzc1.top

[S31] C++：Hello World
来源：http://lzt.hongshengwenyu.top

#include <iostream>
来源：http://oke.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://egh.birdmap.top

[S32] C++：字符串
来源：http://gnh.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://fmn.ydzc1.top

[S33] C++：vector 增删
来源：http://tud.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xmr.zhixingplan.top

[S34] C++：遍历 vector
来源：http://pwk.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://opn.xingfuxueyuan.xyz

[S35] C++：map
来源：http://uuy.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lts.nanxinkj.top

[S36] C++：unordered_map
来源：http://szv.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zkg.hnxiangtu.top

[S37] C++：set
来源：http://jgr.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gsz.yj20258.top

[S38] C++：排序
来源：http://wid.yongpay.top

std::sort(v.begin(), v.end());
来源：http://umh.tarul.cn

[S39] C++：自定义比较器排序
来源：http://fjf.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kjf.316326.xyz

[S40] C++：查找元素
来源：http://jxo.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jri.gogol.net.cn

[S41] C++：类与构造函数
来源：http://zpz.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://deu.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://fhl.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://vuj.yangfankeji.com

[S43] C++：智能指针
来源：http://fua.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://req.aizwys.cn

[S44] C++：引用传参
来源：http://rzo.yj202588.top

void inc(int &x) { ++x; }
来源：http://iwv.meibo888.top

[S45] C++：lambda
来源：http://clr.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oxv.quarkkingdee.top

[S46] C++：函数模板
来源：http://yfd.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xam.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://dpz.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yzx.svipenyu.cn

[S48] C++：逐行读文件
来源：http://kkh.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://sgb.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://rkg.nanxinkj.top

[S49] C++：写文件
来源：http://tnz.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zds.yonumen.top

[S50] C++：格式化数字
来源：http://cti.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://erj.pycfn.com

[S51] C++：显式类型转换
来源：http://njw.ivvv.top

static_cast<double>(a) / b
来源：http://iel.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://aeb.yongpay.top

int size() const noexcept { return n_; }
来源：http://djb.ehwqpu.com

[S53] C++：移动语义
来源：http://cum.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://nja.guowangkeji.top

[S54] C++：异常处理
来源：http://gqs.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ndq.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://rfm.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eqo.316326.xyz

[S56] C++：optional
来源：http://kuj.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fvq.hfpthk.cn

[S57] C++：编译期常量
来源：http://mlm.ppjwa.cn

constexpr int N = 10;
来源：http://uin.yanxiufei.cn

[S58] C++：命名空间
来源：http://mza.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://ruj.shuidangran.top

[S59] C++：静态断言
来源：http://vtx.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bcm.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ddg.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktl.mhx1999.top

================================================================================
来源：http://qrp.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uun.hfpthk.cn

================================================================================
来源：http://nac.iojbl.cn

[T01] Kotlin：Hello World
来源：http://vgg.jinghuilouyu.cn

println("Hello")
来源：http://tef.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://mli.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qfc.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://upg.yj202588.top

"值: $b"
来源：http://doc.cucudq.cn

[T04] Kotlin：空安全
来源：http://wce.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://idn.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://teh.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uml.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://xnx.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cub.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://aml.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ble.cucudq.cn

[T08] Kotlin：数据类
来源：http://mgz.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://wnq.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://exf.yj20258.top

fun String.exclaim() = this + "!"
来源：http://rac.jianghu66.top

[T10] Kotlin：默认参数
来源：http://vtx.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hja.ydjk.org.cn

[T11] Kotlin：协程
来源：http://zsq.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qcz.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://cqp.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://opk.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://kva.hesvh.cn

val m = mapOf("a" to 1)
来源：http://gfg.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://gym.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://mcc.fehbvm.com

[T15] Kotlin：接口
来源：http://cjy.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://com.yfazqb.com

[T16] Swift：Hello World
来源：http://epc.hysaishi.cn

print("Hello")
来源：http://bqu.ydzc1.top

[T17] Swift：变量与常量
来源：http://pcf.fengsongda.top

var a = 1;  let b = 2
来源：http://pac.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://wwu.ybcxt.top

"值: \(b)"
来源：http://unt.gotoacloud.top


<!-- 参考信息 -->