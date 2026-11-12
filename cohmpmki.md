代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tto.hysaishi.cn

[R08] 数值比较
来源：http://xjw.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pom.sjlbkw.cn

[R09] 字符串比较
来源：http://ywl.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cwz.hnxiangtu.top

[R10] 正则匹配
来源：http://ufx.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xsg.gotoacloud.top

[R11] case 多分支
来源：http://nek.fktsv.cn

case "$1" in
来源：http://cvx.kuanghao11.cn

start) echo "启动" ;;
来源：http://ofq.hywenlv.cn

stop)  echo "停止" ;;
来源：http://ukr.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://jtz.gaohongyu789.top

esac
来源：http://hwp.uphjek.com

[R12] for 遍历文件
来源：http://opa.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://eig.epnwcf.com

[R13] for 计数循环
来源：http://xem.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://scc.uphjek.com

[R14] C 风格 for
来源：http://kts.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cwg.yanxiufei.cn

[R15] while 逐行读文件
来源：http://rxn.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ibw.9152youxi.cn

[R16] until 等待条件
来源：http://szf.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cgq.jianghu66.top

[R17] 数组定义与取值
来源：http://wtt.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://tbc.cqqwz.cn

[R18] 遍历数组
来源：http://ytw.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://txa.tarul.cn

[R19] 数组长度
来源：http://bnl.haohaochexian.top

echo "${#arr[@]}"
来源：http://vkx.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://kjh.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nfi.bbcook.cn

[R21] 字符串长度
来源：http://gfm.gaohongyu789.top

echo "${#s}"
来源：http://hor.sysykeji.top

[R22] 截取子串
来源：http://tkz.birdmap.top

echo "${s:0:5}"
来源：http://jel.nwbrower.top

[R23] 字符串替换
来源：http://tmd.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ukz.daria6918.cn

[R24] 大小写转换
来源：http://gme.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://wxt.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://twf.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zxp.jinyuanbaomall.cn

[R26] 命令替换
来源：http://xvb.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://cjp.zhongyouzk.top

[R27] 算术展开
来源：http://ifn.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://udh.iojbl.cn

[R28] 浮点运算
来源：http://kts.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://ztv.yvedp.cn

[R29] 定义函数
来源：http://xpg.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dpk.kuanghao11.cn

[R30] 函数返回状态码
来源：http://nci.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://sen.sysykeji.top

[R31] 局部变量
来源：http://lqo.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://hty.daxiang520.top

[R32] 参数个数校验
来源：http://kox.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://csc.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://iik.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jlf.shzxlz.cn

[R34] 退出时清理
来源：http://jwd.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xhd.zhixingplan.top

[R35] 后台执行并等待
来源：http://gor.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qtv.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://hhe.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hwi.yonumen.top

[R37] 把输出赋给变量
来源：http://zrr.gaohongyu789.top

files=$(ls -1)
来源：http://kwy.daria6918.cn

[R38] 管道串联
来源：http://xai.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://jua.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://kls.yanxiufei.cn

cmd > out.log 2>&1
来源：http://nlu.fanxiaobao.xyz

[R40] 追加写日志
来源：http://ifp.hnqzz.top

echo "log" >> out.log
来源：http://gob.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://tbd.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://rws.fktsv.cn

[R42] 输入重定向
来源：http://uvi.cucudq.cn

wc -l < a.txt
来源：http://yzr.nanxinkj.top

[R43] 按名字查找文件
来源：http://wib.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://ywu.fktsv.cn

[R44] 按修改时间查找
来源：http://eoi.smart0.xyz

find . -mtime -7 -type f
来源：http://azb.yueranfly.top

[R45] 批量删除
来源：http://orb.xuanzx.com

find . -name "*.tmp" -delete
来源：http://upk.zhixingplan.top

[R46] 递归替换文件内容
来源：http://wlr.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eyf.iojbl.cn

[R47] sed 单行替换
来源：http://zak.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://ejb.yj20258.top

[R48] awk 取指定列
来源：http://vhk.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://oki.hcnkem.com

[R49] awk 带条件
来源：http://npz.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wuk.ehwqpu.com

[R50] awk 求和
来源：http://zxm.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cav.wangdashe.top

[R51] 排序去重取前几
来源：http://alp.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iws.fzhhl.top

[R52] 统计行数
来源：http://hlu.sufxvd.cn

wc -l a.txt
来源：http://ulo.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://qhy.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mwx.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://goy.fengsongda.top

diff a.txt b.txt
来源：http://boe.fengsongda.top

[R55] 压缩与解压
来源：http://jsp.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iye.316326.xyz

[R56] 远程拷贝
来源：http://eqn.cdnleiting.top

scp file user@host:/path/
来源：http://ndn.hnxiangtu.top

[R57] 远程执行命令
来源：http://kie.fktsv.cn

ssh user@host 'uptime'
来源：http://irr.zhengqikj.top

[R58] 下载文件
来源：http://num.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://awd.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://ewe.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://agw.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://pmt.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bvp.cashguo.top

[R61] 磁盘占用
来源：http://tpn.ydzc1.top

df -h;  du -sh *
来源：http://muj.zhixingplan.top

[R62] 找最占空间的文件
来源：http://son.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://lxn.nwbrower.top

[R63] 内存与进程
来源：http://kgt.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://muj.daria6918.cn

[R64] 结束进程
来源：http://fto.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://nau.guannengcc.top

[R65] 查看端口占用
来源：http://nwq.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uhq.zhengqikj.top

[R66] 定时任务
来源：http://vkj.sxryk.cn

crontab -e;  crontab -l
来源：http://dsk.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://kbo.hnqzz.top

openssl rand -hex 16
来源：http://lps.chenzaomai.com

[R68] 计算文件校验值
来源：http://frv.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://veq.jinqigufen.top

[R69] 生成随机密码
来源：http://vou.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://kvx.sufxvd.cn

[R70] 时间戳与互转
来源：http://leu.daria6918.cn

date +%s;  date -d @1700000000
来源：http://dun.xuanzx.com

[R71] 日期格式化
来源：http://eay.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bwc.sweek.top

[R72] 等待端口就绪
来源：http://csq.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aaw.ppjwa.cn

[R73] 分割大日志
来源：http://fqi.birdmap.top

split -l 1000 big.log part_
来源：http://tel.sxryk.cn

[R74] 批量重命名
来源：http://lhp.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rzj.dashuyun.cn

[R75] 导出环境变量
来源：http://bvw.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://wlg.yuanzhike.top

[R76] 使用临时文件
来源：http://ycr.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eaa.dianchejie.cn

[R77] 读取用户输入
来源：http://amc.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://vbf.hcnkem.com

[R78] 交互式菜单
来源：http://uwi.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://psx.nanxuanxn.top

[R79] 解析命令行选项
来源：http://jmj.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ugn.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://aue.zhijiandao.cn

time ./run.sh
来源：http://sql.zhaomingkeji.xyz

================================================================================
来源：http://nkn.jlsjyb.cn

S. C / C++ 专题
来源：http://afk.redwolf501.top

================================================================================
来源：http://krp.zdqjudy.top

[S01] C：Hello World
来源：http://muv.pycfn.com

#include <stdio.h>
来源：http://jix.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mbx.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://fig.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://azn.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://bcr.ppjwa.cn

int x; scanf("%d", &x);
来源：http://pjx.shangyingyoupin.top

[S04] C：字符串复制
来源：http://ogp.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pbh.hywenlv.cn

[S05] C：字符串长度
来源：http://cek.sweek.top

strlen(s)
来源：http://trn.zhongyouzk.top

[S06] C：字符串比较
来源：http://btr.xylfe.cn

strcmp(a, b) == 0
来源：http://mfq.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://rer.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jnf.cheryme.top

[S08] C：动态内存分配与释放
来源：http://cgy.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://adx.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://vqt.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lus.ctjpmb.com

[S10] C：指针与解引用
来源：http://bgg.wangdashe.top

int *p = &a;  *p = 5;
来源：http://srr.gzhubu.top

[S11] C：逐行读文件
来源：http://ucr.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://yih.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://boe.yuxming.cn

fclose(f);
来源：http://mzw.zhixingplan.top

[S12] C：写文件
来源：http://wqr.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kdg.yj20258888.top

[S13] C：宏定义
来源：http://vyp.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mew.zycfv.cn

[S14] C：枚举
来源：http://ekl.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://vmq.zdbjq.cn

[S15] C：类型转换
来源：http://zlg.ydjk.org.cn

(double) a / b
来源：http://dih.yj20258888.top

[S16] C：位操作置位
来源：http://bxx.zdbjq.cn

x |= (1 << 3);
来源：http://oap.xuanzx.com

[S17] C：安全拼接字符串
来源：http://nia.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nfv.jiagoushi.top

[S18] C：命令行参数
来源：http://xpf.ctjpmb.com

int main(int argc, char **argv)
来源：http://ihu.ehwqpu.com

[S19] C：快速排序
来源：http://fly.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://rzw.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://mak.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cly.ppjwa.cn

[S21] C：字符类别判断
来源：http://avh.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tqc.jqgfzy.top

[S22] C：字符串转数字
来源：http://ifu.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lat.yfazqb.com

[S23] C：随机数
来源：http://jsq.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://yxf.cucudq.cn

[S24] C：获取本地时间
来源：http://syz.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rft.daxiang520.top

[S25] C：内存拷贝
来源：http://ggp.wangdashe.top

memcpy(dst, src, n);
来源：http://ifx.sweek.top

[S26] C：内存清零
来源：http://xqf.smart0.xyz

memset(a, 0, sizeof a);
来源：http://fbk.nanxinkj.top

[S27] C：定义常量
来源：http://jqk.jqgufenzy.top

const double PI = 3.14159;
来源：http://hld.jianghu66.top

[S28] C：静态变量
来源：http://bdg.jiagoushi.top

static int counter = 0;
来源：http://auf.bbcook.cn

[S29] C：变参函数
来源：http://npj.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eob.gzhubu.top

[S30] C：头文件保护
来源：http://ozg.bjfxy.top

#ifndef X_H
来源：http://wgk.zhixingplan.top

#define X_H
来源：http://mpm.epnwcf.com

#endif
来源：http://jyg.ydjk.org.cn

[S31] C++：Hello World
来源：http://zfs.ivvv.top

#include <iostream>
来源：http://jzl.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://cxd.wangdashe.top

[S32] C++：字符串
来源：http://dnd.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://byt.jianghu66.top

[S33] C++：vector 增删
来源：http://kfd.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://txu.xylfe.cn

[S34] C++：遍历 vector
来源：http://rfe.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://oun.tian-w.cn

[S35] C++：map
来源：http://pjn.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://upu.iojbl.cn

[S36] C++：unordered_map
来源：http://ckw.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fhb.zhixingplan.top

[S37] C++：set
来源：http://syl.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bdy.jinqigfzy.top

[S38] C++：排序
来源：http://kxc.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://jie.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://nfp.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xpr.andypj.xyz

[S40] C++：查找元素
来源：http://lel.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wka.zdbjq.cn

[S41] C++：类与构造函数
来源：http://qqu.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jtc.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://qsa.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://pyc.yangfankeji.com

[S43] C++：智能指针
来源：http://vtg.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://ovz.yj202588.top

[S44] C++：引用传参
来源：http://rzn.yj202588.top

void inc(int &x) { ++x; }
来源：http://gpu.guowangkeji.top

[S45] C++：lambda
来源：http://yhy.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://tzo.aizwys.cn

[S46] C++：函数模板
来源：http://rvg.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gsa.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://lyt.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cdl.sweek.top

[S48] C++：逐行读文件
来源：http://nsc.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ypz.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://jmd.jyoumei.cn

[S49] C++：写文件
来源：http://hrp.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zcc.jiagoushi.top

[S50] C++：格式化数字
来源：http://ghe.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nba.redwolf501.top

[S51] C++：显式类型转换
来源：http://yvu.0kj1m.cn

static_cast<double>(a) / b
来源：http://qtj.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://zhe.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://xsk.tianlin.xyz

[S53] C++：移动语义
来源：http://ujk.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://uxa.vehdjk.com

[S54] C++：异常处理
来源：http://ctu.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tee.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://wme.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://urg.birdmap.top

[S56] C++：optional
来源：http://btx.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fqf.vqdsnc.cn

[S57] C++：编译期常量
来源：http://eto.jiagoushi.top

constexpr int N = 10;
来源：http://cpe.xziqi.cn

[S58] C++：命名空间
来源：http://vbc.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://jch.zycfv.cn

[S59] C++：静态断言
来源：http://vjo.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hze.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://xju.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xse.daxiang520.top

================================================================================
来源：http://zwi.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cey.tian-w.cn

================================================================================
来源：http://cgq.cheryme.top

[T01] Kotlin：Hello World
来源：http://szh.jqgufenzy.top

println("Hello")
来源：http://mne.ybcxt.top

[T02] Kotlin：变量
来源：http://vap.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dja.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://dgt.fengsongda.top

"值: $b"
来源：http://cmz.daria6918.cn

[T04] Kotlin：空安全
来源：http://nro.yangfankeji.com

val n: String? = null;  n?.length
来源：http://czy.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://muh.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eoj.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://vcz.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bmf.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://icq.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lqk.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://sfi.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://mve.andypj.xyz


<!-- 参考信息 -->