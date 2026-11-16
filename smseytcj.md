代发 wailian999

[Q67] 设置隔离级别
来源：http://rcj.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cbj.andypj.xyz

[Q68] 保存点
来源：http://yvy.gogol.net.cn

SAVEPOINT sp1;
来源：http://jru.yueranfly.top

ROLLBACK TO sp1;
来源：http://xlq.zdqjudy.top

[Q69] 查看执行计划
来源：http://hpl.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qjk.pycfn.com

[Q70] 更新统计信息
来源：http://zmu.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://jmo.0kj1m.cn

[Q71] 查看建表语句
来源：http://ade.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zsh.ivvv.top

[Q72] 查看索引
来源：http://pfx.ehwqpu.com

SHOW INDEX FROM users;
来源：http://bwy.yj202588.top

[Q73] 查看表状态
来源：http://dcd.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xnv.zhijiandao.cn

[Q74] 强制使用索引
来源：http://wtj.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gtw.9152youxi.cn

[Q75] 日期格式化
来源：http://mzv.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bfd.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xod.fanxiaobao.xyz

[Q76] 按天统计
来源：http://nkk.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://coi.shanyushiyangtech.top

[Q77] 时间加减
来源：http://iwq.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zlm.cheryme.top

[Q78] 当前时间
来源：http://ptt.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://haz.yonumen.top

[Q79] 字符串拼接
来源：http://agl.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ysa.wangshuangyany.cn

[Q80] 字符串截取
来源：http://ekh.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mvo.yvedp.cn

[Q81] 字符串替换
来源：http://odz.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vzi.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://anm.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://spc.yueranfly.top

[Q83] 大小写转换
来源：http://wif.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://omi.iojbl.cn

[Q84] 去除首尾空格
来源：http://raq.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://sso.yangfankeji.com

[Q85] 数值取整
来源：http://tjz.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nou.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://jsv.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jgp.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://llx.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bml.sweek.top

[Q88] 行转列（条件聚合）
来源：http://kas.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzx.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://imx.cucudq.cn

[Q89] 判断表是否存在
来源：http://zyq.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hrq.tanke756.top

[Q90] 生成序号列
来源：http://tbb.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xww.yuxming.cn

================================================================================
来源：http://rae.zhaomingkeji.xyz

R. Bash 专题
来源：http://kei.9152youxi.cn

================================================================================
来源：http://kyn.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://azi.bjfxy.top

#!/usr/bin/env bash
来源：http://noc.meibo888.top

set -euo pipefail
来源：http://ftg.yueranfly.top

[R02] 变量赋值与使用
来源：http://myk.xylfe.cn

name="Tom"; echo "$name"
来源：http://anu.bbcook.cn

[R03] 只读变量
来源：http://eaw.fengsongda.top

readonly PI=3.14
来源：http://elm.jqgfzy.top

[R04] 位置参数
来源：http://uix.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gct.haohaochexian.top

[R05] 参数默认值
来源：http://ius.cdnleiting.top

name="${1:-default}"
来源：http://qyk.fehbvm.com

[R06] 判断命令是否存在
来源：http://dze.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qhz.zdbjq.cn

[R07] if 判断文件
来源：http://syr.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vgo.ivvv.top

[R08] 数值比较
来源：http://yia.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ctu.snrcjt.cn

[R09] 字符串比较
来源：http://swa.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fiu.dianchejie.cn

[R10] 正则匹配
来源：http://utw.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uvj.ctjpmb.com

[R11] case 多分支
来源：http://qel.ywan-chungtsiang.top

case "$1" in
来源：http://vhg.chenlongwang.top

start) echo "启动" ;;
来源：http://kxo.bjfxy.top

stop)  echo "停止" ;;
来源：http://inr.iojbl.cn

*)     echo "未知命令" ;;
来源：http://jjn.yongpay.top

esac
来源：http://xwt.gogol.net.cn

[R12] for 遍历文件
来源：http://dhs.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://opu.sweek.top

[R13] for 计数循环
来源：http://dex.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://fxi.smart0.xyz

[R14] C 风格 for
来源：http://owp.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nmj.zdbjq.cn

[R15] while 逐行读文件
来源：http://rvz.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://stl.yvedp.cn

[R16] until 等待条件
来源：http://tbp.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://plx.zhijiandao.cn

[R17] 数组定义与取值
来源：http://olw.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://uff.wangdashe.top

[R18] 遍历数组
来源：http://rlf.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wxx.guowangkeji.top

[R19] 数组长度
来源：http://pdx.iojbl.cn

echo "${#arr[@]}"
来源：http://vap.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://hjd.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jum.jinqigfzy.top

[R21] 字符串长度
来源：http://efm.cqqwz.cn

echo "${#s}"
来源：http://oxs.havefunace.top

[R22] 截取子串
来源：http://lkp.ehwqpu.com

echo "${s:0:5}"
来源：http://ioj.tianlin.xyz

[R23] 字符串替换
来源：http://iak.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://msm.fanxiaobao.xyz

[R24] 大小写转换
来源：http://aaw.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://civ.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://zdj.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vhv.yangfankeji.com

[R26] 命令替换
来源：http://lvz.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://esw.redwolf501.top

[R27] 算术展开
来源：http://inz.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://umw.yongpay.top

[R28] 浮点运算
来源：http://sub.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://gvy.yuanzhike.top

[R29] 定义函数
来源：http://zzh.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://luz.bbcook.cn

[R30] 函数返回状态码
来源：http://gjn.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://aic.zhijiandao.cn

[R31] 局部变量
来源：http://lxf.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://aqn.cucudq.cn

[R32] 参数个数校验
来源：http://dsc.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oqh.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://xqj.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wxy.hcnkem.com

[R34] 退出时清理
来源：http://xgo.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://edk.zdqjudy.top

[R35] 后台执行并等待
来源：http://qbw.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gig.pycfn.com

[R36] 并发执行多个任务
来源：http://dbl.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gyj.daxiang520.top

[R37] 把输出赋给变量
来源：http://hfx.gogol.net.cn

files=$(ls -1)
来源：http://jdz.fanxiaobao.xyz

[R38] 管道串联
来源：http://fnp.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://liv.yonumen.top

[R39] 重定向标准输出与错误
来源：http://qjr.tarul.cn

cmd > out.log 2>&1
来源：http://elk.vqdsnc.cn

[R40] 追加写日志
来源：http://gto.tanke756.top

echo "log" >> out.log
来源：http://tgx.tian-w.cn

[R41] 丢弃输出
来源：http://kfm.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://adk.gaohongyu789.top

[R42] 输入重定向
来源：http://mzl.xuanzx.com

wc -l < a.txt
来源：http://vsz.meibo888.top

[R43] 按名字查找文件
来源：http://nkb.dianchejie.cn

find . -name "*.log" -type f
来源：http://dka.yueranfly.top

[R44] 按修改时间查找
来源：http://bwj.hnxiangtu.top

find . -mtime -7 -type f
来源：http://xqp.yfazqb.com

[R45] 批量删除
来源：http://eeq.bjfxy.top

find . -name "*.tmp" -delete
来源：http://kuq.dianchejie.cn

[R46] 递归替换文件内容
来源：http://tqd.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xil.hnxiangtu.top

[R47] sed 单行替换
来源：http://eje.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://dje.ydjk.org.cn

[R48] awk 取指定列
来源：http://kel.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://nun.yonumen.top

[R49] awk 带条件
来源：http://luz.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yso.jqgfzy.top

[R50] awk 求和
来源：http://ibx.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://qcl.redwolf501.top

[R51] 排序去重取前几
来源：http://mms.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://haq.dashuyun.cn

[R52] 统计行数
来源：http://occ.yj202588.top

wc -l a.txt
来源：http://jqw.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://ehd.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://frl.dashuyun.cn

[R54] 比较两个文件
来源：http://hdp.316326.xyz

diff a.txt b.txt
来源：http://qeh.shangyingyoupin.top

[R55] 压缩与解压
来源：http://zgz.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nqx.xuetiantiany.cn

[R56] 远程拷贝
来源：http://mde.smart0.xyz

scp file user@host:/path/
来源：http://aib.fzhhl.top

[R57] 远程执行命令
来源：http://zmq.yonumen.top

ssh user@host 'uptime'
来源：http://onk.feifeiyinyue.top

[R58] 下载文件
来源：http://giu.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mge.cheryme.top

[R59] 发 POST JSON
来源：http://bnw.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qsg.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://rgo.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cxy.svipenyu.cn

[R61] 磁盘占用
来源：http://fhy.cashguo.top

df -h;  du -sh *
来源：http://kmh.hnqzz.top

[R62] 找最占空间的文件
来源：http://fvu.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://ipz.yanxiufei.cn

[R63] 内存与进程
来源：http://bzl.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://vjg.dianchejie.cn

[R64] 结束进程
来源：http://nei.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://zgk.ydzc1.top

[R65] 查看端口占用
来源：http://rdk.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kbs.sysykeji.top

[R66] 定时任务
来源：http://emc.ctjpmb.com

crontab -e;  crontab -l
来源：http://zxi.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://gzm.yuanzhike.top

openssl rand -hex 16
来源：http://tec.ppjwa.cn

[R68] 计算文件校验值
来源：http://gmx.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://dzb.ppjwa.cn

[R69] 生成随机密码
来源：http://gel.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://ytl.xinyue.icu

[R70] 时间戳与互转
来源：http://bkk.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://eje.yanxiufei.cn

[R71] 日期格式化
来源：http://lmg.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fdo.zhixingplan.top

[R72] 等待端口就绪
来源：http://xnc.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iiv.dianchejie.cn

[R73] 分割大日志
来源：http://tlj.birdmap.top

split -l 1000 big.log part_
来源：http://ahg.yangfankeji.com

[R74] 批量重命名
来源：http://vpb.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fzx.jianghu66.top

[R75] 导出环境变量
来源：http://veo.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://ppf.52xcode.cn

[R76] 使用临时文件
来源：http://ewz.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dmb.tarul.cn

[R77] 读取用户输入
来源：http://bwn.bbcook.cn

read -rp "请输入: " ans
来源：http://ezi.shuidangran.top

[R78] 交互式菜单
来源：http://kfp.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://bak.cdnleiting.top

[R79] 解析命令行选项
来源：http://hwb.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rlk.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://gma.jqgfzy.top

time ./run.sh
来源：http://vzo.redwolf501.top

================================================================================
来源：http://hmg.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://ztp.xingfuxueyuan.xyz

================================================================================
来源：http://xkj.havefunace.top

[S01] C：Hello World
来源：http://hek.uphjek.com

#include <stdio.h>
来源：http://whu.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ivq.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://wxt.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://tku.xylfe.cn

[S03] C：读入整数
来源：http://rhp.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://asv.hesvh.cn

[S04] C：字符串复制
来源：http://ywa.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://xbe.gotoacloud.top

[S05] C：字符串长度
来源：http://cjp.fehbvm.com

strlen(s)
来源：http://xpn.nwbrower.top

[S06] C：字符串比较
来源：http://khd.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://sai.hnqzz.top

[S07] C：数组遍历求和
来源：http://jmw.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yoa.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://pcy.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gda.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://aib.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mse.nanxuanxn.top

[S10] C：指针与解引用
来源：http://eby.hammf.cn

int *p = &a;  *p = 5;
来源：http://xdb.yfazqb.com

[S11] C：逐行读文件
来源：http://ayy.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://stj.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sii.yueranfly.top

fclose(f);
来源：http://kop.sysykeji.top

[S12] C：写文件
来源：http://byf.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dsl.snrcjt.cn

[S13] C：宏定义
来源：http://rwc.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://arw.bbcook.cn

[S14] C：枚举
来源：http://her.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://hko.hongshengwenyu.top

[S15] C：类型转换
来源：http://buv.yj202588.top

(double) a / b
来源：http://tum.zdqjudy.top

[S16] C：位操作置位
来源：http://kje.xuetiantiany.cn

x |= (1 << 3);
来源：http://vxf.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://kov.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jsw.wangshuangyany.cn

[S18] C：命令行参数
来源：http://jta.xuanzx.com

int main(int argc, char **argv)
来源：http://tkg.316326.xyz

[S19] C：快速排序
来源：http://uga.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://gga.cashguo.top

[S20] C：二分查找
来源：http://auo.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpa.bbcook.cn

[S21] C：字符类别判断
来源：http://cvv.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aml.jinqigfzy.top

[S22] C：字符串转数字
来源：http://tih.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://kro.zhiwuduotai.top

[S23] C：随机数
来源：http://xon.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dxw.gogol.net.cn

[S24] C：获取本地时间
来源：http://aup.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vze.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://fej.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://dhu.chenzaomai.com

[S26] C：内存清零
来源：http://rjm.mhx1999.top

memset(a, 0, sizeof a);
来源：http://kzp.mhx1999.top

[S27] C：定义常量
来源：http://ibs.xuanzx.com

const double PI = 3.14159;
来源：http://oel.hysaishi.cn

[S28] C：静态变量
来源：http://jfr.tarul.cn

static int counter = 0;
来源：http://mql.snrcjt.cn

[S29] C：变参函数
来源：http://vaj.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zsv.fktsv.cn

[S30] C：头文件保护
来源：http://yog.sysykeji.top

#ifndef X_H
来源：http://ohh.hongshengwenyu.top

#define X_H
来源：http://csc.dianchejie.cn

#endif
来源：http://guf.zhengqikj.top

[S31] C++：Hello World
来源：http://fsx.wangdashe.top

#include <iostream>
来源：http://sbq.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://pxa.shuidangran.top

[S32] C++：字符串
来源：http://xyf.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://apr.bbcook.cn

[S33] C++：vector 增删
来源：http://vzt.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tan.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://oup.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://zoe.xziqi.cn

[S35] C++：map
来源：http://zfc.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rch.hnqzz.top

[S36] C++：unordered_map
来源：http://kps.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://etu.zhaomingkeji.xyz


<!-- 参考信息 -->