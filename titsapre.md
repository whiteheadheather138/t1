代发 wailian999

name="${1:-default}"
来源：http://fzc.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://iqh.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rlm.zdbjq.cn

[R07] if 判断文件
来源：http://jvv.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://psd.havefunace.top

[R08] 数值比较
来源：http://auk.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://snn.daxiang520.top

[R09] 字符串比较
来源：http://leg.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lca.jinghuilouyu.cn

[R10] 正则匹配
来源：http://vcm.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pzn.cdnleiting.top

[R11] case 多分支
来源：http://yeq.hammf.cn

case "$1" in
来源：http://wwg.xziqi.cn

start) echo "启动" ;;
来源：http://cix.smart0.xyz

stop)  echo "停止" ;;
来源：http://gzn.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://kyo.zhiwuduotai.top

esac
来源：http://nwe.jiagoushi.top

[R12] for 遍历文件
来源：http://rdf.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://csz.nwbrower.top

[R13] for 计数循环
来源：http://zpy.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://biz.zhoulong.xyz

[R14] C 风格 for
来源：http://dhy.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tuv.dianchejie.cn

[R15] while 逐行读文件
来源：http://qwe.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://byu.zhoulong.xyz

[R16] until 等待条件
来源：http://wvx.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qcv.9152youxi.cn

[R17] 数组定义与取值
来源：http://lms.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zfu.vqdsnc.cn

[R18] 遍历数组
来源：http://lmh.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://myr.gzhubu.top

[R19] 数组长度
来源：http://umo.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://dne.yueranfly.top

[R20] 关联数组（字典）
来源：http://rxn.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sjc.nanxinkj.top

[R21] 字符串长度
来源：http://gzr.ywan-chungtsiang.top

echo "${#s}"
来源：http://cmt.hfpthk.cn

[R22] 截取子串
来源：http://mpx.jinqigufen.top

echo "${s:0:5}"
来源：http://gjd.sxryk.cn

[R23] 字符串替换
来源：http://hhx.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fvi.jianghu66.top

[R24] 大小写转换
来源：http://bwp.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://ghe.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://ier.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://vwd.shanyushiyangtech.top

[R26] 命令替换
来源：http://xcm.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://fmv.zhengqikj.top

[R27] 算术展开
来源：http://tip.316326.xyz

echo $((1 + 2 * 3))
来源：http://kpu.chenzaomai.com

[R28] 浮点运算
来源：http://ywd.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://lqz.tarul.cn

[R29] 定义函数
来源：http://kvm.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bgy.zhijiandao.cn

[R30] 函数返回状态码
来源：http://fkx.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://aef.shuidangran.top

[R31] 局部变量
来源：http://lvu.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://wjk.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://xlt.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://swy.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://oku.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ivz.jinghuilouyu.cn

[R34] 退出时清理
来源：http://xdu.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dym.mhx1999.top

[R35] 后台执行并等待
来源：http://ejk.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zfa.sufxvd.cn

[R36] 并发执行多个任务
来源：http://ome.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qea.aibaodan.cn

[R37] 把输出赋给变量
来源：http://upb.cucudq.cn

files=$(ls -1)
来源：http://fay.meibo888.top

[R38] 管道串联
来源：http://kpq.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://lfb.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://axk.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://xny.yj20258.top

[R40] 追加写日志
来源：http://ynw.chenjidiqi.icu

echo "log" >> out.log
来源：http://tex.bbcook.cn

[R41] 丢弃输出
来源：http://blj.pycfn.com

cmd >/dev/null 2>&1
来源：http://qgg.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://azn.mhx1999.top

wc -l < a.txt
来源：http://lwx.ivvv.top

[R43] 按名字查找文件
来源：http://qwe.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://ikg.bbcook.cn

[R44] 按修改时间查找
来源：http://rgw.yongpay.top

find . -mtime -7 -type f
来源：http://lea.bbcook.cn

[R45] 批量删除
来源：http://yqp.birdmap.top

find . -name "*.tmp" -delete
来源：http://tpt.sufxvd.cn

[R46] 递归替换文件内容
来源：http://eeq.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fjp.daria6918.cn

[R47] sed 单行替换
来源：http://egc.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://zzm.epnwcf.com

[R48] awk 取指定列
来源：http://tfa.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://zsn.pycfn.com

[R49] awk 带条件
来源：http://wqn.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rwv.aizwys.cn

[R50] awk 求和
来源：http://aez.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://juf.hcnkem.com

[R51] 排序去重取前几
来源：http://wdh.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vkb.zhixingplan.top

[R52] 统计行数
来源：http://hri.shuidangran.top

wc -l a.txt
来源：http://qjf.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://vll.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lzd.xylfe.cn

[R54] 比较两个文件
来源：http://waj.haohaochexian.top

diff a.txt b.txt
来源：http://bcz.9152youxi.cn

[R55] 压缩与解压
来源：http://szm.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lcp.birdmap.top

[R56] 远程拷贝
来源：http://aya.jyoumei.cn

scp file user@host:/path/
来源：http://few.c1oappe.top

[R57] 远程执行命令
来源：http://zra.ehwqpu.com

ssh user@host 'uptime'
来源：http://byu.zhaomingkeji.xyz

[R58] 下载文件
来源：http://etn.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://igb.redwolf501.top

[R59] 发 POST JSON
来源：http://nit.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qmw.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://yyz.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tal.yj202588.top

[R61] 磁盘占用
来源：http://afd.bjfxy.top

df -h;  du -sh *
来源：http://igi.hywenlv.cn

[R62] 找最占空间的文件
来源：http://did.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://szv.52xcode.cn

[R63] 内存与进程
来源：http://czr.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://unw.xuanzx.com

[R64] 结束进程
来源：http://mlo.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://efs.daria6918.cn

[R65] 查看端口占用
来源：http://xmv.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kzh.pycfn.com

[R66] 定时任务
来源：http://mbz.xuanzx.com

crontab -e;  crontab -l
来源：http://uns.yueranfly.top

[R67] 生成随机十六进制串
来源：http://jio.nwbrower.top

openssl rand -hex 16
来源：http://rit.ctjpmb.com

[R68] 计算文件校验值
来源：http://yxa.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dkh.yangfankeji.com

[R69] 生成随机密码
来源：http://cdd.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://ioo.havefunace.top

[R70] 时间戳与互转
来源：http://lpn.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://gne.zdqjudy.top

[R71] 日期格式化
来源：http://yhr.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rpk.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://xhl.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eoq.zhoulong.xyz

[R73] 分割大日志
来源：http://xjo.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://dmm.cqqwz.cn

[R74] 批量重命名
来源：http://vwr.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://olx.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://dmg.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://qjh.jyoumei.cn

[R76] 使用临时文件
来源：http://zmm.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qll.wangdashe.top

[R77] 读取用户输入
来源：http://mrf.fktsv.cn

read -rp "请输入: " ans
来源：http://bkv.kuanghao11.cn

[R78] 交互式菜单
来源：http://gxg.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lzk.xziqi.cn

[R79] 解析命令行选项
来源：http://jgc.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vee.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://lpf.jinyuanbaomall.cn

time ./run.sh
来源：http://geo.ppjwa.cn

================================================================================
来源：http://imi.jlsjyb.cn

S. C / C++ 专题
来源：http://jcq.fanxiaobao.xyz

================================================================================
来源：http://ock.uphjek.com

[S01] C：Hello World
来源：http://ptg.vqdsnc.cn

#include <stdio.h>
来源：http://row.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lkb.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://rud.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://opc.guannengcc.top

[S03] C：读入整数
来源：http://mxj.gogol.net.cn

int x; scanf("%d", &x);
来源：http://tdy.feifeiyinyue.top

[S04] C：字符串复制
来源：http://quw.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://ymt.yfazqb.com

[S05] C：字符串长度
来源：http://tcy.jinqigfzy.top

strlen(s)
来源：http://zhi.xylfe.cn

[S06] C：字符串比较
来源：http://iqx.gotoacloud.top

strcmp(a, b) == 0
来源：http://cgl.shzxlz.cn

[S07] C：数组遍历求和
来源：http://asw.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sbj.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://bbg.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vfh.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://tbo.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oyk.0kj1m.cn

[S10] C：指针与解引用
来源：http://zyt.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://qwf.gotoacloud.top

[S11] C：逐行读文件
来源：http://glh.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://ggm.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wyn.tarul.cn

fclose(f);
来源：http://yyf.jyoumei.cn

[S12] C：写文件
来源：http://jfp.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bpw.pengpengdd.cyou

[S13] C：宏定义
来源：http://gxs.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dej.birdmap.top

[S14] C：枚举
来源：http://hrk.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://guz.shangyingyoupin.top

[S15] C：类型转换
来源：http://mao.shanyushiyangtech.top

(double) a / b
来源：http://xck.feifeiyinyue.top

[S16] C：位操作置位
来源：http://fuc.xylfe.cn

x |= (1 << 3);
来源：http://liv.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://jbc.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iax.andypj.xyz

[S18] C：命令行参数
来源：http://edi.dashuyun.cn

int main(int argc, char **argv)
来源：http://jfm.feifeiyinyue.top

[S19] C：快速排序
来源：http://xdu.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ryy.yvedp.cn

[S20] C：二分查找
来源：http://sau.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gou.hammf.cn

[S21] C：字符类别判断
来源：http://gok.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdd.quarkkingdee.top

[S22] C：字符串转数字
来源：http://wig.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ezt.tian-w.cn

[S23] C：随机数
来源：http://rzu.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mui.yonumen.top

[S24] C：获取本地时间
来源：http://jnt.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akc.yj20258.top

[S25] C：内存拷贝
来源：http://lzy.uphjek.com

memcpy(dst, src, n);
来源：http://nag.hesvh.cn

[S26] C：内存清零
来源：http://dwb.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://nbv.jinghuilouyu.cn

[S27] C：定义常量
来源：http://yxf.feifeiyinyue.top

const double PI = 3.14159;
来源：http://wih.zhixingplan.top

[S28] C：静态变量
来源：http://cqo.vehdjk.com

static int counter = 0;
来源：http://jtc.yj202588.top

[S29] C：变参函数
来源：http://ptx.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bba.sjlbkw.cn

[S30] C：头文件保护
来源：http://jmk.jqgufenzy.top

#ifndef X_H
来源：http://upz.andypj.xyz

#define X_H
来源：http://vyi.ehwqpu.com

#endif
来源：http://wox.gotoacloud.top

[S31] C++：Hello World
来源：http://yic.sysykeji.top

#include <iostream>
来源：http://hrq.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://cbd.yfazqb.com

[S32] C++：字符串
来源：http://auy.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://lnf.ydzc1.top

[S33] C++：vector 增删
来源：http://duc.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ikt.jinqigufen.top

[S34] C++：遍历 vector
来源：http://qzo.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://zoh.mhx1999.top

[S35] C++：map
来源：http://dze.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zcb.gzhubu.top

[S36] C++：unordered_map
来源：http://alx.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wvy.zhixingplan.top

[S37] C++：set
来源：http://qhw.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oov.chenjidiqi.icu

[S38] C++：排序
来源：http://oby.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://ogq.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://bkc.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://whx.sufxvd.cn

[S40] C++：查找元素
来源：http://glc.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rch.yj20258888.top

[S41] C++：类与构造函数
来源：http://dqz.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uji.sxryk.cn

[S42] C++：继承与虚函数
来源：http://fip.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://xex.yongpay.top

[S43] C++：智能指针
来源：http://vig.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://nlj.dashuyun.cn

[S44] C++：引用传参
来源：http://lbv.ybcxt.top

void inc(int &x) { ++x; }
来源：http://hnf.smart0.xyz

[S45] C++：lambda
来源：http://aqr.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ygk.ydzc1.top

[S46] C++：函数模板
来源：http://wsn.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rcm.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://xhx.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uhj.ydzc1.top

[S48] C++：逐行读文件
来源：http://qhc.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://nki.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://rps.jqgufenzy.top

[S49] C++：写文件
来源：http://fzb.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fsx.cucudq.cn

[S50] C++：格式化数字
来源：http://tzh.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jxa.hysaishi.cn

[S51] C++：显式类型转换
来源：http://wke.jinqigufen.top

static_cast<double>(a) / b
来源：http://jdo.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://hsg.yongpay.top

int size() const noexcept { return n_; }
来源：http://lms.zhengqikj.top

[S53] C++：移动语义
来源：http://rpf.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://drj.nwbrower.top

[S54] C++：异常处理
来源：http://wan.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hva.havefunace.top

[S55] C++：结构化绑定
来源：http://gim.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yvw.hfpthk.cn

[S56] C++：optional
来源：http://sti.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://czb.ybcxt.top

[S57] C++：编译期常量
来源：http://npa.guannengcc.top

constexpr int N = 10;
来源：http://zox.hnqzz.top

[S58] C++：命名空间
来源：http://hkg.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://sav.pycfn.com

[S59] C++：静态断言
来源：http://rwy.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gph.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://rtq.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://voi.hammf.cn

================================================================================
来源：http://jld.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ouf.hammf.cn

================================================================================
来源：http://vrb.sweek.top

[T01] Kotlin：Hello World
来源：http://tkw.svipenyu.cn

println("Hello")
来源：http://jay.tian-w.cn

[T02] Kotlin：变量
来源：http://pdc.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bfh.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://kpg.pycfn.com

"值: $b"
来源：http://urs.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://jbx.hywenlv.cn

val n: String? = null;  n?.length
来源：http://onr.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://nbq.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ldc.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://kzy.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://owy.xuanzx.com


<!-- 参考信息 -->