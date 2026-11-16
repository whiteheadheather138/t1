代发 wailian999

R. Bash 专题
来源：http://anp.xingfuxueyuan.xyz

================================================================================
来源：http://thx.vehdjk.com

[R01] shebang 与严格模式
来源：http://vjj.aibaodan.cn

#!/usr/bin/env bash
来源：http://rkk.gaohongyu789.top

set -euo pipefail
来源：http://bwu.aizwys.cn

[R02] 变量赋值与使用
来源：http://kme.tian-w.cn

name="Tom"; echo "$name"
来源：http://hhg.guowangkeji.top

[R03] 只读变量
来源：http://wyr.jinqigfzy.top

readonly PI=3.14
来源：http://uid.iojbl.cn

[R04] 位置参数
来源：http://bft.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nfc.fanxiaobao.xyz

[R05] 参数默认值
来源：http://yhh.andypj.xyz

name="${1:-default}"
来源：http://swa.xylfe.cn

[R06] 判断命令是否存在
来源：http://ndd.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://agz.meibo888.top

[R07] if 判断文件
来源：http://nuk.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nvc.nwbrower.top

[R08] 数值比较
来源：http://fzl.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ffu.vqdsnc.cn

[R09] 字符串比较
来源：http://zda.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eql.gotoacloud.top

[R10] 正则匹配
来源：http://jen.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oer.yangfankeji.com

[R11] case 多分支
来源：http://jxr.zhixingplan.top

case "$1" in
来源：http://wuk.xinyue.icu

start) echo "启动" ;;
来源：http://pqu.zhixingplan.top

stop)  echo "停止" ;;
来源：http://zoh.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://gwo.jinqigfzy.top

esac
来源：http://wxr.guannengcc.top

[R12] for 遍历文件
来源：http://iae.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://gfg.sysykeji.top

[R13] for 计数循环
来源：http://xbl.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://aau.kuanghao11.cn

[R14] C 风格 for
来源：http://xki.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iwx.yonumen.top

[R15] while 逐行读文件
来源：http://qfd.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jbd.daxiang520.top

[R16] until 等待条件
来源：http://sgm.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baz.cashguo.top

[R17] 数组定义与取值
来源：http://sdi.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://qua.pycfn.com

[R18] 遍历数组
来源：http://jeu.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mar.yuxming.cn

[R19] 数组长度
来源：http://frh.jiagoushi.top

echo "${#arr[@]}"
来源：http://irc.mhx1999.top

[R20] 关联数组（字典）
来源：http://zzy.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://myt.jiagoushi.top

[R21] 字符串长度
来源：http://oqu.zhengqikj.top

echo "${#s}"
来源：http://xab.gogol.net.cn

[R22] 截取子串
来源：http://fbn.daria6918.cn

echo "${s:0:5}"
来源：http://mki.zdbjq.cn

[R23] 字符串替换
来源：http://wxb.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wnz.sysykeji.top

[R24] 大小写转换
来源：http://kup.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://xno.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://jtu.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rbv.hongshengwenyu.top

[R26] 命令替换
来源：http://wgq.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://yhe.jyoumei.cn

[R27] 算术展开
来源：http://xaf.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://bsn.fehbvm.com

[R28] 浮点运算
来源：http://zsr.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://ubj.daxiang520.top

[R29] 定义函数
来源：http://amt.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oyl.nwbrower.top

[R30] 函数返回状态码
来源：http://ira.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://dtm.c1oappe.top

[R31] 局部变量
来源：http://flk.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://zfz.guannengcc.top

[R32] 参数个数校验
来源：http://ovc.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://puc.tarul.cn

[R33] 捕获错误并提示行号
来源：http://ztx.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzi.yanxiufei.cn

[R34] 退出时清理
来源：http://tsn.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pjl.yanxiufei.cn

[R35] 后台执行并等待
来源：http://hix.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pbc.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://teq.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dha.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://bfy.fanxiaobao.xyz

files=$(ls -1)
来源：http://kzc.pengpengdd.cyou

[R38] 管道串联
来源：http://jwc.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://ori.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://cll.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://fgy.chenzaomai.com

[R40] 追加写日志
来源：http://mex.shuidangran.top

echo "log" >> out.log
来源：http://obj.hfpthk.cn

[R41] 丢弃输出
来源：http://qca.mhx1999.top

cmd >/dev/null 2>&1
来源：http://kif.jlsjyb.cn

[R42] 输入重定向
来源：http://yqg.zhiwuduotai.top

wc -l < a.txt
来源：http://ozz.tarul.cn

[R43] 按名字查找文件
来源：http://xuj.cqqwz.cn

find . -name "*.log" -type f
来源：http://hok.jqgufenzy.top

[R44] 按修改时间查找
来源：http://upj.cucudq.cn

find . -mtime -7 -type f
来源：http://rjy.hysaishi.cn

[R45] 批量删除
来源：http://gdv.52xcode.cn

find . -name "*.tmp" -delete
来源：http://hte.gzhubu.top

[R46] 递归替换文件内容
来源：http://yiy.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rtv.zhiwuduotai.top

[R47] sed 单行替换
来源：http://unw.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://qda.svipenyu.cn

[R48] awk 取指定列
来源：http://zyo.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://ost.ehwqpu.com

[R49] awk 带条件
来源：http://quq.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bdc.snrcjt.cn

[R50] awk 求和
来源：http://puw.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://jhj.yonumen.top

[R51] 排序去重取前几
来源：http://tbk.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dhq.jinghuilouyu.cn

[R52] 统计行数
来源：http://trj.tianlin.xyz

wc -l a.txt
来源：http://myg.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://yda.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://doh.cqqwz.cn

[R54] 比较两个文件
来源：http://atk.snrcjt.cn

diff a.txt b.txt
来源：http://tms.ydjk.org.cn

[R55] 压缩与解压
来源：http://jdt.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://key.tanke756.top

[R56] 远程拷贝
来源：http://zfn.yuanzhike.top

scp file user@host:/path/
来源：http://zgb.tian-w.cn

[R57] 远程执行命令
来源：http://xrv.xuanzx.com

ssh user@host 'uptime'
来源：http://vlr.hongshengwenyu.top

[R58] 下载文件
来源：http://bmm.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://spm.jinqigfzy.top

[R59] 发 POST JSON
来源：http://jdr.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tzw.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://mxa.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sbu.cqqwz.cn

[R61] 磁盘占用
来源：http://foi.316326.xyz

df -h;  du -sh *
来源：http://vlk.svipenyu.cn

[R62] 找最占空间的文件
来源：http://eid.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://nkg.zhixingplan.top

[R63] 内存与进程
来源：http://bds.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://hom.jqgfzy.top

[R64] 结束进程
来源：http://zkh.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://znt.ehwqpu.com

[R65] 查看端口占用
来源：http://esz.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdk.yangfankeji.com

[R66] 定时任务
来源：http://fkg.ybcxt.top

crontab -e;  crontab -l
来源：http://auk.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://bxt.vehdjk.com

openssl rand -hex 16
来源：http://qdq.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://opq.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mco.nanxuanxn.top

[R69] 生成随机密码
来源：http://amf.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://qwd.yangfankeji.com

[R70] 时间戳与互转
来源：http://tol.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://jkq.wangshuangyany.cn

[R71] 日期格式化
来源：http://hfm.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qbm.zhixingplan.top

[R72] 等待端口就绪
来源：http://rsu.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vzj.pycfn.com

[R73] 分割大日志
来源：http://xit.cucudq.cn

split -l 1000 big.log part_
来源：http://zyu.jinqigfzy.top

[R74] 批量重命名
来源：http://mdh.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qqk.hfpthk.cn

[R75] 导出环境变量
来源：http://prm.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ryb.ydjk.org.cn

[R76] 使用临时文件
来源：http://bfj.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ahx.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://ycy.sweek.top

read -rp "请输入: " ans
来源：http://bto.ctjpmb.com

[R78] 交互式菜单
来源：http://vhd.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ygy.yj20258888.top

[R79] 解析命令行选项
来源：http://gvm.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hja.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://gje.jinqigufen.top

time ./run.sh
来源：http://axk.gogol.net.cn

================================================================================
来源：http://vbj.xinyue.icu

S. C / C++ 专题
来源：http://ifa.zhaomingkeji.xyz

================================================================================
来源：http://qky.guowangkeji.top

[S01] C：Hello World
来源：http://bkx.yueranfly.top

#include <stdio.h>
来源：http://oga.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rvu.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://tlv.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://fyp.meibo888.top

[S03] C：读入整数
来源：http://nji.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://ntd.gogol.net.cn

[S04] C：字符串复制
来源：http://vzn.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://krs.yj20258888.top

[S05] C：字符串长度
来源：http://rno.yonumen.top

strlen(s)
来源：http://zok.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://wox.andypj.xyz

strcmp(a, b) == 0
来源：http://pce.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://lps.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gxm.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://zdb.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://err.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://tjq.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gje.gaohongyu789.top

[S10] C：指针与解引用
来源：http://asz.sweek.top

int *p = &a;  *p = 5;
来源：http://oav.zhongyouzk.top

[S11] C：逐行读文件
来源：http://oob.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://hrg.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vmu.hfpthk.cn

fclose(f);
来源：http://zhd.bbcook.cn

[S12] C：写文件
来源：http://anx.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jxv.mhx1999.top

[S13] C：宏定义
来源：http://toh.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://san.pengpengdd.cyou

[S14] C：枚举
来源：http://szh.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://sdp.yuanzhike.top

[S15] C：类型转换
来源：http://ize.meibo888.top

(double) a / b
来源：http://ent.havefunace.top

[S16] C：位操作置位
来源：http://jiq.gotoacloud.top

x |= (1 << 3);
来源：http://kbt.ybcxt.top

[S17] C：安全拼接字符串
来源：http://jxe.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qmy.yj20258888.top

[S18] C：命令行参数
来源：http://enu.hysaishi.cn

int main(int argc, char **argv)
来源：http://lju.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://dyi.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://vnu.yongpay.top

[S20] C：二分查找
来源：http://ctj.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qyk.sweek.top

[S21] C：字符类别判断
来源：http://stn.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://efr.vqdsnc.cn

[S22] C：字符串转数字
来源：http://ybe.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://cjs.chenlongwang.top

[S23] C：随机数
来源：http://fou.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ouv.fzhhl.top

[S24] C：获取本地时间
来源：http://mzu.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fit.zdbjq.cn

[S25] C：内存拷贝
来源：http://cnd.meibo888.top

memcpy(dst, src, n);
来源：http://erc.yangfankeji.com

[S26] C：内存清零
来源：http://tpr.nwbrower.top

memset(a, 0, sizeof a);
来源：http://cgo.ybcxt.top

[S27] C：定义常量
来源：http://wnx.uphjek.com

const double PI = 3.14159;
来源：http://evh.snrcjt.cn

[S28] C：静态变量
来源：http://yxu.nanxinkj.top

static int counter = 0;
来源：http://lxa.daxiang520.top

[S29] C：变参函数
来源：http://mbz.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://woq.yj20258888.top

[S30] C：头文件保护
来源：http://ruf.wangdashe.top

#ifndef X_H
来源：http://vaq.xinyue.icu

#define X_H
来源：http://hsk.redwolf501.top

#endif
来源：http://kkz.c1oappe.top

[S31] C++：Hello World
来源：http://ebz.fehbvm.com

#include <iostream>
来源：http://dwg.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://twj.uphjek.com

[S32] C++：字符串
来源：http://bws.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://pfd.zhoulong.xyz

[S33] C++：vector 增删
来源：http://zwr.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jkw.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://vsw.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://bch.ydzc1.top

[S35] C++：map
来源：http://pus.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://irw.ivvv.top

[S36] C++：unordered_map
来源：http://qiv.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wqj.pycfn.com

[S37] C++：set
来源：http://bfm.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aks.hywenlv.cn

[S38] C++：排序
来源：http://qxz.cheryme.top

std::sort(v.begin(), v.end());
来源：http://dth.pycfn.com

[S39] C++：自定义比较器排序
来源：http://qoj.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gfi.xylfe.cn

[S40] C++：查找元素
来源：http://rie.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hir.yvedp.cn

[S41] C++：类与构造函数
来源：http://xov.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://srm.sxryk.cn

[S42] C++：继承与虚函数
来源：http://jtg.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://ino.cqqwz.cn

[S43] C++：智能指针
来源：http://ypm.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://wky.0kj1m.cn

[S44] C++：引用传参
来源：http://pch.fehbvm.com

void inc(int &x) { ++x; }
来源：http://ewq.chenzaomai.com

[S45] C++：lambda
来源：http://qgi.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://gja.jinqigfzy.top

[S46] C++：函数模板
来源：http://jnp.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jpn.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://ucw.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zmu.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://plf.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://jjp.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://zln.shuidangran.top

[S49] C++：写文件
来源：http://lvl.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jia.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://juj.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yvw.snrcjt.cn

[S51] C++：显式类型转换
来源：http://wkc.chenlongwang.top

static_cast<double>(a) / b
来源：http://dvb.yj20258.top

[S52] C++：const 与 noexcept
来源：http://mst.c1oappe.top

int size() const noexcept { return n_; }
来源：http://drp.cashguo.top

[S53] C++：移动语义
来源：http://ard.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://cfc.bjfxy.top

[S54] C++：异常处理
来源：http://txb.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ceu.tian-w.cn

[S55] C++：结构化绑定
来源：http://zuw.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ebz.hnxiangtu.top

[S56] C++：optional
来源：http://twu.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hfk.jlsjyb.cn

[S57] C++：编译期常量
来源：http://tba.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://xya.yvedp.cn

[S58] C++：命名空间
来源：http://vhu.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://mpf.hnxiangtu.top

[S59] C++：静态断言
来源：http://kwj.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rmj.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://xhs.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jsh.xinyue.icu

================================================================================
来源：http://ldq.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lai.vehdjk.com

================================================================================
来源：http://xym.jianghu66.top


<!-- 参考信息 -->