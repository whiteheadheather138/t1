代发 wailian999

set -euo pipefail
来源：http://rmn.sysykeji.top

[R02] 变量赋值与使用
来源：http://ght.daria6918.cn

name="Tom"; echo "$name"
来源：http://yro.dianchejie.cn

[R03] 只读变量
来源：http://zzk.nanxinkj.top

readonly PI=3.14
来源：http://pho.tian-w.cn

[R04] 位置参数
来源：http://vby.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tyd.pengpengdd.cyou

[R05] 参数默认值
来源：http://uos.jqgfzy.top

name="${1:-default}"
来源：http://zhs.zdbjq.cn

[R06] 判断命令是否存在
来源：http://mai.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxa.quarkkingdee.top

[R07] if 判断文件
来源：http://ads.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ryj.yj20258.top

[R08] 数值比较
来源：http://qat.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fmf.gogol.net.cn

[R09] 字符串比较
来源：http://bfr.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgk.tanke756.top

[R10] 正则匹配
来源：http://hgx.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xnt.shangyingyoupin.top

[R11] case 多分支
来源：http://laa.xuetiantiany.cn

case "$1" in
来源：http://vbg.hnqzz.top

start) echo "启动" ;;
来源：http://wpn.gotoacloud.top

stop)  echo "停止" ;;
来源：http://vgu.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://yhm.jlsjyb.cn

esac
来源：http://adl.chenlongwang.top

[R12] for 遍历文件
来源：http://pmy.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://alb.nanxuanxn.top

[R13] for 计数循环
来源：http://agr.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://eml.chenjidiqi.icu

[R14] C 风格 for
来源：http://cxq.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bka.cdnleiting.top

[R15] while 逐行读文件
来源：http://and.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://knd.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://jqq.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xzt.c1oappe.top

[R17] 数组定义与取值
来源：http://vlj.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://orp.yj20258888.top

[R18] 遍历数组
来源：http://dwa.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wmy.zhiwuduotai.top

[R19] 数组长度
来源：http://hcq.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://jis.fktsv.cn

[R20] 关联数组（字典）
来源：http://vyi.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ffc.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://ldz.snrcjt.cn

echo "${#s}"
来源：http://hto.mhx1999.top

[R22] 截取子串
来源：http://odn.jiagoushi.top

echo "${s:0:5}"
来源：http://ccr.haohaochexian.top

[R23] 字符串替换
来源：http://ibv.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://caa.ppjwa.cn

[R24] 大小写转换
来源：http://gjr.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://gby.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://lzc.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://eha.cheryme.top

[R26] 命令替换
来源：http://fqo.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://tyx.xylfe.cn

[R27] 算术展开
来源：http://jtf.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://jim.daria6918.cn

[R28] 浮点运算
来源：http://yvh.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://vpu.dianchejie.cn

[R29] 定义函数
来源：http://ack.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mbs.zhengqikj.top

[R30] 函数返回状态码
来源：http://axp.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://nqj.jinyuanbaomall.cn

[R31] 局部变量
来源：http://lee.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://uod.sysykeji.top

[R32] 参数个数校验
来源：http://twv.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jcv.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://lkr.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qqp.shangyingyoupin.top

[R34] 退出时清理
来源：http://tha.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://sgj.zycfv.cn

[R35] 后台执行并等待
来源：http://nxk.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://inj.jyoumei.cn

[R36] 并发执行多个任务
来源：http://qfw.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ojs.jiagoushi.top

[R37] 把输出赋给变量
来源：http://cyd.hywenlv.cn

files=$(ls -1)
来源：http://bss.smart0.xyz

[R38] 管道串联
来源：http://bhb.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://owa.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://xis.hnxiangtu.top

cmd > out.log 2>&1
来源：http://emz.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://wip.ydzc1.top

echo "log" >> out.log
来源：http://xit.havefunace.top

[R41] 丢弃输出
来源：http://tyd.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://xpa.tian-w.cn

[R42] 输入重定向
来源：http://vtd.ywan-chungtsiang.top

wc -l < a.txt
来源：http://xuu.tanke756.top

[R43] 按名字查找文件
来源：http://uqg.chenlongwang.top

find . -name "*.log" -type f
来源：http://aji.gotoacloud.top

[R44] 按修改时间查找
来源：http://gme.haohaochexian.top

find . -mtime -7 -type f
来源：http://qsz.guowangkeji.top

[R45] 批量删除
来源：http://fpe.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://ybg.xziqi.cn

[R46] 递归替换文件内容
来源：http://omr.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nci.jianghu66.top

[R47] sed 单行替换
来源：http://fzn.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://zbl.daria6918.cn

[R48] awk 取指定列
来源：http://xtr.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://nfn.ehwqpu.com

[R49] awk 带条件
来源：http://pmt.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xvh.jinqigufen.top

[R50] awk 求和
来源：http://ybt.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://wwf.yj20258.top

[R51] 排序去重取前几
来源：http://hmr.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xte.9152youxi.cn

[R52] 统计行数
来源：http://fce.pengpengdd.cyou

wc -l a.txt
来源：http://afm.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://isc.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xqa.bbcook.cn

[R54] 比较两个文件
来源：http://xjn.wangdashe.top

diff a.txt b.txt
来源：http://vue.wangshuangyany.cn

[R55] 压缩与解压
来源：http://vzw.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baa.shangyingyoupin.top

[R56] 远程拷贝
来源：http://svl.hammf.cn

scp file user@host:/path/
来源：http://pyt.nanxinkj.top

[R57] 远程执行命令
来源：http://mab.tanke756.top

ssh user@host 'uptime'
来源：http://bsr.zhaomingkeji.xyz

[R58] 下载文件
来源：http://ptr.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mwc.zhoulong.xyz

[R59] 发 POST JSON
来源：http://bno.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zmv.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://qdi.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ffe.jqgufenzy.top

[R61] 磁盘占用
来源：http://kuw.zhoulong.xyz

df -h;  du -sh *
来源：http://wto.zhengqikj.top

[R62] 找最占空间的文件
来源：http://bbt.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://mzy.hammf.cn

[R63] 内存与进程
来源：http://ide.yonumen.top

free -h;  ps aux | grep nginx
来源：http://zpb.ehwqpu.com

[R64] 结束进程
来源：http://nsq.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://chm.hammf.cn

[R65] 查看端口占用
来源：http://uos.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ald.feifeiyinyue.top

[R66] 定时任务
来源：http://fwe.jiagoushi.top

crontab -e;  crontab -l
来源：http://nwl.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://mho.tanke756.top

openssl rand -hex 16
来源：http://ddw.nwbrower.top

[R68] 计算文件校验值
来源：http://klt.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://unf.jqgufenzy.top

[R69] 生成随机密码
来源：http://nfw.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://fix.ydzc1.top

[R70] 时间戳与互转
来源：http://lko.bbcook.cn

date +%s;  date -d @1700000000
来源：http://pek.haohaochexian.top

[R71] 日期格式化
来源：http://xha.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wzu.fktsv.cn

[R72] 等待端口就绪
来源：http://ezl.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mla.gotoacloud.top

[R73] 分割大日志
来源：http://nsh.zdqjudy.top

split -l 1000 big.log part_
来源：http://fpc.zhengqikj.top

[R74] 批量重命名
来源：http://rhp.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ijm.shangyingyoupin.top

[R75] 导出环境变量
来源：http://xhb.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://lyp.hesvh.cn

[R76] 使用临时文件
来源：http://rgr.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xtn.pengpengdd.cyou

[R77] 读取用户输入
来源：http://nmj.guowangkeji.top

read -rp "请输入: " ans
来源：http://yly.sufxvd.cn

[R78] 交互式菜单
来源：http://ljp.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://oyu.sjlbkw.cn

[R79] 解析命令行选项
来源：http://arq.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kst.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://oaw.xingfuxueyuan.xyz

time ./run.sh
来源：http://wkl.epnwcf.com

================================================================================
来源：http://ywg.ydzc1.top

S. C / C++ 专题
来源：http://pns.uphjek.com

================================================================================
来源：http://sol.hfpthk.cn

[S01] C：Hello World
来源：http://kbm.chenjidiqi.icu

#include <stdio.h>
来源：http://swd.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dua.bbcook.cn

[S02] C：变量与格式化输出
来源：http://sap.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://fhz.snrcjt.cn

[S03] C：读入整数
来源：http://tox.zycfv.cn

int x; scanf("%d", &x);
来源：http://myf.xziqi.cn

[S04] C：字符串复制
来源：http://msw.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vxd.redwolf501.top

[S05] C：字符串长度
来源：http://hjs.aizwys.cn

strlen(s)
来源：http://oxx.tian-w.cn

[S06] C：字符串比较
来源：http://mps.aizwys.cn

strcmp(a, b) == 0
来源：http://acs.yuxming.cn

[S07] C：数组遍历求和
来源：http://cst.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://twk.yj202588.top

[S08] C：动态内存分配与释放
来源：http://qmq.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cmb.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://mda.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lie.meibo888.top

[S10] C：指针与解引用
来源：http://dnn.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://zsk.fengsongda.top

[S11] C：逐行读文件
来源：http://emv.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://bot.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://bad.fzhhl.top

fclose(f);
来源：http://csi.yongpay.top

[S12] C：写文件
来源：http://lac.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://std.tianlin.xyz

[S13] C：宏定义
来源：http://fep.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eam.xuetiantiany.cn

[S14] C：枚举
来源：http://wkb.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ldb.jinqigufen.top

[S15] C：类型转换
来源：http://spt.haohaochexian.top

(double) a / b
来源：http://bpe.tian-w.cn

[S16] C：位操作置位
来源：http://kzb.smart0.xyz

x |= (1 << 3);
来源：http://vaw.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://pmx.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dxi.tianlin.xyz

[S18] C：命令行参数
来源：http://uja.dianchejie.cn

int main(int argc, char **argv)
来源：http://igc.birdmap.top

[S19] C：快速排序
来源：http://bca.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ids.sweek.top

[S20] C：二分查找
来源：http://nug.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oqy.chenlongwang.top

[S21] C：字符类别判断
来源：http://bog.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yle.jianghu66.top

[S22] C：字符串转数字
来源：http://utp.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://gbc.zdbjq.cn

[S23] C：随机数
来源：http://jmb.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dyr.cheryme.top

[S24] C：获取本地时间
来源：http://tjj.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mxg.ivvv.top

[S25] C：内存拷贝
来源：http://nrx.ivvv.top

memcpy(dst, src, n);
来源：http://tcx.daxiang520.top

[S26] C：内存清零
来源：http://dic.xuanzx.com

memset(a, 0, sizeof a);
来源：http://brx.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://lic.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://loi.aizwys.cn

[S28] C：静态变量
来源：http://qic.zhixingplan.top

static int counter = 0;
来源：http://isc.yj202588.top

[S29] C：变参函数
来源：http://ysj.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fsw.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://qsj.zdbjq.cn

#ifndef X_H
来源：http://sdi.hcnkem.com

#define X_H
来源：http://kot.gaohongyu789.top

#endif
来源：http://ire.yueranfly.top

[S31] C++：Hello World
来源：http://kot.shanyushiyangkeji.top

#include <iostream>
来源：http://ajk.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://zgc.fehbvm.com

[S32] C++：字符串
来源：http://twb.havefunace.top

std::string s = "hi";  s += "!";
来源：http://ueh.nanxuanxn.top

[S33] C++：vector 增删
来源：http://sjl.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lyl.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://foi.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://rnv.shangyingyoupin.top

[S35] C++：map
来源：http://dze.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lqv.daria6918.cn

[S36] C++：unordered_map
来源：http://gpl.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tzc.fzhhl.top

[S37] C++：set
来源：http://sbv.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://omy.guannengcc.top

[S38] C++：排序
来源：http://tte.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://afz.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://ssj.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ces.sufxvd.cn

[S40] C++：查找元素
来源：http://ptm.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://utu.316326.xyz

[S41] C++：类与构造函数
来源：http://vaj.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hjf.shuidangran.top

[S42] C++：继承与虚函数
来源：http://glh.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://unx.vqdsnc.cn

[S43] C++：智能指针
来源：http://lsk.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://ils.jiagoushi.top

[S44] C++：引用传参
来源：http://now.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://lge.fzhhl.top

[S45] C++：lambda
来源：http://fkf.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://amy.jqgufenzy.top

[S46] C++：函数模板
来源：http://icb.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rdi.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://bmn.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rce.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://tlr.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://vvq.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://vpj.fzhhl.top

[S49] C++：写文件
来源：http://vsf.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uis.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://iur.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yrj.yueranfly.top

[S51] C++：显式类型转换
来源：http://zap.zhixingplan.top

static_cast<double>(a) / b
来源：http://bmz.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://olc.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://epc.sjlbkw.cn

[S53] C++：移动语义
来源：http://nop.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://yvp.hfpthk.cn

[S54] C++：异常处理
来源：http://ryi.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kov.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://vsj.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://auq.yj202588.top

[S56] C++：optional
来源：http://xtm.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qyg.yj20258.top

[S57] C++：编译期常量
来源：http://ozp.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://iwg.xuetiantiany.cn

[S58] C++：命名空间
来源：http://thl.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://bod.nwbrower.top

[S59] C++：静态断言
来源：http://nwj.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yhk.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://xfb.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ncp.shangyingyoupin.top

================================================================================
来源：http://wzc.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vwx.wangshuangyany.cn

================================================================================
来源：http://ubk.pycfn.com

[T01] Kotlin：Hello World
来源：http://lyg.fanxiaobao.xyz

println("Hello")
来源：http://nto.xylfe.cn

[T02] Kotlin：变量
来源：http://apv.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://urh.wangshuangyany.cn


<!-- 参考信息 -->