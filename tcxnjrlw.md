代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cvo.fengsongda.top

[R08] 数值比较
来源：http://fep.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ozs.xuetiantiany.cn

[R09] 字符串比较
来源：http://vvg.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://end.yvedp.cn

[R10] 正则匹配
来源：http://bvd.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mcz.jqgufenzy.top

[R11] case 多分支
来源：http://rzk.sxryk.cn

case "$1" in
来源：http://uqc.yj20258.top

start) echo "启动" ;;
来源：http://bvd.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://njk.aizwys.cn

*)     echo "未知命令" ;;
来源：http://smx.cheryme.top

esac
来源：http://gww.uphjek.com

[R12] for 遍历文件
来源：http://klt.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://jkx.hfpthk.cn

[R13] for 计数循环
来源：http://sgr.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sya.hcnkem.com

[R14] C 风格 for
来源：http://rjb.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fpa.cashguo.top

[R15] while 逐行读文件
来源：http://avy.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kmj.yangfankeji.com

[R16] until 等待条件
来源：http://mwa.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://itq.sufxvd.cn

[R17] 数组定义与取值
来源：http://sjj.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ttt.andypj.xyz

[R18] 遍历数组
来源：http://xjq.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://boc.zdqjudy.top

[R19] 数组长度
来源：http://cdv.fktsv.cn

echo "${#arr[@]}"
来源：http://kji.aizwys.cn

[R20] 关联数组（字典）
来源：http://ked.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wpg.zdbjq.cn

[R21] 字符串长度
来源：http://qag.gogol.net.cn

echo "${#s}"
来源：http://rxu.fehbvm.com

[R22] 截取子串
来源：http://tbg.xylfe.cn

echo "${s:0:5}"
来源：http://vrm.fanxiaobao.xyz

[R23] 字符串替换
来源：http://hdl.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hvs.zdbjq.cn

[R24] 大小写转换
来源：http://mqi.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ejb.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://ndf.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qnh.hfpthk.cn

[R26] 命令替换
来源：http://rpc.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://zbw.feifeiyinyue.top

[R27] 算术展开
来源：http://zey.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://bwh.zhixingplan.top

[R28] 浮点运算
来源：http://ylx.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://yox.shanyushiyangkeji.top

[R29] 定义函数
来源：http://tfz.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cyh.tianlin.xyz

[R30] 函数返回状态码
来源：http://iog.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://pne.nanxinkj.top

[R31] 局部变量
来源：http://wrc.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://dol.yj20258.top

[R32] 参数个数校验
来源：http://odw.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uvn.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://gjd.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://glw.hysaishi.cn

[R34] 退出时清理
来源：http://lze.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://kmd.ctjpmb.com

[R35] 后台执行并等待
来源：http://far.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bfa.cqqwz.cn

[R36] 并发执行多个任务
来源：http://hcm.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ovh.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://mcq.wangshuangyany.cn

files=$(ls -1)
来源：http://uai.fktsv.cn

[R38] 管道串联
来源：http://aiz.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://xlm.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://wbp.redwolf501.top

cmd > out.log 2>&1
来源：http://rzk.smart0.xyz

[R40] 追加写日志
来源：http://ndl.ehwqpu.com

echo "log" >> out.log
来源：http://nen.9152youxi.cn

[R41] 丢弃输出
来源：http://fqo.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://ngw.jinqigfzy.top

[R42] 输入重定向
来源：http://azd.birdmap.top

wc -l < a.txt
来源：http://cko.zhijiandao.cn

[R43] 按名字查找文件
来源：http://yit.ydjk.org.cn

find . -name "*.log" -type f
来源：http://btw.zhixingplan.top

[R44] 按修改时间查找
来源：http://yxe.sufxvd.cn

find . -mtime -7 -type f
来源：http://ilu.ydjk.org.cn

[R45] 批量删除
来源：http://taj.bbcook.cn

find . -name "*.tmp" -delete
来源：http://met.sysykeji.top

[R46] 递归替换文件内容
来源：http://ymk.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lnn.quarkkingdee.top

[R47] sed 单行替换
来源：http://xxa.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://xtl.yuxming.cn

[R48] awk 取指定列
来源：http://oiw.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://iwu.0kj1m.cn

[R49] awk 带条件
来源：http://jun.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mju.bjfxy.top

[R50] awk 求和
来源：http://etz.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jhw.0kj1m.cn

[R51] 排序去重取前几
来源：http://gaq.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ckg.xinyue.icu

[R52] 统计行数
来源：http://lgy.zhiwuduotai.top

wc -l a.txt
来源：http://pdg.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://tki.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ley.fzhhl.top

[R54] 比较两个文件
来源：http://omf.dashuyun.cn

diff a.txt b.txt
来源：http://jru.52xcode.cn

[R55] 压缩与解压
来源：http://vqc.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tlu.cqqwz.cn

[R56] 远程拷贝
来源：http://rjf.guowangkeji.top

scp file user@host:/path/
来源：http://lxt.sjlbkw.cn

[R57] 远程执行命令
来源：http://ptq.meibo888.top

ssh user@host 'uptime'
来源：http://dnj.chenzaomai.com

[R58] 下载文件
来源：http://sjl.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yvz.sxryk.cn

[R59] 发 POST JSON
来源：http://dxf.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vph.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://pxn.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ctm.jinqigufen.top

[R61] 磁盘占用
来源：http://wuf.svipenyu.cn

df -h;  du -sh *
来源：http://tmi.yj20258888.top

[R62] 找最占空间的文件
来源：http://jgq.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://dpb.zdbjq.cn

[R63] 内存与进程
来源：http://zzr.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://pve.xinyue.icu

[R64] 结束进程
来源：http://sml.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://rvz.yangfankeji.com

[R65] 查看端口占用
来源：http://eiy.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bmr.hnqzz.top

[R66] 定时任务
来源：http://cns.c1oappe.top

crontab -e;  crontab -l
来源：http://xia.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://zer.quarkkingdee.top

openssl rand -hex 16
来源：http://hvd.yongpay.top

[R68] 计算文件校验值
来源：http://gop.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lfj.tian-w.cn

[R69] 生成随机密码
来源：http://oer.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://hwv.sjlbkw.cn

[R70] 时间戳与互转
来源：http://gwo.bjfxy.top

date +%s;  date -d @1700000000
来源：http://dkq.epnwcf.com

[R71] 日期格式化
来源：http://nhv.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://roe.bjfxy.top

[R72] 等待端口就绪
来源：http://liq.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://btw.bjfxy.top

[R73] 分割大日志
来源：http://utn.cqqwz.cn

split -l 1000 big.log part_
来源：http://pzk.ivvv.top

[R74] 批量重命名
来源：http://tbj.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mvw.shuidangran.top

[R75] 导出环境变量
来源：http://ryi.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://zdg.nanxinkj.top

[R76] 使用临时文件
来源：http://dwg.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ojh.ydjk.org.cn

[R77] 读取用户输入
来源：http://ywh.sweek.top

read -rp "请输入: " ans
来源：http://pgg.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://azd.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vuh.yuanzhike.top

[R79] 解析命令行选项
来源：http://ehn.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tvw.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://iwx.shanyushiyangtech.top

time ./run.sh
来源：http://hgk.9152youxi.cn

================================================================================
来源：http://ykd.guannengcc.top

S. C / C++ 专题
来源：http://zjf.fanxiaobao.xyz

================================================================================
来源：http://tta.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://jjl.52xcode.cn

#include <stdio.h>
来源：http://lhx.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ooe.xylfe.cn

[S02] C：变量与格式化输出
来源：http://lcr.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://jat.sweek.top

[S03] C：读入整数
来源：http://kfo.dashuyun.cn

int x; scanf("%d", &x);
来源：http://fzo.quarkkingdee.top

[S04] C：字符串复制
来源：http://fqe.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vsy.fengsongda.top

[S05] C：字符串长度
来源：http://oyk.jqgufenzy.top

strlen(s)
来源：http://uct.shuidangran.top

[S06] C：字符串比较
来源：http://etj.andypj.xyz

strcmp(a, b) == 0
来源：http://ffx.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://tql.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://njj.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://hbs.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tgv.cashguo.top

[S09] C：结构体定义与初始化
来源：http://lmy.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kdd.redwolf501.top

[S10] C：指针与解引用
来源：http://iep.epnwcf.com

int *p = &a;  *p = 5;
来源：http://kgv.pycfn.com

[S11] C：逐行读文件
来源：http://ssc.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://vwv.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pqk.chenlongwang.top

fclose(f);
来源：http://zhr.hysaishi.cn

[S12] C：写文件
来源：http://cul.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lmr.xylfe.cn

[S13] C：宏定义
来源：http://naw.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zds.yuanzhike.top

[S14] C：枚举
来源：http://erd.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://ubn.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://amc.ctjpmb.com

(double) a / b
来源：http://dit.cqqwz.cn

[S16] C：位操作置位
来源：http://zyr.aibaodan.cn

x |= (1 << 3);
来源：http://xuq.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://tce.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zjg.zhoulong.xyz

[S18] C：命令行参数
来源：http://ukm.9152youxi.cn

int main(int argc, char **argv)
来源：http://njo.mhx1999.top

[S19] C：快速排序
来源：http://isz.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ozc.hesvh.cn

[S20] C：二分查找
来源：http://ino.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kbn.shuidangran.top

[S21] C：字符类别判断
来源：http://gyg.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zkb.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://hpt.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lep.dashuyun.cn

[S23] C：随机数
来源：http://hsv.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bdp.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://azi.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aac.quarkkingdee.top

[S25] C：内存拷贝
来源：http://kmy.guowangkeji.top

memcpy(dst, src, n);
来源：http://yhy.daria6918.cn

[S26] C：内存清零
来源：http://dvk.birdmap.top

memset(a, 0, sizeof a);
来源：http://dfc.yj20258888.top

[S27] C：定义常量
来源：http://izk.cashguo.top

const double PI = 3.14159;
来源：http://tkr.yj202588.top

[S28] C：静态变量
来源：http://fhp.cdnleiting.top

static int counter = 0;
来源：http://cbt.gaohongyu789.top

[S29] C：变参函数
来源：http://pcu.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cnz.mhx1999.top

[S30] C：头文件保护
来源：http://jaf.cdnleiting.top

#ifndef X_H
来源：http://axt.gaohongyu789.top

#define X_H
来源：http://dzb.xingfuxueyuan.xyz

#endif
来源：http://bxo.jianghu66.top

[S31] C++：Hello World
来源：http://teg.sweek.top

#include <iostream>
来源：http://rjs.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://oec.hesvh.cn

[S32] C++：字符串
来源：http://uqv.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://yth.yuanzhike.top

[S33] C++：vector 增删
来源：http://ftm.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lba.xylfe.cn

[S34] C++：遍历 vector
来源：http://fnk.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://ccg.nanxinkj.top

[S35] C++：map
来源：http://vfq.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gce.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://mzb.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ujy.nwbrower.top

[S37] C++：set
来源：http://dxr.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vec.ydjk.org.cn

[S38] C++：排序
来源：http://rep.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://wyy.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://zfv.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tiy.daxiang520.top

[S40] C++：查找元素
来源：http://tgo.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bpt.zdqjudy.top

[S41] C++：类与构造函数
来源：http://pii.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fsw.pycfn.com

[S42] C++：继承与虚函数
来源：http://wkr.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://kmr.haohaochexian.top

[S43] C++：智能指针
来源：http://fuz.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://sic.52xcode.cn

[S44] C++：引用传参
来源：http://tnm.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://ihj.zhixingplan.top

[S45] C++：lambda
来源：http://jzz.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://qzf.hcnkem.com

[S46] C++：函数模板
来源：http://aqx.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zoh.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://bms.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wqz.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://mei.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://yrf.hammf.cn

while (std::getline(in, line)) { }
来源：http://sot.yuanzhike.top

[S49] C++：写文件
来源：http://wta.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bbr.ydzc1.top

[S50] C++：格式化数字
来源：http://jrn.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://onq.yj20258888.top

[S51] C++：显式类型转换
来源：http://lqq.fzhhl.top

static_cast<double>(a) / b
来源：http://gwx.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://wfa.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://wqp.zhijiandao.cn

[S53] C++：移动语义
来源：http://snt.hammf.cn

std::vector<int> w = std::move(v);
来源：http://dhb.vqdsnc.cn

[S54] C++：异常处理
来源：http://jlb.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aji.guowangkeji.top

[S55] C++：结构化绑定
来源：http://amv.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dpn.fehbvm.com

[S56] C++：optional
来源：http://dxr.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fnm.daxiang520.top

[S57] C++：编译期常量
来源：http://iau.9152youxi.cn

constexpr int N = 10;
来源：http://ume.sjlbkw.cn

[S58] C++：命名空间
来源：http://wll.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://wgu.cdnleiting.top

[S59] C++：静态断言
来源：http://fqs.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ldo.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://vak.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://roc.meibo888.top

================================================================================
来源：http://cmx.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nvz.haohaochexian.top

================================================================================
来源：http://kte.yj202588.top

[T01] Kotlin：Hello World
来源：http://cgs.nwbrower.top

println("Hello")
来源：http://xye.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://wuo.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://brq.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://vih.yj202588.top

"值: $b"
来源：http://pea.jyoumei.cn

[T04] Kotlin：空安全
来源：http://jjr.redwolf501.top

val n: String? = null;  n?.length
来源：http://zwj.yonumen.top

[T05] Kotlin：when 表达式
来源：http://dvi.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://frq.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://dpe.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zol.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://qpb.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qtg.xuanzx.com

[T08] Kotlin：数据类
来源：http://qkc.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://cij.hysaishi.cn


<!-- 参考信息 -->