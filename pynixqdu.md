代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://way.haohaochexian.top

[R24] 大小写转换
来源：http://qsf.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uia.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://hom.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tsq.fanxiaobao.xyz

[R26] 命令替换
来源：http://pup.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://ojw.epnwcf.com

[R27] 算术展开
来源：http://bqd.havefunace.top

echo $((1 + 2 * 3))
来源：http://fei.zdqjudy.top

[R28] 浮点运算
来源：http://elo.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://laa.dianchejie.cn

[R29] 定义函数
来源：http://ctc.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tud.zdqjudy.top

[R30] 函数返回状态码
来源：http://bvw.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://blp.zdqjudy.top

[R31] 局部变量
来源：http://vtr.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://zgn.sxryk.cn

[R32] 参数个数校验
来源：http://ubn.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jph.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://cry.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uqi.redwolf501.top

[R34] 退出时清理
来源：http://gbm.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://kxz.yuxming.cn

[R35] 后台执行并等待
来源：http://qrs.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nhm.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://qoo.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ecw.daria6918.cn

[R37] 把输出赋给变量
来源：http://yqa.cucudq.cn

files=$(ls -1)
来源：http://ndl.shangyingyoupin.top

[R38] 管道串联
来源：http://xjx.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://hep.uphjek.com

[R39] 重定向标准输出与错误
来源：http://wuf.nanxuanxn.top

cmd > out.log 2>&1
来源：http://wqq.yj202588.top

[R40] 追加写日志
来源：http://hry.yvedp.cn

echo "log" >> out.log
来源：http://hhz.birdmap.top

[R41] 丢弃输出
来源：http://ewk.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://kol.ivvv.top

[R42] 输入重定向
来源：http://aes.gaohongyu789.top

wc -l < a.txt
来源：http://zmv.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://eqa.sweek.top

find . -name "*.log" -type f
来源：http://bkn.dianchejie.cn

[R44] 按修改时间查找
来源：http://jkb.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://imx.ivvv.top

[R45] 批量删除
来源：http://ntl.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://bwm.iojbl.cn

[R46] 递归替换文件内容
来源：http://otn.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jmr.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://thk.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://bbs.cashguo.top

[R48] awk 取指定列
来源：http://lgj.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://hhv.hfpthk.cn

[R49] awk 带条件
来源：http://xkj.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rlw.meibo888.top

[R50] awk 求和
来源：http://ngp.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xcv.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://nff.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yht.tianlin.xyz

[R52] 统计行数
来源：http://mav.jinqigfzy.top

wc -l a.txt
来源：http://lkj.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://nny.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ovd.havefunace.top

[R54] 比较两个文件
来源：http://gci.bjfxy.top

diff a.txt b.txt
来源：http://xyo.cqqwz.cn

[R55] 压缩与解压
来源：http://oia.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sjo.ybcxt.top

[R56] 远程拷贝
来源：http://dhy.vehdjk.com

scp file user@host:/path/
来源：http://owf.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://wco.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://wcs.ybcxt.top

[R58] 下载文件
来源：http://hwe.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lpx.shuidangran.top

[R59] 发 POST JSON
来源：http://wam.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hqc.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://ahf.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fvd.chenjidiqi.icu

[R61] 磁盘占用
来源：http://dcm.0kj1m.cn

df -h;  du -sh *
来源：http://dqr.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://xqj.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://cuq.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://kvq.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://wes.0kj1m.cn

[R64] 结束进程
来源：http://unf.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://dqn.tanke756.top

[R65] 查看端口占用
来源：http://ypk.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qvf.ydjk.org.cn

[R66] 定时任务
来源：http://cbi.havefunace.top

crontab -e;  crontab -l
来源：http://flh.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://acu.zhixingplan.top

openssl rand -hex 16
来源：http://gch.xziqi.cn

[R68] 计算文件校验值
来源：http://sic.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ygf.ppjwa.cn

[R69] 生成随机密码
来源：http://bnx.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://ejx.quarkkingdee.top

[R70] 时间戳与互转
来源：http://gwp.sysykeji.top

date +%s;  date -d @1700000000
来源：http://lhl.pycfn.com

[R71] 日期格式化
来源：http://huh.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wne.shzxlz.cn

[R72] 等待端口就绪
来源：http://pcq.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://knd.yvedp.cn

[R73] 分割大日志
来源：http://vhm.snrcjt.cn

split -l 1000 big.log part_
来源：http://qej.yuanzhike.top

[R74] 批量重命名
来源：http://rki.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ogu.c1oappe.top

[R75] 导出环境变量
来源：http://moq.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://rid.zdbjq.cn

[R76] 使用临时文件
来源：http://wjh.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tka.zhiwuduotai.top

[R77] 读取用户输入
来源：http://hbx.hfpthk.cn

read -rp "请输入: " ans
来源：http://ekr.kuanghao11.cn

[R78] 交互式菜单
来源：http://dde.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://upc.fehbvm.com

[R79] 解析命令行选项
来源：http://uji.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tar.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://syb.gotoacloud.top

time ./run.sh
来源：http://fbs.hysaishi.cn

================================================================================
来源：http://hlg.yangfankeji.com

S. C / C++ 专题
来源：http://bjr.vqdsnc.cn

================================================================================
来源：http://ohg.zhoulong.xyz

[S01] C：Hello World
来源：http://lmj.cdnleiting.top

#include <stdio.h>
来源：http://evv.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dsc.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://dgv.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://aht.hammf.cn

[S03] C：读入整数
来源：http://blp.yuanzhike.top

int x; scanf("%d", &x);
来源：http://eyo.sjlbkw.cn

[S04] C：字符串复制
来源：http://qtr.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://xvj.shuidangran.top

[S05] C：字符串长度
来源：http://bkd.jqgfzy.top

strlen(s)
来源：http://pva.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://kpc.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://cgu.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://nru.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rhc.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://vnw.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qil.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://jzv.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xyd.birdmap.top

[S10] C：指针与解引用
来源：http://bti.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://gws.cqqwz.cn

[S11] C：逐行读文件
来源：http://zmy.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://mfx.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://fcz.jianghu66.top

fclose(f);
来源：http://lug.ywan-chungtsiang.top

[S12] C：写文件
来源：http://qar.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bif.xylfe.cn

[S13] C：宏定义
来源：http://jqm.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nbk.wangshuangyany.cn

[S14] C：枚举
来源：http://htn.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://mgk.pycfn.com

[S15] C：类型转换
来源：http://cjf.redwolf501.top

(double) a / b
来源：http://jpq.gogol.net.cn

[S16] C：位操作置位
来源：http://rbc.yfazqb.com

x |= (1 << 3);
来源：http://ueh.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://fuf.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://shp.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://sep.9152youxi.cn

int main(int argc, char **argv)
来源：http://rey.tarul.cn

[S19] C：快速排序
来源：http://cco.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://pbk.mhx1999.top

[S20] C：二分查找
来源：http://dfo.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cje.tanke756.top

[S21] C：字符类别判断
来源：http://qgw.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pnq.ctjpmb.com

[S22] C：字符串转数字
来源：http://frg.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://csg.nanxuanxn.top

[S23] C：随机数
来源：http://apm.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ypw.ivvv.top

[S24] C：获取本地时间
来源：http://bta.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zrn.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://bsz.c1oappe.top

memcpy(dst, src, n);
来源：http://ykz.yj20258888.top

[S26] C：内存清零
来源：http://rej.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://hjx.c1oappe.top

[S27] C：定义常量
来源：http://ckh.zhoulong.xyz

const double PI = 3.14159;
来源：http://jys.ppjwa.cn

[S28] C：静态变量
来源：http://wes.wangdashe.top

static int counter = 0;
来源：http://csx.jqgufenzy.top

[S29] C：变参函数
来源：http://lpd.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://erx.fzhhl.top

[S30] C：头文件保护
来源：http://mop.yongpay.top

#ifndef X_H
来源：http://sly.smart0.xyz

#define X_H
来源：http://hpl.birdmap.top

#endif
来源：http://qbf.tarul.cn

[S31] C++：Hello World
来源：http://owa.fengsongda.top

#include <iostream>
来源：http://nky.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://vjb.cucudq.cn

[S32] C++：字符串
来源：http://xxp.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://btz.yj202588.top

[S33] C++：vector 增删
来源：http://qap.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jyp.xylfe.cn

[S34] C++：遍历 vector
来源：http://cex.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://fxh.sxryk.cn

[S35] C++：map
来源：http://vws.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fye.hcnkem.com

[S36] C++：unordered_map
来源：http://nah.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iil.birdmap.top

[S37] C++：set
来源：http://grz.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cih.shzxlz.cn

[S38] C++：排序
来源：http://tkh.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://hzm.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://tez.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uwo.zycfv.cn

[S40] C++：查找元素
来源：http://pjr.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ndz.yj20258.top

[S41] C++：类与构造函数
来源：http://wiy.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yzd.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://faq.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://uhz.yueranfly.top

[S43] C++：智能指针
来源：http://tbq.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://cnp.zycfv.cn

[S44] C++：引用传参
来源：http://ils.ivvv.top

void inc(int &x) { ++x; }
来源：http://dxj.ctjpmb.com

[S45] C++：lambda
来源：http://zed.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ixr.cashguo.top

[S46] C++：函数模板
来源：http://bej.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jvi.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://pkh.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tom.jinqigufen.top

[S48] C++：逐行读文件
来源：http://kbw.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://aoa.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://plt.aizwys.cn

[S49] C++：写文件
来源：http://izd.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zhd.dashuyun.cn

[S50] C++：格式化数字
来源：http://qay.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xpo.snrcjt.cn

[S51] C++：显式类型转换
来源：http://bkr.ydzc1.top

static_cast<double>(a) / b
来源：http://def.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://wlu.xylfe.cn

int size() const noexcept { return n_; }
来源：http://tgn.daxiang520.top

[S53] C++：移动语义
来源：http://ubc.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://tdc.ehwqpu.com

[S54] C++：异常处理
来源：http://jzw.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://erb.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://cfj.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pnm.jqgufenzy.top

[S56] C++：optional
来源：http://mly.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://axs.jinqigfzy.top

[S57] C++：编译期常量
来源：http://xli.yvedp.cn

constexpr int N = 10;
来源：http://jol.yanxiufei.cn

[S58] C++：命名空间
来源：http://wle.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://iye.ybcxt.top

[S59] C++：静态断言
来源：http://mun.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kdu.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://ywc.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yjd.zhaomingkeji.xyz

================================================================================
来源：http://clg.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxp.xinyue.icu

================================================================================
来源：http://lht.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://hpb.hysaishi.cn

println("Hello")
来源：http://fam.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://ehr.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gwx.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://axr.yongpay.top

"值: $b"
来源：http://zuc.yj202588.top

[T04] Kotlin：空安全
来源：http://raf.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://wwy.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://ahf.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fwg.meibo888.top

[T06] Kotlin：集合映射
来源：http://eit.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mri.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://qbx.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://awu.nanxinkj.top

[T08] Kotlin：数据类
来源：http://fhq.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://ddb.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://vmm.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://suh.guannengcc.top

[T10] Kotlin：默认参数
来源：http://hfd.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uxs.vehdjk.com

[T11] Kotlin：协程
来源：http://zao.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://trx.gzhubu.top

[T12] Kotlin：解构声明
来源：http://nwx.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://gwu.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://aoe.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://sbm.jqgufenzy.top

[T14] Kotlin：循环
来源：http://gzw.fehbvm.com

for (i in 1..10) println(i)
来源：http://lxs.jinqigfzy.top

[T15] Kotlin：接口
来源：http://dmw.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://alg.0kj1m.cn

[T16] Swift：Hello World
来源：http://imo.xziqi.cn

print("Hello")
来源：http://zsx.hysaishi.cn

[T17] Swift：变量与常量
来源：http://hgm.fehbvm.com

var a = 1;  let b = 2
来源：http://ycn.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://fhw.gotoacloud.top

"值: \(b)"
来源：http://nka.tanke756.top

[T19] Swift：可选绑定
来源：http://pwk.zhoulong.xyz

if let n = opt { print(n) }
来源：http://hgc.hywenlv.cn

[T20] Swift：数组操作
来源：http://ttx.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://txv.haohaochexian.top

[T21] Swift：遍历
来源：http://tha.sweek.top

for x in a { print(x) }
来源：http://qng.jiagoushi.top

[T22] Swift：字典
来源：http://dhc.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pjf.jianghu66.top

[T23] Swift：函数
来源：http://oow.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hwk.hammf.cn

[T24] Swift：闭包
来源：http://vzj.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfp.xuetiantiany.cn

[T25] Swift：结构体
来源：http://jfp.hammf.cn

struct P { var x: Int }
来源：http://bea.hysaishi.cn

[T26] Swift：类与重写
来源：http://ycz.hysaishi.cn

class A: Base { override func f() {} }
来源：http://nnj.nanxuanxn.top


<!-- 参考信息 -->