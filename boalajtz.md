代发 wailian999

R. Bash 专题
来源：http://duu.sysykeji.top

================================================================================
来源：http://oph.ybcxt.top

[R01] shebang 与严格模式
来源：http://zed.vehdjk.com

#!/usr/bin/env bash
来源：http://cwt.redwolf501.top

set -euo pipefail
来源：http://ayy.hnqzz.top

[R02] 变量赋值与使用
来源：http://zic.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://aml.ctjpmb.com

[R03] 只读变量
来源：http://tyf.xinyue.icu

readonly PI=3.14
来源：http://eos.sjlbkw.cn

[R04] 位置参数
来源：http://uty.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tmm.jianghu66.top

[R05] 参数默认值
来源：http://hcd.yj20258.top

name="${1:-default}"
来源：http://bhn.mhx1999.top

[R06] 判断命令是否存在
来源：http://kuf.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzn.zhixingplan.top

[R07] if 判断文件
来源：http://row.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hin.hongshengwenyu.top

[R08] 数值比较
来源：http://tih.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nea.zhoulong.xyz

[R09] 字符串比较
来源：http://tun.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zka.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://zrh.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ckf.sufxvd.cn

[R11] case 多分支
来源：http://lch.epnwcf.com

case "$1" in
来源：http://hqr.aizwys.cn

start) echo "启动" ;;
来源：http://jdt.xylfe.cn

stop)  echo "停止" ;;
来源：http://rts.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://awr.gaohongyu789.top

esac
来源：http://jpv.tanke756.top

[R12] for 遍历文件
来源：http://zwm.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://qbx.zhongyouzk.top

[R13] for 计数循环
来源：http://wqj.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://mcb.sxryk.cn

[R14] C 风格 for
来源：http://pit.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lql.birdmap.top

[R15] while 逐行读文件
来源：http://smb.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lio.daxiang520.top

[R16] until 等待条件
来源：http://pvv.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://upy.guowangkeji.top

[R17] 数组定义与取值
来源：http://eax.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uyj.gzhubu.top

[R18] 遍历数组
来源：http://flx.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tsw.hammf.cn

[R19] 数组长度
来源：http://sfa.iojbl.cn

echo "${#arr[@]}"
来源：http://qby.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://yrg.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://prh.chenlongwang.top

[R21] 字符串长度
来源：http://tgc.hammf.cn

echo "${#s}"
来源：http://npc.cheryme.top

[R22] 截取子串
来源：http://bbm.epnwcf.com

echo "${s:0:5}"
来源：http://mxq.hfpthk.cn

[R23] 字符串替换
来源：http://cwh.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zaz.gogol.net.cn

[R24] 大小写转换
来源：http://ekj.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ypt.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://yki.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qmf.fanxiaobao.xyz

[R26] 命令替换
来源：http://dwk.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://vlz.zhijiandao.cn

[R27] 算术展开
来源：http://tyl.fehbvm.com

echo $((1 + 2 * 3))
来源：http://vxb.yonumen.top

[R28] 浮点运算
来源：http://ewr.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://wdj.shuidangran.top

[R29] 定义函数
来源：http://wrt.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jep.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://jyh.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://kdl.zhiwuduotai.top

[R31] 局部变量
来源：http://jri.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://xew.gogol.net.cn

[R32] 参数个数校验
来源：http://icz.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iyh.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://cbo.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hel.hysaishi.cn

[R34] 退出时清理
来源：http://tmy.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://mqm.tian-w.cn

[R35] 后台执行并等待
来源：http://ief.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kvr.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://eut.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgz.yfazqb.com

[R37] 把输出赋给变量
来源：http://zoc.cashguo.top

files=$(ls -1)
来源：http://pyj.guannengcc.top

[R38] 管道串联
来源：http://bvt.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://err.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://rsl.tian-w.cn

cmd > out.log 2>&1
来源：http://ryy.svipenyu.cn

[R40] 追加写日志
来源：http://scv.wangshuangyany.cn

echo "log" >> out.log
来源：http://vyz.ybcxt.top

[R41] 丢弃输出
来源：http://tjz.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://mzh.hesvh.cn

[R42] 输入重定向
来源：http://dod.fehbvm.com

wc -l < a.txt
来源：http://dcv.daria6918.cn

[R43] 按名字查找文件
来源：http://ncb.hammf.cn

find . -name "*.log" -type f
来源：http://ecs.jqgfzy.top

[R44] 按修改时间查找
来源：http://aaj.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://eub.9152youxi.cn

[R45] 批量删除
来源：http://tno.yfazqb.com

find . -name "*.tmp" -delete
来源：http://owp.fengsongda.top

[R46] 递归替换文件内容
来源：http://suw.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wzd.uphjek.com

[R47] sed 单行替换
来源：http://kjg.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://nbz.shzxlz.cn

[R48] awk 取指定列
来源：http://wdb.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://dyr.nanxinkj.top

[R49] awk 带条件
来源：http://nnq.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tio.wangshuangyany.cn

[R50] awk 求和
来源：http://awc.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://cko.epnwcf.com

[R51] 排序去重取前几
来源：http://wlq.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xdl.snrcjt.cn

[R52] 统计行数
来源：http://uoc.yanxiufei.cn

wc -l a.txt
来源：http://yah.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://mmi.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lic.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://cja.yj20258888.top

diff a.txt b.txt
来源：http://znz.xuetiantiany.cn

[R55] 压缩与解压
来源：http://lln.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://poy.kuanghao11.cn

[R56] 远程拷贝
来源：http://pvr.hnqzz.top

scp file user@host:/path/
来源：http://cfo.redwolf501.top

[R57] 远程执行命令
来源：http://iby.yuanzhike.top

ssh user@host 'uptime'
来源：http://szw.gotoacloud.top

[R58] 下载文件
来源：http://pqq.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vdd.jlsjyb.cn

[R59] 发 POST JSON
来源：http://pzk.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxh.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://waq.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://agd.daxiang520.top

[R61] 磁盘占用
来源：http://lix.zhengqikj.top

df -h;  du -sh *
来源：http://cnn.havefunace.top

[R62] 找最占空间的文件
来源：http://dxd.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://kis.ydjk.org.cn

[R63] 内存与进程
来源：http://qho.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://bqf.hfpthk.cn

[R64] 结束进程
来源：http://jfn.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://aue.bbcook.cn

[R65] 查看端口占用
来源：http://zwo.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wzc.xylfe.cn

[R66] 定时任务
来源：http://lra.yfazqb.com

crontab -e;  crontab -l
来源：http://ztr.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://iey.quarkkingdee.top

openssl rand -hex 16
来源：http://pae.nanxinkj.top

[R68] 计算文件校验值
来源：http://mlw.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qte.iojbl.cn

[R69] 生成随机密码
来源：http://nqv.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://peh.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://evy.yuxming.cn

date +%s;  date -d @1700000000
来源：http://ttc.dashuyun.cn

[R71] 日期格式化
来源：http://wnf.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://uai.shuidangran.top

[R72] 等待端口就绪
来源：http://bys.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://amv.zycfv.cn

[R73] 分割大日志
来源：http://ytc.hywenlv.cn

split -l 1000 big.log part_
来源：http://llm.yj20258888.top

[R74] 批量重命名
来源：http://iqk.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fsm.yuxming.cn

[R75] 导出环境变量
来源：http://pnd.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://jav.zhengqikj.top

[R76] 使用临时文件
来源：http://krb.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kfk.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://phu.sysykeji.top

read -rp "请输入: " ans
来源：http://amm.sxryk.cn

[R78] 交互式菜单
来源：http://fqj.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://byk.xylfe.cn

[R79] 解析命令行选项
来源：http://xek.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mak.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://lsw.hnxiangtu.top

time ./run.sh
来源：http://dvx.smart0.xyz

================================================================================
来源：http://sxj.sysykeji.top

S. C / C++ 专题
来源：http://scv.jyoumei.cn

================================================================================
来源：http://nua.ybcxt.top

[S01] C：Hello World
来源：http://rdb.shzxlz.cn

#include <stdio.h>
来源：http://fcx.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwq.wangdashe.top

[S02] C：变量与格式化输出
来源：http://szo.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://fmc.nanxuanxn.top

[S03] C：读入整数
来源：http://gwu.ehwqpu.com

int x; scanf("%d", &x);
来源：http://svz.hysaishi.cn

[S04] C：字符串复制
来源：http://uso.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yhb.pengpengdd.cyou

[S05] C：字符串长度
来源：http://iyf.tian-w.cn

strlen(s)
来源：http://rrc.316326.xyz

[S06] C：字符串比较
来源：http://lwc.meibo888.top

strcmp(a, b) == 0
来源：http://egm.zhixingplan.top

[S07] C：数组遍历求和
来源：http://kmr.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mzo.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://kmz.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://giw.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://juq.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bzl.aibaodan.cn

[S10] C：指针与解引用
来源：http://xid.havefunace.top

int *p = &a;  *p = 5;
来源：http://mga.yfazqb.com

[S11] C：逐行读文件
来源：http://pmk.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://dte.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wew.fehbvm.com

fclose(f);
来源：http://wkk.zhoulong.xyz

[S12] C：写文件
来源：http://mel.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eze.chenjidiqi.icu

[S13] C：宏定义
来源：http://rsc.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bhf.smart0.xyz

[S14] C：枚举
来源：http://gxy.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://rlr.guowangkeji.top

[S15] C：类型转换
来源：http://dlz.nwbrower.top

(double) a / b
来源：http://xtk.hongshengwenyu.top

[S16] C：位操作置位
来源：http://ipb.zhengqikj.top

x |= (1 << 3);
来源：http://ioc.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://kyo.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qau.zdbjq.cn

[S18] C：命令行参数
来源：http://hna.cdnleiting.top

int main(int argc, char **argv)
来源：http://eit.xylfe.cn

[S19] C：快速排序
来源：http://sca.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://utq.vehdjk.com

[S20] C：二分查找
来源：http://hvw.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhn.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://xrx.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://feq.zhijiandao.cn

[S22] C：字符串转数字
来源：http://rzx.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://gvb.xuetiantiany.cn

[S23] C：随机数
来源：http://alo.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dil.yvedp.cn

[S24] C：获取本地时间
来源：http://omn.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://few.tian-w.cn

[S25] C：内存拷贝
来源：http://yby.9152youxi.cn

memcpy(dst, src, n);
来源：http://iyt.zhongyouzk.top

[S26] C：内存清零
来源：http://rly.andypj.xyz

memset(a, 0, sizeof a);
来源：http://rue.ydzc1.top

[S27] C：定义常量
来源：http://xpg.ctjpmb.com

const double PI = 3.14159;
来源：http://iuz.gzhubu.top

[S28] C：静态变量
来源：http://tah.jinqigfzy.top

static int counter = 0;
来源：http://tny.chenlongwang.top

[S29] C：变参函数
来源：http://yad.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xpf.tianlin.xyz

[S30] C：头文件保护
来源：http://cbi.cdnleiting.top

#ifndef X_H
来源：http://yph.ivvv.top

#define X_H
来源：http://tou.ctjpmb.com

#endif
来源：http://cqg.hnqzz.top

[S31] C++：Hello World
来源：http://qop.jqgufenzy.top

#include <iostream>
来源：http://zvc.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://bsg.tian-w.cn

[S32] C++：字符串
来源：http://tmv.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://ljf.xziqi.cn

[S33] C++：vector 增删
来源：http://wjz.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dox.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://dml.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://kcn.tian-w.cn

[S35] C++：map
来源：http://nks.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ftp.cdnleiting.top

[S36] C++：unordered_map
来源：http://jxc.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ade.pycfn.com

[S37] C++：set
来源：http://orw.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ujx.smart0.xyz

[S38] C++：排序
来源：http://guk.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://ndv.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://xuw.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wrn.hnqzz.top

[S40] C++：查找元素
来源：http://hzr.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cri.ydzc1.top

[S41] C++：类与构造函数
来源：http://bon.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zzh.gzhubu.top

[S42] C++：继承与虚函数
来源：http://dbl.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://lvy.vehdjk.com

[S43] C++：智能指针
来源：http://svs.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ugf.52xcode.cn

[S44] C++：引用传参
来源：http://qsd.sweek.top

void inc(int &x) { ++x; }
来源：http://uyr.nanxuanxn.top

[S45] C++：lambda
来源：http://yct.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://wew.shzxlz.cn

[S46] C++：函数模板
来源：http://rwd.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://onb.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://bde.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rdh.andypj.xyz

[S48] C++：逐行读文件
来源：http://jha.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tui.daria6918.cn

while (std::getline(in, line)) { }
来源：http://vku.pycfn.com

[S49] C++：写文件
来源：http://eml.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rhq.hfpthk.cn

[S50] C++：格式化数字
来源：http://srt.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zsa.zycfv.cn

[S51] C++：显式类型转换
来源：http://mgg.sufxvd.cn

static_cast<double>(a) / b
来源：http://uwi.tanke756.top

[S52] C++：const 与 noexcept
来源：http://tty.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://fsp.aibaodan.cn

[S53] C++：移动语义
来源：http://guz.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://uzf.zhengqikj.top

[S54] C++：异常处理
来源：http://sjn.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yqu.havefunace.top

[S55] C++：结构化绑定
来源：http://jxt.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nml.fengsongda.top

[S56] C++：optional
来源：http://erd.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ivg.zycfv.cn

[S57] C++：编译期常量
来源：http://vvz.feifeiyinyue.top

constexpr int N = 10;
来源：http://xdh.yanxiufei.cn

[S58] C++：命名空间
来源：http://gfm.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://hnj.jinqigufen.top

[S59] C++：静态断言
来源：http://btc.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqh.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://vzd.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://svg.wangdashe.top

================================================================================
来源：http://czb.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ckl.shzxlz.cn

================================================================================
来源：http://kdu.yuanzhike.top


<!-- 参考信息 -->