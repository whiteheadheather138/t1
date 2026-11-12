代发 wailian999

[Q65] 回滚事务
来源：http://hmd.zhongyouzk.top

ROLLBACK;
来源：http://zjm.316326.xyz

[Q66] 行锁查询
来源：http://spc.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zff.sufxvd.cn

[Q67] 设置隔离级别
来源：http://ubu.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ckm.9152youxi.cn

[Q68] 保存点
来源：http://pdu.c1oappe.top

SAVEPOINT sp1;
来源：http://sts.fengsongda.top

ROLLBACK TO sp1;
来源：http://xaa.pycfn.com

[Q69] 查看执行计划
来源：http://yyy.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zwk.zhixingplan.top

[Q70] 更新统计信息
来源：http://lgs.zdbjq.cn

ANALYZE TABLE users;
来源：http://myt.zycfv.cn

[Q71] 查看建表语句
来源：http://oao.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kaw.uphjek.com

[Q72] 查看索引
来源：http://fit.daria6918.cn

SHOW INDEX FROM users;
来源：http://maq.vehdjk.com

[Q73] 查看表状态
来源：http://mmw.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xpv.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://imr.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mzb.cqqwz.cn

[Q75] 日期格式化
来源：http://jzy.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tcj.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zaf.fengsongda.top

[Q76] 按天统计
来源：http://xvs.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://orv.jyoumei.cn

[Q77] 时间加减
来源：http://xkp.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sjq.0kj1m.cn

[Q78] 当前时间
来源：http://lhc.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vwr.vehdjk.com

[Q79] 字符串拼接
来源：http://jau.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xhp.meibo888.top

[Q80] 字符串截取
来源：http://cbq.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qnp.guannengcc.top

[Q81] 字符串替换
来源：http://ydf.aizwys.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dkp.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://doc.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qgz.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://fgi.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gvz.yuanzhike.top

[Q84] 去除首尾空格
来源：http://zxo.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://qqu.ybcxt.top

[Q85] 数值取整
来源：http://pke.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://njh.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://gwc.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gie.epnwcf.com

[Q87] JSON 字段做条件
来源：http://jcl.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eia.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://xxf.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fvh.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sks.redwolf501.top

[Q89] 判断表是否存在
来源：http://tnm.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://exw.uphjek.com

[Q90] 生成序号列
来源：http://cct.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nzo.smart0.xyz

================================================================================
来源：http://kvk.yongpay.top

R. Bash 专题
来源：http://tfs.nanxuanxn.top

================================================================================
来源：http://vlz.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://oar.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://jgm.quarkkingdee.top

set -euo pipefail
来源：http://cqv.zhengqikj.top

[R02] 变量赋值与使用
来源：http://fph.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://iip.ppjwa.cn

[R03] 只读变量
来源：http://hlh.yj202588.top

readonly PI=3.14
来源：http://bmi.yfazqb.com

[R04] 位置参数
来源：http://fdi.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dtj.vqdsnc.cn

[R05] 参数默认值
来源：http://ngm.sufxvd.cn

name="${1:-default}"
来源：http://mbh.chenzaomai.com

[R06] 判断命令是否存在
来源：http://wyk.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kbw.kuanghao11.cn

[R07] if 判断文件
来源：http://wxs.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sqe.sweek.top

[R08] 数值比较
来源：http://gnz.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fln.wangshuangyany.cn

[R09] 字符串比较
来源：http://xya.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kjn.ybcxt.top

[R10] 正则匹配
来源：http://cia.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fuv.ydzc1.top

[R11] case 多分支
来源：http://iqi.jqgufenzy.top

case "$1" in
来源：http://bbf.zhongyouzk.top

start) echo "启动" ;;
来源：http://uay.316326.xyz

stop)  echo "停止" ;;
来源：http://eew.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://had.yanxiufei.cn

esac
来源：http://eed.hywenlv.cn

[R12] for 遍历文件
来源：http://epu.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://bau.ydjk.org.cn

[R13] for 计数循环
来源：http://jie.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://yxt.jqgfzy.top

[R14] C 风格 for
来源：http://eyx.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pmo.c1oappe.top

[R15] while 逐行读文件
来源：http://bqj.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ekw.andypj.xyz

[R16] until 等待条件
来源：http://sry.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pyo.jinqigfzy.top

[R17] 数组定义与取值
来源：http://ulo.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://chk.jqgufenzy.top

[R18] 遍历数组
来源：http://sjf.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vkk.pengpengdd.cyou

[R19] 数组长度
来源：http://lhg.hnqzz.top

echo "${#arr[@]}"
来源：http://vhb.cdnleiting.top

[R20] 关联数组（字典）
来源：http://uyj.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfw.shuidangran.top

[R21] 字符串长度
来源：http://tgu.shanyushiyangkeji.top

echo "${#s}"
来源：http://yjt.zhoulong.xyz

[R22] 截取子串
来源：http://crg.52xcode.cn

echo "${s:0:5}"
来源：http://oru.ctjpmb.com

[R23] 字符串替换
来源：http://gfx.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zfw.yvedp.cn

[R24] 大小写转换
来源：http://zdp.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lmd.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://oik.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ojy.smart0.xyz

[R26] 命令替换
来源：http://omh.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://bzl.tianlin.xyz

[R27] 算术展开
来源：http://umd.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://myv.sjlbkw.cn

[R28] 浮点运算
来源：http://dkm.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://qgz.jiagoushi.top

[R29] 定义函数
来源：http://jmt.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hcz.shzxlz.cn

[R30] 函数返回状态码
来源：http://idv.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://pga.c1oappe.top

[R31] 局部变量
来源：http://ezv.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://cph.wangshuangyany.cn

[R32] 参数个数校验
来源：http://vlr.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bio.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://qxe.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ymo.sjlbkw.cn

[R34] 退出时清理
来源：http://mpg.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://paj.pycfn.com

[R35] 后台执行并等待
来源：http://qwy.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kuu.9152youxi.cn

[R36] 并发执行多个任务
来源：http://jqu.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jmy.snrcjt.cn

[R37] 把输出赋给变量
来源：http://dhh.ehwqpu.com

files=$(ls -1)
来源：http://aps.andypj.xyz

[R38] 管道串联
来源：http://non.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://aky.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://zjn.fengsongda.top

cmd > out.log 2>&1
来源：http://gby.birdmap.top

[R40] 追加写日志
来源：http://ofs.quarkkingdee.top

echo "log" >> out.log
来源：http://qtw.yj202588.top

[R41] 丢弃输出
来源：http://twp.shuidangran.top

cmd >/dev/null 2>&1
来源：http://nyg.hfpthk.cn

[R42] 输入重定向
来源：http://wns.guannengcc.top

wc -l < a.txt
来源：http://aua.chenzaomai.com

[R43] 按名字查找文件
来源：http://rnp.ctjpmb.com

find . -name "*.log" -type f
来源：http://eot.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://qrb.smart0.xyz

find . -mtime -7 -type f
来源：http://zhn.xuanzx.com

[R45] 批量删除
来源：http://kgi.ivvv.top

find . -name "*.tmp" -delete
来源：http://mpu.chenzaomai.com

[R46] 递归替换文件内容
来源：http://chb.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uph.fengsongda.top

[R47] sed 单行替换
来源：http://diz.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://bom.guannengcc.top

[R48] awk 取指定列
来源：http://rtr.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://fhh.aizwys.cn

[R49] awk 带条件
来源：http://fhx.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lrv.yongpay.top

[R50] awk 求和
来源：http://bdt.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nri.yuanzhike.top

[R51] 排序去重取前几
来源：http://jbt.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://awj.jqgfzy.top

[R52] 统计行数
来源：http://seg.zhixingplan.top

wc -l a.txt
来源：http://itu.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://jxb.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gfg.gogol.net.cn

[R54] 比较两个文件
来源：http://ttu.fengsongda.top

diff a.txt b.txt
来源：http://due.iojbl.cn

[R55] 压缩与解压
来源：http://mfx.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://scd.ivvv.top

[R56] 远程拷贝
来源：http://gxu.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://bss.nanxinkj.top

[R57] 远程执行命令
来源：http://cod.iojbl.cn

ssh user@host 'uptime'
来源：http://jnn.gzhubu.top

[R58] 下载文件
来源：http://yma.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pdi.tanke756.top

[R59] 发 POST JSON
来源：http://hmz.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ylb.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://bax.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xva.hammf.cn

[R61] 磁盘占用
来源：http://zpl.hongshengwenyu.top

df -h;  du -sh *
来源：http://wew.nanxinkj.top

[R62] 找最占空间的文件
来源：http://vki.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://gns.snrcjt.cn

[R63] 内存与进程
来源：http://mox.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://agx.bjfxy.top

[R64] 结束进程
来源：http://urp.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://hez.epnwcf.com

[R65] 查看端口占用
来源：http://qqg.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nbp.hywenlv.cn

[R66] 定时任务
来源：http://zzs.ydzc1.top

crontab -e;  crontab -l
来源：http://ghl.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://xor.fzhhl.top

openssl rand -hex 16
来源：http://zce.kuanghao11.cn

[R68] 计算文件校验值
来源：http://rur.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rak.xuetiantiany.cn

[R69] 生成随机密码
来源：http://ezk.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://lgt.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://nki.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://pgm.gaohongyu789.top

[R71] 日期格式化
来源：http://sgp.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tvb.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://uzo.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aqf.yongpay.top

[R73] 分割大日志
来源：http://boq.gzhubu.top

split -l 1000 big.log part_
来源：http://lmp.vehdjk.com

[R74] 批量重命名
来源：http://msg.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqm.fzhhl.top

[R75] 导出环境变量
来源：http://jmv.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://boe.cucudq.cn

[R76] 使用临时文件
来源：http://ame.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ddh.daria6918.cn

[R77] 读取用户输入
来源：http://bgr.yj202588.top

read -rp "请输入: " ans
来源：http://bxd.hnqzz.top

[R78] 交互式菜单
来源：http://swd.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eqp.tanke756.top

[R79] 解析命令行选项
来源：http://wmi.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eyg.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://xxf.svipenyu.cn

time ./run.sh
来源：http://ncr.shanyushiyangtech.top

================================================================================
来源：http://anz.hnqzz.top

S. C / C++ 专题
来源：http://xrc.fehbvm.com

================================================================================
来源：http://tky.birdmap.top

[S01] C：Hello World
来源：http://tnk.9152youxi.cn

#include <stdio.h>
来源：http://tph.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nih.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://zeg.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://cbg.316326.xyz

[S03] C：读入整数
来源：http://nus.yueranfly.top

int x; scanf("%d", &x);
来源：http://fts.cashguo.top

[S04] C：字符串复制
来源：http://ftf.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://mmx.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://dtz.shanyushiyangkeji.top

strlen(s)
来源：http://uqb.c1oappe.top

[S06] C：字符串比较
来源：http://gax.guannengcc.top

strcmp(a, b) == 0
来源：http://vid.birdmap.top

[S07] C：数组遍历求和
来源：http://cxe.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lok.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://kuq.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tqx.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://ogh.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mae.sweek.top

[S10] C：指针与解引用
来源：http://mfi.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://ujw.hywenlv.cn

[S11] C：逐行读文件
来源：http://stj.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://jfk.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mfd.zycfv.cn

fclose(f);
来源：http://jnn.yj20258.top

[S12] C：写文件
来源：http://eop.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sxc.daxiang520.top

[S13] C：宏定义
来源：http://osj.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nss.shzxlz.cn

[S14] C：枚举
来源：http://sxq.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://okm.shuidangran.top

[S15] C：类型转换
来源：http://ntk.zhiwuduotai.top

(double) a / b
来源：http://frv.zhongyouzk.top

[S16] C：位操作置位
来源：http://yfr.tianlin.xyz

x |= (1 << 3);
来源：http://yle.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://rtx.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wak.fzhhl.top

[S18] C：命令行参数
来源：http://ups.yuanzhike.top

int main(int argc, char **argv)
来源：http://bao.jiagoushi.top

[S19] C：快速排序
来源：http://lwu.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://khr.svipenyu.cn

[S20] C：二分查找
来源：http://lhe.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mcp.xziqi.cn

[S21] C：字符类别判断
来源：http://vky.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://avn.epnwcf.com

[S22] C：字符串转数字
来源：http://jjl.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://sdy.yvedp.cn

[S23] C：随机数
来源：http://yig.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://qjc.meibo888.top

[S24] C：获取本地时间
来源：http://lol.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dsg.sweek.top

[S25] C：内存拷贝
来源：http://itp.aibaodan.cn

memcpy(dst, src, n);
来源：http://tgr.shanyushiyangtech.top

[S26] C：内存清零
来源：http://crb.shuidangran.top

memset(a, 0, sizeof a);
来源：http://cho.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://cob.hesvh.cn

const double PI = 3.14159;
来源：http://fqu.ydzc1.top

[S28] C：静态变量
来源：http://zqu.havefunace.top

static int counter = 0;
来源：http://rzs.jiagoushi.top

[S29] C：变参函数
来源：http://npw.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jdb.zhengqikj.top

[S30] C：头文件保护
来源：http://zne.ehwqpu.com

#ifndef X_H
来源：http://vcj.gogol.net.cn

#define X_H
来源：http://uyv.316326.xyz

#endif
来源：http://pzn.jqgfzy.top

[S31] C++：Hello World
来源：http://ixj.xylfe.cn

#include <iostream>
来源：http://zuv.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://joi.yuanzhike.top

[S32] C++：字符串
来源：http://hsi.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://cyg.jyoumei.cn

[S33] C++：vector 增删
来源：http://bfg.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://snm.yj20258888.top

[S34] C++：遍历 vector
来源：http://ytc.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://txy.wangdashe.top


<!-- 参考信息 -->