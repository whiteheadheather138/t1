代发 wailian999

R. Bash 专题
来源：http://uas.cheryme.top

================================================================================
来源：http://cht.jqgfzy.top

[R01] shebang 与严格模式
来源：http://xqn.jinqigufen.top

#!/usr/bin/env bash
来源：http://prl.pengpengdd.cyou

set -euo pipefail
来源：http://nds.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://btd.zdqjudy.top

name="Tom"; echo "$name"
来源：http://drf.quarkkingdee.top

[R03] 只读变量
来源：http://eag.haohaochexian.top

readonly PI=3.14
来源：http://vvv.gogol.net.cn

[R04] 位置参数
来源：http://vxi.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://spq.iojbl.cn

[R05] 参数默认值
来源：http://mkf.cdnleiting.top

name="${1:-default}"
来源：http://ywj.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://crx.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wpf.jianghu66.top

[R07] if 判断文件
来源：http://ksp.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pms.yonumen.top

[R08] 数值比较
来源：http://ukd.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ugc.yj20258.top

[R09] 字符串比较
来源：http://hmd.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yys.zdqjudy.top

[R10] 正则匹配
来源：http://jpn.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eln.sxryk.cn

[R11] case 多分支
来源：http://hlb.gotoacloud.top

case "$1" in
来源：http://wwv.pengpengdd.cyou

start) echo "启动" ;;
来源：http://jjq.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://stb.gzhubu.top

*)     echo "未知命令" ;;
来源：http://jek.0kj1m.cn

esac
来源：http://iqz.zhongyouzk.top

[R12] for 遍历文件
来源：http://eun.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://onk.zhiwuduotai.top

[R13] for 计数循环
来源：http://det.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://eqb.nanxuanxn.top

[R14] C 风格 for
来源：http://oww.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ppg.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://dkx.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxm.shzxlz.cn

[R16] until 等待条件
来源：http://jpm.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kja.snrcjt.cn

[R17] 数组定义与取值
来源：http://jec.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://mwg.shanyushiyangtech.top

[R18] 遍历数组
来源：http://avy.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qdn.hammf.cn

[R19] 数组长度
来源：http://pwf.hcnkem.com

echo "${#arr[@]}"
来源：http://mjv.smart0.xyz

[R20] 关联数组（字典）
来源：http://bnf.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jyh.ydjk.org.cn

[R21] 字符串长度
来源：http://pnf.pengpengdd.cyou

echo "${#s}"
来源：http://ddh.jqgufenzy.top

[R22] 截取子串
来源：http://qvy.cqqwz.cn

echo "${s:0:5}"
来源：http://asl.svipenyu.cn

[R23] 字符串替换
来源：http://jdc.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ksn.pycfn.com

[R24] 大小写转换
来源：http://jrk.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://unv.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://vrb.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://asp.dashuyun.cn

[R26] 命令替换
来源：http://qom.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://mkf.yueranfly.top

[R27] 算术展开
来源：http://akq.guannengcc.top

echo $((1 + 2 * 3))
来源：http://bne.ehwqpu.com

[R28] 浮点运算
来源：http://htu.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://ykx.cashguo.top

[R29] 定义函数
来源：http://stx.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hcg.kuanghao11.cn

[R30] 函数返回状态码
来源：http://gyw.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://hxq.fzhhl.top

[R31] 局部变量
来源：http://vqp.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://utf.tian-w.cn

[R32] 参数个数校验
来源：http://xhe.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://csn.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://mzm.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bem.yanxiufei.cn

[R34] 退出时清理
来源：http://jha.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nty.cucudq.cn

[R35] 后台执行并等待
来源：http://yxx.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wez.jiagoushi.top

[R36] 并发执行多个任务
来源：http://bhj.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wms.chenlongwang.top

[R37] 把输出赋给变量
来源：http://hrf.cdnleiting.top

files=$(ls -1)
来源：http://phk.meibo888.top

[R38] 管道串联
来源：http://zwg.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://dtr.tarul.cn

[R39] 重定向标准输出与错误
来源：http://beq.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://mkl.wangdashe.top

[R40] 追加写日志
来源：http://pva.jqgfzy.top

echo "log" >> out.log
来源：http://phv.quarkkingdee.top

[R41] 丢弃输出
来源：http://wpq.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://cbk.daria6918.cn

[R42] 输入重定向
来源：http://qzr.ybcxt.top

wc -l < a.txt
来源：http://hvm.uphjek.com

[R43] 按名字查找文件
来源：http://ubl.zhijiandao.cn

find . -name "*.log" -type f
来源：http://zim.bbcook.cn

[R44] 按修改时间查找
来源：http://lxe.pycfn.com

find . -mtime -7 -type f
来源：http://zcv.tanke756.top

[R45] 批量删除
来源：http://xjc.fktsv.cn

find . -name "*.tmp" -delete
来源：http://xdw.ybcxt.top

[R46] 递归替换文件内容
来源：http://wya.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zwn.epnwcf.com

[R47] sed 单行替换
来源：http://mne.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://zcx.jqgfzy.top

[R48] awk 取指定列
来源：http://mml.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://fnj.ydjk.org.cn

[R49] awk 带条件
来源：http://xqf.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bfi.cheryme.top

[R50] awk 求和
来源：http://pzf.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://lro.yongpay.top

[R51] 排序去重取前几
来源：http://sbx.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wte.havefunace.top

[R52] 统计行数
来源：http://hia.gzhubu.top

wc -l a.txt
来源：http://jrh.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://lps.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://puv.zhengqikj.top

[R54] 比较两个文件
来源：http://hbe.zhengqikj.top

diff a.txt b.txt
来源：http://bzb.fzhhl.top

[R55] 压缩与解压
来源：http://mqd.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kod.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://nuf.sxryk.cn

scp file user@host:/path/
来源：http://avy.fehbvm.com

[R57] 远程执行命令
来源：http://mhk.sjlbkw.cn

ssh user@host 'uptime'
来源：http://xob.redwolf501.top

[R58] 下载文件
来源：http://ikn.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lli.fzhhl.top

[R59] 发 POST JSON
来源：http://cge.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xpe.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://xvr.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nqh.xinyue.icu

[R61] 磁盘占用
来源：http://xsx.epnwcf.com

df -h;  du -sh *
来源：http://obj.andypj.xyz

[R62] 找最占空间的文件
来源：http://kxo.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://bxx.chenzaomai.com

[R63] 内存与进程
来源：http://mtf.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://dcx.yuxming.cn

[R64] 结束进程
来源：http://ejs.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://zmt.xuetiantiany.cn

[R65] 查看端口占用
来源：http://mxw.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vhx.cqqwz.cn

[R66] 定时任务
来源：http://bpe.hysaishi.cn

crontab -e;  crontab -l
来源：http://azv.yueranfly.top

[R67] 生成随机十六进制串
来源：http://hya.haohaochexian.top

openssl rand -hex 16
来源：http://ukb.chenzaomai.com

[R68] 计算文件校验值
来源：http://vro.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mwi.fehbvm.com

[R69] 生成随机密码
来源：http://awr.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://fwn.ydjk.org.cn

[R70] 时间戳与互转
来源：http://dgd.iojbl.cn

date +%s;  date -d @1700000000
来源：http://dlw.cashguo.top

[R71] 日期格式化
来源：http://cdw.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ohz.guowangkeji.top

[R72] 等待端口就绪
来源：http://izv.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://kdg.daria6918.cn

[R73] 分割大日志
来源：http://tnu.hesvh.cn

split -l 1000 big.log part_
来源：http://axq.jiagoushi.top

[R74] 批量重命名
来源：http://aeu.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://keb.zhijiandao.cn

[R75] 导出环境变量
来源：http://abm.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://vcz.wangshuangyany.cn

[R76] 使用临时文件
来源：http://int.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ddd.nanxuanxn.top

[R77] 读取用户输入
来源：http://wwb.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://mji.ppjwa.cn

[R78] 交互式菜单
来源：http://tag.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://boq.sxryk.cn

[R79] 解析命令行选项
来源：http://tsl.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lji.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://lxd.haohaochexian.top

time ./run.sh
来源：http://yqy.iojbl.cn

================================================================================
来源：http://ajs.cashguo.top

S. C / C++ 专题
来源：http://kry.c1oappe.top

================================================================================
来源：http://fsf.shanyushiyangtech.top

[S01] C：Hello World
来源：http://xmc.hnxiangtu.top

#include <stdio.h>
来源：http://kpx.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bwi.yueranfly.top

[S02] C：变量与格式化输出
来源：http://nuh.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://xhc.daria6918.cn

[S03] C：读入整数
来源：http://qhq.aizwys.cn

int x; scanf("%d", &x);
来源：http://ppj.vehdjk.com

[S04] C：字符串复制
来源：http://evt.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://yhl.meibo888.top

[S05] C：字符串长度
来源：http://jlj.fanxiaobao.xyz

strlen(s)
来源：http://ego.zdbjq.cn

[S06] C：字符串比较
来源：http://ifp.tanke756.top

strcmp(a, b) == 0
来源：http://xta.cucudq.cn

[S07] C：数组遍历求和
来源：http://fko.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zzm.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://uos.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nzg.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://uce.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sfg.nanxinkj.top

[S10] C：指针与解引用
来源：http://zgb.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://wyk.iojbl.cn

[S11] C：逐行读文件
来源：http://zwn.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://ahm.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://adm.yangfankeji.com

fclose(f);
来源：http://ohu.yfazqb.com

[S12] C：写文件
来源：http://bjy.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xrz.meibo888.top

[S13] C：宏定义
来源：http://ogx.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gvh.yueranfly.top

[S14] C：枚举
来源：http://rpa.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://mls.52xcode.cn

[S15] C：类型转换
来源：http://dyt.vehdjk.com

(double) a / b
来源：http://omw.nanxuanxn.top

[S16] C：位操作置位
来源：http://ijz.yuanzhike.top

x |= (1 << 3);
来源：http://ngo.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://voa.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tyd.sxryk.cn

[S18] C：命令行参数
来源：http://keq.jqgfzy.top

int main(int argc, char **argv)
来源：http://zso.guannengcc.top

[S19] C：快速排序
来源：http://tsb.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gub.pengpengdd.cyou

[S20] C：二分查找
来源：http://pyh.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dzk.jqgufenzy.top

[S21] C：字符类别判断
来源：http://deg.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wau.hammf.cn

[S22] C：字符串转数字
来源：http://vbp.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://lxc.uphjek.com

[S23] C：随机数
来源：http://hqo.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tgg.xuanzx.com

[S24] C：获取本地时间
来源：http://nko.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lsr.gzhubu.top

[S25] C：内存拷贝
来源：http://hnj.yj202588.top

memcpy(dst, src, n);
来源：http://ivh.dianchejie.cn

[S26] C：内存清零
来源：http://tzv.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://cmg.jlsjyb.cn

[S27] C：定义常量
来源：http://kik.vqdsnc.cn

const double PI = 3.14159;
来源：http://lzv.hysaishi.cn

[S28] C：静态变量
来源：http://urq.fengsongda.top

static int counter = 0;
来源：http://bwx.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://nza.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xfw.gotoacloud.top

[S30] C：头文件保护
来源：http://wpz.uphjek.com

#ifndef X_H
来源：http://bxj.xuetiantiany.cn

#define X_H
来源：http://wpv.yj202588.top

#endif
来源：http://ikk.cqqwz.cn

[S31] C++：Hello World
来源：http://uju.sweek.top

#include <iostream>
来源：http://beh.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://ndb.xylfe.cn

[S32] C++：字符串
来源：http://cvk.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://vfy.tian-w.cn

[S33] C++：vector 增删
来源：http://kqq.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aro.hfpthk.cn

[S34] C++：遍历 vector
来源：http://fbv.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://bis.quarkkingdee.top

[S35] C++：map
来源：http://udv.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rqs.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://wco.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wyh.sufxvd.cn

[S37] C++：set
来源：http://thu.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qpk.sjlbkw.cn

[S38] C++：排序
来源：http://ngg.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://zvx.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://vre.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pex.wangshuangyany.cn

[S40] C++：查找元素
来源：http://glj.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hdh.xinyue.icu

[S41] C++：类与构造函数
来源：http://ijj.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fnb.daxiang520.top

[S42] C++：继承与虚函数
来源：http://ozr.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://nfb.jqgfzy.top

[S43] C++：智能指针
来源：http://tzv.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://ojs.hysaishi.cn

[S44] C++：引用传参
来源：http://sov.nwbrower.top

void inc(int &x) { ++x; }
来源：http://esu.iojbl.cn

[S45] C++：lambda
来源：http://uop.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ptx.wangdashe.top

[S46] C++：函数模板
来源：http://mqi.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nil.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://blw.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vsf.jyoumei.cn

[S48] C++：逐行读文件
来源：http://szu.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://heq.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://xhc.ivvv.top

[S49] C++：写文件
来源：http://elq.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kzq.yfazqb.com

[S50] C++：格式化数字
来源：http://dda.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kgo.316326.xyz

[S51] C++：显式类型转换
来源：http://hhw.cucudq.cn

static_cast<double>(a) / b
来源：http://qwe.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://evu.uphjek.com

int size() const noexcept { return n_; }
来源：http://flm.yangfankeji.com

[S53] C++：移动语义
来源：http://iza.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://pnm.shzxlz.cn

[S54] C++：异常处理
来源：http://hnw.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://okf.pycfn.com

[S55] C++：结构化绑定
来源：http://uuj.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zwg.ydjk.org.cn

[S56] C++：optional
来源：http://nxi.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jcz.bjfxy.top

[S57] C++：编译期常量
来源：http://luf.vehdjk.com

constexpr int N = 10;
来源：http://obp.sysykeji.top

[S58] C++：命名空间
来源：http://ykh.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://pfp.hcnkem.com

[S59] C++：静态断言
来源：http://mha.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bvr.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://ylo.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://byh.shanyushiyangkeji.top

================================================================================
来源：http://kit.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cyz.ywan-chungtsiang.top

================================================================================
来源：http://gni.cqqwz.cn


<!-- 参考信息 -->