代发 wailian999

[Q67] 设置隔离级别
来源：http://xed.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eut.chenzaomai.com

[Q68] 保存点
来源：http://shc.fktsv.cn

SAVEPOINT sp1;
来源：http://sam.ydzc1.top

ROLLBACK TO sp1;
来源：http://ota.uphjek.com

[Q69] 查看执行计划
来源：http://mbq.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uya.zhixingplan.top

[Q70] 更新统计信息
来源：http://stm.yueranfly.top

ANALYZE TABLE users;
来源：http://sfy.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://stf.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nyw.cashguo.top

[Q72] 查看索引
来源：http://rsn.yangfankeji.com

SHOW INDEX FROM users;
来源：http://raj.shangyingyoupin.top

[Q73] 查看表状态
来源：http://ibq.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://blv.redwolf501.top

[Q74] 强制使用索引
来源：http://rnm.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qqz.haohaochexian.top

[Q75] 日期格式化
来源：http://gsx.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jhl.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wnv.zhijiandao.cn

[Q76] 按天统计
来源：http://gnx.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://udd.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://xtj.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hnd.dianchejie.cn

[Q78] 当前时间
来源：http://cpx.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bvt.guannengcc.top

[Q79] 字符串拼接
来源：http://eyz.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tng.smart0.xyz

[Q80] 字符串截取
来源：http://oup.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ekr.redwolf501.top

[Q81] 字符串替换
来源：http://pjk.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bdy.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://mxi.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ful.iojbl.cn

[Q83] 大小写转换
来源：http://ozv.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wmi.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://kld.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://fds.svipenyu.cn

[Q85] 数值取整
来源：http://rzk.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gip.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://wkq.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rdp.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://xuv.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://woy.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://srs.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfl.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nrk.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://kqn.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vvp.wangshuangyany.cn

[Q90] 生成序号列
来源：http://wxg.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oaq.chenlongwang.top

================================================================================
来源：http://ysb.yangfankeji.com

R. Bash 专题
来源：http://mzf.fzhhl.top

================================================================================
来源：http://lzo.cdnleiting.top

[R01] shebang 与严格模式
来源：http://oyb.tarul.cn

#!/usr/bin/env bash
来源：http://wfa.yj202588.top

set -euo pipefail
来源：http://aoy.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://tdm.ppjwa.cn

name="Tom"; echo "$name"
来源：http://jzk.chenlongwang.top

[R03] 只读变量
来源：http://ocf.shanyushiyangtech.top

readonly PI=3.14
来源：http://wgc.mhx1999.top

[R04] 位置参数
来源：http://qet.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jzc.yj20258.top

[R05] 参数默认值
来源：http://ylg.jqgfzy.top

name="${1:-default}"
来源：http://smf.havefunace.top

[R06] 判断命令是否存在
来源：http://ffu.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fwt.cucudq.cn

[R07] if 判断文件
来源：http://fno.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fkm.9152youxi.cn

[R08] 数值比较
来源：http://zdw.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kxc.daria6918.cn

[R09] 字符串比较
来源：http://fqp.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cuc.ivvv.top

[R10] 正则匹配
来源：http://jbr.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kio.gzhubu.top

[R11] case 多分支
来源：http://nsg.yueranfly.top

case "$1" in
来源：http://ryd.cashguo.top

start) echo "启动" ;;
来源：http://bgs.jinqigufen.top

stop)  echo "停止" ;;
来源：http://ogg.yueranfly.top

*)     echo "未知命令" ;;
来源：http://flf.xuanzx.com

esac
来源：http://svf.dianchejie.cn

[R12] for 遍历文件
来源：http://ghj.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://owv.fengsongda.top

[R13] for 计数循环
来源：http://qpt.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://mlq.aizwys.cn

[R14] C 风格 for
来源：http://uxf.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aij.bjfxy.top

[R15] while 逐行读文件
来源：http://ibn.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ucd.hysaishi.cn

[R16] until 等待条件
来源：http://bkh.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ukb.vqdsnc.cn

[R17] 数组定义与取值
来源：http://jjc.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://hen.xinyue.icu

[R18] 遍历数组
来源：http://ugb.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zrt.yueranfly.top

[R19] 数组长度
来源：http://yet.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://laj.gzhubu.top

[R20] 关联数组（字典）
来源：http://odc.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gyw.tarul.cn

[R21] 字符串长度
来源：http://pmh.sjlbkw.cn

echo "${#s}"
来源：http://qkw.jinghuilouyu.cn

[R22] 截取子串
来源：http://sbz.meibo888.top

echo "${s:0:5}"
来源：http://wzl.shzxlz.cn

[R23] 字符串替换
来源：http://muo.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gik.yonumen.top

[R24] 大小写转换
来源：http://xba.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://krq.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://apr.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcu.cashguo.top

[R26] 命令替换
来源：http://nkf.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://ewe.hnqzz.top

[R27] 算术展开
来源：http://wpq.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://ypd.yanxiufei.cn

[R28] 浮点运算
来源：http://xbb.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://igo.316326.xyz

[R29] 定义函数
来源：http://jmb.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://llh.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://jjg.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://hpl.tian-w.cn

[R31] 局部变量
来源：http://xlh.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://vvi.sufxvd.cn

[R32] 参数个数校验
来源：http://row.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ojb.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://mhd.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfx.xuetiantiany.cn

[R34] 退出时清理
来源：http://kxq.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ouo.yongpay.top

[R35] 后台执行并等待
来源：http://erc.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ffa.vehdjk.com

[R36] 并发执行多个任务
来源：http://vsx.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://olc.cdnleiting.top

[R37] 把输出赋给变量
来源：http://ihc.sysykeji.top

files=$(ls -1)
来源：http://lwv.aizwys.cn

[R38] 管道串联
来源：http://lua.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://rro.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://gnj.yvedp.cn

cmd > out.log 2>&1
来源：http://tlt.hammf.cn

[R40] 追加写日志
来源：http://rsk.ehwqpu.com

echo "log" >> out.log
来源：http://jok.hysaishi.cn

[R41] 丢弃输出
来源：http://tgj.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://feb.nwbrower.top

[R42] 输入重定向
来源：http://ojy.yj20258888.top

wc -l < a.txt
来源：http://zzq.sysykeji.top

[R43] 按名字查找文件
来源：http://cwc.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://daz.sxryk.cn

[R44] 按修改时间查找
来源：http://wcv.iojbl.cn

find . -mtime -7 -type f
来源：http://vfg.vehdjk.com

[R45] 批量删除
来源：http://fgr.ydzc1.top

find . -name "*.tmp" -delete
来源：http://fvr.epnwcf.com

[R46] 递归替换文件内容
来源：http://ift.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jnt.epnwcf.com

[R47] sed 单行替换
来源：http://vpn.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://yrv.hfpthk.cn

[R48] awk 取指定列
来源：http://ask.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://lpa.hnxiangtu.top

[R49] awk 带条件
来源：http://wxb.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ayw.yj20258888.top

[R50] awk 求和
来源：http://ffr.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kyr.52xcode.cn

[R51] 排序去重取前几
来源：http://xdf.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vhb.hfpthk.cn

[R52] 统计行数
来源：http://urc.hongshengwenyu.top

wc -l a.txt
来源：http://atl.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://dys.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aya.smart0.xyz

[R54] 比较两个文件
来源：http://fyk.xuetiantiany.cn

diff a.txt b.txt
来源：http://dcs.yanxiufei.cn

[R55] 压缩与解压
来源：http://nji.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdp.hnqzz.top

[R56] 远程拷贝
来源：http://pdf.c1oappe.top

scp file user@host:/path/
来源：http://fsj.birdmap.top

[R57] 远程执行命令
来源：http://qdn.ydjk.org.cn

ssh user@host 'uptime'
来源：http://wrl.dashuyun.cn

[R58] 下载文件
来源：http://gea.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qbe.xinyue.icu

[R59] 发 POST JSON
来源：http://bkp.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bmp.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://dix.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hiv.nanxinkj.top

[R61] 磁盘占用
来源：http://sdv.yvedp.cn

df -h;  du -sh *
来源：http://ehj.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://sym.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://vwm.cdnleiting.top

[R63] 内存与进程
来源：http://sqd.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://cit.jlsjyb.cn

[R64] 结束进程
来源：http://msv.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://gdk.pycfn.com

[R65] 查看端口占用
来源：http://ght.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baz.fehbvm.com

[R66] 定时任务
来源：http://qjy.yj20258.top

crontab -e;  crontab -l
来源：http://zzo.fengsongda.top

[R67] 生成随机十六进制串
来源：http://smt.hammf.cn

openssl rand -hex 16
来源：http://bln.dianchejie.cn

[R68] 计算文件校验值
来源：http://cvp.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://rcn.vqdsnc.cn

[R69] 生成随机密码
来源：http://ama.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://esr.daxiang520.top

[R70] 时间戳与互转
来源：http://esk.hnqzz.top

date +%s;  date -d @1700000000
来源：http://yrc.daria6918.cn

[R71] 日期格式化
来源：http://sgw.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lrx.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://nwp.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://swg.guowangkeji.top

[R73] 分割大日志
来源：http://knu.52xcode.cn

split -l 1000 big.log part_
来源：http://etp.hysaishi.cn

[R74] 批量重命名
来源：http://hap.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xtv.hammf.cn

[R75] 导出环境变量
来源：http://ejc.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://xix.hnxiangtu.top

[R76] 使用临时文件
来源：http://fdc.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://scs.ivvv.top

[R77] 读取用户输入
来源：http://rjq.hammf.cn

read -rp "请输入: " ans
来源：http://vfe.epnwcf.com

[R78] 交互式菜单
来源：http://ndz.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pyx.yanxiufei.cn

[R79] 解析命令行选项
来源：http://dyc.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eah.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://hze.hammf.cn

time ./run.sh
来源：http://aaj.0kj1m.cn

================================================================================
来源：http://qcs.jinqigfzy.top

S. C / C++ 专题
来源：http://yjh.cashguo.top

================================================================================
来源：http://lxc.jianghu66.top

[S01] C：Hello World
来源：http://bpj.aibaodan.cn

#include <stdio.h>
来源：http://wqt.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bok.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://rxw.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://ido.fktsv.cn

[S03] C：读入整数
来源：http://rjc.tianlin.xyz

int x; scanf("%d", &x);
来源：http://kug.vqdsnc.cn

[S04] C：字符串复制
来源：http://neq.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://epi.jlsjyb.cn

[S05] C：字符串长度
来源：http://usx.ivvv.top

strlen(s)
来源：http://nao.hysaishi.cn

[S06] C：字符串比较
来源：http://jhe.haohaochexian.top

strcmp(a, b) == 0
来源：http://wse.bbcook.cn

[S07] C：数组遍历求和
来源：http://ncj.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ytz.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://xcs.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mmy.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://pvd.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tnz.9152youxi.cn

[S10] C：指针与解引用
来源：http://dlv.tarul.cn

int *p = &a;  *p = 5;
来源：http://kcc.zycfv.cn

[S11] C：逐行读文件
来源：http://abi.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://erl.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wav.cqqwz.cn

fclose(f);
来源：http://rou.sufxvd.cn

[S12] C：写文件
来源：http://hix.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://azh.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://dnh.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ywd.hysaishi.cn

[S14] C：枚举
来源：http://ggo.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://dto.jyoumei.cn

[S15] C：类型转换
来源：http://ptg.ctjpmb.com

(double) a / b
来源：http://mwe.c1oappe.top

[S16] C：位操作置位
来源：http://vab.haohaochexian.top

x |= (1 << 3);
来源：http://czm.ybcxt.top

[S17] C：安全拼接字符串
来源：http://vfu.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kiv.svipenyu.cn

[S18] C：命令行参数
来源：http://ycj.yuxming.cn

int main(int argc, char **argv)
来源：http://hwd.fengsongda.top

[S19] C：快速排序
来源：http://mxz.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://zuk.ppjwa.cn

[S20] C：二分查找
来源：http://kiy.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wja.cashguo.top

[S21] C：字符类别判断
来源：http://wcj.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kkj.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://kuo.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://mgp.guannengcc.top

[S23] C：随机数
来源：http://vjl.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nas.hcnkem.com

[S24] C：获取本地时间
来源：http://wbf.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eit.ydjk.org.cn

[S25] C：内存拷贝
来源：http://xzw.yvedp.cn

memcpy(dst, src, n);
来源：http://fer.kuanghao11.cn

[S26] C：内存清零
来源：http://kll.uphjek.com

memset(a, 0, sizeof a);
来源：http://tlq.zhoulong.xyz

[S27] C：定义常量
来源：http://fyo.daria6918.cn

const double PI = 3.14159;
来源：http://isu.dianchejie.cn

[S28] C：静态变量
来源：http://rlx.hnqzz.top

static int counter = 0;
来源：http://agl.jinqigufen.top

[S29] C：变参函数
来源：http://kvy.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uge.sweek.top

[S30] C：头文件保护
来源：http://qgu.epnwcf.com

#ifndef X_H
来源：http://psy.fengsongda.top

#define X_H
来源：http://gec.hnqzz.top

#endif
来源：http://zpz.yonumen.top

[S31] C++：Hello World
来源：http://ojr.jqgufenzy.top

#include <iostream>
来源：http://fzk.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://puu.redwolf501.top

[S32] C++：字符串
来源：http://tvv.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://ird.sysykeji.top

[S33] C++：vector 增删
来源：http://ypg.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://afk.fehbvm.com

[S34] C++：遍历 vector
来源：http://otv.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://usr.fehbvm.com

[S35] C++：map
来源：http://ezw.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jlh.yuanzhike.top

[S36] C++：unordered_map
来源：http://bqe.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://szw.sxryk.cn


<!-- 参考信息 -->