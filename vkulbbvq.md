代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iwb.hywenlv.cn

[Q28] 求和与平均
来源：http://bst.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ukb.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://hij.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://txk.0kj1m.cn

[Q30] 分组统计
来源：http://xrf.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ysq.birdmap.top

[Q31] 分组后过滤
来源：http://voh.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lnk.yuxming.cn

[Q32] 分组拼接字符串
来源：http://dqx.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uol.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://psg.sufxvd.cn

[Q33] 多列分组
来源：http://jyc.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://liq.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://plc.meibo888.top

SELECT * FROM (
来源：http://dnl.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fch.vqdsnc.cn

) t WHERE rn = 1;
来源：http://sdq.ydzc1.top

[Q35] 内连接
来源：http://out.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://isv.jinqigfzy.top

[Q36] 左连接
来源：http://sha.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ubn.cqqwz.cn

[Q37] 右连接
来源：http://kdt.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bbk.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eds.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tyk.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://mpm.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://brh.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cgn.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zbc.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xcu.vqdsnc.cn

[Q41] 多表连接
来源：http://owb.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ith.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://ecz.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://zju.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://nft.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://qsy.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xhh.jinqigufen.top

[Q43] 标量子查询
来源：http://uzi.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://szy.nwbrower.top

[Q44] IN 子查询
来源：http://ekk.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gkc.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://yzy.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybg.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://seq.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://opx.hywenlv.cn

[Q47] 与平均值比较
来源：http://fqe.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tmu.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://bfd.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jmf.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://ppp.shangyingyoupin.top

[Q49] 更新单行
来源：http://adm.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://muf.zhixingplan.top

[Q50] 批量更新
来源：http://byr.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lbl.hywenlv.cn

[Q51] 用子查询更新
来源：http://bwu.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ygt.cqqwz.cn

[Q52] 删除指定行
来源：http://xcj.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://uov.fengsongda.top

[Q53] 按条件删除
来源：http://jmi.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wvo.vehdjk.com

[Q54] 清空表
来源：http://chf.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://kme.fehbvm.com

[Q55] 排名（并列占位）
来源：http://dnk.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rib.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://jlp.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oie.zhiwuduotai.top

[Q57] 行号
来源：http://eaw.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://awh.ivvv.top

[Q58] 累计求和
来源：http://hpz.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jlw.hywenlv.cn

[Q59] 分组内累计
来源：http://xnv.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kgc.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://mgb.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hoj.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rli.epnwcf.com

[Q61] 移动平均
来源：http://hgu.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://luq.sjlbkw.cn

[Q62] 分组占比
来源：http://pyx.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nbs.birdmap.top

[Q63] 开启事务
来源：http://jzn.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fqr.xziqi.cn

[Q64] 提交事务
来源：http://vyl.xuanzx.com

COMMIT;
来源：http://kya.cdnleiting.top

[Q65] 回滚事务
来源：http://kon.sysykeji.top

ROLLBACK;
来源：http://ytw.sufxvd.cn

[Q66] 行锁查询
来源：http://sqs.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tdr.fktsv.cn

[Q67] 设置隔离级别
来源：http://ryx.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ihz.guannengcc.top

[Q68] 保存点
来源：http://rlc.sxryk.cn

SAVEPOINT sp1;
来源：http://ajo.xylfe.cn

ROLLBACK TO sp1;
来源：http://ejy.dianchejie.cn

[Q69] 查看执行计划
来源：http://hwr.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hwl.shuidangran.top

[Q70] 更新统计信息
来源：http://ohd.nanxuanxn.top

ANALYZE TABLE users;
来源：http://asx.jinqigufen.top

[Q71] 查看建表语句
来源：http://cqk.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kgj.ctjpmb.com

[Q72] 查看索引
来源：http://taa.yonumen.top

SHOW INDEX FROM users;
来源：http://chb.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://lsk.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://azp.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://ars.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ejz.havefunace.top

[Q75] 日期格式化
来源：http://cba.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fli.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tcf.tian-w.cn

[Q76] 按天统计
来源：http://mwg.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://emr.xuetiantiany.cn

[Q77] 时间加减
来源：http://jpq.xuetiantiany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nrt.hammf.cn

[Q78] 当前时间
来源：http://stn.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbq.jyoumei.cn

[Q79] 字符串拼接
来源：http://fut.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vzd.zdbjq.cn

[Q80] 字符串截取
来源：http://mpw.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rkk.havefunace.top

[Q81] 字符串替换
来源：http://gky.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwe.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://sgx.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xtm.yanxiufei.cn

[Q83] 大小写转换
来源：http://uhj.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zgi.shuidangran.top

[Q84] 去除首尾空格
来源：http://vzi.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://jmc.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://sbi.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://siu.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://zjg.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://phq.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://cge.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://egf.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://mvq.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gji.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://arh.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://ywh.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sot.yuxming.cn

[Q90] 生成序号列
来源：http://xwf.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ksx.316326.xyz

================================================================================
来源：http://oiz.vehdjk.com

R. Bash 专题
来源：http://hcn.shzxlz.cn

================================================================================
来源：http://wcc.tianlin.xyz

[R01] shebang 与严格模式
来源：http://dka.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://cdu.sweek.top

set -euo pipefail
来源：http://zpq.hcnkem.com

[R02] 变量赋值与使用
来源：http://lis.hfpthk.cn

name="Tom"; echo "$name"
来源：http://pan.snrcjt.cn

[R03] 只读变量
来源：http://lpa.jqgfzy.top

readonly PI=3.14
来源：http://jpo.yvedp.cn

[R04] 位置参数
来源：http://hnh.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wyl.zhengqikj.top

[R05] 参数默认值
来源：http://zzr.aizwys.cn

name="${1:-default}"
来源：http://tcj.mhx1999.top

[R06] 判断命令是否存在
来源：http://aoc.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sat.zhiwuduotai.top

[R07] if 判断文件
来源：http://cxb.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oiq.wangshuangyany.cn

[R08] 数值比较
来源：http://cqz.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xgk.haohaochexian.top

[R09] 字符串比较
来源：http://iag.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://drf.yj20258888.top

[R10] 正则匹配
来源：http://miw.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gyg.tianlin.xyz

[R11] case 多分支
来源：http://cva.wangdashe.top

case "$1" in
来源：http://bzh.havefunace.top

start) echo "启动" ;;
来源：http://qeq.jyoumei.cn

stop)  echo "停止" ;;
来源：http://nbo.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://puj.shzxlz.cn

esac
来源：http://mwl.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://fid.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://sap.wangdashe.top

[R13] for 计数循环
来源：http://vil.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://xda.jqgfzy.top

[R14] C 风格 for
来源：http://fwq.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gei.aibaodan.cn

[R15] while 逐行读文件
来源：http://dmw.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tyt.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://wxb.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zwd.xziqi.cn

[R17] 数组定义与取值
来源：http://qcj.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nkl.jinqigfzy.top

[R18] 遍历数组
来源：http://ddy.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rny.snrcjt.cn

[R19] 数组长度
来源：http://keb.jlsjyb.cn

echo "${#arr[@]}"
来源：http://ddw.xziqi.cn

[R20] 关联数组（字典）
来源：http://pjj.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ygr.shzxlz.cn

[R21] 字符串长度
来源：http://wkw.xylfe.cn

echo "${#s}"
来源：http://fsk.zdbjq.cn

[R22] 截取子串
来源：http://pvw.jinqigfzy.top

echo "${s:0:5}"
来源：http://qti.yj20258.top

[R23] 字符串替换
来源：http://hgp.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gca.nwbrower.top

[R24] 大小写转换
来源：http://ybd.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://vdx.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://gxl.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fdr.havefunace.top

[R26] 命令替换
来源：http://jce.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://ori.c1oappe.top

[R27] 算术展开
来源：http://hvy.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://hsq.ydzc1.top

[R28] 浮点运算
来源：http://ocl.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://tsd.sjlbkw.cn

[R29] 定义函数
来源：http://rtw.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bft.jyoumei.cn

[R30] 函数返回状态码
来源：http://qco.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://idc.yfazqb.com

[R31] 局部变量
来源：http://jpw.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://kly.uphjek.com

[R32] 参数个数校验
来源：http://hia.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://chm.hammf.cn

[R33] 捕获错误并提示行号
来源：http://oor.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bdr.cashguo.top

[R34] 退出时清理
来源：http://oev.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://udg.redwolf501.top

[R35] 后台执行并等待
来源：http://mcu.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://siw.yj20258888.top

[R36] 并发执行多个任务
来源：http://zvm.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjl.tian-w.cn

[R37] 把输出赋给变量
来源：http://ddu.ppjwa.cn

files=$(ls -1)
来源：http://lqf.yuanzhike.top

[R38] 管道串联
来源：http://lna.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://wru.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://eih.hnqzz.top

cmd > out.log 2>&1
来源：http://kqj.zhongyouzk.top

[R40] 追加写日志
来源：http://gjw.hysaishi.cn

echo "log" >> out.log
来源：http://izt.0kj1m.cn

[R41] 丢弃输出
来源：http://xyc.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://pqa.yfazqb.com

[R42] 输入重定向
来源：http://vuv.dashuyun.cn

wc -l < a.txt
来源：http://qqc.chenlongwang.top

[R43] 按名字查找文件
来源：http://eym.hammf.cn

find . -name "*.log" -type f
来源：http://qju.hywenlv.cn

[R44] 按修改时间查找
来源：http://lrj.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://ivu.andypj.xyz

[R45] 批量删除
来源：http://boq.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://ido.daxiang520.top

[R46] 递归替换文件内容
来源：http://eiq.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://maa.cucudq.cn

[R47] sed 单行替换
来源：http://ofe.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://mad.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://vbt.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://fkn.cqqwz.cn

[R49] awk 带条件
来源：http://upw.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://knr.meibo888.top

[R50] awk 求和
来源：http://hxl.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://cxz.jqgfzy.top

[R51] 排序去重取前几
来源：http://nka.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yxj.aizwys.cn

[R52] 统计行数
来源：http://uom.ppjwa.cn

wc -l a.txt
来源：http://fkx.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://dmj.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ixl.pycfn.com

[R54] 比较两个文件
来源：http://trk.fengsongda.top

diff a.txt b.txt
来源：http://dsa.jinqigfzy.top

[R55] 压缩与解压
来源：http://srf.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rmt.jqgufenzy.top

[R56] 远程拷贝
来源：http://mas.ppjwa.cn

scp file user@host:/path/
来源：http://hic.daxiang520.top

[R57] 远程执行命令
来源：http://tjj.yanxiufei.cn

ssh user@host 'uptime'
来源：http://jms.redwolf501.top

[R58] 下载文件
来源：http://ary.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sex.nwbrower.top

[R59] 发 POST JSON
来源：http://tbl.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dos.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://ilv.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dsn.bjfxy.top

[R61] 磁盘占用
来源：http://jqp.tian-w.cn

df -h;  du -sh *
来源：http://zez.zdqjudy.top

[R62] 找最占空间的文件
来源：http://ngg.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://xrp.smart0.xyz

[R63] 内存与进程
来源：http://lto.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://deo.aizwys.cn

[R64] 结束进程
来源：http://fnh.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://nsx.hnxiangtu.top

[R65] 查看端口占用
来源：http://bmz.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xnd.zdbjq.cn

[R66] 定时任务
来源：http://vof.yj20258888.top

crontab -e;  crontab -l
来源：http://kqa.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://puf.daxiang520.top

openssl rand -hex 16
来源：http://knx.smart0.xyz

[R68] 计算文件校验值
来源：http://vbj.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ony.hcnkem.com

[R69] 生成随机密码
来源：http://pcb.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://irg.pycfn.com

[R70] 时间戳与互转
来源：http://zqs.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://mjk.daria6918.cn

[R71] 日期格式化
来源：http://reg.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ncu.vehdjk.com

[R72] 等待端口就绪
来源：http://uqh.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pzy.zhixingplan.top

[R73] 分割大日志
来源：http://uor.sysykeji.top

split -l 1000 big.log part_
来源：http://tnf.hongshengwenyu.top

[R74] 批量重命名
来源：http://ugo.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozt.cheryme.top

[R75] 导出环境变量
来源：http://dfx.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://mbp.zhengqikj.top

[R76] 使用临时文件
来源：http://ahe.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://een.gaohongyu789.top

[R77] 读取用户输入
来源：http://per.jianghu66.top


<!-- 参考信息 -->