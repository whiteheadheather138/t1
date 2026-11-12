代发 wailian999

R. Bash 专题
来源：http://vhm.mhx1999.top

================================================================================
来源：http://fnt.sysykeji.top

[R01] shebang 与严格模式
来源：http://uqh.jinqigfzy.top

#!/usr/bin/env bash
来源：http://sln.vqdsnc.cn

set -euo pipefail
来源：http://blk.aibaodan.cn

[R02] 变量赋值与使用
来源：http://gbj.daxiang520.top

name="Tom"; echo "$name"
来源：http://nzw.yueranfly.top

[R03] 只读变量
来源：http://lpx.cheryme.top

readonly PI=3.14
来源：http://ulk.pycfn.com

[R04] 位置参数
来源：http://qeb.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://svy.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://aob.sjlbkw.cn

name="${1:-default}"
来源：http://zpa.yj202588.top

[R06] 判断命令是否存在
来源：http://jwq.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lfl.0kj1m.cn

[R07] if 判断文件
来源：http://ofg.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mas.gotoacloud.top

[R08] 数值比较
来源：http://kuf.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jei.yvedp.cn

[R09] 字符串比较
来源：http://okc.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cdq.shzxlz.cn

[R10] 正则匹配
来源：http://msq.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://den.zdbjq.cn

[R11] case 多分支
来源：http://guy.zhaomingkeji.xyz

case "$1" in
来源：http://cgr.nanxinkj.top

start) echo "启动" ;;
来源：http://rta.dianchejie.cn

stop)  echo "停止" ;;
来源：http://cpb.yuxming.cn

*)     echo "未知命令" ;;
来源：http://qxi.sweek.top

esac
来源：http://diz.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://zjx.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://twl.meibo888.top

[R13] for 计数循环
来源：http://ttg.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://vpd.yonumen.top

[R14] C 风格 for
来源：http://ccz.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cys.haohaochexian.top

[R15] while 逐行读文件
来源：http://bgm.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tmr.tarul.cn

[R16] until 等待条件
来源：http://ern.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ptb.hywenlv.cn

[R17] 数组定义与取值
来源：http://atr.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://cmd.hcnkem.com

[R18] 遍历数组
来源：http://hqe.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mag.gzhubu.top

[R19] 数组长度
来源：http://ujz.nanxinkj.top

echo "${#arr[@]}"
来源：http://jch.xylfe.cn

[R20] 关联数组（字典）
来源：http://zir.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cgb.aibaodan.cn

[R21] 字符串长度
来源：http://awc.xinyue.icu

echo "${#s}"
来源：http://ayg.dianchejie.cn

[R22] 截取子串
来源：http://ekl.haohaochexian.top

echo "${s:0:5}"
来源：http://cwy.zdbjq.cn

[R23] 字符串替换
来源：http://yxk.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zhz.yongpay.top

[R24] 大小写转换
来源：http://ase.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ybm.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://vkl.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkk.yongpay.top

[R26] 命令替换
来源：http://nnq.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://iia.hongshengwenyu.top

[R27] 算术展开
来源：http://lqs.sysykeji.top

echo $((1 + 2 * 3))
来源：http://duk.sjlbkw.cn

[R28] 浮点运算
来源：http://nfe.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://zfn.dashuyun.cn

[R29] 定义函数
来源：http://mkj.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ygt.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://afg.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://luh.ybcxt.top

[R31] 局部变量
来源：http://gjb.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://lqw.redwolf501.top

[R32] 参数个数校验
来源：http://jik.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ndc.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://zvf.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kud.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://vpf.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ite.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://zjx.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://myg.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://dye.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mpu.shuidangran.top

[R37] 把输出赋给变量
来源：http://pof.gogol.net.cn

files=$(ls -1)
来源：http://eil.birdmap.top

[R38] 管道串联
来源：http://cto.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://nhc.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://fxr.nwbrower.top

cmd > out.log 2>&1
来源：http://lxa.redwolf501.top

[R40] 追加写日志
来源：http://amk.sufxvd.cn

echo "log" >> out.log
来源：http://iue.shuidangran.top

[R41] 丢弃输出
来源：http://sre.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://uig.jinqigufen.top

[R42] 输入重定向
来源：http://owv.tianlin.xyz

wc -l < a.txt
来源：http://tja.yuanzhike.top

[R43] 按名字查找文件
来源：http://tcu.andypj.xyz

find . -name "*.log" -type f
来源：http://xes.tian-w.cn

[R44] 按修改时间查找
来源：http://bxg.hfpthk.cn

find . -mtime -7 -type f
来源：http://ddb.yuanzhike.top

[R45] 批量删除
来源：http://hiw.tian-w.cn

find . -name "*.tmp" -delete
来源：http://ygb.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://gii.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kaa.ctjpmb.com

[R47] sed 单行替换
来源：http://ond.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://klj.yj20258888.top

[R48] awk 取指定列
来源：http://pcv.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://psb.ivvv.top

[R49] awk 带条件
来源：http://yaq.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cqu.jinqigfzy.top

[R50] awk 求和
来源：http://ywu.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jpq.jiagoushi.top

[R51] 排序去重取前几
来源：http://xqe.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://emd.0kj1m.cn

[R52] 统计行数
来源：http://ucw.fktsv.cn

wc -l a.txt
来源：http://mag.tarul.cn

[R53] 查看文件头与实时尾
来源：http://ncz.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xhz.snrcjt.cn

[R54] 比较两个文件
来源：http://qet.gotoacloud.top

diff a.txt b.txt
来源：http://jbp.shuidangran.top

[R55] 压缩与解压
来源：http://kux.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cjm.tanke756.top

[R56] 远程拷贝
来源：http://fbq.wangshuangyany.cn

scp file user@host:/path/
来源：http://glb.yj20258.top

[R57] 远程执行命令
来源：http://bvm.yanxiufei.cn

ssh user@host 'uptime'
来源：http://dtn.52xcode.cn

[R58] 下载文件
来源：http://nod.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rfg.chenzaomai.com

[R59] 发 POST JSON
来源：http://elr.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lba.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://ygl.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qof.bbcook.cn

[R61] 磁盘占用
来源：http://mmx.guannengcc.top

df -h;  du -sh *
来源：http://dna.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://aqg.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://znd.daxiang520.top

[R63] 内存与进程
来源：http://pys.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://hut.ybcxt.top

[R64] 结束进程
来源：http://oco.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://ers.vehdjk.com

[R65] 查看端口占用
来源：http://rtc.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://guq.andypj.xyz

[R66] 定时任务
来源：http://ail.andypj.xyz

crontab -e;  crontab -l
来源：http://bdv.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://rsg.hammf.cn

openssl rand -hex 16
来源：http://urs.redwolf501.top

[R68] 计算文件校验值
来源：http://zmj.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://zaf.guowangkeji.top

[R69] 生成随机密码
来源：http://nli.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://sby.hesvh.cn

[R70] 时间戳与互转
来源：http://eoe.hnqzz.top

date +%s;  date -d @1700000000
来源：http://wza.nwbrower.top

[R71] 日期格式化
来源：http://obp.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wlm.daxiang520.top

[R72] 等待端口就绪
来源：http://nfm.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oxq.yanxiufei.cn

[R73] 分割大日志
来源：http://taz.sjlbkw.cn

split -l 1000 big.log part_
来源：http://hcw.hnqzz.top

[R74] 批量重命名
来源：http://kjk.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://naq.sysykeji.top

[R75] 导出环境变量
来源：http://apl.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://zgs.xuetiantiany.cn

[R76] 使用临时文件
来源：http://lwy.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://all.hongshengwenyu.top

[R77] 读取用户输入
来源：http://yvz.c1oappe.top

read -rp "请输入: " ans
来源：http://rjl.cucudq.cn

[R78] 交互式菜单
来源：http://chx.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kqv.andypj.xyz

[R79] 解析命令行选项
来源：http://ffc.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dwj.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://cua.vqdsnc.cn

time ./run.sh
来源：http://rwe.yj20258888.top

================================================================================
来源：http://pnx.havefunace.top

S. C / C++ 专题
来源：http://bgh.zhongyouzk.top

================================================================================
来源：http://wlq.hywenlv.cn

[S01] C：Hello World
来源：http://zfc.fanxiaobao.xyz

#include <stdio.h>
来源：http://hbn.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sru.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://xtt.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://knh.yuanzhike.top

[S03] C：读入整数
来源：http://yyq.cdnleiting.top

int x; scanf("%d", &x);
来源：http://vfw.vqdsnc.cn

[S04] C：字符串复制
来源：http://msi.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://vte.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://tgl.c1oappe.top

strlen(s)
来源：http://jnb.yuxming.cn

[S06] C：字符串比较
来源：http://qgj.bbcook.cn

strcmp(a, b) == 0
来源：http://jxw.smart0.xyz

[S07] C：数组遍历求和
来源：http://ind.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vnq.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://dtf.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fss.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://mvk.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oho.ybcxt.top

[S10] C：指针与解引用
来源：http://ufg.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://psi.hammf.cn

[S11] C：逐行读文件
来源：http://hrv.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://lbx.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xok.hammf.cn

fclose(f);
来源：http://pvj.epnwcf.com

[S12] C：写文件
来源：http://zag.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gza.hesvh.cn

[S13] C：宏定义
来源：http://uaz.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bcs.wangshuangyany.cn

[S14] C：枚举
来源：http://qjl.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://kxg.hnqzz.top

[S15] C：类型转换
来源：http://kvz.hcnkem.com

(double) a / b
来源：http://gxw.daxiang520.top

[S16] C：位操作置位
来源：http://yow.jinghuilouyu.cn

x |= (1 << 3);
来源：http://cdl.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://ywz.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rid.aizwys.cn

[S18] C：命令行参数
来源：http://itl.ydjk.org.cn

int main(int argc, char **argv)
来源：http://ulq.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://npe.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://xga.daria6918.cn

[S20] C：二分查找
来源：http://rmt.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krc.snrcjt.cn

[S21] C：字符类别判断
来源：http://dvp.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mng.ydzc1.top

[S22] C：字符串转数字
来源：http://xjx.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://yhf.tian-w.cn

[S23] C：随机数
来源：http://vmy.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wev.yueranfly.top

[S24] C：获取本地时间
来源：http://ngv.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yhn.hywenlv.cn

[S25] C：内存拷贝
来源：http://lum.hnxiangtu.top

memcpy(dst, src, n);
来源：http://bpm.ydzc1.top

[S26] C：内存清零
来源：http://srd.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://vgw.iojbl.cn

[S27] C：定义常量
来源：http://ain.cqqwz.cn

const double PI = 3.14159;
来源：http://nzs.wangdashe.top

[S28] C：静态变量
来源：http://nji.bjfxy.top

static int counter = 0;
来源：http://xyy.hfpthk.cn

[S29] C：变参函数
来源：http://ttk.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vaq.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://ddw.xziqi.cn

#ifndef X_H
来源：http://tnd.nwbrower.top

#define X_H
来源：http://tdq.hcnkem.com

#endif
来源：http://ujt.52xcode.cn

[S31] C++：Hello World
来源：http://egd.wangdashe.top

#include <iostream>
来源：http://pce.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://hqr.tanke756.top

[S32] C++：字符串
来源：http://mvr.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://jjk.jianghu66.top

[S33] C++：vector 增删
来源：http://ddl.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oda.316326.xyz

[S34] C++：遍历 vector
来源：http://eqv.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://zfi.yj202588.top

[S35] C++：map
来源：http://ilb.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cam.hcnkem.com

[S36] C++：unordered_map
来源：http://cfz.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tqd.jinqigufen.top

[S37] C++：set
来源：http://nhj.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ccb.tarul.cn

[S38] C++：排序
来源：http://mwx.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://fnh.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://bmh.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dya.iojbl.cn

[S40] C++：查找元素
来源：http://ggu.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ytt.chenzaomai.com

[S41] C++：类与构造函数
来源：http://ato.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dlv.xinyue.icu

[S42] C++：继承与虚函数
来源：http://jsv.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://bnn.mhx1999.top

[S43] C++：智能指针
来源：http://icd.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://kdp.yanxiufei.cn

[S44] C++：引用传参
来源：http://bjb.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://vwt.sjlbkw.cn

[S45] C++：lambda
来源：http://jla.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ifz.gzhubu.top

[S46] C++：函数模板
来源：http://nmu.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rcv.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://bmj.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsu.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://peg.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://faq.aizwys.cn

while (std::getline(in, line)) { }
来源：http://mdn.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://web.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lta.fzhhl.top

[S50] C++：格式化数字
来源：http://mce.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zhm.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://rys.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://ixf.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://egx.nwbrower.top

int size() const noexcept { return n_; }
来源：http://flc.yanxiufei.cn

[S53] C++：移动语义
来源：http://wnf.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://oyg.fehbvm.com

[S54] C++：异常处理
来源：http://xwr.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://obl.meibo888.top

[S55] C++：结构化绑定
来源：http://zkm.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://inp.fzhhl.top

[S56] C++：optional
来源：http://sfv.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pxn.pycfn.com

[S57] C++：编译期常量
来源：http://tnc.gotoacloud.top

constexpr int N = 10;
来源：http://tqa.jianghu66.top

[S58] C++：命名空间
来源：http://kls.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://ioj.xylfe.cn

[S59] C++：静态断言
来源：http://cgm.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aio.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://pxx.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wme.aizwys.cn

================================================================================
来源：http://eei.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hsf.xuanzx.com

================================================================================
来源：http://pkq.feifeiyinyue.top


<!-- 参考信息 -->