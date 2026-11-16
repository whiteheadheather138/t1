代发 wailian999

R. Bash 专题
来源：http://upk.uphjek.com

================================================================================
来源：http://fau.svipenyu.cn

[R01] shebang 与严格模式
来源：http://poz.pycfn.com

#!/usr/bin/env bash
来源：http://ndj.cdnleiting.top

set -euo pipefail
来源：http://pvz.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://wit.xziqi.cn

name="Tom"; echo "$name"
来源：http://tgn.quarkkingdee.top

[R03] 只读变量
来源：http://rwh.gogol.net.cn

readonly PI=3.14
来源：http://gqm.xuetiantiany.cn

[R04] 位置参数
来源：http://gho.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ntv.jqgufenzy.top

[R05] 参数默认值
来源：http://dex.yj20258.top

name="${1:-default}"
来源：http://cgy.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://zyn.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://knp.gogol.net.cn

[R07] if 判断文件
来源：http://ivg.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rmg.chenjidiqi.icu

[R08] 数值比较
来源：http://xwt.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://hve.aizwys.cn

[R09] 字符串比较
来源：http://btq.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://flm.xuetiantiany.cn

[R10] 正则匹配
来源：http://iii.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://spo.jinyuanbaomall.cn

[R11] case 多分支
来源：http://hvf.vehdjk.com

case "$1" in
来源：http://zru.xuetiantiany.cn

start) echo "启动" ;;
来源：http://iih.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://pfk.bjfxy.top

*)     echo "未知命令" ;;
来源：http://nzl.wangshuangyany.cn

esac
来源：http://wlx.hesvh.cn

[R12] for 遍历文件
来源：http://dqt.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://znz.nanxuanxn.top

[R13] for 计数循环
来源：http://tzc.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://vpj.yueranfly.top

[R14] C 风格 for
来源：http://ahk.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hbc.xylfe.cn

[R15] while 逐行读文件
来源：http://zur.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tpi.zhengqikj.top

[R16] until 等待条件
来源：http://dib.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://duk.sjlbkw.cn

[R17] 数组定义与取值
来源：http://afv.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://fup.ctjpmb.com

[R18] 遍历数组
来源：http://byu.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ouq.yangfankeji.com

[R19] 数组长度
来源：http://abb.yuanzhike.top

echo "${#arr[@]}"
来源：http://lyi.yj20258888.top

[R20] 关联数组（字典）
来源：http://pio.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uii.yanxiufei.cn

[R21] 字符串长度
来源：http://zlq.52xcode.cn

echo "${#s}"
来源：http://djd.xuanzx.com

[R22] 截取子串
来源：http://bhx.cheryme.top

echo "${s:0:5}"
来源：http://rfm.hongshengwenyu.top

[R23] 字符串替换
来源：http://udu.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oxx.hnqzz.top

[R24] 大小写转换
来源：http://wmd.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bbu.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://mzs.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxk.sxryk.cn

[R26] 命令替换
来源：http://iwh.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://zmi.shzxlz.cn

[R27] 算术展开
来源：http://cwu.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://exn.iojbl.cn

[R28] 浮点运算
来源：http://cmx.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://nvf.sufxvd.cn

[R29] 定义函数
来源：http://ooz.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rlu.yueranfly.top

[R30] 函数返回状态码
来源：http://fer.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://xrw.vehdjk.com

[R31] 局部变量
来源：http://ivs.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://ilo.xziqi.cn

[R32] 参数个数校验
来源：http://kmb.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gyh.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://evm.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gys.hammf.cn

[R34] 退出时清理
来源：http://men.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://zvj.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://fcr.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lex.nanxinkj.top

[R36] 并发执行多个任务
来源：http://wmj.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oqc.fehbvm.com

[R37] 把输出赋给变量
来源：http://nhy.cqqwz.cn

files=$(ls -1)
来源：http://lgf.yanxiufei.cn

[R38] 管道串联
来源：http://vcp.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://pxz.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://jvl.hywenlv.cn

cmd > out.log 2>&1
来源：http://koe.daxiang520.top

[R40] 追加写日志
来源：http://rqd.fanxiaobao.xyz

echo "log" >> out.log
来源：http://xlx.tarul.cn

[R41] 丢弃输出
来源：http://lps.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://ian.iojbl.cn

[R42] 输入重定向
来源：http://ciw.aizwys.cn

wc -l < a.txt
来源：http://dyq.gotoacloud.top

[R43] 按名字查找文件
来源：http://tut.guowangkeji.top

find . -name "*.log" -type f
来源：http://zad.yvedp.cn

[R44] 按修改时间查找
来源：http://izu.fktsv.cn

find . -mtime -7 -type f
来源：http://qxs.zycfv.cn

[R45] 批量删除
来源：http://zib.cheryme.top

find . -name "*.tmp" -delete
来源：http://nai.0kj1m.cn

[R46] 递归替换文件内容
来源：http://oox.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ubx.ydzc1.top

[R47] sed 单行替换
来源：http://lmh.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lnt.birdmap.top

[R48] awk 取指定列
来源：http://tfj.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://zdw.iojbl.cn

[R49] awk 带条件
来源：http://nvl.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://not.epnwcf.com

[R50] awk 求和
来源：http://raf.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jcb.hcnkem.com

[R51] 排序去重取前几
来源：http://ipw.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nxm.fanxiaobao.xyz

[R52] 统计行数
来源：http://ckx.shuidangran.top

wc -l a.txt
来源：http://emi.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://mye.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hlz.gogol.net.cn

[R54] 比较两个文件
来源：http://nrf.cucudq.cn

diff a.txt b.txt
来源：http://hoy.gaohongyu789.top

[R55] 压缩与解压
来源：http://hol.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://npl.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://huq.9152youxi.cn

scp file user@host:/path/
来源：http://uds.gotoacloud.top

[R57] 远程执行命令
来源：http://wsw.ehwqpu.com

ssh user@host 'uptime'
来源：http://xqj.hnxiangtu.top

[R58] 下载文件
来源：http://mif.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ynd.sufxvd.cn

[R59] 发 POST JSON
来源：http://nxw.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tyt.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://spf.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eod.birdmap.top

[R61] 磁盘占用
来源：http://gkk.sweek.top

df -h;  du -sh *
来源：http://dzn.chenlongwang.top

[R62] 找最占空间的文件
来源：http://gfh.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://vhz.vehdjk.com

[R63] 内存与进程
来源：http://nnm.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://vfs.redwolf501.top

[R64] 结束进程
来源：http://rba.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://wfr.hnxiangtu.top

[R65] 查看端口占用
来源：http://sei.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rco.kuanghao11.cn

[R66] 定时任务
来源：http://tht.dashuyun.cn

crontab -e;  crontab -l
来源：http://pjd.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://mof.quarkkingdee.top

openssl rand -hex 16
来源：http://flz.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://oqs.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://guc.yfazqb.com

[R69] 生成随机密码
来源：http://kwq.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://ssh.zdqjudy.top

[R70] 时间戳与互转
来源：http://xht.yj202588.top

date +%s;  date -d @1700000000
来源：http://ubr.ctjpmb.com

[R71] 日期格式化
来源：http://ddg.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxi.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://jwe.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pwh.redwolf501.top

[R73] 分割大日志
来源：http://ygg.aizwys.cn

split -l 1000 big.log part_
来源：http://ycp.52xcode.cn

[R74] 批量重命名
来源：http://tsv.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dde.chenlongwang.top

[R75] 导出环境变量
来源：http://fas.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://jza.bbcook.cn

[R76] 使用临时文件
来源：http://bvz.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dct.52xcode.cn

[R77] 读取用户输入
来源：http://clg.daria6918.cn

read -rp "请输入: " ans
来源：http://pin.yuxming.cn

[R78] 交互式菜单
来源：http://kgi.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lfh.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://dhp.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zqe.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://een.meibo888.top

time ./run.sh
来源：http://roq.sweek.top

================================================================================
来源：http://lum.sweek.top

S. C / C++ 专题
来源：http://ksw.hysaishi.cn

================================================================================
来源：http://jwp.dashuyun.cn

[S01] C：Hello World
来源：http://ost.c1oappe.top

#include <stdio.h>
来源：http://xzk.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yqo.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://qig.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://fun.yuanzhike.top

[S03] C：读入整数
来源：http://yvy.guowangkeji.top

int x; scanf("%d", &x);
来源：http://cqu.ppjwa.cn

[S04] C：字符串复制
来源：http://txx.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://erp.gotoacloud.top

[S05] C：字符串长度
来源：http://amg.yj20258888.top

strlen(s)
来源：http://tby.vehdjk.com

[S06] C：字符串比较
来源：http://akr.nanxuanxn.top

strcmp(a, b) == 0
来源：http://twy.jyoumei.cn

[S07] C：数组遍历求和
来源：http://not.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://elh.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://jai.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dzu.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://lrl.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ury.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://ajo.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://oox.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://tin.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://yqo.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gxj.cqqwz.cn

fclose(f);
来源：http://rwx.tarul.cn

[S12] C：写文件
来源：http://uik.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vgz.andypj.xyz

[S13] C：宏定义
来源：http://vio.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hun.fehbvm.com

[S14] C：枚举
来源：http://rej.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://uwr.jyoumei.cn

[S15] C：类型转换
来源：http://vki.hnqzz.top

(double) a / b
来源：http://brd.yongpay.top

[S16] C：位操作置位
来源：http://him.wangdashe.top

x |= (1 << 3);
来源：http://flq.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://ffx.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://umz.tianlin.xyz

[S18] C：命令行参数
来源：http://blt.guowangkeji.top

int main(int argc, char **argv)
来源：http://guf.fzhhl.top

[S19] C：快速排序
来源：http://tju.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://mjt.ydzc1.top

[S20] C：二分查找
来源：http://zsp.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://caz.ydzc1.top

[S21] C：字符类别判断
来源：http://upe.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kwi.meibo888.top

[S22] C：字符串转数字
来源：http://ibj.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hev.havefunace.top

[S23] C：随机数
来源：http://iwe.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hoz.hfpthk.cn

[S24] C：获取本地时间
来源：http://gwb.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hkj.zhoulong.xyz

[S25] C：内存拷贝
来源：http://cfw.ydzc1.top

memcpy(dst, src, n);
来源：http://xpi.aibaodan.cn

[S26] C：内存清零
来源：http://fml.yfazqb.com

memset(a, 0, sizeof a);
来源：http://fxl.sjlbkw.cn

[S27] C：定义常量
来源：http://jbe.yfazqb.com

const double PI = 3.14159;
来源：http://gyv.yj20258888.top

[S28] C：静态变量
来源：http://lwr.9152youxi.cn

static int counter = 0;
来源：http://yhj.sjlbkw.cn

[S29] C：变参函数
来源：http://blx.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kta.hysaishi.cn

[S30] C：头文件保护
来源：http://dii.meibo888.top

#ifndef X_H
来源：http://vjd.cqqwz.cn

#define X_H
来源：http://oyt.yfazqb.com

#endif
来源：http://huw.chenjidiqi.icu

[S31] C++：Hello World
来源：http://ztr.sweek.top

#include <iostream>
来源：http://hnd.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://vsy.0kj1m.cn

[S32] C++：字符串
来源：http://yvh.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://umc.ehwqpu.com

[S33] C++：vector 增删
来源：http://hbt.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xnr.ydzc1.top

[S34] C++：遍历 vector
来源：http://adu.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://aly.gotoacloud.top

[S35] C++：map
来源：http://bvu.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qqg.guannengcc.top

[S36] C++：unordered_map
来源：http://itw.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nqi.zhoulong.xyz

[S37] C++：set
来源：http://awv.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xyh.tian-w.cn

[S38] C++：排序
来源：http://ivz.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://ahs.birdmap.top

[S39] C++：自定义比较器排序
来源：http://fwx.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hew.smart0.xyz

[S40] C++：查找元素
来源：http://nbf.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sqd.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://pye.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ifk.xinyue.icu

[S42] C++：继承与虚函数
来源：http://mbs.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://sdb.fzhhl.top

[S43] C++：智能指针
来源：http://leu.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://sck.hammf.cn

[S44] C++：引用传参
来源：http://qid.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://tqb.jianghu66.top

[S45] C++：lambda
来源：http://xmg.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vsf.yj202588.top

[S46] C++：函数模板
来源：http://cpd.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oka.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://eps.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ivw.tarul.cn

[S48] C++：逐行读文件
来源：http://vmq.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://far.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://ejn.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://bbv.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ubi.dianchejie.cn

[S50] C++：格式化数字
来源：http://ndb.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jra.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://oqm.aizwys.cn

static_cast<double>(a) / b
来源：http://lym.tarul.cn

[S52] C++：const 与 noexcept
来源：http://osj.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://dnr.zhengqikj.top

[S53] C++：移动语义
来源：http://uyj.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://mzq.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://gwb.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://izh.hywenlv.cn

[S55] C++：结构化绑定
来源：http://xlf.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gpc.aibaodan.cn

[S56] C++：optional
来源：http://ycn.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jht.zhengqikj.top

[S57] C++：编译期常量
来源：http://nmu.bjfxy.top

constexpr int N = 10;
来源：http://tmv.gaohongyu789.top

[S58] C++：命名空间
来源：http://pag.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://ggx.redwolf501.top

[S59] C++：静态断言
来源：http://dni.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yvi.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://azz.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mjx.zhijiandao.cn

================================================================================
来源：http://fhn.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npo.ywan-chungtsiang.top

================================================================================
来源：http://bzf.tarul.cn


<!-- 参考信息 -->