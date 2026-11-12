代发 wailian999

[Q44] IN 子查询
来源：http://soo.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wnu.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://qwc.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ctt.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zec.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dka.ybcxt.top

[Q47] 与平均值比较
来源：http://age.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bvj.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://wzt.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://clx.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://lpf.vehdjk.com

[Q49] 更新单行
来源：http://swm.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://coa.haohaochexian.top

[Q50] 批量更新
来源：http://arb.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bbh.chenlongwang.top

[Q51] 用子查询更新
来源：http://nqu.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lwu.gotoacloud.top

[Q52] 删除指定行
来源：http://kvt.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://gwh.zhongyouzk.top

[Q53] 按条件删除
来源：http://cmq.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iyw.uphjek.com

[Q54] 清空表
来源：http://ynd.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://lrs.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://wuq.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://npn.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://jbm.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdc.fehbvm.com

[Q57] 行号
来源：http://opa.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gvi.yanxiufei.cn

[Q58] 累计求和
来源：http://wrb.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uhj.hongshengwenyu.top

[Q59] 分组内累计
来源：http://gbo.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bet.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://seb.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ivd.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zvr.xinyue.icu

[Q61] 移动平均
来源：http://zfx.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hal.0kj1m.cn

[Q62] 分组占比
来源：http://sjj.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbd.smart0.xyz

[Q63] 开启事务
来源：http://brj.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://isb.daxiang520.top

[Q64] 提交事务
来源：http://qaq.yfazqb.com

COMMIT;
来源：http://ngh.vehdjk.com

[Q65] 回滚事务
来源：http://xmj.bbcook.cn

ROLLBACK;
来源：http://ith.zhengqikj.top

[Q66] 行锁查询
来源：http://lbz.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xyp.zdqjudy.top

[Q67] 设置隔离级别
来源：http://akf.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rwb.chenjidiqi.icu

[Q68] 保存点
来源：http://syt.guannengcc.top

SAVEPOINT sp1;
来源：http://xfo.yonumen.top

ROLLBACK TO sp1;
来源：http://nxu.ppjwa.cn

[Q69] 查看执行计划
来源：http://yyi.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uoy.hammf.cn

[Q70] 更新统计信息
来源：http://bro.meibo888.top

ANALYZE TABLE users;
来源：http://eoa.dashuyun.cn

[Q71] 查看建表语句
来源：http://dej.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vwy.cqqwz.cn

[Q72] 查看索引
来源：http://ely.yangfankeji.com

SHOW INDEX FROM users;
来源：http://wtr.yfazqb.com

[Q73] 查看表状态
来源：http://xyy.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://oax.yuxming.cn

[Q74] 强制使用索引
来源：http://mzp.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xzp.316326.xyz

[Q75] 日期格式化
来源：http://uln.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rca.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ayc.zhengqikj.top

[Q76] 按天统计
来源：http://brp.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hil.zhiwuduotai.top

[Q77] 时间加减
来源：http://nli.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hmg.andypj.xyz

[Q78] 当前时间
来源：http://ucj.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pnq.ctjpmb.com

[Q79] 字符串拼接
来源：http://cae.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gen.hysaishi.cn

[Q80] 字符串截取
来源：http://gwh.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ppd.chenjidiqi.icu

[Q81] 字符串替换
来源：http://zxr.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nwt.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://qmq.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ycx.316326.xyz

[Q83] 大小写转换
来源：http://ydq.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lep.zdqjudy.top

[Q84] 去除首尾空格
来源：http://cux.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://zfa.iojbl.cn

[Q85] 数值取整
来源：http://gcc.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wgy.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://lhs.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yju.tanke756.top

[Q87] JSON 字段做条件
来源：http://ovd.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vci.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://ukw.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gic.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iqg.xuanzx.com

[Q89] 判断表是否存在
来源：http://dhp.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sre.hesvh.cn

[Q90] 生成序号列
来源：http://tim.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zrn.shzxlz.cn

================================================================================
来源：http://mwy.zycfv.cn

R. Bash 专题
来源：http://udl.redwolf501.top

================================================================================
来源：http://bjr.sysykeji.top

[R01] shebang 与严格模式
来源：http://zcw.yfazqb.com

#!/usr/bin/env bash
来源：http://qdf.daria6918.cn

set -euo pipefail
来源：http://wch.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://nsj.xylfe.cn

name="Tom"; echo "$name"
来源：http://qmy.pycfn.com

[R03] 只读变量
来源：http://auk.shanyushiyangtech.top

readonly PI=3.14
来源：http://vvx.cqqwz.cn

[R04] 位置参数
来源：http://vcf.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://acz.hnqzz.top

[R05] 参数默认值
来源：http://mmh.zhengqikj.top

name="${1:-default}"
来源：http://zpf.tanke756.top

[R06] 判断命令是否存在
来源：http://xuv.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://czq.xylfe.cn

[R07] if 判断文件
来源：http://vbu.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://koy.nanxinkj.top

[R08] 数值比较
来源：http://yjj.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ipn.snrcjt.cn

[R09] 字符串比较
来源：http://iaz.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uiu.gogol.net.cn

[R10] 正则匹配
来源：http://tsg.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ywj.yueranfly.top

[R11] case 多分支
来源：http://btw.wangdashe.top

case "$1" in
来源：http://znk.jinqigufen.top

start) echo "启动" ;;
来源：http://eab.shuidangran.top

stop)  echo "停止" ;;
来源：http://odz.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://vjv.316326.xyz

esac
来源：http://kxp.jianghu66.top

[R12] for 遍历文件
来源：http://gol.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://vmi.svipenyu.cn

[R13] for 计数循环
来源：http://tln.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://yne.yj202588.top

[R14] C 风格 for
来源：http://olt.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://urn.jyoumei.cn

[R15] while 逐行读文件
来源：http://zje.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yst.cheryme.top

[R16] until 等待条件
来源：http://flq.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fha.fzhhl.top

[R17] 数组定义与取值
来源：http://jhl.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pvh.andypj.xyz

[R18] 遍历数组
来源：http://fmr.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dkc.cqqwz.cn

[R19] 数组长度
来源：http://jav.bjfxy.top

echo "${#arr[@]}"
来源：http://stn.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://zka.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://emd.9152youxi.cn

[R21] 字符串长度
来源：http://wnw.cheryme.top

echo "${#s}"
来源：http://baw.svipenyu.cn

[R22] 截取子串
来源：http://xzz.hfpthk.cn

echo "${s:0:5}"
来源：http://jjk.fengsongda.top

[R23] 字符串替换
来源：http://iwq.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oom.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://meo.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://bto.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://zdu.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyh.hywenlv.cn

[R26] 命令替换
来源：http://kof.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://tyi.jinqigufen.top

[R27] 算术展开
来源：http://jnv.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://vbe.zhengqikj.top

[R28] 浮点运算
来源：http://maq.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://ffb.nwbrower.top

[R29] 定义函数
来源：http://dcf.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cri.mhx1999.top

[R30] 函数返回状态码
来源：http://nqs.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://zcu.chenzaomai.com

[R31] 局部变量
来源：http://olf.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://ydp.xinyue.icu

[R32] 参数个数校验
来源：http://vfo.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eej.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://cvb.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gaz.guannengcc.top

[R34] 退出时清理
来源：http://hkg.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://del.hammf.cn

[R35] 后台执行并等待
来源：http://eyd.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wni.nwbrower.top

[R36] 并发执行多个任务
来源：http://oqg.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wky.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://bcq.bjfxy.top

files=$(ls -1)
来源：http://syb.hcnkem.com

[R38] 管道串联
来源：http://uat.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://dee.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://jrm.jinqigfzy.top

cmd > out.log 2>&1
来源：http://cib.0kj1m.cn

[R40] 追加写日志
来源：http://pul.gaohongyu789.top

echo "log" >> out.log
来源：http://srd.hfpthk.cn

[R41] 丢弃输出
来源：http://abi.ivvv.top

cmd >/dev/null 2>&1
来源：http://pca.cqqwz.cn

[R42] 输入重定向
来源：http://eex.zhengqikj.top

wc -l < a.txt
来源：http://geg.redwolf501.top

[R43] 按名字查找文件
来源：http://vna.meibo888.top

find . -name "*.log" -type f
来源：http://mhh.sjlbkw.cn

[R44] 按修改时间查找
来源：http://bwa.sysykeji.top

find . -mtime -7 -type f
来源：http://bzm.gzhubu.top

[R45] 批量删除
来源：http://yqy.meibo888.top

find . -name "*.tmp" -delete
来源：http://gld.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://ysq.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://krj.fengsongda.top

[R47] sed 单行替换
来源：http://xxz.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cwg.wangshuangyany.cn

[R48] awk 取指定列
来源：http://efn.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://qsz.smart0.xyz

[R49] awk 带条件
来源：http://ddp.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://exw.hfpthk.cn

[R50] awk 求和
来源：http://vpk.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://ypz.kuanghao11.cn

[R51] 排序去重取前几
来源：http://dpi.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nao.ehwqpu.com

[R52] 统计行数
来源：http://ezh.hnxiangtu.top

wc -l a.txt
来源：http://yyi.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://ygn.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nte.feifeiyinyue.top

[R54] 比较两个文件
来源：http://uju.redwolf501.top

diff a.txt b.txt
来源：http://fib.bbcook.cn

[R55] 压缩与解压
来源：http://koq.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bhx.ydjk.org.cn

[R56] 远程拷贝
来源：http://bdk.uphjek.com

scp file user@host:/path/
来源：http://iyk.shangyingyoupin.top

[R57] 远程执行命令
来源：http://nge.nwbrower.top

ssh user@host 'uptime'
来源：http://pmr.cheryme.top

[R58] 下载文件
来源：http://izc.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ifj.nwbrower.top

[R59] 发 POST JSON
来源：http://sda.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ama.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://atq.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xyp.shzxlz.cn

[R61] 磁盘占用
来源：http://ock.andypj.xyz

df -h;  du -sh *
来源：http://abg.dashuyun.cn

[R62] 找最占空间的文件
来源：http://jad.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://cnw.birdmap.top

[R63] 内存与进程
来源：http://ngu.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://ncv.kuanghao11.cn

[R64] 结束进程
来源：http://qqs.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://aud.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://gzh.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://juk.chenzaomai.com

[R66] 定时任务
来源：http://lgf.fengsongda.top

crontab -e;  crontab -l
来源：http://dlh.hammf.cn

[R67] 生成随机十六进制串
来源：http://tul.sxryk.cn

openssl rand -hex 16
来源：http://oae.cashguo.top

[R68] 计算文件校验值
来源：http://dzh.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://zxs.gaohongyu789.top

[R69] 生成随机密码
来源：http://ouc.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://vfv.redwolf501.top

[R70] 时间戳与互转
来源：http://hla.hnqzz.top

date +%s;  date -d @1700000000
来源：http://cyj.0kj1m.cn

[R71] 日期格式化
来源：http://lbl.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mns.zhongyouzk.top

[R72] 等待端口就绪
来源：http://zvs.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zuc.ivvv.top

[R73] 分割大日志
来源：http://zlp.yj202588.top

split -l 1000 big.log part_
来源：http://owa.bjfxy.top

[R74] 批量重命名
来源：http://jub.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://swo.guannengcc.top

[R75] 导出环境变量
来源：http://sec.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://seb.bbcook.cn

[R76] 使用临时文件
来源：http://kll.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hzf.yuxming.cn

[R77] 读取用户输入
来源：http://pyv.yfazqb.com

read -rp "请输入: " ans
来源：http://uaz.chenjidiqi.icu

[R78] 交互式菜单
来源：http://esb.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vep.sxryk.cn

[R79] 解析命令行选项
来源：http://hwu.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lvm.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://tjq.meibo888.top

time ./run.sh
来源：http://ptt.tanke756.top

================================================================================
来源：http://zne.zhiwuduotai.top

S. C / C++ 专题
来源：http://enr.guowangkeji.top

================================================================================
来源：http://crm.andypj.xyz

[S01] C：Hello World
来源：http://ynk.zdbjq.cn

#include <stdio.h>
来源：http://mfl.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oma.mhx1999.top

[S02] C：变量与格式化输出
来源：http://ene.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://jrt.tian-w.cn

[S03] C：读入整数
来源：http://zsl.xylfe.cn

int x; scanf("%d", &x);
来源：http://krh.9152youxi.cn

[S04] C：字符串复制
来源：http://ylj.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://pvg.jianghu66.top

[S05] C：字符串长度
来源：http://obi.vqdsnc.cn

strlen(s)
来源：http://jzr.xuetiantiany.cn

[S06] C：字符串比较
来源：http://knw.birdmap.top

strcmp(a, b) == 0
来源：http://mwb.daxiang520.top

[S07] C：数组遍历求和
来源：http://crb.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eio.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://gbo.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://npy.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://ryv.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://izw.tarul.cn

[S10] C：指针与解引用
来源：http://voe.fengsongda.top

int *p = &a;  *p = 5;
来源：http://qqp.vqdsnc.cn

[S11] C：逐行读文件
来源：http://gwm.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://obd.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://beo.uphjek.com

fclose(f);
来源：http://vvi.zhaomingkeji.xyz

[S12] C：写文件
来源：http://dsa.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dls.fehbvm.com

[S13] C：宏定义
来源：http://bnb.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xgw.jinghuilouyu.cn

[S14] C：枚举
来源：http://rim.yvedp.cn


<!-- 参考信息 -->