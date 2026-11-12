代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kev.tianlin.xyz

[Q90] 生成序号列
来源：http://nwk.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxv.ppjwa.cn

================================================================================
来源：http://dta.gaohongyu789.top

R. Bash 专题
来源：http://cpr.aibaodan.cn

================================================================================
来源：http://uyy.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://pxb.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://qxi.zdqjudy.top

set -euo pipefail
来源：http://xve.cucudq.cn

[R02] 变量赋值与使用
来源：http://hpc.fehbvm.com

name="Tom"; echo "$name"
来源：http://opa.hfpthk.cn

[R03] 只读变量
来源：http://nkb.yj20258888.top

readonly PI=3.14
来源：http://pnn.bbcook.cn

[R04] 位置参数
来源：http://kvx.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hqt.yonumen.top

[R05] 参数默认值
来源：http://zwh.wangdashe.top

name="${1:-default}"
来源：http://cbr.chenlongwang.top

[R06] 判断命令是否存在
来源：http://kzb.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lrs.hammf.cn

[R07] if 判断文件
来源：http://oqf.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fld.chenjidiqi.icu

[R08] 数值比较
来源：http://zoy.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lza.daxiang520.top

[R09] 字符串比较
来源：http://bvj.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yrn.yangfankeji.com

[R10] 正则匹配
来源：http://uhm.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eay.ywan-chungtsiang.top

[R11] case 多分支
来源：http://ikc.dianchejie.cn

case "$1" in
来源：http://xhi.yfazqb.com

start) echo "启动" ;;
来源：http://duf.gzhubu.top

stop)  echo "停止" ;;
来源：http://htt.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://xya.daria6918.cn

esac
来源：http://apf.zycfv.cn

[R12] for 遍历文件
来源：http://lzb.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://txk.zhoulong.xyz

[R13] for 计数循环
来源：http://caj.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://feg.fzhhl.top

[R14] C 风格 for
来源：http://fpm.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aym.yj202588.top

[R15] while 逐行读文件
来源：http://zsm.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://abd.shuidangran.top

[R16] until 等待条件
来源：http://jzh.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wie.tanke756.top

[R17] 数组定义与取值
来源：http://gof.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://rdc.jqgufenzy.top

[R18] 遍历数组
来源：http://juw.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zln.gaohongyu789.top

[R19] 数组长度
来源：http://edd.sjlbkw.cn

echo "${#arr[@]}"
来源：http://abr.gzhubu.top

[R20] 关联数组（字典）
来源：http://gbe.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nhb.guowangkeji.top

[R21] 字符串长度
来源：http://gxl.hesvh.cn

echo "${#s}"
来源：http://wjv.jqgfzy.top

[R22] 截取子串
来源：http://hak.tarul.cn

echo "${s:0:5}"
来源：http://ntl.vqdsnc.cn

[R23] 字符串替换
来源：http://vor.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nio.jinqigfzy.top

[R24] 大小写转换
来源：http://gfi.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://twp.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://ecz.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://phd.ppjwa.cn

[R26] 命令替换
来源：http://amv.ivvv.top

now=$(date +%F); echo "$now"
来源：http://hei.xinyue.icu

[R27] 算术展开
来源：http://pdx.tian-w.cn

echo $((1 + 2 * 3))
来源：http://utf.aibaodan.cn

[R28] 浮点运算
来源：http://mtm.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://gqi.chenzaomai.com

[R29] 定义函数
来源：http://nzu.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sez.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://nvc.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://umu.xziqi.cn

[R31] 局部变量
来源：http://ivt.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://rtm.yangfankeji.com

[R32] 参数个数校验
来源：http://lel.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ncl.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://njj.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pvu.svipenyu.cn

[R34] 退出时清理
来源：http://yhb.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xvy.jqgfzy.top

[R35] 后台执行并等待
来源：http://dfl.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uvb.jianghu66.top

[R36] 并发执行多个任务
来源：http://los.fanxiaobao.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lmp.nwbrower.top

[R37] 把输出赋给变量
来源：http://vwv.chenlongwang.top

files=$(ls -1)
来源：http://ymh.pengpengdd.cyou

[R38] 管道串联
来源：http://bst.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://yun.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://mcx.xylfe.cn

cmd > out.log 2>&1
来源：http://aak.yanxiufei.cn

[R40] 追加写日志
来源：http://rba.xuetiantiany.cn

echo "log" >> out.log
来源：http://yfw.sufxvd.cn

[R41] 丢弃输出
来源：http://mqc.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://jdt.meibo888.top

[R42] 输入重定向
来源：http://asu.hnxiangtu.top

wc -l < a.txt
来源：http://raj.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://cmq.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://izu.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://lie.yangfankeji.com

find . -mtime -7 -type f
来源：http://ain.jlsjyb.cn

[R45] 批量删除
来源：http://jfn.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://phe.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://avx.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kfl.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://mjm.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dpn.ivvv.top

[R48] awk 取指定列
来源：http://cam.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://bek.smart0.xyz

[R49] awk 带条件
来源：http://xtt.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wdd.jinyuanbaomall.cn

[R50] awk 求和
来源：http://xav.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fyt.cdnleiting.top

[R51] 排序去重取前几
来源：http://mhc.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fmx.aizwys.cn

[R52] 统计行数
来源：http://vus.c1oappe.top

wc -l a.txt
来源：http://tbl.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://tke.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zxw.shuidangran.top

[R54] 比较两个文件
来源：http://vcw.shangyingyoupin.top

diff a.txt b.txt
来源：http://tai.yuxming.cn

[R55] 压缩与解压
来源：http://tem.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sae.pycfn.com

[R56] 远程拷贝
来源：http://bnk.andypj.xyz

scp file user@host:/path/
来源：http://hlq.fehbvm.com

[R57] 远程执行命令
来源：http://kso.cheryme.top

ssh user@host 'uptime'
来源：http://sxb.jinqigufen.top

[R58] 下载文件
来源：http://gxj.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uge.smart0.xyz

[R59] 发 POST JSON
来源：http://kpj.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://thz.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://wim.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jmh.chenzaomai.com

[R61] 磁盘占用
来源：http://ddb.9152youxi.cn

df -h;  du -sh *
来源：http://ipv.aibaodan.cn

[R62] 找最占空间的文件
来源：http://wgm.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://wcp.sysykeji.top

[R63] 内存与进程
来源：http://wxq.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://idg.quarkkingdee.top

[R64] 结束进程
来源：http://doh.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://gso.sxryk.cn

[R65] 查看端口占用
来源：http://pri.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dde.xuetiantiany.cn

[R66] 定时任务
来源：http://pnj.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://pdv.tian-w.cn

[R67] 生成随机十六进制串
来源：http://zvr.52xcode.cn

openssl rand -hex 16
来源：http://qhd.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://lvy.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://sot.gaohongyu789.top

[R69] 生成随机密码
来源：http://pkr.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://fhg.redwolf501.top

[R70] 时间戳与互转
来源：http://ris.andypj.xyz

date +%s;  date -d @1700000000
来源：http://anv.hnqzz.top

[R71] 日期格式化
来源：http://fmf.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kfx.bbcook.cn

[R72] 等待端口就绪
来源：http://coy.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qbz.aizwys.cn

[R73] 分割大日志
来源：http://zzu.jqgufenzy.top

split -l 1000 big.log part_
来源：http://ttt.hysaishi.cn

[R74] 批量重命名
来源：http://epa.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dsp.epnwcf.com

[R75] 导出环境变量
来源：http://rww.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://dva.yfazqb.com

[R76] 使用临时文件
来源：http://aoo.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rcq.xinyue.icu

[R77] 读取用户输入
来源：http://bko.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://cvk.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://tyb.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ols.fktsv.cn

[R79] 解析命令行选项
来源：http://feq.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzd.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://hog.vehdjk.com

time ./run.sh
来源：http://mtl.xingfuxueyuan.xyz

================================================================================
来源：http://xli.hywenlv.cn

S. C / C++ 专题
来源：http://azn.aibaodan.cn

================================================================================
来源：http://dee.fengsongda.top

[S01] C：Hello World
来源：http://hhg.dashuyun.cn

#include <stdio.h>
来源：http://ncb.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://whm.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://rjo.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://ner.bbcook.cn

[S03] C：读入整数
来源：http://dnl.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://nvg.yj202588.top

[S04] C：字符串复制
来源：http://sgs.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://yvq.jyoumei.cn

[S05] C：字符串长度
来源：http://qwb.ppjwa.cn

strlen(s)
来源：http://blq.fzhhl.top

[S06] C：字符串比较
来源：http://dyz.cashguo.top

strcmp(a, b) == 0
来源：http://dkc.hywenlv.cn

[S07] C：数组遍历求和
来源：http://yoe.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rkp.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://gsh.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkm.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://yio.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vhj.jqgufenzy.top

[S10] C：指针与解引用
来源：http://ytb.yuxming.cn

int *p = &a;  *p = 5;
来源：http://qqq.cheryme.top

[S11] C：逐行读文件
来源：http://yhs.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wmq.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://owa.jyoumei.cn

fclose(f);
来源：http://nof.nanxinkj.top

[S12] C：写文件
来源：http://fxc.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ozr.yvedp.cn

[S13] C：宏定义
来源：http://khq.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hdt.daxiang520.top

[S14] C：枚举
来源：http://scw.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://iwa.shzxlz.cn

[S15] C：类型转换
来源：http://uoi.sjlbkw.cn

(double) a / b
来源：http://lvw.gzhubu.top

[S16] C：位操作置位
来源：http://xjk.sweek.top

x |= (1 << 3);
来源：http://wpy.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://mtc.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aun.gaohongyu789.top

[S18] C：命令行参数
来源：http://puf.zdqjudy.top

int main(int argc, char **argv)
来源：http://jbu.hysaishi.cn

[S19] C：快速排序
来源：http://mgp.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mxb.zhiwuduotai.top

[S20] C：二分查找
来源：http://ohn.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wja.bjfxy.top

[S21] C：字符类别判断
来源：http://wqn.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tzw.haohaochexian.top

[S22] C：字符串转数字
来源：http://gaz.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://arq.xinyue.icu

[S23] C：随机数
来源：http://khc.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oyq.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://iiw.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eov.daxiang520.top

[S25] C：内存拷贝
来源：http://eww.yanxiufei.cn

memcpy(dst, src, n);
来源：http://gwi.iojbl.cn

[S26] C：内存清零
来源：http://fge.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://dhu.jinqigfzy.top

[S27] C：定义常量
来源：http://xsd.hfpthk.cn

const double PI = 3.14159;
来源：http://ycn.daria6918.cn

[S28] C：静态变量
来源：http://glc.xinyue.icu

static int counter = 0;
来源：http://wbb.yanxiufei.cn

[S29] C：变参函数
来源：http://unz.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pwr.fehbvm.com

[S30] C：头文件保护
来源：http://uky.xylfe.cn

#ifndef X_H
来源：http://fcj.0kj1m.cn

#define X_H
来源：http://bsw.tianlin.xyz

#endif
来源：http://xux.hesvh.cn

[S31] C++：Hello World
来源：http://sfn.sysykeji.top

#include <iostream>
来源：http://kmx.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://ehj.feifeiyinyue.top

[S32] C++：字符串
来源：http://zul.yongpay.top

std::string s = "hi";  s += "!";
来源：http://xlk.jqgufenzy.top

[S33] C++：vector 增删
来源：http://gbc.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bbq.smart0.xyz

[S34] C++：遍历 vector
来源：http://uga.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://pjl.kuanghao11.cn

[S35] C++：map
来源：http://czc.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ssr.quarkkingdee.top

[S36] C++：unordered_map
来源：http://lgf.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zkx.yj202588.top

[S37] C++：set
来源：http://rlg.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://toz.shangyingyoupin.top

[S38] C++：排序
来源：http://rtm.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://omp.yj202588.top

[S39] C++：自定义比较器排序
来源：http://yjx.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iuy.shzxlz.cn

[S40] C++：查找元素
来源：http://ows.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tym.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://dba.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://flq.yuxming.cn

[S42] C++：继承与虚函数
来源：http://kqo.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://myq.hfpthk.cn

[S43] C++：智能指针
来源：http://hum.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://chi.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://dfo.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://gfz.yfazqb.com

[S45] C++：lambda
来源：http://psz.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://sma.316326.xyz

[S46] C++：函数模板
来源：http://kus.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cgu.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://kqw.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://beo.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://cxw.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qsw.bjfxy.top

while (std::getline(in, line)) { }
来源：http://wjy.pycfn.com

[S49] C++：写文件
来源：http://yim.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mvk.snrcjt.cn

[S50] C++：格式化数字
来源：http://wyv.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rdp.0kj1m.cn

[S51] C++：显式类型转换
来源：http://ywy.0kj1m.cn

static_cast<double>(a) / b
来源：http://jcm.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://ctd.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://sgk.yvedp.cn

[S53] C++：移动语义
来源：http://pos.cashguo.top

std::vector<int> w = std::move(v);
来源：http://esp.gaohongyu789.top

[S54] C++：异常处理
来源：http://cvk.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nch.havefunace.top

[S55] C++：结构化绑定
来源：http://pdm.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://yxk.yueranfly.top

[S56] C++：optional
来源：http://his.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ahr.jyoumei.cn

[S57] C++：编译期常量
来源：http://dqu.wangshuangyany.cn

constexpr int N = 10;
来源：http://ybs.yuxming.cn

[S58] C++：命名空间
来源：http://zhp.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://osz.pengpengdd.cyou

[S59] C++：静态断言
来源：http://qjp.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xju.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://jzk.birdmap.top


<!-- 参考信息 -->