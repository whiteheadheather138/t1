代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tmp.xuetiantiany.cn

[Q54] 清空表
来源：http://zbw.316326.xyz

TRUNCATE TABLE logs;
来源：http://kdk.redwolf501.top

[Q55] 排名（并列占位）
来源：http://jhk.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gns.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://kpf.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aeo.guannengcc.top

[Q57] 行号
来源：http://cge.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://epe.hesvh.cn

[Q58] 累计求和
来源：http://ahs.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rtm.nwbrower.top

[Q59] 分组内累计
来源：http://sml.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rwb.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://enk.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://udv.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://chn.kuanghao11.cn

[Q61] 移动平均
来源：http://upz.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gwx.smart0.xyz

[Q62] 分组占比
来源：http://txm.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bme.sxryk.cn

[Q63] 开启事务
来源：http://jcw.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://gby.iojbl.cn

[Q64] 提交事务
来源：http://bwg.jlsjyb.cn

COMMIT;
来源：http://ami.xylfe.cn

[Q65] 回滚事务
来源：http://nba.mhx1999.top

ROLLBACK;
来源：http://qwi.jinqigfzy.top

[Q66] 行锁查询
来源：http://nrh.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://euo.cqqwz.cn

[Q67] 设置隔离级别
来源：http://sng.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efs.jiagoushi.top

[Q68] 保存点
来源：http://ati.daxiang520.top

SAVEPOINT sp1;
来源：http://sui.xinyue.icu

ROLLBACK TO sp1;
来源：http://lqk.jianghu66.top

[Q69] 查看执行计划
来源：http://vsw.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qfr.cqqwz.cn

[Q70] 更新统计信息
来源：http://uyk.vqdsnc.cn

ANALYZE TABLE users;
来源：http://dai.jqgfzy.top

[Q71] 查看建表语句
来源：http://xtz.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dyd.ehwqpu.com

[Q72] 查看索引
来源：http://gpa.xziqi.cn

SHOW INDEX FROM users;
来源：http://cvl.zhixingplan.top

[Q73] 查看表状态
来源：http://xso.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xkr.gzhubu.top

[Q74] 强制使用索引
来源：http://ywt.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lck.yj202588.top

[Q75] 日期格式化
来源：http://tzb.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lgi.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aop.sjlbkw.cn

[Q76] 按天统计
来源：http://iej.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ywh.feifeiyinyue.top

[Q77] 时间加减
来源：http://hkt.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kmi.aibaodan.cn

[Q78] 当前时间
来源：http://hsn.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qsn.jqgufenzy.top

[Q79] 字符串拼接
来源：http://dio.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ibq.gzhubu.top

[Q80] 字符串截取
来源：http://hoe.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtf.dianchejie.cn

[Q81] 字符串替换
来源：http://vcs.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cdr.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://kek.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hti.kuanghao11.cn

[Q83] 大小写转换
来源：http://acu.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bnf.hfpthk.cn

[Q84] 去除首尾空格
来源：http://ylr.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://mrl.yangfankeji.com

[Q85] 数值取整
来源：http://tox.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iki.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://wvl.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hld.tian-w.cn

[Q87] JSON 字段做条件
来源：http://gff.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://non.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://lpz.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cwl.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bbg.nwbrower.top

[Q89] 判断表是否存在
来源：http://qvh.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sxt.zdbjq.cn

[Q90] 生成序号列
来源：http://sbc.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ncf.shanyushiyangtech.top

================================================================================
来源：http://nvs.smart0.xyz

R. Bash 专题
来源：http://sko.hfpthk.cn

================================================================================
来源：http://uml.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://xxj.yfazqb.com

#!/usr/bin/env bash
来源：http://ksi.shanyushiyangkeji.top

set -euo pipefail
来源：http://xxs.cheryme.top

[R02] 变量赋值与使用
来源：http://foo.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://coh.redwolf501.top

[R03] 只读变量
来源：http://ivw.chenzaomai.com

readonly PI=3.14
来源：http://tve.yuanzhike.top

[R04] 位置参数
来源：http://wcf.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rlk.zdqjudy.top

[R05] 参数默认值
来源：http://knd.nanxuanxn.top

name="${1:-default}"
来源：http://ali.sxryk.cn

[R06] 判断命令是否存在
来源：http://qme.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://phg.shzxlz.cn

[R07] if 判断文件
来源：http://bgv.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jsx.smart0.xyz

[R08] 数值比较
来源：http://cpx.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://bgd.nanxuanxn.top

[R09] 字符串比较
来源：http://fpy.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://irw.hywenlv.cn

[R10] 正则匹配
来源：http://cmn.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qxm.shuidangran.top

[R11] case 多分支
来源：http://mic.jinyuanbaomall.cn

case "$1" in
来源：http://zhk.yj202588.top

start) echo "启动" ;;
来源：http://zyv.aibaodan.cn

stop)  echo "停止" ;;
来源：http://owu.birdmap.top

*)     echo "未知命令" ;;
来源：http://ois.ywan-chungtsiang.top

esac
来源：http://ysh.daxiang520.top

[R12] for 遍历文件
来源：http://rld.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://xal.birdmap.top

[R13] for 计数循环
来源：http://ums.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://tfh.tian-w.cn

[R14] C 风格 for
来源：http://myl.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jfr.nanxuanxn.top

[R15] while 逐行读文件
来源：http://vqj.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qjn.sxryk.cn

[R16] until 等待条件
来源：http://dax.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kbc.hywenlv.cn

[R17] 数组定义与取值
来源：http://twt.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://wxf.9152youxi.cn

[R18] 遍历数组
来源：http://fuk.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://abq.ydzc1.top

[R19] 数组长度
来源：http://dez.ehwqpu.com

echo "${#arr[@]}"
来源：http://nzc.ctjpmb.com

[R20] 关联数组（字典）
来源：http://qhr.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://txv.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://zme.daria6918.cn

echo "${#s}"
来源：http://wbj.c1oappe.top

[R22] 截取子串
来源：http://rqi.zhoulong.xyz

echo "${s:0:5}"
来源：http://prl.yangfankeji.com

[R23] 字符串替换
来源：http://sop.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vpj.pengpengdd.cyou

[R24] 大小写转换
来源：http://alf.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://rai.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://wlm.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wyc.yj202588.top

[R26] 命令替换
来源：http://clj.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://rgh.cqqwz.cn

[R27] 算术展开
来源：http://bzv.xinyue.icu

echo $((1 + 2 * 3))
来源：http://rlq.chenjidiqi.icu

[R28] 浮点运算
来源：http://uzm.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://wfh.cqqwz.cn

[R29] 定义函数
来源：http://neu.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zfb.iojbl.cn

[R30] 函数返回状态码
来源：http://tqz.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://vrz.wangshuangyany.cn

[R31] 局部变量
来源：http://pnv.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://olj.jinqigfzy.top

[R32] 参数个数校验
来源：http://egl.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tsx.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://jlm.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lam.nwbrower.top

[R34] 退出时清理
来源：http://bns.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cop.hammf.cn

[R35] 后台执行并等待
来源：http://gns.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uog.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://uvm.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mnk.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://txb.hnxiangtu.top

files=$(ls -1)
来源：http://zlh.yueranfly.top

[R38] 管道串联
来源：http://bhv.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://wtf.tanke756.top

[R39] 重定向标准输出与错误
来源：http://svo.uphjek.com

cmd > out.log 2>&1
来源：http://cgn.dianchejie.cn

[R40] 追加写日志
来源：http://bpf.smart0.xyz

echo "log" >> out.log
来源：http://nyt.0kj1m.cn

[R41] 丢弃输出
来源：http://fcl.daria6918.cn

cmd >/dev/null 2>&1
来源：http://ygn.aibaodan.cn

[R42] 输入重定向
来源：http://xrg.ctjpmb.com

wc -l < a.txt
来源：http://ttd.jiagoushi.top

[R43] 按名字查找文件
来源：http://nlr.havefunace.top

find . -name "*.log" -type f
来源：http://vlc.yj20258.top

[R44] 按修改时间查找
来源：http://fbx.fehbvm.com

find . -mtime -7 -type f
来源：http://ols.nanxuanxn.top

[R45] 批量删除
来源：http://bsr.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://hxu.hnqzz.top

[R46] 递归替换文件内容
来源：http://plf.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gxh.yj20258.top

[R47] sed 单行替换
来源：http://ggu.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://dyk.fktsv.cn

[R48] awk 取指定列
来源：http://zbh.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://oat.pycfn.com

[R49] awk 带条件
来源：http://rkh.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lix.quarkkingdee.top

[R50] awk 求和
来源：http://nsd.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ysn.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://izw.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fok.jqgufenzy.top

[R52] 统计行数
来源：http://xkd.shzxlz.cn

wc -l a.txt
来源：http://jil.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://jly.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lgo.jinqigfzy.top

[R54] 比较两个文件
来源：http://ycc.vqdsnc.cn

diff a.txt b.txt
来源：http://kcn.tarul.cn

[R55] 压缩与解压
来源：http://rma.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uhh.havefunace.top

[R56] 远程拷贝
来源：http://xzv.andypj.xyz

scp file user@host:/path/
来源：http://hcm.gaohongyu789.top

[R57] 远程执行命令
来源：http://fxn.daxiang520.top

ssh user@host 'uptime'
来源：http://yhl.andypj.xyz

[R58] 下载文件
来源：http://uie.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tnc.sxryk.cn

[R59] 发 POST JSON
来源：http://mnx.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gzx.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://ufc.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ckr.nanxuanxn.top

[R61] 磁盘占用
来源：http://kdj.zdbjq.cn

df -h;  du -sh *
来源：http://uao.sweek.top

[R62] 找最占空间的文件
来源：http://uqf.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://nzs.xinyue.icu

[R63] 内存与进程
来源：http://gib.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://wfd.hongshengwenyu.top

[R64] 结束进程
来源：http://vkg.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://lwl.sjlbkw.cn

[R65] 查看端口占用
来源：http://gdd.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nov.sweek.top

[R66] 定时任务
来源：http://ktq.guannengcc.top

crontab -e;  crontab -l
来源：http://poa.fehbvm.com

[R67] 生成随机十六进制串
来源：http://npm.quarkkingdee.top

openssl rand -hex 16
来源：http://veg.ybcxt.top

[R68] 计算文件校验值
来源：http://yig.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://jfa.hfpthk.cn

[R69] 生成随机密码
来源：http://lqi.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://ued.sweek.top

[R70] 时间戳与互转
来源：http://ies.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://zfc.ydzc1.top

[R71] 日期格式化
来源：http://jxe.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vdl.sweek.top

[R72] 等待端口就绪
来源：http://cvl.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gka.havefunace.top

[R73] 分割大日志
来源：http://rjn.ydjk.org.cn

split -l 1000 big.log part_
来源：http://dps.guannengcc.top

[R74] 批量重命名
来源：http://psr.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ast.fengsongda.top

[R75] 导出环境变量
来源：http://vqf.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://jfc.bbcook.cn

[R76] 使用临时文件
来源：http://smq.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lzo.ybcxt.top

[R77] 读取用户输入
来源：http://hng.sxryk.cn

read -rp "请输入: " ans
来源：http://fuo.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://yvh.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ihr.yvedp.cn

[R79] 解析命令行选项
来源：http://wqw.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wvr.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://hcs.yj202588.top

time ./run.sh
来源：http://jlp.tianlin.xyz

================================================================================
来源：http://tbg.vehdjk.com

S. C / C++ 专题
来源：http://qwk.0kj1m.cn

================================================================================
来源：http://wkh.redwolf501.top

[S01] C：Hello World
来源：http://gdd.9152youxi.cn

#include <stdio.h>
来源：http://ooj.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://tip.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://gln.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://zlw.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://kuo.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://lui.sufxvd.cn

[S04] C：字符串复制
来源：http://zjo.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://xip.jiagoushi.top

[S05] C：字符串长度
来源：http://pcf.jinqigufen.top

strlen(s)
来源：http://vbi.gogol.net.cn

[S06] C：字符串比较
来源：http://odp.xziqi.cn

strcmp(a, b) == 0
来源：http://bra.yangfankeji.com

[S07] C：数组遍历求和
来源：http://oka.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jvd.hongshengwenyu.top

[S08] C：动态内存分配与释放
来源：http://tff.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tam.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://lty.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zkc.fzhhl.top

[S10] C：指针与解引用
来源：http://ohg.sysykeji.top

int *p = &a;  *p = 5;
来源：http://tmk.epnwcf.com

[S11] C：逐行读文件
来源：http://efm.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://yvv.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jfy.fktsv.cn

fclose(f);
来源：http://rrx.jinqigufen.top

[S12] C：写文件
来源：http://qor.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iyi.ydjk.org.cn

[S13] C：宏定义
来源：http://son.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mpc.hcnkem.com

[S14] C：枚举
来源：http://ljx.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://gnn.gzhubu.top

[S15] C：类型转换
来源：http://wus.ctjpmb.com

(double) a / b
来源：http://zyq.xuetiantiany.cn

[S16] C：位操作置位
来源：http://udr.yfazqb.com

x |= (1 << 3);
来源：http://whx.bbcook.cn

[S17] C：安全拼接字符串
来源：http://czm.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slu.yonumen.top

[S18] C：命令行参数
来源：http://mjt.ydzc1.top

int main(int argc, char **argv)
来源：http://fwt.zhoulong.xyz

[S19] C：快速排序
来源：http://jqr.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://sjs.uphjek.com

[S20] C：二分查找
来源：http://fqh.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uea.jlsjyb.cn

[S21] C：字符类别判断
来源：http://qqo.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mca.cheryme.top

[S22] C：字符串转数字
来源：http://roq.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ngj.chenjidiqi.icu

[S23] C：随机数
来源：http://opp.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ytm.dianchejie.cn

[S24] C：获取本地时间
来源：http://xbj.dashuyun.cn


<!-- 参考信息 -->