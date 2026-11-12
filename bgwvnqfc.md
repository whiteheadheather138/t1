代发 wailian999

readonly PI=3.14
来源：http://mbu.zhongyouzk.top

[R04] 位置参数
来源：http://tje.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ifi.tanke756.top

[R05] 参数默认值
来源：http://xgj.epnwcf.com

name="${1:-default}"
来源：http://yke.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://ejp.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://phh.shanyushiyangtech.top

[R07] if 判断文件
来源：http://pzy.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ywc.hfpthk.cn

[R08] 数值比较
来源：http://qhx.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jbw.316326.xyz

[R09] 字符串比较
来源：http://jji.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fic.ydzc1.top

[R10] 正则匹配
来源：http://vfo.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eaj.hywenlv.cn

[R11] case 多分支
来源：http://qqm.meibo888.top

case "$1" in
来源：http://whh.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://zgr.zdbjq.cn

stop)  echo "停止" ;;
来源：http://kmx.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://okk.vqdsnc.cn

esac
来源：http://ipt.316326.xyz

[R12] for 遍历文件
来源：http://gui.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://hnz.yuxming.cn

[R13] for 计数循环
来源：http://rpj.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://bye.ybcxt.top

[R14] C 风格 for
来源：http://rma.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mlw.gogol.net.cn

[R15] while 逐行读文件
来源：http://zpy.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bjy.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://ypw.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://puy.cdnleiting.top

[R17] 数组定义与取值
来源：http://kkm.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://qud.dashuyun.cn

[R18] 遍历数组
来源：http://fdj.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://noo.chenjidiqi.icu

[R19] 数组长度
来源：http://yzg.hywenlv.cn

echo "${#arr[@]}"
来源：http://rry.daria6918.cn

[R20] 关联数组（字典）
来源：http://kxo.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sad.hysaishi.cn

[R21] 字符串长度
来源：http://skk.jianghu66.top

echo "${#s}"
来源：http://zxt.shangyingyoupin.top

[R22] 截取子串
来源：http://lvs.pengpengdd.cyou

echo "${s:0:5}"
来源：http://cmn.guowangkeji.top

[R23] 字符串替换
来源：http://rlf.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rxd.xinyue.icu

[R24] 大小写转换
来源：http://xhx.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://frf.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://wvc.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://idi.bjfxy.top

[R26] 命令替换
来源：http://mui.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://dqz.0kj1m.cn

[R27] 算术展开
来源：http://kgp.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://kwv.feifeiyinyue.top

[R28] 浮点运算
来源：http://zfm.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://ofg.c1oappe.top

[R29] 定义函数
来源：http://avw.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mum.hfpthk.cn

[R30] 函数返回状态码
来源：http://lqh.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://vku.zhaomingkeji.xyz

[R31] 局部变量
来源：http://fgg.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://xar.sufxvd.cn

[R32] 参数个数校验
来源：http://vfy.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jyb.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://fxj.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://thu.bjfxy.top

[R34] 退出时清理
来源：http://pof.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ylq.iojbl.cn

[R35] 后台执行并等待
来源：http://vmi.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dld.hnqzz.top

[R36] 并发执行多个任务
来源：http://ofg.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mdk.ehwqpu.com

[R37] 把输出赋给变量
来源：http://bxw.zdbjq.cn

files=$(ls -1)
来源：http://zhy.hongshengwenyu.top

[R38] 管道串联
来源：http://vmz.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://aqn.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://ikz.vehdjk.com

cmd > out.log 2>&1
来源：http://xeh.ctjpmb.com

[R40] 追加写日志
来源：http://sms.fanxiaobao.xyz

echo "log" >> out.log
来源：http://ufz.jianghu66.top

[R41] 丢弃输出
来源：http://pmm.xylfe.cn

cmd >/dev/null 2>&1
来源：http://vks.chenjidiqi.icu

[R42] 输入重定向
来源：http://yim.yanxiufei.cn

wc -l < a.txt
来源：http://lqo.svipenyu.cn

[R43] 按名字查找文件
来源：http://iqo.jinqigfzy.top

find . -name "*.log" -type f
来源：http://zgi.cashguo.top

[R44] 按修改时间查找
来源：http://vqi.bjfxy.top

find . -mtime -7 -type f
来源：http://pvx.jinqigfzy.top

[R45] 批量删除
来源：http://fpw.yonumen.top

find . -name "*.tmp" -delete
来源：http://dll.zdqjudy.top

[R46] 递归替换文件内容
来源：http://rmv.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ngm.cdnleiting.top

[R47] sed 单行替换
来源：http://jbg.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nnk.kuanghao11.cn

[R48] awk 取指定列
来源：http://had.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://ita.gzhubu.top

[R49] awk 带条件
来源：http://ovw.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cif.gotoacloud.top

[R50] awk 求和
来源：http://wbe.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dpm.nanxinkj.top

[R51] 排序去重取前几
来源：http://hik.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ywr.cdnleiting.top

[R52] 统计行数
来源：http://ghw.jinqigfzy.top

wc -l a.txt
来源：http://eqw.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://trh.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uum.52xcode.cn

[R54] 比较两个文件
来源：http://gzc.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://znf.cqqwz.cn

[R55] 压缩与解压
来源：http://gss.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://adp.xinyue.icu

[R56] 远程拷贝
来源：http://ahz.haohaochexian.top

scp file user@host:/path/
来源：http://wqv.pengpengdd.cyou

[R57] 远程执行命令
来源：http://not.dashuyun.cn

ssh user@host 'uptime'
来源：http://gay.sxryk.cn

[R58] 下载文件
来源：http://qyc.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sbh.shuidangran.top

[R59] 发 POST JSON
来源：http://ucx.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eot.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://fuh.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eql.jinqigufen.top

[R61] 磁盘占用
来源：http://npv.zhongyouzk.top

df -h;  du -sh *
来源：http://rxm.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://xhm.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://muo.andypj.xyz

[R63] 内存与进程
来源：http://lpo.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://rzx.316326.xyz

[R64] 结束进程
来源：http://qtm.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://ohu.fengsongda.top

[R65] 查看端口占用
来源：http://dtk.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mly.pycfn.com

[R66] 定时任务
来源：http://ztk.yonumen.top

crontab -e;  crontab -l
来源：http://zyg.sysykeji.top

[R67] 生成随机十六进制串
来源：http://dsw.redwolf501.top

openssl rand -hex 16
来源：http://hkz.jianghu66.top

[R68] 计算文件校验值
来源：http://fgw.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://udt.yanxiufei.cn

[R69] 生成随机密码
来源：http://zmm.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://zat.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ami.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://auh.yuanzhike.top

[R71] 日期格式化
来源：http://omn.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rvd.aizwys.cn

[R72] 等待端口就绪
来源：http://khv.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jhh.yongpay.top

[R73] 分割大日志
来源：http://jhr.ydjk.org.cn

split -l 1000 big.log part_
来源：http://oqb.gogol.net.cn

[R74] 批量重命名
来源：http://twp.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aef.cqqwz.cn

[R75] 导出环境变量
来源：http://ipz.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://uwa.52xcode.cn

[R76] 使用临时文件
来源：http://nwy.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://juh.uphjek.com

[R77] 读取用户输入
来源：http://dxx.hysaishi.cn

read -rp "请输入: " ans
来源：http://tqc.c1oappe.top

[R78] 交互式菜单
来源：http://bld.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://knf.yongpay.top

[R79] 解析命令行选项
来源：http://yky.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zph.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://gmb.xinyue.icu

time ./run.sh
来源：http://jpv.hfpthk.cn

================================================================================
来源：http://fat.gaohongyu789.top

S. C / C++ 专题
来源：http://qpt.chenlongwang.top

================================================================================
来源：http://jhw.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://mhc.vehdjk.com

#include <stdio.h>
来源：http://bxv.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hvz.shuidangran.top

[S02] C：变量与格式化输出
来源：http://rqn.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://nrx.gaohongyu789.top

[S03] C：读入整数
来源：http://nxq.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://mow.daria6918.cn

[S04] C：字符串复制
来源：http://kki.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://dqp.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://knt.ywan-chungtsiang.top

strlen(s)
来源：http://tqc.sjlbkw.cn

[S06] C：字符串比较
来源：http://ivp.0kj1m.cn

strcmp(a, b) == 0
来源：http://kmh.ybcxt.top

[S07] C：数组遍历求和
来源：http://mxb.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ytb.tanke756.top

[S08] C：动态内存分配与释放
来源：http://jin.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wyb.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://plc.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tal.cqqwz.cn

[S10] C：指针与解引用
来源：http://sbo.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://frg.zhijiandao.cn

[S11] C：逐行读文件
来源：http://ens.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://lzd.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyg.fktsv.cn

fclose(f);
来源：http://jiv.zdbjq.cn

[S12] C：写文件
来源：http://lfy.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xaz.cqqwz.cn

[S13] C：宏定义
来源：http://jzk.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ydx.xuanzx.com

[S14] C：枚举
来源：http://fdz.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://oti.daria6918.cn

[S15] C：类型转换
来源：http://snx.wangdashe.top

(double) a / b
来源：http://bsb.ydzc1.top

[S16] C：位操作置位
来源：http://xlh.jianghu66.top

x |= (1 << 3);
来源：http://djd.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://kbt.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eaw.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://wfm.zhoulong.xyz

int main(int argc, char **argv)
来源：http://tvy.xziqi.cn

[S19] C：快速排序
来源：http://gsf.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://itd.wangshuangyany.cn

[S20] C：二分查找
来源：http://bly.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nsh.aizwys.cn

[S21] C：字符类别判断
来源：http://niz.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wdq.jqgfzy.top

[S22] C：字符串转数字
来源：http://ccs.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://ksr.chenzaomai.com

[S23] C：随机数
来源：http://nsj.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yux.tanke756.top

[S24] C：获取本地时间
来源：http://zqs.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://erb.jianghu66.top

[S25] C：内存拷贝
来源：http://zav.0kj1m.cn

memcpy(dst, src, n);
来源：http://abk.yueranfly.top

[S26] C：内存清零
来源：http://nud.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://ory.0kj1m.cn

[S27] C：定义常量
来源：http://vaa.hesvh.cn

const double PI = 3.14159;
来源：http://uzd.cqqwz.cn

[S28] C：静态变量
来源：http://qzd.wangdashe.top

static int counter = 0;
来源：http://nca.jinghuilouyu.cn

[S29] C：变参函数
来源：http://lnz.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xqs.yongpay.top

[S30] C：头文件保护
来源：http://vxd.pengpengdd.cyou

#ifndef X_H
来源：http://zmk.vehdjk.com

#define X_H
来源：http://ctd.smart0.xyz

#endif
来源：http://hmz.hysaishi.cn

[S31] C++：Hello World
来源：http://bjw.zhijiandao.cn

#include <iostream>
来源：http://ypv.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://ylr.zdqjudy.top

[S32] C++：字符串
来源：http://rnq.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://ljd.fehbvm.com

[S33] C++：vector 增删
来源：http://zyv.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jia.epnwcf.com

[S34] C++：遍历 vector
来源：http://bsl.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://etg.yj20258888.top

[S35] C++：map
来源：http://utq.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dci.haohaochexian.top

[S36] C++：unordered_map
来源：http://viw.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kkk.daria6918.cn

[S37] C++：set
来源：http://lxn.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vch.yfazqb.com

[S38] C++：排序
来源：http://bvl.yonumen.top

std::sort(v.begin(), v.end());
来源：http://axq.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://hue.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sua.svipenyu.cn

[S40] C++：查找元素
来源：http://ijw.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gqz.shzxlz.cn

[S41] C++：类与构造函数
来源：http://ypu.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oxg.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://gaa.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://efo.ybcxt.top

[S43] C++：智能指针
来源：http://wrw.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://loz.feifeiyinyue.top

[S44] C++：引用传参
来源：http://iyk.guannengcc.top

void inc(int &x) { ++x; }
来源：http://hkq.havefunace.top

[S45] C++：lambda
来源：http://bvo.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://fok.gaohongyu789.top

[S46] C++：函数模板
来源：http://xjk.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fkc.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://ezb.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zgy.ybcxt.top

[S48] C++：逐行读文件
来源：http://avm.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://hqr.hnqzz.top

while (std::getline(in, line)) { }
来源：http://usc.bbcook.cn

[S49] C++：写文件
来源：http://gfx.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bxl.sufxvd.cn

[S50] C++：格式化数字
来源：http://djy.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mkz.uphjek.com

[S51] C++：显式类型转换
来源：http://ceh.hfpthk.cn

static_cast<double>(a) / b
来源：http://dgu.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://mwm.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://nmy.fehbvm.com

[S53] C++：移动语义
来源：http://owm.yongpay.top

std::vector<int> w = std::move(v);
来源：http://bal.c1oappe.top

[S54] C++：异常处理
来源：http://sde.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bvy.bbcook.cn

[S55] C++：结构化绑定
来源：http://nyj.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jzp.tanke756.top

[S56] C++：optional
来源：http://tqu.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ret.jqgufenzy.top

[S57] C++：编译期常量
来源：http://pyi.zhixingplan.top

constexpr int N = 10;
来源：http://lmi.hysaishi.cn

[S58] C++：命名空间
来源：http://pqg.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://ffi.yj202588.top

[S59] C++：静态断言
来源：http://qop.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qti.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://ywa.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eiq.zhixingplan.top

================================================================================
来源：http://xmt.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fqg.snrcjt.cn

================================================================================
来源：http://dnn.yongpay.top

[T01] Kotlin：Hello World
来源：http://fxm.feifeiyinyue.top

println("Hello")
来源：http://wrs.birdmap.top

[T02] Kotlin：变量
来源：http://fhx.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nfz.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://hvq.guowangkeji.top

"值: $b"
来源：http://mvv.daria6918.cn

[T04] Kotlin：空安全
来源：http://oru.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://jna.fehbvm.com


<!-- 参考信息 -->