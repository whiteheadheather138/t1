代发 wailian999

readonly PI=3.14
来源：http://aly.cdnleiting.top

[R04] 位置参数
来源：http://qmz.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zhj.xziqi.cn

[R05] 参数默认值
来源：http://pei.gaohongyu789.top

name="${1:-default}"
来源：http://dij.jianghu66.top

[R06] 判断命令是否存在
来源：http://bja.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cso.nanxinkj.top

[R07] if 判断文件
来源：http://hkh.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sfc.hnqzz.top

[R08] 数值比较
来源：http://adw.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rkz.pengpengdd.cyou

[R09] 字符串比较
来源：http://okk.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ktb.tian-w.cn

[R10] 正则匹配
来源：http://gnv.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ahs.meibo888.top

[R11] case 多分支
来源：http://orp.52xcode.cn

case "$1" in
来源：http://zwy.jqgufenzy.top

start) echo "启动" ;;
来源：http://olm.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://jnc.zycfv.cn

*)     echo "未知命令" ;;
来源：http://xtc.feifeiyinyue.top

esac
来源：http://tzn.sxryk.cn

[R12] for 遍历文件
来源：http://buc.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://qtl.snrcjt.cn

[R13] for 计数循环
来源：http://vel.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://jnt.316326.xyz

[R14] C 风格 for
来源：http://gtp.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hub.daxiang520.top

[R15] while 逐行读文件
来源：http://brl.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ybj.hesvh.cn

[R16] until 等待条件
来源：http://bsm.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://giq.yfazqb.com

[R17] 数组定义与取值
来源：http://alc.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jkc.gzhubu.top

[R18] 遍历数组
来源：http://pfd.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dqt.tian-w.cn

[R19] 数组长度
来源：http://aht.sweek.top

echo "${#arr[@]}"
来源：http://bac.ctjpmb.com

[R20] 关联数组（字典）
来源：http://tjs.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xmc.yongpay.top

[R21] 字符串长度
来源：http://irc.shzxlz.cn

echo "${#s}"
来源：http://mux.yueranfly.top

[R22] 截取子串
来源：http://htk.zhengqikj.top

echo "${s:0:5}"
来源：http://toa.gotoacloud.top

[R23] 字符串替换
来源：http://tzp.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tuy.tian-w.cn

[R24] 大小写转换
来源：http://wvr.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://gzu.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://lvz.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ujp.chenlongwang.top

[R26] 命令替换
来源：http://rgm.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://cqz.yueranfly.top

[R27] 算术展开
来源：http://hkj.yj202588.top

echo $((1 + 2 * 3))
来源：http://dyk.pengpengdd.cyou

[R28] 浮点运算
来源：http://uww.bjfxy.top

echo "scale=2; 10/3" | bc
来源：http://lcv.yvedp.cn

[R29] 定义函数
来源：http://akh.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uqk.zdqjudy.top

[R30] 函数返回状态码
来源：http://gmi.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://kkk.jqgfzy.top

[R31] 局部变量
来源：http://guk.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://ujw.wangshuangyany.cn

[R32] 参数个数校验
来源：http://yqo.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wtl.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://zyk.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ghf.zhixingplan.top

[R34] 退出时清理
来源：http://mco.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://kyw.yuanzhike.top

[R35] 后台执行并等待
来源：http://etd.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tki.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://zcs.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hoq.haohaochexian.top

[R37] 把输出赋给变量
来源：http://jqf.52xcode.cn

files=$(ls -1)
来源：http://jse.yuxming.cn

[R38] 管道串联
来源：http://kqk.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://qog.cashguo.top

[R39] 重定向标准输出与错误
来源：http://eek.bbcook.cn

cmd > out.log 2>&1
来源：http://tpq.yuanzhike.top

[R40] 追加写日志
来源：http://hgq.0kj1m.cn

echo "log" >> out.log
来源：http://ngw.ivvv.top

[R41] 丢弃输出
来源：http://aof.yonumen.top

cmd >/dev/null 2>&1
来源：http://jsf.xuetiantiany.cn

[R42] 输入重定向
来源：http://sus.vqdsnc.cn

wc -l < a.txt
来源：http://uhg.tanke756.top

[R43] 按名字查找文件
来源：http://pin.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://gsn.birdmap.top

[R44] 按修改时间查找
来源：http://fxb.fzhhl.top

find . -mtime -7 -type f
来源：http://phg.hnqzz.top

[R45] 批量删除
来源：http://jjo.wangdashe.top

find . -name "*.tmp" -delete
来源：http://ovr.zycfv.cn

[R46] 递归替换文件内容
来源：http://bwr.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jwu.0kj1m.cn

[R47] sed 单行替换
来源：http://fkl.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://afu.zdbjq.cn

[R48] awk 取指定列
来源：http://zdk.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://sha.9152youxi.cn

[R49] awk 带条件
来源：http://afs.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rui.redwolf501.top

[R50] awk 求和
来源：http://svo.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ybo.hesvh.cn

[R51] 排序去重取前几
来源：http://bia.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wrt.daria6918.cn

[R52] 统计行数
来源：http://xop.xylfe.cn

wc -l a.txt
来源：http://ilb.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://fkt.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ptj.aibaodan.cn

[R54] 比较两个文件
来源：http://wyi.birdmap.top

diff a.txt b.txt
来源：http://lkb.ctjpmb.com

[R55] 压缩与解压
来源：http://bwp.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lpy.ydjk.org.cn

[R56] 远程拷贝
来源：http://twk.zhengqikj.top

scp file user@host:/path/
来源：http://iwu.epnwcf.com

[R57] 远程执行命令
来源：http://nau.snrcjt.cn

ssh user@host 'uptime'
来源：http://rgu.gogol.net.cn

[R58] 下载文件
来源：http://jdr.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oyw.gogol.net.cn

[R59] 发 POST JSON
来源：http://wbb.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gbn.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://epm.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wsu.yj202588.top

[R61] 磁盘占用
来源：http://wva.wangshuangyany.cn

df -h;  du -sh *
来源：http://lid.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://ktb.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://afb.birdmap.top

[R63] 内存与进程
来源：http://cqw.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://ufl.hysaishi.cn

[R64] 结束进程
来源：http://mkf.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://kpe.52xcode.cn

[R65] 查看端口占用
来源：http://ozr.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oki.cqqwz.cn

[R66] 定时任务
来源：http://lez.meibo888.top

crontab -e;  crontab -l
来源：http://zdx.havefunace.top

[R67] 生成随机十六进制串
来源：http://zwr.tian-w.cn

openssl rand -hex 16
来源：http://ntk.ydjk.org.cn

[R68] 计算文件校验值
来源：http://qsm.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://tvv.chenjidiqi.icu

[R69] 生成随机密码
来源：http://bmk.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://fwg.haohaochexian.top

[R70] 时间戳与互转
来源：http://ghr.redwolf501.top

date +%s;  date -d @1700000000
来源：http://phj.nanxinkj.top

[R71] 日期格式化
来源：http://cuv.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pyf.ctjpmb.com

[R72] 等待端口就绪
来源：http://ony.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://whp.nanxuanxn.top

[R73] 分割大日志
来源：http://gva.vqdsnc.cn

split -l 1000 big.log part_
来源：http://oce.hcnkem.com

[R74] 批量重命名
来源：http://iym.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://geb.yj20258.top

[R75] 导出环境变量
来源：http://qlp.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://fkz.jqgufenzy.top

[R76] 使用临时文件
来源：http://ilt.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://znj.iojbl.cn

[R77] 读取用户输入
来源：http://gpn.jinqigfzy.top

read -rp "请输入: " ans
来源：http://feg.guowangkeji.top

[R78] 交互式菜单
来源：http://bsw.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://guk.iojbl.cn

[R79] 解析命令行选项
来源：http://jlg.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xlx.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://jgw.epnwcf.com

time ./run.sh
来源：http://ogi.zhongyouzk.top

================================================================================
来源：http://kij.yuanzhike.top

S. C / C++ 专题
来源：http://jpk.fengsongda.top

================================================================================
来源：http://epf.gogol.net.cn

[S01] C：Hello World
来源：http://elu.fktsv.cn

#include <stdio.h>
来源：http://sbz.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hin.316326.xyz

[S02] C：变量与格式化输出
来源：http://xmc.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://uzz.cqqwz.cn

[S03] C：读入整数
来源：http://zza.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://tco.jianghu66.top

[S04] C：字符串复制
来源：http://rcu.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://yxb.jinqigufen.top

[S05] C：字符串长度
来源：http://fyu.cqqwz.cn

strlen(s)
来源：http://doo.yonumen.top

[S06] C：字符串比较
来源：http://zgv.guowangkeji.top

strcmp(a, b) == 0
来源：http://ddg.jqgfzy.top

[S07] C：数组遍历求和
来源：http://daz.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ird.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://coe.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cxe.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://ctf.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://irg.fktsv.cn

[S10] C：指针与解引用
来源：http://nyc.xuanzx.com

int *p = &a;  *p = 5;
来源：http://dpq.gotoacloud.top

[S11] C：逐行读文件
来源：http://guc.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://lmt.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://fbg.9152youxi.cn

fclose(f);
来源：http://xcz.yj202588.top

[S12] C：写文件
来源：http://wdl.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uee.zdqjudy.top

[S13] C：宏定义
来源：http://dpv.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxr.ppjwa.cn

[S14] C：枚举
来源：http://xjm.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://zyx.uphjek.com

[S15] C：类型转换
来源：http://eoa.bbcook.cn

(double) a / b
来源：http://qlh.wangdashe.top

[S16] C：位操作置位
来源：http://kio.pycfn.com

x |= (1 << 3);
来源：http://tbr.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://oyn.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qfy.mhx1999.top

[S18] C：命令行参数
来源：http://qxp.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://olt.epnwcf.com

[S19] C：快速排序
来源：http://cct.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://kuc.sufxvd.cn

[S20] C：二分查找
来源：http://her.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vot.cdnleiting.top

[S21] C：字符类别判断
来源：http://utb.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvz.yongpay.top

[S22] C：字符串转数字
来源：http://cej.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wgg.sxryk.cn

[S23] C：随机数
来源：http://zfe.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bwk.sufxvd.cn

[S24] C：获取本地时间
来源：http://ugo.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mbw.aibaodan.cn

[S25] C：内存拷贝
来源：http://wnk.chenlongwang.top

memcpy(dst, src, n);
来源：http://xhm.daxiang520.top

[S26] C：内存清零
来源：http://rjc.pycfn.com

memset(a, 0, sizeof a);
来源：http://otf.cheryme.top

[S27] C：定义常量
来源：http://fvf.fehbvm.com

const double PI = 3.14159;
来源：http://dkg.316326.xyz

[S28] C：静态变量
来源：http://dwh.bbcook.cn

static int counter = 0;
来源：http://kmu.shuidangran.top

[S29] C：变参函数
来源：http://bje.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tue.wangshuangyany.cn

[S30] C：头文件保护
来源：http://xfu.zhoulong.xyz

#ifndef X_H
来源：http://dxm.hywenlv.cn

#define X_H
来源：http://hnd.ydjk.org.cn

#endif
来源：http://oej.vehdjk.com

[S31] C++：Hello World
来源：http://rft.bbcook.cn

#include <iostream>
来源：http://oia.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://koh.zycfv.cn

[S32] C++：字符串
来源：http://llj.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://vml.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://ozf.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qqb.sysykeji.top

[S34] C++：遍历 vector
来源：http://gan.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://edz.yongpay.top

[S35] C++：map
来源：http://kyq.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxa.yueranfly.top

[S36] C++：unordered_map
来源：http://dmc.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khf.yangfankeji.com

[S37] C++：set
来源：http://ssa.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://noi.cheryme.top

[S38] C++：排序
来源：http://jip.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://ugh.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://cxj.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmd.jianghu66.top

[S40] C++：查找元素
来源：http://dte.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pfo.sufxvd.cn

[S41] C++：类与构造函数
来源：http://yni.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hxp.jianghu66.top

[S42] C++：继承与虚函数
来源：http://raq.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://gvw.zycfv.cn

[S43] C++：智能指针
来源：http://twx.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://gzg.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://dkp.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://wnt.hywenlv.cn

[S45] C++：lambda
来源：http://blm.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://adp.jiagoushi.top

[S46] C++：函数模板
来源：http://wpk.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oij.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://cqf.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqb.yuxming.cn

[S48] C++：逐行读文件
来源：http://djg.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://scp.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://fgi.shzxlz.cn

[S49] C++：写文件
来源：http://peq.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ijq.meibo888.top

[S50] C++：格式化数字
来源：http://pva.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vdp.dianchejie.cn

[S51] C++：显式类型转换
来源：http://alz.yuxming.cn

static_cast<double>(a) / b
来源：http://cjr.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://tfz.hcnkem.com

int size() const noexcept { return n_; }
来源：http://wnh.fzhhl.top

[S53] C++：移动语义
来源：http://qkx.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://cbt.xinyue.icu

[S54] C++：异常处理
来源：http://sau.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ugh.sweek.top

[S55] C++：结构化绑定
来源：http://lvb.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jhp.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://mxn.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uta.zhongyouzk.top

[S57] C++：编译期常量
来源：http://xlo.jinghuilouyu.cn

constexpr int N = 10;
来源：http://yxk.fehbvm.com

[S58] C++：命名空间
来源：http://qqa.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://tsu.fzhhl.top

[S59] C++：静态断言
来源：http://fbd.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cwu.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://scg.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zyf.jianghu66.top

================================================================================
来源：http://xpb.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dsx.yongpay.top

================================================================================
来源：http://sei.yongpay.top

[T01] Kotlin：Hello World
来源：http://daw.cheryme.top

println("Hello")
来源：http://djz.nanxuanxn.top

[T02] Kotlin：变量
来源：http://hmh.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xwu.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://taj.xuetiantiany.cn

"值: $b"
来源：http://txy.yj20258888.top

[T04] Kotlin：空安全
来源：http://ytv.jinqigufen.top

val n: String? = null;  n?.length
来源：http://szr.gzhubu.top


<!-- 参考信息 -->