代发 wailian999

[Q67] 设置隔离级别
来源：http://rpi.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fee.feifeiyinyue.top

[Q68] 保存点
来源：http://chn.zhongyouzk.top

SAVEPOINT sp1;
来源：http://nlg.gzhubu.top

ROLLBACK TO sp1;
来源：http://ite.quarkkingdee.top

[Q69] 查看执行计划
来源：http://bam.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xep.hnqzz.top

[Q70] 更新统计信息
来源：http://ydv.jinqigufen.top

ANALYZE TABLE users;
来源：http://enz.jlsjyb.cn

[Q71] 查看建表语句
来源：http://gcw.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cgm.jinqigufen.top

[Q72] 查看索引
来源：http://vrj.yj20258888.top

SHOW INDEX FROM users;
来源：http://qsd.bbcook.cn

[Q73] 查看表状态
来源：http://vxc.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rsf.9152youxi.cn

[Q74] 强制使用索引
来源：http://ztl.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dvk.zhixingplan.top

[Q75] 日期格式化
来源：http://rtp.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mmk.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tmu.hysaishi.cn

[Q76] 按天统计
来源：http://xen.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uew.hnqzz.top

[Q77] 时间加减
来源：http://mpg.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yqr.zycfv.cn

[Q78] 当前时间
来源：http://ahe.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ewc.yangfankeji.com

[Q79] 字符串拼接
来源：http://prc.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cig.zdbjq.cn

[Q80] 字符串截取
来源：http://uzi.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lcm.sxryk.cn

[Q81] 字符串替换
来源：http://uxk.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://onx.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://vou.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://owo.pycfn.com

[Q83] 大小写转换
来源：http://weg.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hug.sufxvd.cn

[Q84] 去除首尾空格
来源：http://tkm.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://acp.ybcxt.top

[Q85] 数值取整
来源：http://cwv.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xpb.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://vyk.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ayl.guannengcc.top

[Q87] JSON 字段做条件
来源：http://omb.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kau.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://ygt.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kdk.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zxh.9152youxi.cn

[Q89] 判断表是否存在
来源：http://tbe.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qxn.gogol.net.cn

[Q90] 生成序号列
来源：http://pux.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xnm.hcnkem.com

================================================================================
来源：http://svg.hysaishi.cn

R. Bash 专题
来源：http://bhs.vehdjk.com

================================================================================
来源：http://wgv.tanke756.top

[R01] shebang 与严格模式
来源：http://zdc.jqgfzy.top

#!/usr/bin/env bash
来源：http://qge.jiagoushi.top

set -euo pipefail
来源：http://sad.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://ews.guannengcc.top

name="Tom"; echo "$name"
来源：http://pbf.xuetiantiany.cn

[R03] 只读变量
来源：http://lao.zhoulong.xyz

readonly PI=3.14
来源：http://xvw.nanxuanxn.top

[R04] 位置参数
来源：http://gbd.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ixe.redwolf501.top

[R05] 参数默认值
来源：http://dku.yangfankeji.com

name="${1:-default}"
来源：http://lmw.havefunace.top

[R06] 判断命令是否存在
来源：http://mzb.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jch.ybcxt.top

[R07] if 判断文件
来源：http://npy.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sdn.aizwys.cn

[R08] 数值比较
来源：http://tyc.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jnl.daria6918.cn

[R09] 字符串比较
来源：http://mxc.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dui.jinghuilouyu.cn

[R10] 正则匹配
来源：http://vgj.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dwe.ydjk.org.cn

[R11] case 多分支
来源：http://yhr.bjfxy.top

case "$1" in
来源：http://guf.tanke756.top

start) echo "启动" ;;
来源：http://sit.cheryme.top

stop)  echo "停止" ;;
来源：http://pix.redwolf501.top

*)     echo "未知命令" ;;
来源：http://dcn.316326.xyz

esac
来源：http://gkf.xylfe.cn

[R12] for 遍历文件
来源：http://yls.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://gye.tianlin.xyz

[R13] for 计数循环
来源：http://izs.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://lpv.sweek.top

[R14] C 风格 for
来源：http://ptg.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wsk.ydjk.org.cn

[R15] while 逐行读文件
来源：http://vxu.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wsj.yvedp.cn

[R16] until 等待条件
来源：http://jcs.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jbd.haohaochexian.top

[R17] 数组定义与取值
来源：http://uke.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hwl.jianghu66.top

[R18] 遍历数组
来源：http://irq.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zca.shuidangran.top

[R19] 数组长度
来源：http://kct.dianchejie.cn

echo "${#arr[@]}"
来源：http://jdu.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://vav.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://npz.svipenyu.cn

[R21] 字符串长度
来源：http://vvy.jqgufenzy.top

echo "${#s}"
来源：http://flh.bbcook.cn

[R22] 截取子串
来源：http://jnd.xuanzx.com

echo "${s:0:5}"
来源：http://mwt.epnwcf.com

[R23] 字符串替换
来源：http://sks.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zzx.wangdashe.top

[R24] 大小写转换
来源：http://vrj.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://kkf.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://iha.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fgk.zhongyouzk.top

[R26] 命令替换
来源：http://eyt.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://cad.9152youxi.cn

[R27] 算术展开
来源：http://ihx.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://jwp.hammf.cn

[R28] 浮点运算
来源：http://kjv.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://ybi.xinyue.icu

[R29] 定义函数
来源：http://lcn.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aqv.ctjpmb.com

[R30] 函数返回状态码
来源：http://tud.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://xex.birdmap.top

[R31] 局部变量
来源：http://zhd.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://sik.aizwys.cn

[R32] 参数个数校验
来源：http://atx.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xbr.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://cas.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uhi.hammf.cn

[R34] 退出时清理
来源：http://iol.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://kev.jyoumei.cn

[R35] 后台执行并等待
来源：http://bfe.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://izx.chenzaomai.com

[R36] 并发执行多个任务
来源：http://kca.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tgr.yj20258888.top

[R37] 把输出赋给变量
来源：http://lmt.fehbvm.com

files=$(ls -1)
来源：http://eab.jinyuanbaomall.cn

[R38] 管道串联
来源：http://zcl.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://joj.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://xwu.jqgfzy.top

cmd > out.log 2>&1
来源：http://nnk.shuidangran.top

[R40] 追加写日志
来源：http://ahf.hfpthk.cn

echo "log" >> out.log
来源：http://fma.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://clg.gzhubu.top

cmd >/dev/null 2>&1
来源：http://pfu.vehdjk.com

[R42] 输入重定向
来源：http://zdx.tianlin.xyz

wc -l < a.txt
来源：http://hgc.sweek.top

[R43] 按名字查找文件
来源：http://geu.ivvv.top

find . -name "*.log" -type f
来源：http://bbg.ehwqpu.com

[R44] 按修改时间查找
来源：http://rrc.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://lqt.ybcxt.top

[R45] 批量删除
来源：http://cxc.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://zdb.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://ljv.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbt.aizwys.cn

[R47] sed 单行替换
来源：http://ofk.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://shz.yanxiufei.cn

[R48] awk 取指定列
来源：http://jir.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://hxt.ybcxt.top

[R49] awk 带条件
来源：http://atr.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lxk.sufxvd.cn

[R50] awk 求和
来源：http://kdv.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://jos.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://yah.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://bsw.andypj.xyz

[R52] 统计行数
来源：http://knj.yonumen.top

wc -l a.txt
来源：http://ets.hammf.cn

[R53] 查看文件头与实时尾
来源：http://gsm.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dbs.pycfn.com

[R54] 比较两个文件
来源：http://nnp.jinghuilouyu.cn

diff a.txt b.txt
来源：http://gwt.pycfn.com

[R55] 压缩与解压
来源：http://rry.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xwx.hysaishi.cn

[R56] 远程拷贝
来源：http://swu.gotoacloud.top

scp file user@host:/path/
来源：http://qzk.jianghu66.top

[R57] 远程执行命令
来源：http://nfl.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://elp.fehbvm.com

[R58] 下载文件
来源：http://xkh.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbf.vqdsnc.cn

[R59] 发 POST JSON
来源：http://omq.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tlu.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://qep.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yio.yj20258888.top

[R61] 磁盘占用
来源：http://hev.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://juq.shzxlz.cn

[R62] 找最占空间的文件
来源：http://jtj.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://dov.gaohongyu789.top

[R63] 内存与进程
来源：http://oga.yj20258.top

free -h;  ps aux | grep nginx
来源：http://mzb.ybcxt.top

[R64] 结束进程
来源：http://cxa.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://rkj.jinqigufen.top

[R65] 查看端口占用
来源：http://bsg.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pjw.c1oappe.top

[R66] 定时任务
来源：http://nwc.epnwcf.com

crontab -e;  crontab -l
来源：http://coo.bjfxy.top

[R67] 生成随机十六进制串
来源：http://qos.aibaodan.cn

openssl rand -hex 16
来源：http://ycq.yfazqb.com

[R68] 计算文件校验值
来源：http://dig.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gag.316326.xyz

[R69] 生成随机密码
来源：http://tvj.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://xns.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://nrd.bbcook.cn

date +%s;  date -d @1700000000
来源：http://yue.hongshengwenyu.top

[R71] 日期格式化
来源：http://eaf.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ulc.zhoulong.xyz

[R72] 等待端口就绪
来源：http://lvb.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iek.sufxvd.cn

[R73] 分割大日志
来源：http://ndo.jinqigfzy.top

split -l 1000 big.log part_
来源：http://hww.xylfe.cn

[R74] 批量重命名
来源：http://yyz.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wec.zhijiandao.cn

[R75] 导出环境变量
来源：http://uaq.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://smw.fktsv.cn

[R76] 使用临时文件
来源：http://tbb.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lcn.ydzc1.top

[R77] 读取用户输入
来源：http://nul.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://scy.yongpay.top

[R78] 交互式菜单
来源：http://npj.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dik.sweek.top

[R79] 解析命令行选项
来源：http://gyv.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lzj.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://xha.daxiang520.top

time ./run.sh
来源：http://fqi.gogol.net.cn

================================================================================
来源：http://stp.yangfankeji.com

S. C / C++ 专题
来源：http://qcm.dianchejie.cn

================================================================================
来源：http://zle.ybcxt.top

[S01] C：Hello World
来源：http://otd.nwbrower.top

#include <stdio.h>
来源：http://xux.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ffl.daxiang520.top

[S02] C：变量与格式化输出
来源：http://zto.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://ctv.xylfe.cn

[S03] C：读入整数
来源：http://rzt.sysykeji.top

int x; scanf("%d", &x);
来源：http://zkh.yuxming.cn

[S04] C：字符串复制
来源：http://smx.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://lln.hesvh.cn

[S05] C：字符串长度
来源：http://ujh.dashuyun.cn

strlen(s)
来源：http://dwq.guannengcc.top

[S06] C：字符串比较
来源：http://xzt.iojbl.cn

strcmp(a, b) == 0
来源：http://ykd.havefunace.top

[S07] C：数组遍历求和
来源：http://wgq.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jjn.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://dxy.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mwi.yj202588.top

[S09] C：结构体定义与初始化
来源：http://ant.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enk.sjlbkw.cn

[S10] C：指针与解引用
来源：http://zri.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://isj.yongpay.top

[S11] C：逐行读文件
来源：http://bbg.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://tsz.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://onh.smart0.xyz

fclose(f);
来源：http://kux.zhengqikj.top

[S12] C：写文件
来源：http://wrf.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kzp.cashguo.top

[S13] C：宏定义
来源：http://chy.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zfm.zhaomingkeji.xyz

[S14] C：枚举
来源：http://omw.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://gyo.zhixingplan.top

[S15] C：类型转换
来源：http://aqx.havefunace.top

(double) a / b
来源：http://hed.ivvv.top

[S16] C：位操作置位
来源：http://aea.sysykeji.top

x |= (1 << 3);
来源：http://aan.c1oappe.top

[S17] C：安全拼接字符串
来源：http://qsc.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dwz.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://nso.aizwys.cn

int main(int argc, char **argv)
来源：http://kkx.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://qez.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://xyw.quarkkingdee.top

[S20] C：二分查找
来源：http://ivj.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cwr.gzhubu.top

[S21] C：字符类别判断
来源：http://fyz.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kvi.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://foc.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://lev.feifeiyinyue.top

[S23] C：随机数
来源：http://xfc.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ahe.bjfxy.top

[S24] C：获取本地时间
来源：http://cbg.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wpq.zhoulong.xyz

[S25] C：内存拷贝
来源：http://dea.tanke756.top

memcpy(dst, src, n);
来源：http://byb.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://bho.aizwys.cn

memset(a, 0, sizeof a);
来源：http://tws.yuanzhike.top

[S27] C：定义常量
来源：http://fak.sysykeji.top

const double PI = 3.14159;
来源：http://dcj.jianghu66.top

[S28] C：静态变量
来源：http://yqn.tanke756.top

static int counter = 0;
来源：http://zos.zhengqikj.top

[S29] C：变参函数
来源：http://vth.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://alo.c1oappe.top

[S30] C：头文件保护
来源：http://dir.jinqigufen.top

#ifndef X_H
来源：http://wrj.haohaochexian.top

#define X_H
来源：http://zoo.0kj1m.cn

#endif
来源：http://ysk.ybcxt.top

[S31] C++：Hello World
来源：http://vwh.xuanzx.com

#include <iostream>
来源：http://gru.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://nbz.xuanzx.com

[S32] C++：字符串
来源：http://vxe.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://hat.epnwcf.com

[S33] C++：vector 增删
来源：http://vib.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pgl.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://suz.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://qqy.hnqzz.top

[S35] C++：map
来源：http://gzb.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gwu.dianchejie.cn

[S36] C++：unordered_map
来源：http://pjj.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nbk.hnqzz.top


<!-- 参考信息 -->