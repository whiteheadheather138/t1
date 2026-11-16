代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://kon.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sog.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://drd.birdmap.top

[Q15] 查询全部
来源：http://iyw.yangfankeji.com

SELECT * FROM users;
来源：http://btg.guowangkeji.top

[Q16] 查询指定列
来源：http://pam.andypj.xyz

SELECT id, name FROM users;
来源：http://kjx.xinyue.icu

[Q17] 条件查询
来源：http://kdj.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://emg.yj202588.top

[Q18] 模糊匹配
来源：http://vhd.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://foz.hnqzz.top

[Q19] 范围查询
来源：http://sjo.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dta.zdqjudy.top

[Q20] IN 列表
来源：http://fyu.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://duo.vehdjk.com

[Q21] 空值判断
来源：http://wdl.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://vpy.feifeiyinyue.top

[Q22] 排序
来源：http://pne.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qhr.yuxming.cn

[Q23] 分页
来源：http://jsx.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ddw.tianlin.xyz

[Q24] 去重
来源：http://qvq.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://ssm.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://wph.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dyk.wangshuangyany.cn

[Q26] 计数
来源：http://cbn.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://snd.9152youxi.cn

[Q27] 条件计数
来源：http://hbz.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mdk.hywenlv.cn

[Q28] 求和与平均
来源：http://scn.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xhm.nwbrower.top

[Q29] 最大最小值
来源：http://mxk.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://crp.fehbvm.com

[Q30] 分组统计
来源：http://ajq.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mhp.gotoacloud.top

[Q31] 分组后过滤
来源：http://knm.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hao.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://qmu.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://biw.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://prb.yj202588.top

[Q33] 多列分组
来源：http://xym.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wwv.shuidangran.top

[Q34] 每组取第一条
来源：http://zoq.ppjwa.cn

SELECT * FROM (
来源：http://fpw.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gzj.yvedp.cn

) t WHERE rn = 1;
来源：http://yyb.sweek.top

[Q35] 内连接
来源：http://vkt.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xsi.zdqjudy.top

[Q36] 左连接
来源：http://fky.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zym.ppjwa.cn

[Q37] 右连接
来源：http://ytl.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://myc.tian-w.cn

[Q38] 全外连接（PostgreSQL）
来源：http://obz.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://owh.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://vmb.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gen.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://meg.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zcv.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aet.yongpay.top

[Q41] 多表连接
来源：http://udd.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://huq.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://kmt.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://dru.meibo888.top

[Q42] 连接条件附加过滤
来源：http://pvj.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://jph.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gvy.cucudq.cn

[Q43] 标量子查询
来源：http://zxg.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ywr.yvedp.cn

[Q44] IN 子查询
来源：http://zil.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcb.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://vsc.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpw.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://oqu.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hok.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://npq.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fxu.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://crn.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uqg.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://zwk.cqqwz.cn

[Q49] 更新单行
来源：http://zow.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zzf.mhx1999.top

[Q50] 批量更新
来源：http://jka.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mon.snrcjt.cn

[Q51] 用子查询更新
来源：http://rvd.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jna.yvedp.cn

[Q52] 删除指定行
来源：http://gvy.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://jqc.chenlongwang.top

[Q53] 按条件删除
来源：http://mzs.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hbs.hnxiangtu.top

[Q54] 清空表
来源：http://xwy.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://jmv.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://rfj.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://enq.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://vrm.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zsc.hnqzz.top

[Q57] 行号
来源：http://blj.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://liw.shzxlz.cn

[Q58] 累计求和
来源：http://fxj.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zfx.52xcode.cn

[Q59] 分组内累计
来源：http://yex.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jzn.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://hee.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xvm.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lnb.cheryme.top

[Q61] 移动平均
来源：http://wjx.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vnm.tarul.cn

[Q62] 分组占比
来源：http://gbn.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gfq.sweek.top

[Q63] 开启事务
来源：http://dyw.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wov.mhx1999.top

[Q64] 提交事务
来源：http://aiu.xuetiantiany.cn

COMMIT;
来源：http://fjy.bjfxy.top

[Q65] 回滚事务
来源：http://ljx.hcnkem.com

ROLLBACK;
来源：http://gxj.tianlin.xyz

[Q66] 行锁查询
来源：http://mrr.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zyv.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://ceb.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pbm.dashuyun.cn

[Q68] 保存点
来源：http://jvg.ydjk.org.cn

SAVEPOINT sp1;
来源：http://qfr.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://ryo.chenzaomai.com

[Q69] 查看执行计划
来源：http://asi.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xby.fktsv.cn

[Q70] 更新统计信息
来源：http://psq.cdnleiting.top

ANALYZE TABLE users;
来源：http://jlr.uphjek.com

[Q71] 查看建表语句
来源：http://bpv.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xpf.shangyingyoupin.top

[Q72] 查看索引
来源：http://xry.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://mmc.9152youxi.cn

[Q73] 查看表状态
来源：http://fao.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gnh.tian-w.cn

[Q74] 强制使用索引
来源：http://xvd.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xmn.chenlongwang.top

[Q75] 日期格式化
来源：http://jxs.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yps.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eoj.chenjidiqi.icu

[Q76] 按天统计
来源：http://egu.xylfe.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wgj.gaohongyu789.top

[Q77] 时间加减
来源：http://kpu.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://spq.bjfxy.top

[Q78] 当前时间
来源：http://spf.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://umy.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://gse.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkm.jqgufenzy.top

[Q80] 字符串截取
来源：http://rah.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iwf.yuxming.cn

[Q81] 字符串替换
来源：http://cjp.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zhg.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://bxo.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dpj.hywenlv.cn

[Q83] 大小写转换
来源：http://iew.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sgx.epnwcf.com

[Q84] 去除首尾空格
来源：http://lwd.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://izx.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://uga.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yej.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://gjl.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ocj.smart0.xyz

[Q87] JSON 字段做条件
来源：http://xbe.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fmh.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://lmq.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tzl.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mvk.cashguo.top

[Q89] 判断表是否存在
来源：http://gzk.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://emt.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://lso.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://niv.zhaomingkeji.xyz

================================================================================
来源：http://mfk.ctjpmb.com

R. Bash 专题
来源：http://zta.0kj1m.cn

================================================================================
来源：http://uop.vehdjk.com

[R01] shebang 与严格模式
来源：http://pmn.zhongyouzk.top

#!/usr/bin/env bash
来源：http://kip.pycfn.com

set -euo pipefail
来源：http://xzi.guowangkeji.top

[R02] 变量赋值与使用
来源：http://wvo.ybcxt.top

name="Tom"; echo "$name"
来源：http://igh.jlsjyb.cn

[R03] 只读变量
来源：http://vuf.yj20258.top

readonly PI=3.14
来源：http://yzu.haohaochexian.top

[R04] 位置参数
来源：http://uud.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aco.quarkkingdee.top

[R05] 参数默认值
来源：http://mef.ywan-chungtsiang.top

name="${1:-default}"
来源：http://jgt.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://biy.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mih.shuidangran.top

[R07] if 判断文件
来源：http://znn.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mqz.jyoumei.cn

[R08] 数值比较
来源：http://ywn.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eri.wangshuangyany.cn

[R09] 字符串比较
来源：http://skt.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://toc.tarul.cn

[R10] 正则匹配
来源：http://ahh.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gvx.nwbrower.top

[R11] case 多分支
来源：http://ryj.shuidangran.top

case "$1" in
来源：http://arv.cucudq.cn

start) echo "启动" ;;
来源：http://ivx.snrcjt.cn

stop)  echo "停止" ;;
来源：http://sej.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://yao.andypj.xyz

esac
来源：http://hmy.yvedp.cn

[R12] for 遍历文件
来源：http://qnt.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://qac.hywenlv.cn

[R13] for 计数循环
来源：http://mxn.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://qim.hnxiangtu.top

[R14] C 风格 for
来源：http://unj.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqp.uphjek.com

[R15] while 逐行读文件
来源：http://zxo.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zzx.meibo888.top

[R16] until 等待条件
来源：http://udg.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uky.aibaodan.cn

[R17] 数组定义与取值
来源：http://iwc.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://wne.jinqigufen.top

[R18] 遍历数组
来源：http://mqe.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bnc.jinyuanbaomall.cn

[R19] 数组长度
来源：http://ora.sxryk.cn

echo "${#arr[@]}"
来源：http://crc.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://qku.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vuq.zhijiandao.cn

[R21] 字符串长度
来源：http://aap.zdbjq.cn

echo "${#s}"
来源：http://bhf.zhiwuduotai.top

[R22] 截取子串
来源：http://obt.sxryk.cn

echo "${s:0:5}"
来源：http://vxy.fktsv.cn

[R23] 字符串替换
来源：http://zte.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fhk.zhixingplan.top

[R24] 大小写转换
来源：http://bvy.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://hza.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://hnb.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pxi.zhaomingkeji.xyz

[R26] 命令替换
来源：http://qpc.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://ixl.52xcode.cn

[R27] 算术展开
来源：http://daj.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://gss.ydzc1.top

[R28] 浮点运算
来源：http://gio.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://bjq.zdqjudy.top

[R29] 定义函数
来源：http://uxd.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://afm.52xcode.cn

[R30] 函数返回状态码
来源：http://ejz.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://xfh.chenlongwang.top

[R31] 局部变量
来源：http://rvm.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://dyl.hesvh.cn

[R32] 参数个数校验
来源：http://doe.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xld.havefunace.top

[R33] 捕获错误并提示行号
来源：http://tch.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://thg.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://rud.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zdj.xinyue.icu

[R35] 后台执行并等待
来源：http://tzs.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://byw.wangdashe.top

[R36] 并发执行多个任务
来源：http://drp.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jit.ydzc1.top

[R37] 把输出赋给变量
来源：http://nrp.chenjidiqi.icu

files=$(ls -1)
来源：http://krz.guowangkeji.top

[R38] 管道串联
来源：http://exz.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://slb.yonumen.top

[R39] 重定向标准输出与错误
来源：http://tfi.nwbrower.top

cmd > out.log 2>&1
来源：http://jpe.hnxiangtu.top

[R40] 追加写日志
来源：http://uiw.wangshuangyany.cn

echo "log" >> out.log
来源：http://ldb.yueranfly.top

[R41] 丢弃输出
来源：http://gln.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://vgy.zhengqikj.top

[R42] 输入重定向
来源：http://ruz.jlsjyb.cn

wc -l < a.txt
来源：http://woq.sxryk.cn

[R43] 按名字查找文件
来源：http://ezu.zhengqikj.top

find . -name "*.log" -type f
来源：http://ygm.cheryme.top

[R44] 按修改时间查找
来源：http://jax.hnxiangtu.top

find . -mtime -7 -type f
来源：http://yje.tanke756.top

[R45] 批量删除
来源：http://lzs.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://gjn.yueranfly.top

[R46] 递归替换文件内容
来源：http://ilg.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ruj.cdnleiting.top

[R47] sed 单行替换
来源：http://oga.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://epc.xziqi.cn

[R48] awk 取指定列
来源：http://hap.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://zcx.chenlongwang.top

[R49] awk 带条件
来源：http://cwn.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zrn.nanxuanxn.top

[R50] awk 求和
来源：http://iuk.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpg.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://wev.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xgo.zhoulong.xyz

[R52] 统计行数
来源：http://xwd.chenjidiqi.icu

wc -l a.txt
来源：http://bci.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://tqv.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vyx.uphjek.com

[R54] 比较两个文件
来源：http://zcx.svipenyu.cn

diff a.txt b.txt
来源：http://ule.wangdashe.top

[R55] 压缩与解压
来源：http://fdv.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eto.bbcook.cn

[R56] 远程拷贝
来源：http://bpu.daria6918.cn

scp file user@host:/path/
来源：http://yde.xinyue.icu

[R57] 远程执行命令
来源：http://drg.guannengcc.top

ssh user@host 'uptime'
来源：http://yvb.hammf.cn

[R58] 下载文件
来源：http://tpy.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yxj.hnxiangtu.top

[R59] 发 POST JSON
来源：http://azo.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aqf.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://xon.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbn.kuanghao11.cn

[R61] 磁盘占用
来源：http://xjk.sweek.top

df -h;  du -sh *
来源：http://onx.daria6918.cn

[R62] 找最占空间的文件
来源：http://dxr.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://ptg.hywenlv.cn

[R63] 内存与进程
来源：http://gkf.jiagoushi.top


<!-- 参考信息 -->