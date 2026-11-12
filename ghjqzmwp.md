代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fst.hnxiangtu.top

[R08] 数值比较
来源：http://xsy.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uux.dashuyun.cn

[R09] 字符串比较
来源：http://jti.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kme.xuetiantiany.cn

[R10] 正则匹配
来源：http://lvw.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dhh.yangfankeji.com

[R11] case 多分支
来源：http://gpg.cashguo.top

case "$1" in
来源：http://olk.pengpengdd.cyou

start) echo "启动" ;;
来源：http://fpw.yongpay.top

stop)  echo "停止" ;;
来源：http://cea.ivvv.top

*)     echo "未知命令" ;;
来源：http://maj.xziqi.cn

esac
来源：http://tyc.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://ufr.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://gso.zhiwuduotai.top

[R13] for 计数循环
来源：http://nyl.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://syq.jyoumei.cn

[R14] C 风格 for
来源：http://jzb.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ata.yongpay.top

[R15] while 逐行读文件
来源：http://smf.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mvt.jqgfzy.top

[R16] until 等待条件
来源：http://fkc.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ugk.hysaishi.cn

[R17] 数组定义与取值
来源：http://nxi.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://klm.yvedp.cn

[R18] 遍历数组
来源：http://zto.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jjd.aizwys.cn

[R19] 数组长度
来源：http://qzh.nanxinkj.top

echo "${#arr[@]}"
来源：http://jph.hammf.cn

[R20] 关联数组（字典）
来源：http://agz.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uka.bbcook.cn

[R21] 字符串长度
来源：http://nqg.9152youxi.cn

echo "${#s}"
来源：http://obs.vehdjk.com

[R22] 截取子串
来源：http://nuj.gotoacloud.top

echo "${s:0:5}"
来源：http://min.gaohongyu789.top

[R23] 字符串替换
来源：http://lum.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lpd.316326.xyz

[R24] 大小写转换
来源：http://jao.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://gzv.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://syt.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jrb.zhengqikj.top

[R26] 命令替换
来源：http://irq.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://mxx.zycfv.cn

[R27] 算术展开
来源：http://oto.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://cck.yfazqb.com

[R28] 浮点运算
来源：http://aew.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://zps.daxiang520.top

[R29] 定义函数
来源：http://npp.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qzq.xylfe.cn

[R30] 函数返回状态码
来源：http://zsx.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://onz.birdmap.top

[R31] 局部变量
来源：http://auv.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://jbo.cqqwz.cn

[R32] 参数个数校验
来源：http://cde.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://znl.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://awp.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://css.tianlin.xyz

[R34] 退出时清理
来源：http://pql.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://woe.ctjpmb.com

[R35] 后台执行并等待
来源：http://jwf.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rdl.vehdjk.com

[R36] 并发执行多个任务
来源：http://sgv.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://spp.chenlongwang.top

[R37] 把输出赋给变量
来源：http://wiz.hysaishi.cn

files=$(ls -1)
来源：http://xxv.tarul.cn

[R38] 管道串联
来源：http://ili.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://auu.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://zre.ybcxt.top

cmd > out.log 2>&1
来源：http://hdw.yj20258.top

[R40] 追加写日志
来源：http://ofh.uphjek.com

echo "log" >> out.log
来源：http://ogs.yj202588.top

[R41] 丢弃输出
来源：http://fwp.epnwcf.com

cmd >/dev/null 2>&1
来源：http://xjz.guannengcc.top

[R42] 输入重定向
来源：http://ndq.sjlbkw.cn

wc -l < a.txt
来源：http://xqh.zhoulong.xyz

[R43] 按名字查找文件
来源：http://fqc.sweek.top

find . -name "*.log" -type f
来源：http://pjn.smart0.xyz

[R44] 按修改时间查找
来源：http://jvq.guowangkeji.top

find . -mtime -7 -type f
来源：http://yxy.dianchejie.cn

[R45] 批量删除
来源：http://owi.52xcode.cn

find . -name "*.tmp" -delete
来源：http://tix.gogol.net.cn

[R46] 递归替换文件内容
来源：http://zbu.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mrn.sweek.top

[R47] sed 单行替换
来源：http://alj.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ljs.yuxming.cn

[R48] awk 取指定列
来源：http://rip.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://yvu.bbcook.cn

[R49] awk 带条件
来源：http://ltl.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvm.nwbrower.top

[R50] awk 求和
来源：http://ijs.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://tvt.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://tbg.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pbs.redwolf501.top

[R52] 统计行数
来源：http://quo.hfpthk.cn

wc -l a.txt
来源：http://lvl.yj20258.top

[R53] 查看文件头与实时尾
来源：http://bxa.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bgf.wangdashe.top

[R54] 比较两个文件
来源：http://ypw.gotoacloud.top

diff a.txt b.txt
来源：http://vuj.yuxming.cn

[R55] 压缩与解压
来源：http://eth.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://phk.jiagoushi.top

[R56] 远程拷贝
来源：http://wjx.yanxiufei.cn

scp file user@host:/path/
来源：http://zab.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://uih.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://zue.316326.xyz

[R58] 下载文件
来源：http://vag.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfi.fehbvm.com

[R59] 发 POST JSON
来源：http://fgx.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fvi.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://sir.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dyu.smart0.xyz

[R61] 磁盘占用
来源：http://epq.fengsongda.top

df -h;  du -sh *
来源：http://wkb.dashuyun.cn

[R62] 找最占空间的文件
来源：http://heh.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://jxi.jyoumei.cn

[R63] 内存与进程
来源：http://nen.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://xdp.quarkkingdee.top

[R64] 结束进程
来源：http://btm.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://bci.hywenlv.cn

[R65] 查看端口占用
来源：http://btx.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rfk.wangshuangyany.cn

[R66] 定时任务
来源：http://rkz.gotoacloud.top

crontab -e;  crontab -l
来源：http://ftl.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://zsx.jinqigufen.top

openssl rand -hex 16
来源：http://mty.dashuyun.cn

[R68] 计算文件校验值
来源：http://cdc.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://fam.aizwys.cn

[R69] 生成随机密码
来源：http://bvd.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://jpm.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://poq.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://cku.pengpengdd.cyou

[R71] 日期格式化
来源：http://whw.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ytk.hcnkem.com

[R72] 等待端口就绪
来源：http://hra.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nbu.zdqjudy.top

[R73] 分割大日志
来源：http://znn.uphjek.com

split -l 1000 big.log part_
来源：http://elu.cucudq.cn

[R74] 批量重命名
来源：http://rgd.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://azb.bjfxy.top

[R75] 导出环境变量
来源：http://sfe.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://ycy.jinqigfzy.top

[R76] 使用临时文件
来源：http://hzr.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hgd.sysykeji.top

[R77] 读取用户输入
来源：http://pgd.yj20258888.top

read -rp "请输入: " ans
来源：http://fhl.ppjwa.cn

[R78] 交互式菜单
来源：http://ncb.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ycf.nanxinkj.top

[R79] 解析命令行选项
来源：http://hte.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oap.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://fmk.feifeiyinyue.top

time ./run.sh
来源：http://lev.zdbjq.cn

================================================================================
来源：http://uzq.yfazqb.com

S. C / C++ 专题
来源：http://cge.cucudq.cn

================================================================================
来源：http://dfj.zhijiandao.cn

[S01] C：Hello World
来源：http://qcx.bjfxy.top

#include <stdio.h>
来源：http://ado.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xju.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://mej.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://sls.cucudq.cn

[S03] C：读入整数
来源：http://pyj.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://mnz.vehdjk.com

[S04] C：字符串复制
来源：http://nzb.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://mgc.yj20258888.top

[S05] C：字符串长度
来源：http://jzf.guowangkeji.top

strlen(s)
来源：http://kkj.zhongyouzk.top

[S06] C：字符串比较
来源：http://ehz.hysaishi.cn

strcmp(a, b) == 0
来源：http://fzr.jianghu66.top

[S07] C：数组遍历求和
来源：http://amj.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tfz.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://rsi.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kjr.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://dqo.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kue.andypj.xyz

[S10] C：指针与解引用
来源：http://oif.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://jpn.zhijiandao.cn

[S11] C：逐行读文件
来源：http://poi.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://hre.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qae.ivvv.top

fclose(f);
来源：http://fyz.tarul.cn

[S12] C：写文件
来源：http://jtn.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lnx.haohaochexian.top

[S13] C：宏定义
来源：http://kga.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://amr.sysykeji.top

[S14] C：枚举
来源：http://mkr.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://our.gogol.net.cn

[S15] C：类型转换
来源：http://lhy.yonumen.top

(double) a / b
来源：http://owp.sysykeji.top

[S16] C：位操作置位
来源：http://pdl.tianlin.xyz

x |= (1 << 3);
来源：http://igh.uphjek.com

[S17] C：安全拼接字符串
来源：http://yje.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yhs.yfazqb.com

[S18] C：命令行参数
来源：http://zwu.sxryk.cn

int main(int argc, char **argv)
来源：http://lse.c1oappe.top

[S19] C：快速排序
来源：http://bym.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://kza.sufxvd.cn

[S20] C：二分查找
来源：http://hwz.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tbl.fengsongda.top

[S21] C：字符类别判断
来源：http://rwy.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tvz.gogol.net.cn

[S22] C：字符串转数字
来源：http://clt.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wmk.aizwys.cn

[S23] C：随机数
来源：http://rpy.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mii.ydjk.org.cn

[S24] C：获取本地时间
来源：http://gwp.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jye.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://laz.yonumen.top

memcpy(dst, src, n);
来源：http://paq.hywenlv.cn

[S26] C：内存清零
来源：http://eur.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://mee.redwolf501.top

[S27] C：定义常量
来源：http://hyh.tanke756.top

const double PI = 3.14159;
来源：http://ojp.c1oappe.top

[S28] C：静态变量
来源：http://wmq.cashguo.top

static int counter = 0;
来源：http://tsz.tanke756.top

[S29] C：变参函数
来源：http://mus.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yir.hfpthk.cn

[S30] C：头文件保护
来源：http://gqs.sufxvd.cn

#ifndef X_H
来源：http://rej.shzxlz.cn

#define X_H
来源：http://lcc.hfpthk.cn

#endif
来源：http://gpw.yvedp.cn

[S31] C++：Hello World
来源：http://rgw.ctjpmb.com

#include <iostream>
来源：http://rmx.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://sbk.hesvh.cn

[S32] C++：字符串
来源：http://kda.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://jhd.sxryk.cn

[S33] C++：vector 增删
来源：http://kio.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wej.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://jhc.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://gsi.hesvh.cn

[S35] C++：map
来源：http://pmh.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://glr.zhongyouzk.top

[S36] C++：unordered_map
来源：http://sfp.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ukj.quarkkingdee.top

[S37] C++：set
来源：http://bms.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nro.c1oappe.top

[S38] C++：排序
来源：http://bge.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://kjs.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://yhp.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcd.snrcjt.cn

[S40] C++：查找元素
来源：http://aun.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rhi.tarul.cn

[S41] C++：类与构造函数
来源：http://sfu.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fsg.wangdashe.top

[S42] C++：继承与虚函数
来源：http://mlh.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://igk.wangdashe.top

[S43] C++：智能指针
来源：http://tmk.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://hrk.jyoumei.cn

[S44] C++：引用传参
来源：http://utm.yueranfly.top

void inc(int &x) { ++x; }
来源：http://pxn.hammf.cn

[S45] C++：lambda
来源：http://jtq.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://plc.sweek.top

[S46] C++：函数模板
来源：http://yrx.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bqj.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://bal.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqw.xziqi.cn

[S48] C++：逐行读文件
来源：http://roj.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://igw.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://dpa.fanxiaobao.xyz

[S49] C++：写文件
来源：http://kzn.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dom.iojbl.cn

[S50] C++：格式化数字
来源：http://dmr.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wab.52xcode.cn

[S51] C++：显式类型转换
来源：http://zrv.jinqigufen.top

static_cast<double>(a) / b
来源：http://arb.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://nxw.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://kuu.yangfankeji.com

[S53] C++：移动语义
来源：http://ivw.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://ihf.hesvh.cn

[S54] C++：异常处理
来源：http://lcd.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pja.shuidangran.top

[S55] C++：结构化绑定
来源：http://wtw.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zkm.chenlongwang.top

[S56] C++：optional
来源：http://hqx.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sjo.zdbjq.cn

[S57] C++：编译期常量
来源：http://lzj.yanxiufei.cn

constexpr int N = 10;
来源：http://gdm.ctjpmb.com

[S58] C++：命名空间
来源：http://exv.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://ybx.zhengqikj.top

[S59] C++：静态断言
来源：http://ats.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jfx.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://drs.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nzp.sxryk.cn

================================================================================
来源：http://sfd.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ldw.dashuyun.cn

================================================================================
来源：http://cgj.shuidangran.top

[T01] Kotlin：Hello World
来源：http://qjz.ybcxt.top

println("Hello")
来源：http://wbi.yfazqb.com

[T02] Kotlin：变量
来源：http://pmx.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xdk.tarul.cn

[T03] Kotlin：字符串模板
来源：http://nuu.zhiwuduotai.top

"值: $b"
来源：http://hgj.zhengqikj.top

[T04] Kotlin：空安全
来源：http://mmi.zhengqikj.top

val n: String? = null;  n?.length
来源：http://wtb.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://yys.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lqf.fktsv.cn

[T06] Kotlin：集合映射
来源：http://anv.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://yik.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://iog.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uil.tian-w.cn

[T08] Kotlin：数据类
来源：http://ywx.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://tyr.sweek.top


<!-- 参考信息 -->