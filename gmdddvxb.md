代发 wailian999

[Q84] 去除首尾空格
来源：http://rym.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://ryh.ybcxt.top

[Q85] 数值取整
来源：http://jvm.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vly.pycfn.com

[Q86] 读取 JSON 字段
来源：http://qob.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dyn.xziqi.cn

[Q87] JSON 字段做条件
来源：http://nzk.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hyk.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://stb.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qhi.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ord.snrcjt.cn

[Q89] 判断表是否存在
来源：http://fkt.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://peu.zhijiandao.cn

[Q90] 生成序号列
来源：http://mkc.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://czj.nwbrower.top

================================================================================
来源：http://ncs.fzhhl.top

R. Bash 专题
来源：http://vju.epnwcf.com

================================================================================
来源：http://ppr.hysaishi.cn

[R01] shebang 与严格模式
来源：http://egr.epnwcf.com

#!/usr/bin/env bash
来源：http://kgk.zhiwuduotai.top

set -euo pipefail
来源：http://hxd.ctjpmb.com

[R02] 变量赋值与使用
来源：http://fqh.ydzc1.top

name="Tom"; echo "$name"
来源：http://ajo.nanxuanxn.top

[R03] 只读变量
来源：http://chd.xziqi.cn

readonly PI=3.14
来源：http://gio.yonumen.top

[R04] 位置参数
来源：http://owc.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bqj.fehbvm.com

[R05] 参数默认值
来源：http://grg.52xcode.cn

name="${1:-default}"
来源：http://qqt.yangfankeji.com

[R06] 判断命令是否存在
来源：http://ujh.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lho.nanxinkj.top

[R07] if 判断文件
来源：http://yqh.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://src.zycfv.cn

[R08] 数值比较
来源：http://zwk.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aqh.tanke756.top

[R09] 字符串比较
来源：http://ehr.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ahp.gaohongyu789.top

[R10] 正则匹配
来源：http://wkv.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://avl.bjfxy.top

[R11] case 多分支
来源：http://qng.jqgufenzy.top

case "$1" in
来源：http://dmj.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://jrq.fehbvm.com

stop)  echo "停止" ;;
来源：http://tpa.tarul.cn

*)     echo "未知命令" ;;
来源：http://fzh.9152youxi.cn

esac
来源：http://mlc.fzhhl.top

[R12] for 遍历文件
来源：http://kex.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://rpk.nwbrower.top

[R13] for 计数循环
来源：http://rla.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://asr.shuidangran.top

[R14] C 风格 for
来源：http://tlm.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lzq.gogol.net.cn

[R15] while 逐行读文件
来源：http://wpq.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tmo.sufxvd.cn

[R16] until 等待条件
来源：http://ljq.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zko.guowangkeji.top

[R17] 数组定义与取值
来源：http://chv.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://vcd.jianghu66.top

[R18] 遍历数组
来源：http://wbu.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mfb.uphjek.com

[R19] 数组长度
来源：http://uhn.zhengqikj.top

echo "${#arr[@]}"
来源：http://ssr.ydzc1.top

[R20] 关联数组（字典）
来源：http://gez.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vdw.gaohongyu789.top

[R21] 字符串长度
来源：http://emx.chenlongwang.top

echo "${#s}"
来源：http://lwm.yj202588.top

[R22] 截取子串
来源：http://hka.mhx1999.top

echo "${s:0:5}"
来源：http://fhj.cdnleiting.top

[R23] 字符串替换
来源：http://fvq.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yib.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://isg.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://oka.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://gzm.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nnv.9152youxi.cn

[R26] 命令替换
来源：http://xwh.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://fdl.hywenlv.cn

[R27] 算术展开
来源：http://rrd.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://xuo.epnwcf.com

[R28] 浮点运算
来源：http://sgp.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://zhl.yj20258.top

[R29] 定义函数
来源：http://brs.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ikp.fzhhl.top

[R30] 函数返回状态码
来源：http://izs.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://lfw.zycfv.cn

[R31] 局部变量
来源：http://pym.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://ihp.hongshengwenyu.top

[R32] 参数个数校验
来源：http://sns.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nvc.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://ngu.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tur.hnxiangtu.top

[R34] 退出时清理
来源：http://vtk.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://kvh.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://cuj.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ene.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://vnn.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nex.guowangkeji.top

[R37] 把输出赋给变量
来源：http://lir.yfazqb.com

files=$(ls -1)
来源：http://jfw.jinqigufen.top

[R38] 管道串联
来源：http://dck.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://vgg.havefunace.top

[R39] 重定向标准输出与错误
来源：http://jly.ehwqpu.com

cmd > out.log 2>&1
来源：http://ewi.birdmap.top

[R40] 追加写日志
来源：http://jlp.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://tax.yongpay.top

[R41] 丢弃输出
来源：http://zsa.tarul.cn

cmd >/dev/null 2>&1
来源：http://dhp.ctjpmb.com

[R42] 输入重定向
来源：http://zqu.jiagoushi.top

wc -l < a.txt
来源：http://ddg.aibaodan.cn

[R43] 按名字查找文件
来源：http://dvo.daxiang520.top

find . -name "*.log" -type f
来源：http://rny.smart0.xyz

[R44] 按修改时间查找
来源：http://qyj.zhoulong.xyz

find . -mtime -7 -type f
来源：http://lwz.dashuyun.cn

[R45] 批量删除
来源：http://abh.tanke756.top

find . -name "*.tmp" -delete
来源：http://mua.jianghu66.top

[R46] 递归替换文件内容
来源：http://kbk.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yhy.52xcode.cn

[R47] sed 单行替换
来源：http://wlb.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yet.jinqigfzy.top

[R48] awk 取指定列
来源：http://oga.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://evt.ydjk.org.cn

[R49] awk 带条件
来源：http://czf.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qnl.jianghu66.top

[R50] awk 求和
来源：http://nlq.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://edk.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://tab.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mcc.sweek.top

[R52] 统计行数
来源：http://qkg.9152youxi.cn

wc -l a.txt
来源：http://bit.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://iov.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://irq.vehdjk.com

[R54] 比较两个文件
来源：http://crz.0kj1m.cn

diff a.txt b.txt
来源：http://fvt.cashguo.top

[R55] 压缩与解压
来源：http://txg.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ozz.ybcxt.top

[R56] 远程拷贝
来源：http://hkw.aibaodan.cn

scp file user@host:/path/
来源：http://ulr.sysykeji.top

[R57] 远程执行命令
来源：http://tvq.wangdashe.top

ssh user@host 'uptime'
来源：http://pqo.yueranfly.top

[R58] 下载文件
来源：http://ccy.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jyb.ehwqpu.com

[R59] 发 POST JSON
来源：http://iow.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rsf.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://rlc.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://etq.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://lxy.shzxlz.cn

df -h;  du -sh *
来源：http://ecw.yuxming.cn

[R62] 找最占空间的文件
来源：http://rrx.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://ppo.cucudq.cn

[R63] 内存与进程
来源：http://xkz.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://ymg.xylfe.cn

[R64] 结束进程
来源：http://sel.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://yhq.cqqwz.cn

[R65] 查看端口占用
来源：http://zfc.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uzj.iojbl.cn

[R66] 定时任务
来源：http://flz.aizwys.cn

crontab -e;  crontab -l
来源：http://bmv.sweek.top

[R67] 生成随机十六进制串
来源：http://iyu.wangdashe.top

openssl rand -hex 16
来源：http://ibn.andypj.xyz

[R68] 计算文件校验值
来源：http://omr.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sjp.gzhubu.top

[R69] 生成随机密码
来源：http://ccx.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://thb.xziqi.cn

[R70] 时间戳与互转
来源：http://ryi.havefunace.top

date +%s;  date -d @1700000000
来源：http://sik.hongshengwenyu.top

[R71] 日期格式化
来源：http://xed.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://zrz.cheryme.top

[R72] 等待端口就绪
来源：http://htd.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://scj.zycfv.cn

[R73] 分割大日志
来源：http://yvq.yongpay.top

split -l 1000 big.log part_
来源：http://ajm.jianghu66.top

[R74] 批量重命名
来源：http://ayy.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://swy.9152youxi.cn

[R75] 导出环境变量
来源：http://bun.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://edt.tianlin.xyz

[R76] 使用临时文件
来源：http://gou.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lto.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://mfx.zhijiandao.cn

read -rp "请输入: " ans
来源：http://jzz.chenzaomai.com

[R78] 交互式菜单
来源：http://asx.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://vsu.jlsjyb.cn

[R79] 解析命令行选项
来源：http://rsf.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bjr.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://ytv.bbcook.cn

time ./run.sh
来源：http://rsy.yj20258.top

================================================================================
来源：http://ewl.jianghu66.top

S. C / C++ 专题
来源：http://xzq.ivvv.top

================================================================================
来源：http://kxa.ivvv.top

[S01] C：Hello World
来源：http://baq.316326.xyz

#include <stdio.h>
来源：http://kfq.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bbs.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://lva.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://swk.gaohongyu789.top

[S03] C：读入整数
来源：http://nki.zycfv.cn

int x; scanf("%d", &x);
来源：http://wup.tianlin.xyz

[S04] C：字符串复制
来源：http://kgj.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://mhs.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://orb.bjfxy.top

strlen(s)
来源：http://vgc.nwbrower.top

[S06] C：字符串比较
来源：http://upw.yj20258.top

strcmp(a, b) == 0
来源：http://oxq.ehwqpu.com

[S07] C：数组遍历求和
来源：http://sgh.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jru.uphjek.com

[S08] C：动态内存分配与释放
来源：http://xpo.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nfh.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://fqv.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uea.vehdjk.com

[S10] C：指针与解引用
来源：http://vix.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://dbi.tarul.cn

[S11] C：逐行读文件
来源：http://wtx.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://iea.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zig.pycfn.com

fclose(f);
来源：http://prr.jqgfzy.top

[S12] C：写文件
来源：http://hrq.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qpw.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://oul.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://foc.gzhubu.top

[S14] C：枚举
来源：http://ttm.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://tap.guannengcc.top

[S15] C：类型转换
来源：http://sgu.birdmap.top

(double) a / b
来源：http://djp.sysykeji.top

[S16] C：位操作置位
来源：http://vig.gotoacloud.top

x |= (1 << 3);
来源：http://cse.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://mmc.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uwx.jiagoushi.top

[S18] C：命令行参数
来源：http://evt.tianlin.xyz

int main(int argc, char **argv)
来源：http://afl.vehdjk.com

[S19] C：快速排序
来源：http://okh.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://unj.smart0.xyz

[S20] C：二分查找
来源：http://heb.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vhg.guannengcc.top

[S21] C：字符类别判断
来源：http://gul.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://izj.jianghu66.top

[S22] C：字符串转数字
来源：http://ycv.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://qfb.zhengqikj.top

[S23] C：随机数
来源：http://fey.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iir.cqqwz.cn

[S24] C：获取本地时间
来源：http://syy.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://moq.bbcook.cn

[S25] C：内存拷贝
来源：http://kue.yueranfly.top

memcpy(dst, src, n);
来源：http://ump.hesvh.cn

[S26] C：内存清零
来源：http://ngq.c1oappe.top

memset(a, 0, sizeof a);
来源：http://duw.jlsjyb.cn

[S27] C：定义常量
来源：http://yaa.ctjpmb.com

const double PI = 3.14159;
来源：http://dql.fktsv.cn

[S28] C：静态变量
来源：http://cqw.316326.xyz

static int counter = 0;
来源：http://nqw.ppjwa.cn

[S29] C：变参函数
来源：http://bbb.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zlh.ybcxt.top

[S30] C：头文件保护
来源：http://yzk.yfazqb.com

#ifndef X_H
来源：http://mbq.fktsv.cn

#define X_H
来源：http://qgo.ctjpmb.com

#endif
来源：http://aqh.yuanzhike.top

[S31] C++：Hello World
来源：http://exx.xylfe.cn

#include <iostream>
来源：http://ujl.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://erv.zdbjq.cn

[S32] C++：字符串
来源：http://prx.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://qta.guannengcc.top

[S33] C++：vector 增删
来源：http://rsm.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hgt.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://kvh.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://pmt.shuidangran.top

[S35] C++：map
来源：http://wot.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rrn.hywenlv.cn

[S36] C++：unordered_map
来源：http://wtq.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awg.yueranfly.top

[S37] C++：set
来源：http://vtj.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sen.316326.xyz

[S38] C++：排序
来源：http://zmz.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://hau.tanke756.top

[S39] C++：自定义比较器排序
来源：http://rgi.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zkx.dianchejie.cn

[S40] C++：查找元素
来源：http://wti.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ugy.yj20258888.top

[S41] C++：类与构造函数
来源：http://xjo.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://atx.hesvh.cn

[S42] C++：继承与虚函数
来源：http://opw.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://iyn.daria6918.cn

[S43] C++：智能指针
来源：http://szw.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://nlm.mhx1999.top

[S44] C++：引用传参
来源：http://ash.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://bnf.xuanzx.com

[S45] C++：lambda
来源：http://vrx.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://rar.jiagoushi.top

[S46] C++：函数模板
来源：http://xyp.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bis.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://crn.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gqz.aizwys.cn

[S48] C++：逐行读文件
来源：http://xjv.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://czh.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://olg.epnwcf.com

[S49] C++：写文件
来源：http://ilo.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wmk.cqqwz.cn

[S50] C++：格式化数字
来源：http://cyw.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xuf.c1oappe.top

[S51] C++：显式类型转换
来源：http://pqe.shzxlz.cn

static_cast<double>(a) / b
来源：http://nua.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://hwx.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://vux.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://cyf.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://dpk.zhengqikj.top

[S54] C++：异常处理
来源：http://vut.bbcook.cn


<!-- 参考信息 -->