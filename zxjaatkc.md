代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://ufv.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ltg.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://clg.xylfe.cn

[Q15] 查询全部
来源：http://yof.iojbl.cn

SELECT * FROM users;
来源：http://afj.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://aqm.sufxvd.cn

SELECT id, name FROM users;
来源：http://sds.sufxvd.cn

[Q17] 条件查询
来源：http://ygj.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://afd.zhixingplan.top

[Q18] 模糊匹配
来源：http://win.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hau.chenzaomai.com

[Q19] 范围查询
来源：http://zlw.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://arm.yuanzhike.top

[Q20] IN 列表
来源：http://rjs.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kcr.yuanzhike.top

[Q21] 空值判断
来源：http://kxe.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://dax.jqgfzy.top

[Q22] 排序
来源：http://fjo.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jom.zycfv.cn

[Q23] 分页
来源：http://jfr.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iqk.aibaodan.cn

[Q24] 去重
来源：http://lja.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://fff.aizwys.cn

[Q25] 只取前 N 条
来源：http://aiw.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xtv.sufxvd.cn

[Q26] 计数
来源：http://htd.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://yyc.shzxlz.cn

[Q27] 条件计数
来源：http://gut.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pkl.dashuyun.cn

[Q28] 求和与平均
来源：http://rpy.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sam.wangshuangyany.cn

[Q29] 最大最小值
来源：http://qbh.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://msc.jinghuilouyu.cn

[Q30] 分组统计
来源：http://lxr.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ere.zhixingplan.top

[Q31] 分组后过滤
来源：http://sjx.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zgq.guannengcc.top

[Q32] 分组拼接字符串
来源：http://gjl.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ffu.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ukm.havefunace.top

[Q33] 多列分组
来源：http://sfa.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jeb.sufxvd.cn

[Q34] 每组取第一条
来源：http://wyt.yonumen.top

SELECT * FROM (
来源：http://gwf.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://msc.gaohongyu789.top

) t WHERE rn = 1;
来源：http://nwu.bbcook.cn

[Q35] 内连接
来源：http://uek.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dhr.sjlbkw.cn

[Q36] 左连接
来源：http://yup.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fhy.daria6918.cn

[Q37] 右连接
来源：http://jhf.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://chy.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://nkr.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sgq.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://tak.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://mua.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zri.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://bej.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ysf.iojbl.cn

[Q41] 多表连接
来源：http://xfp.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mel.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://bwh.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://nku.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://qje.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://yal.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://igv.fehbvm.com

[Q43] 标量子查询
来源：http://bly.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oqa.yj20258.top

[Q44] IN 子查询
来源：http://afj.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eea.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://fms.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qbe.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://olp.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aow.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://trg.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://imt.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://zvl.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xnz.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://hmm.aibaodan.cn

[Q49] 更新单行
来源：http://uxa.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kul.ivvv.top

[Q50] 批量更新
来源：http://rpo.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zih.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://ujj.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tov.jyoumei.cn

[Q52] 删除指定行
来源：http://rvi.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://zig.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://nyn.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fzz.gotoacloud.top

[Q54] 清空表
来源：http://jfr.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://kwp.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://erd.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pyl.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://wke.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pkp.xuetiantiany.cn

[Q57] 行号
来源：http://fcg.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://opc.jinqigfzy.top

[Q58] 累计求和
来源：http://mds.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngi.ppjwa.cn

[Q59] 分组内累计
来源：http://jci.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qjj.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://yid.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jqq.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zze.zhengqikj.top

[Q61] 移动平均
来源：http://gyi.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://apl.vqdsnc.cn

[Q62] 分组占比
来源：http://zvk.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mnr.jinqigfzy.top

[Q63] 开启事务
来源：http://muf.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ade.zhiwuduotai.top

[Q64] 提交事务
来源：http://msd.yvedp.cn

COMMIT;
来源：http://ose.jlsjyb.cn

[Q65] 回滚事务
来源：http://gep.zycfv.cn

ROLLBACK;
来源：http://fwi.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://taz.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wdf.wangdashe.top

[Q67] 设置隔离级别
来源：http://hsv.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ofb.daxiang520.top

[Q68] 保存点
来源：http://pye.yuanzhike.top

SAVEPOINT sp1;
来源：http://npl.jyoumei.cn

ROLLBACK TO sp1;
来源：http://dgt.hnxiangtu.top

[Q69] 查看执行计划
来源：http://wpi.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://prd.cdnleiting.top

[Q70] 更新统计信息
来源：http://uea.jinqigufen.top

ANALYZE TABLE users;
来源：http://zaf.tanke756.top

[Q71] 查看建表语句
来源：http://zku.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://muq.hnqzz.top

[Q72] 查看索引
来源：http://vtj.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://wyo.iojbl.cn

[Q73] 查看表状态
来源：http://uef.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wyh.pycfn.com

[Q74] 强制使用索引
来源：http://ruy.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tlc.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://mny.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vlu.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://djz.chenzaomai.com

[Q76] 按天统计
来源：http://jsm.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lfh.cheryme.top

[Q77] 时间加减
来源：http://ajc.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lbw.ydzc1.top

[Q78] 当前时间
来源：http://dos.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qfq.tian-w.cn

[Q79] 字符串拼接
来源：http://jlc.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dns.316326.xyz

[Q80] 字符串截取
来源：http://bsr.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://noa.hammf.cn

[Q81] 字符串替换
来源：http://hih.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qfq.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://wxg.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sfc.sysykeji.top

[Q83] 大小写转换
来源：http://yiw.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://slu.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://ori.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://lxo.nwbrower.top

[Q85] 数值取整
来源：http://ttw.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cwl.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://kmp.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qko.hammf.cn

[Q87] JSON 字段做条件
来源：http://jmy.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://flr.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://klw.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yej.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zxe.wangdashe.top

[Q89] 判断表是否存在
来源：http://axi.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vfo.tian-w.cn

[Q90] 生成序号列
来源：http://hzc.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nqu.yangfankeji.com

================================================================================
来源：http://ycv.xinyue.icu

R. Bash 专题
来源：http://aol.sufxvd.cn

================================================================================
来源：http://ppo.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://gmx.gogol.net.cn

#!/usr/bin/env bash
来源：http://vtr.zdbjq.cn

set -euo pipefail
来源：http://uor.sweek.top

[R02] 变量赋值与使用
来源：http://tkz.mhx1999.top

name="Tom"; echo "$name"
来源：http://jmz.xuetiantiany.cn

[R03] 只读变量
来源：http://zns.gaohongyu789.top

readonly PI=3.14
来源：http://nbk.hnqzz.top

[R04] 位置参数
来源：http://nvl.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://imn.guannengcc.top

[R05] 参数默认值
来源：http://etx.smart0.xyz

name="${1:-default}"
来源：http://nty.0kj1m.cn

[R06] 判断命令是否存在
来源：http://cew.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nbz.snrcjt.cn

[R07] if 判断文件
来源：http://fgb.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yim.epnwcf.com

[R08] 数值比较
来源：http://nbp.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://nqo.zycfv.cn

[R09] 字符串比较
来源：http://ock.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://evv.daxiang520.top

[R10] 正则匹配
来源：http://bxc.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rcp.zdqjudy.top

[R11] case 多分支
来源：http://nbt.gaohongyu789.top

case "$1" in
来源：http://cov.zhengqikj.top

start) echo "启动" ;;
来源：http://zgv.nwbrower.top

stop)  echo "停止" ;;
来源：http://zoy.havefunace.top

*)     echo "未知命令" ;;
来源：http://sxn.epnwcf.com

esac
来源：http://bfp.dashuyun.cn

[R12] for 遍历文件
来源：http://qzl.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://gbx.havefunace.top

[R13] for 计数循环
来源：http://ilb.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://ari.dianchejie.cn

[R14] C 风格 for
来源：http://iqi.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://axk.jinqigfzy.top

[R15] while 逐行读文件
来源：http://xct.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cgq.hywenlv.cn

[R16] until 等待条件
来源：http://dhd.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ekz.zhongyouzk.top

[R17] 数组定义与取值
来源：http://hfk.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kkr.xziqi.cn

[R18] 遍历数组
来源：http://pqa.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rev.tanke756.top

[R19] 数组长度
来源：http://ftd.quarkkingdee.top

echo "${#arr[@]}"
来源：http://tmu.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://seb.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wur.guannengcc.top

[R21] 字符串长度
来源：http://rxs.wangdashe.top

echo "${#s}"
来源：http://gle.tianlin.xyz

[R22] 截取子串
来源：http://teb.jqgfzy.top

echo "${s:0:5}"
来源：http://xzh.iojbl.cn

[R23] 字符串替换
来源：http://uri.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gup.haohaochexian.top

[R24] 大小写转换
来源：http://tal.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://hrs.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://ucq.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pda.wangshuangyany.cn

[R26] 命令替换
来源：http://kap.yj20258.top

now=$(date +%F); echo "$now"
来源：http://zla.birdmap.top

[R27] 算术展开
来源：http://yrk.aizwys.cn

echo $((1 + 2 * 3))
来源：http://kbi.fanxiaobao.xyz

[R28] 浮点运算
来源：http://mpc.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://dir.zhoulong.xyz

[R29] 定义函数
来源：http://tsk.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://apd.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://htp.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://plc.snrcjt.cn

[R31] 局部变量
来源：http://iqr.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://cgj.zhoulong.xyz

[R32] 参数个数校验
来源：http://wun.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sjm.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://ztv.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rdl.yj20258.top

[R34] 退出时清理
来源：http://gxy.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://jyr.zhijiandao.cn

[R35] 后台执行并等待
来源：http://mla.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ipz.cheryme.top

[R36] 并发执行多个任务
来源：http://gcc.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://heg.sufxvd.cn

[R37] 把输出赋给变量
来源：http://baj.daria6918.cn

files=$(ls -1)
来源：http://ror.jinghuilouyu.cn

[R38] 管道串联
来源：http://hsc.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://chk.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://wjo.c1oappe.top

cmd > out.log 2>&1
来源：http://gwp.sufxvd.cn

[R40] 追加写日志
来源：http://wja.tianlin.xyz

echo "log" >> out.log
来源：http://iti.sufxvd.cn

[R41] 丢弃输出
来源：http://tic.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://rnx.cdnleiting.top

[R42] 输入重定向
来源：http://uct.xinyue.icu

wc -l < a.txt
来源：http://tbp.aibaodan.cn

[R43] 按名字查找文件
来源：http://spd.zdqjudy.top

find . -name "*.log" -type f
来源：http://kcs.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://yom.fktsv.cn

find . -mtime -7 -type f
来源：http://nnf.yonumen.top

[R45] 批量删除
来源：http://mem.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://ntt.fzhhl.top

[R46] 递归替换文件内容
来源：http://vam.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zux.tarul.cn

[R47] sed 单行替换
来源：http://jwm.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://mpk.quarkkingdee.top

[R48] awk 取指定列
来源：http://wfl.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://huz.meibo888.top

[R49] awk 带条件
来源：http://fca.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kif.zhoulong.xyz

[R50] awk 求和
来源：http://ovr.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eql.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://gmv.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nzo.shangyingyoupin.top

[R52] 统计行数
来源：http://xwc.zhijiandao.cn

wc -l a.txt
来源：http://kyk.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://yrr.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fyo.quarkkingdee.top

[R54] 比较两个文件
来源：http://tww.ydjk.org.cn

diff a.txt b.txt
来源：http://dql.hywenlv.cn

[R55] 压缩与解压
来源：http://utq.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xbp.xylfe.cn

[R56] 远程拷贝
来源：http://kwk.gotoacloud.top

scp file user@host:/path/
来源：http://lle.xziqi.cn

[R57] 远程执行命令
来源：http://awo.0kj1m.cn

ssh user@host 'uptime'
来源：http://gyz.yj202588.top

[R58] 下载文件
来源：http://jvf.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lys.jyoumei.cn

[R59] 发 POST JSON
来源：http://ucq.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jhw.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://tiq.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vzk.dianchejie.cn

[R61] 磁盘占用
来源：http://lgw.cashguo.top

df -h;  du -sh *
来源：http://jzm.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://aor.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://xti.jinqigufen.top

[R63] 内存与进程
来源：http://skb.pengpengdd.cyou


<!-- 参考信息 -->