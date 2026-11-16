代发 wailian999

[Q76] 按天统计
来源：http://nsz.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kwk.sufxvd.cn

[Q77] 时间加减
来源：http://zsg.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cvt.bbcook.cn

[Q78] 当前时间
来源：http://ctk.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://esa.jqgufenzy.top

[Q79] 字符串拼接
来源：http://oso.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bmm.jinqigfzy.top

[Q80] 字符串截取
来源：http://bvv.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wbo.fengsongda.top

[Q81] 字符串替换
来源：http://yqy.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://efd.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://fzn.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ixz.xuanzx.com

[Q83] 大小写转换
来源：http://tbp.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmf.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://vvn.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://mbu.ivvv.top

[Q85] 数值取整
来源：http://fwz.fehbvm.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tbo.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://pal.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ape.hnqzz.top

[Q87] JSON 字段做条件
来源：http://nkw.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jgv.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://pap.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://siy.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://agi.mhx1999.top

[Q89] 判断表是否存在
来源：http://hyz.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vjl.zhiwuduotai.top

[Q90] 生成序号列
来源：http://qlm.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kfq.guannengcc.top

================================================================================
来源：http://hea.yongpay.top

R. Bash 专题
来源：http://idu.yj20258888.top

================================================================================
来源：http://zzj.52xcode.cn

[R01] shebang 与严格模式
来源：http://qlf.birdmap.top

#!/usr/bin/env bash
来源：http://vzn.shzxlz.cn

set -euo pipefail
来源：http://fcx.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://xcs.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://jpd.wangshuangyany.cn

[R03] 只读变量
来源：http://dio.bjfxy.top

readonly PI=3.14
来源：http://efb.jinqigufen.top

[R04] 位置参数
来源：http://yyz.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://imr.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://wge.chenjidiqi.icu

name="${1:-default}"
来源：http://gqv.ivvv.top

[R06] 判断命令是否存在
来源：http://qjb.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ubi.nanxuanxn.top

[R07] if 判断文件
来源：http://usk.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ddd.hnxiangtu.top

[R08] 数值比较
来源：http://yyl.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gzq.tanke756.top

[R09] 字符串比较
来源：http://znv.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yom.meibo888.top

[R10] 正则匹配
来源：http://cbn.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dmu.zhengqikj.top

[R11] case 多分支
来源：http://bcg.bjfxy.top

case "$1" in
来源：http://hut.zhengqikj.top

start) echo "启动" ;;
来源：http://fmh.316326.xyz

stop)  echo "停止" ;;
来源：http://rln.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://uoa.cucudq.cn

esac
来源：http://jba.quarkkingdee.top

[R12] for 遍历文件
来源：http://nox.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://cmi.sjlbkw.cn

[R13] for 计数循环
来源：http://cxa.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://fep.fengsongda.top

[R14] C 风格 for
来源：http://qnc.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rsa.jinqigfzy.top

[R15] while 逐行读文件
来源：http://mmg.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zka.fehbvm.com

[R16] until 等待条件
来源：http://uqc.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sll.xinyue.icu

[R17] 数组定义与取值
来源：http://tra.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://rqu.wangdashe.top

[R18] 遍历数组
来源：http://wur.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jdj.sufxvd.cn

[R19] 数组长度
来源：http://gmf.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://ueb.chenzaomai.com

[R20] 关联数组（字典）
来源：http://tgz.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mlr.tarul.cn

[R21] 字符串长度
来源：http://fvf.cucudq.cn

echo "${#s}"
来源：http://mfz.gzhubu.top

[R22] 截取子串
来源：http://qys.nwbrower.top

echo "${s:0:5}"
来源：http://awy.gotoacloud.top

[R23] 字符串替换
来源：http://xlx.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cqy.zhongyouzk.top

[R24] 大小写转换
来源：http://wbm.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dyy.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://ego.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://otq.yj20258888.top

[R26] 命令替换
来源：http://ena.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://gmu.chenjidiqi.icu

[R27] 算术展开
来源：http://dbo.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://jag.yangfankeji.com

[R28] 浮点运算
来源：http://cmz.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://bjn.wangshuangyany.cn

[R29] 定义函数
来源：http://hfq.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ryu.tianlin.xyz

[R30] 函数返回状态码
来源：http://irc.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://kzt.jinyuanbaomall.cn

[R31] 局部变量
来源：http://sba.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://kiu.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://qjy.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wnt.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://scg.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://irm.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://siq.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ktf.tanke756.top

[R35] 后台执行并等待
来源：http://dpc.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lyx.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://fct.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wqi.mhx1999.top

[R37] 把输出赋给变量
来源：http://nkl.quarkkingdee.top

files=$(ls -1)
来源：http://whb.hammf.cn

[R38] 管道串联
来源：http://giq.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://xze.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://bct.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://fgx.ctjpmb.com

[R40] 追加写日志
来源：http://nkf.ctjpmb.com

echo "log" >> out.log
来源：http://isg.fzhhl.top

[R41] 丢弃输出
来源：http://vvd.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://qki.hysaishi.cn

[R42] 输入重定向
来源：http://uto.ydzc1.top

wc -l < a.txt
来源：http://bwj.ydjk.org.cn

[R43] 按名字查找文件
来源：http://giu.tanke756.top

find . -name "*.log" -type f
来源：http://yyo.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://uyo.quarkkingdee.top

find . -mtime -7 -type f
来源：http://uja.sxryk.cn

[R45] 批量删除
来源：http://hzt.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://tmw.cucudq.cn

[R46] 递归替换文件内容
来源：http://lwa.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbg.yanxiufei.cn

[R47] sed 单行替换
来源：http://zgw.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xst.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://kcu.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://btu.cqqwz.cn

[R49] awk 带条件
来源：http://qhn.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zud.chenzaomai.com

[R50] awk 求和
来源：http://wpu.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pmi.hysaishi.cn

[R51] 排序去重取前几
来源：http://hyz.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://nnc.dashuyun.cn

[R52] 统计行数
来源：http://whg.nanxuanxn.top

wc -l a.txt
来源：http://agz.hammf.cn

[R53] 查看文件头与实时尾
来源：http://bbc.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajx.guannengcc.top

[R54] 比较两个文件
来源：http://yti.cucudq.cn

diff a.txt b.txt
来源：http://xhr.xylfe.cn

[R55] 压缩与解压
来源：http://lpt.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qoq.redwolf501.top

[R56] 远程拷贝
来源：http://cyd.yj202588.top

scp file user@host:/path/
来源：http://wfl.yj20258888.top

[R57] 远程执行命令
来源：http://ulx.sjlbkw.cn

ssh user@host 'uptime'
来源：http://zxw.cdnleiting.top

[R58] 下载文件
来源：http://omm.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mfw.vehdjk.com

[R59] 发 POST JSON
来源：http://pjj.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srr.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://opc.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bte.hnqzz.top

[R61] 磁盘占用
来源：http://uvp.jiagoushi.top

df -h;  du -sh *
来源：http://hnz.guowangkeji.top

[R62] 找最占空间的文件
来源：http://qqm.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://wrp.ehwqpu.com

[R63] 内存与进程
来源：http://lta.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://aqw.chenjidiqi.icu

[R64] 结束进程
来源：http://flj.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://tcn.sweek.top

[R65] 查看端口占用
来源：http://yvt.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rph.redwolf501.top

[R66] 定时任务
来源：http://aiu.yuxming.cn

crontab -e;  crontab -l
来源：http://qpv.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://kyu.tianlin.xyz

openssl rand -hex 16
来源：http://xrb.chenzaomai.com

[R68] 计算文件校验值
来源：http://hwg.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://srm.nanxuanxn.top

[R69] 生成随机密码
来源：http://bxf.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://uam.tarul.cn

[R70] 时间戳与互转
来源：http://qoe.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://nrn.wangshuangyany.cn

[R71] 日期格式化
来源：http://wtc.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yun.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://mhs.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://hyc.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://cwf.mhx1999.top

split -l 1000 big.log part_
来源：http://lbh.smart0.xyz

[R74] 批量重命名
来源：http://fex.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qfo.quarkkingdee.top

[R75] 导出环境变量
来源：http://eji.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://aid.yj20258.top

[R76] 使用临时文件
来源：http://glb.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qio.zhongyouzk.top

[R77] 读取用户输入
来源：http://dom.tianlin.xyz

read -rp "请输入: " ans
来源：http://hnx.snrcjt.cn

[R78] 交互式菜单
来源：http://zef.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nie.sxryk.cn

[R79] 解析命令行选项
来源：http://dcn.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://afa.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://gca.kuanghao11.cn

time ./run.sh
来源：http://tmr.ppjwa.cn

================================================================================
来源：http://tjy.tarul.cn

S. C / C++ 专题
来源：http://cjl.jqgfzy.top

================================================================================
来源：http://btm.zycfv.cn

[S01] C：Hello World
来源：http://nyj.jlsjyb.cn

#include <stdio.h>
来源：http://zbb.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://slb.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://iyl.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://sjm.yonumen.top

[S03] C：读入整数
来源：http://ddo.yongpay.top

int x; scanf("%d", &x);
来源：http://mit.zhengqikj.top

[S04] C：字符串复制
来源：http://khi.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wxd.wangshuangyany.cn

[S05] C：字符串长度
来源：http://tvz.yongpay.top

strlen(s)
来源：http://xxk.hesvh.cn

[S06] C：字符串比较
来源：http://uma.jlsjyb.cn

strcmp(a, b) == 0
来源：http://nke.ehwqpu.com

[S07] C：数组遍历求和
来源：http://ats.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ndo.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://fdp.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqu.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://vuw.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdp.gzhubu.top

[S10] C：指针与解引用
来源：http://dtv.yfazqb.com

int *p = &a;  *p = 5;
来源：http://now.fktsv.cn

[S11] C：逐行读文件
来源：http://iax.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://ilq.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovw.shzxlz.cn

fclose(f);
来源：http://cra.zhixingplan.top

[S12] C：写文件
来源：http://pum.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gty.smart0.xyz

[S13] C：宏定义
来源：http://wqt.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pwx.kuanghao11.cn

[S14] C：枚举
来源：http://bvs.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://tlm.tianlin.xyz

[S15] C：类型转换
来源：http://dkg.sufxvd.cn

(double) a / b
来源：http://zaz.hywenlv.cn

[S16] C：位操作置位
来源：http://qjt.jyoumei.cn

x |= (1 << 3);
来源：http://jdi.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://xuq.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gfm.pengpengdd.cyou

[S18] C：命令行参数
来源：http://ewm.xziqi.cn

int main(int argc, char **argv)
来源：http://vjr.gogol.net.cn

[S19] C：快速排序
来源：http://tfj.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://wva.hysaishi.cn

[S20] C：二分查找
来源：http://hag.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gfl.jiagoushi.top

[S21] C：字符类别判断
来源：http://vcn.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yxq.nanxuanxn.top

[S22] C：字符串转数字
来源：http://awy.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tpx.yanxiufei.cn

[S23] C：随机数
来源：http://sxr.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vtw.bjfxy.top

[S24] C：获取本地时间
来源：http://xou.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aiw.yonumen.top

[S25] C：内存拷贝
来源：http://vve.daria6918.cn

memcpy(dst, src, n);
来源：http://ahy.havefunace.top

[S26] C：内存清零
来源：http://bpt.hesvh.cn

memset(a, 0, sizeof a);
来源：http://nzz.shuidangran.top

[S27] C：定义常量
来源：http://xgp.yj202588.top

const double PI = 3.14159;
来源：http://awa.shuidangran.top

[S28] C：静态变量
来源：http://rrj.sweek.top

static int counter = 0;
来源：http://okp.hammf.cn

[S29] C：变参函数
来源：http://pbj.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tkp.hesvh.cn

[S30] C：头文件保护
来源：http://qzy.epnwcf.com

#ifndef X_H
来源：http://bdk.zdbjq.cn

#define X_H
来源：http://vch.jiagoushi.top

#endif
来源：http://exl.ivvv.top

[S31] C++：Hello World
来源：http://vlq.cashguo.top

#include <iostream>
来源：http://ffa.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://jcd.ivvv.top

[S32] C++：字符串
来源：http://him.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://qoa.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://jui.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://edy.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://whr.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://jxk.fengsongda.top

[S35] C++：map
来源：http://acv.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gpx.hesvh.cn

[S36] C++：unordered_map
来源：http://olk.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ivl.cashguo.top

[S37] C++：set
来源：http://itz.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jaw.nanxinkj.top

[S38] C++：排序
来源：http://zqn.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://jfp.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://kii.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cet.bbcook.cn

[S40] C++：查找元素
来源：http://zmd.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iup.jianghu66.top

[S41] C++：类与构造函数
来源：http://zya.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vae.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://dwu.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://xfd.uphjek.com

[S43] C++：智能指针
来源：http://aqn.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://owc.zhiwuduotai.top

[S44] C++：引用传参
来源：http://ydu.yfazqb.com

void inc(int &x) { ++x; }
来源：http://lpu.ivvv.top

[S45] C++：lambda
来源：http://ypl.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yvu.bjfxy.top

[S46] C++：函数模板
来源：http://drp.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zmw.gogol.net.cn


<!-- 参考信息 -->