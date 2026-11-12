代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ytt.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hcc.sufxvd.cn

[Q13] 忽略重复插入
来源：http://dfh.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gia.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://zaa.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zsx.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ajq.xuanzx.com

[Q15] 查询全部
来源：http://kup.zdqjudy.top

SELECT * FROM users;
来源：http://ojt.xylfe.cn

[Q16] 查询指定列
来源：http://lne.hysaishi.cn

SELECT id, name FROM users;
来源：http://ugy.shanyushiyangtech.top

[Q17] 条件查询
来源：http://bya.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ekt.haohaochexian.top

[Q18] 模糊匹配
来源：http://irq.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wrk.ydjk.org.cn

[Q19] 范围查询
来源：http://ayg.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ogd.guannengcc.top

[Q20] IN 列表
来源：http://aiw.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bip.meibo888.top

[Q21] 空值判断
来源：http://ipm.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zzg.yj20258888.top

[Q22] 排序
来源：http://kjr.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://can.hcnkem.com

[Q23] 分页
来源：http://qrd.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nuj.yongpay.top

[Q24] 去重
来源：http://bfi.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://lbh.yongpay.top

[Q25] 只取前 N 条
来源：http://rtq.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pll.ehwqpu.com

[Q26] 计数
来源：http://uvs.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://kru.birdmap.top

[Q27] 条件计数
来源：http://chy.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iaf.dianchejie.cn

[Q28] 求和与平均
来源：http://emn.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxs.shangyingyoupin.top

[Q29] 最大最小值
来源：http://wgs.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://djs.chenzaomai.com

[Q30] 分组统计
来源：http://jzh.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wee.ehwqpu.com

[Q31] 分组后过滤
来源：http://jbg.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rio.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://yri.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lwt.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hjs.yanxiufei.cn

[Q33] 多列分组
来源：http://zoh.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ucp.nanxinkj.top

[Q34] 每组取第一条
来源：http://bxf.cucudq.cn

SELECT * FROM (
来源：http://djy.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dlt.daxiang520.top

) t WHERE rn = 1;
来源：http://dat.hesvh.cn

[Q35] 内连接
来源：http://azr.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pkr.cheryme.top

[Q36] 左连接
来源：http://yez.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xby.tanke756.top

[Q37] 右连接
来源：http://tnf.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jvr.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://rrq.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uwc.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://yko.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vfh.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aia.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ube.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vww.chenlongwang.top

[Q41] 多表连接
来源：http://etr.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bnm.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://mkf.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://dgc.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://jed.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://doo.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ozt.yanxiufei.cn

[Q43] 标量子查询
来源：http://zbv.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jrc.dianchejie.cn

[Q44] IN 子查询
来源：http://ndj.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bow.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://kvu.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jss.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://lsr.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ojf.shzxlz.cn

[Q47] 与平均值比较
来源：http://rhl.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bhg.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://nve.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hwf.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://hqw.yfazqb.com

[Q49] 更新单行
来源：http://qan.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lna.hongshengwenyu.top

[Q50] 批量更新
来源：http://yzx.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gcd.ivvv.top

[Q51] 用子查询更新
来源：http://fdl.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xly.chenzaomai.com

[Q52] 删除指定行
来源：http://vee.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://bql.vqdsnc.cn

[Q53] 按条件删除
来源：http://gvz.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wqo.tanke756.top

[Q54] 清空表
来源：http://smd.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://hax.yonumen.top

[Q55] 排名（并列占位）
来源：http://yqd.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://orn.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://vaq.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lxx.chenzaomai.com

[Q57] 行号
来源：http://jsu.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qns.hcnkem.com

[Q58] 累计求和
来源：http://itg.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aqp.zycfv.cn

[Q59] 分组内累计
来源：http://hjn.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hdi.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://cgm.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ztf.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvs.ctjpmb.com

[Q61] 移动平均
来源：http://hkh.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wgb.chenjidiqi.icu

[Q62] 分组占比
来源：http://tyq.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rxo.fehbvm.com

[Q63] 开启事务
来源：http://uqe.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kww.guowangkeji.top

[Q64] 提交事务
来源：http://tsa.jianghu66.top

COMMIT;
来源：http://vul.mhx1999.top

[Q65] 回滚事务
来源：http://ovp.52xcode.cn

ROLLBACK;
来源：http://ofg.zdqjudy.top

[Q66] 行锁查询
来源：http://oqp.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nln.gzhubu.top

[Q67] 设置隔离级别
来源：http://gju.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wfp.hongshengwenyu.top

[Q68] 保存点
来源：http://xga.ybcxt.top

SAVEPOINT sp1;
来源：http://jbx.hysaishi.cn

ROLLBACK TO sp1;
来源：http://syy.andypj.xyz

[Q69] 查看执行计划
来源：http://wrj.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mdj.yj20258888.top

[Q70] 更新统计信息
来源：http://gjj.jiagoushi.top

ANALYZE TABLE users;
来源：http://sqc.hfpthk.cn

[Q71] 查看建表语句
来源：http://kja.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tkq.epnwcf.com

[Q72] 查看索引
来源：http://qej.uphjek.com

SHOW INDEX FROM users;
来源：http://bta.gzhubu.top

[Q73] 查看表状态
来源：http://yio.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fkl.mhx1999.top

[Q74] 强制使用索引
来源：http://jjw.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eas.yuanzhike.top

[Q75] 日期格式化
来源：http://lck.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jwe.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://csx.andypj.xyz

[Q76] 按天统计
来源：http://zch.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dnf.ctjpmb.com

[Q77] 时间加减
来源：http://kzz.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dcw.fzhhl.top

[Q78] 当前时间
来源：http://qwl.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bqy.nanxuanxn.top

[Q79] 字符串拼接
来源：http://spu.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pcf.ybcxt.top

[Q80] 字符串截取
来源：http://stk.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zmw.smart0.xyz

[Q81] 字符串替换
来源：http://ann.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://epf.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://hnm.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwk.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://ebl.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jcf.cdnleiting.top

[Q84] 去除首尾空格
来源：http://flt.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://kgs.havefunace.top

[Q85] 数值取整
来源：http://vbn.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lth.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://wfq.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lud.yfazqb.com

[Q87] JSON 字段做条件
来源：http://tev.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://azy.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://cpu.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kej.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qli.yuxming.cn

[Q89] 判断表是否存在
来源：http://exh.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmd.nanxinkj.top

[Q90] 生成序号列
来源：http://esx.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tsv.cucudq.cn

================================================================================
来源：http://cxe.daxiang520.top

R. Bash 专题
来源：http://wvc.zdqjudy.top

================================================================================
来源：http://bii.cqqwz.cn

[R01] shebang 与严格模式
来源：http://bfu.cheryme.top

#!/usr/bin/env bash
来源：http://ora.yfazqb.com

set -euo pipefail
来源：http://cjo.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://nlq.dianchejie.cn

name="Tom"; echo "$name"
来源：http://rad.tian-w.cn

[R03] 只读变量
来源：http://wza.zhiwuduotai.top

readonly PI=3.14
来源：http://vyh.hnxiangtu.top

[R04] 位置参数
来源：http://ofw.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://egx.zycfv.cn

[R05] 参数默认值
来源：http://kph.havefunace.top

name="${1:-default}"
来源：http://gvp.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://gfw.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qmy.ydzc1.top

[R07] if 判断文件
来源：http://haw.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://woi.aibaodan.cn

[R08] 数值比较
来源：http://lcx.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zio.tanke756.top

[R09] 字符串比较
来源：http://aue.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ggk.aibaodan.cn

[R10] 正则匹配
来源：http://wyh.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kcp.fanxiaobao.xyz

[R11] case 多分支
来源：http://lje.xylfe.cn

case "$1" in
来源：http://pol.daria6918.cn

start) echo "启动" ;;
来源：http://kgl.nanxinkj.top

stop)  echo "停止" ;;
来源：http://vif.hcnkem.com

*)     echo "未知命令" ;;
来源：http://zwv.nanxinkj.top

esac
来源：http://hit.yongpay.top

[R12] for 遍历文件
来源：http://nih.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://xbk.cdnleiting.top

[R13] for 计数循环
来源：http://vrb.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://isc.jinqigfzy.top

[R14] C 风格 for
来源：http://ewz.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rka.yuanzhike.top

[R15] while 逐行读文件
来源：http://dej.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jov.tian-w.cn

[R16] until 等待条件
来源：http://yqs.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mbk.jianghu66.top

[R17] 数组定义与取值
来源：http://ugh.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://lkw.hesvh.cn

[R18] 遍历数组
来源：http://wkp.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://voz.yueranfly.top

[R19] 数组长度
来源：http://nqf.gogol.net.cn

echo "${#arr[@]}"
来源：http://tyq.aizwys.cn

[R20] 关联数组（字典）
来源：http://ybg.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ufp.mhx1999.top

[R21] 字符串长度
来源：http://pze.zdqjudy.top

echo "${#s}"
来源：http://hji.gotoacloud.top

[R22] 截取子串
来源：http://aot.jiagoushi.top

echo "${s:0:5}"
来源：http://pni.gaohongyu789.top

[R23] 字符串替换
来源：http://jym.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aew.hammf.cn

[R24] 大小写转换
来源：http://utq.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://xbs.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://idr.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nnt.hongshengwenyu.top

[R26] 命令替换
来源：http://xnm.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://fmz.dashuyun.cn

[R27] 算术展开
来源：http://qac.tian-w.cn

echo $((1 + 2 * 3))
来源：http://qnc.aibaodan.cn

[R28] 浮点运算
来源：http://tuf.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://mkj.tarul.cn

[R29] 定义函数
来源：http://blp.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ehd.havefunace.top

[R30] 函数返回状态码
来源：http://usy.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://ovc.cdnleiting.top

[R31] 局部变量
来源：http://eqm.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://fkq.zhongyouzk.top

[R32] 参数个数校验
来源：http://wvf.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://knb.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://riw.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fxm.chenzaomai.com

[R34] 退出时清理
来源：http://krw.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://fyl.gaohongyu789.top

[R35] 后台执行并等待
来源：http://gwj.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pht.sweek.top

[R36] 并发执行多个任务
来源：http://zhi.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qof.hywenlv.cn

[R37] 把输出赋给变量
来源：http://ycx.aibaodan.cn

files=$(ls -1)
来源：http://wzi.yuanzhike.top

[R38] 管道串联
来源：http://slt.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://ivq.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://wcn.epnwcf.com

cmd > out.log 2>&1
来源：http://ouw.hnxiangtu.top

[R40] 追加写日志
来源：http://odx.quarkkingdee.top

echo "log" >> out.log
来源：http://ilu.aibaodan.cn

[R41] 丢弃输出
来源：http://gjn.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://gnf.aizwys.cn

[R42] 输入重定向
来源：http://bco.0kj1m.cn

wc -l < a.txt
来源：http://otd.yangfankeji.com

[R43] 按名字查找文件
来源：http://yaj.ehwqpu.com

find . -name "*.log" -type f
来源：http://dqy.sxryk.cn

[R44] 按修改时间查找
来源：http://poq.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://xuu.jinyuanbaomall.cn

[R45] 批量删除
来源：http://occ.yj20258888.top

find . -name "*.tmp" -delete
来源：http://cpo.zdbjq.cn

[R46] 递归替换文件内容
来源：http://wbb.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eoj.svipenyu.cn

[R47] sed 单行替换
来源：http://dvz.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://pre.0kj1m.cn

[R48] awk 取指定列
来源：http://ipt.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://hwq.yuanzhike.top

[R49] awk 带条件
来源：http://qca.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://exf.c1oappe.top

[R50] awk 求和
来源：http://ual.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kte.vehdjk.com

[R51] 排序去重取前几
来源：http://hvc.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iby.epnwcf.com

[R52] 统计行数
来源：http://fdb.zdqjudy.top

wc -l a.txt
来源：http://nkc.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://kgr.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rus.chenjidiqi.icu

[R54] 比较两个文件
来源：http://fhd.52xcode.cn

diff a.txt b.txt
来源：http://hut.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://yuj.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gmi.jianghu66.top

[R56] 远程拷贝
来源：http://zlf.nwbrower.top

scp file user@host:/path/
来源：http://vml.hywenlv.cn

[R57] 远程执行命令
来源：http://ack.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://ffc.jlsjyb.cn

[R58] 下载文件
来源：http://ukb.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxa.0kj1m.cn

[R59] 发 POST JSON
来源：http://mdh.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uch.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://lfg.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qsi.hongshengwenyu.top

[R61] 磁盘占用
来源：http://yow.shanyushiyangtech.top


<!-- 参考信息 -->