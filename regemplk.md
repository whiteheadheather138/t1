代发 wailian999

case "$1" in
来源：http://una.chenjidiqi.icu

start) echo "启动" ;;
来源：http://djf.52xcode.cn

stop)  echo "停止" ;;
来源：http://fqo.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://sdd.chenjidiqi.icu

esac
来源：http://avh.hongshengwenyu.top

[R12] for 遍历文件
来源：http://zjp.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://emi.andypj.xyz

[R13] for 计数循环
来源：http://koa.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://nli.zhoulong.xyz

[R14] C 风格 for
来源：http://jbk.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kbb.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://vpq.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://twt.xinyue.icu

[R16] until 等待条件
来源：http://rat.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nil.bbcook.cn

[R17] 数组定义与取值
来源：http://qhw.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://qoj.hywenlv.cn

[R18] 遍历数组
来源：http://ajv.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rks.hammf.cn

[R19] 数组长度
来源：http://eit.svipenyu.cn

echo "${#arr[@]}"
来源：http://gjo.yj202588.top

[R20] 关联数组（字典）
来源：http://iah.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://srn.havefunace.top

[R21] 字符串长度
来源：http://cza.zdqjudy.top

echo "${#s}"
来源：http://fho.zhaomingkeji.xyz

[R22] 截取子串
来源：http://krf.yuanzhike.top

echo "${s:0:5}"
来源：http://eee.nwbrower.top

[R23] 字符串替换
来源：http://yna.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ffq.mhx1999.top

[R24] 大小写转换
来源：http://kza.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pcw.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://euv.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jop.gaohongyu789.top

[R26] 命令替换
来源：http://bkb.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://yyz.sxryk.cn

[R27] 算术展开
来源：http://lma.sxryk.cn

echo $((1 + 2 * 3))
来源：http://ctf.jinqigufen.top

[R28] 浮点运算
来源：http://yjt.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://qtr.yanxiufei.cn

[R29] 定义函数
来源：http://kst.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://akq.ydzc1.top

[R30] 函数返回状态码
来源：http://pnm.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://pka.yj202588.top

[R31] 局部变量
来源：http://fyc.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://eeh.hfpthk.cn

[R32] 参数个数校验
来源：http://xad.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xjx.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://npe.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gyb.ppjwa.cn

[R34] 退出时清理
来源：http://eph.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://afx.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://pog.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oza.epnwcf.com

[R36] 并发执行多个任务
来源：http://gsa.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vjf.vehdjk.com

[R37] 把输出赋给变量
来源：http://cye.jianghu66.top

files=$(ls -1)
来源：http://jqc.jinqigfzy.top

[R38] 管道串联
来源：http://eab.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://xrh.cashguo.top

[R39] 重定向标准输出与错误
来源：http://taa.jyoumei.cn

cmd > out.log 2>&1
来源：http://wfp.haohaochexian.top

[R40] 追加写日志
来源：http://fai.zhongyouzk.top

echo "log" >> out.log
来源：http://kap.zdqjudy.top

[R41] 丢弃输出
来源：http://xrc.yonumen.top

cmd >/dev/null 2>&1
来源：http://pto.ppjwa.cn

[R42] 输入重定向
来源：http://del.zhiwuduotai.top

wc -l < a.txt
来源：http://ilu.hesvh.cn

[R43] 按名字查找文件
来源：http://zqw.gogol.net.cn

find . -name "*.log" -type f
来源：http://dpd.hammf.cn

[R44] 按修改时间查找
来源：http://dls.zhixingplan.top

find . -mtime -7 -type f
来源：http://xrm.sxryk.cn

[R45] 批量删除
来源：http://dmi.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://bhj.gzhubu.top

[R46] 递归替换文件内容
来源：http://anl.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mqf.fengsongda.top

[R47] sed 单行替换
来源：http://rbf.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ovm.cashguo.top

[R48] awk 取指定列
来源：http://wxc.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://rbe.vqdsnc.cn

[R49] awk 带条件
来源：http://pwb.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sld.gogol.net.cn

[R50] awk 求和
来源：http://twf.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://oaz.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://dxc.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xls.ydzc1.top

[R52] 统计行数
来源：http://fnl.yvedp.cn

wc -l a.txt
来源：http://tqf.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://yfx.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chu.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://sqs.xylfe.cn

diff a.txt b.txt
来源：http://cji.jianghu66.top

[R55] 压缩与解压
来源：http://uxv.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://utz.quarkkingdee.top

[R56] 远程拷贝
来源：http://suw.cashguo.top

scp file user@host:/path/
来源：http://fkv.aizwys.cn

[R57] 远程执行命令
来源：http://cgw.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://bhw.jiagoushi.top

[R58] 下载文件
来源：http://sze.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rjw.vehdjk.com

[R59] 发 POST JSON
来源：http://xjq.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rvl.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://xte.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rdj.yj202588.top

[R61] 磁盘占用
来源：http://ruy.316326.xyz

df -h;  du -sh *
来源：http://swa.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://zsf.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://dog.svipenyu.cn

[R63] 内存与进程
来源：http://yqz.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://mjy.yangfankeji.com

[R64] 结束进程
来源：http://ykp.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://kkx.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://mps.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bjg.chenzaomai.com

[R66] 定时任务
来源：http://tsn.zhixingplan.top

crontab -e;  crontab -l
来源：http://ekw.ivvv.top

[R67] 生成随机十六进制串
来源：http://luo.zdbjq.cn

openssl rand -hex 16
来源：http://rhe.uphjek.com

[R68] 计算文件校验值
来源：http://jtc.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://nqo.jqgufenzy.top

[R69] 生成随机密码
来源：http://qma.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://urc.shzxlz.cn

[R70] 时间戳与互转
来源：http://jet.ydzc1.top

date +%s;  date -d @1700000000
来源：http://rxi.c1oappe.top

[R71] 日期格式化
来源：http://drn.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eae.bbcook.cn

[R72] 等待端口就绪
来源：http://zsc.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ruo.bjfxy.top

[R73] 分割大日志
来源：http://tyf.yvedp.cn

split -l 1000 big.log part_
来源：http://btx.ctjpmb.com

[R74] 批量重命名
来源：http://jsj.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fbi.cqqwz.cn

[R75] 导出环境变量
来源：http://xjz.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ivq.yvedp.cn

[R76] 使用临时文件
来源：http://dzo.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hmg.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://mgy.zhengqikj.top

read -rp "请输入: " ans
来源：http://tgj.jqgfzy.top

[R78] 交互式菜单
来源：http://ako.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nyo.xuanzx.com

[R79] 解析命令行选项
来源：http://azz.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pse.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://kte.yj202588.top

time ./run.sh
来源：http://wxe.gotoacloud.top

================================================================================
来源：http://kfg.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://bgr.hysaishi.cn

================================================================================
来源：http://jmj.nwbrower.top

[S01] C：Hello World
来源：http://gze.jyoumei.cn

#include <stdio.h>
来源：http://dog.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://jbt.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://ggt.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://zhw.cdnleiting.top

[S03] C：读入整数
来源：http://moo.daxiang520.top

int x; scanf("%d", &x);
来源：http://epf.guannengcc.top

[S04] C：字符串复制
来源：http://lle.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://kic.chenlongwang.top

[S05] C：字符串长度
来源：http://wdf.fzhhl.top

strlen(s)
来源：http://tqe.yj20258.top

[S06] C：字符串比较
来源：http://wko.quarkkingdee.top

strcmp(a, b) == 0
来源：http://hkn.zycfv.cn

[S07] C：数组遍历求和
来源：http://eiv.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bmh.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://kck.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vxq.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://adq.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cko.cashguo.top

[S10] C：指针与解引用
来源：http://rcd.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://emz.quarkkingdee.top

[S11] C：逐行读文件
来源：http://wbv.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://lwz.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zav.pycfn.com

fclose(f);
来源：http://wpn.jinghuilouyu.cn

[S12] C：写文件
来源：http://oua.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://awx.zycfv.cn

[S13] C：宏定义
来源：http://hih.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vyd.jinyuanbaomall.cn

[S14] C：枚举
来源：http://glv.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://qiw.52xcode.cn

[S15] C：类型转换
来源：http://rtk.hesvh.cn

(double) a / b
来源：http://twa.yuanzhike.top

[S16] C：位操作置位
来源：http://szr.9152youxi.cn

x |= (1 << 3);
来源：http://sod.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://tal.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ahc.fengsongda.top

[S18] C：命令行参数
来源：http://bpz.mhx1999.top

int main(int argc, char **argv)
来源：http://gpq.smart0.xyz

[S19] C：快速排序
来源：http://bkx.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://rhp.yfazqb.com

[S20] C：二分查找
来源：http://xeo.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yce.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://vpw.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vec.jlsjyb.cn

[S22] C：字符串转数字
来源：http://bou.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://ylf.redwolf501.top

[S23] C：随机数
来源：http://oqa.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://slv.yj202588.top

[S24] C：获取本地时间
来源：http://mhs.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zcy.chenzaomai.com

[S25] C：内存拷贝
来源：http://epm.nanxuanxn.top

memcpy(dst, src, n);
来源：http://obh.fanxiaobao.xyz

[S26] C：内存清零
来源：http://bry.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://cfh.daxiang520.top

[S27] C：定义常量
来源：http://zgy.xuetiantiany.cn

const double PI = 3.14159;
来源：http://jgl.bjfxy.top

[S28] C：静态变量
来源：http://ipe.sysykeji.top

static int counter = 0;
来源：http://rem.jinqigfzy.top

[S29] C：变参函数
来源：http://xmz.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cry.bbcook.cn

[S30] C：头文件保护
来源：http://cbq.guowangkeji.top

#ifndef X_H
来源：http://dps.fehbvm.com

#define X_H
来源：http://gnn.ivvv.top

#endif
来源：http://yoi.cdnleiting.top

[S31] C++：Hello World
来源：http://mor.fktsv.cn

#include <iostream>
来源：http://ahg.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://tan.jinqigfzy.top

[S32] C++：字符串
来源：http://uaq.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://vga.ydjk.org.cn

[S33] C++：vector 增删
来源：http://bhg.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zlp.zhixingplan.top

[S34] C++：遍历 vector
来源：http://tae.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://njw.jinqigfzy.top

[S35] C++：map
来源：http://tvy.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yla.daria6918.cn

[S36] C++：unordered_map
来源：http://goo.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jky.vqdsnc.cn

[S37] C++：set
来源：http://dqn.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dta.sweek.top

[S38] C++：排序
来源：http://hkk.meibo888.top

std::sort(v.begin(), v.end());
来源：http://glq.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://hmg.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://guz.chenlongwang.top

[S40] C++：查找元素
来源：http://ymt.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uga.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://wue.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://irv.yj20258888.top

[S42] C++：继承与虚函数
来源：http://xod.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://kuv.guowangkeji.top

[S43] C++：智能指针
来源：http://ydt.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://ewi.yangfankeji.com

[S44] C++：引用传参
来源：http://snn.tanke756.top

void inc(int &x) { ++x; }
来源：http://ouv.vehdjk.com

[S45] C++：lambda
来源：http://kve.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://zsx.zhiwuduotai.top

[S46] C++：函数模板
来源：http://cms.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://clg.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://wyy.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jad.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://tiq.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://zoc.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://anb.cheryme.top

[S49] C++：写文件
来源：http://tia.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bpm.birdmap.top

[S50] C++：格式化数字
来源：http://rrb.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdz.ctjpmb.com

[S51] C++：显式类型转换
来源：http://nno.chenzaomai.com

static_cast<double>(a) / b
来源：http://ocm.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://vzw.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://nqn.yuanzhike.top

[S53] C++：移动语义
来源：http://yiy.ivvv.top

std::vector<int> w = std::move(v);
来源：http://muk.sufxvd.cn

[S54] C++：异常处理
来源：http://fgf.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uhj.yj20258.top

[S55] C++：结构化绑定
来源：http://qwa.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pnk.daria6918.cn

[S56] C++：optional
来源：http://tpv.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bxv.tanke756.top

[S57] C++：编译期常量
来源：http://ctf.dianchejie.cn

constexpr int N = 10;
来源：http://tvq.hongshengwenyu.top

[S58] C++：命名空间
来源：http://nks.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://rtf.yvedp.cn

[S59] C++：静态断言
来源：http://gtk.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://typ.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://rhs.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pog.xinyue.icu

================================================================================
来源：http://iof.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pzh.jyoumei.cn

================================================================================
来源：http://gtc.316326.xyz

[T01] Kotlin：Hello World
来源：http://ujz.zdqjudy.top

println("Hello")
来源：http://jpy.c1oappe.top

[T02] Kotlin：变量
来源：http://eeq.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pip.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://lss.aizwys.cn

"值: $b"
来源：http://fph.epnwcf.com

[T04] Kotlin：空安全
来源：http://xws.hesvh.cn

val n: String? = null;  n?.length
来源：http://ggp.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://apk.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://apx.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://xwm.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://adi.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://lry.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxx.yonumen.top

[T08] Kotlin：数据类
来源：http://jxj.hammf.cn

data class User(val name: String, val age: Int)
来源：http://xfp.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://ujk.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://lkf.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://arp.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lxw.yangfankeji.com

[T11] Kotlin：协程
来源：http://pyv.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://saq.fehbvm.com

[T12] Kotlin：解构声明
来源：http://qmo.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://guo.pycfn.com


<!-- 参考信息 -->