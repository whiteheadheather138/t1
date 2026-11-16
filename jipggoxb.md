代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://zrh.hammf.cn

[R14] C 风格 for
来源：http://ueg.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wgt.hcnkem.com

[R15] while 逐行读文件
来源：http://uyv.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gvh.yanxiufei.cn

[R16] until 等待条件
来源：http://pxv.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ibe.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://uuc.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://lvs.aibaodan.cn

[R18] 遍历数组
来源：http://jxf.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uxy.nwbrower.top

[R19] 数组长度
来源：http://vnm.hesvh.cn

echo "${#arr[@]}"
来源：http://uaz.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://dst.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tos.0kj1m.cn

[R21] 字符串长度
来源：http://qpn.zdbjq.cn

echo "${#s}"
来源：http://ptr.ppjwa.cn

[R22] 截取子串
来源：http://xlp.jinqigufen.top

echo "${s:0:5}"
来源：http://ahc.sxryk.cn

[R23] 字符串替换
来源：http://ipv.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xpm.gogol.net.cn

[R24] 大小写转换
来源：http://xls.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://ubn.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://iau.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vnl.haohaochexian.top

[R26] 命令替换
来源：http://wmb.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://irb.hesvh.cn

[R27] 算术展开
来源：http://oja.xuanzx.com

echo $((1 + 2 * 3))
来源：http://eug.yvedp.cn

[R28] 浮点运算
来源：http://nic.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://wmu.fehbvm.com

[R29] 定义函数
来源：http://xsj.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lfc.ydzc1.top

[R30] 函数返回状态码
来源：http://ros.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://auy.nanxinkj.top

[R31] 局部变量
来源：http://xez.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://fmh.zdbjq.cn

[R32] 参数个数校验
来源：http://vnn.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lzf.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://fmx.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pkb.gotoacloud.top

[R34] 退出时清理
来源：http://gcx.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://vll.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://yyc.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lzo.zycfv.cn

[R36] 并发执行多个任务
来源：http://dqy.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wra.ybcxt.top

[R37] 把输出赋给变量
来源：http://zkr.nwbrower.top

files=$(ls -1)
来源：http://ffq.daxiang520.top

[R38] 管道串联
来源：http://sky.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://ool.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://fum.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://puq.wangshuangyany.cn

[R40] 追加写日志
来源：http://jdd.jiagoushi.top

echo "log" >> out.log
来源：http://bay.hysaishi.cn

[R41] 丢弃输出
来源：http://brp.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://tzs.bbcook.cn

[R42] 输入重定向
来源：http://dyb.hnxiangtu.top

wc -l < a.txt
来源：http://axu.smart0.xyz

[R43] 按名字查找文件
来源：http://xmv.tian-w.cn

find . -name "*.log" -type f
来源：http://vuh.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://out.sxryk.cn

find . -mtime -7 -type f
来源：http://ixt.nwbrower.top

[R45] 批量删除
来源：http://mhz.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://nrc.yj202588.top

[R46] 递归替换文件内容
来源：http://xsp.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uag.sweek.top

[R47] sed 单行替换
来源：http://bkn.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://swd.hfpthk.cn

[R48] awk 取指定列
来源：http://pzp.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://axt.meibo888.top

[R49] awk 带条件
来源：http://tvc.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wqm.52xcode.cn

[R50] awk 求和
来源：http://xhu.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yxp.bbcook.cn

[R51] 排序去重取前几
来源：http://djx.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zjq.svipenyu.cn

[R52] 统计行数
来源：http://sax.zdbjq.cn

wc -l a.txt
来源：http://uus.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://kya.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cla.chenzaomai.com

[R54] 比较两个文件
来源：http://uhn.yonumen.top

diff a.txt b.txt
来源：http://bdc.hfpthk.cn

[R55] 压缩与解压
来源：http://lxm.c1oappe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zre.c1oappe.top

[R56] 远程拷贝
来源：http://sht.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://jpu.yanxiufei.cn

[R57] 远程执行命令
来源：http://hkj.ppjwa.cn

ssh user@host 'uptime'
来源：http://cpq.fzhhl.top

[R58] 下载文件
来源：http://dax.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qie.aibaodan.cn

[R59] 发 POST JSON
来源：http://vfr.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hfe.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://bdv.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ovn.uphjek.com

[R61] 磁盘占用
来源：http://pck.yonumen.top

df -h;  du -sh *
来源：http://xex.jinqigufen.top

[R62] 找最占空间的文件
来源：http://cmv.hammf.cn

du -ah . | sort -rh | head -10
来源：http://xgu.tian-w.cn

[R63] 内存与进程
来源：http://pdk.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://ful.guannengcc.top

[R64] 结束进程
来源：http://cnx.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://tyq.xinyue.icu

[R65] 查看端口占用
来源：http://fwz.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cef.uphjek.com

[R66] 定时任务
来源：http://ltj.zycfv.cn

crontab -e;  crontab -l
来源：http://rrb.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://dcx.zhijiandao.cn

openssl rand -hex 16
来源：http://xav.gaohongyu789.top

[R68] 计算文件校验值
来源：http://pmc.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://ywv.smart0.xyz

[R69] 生成随机密码
来源：http://lvc.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://ady.quarkkingdee.top

[R70] 时间戳与互转
来源：http://lyg.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://car.zhoulong.xyz

[R71] 日期格式化
来源：http://wws.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sqo.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://gog.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://dyc.zhoulong.xyz

[R73] 分割大日志
来源：http://mnh.hysaishi.cn

split -l 1000 big.log part_
来源：http://aql.sxryk.cn

[R74] 批量重命名
来源：http://geu.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kgu.nanxuanxn.top

[R75] 导出环境变量
来源：http://fxh.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://oep.guannengcc.top

[R76] 使用临时文件
来源：http://etq.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kfq.zhiwuduotai.top

[R77] 读取用户输入
来源：http://tam.cheryme.top

read -rp "请输入: " ans
来源：http://hsf.jinqigufen.top

[R78] 交互式菜单
来源：http://uhp.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hrc.vehdjk.com

[R79] 解析命令行选项
来源：http://mey.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fjc.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://qmr.wangdashe.top

time ./run.sh
来源：http://bfy.hywenlv.cn

================================================================================
来源：http://hkp.gzhubu.top

S. C / C++ 专题
来源：http://rys.jinqigufen.top

================================================================================
来源：http://btx.yvedp.cn

[S01] C：Hello World
来源：http://hda.yangfankeji.com

#include <stdio.h>
来源：http://kam.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kmm.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://jvy.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://njj.feifeiyinyue.top

[S03] C：读入整数
来源：http://vej.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://hcr.gogol.net.cn

[S04] C：字符串复制
来源：http://vgj.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fwn.zhiwuduotai.top

[S05] C：字符串长度
来源：http://xqx.zycfv.cn

strlen(s)
来源：http://ohf.cqqwz.cn

[S06] C：字符串比较
来源：http://csw.cucudq.cn

strcmp(a, b) == 0
来源：http://hlz.ivvv.top

[S07] C：数组遍历求和
来源：http://mwp.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fat.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://dvg.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zkq.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://aqs.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://czf.yangfankeji.com

[S10] C：指针与解引用
来源：http://vms.ybcxt.top

int *p = &a;  *p = 5;
来源：http://rbc.kuanghao11.cn

[S11] C：逐行读文件
来源：http://yut.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://bks.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://czg.haohaochexian.top

fclose(f);
来源：http://ebs.hcnkem.com

[S12] C：写文件
来源：http://ohj.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://adn.dashuyun.cn

[S13] C：宏定义
来源：http://cbc.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jrx.zhixingplan.top

[S14] C：枚举
来源：http://lzo.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://ouv.jinghuilouyu.cn

[S15] C：类型转换
来源：http://qxv.yueranfly.top

(double) a / b
来源：http://hhv.nanxuanxn.top

[S16] C：位操作置位
来源：http://rlp.ivvv.top

x |= (1 << 3);
来源：http://zvc.tian-w.cn

[S17] C：安全拼接字符串
来源：http://jay.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uyv.zhoulong.xyz

[S18] C：命令行参数
来源：http://exf.yj20258888.top

int main(int argc, char **argv)
来源：http://prv.jiagoushi.top

[S19] C：快速排序
来源：http://zjz.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://zsd.xuetiantiany.cn

[S20] C：二分查找
来源：http://qhu.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pyb.jyoumei.cn

[S21] C：字符类别判断
来源：http://yyb.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpu.ydzc1.top

[S22] C：字符串转数字
来源：http://kwb.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://azh.fzhhl.top

[S23] C：随机数
来源：http://irx.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fam.cashguo.top

[S24] C：获取本地时间
来源：http://baa.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uhj.bbcook.cn

[S25] C：内存拷贝
来源：http://dgs.hcnkem.com

memcpy(dst, src, n);
来源：http://acz.ppjwa.cn

[S26] C：内存清零
来源：http://rat.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://yrb.hesvh.cn

[S27] C：定义常量
来源：http://pye.uphjek.com

const double PI = 3.14159;
来源：http://bqd.shanyushiyangtech.top

[S28] C：静态变量
来源：http://zkz.hysaishi.cn

static int counter = 0;
来源：http://syr.yuanzhike.top

[S29] C：变参函数
来源：http://umc.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ojh.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://mpw.meibo888.top

#ifndef X_H
来源：http://xqi.316326.xyz

#define X_H
来源：http://phd.redwolf501.top

#endif
来源：http://xct.cucudq.cn

[S31] C++：Hello World
来源：http://sqb.yuxming.cn

#include <iostream>
来源：http://dvl.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://scb.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://tor.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://xfx.tianlin.xyz

[S33] C++：vector 增删
来源：http://itz.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jex.yueranfly.top

[S34] C++：遍历 vector
来源：http://eel.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://ntu.sxryk.cn

[S35] C++：map
来源：http://rlj.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nff.hcnkem.com

[S36] C++：unordered_map
来源：http://hxu.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahl.dianchejie.cn

[S37] C++：set
来源：http://wli.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqp.ppjwa.cn

[S38] C++：排序
来源：http://gwk.sweek.top

std::sort(v.begin(), v.end());
来源：http://cuw.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://yab.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lhb.yangfankeji.com

[S40] C++：查找元素
来源：http://ecu.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wwg.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://ajs.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hwv.daria6918.cn

[S42] C++：继承与虚函数
来源：http://qdx.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://npo.tanke756.top

[S43] C++：智能指针
来源：http://kqx.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://rig.feifeiyinyue.top

[S44] C++：引用传参
来源：http://ggn.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://qxy.birdmap.top

[S45] C++：lambda
来源：http://zcu.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ewa.zhiwuduotai.top

[S46] C++：函数模板
来源：http://ysq.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eio.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://ewz.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sea.yj20258.top

[S48] C++：逐行读文件
来源：http://eqf.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://inl.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://dxu.jinghuilouyu.cn

[S49] C++：写文件
来源：http://ebr.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://izs.cashguo.top

[S50] C++：格式化数字
来源：http://kin.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ixw.epnwcf.com

[S51] C++：显式类型转换
来源：http://hcd.snrcjt.cn

static_cast<double>(a) / b
来源：http://axr.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://dop.316326.xyz

int size() const noexcept { return n_; }
来源：http://ruo.iojbl.cn

[S53] C++：移动语义
来源：http://msx.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://ctn.tianlin.xyz

[S54] C++：异常处理
来源：http://zxh.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://myn.hysaishi.cn

[S55] C++：结构化绑定
来源：http://zit.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ebm.daria6918.cn

[S56] C++：optional
来源：http://hrv.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qfl.hysaishi.cn

[S57] C++：编译期常量
来源：http://jxc.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://zwp.yuxming.cn

[S58] C++：命名空间
来源：http://ibz.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://qbx.daria6918.cn

[S59] C++：静态断言
来源：http://exo.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://itv.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://cwu.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bzf.sjlbkw.cn

================================================================================
来源：http://rph.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzy.dashuyun.cn

================================================================================
来源：http://fsq.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://szx.yj20258888.top

println("Hello")
来源：http://hkf.xziqi.cn

[T02] Kotlin：变量
来源：http://hpa.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jeo.meibo888.top

[T03] Kotlin：字符串模板
来源：http://szp.fengsongda.top

"值: $b"
来源：http://hla.bbcook.cn

[T04] Kotlin：空安全
来源：http://sfp.yuanzhike.top

val n: String? = null;  n?.length
来源：http://uxs.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://sui.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tad.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://dzd.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tgu.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://fre.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lzq.yangfankeji.com

[T08] Kotlin：数据类
来源：http://uwz.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://cdn.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://snf.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://suf.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://lhw.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ksb.cdnleiting.top

[T11] Kotlin：协程
来源：http://sqo.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vyq.yuxming.cn

[T12] Kotlin：解构声明
来源：http://syv.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://lgf.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://yxf.fehbvm.com

val m = mapOf("a" to 1)
来源：http://ryp.sysykeji.top

[T14] Kotlin：循环
来源：http://wqt.yj202588.top

for (i in 1..10) println(i)
来源：http://onz.jqgfzy.top

[T15] Kotlin：接口
来源：http://hcx.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://kue.gogol.net.cn

[T16] Swift：Hello World
来源：http://zmf.fengsongda.top

print("Hello")
来源：http://hwa.yongpay.top


<!-- 参考信息 -->