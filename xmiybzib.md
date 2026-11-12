代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uwj.wangdashe.top

[Q75] 日期格式化
来源：http://dsc.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fox.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://leq.jyoumei.cn

[Q76] 按天统计
来源：http://rtc.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fvm.xuanzx.com

[Q77] 时间加减
来源：http://wqv.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cxt.zdqjudy.top

[Q78] 当前时间
来源：http://mqn.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wod.jqgfzy.top

[Q79] 字符串拼接
来源：http://cok.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oxx.xuetiantiany.cn

[Q80] 字符串截取
来源：http://gwl.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bls.yfazqb.com

[Q81] 字符串替换
来源：http://sho.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bjh.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://dbg.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bcb.ydjk.org.cn

[Q83] 大小写转换
来源：http://idf.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ilr.cucudq.cn

[Q84] 去除首尾空格
来源：http://abb.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://aha.zycfv.cn

[Q85] 数值取整
来源：http://bqc.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dyz.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://zrm.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kog.fehbvm.com

[Q87] JSON 字段做条件
来源：http://omt.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ttm.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://pbs.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://feg.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://thw.birdmap.top

[Q89] 判断表是否存在
来源：http://jnm.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bqb.snrcjt.cn

[Q90] 生成序号列
来源：http://bpq.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xes.dashuyun.cn

================================================================================
来源：http://lqc.snrcjt.cn

R. Bash 专题
来源：http://hlx.vqdsnc.cn

================================================================================
来源：http://ndd.wangdashe.top

[R01] shebang 与严格模式
来源：http://pqa.sxryk.cn

#!/usr/bin/env bash
来源：http://umz.xinyue.icu

set -euo pipefail
来源：http://yps.c1oappe.top

[R02] 变量赋值与使用
来源：http://tam.sufxvd.cn

name="Tom"; echo "$name"
来源：http://ezo.vehdjk.com

[R03] 只读变量
来源：http://uwk.jianghu66.top

readonly PI=3.14
来源：http://zwk.ivvv.top

[R04] 位置参数
来源：http://vzt.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jva.sjlbkw.cn

[R05] 参数默认值
来源：http://mtj.ivvv.top

name="${1:-default}"
来源：http://gai.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://wxt.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eni.hongshengwenyu.top

[R07] if 判断文件
来源：http://tbu.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wmw.ivvv.top

[R08] 数值比较
来源：http://luw.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xcy.zhixingplan.top

[R09] 字符串比较
来源：http://rlt.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kna.nanxuanxn.top

[R10] 正则匹配
来源：http://cgl.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zag.shuidangran.top

[R11] case 多分支
来源：http://wjw.vqdsnc.cn

case "$1" in
来源：http://ppi.hysaishi.cn

start) echo "启动" ;;
来源：http://bmh.redwolf501.top

stop)  echo "停止" ;;
来源：http://zje.wangdashe.top

*)     echo "未知命令" ;;
来源：http://oyf.fzhhl.top

esac
来源：http://buk.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://dgc.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://xob.yangfankeji.com

[R13] for 计数循环
来源：http://atx.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://aky.jlsjyb.cn

[R14] C 风格 for
来源：http://zvm.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rar.zhoulong.xyz

[R15] while 逐行读文件
来源：http://ogt.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vla.shzxlz.cn

[R16] until 等待条件
来源：http://uvm.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rwu.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://xfr.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sdy.yj20258888.top

[R18] 遍历数组
来源：http://vct.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ccf.andypj.xyz

[R19] 数组长度
来源：http://tar.pycfn.com

echo "${#arr[@]}"
来源：http://gud.fehbvm.com

[R20] 关联数组（字典）
来源：http://aio.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tqb.gogol.net.cn

[R21] 字符串长度
来源：http://ynv.cucudq.cn

echo "${#s}"
来源：http://nld.shangyingyoupin.top

[R22] 截取子串
来源：http://dgn.hysaishi.cn

echo "${s:0:5}"
来源：http://vmw.nanxuanxn.top

[R23] 字符串替换
来源：http://dhe.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cnf.jiagoushi.top

[R24] 大小写转换
来源：http://gri.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vyy.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://kpp.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eyu.wangdashe.top

[R26] 命令替换
来源：http://klu.yj202588.top

now=$(date +%F); echo "$now"
来源：http://xer.gotoacloud.top

[R27] 算术展开
来源：http://ujq.meibo888.top

echo $((1 + 2 * 3))
来源：http://vgg.jinghuilouyu.cn

[R28] 浮点运算
来源：http://ccu.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://hwh.guannengcc.top

[R29] 定义函数
来源：http://vvo.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jkd.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://uej.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://pxl.ivvv.top

[R31] 局部变量
来源：http://oaj.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://hmi.nanxuanxn.top

[R32] 参数个数校验
来源：http://mwn.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zrf.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://vkr.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ewb.xuanzx.com

[R34] 退出时清理
来源：http://nsa.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kwq.xziqi.cn

[R35] 后台执行并等待
来源：http://tzr.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mlz.aibaodan.cn

[R36] 并发执行多个任务
来源：http://lge.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zng.yvedp.cn

[R37] 把输出赋给变量
来源：http://fvb.yj20258888.top

files=$(ls -1)
来源：http://qhr.cdnleiting.top

[R38] 管道串联
来源：http://sth.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://lpn.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://jlx.cqqwz.cn

cmd > out.log 2>&1
来源：http://fem.bbcook.cn

[R40] 追加写日志
来源：http://psa.yangfankeji.com

echo "log" >> out.log
来源：http://pmh.yonumen.top

[R41] 丢弃输出
来源：http://mqc.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://ftw.dashuyun.cn

[R42] 输入重定向
来源：http://tzy.yj20258888.top

wc -l < a.txt
来源：http://lrs.jyoumei.cn

[R43] 按名字查找文件
来源：http://lqq.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://kww.smart0.xyz

[R44] 按修改时间查找
来源：http://jqb.shzxlz.cn

find . -mtime -7 -type f
来源：http://kdi.52xcode.cn

[R45] 批量删除
来源：http://vdm.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://tie.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://bmw.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pew.chenzaomai.com

[R47] sed 单行替换
来源：http://mju.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://dxj.zycfv.cn

[R48] awk 取指定列
来源：http://tka.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://fen.hongshengwenyu.top

[R49] awk 带条件
来源：http://bpk.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kud.zhongyouzk.top

[R50] awk 求和
来源：http://uhh.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://peb.zhixingplan.top

[R51] 排序去重取前几
来源：http://rng.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fhs.sweek.top

[R52] 统计行数
来源：http://fjb.cheryme.top

wc -l a.txt
来源：http://otz.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://qbi.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ivg.yfazqb.com

[R54] 比较两个文件
来源：http://usy.yj20258888.top

diff a.txt b.txt
来源：http://gbk.sysykeji.top

[R55] 压缩与解压
来源：http://dmi.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vds.zhixingplan.top

[R56] 远程拷贝
来源：http://shq.vehdjk.com

scp file user@host:/path/
来源：http://qbk.yuxming.cn

[R57] 远程执行命令
来源：http://oup.yj202588.top

ssh user@host 'uptime'
来源：http://zxc.ywan-chungtsiang.top

[R58] 下载文件
来源：http://ama.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cui.yongpay.top

[R59] 发 POST JSON
来源：http://uvl.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://clc.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://pkg.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kvz.svipenyu.cn

[R61] 磁盘占用
来源：http://ruv.shangyingyoupin.top

df -h;  du -sh *
来源：http://ljm.meibo888.top

[R62] 找最占空间的文件
来源：http://zsk.yj20258.top

du -ah . | sort -rh | head -10
来源：http://xkq.chenjidiqi.icu

[R63] 内存与进程
来源：http://fzk.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://ddu.gaohongyu789.top

[R64] 结束进程
来源：http://lsm.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://qer.zdqjudy.top

[R65] 查看端口占用
来源：http://zbj.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfp.sufxvd.cn

[R66] 定时任务
来源：http://eal.xuanzx.com

crontab -e;  crontab -l
来源：http://smd.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://xci.shzxlz.cn

openssl rand -hex 16
来源：http://fol.daxiang520.top

[R68] 计算文件校验值
来源：http://njb.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ycu.9152youxi.cn

[R69] 生成随机密码
来源：http://wls.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://cpv.cucudq.cn

[R70] 时间戳与互转
来源：http://pkn.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://dye.aizwys.cn

[R71] 日期格式化
来源：http://ily.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://stz.aizwys.cn

[R72] 等待端口就绪
来源：http://emd.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zyw.yj202588.top

[R73] 分割大日志
来源：http://zui.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://ukz.jqgufenzy.top

[R74] 批量重命名
来源：http://twe.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xcj.nanxuanxn.top

[R75] 导出环境变量
来源：http://jrr.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://afu.fktsv.cn

[R76] 使用临时文件
来源：http://nzt.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://szd.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://iol.fengsongda.top

read -rp "请输入: " ans
来源：http://per.yuanzhike.top

[R78] 交互式菜单
来源：http://orl.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pdx.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://gqx.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sns.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://kgo.ctjpmb.com

time ./run.sh
来源：http://jdb.xuanzx.com

================================================================================
来源：http://hka.fengsongda.top

S. C / C++ 专题
来源：http://aua.yj202588.top

================================================================================
来源：http://kbm.yvedp.cn

[S01] C：Hello World
来源：http://gmz.gaohongyu789.top

#include <stdio.h>
来源：http://pnx.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://sop.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://gtg.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://nap.yfazqb.com

[S03] C：读入整数
来源：http://tgx.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://pip.yvedp.cn

[S04] C：字符串复制
来源：http://hzh.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hfj.chenjidiqi.icu

[S05] C：字符串长度
来源：http://vdb.yonumen.top

strlen(s)
来源：http://npf.sjlbkw.cn

[S06] C：字符串比较
来源：http://als.quarkkingdee.top

strcmp(a, b) == 0
来源：http://yvv.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://cub.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kkj.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://oze.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aja.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://wub.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vmd.sysykeji.top

[S10] C：指针与解引用
来源：http://nqx.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://tvp.chenlongwang.top

[S11] C：逐行读文件
来源：http://cgb.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://wjb.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://cip.wangshuangyany.cn

fclose(f);
来源：http://lvv.ydjk.org.cn

[S12] C：写文件
来源：http://pvm.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sze.yanxiufei.cn

[S13] C：宏定义
来源：http://wwu.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dcx.yuanzhike.top

[S14] C：枚举
来源：http://qtw.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://rzb.0kj1m.cn

[S15] C：类型转换
来源：http://fha.shzxlz.cn

(double) a / b
来源：http://yxo.nwbrower.top

[S16] C：位操作置位
来源：http://ejc.tianlin.xyz

x |= (1 << 3);
来源：http://ubd.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://izr.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nus.ybcxt.top

[S18] C：命令行参数
来源：http://pog.zycfv.cn

int main(int argc, char **argv)
来源：http://ykr.zhiwuduotai.top

[S19] C：快速排序
来源：http://vhq.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rvt.cdnleiting.top

[S20] C：二分查找
来源：http://aen.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xrl.hesvh.cn

[S21] C：字符类别判断
来源：http://wyo.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ymt.yonumen.top

[S22] C：字符串转数字
来源：http://dkj.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zix.9152youxi.cn

[S23] C：随机数
来源：http://nmq.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yuz.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://htj.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hzs.ctjpmb.com

[S25] C：内存拷贝
来源：http://ouq.jianghu66.top

memcpy(dst, src, n);
来源：http://njp.yj20258888.top

[S26] C：内存清零
来源：http://ixs.havefunace.top

memset(a, 0, sizeof a);
来源：http://nxo.nwbrower.top

[S27] C：定义常量
来源：http://jin.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://ypx.uphjek.com

[S28] C：静态变量
来源：http://jnd.dianchejie.cn

static int counter = 0;
来源：http://mbc.vehdjk.com

[S29] C：变参函数
来源：http://tno.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lcp.jqgfzy.top

[S30] C：头文件保护
来源：http://zgs.aibaodan.cn

#ifndef X_H
来源：http://rhe.zhongyouzk.top

#define X_H
来源：http://ztn.cqqwz.cn

#endif
来源：http://luc.jyoumei.cn

[S31] C++：Hello World
来源：http://neq.yj20258888.top

#include <iostream>
来源：http://ect.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://ueq.hammf.cn

[S32] C++：字符串
来源：http://inp.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://csu.redwolf501.top

[S33] C++：vector 增删
来源：http://abf.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://esm.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://mtt.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ptq.yfazqb.com

[S35] C++：map
来源：http://nus.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iuj.wangdashe.top

[S36] C++：unordered_map
来源：http://tfm.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nub.wangdashe.top

[S37] C++：set
来源：http://dqf.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ltn.ehwqpu.com

[S38] C++：排序
来源：http://wbs.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://hof.meibo888.top

[S39] C++：自定义比较器排序
来源：http://nfn.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gub.sxryk.cn

[S40] C++：查找元素
来源：http://gnw.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sxu.hfpthk.cn

[S41] C++：类与构造函数
来源：http://mge.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vii.andypj.xyz

[S42] C++：继承与虚函数
来源：http://rub.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://fla.yuxming.cn

[S43] C++：智能指针
来源：http://kbl.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://nwk.daria6918.cn

[S44] C++：引用传参
来源：http://wxf.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://nlt.iojbl.cn


<!-- 参考信息 -->