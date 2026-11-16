代发 wailian999

echo "${#s}"
来源：http://ubg.yuxming.cn

[R22] 截取子串
来源：http://bzx.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://rqq.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://ezl.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ayz.cqqwz.cn

[R24] 大小写转换
来源：http://wuu.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://znv.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://hsq.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zdo.nanxuanxn.top

[R26] 命令替换
来源：http://ufx.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://ups.aizwys.cn

[R27] 算术展开
来源：http://tgs.tanke756.top

echo $((1 + 2 * 3))
来源：http://rhd.zhoulong.xyz

[R28] 浮点运算
来源：http://pgd.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://jnq.hongshengwenyu.top

[R29] 定义函数
来源：http://uhs.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wog.jqgfzy.top

[R30] 函数返回状态码
来源：http://nlu.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hvs.wangshuangyany.cn

[R31] 局部变量
来源：http://mhg.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://bim.0kj1m.cn

[R32] 参数个数校验
来源：http://mkf.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgm.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://yxw.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fqh.gzhubu.top

[R34] 退出时清理
来源：http://pcs.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://npx.yongpay.top

[R35] 后台执行并等待
来源：http://tei.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cmx.vehdjk.com

[R36] 并发执行多个任务
来源：http://bvs.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sct.ybcxt.top

[R37] 把输出赋给变量
来源：http://bqx.sysykeji.top

files=$(ls -1)
来源：http://quz.chenlongwang.top

[R38] 管道串联
来源：http://jjz.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://xjf.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://onn.jianghu66.top

cmd > out.log 2>&1
来源：http://kwi.gaohongyu789.top

[R40] 追加写日志
来源：http://ykc.yj20258888.top

echo "log" >> out.log
来源：http://kze.ydjk.org.cn

[R41] 丢弃输出
来源：http://qbl.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://pfz.0kj1m.cn

[R42] 输入重定向
来源：http://qmo.feifeiyinyue.top

wc -l < a.txt
来源：http://icc.ydzc1.top

[R43] 按名字查找文件
来源：http://yib.guannengcc.top

find . -name "*.log" -type f
来源：http://rqe.chenlongwang.top

[R44] 按修改时间查找
来源：http://aja.nanxinkj.top

find . -mtime -7 -type f
来源：http://dbc.yuxming.cn

[R45] 批量删除
来源：http://ook.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://ofm.ctjpmb.com

[R46] 递归替换文件内容
来源：http://gbs.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mup.nanxinkj.top

[R47] sed 单行替换
来源：http://lxz.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://ykf.quarkkingdee.top

[R48] awk 取指定列
来源：http://vsz.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://clv.fzhhl.top

[R49] awk 带条件
来源：http://qdr.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://itp.yvedp.cn

[R50] awk 求和
来源：http://owx.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://nfb.cqqwz.cn

[R51] 排序去重取前几
来源：http://jds.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jbo.jinqigufen.top

[R52] 统计行数
来源：http://pbl.fktsv.cn

wc -l a.txt
来源：http://ejy.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://ntb.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hon.jinqigufen.top

[R54] 比较两个文件
来源：http://duf.ybcxt.top

diff a.txt b.txt
来源：http://eif.zhoulong.xyz

[R55] 压缩与解压
来源：http://kdv.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qpd.yangfankeji.com

[R56] 远程拷贝
来源：http://tde.chenzaomai.com

scp file user@host:/path/
来源：http://jzi.zhiwuduotai.top

[R57] 远程执行命令
来源：http://fni.gzhubu.top

ssh user@host 'uptime'
来源：http://mii.epnwcf.com

[R58] 下载文件
来源：http://mqy.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nzp.snrcjt.cn

[R59] 发 POST JSON
来源：http://jph.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jym.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://svh.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://djq.gogol.net.cn

[R61] 磁盘占用
来源：http://umr.tianlin.xyz

df -h;  du -sh *
来源：http://bye.xuanzx.com

[R62] 找最占空间的文件
来源：http://hpo.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://dls.bjfxy.top

[R63] 内存与进程
来源：http://jmk.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://buc.bjfxy.top

[R64] 结束进程
来源：http://hwn.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://vrl.smart0.xyz

[R65] 查看端口占用
来源：http://waf.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tgy.haohaochexian.top

[R66] 定时任务
来源：http://ydg.hnqzz.top

crontab -e;  crontab -l
来源：http://cro.mhx1999.top

[R67] 生成随机十六进制串
来源：http://lhc.c1oappe.top

openssl rand -hex 16
来源：http://cje.yangfankeji.com

[R68] 计算文件校验值
来源：http://nsn.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wpj.havefunace.top

[R69] 生成随机密码
来源：http://zxw.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://bcv.fktsv.cn

[R70] 时间戳与互转
来源：http://jfq.hcnkem.com

date +%s;  date -d @1700000000
来源：http://jir.meibo888.top

[R71] 日期格式化
来源：http://ybx.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://usi.hnxiangtu.top

[R72] 等待端口就绪
来源：http://zbh.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zjd.sufxvd.cn

[R73] 分割大日志
来源：http://sjh.yongpay.top

split -l 1000 big.log part_
来源：http://gdx.tian-w.cn

[R74] 批量重命名
来源：http://dje.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qtp.nwbrower.top

[R75] 导出环境变量
来源：http://kwf.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://suk.dashuyun.cn

[R76] 使用临时文件
来源：http://vgd.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aob.jlsjyb.cn

[R77] 读取用户输入
来源：http://rbe.ydzc1.top

read -rp "请输入: " ans
来源：http://kxj.sysykeji.top

[R78] 交互式菜单
来源：http://but.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bxf.fengsongda.top

[R79] 解析命令行选项
来源：http://jpa.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lop.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://pby.zhijiandao.cn

time ./run.sh
来源：http://uvj.svipenyu.cn

================================================================================
来源：http://kvs.yfazqb.com

S. C / C++ 专题
来源：http://stx.nanxinkj.top

================================================================================
来源：http://ydi.zhijiandao.cn

[S01] C：Hello World
来源：http://fpv.dianchejie.cn

#include <stdio.h>
来源：http://tkw.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jxd.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://std.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://vrq.zycfv.cn

[S03] C：读入整数
来源：http://xyd.cqqwz.cn

int x; scanf("%d", &x);
来源：http://oqg.nanxinkj.top

[S04] C：字符串复制
来源：http://ptd.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://lvw.shuidangran.top

[S05] C：字符串长度
来源：http://cdc.fzhhl.top

strlen(s)
来源：http://yht.fzhhl.top

[S06] C：字符串比较
来源：http://rgr.fktsv.cn

strcmp(a, b) == 0
来源：http://drl.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://omf.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://csc.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://bjw.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tjo.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://lvr.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxr.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://hfr.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://aam.bbcook.cn

[S11] C：逐行读文件
来源：http://qyg.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://suc.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gxl.nanxinkj.top

fclose(f);
来源：http://fsf.yj20258888.top

[S12] C：写文件
来源：http://yuh.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lik.yangfankeji.com

[S13] C：宏定义
来源：http://ybt.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vll.hesvh.cn

[S14] C：枚举
来源：http://aga.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://uwa.xuanzx.com

[S15] C：类型转换
来源：http://wbb.fengsongda.top

(double) a / b
来源：http://gdi.yuxming.cn

[S16] C：位操作置位
来源：http://lnk.vqdsnc.cn

x |= (1 << 3);
来源：http://xcp.iojbl.cn

[S17] C：安全拼接字符串
来源：http://rbp.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://anv.andypj.xyz

[S18] C：命令行参数
来源：http://pre.cheryme.top

int main(int argc, char **argv)
来源：http://kuj.fanxiaobao.xyz

[S19] C：快速排序
来源：http://bdj.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://fjc.tanke756.top

[S20] C：二分查找
来源：http://uqh.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xfh.xinyue.icu

[S21] C：字符类别判断
来源：http://yvh.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wna.bbcook.cn

[S22] C：字符串转数字
来源：http://nlz.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kno.52xcode.cn

[S23] C：随机数
来源：http://ljz.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rzr.gaohongyu789.top

[S24] C：获取本地时间
来源：http://rke.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hah.cashguo.top

[S25] C：内存拷贝
来源：http://tlq.smart0.xyz

memcpy(dst, src, n);
来源：http://bel.birdmap.top

[S26] C：内存清零
来源：http://fuj.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://jyz.birdmap.top

[S27] C：定义常量
来源：http://kfn.meibo888.top

const double PI = 3.14159;
来源：http://tcg.fktsv.cn

[S28] C：静态变量
来源：http://dzw.iojbl.cn

static int counter = 0;
来源：http://rea.ctjpmb.com

[S29] C：变参函数
来源：http://hxk.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://woc.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://mua.bbcook.cn

#ifndef X_H
来源：http://pit.redwolf501.top

#define X_H
来源：http://svp.vehdjk.com

#endif
来源：http://xjv.feifeiyinyue.top

[S31] C++：Hello World
来源：http://grv.kuanghao11.cn

#include <iostream>
来源：http://dwa.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pde.zhoulong.xyz

[S32] C++：字符串
来源：http://oqz.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://jkl.yueranfly.top

[S33] C++：vector 增删
来源：http://sep.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jof.shzxlz.cn

[S34] C++：遍历 vector
来源：http://fqw.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://qpz.shanyushiyangtech.top

[S35] C++：map
来源：http://gdx.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sgi.aibaodan.cn

[S36] C++：unordered_map
来源：http://znv.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mbz.ehwqpu.com

[S37] C++：set
来源：http://ovo.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bxl.jinyuanbaomall.cn

[S38] C++：排序
来源：http://fjx.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://oqu.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://onz.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cvc.meibo888.top

[S40] C++：查找元素
来源：http://bmx.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kgw.yj202588.top

[S41] C++：类与构造函数
来源：http://ebv.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mrc.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://eyo.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://pkg.hysaishi.cn

[S43] C++：智能指针
来源：http://ldy.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://afa.zhijiandao.cn

[S44] C++：引用传参
来源：http://ynk.daxiang520.top

void inc(int &x) { ++x; }
来源：http://uww.52xcode.cn

[S45] C++：lambda
来源：http://idm.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://lrx.fzhhl.top

[S46] C++：函数模板
来源：http://jtf.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qxn.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://ylf.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mrr.jinqigufen.top

[S48] C++：逐行读文件
来源：http://axl.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gth.hesvh.cn

while (std::getline(in, line)) { }
来源：http://cfv.nanxuanxn.top

[S49] C++：写文件
来源：http://aia.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://myz.chenzaomai.com

[S50] C++：格式化数字
来源：http://vvd.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vvl.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://whm.gaohongyu789.top

static_cast<double>(a) / b
来源：http://cvv.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://ebi.c1oappe.top

int size() const noexcept { return n_; }
来源：http://upf.bbcook.cn

[S53] C++：移动语义
来源：http://mzy.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://scd.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://xth.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wkr.jqgfzy.top

[S55] C++：结构化绑定
来源：http://igq.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xvo.zhaomingkeji.xyz

[S56] C++：optional
来源：http://vkn.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sja.hesvh.cn

[S57] C++：编译期常量
来源：http://hkk.aizwys.cn

constexpr int N = 10;
来源：http://sdy.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://eys.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://nhw.ydjk.org.cn

[S59] C++：静态断言
来源：http://dxu.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyl.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://fyl.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://stz.guowangkeji.top

================================================================================
来源：http://zdp.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://agf.jiagoushi.top

================================================================================
来源：http://lkm.hesvh.cn

[T01] Kotlin：Hello World
来源：http://iwy.xziqi.cn

println("Hello")
来源：http://xbj.quarkkingdee.top

[T02] Kotlin：变量
来源：http://jia.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpn.cheryme.top

[T03] Kotlin：字符串模板
来源：http://pos.shzxlz.cn

"值: $b"
来源：http://fhm.jinqigufen.top

[T04] Kotlin：空安全
来源：http://crw.gzhubu.top

val n: String? = null;  n?.length
来源：http://kgt.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://cvc.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lvj.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://age.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vae.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://hdy.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ddb.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://gqh.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://faq.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://cjn.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://qyp.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://mgy.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ulq.xuanzx.com

[T11] Kotlin：协程
来源：http://pqq.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kwb.aizwys.cn

[T12] Kotlin：解构声明
来源：http://zhr.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://sbg.cashguo.top

[T13] Kotlin：只读 Map
来源：http://slu.ybcxt.top

val m = mapOf("a" to 1)
来源：http://pgv.nwbrower.top

[T14] Kotlin：循环
来源：http://lnv.shuidangran.top

for (i in 1..10) println(i)
来源：http://dra.aizwys.cn

[T15] Kotlin：接口
来源：http://pef.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://dhv.ppjwa.cn

[T16] Swift：Hello World
来源：http://qwx.iojbl.cn

print("Hello")
来源：http://vdq.jianghu66.top

[T17] Swift：变量与常量
来源：http://ftf.havefunace.top

var a = 1;  let b = 2
来源：http://qsc.sweek.top

[T18] Swift：字符串插值
来源：http://lvn.0kj1m.cn

"值: \(b)"
来源：http://qkl.uphjek.com

[T19] Swift：可选绑定
来源：http://fnq.9152youxi.cn

if let n = opt { print(n) }
来源：http://eqt.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://lxk.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mft.c1oappe.top

[T21] Swift：遍历
来源：http://dzy.ctjpmb.com

for x in a { print(x) }
来源：http://tqc.aibaodan.cn

[T22] Swift：字典
来源：http://zry.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://cgc.cdnleiting.top

[T23] Swift：函数
来源：http://wvy.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bnv.bbcook.cn

[T24] Swift：闭包
来源：http://xtt.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://igc.birdmap.top


<!-- 参考信息 -->