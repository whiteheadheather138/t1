代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qdx.meibo888.top

[Q05] 重命名列
来源：http://yrq.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hoo.aibaodan.cn

[Q06] 删除列
来源：http://eaa.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://isa.pengpengdd.cyou

[Q07] 删除表
来源：http://pyf.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://jqr.yfazqb.com

[Q08] 创建普通索引
来源：http://ldh.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gob.dashuyun.cn

[Q09] 创建唯一索引
来源：http://nmb.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dje.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://pnc.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nqo.jyoumei.cn

[Q11] 一次插入多行
来源：http://mgo.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ptf.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://szn.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://zoo.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://khe.snrcjt.cn

[Q13] 忽略重复插入
来源：http://rxg.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ozs.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://jtn.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://acg.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dtg.cdnleiting.top

[Q15] 查询全部
来源：http://ejv.kuanghao11.cn

SELECT * FROM users;
来源：http://tph.redwolf501.top

[Q16] 查询指定列
来源：http://bwo.316326.xyz

SELECT id, name FROM users;
来源：http://mqd.guannengcc.top

[Q17] 条件查询
来源：http://fln.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jur.yfazqb.com

[Q18] 模糊匹配
来源：http://avj.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://skh.tianlin.xyz

[Q19] 范围查询
来源：http://bue.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvp.guannengcc.top

[Q20] IN 列表
来源：http://vjt.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ytn.sweek.top

[Q21] 空值判断
来源：http://keb.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yzt.sysykeji.top

[Q22] 排序
来源：http://dlg.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lhx.daxiang520.top

[Q23] 分页
来源：http://tlk.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cpu.zhixingplan.top

[Q24] 去重
来源：http://pct.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://vxq.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://pzo.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fjb.yfazqb.com

[Q26] 计数
来源：http://upj.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://mnm.zhoulong.xyz

[Q27] 条件计数
来源：http://qlt.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tsp.daxiang520.top

[Q28] 求和与平均
来源：http://axx.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fhg.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://wbs.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ftg.9152youxi.cn

[Q30] 分组统计
来源：http://kof.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://edl.gotoacloud.top

[Q31] 分组后过滤
来源：http://btf.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fxi.smart0.xyz

[Q32] 分组拼接字符串
来源：http://ngx.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qak.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kgb.zhoulong.xyz

[Q33] 多列分组
来源：http://nrl.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zch.smart0.xyz

[Q34] 每组取第一条
来源：http://kfz.ydjk.org.cn

SELECT * FROM (
来源：http://czn.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gcv.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://zee.ydzc1.top

[Q35] 内连接
来源：http://zvf.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://war.iojbl.cn

[Q36] 左连接
来源：http://qyl.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vkt.tianlin.xyz

[Q37] 右连接
来源：http://uwe.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dye.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://pim.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mhi.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://wzm.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://huc.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rbg.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jru.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://omb.svipenyu.cn

[Q41] 多表连接
来源：http://bbu.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jql.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://bex.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://sil.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://eqk.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://iih.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ptl.meibo888.top

[Q43] 标量子查询
来源：http://rag.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://smz.shuidangran.top

[Q44] IN 子查询
来源：http://abp.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mob.cheryme.top

[Q45] EXISTS 判断存在
来源：http://ako.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dqr.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://brm.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://geu.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://vrp.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://unn.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://qwx.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ngk.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://nbh.ydjk.org.cn

[Q49] 更新单行
来源：http://yns.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kdp.sweek.top

[Q50] 批量更新
来源：http://run.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bzh.fktsv.cn

[Q51] 用子查询更新
来源：http://fsf.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://txp.guowangkeji.top

[Q52] 删除指定行
来源：http://aov.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://oms.ydzc1.top

[Q53] 按条件删除
来源：http://qve.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fyz.nanxuanxn.top

[Q54] 清空表
来源：http://wfs.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://sar.epnwcf.com

[Q55] 排名（并列占位）
来源：http://iri.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hoh.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://owi.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tfh.hywenlv.cn

[Q57] 行号
来源：http://ykc.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lgf.cqqwz.cn

[Q58] 累计求和
来源：http://fsf.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://skf.gogol.net.cn

[Q59] 分组内累计
来源：http://suy.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://evv.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://qjz.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cmd.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dqx.jinghuilouyu.cn

[Q61] 移动平均
来源：http://oqx.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://boy.xylfe.cn

[Q62] 分组占比
来源：http://zoa.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://krs.fzhhl.top

[Q63] 开启事务
来源：http://eqx.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hnv.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://fkd.birdmap.top

COMMIT;
来源：http://nfp.yanxiufei.cn

[Q65] 回滚事务
来源：http://bvs.zhoulong.xyz

ROLLBACK;
来源：http://myi.52xcode.cn

[Q66] 行锁查询
来源：http://nhw.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kwz.hysaishi.cn

[Q67] 设置隔离级别
来源：http://gry.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iof.tanke756.top

[Q68] 保存点
来源：http://lqn.chenlongwang.top

SAVEPOINT sp1;
来源：http://fxt.sysykeji.top

ROLLBACK TO sp1;
来源：http://jpm.cucudq.cn

[Q69] 查看执行计划
来源：http://mwt.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gst.nanxinkj.top

[Q70] 更新统计信息
来源：http://myh.yj20258888.top

ANALYZE TABLE users;
来源：http://ubo.cashguo.top

[Q71] 查看建表语句
来源：http://ebl.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://otp.birdmap.top

[Q72] 查看索引
来源：http://kqz.ppjwa.cn

SHOW INDEX FROM users;
来源：http://hxv.cucudq.cn

[Q73] 查看表状态
来源：http://xcl.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kji.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://iff.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ilv.hesvh.cn

[Q75] 日期格式化
来源：http://eiv.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wan.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fab.uphjek.com

[Q76] 按天统计
来源：http://mht.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ggs.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://may.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ehj.smart0.xyz

[Q78] 当前时间
来源：http://bmh.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jbm.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://cvm.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kok.nanxinkj.top

[Q80] 字符串截取
来源：http://twp.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rpo.xylfe.cn

[Q81] 字符串替换
来源：http://bsx.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ros.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://wpg.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xdp.shangyingyoupin.top

[Q83] 大小写转换
来源：http://fcf.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cgp.zycfv.cn

[Q84] 去除首尾空格
来源：http://sxl.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://gdg.yanxiufei.cn

[Q85] 数值取整
来源：http://ctx.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://exv.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://uwy.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ioj.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://ltc.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qhl.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://bur.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zay.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vfu.fktsv.cn

[Q89] 判断表是否存在
来源：http://xap.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vsf.mhx1999.top

[Q90] 生成序号列
来源：http://xav.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jbk.zhongyouzk.top

================================================================================
来源：http://kxq.c1oappe.top

R. Bash 专题
来源：http://orw.gzhubu.top

================================================================================
来源：http://fyj.tianlin.xyz

[R01] shebang 与严格模式
来源：http://fda.yuxming.cn

#!/usr/bin/env bash
来源：http://yxq.jianghu66.top

set -euo pipefail
来源：http://plc.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://qva.nanxinkj.top

name="Tom"; echo "$name"
来源：http://sok.xuetiantiany.cn

[R03] 只读变量
来源：http://lwt.zhengqikj.top

readonly PI=3.14
来源：http://gig.birdmap.top

[R04] 位置参数
来源：http://lre.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sbg.wangdashe.top

[R05] 参数默认值
来源：http://wbn.tianlin.xyz

name="${1:-default}"
来源：http://sbd.nanxinkj.top

[R06] 判断命令是否存在
来源：http://gxd.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yhn.ppjwa.cn

[R07] if 判断文件
来源：http://onb.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbu.316326.xyz

[R08] 数值比较
来源：http://sos.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cqx.zhoulong.xyz

[R09] 字符串比较
来源：http://dlb.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://why.zdbjq.cn

[R10] 正则匹配
来源：http://seq.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oby.hcnkem.com

[R11] case 多分支
来源：http://gbv.jqgufenzy.top

case "$1" in
来源：http://nsq.cdnleiting.top

start) echo "启动" ;;
来源：http://gcq.iojbl.cn

stop)  echo "停止" ;;
来源：http://hpm.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://bfd.nwbrower.top

esac
来源：http://aid.gogol.net.cn

[R12] for 遍历文件
来源：http://zvl.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://ite.hywenlv.cn

[R13] for 计数循环
来源：http://gpn.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://rvq.cashguo.top

[R14] C 风格 for
来源：http://blu.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lwu.aibaodan.cn

[R15] while 逐行读文件
来源：http://mqw.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dtu.yonumen.top

[R16] until 等待条件
来源：http://kvy.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dcb.vehdjk.com

[R17] 数组定义与取值
来源：http://tau.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://dcp.sufxvd.cn

[R18] 遍历数组
来源：http://mhx.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bmk.zhiwuduotai.top

[R19] 数组长度
来源：http://ucf.316326.xyz

echo "${#arr[@]}"
来源：http://bsu.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://hvc.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xlv.sufxvd.cn

[R21] 字符串长度
来源：http://gjb.haohaochexian.top

echo "${#s}"
来源：http://xej.fzhhl.top

[R22] 截取子串
来源：http://gvh.yuanzhike.top

echo "${s:0:5}"
来源：http://lty.zhixingplan.top

[R23] 字符串替换
来源：http://poi.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ghk.yj202588.top

[R24] 大小写转换
来源：http://zbe.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rth.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://wuv.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gmd.shangyingyoupin.top

[R26] 命令替换
来源：http://ths.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://wnz.pycfn.com

[R27] 算术展开
来源：http://njs.cucudq.cn

echo $((1 + 2 * 3))
来源：http://emr.pengpengdd.cyou

[R28] 浮点运算
来源：http://qrf.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://eal.svipenyu.cn

[R29] 定义函数
来源：http://hnm.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://etx.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://yfp.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://gph.bjfxy.top

[R31] 局部变量
来源：http://bud.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://bvu.fktsv.cn

[R32] 参数个数校验
来源：http://wmr.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://box.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://ayn.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eke.yj20258888.top

[R34] 退出时清理
来源：http://zmh.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://ogn.gzhubu.top

[R35] 后台执行并等待
来源：http://fro.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bvd.shzxlz.cn

[R36] 并发执行多个任务
来源：http://khk.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unb.xziqi.cn

[R37] 把输出赋给变量
来源：http://jbh.gotoacloud.top

files=$(ls -1)
来源：http://qiy.iojbl.cn

[R38] 管道串联
来源：http://jtv.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://qee.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://vor.yonumen.top

cmd > out.log 2>&1
来源：http://rgn.zdqjudy.top

[R40] 追加写日志
来源：http://zig.yuanzhike.top

echo "log" >> out.log
来源：http://avp.yj20258888.top

[R41] 丢弃输出
来源：http://aqs.havefunace.top

cmd >/dev/null 2>&1
来源：http://vgn.zhongyouzk.top

[R42] 输入重定向
来源：http://wqb.epnwcf.com

wc -l < a.txt
来源：http://mvz.jianghu66.top

[R43] 按名字查找文件
来源：http://lhh.ybcxt.top

find . -name "*.log" -type f
来源：http://ghf.quarkkingdee.top

[R44] 按修改时间查找
来源：http://uhi.yfazqb.com

find . -mtime -7 -type f
来源：http://fvd.zhongyouzk.top

[R45] 批量删除
来源：http://ivq.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://bfc.tarul.cn

[R46] 递归替换文件内容
来源：http://hph.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uat.aizwys.cn

[R47] sed 单行替换
来源：http://eep.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://fxp.ppjwa.cn

[R48] awk 取指定列
来源：http://byi.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://ucs.meibo888.top

[R49] awk 带条件
来源：http://sja.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ynq.shuidangran.top

[R50] awk 求和
来源：http://usf.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://hbf.yfazqb.com

[R51] 排序去重取前几
来源：http://xay.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fug.jinqigufen.top

[R52] 统计行数
来源：http://ngv.zhijiandao.cn

wc -l a.txt
来源：http://bgg.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://gvn.kuanghao11.cn


<!-- 参考信息 -->