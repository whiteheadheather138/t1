代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tpe.xinyue.icu

[R16] until 等待条件
来源：http://xgo.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kwp.snrcjt.cn

[R17] 数组定义与取值
来源：http://yac.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nih.sjlbkw.cn

[R18] 遍历数组
来源：http://fai.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kvb.gogol.net.cn

[R19] 数组长度
来源：http://hve.sxryk.cn

echo "${#arr[@]}"
来源：http://egq.cqqwz.cn

[R20] 关联数组（字典）
来源：http://bdm.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gmn.andypj.xyz

[R21] 字符串长度
来源：http://upx.chenzaomai.com

echo "${#s}"
来源：http://ubb.vqdsnc.cn

[R22] 截取子串
来源：http://bgq.yanxiufei.cn

echo "${s:0:5}"
来源：http://tny.ppjwa.cn

[R23] 字符串替换
来源：http://pcn.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ipr.andypj.xyz

[R24] 大小写转换
来源：http://seb.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://zxf.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://yll.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrb.gotoacloud.top

[R26] 命令替换
来源：http://jim.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://fcn.bbcook.cn

[R27] 算术展开
来源：http://yrn.xziqi.cn

echo $((1 + 2 * 3))
来源：http://qqs.hongshengwenyu.top

[R28] 浮点运算
来源：http://ami.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://gop.yvedp.cn

[R29] 定义函数
来源：http://dqt.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kfr.jinqigufen.top

[R30] 函数返回状态码
来源：http://srt.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://uni.ydzc1.top

[R31] 局部变量
来源：http://ndw.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://dlv.ivvv.top

[R32] 参数个数校验
来源：http://icp.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ixd.tarul.cn

[R33] 捕获错误并提示行号
来源：http://iqf.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ljj.sysykeji.top

[R34] 退出时清理
来源：http://hfu.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://gxt.yangfankeji.com

[R35] 后台执行并等待
来源：http://kil.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qjk.jqgfzy.top

[R36] 并发执行多个任务
来源：http://mlv.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://flb.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://rcw.hnqzz.top

files=$(ls -1)
来源：http://lxg.sjlbkw.cn

[R38] 管道串联
来源：http://xoq.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://lei.316326.xyz

[R39] 重定向标准输出与错误
来源：http://mlz.dianchejie.cn

cmd > out.log 2>&1
来源：http://ovi.gaohongyu789.top

[R40] 追加写日志
来源：http://lyo.yonumen.top

echo "log" >> out.log
来源：http://rfr.ppjwa.cn

[R41] 丢弃输出
来源：http://icu.xylfe.cn

cmd >/dev/null 2>&1
来源：http://fsm.daria6918.cn

[R42] 输入重定向
来源：http://htl.smart0.xyz

wc -l < a.txt
来源：http://rrr.xylfe.cn

[R43] 按名字查找文件
来源：http://ady.0kj1m.cn

find . -name "*.log" -type f
来源：http://jaf.zhoulong.xyz

[R44] 按修改时间查找
来源：http://yic.fzhhl.top

find . -mtime -7 -type f
来源：http://owy.zhijiandao.cn

[R45] 批量删除
来源：http://lsq.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://fgd.pycfn.com

[R46] 递归替换文件内容
来源：http://ltm.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dga.zdbjq.cn

[R47] sed 单行替换
来源：http://ccw.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://ezm.gotoacloud.top

[R48] awk 取指定列
来源：http://cve.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://hyf.dianchejie.cn

[R49] awk 带条件
来源：http://hjg.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvj.hfpthk.cn

[R50] awk 求和
来源：http://dvh.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ciq.epnwcf.com

[R51] 排序去重取前几
来源：http://kgr.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zod.yuanzhike.top

[R52] 统计行数
来源：http://ohq.bjfxy.top

wc -l a.txt
来源：http://sfl.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://bbo.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://alk.316326.xyz

[R54] 比较两个文件
来源：http://eqj.xziqi.cn

diff a.txt b.txt
来源：http://foo.daria6918.cn

[R55] 压缩与解压
来源：http://jii.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idz.guowangkeji.top

[R56] 远程拷贝
来源：http://xav.xylfe.cn

scp file user@host:/path/
来源：http://hpk.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://fle.xziqi.cn

ssh user@host 'uptime'
来源：http://evn.hongshengwenyu.top

[R58] 下载文件
来源：http://ozt.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tvm.ydjk.org.cn

[R59] 发 POST JSON
来源：http://fyt.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uta.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://ybu.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nph.wangshuangyany.cn

[R61] 磁盘占用
来源：http://kdd.sjlbkw.cn

df -h;  du -sh *
来源：http://pho.svipenyu.cn

[R62] 找最占空间的文件
来源：http://wcu.hammf.cn

du -ah . | sort -rh | head -10
来源：http://cwu.xinyue.icu

[R63] 内存与进程
来源：http://gia.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://hxl.gotoacloud.top

[R64] 结束进程
来源：http://agb.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://mtw.gzhubu.top

[R65] 查看端口占用
来源：http://eze.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xtu.nwbrower.top

[R66] 定时任务
来源：http://qvw.ehwqpu.com

crontab -e;  crontab -l
来源：http://ujy.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://fym.wangshuangyany.cn

openssl rand -hex 16
来源：http://lrv.yongpay.top

[R68] 计算文件校验值
来源：http://oqe.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ukj.sjlbkw.cn

[R69] 生成随机密码
来源：http://oqm.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://irl.bjfxy.top

[R70] 时间戳与互转
来源：http://msf.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://wah.kuanghao11.cn

[R71] 日期格式化
来源：http://occ.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vth.andypj.xyz

[R72] 等待端口就绪
来源：http://yxn.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qzl.hongshengwenyu.top

[R73] 分割大日志
来源：http://mbs.hesvh.cn

split -l 1000 big.log part_
来源：http://ugj.hesvh.cn

[R74] 批量重命名
来源：http://fdy.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://njc.cucudq.cn

[R75] 导出环境变量
来源：http://lhc.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://hcz.chenzaomai.com

[R76] 使用临时文件
来源：http://jci.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bij.jqgfzy.top

[R77] 读取用户输入
来源：http://azs.nanxuanxn.top

read -rp "请输入: " ans
来源：http://nwe.jinqigfzy.top

[R78] 交互式菜单
来源：http://qtq.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jjl.jinqigfzy.top

[R79] 解析命令行选项
来源：http://vmg.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mmd.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://jkg.9152youxi.cn

time ./run.sh
来源：http://bxr.jlsjyb.cn

================================================================================
来源：http://jkh.ydzc1.top

S. C / C++ 专题
来源：http://nuu.316326.xyz

================================================================================
来源：http://ywf.xuetiantiany.cn

[S01] C：Hello World
来源：http://rvh.guannengcc.top

#include <stdio.h>
来源：http://brc.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vqs.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://oer.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://ban.tianlin.xyz

[S03] C：读入整数
来源：http://hdy.pycfn.com

int x; scanf("%d", &x);
来源：http://jnq.ehwqpu.com

[S04] C：字符串复制
来源：http://thy.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://ist.redwolf501.top

[S05] C：字符串长度
来源：http://ajv.xingfuxueyuan.xyz

strlen(s)
来源：http://ppq.hnqzz.top

[S06] C：字符串比较
来源：http://pzw.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://bll.epnwcf.com

[S07] C：数组遍历求和
来源：http://kzz.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hlq.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://qqr.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aqn.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://wfn.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vvf.gaohongyu789.top

[S10] C：指针与解引用
来源：http://cwq.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://ybh.jiagoushi.top

[S11] C：逐行读文件
来源：http://jlj.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://tbt.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://stn.hfpthk.cn

fclose(f);
来源：http://gps.zhixingplan.top

[S12] C：写文件
来源：http://ieo.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kkf.yongpay.top

[S13] C：宏定义
来源：http://zlk.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gmx.hfpthk.cn

[S14] C：枚举
来源：http://izm.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://imy.wangshuangyany.cn

[S15] C：类型转换
来源：http://emk.guowangkeji.top

(double) a / b
来源：http://vpj.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://wek.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://vhh.nwbrower.top

[S17] C：安全拼接字符串
来源：http://egm.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kym.ehwqpu.com

[S18] C：命令行参数
来源：http://ukg.jinqigufen.top

int main(int argc, char **argv)
来源：http://htq.yuxming.cn

[S19] C：快速排序
来源：http://pgp.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aya.hnqzz.top

[S20] C：二分查找
来源：http://ywz.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://leu.yfazqb.com

[S21] C：字符类别判断
来源：http://gyl.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tzr.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://pkn.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://wen.fehbvm.com

[S23] C：随机数
来源：http://uqv.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://fzc.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://kbc.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rmt.daxiang520.top

[S25] C：内存拷贝
来源：http://hal.hnxiangtu.top

memcpy(dst, src, n);
来源：http://iqd.jyoumei.cn

[S26] C：内存清零
来源：http://azi.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://mvn.yanxiufei.cn

[S27] C：定义常量
来源：http://xnl.zhongyouzk.top

const double PI = 3.14159;
来源：http://swc.hysaishi.cn

[S28] C：静态变量
来源：http://pll.hysaishi.cn

static int counter = 0;
来源：http://sxv.guowangkeji.top

[S29] C：变参函数
来源：http://kos.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lvv.chenlongwang.top

[S30] C：头文件保护
来源：http://hgg.yanxiufei.cn

#ifndef X_H
来源：http://mzs.xuanzx.com

#define X_H
来源：http://obr.fzhhl.top

#endif
来源：http://hyw.fktsv.cn

[S31] C++：Hello World
来源：http://pai.nwbrower.top

#include <iostream>
来源：http://shm.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://elu.hcnkem.com

[S32] C++：字符串
来源：http://oac.meibo888.top

std::string s = "hi";  s += "!";
来源：http://mlz.dianchejie.cn

[S33] C++：vector 增删
来源：http://aru.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eih.ybcxt.top

[S34] C++：遍历 vector
来源：http://fef.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://alh.epnwcf.com

[S35] C++：map
来源：http://zgx.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vbw.xylfe.cn

[S36] C++：unordered_map
来源：http://smb.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tnk.zhaomingkeji.xyz

[S37] C++：set
来源：http://xls.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://psa.vehdjk.com

[S38] C++：排序
来源：http://tqj.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://pfg.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://cqo.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wkn.yueranfly.top

[S40] C++：查找元素
来源：http://nbx.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nqw.svipenyu.cn

[S41] C++：类与构造函数
来源：http://suw.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cra.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://xuo.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://ilc.hongshengwenyu.top

[S43] C++：智能指针
来源：http://wzv.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://vxk.zhongyouzk.top

[S44] C++：引用传参
来源：http://naf.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://mbt.tarul.cn

[S45] C++：lambda
来源：http://tnr.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://rkw.yuxming.cn

[S46] C++：函数模板
来源：http://jln.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uey.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://min.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvb.bbcook.cn

[S48] C++：逐行读文件
来源：http://blm.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://tyu.yuxming.cn

while (std::getline(in, line)) { }
来源：http://aeo.chenlongwang.top

[S49] C++：写文件
来源：http://mnc.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ntj.shuidangran.top

[S50] C++：格式化数字
来源：http://ikn.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bky.ybcxt.top

[S51] C++：显式类型转换
来源：http://roc.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://lpz.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://skm.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://ymh.tanke756.top

[S53] C++：移动语义
来源：http://rmq.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://irb.mhx1999.top

[S54] C++：异常处理
来源：http://rnz.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://scb.mhx1999.top

[S55] C++：结构化绑定
来源：http://mof.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vxh.vehdjk.com

[S56] C++：optional
来源：http://sxy.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nkv.shzxlz.cn

[S57] C++：编译期常量
来源：http://vpe.hnxiangtu.top

constexpr int N = 10;
来源：http://zok.kuanghao11.cn

[S58] C++：命名空间
来源：http://ydg.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://iwv.vqdsnc.cn

[S59] C++：静态断言
来源：http://fxy.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nyx.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://xtr.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://opo.316326.xyz

================================================================================
来源：http://hxy.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfb.ivvv.top

================================================================================
来源：http://ehi.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://gwx.nanxuanxn.top

println("Hello")
来源：http://nmz.sweek.top

[T02] Kotlin：变量
来源：http://msn.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ulq.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://cgu.hongshengwenyu.top

"值: $b"
来源：http://cyh.9152youxi.cn

[T04] Kotlin：空安全
来源：http://gvh.daxiang520.top

val n: String? = null;  n?.length
来源：http://fxi.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://bco.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xkx.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://jeg.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://axz.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://lrl.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ioy.zhengqikj.top

[T08] Kotlin：数据类
来源：http://neh.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://gop.yongpay.top

[T09] Kotlin：扩展函数
来源：http://bgy.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://qeb.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://lpr.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oai.hywenlv.cn

[T11] Kotlin：协程
来源：http://nwe.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cmr.yj202588.top

[T12] Kotlin：解构声明
来源：http://xph.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://cyy.ivvv.top

[T13] Kotlin：只读 Map
来源：http://ahv.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://kyp.cheryme.top

[T14] Kotlin：循环
来源：http://bqi.jqgfzy.top

for (i in 1..10) println(i)
来源：http://sha.0kj1m.cn

[T15] Kotlin：接口
来源：http://bwe.havefunace.top

interface Shape { fun area(): Double }
来源：http://btt.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://qpf.nanxuanxn.top

print("Hello")
来源：http://ecd.daria6918.cn

[T17] Swift：变量与常量
来源：http://jlx.tianlin.xyz

var a = 1;  let b = 2
来源：http://vnf.aibaodan.cn

[T18] Swift：字符串插值
来源：http://kil.aizwys.cn

"值: \(b)"
来源：http://ltf.tarul.cn


<!-- 参考信息 -->