代发 wailian999

readonly PI=3.14
来源：http://now.ybcxt.top

[R04] 位置参数
来源：http://eyw.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wlm.fzhhl.top

[R05] 参数默认值
来源：http://mls.gaohongyu789.top

name="${1:-default}"
来源：http://fsg.jqgfzy.top

[R06] 判断命令是否存在
来源：http://swz.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zef.hnxiangtu.top

[R07] if 判断文件
来源：http://bxa.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mfb.ppjwa.cn

[R08] 数值比较
来源：http://sfe.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xta.hywenlv.cn

[R09] 字符串比较
来源：http://bne.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vpv.xinyue.icu

[R10] 正则匹配
来源：http://efb.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ouz.52xcode.cn

[R11] case 多分支
来源：http://wis.smart0.xyz

case "$1" in
来源：http://eze.jianghu66.top

start) echo "启动" ;;
来源：http://xvg.fengsongda.top

stop)  echo "停止" ;;
来源：http://bce.epnwcf.com

*)     echo "未知命令" ;;
来源：http://mvd.zdbjq.cn

esac
来源：http://jce.daria6918.cn

[R12] for 遍历文件
来源：http://cmo.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://jpv.uphjek.com

[R13] for 计数循环
来源：http://xxp.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ogc.fengsongda.top

[R14] C 风格 for
来源：http://eim.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zft.wangdashe.top

[R15] while 逐行读文件
来源：http://cem.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qyv.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://vmb.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qyi.c1oappe.top

[R17] 数组定义与取值
来源：http://zqy.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://trk.gaohongyu789.top

[R18] 遍历数组
来源：http://lcp.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gwp.zhaomingkeji.xyz

[R19] 数组长度
来源：http://fcb.hywenlv.cn

echo "${#arr[@]}"
来源：http://byc.yfazqb.com

[R20] 关联数组（字典）
来源：http://gze.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dlt.mhx1999.top

[R21] 字符串长度
来源：http://mlq.hesvh.cn

echo "${#s}"
来源：http://cxw.yueranfly.top

[R22] 截取子串
来源：http://gth.meibo888.top

echo "${s:0:5}"
来源：http://clo.9152youxi.cn

[R23] 字符串替换
来源：http://cqd.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tay.fktsv.cn

[R24] 大小写转换
来源：http://bua.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://nbb.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://leg.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://qyr.ydjk.org.cn

[R26] 命令替换
来源：http://nvw.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://mwe.chenjidiqi.icu

[R27] 算术展开
来源：http://cuq.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://joy.aizwys.cn

[R28] 浮点运算
来源：http://mde.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://tfb.zhijiandao.cn

[R29] 定义函数
来源：http://kdd.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jsm.jianghu66.top

[R30] 函数返回状态码
来源：http://suy.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://twz.xziqi.cn

[R31] 局部变量
来源：http://yue.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://azy.tianlin.xyz

[R32] 参数个数校验
来源：http://xbt.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dld.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://xow.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xfe.hammf.cn

[R34] 退出时清理
来源：http://rzd.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uwp.52xcode.cn

[R35] 后台执行并等待
来源：http://mzl.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://vid.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://yer.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://non.nanxinkj.top

[R37] 把输出赋给变量
来源：http://byn.hammf.cn

files=$(ls -1)
来源：http://aeb.sjlbkw.cn

[R38] 管道串联
来源：http://isi.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://nnn.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://stx.sufxvd.cn

cmd > out.log 2>&1
来源：http://erj.fzhhl.top

[R40] 追加写日志
来源：http://vrl.yuanzhike.top

echo "log" >> out.log
来源：http://apz.zhoulong.xyz

[R41] 丢弃输出
来源：http://oix.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://ypg.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://tka.cheryme.top

wc -l < a.txt
来源：http://qru.jqgufenzy.top

[R43] 按名字查找文件
来源：http://hou.yonumen.top

find . -name "*.log" -type f
来源：http://wnf.xylfe.cn

[R44] 按修改时间查找
来源：http://ozq.cdnleiting.top

find . -mtime -7 -type f
来源：http://gcj.chenjidiqi.icu

[R45] 批量删除
来源：http://dca.yuxming.cn

find . -name "*.tmp" -delete
来源：http://lev.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://ckf.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cpk.aibaodan.cn

[R47] sed 单行替换
来源：http://txe.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mks.jlsjyb.cn

[R48] awk 取指定列
来源：http://jrn.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://zav.aibaodan.cn

[R49] awk 带条件
来源：http://tem.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pny.sufxvd.cn

[R50] awk 求和
来源：http://zgn.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mzh.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://wll.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ura.shuidangran.top

[R52] 统计行数
来源：http://ulp.gogol.net.cn

wc -l a.txt
来源：http://bro.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://fkw.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sdm.hysaishi.cn

[R54] 比较两个文件
来源：http://yld.hysaishi.cn

diff a.txt b.txt
来源：http://ypp.hcnkem.com

[R55] 压缩与解压
来源：http://dek.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bbo.aizwys.cn

[R56] 远程拷贝
来源：http://giw.shzxlz.cn

scp file user@host:/path/
来源：http://ykr.shuidangran.top

[R57] 远程执行命令
来源：http://doo.ehwqpu.com

ssh user@host 'uptime'
来源：http://erw.zhixingplan.top

[R58] 下载文件
来源：http://qfs.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hrm.sweek.top

[R59] 发 POST JSON
来源：http://wpr.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fmx.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://nsz.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yvi.yongpay.top

[R61] 磁盘占用
来源：http://pae.jianghu66.top

df -h;  du -sh *
来源：http://fxq.yj202588.top

[R62] 找最占空间的文件
来源：http://efg.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://ctg.yueranfly.top

[R63] 内存与进程
来源：http://qiq.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://qxk.dashuyun.cn

[R64] 结束进程
来源：http://eyr.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://xem.yuxming.cn

[R65] 查看端口占用
来源：http://opk.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gab.guannengcc.top

[R66] 定时任务
来源：http://lgj.daria6918.cn

crontab -e;  crontab -l
来源：http://uye.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://gmp.jqgufenzy.top

openssl rand -hex 16
来源：http://rrv.xziqi.cn

[R68] 计算文件校验值
来源：http://vaz.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://krn.iojbl.cn

[R69] 生成随机密码
来源：http://dtx.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://xgp.quarkkingdee.top

[R70] 时间戳与互转
来源：http://ajj.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://smg.birdmap.top

[R71] 日期格式化
来源：http://jog.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lvk.cucudq.cn

[R72] 等待端口就绪
来源：http://trl.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uyd.iojbl.cn

[R73] 分割大日志
来源：http://kms.jianghu66.top

split -l 1000 big.log part_
来源：http://dou.jinqigfzy.top

[R74] 批量重命名
来源：http://hpl.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nnm.nanxuanxn.top

[R75] 导出环境变量
来源：http://piw.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://dpu.bbcook.cn

[R76] 使用临时文件
来源：http://mjh.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wef.fzhhl.top

[R77] 读取用户输入
来源：http://ckt.sxryk.cn

read -rp "请输入: " ans
来源：http://nsp.ybcxt.top

[R78] 交互式菜单
来源：http://yqh.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uub.xziqi.cn

[R79] 解析命令行选项
来源：http://xau.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hst.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://dyd.redwolf501.top

time ./run.sh
来源：http://wfw.guannengcc.top

================================================================================
来源：http://oxs.nwbrower.top

S. C / C++ 专题
来源：http://tqs.xingfuxueyuan.xyz

================================================================================
来源：http://qwj.snrcjt.cn

[S01] C：Hello World
来源：http://oge.uphjek.com

#include <stdio.h>
来源：http://avz.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yzk.redwolf501.top

[S02] C：变量与格式化输出
来源：http://yfe.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://zxn.fanxiaobao.xyz

[S03] C：读入整数
来源：http://nku.vehdjk.com

int x; scanf("%d", &x);
来源：http://ird.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://wwq.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://vtg.chenzaomai.com

[S05] C：字符串长度
来源：http://sin.yvedp.cn

strlen(s)
来源：http://ghf.yj20258.top

[S06] C：字符串比较
来源：http://vpz.yangfankeji.com

strcmp(a, b) == 0
来源：http://gkw.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://fjd.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ilz.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://pqm.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://khz.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://svy.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rih.sufxvd.cn

[S10] C：指针与解引用
来源：http://kwo.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://jly.cqqwz.cn

[S11] C：逐行读文件
来源：http://lrv.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://ice.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cqf.pycfn.com

fclose(f);
来源：http://oua.shanyushiyangtech.top

[S12] C：写文件
来源：http://zvp.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qxh.zhoulong.xyz

[S13] C：宏定义
来源：http://nmn.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yih.ctjpmb.com

[S14] C：枚举
来源：http://lhp.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://ggv.kuanghao11.cn

[S15] C：类型转换
来源：http://knt.gzhubu.top

(double) a / b
来源：http://qvk.hfpthk.cn

[S16] C：位操作置位
来源：http://cxa.shzxlz.cn

x |= (1 << 3);
来源：http://guh.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://qss.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kdl.pycfn.com

[S18] C：命令行参数
来源：http://iqr.yj20258888.top

int main(int argc, char **argv)
来源：http://lkf.bjfxy.top

[S19] C：快速排序
来源：http://fso.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mjp.fzhhl.top

[S20] C：二分查找
来源：http://lzk.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ypm.yueranfly.top

[S21] C：字符类别判断
来源：http://qnw.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eys.wangdashe.top

[S22] C：字符串转数字
来源：http://beq.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ris.svipenyu.cn

[S23] C：随机数
来源：http://kim.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qoz.cucudq.cn

[S24] C：获取本地时间
来源：http://dxe.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jmh.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://sce.yuanzhike.top

memcpy(dst, src, n);
来源：http://rkp.bbcook.cn

[S26] C：内存清零
来源：http://unr.havefunace.top

memset(a, 0, sizeof a);
来源：http://ghj.zhoulong.xyz

[S27] C：定义常量
来源：http://roh.bbcook.cn

const double PI = 3.14159;
来源：http://ayk.jiagoushi.top

[S28] C：静态变量
来源：http://ncj.shanyushiyangtech.top

static int counter = 0;
来源：http://qqq.gotoacloud.top

[S29] C：变参函数
来源：http://llq.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nis.zdbjq.cn

[S30] C：头文件保护
来源：http://ofu.yongpay.top

#ifndef X_H
来源：http://ibt.hysaishi.cn

#define X_H
来源：http://ehk.ydjk.org.cn

#endif
来源：http://mla.jiagoushi.top

[S31] C++：Hello World
来源：http://nrq.zhengqikj.top

#include <iostream>
来源：http://xos.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://hyv.dianchejie.cn

[S32] C++：字符串
来源：http://vkv.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://ndo.jyoumei.cn

[S33] C++：vector 增删
来源：http://uot.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sxu.guowangkeji.top

[S34] C++：遍历 vector
来源：http://ers.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://xgs.zhengqikj.top

[S35] C++：map
来源：http://lcl.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://umy.tarul.cn

[S36] C++：unordered_map
来源：http://pus.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uwx.iojbl.cn

[S37] C++：set
来源：http://ocz.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mjp.gaohongyu789.top

[S38] C++：排序
来源：http://taf.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://jkc.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://rav.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tkl.quarkkingdee.top

[S40] C++：查找元素
来源：http://alc.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lie.guannengcc.top

[S41] C++：类与构造函数
来源：http://dal.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fbf.yvedp.cn

[S42] C++：继承与虚函数
来源：http://mfx.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://qrr.jyoumei.cn

[S43] C++：智能指针
来源：http://fns.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://hmy.gaohongyu789.top

[S44] C++：引用传参
来源：http://gqa.hesvh.cn

void inc(int &x) { ++x; }
来源：http://kwa.sweek.top

[S45] C++：lambda
来源：http://udl.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://mea.sysykeji.top

[S46] C++：函数模板
来源：http://jhg.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wwj.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://gtf.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wxm.cheryme.top

[S48] C++：逐行读文件
来源：http://zzk.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://puv.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://afq.svipenyu.cn

[S49] C++：写文件
来源：http://wmq.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uaw.zhixingplan.top

[S50] C++：格式化数字
来源：http://eyd.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vub.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://bwy.daxiang520.top

static_cast<double>(a) / b
来源：http://fvo.meibo888.top

[S52] C++：const 与 noexcept
来源：http://cdj.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://pls.hammf.cn

[S53] C++：移动语义
来源：http://lhl.yj20258.top

std::vector<int> w = std::move(v);
来源：http://ppr.iojbl.cn

[S54] C++：异常处理
来源：http://pti.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mgb.guannengcc.top

[S55] C++：结构化绑定
来源：http://vxo.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xcm.hfpthk.cn

[S56] C++：optional
来源：http://cya.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://njv.xuanzx.com

[S57] C++：编译期常量
来源：http://jxh.zhijiandao.cn

constexpr int N = 10;
来源：http://wun.guowangkeji.top

[S58] C++：命名空间
来源：http://uus.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://seu.feifeiyinyue.top

[S59] C++：静态断言
来源：http://bjv.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wza.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://man.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uye.hfpthk.cn

================================================================================
来源：http://mwk.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qll.jinghuilouyu.cn

================================================================================
来源：http://xaw.cucudq.cn

[T01] Kotlin：Hello World
来源：http://dmr.gzhubu.top

println("Hello")
来源：http://vso.xinyue.icu

[T02] Kotlin：变量
来源：http://eie.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://apt.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://deo.tian-w.cn

"值: $b"
来源：http://rpt.ehwqpu.com

[T04] Kotlin：空安全
来源：http://nis.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://cby.tianlin.xyz


<!-- 参考信息 -->