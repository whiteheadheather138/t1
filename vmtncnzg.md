代发 wailian999

readonly PI=3.14
来源：http://zyt.fanxiaobao.xyz

[R04] 位置参数
来源：http://pxz.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bog.zhengqikj.top

[R05] 参数默认值
来源：http://lpq.zhiwuduotai.top

name="${1:-default}"
来源：http://fea.yvedp.cn

[R06] 判断命令是否存在
来源：http://tlt.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lez.sxryk.cn

[R07] if 判断文件
来源：http://gki.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://daw.hfpthk.cn

[R08] 数值比较
来源：http://sms.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://dte.gaohongyu789.top

[R09] 字符串比较
来源：http://frg.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gpe.xuanzx.com

[R10] 正则匹配
来源：http://pyj.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nlw.gzhubu.top

[R11] case 多分支
来源：http://mck.hcnkem.com

case "$1" in
来源：http://rkn.snrcjt.cn

start) echo "启动" ;;
来源：http://loi.xuanzx.com

stop)  echo "停止" ;;
来源：http://wgn.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://zdi.jinqigfzy.top

esac
来源：http://hjk.sysykeji.top

[R12] for 遍历文件
来源：http://fht.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://smr.yj202588.top

[R13] for 计数循环
来源：http://mta.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://jld.tarul.cn

[R14] C 风格 for
来源：http://jpn.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rva.andypj.xyz

[R15] while 逐行读文件
来源：http://bed.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ffu.cheryme.top

[R16] until 等待条件
来源：http://auo.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tmu.haohaochexian.top

[R17] 数组定义与取值
来源：http://sdk.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://rsd.havefunace.top

[R18] 遍历数组
来源：http://ltu.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://slz.kuanghao11.cn

[R19] 数组长度
来源：http://rjw.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://kga.hcnkem.com

[R20] 关联数组（字典）
来源：http://edp.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjb.dianchejie.cn

[R21] 字符串长度
来源：http://xpv.ydjk.org.cn

echo "${#s}"
来源：http://ihr.pycfn.com

[R22] 截取子串
来源：http://otk.guowangkeji.top

echo "${s:0:5}"
来源：http://fjo.redwolf501.top

[R23] 字符串替换
来源：http://giq.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://goj.tian-w.cn

[R24] 大小写转换
来源：http://vfv.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://vdd.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://qfg.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zxd.nanxinkj.top

[R26] 命令替换
来源：http://kxl.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://pgg.cheryme.top

[R27] 算术展开
来源：http://djb.tarul.cn

echo $((1 + 2 * 3))
来源：http://wyq.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://hoy.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://xfl.sjlbkw.cn

[R29] 定义函数
来源：http://xnz.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qxg.cashguo.top

[R30] 函数返回状态码
来源：http://anu.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://ckr.yangfankeji.com

[R31] 局部变量
来源：http://kux.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://whn.yueranfly.top

[R32] 参数个数校验
来源：http://bqm.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xdz.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://swk.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fjb.jqgufenzy.top

[R34] 退出时清理
来源：http://qjz.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://tbo.yj20258.top

[R35] 后台执行并等待
来源：http://lmn.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pvj.snrcjt.cn

[R36] 并发执行多个任务
来源：http://oyr.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ofe.zdbjq.cn

[R37] 把输出赋给变量
来源：http://xvp.fktsv.cn

files=$(ls -1)
来源：http://wcl.quarkkingdee.top

[R38] 管道串联
来源：http://ebk.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://qhc.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://pyt.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://pbz.fktsv.cn

[R40] 追加写日志
来源：http://zep.sufxvd.cn

echo "log" >> out.log
来源：http://lmy.ybcxt.top

[R41] 丢弃输出
来源：http://zuy.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://jtf.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://okm.tianlin.xyz

wc -l < a.txt
来源：http://fzu.xylfe.cn

[R43] 按名字查找文件
来源：http://ghj.cdnleiting.top

find . -name "*.log" -type f
来源：http://gkx.chenlongwang.top

[R44] 按修改时间查找
来源：http://swx.iojbl.cn

find . -mtime -7 -type f
来源：http://xpn.yuanzhike.top

[R45] 批量删除
来源：http://psh.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://apa.jiagoushi.top

[R46] 递归替换文件内容
来源：http://vlw.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhm.zycfv.cn

[R47] sed 单行替换
来源：http://nlb.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://ngd.ppjwa.cn

[R48] awk 取指定列
来源：http://abu.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://nfs.sufxvd.cn

[R49] awk 带条件
来源：http://qgk.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lrg.zycfv.cn

[R50] awk 求和
来源：http://zuv.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://zem.shuidangran.top

[R51] 排序去重取前几
来源：http://osn.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iwq.c1oappe.top

[R52] 统计行数
来源：http://ugt.ydjk.org.cn

wc -l a.txt
来源：http://aat.zhijiandao.cn

[R53] 查看文件头与实时尾
来源：http://qku.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://shg.vqdsnc.cn

[R54] 比较两个文件
来源：http://wjo.cheryme.top

diff a.txt b.txt
来源：http://azp.jqgfzy.top

[R55] 压缩与解压
来源：http://rbo.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pql.epnwcf.com

[R56] 远程拷贝
来源：http://afe.zhiwuduotai.top

scp file user@host:/path/
来源：http://fnz.meibo888.top

[R57] 远程执行命令
来源：http://mon.birdmap.top

ssh user@host 'uptime'
来源：http://dth.mhx1999.top

[R58] 下载文件
来源：http://sku.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hlo.pycfn.com

[R59] 发 POST JSON
来源：http://ncv.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://poi.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://nxp.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://akj.zhoulong.xyz

[R61] 磁盘占用
来源：http://xgi.hywenlv.cn

df -h;  du -sh *
来源：http://hxv.snrcjt.cn

[R62] 找最占空间的文件
来源：http://ixe.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://klo.ydjk.org.cn

[R63] 内存与进程
来源：http://vph.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://bmi.zhaomingkeji.xyz

[R64] 结束进程
来源：http://pfj.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://oza.yj20258888.top

[R65] 查看端口占用
来源：http://qrb.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gbz.yuanzhike.top

[R66] 定时任务
来源：http://yst.ivvv.top

crontab -e;  crontab -l
来源：http://and.xuanzx.com

[R67] 生成随机十六进制串
来源：http://tur.ehwqpu.com

openssl rand -hex 16
来源：http://nwh.yfazqb.com

[R68] 计算文件校验值
来源：http://rhm.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://moh.feifeiyinyue.top

[R69] 生成随机密码
来源：http://udq.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://pek.sweek.top

[R70] 时间戳与互转
来源：http://pry.cashguo.top

date +%s;  date -d @1700000000
来源：http://jcj.shangyingyoupin.top

[R71] 日期格式化
来源：http://ndh.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://apk.hcnkem.com

[R72] 等待端口就绪
来源：http://qxn.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wvc.xziqi.cn

[R73] 分割大日志
来源：http://uiv.0kj1m.cn

split -l 1000 big.log part_
来源：http://dai.cdnleiting.top

[R74] 批量重命名
来源：http://vmc.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ssj.cucudq.cn

[R75] 导出环境变量
来源：http://xis.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://vsd.yj202588.top

[R76] 使用临时文件
来源：http://dvq.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lze.jinqigufen.top

[R77] 读取用户输入
来源：http://azq.ydjk.org.cn

read -rp "请输入: " ans
来源：http://dsc.daxiang520.top

[R78] 交互式菜单
来源：http://xaf.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rdu.yfazqb.com

[R79] 解析命令行选项
来源：http://lmv.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dnc.cashguo.top

[R80] 查看脚本执行耗时
来源：http://nar.jqgufenzy.top

time ./run.sh
来源：http://umf.0kj1m.cn

================================================================================
来源：http://sxd.nanxinkj.top

S. C / C++ 专题
来源：http://jur.cdnleiting.top

================================================================================
来源：http://ovh.zdbjq.cn

[S01] C：Hello World
来源：http://sra.vqdsnc.cn

#include <stdio.h>
来源：http://ayb.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hje.nwbrower.top

[S02] C：变量与格式化输出
来源：http://oaf.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://wnz.ehwqpu.com

[S03] C：读入整数
来源：http://byr.uphjek.com

int x; scanf("%d", &x);
来源：http://sxc.dianchejie.cn

[S04] C：字符串复制
来源：http://hks.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sfp.sufxvd.cn

[S05] C：字符串长度
来源：http://yxc.shanyushiyangkeji.top

strlen(s)
来源：http://vjz.hysaishi.cn

[S06] C：字符串比较
来源：http://eoo.vehdjk.com

strcmp(a, b) == 0
来源：http://hug.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://cfl.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ktq.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://cej.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vnc.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://uys.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rhh.iojbl.cn

[S10] C：指针与解引用
来源：http://nms.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://ppx.zdbjq.cn

[S11] C：逐行读文件
来源：http://ork.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://oji.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ybx.jianghu66.top

fclose(f);
来源：http://nfs.sxryk.cn

[S12] C：写文件
来源：http://efn.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://loa.zhijiandao.cn

[S13] C：宏定义
来源：http://bib.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xqc.sweek.top

[S14] C：枚举
来源：http://dkl.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://jyu.guowangkeji.top

[S15] C：类型转换
来源：http://dey.yanxiufei.cn

(double) a / b
来源：http://yvn.shuidangran.top

[S16] C：位操作置位
来源：http://pif.shzxlz.cn

x |= (1 << 3);
来源：http://rbt.gzhubu.top

[S17] C：安全拼接字符串
来源：http://xac.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egb.zycfv.cn

[S18] C：命令行参数
来源：http://gmx.gogol.net.cn

int main(int argc, char **argv)
来源：http://tsv.andypj.xyz

[S19] C：快速排序
来源：http://hjh.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://qaf.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://tby.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://enm.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://aki.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://utn.fzhhl.top

[S22] C：字符串转数字
来源：http://hmv.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://hyb.zdqjudy.top

[S23] C：随机数
来源：http://fif.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gax.guowangkeji.top

[S24] C：获取本地时间
来源：http://pzn.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qup.tanke756.top

[S25] C：内存拷贝
来源：http://cng.cheryme.top

memcpy(dst, src, n);
来源：http://rca.svipenyu.cn

[S26] C：内存清零
来源：http://xlz.fengsongda.top

memset(a, 0, sizeof a);
来源：http://bkk.pengpengdd.cyou

[S27] C：定义常量
来源：http://afi.hammf.cn

const double PI = 3.14159;
来源：http://vpu.yj20258888.top

[S28] C：静态变量
来源：http://lmb.c1oappe.top

static int counter = 0;
来源：http://pgu.zhiwuduotai.top

[S29] C：变参函数
来源：http://iyx.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yst.zycfv.cn

[S30] C：头文件保护
来源：http://fma.daxiang520.top

#ifndef X_H
来源：http://pkf.jinyuanbaomall.cn

#define X_H
来源：http://nsm.gogol.net.cn

#endif
来源：http://fdp.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://vxp.tanke756.top

#include <iostream>
来源：http://cpj.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://rrr.fzhhl.top

[S32] C++：字符串
来源：http://qvj.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://vhi.sweek.top

[S33] C++：vector 增删
来源：http://aqv.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eyy.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://hpt.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://xlf.yangfankeji.com

[S35] C++：map
来源：http://mig.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vxk.yonumen.top

[S36] C++：unordered_map
来源：http://wsc.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://agp.yj20258888.top

[S37] C++：set
来源：http://ibu.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://crn.fehbvm.com

[S38] C++：排序
来源：http://wta.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://oci.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://ics.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hco.iojbl.cn

[S40] C++：查找元素
来源：http://ono.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pxf.iojbl.cn

[S41] C++：类与构造函数
来源：http://pse.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hgl.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://oyp.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://sau.kuanghao11.cn

[S43] C++：智能指针
来源：http://hvy.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://fjn.c1oappe.top

[S44] C++：引用传参
来源：http://rwt.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://imv.9152youxi.cn

[S45] C++：lambda
来源：http://chv.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://aca.316326.xyz

[S46] C++：函数模板
来源：http://fyo.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://clr.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://lit.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hyn.vehdjk.com

[S48] C++：逐行读文件
来源：http://hmc.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://ajm.xuanzx.com

while (std::getline(in, line)) { }
来源：http://xki.hywenlv.cn

[S49] C++：写文件
来源：http://iwm.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jov.yj20258888.top

[S50] C++：格式化数字
来源：http://xkd.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sft.xylfe.cn

[S51] C++：显式类型转换
来源：http://wvf.jinqigufen.top

static_cast<double>(a) / b
来源：http://nfi.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://hge.ivvv.top

int size() const noexcept { return n_; }
来源：http://yax.yvedp.cn

[S53] C++：移动语义
来源：http://hsm.birdmap.top

std::vector<int> w = std::move(v);
来源：http://rye.chenzaomai.com

[S54] C++：异常处理
来源：http://ana.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mdq.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://bqe.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jhm.jlsjyb.cn

[S56] C++：optional
来源：http://yqt.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gaz.ehwqpu.com

[S57] C++：编译期常量
来源：http://xrv.daxiang520.top

constexpr int N = 10;
来源：http://men.bjfxy.top

[S58] C++：命名空间
来源：http://gdo.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://ywt.52xcode.cn

[S59] C++：静态断言
来源：http://qkr.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://puf.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://aqb.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mso.sweek.top

================================================================================
来源：http://cuj.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zvy.fehbvm.com

================================================================================
来源：http://vak.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://hfr.chenzaomai.com

println("Hello")
来源：http://pgl.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://ahx.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ktg.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://ggk.shuidangran.top

"值: $b"
来源：http://lqx.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://gvl.snrcjt.cn

val n: String? = null;  n?.length
来源：http://fxi.ybcxt.top


<!-- 参考信息 -->