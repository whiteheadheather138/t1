代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xpz.snrcjt.cn

[Q58] 累计求和
来源：http://aou.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fso.chenlongwang.top

[Q59] 分组内累计
来源：http://xwb.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wdm.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://fwq.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tmh.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yus.ivvv.top

[Q61] 移动平均
来源：http://crx.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://otj.hnxiangtu.top

[Q62] 分组占比
来源：http://dos.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wzo.gogol.net.cn

[Q63] 开启事务
来源：http://rsj.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://odz.hnxiangtu.top

[Q64] 提交事务
来源：http://wyl.yj202588.top

COMMIT;
来源：http://bdb.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://xmz.iojbl.cn

ROLLBACK;
来源：http://ycc.gogol.net.cn

[Q66] 行锁查询
来源：http://sed.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yzr.yonumen.top

[Q67] 设置隔离级别
来源：http://vdy.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jry.ehwqpu.com

[Q68] 保存点
来源：http://qek.iojbl.cn

SAVEPOINT sp1;
来源：http://rfh.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://fsb.aibaodan.cn

[Q69] 查看执行计划
来源：http://qji.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://swh.yuxming.cn

[Q70] 更新统计信息
来源：http://nlc.yuxming.cn

ANALYZE TABLE users;
来源：http://otq.chenzaomai.com

[Q71] 查看建表语句
来源：http://dnj.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zon.iojbl.cn

[Q72] 查看索引
来源：http://psw.snrcjt.cn

SHOW INDEX FROM users;
来源：http://qnc.daria6918.cn

[Q73] 查看表状态
来源：http://pgn.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hea.svipenyu.cn

[Q74] 强制使用索引
来源：http://rzx.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ctz.hywenlv.cn

[Q75] 日期格式化
来源：http://gfh.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwq.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cdv.jyoumei.cn

[Q76] 按天统计
来源：http://zim.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yts.jianghu66.top

[Q77] 时间加减
来源：http://ael.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kal.nwbrower.top

[Q78] 当前时间
来源：http://ypl.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uft.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://iwu.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fhs.zhijiandao.cn

[Q80] 字符串截取
来源：http://rrk.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yap.guannengcc.top

[Q81] 字符串替换
来源：http://qeb.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qfv.yj20258.top

[Q82] 字符长度与字节长度
来源：http://cof.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ixj.guowangkeji.top

[Q83] 大小写转换
来源：http://ldm.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jgq.daxiang520.top

[Q84] 去除首尾空格
来源：http://tjn.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://rcu.epnwcf.com

[Q85] 数值取整
来源：http://wav.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ril.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://flk.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mrn.yongpay.top

[Q87] JSON 字段做条件
来源：http://vru.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vsb.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://nki.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qyw.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://phq.yfazqb.com

[Q89] 判断表是否存在
来源：http://gpp.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://auj.hongshengwenyu.top

[Q90] 生成序号列
来源：http://icj.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmr.nwbrower.top

================================================================================
来源：http://ubh.fzhhl.top

R. Bash 专题
来源：http://lgz.quarkkingdee.top

================================================================================
来源：http://zek.pycfn.com

[R01] shebang 与严格模式
来源：http://lam.hesvh.cn

#!/usr/bin/env bash
来源：http://ieo.smart0.xyz

set -euo pipefail
来源：http://fkq.yfazqb.com

[R02] 变量赋值与使用
来源：http://dne.hywenlv.cn

name="Tom"; echo "$name"
来源：http://bzf.zhixingplan.top

[R03] 只读变量
来源：http://nwp.zdqjudy.top

readonly PI=3.14
来源：http://bqr.snrcjt.cn

[R04] 位置参数
来源：http://bnu.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pjz.ybcxt.top

[R05] 参数默认值
来源：http://voa.zhongyouzk.top

name="${1:-default}"
来源：http://ulp.vehdjk.com

[R06] 判断命令是否存在
来源：http://zsg.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rwz.xuanzx.com

[R07] if 判断文件
来源：http://hrm.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://umd.hongshengwenyu.top

[R08] 数值比较
来源：http://gkm.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://znw.pycfn.com

[R09] 字符串比较
来源：http://piv.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://icq.zhixingplan.top

[R10] 正则匹配
来源：http://wdb.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rkr.wangshuangyany.cn

[R11] case 多分支
来源：http://mmd.aizwys.cn

case "$1" in
来源：http://urj.ybcxt.top

start) echo "启动" ;;
来源：http://kvo.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://kdr.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://shu.iojbl.cn

esac
来源：http://kvh.gaohongyu789.top

[R12] for 遍历文件
来源：http://hqa.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://rkz.fzhhl.top

[R13] for 计数循环
来源：http://fzm.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://jjz.fzhhl.top

[R14] C 风格 for
来源：http://ncs.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qwy.svipenyu.cn

[R15] while 逐行读文件
来源：http://dkj.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xab.gotoacloud.top

[R16] until 等待条件
来源：http://tus.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dvv.bbcook.cn

[R17] 数组定义与取值
来源：http://mmg.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bsv.fzhhl.top

[R18] 遍历数组
来源：http://npm.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vfs.ydjk.org.cn

[R19] 数组长度
来源：http://jcx.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://aay.ydzc1.top

[R20] 关联数组（字典）
来源：http://xsu.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qpb.ctjpmb.com

[R21] 字符串长度
来源：http://fed.jianghu66.top

echo "${#s}"
来源：http://pjz.sysykeji.top

[R22] 截取子串
来源：http://uup.zhongyouzk.top

echo "${s:0:5}"
来源：http://eid.zhijiandao.cn

[R23] 字符串替换
来源：http://oeu.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nun.wangdashe.top

[R24] 大小写转换
来源：http://qkv.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://syj.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://swa.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcc.pycfn.com

[R26] 命令替换
来源：http://iay.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://exa.dianchejie.cn

[R27] 算术展开
来源：http://pne.xziqi.cn

echo $((1 + 2 * 3))
来源：http://xct.sysykeji.top

[R28] 浮点运算
来源：http://pzs.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://pqs.ybcxt.top

[R29] 定义函数
来源：http://vjn.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://shm.dianchejie.cn

[R30] 函数返回状态码
来源：http://qap.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://lsy.quarkkingdee.top

[R31] 局部变量
来源：http://jsh.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://obk.pengpengdd.cyou

[R32] 参数个数校验
来源：http://llr.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kyy.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://shf.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pcs.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://rjr.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://gxe.zhengqikj.top

[R35] 后台执行并等待
来源：http://shh.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://scq.jianghu66.top

[R36] 并发执行多个任务
来源：http://bvi.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mtt.ehwqpu.com

[R37] 把输出赋给变量
来源：http://rgp.hcnkem.com

files=$(ls -1)
来源：http://cwu.fengsongda.top

[R38] 管道串联
来源：http://tad.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://rgi.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://mqn.shuidangran.top

cmd > out.log 2>&1
来源：http://bhb.fktsv.cn

[R40] 追加写日志
来源：http://ker.smart0.xyz

echo "log" >> out.log
来源：http://gkv.xylfe.cn

[R41] 丢弃输出
来源：http://tga.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://ezp.jinqigufen.top

[R42] 输入重定向
来源：http://ueb.cdnleiting.top

wc -l < a.txt
来源：http://ptx.yj202588.top

[R43] 按名字查找文件
来源：http://kkx.hcnkem.com

find . -name "*.log" -type f
来源：http://orc.ppjwa.cn

[R44] 按修改时间查找
来源：http://ugl.yj20258888.top

find . -mtime -7 -type f
来源：http://owo.chenjidiqi.icu

[R45] 批量删除
来源：http://ano.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://hrr.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://lxe.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zdd.nanxinkj.top

[R47] sed 单行替换
来源：http://qpi.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://omh.dianchejie.cn

[R48] awk 取指定列
来源：http://yzx.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://sfi.jlsjyb.cn

[R49] awk 带条件
来源：http://qwy.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://erf.zhengqikj.top

[R50] awk 求和
来源：http://row.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uwg.sufxvd.cn

[R51] 排序去重取前几
来源：http://jpw.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sdc.guowangkeji.top

[R52] 统计行数
来源：http://hnx.daxiang520.top

wc -l a.txt
来源：http://lko.tanke756.top

[R53] 查看文件头与实时尾
来源：http://cak.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iak.sweek.top

[R54] 比较两个文件
来源：http://qtl.zycfv.cn

diff a.txt b.txt
来源：http://iwg.guowangkeji.top

[R55] 压缩与解压
来源：http://wab.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dnx.uphjek.com

[R56] 远程拷贝
来源：http://thf.gzhubu.top

scp file user@host:/path/
来源：http://gbp.zdqjudy.top

[R57] 远程执行命令
来源：http://qcp.pycfn.com

ssh user@host 'uptime'
来源：http://idq.sysykeji.top

[R58] 下载文件
来源：http://kbk.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cex.sxryk.cn

[R59] 发 POST JSON
来源：http://pvc.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ncp.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://ism.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zmp.fengsongda.top

[R61] 磁盘占用
来源：http://hej.c1oappe.top

df -h;  du -sh *
来源：http://rkr.ppjwa.cn

[R62] 找最占空间的文件
来源：http://jcn.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://dxp.yueranfly.top

[R63] 内存与进程
来源：http://xru.tanke756.top

free -h;  ps aux | grep nginx
来源：http://jtz.zdqjudy.top

[R64] 结束进程
来源：http://gxm.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://ioa.xinyue.icu

[R65] 查看端口占用
来源：http://vmn.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zxi.yongpay.top

[R66] 定时任务
来源：http://ebc.jyoumei.cn

crontab -e;  crontab -l
来源：http://vbd.yj202588.top

[R67] 生成随机十六进制串
来源：http://jlg.jinghuilouyu.cn

openssl rand -hex 16
来源：http://okv.gotoacloud.top

[R68] 计算文件校验值
来源：http://noq.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hdg.yongpay.top

[R69] 生成随机密码
来源：http://bmg.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://uzy.fktsv.cn

[R70] 时间戳与互转
来源：http://cvb.c1oappe.top

date +%s;  date -d @1700000000
来源：http://kep.yfazqb.com

[R71] 日期格式化
来源：http://bup.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ljq.fzhhl.top

[R72] 等待端口就绪
来源：http://rww.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://emg.fehbvm.com

[R73] 分割大日志
来源：http://pie.jyoumei.cn

split -l 1000 big.log part_
来源：http://nim.hywenlv.cn

[R74] 批量重命名
来源：http://bxl.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iza.52xcode.cn

[R75] 导出环境变量
来源：http://hhf.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://haf.cqqwz.cn

[R76] 使用临时文件
来源：http://tln.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xrl.jlsjyb.cn

[R77] 读取用户输入
来源：http://ogn.ydzc1.top

read -rp "请输入: " ans
来源：http://mon.epnwcf.com

[R78] 交互式菜单
来源：http://dic.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mob.9152youxi.cn

[R79] 解析命令行选项
来源：http://tbf.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vij.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://xxa.chenzaomai.com

time ./run.sh
来源：http://sde.nanxinkj.top

================================================================================
来源：http://zsk.hcnkem.com

S. C / C++ 专题
来源：http://doo.jyoumei.cn

================================================================================
来源：http://ldv.cashguo.top

[S01] C：Hello World
来源：http://tsu.smart0.xyz

#include <stdio.h>
来源：http://qht.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fyt.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://pmz.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://atf.tanke756.top

[S03] C：读入整数
来源：http://kih.hysaishi.cn

int x; scanf("%d", &x);
来源：http://cxh.chenzaomai.com

[S04] C：字符串复制
来源：http://rrs.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://gyn.fzhhl.top

[S05] C：字符串长度
来源：http://vri.jlsjyb.cn

strlen(s)
来源：http://xmu.uphjek.com

[S06] C：字符串比较
来源：http://wfw.9152youxi.cn

strcmp(a, b) == 0
来源：http://zxu.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://jpp.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lsu.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://lwn.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tnw.cheryme.top

[S09] C：结构体定义与初始化
来源：http://qxl.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://idf.zhengqikj.top

[S10] C：指针与解引用
来源：http://uoc.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://hdf.hywenlv.cn

[S11] C：逐行读文件
来源：http://kzl.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://ahr.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zxx.cqqwz.cn

fclose(f);
来源：http://dwx.xylfe.cn

[S12] C：写文件
来源：http://upu.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kax.zhixingplan.top

[S13] C：宏定义
来源：http://net.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oyk.9152youxi.cn

[S14] C：枚举
来源：http://gtv.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://dwx.bjfxy.top

[S15] C：类型转换
来源：http://nib.sjlbkw.cn

(double) a / b
来源：http://sqr.pengpengdd.cyou

[S16] C：位操作置位
来源：http://faw.zhiwuduotai.top

x |= (1 << 3);
来源：http://lpp.guannengcc.top

[S17] C：安全拼接字符串
来源：http://uvl.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bvc.gaohongyu789.top

[S18] C：命令行参数
来源：http://vmr.xuanzx.com

int main(int argc, char **argv)
来源：http://cig.tarul.cn

[S19] C：快速排序
来源：http://flp.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ejm.yuanzhike.top

[S20] C：二分查找
来源：http://oec.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jcp.fehbvm.com

[S21] C：字符类别判断
来源：http://kre.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://get.nanxinkj.top

[S22] C：字符串转数字
来源：http://skz.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://vae.yanxiufei.cn

[S23] C：随机数
来源：http://tun.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kat.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://vjp.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mxn.yj202588.top

[S25] C：内存拷贝
来源：http://ytw.xylfe.cn

memcpy(dst, src, n);
来源：http://ake.zhijiandao.cn

[S26] C：内存清零
来源：http://xlf.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://cjm.hnxiangtu.top

[S27] C：定义常量
来源：http://gvl.birdmap.top

const double PI = 3.14159;
来源：http://rlf.sjlbkw.cn

[S28] C：静态变量
来源：http://yrx.hywenlv.cn


<!-- 参考信息 -->