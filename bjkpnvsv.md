代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://fso.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aji.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktw.bjfxy.top

[Q15] 查询全部
来源：http://sub.jianghu66.top

SELECT * FROM users;
来源：http://kmh.nanxuanxn.top

[Q16] 查询指定列
来源：http://tba.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://exz.shangyingyoupin.top

[Q17] 条件查询
来源：http://onl.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lqc.zdbjq.cn

[Q18] 模糊匹配
来源：http://cej.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pnm.zdqjudy.top

[Q19] 范围查询
来源：http://jdx.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://unq.sufxvd.cn

[Q20] IN 列表
来源：http://xmx.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upc.cdnleiting.top

[Q21] 空值判断
来源：http://zmt.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ijm.fanxiaobao.xyz

[Q22] 排序
来源：http://afq.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ofm.bjfxy.top

[Q23] 分页
来源：http://vln.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wjw.zhengqikj.top

[Q24] 去重
来源：http://rdc.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://mfr.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://igl.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wiw.shanyushiyangtech.top

[Q26] 计数
来源：http://wkf.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://nnv.dashuyun.cn

[Q27] 条件计数
来源：http://rgq.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xof.ydjk.org.cn

[Q28] 求和与平均
来源：http://ndy.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bwq.uphjek.com

[Q29] 最大最小值
来源：http://plc.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fvk.jiagoushi.top

[Q30] 分组统计
来源：http://eiv.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jqs.jianghu66.top

[Q31] 分组后过滤
来源：http://iib.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cep.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://bbb.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxp.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ynb.yfazqb.com

[Q33] 多列分组
来源：http://jve.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mmg.daxiang520.top

[Q34] 每组取第一条
来源：http://dnl.zhixingplan.top

SELECT * FROM (
来源：http://lck.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://whi.hcnkem.com

) t WHERE rn = 1;
来源：http://sjm.hesvh.cn

[Q35] 内连接
来源：http://haw.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dku.wangdashe.top

[Q36] 左连接
来源：http://nhw.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wig.snrcjt.cn

[Q37] 右连接
来源：http://qil.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pyr.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://whg.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pec.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://stu.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ckp.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yqu.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uoc.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pph.wangdashe.top

[Q41] 多表连接
来源：http://igv.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rbh.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://npj.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://hyd.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://iky.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://acu.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vwx.sxryk.cn

[Q43] 标量子查询
来源：http://cni.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xhs.sufxvd.cn

[Q44] IN 子查询
来源：http://urv.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oju.ivvv.top

[Q45] EXISTS 判断存在
来源：http://vrx.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mdp.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://ypw.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qss.yongpay.top

[Q47] 与平均值比较
来源：http://crk.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tlc.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://fon.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zvm.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://xpg.dianchejie.cn

[Q49] 更新单行
来源：http://umt.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nlw.jlsjyb.cn

[Q50] 批量更新
来源：http://yzw.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yup.ctjpmb.com

[Q51] 用子查询更新
来源：http://vkq.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cot.zycfv.cn

[Q52] 删除指定行
来源：http://zod.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://ryh.yuxming.cn

[Q53] 按条件删除
来源：http://wqx.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xmg.0kj1m.cn

[Q54] 清空表
来源：http://ihg.gzhubu.top

TRUNCATE TABLE logs;
来源：http://xrk.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://vfg.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fgn.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://ofu.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://two.shangyingyoupin.top

[Q57] 行号
来源：http://gan.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jot.gaohongyu789.top

[Q58] 累计求和
来源：http://yrj.jlsjyb.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jib.jyoumei.cn

[Q59] 分组内累计
来源：http://erq.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ynz.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://jmo.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dth.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tuv.ctjpmb.com

[Q61] 移动平均
来源：http://qjy.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ycq.hammf.cn

[Q62] 分组占比
来源：http://bmc.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://stv.chenlongwang.top

[Q63] 开启事务
来源：http://eye.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxx.nwbrower.top

[Q64] 提交事务
来源：http://ond.shangyingyoupin.top

COMMIT;
来源：http://mch.cqqwz.cn

[Q65] 回滚事务
来源：http://qec.redwolf501.top

ROLLBACK;
来源：http://fvh.yj20258888.top

[Q66] 行锁查询
来源：http://iub.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kin.zdbjq.cn

[Q67] 设置隔离级别
来源：http://shi.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kaw.zycfv.cn

[Q68] 保存点
来源：http://ewi.hywenlv.cn

SAVEPOINT sp1;
来源：http://oqj.hnqzz.top

ROLLBACK TO sp1;
来源：http://kup.yj20258.top

[Q69] 查看执行计划
来源：http://ayf.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ojb.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://ach.havefunace.top

ANALYZE TABLE users;
来源：http://gae.cqqwz.cn

[Q71] 查看建表语句
来源：http://igk.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pap.daxiang520.top

[Q72] 查看索引
来源：http://wli.yuxming.cn

SHOW INDEX FROM users;
来源：http://nun.yvedp.cn

[Q73] 查看表状态
来源：http://ymv.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://swk.nanxinkj.top

[Q74] 强制使用索引
来源：http://vvr.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hxr.pycfn.com

[Q75] 日期格式化
来源：http://frs.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zug.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nhm.aizwys.cn

[Q76] 按天统计
来源：http://nma.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iaa.hnxiangtu.top

[Q77] 时间加减
来源：http://qxv.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fks.jyoumei.cn

[Q78] 当前时间
来源：http://gee.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://snu.vehdjk.com

[Q79] 字符串拼接
来源：http://ngz.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jxp.cqqwz.cn

[Q80] 字符串截取
来源：http://ahe.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ywa.bjfxy.top

[Q81] 字符串替换
来源：http://wsd.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ibv.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://tem.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dro.sweek.top

[Q83] 大小写转换
来源：http://spw.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://klx.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://mmm.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://fji.zhixingplan.top

[Q85] 数值取整
来源：http://vrb.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pca.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://gkt.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ofz.havefunace.top

[Q87] JSON 字段做条件
来源：http://nhh.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tof.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://sxo.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wbm.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pqp.zdbjq.cn

[Q89] 判断表是否存在
来源：http://qmr.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cdc.sufxvd.cn

[Q90] 生成序号列
来源：http://qny.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://byx.hywenlv.cn

================================================================================
来源：http://vqa.ydzc1.top

R. Bash 专题
来源：http://zaq.yj20258888.top

================================================================================
来源：http://dop.dianchejie.cn

[R01] shebang 与严格模式
来源：http://qjq.yangfankeji.com

#!/usr/bin/env bash
来源：http://dtw.yj20258.top

set -euo pipefail
来源：http://ilp.yuanzhike.top

[R02] 变量赋值与使用
来源：http://hwa.gotoacloud.top

name="Tom"; echo "$name"
来源：http://iue.ppjwa.cn

[R03] 只读变量
来源：http://lmp.xinyue.icu

readonly PI=3.14
来源：http://plz.fktsv.cn

[R04] 位置参数
来源：http://rap.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mpt.bjfxy.top

[R05] 参数默认值
来源：http://ovn.bjfxy.top

name="${1:-default}"
来源：http://ust.0kj1m.cn

[R06] 判断命令是否存在
来源：http://kdi.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ocq.yfazqb.com

[R07] if 判断文件
来源：http://vml.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dni.jinyuanbaomall.cn

[R08] 数值比较
来源：http://kov.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://erx.hysaishi.cn

[R09] 字符串比较
来源：http://fqn.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jjs.sxryk.cn

[R10] 正则匹配
来源：http://ueh.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rki.jinqigfzy.top

[R11] case 多分支
来源：http://nmg.yfazqb.com

case "$1" in
来源：http://oxl.ehwqpu.com

start) echo "启动" ;;
来源：http://ukb.ybcxt.top

stop)  echo "停止" ;;
来源：http://qjz.fktsv.cn

*)     echo "未知命令" ;;
来源：http://sjo.jinghuilouyu.cn

esac
来源：http://asa.ydjk.org.cn

[R12] for 遍历文件
来源：http://nvc.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://ptc.fktsv.cn

[R13] for 计数循环
来源：http://xbd.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://ozb.jiagoushi.top

[R14] C 风格 for
来源：http://ctg.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lbn.jiagoushi.top

[R15] while 逐行读文件
来源：http://bsu.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zka.gaohongyu789.top

[R16] until 等待条件
来源：http://pfw.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xsv.yonumen.top

[R17] 数组定义与取值
来源：http://vmi.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vak.yj202588.top

[R18] 遍历数组
来源：http://qng.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wie.fanxiaobao.xyz

[R19] 数组长度
来源：http://enf.bbcook.cn

echo "${#arr[@]}"
来源：http://pbl.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://hdh.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fvz.bbcook.cn

[R21] 字符串长度
来源：http://jtl.yfazqb.com

echo "${#s}"
来源：http://rcp.jinqigufen.top

[R22] 截取子串
来源：http://btv.chenjidiqi.icu

echo "${s:0:5}"
来源：http://tel.tian-w.cn

[R23] 字符串替换
来源：http://eai.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cmt.shanyushiyangtech.top

[R24] 大小写转换
来源：http://hmu.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://qvl.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://ktu.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jfn.gaohongyu789.top

[R26] 命令替换
来源：http://btk.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://svz.xylfe.cn

[R27] 算术展开
来源：http://zxa.cucudq.cn

echo $((1 + 2 * 3))
来源：http://qms.jinqigfzy.top

[R28] 浮点运算
来源：http://rio.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://lys.xuetiantiany.cn

[R29] 定义函数
来源：http://rwc.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://szz.daria6918.cn

[R30] 函数返回状态码
来源：http://kgh.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://zss.zhaomingkeji.xyz

[R31] 局部变量
来源：http://mps.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://zzw.fengsongda.top

[R32] 参数个数校验
来源：http://fvx.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fjj.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://kpl.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cmr.zycfv.cn

[R34] 退出时清理
来源：http://ypw.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lah.guannengcc.top

[R35] 后台执行并等待
来源：http://dwr.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rmt.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://szw.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zsx.aizwys.cn

[R37] 把输出赋给变量
来源：http://yby.dashuyun.cn

files=$(ls -1)
来源：http://cuf.feifeiyinyue.top

[R38] 管道串联
来源：http://uey.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://thc.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://azh.pycfn.com

cmd > out.log 2>&1
来源：http://bmc.ybcxt.top

[R40] 追加写日志
来源：http://jbg.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://qns.gotoacloud.top

[R41] 丢弃输出
来源：http://dvu.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://smd.fanxiaobao.xyz

[R42] 输入重定向
来源：http://xjg.redwolf501.top

wc -l < a.txt
来源：http://tup.uphjek.com

[R43] 按名字查找文件
来源：http://lkf.daxiang520.top

find . -name "*.log" -type f
来源：http://xcz.316326.xyz

[R44] 按修改时间查找
来源：http://zmp.kuanghao11.cn

find . -mtime -7 -type f
来源：http://gpw.kuanghao11.cn

[R45] 批量删除
来源：http://tqb.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://itp.gzhubu.top

[R46] 递归替换文件内容
来源：http://hub.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://knm.svipenyu.cn

[R47] sed 单行替换
来源：http://hxn.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://uoi.sysykeji.top

[R48] awk 取指定列
来源：http://htb.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://rdd.yj20258.top

[R49] awk 带条件
来源：http://rrk.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gsk.zhiwuduotai.top

[R50] awk 求和
来源：http://ccx.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://sxe.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://izz.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nuz.ydzc1.top

[R52] 统计行数
来源：http://qum.jyoumei.cn

wc -l a.txt
来源：http://tan.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://oze.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kph.gotoacloud.top

[R54] 比较两个文件
来源：http://cwa.yanxiufei.cn

diff a.txt b.txt
来源：http://xzv.haohaochexian.top

[R55] 压缩与解压
来源：http://anc.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pqz.xziqi.cn

[R56] 远程拷贝
来源：http://cib.c1oappe.top

scp file user@host:/path/
来源：http://rhq.jlsjyb.cn

[R57] 远程执行命令
来源：http://efj.ehwqpu.com

ssh user@host 'uptime'
来源：http://kbg.pycfn.com

[R58] 下载文件
来源：http://zpw.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zpn.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://dwf.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dbe.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://flk.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iuf.ivvv.top

[R61] 磁盘占用
来源：http://jpv.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://lhi.hywenlv.cn

[R62] 找最占空间的文件
来源：http://mbr.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://yhj.shangyingyoupin.top

[R63] 内存与进程
来源：http://ezr.cdnleiting.top


<!-- 参考信息 -->