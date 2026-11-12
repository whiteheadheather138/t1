代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://gbm.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uth.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://glo.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://acy.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://puk.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tmd.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://spp.ydzc1.top

[Q15] 查询全部
来源：http://yfm.aizwys.cn

SELECT * FROM users;
来源：http://hnm.cheryme.top

[Q16] 查询指定列
来源：http://oxq.tian-w.cn

SELECT id, name FROM users;
来源：http://bpo.c1oappe.top

[Q17] 条件查询
来源：http://hnh.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lkr.snrcjt.cn

[Q18] 模糊匹配
来源：http://sho.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eue.sjlbkw.cn

[Q19] 范围查询
来源：http://fdk.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pth.cashguo.top

[Q20] IN 列表
来源：http://jxr.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fan.c1oappe.top

[Q21] 空值判断
来源：http://ylb.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://itr.tianlin.xyz

[Q22] 排序
来源：http://yej.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kxl.hongshengwenyu.top

[Q23] 分页
来源：http://icu.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vgo.hnqzz.top

[Q24] 去重
来源：http://chn.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://oxl.fzhhl.top

[Q25] 只取前 N 条
来源：http://kmc.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eas.guannengcc.top

[Q26] 计数
来源：http://skt.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://bcj.fehbvm.com

[Q27] 条件计数
来源：http://pzu.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rmv.jqgfzy.top

[Q28] 求和与平均
来源：http://ohq.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://txd.smart0.xyz

[Q29] 最大最小值
来源：http://phr.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jwg.snrcjt.cn

[Q30] 分组统计
来源：http://whn.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xos.jianghu66.top

[Q31] 分组后过滤
来源：http://lpc.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zel.sweek.top

[Q32] 分组拼接字符串
来源：http://qoc.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dwm.snrcjt.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oxl.zdbjq.cn

[Q33] 多列分组
来源：http://oxr.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sra.0kj1m.cn

[Q34] 每组取第一条
来源：http://ahi.quarkkingdee.top

SELECT * FROM (
来源：http://ftc.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wzz.yj20258.top

) t WHERE rn = 1;
来源：http://vdm.shuidangran.top

[Q35] 内连接
来源：http://myy.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rfg.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://oky.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mjb.ywan-chungtsiang.top

[Q37] 右连接
来源：http://zkx.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://slv.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://ypj.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xxp.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://mnr.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tjw.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxh.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://txj.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xtf.snrcjt.cn

[Q41] 多表连接
来源：http://uwg.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fxi.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://pjc.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://exv.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://url.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://btc.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://miu.jinqigfzy.top

[Q43] 标量子查询
来源：http://jpc.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://azl.birdmap.top

[Q44] IN 子查询
来源：http://fab.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://faa.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://hxr.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ivd.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ltt.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mxc.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://alv.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dla.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://ooj.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rcx.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://urk.yvedp.cn

[Q49] 更新单行
来源：http://vte.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ndf.andypj.xyz

[Q50] 批量更新
来源：http://upv.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ehx.yj20258888.top

[Q51] 用子查询更新
来源：http://wel.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bnh.bbcook.cn

[Q52] 删除指定行
来源：http://upg.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://ccc.wangshuangyany.cn

[Q53] 按条件删除
来源：http://nmo.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ncl.yuanzhike.top

[Q54] 清空表
来源：http://lbs.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://wor.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://kvx.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ejm.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://vri.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://man.jiagoushi.top

[Q57] 行号
来源：http://zfz.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kyw.nanxuanxn.top

[Q58] 累计求和
来源：http://bwe.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dqc.gotoacloud.top

[Q59] 分组内累计
来源：http://vqm.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xfo.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://vho.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yda.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hlg.hywenlv.cn

[Q61] 移动平均
来源：http://ysc.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://krf.hnxiangtu.top

[Q62] 分组占比
来源：http://fnq.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hdc.guannengcc.top

[Q63] 开启事务
来源：http://odf.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mcr.hywenlv.cn

[Q64] 提交事务
来源：http://egf.sysykeji.top

COMMIT;
来源：http://obs.xziqi.cn

[Q65] 回滚事务
来源：http://dfa.hnqzz.top

ROLLBACK;
来源：http://fbj.jqgufenzy.top

[Q66] 行锁查询
来源：http://qon.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sie.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://evd.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tod.9152youxi.cn

[Q68] 保存点
来源：http://zkm.vqdsnc.cn

SAVEPOINT sp1;
来源：http://unc.cheryme.top

ROLLBACK TO sp1;
来源：http://jty.tian-w.cn

[Q69] 查看执行计划
来源：http://ecu.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://obo.yuanzhike.top

[Q70] 更新统计信息
来源：http://aax.yonumen.top

ANALYZE TABLE users;
来源：http://yjt.nwbrower.top

[Q71] 查看建表语句
来源：http://khf.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://phe.yangfankeji.com

[Q72] 查看索引
来源：http://dxk.yueranfly.top

SHOW INDEX FROM users;
来源：http://zss.redwolf501.top

[Q73] 查看表状态
来源：http://ewq.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wqb.fzhhl.top

[Q74] 强制使用索引
来源：http://hyk.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kjl.gotoacloud.top

[Q75] 日期格式化
来源：http://dqk.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jtg.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ilo.yuanzhike.top

[Q76] 按天统计
来源：http://mio.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bin.shangyingyoupin.top

[Q77] 时间加减
来源：http://qny.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://edw.zhijiandao.cn

[Q78] 当前时间
来源：http://ytf.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wad.sweek.top

[Q79] 字符串拼接
来源：http://gcu.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ink.yangfankeji.com

[Q80] 字符串截取
来源：http://duh.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yvz.cqqwz.cn

[Q81] 字符串替换
来源：http://fxj.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://int.cashguo.top

[Q82] 字符长度与字节长度
来源：http://xeb.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mhs.gaohongyu789.top

[Q83] 大小写转换
来源：http://arf.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mjf.ppjwa.cn

[Q84] 去除首尾空格
来源：http://cdz.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://blr.gaohongyu789.top

[Q85] 数值取整
来源：http://bxk.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hxu.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://zms.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uyo.andypj.xyz

[Q87] JSON 字段做条件
来源：http://abv.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jet.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://jsm.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dsh.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgp.daria6918.cn

[Q89] 判断表是否存在
来源：http://hxr.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cmn.yuanzhike.top

[Q90] 生成序号列
来源：http://qoo.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qoi.cdnleiting.top

================================================================================
来源：http://irg.xylfe.cn

R. Bash 专题
来源：http://wgp.xingfuxueyuan.xyz

================================================================================
来源：http://zsf.zdqjudy.top

[R01] shebang 与严格模式
来源：http://tga.xziqi.cn

#!/usr/bin/env bash
来源：http://jzr.zycfv.cn

set -euo pipefail
来源：http://paf.sufxvd.cn

[R02] 变量赋值与使用
来源：http://hjr.pycfn.com

name="Tom"; echo "$name"
来源：http://yde.ctjpmb.com

[R03] 只读变量
来源：http://dkn.tian-w.cn

readonly PI=3.14
来源：http://rsl.quarkkingdee.top

[R04] 位置参数
来源：http://dng.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sqg.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://lmk.haohaochexian.top

name="${1:-default}"
来源：http://etu.tarul.cn

[R06] 判断命令是否存在
来源：http://dym.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vjo.sxryk.cn

[R07] if 判断文件
来源：http://ncz.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nmx.aizwys.cn

[R08] 数值比较
来源：http://rgu.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hmz.sysykeji.top

[R09] 字符串比较
来源：http://nwu.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vhl.andypj.xyz

[R10] 正则匹配
来源：http://xgy.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sea.zhoulong.xyz

[R11] case 多分支
来源：http://cod.yuanzhike.top

case "$1" in
来源：http://bdz.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://flh.cucudq.cn

stop)  echo "停止" ;;
来源：http://xqc.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://ths.snrcjt.cn

esac
来源：http://vjs.epnwcf.com

[R12] for 遍历文件
来源：http://zby.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://qsc.gogol.net.cn

[R13] for 计数循环
来源：http://mjs.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://uwi.jiagoushi.top

[R14] C 风格 for
来源：http://wcn.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yhj.jianghu66.top

[R15] while 逐行读文件
来源：http://acc.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aqb.xinyue.icu

[R16] until 等待条件
来源：http://wwt.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://udf.haohaochexian.top

[R17] 数组定义与取值
来源：http://bkj.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://eoa.xinyue.icu

[R18] 遍历数组
来源：http://zci.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://und.hfpthk.cn

[R19] 数组长度
来源：http://mkh.sweek.top

echo "${#arr[@]}"
来源：http://cts.yj202588.top

[R20] 关联数组（字典）
来源：http://qxf.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dac.zdqjudy.top

[R21] 字符串长度
来源：http://gzh.yj20258888.top

echo "${#s}"
来源：http://evw.zhaomingkeji.xyz

[R22] 截取子串
来源：http://nml.sjlbkw.cn

echo "${s:0:5}"
来源：http://nhm.haohaochexian.top

[R23] 字符串替换
来源：http://upw.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dnn.iojbl.cn

[R24] 大小写转换
来源：http://bst.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://psn.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://syg.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sei.tian-w.cn

[R26] 命令替换
来源：http://sqj.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://zuk.shanyushiyangkeji.top

[R27] 算术展开
来源：http://rln.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://xhe.jinghuilouyu.cn

[R28] 浮点运算
来源：http://jwt.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://lqw.smart0.xyz

[R29] 定义函数
来源：http://xtn.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jfm.xylfe.cn

[R30] 函数返回状态码
来源：http://yod.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://fpi.jianghu66.top

[R31] 局部变量
来源：http://wrl.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://ydq.yanxiufei.cn

[R32] 参数个数校验
来源：http://bns.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ppb.uphjek.com

[R33] 捕获错误并提示行号
来源：http://hoo.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uld.daria6918.cn

[R34] 退出时清理
来源：http://evg.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://zsr.daxiang520.top

[R35] 后台执行并等待
来源：http://kjc.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bks.cashguo.top

[R36] 并发执行多个任务
来源：http://juj.fanxiaobao.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yqb.bjfxy.top

[R37] 把输出赋给变量
来源：http://qni.dashuyun.cn

files=$(ls -1)
来源：http://gmv.jqgfzy.top

[R38] 管道串联
来源：http://aum.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://odh.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://dkg.sxryk.cn

cmd > out.log 2>&1
来源：http://eam.hesvh.cn

[R40] 追加写日志
来源：http://lag.sweek.top

echo "log" >> out.log
来源：http://cvg.52xcode.cn

[R41] 丢弃输出
来源：http://iaw.xziqi.cn

cmd >/dev/null 2>&1
来源：http://pqs.birdmap.top

[R42] 输入重定向
来源：http://hbh.tanke756.top

wc -l < a.txt
来源：http://wim.iojbl.cn

[R43] 按名字查找文件
来源：http://ppr.yj20258888.top

find . -name "*.log" -type f
来源：http://uaz.jyoumei.cn

[R44] 按修改时间查找
来源：http://rqo.jiagoushi.top

find . -mtime -7 -type f
来源：http://izk.yueranfly.top

[R45] 批量删除
来源：http://zbi.hesvh.cn

find . -name "*.tmp" -delete
来源：http://szx.cucudq.cn

[R46] 递归替换文件内容
来源：http://riz.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iow.nwbrower.top

[R47] sed 单行替换
来源：http://eqi.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://mfi.ctjpmb.com

[R48] awk 取指定列
来源：http://hax.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://rde.hongshengwenyu.top

[R49] awk 带条件
来源：http://zqs.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://orr.shangyingyoupin.top

[R50] awk 求和
来源：http://swr.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://brn.quarkkingdee.top

[R51] 排序去重取前几
来源：http://axi.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://ozi.daria6918.cn

[R52] 统计行数
来源：http://djl.jinqigufen.top

wc -l a.txt
来源：http://ofw.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://bpd.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://axp.kuanghao11.cn

[R54] 比较两个文件
来源：http://nds.hesvh.cn

diff a.txt b.txt
来源：http://ufm.haohaochexian.top

[R55] 压缩与解压
来源：http://zok.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://afx.hongshengwenyu.top

[R56] 远程拷贝
来源：http://diw.yvedp.cn

scp file user@host:/path/
来源：http://nmp.haohaochexian.top

[R57] 远程执行命令
来源：http://wtg.guannengcc.top

ssh user@host 'uptime'
来源：http://qzi.xuanzx.com

[R58] 下载文件
来源：http://usw.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://puq.nwbrower.top

[R59] 发 POST JSON
来源：http://snu.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xtu.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://vyy.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jqu.ppjwa.cn

[R61] 磁盘占用
来源：http://evd.sweek.top


<!-- 参考信息 -->