代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://atr.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ruc.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bcz.tanke756.top

[Q15] 查询全部
来源：http://mle.yanxiufei.cn

SELECT * FROM users;
来源：http://evb.cdnleiting.top

[Q16] 查询指定列
来源：http://qmd.chenzaomai.com

SELECT id, name FROM users;
来源：http://wxz.yfazqb.com

[Q17] 条件查询
来源：http://gin.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dma.jiagoushi.top

[Q18] 模糊匹配
来源：http://csc.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://znk.tian-w.cn

[Q19] 范围查询
来源：http://zdt.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://win.cucudq.cn

[Q20] IN 列表
来源：http://ffw.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bjj.jlsjyb.cn

[Q21] 空值判断
来源：http://jek.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mao.gotoacloud.top

[Q22] 排序
来源：http://sdd.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qui.hesvh.cn

[Q23] 分页
来源：http://tac.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hjo.dashuyun.cn

[Q24] 去重
来源：http://zpf.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://kkh.uphjek.com

[Q25] 只取前 N 条
来源：http://glk.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cpq.aibaodan.cn

[Q26] 计数
来源：http://ars.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://qrv.fengsongda.top

[Q27] 条件计数
来源：http://pup.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tkx.daria6918.cn

[Q28] 求和与平均
来源：http://zbv.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jsr.aizwys.cn

[Q29] 最大最小值
来源：http://ihm.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ywg.zhijiandao.cn

[Q30] 分组统计
来源：http://aja.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ajl.dianchejie.cn

[Q31] 分组后过滤
来源：http://thy.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nzv.fengsongda.top

[Q32] 分组拼接字符串
来源：http://nkw.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://edw.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sgk.bbcook.cn

[Q33] 多列分组
来源：http://sfy.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qrt.jinqigufen.top

[Q34] 每组取第一条
来源：http://hoe.svipenyu.cn

SELECT * FROM (
来源：http://amt.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kpx.yuxming.cn

) t WHERE rn = 1;
来源：http://bli.redwolf501.top

[Q35] 内连接
来源：http://prl.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hob.gaohongyu789.top

[Q36] 左连接
来源：http://jql.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tpa.cucudq.cn

[Q37] 右连接
来源：http://omn.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qmw.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tni.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ipe.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://zer.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ydl.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rje.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lud.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eww.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://wnf.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zxw.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://zoi.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://ayi.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://plx.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://vwj.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yin.chenlongwang.top

[Q43] 标量子查询
来源：http://beb.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ceu.redwolf501.top

[Q44] IN 子查询
来源：http://tvx.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ihe.hammf.cn

[Q45] EXISTS 判断存在
来源：http://dbq.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rxm.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ndy.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oxw.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://aiv.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hhb.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://poy.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://efb.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://npj.uphjek.com

[Q49] 更新单行
来源：http://wjs.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bxx.hnxiangtu.top

[Q50] 批量更新
来源：http://wql.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ong.yuanzhike.top

[Q51] 用子查询更新
来源：http://jah.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ayq.jinqigfzy.top

[Q52] 删除指定行
来源：http://qyc.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://hya.iojbl.cn

[Q53] 按条件删除
来源：http://fpk.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kzx.yj20258888.top

[Q54] 清空表
来源：http://rag.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://xox.daxiang520.top

[Q55] 排名（并列占位）
来源：http://wvi.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hmq.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://eay.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aob.sysykeji.top

[Q57] 行号
来源：http://fld.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://amb.zhengqikj.top

[Q58] 累计求和
来源：http://jxa.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ore.cdnleiting.top

[Q59] 分组内累计
来源：http://ctp.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xmp.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://hxr.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gzj.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tkz.pengpengdd.cyou

[Q61] 移动平均
来源：http://ncv.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hrk.nanxinkj.top

[Q62] 分组占比
来源：http://vnl.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kia.xuetiantiany.cn

[Q63] 开启事务
来源：http://jel.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://arm.chenlongwang.top

[Q64] 提交事务
来源：http://qqg.yanxiufei.cn

COMMIT;
来源：http://hif.wangshuangyany.cn

[Q65] 回滚事务
来源：http://tdj.aizwys.cn

ROLLBACK;
来源：http://miy.xziqi.cn

[Q66] 行锁查询
来源：http://fgk.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://owg.nanxinkj.top

[Q67] 设置隔离级别
来源：http://hbx.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jcv.hammf.cn

[Q68] 保存点
来源：http://yps.kuanghao11.cn

SAVEPOINT sp1;
来源：http://cbw.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://llq.xuanzx.com

[Q69] 查看执行计划
来源：http://rot.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mnk.hammf.cn

[Q70] 更新统计信息
来源：http://rgb.ehwqpu.com

ANALYZE TABLE users;
来源：http://keb.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://jyv.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lfo.xinyue.icu

[Q72] 查看索引
来源：http://aqm.ppjwa.cn

SHOW INDEX FROM users;
来源：http://nud.yj20258.top

[Q73] 查看表状态
来源：http://gqn.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kkw.zhoulong.xyz

[Q74] 强制使用索引
来源：http://ynd.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://okm.jqgfzy.top

[Q75] 日期格式化
来源：http://uuf.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://svn.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tkk.wangshuangyany.cn

[Q76] 按天统计
来源：http://kdx.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bmm.zhongyouzk.top

[Q77] 时间加减
来源：http://iju.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lfr.ydjk.org.cn

[Q78] 当前时间
来源：http://olg.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://equ.meibo888.top

[Q79] 字符串拼接
来源：http://juu.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nov.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://gxj.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wlf.zhixingplan.top

[Q81] 字符串替换
来源：http://hvk.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://naw.cheryme.top

[Q82] 字符长度与字节长度
来源：http://mmf.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hgl.0kj1m.cn

[Q83] 大小写转换
来源：http://fec.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ihx.tarul.cn

[Q84] 去除首尾空格
来源：http://qkd.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://xkr.nanxuanxn.top

[Q85] 数值取整
来源：http://dex.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dun.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://kgy.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fvz.xylfe.cn

[Q87] JSON 字段做条件
来源：http://kum.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xcz.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://bfa.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dae.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ysp.svipenyu.cn

[Q89] 判断表是否存在
来源：http://xpi.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fmh.hywenlv.cn

[Q90] 生成序号列
来源：http://ngt.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sgv.fehbvm.com

================================================================================
来源：http://jtd.nanxuanxn.top

R. Bash 专题
来源：http://vno.sufxvd.cn

================================================================================
来源：http://tlb.cashguo.top

[R01] shebang 与严格模式
来源：http://aar.cashguo.top

#!/usr/bin/env bash
来源：http://ujs.ivvv.top

set -euo pipefail
来源：http://dhj.vehdjk.com

[R02] 变量赋值与使用
来源：http://hpy.snrcjt.cn

name="Tom"; echo "$name"
来源：http://oij.zdbjq.cn

[R03] 只读变量
来源：http://xzf.tarul.cn

readonly PI=3.14
来源：http://qtd.hnqzz.top

[R04] 位置参数
来源：http://gpb.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grx.fengsongda.top

[R05] 参数默认值
来源：http://udi.sjlbkw.cn

name="${1:-default}"
来源：http://xdz.yfazqb.com

[R06] 判断命令是否存在
来源：http://oik.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ewp.chenlongwang.top

[R07] if 判断文件
来源：http://hkf.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://odj.yuanzhike.top

[R08] 数值比较
来源：http://wuc.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vre.jianghu66.top

[R09] 字符串比较
来源：http://rdq.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ajb.pycfn.com

[R10] 正则匹配
来源：http://ecr.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rvt.nwbrower.top

[R11] case 多分支
来源：http://qcw.zhiwuduotai.top

case "$1" in
来源：http://emv.fzhhl.top

start) echo "启动" ;;
来源：http://ekh.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://yxs.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://ews.uphjek.com

esac
来源：http://xmz.meibo888.top

[R12] for 遍历文件
来源：http://sgb.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://jix.jqgfzy.top

[R13] for 计数循环
来源：http://bxh.feifeiyinyue.top

for i in {1..10}; do echo "$i"; done
来源：http://yyv.c1oappe.top

[R14] C 风格 for
来源：http://nof.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://exz.epnwcf.com

[R15] while 逐行读文件
来源：http://cjg.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mai.jinghuilouyu.cn

[R16] until 等待条件
来源：http://yqp.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rwa.snrcjt.cn

[R17] 数组定义与取值
来源：http://xvy.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://fxu.ivvv.top

[R18] 遍历数组
来源：http://dmf.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bgh.havefunace.top

[R19] 数组长度
来源：http://uae.hnqzz.top

echo "${#arr[@]}"
来源：http://xrz.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://tal.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ccs.quarkkingdee.top

[R21] 字符串长度
来源：http://txc.daria6918.cn

echo "${#s}"
来源：http://rss.yj202588.top

[R22] 截取子串
来源：http://xyx.zhongyouzk.top

echo "${s:0:5}"
来源：http://wok.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://zkl.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nwf.tian-w.cn

[R24] 大小写转换
来源：http://cpa.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://xns.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://cln.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eel.tanke756.top

[R26] 命令替换
来源：http://hap.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://zkc.yongpay.top

[R27] 算术展开
来源：http://dnc.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://xhp.cucudq.cn

[R28] 浮点运算
来源：http://umx.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://dnl.0kj1m.cn

[R29] 定义函数
来源：http://kfn.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rso.mhx1999.top

[R30] 函数返回状态码
来源：http://des.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://kyu.jqgufenzy.top

[R31] 局部变量
来源：http://zmc.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://bnf.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://iaz.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gro.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://voq.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://klu.cucudq.cn

[R34] 退出时清理
来源：http://ibh.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://gav.cdnleiting.top

[R35] 后台执行并等待
来源：http://vjc.zhiwuduotai.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wdo.meibo888.top

[R36] 并发执行多个任务
来源：http://hso.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xaw.iojbl.cn

[R37] 把输出赋给变量
来源：http://wdc.jinqigfzy.top

files=$(ls -1)
来源：http://qpn.xinyue.icu

[R38] 管道串联
来源：http://cpl.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://csr.redwolf501.top

[R39] 重定向标准输出与错误
来源：http://wlz.cdnleiting.top

cmd > out.log 2>&1
来源：http://sok.jiagoushi.top

[R40] 追加写日志
来源：http://ljs.zdbjq.cn

echo "log" >> out.log
来源：http://eft.jinqigufen.top

[R41] 丢弃输出
来源：http://vca.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://tji.ppjwa.cn

[R42] 输入重定向
来源：http://yap.jlsjyb.cn

wc -l < a.txt
来源：http://jvu.gzhubu.top

[R43] 按名字查找文件
来源：http://srm.dianchejie.cn

find . -name "*.log" -type f
来源：http://bxn.c1oappe.top

[R44] 按修改时间查找
来源：http://kub.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://rns.smart0.xyz

[R45] 批量删除
来源：http://pwj.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://bfj.gotoacloud.top

[R46] 递归替换文件内容
来源：http://btb.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mml.nanxuanxn.top

[R47] sed 单行替换
来源：http://tdb.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zme.zdbjq.cn

[R48] awk 取指定列
来源：http://exu.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://ike.dashuyun.cn

[R49] awk 带条件
来源：http://xmh.ppjwa.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://acg.gotoacloud.top

[R50] awk 求和
来源：http://ufc.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ztc.jinqigufen.top

[R51] 排序去重取前几
来源：http://pmi.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://alo.yj20258.top

[R52] 统计行数
来源：http://gjp.yuxming.cn

wc -l a.txt
来源：http://des.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://fxz.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zwq.tarul.cn

[R54] 比较两个文件
来源：http://ste.vehdjk.com

diff a.txt b.txt
来源：http://hbw.vqdsnc.cn

[R55] 压缩与解压
来源：http://kpv.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tnx.tianlin.xyz

[R56] 远程拷贝
来源：http://edh.iojbl.cn

scp file user@host:/path/
来源：http://izx.yj20258.top

[R57] 远程执行命令
来源：http://ael.sweek.top

ssh user@host 'uptime'
来源：http://tpq.zhaomingkeji.xyz

[R58] 下载文件
来源：http://nvp.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xuc.iojbl.cn

[R59] 发 POST JSON
来源：http://ckp.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://spi.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://edg.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://egb.dashuyun.cn

[R61] 磁盘占用
来源：http://aig.havefunace.top

df -h;  du -sh *
来源：http://jev.shzxlz.cn

[R62] 找最占空间的文件
来源：http://tll.uphjek.com

du -ah . | sort -rh | head -10
来源：http://ilg.dianchejie.cn

[R63] 内存与进程
来源：http://bic.wangdashe.top


<!-- 参考信息 -->