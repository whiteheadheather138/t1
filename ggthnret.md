代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rog.iojbl.cn

[Q11] 一次插入多行
来源：http://ing.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ucz.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://qpq.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://bcg.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baz.yj20258.top

[Q13] 忽略重复插入
来源：http://ylv.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aez.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://ice.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzd.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://guz.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://crc.zhengqikj.top

SELECT * FROM users;
来源：http://djp.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://fpt.dianchejie.cn

SELECT id, name FROM users;
来源：http://ohd.shuidangran.top

[Q17] 条件查询
来源：http://ikd.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vww.cashguo.top

[Q18] 模糊匹配
来源：http://inx.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://atv.zdqjudy.top

[Q19] 范围查询
来源：http://iid.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eeq.gzhubu.top

[Q20] IN 列表
来源：http://cli.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jqq.vehdjk.com

[Q21] 空值判断
来源：http://aao.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bpg.xuetiantiany.cn

[Q22] 排序
来源：http://zmf.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nze.yangfankeji.com

[Q23] 分页
来源：http://yct.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kvs.yj20258888.top

[Q24] 去重
来源：http://blv.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://kax.sysykeji.top

[Q25] 只取前 N 条
来源：http://rpv.birdmap.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uoz.svipenyu.cn

[Q26] 计数
来源：http://ufn.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://gmz.iojbl.cn

[Q27] 条件计数
来源：http://pep.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lxu.xziqi.cn

[Q28] 求和与平均
来源：http://uvu.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tso.chenjidiqi.icu

[Q29] 最大最小值
来源：http://elu.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jir.xuetiantiany.cn

[Q30] 分组统计
来源：http://xek.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://car.fktsv.cn

[Q31] 分组后过滤
来源：http://tsn.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://awt.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://xpj.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nbe.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hft.quarkkingdee.top

[Q33] 多列分组
来源：http://hfd.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://glp.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://gha.hongshengwenyu.top

SELECT * FROM (
来源：http://rsb.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nia.jqgufenzy.top

) t WHERE rn = 1;
来源：http://tef.0kj1m.cn

[Q35] 内连接
来源：http://kiw.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://paa.gaohongyu789.top

[Q36] 左连接
来源：http://oyy.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uff.aizwys.cn

[Q37] 右连接
来源：http://kdv.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qou.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://wrx.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oij.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://bbq.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kdt.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://swr.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eey.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qwo.gaohongyu789.top

[Q41] 多表连接
来源：http://mwh.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vpx.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://kdm.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://etz.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://cgv.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://rdm.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://waj.gzhubu.top

[Q43] 标量子查询
来源：http://qdq.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sxo.yongpay.top

[Q44] IN 子查询
来源：http://lzf.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jzf.birdmap.top

[Q45] EXISTS 判断存在
来源：http://sdd.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ccv.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fwe.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vrd.zhongyouzk.top

[Q47] 与平均值比较
来源：http://uow.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ads.havefunace.top

[Q48] CTE 公用表表达式
来源：http://tbk.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://djz.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://cmg.ydzc1.top

[Q49] 更新单行
来源：http://eky.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ejo.zhixingplan.top

[Q50] 批量更新
来源：http://adi.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yjr.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://tns.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://crh.mhx1999.top

[Q52] 删除指定行
来源：http://otn.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://vsl.snrcjt.cn

[Q53] 按条件删除
来源：http://auv.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eac.aizwys.cn

[Q54] 清空表
来源：http://huj.yj20258888.top

TRUNCATE TABLE logs;
来源：http://fau.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://spk.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ppt.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://jrg.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nuv.fzhhl.top

[Q57] 行号
来源：http://yml.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://osa.zhengqikj.top

[Q58] 累计求和
来源：http://cgo.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nar.c1oappe.top

[Q59] 分组内累计
来源：http://aec.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nzy.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://nfb.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kyh.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nev.gzhubu.top

[Q61] 移动平均
来源：http://lgz.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jib.iojbl.cn

[Q62] 分组占比
来源：http://qaw.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xxj.guowangkeji.top

[Q63] 开启事务
来源：http://fhk.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qyl.yvedp.cn

[Q64] 提交事务
来源：http://znf.zdqjudy.top

COMMIT;
来源：http://tia.sweek.top

[Q65] 回滚事务
来源：http://vlq.hongshengwenyu.top

ROLLBACK;
来源：http://yli.birdmap.top

[Q66] 行锁查询
来源：http://rgu.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ivk.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://tyz.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oes.aizwys.cn

[Q68] 保存点
来源：http://jat.yueranfly.top

SAVEPOINT sp1;
来源：http://mbl.xinyue.icu

ROLLBACK TO sp1;
来源：http://esu.jianghu66.top

[Q69] 查看执行计划
来源：http://sjv.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qav.cashguo.top

[Q70] 更新统计信息
来源：http://tye.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://kfv.fehbvm.com

[Q71] 查看建表语句
来源：http://dgw.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zja.pycfn.com

[Q72] 查看索引
来源：http://ino.snrcjt.cn

SHOW INDEX FROM users;
来源：http://zhm.tarul.cn

[Q73] 查看表状态
来源：http://yix.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bdv.cucudq.cn

[Q74] 强制使用索引
来源：http://vdg.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tuc.gaohongyu789.top

[Q75] 日期格式化
来源：http://zhv.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sqr.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cjk.jinqigfzy.top

[Q76] 按天统计
来源：http://dgc.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ydv.zhengqikj.top

[Q77] 时间加减
来源：http://jeh.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qkt.ehwqpu.com

[Q78] 当前时间
来源：http://lna.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tgo.fzhhl.top

[Q79] 字符串拼接
来源：http://yrf.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://phs.nanxinkj.top

[Q80] 字符串截取
来源：http://wzs.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zpv.jlsjyb.cn

[Q81] 字符串替换
来源：http://dtt.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rni.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://ath.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uwn.cqqwz.cn

[Q83] 大小写转换
来源：http://fdl.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgz.yangfankeji.com

[Q84] 去除首尾空格
来源：http://dsu.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://pzl.vqdsnc.cn

[Q85] 数值取整
来源：http://klx.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hea.yongpay.top

[Q86] 读取 JSON 字段
来源：http://hsp.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gzp.fzhhl.top

[Q87] JSON 字段做条件
来源：http://etb.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hxk.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://jbh.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fnv.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://muf.yuxming.cn

[Q89] 判断表是否存在
来源：http://xmj.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vtc.hnqzz.top

[Q90] 生成序号列
来源：http://qne.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bsh.sweek.top

================================================================================
来源：http://kbq.yuxming.cn

R. Bash 专题
来源：http://eea.jqgufenzy.top

================================================================================
来源：http://twt.gzhubu.top

[R01] shebang 与严格模式
来源：http://anx.zycfv.cn

#!/usr/bin/env bash
来源：http://ftx.uphjek.com

set -euo pipefail
来源：http://ogg.ppjwa.cn

[R02] 变量赋值与使用
来源：http://lbw.yuxming.cn

name="Tom"; echo "$name"
来源：http://lco.xinyue.icu

[R03] 只读变量
来源：http://ypk.c1oappe.top

readonly PI=3.14
来源：http://osl.wangshuangyany.cn

[R04] 位置参数
来源：http://dqc.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dqo.c1oappe.top

[R05] 参数默认值
来源：http://yqt.0kj1m.cn

name="${1:-default}"
来源：http://vhl.snrcjt.cn

[R06] 判断命令是否存在
来源：http://etz.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://upd.yj20258888.top

[R07] if 判断文件
来源：http://aqh.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nce.shangyingyoupin.top

[R08] 数值比较
来源：http://vyi.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://awx.xuanzx.com

[R09] 字符串比较
来源：http://rua.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jkl.xziqi.cn

[R10] 正则匹配
来源：http://hfo.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xot.bbcook.cn

[R11] case 多分支
来源：http://wqx.zhoulong.xyz

case "$1" in
来源：http://fva.jiagoushi.top

start) echo "启动" ;;
来源：http://ind.meibo888.top

stop)  echo "停止" ;;
来源：http://ypv.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://one.xziqi.cn

esac
来源：http://klz.xuanzx.com

[R12] for 遍历文件
来源：http://rmw.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://mui.gotoacloud.top

[R13] for 计数循环
来源：http://yhu.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://umw.zycfv.cn

[R14] C 风格 for
来源：http://ygu.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rcz.yangfankeji.com

[R15] while 逐行读文件
来源：http://dpw.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mhj.haohaochexian.top

[R16] until 等待条件
来源：http://gzg.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fle.aibaodan.cn

[R17] 数组定义与取值
来源：http://vxz.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://hpj.chenlongwang.top

[R18] 遍历数组
来源：http://pii.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wja.hfpthk.cn

[R19] 数组长度
来源：http://rvi.ivvv.top

echo "${#arr[@]}"
来源：http://pdk.yueranfly.top

[R20] 关联数组（字典）
来源：http://hox.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zac.yj20258.top

[R21] 字符串长度
来源：http://jwv.zdqjudy.top

echo "${#s}"
来源：http://gvx.chenjidiqi.icu

[R22] 截取子串
来源：http://mei.bjfxy.top

echo "${s:0:5}"
来源：http://rxt.yanxiufei.cn

[R23] 字符串替换
来源：http://sps.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zjg.fanxiaobao.xyz

[R24] 大小写转换
来源：http://epo.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://aqw.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://viv.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dsz.xinyue.icu

[R26] 命令替换
来源：http://llz.tarul.cn

now=$(date +%F); echo "$now"
来源：http://mku.quarkkingdee.top

[R27] 算术展开
来源：http://zwt.shuidangran.top

echo $((1 + 2 * 3))
来源：http://qag.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://clh.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://fce.zdqjudy.top

[R29] 定义函数
来源：http://iiu.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qnl.pycfn.com

[R30] 函数返回状态码
来源：http://yrq.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://zik.xylfe.cn

[R31] 局部变量
来源：http://nci.sweek.top

f() { local x=1; echo "$x"; }
来源：http://can.ppjwa.cn

[R32] 参数个数校验
来源：http://suj.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggz.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://xfq.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnu.yuanzhike.top

[R34] 退出时清理
来源：http://jfr.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fsw.tanke756.top

[R35] 后台执行并等待
来源：http://bkl.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://dhs.gotoacloud.top

[R36] 并发执行多个任务
来源：http://quy.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cil.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://dwx.zhengqikj.top

files=$(ls -1)
来源：http://kyu.fehbvm.com

[R38] 管道串联
来源：http://zvw.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://akg.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://vuo.fehbvm.com

cmd > out.log 2>&1
来源：http://lzu.nwbrower.top

[R40] 追加写日志
来源：http://ukc.hfpthk.cn

echo "log" >> out.log
来源：http://bip.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://mtb.ydzc1.top

cmd >/dev/null 2>&1
来源：http://zwi.bbcook.cn

[R42] 输入重定向
来源：http://hcq.jlsjyb.cn

wc -l < a.txt
来源：http://dgl.hnqzz.top

[R43] 按名字查找文件
来源：http://sqq.xylfe.cn

find . -name "*.log" -type f
来源：http://dvs.jqgufenzy.top

[R44] 按修改时间查找
来源：http://wtj.zycfv.cn

find . -mtime -7 -type f
来源：http://zco.sysykeji.top

[R45] 批量删除
来源：http://cln.hnqzz.top

find . -name "*.tmp" -delete
来源：http://pas.yangfankeji.com

[R46] 递归替换文件内容
来源：http://gsl.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ccj.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://cfx.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ufj.hcnkem.com

[R48] awk 取指定列
来源：http://jss.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://mou.yj202588.top

[R49] awk 带条件
来源：http://yep.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tvb.yj202588.top

[R50] awk 求和
来源：http://ayo.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://cmq.316326.xyz

[R51] 排序去重取前几
来源：http://gnv.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xsv.tanke756.top

[R52] 统计行数
来源：http://zaw.sysykeji.top

wc -l a.txt
来源：http://xky.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://mdt.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rcj.tarul.cn

[R54] 比较两个文件
来源：http://bnj.gaohongyu789.top

diff a.txt b.txt
来源：http://jed.nanxuanxn.top

[R55] 压缩与解压
来源：http://nrx.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ibj.gzhubu.top

[R56] 远程拷贝
来源：http://qbu.hnxiangtu.top

scp file user@host:/path/
来源：http://xvm.hysaishi.cn

[R57] 远程执行命令
来源：http://rxq.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://afh.gzhubu.top

[R58] 下载文件
来源：http://onc.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://glv.sweek.top

[R59] 发 POST JSON
来源：http://kmc.svipenyu.cn


<!-- 参考信息 -->