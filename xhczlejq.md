代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kop.nanxinkj.top

[Q90] 生成序号列
来源：http://wbr.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dnl.zhixingplan.top

================================================================================
来源：http://vso.jqgufenzy.top

R. Bash 专题
来源：http://udx.tanke756.top

================================================================================
来源：http://uje.bjfxy.top

[R01] shebang 与严格模式
来源：http://vax.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://dnz.wangshuangyany.cn

set -euo pipefail
来源：http://sgr.svipenyu.cn

[R02] 变量赋值与使用
来源：http://iwx.yangfankeji.com

name="Tom"; echo "$name"
来源：http://nrm.kuanghao11.cn

[R03] 只读变量
来源：http://gxk.chenlongwang.top

readonly PI=3.14
来源：http://mzy.shzxlz.cn

[R04] 位置参数
来源：http://knb.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://alx.cashguo.top

[R05] 参数默认值
来源：http://hdi.dianchejie.cn

name="${1:-default}"
来源：http://vqy.xylfe.cn

[R06] 判断命令是否存在
来源：http://iwn.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khx.yueranfly.top

[R07] if 判断文件
来源：http://mfe.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jmt.hcnkem.com

[R08] 数值比较
来源：http://igr.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zce.daria6918.cn

[R09] 字符串比较
来源：http://ets.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://smq.zdqjudy.top

[R10] 正则匹配
来源：http://ipt.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uqd.gaohongyu789.top

[R11] case 多分支
来源：http://zkn.0kj1m.cn

case "$1" in
来源：http://xgg.iojbl.cn

start) echo "启动" ;;
来源：http://ece.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://epr.mhx1999.top

*)     echo "未知命令" ;;
来源：http://zkm.fengsongda.top

esac
来源：http://ash.316326.xyz

[R12] for 遍历文件
来源：http://quh.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://tvk.birdmap.top

[R13] for 计数循环
来源：http://czz.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://dtj.yj20258.top

[R14] C 风格 for
来源：http://evz.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bze.sweek.top

[R15] while 逐行读文件
来源：http://zqw.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gma.hongshengwenyu.top

[R16] until 等待条件
来源：http://zqm.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xkn.sweek.top

[R17] 数组定义与取值
来源：http://whb.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://ffe.ehwqpu.com

[R18] 遍历数组
来源：http://jld.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://toq.haohaochexian.top

[R19] 数组长度
来源：http://oiy.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://tia.yangfankeji.com

[R20] 关联数组（字典）
来源：http://jnv.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rzh.wangshuangyany.cn

[R21] 字符串长度
来源：http://kuf.xinyue.icu

echo "${#s}"
来源：http://hyj.zhaomingkeji.xyz

[R22] 截取子串
来源：http://pmx.zhongyouzk.top

echo "${s:0:5}"
来源：http://ams.ctjpmb.com

[R23] 字符串替换
来源：http://rcq.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dxi.chenlongwang.top

[R24] 大小写转换
来源：http://vik.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uxo.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://inn.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://pxi.andypj.xyz

[R26] 命令替换
来源：http://did.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://qcl.hongshengwenyu.top

[R27] 算术展开
来源：http://qjg.ydzc1.top

echo $((1 + 2 * 3))
来源：http://buc.daria6918.cn

[R28] 浮点运算
来源：http://utj.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://ugk.zhoulong.xyz

[R29] 定义函数
来源：http://bmv.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nyv.epnwcf.com

[R30] 函数返回状态码
来源：http://pwq.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://noq.yj20258888.top

[R31] 局部变量
来源：http://xoh.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://ims.jqgufenzy.top

[R32] 参数个数校验
来源：http://nua.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mui.yonumen.top

[R33] 捕获错误并提示行号
来源：http://wcn.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xid.smart0.xyz

[R34] 退出时清理
来源：http://cpi.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bzi.zhengqikj.top

[R35] 后台执行并等待
来源：http://wes.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://chf.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://vpw.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vdh.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://uev.jinyuanbaomall.cn

files=$(ls -1)
来源：http://mld.hongshengwenyu.top

[R38] 管道串联
来源：http://jzc.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://kdo.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://kvj.hesvh.cn

cmd > out.log 2>&1
来源：http://vst.fzhhl.top

[R40] 追加写日志
来源：http://prq.zhiwuduotai.top

echo "log" >> out.log
来源：http://dwm.meibo888.top

[R41] 丢弃输出
来源：http://wai.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://gyi.fengsongda.top

[R42] 输入重定向
来源：http://uvb.xziqi.cn

wc -l < a.txt
来源：http://hfr.pycfn.com

[R43] 按名字查找文件
来源：http://pgq.zycfv.cn

find . -name "*.log" -type f
来源：http://jnj.mhx1999.top

[R44] 按修改时间查找
来源：http://pbl.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://jia.nanxuanxn.top

[R45] 批量删除
来源：http://vmc.wangdashe.top

find . -name "*.tmp" -delete
来源：http://sga.jqgfzy.top

[R46] 递归替换文件内容
来源：http://rrd.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sny.zycfv.cn

[R47] sed 单行替换
来源：http://tmi.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://iza.nanxuanxn.top

[R48] awk 取指定列
来源：http://ptb.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://bvg.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://iln.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tfy.meibo888.top

[R50] awk 求和
来源：http://yja.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://lfb.chenlongwang.top

[R51] 排序去重取前几
来源：http://ohu.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jeg.xylfe.cn

[R52] 统计行数
来源：http://jkq.aizwys.cn

wc -l a.txt
来源：http://gwf.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://gwv.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ehn.smart0.xyz

[R54] 比较两个文件
来源：http://nyq.mhx1999.top

diff a.txt b.txt
来源：http://bli.ydjk.org.cn

[R55] 压缩与解压
来源：http://tff.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pct.yj20258.top

[R56] 远程拷贝
来源：http://jal.aibaodan.cn

scp file user@host:/path/
来源：http://zoi.9152youxi.cn

[R57] 远程执行命令
来源：http://xcg.hcnkem.com

ssh user@host 'uptime'
来源：http://xpj.shangyingyoupin.top

[R58] 下载文件
来源：http://apy.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ahs.zdqjudy.top

[R59] 发 POST JSON
来源：http://nqb.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mum.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://lir.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tjt.guowangkeji.top

[R61] 磁盘占用
来源：http://mvv.cucudq.cn

df -h;  du -sh *
来源：http://wyl.redwolf501.top

[R62] 找最占空间的文件
来源：http://bmb.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://hmz.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://yce.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://vyy.ywan-chungtsiang.top

[R64] 结束进程
来源：http://iza.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://fxs.nanxuanxn.top

[R65] 查看端口占用
来源：http://ilg.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bbc.nanxinkj.top

[R66] 定时任务
来源：http://odm.hfpthk.cn

crontab -e;  crontab -l
来源：http://zis.ybcxt.top

[R67] 生成随机十六进制串
来源：http://arq.gaohongyu789.top

openssl rand -hex 16
来源：http://wpj.gaohongyu789.top

[R68] 计算文件校验值
来源：http://geq.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zgs.jianghu66.top

[R69] 生成随机密码
来源：http://lhx.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://jiq.fehbvm.com

[R70] 时间戳与互转
来源：http://szl.fktsv.cn

date +%s;  date -d @1700000000
来源：http://znt.c1oappe.top

[R71] 日期格式化
来源：http://cfr.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pub.wangdashe.top

[R72] 等待端口就绪
来源：http://xfu.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tsw.jqgfzy.top

[R73] 分割大日志
来源：http://kli.jiagoushi.top

split -l 1000 big.log part_
来源：http://qmd.fengsongda.top

[R74] 批量重命名
来源：http://bsh.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mdw.gotoacloud.top

[R75] 导出环境变量
来源：http://kjq.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://gmb.ctjpmb.com

[R76] 使用临时文件
来源：http://xat.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mdo.yanxiufei.cn

[R77] 读取用户输入
来源：http://ciy.yuxming.cn

read -rp "请输入: " ans
来源：http://bsg.vehdjk.com

[R78] 交互式菜单
来源：http://jtv.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kgw.9152youxi.cn

[R79] 解析命令行选项
来源：http://izp.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wqt.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://vgw.ywan-chungtsiang.top

time ./run.sh
来源：http://pjg.jinqigfzy.top

================================================================================
来源：http://oux.jyoumei.cn

S. C / C++ 专题
来源：http://jsm.yj202588.top

================================================================================
来源：http://kgl.jiagoushi.top

[S01] C：Hello World
来源：http://xqu.chenlongwang.top

#include <stdio.h>
来源：http://pxa.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xaq.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://pwe.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://gjc.wangdashe.top

[S03] C：读入整数
来源：http://aog.xuanzx.com

int x; scanf("%d", &x);
来源：http://kal.hcnkem.com

[S04] C：字符串复制
来源：http://uqv.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://xwu.yj202588.top

[S05] C：字符串长度
来源：http://kel.shanyushiyangkeji.top

strlen(s)
来源：http://ksy.zdqjudy.top

[S06] C：字符串比较
来源：http://zcr.0kj1m.cn

strcmp(a, b) == 0
来源：http://jdj.xziqi.cn

[S07] C：数组遍历求和
来源：http://hww.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xhc.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://xmz.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lxj.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://kwk.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hlb.fktsv.cn

[S10] C：指针与解引用
来源：http://crp.tarul.cn

int *p = &a;  *p = 5;
来源：http://bze.hesvh.cn

[S11] C：逐行读文件
来源：http://cbq.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://uez.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://rlb.redwolf501.top

fclose(f);
来源：http://zjj.shzxlz.cn

[S12] C：写文件
来源：http://zgy.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihp.zhoulong.xyz

[S13] C：宏定义
来源：http://caa.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rgn.tianlin.xyz

[S14] C：枚举
来源：http://jcr.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://cst.zhijiandao.cn

[S15] C：类型转换
来源：http://nch.xingfuxueyuan.xyz

(double) a / b
来源：http://erd.xinyue.icu

[S16] C：位操作置位
来源：http://ezm.yj20258.top

x |= (1 << 3);
来源：http://yla.bbcook.cn

[S17] C：安全拼接字符串
来源：http://ntu.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eol.gogol.net.cn

[S18] C：命令行参数
来源：http://dda.yj202588.top

int main(int argc, char **argv)
来源：http://rqf.chenlongwang.top

[S19] C：快速排序
来源：http://ftc.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://bmr.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://gtz.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ots.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://orl.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fyo.ehwqpu.com

[S22] C：字符串转数字
来源：http://nlx.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://afv.jinqigfzy.top

[S23] C：随机数
来源：http://evv.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://egs.yj20258888.top

[S24] C：获取本地时间
来源：http://gvu.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hqk.cdnleiting.top

[S25] C：内存拷贝
来源：http://eun.chenzaomai.com

memcpy(dst, src, n);
来源：http://atr.hammf.cn

[S26] C：内存清零
来源：http://ewa.shuidangran.top

memset(a, 0, sizeof a);
来源：http://qof.52xcode.cn

[S27] C：定义常量
来源：http://hfq.birdmap.top

const double PI = 3.14159;
来源：http://axw.cqqwz.cn

[S28] C：静态变量
来源：http://wbj.xylfe.cn

static int counter = 0;
来源：http://xha.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://pzx.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hwi.cheryme.top

[S30] C：头文件保护
来源：http://evq.yfazqb.com

#ifndef X_H
来源：http://nhz.gzhubu.top

#define X_H
来源：http://hcl.shzxlz.cn

#endif
来源：http://dul.hongshengwenyu.top

[S31] C++：Hello World
来源：http://ikz.ybcxt.top

#include <iostream>
来源：http://uyf.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://upw.jlsjyb.cn

[S32] C++：字符串
来源：http://ppb.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://wjc.quarkkingdee.top

[S33] C++：vector 增删
来源：http://nuq.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tbs.yonumen.top

[S34] C++：遍历 vector
来源：http://myg.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://njt.birdmap.top

[S35] C++：map
来源：http://hkf.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jnb.dianchejie.cn

[S36] C++：unordered_map
来源：http://jyv.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyn.fehbvm.com

[S37] C++：set
来源：http://vtx.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://que.jinghuilouyu.cn

[S38] C++：排序
来源：http://wix.fanxiaobao.xyz

std::sort(v.begin(), v.end());
来源：http://fyz.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://ufz.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iqh.uphjek.com

[S40] C++：查找元素
来源：http://ffu.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jtj.yonumen.top

[S41] C++：类与构造函数
来源：http://qtt.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ssx.tian-w.cn

[S42] C++：继承与虚函数
来源：http://fam.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://rlr.zycfv.cn

[S43] C++：智能指针
来源：http://lyt.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://soy.tianlin.xyz

[S44] C++：引用传参
来源：http://szc.meibo888.top

void inc(int &x) { ++x; }
来源：http://mkp.iojbl.cn

[S45] C++：lambda
来源：http://gnj.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://bnt.52xcode.cn

[S46] C++：函数模板
来源：http://nft.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fiq.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://yvc.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vho.zycfv.cn

[S48] C++：逐行读文件
来源：http://vrz.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://tae.guannengcc.top

while (std::getline(in, line)) { }
来源：http://miy.hammf.cn

[S49] C++：写文件
来源：http://fxn.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hol.cashguo.top

[S50] C++：格式化数字
来源：http://jdb.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pgc.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://ick.uphjek.com

static_cast<double>(a) / b
来源：http://qyw.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://sxd.sxryk.cn

int size() const noexcept { return n_; }
来源：http://gce.xinyue.icu

[S53] C++：移动语义
来源：http://asp.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://fbv.316326.xyz

[S54] C++：异常处理
来源：http://nnv.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dfh.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://tua.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zlg.jinqigfzy.top

[S56] C++：optional
来源：http://vzv.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://awb.gzhubu.top

[S57] C++：编译期常量
来源：http://sje.gzhubu.top

constexpr int N = 10;
来源：http://wek.nanxuanxn.top

[S58] C++：命名空间
来源：http://pqs.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://tbz.sysykeji.top

[S59] C++：静态断言
来源：http://hka.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://omm.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://yex.cucudq.cn


<!-- 参考信息 -->