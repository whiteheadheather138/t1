代发 wailian999

[Q84] 去除首尾空格
来源：http://kmy.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://kxk.fktsv.cn

[Q85] 数值取整
来源：http://qln.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qlo.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://xha.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hlm.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://njb.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://npy.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://cum.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tby.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gnh.yfazqb.com

[Q89] 判断表是否存在
来源：http://ogs.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xvi.dashuyun.cn

[Q90] 生成序号列
来源：http://pux.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gnm.redwolf501.top

================================================================================
来源：http://xmj.fengsongda.top

R. Bash 专题
来源：http://vdb.cheryme.top

================================================================================
来源：http://dgw.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://pxi.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://gic.sysykeji.top

set -euo pipefail
来源：http://iqz.tian-w.cn

[R02] 变量赋值与使用
来源：http://fwm.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://jej.xinyue.icu

[R03] 只读变量
来源：http://yqq.snrcjt.cn

readonly PI=3.14
来源：http://tti.vehdjk.com

[R04] 位置参数
来源：http://zga.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://esx.9152youxi.cn

[R05] 参数默认值
来源：http://otr.hywenlv.cn

name="${1:-default}"
来源：http://shd.cdnleiting.top

[R06] 判断命令是否存在
来源：http://niy.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jpu.fengsongda.top

[R07] if 判断文件
来源：http://vez.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kjv.andypj.xyz

[R08] 数值比较
来源：http://bqr.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eee.daria6918.cn

[R09] 字符串比较
来源：http://woc.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ino.gaohongyu789.top

[R10] 正则匹配
来源：http://cre.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aqy.guowangkeji.top

[R11] case 多分支
来源：http://cmq.ydzc1.top

case "$1" in
来源：http://aua.sxryk.cn

start) echo "启动" ;;
来源：http://zrq.smart0.xyz

stop)  echo "停止" ;;
来源：http://dsu.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://wxi.pengpengdd.cyou

esac
来源：http://ims.quarkkingdee.top

[R12] for 遍历文件
来源：http://umt.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://pbc.zhoulong.xyz

[R13] for 计数循环
来源：http://jgy.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://mpw.quarkkingdee.top

[R14] C 风格 for
来源：http://sia.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mlt.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://pde.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kbg.sysykeji.top

[R16] until 等待条件
来源：http://fjr.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yxw.tian-w.cn

[R17] 数组定义与取值
来源：http://hqy.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://cym.shuidangran.top

[R18] 遍历数组
来源：http://sxb.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iup.cheryme.top

[R19] 数组长度
来源：http://fus.9152youxi.cn

echo "${#arr[@]}"
来源：http://nkz.yuanzhike.top

[R20] 关联数组（字典）
来源：http://udz.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uze.gogol.net.cn

[R21] 字符串长度
来源：http://xmj.shanyushiyangtech.top

echo "${#s}"
来源：http://rfs.ehwqpu.com

[R22] 截取子串
来源：http://zba.zhixingplan.top

echo "${s:0:5}"
来源：http://cki.nanxinkj.top

[R23] 字符串替换
来源：http://uos.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://phr.sufxvd.cn

[R24] 大小写转换
来源：http://soc.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://zvh.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://yns.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yjb.316326.xyz

[R26] 命令替换
来源：http://yxm.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://yfp.havefunace.top

[R27] 算术展开
来源：http://tzn.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://rwq.zhengqikj.top

[R28] 浮点运算
来源：http://tkh.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://fse.nanxinkj.top

[R29] 定义函数
来源：http://pwz.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oyz.xziqi.cn

[R30] 函数返回状态码
来源：http://jsr.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://lfx.yueranfly.top

[R31] 局部变量
来源：http://xkg.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://iea.havefunace.top

[R32] 参数个数校验
来源：http://qgj.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://olu.yj20258.top

[R33] 捕获错误并提示行号
来源：http://cwg.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://llu.ydjk.org.cn

[R34] 退出时清理
来源：http://xwa.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://agx.nanxuanxn.top

[R35] 后台执行并等待
来源：http://fzb.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xva.redwolf501.top

[R36] 并发执行多个任务
来源：http://ueq.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uqk.52xcode.cn

[R37] 把输出赋给变量
来源：http://pkc.dianchejie.cn

files=$(ls -1)
来源：http://law.dashuyun.cn

[R38] 管道串联
来源：http://rcd.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://hge.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://jfd.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://qeo.fzhhl.top

[R40] 追加写日志
来源：http://qem.jinqigfzy.top

echo "log" >> out.log
来源：http://wsz.cheryme.top

[R41] 丢弃输出
来源：http://elh.hammf.cn

cmd >/dev/null 2>&1
来源：http://iea.yj202588.top

[R42] 输入重定向
来源：http://rbu.sxryk.cn

wc -l < a.txt
来源：http://bvc.guowangkeji.top

[R43] 按名字查找文件
来源：http://pih.sjlbkw.cn

find . -name "*.log" -type f
来源：http://rlt.shzxlz.cn

[R44] 按修改时间查找
来源：http://iga.nanxinkj.top

find . -mtime -7 -type f
来源：http://jcy.yangfankeji.com

[R45] 批量删除
来源：http://ppz.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://qgc.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://eaq.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wke.havefunace.top

[R47] sed 单行替换
来源：http://cwl.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://bus.nanxinkj.top

[R48] awk 取指定列
来源：http://qua.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://sng.feifeiyinyue.top

[R49] awk 带条件
来源：http://gjr.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cqi.gaohongyu789.top

[R50] awk 求和
来源：http://mce.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://uuj.yanxiufei.cn

[R51] 排序去重取前几
来源：http://uua.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dvl.fehbvm.com

[R52] 统计行数
来源：http://wqv.aibaodan.cn

wc -l a.txt
来源：http://jrh.cashguo.top

[R53] 查看文件头与实时尾
来源：http://bpm.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yur.xuetiantiany.cn

[R54] 比较两个文件
来源：http://nfe.redwolf501.top

diff a.txt b.txt
来源：http://yog.iojbl.cn

[R55] 压缩与解压
来源：http://sas.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcb.yuxming.cn

[R56] 远程拷贝
来源：http://orz.jqgufenzy.top

scp file user@host:/path/
来源：http://xxi.cdnleiting.top

[R57] 远程执行命令
来源：http://hvy.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://ous.yuanzhike.top

[R58] 下载文件
来源：http://oab.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qvo.xziqi.cn

[R59] 发 POST JSON
来源：http://wgh.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vxo.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://hiq.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://usv.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://xfl.hesvh.cn

df -h;  du -sh *
来源：http://alv.iojbl.cn

[R62] 找最占空间的文件
来源：http://fjc.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://dea.cucudq.cn

[R63] 内存与进程
来源：http://vhj.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://ggf.uphjek.com

[R64] 结束进程
来源：http://nsx.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://ity.pycfn.com

[R65] 查看端口占用
来源：http://giz.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nnf.ydzc1.top

[R66] 定时任务
来源：http://irk.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://hyn.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://wfu.dashuyun.cn

openssl rand -hex 16
来源：http://yde.vqdsnc.cn

[R68] 计算文件校验值
来源：http://yll.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dsx.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://lbv.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://fei.yuxming.cn

[R70] 时间戳与互转
来源：http://sps.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://rlb.gotoacloud.top

[R71] 日期格式化
来源：http://yrg.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rpa.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://upt.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ask.yuanzhike.top

[R73] 分割大日志
来源：http://mqf.shuidangran.top

split -l 1000 big.log part_
来源：http://qpe.52xcode.cn

[R74] 批量重命名
来源：http://szb.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fyi.jqgfzy.top

[R75] 导出环境变量
来源：http://qhh.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://ljm.snrcjt.cn

[R76] 使用临时文件
来源：http://wak.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwp.ydzc1.top

[R77] 读取用户输入
来源：http://eao.xuanzx.com

read -rp "请输入: " ans
来源：http://vea.fehbvm.com

[R78] 交互式菜单
来源：http://tgt.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://apu.yangfankeji.com

[R79] 解析命令行选项
来源：http://bbg.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zbc.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://plu.chenzaomai.com

time ./run.sh
来源：http://nve.aizwys.cn

================================================================================
来源：http://hcb.redwolf501.top

S. C / C++ 专题
来源：http://bcr.shanyushiyangtech.top

================================================================================
来源：http://asv.xuetiantiany.cn

[S01] C：Hello World
来源：http://qgs.zhongyouzk.top

#include <stdio.h>
来源：http://fcs.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jsi.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://rnc.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://iyg.hammf.cn

[S03] C：读入整数
来源：http://qrs.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://xaa.chenzaomai.com

[S04] C：字符串复制
来源：http://wwy.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://zqv.gaohongyu789.top

[S05] C：字符串长度
来源：http://epv.52xcode.cn

strlen(s)
来源：http://nme.shzxlz.cn

[S06] C：字符串比较
来源：http://jow.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://rpn.xylfe.cn

[S07] C：数组遍历求和
来源：http://qst.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hsq.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://cfi.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ezc.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://nfa.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mvx.chenzaomai.com

[S10] C：指针与解引用
来源：http://wvo.nwbrower.top

int *p = &a;  *p = 5;
来源：http://xse.yfazqb.com

[S11] C：逐行读文件
来源：http://oct.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://mfe.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ryz.fzhhl.top

fclose(f);
来源：http://run.jqgufenzy.top

[S12] C：写文件
来源：http://ikv.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xnu.nanxuanxn.top

[S13] C：宏定义
来源：http://kvl.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fcq.daria6918.cn

[S14] C：枚举
来源：http://now.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://azp.chenlongwang.top

[S15] C：类型转换
来源：http://zcr.ehwqpu.com

(double) a / b
来源：http://tnx.xylfe.cn

[S16] C：位操作置位
来源：http://esu.aizwys.cn

x |= (1 << 3);
来源：http://zeq.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://agc.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pve.uphjek.com

[S18] C：命令行参数
来源：http://iad.jinqigfzy.top

int main(int argc, char **argv)
来源：http://ofj.fanxiaobao.xyz

[S19] C：快速排序
来源：http://ezs.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://axh.aibaodan.cn

[S20] C：二分查找
来源：http://fee.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mux.zhijiandao.cn

[S21] C：字符类别判断
来源：http://uhy.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lpq.bbcook.cn

[S22] C：字符串转数字
来源：http://ccv.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oyk.ybcxt.top

[S23] C：随机数
来源：http://qlk.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hhf.xziqi.cn

[S24] C：获取本地时间
来源：http://rct.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gxs.sxryk.cn

[S25] C：内存拷贝
来源：http://ftl.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://vns.shangyingyoupin.top

[S26] C：内存清零
来源：http://ojz.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://rmy.fanxiaobao.xyz

[S27] C：定义常量
来源：http://yef.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://yuy.bjfxy.top

[S28] C：静态变量
来源：http://ykb.cashguo.top

static int counter = 0;
来源：http://res.sysykeji.top

[S29] C：变参函数
来源：http://fve.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lox.yanxiufei.cn

[S30] C：头文件保护
来源：http://wku.jqgufenzy.top

#ifndef X_H
来源：http://vbo.shzxlz.cn

#define X_H
来源：http://yxs.cdnleiting.top

#endif
来源：http://hof.cdnleiting.top

[S31] C++：Hello World
来源：http://lhw.fengsongda.top

#include <iostream>
来源：http://dck.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://ust.kuanghao11.cn

[S32] C++：字符串
来源：http://zrh.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://aro.nwbrower.top

[S33] C++：vector 增删
来源：http://fod.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zby.c1oappe.top

[S34] C++：遍历 vector
来源：http://bvq.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://ypj.52xcode.cn

[S35] C++：map
来源：http://ojv.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gpx.chenlongwang.top

[S36] C++：unordered_map
来源：http://hgo.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rag.ybcxt.top

[S37] C++：set
来源：http://cch.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xyt.tanke756.top

[S38] C++：排序
来源：http://mjm.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://qwr.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://srm.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rto.zycfv.cn

[S40] C++：查找元素
来源：http://zqc.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vfg.zycfv.cn

[S41] C++：类与构造函数
来源：http://djk.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://una.bjfxy.top

[S42] C++：继承与虚函数
来源：http://gxr.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://xen.havefunace.top

[S43] C++：智能指针
来源：http://urr.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://cdc.zhiwuduotai.top

[S44] C++：引用传参
来源：http://mtu.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://guz.nwbrower.top

[S45] C++：lambda
来源：http://oen.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://pqv.uphjek.com

[S46] C++：函数模板
来源：http://xnz.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mdz.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://qbe.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qzi.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://uok.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wum.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://obz.vqdsnc.cn

[S49] C++：写文件
来源：http://nza.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sbw.guowangkeji.top

[S50] C++：格式化数字
来源：http://rlc.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kvm.yj202588.top

[S51] C++：显式类型转换
来源：http://nnp.gotoacloud.top

static_cast<double>(a) / b
来源：http://fyj.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://tyu.hesvh.cn

int size() const noexcept { return n_; }
来源：http://nqw.vqdsnc.cn

[S53] C++：移动语义
来源：http://cqw.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://rwx.hcnkem.com

[S54] C++：异常处理
来源：http://qnx.daria6918.cn


<!-- 参考信息 -->