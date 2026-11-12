代发 wailian999

[Q44] IN 子查询
来源：http://tjh.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iyq.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://msr.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ric.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qns.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mer.haohaochexian.top

[Q47] 与平均值比较
来源：http://rfd.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pad.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://jky.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kqt.shuidangran.top

SELECT * FROM t WHERE c > 5;
来源：http://zjz.fktsv.cn

[Q49] 更新单行
来源：http://uka.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gjs.ctjpmb.com

[Q50] 批量更新
来源：http://rtr.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ifm.jqgfzy.top

[Q51] 用子查询更新
来源：http://knr.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eab.fzhhl.top

[Q52] 删除指定行
来源：http://ipv.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://txb.fengsongda.top

[Q53] 按条件删除
来源：http://uts.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sgy.dianchejie.cn

[Q54] 清空表
来源：http://gsj.daxiang520.top

TRUNCATE TABLE logs;
来源：http://nyn.tanke756.top

[Q55] 排名（并列占位）
来源：http://tdz.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jrm.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://mmu.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wpo.tanke756.top

[Q57] 行号
来源：http://vfc.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gag.yuxming.cn

[Q58] 累计求和
来源：http://mas.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lpm.xinyue.icu

[Q59] 分组内累计
来源：http://ixa.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xwe.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://ecw.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://igl.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cak.zhixingplan.top

[Q61] 移动平均
来源：http://zfk.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ssa.316326.xyz

[Q62] 分组占比
来源：http://dwg.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xqi.shanyushiyangtech.top

[Q63] 开启事务
来源：http://bgw.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ovw.daxiang520.top

[Q64] 提交事务
来源：http://gse.daria6918.cn

COMMIT;
来源：http://jrw.cdnleiting.top

[Q65] 回滚事务
来源：http://uol.feifeiyinyue.top

ROLLBACK;
来源：http://dun.tarul.cn

[Q66] 行锁查询
来源：http://qya.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xta.xziqi.cn

[Q67] 设置隔离级别
来源：http://cny.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qos.zhiwuduotai.top

[Q68] 保存点
来源：http://tvb.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://boo.ehwqpu.com

ROLLBACK TO sp1;
来源：http://iqk.vehdjk.com

[Q69] 查看执行计划
来源：http://ksw.shanyushiyangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://olj.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://vnr.gotoacloud.top

ANALYZE TABLE users;
来源：http://fvs.jinqigfzy.top

[Q71] 查看建表语句
来源：http://nvj.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fgk.hysaishi.cn

[Q72] 查看索引
来源：http://scl.uphjek.com

SHOW INDEX FROM users;
来源：http://pkx.uphjek.com

[Q73] 查看表状态
来源：http://mfu.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bhm.gaohongyu789.top

[Q74] 强制使用索引
来源：http://wdy.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dwf.wangdashe.top

[Q75] 日期格式化
来源：http://ady.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wam.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yba.nanxuanxn.top

[Q76] 按天统计
来源：http://qen.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://taf.nanxinkj.top

[Q77] 时间加减
来源：http://dzt.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kic.yj20258888.top

[Q78] 当前时间
来源：http://yyc.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfa.zhiwuduotai.top

[Q79] 字符串拼接
来源：http://mpb.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zcs.yanxiufei.cn

[Q80] 字符串截取
来源：http://ymg.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oaf.yongpay.top

[Q81] 字符串替换
来源：http://dav.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wsn.tarul.cn

[Q82] 字符长度与字节长度
来源：http://nrz.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nvr.pengpengdd.cyou

[Q83] 大小写转换
来源：http://avs.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vmk.shuidangran.top

[Q84] 去除首尾空格
来源：http://ejm.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://xfr.zhoulong.xyz

[Q85] 数值取整
来源：http://vpa.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://miu.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://rfc.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lqt.yonumen.top

[Q87] JSON 字段做条件
来源：http://ehg.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dam.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://run.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mgi.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gru.gotoacloud.top

[Q89] 判断表是否存在
来源：http://ngk.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://van.zdqjudy.top

[Q90] 生成序号列
来源：http://aro.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aaw.yvedp.cn

================================================================================
来源：http://jgr.gaohongyu789.top

R. Bash 专题
来源：http://cyd.svipenyu.cn

================================================================================
来源：http://tdz.fengsongda.top

[R01] shebang 与严格模式
来源：http://lys.hnxiangtu.top

#!/usr/bin/env bash
来源：http://wse.gotoacloud.top

set -euo pipefail
来源：http://ddx.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://edc.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://sbs.sweek.top

[R03] 只读变量
来源：http://khq.andypj.xyz

readonly PI=3.14
来源：http://fkj.bjfxy.top

[R04] 位置参数
来源：http://ffw.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tzi.smart0.xyz

[R05] 参数默认值
来源：http://tbi.smart0.xyz

name="${1:-default}"
来源：http://jge.shzxlz.cn

[R06] 判断命令是否存在
来源：http://fkg.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kxb.vehdjk.com

[R07] if 判断文件
来源：http://eit.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zoo.xziqi.cn

[R08] 数值比较
来源：http://xof.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tun.tanke756.top

[R09] 字符串比较
来源：http://trs.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qjj.tarul.cn

[R10] 正则匹配
来源：http://whk.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dnm.meibo888.top

[R11] case 多分支
来源：http://apa.yj20258888.top

case "$1" in
来源：http://ijo.wangshuangyany.cn

start) echo "启动" ;;
来源：http://vqd.sxryk.cn

stop)  echo "停止" ;;
来源：http://myx.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://imb.cqqwz.cn

esac
来源：http://lbj.zycfv.cn

[R12] for 遍历文件
来源：http://dpq.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://are.shanyushiyangtech.top

[R13] for 计数循环
来源：http://bzo.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://wky.cheryme.top

[R14] C 风格 for
来源：http://wfh.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fhp.yuxming.cn

[R15] while 逐行读文件
来源：http://fve.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iml.hfpthk.cn

[R16] until 等待条件
来源：http://hvk.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dxo.cucudq.cn

[R17] 数组定义与取值
来源：http://tcg.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://omx.kuanghao11.cn

[R18] 遍历数组
来源：http://pst.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cgu.zhijiandao.cn

[R19] 数组长度
来源：http://kmp.guowangkeji.top

echo "${#arr[@]}"
来源：http://pkh.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://eee.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yqo.jqgfzy.top

[R21] 字符串长度
来源：http://iuh.daxiang520.top

echo "${#s}"
来源：http://ton.fanxiaobao.xyz

[R22] 截取子串
来源：http://srx.tarul.cn

echo "${s:0:5}"
来源：http://yxj.birdmap.top

[R23] 字符串替换
来源：http://wuu.sysykeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lsp.hysaishi.cn

[R24] 大小写转换
来源：http://wqp.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://vss.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://wfd.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pzx.tianlin.xyz

[R26] 命令替换
来源：http://rce.316326.xyz

now=$(date +%F); echo "$now"
来源：http://syn.xziqi.cn

[R27] 算术展开
来源：http://vyx.zycfv.cn

echo $((1 + 2 * 3))
来源：http://hey.sysykeji.top

[R28] 浮点运算
来源：http://mei.bjfxy.top

echo "scale=2; 10/3" | bc
来源：http://qdz.xinyue.icu

[R29] 定义函数
来源：http://csk.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zef.gaohongyu789.top

[R30] 函数返回状态码
来源：http://gsk.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://afg.yueranfly.top

[R31] 局部变量
来源：http://cil.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://iwj.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://hmx.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dks.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://ucz.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjo.ydzc1.top

[R34] 退出时清理
来源：http://seq.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oym.jqgufenzy.top

[R35] 后台执行并等待
来源：http://fkq.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://hzq.sysykeji.top

[R36] 并发执行多个任务
来源：http://yhz.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://adg.mhx1999.top

[R37] 把输出赋给变量
来源：http://jxx.ivvv.top

files=$(ls -1)
来源：http://tuu.uphjek.com

[R38] 管道串联
来源：http://zxx.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://pef.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://faz.aizwys.cn

cmd > out.log 2>&1
来源：http://sad.shzxlz.cn

[R40] 追加写日志
来源：http://hrm.bbcook.cn

echo "log" >> out.log
来源：http://gbf.smart0.xyz

[R41] 丢弃输出
来源：http://ydc.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://xvl.hysaishi.cn

[R42] 输入重定向
来源：http://nip.gogol.net.cn

wc -l < a.txt
来源：http://scb.tarul.cn

[R43] 按名字查找文件
来源：http://ytp.chenzaomai.com

find . -name "*.log" -type f
来源：http://rmz.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://vaq.xylfe.cn

find . -mtime -7 -type f
来源：http://wse.aizwys.cn

[R45] 批量删除
来源：http://qiq.yj20258.top

find . -name "*.tmp" -delete
来源：http://orz.bbcook.cn

[R46] 递归替换文件内容
来源：http://dkx.jqgfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mgi.jianghu66.top

[R47] sed 单行替换
来源：http://wnl.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ncg.52xcode.cn

[R48] awk 取指定列
来源：http://evl.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://cpz.cqqwz.cn

[R49] awk 带条件
来源：http://qbb.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sbb.jiagoushi.top

[R50] awk 求和
来源：http://irz.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gro.sjlbkw.cn

[R51] 排序去重取前几
来源：http://ptz.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bbu.jlsjyb.cn

[R52] 统计行数
来源：http://cyu.hnqzz.top

wc -l a.txt
来源：http://fzb.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://bte.haohaochexian.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qdx.yueranfly.top

[R54] 比较两个文件
来源：http://fmj.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://hjc.hnqzz.top

[R55] 压缩与解压
来源：http://kre.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ija.yj20258888.top

[R56] 远程拷贝
来源：http://sjq.yueranfly.top

scp file user@host:/path/
来源：http://dzg.9152youxi.cn

[R57] 远程执行命令
来源：http://mso.yanxiufei.cn

ssh user@host 'uptime'
来源：http://kfq.jyoumei.cn

[R58] 下载文件
来源：http://afv.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://asi.zhixingplan.top

[R59] 发 POST JSON
来源：http://bua.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqd.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://bow.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ide.shzxlz.cn

[R61] 磁盘占用
来源：http://mei.svipenyu.cn

df -h;  du -sh *
来源：http://hfl.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://yyj.uphjek.com

du -ah . | sort -rh | head -10
来源：http://fnd.pengpengdd.cyou

[R63] 内存与进程
来源：http://zcj.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://een.quarkkingdee.top

[R64] 结束进程
来源：http://kme.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://ruw.mhx1999.top

[R65] 查看端口占用
来源：http://rbf.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rcu.quarkkingdee.top

[R66] 定时任务
来源：http://ejm.shuidangran.top

crontab -e;  crontab -l
来源：http://yxs.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://cid.gotoacloud.top

openssl rand -hex 16
来源：http://nvg.316326.xyz

[R68] 计算文件校验值
来源：http://eca.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://nbi.birdmap.top

[R69] 生成随机密码
来源：http://aka.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://dyu.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://tmr.sysykeji.top

date +%s;  date -d @1700000000
来源：http://prq.dashuyun.cn

[R71] 日期格式化
来源：http://bez.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://zxm.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://csp.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ato.xinyue.icu

[R73] 分割大日志
来源：http://glp.hammf.cn

split -l 1000 big.log part_
来源：http://okl.zhengqikj.top

[R74] 批量重命名
来源：http://wcn.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zur.xuetiantiany.cn

[R75] 导出环境变量
来源：http://wzs.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://usf.hesvh.cn

[R76] 使用临时文件
来源：http://buh.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ltw.cqqwz.cn

[R77] 读取用户输入
来源：http://gif.nanxinkj.top

read -rp "请输入: " ans
来源：http://axv.hnqzz.top

[R78] 交互式菜单
来源：http://ftv.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jzj.gogol.net.cn

[R79] 解析命令行选项
来源：http://fdw.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vcz.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://ksd.c1oappe.top

time ./run.sh
来源：http://rso.zycfv.cn

================================================================================
来源：http://gay.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://mwc.hnqzz.top

================================================================================
来源：http://quz.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://puw.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://ins.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bbc.uphjek.com

[S02] C：变量与格式化输出
来源：http://olc.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://kxe.quarkkingdee.top

[S03] C：读入整数
来源：http://utb.guannengcc.top

int x; scanf("%d", &x);
来源：http://xyi.jqgfzy.top

[S04] C：字符串复制
来源：http://cpb.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jqy.hfpthk.cn

[S05] C：字符串长度
来源：http://oac.chenzaomai.com

strlen(s)
来源：http://hkx.yueranfly.top

[S06] C：字符串比较
来源：http://sbj.zhijiandao.cn

strcmp(a, b) == 0
来源：http://pjs.fzhhl.top

[S07] C：数组遍历求和
来源：http://bzk.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mmi.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://slk.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wwi.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://awz.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utc.gogol.net.cn

[S10] C：指针与解引用
来源：http://qfn.xziqi.cn

int *p = &a;  *p = 5;
来源：http://xoa.hnxiangtu.top

[S11] C：逐行读文件
来源：http://vnr.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://rau.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bki.yuanzhike.top

fclose(f);
来源：http://lxr.feifeiyinyue.top

[S12] C：写文件
来源：http://qnd.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bdn.dianchejie.cn

[S13] C：宏定义
来源：http://tms.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsp.yj202588.top

[S14] C：枚举
来源：http://jmz.guannengcc.top


<!-- 参考信息 -->