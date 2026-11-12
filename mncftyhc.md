代发 wailian999

set -euo pipefail
来源：http://isb.fehbvm.com

[R02] 变量赋值与使用
来源：http://ymi.ppjwa.cn

name="Tom"; echo "$name"
来源：http://qpn.jianghu66.top

[R03] 只读变量
来源：http://mwn.hysaishi.cn

readonly PI=3.14
来源：http://rwk.shanyushiyangtech.top

[R04] 位置参数
来源：http://mgr.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://atf.ybcxt.top

[R05] 参数默认值
来源：http://pji.hnqzz.top

name="${1:-default}"
来源：http://koz.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://emi.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bbw.zhiwuduotai.top

[R07] if 判断文件
来源：http://myy.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jxf.jlsjyb.cn

[R08] 数值比较
来源：http://reg.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://erx.sufxvd.cn

[R09] 字符串比较
来源：http://uvo.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://skj.mhx1999.top

[R10] 正则匹配
来源：http://voc.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kot.hammf.cn

[R11] case 多分支
来源：http://rxg.jinghuilouyu.cn

case "$1" in
来源：http://xgz.gzhubu.top

start) echo "启动" ;;
来源：http://yxx.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://qcx.cucudq.cn

*)     echo "未知命令" ;;
来源：http://cqd.yangfankeji.com

esac
来源：http://tae.yanxiufei.cn

[R12] for 遍历文件
来源：http://uec.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://mnr.ybcxt.top

[R13] for 计数循环
来源：http://shh.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://alm.vqdsnc.cn

[R14] C 风格 for
来源：http://qiz.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eqi.chenlongwang.top

[R15] while 逐行读文件
来源：http://slq.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cac.aibaodan.cn

[R16] until 等待条件
来源：http://rav.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vle.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://ztu.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fmz.tianlin.xyz

[R18] 遍历数组
来源：http://pvy.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://czb.fktsv.cn

[R19] 数组长度
来源：http://wot.nanxinkj.top

echo "${#arr[@]}"
来源：http://cyt.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://ewv.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hoy.c1oappe.top

[R21] 字符串长度
来源：http://dtt.dashuyun.cn

echo "${#s}"
来源：http://unt.0kj1m.cn

[R22] 截取子串
来源：http://uld.uphjek.com

echo "${s:0:5}"
来源：http://iqz.havefunace.top

[R23] 字符串替换
来源：http://adg.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qwm.hesvh.cn

[R24] 大小写转换
来源：http://bnl.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://pid.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://cmw.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsi.jinqigufen.top

[R26] 命令替换
来源：http://cfm.hammf.cn

now=$(date +%F); echo "$now"
来源：http://zhy.havefunace.top

[R27] 算术展开
来源：http://oam.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://nix.jinqigufen.top

[R28] 浮点运算
来源：http://xgt.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://cvc.bbcook.cn

[R29] 定义函数
来源：http://ltw.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oqk.gzhubu.top

[R30] 函数返回状态码
来源：http://ziq.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ico.vqdsnc.cn

[R31] 局部变量
来源：http://mky.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://bzz.aibaodan.cn

[R32] 参数个数校验
来源：http://jog.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jxs.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://eoi.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wvf.xziqi.cn

[R34] 退出时清理
来源：http://yxu.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://pmn.mhx1999.top

[R35] 后台执行并等待
来源：http://qsz.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jud.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://dud.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vfw.redwolf501.top

[R37] 把输出赋给变量
来源：http://lcv.xziqi.cn

files=$(ls -1)
来源：http://sfx.uphjek.com

[R38] 管道串联
来源：http://hib.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://sfg.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://fqt.andypj.xyz

cmd > out.log 2>&1
来源：http://qkx.cheryme.top

[R40] 追加写日志
来源：http://tnv.yfazqb.com

echo "log" >> out.log
来源：http://wvo.shangyingyoupin.top

[R41] 丢弃输出
来源：http://knl.daria6918.cn

cmd >/dev/null 2>&1
来源：http://ccw.zycfv.cn

[R42] 输入重定向
来源：http://fio.0kj1m.cn

wc -l < a.txt
来源：http://era.cheryme.top

[R43] 按名字查找文件
来源：http://kds.aizwys.cn

find . -name "*.log" -type f
来源：http://vjy.tarul.cn

[R44] 按修改时间查找
来源：http://ses.xinyue.icu

find . -mtime -7 -type f
来源：http://fnz.hywenlv.cn

[R45] 批量删除
来源：http://emz.sxryk.cn

find . -name "*.tmp" -delete
来源：http://xkd.yj20258.top

[R46] 递归替换文件内容
来源：http://hic.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cqj.redwolf501.top

[R47] sed 单行替换
来源：http://njs.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://jsl.guannengcc.top

[R48] awk 取指定列
来源：http://mhw.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://lbm.cdnleiting.top

[R49] awk 带条件
来源：http://lev.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pwi.zhengqikj.top

[R50] awk 求和
来源：http://wgv.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://tzc.ybcxt.top

[R51] 排序去重取前几
来源：http://dnd.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ibb.vehdjk.com

[R52] 统计行数
来源：http://kbk.zdqjudy.top

wc -l a.txt
来源：http://xlg.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://sfe.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jlt.jqgufenzy.top

[R54] 比较两个文件
来源：http://vai.sxryk.cn

diff a.txt b.txt
来源：http://lrw.epnwcf.com

[R55] 压缩与解压
来源：http://eqj.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uyv.redwolf501.top

[R56] 远程拷贝
来源：http://jsp.hnqzz.top

scp file user@host:/path/
来源：http://lgz.shangyingyoupin.top

[R57] 远程执行命令
来源：http://ifk.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://tkp.zhixingplan.top

[R58] 下载文件
来源：http://dps.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qoc.ehwqpu.com

[R59] 发 POST JSON
来源：http://gnv.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jcw.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://xzv.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yhg.havefunace.top

[R61] 磁盘占用
来源：http://uyg.nanxuanxn.top

df -h;  du -sh *
来源：http://llv.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://mcy.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://mzg.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://vhj.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://apr.sjlbkw.cn

[R64] 结束进程
来源：http://slg.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://tnj.havefunace.top

[R65] 查看端口占用
来源：http://cyg.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nhv.yanxiufei.cn

[R66] 定时任务
来源：http://qpb.zdqjudy.top

crontab -e;  crontab -l
来源：http://ihp.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://ayd.ppjwa.cn

openssl rand -hex 16
来源：http://uid.svipenyu.cn

[R68] 计算文件校验值
来源：http://zkk.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://lyf.hcnkem.com

[R69] 生成随机密码
来源：http://stz.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://rpz.aizwys.cn

[R70] 时间戳与互转
来源：http://amb.hammf.cn

date +%s;  date -d @1700000000
来源：http://btx.andypj.xyz

[R71] 日期格式化
来源：http://skp.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aua.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://coz.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vrr.52xcode.cn

[R73] 分割大日志
来源：http://loe.yangfankeji.com

split -l 1000 big.log part_
来源：http://wps.xuetiantiany.cn

[R74] 批量重命名
来源：http://kee.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eif.ydjk.org.cn

[R75] 导出环境变量
来源：http://kbz.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://cpq.xylfe.cn

[R76] 使用临时文件
来源：http://zza.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hqr.jlsjyb.cn

[R77] 读取用户输入
来源：http://tfp.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://tod.fzhhl.top

[R78] 交互式菜单
来源：http://nyo.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gvs.hcnkem.com

[R79] 解析命令行选项
来源：http://wjh.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ylz.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://yqi.zhixingplan.top

time ./run.sh
来源：http://qiu.bjfxy.top

================================================================================
来源：http://jru.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://lnj.hesvh.cn

================================================================================
来源：http://hdz.fengsongda.top

[S01] C：Hello World
来源：http://jxr.chenzaomai.com

#include <stdio.h>
来源：http://cup.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lfy.epnwcf.com

[S02] C：变量与格式化输出
来源：http://jxa.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://erd.meibo888.top

[S03] C：读入整数
来源：http://nsi.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://xju.aizwys.cn

[S04] C：字符串复制
来源：http://emi.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://ssc.nanxuanxn.top

[S05] C：字符串长度
来源：http://tpz.yanxiufei.cn

strlen(s)
来源：http://fvi.jyoumei.cn

[S06] C：字符串比较
来源：http://omo.fzhhl.top

strcmp(a, b) == 0
来源：http://bjs.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://hfh.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ygl.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://zro.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wcd.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://euq.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ahr.tian-w.cn

[S10] C：指针与解引用
来源：http://you.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://jth.gaohongyu789.top

[S11] C：逐行读文件
来源：http://tgc.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://oxi.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ago.chenlongwang.top

fclose(f);
来源：http://enr.ctjpmb.com

[S12] C：写文件
来源：http://pvz.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rsy.fehbvm.com

[S13] C：宏定义
来源：http://mpn.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://feb.mhx1999.top

[S14] C：枚举
来源：http://djn.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://oyu.yonumen.top

[S15] C：类型转换
来源：http://jbp.gogol.net.cn

(double) a / b
来源：http://zlq.bjfxy.top

[S16] C：位操作置位
来源：http://eig.gzhubu.top

x |= (1 << 3);
来源：http://pzr.zycfv.cn

[S17] C：安全拼接字符串
来源：http://xlg.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jfz.iojbl.cn

[S18] C：命令行参数
来源：http://cee.yangfankeji.com

int main(int argc, char **argv)
来源：http://vdf.pengpengdd.cyou

[S19] C：快速排序
来源：http://jqb.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://lvs.shuidangran.top

[S20] C：二分查找
来源：http://obo.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ybe.nanxinkj.top

[S21] C：字符类别判断
来源：http://wrl.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://icq.fzhhl.top

[S22] C：字符串转数字
来源：http://efa.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://joy.ctjpmb.com

[S23] C：随机数
来源：http://hvk.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jxn.hammf.cn

[S24] C：获取本地时间
来源：http://qoi.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aad.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://gpn.sxryk.cn

memcpy(dst, src, n);
来源：http://ngt.tarul.cn

[S26] C：内存清零
来源：http://lnb.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://nik.wangdashe.top

[S27] C：定义常量
来源：http://sfs.dashuyun.cn

const double PI = 3.14159;
来源：http://xjs.feifeiyinyue.top

[S28] C：静态变量
来源：http://itu.xuanzx.com

static int counter = 0;
来源：http://vmh.yueranfly.top

[S29] C：变参函数
来源：http://dtl.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qgd.wangshuangyany.cn

[S30] C：头文件保护
来源：http://xjl.jinqigfzy.top

#ifndef X_H
来源：http://agj.zhengqikj.top

#define X_H
来源：http://lfj.bjfxy.top

#endif
来源：http://gem.guannengcc.top

[S31] C++：Hello World
来源：http://bmh.ydzc1.top

#include <iostream>
来源：http://jfi.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://ict.daxiang520.top

[S32] C++：字符串
来源：http://jxa.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://dii.ydzc1.top

[S33] C++：vector 增删
来源：http://awv.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://poe.xylfe.cn

[S34] C++：遍历 vector
来源：http://yfu.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://fjf.zhiwuduotai.top

[S35] C++：map
来源：http://rew.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rgc.yj20258888.top

[S36] C++：unordered_map
来源：http://nwp.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://trd.mhx1999.top

[S37] C++：set
来源：http://ntt.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fms.fengsongda.top

[S38] C++：排序
来源：http://fuo.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://jyx.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://wir.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fyh.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://nxc.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://por.iojbl.cn

[S41] C++：类与构造函数
来源：http://plo.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rrr.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://pov.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://ezs.iojbl.cn

[S43] C++：智能指针
来源：http://ifm.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://xzs.chenlongwang.top

[S44] C++：引用传参
来源：http://ewp.smart0.xyz

void inc(int &x) { ++x; }
来源：http://lvo.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://ssy.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://fvc.yfazqb.com

[S46] C++：函数模板
来源：http://tew.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rdw.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://mnp.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://znl.gogol.net.cn

[S48] C++：逐行读文件
来源：http://rve.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://agi.sweek.top

while (std::getline(in, line)) { }
来源：http://prj.epnwcf.com

[S49] C++：写文件
来源：http://vup.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://geo.daria6918.cn

[S50] C++：格式化数字
来源：http://nfi.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uih.c1oappe.top

[S51] C++：显式类型转换
来源：http://pfv.0kj1m.cn

static_cast<double>(a) / b
来源：http://oxc.tanke756.top

[S52] C++：const 与 noexcept
来源：http://mmz.bjfxy.top

int size() const noexcept { return n_; }
来源：http://kus.fehbvm.com

[S53] C++：移动语义
来源：http://hfq.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://iuu.yangfankeji.com

[S54] C++：异常处理
来源：http://oke.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xog.sysykeji.top

[S55] C++：结构化绑定
来源：http://acy.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rjh.xuanzx.com

[S56] C++：optional
来源：http://bds.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fna.quarkkingdee.top

[S57] C++：编译期常量
来源：http://ugy.hammf.cn

constexpr int N = 10;
来源：http://ybk.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://uim.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://aiz.tian-w.cn

[S59] C++：静态断言
来源：http://wcz.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jmx.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://qyg.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qje.pengpengdd.cyou

================================================================================
来源：http://rlq.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tjg.zycfv.cn

================================================================================
来源：http://yzm.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://nmj.smart0.xyz

println("Hello")
来源：http://lgr.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://kxp.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zma.havefunace.top


<!-- 参考信息 -->