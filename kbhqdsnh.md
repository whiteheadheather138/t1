代发 wailian999

[Q80] 字符串截取
来源：http://cut.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://obu.wangshuangyany.cn

[Q81] 字符串替换
来源：http://zro.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://auy.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://kox.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hdm.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://fdl.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://udm.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://hxi.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://byi.guannengcc.top

[Q85] 数值取整
来源：http://jbd.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bma.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://lof.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xab.sxryk.cn

[Q87] JSON 字段做条件
来源：http://wsb.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://adf.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://dzt.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aes.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://omu.hfpthk.cn

[Q89] 判断表是否存在
来源：http://yoo.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tvo.sjlbkw.cn

[Q90] 生成序号列
来源：http://qyk.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ejo.ydzc1.top

================================================================================
来源：http://gwq.nanxinkj.top

R. Bash 专题
来源：http://jxe.hammf.cn

================================================================================
来源：http://pqq.havefunace.top

[R01] shebang 与严格模式
来源：http://nth.yuxming.cn

#!/usr/bin/env bash
来源：http://zvp.0kj1m.cn

set -euo pipefail
来源：http://qgo.hywenlv.cn

[R02] 变量赋值与使用
来源：http://blu.yongpay.top

name="Tom"; echo "$name"
来源：http://igw.cheryme.top

[R03] 只读变量
来源：http://gkg.fzhhl.top

readonly PI=3.14
来源：http://aph.iojbl.cn

[R04] 位置参数
来源：http://cko.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vdq.smart0.xyz

[R05] 参数默认值
来源：http://rxk.feifeiyinyue.top

name="${1:-default}"
来源：http://qcm.tarul.cn

[R06] 判断命令是否存在
来源：http://jby.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oxu.yanxiufei.cn

[R07] if 判断文件
来源：http://hbt.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sit.wangshuangyany.cn

[R08] 数值比较
来源：http://esa.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://myu.zdbjq.cn

[R09] 字符串比较
来源：http://wxf.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cqn.havefunace.top

[R10] 正则匹配
来源：http://xio.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mdm.aibaodan.cn

[R11] case 多分支
来源：http://obh.shuidangran.top

case "$1" in
来源：http://mbo.hnxiangtu.top

start) echo "启动" ;;
来源：http://bzv.smart0.xyz

stop)  echo "停止" ;;
来源：http://uxy.xziqi.cn

*)     echo "未知命令" ;;
来源：http://phi.vehdjk.com

esac
来源：http://vmd.zdqjudy.top

[R12] for 遍历文件
来源：http://jjd.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://ioq.9152youxi.cn

[R13] for 计数循环
来源：http://vqa.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://uig.zhengqikj.top

[R14] C 风格 for
来源：http://jki.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bfb.hfpthk.cn

[R15] while 逐行读文件
来源：http://ihl.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uit.cqqwz.cn

[R16] until 等待条件
来源：http://pup.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jat.nwbrower.top

[R17] 数组定义与取值
来源：http://fpt.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xaz.jlsjyb.cn

[R18] 遍历数组
来源：http://fxj.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qbe.hcnkem.com

[R19] 数组长度
来源：http://igt.hywenlv.cn

echo "${#arr[@]}"
来源：http://prz.yj20258.top

[R20] 关联数组（字典）
来源：http://nhf.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iwd.uphjek.com

[R21] 字符串长度
来源：http://lrt.daxiang520.top

echo "${#s}"
来源：http://rmi.jinghuilouyu.cn

[R22] 截取子串
来源：http://quj.fzhhl.top

echo "${s:0:5}"
来源：http://bxq.fzhhl.top

[R23] 字符串替换
来源：http://bcu.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jrb.jianghu66.top

[R24] 大小写转换
来源：http://fps.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://opw.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://qfo.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oip.jlsjyb.cn

[R26] 命令替换
来源：http://hkr.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://pty.gzhubu.top

[R27] 算术展开
来源：http://xcm.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://lhv.ivvv.top

[R28] 浮点运算
来源：http://qnj.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://bfq.tian-w.cn

[R29] 定义函数
来源：http://dow.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yso.hnqzz.top

[R30] 函数返回状态码
来源：http://ihk.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://suo.jinyuanbaomall.cn

[R31] 局部变量
来源：http://ohg.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://wvl.hnqzz.top

[R32] 参数个数校验
来源：http://dfq.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ynm.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://ugb.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mfw.bjfxy.top

[R34] 退出时清理
来源：http://ihj.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://bst.guannengcc.top

[R35] 后台执行并等待
来源：http://yjs.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dra.jyoumei.cn

[R36] 并发执行多个任务
来源：http://zcj.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rfk.zdqjudy.top

[R37] 把输出赋给变量
来源：http://rcn.fengsongda.top

files=$(ls -1)
来源：http://wym.guannengcc.top

[R38] 管道串联
来源：http://yew.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://ztt.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://xnk.316326.xyz

cmd > out.log 2>&1
来源：http://qnc.zhengqikj.top

[R40] 追加写日志
来源：http://mdx.fzhhl.top

echo "log" >> out.log
来源：http://gbv.gzhubu.top

[R41] 丢弃输出
来源：http://wdl.nwbrower.top

cmd >/dev/null 2>&1
来源：http://idj.ehwqpu.com

[R42] 输入重定向
来源：http://kjm.zhaomingkeji.xyz

wc -l < a.txt
来源：http://hrb.jqgufenzy.top

[R43] 按名字查找文件
来源：http://ekq.chenlongwang.top

find . -name "*.log" -type f
来源：http://vwm.snrcjt.cn

[R44] 按修改时间查找
来源：http://eui.yj20258888.top

find . -mtime -7 -type f
来源：http://bdu.zhoulong.xyz

[R45] 批量删除
来源：http://jjn.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://kpa.zhengqikj.top

[R46] 递归替换文件内容
来源：http://gjl.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xhk.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://zgq.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vla.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://dbm.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://fbn.quarkkingdee.top

[R49] awk 带条件
来源：http://xbh.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pxf.52xcode.cn

[R50] awk 求和
来源：http://quq.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://jao.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://pgh.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ooa.gotoacloud.top

[R52] 统计行数
来源：http://vsd.ivvv.top

wc -l a.txt
来源：http://nzt.yj202588.top

[R53] 查看文件头与实时尾
来源：http://zwp.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iqu.hammf.cn

[R54] 比较两个文件
来源：http://dlw.jiagoushi.top

diff a.txt b.txt
来源：http://uax.shangyingyoupin.top

[R55] 压缩与解压
来源：http://stj.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zzj.hfpthk.cn

[R56] 远程拷贝
来源：http://hzt.hfpthk.cn

scp file user@host:/path/
来源：http://aqh.zycfv.cn

[R57] 远程执行命令
来源：http://ewb.yueranfly.top

ssh user@host 'uptime'
来源：http://lmr.yj20258.top

[R58] 下载文件
来源：http://lja.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vwd.vehdjk.com

[R59] 发 POST JSON
来源：http://ujg.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lag.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://xjq.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://soq.cashguo.top

[R61] 磁盘占用
来源：http://buy.ctjpmb.com

df -h;  du -sh *
来源：http://gfk.chenlongwang.top

[R62] 找最占空间的文件
来源：http://meb.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://meo.zhixingplan.top

[R63] 内存与进程
来源：http://xzq.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://oob.ctjpmb.com

[R64] 结束进程
来源：http://uyk.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://cui.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://yrh.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ilh.dashuyun.cn

[R66] 定时任务
来源：http://tfh.hcnkem.com

crontab -e;  crontab -l
来源：http://cis.pycfn.com

[R67] 生成随机十六进制串
来源：http://fxc.jyoumei.cn

openssl rand -hex 16
来源：http://kcs.gzhubu.top

[R68] 计算文件校验值
来源：http://bzs.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://jgg.zhixingplan.top

[R69] 生成随机密码
来源：http://jyn.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://bgh.nwbrower.top

[R70] 时间戳与互转
来源：http://qis.ydzc1.top

date +%s;  date -d @1700000000
来源：http://yzw.cheryme.top

[R71] 日期格式化
来源：http://vvw.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uey.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://rsm.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ucx.snrcjt.cn

[R73] 分割大日志
来源：http://fzs.gogol.net.cn

split -l 1000 big.log part_
来源：http://dqs.chenlongwang.top

[R74] 批量重命名
来源：http://par.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rji.cashguo.top

[R75] 导出环境变量
来源：http://czr.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://pml.jyoumei.cn

[R76] 使用临时文件
来源：http://hjb.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vcb.hammf.cn

[R77] 读取用户输入
来源：http://oru.fengsongda.top

read -rp "请输入: " ans
来源：http://apd.yj20258.top

[R78] 交互式菜单
来源：http://moj.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eui.tanke756.top

[R79] 解析命令行选项
来源：http://erl.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tcv.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://rgr.xingfuxueyuan.xyz

time ./run.sh
来源：http://ohj.yj20258888.top

================================================================================
来源：http://kzv.fktsv.cn

S. C / C++ 专题
来源：http://ark.hfpthk.cn

================================================================================
来源：http://ken.gogol.net.cn

[S01] C：Hello World
来源：http://bij.sjlbkw.cn

#include <stdio.h>
来源：http://wtj.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://rmv.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://pjf.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://izl.fanxiaobao.xyz

[S03] C：读入整数
来源：http://lii.hesvh.cn

int x; scanf("%d", &x);
来源：http://eyy.jianghu66.top

[S04] C：字符串复制
来源：http://nyp.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://rxf.hnxiangtu.top

[S05] C：字符串长度
来源：http://mjg.shanyushiyangtech.top

strlen(s)
来源：http://pgj.0kj1m.cn

[S06] C：字符串比较
来源：http://kaq.sjlbkw.cn

strcmp(a, b) == 0
来源：http://ols.fzhhl.top

[S07] C：数组遍历求和
来源：http://gsq.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://thv.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://dhh.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qvr.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://evj.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dvk.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://wkm.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://sax.gotoacloud.top

[S11] C：逐行读文件
来源：http://jtp.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://azs.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ioj.hesvh.cn

fclose(f);
来源：http://dgo.jinghuilouyu.cn

[S12] C：写文件
来源：http://xqt.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mtz.xuetiantiany.cn

[S13] C：宏定义
来源：http://mby.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vja.tarul.cn

[S14] C：枚举
来源：http://tzr.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://qdo.pengpengdd.cyou

[S15] C：类型转换
来源：http://eiz.svipenyu.cn

(double) a / b
来源：http://hbt.jinqigfzy.top

[S16] C：位操作置位
来源：http://jvf.iojbl.cn

x |= (1 << 3);
来源：http://xju.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://hjj.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bim.yj20258.top

[S18] C：命令行参数
来源：http://wja.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://iou.pengpengdd.cyou

[S19] C：快速排序
来源：http://hyw.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://axv.xinyue.icu

[S20] C：二分查找
来源：http://xgg.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qgc.zdbjq.cn

[S21] C：字符类别判断
来源：http://ohk.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ypl.fzhhl.top

[S22] C：字符串转数字
来源：http://cqc.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://sbw.daria6918.cn

[S23] C：随机数
来源：http://ftp.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ykc.yfazqb.com

[S24] C：获取本地时间
来源：http://ywg.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lso.xuanzx.com

[S25] C：内存拷贝
来源：http://xcz.xylfe.cn

memcpy(dst, src, n);
来源：http://uip.yongpay.top

[S26] C：内存清零
来源：http://fkl.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://nwk.fehbvm.com

[S27] C：定义常量
来源：http://tyj.dashuyun.cn

const double PI = 3.14159;
来源：http://aty.pengpengdd.cyou

[S28] C：静态变量
来源：http://xwx.jinghuilouyu.cn

static int counter = 0;
来源：http://mxl.daxiang520.top

[S29] C：变参函数
来源：http://vhq.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cxi.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://fuw.cdnleiting.top

#ifndef X_H
来源：http://fma.ydzc1.top

#define X_H
来源：http://zar.mhx1999.top

#endif
来源：http://khv.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://ejr.ehwqpu.com

#include <iostream>
来源：http://gtg.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://otr.shanyushiyangtech.top

[S32] C++：字符串
来源：http://yhw.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://zon.chenlongwang.top

[S33] C++：vector 增删
来源：http://uke.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ipr.shzxlz.cn

[S34] C++：遍历 vector
来源：http://fph.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://qga.ctjpmb.com

[S35] C++：map
来源：http://pcq.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://owx.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://nhp.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nfd.yongpay.top

[S37] C++：set
来源：http://axy.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nch.fzhhl.top

[S38] C++：排序
来源：http://opi.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://teb.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://acs.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blt.hammf.cn

[S40] C++：查找元素
来源：http://ubx.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxe.xylfe.cn

[S41] C++：类与构造函数
来源：http://kxr.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kpl.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://lkt.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://nwc.yonumen.top

[S43] C++：智能指针
来源：http://afc.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://rjs.c1oappe.top

[S44] C++：引用传参
来源：http://bcu.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://hdm.guowangkeji.top

[S45] C++：lambda
来源：http://sgo.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lrp.cucudq.cn

[S46] C++：函数模板
来源：http://vbp.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hap.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://vzn.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blm.haohaochexian.top

[S48] C++：逐行读文件
来源：http://oas.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xty.tarul.cn

while (std::getline(in, line)) { }
来源：http://bvn.yanxiufei.cn

[S49] C++：写文件
来源：http://iuy.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljo.gogol.net.cn

[S50] C++：格式化数字
来源：http://seb.cqqwz.cn


<!-- 参考信息 -->