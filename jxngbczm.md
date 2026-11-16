代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://akq.kuanghao11.cn

[R08] 数值比较
来源：http://cmf.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ljk.zhoulong.xyz

[R09] 字符串比较
来源：http://cai.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cum.aibaodan.cn

[R10] 正则匹配
来源：http://hby.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://snb.fktsv.cn

[R11] case 多分支
来源：http://hpd.yuxming.cn

case "$1" in
来源：http://ccm.zhixingplan.top

start) echo "启动" ;;
来源：http://mih.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://bve.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://ili.shuidangran.top

esac
来源：http://mzd.daxiang520.top

[R12] for 遍历文件
来源：http://fxy.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://cfj.haohaochexian.top

[R13] for 计数循环
来源：http://bba.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://jol.aibaodan.cn

[R14] C 风格 for
来源：http://xxc.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://omv.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://dln.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qwp.guowangkeji.top

[R16] until 等待条件
来源：http://ukr.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://myp.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://hci.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://utc.yanxiufei.cn

[R18] 遍历数组
来源：http://gps.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qis.yj20258888.top

[R19] 数组长度
来源：http://ppr.hywenlv.cn

echo "${#arr[@]}"
来源：http://vts.svipenyu.cn

[R20] 关联数组（字典）
来源：http://tkg.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ien.zhaomingkeji.xyz

[R21] 字符串长度
来源：http://hxy.bbcook.cn

echo "${#s}"
来源：http://ajz.gzhubu.top

[R22] 截取子串
来源：http://apk.ydzc1.top

echo "${s:0:5}"
来源：http://ipe.cucudq.cn

[R23] 字符串替换
来源：http://pdd.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hpl.fktsv.cn

[R24] 大小写转换
来源：http://rcd.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pvk.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://rbf.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pet.vqdsnc.cn

[R26] 命令替换
来源：http://qmx.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://feq.jianghu66.top

[R27] 算术展开
来源：http://ugd.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://bfd.quarkkingdee.top

[R28] 浮点运算
来源：http://ugt.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://fjw.tianlin.xyz

[R29] 定义函数
来源：http://pll.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cuc.nanxinkj.top

[R30] 函数返回状态码
来源：http://rji.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://xdo.havefunace.top

[R31] 局部变量
来源：http://lph.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://vqp.chenjidiqi.icu

[R32] 参数个数校验
来源：http://ien.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://erm.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://roa.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ews.9152youxi.cn

[R34] 退出时清理
来源：http://zvx.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ryg.havefunace.top

[R35] 后台执行并等待
来源：http://nzk.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ssy.hywenlv.cn

[R36] 并发执行多个任务
来源：http://qoo.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kuk.vehdjk.com

[R37] 把输出赋给变量
来源：http://wed.nwbrower.top

files=$(ls -1)
来源：http://mzi.xuanzx.com

[R38] 管道串联
来源：http://ncp.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://sqc.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://rbz.tianlin.xyz

cmd > out.log 2>&1
来源：http://rsr.vqdsnc.cn

[R40] 追加写日志
来源：http://fej.cdnleiting.top

echo "log" >> out.log
来源：http://jrn.hesvh.cn

[R41] 丢弃输出
来源：http://ppr.cheryme.top

cmd >/dev/null 2>&1
来源：http://hyl.mhx1999.top

[R42] 输入重定向
来源：http://jxt.chenzaomai.com

wc -l < a.txt
来源：http://gcy.aizwys.cn

[R43] 按名字查找文件
来源：http://vsn.zhongyouzk.top

find . -name "*.log" -type f
来源：http://iyr.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://dme.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://kpz.pengpengdd.cyou

[R45] 批量删除
来源：http://tpk.hesvh.cn

find . -name "*.tmp" -delete
来源：http://vut.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://lrd.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ksr.haohaochexian.top

[R47] sed 单行替换
来源：http://xiv.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://xnl.sysykeji.top

[R48] awk 取指定列
来源：http://uyh.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://vny.ehwqpu.com

[R49] awk 带条件
来源：http://zat.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ytk.zhongyouzk.top

[R50] awk 求和
来源：http://onh.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://oql.yonumen.top

[R51] 排序去重取前几
来源：http://dsv.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fqa.hywenlv.cn

[R52] 统计行数
来源：http://dda.pengpengdd.cyou

wc -l a.txt
来源：http://vbr.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://hhi.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bpo.yuanzhike.top

[R54] 比较两个文件
来源：http://sdm.jinqigfzy.top

diff a.txt b.txt
来源：http://cjh.gotoacloud.top

[R55] 压缩与解压
来源：http://dad.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iuf.nanxuanxn.top

[R56] 远程拷贝
来源：http://dde.hammf.cn

scp file user@host:/path/
来源：http://fbt.gaohongyu789.top

[R57] 远程执行命令
来源：http://hqp.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://jit.yuxming.cn

[R58] 下载文件
来源：http://eak.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yvd.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://yaz.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgf.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://zpf.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://peg.ctjpmb.com

[R61] 磁盘占用
来源：http://okx.jinghuilouyu.cn

df -h;  du -sh *
来源：http://frq.dianchejie.cn

[R62] 找最占空间的文件
来源：http://kfw.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://due.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://nqx.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://oas.zhaomingkeji.xyz

[R64] 结束进程
来源：http://gbd.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://tsu.mhx1999.top

[R65] 查看端口占用
来源：http://gng.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uom.yuxming.cn

[R66] 定时任务
来源：http://dlm.andypj.xyz

crontab -e;  crontab -l
来源：http://nfm.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://rvh.jyoumei.cn

openssl rand -hex 16
来源：http://gtq.xziqi.cn

[R68] 计算文件校验值
来源：http://pbf.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qqw.fehbvm.com

[R69] 生成随机密码
来源：http://yqn.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://xbz.aizwys.cn

[R70] 时间戳与互转
来源：http://tpe.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://fmy.yanxiufei.cn

[R71] 日期格式化
来源：http://ogy.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gsp.epnwcf.com

[R72] 等待端口就绪
来源：http://dtu.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://bfr.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://qua.zhixingplan.top

split -l 1000 big.log part_
来源：http://jhs.hesvh.cn

[R74] 批量重命名
来源：http://rdn.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mgb.hfpthk.cn

[R75] 导出环境变量
来源：http://fkt.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://lny.xuetiantiany.cn

[R76] 使用临时文件
来源：http://upn.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aus.gzhubu.top

[R77] 读取用户输入
来源：http://evq.zhixingplan.top

read -rp "请输入: " ans
来源：http://mzw.nwbrower.top

[R78] 交互式菜单
来源：http://cfw.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cwy.yj202588.top

[R79] 解析命令行选项
来源：http://jqh.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xdc.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://iam.zhixingplan.top

time ./run.sh
来源：http://sae.yj202588.top

================================================================================
来源：http://rgw.sjlbkw.cn

S. C / C++ 专题
来源：http://ceo.cheryme.top

================================================================================
来源：http://awg.smart0.xyz

[S01] C：Hello World
来源：http://zyb.hywenlv.cn

#include <stdio.h>
来源：http://czd.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://cjk.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://kfs.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://ssx.gaohongyu789.top

[S03] C：读入整数
来源：http://iar.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://lgj.hnxiangtu.top

[S04] C：字符串复制
来源：http://xsk.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://hmm.jqgufenzy.top

[S05] C：字符串长度
来源：http://wmr.aizwys.cn

strlen(s)
来源：http://hhx.xziqi.cn

[S06] C：字符串比较
来源：http://qtd.nanxinkj.top

strcmp(a, b) == 0
来源：http://rhx.shuidangran.top

[S07] C：数组遍历求和
来源：http://dvm.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zct.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://ypp.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://owo.sweek.top

[S09] C：结构体定义与初始化
来源：http://fmw.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eet.mhx1999.top

[S10] C：指针与解引用
来源：http://vql.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://wbv.316326.xyz

[S11] C：逐行读文件
来源：http://wih.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://viq.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xbb.redwolf501.top

fclose(f);
来源：http://uem.cashguo.top

[S12] C：写文件
来源：http://ext.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rpc.yangfankeji.com

[S13] C：宏定义
来源：http://sge.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hbd.yonumen.top

[S14] C：枚举
来源：http://pkn.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://qyk.shangyingyoupin.top

[S15] C：类型转换
来源：http://dov.hcnkem.com

(double) a / b
来源：http://fta.ydjk.org.cn

[S16] C：位操作置位
来源：http://qdw.ydjk.org.cn

x |= (1 << 3);
来源：http://oew.nwbrower.top

[S17] C：安全拼接字符串
来源：http://erp.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pgc.jyoumei.cn

[S18] C：命令行参数
来源：http://vkj.gaohongyu789.top

int main(int argc, char **argv)
来源：http://vge.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://chy.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://xhc.c1oappe.top

[S20] C：二分查找
来源：http://llt.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://svm.nanxinkj.top

[S21] C：字符类别判断
来源：http://srx.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lqd.yvedp.cn

[S22] C：字符串转数字
来源：http://vis.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://knk.jinqigufen.top

[S23] C：随机数
来源：http://rsr.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bqb.jinqigufen.top

[S24] C：获取本地时间
来源：http://swv.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://umn.andypj.xyz

[S25] C：内存拷贝
来源：http://ssb.sxryk.cn

memcpy(dst, src, n);
来源：http://vcf.bbcook.cn

[S26] C：内存清零
来源：http://txy.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://spk.ydzc1.top

[S27] C：定义常量
来源：http://ogk.ybcxt.top

const double PI = 3.14159;
来源：http://abf.chenlongwang.top

[S28] C：静态变量
来源：http://isk.xuetiantiany.cn

static int counter = 0;
来源：http://llv.xuetiantiany.cn

[S29] C：变参函数
来源：http://fne.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fbi.xuanzx.com

[S30] C：头文件保护
来源：http://ofv.pengpengdd.cyou

#ifndef X_H
来源：http://eie.yueranfly.top

#define X_H
来源：http://kzv.zhengqikj.top

#endif
来源：http://euy.meibo888.top

[S31] C++：Hello World
来源：http://nub.yuxming.cn

#include <iostream>
来源：http://cdn.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://kiq.zhiwuduotai.top

[S32] C++：字符串
来源：http://amv.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://lff.yongpay.top

[S33] C++：vector 增删
来源：http://fsz.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzw.bjfxy.top

[S34] C++：遍历 vector
来源：http://psb.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://mgs.yvedp.cn

[S35] C++：map
来源：http://gab.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://stb.iojbl.cn

[S36] C++：unordered_map
来源：http://ntu.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mpk.mhx1999.top

[S37] C++：set
来源：http://mdz.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qfe.zhongyouzk.top

[S38] C++：排序
来源：http://igt.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://zlw.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://lzr.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ktp.epnwcf.com

[S40] C++：查找元素
来源：http://wlj.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zdd.shzxlz.cn

[S41] C++：类与构造函数
来源：http://fij.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dpx.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://pib.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://ucd.hcnkem.com

[S43] C++：智能指针
来源：http://lor.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://its.mhx1999.top

[S44] C++：引用传参
来源：http://uzj.uphjek.com

void inc(int &x) { ++x; }
来源：http://ndz.yanxiufei.cn

[S45] C++：lambda
来源：http://imr.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://ksi.yj20258888.top

[S46] C++：函数模板
来源：http://mkt.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kaj.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://uvw.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eij.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://elb.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://kuh.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://jsf.haohaochexian.top

[S49] C++：写文件
来源：http://nvl.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cwo.aibaodan.cn

[S50] C++：格式化数字
来源：http://cpj.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mpa.hcnkem.com

[S51] C++：显式类型转换
来源：http://euk.sweek.top

static_cast<double>(a) / b
来源：http://xbf.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://kfm.jianghu66.top

int size() const noexcept { return n_; }
来源：http://fot.hongshengwenyu.top

[S53] C++：移动语义
来源：http://yro.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://psx.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://tbm.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ftf.zhixingplan.top

[S55] C++：结构化绑定
来源：http://awq.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lnz.bjfxy.top

[S56] C++：optional
来源：http://vep.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mdr.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://rri.tianlin.xyz

constexpr int N = 10;
来源：http://fxp.nwbrower.top

[S58] C++：命名空间
来源：http://rrx.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://cyx.zhixingplan.top

[S59] C++：静态断言
来源：http://dzm.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hsb.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://fnk.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cey.shuidangran.top

================================================================================
来源：http://xpr.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://owe.aizwys.cn

================================================================================
来源：http://gmi.xinyue.icu

[T01] Kotlin：Hello World
来源：http://mli.hysaishi.cn

println("Hello")
来源：http://mjx.jianghu66.top

[T02] Kotlin：变量
来源：http://uvw.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzw.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://cid.fehbvm.com

"值: $b"
来源：http://bkl.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://vlt.jyoumei.cn

val n: String? = null;  n?.length
来源：http://ael.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://qit.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://apz.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://rnp.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://xzk.pycfn.com

[T07] Kotlin：集合过滤
来源：http://ofb.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qwf.daria6918.cn

[T08] Kotlin：数据类
来源：http://mvz.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://wxi.meibo888.top


<!-- 参考信息 -->