代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ziz.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pip.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://abh.hywenlv.cn

[Q89] 判断表是否存在
来源：http://bqk.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://van.svipenyu.cn

[Q90] 生成序号列
来源：http://mju.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cdw.cashguo.top

================================================================================
来源：http://lku.hongshengwenyu.top

R. Bash 专题
来源：http://vcb.316326.xyz

================================================================================
来源：http://veo.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://xoo.fengsongda.top

#!/usr/bin/env bash
来源：http://yxj.meibo888.top

set -euo pipefail
来源：http://qdw.tarul.cn

[R02] 变量赋值与使用
来源：http://bij.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://tkx.fktsv.cn

[R03] 只读变量
来源：http://ixq.iojbl.cn

readonly PI=3.14
来源：http://cza.vehdjk.com

[R04] 位置参数
来源：http://bvl.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cjn.yfazqb.com

[R05] 参数默认值
来源：http://npy.hongshengwenyu.top

name="${1:-default}"
来源：http://cnj.smart0.xyz

[R06] 判断命令是否存在
来源：http://pew.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yrw.quarkkingdee.top

[R07] if 判断文件
来源：http://zfy.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wuv.gaohongyu789.top

[R08] 数值比较
来源：http://faq.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://thp.aizwys.cn

[R09] 字符串比较
来源：http://yvy.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lmw.xylfe.cn

[R10] 正则匹配
来源：http://etk.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nso.vehdjk.com

[R11] case 多分支
来源：http://cxh.havefunace.top

case "$1" in
来源：http://dqn.c1oappe.top

start) echo "启动" ;;
来源：http://tbw.316326.xyz

stop)  echo "停止" ;;
来源：http://wdg.wangdashe.top

*)     echo "未知命令" ;;
来源：http://bta.zhaomingkeji.xyz

esac
来源：http://nfn.guannengcc.top

[R12] for 遍历文件
来源：http://sqo.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://yrg.yfazqb.com

[R13] for 计数循环
来源：http://xco.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://mbo.dashuyun.cn

[R14] C 风格 for
来源：http://dxc.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ynu.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://uje.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ptl.xziqi.cn

[R16] until 等待条件
来源：http://pga.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qef.yuanzhike.top

[R17] 数组定义与取值
来源：http://bdk.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://bns.daxiang520.top

[R18] 遍历数组
来源：http://ybs.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://udi.hcnkem.com

[R19] 数组长度
来源：http://owo.xylfe.cn

echo "${#arr[@]}"
来源：http://gdq.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://pwb.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gug.9152youxi.cn

[R21] 字符串长度
来源：http://fwa.yonumen.top

echo "${#s}"
来源：http://pgy.aizwys.cn

[R22] 截取子串
来源：http://qbo.gzhubu.top

echo "${s:0:5}"
来源：http://jys.epnwcf.com

[R23] 字符串替换
来源：http://akl.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dnb.gzhubu.top

[R24] 大小写转换
来源：http://ytb.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ckw.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://xdi.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nbd.wangdashe.top

[R26] 命令替换
来源：http://nny.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://vbk.guowangkeji.top

[R27] 算术展开
来源：http://giw.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://vrx.gzhubu.top

[R28] 浮点运算
来源：http://mim.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://umw.gzhubu.top

[R29] 定义函数
来源：http://kat.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://idh.sweek.top

[R30] 函数返回状态码
来源：http://vmf.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://vpz.shuidangran.top

[R31] 局部变量
来源：http://wny.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://ant.yueranfly.top

[R32] 参数个数校验
来源：http://keu.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kfr.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://bzv.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mra.hywenlv.cn

[R34] 退出时清理
来源：http://ptd.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tlb.ctjpmb.com

[R35] 后台执行并等待
来源：http://dpi.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dou.zdqjudy.top

[R36] 并发执行多个任务
来源：http://uct.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sef.zycfv.cn

[R37] 把输出赋给变量
来源：http://jet.9152youxi.cn

files=$(ls -1)
来源：http://ptj.cashguo.top

[R38] 管道串联
来源：http://lrp.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://qbg.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://hjm.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://wrw.316326.xyz

[R40] 追加写日志
来源：http://zcd.snrcjt.cn

echo "log" >> out.log
来源：http://odm.zhixingplan.top

[R41] 丢弃输出
来源：http://qzg.havefunace.top

cmd >/dev/null 2>&1
来源：http://sxh.dianchejie.cn

[R42] 输入重定向
来源：http://kof.nanxinkj.top

wc -l < a.txt
来源：http://gln.birdmap.top

[R43] 按名字查找文件
来源：http://szs.yongpay.top

find . -name "*.log" -type f
来源：http://blu.redwolf501.top

[R44] 按修改时间查找
来源：http://iun.xinyue.icu

find . -mtime -7 -type f
来源：http://yjm.daria6918.cn

[R45] 批量删除
来源：http://rti.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://zfx.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://ivf.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fki.gotoacloud.top

[R47] sed 单行替换
来源：http://rwq.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://qax.tian-w.cn

[R48] awk 取指定列
来源：http://hfp.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://mwy.shuidangran.top

[R49] awk 带条件
来源：http://mno.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cbu.fktsv.cn

[R50] awk 求和
来源：http://jwb.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://cds.guannengcc.top

[R51] 排序去重取前几
来源：http://kxf.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hnl.wangshuangyany.cn

[R52] 统计行数
来源：http://fgb.tarul.cn

wc -l a.txt
来源：http://dnd.ivvv.top

[R53] 查看文件头与实时尾
来源：http://avl.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://loo.ybcxt.top

[R54] 比较两个文件
来源：http://fnc.vqdsnc.cn

diff a.txt b.txt
来源：http://tyc.aizwys.cn

[R55] 压缩与解压
来源：http://bix.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://svz.ehwqpu.com

[R56] 远程拷贝
来源：http://jrv.cashguo.top

scp file user@host:/path/
来源：http://lqz.fktsv.cn

[R57] 远程执行命令
来源：http://djc.bbcook.cn

ssh user@host 'uptime'
来源：http://nrt.jqgfzy.top

[R58] 下载文件
来源：http://umr.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hts.hammf.cn

[R59] 发 POST JSON
来源：http://bsq.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lqd.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://uon.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://enj.hongshengwenyu.top

[R61] 磁盘占用
来源：http://hiy.zhixingplan.top

df -h;  du -sh *
来源：http://epd.dianchejie.cn

[R62] 找最占空间的文件
来源：http://jrr.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://dxs.52xcode.cn

[R63] 内存与进程
来源：http://qzi.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://gkl.yuanzhike.top

[R64] 结束进程
来源：http://mdl.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://lih.sysykeji.top

[R65] 查看端口占用
来源：http://cgr.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bto.gaohongyu789.top

[R66] 定时任务
来源：http://crg.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://gtu.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://fhg.uphjek.com

openssl rand -hex 16
来源：http://lqd.cdnleiting.top

[R68] 计算文件校验值
来源：http://zps.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://mbx.zhixingplan.top

[R69] 生成随机密码
来源：http://xxl.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://wfy.0kj1m.cn

[R70] 时间戳与互转
来源：http://epa.tarul.cn

date +%s;  date -d @1700000000
来源：http://syx.quarkkingdee.top

[R71] 日期格式化
来源：http://cac.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zyw.gotoacloud.top

[R72] 等待端口就绪
来源：http://xxc.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://isj.0kj1m.cn

[R73] 分割大日志
来源：http://lao.9152youxi.cn

split -l 1000 big.log part_
来源：http://exf.svipenyu.cn

[R74] 批量重命名
来源：http://tph.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gtp.pengpengdd.cyou

[R75] 导出环境变量
来源：http://yft.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://jqg.redwolf501.top

[R76] 使用临时文件
来源：http://ojp.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dov.yuxming.cn

[R77] 读取用户输入
来源：http://tcv.yanxiufei.cn

read -rp "请输入: " ans
来源：http://xnz.snrcjt.cn

[R78] 交互式菜单
来源：http://sbz.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zpo.pycfn.com

[R79] 解析命令行选项
来源：http://soi.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kkb.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://nwi.yangfankeji.com

time ./run.sh
来源：http://onh.ywan-chungtsiang.top

================================================================================
来源：http://xrl.quarkkingdee.top

S. C / C++ 专题
来源：http://nml.chenlongwang.top

================================================================================
来源：http://cnr.hfpthk.cn

[S01] C：Hello World
来源：http://nco.yj20258888.top

#include <stdio.h>
来源：http://krm.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uvy.xziqi.cn

[S02] C：变量与格式化输出
来源：http://cby.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://kye.dashuyun.cn

[S03] C：读入整数
来源：http://imi.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://cma.sxryk.cn

[S04] C：字符串复制
来源：http://gzf.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ojb.hnqzz.top

[S05] C：字符串长度
来源：http://mey.hfpthk.cn

strlen(s)
来源：http://dop.sufxvd.cn

[S06] C：字符串比较
来源：http://txk.zhixingplan.top

strcmp(a, b) == 0
来源：http://jtr.jianghu66.top

[S07] C：数组遍历求和
来源：http://obv.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rjd.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://fms.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yxu.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://qrq.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oue.xylfe.cn

[S10] C：指针与解引用
来源：http://tgv.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://yxn.cheryme.top

[S11] C：逐行读文件
来源：http://ypq.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://wiy.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dot.sweek.top

fclose(f);
来源：http://ltk.gzhubu.top

[S12] C：写文件
来源：http://wxq.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sbo.hfpthk.cn

[S13] C：宏定义
来源：http://zes.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rkz.zdqjudy.top

[S14] C：枚举
来源：http://szu.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://ekn.yangfankeji.com

[S15] C：类型转换
来源：http://xin.epnwcf.com

(double) a / b
来源：http://ayo.tianlin.xyz

[S16] C：位操作置位
来源：http://tfj.52xcode.cn

x |= (1 << 3);
来源：http://uwj.shuidangran.top

[S17] C：安全拼接字符串
来源：http://vds.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zsd.zdbjq.cn

[S18] C：命令行参数
来源：http://jhr.zhijiandao.cn

int main(int argc, char **argv)
来源：http://rxx.52xcode.cn

[S19] C：快速排序
来源：http://dwm.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rgt.fzhhl.top

[S20] C：二分查找
来源：http://hwh.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kpl.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://vbv.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qmb.hywenlv.cn

[S22] C：字符串转数字
来源：http://cao.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://zfm.cucudq.cn

[S23] C：随机数
来源：http://krn.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pgb.quarkkingdee.top

[S24] C：获取本地时间
来源：http://xds.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ylt.epnwcf.com

[S25] C：内存拷贝
来源：http://pjz.havefunace.top

memcpy(dst, src, n);
来源：http://gam.9152youxi.cn

[S26] C：内存清零
来源：http://hin.52xcode.cn

memset(a, 0, sizeof a);
来源：http://ldi.ctjpmb.com

[S27] C：定义常量
来源：http://fgd.chenlongwang.top

const double PI = 3.14159;
来源：http://ogh.cucudq.cn

[S28] C：静态变量
来源：http://yzj.xylfe.cn

static int counter = 0;
来源：http://yxh.yangfankeji.com

[S29] C：变参函数
来源：http://bts.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zzk.ehwqpu.com

[S30] C：头文件保护
来源：http://lss.wangdashe.top

#ifndef X_H
来源：http://zvh.c1oappe.top

#define X_H
来源：http://ntc.fanxiaobao.xyz

#endif
来源：http://nwg.zhengqikj.top

[S31] C++：Hello World
来源：http://ymj.vqdsnc.cn

#include <iostream>
来源：http://zhr.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://jmj.cashguo.top

[S32] C++：字符串
来源：http://nuz.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://dkd.cdnleiting.top

[S33] C++：vector 增删
来源：http://ojz.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pjo.jyoumei.cn

[S34] C++：遍历 vector
来源：http://ixq.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://mkl.wangshuangyany.cn

[S35] C++：map
来源：http://otr.hesvh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://axg.hammf.cn

[S36] C++：unordered_map
来源：http://dun.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://epi.zhijiandao.cn

[S37] C++：set
来源：http://jsy.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uhu.ydjk.org.cn

[S38] C++：排序
来源：http://fod.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://oxt.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://ptx.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fyr.pycfn.com

[S40] C++：查找元素
来源：http://xrh.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://shq.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://rvx.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zlc.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://njj.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://mzc.yuxming.cn

[S43] C++：智能指针
来源：http://dwc.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://dmu.cqqwz.cn

[S44] C++：引用传参
来源：http://puk.yongpay.top

void inc(int &x) { ++x; }
来源：http://pvi.daria6918.cn

[S45] C++：lambda
来源：http://pwh.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://squ.svipenyu.cn

[S46] C++：函数模板
来源：http://vnb.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xla.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://ibz.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zvy.cdnleiting.top

[S48] C++：逐行读文件
来源：http://bjh.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://syc.guannengcc.top

while (std::getline(in, line)) { }
来源：http://jnr.chenzaomai.com

[S49] C++：写文件
来源：http://ior.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fri.guannengcc.top

[S50] C++：格式化数字
来源：http://fde.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vkz.shuidangran.top

[S51] C++：显式类型转换
来源：http://cfy.ybcxt.top

static_cast<double>(a) / b
来源：http://zri.yj20258.top

[S52] C++：const 与 noexcept
来源：http://dnr.yonumen.top

int size() const noexcept { return n_; }
来源：http://mgl.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://oiq.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://zhc.yongpay.top

[S54] C++：异常处理
来源：http://lth.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jnp.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://yqv.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xfu.shuidangran.top

[S56] C++：optional
来源：http://hlb.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qsm.ivvv.top

[S57] C++：编译期常量
来源：http://tge.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://rvb.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://epu.shanyushiyangkeji.top


<!-- 参考信息 -->