代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hxb.svipenyu.cn

[R18] 遍历数组
来源：http://wre.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rjo.nanxinkj.top

[R19] 数组长度
来源：http://qed.nanxuanxn.top

echo "${#arr[@]}"
来源：http://haq.fengsongda.top

[R20] 关联数组（字典）
来源：http://ala.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pov.yuanzhike.top

[R21] 字符串长度
来源：http://heo.zhengqikj.top

echo "${#s}"
来源：http://wgb.ehwqpu.com

[R22] 截取子串
来源：http://byx.yvedp.cn

echo "${s:0:5}"
来源：http://atc.yj202588.top

[R23] 字符串替换
来源：http://eal.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://obm.yj20258888.top

[R24] 大小写转换
来源：http://fjc.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://amx.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://dtu.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oft.aibaodan.cn

[R26] 命令替换
来源：http://zkh.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://zau.shanyushiyangtech.top

[R27] 算术展开
来源：http://dce.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://iax.redwolf501.top

[R28] 浮点运算
来源：http://xxu.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://pmu.gaohongyu789.top

[R29] 定义函数
来源：http://zhj.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://poz.yj20258888.top

[R30] 函数返回状态码
来源：http://uyf.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://hmh.smart0.xyz

[R31] 局部变量
来源：http://exl.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://rxj.hysaishi.cn

[R32] 参数个数校验
来源：http://pml.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dhz.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://qpa.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zyw.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://wsu.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://rew.shzxlz.cn

[R35] 后台执行并等待
来源：http://jlk.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ezh.316326.xyz

[R36] 并发执行多个任务
来源：http://xgw.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zeq.dashuyun.cn

[R37] 把输出赋给变量
来源：http://saz.aizwys.cn

files=$(ls -1)
来源：http://pvi.fanxiaobao.xyz

[R38] 管道串联
来源：http://tna.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://edl.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://dyk.guannengcc.top

cmd > out.log 2>&1
来源：http://grq.chenlongwang.top

[R40] 追加写日志
来源：http://wzr.shanyushiyangtech.top

echo "log" >> out.log
来源：http://mmo.hfpthk.cn

[R41] 丢弃输出
来源：http://kvw.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://efh.pycfn.com

[R42] 输入重定向
来源：http://pvt.xinyue.icu

wc -l < a.txt
来源：http://bzl.haohaochexian.top

[R43] 按名字查找文件
来源：http://bvg.yj202588.top

find . -name "*.log" -type f
来源：http://jng.yangfankeji.com

[R44] 按修改时间查找
来源：http://sfh.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://uvf.zhaomingkeji.xyz

[R45] 批量删除
来源：http://eqn.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://swe.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://zwn.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cea.aizwys.cn

[R47] sed 单行替换
来源：http://syk.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fvb.xziqi.cn

[R48] awk 取指定列
来源：http://uzx.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://hii.jinqigfzy.top

[R49] awk 带条件
来源：http://knh.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hxn.jinyuanbaomall.cn

[R50] awk 求和
来源：http://ues.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://mxo.xuanzx.com

[R51] 排序去重取前几
来源：http://hxy.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dpo.sweek.top

[R52] 统计行数
来源：http://wgy.hywenlv.cn

wc -l a.txt
来源：http://cuq.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://tbt.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://usc.pengpengdd.cyou

[R54] 比较两个文件
来源：http://prc.jinghuilouyu.cn

diff a.txt b.txt
来源：http://deg.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://fbf.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kzx.cqqwz.cn

[R56] 远程拷贝
来源：http://bqw.jqgufenzy.top

scp file user@host:/path/
来源：http://sfq.shuidangran.top

[R57] 远程执行命令
来源：http://xxq.hnxiangtu.top

ssh user@host 'uptime'
来源：http://efy.sufxvd.cn

[R58] 下载文件
来源：http://sap.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wpt.andypj.xyz

[R59] 发 POST JSON
来源：http://nrw.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rxe.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://xbk.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qme.yonumen.top

[R61] 磁盘占用
来源：http://anq.dianchejie.cn

df -h;  du -sh *
来源：http://mla.sxryk.cn

[R62] 找最占空间的文件
来源：http://nad.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://uwx.pycfn.com

[R63] 内存与进程
来源：http://fhz.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://dld.ywan-chungtsiang.top

[R64] 结束进程
来源：http://jup.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://lki.havefunace.top

[R65] 查看端口占用
来源：http://rtb.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://erb.haohaochexian.top

[R66] 定时任务
来源：http://deq.nanxuanxn.top

crontab -e;  crontab -l
来源：http://jde.fehbvm.com

[R67] 生成随机十六进制串
来源：http://aib.jinqigfzy.top

openssl rand -hex 16
来源：http://axi.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://sqq.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://est.vehdjk.com

[R69] 生成随机密码
来源：http://zug.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://vjg.hnxiangtu.top

[R70] 时间戳与互转
来源：http://rlw.hesvh.cn

date +%s;  date -d @1700000000
来源：http://xpn.ivvv.top

[R71] 日期格式化
来源：http://zhh.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://yql.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://coe.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mnc.9152youxi.cn

[R73] 分割大日志
来源：http://oze.yj20258888.top

split -l 1000 big.log part_
来源：http://uhn.gotoacloud.top

[R74] 批量重命名
来源：http://vsf.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://emf.sweek.top

[R75] 导出环境变量
来源：http://zxi.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://kcw.zdbjq.cn

[R76] 使用临时文件
来源：http://lru.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fdn.bjfxy.top

[R77] 读取用户输入
来源：http://tua.yj20258.top

read -rp "请输入: " ans
来源：http://sdq.yangfankeji.com

[R78] 交互式菜单
来源：http://yez.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://krl.xylfe.cn

[R79] 解析命令行选项
来源：http://kyf.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://axv.yj202588.top

[R80] 查看脚本执行耗时
来源：http://der.havefunace.top

time ./run.sh
来源：http://jsz.dashuyun.cn

================================================================================
来源：http://hit.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://bhy.smart0.xyz

================================================================================
来源：http://vab.quarkkingdee.top

[S01] C：Hello World
来源：http://qzv.havefunace.top

#include <stdio.h>
来源：http://lwi.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://tcw.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://iwc.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://rmn.shuidangran.top

[S03] C：读入整数
来源：http://iqs.tianlin.xyz

int x; scanf("%d", &x);
来源：http://qgk.fehbvm.com

[S04] C：字符串复制
来源：http://ifs.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://qkq.vqdsnc.cn

[S05] C：字符串长度
来源：http://pkr.birdmap.top

strlen(s)
来源：http://psm.zhijiandao.cn

[S06] C：字符串比较
来源：http://ngk.hcnkem.com

strcmp(a, b) == 0
来源：http://wpr.aibaodan.cn

[S07] C：数组遍历求和
来源：http://hee.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ubb.pycfn.com

[S08] C：动态内存分配与释放
来源：http://irv.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qee.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://xax.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bao.gogol.net.cn

[S10] C：指针与解引用
来源：http://vpv.sysykeji.top

int *p = &a;  *p = 5;
来源：http://peu.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://vdi.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ubg.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sip.hnqzz.top

fclose(f);
来源：http://xhv.0kj1m.cn

[S12] C：写文件
来源：http://zre.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfp.xziqi.cn

[S13] C：宏定义
来源：http://qza.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ksj.cheryme.top

[S14] C：枚举
来源：http://ezt.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://cxg.hnqzz.top

[S15] C：类型转换
来源：http://gjj.cashguo.top

(double) a / b
来源：http://uuc.havefunace.top

[S16] C：位操作置位
来源：http://sbh.sweek.top

x |= (1 << 3);
来源：http://jgm.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://piz.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ejt.ybcxt.top

[S18] C：命令行参数
来源：http://aka.yfazqb.com

int main(int argc, char **argv)
来源：http://qiu.hammf.cn

[S19] C：快速排序
来源：http://dcn.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://tjo.yanxiufei.cn

[S20] C：二分查找
来源：http://pny.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ydi.zdbjq.cn

[S21] C：字符类别判断
来源：http://vit.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bza.pycfn.com

[S22] C：字符串转数字
来源：http://dzc.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://idm.shanyushiyangtech.top

[S23] C：随机数
来源：http://wev.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://vke.uphjek.com

[S24] C：获取本地时间
来源：http://kod.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oar.hfpthk.cn

[S25] C：内存拷贝
来源：http://tim.xylfe.cn

memcpy(dst, src, n);
来源：http://dxl.cucudq.cn

[S26] C：内存清零
来源：http://ulp.cheryme.top

memset(a, 0, sizeof a);
来源：http://uby.havefunace.top

[S27] C：定义常量
来源：http://udo.9152youxi.cn

const double PI = 3.14159;
来源：http://axs.nanxinkj.top

[S28] C：静态变量
来源：http://uqq.fzhhl.top

static int counter = 0;
来源：http://xvv.ybcxt.top

[S29] C：变参函数
来源：http://ezg.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yuo.yanxiufei.cn

[S30] C：头文件保护
来源：http://ler.fzhhl.top

#ifndef X_H
来源：http://amf.zhoulong.xyz

#define X_H
来源：http://ysk.jianghu66.top

#endif
来源：http://sfg.hfpthk.cn

[S31] C++：Hello World
来源：http://uyg.dianchejie.cn

#include <iostream>
来源：http://dmq.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://fts.jqgfzy.top

[S32] C++：字符串
来源：http://fqb.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://oeh.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://jim.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukt.hysaishi.cn

[S34] C++：遍历 vector
来源：http://skp.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://ttx.smart0.xyz

[S35] C++：map
来源：http://nub.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhz.jqgfzy.top

[S36] C++：unordered_map
来源：http://ypp.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jbs.kuanghao11.cn

[S37] C++：set
来源：http://vwf.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqp.hywenlv.cn

[S38] C++：排序
来源：http://opn.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://srx.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://fhg.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rpm.andypj.xyz

[S40] C++：查找元素
来源：http://xjz.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pmy.gzhubu.top

[S41] C++：类与构造函数
来源：http://uqk.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://drt.xuanzx.com

[S42] C++：继承与虚函数
来源：http://cat.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://zcz.havefunace.top

[S43] C++：智能指针
来源：http://kvl.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://xqp.andypj.xyz

[S44] C++：引用传参
来源：http://fak.mhx1999.top

void inc(int &x) { ++x; }
来源：http://deg.tianlin.xyz

[S45] C++：lambda
来源：http://ofy.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ybr.cucudq.cn

[S46] C++：函数模板
来源：http://akl.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dxm.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://twe.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dpl.hcnkem.com

[S48] C++：逐行读文件
来源：http://gbd.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://ifl.daria6918.cn

while (std::getline(in, line)) { }
来源：http://ape.ydjk.org.cn

[S49] C++：写文件
来源：http://dwg.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://whw.havefunace.top

[S50] C++：格式化数字
来源：http://nyu.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nmu.ybcxt.top

[S51] C++：显式类型转换
来源：http://spn.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://bmw.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://ipt.uphjek.com

int size() const noexcept { return n_; }
来源：http://uwy.hongshengwenyu.top

[S53] C++：移动语义
来源：http://tmj.tarul.cn

std::vector<int> w = std::move(v);
来源：http://fjr.wangdashe.top

[S54] C++：异常处理
来源：http://qdp.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://omj.cucudq.cn

[S55] C++：结构化绑定
来源：http://wiy.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://igp.ehwqpu.com

[S56] C++：optional
来源：http://cbn.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rcb.ctjpmb.com

[S57] C++：编译期常量
来源：http://osg.bjfxy.top

constexpr int N = 10;
来源：http://mti.hfpthk.cn

[S58] C++：命名空间
来源：http://are.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://tgj.jlsjyb.cn

[S59] C++：静态断言
来源：http://rdh.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tkk.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://wqp.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fym.wangshuangyany.cn

================================================================================
来源：http://koc.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aif.316326.xyz

================================================================================
来源：http://vas.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://oce.havefunace.top

println("Hello")
来源：http://atg.yuxming.cn

[T02] Kotlin：变量
来源：http://yvb.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://roy.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://ptg.sxryk.cn

"值: $b"
来源：http://oaa.tianlin.xyz

[T04] Kotlin：空安全
来源：http://dsg.xinyue.icu

val n: String? = null;  n?.length
来源：http://kpi.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://azg.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bvz.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://ass.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rgk.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://hqy.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://viq.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://lve.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://azu.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://fav.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://sou.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://rav.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xgd.hywenlv.cn

[T11] Kotlin：协程
来源：http://ooa.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://diy.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://iwr.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://nai.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://fap.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://hog.epnwcf.com

[T14] Kotlin：循环
来源：http://vmp.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://pxb.xylfe.cn

[T15] Kotlin：接口
来源：http://rkz.cucudq.cn

interface Shape { fun area(): Double }
来源：http://saw.sufxvd.cn

[T16] Swift：Hello World
来源：http://kan.52xcode.cn

print("Hello")
来源：http://ytn.daxiang520.top

[T17] Swift：变量与常量
来源：http://zxq.ydjk.org.cn

var a = 1;  let b = 2
来源：http://iou.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://zdt.zycfv.cn

"值: \(b)"
来源：http://exg.iojbl.cn

[T19] Swift：可选绑定
来源：http://dbo.zdqjudy.top

if let n = opt { print(n) }
来源：http://ijh.zhongyouzk.top

[T20] Swift：数组操作
来源：http://bfr.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://sfe.jlsjyb.cn


<!-- 参考信息 -->