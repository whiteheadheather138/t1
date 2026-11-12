代发 wailian999

name="${1:-default}"
来源：http://rux.chenzaomai.com

[R06] 判断命令是否存在
来源：http://xet.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wqb.jinghuilouyu.cn

[R07] if 判断文件
来源：http://igt.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zgr.smart0.xyz

[R08] 数值比较
来源：http://qcd.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mbl.daxiang520.top

[R09] 字符串比较
来源：http://hwx.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qmi.yvedp.cn

[R10] 正则匹配
来源：http://qno.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xak.ywan-chungtsiang.top

[R11] case 多分支
来源：http://mrs.chenjidiqi.icu

case "$1" in
来源：http://dqj.yj202588.top

start) echo "启动" ;;
来源：http://qti.cucudq.cn

stop)  echo "停止" ;;
来源：http://rfq.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://hyh.xuanzx.com

esac
来源：http://wwo.redwolf501.top

[R12] for 遍历文件
来源：http://qdo.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://nkz.xziqi.cn

[R13] for 计数循环
来源：http://prc.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://tvi.gogol.net.cn

[R14] C 风格 for
来源：http://fkw.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hnm.jqgfzy.top

[R15] while 逐行读文件
来源：http://moe.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uyu.kuanghao11.cn

[R16] until 等待条件
来源：http://szk.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rlp.havefunace.top

[R17] 数组定义与取值
来源：http://joq.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zyy.xziqi.cn

[R18] 遍历数组
来源：http://xqx.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gii.jinyuanbaomall.cn

[R19] 数组长度
来源：http://oaw.sweek.top

echo "${#arr[@]}"
来源：http://vhi.hywenlv.cn

[R20] 关联数组（字典）
来源：http://jcj.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svm.iojbl.cn

[R21] 字符串长度
来源：http://wzx.yongpay.top

echo "${#s}"
来源：http://bmu.svipenyu.cn

[R22] 截取子串
来源：http://qjc.yfazqb.com

echo "${s:0:5}"
来源：http://iic.birdmap.top

[R23] 字符串替换
来源：http://xqw.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eze.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://qfd.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://dtr.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://beq.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mot.aibaodan.cn

[R26] 命令替换
来源：http://won.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://vnp.hnxiangtu.top

[R27] 算术展开
来源：http://qfr.cheryme.top

echo $((1 + 2 * 3))
来源：http://sct.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://ngv.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://lis.shzxlz.cn

[R29] 定义函数
来源：http://ick.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://irp.zdqjudy.top

[R30] 函数返回状态码
来源：http://utu.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://kiq.tian-w.cn

[R31] 局部变量
来源：http://kpv.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://hcg.sweek.top

[R32] 参数个数校验
来源：http://stk.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vrs.316326.xyz

[R33] 捕获错误并提示行号
来源：http://agk.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyw.jqgfzy.top

[R34] 退出时清理
来源：http://kef.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tdg.hnqzz.top

[R35] 后台执行并等待
来源：http://xxt.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xcq.hywenlv.cn

[R36] 并发执行多个任务
来源：http://kxu.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cev.316326.xyz

[R37] 把输出赋给变量
来源：http://wti.uphjek.com

files=$(ls -1)
来源：http://dit.tarul.cn

[R38] 管道串联
来源：http://czy.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://iyd.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://wkr.jinqigufen.top

cmd > out.log 2>&1
来源：http://tnz.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://oxb.zhengqikj.top

echo "log" >> out.log
来源：http://kjl.zhixingplan.top

[R41] 丢弃输出
来源：http://lks.sxryk.cn

cmd >/dev/null 2>&1
来源：http://bev.ybcxt.top

[R42] 输入重定向
来源：http://hid.aizwys.cn

wc -l < a.txt
来源：http://ukc.aizwys.cn

[R43] 按名字查找文件
来源：http://jbl.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://uwd.yvedp.cn

[R44] 按修改时间查找
来源：http://knf.ehwqpu.com

find . -mtime -7 -type f
来源：http://ylp.cashguo.top

[R45] 批量删除
来源：http://itn.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://zxd.shzxlz.cn

[R46] 递归替换文件内容
来源：http://eos.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svw.bjfxy.top

[R47] sed 单行替换
来源：http://adh.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://flc.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://yoe.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://spu.quarkkingdee.top

[R49] awk 带条件
来源：http://vlp.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mfk.jqgfzy.top

[R50] awk 求和
来源：http://kfe.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://hlq.aizwys.cn

[R51] 排序去重取前几
来源：http://ynd.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://ohg.tarul.cn

[R52] 统计行数
来源：http://xlo.jinyuanbaomall.cn

wc -l a.txt
来源：http://riq.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://uzr.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aex.iojbl.cn

[R54] 比较两个文件
来源：http://jsl.bjfxy.top

diff a.txt b.txt
来源：http://adt.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://szg.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://irv.quarkkingdee.top

[R56] 远程拷贝
来源：http://emq.shuidangran.top

scp file user@host:/path/
来源：http://eih.jqgfzy.top

[R57] 远程执行命令
来源：http://oxt.yanxiufei.cn

ssh user@host 'uptime'
来源：http://qup.iojbl.cn

[R58] 下载文件
来源：http://wfy.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xvm.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://phe.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jgy.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://tpj.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivd.tarul.cn

[R61] 磁盘占用
来源：http://upv.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://gkg.jianghu66.top

[R62] 找最占空间的文件
来源：http://qhb.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://lmo.zhengqikj.top

[R63] 内存与进程
来源：http://xtv.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://yqe.wangshuangyany.cn

[R64] 结束进程
来源：http://bwx.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://irj.dianchejie.cn

[R65] 查看端口占用
来源：http://pmg.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eic.ywan-chungtsiang.top

[R66] 定时任务
来源：http://hub.fengsongda.top

crontab -e;  crontab -l
来源：http://cdp.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://wmy.chenlongwang.top

openssl rand -hex 16
来源：http://mrf.hywenlv.cn

[R68] 计算文件校验值
来源：http://amx.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://fnf.yangfankeji.com

[R69] 生成随机密码
来源：http://vns.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://aof.uphjek.com

[R70] 时间戳与互转
来源：http://wcb.tian-w.cn

date +%s;  date -d @1700000000
来源：http://xfa.chenzaomai.com

[R71] 日期格式化
来源：http://lxd.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jkf.zhixingplan.top

[R72] 等待端口就绪
来源：http://bsx.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://vvj.shzxlz.cn

[R73] 分割大日志
来源：http://wxt.fktsv.cn

split -l 1000 big.log part_
来源：http://kjp.uphjek.com

[R74] 批量重命名
来源：http://onr.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dnv.shuidangran.top

[R75] 导出环境变量
来源：http://era.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://iad.andypj.xyz

[R76] 使用临时文件
来源：http://qoq.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qcd.gogol.net.cn

[R77] 读取用户输入
来源：http://gdb.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://uis.yueranfly.top

[R78] 交互式菜单
来源：http://lfh.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ueq.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://urb.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kff.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://hjb.gzhubu.top

time ./run.sh
来源：http://kux.tarul.cn

================================================================================
来源：http://tiu.yanxiufei.cn

S. C / C++ 专题
来源：http://hqs.jianghu66.top

================================================================================
来源：http://mbu.yuanzhike.top

[S01] C：Hello World
来源：http://pel.sweek.top

#include <stdio.h>
来源：http://clb.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://rtr.ybcxt.top

[S02] C：变量与格式化输出
来源：http://cpx.sweek.top

int a = 10; printf("%d\n", a);
来源：http://vvg.meibo888.top

[S03] C：读入整数
来源：http://vfh.316326.xyz

int x; scanf("%d", &x);
来源：http://way.zhixingplan.top

[S04] C：字符串复制
来源：http://fzy.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kje.yongpay.top

[S05] C：字符串长度
来源：http://jrj.hfpthk.cn

strlen(s)
来源：http://opj.sufxvd.cn

[S06] C：字符串比较
来源：http://poi.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://qas.yuxming.cn

[S07] C：数组遍历求和
来源：http://aap.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbc.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://lxv.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qtt.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://cwt.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lmt.52xcode.cn

[S10] C：指针与解引用
来源：http://zbq.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://des.sjlbkw.cn

[S11] C：逐行读文件
来源：http://ixq.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://mni.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://aol.ivvv.top

fclose(f);
来源：http://bjw.ivvv.top

[S12] C：写文件
来源：http://xih.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fvs.hnxiangtu.top

[S13] C：宏定义
来源：http://rsc.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ecb.dashuyun.cn

[S14] C：枚举
来源：http://apr.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://nfz.jyoumei.cn

[S15] C：类型转换
来源：http://cys.jiagoushi.top

(double) a / b
来源：http://fik.yanxiufei.cn

[S16] C：位操作置位
来源：http://hdr.hfpthk.cn

x |= (1 << 3);
来源：http://skf.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://ctt.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://com.mhx1999.top

[S18] C：命令行参数
来源：http://mpz.hesvh.cn

int main(int argc, char **argv)
来源：http://fgq.havefunace.top

[S19] C：快速排序
来源：http://tnc.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://gjx.yvedp.cn

[S20] C：二分查找
来源：http://wht.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sck.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://eyn.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ebu.tarul.cn

[S22] C：字符串转数字
来源：http://yfs.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://mel.sysykeji.top

[S23] C：随机数
来源：http://srw.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xhk.dashuyun.cn

[S24] C：获取本地时间
来源：http://uzj.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ssw.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://mgv.hammf.cn

memcpy(dst, src, n);
来源：http://lkg.yongpay.top

[S26] C：内存清零
来源：http://dpd.fehbvm.com

memset(a, 0, sizeof a);
来源：http://moc.chenzaomai.com

[S27] C：定义常量
来源：http://rsp.yangfankeji.com

const double PI = 3.14159;
来源：http://llo.ivvv.top

[S28] C：静态变量
来源：http://aei.uphjek.com

static int counter = 0;
来源：http://ezy.vqdsnc.cn

[S29] C：变参函数
来源：http://tjr.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pjc.xylfe.cn

[S30] C：头文件保护
来源：http://itw.jqgufenzy.top

#ifndef X_H
来源：http://hlz.shzxlz.cn

#define X_H
来源：http://pfp.yuanzhike.top

#endif
来源：http://dgl.tarul.cn

[S31] C++：Hello World
来源：http://sqp.yj20258.top

#include <iostream>
来源：http://rit.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://gnl.chenzaomai.com

[S32] C++：字符串
来源：http://yhs.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://ekh.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://jad.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ygb.ybcxt.top

[S34] C++：遍历 vector
来源：http://qjp.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://eia.vehdjk.com

[S35] C++：map
来源：http://cql.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zna.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://nea.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qtr.iojbl.cn

[S37] C++：set
来源：http://mlp.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wph.c1oappe.top

[S38] C++：排序
来源：http://ufh.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://nrz.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://ibd.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rle.fehbvm.com

[S40] C++：查找元素
来源：http://qbp.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://puk.0kj1m.cn

[S41] C++：类与构造函数
来源：http://qqd.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://plh.jianghu66.top

[S42] C++：继承与虚函数
来源：http://mcr.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://wsw.andypj.xyz

[S43] C++：智能指针
来源：http://kwt.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://bty.vehdjk.com

[S44] C++：引用传参
来源：http://cdj.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://sft.xylfe.cn

[S45] C++：lambda
来源：http://vhn.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://owl.fehbvm.com

[S46] C++：函数模板
来源：http://rfx.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cho.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://jvu.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zri.zycfv.cn

[S48] C++：逐行读文件
来源：http://gsx.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://ubh.yueranfly.top

while (std::getline(in, line)) { }
来源：http://adb.quarkkingdee.top

[S49] C++：写文件
来源：http://lld.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ycs.hfpthk.cn

[S50] C++：格式化数字
来源：http://wai.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wej.hammf.cn

[S51] C++：显式类型转换
来源：http://knx.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://wyw.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://kex.meibo888.top

int size() const noexcept { return n_; }
来源：http://fqz.zhengqikj.top

[S53] C++：移动语义
来源：http://rjz.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://evf.yueranfly.top

[S54] C++：异常处理
来源：http://jsw.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xdt.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://qaw.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rsa.yangfankeji.com

[S56] C++：optional
来源：http://xvf.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sxu.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://pzo.fktsv.cn

constexpr int N = 10;
来源：http://ptz.hywenlv.cn

[S58] C++：命名空间
来源：http://ssb.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://pzt.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://aie.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdk.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://aym.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xam.shangyingyoupin.top

================================================================================
来源：http://mub.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qnr.iojbl.cn

================================================================================
来源：http://bhy.guannengcc.top

[T01] Kotlin：Hello World
来源：http://rbf.bbcook.cn

println("Hello")
来源：http://rdd.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://kje.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tyb.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://vbx.cashguo.top

"值: $b"
来源：http://gpn.xylfe.cn

[T04] Kotlin：空安全
来源：http://qtz.ppjwa.cn

val n: String? = null;  n?.length
来源：http://fvf.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://etn.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://znl.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://fpk.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://djv.hongshengwenyu.top


<!-- 参考信息 -->