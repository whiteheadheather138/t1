代发 wailian999

R. Bash 专题
来源：http://nnq.yj202588.top

================================================================================
来源：http://yzq.jqgfzy.top

[R01] shebang 与严格模式
来源：http://zbc.yuanzhike.top

#!/usr/bin/env bash
来源：http://mvr.mhx1999.top

set -euo pipefail
来源：http://ybx.sysykeji.top

[R02] 变量赋值与使用
来源：http://tpk.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://abr.snrcjt.cn

[R03] 只读变量
来源：http://ute.kuanghao11.cn

readonly PI=3.14
来源：http://vsr.xinyue.icu

[R04] 位置参数
来源：http://lgs.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://trj.chenzaomai.com

[R05] 参数默认值
来源：http://ahj.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://xxj.yangfankeji.com

[R06] 判断命令是否存在
来源：http://awz.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xly.0kj1m.cn

[R07] if 判断文件
来源：http://uln.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nnt.shzxlz.cn

[R08] 数值比较
来源：http://cpn.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://itl.yj202588.top

[R09] 字符串比较
来源：http://atu.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lsd.pycfn.com

[R10] 正则匹配
来源：http://vrs.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zrc.yj20258.top

[R11] case 多分支
来源：http://dxd.xuetiantiany.cn

case "$1" in
来源：http://rze.ydzc1.top

start) echo "启动" ;;
来源：http://lkm.mhx1999.top

stop)  echo "停止" ;;
来源：http://rpe.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://ncf.yj202588.top

esac
来源：http://uni.jinqigfzy.top

[R12] for 遍历文件
来源：http://jpb.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://vuy.fktsv.cn

[R13] for 计数循环
来源：http://hfq.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://how.ydzc1.top

[R14] C 风格 for
来源：http://kjh.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gts.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://jko.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://inm.yj202588.top

[R16] until 等待条件
来源：http://fuy.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zcy.birdmap.top

[R17] 数组定义与取值
来源：http://iir.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hzh.uphjek.com

[R18] 遍历数组
来源：http://zqq.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://agk.tarul.cn

[R19] 数组长度
来源：http://hsz.redwolf501.top

echo "${#arr[@]}"
来源：http://rzh.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://dlf.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xpy.chenzaomai.com

[R21] 字符串长度
来源：http://vrc.haohaochexian.top

echo "${#s}"
来源：http://vha.xuanzx.com

[R22] 截取子串
来源：http://mtf.hysaishi.cn

echo "${s:0:5}"
来源：http://zkx.gzhubu.top

[R23] 字符串替换
来源：http://yzo.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://brt.guannengcc.top

[R24] 大小写转换
来源：http://hzj.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://rkr.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://snb.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ukg.epnwcf.com

[R26] 命令替换
来源：http://ves.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://sqx.sweek.top

[R27] 算术展开
来源：http://txs.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://bsp.nanxinkj.top

[R28] 浮点运算
来源：http://dhc.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://qio.gaohongyu789.top

[R29] 定义函数
来源：http://bxs.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imz.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://zaa.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://gkn.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://dht.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://qpz.nwbrower.top

[R32] 参数个数校验
来源：http://sem.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vny.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://xnz.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rrs.fanxiaobao.xyz

[R34] 退出时清理
来源：http://ylb.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://rhf.jinqigfzy.top

[R35] 后台执行并等待
来源：http://pkv.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lxf.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://ywj.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wuy.52xcode.cn

[R37] 把输出赋给变量
来源：http://hvu.shzxlz.cn

files=$(ls -1)
来源：http://rxc.zhoulong.xyz

[R38] 管道串联
来源：http://txt.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://tlx.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://sqn.bbcook.cn

cmd > out.log 2>&1
来源：http://lze.hcnkem.com

[R40] 追加写日志
来源：http://vtz.yanxiufei.cn

echo "log" >> out.log
来源：http://kls.pycfn.com

[R41] 丢弃输出
来源：http://adi.cashguo.top

cmd >/dev/null 2>&1
来源：http://fuw.ydjk.org.cn

[R42] 输入重定向
来源：http://bww.aibaodan.cn

wc -l < a.txt
来源：http://elg.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://qli.zdbjq.cn

find . -name "*.log" -type f
来源：http://jwt.ydjk.org.cn

[R44] 按修改时间查找
来源：http://pgs.sxryk.cn

find . -mtime -7 -type f
来源：http://gbh.gogol.net.cn

[R45] 批量删除
来源：http://yuz.birdmap.top

find . -name "*.tmp" -delete
来源：http://eii.guannengcc.top

[R46] 递归替换文件内容
来源：http://tnx.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cgy.yueranfly.top

[R47] sed 单行替换
来源：http://rmh.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rgg.ehwqpu.com

[R48] awk 取指定列
来源：http://bok.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://wdz.meibo888.top

[R49] awk 带条件
来源：http://ccd.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uqa.shangyingyoupin.top

[R50] awk 求和
来源：http://jmd.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tjf.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://nfp.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fgc.iojbl.cn

[R52] 统计行数
来源：http://nyc.nwbrower.top

wc -l a.txt
来源：http://qan.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://jkn.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iet.zhiwuduotai.top

[R54] 比较两个文件
来源：http://xoe.yuxming.cn

diff a.txt b.txt
来源：http://rum.jyoumei.cn

[R55] 压缩与解压
来源：http://iua.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gjb.tanke756.top

[R56] 远程拷贝
来源：http://zmi.gotoacloud.top

scp file user@host:/path/
来源：http://smj.zhoulong.xyz

[R57] 远程执行命令
来源：http://znq.aibaodan.cn

ssh user@host 'uptime'
来源：http://gih.wangshuangyany.cn

[R58] 下载文件
来源：http://jyf.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://isb.sjlbkw.cn

[R59] 发 POST JSON
来源：http://lgj.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bob.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://vge.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gmx.iojbl.cn

[R61] 磁盘占用
来源：http://ixn.jianghu66.top

df -h;  du -sh *
来源：http://hqq.dashuyun.cn

[R62] 找最占空间的文件
来源：http://dnm.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://ohw.ydzc1.top

[R63] 内存与进程
来源：http://viu.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://rha.sysykeji.top

[R64] 结束进程
来源：http://awl.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://qhq.daxiang520.top

[R65] 查看端口占用
来源：http://ttx.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://udb.yuanzhike.top

[R66] 定时任务
来源：http://qru.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://vcw.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://gah.ybcxt.top

openssl rand -hex 16
来源：http://chx.gogol.net.cn

[R68] 计算文件校验值
来源：http://uwv.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tvt.nanxuanxn.top

[R69] 生成随机密码
来源：http://nnw.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://cuv.shzxlz.cn

[R70] 时间戳与互转
来源：http://zww.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://znt.xylfe.cn

[R71] 日期格式化
来源：http://bpj.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vlo.yuxming.cn

[R72] 等待端口就绪
来源：http://mqt.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dbv.fzhhl.top

[R73] 分割大日志
来源：http://hea.daria6918.cn

split -l 1000 big.log part_
来源：http://kwa.jinghuilouyu.cn

[R74] 批量重命名
来源：http://cwo.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cfy.fzhhl.top

[R75] 导出环境变量
来源：http://tjr.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://nfn.wangshuangyany.cn

[R76] 使用临时文件
来源：http://skl.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zvg.cdnleiting.top

[R77] 读取用户输入
来源：http://fib.sxryk.cn

read -rp "请输入: " ans
来源：http://xam.guowangkeji.top

[R78] 交互式菜单
来源：http://gse.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ffa.yonumen.top

[R79] 解析命令行选项
来源：http://sbh.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kws.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://nxu.daxiang520.top

time ./run.sh
来源：http://lbb.yfazqb.com

================================================================================
来源：http://grp.chenjidiqi.icu

S. C / C++ 专题
来源：http://hwa.pengpengdd.cyou

================================================================================
来源：http://gxc.vehdjk.com

[S01] C：Hello World
来源：http://kom.shzxlz.cn

#include <stdio.h>
来源：http://ycr.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://zur.hcnkem.com

[S02] C：变量与格式化输出
来源：http://kdh.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://ylu.ydzc1.top

[S03] C：读入整数
来源：http://kij.jyoumei.cn

int x; scanf("%d", &x);
来源：http://ldj.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://ceo.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://whi.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://rrh.ydjk.org.cn

strlen(s)
来源：http://tvi.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://fle.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://hlv.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://gll.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sno.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://alc.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exl.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://wfw.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zjq.yj20258888.top

[S10] C：指针与解引用
来源：http://qev.vehdjk.com

int *p = &a;  *p = 5;
来源：http://zvb.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://dhx.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://dmd.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://grs.shanyushiyangtech.top

fclose(f);
来源：http://vmx.sxryk.cn

[S12] C：写文件
来源：http://rpf.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://svc.tian-w.cn

[S13] C：宏定义
来源：http://ehu.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucg.jiagoushi.top

[S14] C：枚举
来源：http://omk.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://tjs.dianchejie.cn

[S15] C：类型转换
来源：http://qqz.ehwqpu.com

(double) a / b
来源：http://mxo.guowangkeji.top

[S16] C：位操作置位
来源：http://rba.aizwys.cn

x |= (1 << 3);
来源：http://xqs.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://pqm.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gyf.jqgfzy.top

[S18] C：命令行参数
来源：http://nol.jlsjyb.cn

int main(int argc, char **argv)
来源：http://gfc.yongpay.top

[S19] C：快速排序
来源：http://xuj.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://bza.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://hsr.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wwe.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://uln.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ihy.uphjek.com

[S22] C：字符串转数字
来源：http://kdo.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://rzn.yuxming.cn

[S23] C：随机数
来源：http://ahv.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eat.vqdsnc.cn

[S24] C：获取本地时间
来源：http://vdy.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bcx.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://eqz.zycfv.cn

memcpy(dst, src, n);
来源：http://xwk.52xcode.cn

[S26] C：内存清零
来源：http://zbs.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://zho.jlsjyb.cn

[S27] C：定义常量
来源：http://vcl.hcnkem.com

const double PI = 3.14159;
来源：http://tis.shangyingyoupin.top

[S28] C：静态变量
来源：http://dhx.fehbvm.com

static int counter = 0;
来源：http://ltg.tian-w.cn

[S29] C：变参函数
来源：http://acc.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://spe.guowangkeji.top

[S30] C：头文件保护
来源：http://ifn.fktsv.cn

#ifndef X_H
来源：http://rzg.52xcode.cn

#define X_H
来源：http://lku.cashguo.top

#endif
来源：http://omm.fzhhl.top

[S31] C++：Hello World
来源：http://wig.birdmap.top

#include <iostream>
来源：http://oky.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://wds.gaohongyu789.top

[S32] C++：字符串
来源：http://pbv.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://hkz.fzhhl.top

[S33] C++：vector 增删
来源：http://zcg.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sug.jqgfzy.top

[S34] C++：遍历 vector
来源：http://rxi.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://huf.yangfankeji.com

[S35] C++：map
来源：http://yvu.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cwj.daxiang520.top

[S36] C++：unordered_map
来源：http://lmv.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lia.xinyue.icu

[S37] C++：set
来源：http://gqp.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ead.hfpthk.cn

[S38] C++：排序
来源：http://nqh.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://jfa.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://luh.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pgj.cashguo.top

[S40] C++：查找元素
来源：http://nwm.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yfq.52xcode.cn

[S41] C++：类与构造函数
来源：http://aqr.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ylz.yuxming.cn

[S42] C++：继承与虚函数
来源：http://aeb.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://rqk.ivvv.top

[S43] C++：智能指针
来源：http://kni.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://rmt.52xcode.cn

[S44] C++：引用传参
来源：http://svb.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://tpk.zhijiandao.cn

[S45] C++：lambda
来源：http://hfx.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://zjb.ydjk.org.cn

[S46] C++：函数模板
来源：http://yry.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vfq.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://ppf.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xyb.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://mdd.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://hgc.cucudq.cn

while (std::getline(in, line)) { }
来源：http://gre.yfazqb.com

[S49] C++：写文件
来源：http://exx.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tze.jiagoushi.top

[S50] C++：格式化数字
来源：http://zsa.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rqp.zdqjudy.top

[S51] C++：显式类型转换
来源：http://dfi.pycfn.com

static_cast<double>(a) / b
来源：http://wxl.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://wor.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://ilk.yvedp.cn

[S53] C++：移动语义
来源：http://ujb.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://gix.yj202588.top

[S54] C++：异常处理
来源：http://kuz.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mut.bjfxy.top

[S55] C++：结构化绑定
来源：http://ucz.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hwh.vqdsnc.cn

[S56] C++：optional
来源：http://pze.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ovq.xylfe.cn

[S57] C++：编译期常量
来源：http://fvu.hysaishi.cn

constexpr int N = 10;
来源：http://oyh.cucudq.cn

[S58] C++：命名空间
来源：http://qtn.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://cgb.yvedp.cn

[S59] C++：静态断言
来源：http://nmg.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uqq.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://ntj.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gzg.tian-w.cn

================================================================================
来源：http://tbi.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://inr.svipenyu.cn

================================================================================
来源：http://kis.shuidangran.top


<!-- 参考信息 -->