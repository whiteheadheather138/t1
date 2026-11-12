代发 wailian999

R. Bash 专题
来源：http://kzi.yj202588.top

================================================================================
来源：http://jsi.svipenyu.cn

[R01] shebang 与严格模式
来源：http://cdr.hcnkem.com

#!/usr/bin/env bash
来源：http://dzf.fzhhl.top

set -euo pipefail
来源：http://awv.cqqwz.cn

[R02] 变量赋值与使用
来源：http://mbf.hcnkem.com

name="Tom"; echo "$name"
来源：http://vcd.zhijiandao.cn

[R03] 只读变量
来源：http://jql.chenlongwang.top

readonly PI=3.14
来源：http://gul.aibaodan.cn

[R04] 位置参数
来源：http://ubq.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vqw.yvedp.cn

[R05] 参数默认值
来源：http://rrj.cqqwz.cn

name="${1:-default}"
来源：http://aux.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://gev.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gwh.gotoacloud.top

[R07] if 判断文件
来源：http://tco.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zpc.xylfe.cn

[R08] 数值比较
来源：http://vmc.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://kjs.hongshengwenyu.top

[R09] 字符串比较
来源：http://gno.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vto.vqdsnc.cn

[R10] 正则匹配
来源：http://sal.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://prm.hesvh.cn

[R11] case 多分支
来源：http://wxs.nwbrower.top

case "$1" in
来源：http://ktu.nanxuanxn.top

start) echo "启动" ;;
来源：http://dnf.epnwcf.com

stop)  echo "停止" ;;
来源：http://cbm.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://ayj.chenzaomai.com

esac
来源：http://usv.cqqwz.cn

[R12] for 遍历文件
来源：http://qng.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://fuz.jinghuilouyu.cn

[R13] for 计数循环
来源：http://bib.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://ifd.0kj1m.cn

[R14] C 风格 for
来源：http://nyj.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qke.xinyue.icu

[R15] while 逐行读文件
来源：http://eom.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xay.yj20258.top

[R16] until 等待条件
来源：http://lbb.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://akz.c1oappe.top

[R17] 数组定义与取值
来源：http://xom.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://vnl.zhixingplan.top

[R18] 遍历数组
来源：http://yog.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jqe.wangdashe.top

[R19] 数组长度
来源：http://xeu.sxryk.cn

echo "${#arr[@]}"
来源：http://ldm.sysykeji.top

[R20] 关联数组（字典）
来源：http://kva.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjo.meibo888.top

[R21] 字符串长度
来源：http://mvd.shanyushiyangkeji.top

echo "${#s}"
来源：http://wrs.ydzc1.top

[R22] 截取子串
来源：http://kju.gogol.net.cn

echo "${s:0:5}"
来源：http://gie.nanxuanxn.top

[R23] 字符串替换
来源：http://vam.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rju.hcnkem.com

[R24] 大小写转换
来源：http://xti.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://vgp.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://tts.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kyy.yangfankeji.com

[R26] 命令替换
来源：http://msq.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://pkn.guowangkeji.top

[R27] 算术展开
来源：http://mtl.yonumen.top

echo $((1 + 2 * 3))
来源：http://qqr.yj20258888.top

[R28] 浮点运算
来源：http://mrw.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://wxh.havefunace.top

[R29] 定义函数
来源：http://eth.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sqx.bbcook.cn

[R30] 函数返回状态码
来源：http://haj.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://gsf.sweek.top

[R31] 局部变量
来源：http://uws.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://goe.ydzc1.top

[R32] 参数个数校验
来源：http://biq.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hap.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://fmj.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yrf.yj202588.top

[R34] 退出时清理
来源：http://nqf.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://bbw.ehwqpu.com

[R35] 后台执行并等待
来源：http://dyu.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rlo.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://eom.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hyp.hywenlv.cn

[R37] 把输出赋给变量
来源：http://rmq.redwolf501.top

files=$(ls -1)
来源：http://ynu.cheryme.top

[R38] 管道串联
来源：http://zox.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://vtb.tarul.cn

[R39] 重定向标准输出与错误
来源：http://muh.ppjwa.cn

cmd > out.log 2>&1
来源：http://qrs.chenjidiqi.icu

[R40] 追加写日志
来源：http://kom.fengsongda.top

echo "log" >> out.log
来源：http://uik.chenlongwang.top

[R41] 丢弃输出
来源：http://lvx.havefunace.top

cmd >/dev/null 2>&1
来源：http://zwj.jqgfzy.top

[R42] 输入重定向
来源：http://gjb.hywenlv.cn

wc -l < a.txt
来源：http://kaz.iojbl.cn

[R43] 按名字查找文件
来源：http://dtp.yangfankeji.com

find . -name "*.log" -type f
来源：http://rgf.nwbrower.top

[R44] 按修改时间查找
来源：http://qxl.0kj1m.cn

find . -mtime -7 -type f
来源：http://acx.nanxinkj.top

[R45] 批量删除
来源：http://ytx.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://jyv.gzhubu.top

[R46] 递归替换文件内容
来源：http://mfs.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://evw.vqdsnc.cn

[R47] sed 单行替换
来源：http://rpl.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://wte.yuxming.cn

[R48] awk 取指定列
来源：http://gwa.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://hub.jiagoushi.top

[R49] awk 带条件
来源：http://cvi.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://puw.c1oappe.top

[R50] awk 求和
来源：http://xna.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://lrg.ehwqpu.com

[R51] 排序去重取前几
来源：http://zxy.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ikj.9152youxi.cn

[R52] 统计行数
来源：http://yse.epnwcf.com

wc -l a.txt
来源：http://wyt.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://kxr.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yfa.guannengcc.top

[R54] 比较两个文件
来源：http://vjv.sxryk.cn

diff a.txt b.txt
来源：http://vos.jyoumei.cn

[R55] 压缩与解压
来源：http://fvz.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qxr.fktsv.cn

[R56] 远程拷贝
来源：http://qiv.yj20258888.top

scp file user@host:/path/
来源：http://tmm.yanxiufei.cn

[R57] 远程执行命令
来源：http://xps.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://oes.iojbl.cn

[R58] 下载文件
来源：http://xgz.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aqc.hfpthk.cn

[R59] 发 POST JSON
来源：http://vbq.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://djb.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://hpe.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fdv.yanxiufei.cn

[R61] 磁盘占用
来源：http://aqc.epnwcf.com

df -h;  du -sh *
来源：http://sgg.xylfe.cn

[R62] 找最占空间的文件
来源：http://qbz.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://bav.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://tes.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://rve.shuidangran.top

[R64] 结束进程
来源：http://anj.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://xul.uphjek.com

[R65] 查看端口占用
来源：http://sqq.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://koe.guannengcc.top

[R66] 定时任务
来源：http://mpe.tian-w.cn

crontab -e;  crontab -l
来源：http://hhg.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://qbo.cdnleiting.top

openssl rand -hex 16
来源：http://tsy.quarkkingdee.top

[R68] 计算文件校验值
来源：http://xob.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://uyf.zhijiandao.cn

[R69] 生成随机密码
来源：http://smy.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://utb.vehdjk.com

[R70] 时间戳与互转
来源：http://ecv.zycfv.cn

date +%s;  date -d @1700000000
来源：http://ucg.ydjk.org.cn

[R71] 日期格式化
来源：http://onn.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hem.hysaishi.cn

[R72] 等待端口就绪
来源：http://zch.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xzm.yj202588.top

[R73] 分割大日志
来源：http://ira.yongpay.top

split -l 1000 big.log part_
来源：http://ojq.havefunace.top

[R74] 批量重命名
来源：http://puk.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kwu.ydzc1.top

[R75] 导出环境变量
来源：http://xar.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://mvi.bbcook.cn

[R76] 使用临时文件
来源：http://rbt.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bil.sysykeji.top

[R77] 读取用户输入
来源：http://ucd.gaohongyu789.top

read -rp "请输入: " ans
来源：http://arg.ivvv.top

[R78] 交互式菜单
来源：http://gqp.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kbv.yongpay.top

[R79] 解析命令行选项
来源：http://cmq.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://drj.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://prj.ydjk.org.cn

time ./run.sh
来源：http://skn.yuanzhike.top

================================================================================
来源：http://fop.yonumen.top

S. C / C++ 专题
来源：http://iud.jinqigufen.top

================================================================================
来源：http://wqy.zhijiandao.cn

[S01] C：Hello World
来源：http://uyt.hnxiangtu.top

#include <stdio.h>
来源：http://wyr.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iqt.bbcook.cn

[S02] C：变量与格式化输出
来源：http://fyw.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://kzv.yanxiufei.cn

[S03] C：读入整数
来源：http://wyr.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://xlb.jqgfzy.top

[S04] C：字符串复制
来源：http://hmy.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://tfk.hnqzz.top

[S05] C：字符串长度
来源：http://cwj.nwbrower.top

strlen(s)
来源：http://cey.hesvh.cn

[S06] C：字符串比较
来源：http://afl.zhixingplan.top

strcmp(a, b) == 0
来源：http://dwb.daxiang520.top

[S07] C：数组遍历求和
来源：http://eqk.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vko.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://jht.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lde.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://ahl.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eqm.cucudq.cn

[S10] C：指针与解引用
来源：http://okr.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://ele.jinqigufen.top

[S11] C：逐行读文件
来源：http://yiw.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://tfz.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ziw.xylfe.cn

fclose(f);
来源：http://hfj.yuxming.cn

[S12] C：写文件
来源：http://pqe.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gvj.jlsjyb.cn

[S13] C：宏定义
来源：http://rjw.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nfo.fzhhl.top

[S14] C：枚举
来源：http://pkp.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://etg.316326.xyz

[S15] C：类型转换
来源：http://wqm.jlsjyb.cn

(double) a / b
来源：http://nze.gaohongyu789.top

[S16] C：位操作置位
来源：http://qdu.jianghu66.top

x |= (1 << 3);
来源：http://bxi.ivvv.top

[S17] C：安全拼接字符串
来源：http://blv.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://abi.yanxiufei.cn

[S18] C：命令行参数
来源：http://olj.hfpthk.cn

int main(int argc, char **argv)
来源：http://tpi.shuidangran.top

[S19] C：快速排序
来源：http://jdy.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://hjr.ydjk.org.cn

[S20] C：二分查找
来源：http://rwn.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rwh.gaohongyu789.top

[S21] C：字符类别判断
来源：http://bsi.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbz.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://npu.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://iww.xinyue.icu

[S23] C：随机数
来源：http://hub.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xas.nanxuanxn.top

[S24] C：获取本地时间
来源：http://qju.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pro.nanxinkj.top

[S25] C：内存拷贝
来源：http://nga.kuanghao11.cn

memcpy(dst, src, n);
来源：http://aix.aibaodan.cn

[S26] C：内存清零
来源：http://pgn.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://yah.chenjidiqi.icu

[S27] C：定义常量
来源：http://tsh.daxiang520.top

const double PI = 3.14159;
来源：http://ucu.guowangkeji.top

[S28] C：静态变量
来源：http://daq.fzhhl.top

static int counter = 0;
来源：http://khk.uphjek.com

[S29] C：变参函数
来源：http://lcj.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aum.yangfankeji.com

[S30] C：头文件保护
来源：http://vnf.ehwqpu.com

#ifndef X_H
来源：http://rva.pycfn.com

#define X_H
来源：http://lrd.316326.xyz

#endif
来源：http://gko.hywenlv.cn

[S31] C++：Hello World
来源：http://zip.yvedp.cn

#include <iostream>
来源：http://xwn.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://qom.ehwqpu.com

[S32] C++：字符串
来源：http://bgl.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://wyn.vehdjk.com

[S33] C++：vector 增删
来源：http://msi.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yto.svipenyu.cn

[S34] C++：遍历 vector
来源：http://rmq.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://iyt.jqgfzy.top

[S35] C++：map
来源：http://ghd.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pji.52xcode.cn

[S36] C++：unordered_map
来源：http://eoh.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ybp.xinyue.icu

[S37] C++：set
来源：http://wic.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://smg.aizwys.cn

[S38] C++：排序
来源：http://erb.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://ziq.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://uqr.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ykw.iojbl.cn

[S40] C++：查找元素
来源：http://gne.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vyo.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://qdy.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vvt.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://njl.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://jnl.hysaishi.cn

[S43] C++：智能指针
来源：http://pul.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://gtd.ydzc1.top

[S44] C++：引用传参
来源：http://kcc.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://usk.tanke756.top

[S45] C++：lambda
来源：http://hhd.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://liz.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://fzw.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mkh.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://mah.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvj.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://mvp.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zei.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://wth.wangshuangyany.cn

[S49] C++：写文件
来源：http://wna.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zst.ppjwa.cn

[S50] C++：格式化数字
来源：http://uni.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nkb.hysaishi.cn

[S51] C++：显式类型转换
来源：http://erc.jinqigfzy.top

static_cast<double>(a) / b
来源：http://hpo.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://hxi.wangdashe.top

int size() const noexcept { return n_; }
来源：http://pdx.ydzc1.top

[S53] C++：移动语义
来源：http://ydm.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://vzk.guowangkeji.top

[S54] C++：异常处理
来源：http://jqw.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fqi.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://qoh.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lcj.sufxvd.cn

[S56] C++：optional
来源：http://ybd.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szw.sysykeji.top

[S57] C++：编译期常量
来源：http://mll.zhiwuduotai.top

constexpr int N = 10;
来源：http://lmi.jinqigfzy.top

[S58] C++：命名空间
来源：http://gwd.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://ojg.yonumen.top

[S59] C++：静态断言
来源：http://mwn.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ceh.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://loz.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bvm.0kj1m.cn

================================================================================
来源：http://hky.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://msl.sweek.top

================================================================================
来源：http://sww.ydjk.org.cn


<!-- 参考信息 -->