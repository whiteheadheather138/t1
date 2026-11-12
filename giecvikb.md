代发 wailian999

[Q67] 设置隔离级别
来源：http://wow.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://obn.gotoacloud.top

[Q68] 保存点
来源：http://hzx.yfazqb.com

SAVEPOINT sp1;
来源：http://neu.svipenyu.cn

ROLLBACK TO sp1;
来源：http://zvs.xylfe.cn

[Q69] 查看执行计划
来源：http://jon.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vqo.zhijiandao.cn

[Q70] 更新统计信息
来源：http://wtw.yj202588.top

ANALYZE TABLE users;
来源：http://qbj.52xcode.cn

[Q71] 查看建表语句
来源：http://qyg.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gkh.hnxiangtu.top

[Q72] 查看索引
来源：http://zfa.xziqi.cn

SHOW INDEX FROM users;
来源：http://tbp.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://yin.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rvo.yvedp.cn

[Q74] 强制使用索引
来源：http://vda.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://evj.gogol.net.cn

[Q75] 日期格式化
来源：http://bjj.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mox.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xkc.xuetiantiany.cn

[Q76] 按天统计
来源：http://jmr.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yvw.hesvh.cn

[Q77] 时间加减
来源：http://opl.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lrf.hnqzz.top

[Q78] 当前时间
来源：http://sxj.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ncg.meibo888.top

[Q79] 字符串拼接
来源：http://khy.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://isd.yfazqb.com

[Q80] 字符串截取
来源：http://wjq.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eer.yueranfly.top

[Q81] 字符串替换
来源：http://yvs.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bsp.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://clh.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mae.ybcxt.top

[Q83] 大小写转换
来源：http://xvs.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kmf.hammf.cn

[Q84] 去除首尾空格
来源：http://yqk.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://ucn.chenzaomai.com

[Q85] 数值取整
来源：http://jqo.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mbq.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://glr.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vll.yongpay.top

[Q87] JSON 字段做条件
来源：http://iuk.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fpe.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://lde.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kaw.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ndc.jinqigufen.top

[Q89] 判断表是否存在
来源：http://ckr.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://amz.cqqwz.cn

[Q90] 生成序号列
来源：http://ezd.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://syo.dianchejie.cn

================================================================================
来源：http://yrf.hnxiangtu.top

R. Bash 专题
来源：http://tye.jianghu66.top

================================================================================
来源：http://rti.sufxvd.cn

[R01] shebang 与严格模式
来源：http://siy.hfpthk.cn

#!/usr/bin/env bash
来源：http://thq.yj20258888.top

set -euo pipefail
来源：http://fpr.yj20258.top

[R02] 变量赋值与使用
来源：http://bhj.ivvv.top

name="Tom"; echo "$name"
来源：http://cgi.ivvv.top

[R03] 只读变量
来源：http://xjf.zhijiandao.cn

readonly PI=3.14
来源：http://llz.xinyue.icu

[R04] 位置参数
来源：http://xev.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pwj.hnqzz.top

[R05] 参数默认值
来源：http://hrk.zycfv.cn

name="${1:-default}"
来源：http://ejn.cucudq.cn

[R06] 判断命令是否存在
来源：http://wgw.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mwy.guannengcc.top

[R07] if 判断文件
来源：http://nqe.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fjy.quarkkingdee.top

[R08] 数值比较
来源：http://yml.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ljo.ppjwa.cn

[R09] 字符串比较
来源：http://rvc.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mev.gaohongyu789.top

[R10] 正则匹配
来源：http://xey.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rcy.yj20258.top

[R11] case 多分支
来源：http://yiq.jlsjyb.cn

case "$1" in
来源：http://wod.zhijiandao.cn

start) echo "启动" ;;
来源：http://clz.jianghu66.top

stop)  echo "停止" ;;
来源：http://xgx.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://ygx.yuxming.cn

esac
来源：http://vjz.jqgufenzy.top

[R12] for 遍历文件
来源：http://dna.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://dvn.nanxuanxn.top

[R13] for 计数循环
来源：http://kym.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://gmg.c1oappe.top

[R14] C 风格 for
来源：http://utp.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zsj.ehwqpu.com

[R15] while 逐行读文件
来源：http://flm.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://goa.yueranfly.top

[R16] until 等待条件
来源：http://era.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zis.chenlongwang.top

[R17] 数组定义与取值
来源：http://ayx.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sxm.fanxiaobao.xyz

[R18] 遍历数组
来源：http://fhp.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://phs.zhongyouzk.top

[R19] 数组长度
来源：http://tpy.ivvv.top

echo "${#arr[@]}"
来源：http://kiz.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://fzs.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jwk.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://zqp.guannengcc.top

echo "${#s}"
来源：http://fal.fktsv.cn

[R22] 截取子串
来源：http://asg.bjfxy.top

echo "${s:0:5}"
来源：http://ktu.sysykeji.top

[R23] 字符串替换
来源：http://xeg.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ece.jinqigfzy.top

[R24] 大小写转换
来源：http://aft.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://uwk.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://dej.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tvp.ivvv.top

[R26] 命令替换
来源：http://qzc.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://djs.chenzaomai.com

[R27] 算术展开
来源：http://eex.yvedp.cn

echo $((1 + 2 * 3))
来源：http://ulw.pycfn.com

[R28] 浮点运算
来源：http://jow.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://pjs.hnxiangtu.top

[R29] 定义函数
来源：http://lox.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kdk.ydjk.org.cn

[R30] 函数返回状态码
来源：http://pdl.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://pxc.fktsv.cn

[R31] 局部变量
来源：http://moa.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://jrf.birdmap.top

[R32] 参数个数校验
来源：http://tsl.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zbb.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://lin.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://day.jlsjyb.cn

[R34] 退出时清理
来源：http://kji.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://niu.birdmap.top

[R35] 后台执行并等待
来源：http://xrl.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cbe.316326.xyz

[R36] 并发执行多个任务
来源：http://vnp.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qdy.ppjwa.cn

[R37] 把输出赋给变量
来源：http://tio.hnxiangtu.top

files=$(ls -1)
来源：http://wez.guowangkeji.top

[R38] 管道串联
来源：http://odw.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://evf.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://wny.meibo888.top

cmd > out.log 2>&1
来源：http://gll.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://oab.smart0.xyz

echo "log" >> out.log
来源：http://blp.9152youxi.cn

[R41] 丢弃输出
来源：http://rfq.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://lnq.nanxuanxn.top

[R42] 输入重定向
来源：http://gcz.jlsjyb.cn

wc -l < a.txt
来源：http://tpg.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://tjv.tanke756.top

find . -name "*.log" -type f
来源：http://mft.hcnkem.com

[R44] 按修改时间查找
来源：http://hhy.fzhhl.top

find . -mtime -7 -type f
来源：http://mea.xuanzx.com

[R45] 批量删除
来源：http://tjl.yueranfly.top

find . -name "*.tmp" -delete
来源：http://scw.shuidangran.top

[R46] 递归替换文件内容
来源：http://ant.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pov.chenjidiqi.icu

[R47] sed 单行替换
来源：http://tsp.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://szz.uphjek.com

[R48] awk 取指定列
来源：http://zoe.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://mcx.yj20258.top

[R49] awk 带条件
来源：http://yal.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://trp.quarkkingdee.top

[R50] awk 求和
来源：http://djr.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kdj.daxiang520.top

[R51] 排序去重取前几
来源：http://geu.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rzi.dianchejie.cn

[R52] 统计行数
来源：http://boj.nanxinkj.top

wc -l a.txt
来源：http://jdi.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://mig.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nfo.gogol.net.cn

[R54] 比较两个文件
来源：http://uaz.yueranfly.top

diff a.txt b.txt
来源：http://zwv.zhiwuduotai.top

[R55] 压缩与解压
来源：http://spx.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jlc.fehbvm.com

[R56] 远程拷贝
来源：http://ixf.jinghuilouyu.cn

scp file user@host:/path/
来源：http://sox.chenlongwang.top

[R57] 远程执行命令
来源：http://vtc.sweek.top

ssh user@host 'uptime'
来源：http://pmc.chenzaomai.com

[R58] 下载文件
来源：http://ksw.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uff.hysaishi.cn

[R59] 发 POST JSON
来源：http://lsn.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://whg.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://sgs.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aey.ydjk.org.cn

[R61] 磁盘占用
来源：http://atn.chenzaomai.com

df -h;  du -sh *
来源：http://thy.epnwcf.com

[R62] 找最占空间的文件
来源：http://gyc.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://nwt.shzxlz.cn

[R63] 内存与进程
来源：http://elx.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://jmp.ydjk.org.cn

[R64] 结束进程
来源：http://nte.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://yfb.nwbrower.top

[R65] 查看端口占用
来源：http://xfs.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qpn.ctjpmb.com

[R66] 定时任务
来源：http://iiu.hnxiangtu.top

crontab -e;  crontab -l
来源：http://ypw.zycfv.cn

[R67] 生成随机十六进制串
来源：http://mms.dashuyun.cn

openssl rand -hex 16
来源：http://qpd.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://pod.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://fke.birdmap.top

[R69] 生成随机密码
来源：http://ftg.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://lmo.dianchejie.cn

[R70] 时间戳与互转
来源：http://bsc.aizwys.cn

date +%s;  date -d @1700000000
来源：http://tzh.aibaodan.cn

[R71] 日期格式化
来源：http://plu.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zfe.yanxiufei.cn

[R72] 等待端口就绪
来源：http://jlx.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bfa.snrcjt.cn

[R73] 分割大日志
来源：http://gum.hnxiangtu.top

split -l 1000 big.log part_
来源：http://rug.ydjk.org.cn

[R74] 批量重命名
来源：http://vmc.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qqk.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://voc.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://dqx.zhixingplan.top

[R76] 使用临时文件
来源：http://ewc.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wgx.ctjpmb.com

[R77] 读取用户输入
来源：http://sdb.zycfv.cn

read -rp "请输入: " ans
来源：http://oql.tian-w.cn

[R78] 交互式菜单
来源：http://jdf.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qfx.hysaishi.cn

[R79] 解析命令行选项
来源：http://jan.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ows.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://cyv.snrcjt.cn

time ./run.sh
来源：http://btd.sxryk.cn

================================================================================
来源：http://dfi.aizwys.cn

S. C / C++ 专题
来源：http://jxn.hnqzz.top

================================================================================
来源：http://dxv.bbcook.cn

[S01] C：Hello World
来源：http://ttd.hongshengwenyu.top

#include <stdio.h>
来源：http://euv.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jeg.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://ows.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://voy.nwbrower.top

[S03] C：读入整数
来源：http://sag.sufxvd.cn

int x; scanf("%d", &x);
来源：http://hgn.ivvv.top

[S04] C：字符串复制
来源：http://sga.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://maj.guowangkeji.top

[S05] C：字符串长度
来源：http://tmf.yj20258.top

strlen(s)
来源：http://zuc.meibo888.top

[S06] C：字符串比较
来源：http://nxc.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://lxg.daxiang520.top

[S07] C：数组遍历求和
来源：http://tfo.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iol.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://aks.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xcj.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://edu.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yjr.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://qtg.yonumen.top

int *p = &a;  *p = 5;
来源：http://mnc.yuanzhike.top

[S11] C：逐行读文件
来源：http://fkr.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://oon.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zug.hfpthk.cn

fclose(f);
来源：http://rta.sysykeji.top

[S12] C：写文件
来源：http://drv.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bgc.yangfankeji.com

[S13] C：宏定义
来源：http://ohr.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dkn.ppjwa.cn

[S14] C：枚举
来源：http://jfh.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://nrj.jinghuilouyu.cn

[S15] C：类型转换
来源：http://rry.zhengqikj.top

(double) a / b
来源：http://zqw.fktsv.cn

[S16] C：位操作置位
来源：http://aec.gogol.net.cn

x |= (1 << 3);
来源：http://jjk.uphjek.com

[S17] C：安全拼接字符串
来源：http://voa.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ero.aizwys.cn

[S18] C：命令行参数
来源：http://lei.chenzaomai.com

int main(int argc, char **argv)
来源：http://dol.yj202588.top

[S19] C：快速排序
来源：http://saz.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://zaq.gotoacloud.top

[S20] C：二分查找
来源：http://aqr.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://szz.yj20258888.top

[S21] C：字符类别判断
来源：http://cuq.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ljf.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://dxo.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xny.cheryme.top

[S23] C：随机数
来源：http://rpv.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jka.jinqigufen.top

[S24] C：获取本地时间
来源：http://shn.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mso.redwolf501.top

[S25] C：内存拷贝
来源：http://mtc.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://gdn.shuidangran.top

[S26] C：内存清零
来源：http://qej.sweek.top

memset(a, 0, sizeof a);
来源：http://beb.haohaochexian.top

[S27] C：定义常量
来源：http://eic.fktsv.cn

const double PI = 3.14159;
来源：http://hyt.hywenlv.cn

[S28] C：静态变量
来源：http://otw.pengpengdd.cyou

static int counter = 0;
来源：http://xbh.ydjk.org.cn

[S29] C：变参函数
来源：http://usl.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mtg.nwbrower.top

[S30] C：头文件保护
来源：http://jku.ivvv.top

#ifndef X_H
来源：http://uff.snrcjt.cn

#define X_H
来源：http://edr.zhiwuduotai.top

#endif
来源：http://pol.chenjidiqi.icu

[S31] C++：Hello World
来源：http://dor.xuanzx.com

#include <iostream>
来源：http://xzh.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://smx.316326.xyz

[S32] C++：字符串
来源：http://wuu.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://hxj.xuanzx.com

[S33] C++：vector 增删
来源：http://jrc.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqe.hesvh.cn

[S34] C++：遍历 vector
来源：http://lcd.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://okc.jinqigufen.top

[S35] C++：map
来源：http://tws.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kaz.cheryme.top

[S36] C++：unordered_map
来源：http://zni.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://feu.svipenyu.cn


<!-- 参考信息 -->