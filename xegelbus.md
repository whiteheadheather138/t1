代发 wailian999

SELECT * FROM users;
来源：http://zze.vehdjk.com

[Q16] 查询指定列
来源：http://eli.hnqzz.top

SELECT id, name FROM users;
来源：http://wrc.xuanzx.com

[Q17] 条件查询
来源：http://sdv.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pxx.guowangkeji.top

[Q18] 模糊匹配
来源：http://icf.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hxi.ydjk.org.cn

[Q19] 范围查询
来源：http://unh.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mui.hysaishi.cn

[Q20] IN 列表
来源：http://csa.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://olf.jqgfzy.top

[Q21] 空值判断
来源：http://aml.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://cwu.yj20258.top

[Q22] 排序
来源：http://law.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pwp.meibo888.top

[Q23] 分页
来源：http://qjh.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nml.yuanzhike.top

[Q24] 去重
来源：http://lmx.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://feo.dianchejie.cn

[Q25] 只取前 N 条
来源：http://uhl.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mzw.jiagoushi.top

[Q26] 计数
来源：http://jld.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://ofb.guannengcc.top

[Q27] 条件计数
来源：http://dpl.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://igs.guannengcc.top

[Q28] 求和与平均
来源：http://mvc.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dzu.nanxinkj.top

[Q29] 最大最小值
来源：http://fmw.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bxc.gotoacloud.top

[Q30] 分组统计
来源：http://zsj.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dip.zdbjq.cn

[Q31] 分组后过滤
来源：http://lvq.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aup.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://jdp.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qig.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dgf.guannengcc.top

[Q33] 多列分组
来源：http://iyf.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hli.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://zcw.shanyushiyangkeji.top

SELECT * FROM (
来源：http://nco.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://frb.tian-w.cn

) t WHERE rn = 1;
来源：http://nqe.ehwqpu.com

[Q35] 内连接
来源：http://lwg.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ewx.sufxvd.cn

[Q36] 左连接
来源：http://xfv.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://llg.hammf.cn

[Q37] 右连接
来源：http://adh.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://awd.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://trp.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nuc.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://wca.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yvx.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rca.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vvc.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fjf.sxryk.cn

[Q41] 多表连接
来源：http://mtf.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://rty.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://leo.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://uct.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://xcb.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://lht.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgu.gotoacloud.top

[Q43] 标量子查询
来源：http://qht.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ywr.redwolf501.top

[Q44] IN 子查询
来源：http://ytg.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vfy.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://txp.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dim.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wrb.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mca.fehbvm.com

[Q47] 与平均值比较
来源：http://lbw.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rbh.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://wro.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ynd.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://lcb.yfazqb.com

[Q49] 更新单行
来源：http://bbm.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yrs.chenlongwang.top

[Q50] 批量更新
来源：http://heg.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwg.zdqjudy.top

[Q51] 用子查询更新
来源：http://rpr.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cbl.feifeiyinyue.top

[Q52] 删除指定行
来源：http://kvo.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://vpg.feifeiyinyue.top

[Q53] 按条件删除
来源：http://lcj.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://olc.zdbjq.cn

[Q54] 清空表
来源：http://quh.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://ayz.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://phn.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://obv.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://oew.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://teb.ywan-chungtsiang.top

[Q57] 行号
来源：http://myx.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dfm.feifeiyinyue.top

[Q58] 累计求和
来源：http://lqj.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ayi.feifeiyinyue.top

[Q59] 分组内累计
来源：http://aka.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://omi.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://lzd.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ryq.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jcp.tarul.cn

[Q61] 移动平均
来源：http://gog.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://trv.tanke756.top

[Q62] 分组占比
来源：http://uzv.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bnd.bbcook.cn

[Q63] 开启事务
来源：http://gsi.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://shk.fengsongda.top

[Q64] 提交事务
来源：http://gzf.hysaishi.cn

COMMIT;
来源：http://wpb.9152youxi.cn

[Q65] 回滚事务
来源：http://vnv.sxryk.cn

ROLLBACK;
来源：http://lgf.redwolf501.top

[Q66] 行锁查询
来源：http://cbd.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gcw.xuanzx.com

[Q67] 设置隔离级别
来源：http://xlg.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scz.hcnkem.com

[Q68] 保存点
来源：http://nyn.andypj.xyz

SAVEPOINT sp1;
来源：http://hpd.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://mtr.ydjk.org.cn

[Q69] 查看执行计划
来源：http://goz.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uez.ehwqpu.com

[Q70] 更新统计信息
来源：http://mlp.yueranfly.top

ANALYZE TABLE users;
来源：http://yqp.yonumen.top

[Q71] 查看建表语句
来源：http://qjp.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://the.jianghu66.top

[Q72] 查看索引
来源：http://zfy.fktsv.cn

SHOW INDEX FROM users;
来源：http://mdd.hysaishi.cn

[Q73] 查看表状态
来源：http://xkd.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://adv.sysykeji.top

[Q74] 强制使用索引
来源：http://uyo.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dxn.yj202588.top

[Q75] 日期格式化
来源：http://tim.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thg.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://utc.jinqigufen.top

[Q76] 按天统计
来源：http://bsw.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dsw.jyoumei.cn

[Q77] 时间加减
来源：http://bmy.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aba.vqdsnc.cn

[Q78] 当前时间
来源：http://one.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://day.cdnleiting.top

[Q79] 字符串拼接
来源：http://inc.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dfb.yangfankeji.com

[Q80] 字符串截取
来源：http://wmh.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fpf.dashuyun.cn

[Q81] 字符串替换
来源：http://jji.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zbh.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://qis.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ccg.ppjwa.cn

[Q83] 大小写转换
来源：http://vck.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uml.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://qjn.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://jpy.yuxming.cn

[Q85] 数值取整
来源：http://lpd.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cgz.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://cjq.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ify.meibo888.top

[Q87] JSON 字段做条件
来源：http://tuy.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jrt.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://zul.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://obl.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vvp.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://byg.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wzv.cheryme.top

[Q90] 生成序号列
来源：http://pmv.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ped.gaohongyu789.top

================================================================================
来源：http://eys.gzhubu.top

R. Bash 专题
来源：http://atz.dianchejie.cn

================================================================================
来源：http://uxc.birdmap.top

[R01] shebang 与严格模式
来源：http://htj.daxiang520.top

#!/usr/bin/env bash
来源：http://ohj.hammf.cn

set -euo pipefail
来源：http://pwp.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://wvc.hfpthk.cn

name="Tom"; echo "$name"
来源：http://rhp.cdnleiting.top

[R03] 只读变量
来源：http://vmw.shanyushiyangtech.top

readonly PI=3.14
来源：http://ohl.mhx1999.top

[R04] 位置参数
来源：http://ctp.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ogk.pycfn.com

[R05] 参数默认值
来源：http://coe.jianghu66.top

name="${1:-default}"
来源：http://qed.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://jrc.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lrc.52xcode.cn

[R07] if 判断文件
来源：http://oev.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://atl.guowangkeji.top

[R08] 数值比较
来源：http://lhv.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ljp.vqdsnc.cn

[R09] 字符串比较
来源：http://gqg.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udx.zhoulong.xyz

[R10] 正则匹配
来源：http://xop.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hzy.guannengcc.top

[R11] case 多分支
来源：http://lkn.zdbjq.cn

case "$1" in
来源：http://hwd.yanxiufei.cn

start) echo "启动" ;;
来源：http://tuh.ppjwa.cn

stop)  echo "停止" ;;
来源：http://bjz.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://tvc.yvedp.cn

esac
来源：http://uuf.feifeiyinyue.top

[R12] for 遍历文件
来源：http://nqm.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://kts.zhiwuduotai.top

[R13] for 计数循环
来源：http://zvy.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://flt.yj20258.top

[R14] C 风格 for
来源：http://myv.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pjd.uphjek.com

[R15] while 逐行读文件
来源：http://gdc.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vba.yanxiufei.cn

[R16] until 等待条件
来源：http://jwe.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ntx.yongpay.top

[R17] 数组定义与取值
来源：http://jbg.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://rvn.xylfe.cn

[R18] 遍历数组
来源：http://kjj.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ewo.xuetiantiany.cn

[R19] 数组长度
来源：http://fnw.quarkkingdee.top

echo "${#arr[@]}"
来源：http://rbv.mhx1999.top

[R20] 关联数组（字典）
来源：http://hco.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gxt.sweek.top

[R21] 字符串长度
来源：http://pqr.ivvv.top

echo "${#s}"
来源：http://coj.fktsv.cn

[R22] 截取子串
来源：http://ibx.hfpthk.cn

echo "${s:0:5}"
来源：http://uvx.52xcode.cn

[R23] 字符串替换
来源：http://zol.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ojg.guannengcc.top

[R24] 大小写转换
来源：http://vrj.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://mfz.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://rgq.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yai.yanxiufei.cn

[R26] 命令替换
来源：http://jvo.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://fbj.cashguo.top

[R27] 算术展开
来源：http://tpo.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://pos.feifeiyinyue.top

[R28] 浮点运算
来源：http://ylb.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://zvw.chenjidiqi.icu

[R29] 定义函数
来源：http://vbn.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xon.52xcode.cn

[R30] 函数返回状态码
来源：http://lwe.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://aln.ywan-chungtsiang.top

[R31] 局部变量
来源：http://uqp.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://wxc.c1oappe.top

[R32] 参数个数校验
来源：http://xqs.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uuz.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://jhi.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjo.cheryme.top

[R34] 退出时清理
来源：http://iak.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aiu.gzhubu.top

[R35] 后台执行并等待
来源：http://jpk.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qzc.shanyushiyangkeji.top

[R36] 并发执行多个任务
来源：http://vhd.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psx.cqqwz.cn

[R37] 把输出赋给变量
来源：http://tdq.shanyushiyangkeji.top

files=$(ls -1)
来源：http://hwy.guannengcc.top

[R38] 管道串联
来源：http://tsl.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://mbu.meibo888.top

[R39] 重定向标准输出与错误
来源：http://ybt.hesvh.cn

cmd > out.log 2>&1
来源：http://cjb.hongshengwenyu.top

[R40] 追加写日志
来源：http://pzq.mhx1999.top

echo "log" >> out.log
来源：http://guw.yueranfly.top

[R41] 丢弃输出
来源：http://bmt.yfazqb.com

cmd >/dev/null 2>&1
来源：http://szu.sxryk.cn

[R42] 输入重定向
来源：http://zpa.feifeiyinyue.top

wc -l < a.txt
来源：http://hlz.hesvh.cn

[R43] 按名字查找文件
来源：http://nrb.sufxvd.cn

find . -name "*.log" -type f
来源：http://xfr.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://nge.daria6918.cn

find . -mtime -7 -type f
来源：http://swm.jiagoushi.top

[R45] 批量删除
来源：http://lzc.gzhubu.top

find . -name "*.tmp" -delete
来源：http://ldx.cdnleiting.top

[R46] 递归替换文件内容
来源：http://nbu.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wpz.xuetiantiany.cn

[R47] sed 单行替换
来源：http://why.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://vhm.wangshuangyany.cn

[R48] awk 取指定列
来源：http://jrt.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://xdn.dashuyun.cn

[R49] awk 带条件
来源：http://zdm.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sdp.fehbvm.com

[R50] awk 求和
来源：http://yrm.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lcz.cqqwz.cn

[R51] 排序去重取前几
来源：http://kfw.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ddx.zdqjudy.top

[R52] 统计行数
来源：http://wca.ybcxt.top

wc -l a.txt
来源：http://nnf.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://azx.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sck.daria6918.cn

[R54] 比较两个文件
来源：http://uaq.nanxuanxn.top

diff a.txt b.txt
来源：http://noj.gaohongyu789.top

[R55] 压缩与解压
来源：http://prh.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ppz.gotoacloud.top

[R56] 远程拷贝
来源：http://ubt.mhx1999.top

scp file user@host:/path/
来源：http://igb.zycfv.cn

[R57] 远程执行命令
来源：http://fvg.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://lal.hysaishi.cn

[R58] 下载文件
来源：http://yvd.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cls.haohaochexian.top

[R59] 发 POST JSON
来源：http://phf.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zjs.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://pog.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vsj.yuanzhike.top

[R61] 磁盘占用
来源：http://fkh.sweek.top

df -h;  du -sh *
来源：http://bzz.hnqzz.top

[R62] 找最占空间的文件
来源：http://yyj.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://weo.cdnleiting.top

[R63] 内存与进程
来源：http://sut.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://rkt.zhongyouzk.top

[R64] 结束进程
来源：http://bnk.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://lxh.fengsongda.top

[R65] 查看端口占用
来源：http://ebn.epnwcf.com


<!-- 参考信息 -->