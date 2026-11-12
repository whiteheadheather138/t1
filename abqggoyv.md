代发 wailian999

SELECT * FROM users;
来源：http://rjf.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://cer.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://zgb.iojbl.cn

[Q17] 条件查询
来源：http://ipe.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ccf.tian-w.cn

[Q18] 模糊匹配
来源：http://zyc.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gzd.yuanzhike.top

[Q19] 范围查询
来源：http://xnp.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ymg.xziqi.cn

[Q20] IN 列表
来源：http://uzb.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oxs.pengpengdd.cyou

[Q21] 空值判断
来源：http://bfj.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://znj.9152youxi.cn

[Q22] 排序
来源：http://nru.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://frt.nanxuanxn.top

[Q23] 分页
来源：http://erj.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bfo.ctjpmb.com

[Q24] 去重
来源：http://rtw.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://fqi.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://bnb.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sqz.nanxinkj.top

[Q26] 计数
来源：http://xhc.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://ckm.hesvh.cn

[Q27] 条件计数
来源：http://yob.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://luh.ctjpmb.com

[Q28] 求和与平均
来源：http://zoy.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uvi.zhoulong.xyz

[Q29] 最大最小值
来源：http://fkb.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kyy.snrcjt.cn

[Q30] 分组统计
来源：http://jcx.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zqh.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://gor.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lnh.wangdashe.top

[Q32] 分组拼接字符串
来源：http://tdv.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fhl.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://shh.yonumen.top

[Q33] 多列分组
来源：http://akc.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vde.hfpthk.cn

[Q34] 每组取第一条
来源：http://qob.dianchejie.cn

SELECT * FROM (
来源：http://jzt.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ajl.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://iig.tianlin.xyz

[Q35] 内连接
来源：http://wju.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://shi.xylfe.cn

[Q36] 左连接
来源：http://nxo.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kmc.yueranfly.top

[Q37] 右连接
来源：http://xzf.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://atg.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://yyg.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wyt.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://ipt.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gqq.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tzx.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sqs.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fbq.havefunace.top

[Q41] 多表连接
来源：http://glw.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tio.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://bdn.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://mjt.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://eso.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://vil.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hrz.andypj.xyz

[Q43] 标量子查询
来源：http://ztr.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ebx.shzxlz.cn

[Q44] IN 子查询
来源：http://txs.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ymq.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://kwd.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sjz.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lvc.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ars.fzhhl.top

[Q47] 与平均值比较
来源：http://jiz.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nxo.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://xdf.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vfy.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ymh.pengpengdd.cyou

[Q49] 更新单行
来源：http://wjt.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://noy.yuxming.cn

[Q50] 批量更新
来源：http://evd.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ssp.xuanzx.com

[Q51] 用子查询更新
来源：http://obd.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cnw.andypj.xyz

[Q52] 删除指定行
来源：http://bsl.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://hsa.yanxiufei.cn

[Q53] 按条件删除
来源：http://wqh.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pfv.pengpengdd.cyou

[Q54] 清空表
来源：http://hyb.cheryme.top

TRUNCATE TABLE logs;
来源：http://ydu.hnqzz.top

[Q55] 排名（并列占位）
来源：http://rwf.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://apq.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://ukx.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehw.chenlongwang.top

[Q57] 行号
来源：http://ykl.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nqb.quarkkingdee.top

[Q58] 累计求和
来源：http://rhm.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uha.iojbl.cn

[Q59] 分组内累计
来源：http://dut.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zlz.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://asu.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vuv.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uoe.tian-w.cn

[Q61] 移动平均
来源：http://nvq.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vhr.andypj.xyz

[Q62] 分组占比
来源：http://wzx.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wwi.fengsongda.top

[Q63] 开启事务
来源：http://ule.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ckx.sjlbkw.cn

[Q64] 提交事务
来源：http://mvu.cashguo.top

COMMIT;
来源：http://iwz.dianchejie.cn

[Q65] 回滚事务
来源：http://dew.redwolf501.top

ROLLBACK;
来源：http://pta.jianghu66.top

[Q66] 行锁查询
来源：http://alt.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cza.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://nrv.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgl.yongpay.top

[Q68] 保存点
来源：http://kot.daxiang520.top

SAVEPOINT sp1;
来源：http://guj.birdmap.top

ROLLBACK TO sp1;
来源：http://xfd.316326.xyz

[Q69] 查看执行计划
来源：http://eed.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iak.jianghu66.top

[Q70] 更新统计信息
来源：http://nxv.tian-w.cn

ANALYZE TABLE users;
来源：http://scd.ivvv.top

[Q71] 查看建表语句
来源：http://gqw.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fhy.hnqzz.top

[Q72] 查看索引
来源：http://flf.pycfn.com

SHOW INDEX FROM users;
来源：http://ihx.sxryk.cn

[Q73] 查看表状态
来源：http://abo.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://toe.yangfankeji.com

[Q74] 强制使用索引
来源：http://eiw.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ioi.ydjk.org.cn

[Q75] 日期格式化
来源：http://ykg.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hed.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qau.cashguo.top

[Q76] 按天统计
来源：http://pfz.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ezi.aizwys.cn

[Q77] 时间加减
来源：http://qgv.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ufx.daria6918.cn

[Q78] 当前时间
来源：http://irj.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bzw.cqqwz.cn

[Q79] 字符串拼接
来源：http://hnw.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chh.hongshengwenyu.top

[Q80] 字符串截取
来源：http://txw.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ggg.zhixingplan.top

[Q81] 字符串替换
来源：http://aay.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xnv.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://ggi.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hyu.fehbvm.com

[Q83] 大小写转换
来源：http://ivi.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ilv.sufxvd.cn

[Q84] 去除首尾空格
来源：http://gth.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://dhu.cashguo.top

[Q85] 数值取整
来源：http://exb.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nvw.meibo888.top

[Q86] 读取 JSON 字段
来源：http://ugq.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cww.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://udc.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pqn.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://uoc.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyk.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://luj.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://obw.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vrs.hammf.cn

[Q90] 生成序号列
来源：http://zsc.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gzr.shanyushiyangtech.top

================================================================================
来源：http://rwr.quarkkingdee.top

R. Bash 专题
来源：http://xjb.yvedp.cn

================================================================================
来源：http://tls.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://oja.hcnkem.com

#!/usr/bin/env bash
来源：http://gid.nanxuanxn.top

set -euo pipefail
来源：http://vzq.yj20258888.top

[R02] 变量赋值与使用
来源：http://vrk.mhx1999.top

name="Tom"; echo "$name"
来源：http://umb.smart0.xyz

[R03] 只读变量
来源：http://pao.nanxuanxn.top

readonly PI=3.14
来源：http://yew.ivvv.top

[R04] 位置参数
来源：http://zpm.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fkn.9152youxi.cn

[R05] 参数默认值
来源：http://ccj.jinqigufen.top

name="${1:-default}"
来源：http://wpj.birdmap.top

[R06] 判断命令是否存在
来源：http://bno.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jpv.hcnkem.com

[R07] if 判断文件
来源：http://ujd.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fpk.xziqi.cn

[R08] 数值比较
来源：http://vsg.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://azl.fzhhl.top

[R09] 字符串比较
来源：http://slo.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kvb.cucudq.cn

[R10] 正则匹配
来源：http://xhh.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ebs.0kj1m.cn

[R11] case 多分支
来源：http://iqz.ydjk.org.cn

case "$1" in
来源：http://enr.jqgufenzy.top

start) echo "启动" ;;
来源：http://lkl.hfpthk.cn

stop)  echo "停止" ;;
来源：http://udx.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://inw.aizwys.cn

esac
来源：http://ddm.zhengqikj.top

[R12] for 遍历文件
来源：http://yzs.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://kmv.pycfn.com

[R13] for 计数循环
来源：http://eny.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://nui.feifeiyinyue.top

[R14] C 风格 for
来源：http://fpf.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://scg.nwbrower.top

[R15] while 逐行读文件
来源：http://fpy.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://stn.snrcjt.cn

[R16] until 等待条件
来源：http://pwm.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lgt.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://hfu.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://llo.xziqi.cn

[R18] 遍历数组
来源：http://jgs.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kdn.yuxming.cn

[R19] 数组长度
来源：http://mcm.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://uph.birdmap.top

[R20] 关联数组（字典）
来源：http://fol.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tab.xziqi.cn

[R21] 字符串长度
来源：http://egr.yfazqb.com

echo "${#s}"
来源：http://cwn.guowangkeji.top

[R22] 截取子串
来源：http://agc.yonumen.top

echo "${s:0:5}"
来源：http://uwa.yuanzhike.top

[R23] 字符串替换
来源：http://miz.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fef.kuanghao11.cn

[R24] 大小写转换
来源：http://bjp.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://krc.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://obp.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mhr.zycfv.cn

[R26] 命令替换
来源：http://cti.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://alu.yj20258888.top

[R27] 算术展开
来源：http://hfe.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://oqo.shuidangran.top

[R28] 浮点运算
来源：http://gda.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://jty.cdnleiting.top

[R29] 定义函数
来源：http://lmg.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://buh.fktsv.cn

[R30] 函数返回状态码
来源：http://cen.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://zyz.tianlin.xyz

[R31] 局部变量
来源：http://knl.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://ryb.jinqigfzy.top

[R32] 参数个数校验
来源：http://ymq.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gfv.hammf.cn

[R33] 捕获错误并提示行号
来源：http://gkw.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fpd.wangdashe.top

[R34] 退出时清理
来源：http://ssf.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eab.ydzc1.top

[R35] 后台执行并等待
来源：http://erv.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://twk.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://yix.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pxf.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://apy.guowangkeji.top

files=$(ls -1)
来源：http://ucq.svipenyu.cn

[R38] 管道串联
来源：http://akf.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://sux.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://xvw.fktsv.cn

cmd > out.log 2>&1
来源：http://upg.gogol.net.cn

[R40] 追加写日志
来源：http://dye.yanxiufei.cn

echo "log" >> out.log
来源：http://ztu.c1oappe.top

[R41] 丢弃输出
来源：http://dvz.guannengcc.top

cmd >/dev/null 2>&1
来源：http://app.yuxming.cn

[R42] 输入重定向
来源：http://vxn.haohaochexian.top

wc -l < a.txt
来源：http://pil.ydjk.org.cn

[R43] 按名字查找文件
来源：http://dgi.zhengqikj.top

find . -name "*.log" -type f
来源：http://srj.sjlbkw.cn

[R44] 按修改时间查找
来源：http://pyh.yueranfly.top

find . -mtime -7 -type f
来源：http://gqu.yuanzhike.top

[R45] 批量删除
来源：http://qpj.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://tiw.jqgfzy.top

[R46] 递归替换文件内容
来源：http://xfq.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxh.nwbrower.top

[R47] sed 单行替换
来源：http://mmg.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tiz.nanxinkj.top

[R48] awk 取指定列
来源：http://luo.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://mie.hysaishi.cn

[R49] awk 带条件
来源：http://oig.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uwq.yj20258888.top

[R50] awk 求和
来源：http://lok.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://sau.hammf.cn

[R51] 排序去重取前几
来源：http://swu.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kiq.hammf.cn

[R52] 统计行数
来源：http://guz.jianghu66.top

wc -l a.txt
来源：http://xpy.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://ipq.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zrd.jlsjyb.cn

[R54] 比较两个文件
来源：http://dmx.ehwqpu.com

diff a.txt b.txt
来源：http://jed.ydzc1.top

[R55] 压缩与解压
来源：http://ohp.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ebw.aibaodan.cn

[R56] 远程拷贝
来源：http://wsy.cucudq.cn

scp file user@host:/path/
来源：http://dpy.tian-w.cn

[R57] 远程执行命令
来源：http://wtv.fktsv.cn

ssh user@host 'uptime'
来源：http://bkh.ctjpmb.com

[R58] 下载文件
来源：http://cbw.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kor.sufxvd.cn

[R59] 发 POST JSON
来源：http://ezm.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fnd.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://wyy.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mpl.316326.xyz

[R61] 磁盘占用
来源：http://tsc.uphjek.com

df -h;  du -sh *
来源：http://wyg.xinyue.icu

[R62] 找最占空间的文件
来源：http://cht.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://dif.bjfxy.top

[R63] 内存与进程
来源：http://fry.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://gpj.svipenyu.cn

[R64] 结束进程
来源：http://ach.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://rmz.jyoumei.cn

[R65] 查看端口占用
来源：http://xzk.tanke756.top


<!-- 参考信息 -->