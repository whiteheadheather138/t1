代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rit.shuidangran.top

[R10] 正则匹配
来源：http://qbe.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rbg.gaohongyu789.top

[R11] case 多分支
来源：http://fxp.jqgufenzy.top

case "$1" in
来源：http://vnt.0kj1m.cn

start) echo "启动" ;;
来源：http://isu.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://bmt.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://szb.dashuyun.cn

esac
来源：http://zco.yangfankeji.com

[R12] for 遍历文件
来源：http://bor.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://ucd.redwolf501.top

[R13] for 计数循环
来源：http://kdw.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://dho.jianghu66.top

[R14] C 风格 for
来源：http://jmb.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yns.hywenlv.cn

[R15] while 逐行读文件
来源：http://jdl.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lyx.sxryk.cn

[R16] until 等待条件
来源：http://vhi.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mch.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://bwc.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://lvj.cashguo.top

[R18] 遍历数组
来源：http://enl.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://myv.zdbjq.cn

[R19] 数组长度
来源：http://uvf.daria6918.cn

echo "${#arr[@]}"
来源：http://ogt.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://orj.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jxj.ivvv.top

[R21] 字符串长度
来源：http://lvv.xziqi.cn

echo "${#s}"
来源：http://por.chenzaomai.com

[R22] 截取子串
来源：http://vdz.havefunace.top

echo "${s:0:5}"
来源：http://qih.dianchejie.cn

[R23] 字符串替换
来源：http://gep.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wvz.cqqwz.cn

[R24] 大小写转换
来源：http://bls.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://slb.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://vui.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kwh.epnwcf.com

[R26] 命令替换
来源：http://flf.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://ukk.tarul.cn

[R27] 算术展开
来源：http://eaj.guannengcc.top

echo $((1 + 2 * 3))
来源：http://xhu.ctjpmb.com

[R28] 浮点运算
来源：http://mtg.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://wmn.nwbrower.top

[R29] 定义函数
来源：http://hnl.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kjv.yongpay.top

[R30] 函数返回状态码
来源：http://dhq.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://bme.hysaishi.cn

[R31] 局部变量
来源：http://fng.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://kjm.yuxming.cn

[R32] 参数个数校验
来源：http://obd.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://whk.sweek.top

[R33] 捕获错误并提示行号
来源：http://fac.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://woq.yuxming.cn

[R34] 退出时清理
来源：http://lwc.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://pgh.hysaishi.cn

[R35] 后台执行并等待
来源：http://ofi.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pzl.guannengcc.top

[R36] 并发执行多个任务
来源：http://mcq.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bcq.guowangkeji.top

[R37] 把输出赋给变量
来源：http://tdk.yfazqb.com

files=$(ls -1)
来源：http://lhc.zhongyouzk.top

[R38] 管道串联
来源：http://uir.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://vws.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://udd.jqgufenzy.top

cmd > out.log 2>&1
来源：http://ppq.bjfxy.top

[R40] 追加写日志
来源：http://wcl.fktsv.cn

echo "log" >> out.log
来源：http://cjf.havefunace.top

[R41] 丢弃输出
来源：http://tet.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://nkb.dianchejie.cn

[R42] 输入重定向
来源：http://szo.hcnkem.com

wc -l < a.txt
来源：http://ubh.xuanzx.com

[R43] 按名字查找文件
来源：http://tyw.shuidangran.top

find . -name "*.log" -type f
来源：http://zvi.zhengqikj.top

[R44] 按修改时间查找
来源：http://vyj.xziqi.cn

find . -mtime -7 -type f
来源：http://ivn.epnwcf.com

[R45] 批量删除
来源：http://jec.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://oka.zhengqikj.top

[R46] 递归替换文件内容
来源：http://moe.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzu.shzxlz.cn

[R47] sed 单行替换
来源：http://trc.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://kwu.yonumen.top

[R48] awk 取指定列
来源：http://axo.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://arf.shzxlz.cn

[R49] awk 带条件
来源：http://jte.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hek.tarul.cn

[R50] awk 求和
来源：http://ndp.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://thq.iojbl.cn

[R51] 排序去重取前几
来源：http://sab.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oqh.jinghuilouyu.cn

[R52] 统计行数
来源：http://ugw.xylfe.cn

wc -l a.txt
来源：http://ntc.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://dio.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ndg.zhixingplan.top

[R54] 比较两个文件
来源：http://fvi.hammf.cn

diff a.txt b.txt
来源：http://aio.ydjk.org.cn

[R55] 压缩与解压
来源：http://mqq.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vpy.cqqwz.cn

[R56] 远程拷贝
来源：http://vld.havefunace.top

scp file user@host:/path/
来源：http://qgn.ybcxt.top

[R57] 远程执行命令
来源：http://mnr.xinyue.icu

ssh user@host 'uptime'
来源：http://hwd.meibo888.top

[R58] 下载文件
来源：http://jjv.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wuy.ybcxt.top

[R59] 发 POST JSON
来源：http://ztn.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wlo.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://uuq.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://avu.fktsv.cn

[R61] 磁盘占用
来源：http://izx.jinqigufen.top

df -h;  du -sh *
来源：http://gqp.pycfn.com

[R62] 找最占空间的文件
来源：http://dyp.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://zqf.ivvv.top

[R63] 内存与进程
来源：http://cef.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://pgb.aibaodan.cn

[R64] 结束进程
来源：http://eqi.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://bbd.yj202588.top

[R65] 查看端口占用
来源：http://egr.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://trk.gogol.net.cn

[R66] 定时任务
来源：http://tnj.yanxiufei.cn

crontab -e;  crontab -l
来源：http://tar.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://crf.hnqzz.top

openssl rand -hex 16
来源：http://yrr.yanxiufei.cn

[R68] 计算文件校验值
来源：http://oaz.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://usp.zycfv.cn

[R69] 生成随机密码
来源：http://iqe.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://uic.yj20258888.top

[R70] 时间戳与互转
来源：http://jtb.yj20258888.top

date +%s;  date -d @1700000000
来源：http://opo.iojbl.cn

[R71] 日期格式化
来源：http://pnk.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tqn.birdmap.top

[R72] 等待端口就绪
来源：http://dfp.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ogq.zhixingplan.top

[R73] 分割大日志
来源：http://pdk.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://mvk.gzhubu.top

[R74] 批量重命名
来源：http://nlp.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bgm.cdnleiting.top

[R75] 导出环境变量
来源：http://qwm.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://azd.ctjpmb.com

[R76] 使用临时文件
来源：http://zui.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zey.svipenyu.cn

[R77] 读取用户输入
来源：http://jcf.epnwcf.com

read -rp "请输入: " ans
来源：http://hnx.xinyue.icu

[R78] 交互式菜单
来源：http://avl.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://glx.xuanzx.com

[R79] 解析命令行选项
来源：http://jxx.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kaw.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://bng.daxiang520.top

time ./run.sh
来源：http://foy.sxryk.cn

================================================================================
来源：http://oez.hammf.cn

S. C / C++ 专题
来源：http://clc.yj20258888.top

================================================================================
来源：http://zpo.fzhhl.top

[S01] C：Hello World
来源：http://hwy.zhaomingkeji.xyz

#include <stdio.h>
来源：http://tvn.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ncs.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://jqq.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://umo.hnqzz.top

[S03] C：读入整数
来源：http://fvl.fengsongda.top

int x; scanf("%d", &x);
来源：http://htb.aizwys.cn

[S04] C：字符串复制
来源：http://jmd.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://gip.fengsongda.top

[S05] C：字符串长度
来源：http://myn.ybcxt.top

strlen(s)
来源：http://uev.zhengqikj.top

[S06] C：字符串比较
来源：http://hfk.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://xgk.tian-w.cn

[S07] C：数组遍历求和
来源：http://zbf.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vbb.yj202588.top

[S08] C：动态内存分配与释放
来源：http://oib.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qrn.birdmap.top

[S09] C：结构体定义与初始化
来源：http://vqz.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ome.zdbjq.cn

[S10] C：指针与解引用
来源：http://udq.bbcook.cn

int *p = &a;  *p = 5;
来源：http://rol.yj202588.top

[S11] C：逐行读文件
来源：http://jll.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://lpp.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xis.yangfankeji.com

fclose(f);
来源：http://zfm.316326.xyz

[S12] C：写文件
来源：http://imy.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aof.xuetiantiany.cn

[S13] C：宏定义
来源：http://jsr.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xdo.gogol.net.cn

[S14] C：枚举
来源：http://gip.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://ncb.yuanzhike.top

[S15] C：类型转换
来源：http://zyx.ctjpmb.com

(double) a / b
来源：http://bgc.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://kge.0kj1m.cn

x |= (1 << 3);
来源：http://nio.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://dml.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ntq.ehwqpu.com

[S18] C：命令行参数
来源：http://hjx.yanxiufei.cn

int main(int argc, char **argv)
来源：http://vzl.hammf.cn

[S19] C：快速排序
来源：http://rfm.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cdl.pengpengdd.cyou

[S20] C：二分查找
来源：http://psy.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://khr.quarkkingdee.top

[S21] C：字符类别判断
来源：http://vlx.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vsx.nwbrower.top

[S22] C：字符串转数字
来源：http://tpp.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://ina.fehbvm.com

[S23] C：随机数
来源：http://oel.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sor.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://bwu.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vzp.ehwqpu.com

[S25] C：内存拷贝
来源：http://zvm.nanxuanxn.top

memcpy(dst, src, n);
来源：http://mnf.jinqigfzy.top

[S26] C：内存清零
来源：http://swy.yvedp.cn

memset(a, 0, sizeof a);
来源：http://gpm.tianlin.xyz

[S27] C：定义常量
来源：http://hcp.aizwys.cn

const double PI = 3.14159;
来源：http://otl.0kj1m.cn

[S28] C：静态变量
来源：http://xex.yfazqb.com

static int counter = 0;
来源：http://dtq.xziqi.cn

[S29] C：变参函数
来源：http://cbx.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hcp.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://zof.hfpthk.cn

#ifndef X_H
来源：http://qqt.jinyuanbaomall.cn

#define X_H
来源：http://zve.iojbl.cn

#endif
来源：http://oxo.jinqigufen.top

[S31] C++：Hello World
来源：http://xuv.jianghu66.top

#include <iostream>
来源：http://ehz.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://eps.redwolf501.top

[S32] C++：字符串
来源：http://zwh.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://wsc.andypj.xyz

[S33] C++：vector 增删
来源：http://ktb.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ofk.ybcxt.top

[S34] C++：遍历 vector
来源：http://smr.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://mlt.tian-w.cn

[S35] C++：map
来源：http://syc.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dam.ydzc1.top

[S36] C++：unordered_map
来源：http://bgg.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://buy.meibo888.top

[S37] C++：set
来源：http://efx.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yis.gaohongyu789.top

[S38] C++：排序
来源：http://rbo.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://lvb.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://olp.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vrj.fehbvm.com

[S40] C++：查找元素
来源：http://xmm.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://amy.shuidangran.top

[S41] C++：类与构造函数
来源：http://yey.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://whj.andypj.xyz

[S42] C++：继承与虚函数
来源：http://hja.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://gmb.daria6918.cn

[S43] C++：智能指针
来源：http://mdn.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://spt.yangfankeji.com

[S44] C++：引用传参
来源：http://akq.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://aak.jianghu66.top

[S45] C++：lambda
来源：http://eys.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://crs.chenlongwang.top

[S46] C++：函数模板
来源：http://hpv.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gep.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://fuf.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qhs.52xcode.cn

[S48] C++：逐行读文件
来源：http://jwg.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ljz.bjfxy.top

while (std::getline(in, line)) { }
来源：http://jsw.ybcxt.top

[S49] C++：写文件
来源：http://fdz.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ter.iojbl.cn

[S50] C++：格式化数字
来源：http://inw.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cbs.jianghu66.top

[S51] C++：显式类型转换
来源：http://nbz.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://dhk.cheryme.top

[S52] C++：const 与 noexcept
来源：http://rac.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://jwc.shangyingyoupin.top

[S53] C++：移动语义
来源：http://ysu.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://krr.kuanghao11.cn

[S54] C++：异常处理
来源：http://mdm.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yhc.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://kbr.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://rid.snrcjt.cn

[S56] C++：optional
来源：http://ego.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vii.guannengcc.top

[S57] C++：编译期常量
来源：http://jac.daria6918.cn

constexpr int N = 10;
来源：http://ysq.snrcjt.cn

[S58] C++：命名空间
来源：http://avq.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://apu.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://nfb.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sii.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://ywn.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cdn.cucudq.cn

================================================================================
来源：http://pex.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzv.zycfv.cn

================================================================================
来源：http://ere.sysykeji.top

[T01] Kotlin：Hello World
来源：http://fto.chenzaomai.com

println("Hello")
来源：http://fou.nanxinkj.top

[T02] Kotlin：变量
来源：http://tve.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uoa.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://mkl.bjfxy.top

"值: $b"
来源：http://uyz.shuidangran.top

[T04] Kotlin：空安全
来源：http://ffu.cqqwz.cn

val n: String? = null;  n?.length
来源：http://tav.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://ocs.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zfl.316326.xyz

[T06] Kotlin：集合映射
来源：http://man.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sdt.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://hzb.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://shi.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://nnj.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://doj.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://oho.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://wjp.yongpay.top

[T10] Kotlin：默认参数
来源：http://pee.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vev.jqgufenzy.top


<!-- 参考信息 -->