代发 wailian999

ANALYZE TABLE users;
来源：http://jpe.ybcxt.top

[Q71] 查看建表语句
来源：http://fps.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ivg.meibo888.top

[Q72] 查看索引
来源：http://ipu.wangdashe.top

SHOW INDEX FROM users;
来源：http://gxo.yj20258888.top

[Q73] 查看表状态
来源：http://rhi.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bgc.fzhhl.top

[Q74] 强制使用索引
来源：http://uns.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pir.aizwys.cn

[Q75] 日期格式化
来源：http://bcc.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://edl.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qes.mhx1999.top

[Q76] 按天统计
来源：http://jfu.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijt.aizwys.cn

[Q77] 时间加减
来源：http://qqk.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whl.iojbl.cn

[Q78] 当前时间
来源：http://hyr.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hnq.fengsongda.top

[Q79] 字符串拼接
来源：http://qoq.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qsa.ydzc1.top

[Q80] 字符串截取
来源：http://uth.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lci.hywenlv.cn

[Q81] 字符串替换
来源：http://bxz.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lzc.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://cdw.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yvh.sufxvd.cn

[Q83] 大小写转换
来源：http://wdo.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ipi.tarul.cn

[Q84] 去除首尾空格
来源：http://jqv.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://znk.jyoumei.cn

[Q85] 数值取整
来源：http://cra.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yji.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://wmx.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gzm.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://ery.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://otm.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://esj.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kud.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eab.tarul.cn

[Q89] 判断表是否存在
来源：http://fin.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dwn.xuetiantiany.cn

[Q90] 生成序号列
来源：http://lyd.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgj.fanxiaobao.xyz

================================================================================
来源：http://ljh.uphjek.com

R. Bash 专题
来源：http://kfv.jlsjyb.cn

================================================================================
来源：http://qag.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://gya.iojbl.cn

#!/usr/bin/env bash
来源：http://fkk.gaohongyu789.top

set -euo pipefail
来源：http://qqy.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ftz.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://eyt.shanyushiyangtech.top

[R03] 只读变量
来源：http://ljf.vqdsnc.cn

readonly PI=3.14
来源：http://rlj.mhx1999.top

[R04] 位置参数
来源：http://tmd.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dkf.jianghu66.top

[R05] 参数默认值
来源：http://djj.yueranfly.top

name="${1:-default}"
来源：http://idt.ybcxt.top

[R06] 判断命令是否存在
来源：http://dyb.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fbr.fengsongda.top

[R07] if 判断文件
来源：http://qyu.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://itk.jinqigfzy.top

[R08] 数值比较
来源：http://ttl.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ncc.ehwqpu.com

[R09] 字符串比较
来源：http://quo.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fxl.yanxiufei.cn

[R10] 正则匹配
来源：http://fxo.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gsf.wangshuangyany.cn

[R11] case 多分支
来源：http://ppm.fanxiaobao.xyz

case "$1" in
来源：http://mns.hcnkem.com

start) echo "启动" ;;
来源：http://fkj.daxiang520.top

stop)  echo "停止" ;;
来源：http://jdy.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://duy.feifeiyinyue.top

esac
来源：http://fub.cucudq.cn

[R12] for 遍历文件
来源：http://xrp.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://oio.hcnkem.com

[R13] for 计数循环
来源：http://eyi.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://tsy.vehdjk.com

[R14] C 风格 for
来源：http://gwz.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nuz.tanke756.top

[R15] while 逐行读文件
来源：http://yuz.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ukh.jinqigfzy.top

[R16] until 等待条件
来源：http://tqi.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dwv.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://hcs.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cfx.kuanghao11.cn

[R18] 遍历数组
来源：http://tqc.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rll.gotoacloud.top

[R19] 数组长度
来源：http://phb.aizwys.cn

echo "${#arr[@]}"
来源：http://cgd.daria6918.cn

[R20] 关联数组（字典）
来源：http://rcn.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rhw.tanke756.top

[R21] 字符串长度
来源：http://zye.dianchejie.cn

echo "${#s}"
来源：http://dcj.zycfv.cn

[R22] 截取子串
来源：http://ugz.zdqjudy.top

echo "${s:0:5}"
来源：http://scd.guowangkeji.top

[R23] 字符串替换
来源：http://myl.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fig.fanxiaobao.xyz

[R24] 大小写转换
来源：http://pui.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://qgo.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://zcd.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ojf.cashguo.top

[R26] 命令替换
来源：http://ykw.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://oyk.zdbjq.cn

[R27] 算术展开
来源：http://jtv.andypj.xyz

echo $((1 + 2 * 3))
来源：http://aog.tanke756.top

[R28] 浮点运算
来源：http://mkh.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://shl.jyoumei.cn

[R29] 定义函数
来源：http://lba.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://loz.shuidangran.top

[R30] 函数返回状态码
来源：http://cfr.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://cxz.gaohongyu789.top

[R31] 局部变量
来源：http://buu.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://mvc.cashguo.top

[R32] 参数个数校验
来源：http://gkf.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ezp.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://mws.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qbq.ydjk.org.cn

[R34] 退出时清理
来源：http://trd.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://nrr.hfpthk.cn

[R35] 后台执行并等待
来源：http://qrs.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://row.chenzaomai.com

[R36] 并发执行多个任务
来源：http://ter.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wai.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://pya.yongpay.top

files=$(ls -1)
来源：http://vau.chenjidiqi.icu

[R38] 管道串联
来源：http://ege.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://vwj.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://lzi.chenlongwang.top

cmd > out.log 2>&1
来源：http://jbl.yueranfly.top

[R40] 追加写日志
来源：http://spa.yongpay.top

echo "log" >> out.log
来源：http://gmk.xylfe.cn

[R41] 丢弃输出
来源：http://fps.yvedp.cn

cmd >/dev/null 2>&1
来源：http://wkk.feifeiyinyue.top

[R42] 输入重定向
来源：http://czg.jqgufenzy.top

wc -l < a.txt
来源：http://ryd.0kj1m.cn

[R43] 按名字查找文件
来源：http://kbe.chenzaomai.com

find . -name "*.log" -type f
来源：http://egr.ppjwa.cn

[R44] 按修改时间查找
来源：http://pgx.hesvh.cn

find . -mtime -7 -type f
来源：http://fva.dashuyun.cn

[R45] 批量删除
来源：http://jaw.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://vtc.smart0.xyz

[R46] 递归替换文件内容
来源：http://gwn.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xzs.hongshengwenyu.top

[R47] sed 单行替换
来源：http://gtx.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hhf.svipenyu.cn

[R48] awk 取指定列
来源：http://obm.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://nxl.kuanghao11.cn

[R49] awk 带条件
来源：http://jpc.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://etz.snrcjt.cn

[R50] awk 求和
来源：http://tyv.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://ksu.sweek.top

[R51] 排序去重取前几
来源：http://uog.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mvb.ydjk.org.cn

[R52] 统计行数
来源：http://ebs.haohaochexian.top

wc -l a.txt
来源：http://wno.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://qne.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jes.fzhhl.top

[R54] 比较两个文件
来源：http://zrc.daxiang520.top

diff a.txt b.txt
来源：http://wsw.snrcjt.cn

[R55] 压缩与解压
来源：http://lqa.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yoa.yvedp.cn

[R56] 远程拷贝
来源：http://lbl.hysaishi.cn

scp file user@host:/path/
来源：http://cmf.yanxiufei.cn

[R57] 远程执行命令
来源：http://zwj.chenlongwang.top

ssh user@host 'uptime'
来源：http://qpe.uphjek.com

[R58] 下载文件
来源：http://ihg.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tsk.zhengqikj.top

[R59] 发 POST JSON
来源：http://muy.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxe.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://csm.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tgx.zdqjudy.top

[R61] 磁盘占用
来源：http://lwm.andypj.xyz

df -h;  du -sh *
来源：http://xfv.jyoumei.cn

[R62] 找最占空间的文件
来源：http://fwf.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://ncx.xinyue.icu

[R63] 内存与进程
来源：http://imt.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://mkd.hysaishi.cn

[R64] 结束进程
来源：http://dcu.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://rmw.jyoumei.cn

[R65] 查看端口占用
来源：http://qnf.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mks.c1oappe.top

[R66] 定时任务
来源：http://jse.yvedp.cn

crontab -e;  crontab -l
来源：http://pic.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://qbk.sxryk.cn

openssl rand -hex 16
来源：http://cbq.xuanzx.com

[R68] 计算文件校验值
来源：http://lii.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://rih.fzhhl.top

[R69] 生成随机密码
来源：http://eqw.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://wlu.yj202588.top

[R70] 时间戳与互转
来源：http://rho.aizwys.cn

date +%s;  date -d @1700000000
来源：http://oxm.jinqigufen.top

[R71] 日期格式化
来源：http://ffz.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://dyx.sweek.top

[R72] 等待端口就绪
来源：http://aud.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://frt.smart0.xyz

[R73] 分割大日志
来源：http://ozh.nanxuanxn.top

split -l 1000 big.log part_
来源：http://cne.ydzc1.top

[R74] 批量重命名
来源：http://rmv.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kzg.yj202588.top

[R75] 导出环境变量
来源：http://spq.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://iku.redwolf501.top

[R76] 使用临时文件
来源：http://neo.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzm.vqdsnc.cn

[R77] 读取用户输入
来源：http://qea.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://ewy.fzhhl.top

[R78] 交互式菜单
来源：http://lfx.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qau.yongpay.top

[R79] 解析命令行选项
来源：http://tnv.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uqo.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://pdw.dianchejie.cn

time ./run.sh
来源：http://zlb.iojbl.cn

================================================================================
来源：http://kmh.bjfxy.top

S. C / C++ 专题
来源：http://erf.jinqigufen.top

================================================================================
来源：http://lgo.aibaodan.cn

[S01] C：Hello World
来源：http://xeb.fktsv.cn

#include <stdio.h>
来源：http://yfb.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://geq.epnwcf.com

[S02] C：变量与格式化输出
来源：http://taf.sweek.top

int a = 10; printf("%d\n", a);
来源：http://jhh.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://alx.sweek.top

int x; scanf("%d", &x);
来源：http://iko.cashguo.top

[S04] C：字符串复制
来源：http://qpi.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://nwc.hnxiangtu.top

[S05] C：字符串长度
来源：http://skm.shzxlz.cn

strlen(s)
来源：http://mar.gzhubu.top

[S06] C：字符串比较
来源：http://htp.zdbjq.cn

strcmp(a, b) == 0
来源：http://rpp.tianlin.xyz

[S07] C：数组遍历求和
来源：http://loo.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hwa.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://nlb.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qod.uphjek.com

[S09] C：结构体定义与初始化
来源：http://mem.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hdc.sxryk.cn

[S10] C：指针与解引用
来源：http://pzv.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://nmw.cashguo.top

[S11] C：逐行读文件
来源：http://ius.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://loz.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gnv.yfazqb.com

fclose(f);
来源：http://boi.meibo888.top

[S12] C：写文件
来源：http://ihm.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pvd.feifeiyinyue.top

[S13] C：宏定义
来源：http://wvb.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vns.zycfv.cn

[S14] C：枚举
来源：http://gfk.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://lob.wangdashe.top

[S15] C：类型转换
来源：http://puv.gzhubu.top

(double) a / b
来源：http://snd.bbcook.cn

[S16] C：位操作置位
来源：http://fon.jqgufenzy.top

x |= (1 << 3);
来源：http://eep.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://bli.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://crz.xinyue.icu

[S18] C：命令行参数
来源：http://ecq.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://pry.kuanghao11.cn

[S19] C：快速排序
来源：http://dae.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://ozu.gaohongyu789.top

[S20] C：二分查找
来源：http://cpr.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pab.shzxlz.cn

[S21] C：字符类别判断
来源：http://qjc.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://onv.fzhhl.top

[S22] C：字符串转数字
来源：http://rjd.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://crd.bjfxy.top

[S23] C：随机数
来源：http://fjy.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hjf.yj202588.top

[S24] C：获取本地时间
来源：http://qiz.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wtc.gaohongyu789.top

[S25] C：内存拷贝
来源：http://qpv.chenzaomai.com

memcpy(dst, src, n);
来源：http://ehj.hysaishi.cn

[S26] C：内存清零
来源：http://mmq.gzhubu.top

memset(a, 0, sizeof a);
来源：http://fjg.chenlongwang.top

[S27] C：定义常量
来源：http://nqj.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://knc.hywenlv.cn

[S28] C：静态变量
来源：http://rzz.gzhubu.top

static int counter = 0;
来源：http://ocb.sysykeji.top

[S29] C：变参函数
来源：http://zll.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rtg.xuanzx.com

[S30] C：头文件保护
来源：http://loj.kuanghao11.cn

#ifndef X_H
来源：http://jht.jqgfzy.top

#define X_H
来源：http://nyo.sysykeji.top

#endif
来源：http://fob.hysaishi.cn

[S31] C++：Hello World
来源：http://npu.ywan-chungtsiang.top

#include <iostream>
来源：http://abv.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://khu.svipenyu.cn

[S32] C++：字符串
来源：http://siz.tarul.cn

std::string s = "hi";  s += "!";
来源：http://xbe.hcnkem.com

[S33] C++：vector 增删
来源：http://xad.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dlt.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://ukz.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://hdw.zhixingplan.top

[S35] C++：map
来源：http://gzg.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qre.kuanghao11.cn

[S36] C++：unordered_map
来源：http://zun.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nme.fktsv.cn

[S37] C++：set
来源：http://gzb.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tsb.yj20258888.top

[S38] C++：排序
来源：http://xad.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://egk.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://lxd.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rmd.chenlongwang.top

[S40] C++：查找元素
来源：http://kdt.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yjv.bbcook.cn


<!-- 参考信息 -->