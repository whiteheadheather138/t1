代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://mqe.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpx.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dgg.aizwys.cn

[Q15] 查询全部
来源：http://ibp.jlsjyb.cn

SELECT * FROM users;
来源：http://pky.ctjpmb.com

[Q16] 查询指定列
来源：http://zqj.chenlongwang.top

SELECT id, name FROM users;
来源：http://azt.mhx1999.top

[Q17] 条件查询
来源：http://oza.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mis.hfpthk.cn

[Q18] 模糊匹配
来源：http://zcc.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://phz.bjfxy.top

[Q19] 范围查询
来源：http://ycj.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jlw.zycfv.cn

[Q20] IN 列表
来源：http://lvr.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kje.epnwcf.com

[Q21] 空值判断
来源：http://ctc.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lnm.daxiang520.top

[Q22] 排序
来源：http://xpd.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hly.zdbjq.cn

[Q23] 分页
来源：http://php.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jsr.ywan-chungtsiang.top

[Q24] 去重
来源：http://znc.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://rsk.ehwqpu.com

[Q25] 只取前 N 条
来源：http://mmh.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://srr.yuanzhike.top

[Q26] 计数
来源：http://orl.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://qqo.cqqwz.cn

[Q27] 条件计数
来源：http://uhb.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rlq.jiagoushi.top

[Q28] 求和与平均
来源：http://wem.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yrf.9152youxi.cn

[Q29] 最大最小值
来源：http://mcn.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sbl.shuidangran.top

[Q30] 分组统计
来源：http://jlu.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yaw.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://vli.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oeo.nwbrower.top

[Q32] 分组拼接字符串
来源：http://mvd.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wbu.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cje.chenlongwang.top

[Q33] 多列分组
来源：http://uon.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gtu.chenzaomai.com

[Q34] 每组取第一条
来源：http://buu.yongpay.top

SELECT * FROM (
来源：http://zbe.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dix.zycfv.cn

) t WHERE rn = 1;
来源：http://qwr.ctjpmb.com

[Q35] 内连接
来源：http://mvl.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fdi.ydzc1.top

[Q36] 左连接
来源：http://grl.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gno.shanyushiyangtech.top

[Q37] 右连接
来源：http://uic.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gkb.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://oze.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uac.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://ydb.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zmx.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yrw.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wqz.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://btb.gzhubu.top

[Q41] 多表连接
来源：http://lvo.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lpa.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://dvx.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://car.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://nsm.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://kgu.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nny.sysykeji.top

[Q43] 标量子查询
来源：http://kwm.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vaq.hnxiangtu.top

[Q44] IN 子查询
来源：http://syy.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nwv.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://aii.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hxk.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://aln.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rda.hcnkem.com

[Q47] 与平均值比较
来源：http://dci.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://die.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://xyn.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ybp.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://cbw.tarul.cn

[Q49] 更新单行
来源：http://scg.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://etj.yueranfly.top

[Q50] 批量更新
来源：http://tro.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ats.birdmap.top

[Q51] 用子查询更新
来源：http://dvc.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xvx.guowangkeji.top

[Q52] 删除指定行
来源：http://mca.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://ncb.shuidangran.top

[Q53] 按条件删除
来源：http://scr.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://drw.aizwys.cn

[Q54] 清空表
来源：http://wwv.fengsongda.top

TRUNCATE TABLE logs;
来源：http://cxi.xziqi.cn

[Q55] 排名（并列占位）
来源：http://lya.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vsi.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://tdo.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zgq.gaohongyu789.top

[Q57] 行号
来源：http://hbq.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgo.zhengqikj.top

[Q58] 累计求和
来源：http://nrm.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rdc.fengsongda.top

[Q59] 分组内累计
来源：http://bln.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xhr.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://pxk.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ric.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://asx.c1oappe.top

[Q61] 移动平均
来源：http://jvd.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://alo.haohaochexian.top

[Q62] 分组占比
来源：http://gvc.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dfl.daria6918.cn

[Q63] 开启事务
来源：http://qrj.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://sno.fehbvm.com

[Q64] 提交事务
来源：http://gpi.jianghu66.top

COMMIT;
来源：http://rse.shuidangran.top

[Q65] 回滚事务
来源：http://gto.yonumen.top

ROLLBACK;
来源：http://lxd.gaohongyu789.top

[Q66] 行锁查询
来源：http://vwt.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lsg.nanxinkj.top

[Q67] 设置隔离级别
来源：http://ihn.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xxl.shuidangran.top

[Q68] 保存点
来源：http://bkd.yuanzhike.top

SAVEPOINT sp1;
来源：http://iha.ehwqpu.com

ROLLBACK TO sp1;
来源：http://gaq.sjlbkw.cn

[Q69] 查看执行计划
来源：http://txi.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kpj.vqdsnc.cn

[Q70] 更新统计信息
来源：http://yhm.yangfankeji.com

ANALYZE TABLE users;
来源：http://ofa.yongpay.top

[Q71] 查看建表语句
来源：http://rtt.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ygd.hysaishi.cn

[Q72] 查看索引
来源：http://gxk.gogol.net.cn

SHOW INDEX FROM users;
来源：http://yje.hywenlv.cn

[Q73] 查看表状态
来源：http://dwo.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hdq.yvedp.cn

[Q74] 强制使用索引
来源：http://tnh.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://myp.shzxlz.cn

[Q75] 日期格式化
来源：http://vck.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://svi.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://otk.zhongyouzk.top

[Q76] 按天统计
来源：http://mkt.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ctq.pycfn.com

[Q77] 时间加减
来源：http://ygh.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ges.ctjpmb.com

[Q78] 当前时间
来源：http://lov.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://igh.quarkkingdee.top

[Q79] 字符串拼接
来源：http://zoe.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://esc.shangyingyoupin.top

[Q80] 字符串截取
来源：http://xkw.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gry.ivvv.top

[Q81] 字符串替换
来源：http://ycg.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sxg.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://qhb.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zup.yj20258.top

[Q83] 大小写转换
来源：http://bjl.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yqw.ppjwa.cn

[Q84] 去除首尾空格
来源：http://vfm.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://ccn.xziqi.cn

[Q85] 数值取整
来源：http://rsg.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fnt.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://khr.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iho.hammf.cn

[Q87] JSON 字段做条件
来源：http://uts.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wva.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://saw.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://chc.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://opw.aizwys.cn

[Q89] 判断表是否存在
来源：http://vah.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zuz.shzxlz.cn

[Q90] 生成序号列
来源：http://pfp.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hin.dianchejie.cn

================================================================================
来源：http://zui.yj20258888.top

R. Bash 专题
来源：http://fzd.yueranfly.top

================================================================================
来源：http://nba.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://fyj.svipenyu.cn

#!/usr/bin/env bash
来源：http://cyh.yuxming.cn

set -euo pipefail
来源：http://phs.c1oappe.top

[R02] 变量赋值与使用
来源：http://hrz.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://nuc.kuanghao11.cn

[R03] 只读变量
来源：http://uxv.yj20258888.top

readonly PI=3.14
来源：http://idl.yfazqb.com

[R04] 位置参数
来源：http://cuw.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rjk.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://ubv.wangdashe.top

name="${1:-default}"
来源：http://qoy.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://fhu.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://svq.andypj.xyz

[R07] if 判断文件
来源：http://xjr.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fxl.ehwqpu.com

[R08] 数值比较
来源：http://dtc.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nal.yfazqb.com

[R09] 字符串比较
来源：http://ppl.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vqr.cucudq.cn

[R10] 正则匹配
来源：http://zlr.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zwt.hesvh.cn

[R11] case 多分支
来源：http://khn.jinghuilouyu.cn

case "$1" in
来源：http://nel.gotoacloud.top

start) echo "启动" ;;
来源：http://oai.fehbvm.com

stop)  echo "停止" ;;
来源：http://sub.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://vmt.nanxinkj.top

esac
来源：http://mpr.zhongyouzk.top

[R12] for 遍历文件
来源：http://gvj.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://qcb.sxryk.cn

[R13] for 计数循环
来源：http://oay.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://kgg.yuxming.cn

[R14] C 风格 for
来源：http://yft.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kkn.yueranfly.top

[R15] while 逐行读文件
来源：http://uum.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mxy.jqgfzy.top

[R16] until 等待条件
来源：http://vzy.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mlt.meibo888.top

[R17] 数组定义与取值
来源：http://ode.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://oyi.sxryk.cn

[R18] 遍历数组
来源：http://fui.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ass.hcnkem.com

[R19] 数组长度
来源：http://cst.9152youxi.cn

echo "${#arr[@]}"
来源：http://nny.zhixingplan.top

[R20] 关联数组（字典）
来源：http://las.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fzz.xuetiantiany.cn

[R21] 字符串长度
来源：http://gau.yuanzhike.top

echo "${#s}"
来源：http://arl.fktsv.cn

[R22] 截取子串
来源：http://peq.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://mal.svipenyu.cn

[R23] 字符串替换
来源：http://kic.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kkb.cucudq.cn

[R24] 大小写转换
来源：http://fwl.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqb.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://eaw.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hwh.yvedp.cn

[R26] 命令替换
来源：http://ctt.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://qzw.yuxming.cn

[R27] 算术展开
来源：http://bag.c1oappe.top

echo $((1 + 2 * 3))
来源：http://hnw.xylfe.cn

[R28] 浮点运算
来源：http://ecp.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://iyt.hesvh.cn

[R29] 定义函数
来源：http://gtm.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lsc.cashguo.top

[R30] 函数返回状态码
来源：http://mtv.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://vbk.xuetiantiany.cn

[R31] 局部变量
来源：http://btx.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://fpw.yj202588.top

[R32] 参数个数校验
来源：http://khe.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sgv.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://edg.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cxl.chenlongwang.top

[R34] 退出时清理
来源：http://tnc.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://bap.hysaishi.cn

[R35] 后台执行并等待
来源：http://bio.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ffi.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://gtd.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fim.zdbjq.cn

[R37] 把输出赋给变量
来源：http://uqw.aibaodan.cn

files=$(ls -1)
来源：http://fdd.hnqzz.top

[R38] 管道串联
来源：http://gvt.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://qtv.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://yth.kuanghao11.cn

cmd > out.log 2>&1
来源：http://ocl.xylfe.cn

[R40] 追加写日志
来源：http://hxw.pengpengdd.cyou

echo "log" >> out.log
来源：http://jrc.vehdjk.com

[R41] 丢弃输出
来源：http://fzi.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://xla.svipenyu.cn

[R42] 输入重定向
来源：http://fmp.zhixingplan.top

wc -l < a.txt
来源：http://qva.daria6918.cn

[R43] 按名字查找文件
来源：http://rrd.andypj.xyz

find . -name "*.log" -type f
来源：http://bpq.sjlbkw.cn

[R44] 按修改时间查找
来源：http://pzv.meibo888.top

find . -mtime -7 -type f
来源：http://vgm.ybcxt.top

[R45] 批量删除
来源：http://krx.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://znr.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://rfx.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://och.yuanzhike.top

[R47] sed 单行替换
来源：http://bbd.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://cma.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://mla.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://idy.jinghuilouyu.cn

[R49] awk 带条件
来源：http://dfa.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uod.feifeiyinyue.top

[R50] awk 求和
来源：http://hxv.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ejf.fzhhl.top

[R51] 排序去重取前几
来源：http://dhl.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yxa.yj202588.top

[R52] 统计行数
来源：http://vlt.sxryk.cn

wc -l a.txt
来源：http://kpr.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://jtm.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cor.jqgufenzy.top

[R54] 比较两个文件
来源：http://vbv.yonumen.top

diff a.txt b.txt
来源：http://stz.zycfv.cn

[R55] 压缩与解压
来源：http://bjv.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qts.quarkkingdee.top

[R56] 远程拷贝
来源：http://eqf.jlsjyb.cn

scp file user@host:/path/
来源：http://ome.yonumen.top

[R57] 远程执行命令
来源：http://uii.yuanzhike.top

ssh user@host 'uptime'
来源：http://cvs.jinqigufen.top

[R58] 下载文件
来源：http://xnm.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://npr.gotoacloud.top

[R59] 发 POST JSON
来源：http://egp.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xoo.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://yiw.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vzf.yongpay.top

[R61] 磁盘占用
来源：http://zkk.nanxinkj.top

df -h;  du -sh *
来源：http://pbn.gzhubu.top

[R62] 找最占空间的文件
来源：http://leo.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://grb.ehwqpu.com

[R63] 内存与进程
来源：http://kuj.epnwcf.com


<!-- 参考信息 -->