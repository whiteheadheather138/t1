代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://yci.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mlt.uphjek.com

[Q43] 标量子查询
来源：http://nyj.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://htq.redwolf501.top

[Q44] IN 子查询
来源：http://mct.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kkl.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://ydo.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cdv.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://vlr.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnx.yvedp.cn

[Q47] 与平均值比较
来源：http://jnu.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zgl.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://zdp.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zxi.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://mdw.cashguo.top

[Q49] 更新单行
来源：http://ypw.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nro.haohaochexian.top

[Q50] 批量更新
来源：http://jbq.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://grd.nanxinkj.top

[Q51] 用子查询更新
来源：http://pjl.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ayo.hfpthk.cn

[Q52] 删除指定行
来源：http://mwe.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://uko.chenjidiqi.icu

[Q53] 按条件删除
来源：http://pmh.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rue.yonumen.top

[Q54] 清空表
来源：http://rjc.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://nnf.hammf.cn

[Q55] 排名（并列占位）
来源：http://pdc.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://obb.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://xhh.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rea.jinqigfzy.top

[Q57] 行号
来源：http://xze.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://llk.c1oappe.top

[Q58] 累计求和
来源：http://tdv.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nio.redwolf501.top

[Q59] 分组内累计
来源：http://xzq.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xor.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://ryp.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzl.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jhq.dianchejie.cn

[Q61] 移动平均
来源：http://cid.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vxr.hfpthk.cn

[Q62] 分组占比
来源：http://gmv.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qax.shuidangran.top

[Q63] 开启事务
来源：http://lpt.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xey.guannengcc.top

[Q64] 提交事务
来源：http://tre.hfpthk.cn

COMMIT;
来源：http://ynv.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://dmm.ydjk.org.cn

ROLLBACK;
来源：http://rey.hongshengwenyu.top

[Q66] 行锁查询
来源：http://lkm.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qaq.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://rjf.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hmn.hnqzz.top

[Q68] 保存点
来源：http://ryz.nanxinkj.top

SAVEPOINT sp1;
来源：http://fbk.hammf.cn

ROLLBACK TO sp1;
来源：http://tok.dianchejie.cn

[Q69] 查看执行计划
来源：http://rzp.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cfd.jyoumei.cn

[Q70] 更新统计信息
来源：http://wjo.52xcode.cn

ANALYZE TABLE users;
来源：http://dqj.bjfxy.top

[Q71] 查看建表语句
来源：http://nyi.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zpr.tanke756.top

[Q72] 查看索引
来源：http://snk.52xcode.cn

SHOW INDEX FROM users;
来源：http://vng.zhongyouzk.top

[Q73] 查看表状态
来源：http://gqw.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dps.chenlongwang.top

[Q74] 强制使用索引
来源：http://kkv.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gxn.52xcode.cn

[Q75] 日期格式化
来源：http://kef.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iib.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fwt.gzhubu.top

[Q76] 按天统计
来源：http://ogq.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bvv.dashuyun.cn

[Q77] 时间加减
来源：http://jxl.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cvk.zhoulong.xyz

[Q78] 当前时间
来源：http://zav.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qpk.gogol.net.cn

[Q79] 字符串拼接
来源：http://usr.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kkh.tianlin.xyz

[Q80] 字符串截取
来源：http://otg.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://enx.meibo888.top

[Q81] 字符串替换
来源：http://irl.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vct.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://ziy.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hyy.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://qww.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kwv.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://xnh.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://cpa.hysaishi.cn

[Q85] 数值取整
来源：http://tzn.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wik.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://lqo.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gkf.meibo888.top

[Q87] JSON 字段做条件
来源：http://eou.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mld.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://nst.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fqj.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hbg.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://ccc.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkw.hnxiangtu.top

[Q90] 生成序号列
来源：http://oxp.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fwh.chenlongwang.top

================================================================================
来源：http://qba.cheryme.top

R. Bash 专题
来源：http://aau.dashuyun.cn

================================================================================
来源：http://bal.xylfe.cn

[R01] shebang 与严格模式
来源：http://nxx.bbcook.cn

#!/usr/bin/env bash
来源：http://gnz.sufxvd.cn

set -euo pipefail
来源：http://dhr.sweek.top

[R02] 变量赋值与使用
来源：http://fsl.316326.xyz

name="Tom"; echo "$name"
来源：http://iiy.ehwqpu.com

[R03] 只读变量
来源：http://med.jinghuilouyu.cn

readonly PI=3.14
来源：http://vqn.shangyingyoupin.top

[R04] 位置参数
来源：http://bhx.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nsz.svipenyu.cn

[R05] 参数默认值
来源：http://wly.zhijiandao.cn

name="${1:-default}"
来源：http://waj.daria6918.cn

[R06] 判断命令是否存在
来源：http://pex.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ptk.guannengcc.top

[R07] if 判断文件
来源：http://kbu.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bzf.iojbl.cn

[R08] 数值比较
来源：http://ekc.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fsx.hywenlv.cn

[R09] 字符串比较
来源：http://zru.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ujx.c1oappe.top

[R10] 正则匹配
来源：http://gcr.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fkf.ivvv.top

[R11] case 多分支
来源：http://qpk.snrcjt.cn

case "$1" in
来源：http://hgw.yj20258888.top

start) echo "启动" ;;
来源：http://enp.cdnleiting.top

stop)  echo "停止" ;;
来源：http://euc.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://npc.nwbrower.top

esac
来源：http://mhx.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://zdz.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://ttn.yj20258.top

[R13] for 计数循环
来源：http://shy.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://bck.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://wdc.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kyi.svipenyu.cn

[R15] while 逐行读文件
来源：http://ndf.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ema.ydjk.org.cn

[R16] until 等待条件
来源：http://oof.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://air.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://dop.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vkw.chenzaomai.com

[R18] 遍历数组
来源：http://wsb.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wzc.gotoacloud.top

[R19] 数组长度
来源：http://nki.nwbrower.top

echo "${#arr[@]}"
来源：http://ebu.yangfankeji.com

[R20] 关联数组（字典）
来源：http://ujv.dashuyun.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vqv.shangyingyoupin.top

[R21] 字符串长度
来源：http://jjo.vqdsnc.cn

echo "${#s}"
来源：http://hvv.zdqjudy.top

[R22] 截取子串
来源：http://noy.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://iin.kuanghao11.cn

[R23] 字符串替换
来源：http://gjm.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://avf.yuanzhike.top

[R24] 大小写转换
来源：http://nnv.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://htd.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://fvj.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxh.ivvv.top

[R26] 命令替换
来源：http://yea.havefunace.top

now=$(date +%F); echo "$now"
来源：http://joe.haohaochexian.top

[R27] 算术展开
来源：http://dhr.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://otu.quarkkingdee.top

[R28] 浮点运算
来源：http://nzz.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://ciu.xuanzx.com

[R29] 定义函数
来源：http://zmf.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rth.cucudq.cn

[R30] 函数返回状态码
来源：http://mvi.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://fhp.bbcook.cn

[R31] 局部变量
来源：http://ytt.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://uxf.ydzc1.top

[R32] 参数个数校验
来源：http://qwk.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://smm.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://bqm.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsf.cqqwz.cn

[R34] 退出时清理
来源：http://hlm.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://ndv.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://wxa.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://umd.xylfe.cn

[R36] 并发执行多个任务
来源：http://gqt.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqx.hcnkem.com

[R37] 把输出赋给变量
来源：http://wkc.meibo888.top

files=$(ls -1)
来源：http://ljh.epnwcf.com

[R38] 管道串联
来源：http://ytm.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://uje.ivvv.top

[R39] 重定向标准输出与错误
来源：http://pog.nwbrower.top

cmd > out.log 2>&1
来源：http://iuj.bbcook.cn

[R40] 追加写日志
来源：http://sbc.gogol.net.cn

echo "log" >> out.log
来源：http://ijw.gzhubu.top

[R41] 丢弃输出
来源：http://fez.vehdjk.com

cmd >/dev/null 2>&1
来源：http://ovf.ehwqpu.com

[R42] 输入重定向
来源：http://pjb.chenjidiqi.icu

wc -l < a.txt
来源：http://wbq.sufxvd.cn

[R43] 按名字查找文件
来源：http://kdn.redwolf501.top

find . -name "*.log" -type f
来源：http://auc.hfpthk.cn

[R44] 按修改时间查找
来源：http://hjc.yfazqb.com

find . -mtime -7 -type f
来源：http://dld.shzxlz.cn

[R45] 批量删除
来源：http://xtj.ivvv.top

find . -name "*.tmp" -delete
来源：http://wwq.0kj1m.cn

[R46] 递归替换文件内容
来源：http://iwv.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qmh.sweek.top

[R47] sed 单行替换
来源：http://ite.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jlw.sufxvd.cn

[R48] awk 取指定列
来源：http://uch.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://vyw.sysykeji.top

[R49] awk 带条件
来源：http://trh.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gbo.quarkkingdee.top

[R50] awk 求和
来源：http://aqy.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://awz.yangfankeji.com

[R51] 排序去重取前几
来源：http://fuk.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bps.zhijiandao.cn

[R52] 统计行数
来源：http://hhu.dashuyun.cn

wc -l a.txt
来源：http://kgj.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://cmf.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ztz.yongpay.top

[R54] 比较两个文件
来源：http://kuy.daxiang520.top

diff a.txt b.txt
来源：http://uxn.9152youxi.cn

[R55] 压缩与解压
来源：http://twf.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://edy.hywenlv.cn

[R56] 远程拷贝
来源：http://jvx.cucudq.cn

scp file user@host:/path/
来源：http://qbq.xylfe.cn

[R57] 远程执行命令
来源：http://lav.yangfankeji.com

ssh user@host 'uptime'
来源：http://pkm.nanxuanxn.top

[R58] 下载文件
来源：http://vrp.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bai.dianchejie.cn

[R59] 发 POST JSON
来源：http://kkk.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jbe.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://utl.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cux.kuanghao11.cn

[R61] 磁盘占用
来源：http://ehf.redwolf501.top

df -h;  du -sh *
来源：http://rpn.yfazqb.com

[R62] 找最占空间的文件
来源：http://ebr.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://uqf.vehdjk.com

[R63] 内存与进程
来源：http://hyx.tarul.cn

free -h;  ps aux | grep nginx
来源：http://bwe.xinyue.icu

[R64] 结束进程
来源：http://ncb.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://nvf.zhijiandao.cn

[R65] 查看端口占用
来源：http://wcg.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lly.jinqigufen.top

[R66] 定时任务
来源：http://klf.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://rxe.hesvh.cn

[R67] 生成随机十六进制串
来源：http://cml.0kj1m.cn

openssl rand -hex 16
来源：http://yic.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://wmc.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bad.xuetiantiany.cn

[R69] 生成随机密码
来源：http://ftp.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://ayu.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://mwh.yj20258888.top

date +%s;  date -d @1700000000
来源：http://opv.zhiwuduotai.top

[R71] 日期格式化
来源：http://fxs.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lpy.jinqigufen.top

[R72] 等待端口就绪
来源：http://vdc.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mgo.fzhhl.top

[R73] 分割大日志
来源：http://alj.aizwys.cn

split -l 1000 big.log part_
来源：http://qla.yj20258.top

[R74] 批量重命名
来源：http://pcb.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://czs.zhixingplan.top

[R75] 导出环境变量
来源：http://jxt.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://jnz.ivvv.top

[R76] 使用临时文件
来源：http://ovq.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqc.vqdsnc.cn

[R77] 读取用户输入
来源：http://ewl.yangfankeji.com

read -rp "请输入: " ans
来源：http://awm.dashuyun.cn

[R78] 交互式菜单
来源：http://eht.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jhb.guannengcc.top

[R79] 解析命令行选项
来源：http://prw.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ter.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://csc.fanxiaobao.xyz

time ./run.sh
来源：http://bey.gaohongyu789.top

================================================================================
来源：http://vgl.guannengcc.top

S. C / C++ 专题
来源：http://yru.hfpthk.cn

================================================================================
来源：http://crm.chenzaomai.com

[S01] C：Hello World
来源：http://lid.ydjk.org.cn

#include <stdio.h>
来源：http://vyy.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fhp.hcnkem.com

[S02] C：变量与格式化输出
来源：http://rvz.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://kkg.jianghu66.top

[S03] C：读入整数
来源：http://xyw.aizwys.cn

int x; scanf("%d", &x);
来源：http://ydn.aibaodan.cn

[S04] C：字符串复制
来源：http://xfq.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://het.epnwcf.com

[S05] C：字符串长度
来源：http://aju.ywan-chungtsiang.top

strlen(s)
来源：http://kyx.chenzaomai.com

[S06] C：字符串比较
来源：http://qev.fengsongda.top

strcmp(a, b) == 0
来源：http://kgf.316326.xyz

[S07] C：数组遍历求和
来源：http://ufs.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://amv.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://pye.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zak.tanke756.top

[S09] C：结构体定义与初始化
来源：http://zom.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hht.ppjwa.cn

[S10] C：指针与解引用
来源：http://pcc.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://hvo.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://dqn.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://kiv.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uxf.haohaochexian.top

fclose(f);
来源：http://wml.jlsjyb.cn

[S12] C：写文件
来源：http://lhz.ivvv.top


<!-- 参考信息 -->