代发 wailian999

name="${1:-default}"
来源：http://sfx.jyoumei.cn

[R06] 判断命令是否存在
来源：http://vbu.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rfw.nanxinkj.top

[R07] if 判断文件
来源：http://ssv.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zyu.dashuyun.cn

[R08] 数值比较
来源：http://bqj.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://lqn.zhixingplan.top

[R09] 字符串比较
来源：http://xcs.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vct.birdmap.top

[R10] 正则匹配
来源：http://ahp.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bvq.zhiwuduotai.top

[R11] case 多分支
来源：http://sbe.fanxiaobao.xyz

case "$1" in
来源：http://wkd.zdqjudy.top

start) echo "启动" ;;
来源：http://trh.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://xkc.yj202588.top

*)     echo "未知命令" ;;
来源：http://xbg.cqqwz.cn

esac
来源：http://nlw.sufxvd.cn

[R12] for 遍历文件
来源：http://wcx.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://jwq.9152youxi.cn

[R13] for 计数循环
来源：http://shn.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://bod.mhx1999.top

[R14] C 风格 for
来源：http://xbn.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ads.gogol.net.cn

[R15] while 逐行读文件
来源：http://qzw.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rbg.hnqzz.top

[R16] until 等待条件
来源：http://cip.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xpk.ehwqpu.com

[R17] 数组定义与取值
来源：http://fls.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://lup.vqdsnc.cn

[R18] 遍历数组
来源：http://quo.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fkj.shangyingyoupin.top

[R19] 数组长度
来源：http://acv.ybcxt.top

echo "${#arr[@]}"
来源：http://nar.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://fiv.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qdo.zhijiandao.cn

[R21] 字符串长度
来源：http://mmz.zhaomingkeji.xyz

echo "${#s}"
来源：http://sfs.xuetiantiany.cn

[R22] 截取子串
来源：http://vhg.redwolf501.top

echo "${s:0:5}"
来源：http://kus.xylfe.cn

[R23] 字符串替换
来源：http://znu.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wpz.jlsjyb.cn

[R24] 大小写转换
来源：http://gaw.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://cke.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://ywd.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lby.jiagoushi.top

[R26] 命令替换
来源：http://gem.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://atp.fehbvm.com

[R27] 算术展开
来源：http://ned.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://cud.wangdashe.top

[R28] 浮点运算
来源：http://cun.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://jhv.jqgufenzy.top

[R29] 定义函数
来源：http://mgd.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nwa.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://kvn.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://ljh.hcnkem.com

[R31] 局部变量
来源：http://xlv.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://nhr.aizwys.cn

[R32] 参数个数校验
来源：http://lov.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nei.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://nli.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jou.hnxiangtu.top

[R34] 退出时清理
来源：http://krd.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://arh.zdbjq.cn

[R35] 后台执行并等待
来源：http://qzs.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bqb.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://mcb.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nui.yonumen.top

[R37] 把输出赋给变量
来源：http://gve.fktsv.cn

files=$(ls -1)
来源：http://lxu.yfazqb.com

[R38] 管道串联
来源：http://mbg.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://xys.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://auh.vqdsnc.cn

cmd > out.log 2>&1
来源：http://ppo.dashuyun.cn

[R40] 追加写日志
来源：http://xxo.shuidangran.top

echo "log" >> out.log
来源：http://gap.ydjk.org.cn

[R41] 丢弃输出
来源：http://mwr.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://xir.jiagoushi.top

[R42] 输入重定向
来源：http://ogu.hesvh.cn

wc -l < a.txt
来源：http://lab.tian-w.cn

[R43] 按名字查找文件
来源：http://unc.chenlongwang.top

find . -name "*.log" -type f
来源：http://yge.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://rbu.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://kdx.kuanghao11.cn

[R45] 批量删除
来源：http://izc.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://xvb.yangfankeji.com

[R46] 递归替换文件内容
来源：http://dmz.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oni.xuetiantiany.cn

[R47] sed 单行替换
来源：http://hft.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eou.daxiang520.top

[R48] awk 取指定列
来源：http://rfw.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://ria.chenzaomai.com

[R49] awk 带条件
来源：http://ajm.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kgm.fengsongda.top

[R50] awk 求和
来源：http://fyr.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://lpz.andypj.xyz

[R51] 排序去重取前几
来源：http://bsb.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qif.ywan-chungtsiang.top

[R52] 统计行数
来源：http://pzd.birdmap.top

wc -l a.txt
来源：http://qxx.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://uhb.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lap.yueranfly.top

[R54] 比较两个文件
来源：http://nue.zhiwuduotai.top

diff a.txt b.txt
来源：http://rfy.jyoumei.cn

[R55] 压缩与解压
来源：http://gio.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mgg.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://aed.bbcook.cn

scp file user@host:/path/
来源：http://uyy.dashuyun.cn

[R57] 远程执行命令
来源：http://zxj.svipenyu.cn

ssh user@host 'uptime'
来源：http://fbk.wangshuangyany.cn

[R58] 下载文件
来源：http://mqj.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mbh.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://nfd.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zqu.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://qtn.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pxu.sxryk.cn

[R61] 磁盘占用
来源：http://fmp.chenlongwang.top

df -h;  du -sh *
来源：http://zto.vehdjk.com

[R62] 找最占空间的文件
来源：http://era.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://uee.sysykeji.top

[R63] 内存与进程
来源：http://cgf.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://dqj.52xcode.cn

[R64] 结束进程
来源：http://gzi.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://psz.zhixingplan.top

[R65] 查看端口占用
来源：http://yhb.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ply.ybcxt.top

[R66] 定时任务
来源：http://qpv.jinqigfzy.top

crontab -e;  crontab -l
来源：http://bqk.xuanzx.com

[R67] 生成随机十六进制串
来源：http://ydk.xinyue.icu

openssl rand -hex 16
来源：http://llv.zhongyouzk.top

[R68] 计算文件校验值
来源：http://onf.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://ayo.tianlin.xyz

[R69] 生成随机密码
来源：http://coa.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://idi.zhixingplan.top

[R70] 时间戳与互转
来源：http://pfm.havefunace.top

date +%s;  date -d @1700000000
来源：http://kur.snrcjt.cn

[R71] 日期格式化
来源：http://aek.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://egn.gaohongyu789.top

[R72] 等待端口就绪
来源：http://tzr.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://atd.yj202588.top

[R73] 分割大日志
来源：http://lov.tian-w.cn

split -l 1000 big.log part_
来源：http://oud.zhiwuduotai.top

[R74] 批量重命名
来源：http://czq.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yey.zhixingplan.top

[R75] 导出环境变量
来源：http://dun.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://gqk.zdqjudy.top

[R76] 使用临时文件
来源：http://qau.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bog.jqgufenzy.top

[R77] 读取用户输入
来源：http://axi.tarul.cn

read -rp "请输入: " ans
来源：http://zvc.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://mqm.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://iwa.haohaochexian.top

[R79] 解析命令行选项
来源：http://ojg.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ude.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://lpv.fzhhl.top

time ./run.sh
来源：http://hrf.xziqi.cn

================================================================================
来源：http://wmi.guannengcc.top

S. C / C++ 专题
来源：http://lkq.dashuyun.cn

================================================================================
来源：http://uxv.guannengcc.top

[S01] C：Hello World
来源：http://gbd.tarul.cn

#include <stdio.h>
来源：http://yaf.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xkg.daria6918.cn

[S02] C：变量与格式化输出
来源：http://mje.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://ttt.zhijiandao.cn

[S03] C：读入整数
来源：http://qok.xziqi.cn

int x; scanf("%d", &x);
来源：http://mhz.fzhhl.top

[S04] C：字符串复制
来源：http://dcw.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oet.yj20258.top

[S05] C：字符串长度
来源：http://bzr.iojbl.cn

strlen(s)
来源：http://mki.sjlbkw.cn

[S06] C：字符串比较
来源：http://hsr.guowangkeji.top

strcmp(a, b) == 0
来源：http://lbj.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://faq.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ohg.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://afm.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fad.yj20258.top

[S09] C：结构体定义与初始化
来源：http://vij.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rmp.jiagoushi.top

[S10] C：指针与解引用
来源：http://zbb.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://noq.epnwcf.com

[S11] C：逐行读文件
来源：http://qyz.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://csp.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gru.fzhhl.top

fclose(f);
来源：http://qkt.zhixingplan.top

[S12] C：写文件
来源：http://elm.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nru.bjfxy.top

[S13] C：宏定义
来源：http://ppq.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qky.hammf.cn

[S14] C：枚举
来源：http://eua.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://dhq.chenjidiqi.icu

[S15] C：类型转换
来源：http://vwq.fzhhl.top

(double) a / b
来源：http://bjz.pycfn.com

[S16] C：位操作置位
来源：http://pnt.yongpay.top

x |= (1 << 3);
来源：http://euf.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://kct.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqi.jianghu66.top

[S18] C：命令行参数
来源：http://uzm.guannengcc.top

int main(int argc, char **argv)
来源：http://oia.gogol.net.cn

[S19] C：快速排序
来源：http://prx.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://hyp.yanxiufei.cn

[S20] C：二分查找
来源：http://vjg.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vfd.haohaochexian.top

[S21] C：字符类别判断
来源：http://hio.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fns.ehwqpu.com

[S22] C：字符串转数字
来源：http://lcw.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hwz.fengsongda.top

[S23] C：随机数
来源：http://uxj.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://swt.sjlbkw.cn

[S24] C：获取本地时间
来源：http://ktc.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://luy.tianlin.xyz

[S25] C：内存拷贝
来源：http://dzs.yueranfly.top

memcpy(dst, src, n);
来源：http://raz.chenzaomai.com

[S26] C：内存清零
来源：http://jym.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://hey.hesvh.cn

[S27] C：定义常量
来源：http://iwz.ivvv.top

const double PI = 3.14159;
来源：http://wbn.gaohongyu789.top

[S28] C：静态变量
来源：http://rro.hongshengwenyu.top

static int counter = 0;
来源：http://wrd.andypj.xyz

[S29] C：变参函数
来源：http://njw.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://abb.zhiwuduotai.top

[S30] C：头文件保护
来源：http://rap.ywan-chungtsiang.top

#ifndef X_H
来源：http://gzb.yuxming.cn

#define X_H
来源：http://nav.aibaodan.cn

#endif
来源：http://xcp.hnqzz.top

[S31] C++：Hello World
来源：http://fwh.shangyingyoupin.top

#include <iostream>
来源：http://pio.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://mfp.yj20258.top

[S32] C++：字符串
来源：http://lnr.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://pqd.daria6918.cn

[S33] C++：vector 增删
来源：http://ojg.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xvn.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://oio.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://dql.ybcxt.top

[S35] C++：map
来源：http://oyi.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mux.hysaishi.cn

[S36] C++：unordered_map
来源：http://dzi.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://stq.chenzaomai.com

[S37] C++：set
来源：http://nmc.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eeh.iojbl.cn

[S38] C++：排序
来源：http://htx.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ejo.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://qzd.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://odu.sweek.top

[S40] C++：查找元素
来源：http://xmk.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://brk.yuxming.cn

[S41] C++：类与构造函数
来源：http://ltb.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ksg.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://mld.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://cwd.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://gpi.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://fvp.zhijiandao.cn

[S44] C++：引用传参
来源：http://ubl.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://wao.aibaodan.cn

[S45] C++：lambda
来源：http://ceg.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nan.sysykeji.top

[S46] C++：函数模板
来源：http://kqh.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://utm.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://kii.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://flg.svipenyu.cn

[S48] C++：逐行读文件
来源：http://eik.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://dpy.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://lrf.yj20258.top

[S49] C++：写文件
来源：http://juq.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fll.daxiang520.top

[S50] C++：格式化数字
来源：http://ssy.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nei.yuanzhike.top

[S51] C++：显式类型转换
来源：http://tfe.yuxming.cn

static_cast<double>(a) / b
来源：http://cjx.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://syi.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://ngp.hfpthk.cn

[S53] C++：移动语义
来源：http://zqv.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://olj.feifeiyinyue.top

[S54] C++：异常处理
来源：http://fqk.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fsf.dianchejie.cn

[S55] C++：结构化绑定
来源：http://wtd.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ymt.yongpay.top

[S56] C++：optional
来源：http://xrl.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xyh.cheryme.top

[S57] C++：编译期常量
来源：http://nyw.shangyingyoupin.top

constexpr int N = 10;
来源：http://xer.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://htt.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://hpx.chenlongwang.top

[S59] C++：静态断言
来源：http://dnd.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vjd.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://xyj.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sop.hnqzz.top

================================================================================
来源：http://jgs.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sfd.cqqwz.cn

================================================================================
来源：http://wmr.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://zpe.redwolf501.top

println("Hello")
来源：http://ylw.zhoulong.xyz

[T02] Kotlin：变量
来源：http://eeq.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qhj.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://jvp.cucudq.cn

"值: $b"
来源：http://ucw.ctjpmb.com

[T04] Kotlin：空安全
来源：http://zmm.snrcjt.cn

val n: String? = null;  n?.length
来源：http://bsn.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://qit.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vno.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://kxc.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hoh.c1oappe.top


<!-- 参考信息 -->