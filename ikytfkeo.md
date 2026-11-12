代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jmt.dashuyun.cn

[R08] 数值比较
来源：http://lem.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ssi.yanxiufei.cn

[R09] 字符串比较
来源：http://leh.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dyd.xziqi.cn

[R10] 正则匹配
来源：http://imz.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cjv.dianchejie.cn

[R11] case 多分支
来源：http://nxg.hammf.cn

case "$1" in
来源：http://tvh.jinqigufen.top

start) echo "启动" ;;
来源：http://idx.jqgfzy.top

stop)  echo "停止" ;;
来源：http://vqq.gzhubu.top

*)     echo "未知命令" ;;
来源：http://yyc.yj202588.top

esac
来源：http://jto.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://mft.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://awp.hcnkem.com

[R13] for 计数循环
来源：http://ulq.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://xuc.iojbl.cn

[R14] C 风格 for
来源：http://ogq.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yoa.cheryme.top

[R15] while 逐行读文件
来源：http://ast.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqh.sysykeji.top

[R16] until 等待条件
来源：http://mhx.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dfs.sweek.top

[R17] 数组定义与取值
来源：http://imv.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qnj.fzhhl.top

[R18] 遍历数组
来源：http://iic.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://acs.shanyushiyangkeji.top

[R19] 数组长度
来源：http://xwx.yangfankeji.com

echo "${#arr[@]}"
来源：http://doy.wangdashe.top

[R20] 关联数组（字典）
来源：http://zjx.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://neu.vqdsnc.cn

[R21] 字符串长度
来源：http://atb.fzhhl.top

echo "${#s}"
来源：http://iru.zhixingplan.top

[R22] 截取子串
来源：http://xxw.gaohongyu789.top

echo "${s:0:5}"
来源：http://jju.guannengcc.top

[R23] 字符串替换
来源：http://yvy.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zyc.uphjek.com

[R24] 大小写转换
来源：http://abz.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://tsv.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://lty.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nej.zhengqikj.top

[R26] 命令替换
来源：http://vyx.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://usd.hfpthk.cn

[R27] 算术展开
来源：http://nht.epnwcf.com

echo $((1 + 2 * 3))
来源：http://btg.jlsjyb.cn

[R28] 浮点运算
来源：http://bvt.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://yrr.zycfv.cn

[R29] 定义函数
来源：http://chx.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eid.tanke756.top

[R30] 函数返回状态码
来源：http://hvt.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://muv.aibaodan.cn

[R31] 局部变量
来源：http://xsh.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://fcj.epnwcf.com

[R32] 参数个数校验
来源：http://oql.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqp.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://vrd.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://voo.chenzaomai.com

[R34] 退出时清理
来源：http://sjm.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tkl.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://fns.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fww.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://hxu.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hst.sufxvd.cn

[R37] 把输出赋给变量
来源：http://qzg.fehbvm.com

files=$(ls -1)
来源：http://vnb.cucudq.cn

[R38] 管道串联
来源：http://niw.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://baq.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://bzs.smart0.xyz

cmd > out.log 2>&1
来源：http://fzc.fktsv.cn

[R40] 追加写日志
来源：http://qzp.chenlongwang.top

echo "log" >> out.log
来源：http://bci.jyoumei.cn

[R41] 丢弃输出
来源：http://chi.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://qig.yuanzhike.top

[R42] 输入重定向
来源：http://usr.gotoacloud.top

wc -l < a.txt
来源：http://qvm.gaohongyu789.top

[R43] 按名字查找文件
来源：http://ewe.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://kbd.hnqzz.top

[R44] 按修改时间查找
来源：http://pvk.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://fzo.havefunace.top

[R45] 批量删除
来源：http://iik.yj20258888.top

find . -name "*.tmp" -delete
来源：http://ksq.nanxinkj.top

[R46] 递归替换文件内容
来源：http://qiy.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hnc.cdnleiting.top

[R47] sed 单行替换
来源：http://lia.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xxy.shangyingyoupin.top

[R48] awk 取指定列
来源：http://xfv.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://iqv.shanyushiyangtech.top

[R49] awk 带条件
来源：http://yia.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://izd.hammf.cn

[R50] awk 求和
来源：http://bzm.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://npf.ctjpmb.com

[R51] 排序去重取前几
来源：http://ipt.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rma.yuxming.cn

[R52] 统计行数
来源：http://cei.zdbjq.cn

wc -l a.txt
来源：http://out.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://hun.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pqp.zhixingplan.top

[R54] 比较两个文件
来源：http://pdd.tian-w.cn

diff a.txt b.txt
来源：http://vcs.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://fkr.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ceh.vehdjk.com

[R56] 远程拷贝
来源：http://xzc.jlsjyb.cn

scp file user@host:/path/
来源：http://gni.epnwcf.com

[R57] 远程执行命令
来源：http://dly.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://jsm.yongpay.top

[R58] 下载文件
来源：http://lfp.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpt.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://zlb.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qbr.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://aof.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uej.havefunace.top

[R61] 磁盘占用
来源：http://ntc.jianghu66.top

df -h;  du -sh *
来源：http://xbu.0kj1m.cn

[R62] 找最占空间的文件
来源：http://jsp.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://dit.jianghu66.top

[R63] 内存与进程
来源：http://hxr.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://qsj.zhoulong.xyz

[R64] 结束进程
来源：http://lfs.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://ate.ybcxt.top

[R65] 查看端口占用
来源：http://vnn.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://voy.vqdsnc.cn

[R66] 定时任务
来源：http://pzi.hnxiangtu.top

crontab -e;  crontab -l
来源：http://ywh.fehbvm.com

[R67] 生成随机十六进制串
来源：http://nbr.yuxming.cn

openssl rand -hex 16
来源：http://qmp.sweek.top

[R68] 计算文件校验值
来源：http://wmo.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://bxz.andypj.xyz

[R69] 生成随机密码
来源：http://bik.sweek.top

head -c 16 /dev/urandom | base64
来源：http://ykg.zdqjudy.top

[R70] 时间戳与互转
来源：http://iqz.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://cxz.pycfn.com

[R71] 日期格式化
来源：http://fjl.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nyf.yj20258.top

[R72] 等待端口就绪
来源：http://tiw.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ddk.yj20258888.top

[R73] 分割大日志
来源：http://ulz.cqqwz.cn

split -l 1000 big.log part_
来源：http://lby.hnxiangtu.top

[R74] 批量重命名
来源：http://bax.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ejv.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://cpf.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://gea.tanke756.top

[R76] 使用临时文件
来源：http://ejw.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dtx.xylfe.cn

[R77] 读取用户输入
来源：http://spl.daxiang520.top

read -rp "请输入: " ans
来源：http://hfw.yj20258888.top

[R78] 交互式菜单
来源：http://clv.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nsl.fengsongda.top

[R79] 解析命令行选项
来源：http://kfs.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iul.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://oqa.pengpengdd.cyou

time ./run.sh
来源：http://hzb.wangdashe.top

================================================================================
来源：http://eud.wangshuangyany.cn

S. C / C++ 专题
来源：http://fud.guowangkeji.top

================================================================================
来源：http://yct.zhongyouzk.top

[S01] C：Hello World
来源：http://bip.redwolf501.top

#include <stdio.h>
来源：http://swq.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://sxn.yongpay.top

[S02] C：变量与格式化输出
来源：http://gdt.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://mdm.hysaishi.cn

[S03] C：读入整数
来源：http://xmo.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://sgb.zdqjudy.top

[S04] C：字符串复制
来源：http://gpl.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://iuw.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://wmw.jinyuanbaomall.cn

strlen(s)
来源：http://wun.dashuyun.cn

[S06] C：字符串比较
来源：http://cho.sweek.top

strcmp(a, b) == 0
来源：http://niq.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://qjb.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qhk.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://vbb.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ruy.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://ztw.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zdl.52xcode.cn

[S10] C：指针与解引用
来源：http://csn.meibo888.top

int *p = &a;  *p = 5;
来源：http://qlu.zdbjq.cn

[S11] C：逐行读文件
来源：http://jfn.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://yrs.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lxf.shanyushiyangkeji.top

fclose(f);
来源：http://fsf.jianghu66.top

[S12] C：写文件
来源：http://cap.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lwf.yfazqb.com

[S13] C：宏定义
来源：http://tvq.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://izl.snrcjt.cn

[S14] C：枚举
来源：http://bue.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://jxm.gogol.net.cn

[S15] C：类型转换
来源：http://uch.jinghuilouyu.cn

(double) a / b
来源：http://wts.cucudq.cn

[S16] C：位操作置位
来源：http://ths.pengpengdd.cyou

x |= (1 << 3);
来源：http://gox.uphjek.com

[S17] C：安全拼接字符串
来源：http://vbz.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://avv.hnqzz.top

[S18] C：命令行参数
来源：http://moj.0kj1m.cn

int main(int argc, char **argv)
来源：http://byt.dashuyun.cn

[S19] C：快速排序
来源：http://kzf.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://qsj.cashguo.top

[S20] C：二分查找
来源：http://pun.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qcn.bbcook.cn

[S21] C：字符类别判断
来源：http://kib.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vrv.jqgfzy.top

[S22] C：字符串转数字
来源：http://ski.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://wvl.ehwqpu.com

[S23] C：随机数
来源：http://yfi.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ajm.jlsjyb.cn

[S24] C：获取本地时间
来源：http://ghz.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vrk.gotoacloud.top

[S25] C：内存拷贝
来源：http://sxg.kuanghao11.cn

memcpy(dst, src, n);
来源：http://sel.guowangkeji.top

[S26] C：内存清零
来源：http://bri.nwbrower.top

memset(a, 0, sizeof a);
来源：http://cnw.xuetiantiany.cn

[S27] C：定义常量
来源：http://oya.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://pye.jyoumei.cn

[S28] C：静态变量
来源：http://xta.jinghuilouyu.cn

static int counter = 0;
来源：http://rhk.yuanzhike.top

[S29] C：变参函数
来源：http://eqt.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oql.zdqjudy.top

[S30] C：头文件保护
来源：http://kpv.epnwcf.com

#ifndef X_H
来源：http://hsi.ppjwa.cn

#define X_H
来源：http://apt.ppjwa.cn

#endif
来源：http://spy.yuxming.cn

[S31] C++：Hello World
来源：http://acv.pycfn.com

#include <iostream>
来源：http://fwf.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://dgc.hysaishi.cn

[S32] C++：字符串
来源：http://dtz.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://hux.jlsjyb.cn

[S33] C++：vector 增删
来源：http://qpi.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pka.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://ocx.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://rcv.cqqwz.cn

[S35] C++：map
来源：http://kiu.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bzo.ehwqpu.com

[S36] C++：unordered_map
来源：http://rhy.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zyj.yvedp.cn

[S37] C++：set
来源：http://oci.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uxt.guowangkeji.top

[S38] C++：排序
来源：http://ebu.tarul.cn

std::sort(v.begin(), v.end());
来源：http://wcd.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://pbh.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wce.redwolf501.top

[S40] C++：查找元素
来源：http://tgh.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kjm.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://hyd.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mqc.52xcode.cn

[S42] C++：继承与虚函数
来源：http://etx.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://rje.feifeiyinyue.top

[S43] C++：智能指针
来源：http://pxh.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://puu.dianchejie.cn

[S44] C++：引用传参
来源：http://inn.ydzc1.top

void inc(int &x) { ++x; }
来源：http://uxa.uphjek.com

[S45] C++：lambda
来源：http://mxq.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://gzc.0kj1m.cn

[S46] C++：函数模板
来源：http://qah.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rdg.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://hko.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dyy.ehwqpu.com

[S48] C++：逐行读文件
来源：http://qns.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cby.meibo888.top

while (std::getline(in, line)) { }
来源：http://ozw.daxiang520.top

[S49] C++：写文件
来源：http://ixp.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nia.ppjwa.cn

[S50] C++：格式化数字
来源：http://nvs.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://npr.jyoumei.cn

[S51] C++：显式类型转换
来源：http://bfd.fzhhl.top

static_cast<double>(a) / b
来源：http://acm.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://jzj.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://tbh.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://kpn.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://rvg.fehbvm.com

[S54] C++：异常处理
来源：http://uom.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fky.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://rrd.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qwc.zhixingplan.top

[S56] C++：optional
来源：http://bih.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ulv.ehwqpu.com

[S57] C++：编译期常量
来源：http://yba.tanke756.top

constexpr int N = 10;
来源：http://gzb.tanke756.top

[S58] C++：命名空间
来源：http://eyv.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://iud.jiagoushi.top

[S59] C++：静态断言
来源：http://hdy.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lrd.tarul.cn

[S60] C++：遍历并删除元素
来源：http://mvy.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zmh.vehdjk.com

================================================================================
来源：http://yzb.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eme.jyoumei.cn

================================================================================
来源：http://hdi.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://zjm.jinqigfzy.top

println("Hello")
来源：http://rnv.vqdsnc.cn

[T02] Kotlin：变量
来源：http://cls.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uui.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://hjj.hammf.cn

"值: $b"
来源：http://vgg.pycfn.com

[T04] Kotlin：空安全
来源：http://sjh.fzhhl.top

val n: String? = null;  n?.length
来源：http://nkq.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://mmv.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xjo.uphjek.com

[T06] Kotlin：集合映射
来源：http://pcq.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pni.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://fbu.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tdx.sxryk.cn

[T08] Kotlin：数据类
来源：http://vjz.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://hvq.guannengcc.top


<!-- 参考信息 -->