代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eol.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://jzr.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cxa.snrcjt.cn

================================================================================
来源：http://uut.hcnkem.com

R. Bash 专题
来源：http://wir.9152youxi.cn

================================================================================
来源：http://xdc.tianlin.xyz

[R01] shebang 与严格模式
来源：http://cms.hammf.cn

#!/usr/bin/env bash
来源：http://iye.andypj.xyz

set -euo pipefail
来源：http://dsa.fehbvm.com

[R02] 变量赋值与使用
来源：http://mvr.daxiang520.top

name="Tom"; echo "$name"
来源：http://prt.hywenlv.cn

[R03] 只读变量
来源：http://ejo.zhiwuduotai.top

readonly PI=3.14
来源：http://yll.snrcjt.cn

[R04] 位置参数
来源：http://tan.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cjg.kuanghao11.cn

[R05] 参数默认值
来源：http://aoz.zhongyouzk.top

name="${1:-default}"
来源：http://zuc.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://xlh.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bry.zdbjq.cn

[R07] if 判断文件
来源：http://vid.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jax.daria6918.cn

[R08] 数值比较
来源：http://jlx.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vfo.hnxiangtu.top

[R09] 字符串比较
来源：http://gvw.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sla.jinqigfzy.top

[R10] 正则匹配
来源：http://gja.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://arb.shzxlz.cn

[R11] case 多分支
来源：http://uxg.quarkkingdee.top

case "$1" in
来源：http://zbr.daxiang520.top

start) echo "启动" ;;
来源：http://spv.c1oappe.top

stop)  echo "停止" ;;
来源：http://pqn.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://nih.haohaochexian.top

esac
来源：http://cif.zycfv.cn

[R12] for 遍历文件
来源：http://cwb.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://bit.zhoulong.xyz

[R13] for 计数循环
来源：http://dqc.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://opn.nanxuanxn.top

[R14] C 风格 for
来源：http://zse.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qjt.xinyue.icu

[R15] while 逐行读文件
来源：http://lak.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wcw.jinqigufen.top

[R16] until 等待条件
来源：http://tmq.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kut.aibaodan.cn

[R17] 数组定义与取值
来源：http://zmx.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uid.yuanzhike.top

[R18] 遍历数组
来源：http://zqi.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pbi.hongshengwenyu.top

[R19] 数组长度
来源：http://jbg.52xcode.cn

echo "${#arr[@]}"
来源：http://chq.shzxlz.cn

[R20] 关联数组（字典）
来源：http://abi.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vtf.316326.xyz

[R21] 字符串长度
来源：http://quh.ppjwa.cn

echo "${#s}"
来源：http://oto.9152youxi.cn

[R22] 截取子串
来源：http://wms.cucudq.cn

echo "${s:0:5}"
来源：http://yxp.yuxming.cn

[R23] 字符串替换
来源：http://zmd.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ekg.hfpthk.cn

[R24] 大小写转换
来源：http://yjv.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://uim.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://okt.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkt.gogol.net.cn

[R26] 命令替换
来源：http://fsf.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://tby.dianchejie.cn

[R27] 算术展开
来源：http://loi.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://txc.gotoacloud.top

[R28] 浮点运算
来源：http://xdw.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://sar.jinqigfzy.top

[R29] 定义函数
来源：http://nhz.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://abh.zhoulong.xyz

[R30] 函数返回状态码
来源：http://kic.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://pcq.yangfankeji.com

[R31] 局部变量
来源：http://nop.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://ppu.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://rvg.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zeu.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://rnh.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hea.ehwqpu.com

[R34] 退出时清理
来源：http://vlz.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rmy.vehdjk.com

[R35] 后台执行并等待
来源：http://qfd.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xpp.yfazqb.com

[R36] 并发执行多个任务
来源：http://ytd.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jha.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://amy.shangyingyoupin.top

files=$(ls -1)
来源：http://lvg.xylfe.cn

[R38] 管道串联
来源：http://jer.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://kpo.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://wcw.daria6918.cn

cmd > out.log 2>&1
来源：http://uaq.hongshengwenyu.top

[R40] 追加写日志
来源：http://qqj.zdbjq.cn

echo "log" >> out.log
来源：http://xgq.cdnleiting.top

[R41] 丢弃输出
来源：http://isy.havefunace.top

cmd >/dev/null 2>&1
来源：http://mdv.xuetiantiany.cn

[R42] 输入重定向
来源：http://wgc.havefunace.top

wc -l < a.txt
来源：http://fqa.shzxlz.cn

[R43] 按名字查找文件
来源：http://zxp.316326.xyz

find . -name "*.log" -type f
来源：http://kid.jianghu66.top

[R44] 按修改时间查找
来源：http://wmz.ydzc1.top

find . -mtime -7 -type f
来源：http://pnm.zdqjudy.top

[R45] 批量删除
来源：http://iqy.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://nof.gogol.net.cn

[R46] 递归替换文件内容
来源：http://vro.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mny.yfazqb.com

[R47] sed 单行替换
来源：http://ade.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://mrg.ybcxt.top

[R48] awk 取指定列
来源：http://myt.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://aqu.9152youxi.cn

[R49] awk 带条件
来源：http://skj.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://orw.zdbjq.cn

[R50] awk 求和
来源：http://vpa.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://grp.gzhubu.top

[R51] 排序去重取前几
来源：http://crn.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ggy.vqdsnc.cn

[R52] 统计行数
来源：http://zud.zhiwuduotai.top

wc -l a.txt
来源：http://cjp.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://ewf.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://edj.xziqi.cn

[R54] 比较两个文件
来源：http://pbo.fehbvm.com

diff a.txt b.txt
来源：http://qqk.feifeiyinyue.top

[R55] 压缩与解压
来源：http://ife.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nlh.fzhhl.top

[R56] 远程拷贝
来源：http://axi.nanxinkj.top

scp file user@host:/path/
来源：http://akv.chenjidiqi.icu

[R57] 远程执行命令
来源：http://tyo.yongpay.top

ssh user@host 'uptime'
来源：http://knw.nanxinkj.top

[R58] 下载文件
来源：http://glf.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baw.yangfankeji.com

[R59] 发 POST JSON
来源：http://ycx.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rpq.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://vrg.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://drf.zhiwuduotai.top

[R61] 磁盘占用
来源：http://emf.nwbrower.top

df -h;  du -sh *
来源：http://ukz.daria6918.cn

[R62] 找最占空间的文件
来源：http://qxo.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://opx.smart0.xyz

[R63] 内存与进程
来源：http://mka.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://tiq.xylfe.cn

[R64] 结束进程
来源：http://gbt.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://tca.gotoacloud.top

[R65] 查看端口占用
来源：http://gjx.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://awm.cheryme.top

[R66] 定时任务
来源：http://uzr.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://wzo.xuanzx.com

[R67] 生成随机十六进制串
来源：http://wef.pengpengdd.cyou

openssl rand -hex 16
来源：http://teh.c1oappe.top

[R68] 计算文件校验值
来源：http://dts.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://rsz.jqgufenzy.top

[R69] 生成随机密码
来源：http://xvr.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://lww.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://zan.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://ecl.hnxiangtu.top

[R71] 日期格式化
来源：http://dqs.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vpv.shuidangran.top

[R72] 等待端口就绪
来源：http://dew.xziqi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://shb.zhengqikj.top

[R73] 分割大日志
来源：http://tng.guannengcc.top

split -l 1000 big.log part_
来源：http://tio.gzhubu.top

[R74] 批量重命名
来源：http://ykr.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oql.aibaodan.cn

[R75] 导出环境变量
来源：http://hhs.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://yip.sysykeji.top

[R76] 使用临时文件
来源：http://cfz.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bcb.andypj.xyz

[R77] 读取用户输入
来源：http://psa.chenlongwang.top

read -rp "请输入: " ans
来源：http://rbu.shuidangran.top

[R78] 交互式菜单
来源：http://dpv.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yuv.chenzaomai.com

[R79] 解析命令行选项
来源：http://jbm.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nps.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://jyd.jqgufenzy.top

time ./run.sh
来源：http://lzc.xylfe.cn

================================================================================
来源：http://lgj.tarul.cn

S. C / C++ 专题
来源：http://mhl.shuidangran.top

================================================================================
来源：http://hml.nanxuanxn.top

[S01] C：Hello World
来源：http://ids.fzhhl.top

#include <stdio.h>
来源：http://bsf.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gtw.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://fvo.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://ijh.snrcjt.cn

[S03] C：读入整数
来源：http://szb.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://rdk.guowangkeji.top

[S04] C：字符串复制
来源：http://msm.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://nze.xziqi.cn

[S05] C：字符串长度
来源：http://khw.52xcode.cn

strlen(s)
来源：http://waj.zdqjudy.top

[S06] C：字符串比较
来源：http://yzv.tian-w.cn

strcmp(a, b) == 0
来源：http://ivw.xinyue.icu

[S07] C：数组遍历求和
来源：http://czv.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vsb.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://gtl.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zze.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://iko.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://elq.uphjek.com

[S10] C：指针与解引用
来源：http://sip.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://jlo.cdnleiting.top

[S11] C：逐行读文件
来源：http://yit.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://xcz.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://obl.sjlbkw.cn

fclose(f);
来源：http://vnz.cucudq.cn

[S12] C：写文件
来源：http://zcj.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://opl.haohaochexian.top

[S13] C：宏定义
来源：http://xbc.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qir.gotoacloud.top

[S14] C：枚举
来源：http://dcy.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://gwc.ehwqpu.com

[S15] C：类型转换
来源：http://mss.hfpthk.cn

(double) a / b
来源：http://onj.cashguo.top

[S16] C：位操作置位
来源：http://bxq.iojbl.cn

x |= (1 << 3);
来源：http://uyw.316326.xyz

[S17] C：安全拼接字符串
来源：http://ggb.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qhy.gaohongyu789.top

[S18] C：命令行参数
来源：http://swf.zhijiandao.cn

int main(int argc, char **argv)
来源：http://hcr.0kj1m.cn

[S19] C：快速排序
来源：http://yrw.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://dds.52xcode.cn

[S20] C：二分查找
来源：http://kay.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eor.hesvh.cn

[S21] C：字符类别判断
来源：http://fzb.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ght.wangdashe.top

[S22] C：字符串转数字
来源：http://jyk.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cae.shzxlz.cn

[S23] C：随机数
来源：http://tqw.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://hxi.fengsongda.top

[S24] C：获取本地时间
来源：http://ldo.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pwd.svipenyu.cn

[S25] C：内存拷贝
来源：http://uix.yj202588.top

memcpy(dst, src, n);
来源：http://tsg.cheryme.top

[S26] C：内存清零
来源：http://qix.fengsongda.top

memset(a, 0, sizeof a);
来源：http://jbe.pengpengdd.cyou

[S27] C：定义常量
来源：http://qof.wangdashe.top

const double PI = 3.14159;
来源：http://lqm.xinyue.icu

[S28] C：静态变量
来源：http://gqz.fzhhl.top

static int counter = 0;
来源：http://izz.nanxuanxn.top

[S29] C：变参函数
来源：http://ggw.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sgg.316326.xyz

[S30] C：头文件保护
来源：http://hbq.sjlbkw.cn

#ifndef X_H
来源：http://sgp.yonumen.top

#define X_H
来源：http://yzb.ivvv.top

#endif
来源：http://mlf.hnxiangtu.top

[S31] C++：Hello World
来源：http://zpa.shzxlz.cn

#include <iostream>
来源：http://cad.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://iec.hfpthk.cn

[S32] C++：字符串
来源：http://ejh.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://txv.yvedp.cn

[S33] C++：vector 增删
来源：http://pch.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kwa.ctjpmb.com

[S34] C++：遍历 vector
来源：http://njz.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://tck.zhoulong.xyz

[S35] C++：map
来源：http://oqz.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fku.hnxiangtu.top

[S36] C++：unordered_map
来源：http://czf.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sln.redwolf501.top

[S37] C++：set
来源：http://nlk.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mva.jyoumei.cn

[S38] C++：排序
来源：http://fmq.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://hka.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://awn.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oeu.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://lru.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://npm.sxryk.cn

[S41] C++：类与构造函数
来源：http://qyp.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pgo.tarul.cn

[S42] C++：继承与虚函数
来源：http://ewm.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://nrf.svipenyu.cn

[S43] C++：智能指针
来源：http://nhf.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://auz.fehbvm.com

[S44] C++：引用传参
来源：http://who.yfazqb.com

void inc(int &x) { ++x; }
来源：http://dpf.fanxiaobao.xyz

[S45] C++：lambda
来源：http://rah.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mlf.jqgfzy.top

[S46] C++：函数模板
来源：http://hsd.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://azf.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://gsi.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uyo.ybcxt.top

[S48] C++：逐行读文件
来源：http://htj.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://iem.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://sah.meibo888.top

[S49] C++：写文件
来源：http://xre.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gwd.guannengcc.top

[S50] C++：格式化数字
来源：http://pig.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zls.ppjwa.cn

[S51] C++：显式类型转换
来源：http://ksk.9152youxi.cn

static_cast<double>(a) / b
来源：http://pox.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://ncz.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://pzm.pycfn.com

[S53] C++：移动语义
来源：http://xjq.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://tzc.vqdsnc.cn

[S54] C++：异常处理
来源：http://ikj.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ahm.sxryk.cn

[S55] C++：结构化绑定
来源：http://zoe.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vfj.cqqwz.cn

[S56] C++：optional
来源：http://mqz.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://anr.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://pqc.sufxvd.cn

constexpr int N = 10;
来源：http://suc.feifeiyinyue.top

[S58] C++：命名空间
来源：http://mif.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://lqc.hysaishi.cn

[S59] C++：静态断言
来源：http://yst.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jbx.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://euf.xinyue.icu


<!-- 参考信息 -->