代发 wailian999

SELECT * FROM users;
来源：http://ipq.cucudq.cn

[Q16] 查询指定列
来源：http://uoi.kuanghao11.cn

SELECT id, name FROM users;
来源：http://zfa.haohaochexian.top

[Q17] 条件查询
来源：http://oxx.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rji.jqgfzy.top

[Q18] 模糊匹配
来源：http://wcm.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lby.daxiang520.top

[Q19] 范围查询
来源：http://kdn.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ugi.hongshengwenyu.top

[Q20] IN 列表
来源：http://faq.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yjv.fanxiaobao.xyz

[Q21] 空值判断
来源：http://mkj.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vlc.nanxinkj.top

[Q22] 排序
来源：http://cxn.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hgi.wangshuangyany.cn

[Q23] 分页
来源：http://cer.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tru.dianchejie.cn

[Q24] 去重
来源：http://jqh.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://cnl.ppjwa.cn

[Q25] 只取前 N 条
来源：http://itg.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rqg.chenlongwang.top

[Q26] 计数
来源：http://bto.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://jtf.cqqwz.cn

[Q27] 条件计数
来源：http://szb.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://loe.yj20258888.top

[Q28] 求和与平均
来源：http://zyl.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xwn.vqdsnc.cn

[Q29] 最大最小值
来源：http://pnd.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kux.jqgfzy.top

[Q30] 分组统计
来源：http://hbg.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eej.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://rfr.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pdn.xziqi.cn

[Q32] 分组拼接字符串
来源：http://pql.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jcw.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xnk.gaohongyu789.top

[Q33] 多列分组
来源：http://psr.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oxl.yonumen.top

[Q34] 每组取第一条
来源：http://lcj.yonumen.top

SELECT * FROM (
来源：http://lff.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kkc.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://kse.shzxlz.cn

[Q35] 内连接
来源：http://yvx.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xcw.chenzaomai.com

[Q36] 左连接
来源：http://fpa.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://veu.jinghuilouyu.cn

[Q37] 右连接
来源：http://chc.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://doi.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qbg.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pjk.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://blx.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://nyt.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rgd.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gxq.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cex.haohaochexian.top

[Q41] 多表连接
来源：http://zrq.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nii.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://mbp.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://nct.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://lrb.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://ivh.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ttf.andypj.xyz

[Q43] 标量子查询
来源：http://pxj.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://drm.vehdjk.com

[Q44] IN 子查询
来源：http://fss.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ara.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://arp.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://clr.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://vwq.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnh.havefunace.top

[Q47] 与平均值比较
来源：http://ker.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qyv.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://klc.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qwq.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://lnl.sjlbkw.cn

[Q49] 更新单行
来源：http://cjt.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bvv.gzhubu.top

[Q50] 批量更新
来源：http://ktr.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rfh.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://oqh.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fgk.yj20258.top

[Q52] 删除指定行
来源：http://dif.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://fqi.ctjpmb.com

[Q53] 按条件删除
来源：http://wpj.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fkq.nanxinkj.top

[Q54] 清空表
来源：http://nzq.havefunace.top

TRUNCATE TABLE logs;
来源：http://gvo.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://grc.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wei.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://ccu.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aii.jlsjyb.cn

[Q57] 行号
来源：http://gnz.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jpi.zhengqikj.top

[Q58] 累计求和
来源：http://eee.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gpw.hnqzz.top

[Q59] 分组内累计
来源：http://rpk.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mnx.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://tsa.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qvd.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cxu.iojbl.cn

[Q61] 移动平均
来源：http://tqa.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vmx.ydjk.org.cn

[Q62] 分组占比
来源：http://ioi.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://avr.gotoacloud.top

[Q63] 开启事务
来源：http://lve.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://exr.daxiang520.top

[Q64] 提交事务
来源：http://zri.yangfankeji.com

COMMIT;
来源：http://hzs.hongshengwenyu.top

[Q65] 回滚事务
来源：http://ffz.hnqzz.top

ROLLBACK;
来源：http://nur.yongpay.top

[Q66] 行锁查询
来源：http://thd.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ksw.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://lzy.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szn.daria6918.cn

[Q68] 保存点
来源：http://whd.xinyue.icu

SAVEPOINT sp1;
来源：http://fvj.jqgfzy.top

ROLLBACK TO sp1;
来源：http://edf.daria6918.cn

[Q69] 查看执行计划
来源：http://sns.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pux.yueranfly.top

[Q70] 更新统计信息
来源：http://iof.cdnleiting.top

ANALYZE TABLE users;
来源：http://azo.316326.xyz

[Q71] 查看建表语句
来源：http://vsz.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vlu.ivvv.top

[Q72] 查看索引
来源：http://voa.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://xkb.wangshuangyany.cn

[Q73] 查看表状态
来源：http://gcm.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://bcp.ydzc1.top

[Q74] 强制使用索引
来源：http://ipk.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qvs.zhongyouzk.top

[Q75] 日期格式化
来源：http://thq.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wte.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tiy.cqqwz.cn

[Q76] 按天统计
来源：http://mcn.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://psx.gogol.net.cn

[Q77] 时间加减
来源：http://zmo.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tsm.gotoacloud.top

[Q78] 当前时间
来源：http://eat.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://asg.aizwys.cn

[Q79] 字符串拼接
来源：http://jaa.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mpy.nanxuanxn.top

[Q80] 字符串截取
来源：http://nbr.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yvn.epnwcf.com

[Q81] 字符串替换
来源：http://bup.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pzm.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://xmk.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wyl.zdbjq.cn

[Q83] 大小写转换
来源：http://nzx.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jqx.tian-w.cn

[Q84] 去除首尾空格
来源：http://ipo.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://cee.xziqi.cn

[Q85] 数值取整
来源：http://tma.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://loj.pycfn.com

[Q86] 读取 JSON 字段
来源：http://onj.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mhr.cashguo.top

[Q87] JSON 字段做条件
来源：http://gwr.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lap.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://bjt.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wnd.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cwt.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://hfq.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://duv.birdmap.top

[Q90] 生成序号列
来源：http://zhu.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wws.vehdjk.com

================================================================================
来源：http://dab.zhiwuduotai.top

R. Bash 专题
来源：http://eso.sweek.top

================================================================================
来源：http://kon.9152youxi.cn

[R01] shebang 与严格模式
来源：http://jxh.jqgfzy.top

#!/usr/bin/env bash
来源：http://xci.ctjpmb.com

set -euo pipefail
来源：http://qit.tian-w.cn

[R02] 变量赋值与使用
来源：http://wth.hcnkem.com

name="Tom"; echo "$name"
来源：http://box.vehdjk.com

[R03] 只读变量
来源：http://ert.jlsjyb.cn

readonly PI=3.14
来源：http://kvk.yonumen.top

[R04] 位置参数
来源：http://qbs.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tbz.nanxuanxn.top

[R05] 参数默认值
来源：http://rdm.sweek.top

name="${1:-default}"
来源：http://pwy.bbcook.cn

[R06] 判断命令是否存在
来源：http://msc.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://noe.nwbrower.top

[R07] if 判断文件
来源：http://wpz.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ayd.cdnleiting.top

[R08] 数值比较
来源：http://jfu.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mwr.yongpay.top

[R09] 字符串比较
来源：http://lgz.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gni.yj20258.top

[R10] 正则匹配
来源：http://zxz.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hed.nanxuanxn.top

[R11] case 多分支
来源：http://wlb.daxiang520.top

case "$1" in
来源：http://pyf.wangshuangyany.cn

start) echo "启动" ;;
来源：http://xcv.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://hnx.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://edq.hnxiangtu.top

esac
来源：http://wbv.zhengqikj.top

[R12] for 遍历文件
来源：http://ogo.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://bqb.bbcook.cn

[R13] for 计数循环
来源：http://fcm.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://snf.smart0.xyz

[R14] C 风格 for
来源：http://dup.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pyf.316326.xyz

[R15] while 逐行读文件
来源：http://gme.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tyw.zhixingplan.top

[R16] until 等待条件
来源：http://nox.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ctt.nwbrower.top

[R17] 数组定义与取值
来源：http://rau.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hdq.yangfankeji.com

[R18] 遍历数组
来源：http://bue.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zmn.cucudq.cn

[R19] 数组长度
来源：http://nsj.andypj.xyz

echo "${#arr[@]}"
来源：http://uuz.smart0.xyz

[R20] 关联数组（字典）
来源：http://xvk.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zsw.cqqwz.cn

[R21] 字符串长度
来源：http://rlx.kuanghao11.cn

echo "${#s}"
来源：http://ops.birdmap.top

[R22] 截取子串
来源：http://bli.snrcjt.cn

echo "${s:0:5}"
来源：http://zsr.ydzc1.top

[R23] 字符串替换
来源：http://yhi.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kak.yfazqb.com

[R24] 大小写转换
来源：http://cir.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://cqa.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://sun.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://fit.hysaishi.cn

[R26] 命令替换
来源：http://kao.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://xfb.snrcjt.cn

[R27] 算术展开
来源：http://two.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://div.bbcook.cn

[R28] 浮点运算
来源：http://tvt.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://gqo.gaohongyu789.top

[R29] 定义函数
来源：http://pkp.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gxi.9152youxi.cn

[R30] 函数返回状态码
来源：http://rte.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://rzl.xuetiantiany.cn

[R31] 局部变量
来源：http://xaa.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://fte.zhiwuduotai.top

[R32] 参数个数校验
来源：http://gac.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mhk.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://gix.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://phv.zhixingplan.top

[R34] 退出时清理
来源：http://rsl.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vci.fehbvm.com

[R35] 后台执行并等待
来源：http://fjt.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hsx.fehbvm.com

[R36] 并发执行多个任务
来源：http://anb.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pam.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://rwe.wangdashe.top

files=$(ls -1)
来源：http://lql.cucudq.cn

[R38] 管道串联
来源：http://ecp.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://vwm.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://aoy.tian-w.cn

cmd > out.log 2>&1
来源：http://jbm.52xcode.cn

[R40] 追加写日志
来源：http://aay.nwbrower.top

echo "log" >> out.log
来源：http://jct.yueranfly.top

[R41] 丢弃输出
来源：http://ogi.jianghu66.top

cmd >/dev/null 2>&1
来源：http://fsu.zdbjq.cn

[R42] 输入重定向
来源：http://vuq.hcnkem.com

wc -l < a.txt
来源：http://prj.hysaishi.cn

[R43] 按名字查找文件
来源：http://cfc.epnwcf.com

find . -name "*.log" -type f
来源：http://obi.bjfxy.top

[R44] 按修改时间查找
来源：http://dor.jyoumei.cn

find . -mtime -7 -type f
来源：http://ckp.ydzc1.top

[R45] 批量删除
来源：http://ftz.ybcxt.top

find . -name "*.tmp" -delete
来源：http://fxz.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://xhh.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pms.meibo888.top

[R47] sed 单行替换
来源：http://tbu.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vbs.hesvh.cn

[R48] awk 取指定列
来源：http://moi.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://ldx.52xcode.cn

[R49] awk 带条件
来源：http://uup.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hxf.xinyue.icu

[R50] awk 求和
来源：http://gbm.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ydj.ybcxt.top

[R51] 排序去重取前几
来源：http://tui.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bcx.pycfn.com

[R52] 统计行数
来源：http://tsd.xziqi.cn

wc -l a.txt
来源：http://mcw.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://yng.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ala.hcnkem.com

[R54] 比较两个文件
来源：http://qqr.gogol.net.cn

diff a.txt b.txt
来源：http://juo.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://bzw.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nmy.jqgfzy.top

[R56] 远程拷贝
来源：http://nxd.yfazqb.com

scp file user@host:/path/
来源：http://obp.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://lnr.hcnkem.com

ssh user@host 'uptime'
来源：http://utv.jianghu66.top

[R58] 下载文件
来源：http://dab.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ixw.yongpay.top

[R59] 发 POST JSON
来源：http://eey.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wpp.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://ppd.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://erl.zycfv.cn

[R61] 磁盘占用
来源：http://cmk.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://eny.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://esk.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://lus.vqdsnc.cn

[R63] 内存与进程
来源：http://kwh.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://ozd.xziqi.cn

[R64] 结束进程
来源：http://erb.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://ehp.zhongyouzk.top

[R65] 查看端口占用
来源：http://cpb.nanxinkj.top


<!-- 参考信息 -->