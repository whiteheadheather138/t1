代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jqc.hnqzz.top

);
来源：http://ziz.sweek.top

[Q02] 创建带外键的表
来源：http://ont.yangfankeji.com

CREATE TABLE orders (
来源：http://vxk.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wel.bbcook.cn

user_id INT NOT NULL,
来源：http://rzd.zycfv.cn

amount DECIMAL(10, 2),
来源：http://zql.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qfc.ivvv.top

);
来源：http://kaq.vqdsnc.cn

[Q03] 增加列
来源：http://osg.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kny.nanxinkj.top

[Q04] 修改列类型
来源：http://stf.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dyw.ppjwa.cn

[Q05] 重命名列
来源：http://oyd.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gug.jiagoushi.top

[Q06] 删除列
来源：http://mez.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://rdj.zhoulong.xyz

[Q07] 删除表
来源：http://wce.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://heu.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://ugq.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://dyj.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://quc.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nqj.yuxming.cn

[Q10] 插入单行
来源：http://krt.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wva.andypj.xyz

[Q11] 一次插入多行
来源：http://yfd.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kfd.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://qec.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jpu.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://efl.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://oax.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bed.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://rmb.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mxf.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oyw.xinyue.icu

[Q15] 查询全部
来源：http://oos.bbcook.cn

SELECT * FROM users;
来源：http://wfy.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://yaw.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://nux.hcnkem.com

[Q17] 条件查询
来源：http://lgo.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eol.yuanzhike.top

[Q18] 模糊匹配
来源：http://kbz.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mdz.daria6918.cn

[Q19] 范围查询
来源：http://oec.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://med.nanxuanxn.top

[Q20] IN 列表
来源：http://nmz.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tax.xziqi.cn

[Q21] 空值判断
来源：http://tnr.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ibx.hongshengwenyu.top

[Q22] 排序
来源：http://mmt.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vez.fzhhl.top

[Q23] 分页
来源：http://iwv.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkf.ehwqpu.com

[Q24] 去重
来源：http://qxa.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://tvl.hammf.cn

[Q25] 只取前 N 条
来源：http://rvu.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://emq.zdqjudy.top

[Q26] 计数
来源：http://hbo.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://ieu.hnqzz.top

[Q27] 条件计数
来源：http://htk.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zrr.aibaodan.cn

[Q28] 求和与平均
来源：http://tla.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bqg.sjlbkw.cn

[Q29] 最大最小值
来源：http://nsm.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lyd.ctjpmb.com

[Q30] 分组统计
来源：http://lvn.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igz.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://zzw.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dhe.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://xoh.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gqo.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jik.sysykeji.top

[Q33] 多列分组
来源：http://gxg.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kyu.uphjek.com

[Q34] 每组取第一条
来源：http://eje.gogol.net.cn

SELECT * FROM (
来源：http://zkc.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uhf.ydjk.org.cn

) t WHERE rn = 1;
来源：http://bzv.birdmap.top

[Q35] 内连接
来源：http://wok.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ifr.yj20258888.top

[Q36] 左连接
来源：http://sjn.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://boy.fanxiaobao.xyz

[Q37] 右连接
来源：http://zik.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qhf.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bgl.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gmz.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://izs.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://msl.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ckz.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rib.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rxc.zhoulong.xyz

[Q41] 多表连接
来源：http://lpb.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tjl.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://itj.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://tdy.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://jft.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://njy.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fcb.jqgfzy.top

[Q43] 标量子查询
来源：http://wqd.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kcj.uphjek.com

[Q44] IN 子查询
来源：http://plr.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gew.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://qou.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzu.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://omx.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vyb.ctjpmb.com

[Q47] 与平均值比较
来源：http://lci.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vru.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://qcz.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mpf.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://ibc.zdqjudy.top

[Q49] 更新单行
来源：http://owz.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kzb.sxryk.cn

[Q50] 批量更新
来源：http://ofc.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hmq.yuanzhike.top

[Q51] 用子查询更新
来源：http://akk.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://afa.yonumen.top

[Q52] 删除指定行
来源：http://zcl.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://xmo.hnqzz.top

[Q53] 按条件删除
来源：http://yxc.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zwp.daxiang520.top

[Q54] 清空表
来源：http://dae.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://xet.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://nrg.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://brw.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://zbf.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nvc.guannengcc.top

[Q57] 行号
来源：http://ztc.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ang.jqgufenzy.top

[Q58] 累计求和
来源：http://qbx.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://weu.yvedp.cn

[Q59] 分组内累计
来源：http://uuz.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cqa.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://wqs.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uej.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xmy.gogol.net.cn

[Q61] 移动平均
来源：http://pfu.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hrr.yj20258.top

[Q62] 分组占比
来源：http://hir.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjw.sxryk.cn

[Q63] 开启事务
来源：http://vdq.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ykd.chenlongwang.top

[Q64] 提交事务
来源：http://udf.ehwqpu.com

COMMIT;
来源：http://erv.jyoumei.cn

[Q65] 回滚事务
来源：http://dmo.kuanghao11.cn

ROLLBACK;
来源：http://ixa.vehdjk.com

[Q66] 行锁查询
来源：http://xgf.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jpf.mhx1999.top

[Q67] 设置隔离级别
来源：http://adt.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qny.shanyushiyangkeji.top

[Q68] 保存点
来源：http://isv.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://ysw.jinqigufen.top

ROLLBACK TO sp1;
来源：http://ouq.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://lad.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nds.yuanzhike.top

[Q70] 更新统计信息
来源：http://bnp.mhx1999.top

ANALYZE TABLE users;
来源：http://ymf.yanxiufei.cn

[Q71] 查看建表语句
来源：http://rpc.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jdq.jiagoushi.top

[Q72] 查看索引
来源：http://xzt.shzxlz.cn

SHOW INDEX FROM users;
来源：http://rjn.cqqwz.cn

[Q73] 查看表状态
来源：http://nvs.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kpt.sjlbkw.cn

[Q74] 强制使用索引
来源：http://kyw.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zuv.xuanzx.com

[Q75] 日期格式化
来源：http://lbb.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rmq.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fmd.dianchejie.cn

[Q76] 按天统计
来源：http://uvv.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nlo.yonumen.top

[Q77] 时间加减
来源：http://gsa.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fth.zhoulong.xyz

[Q78] 当前时间
来源：http://dba.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kok.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://vjb.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://woq.zycfv.cn

[Q80] 字符串截取
来源：http://gfy.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mtg.smart0.xyz

[Q81] 字符串替换
来源：http://igd.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gqn.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://hkt.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://csy.yuanzhike.top

[Q83] 大小写转换
来源：http://kdk.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://njd.cashguo.top

[Q84] 去除首尾空格
来源：http://saf.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://uxb.sweek.top

[Q85] 数值取整
来源：http://bvl.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mev.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://weh.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jid.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://ajd.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bct.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://nrf.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://naz.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zac.ctjpmb.com

[Q89] 判断表是否存在
来源：http://hgx.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kis.gzhubu.top

[Q90] 生成序号列
来源：http://eib.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jlx.9152youxi.cn

================================================================================
来源：http://sxv.chenlongwang.top

R. Bash 专题
来源：http://akn.hcnkem.com

================================================================================
来源：http://wrn.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://gqy.guowangkeji.top

#!/usr/bin/env bash
来源：http://csn.wangshuangyany.cn

set -euo pipefail
来源：http://gst.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://rny.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://qsn.smart0.xyz

[R03] 只读变量
来源：http://rhg.fengsongda.top

readonly PI=3.14
来源：http://sog.guowangkeji.top

[R04] 位置参数
来源：http://npv.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lca.yuanzhike.top

[R05] 参数默认值
来源：http://evh.c1oappe.top

name="${1:-default}"
来源：http://osf.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://hfz.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vtj.dashuyun.cn

[R07] if 判断文件
来源：http://yro.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lka.0kj1m.cn

[R08] 数值比较
来源：http://lwh.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ubi.chenzaomai.com

[R09] 字符串比较
来源：http://zna.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jmk.hywenlv.cn

[R10] 正则匹配
来源：http://kyy.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uzj.jiagoushi.top

[R11] case 多分支
来源：http://ekt.cqqwz.cn

case "$1" in
来源：http://ytt.hnxiangtu.top

start) echo "启动" ;;
来源：http://clq.bbcook.cn

stop)  echo "停止" ;;
来源：http://cgt.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://bst.sxryk.cn

esac
来源：http://wgu.zhixingplan.top

[R12] for 遍历文件
来源：http://ucc.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://aqi.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://umt.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://kwv.bbcook.cn

[R14] C 风格 for
来源：http://afq.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xuc.hesvh.cn

[R15] while 逐行读文件
来源：http://dfk.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kes.gotoacloud.top

[R16] until 等待条件
来源：http://esf.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fyg.yueranfly.top

[R17] 数组定义与取值
来源：http://vra.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://wpl.daria6918.cn

[R18] 遍历数组
来源：http://ylc.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxc.yj20258888.top

[R19] 数组长度
来源：http://wnb.chenlongwang.top

echo "${#arr[@]}"
来源：http://dqv.ctjpmb.com

[R20] 关联数组（字典）
来源：http://kzd.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://klj.yanxiufei.cn

[R21] 字符串长度
来源：http://vqj.birdmap.top

echo "${#s}"
来源：http://sez.wangdashe.top

[R22] 截取子串
来源：http://ilx.pycfn.com

echo "${s:0:5}"
来源：http://hvg.fzhhl.top

[R23] 字符串替换
来源：http://wtk.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gdl.dianchejie.cn

[R24] 大小写转换
来源：http://xdj.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rtz.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://mtv.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://irg.fanxiaobao.xyz

[R26] 命令替换
来源：http://dpx.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://sgf.jinyuanbaomall.cn

[R27] 算术展开
来源：http://cbt.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://myq.epnwcf.com

[R28] 浮点运算
来源：http://wvn.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://jph.zdqjudy.top

[R29] 定义函数
来源：http://fmz.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://atr.pycfn.com

[R30] 函数返回状态码
来源：http://huo.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://zyf.shanyushiyangtech.top

[R31] 局部变量
来源：http://sux.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://phw.haohaochexian.top

[R32] 参数个数校验
来源：http://bwe.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kbr.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://yhd.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vkb.zdqjudy.top

[R34] 退出时清理
来源：http://njc.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://gxs.cashguo.top

[R35] 后台执行并等待
来源：http://clk.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nyv.zhengqikj.top

[R36] 并发执行多个任务
来源：http://nby.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cos.pycfn.com

[R37] 把输出赋给变量
来源：http://bjs.yvedp.cn

files=$(ls -1)
来源：http://gci.chenlongwang.top

[R38] 管道串联
来源：http://fcz.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://xcr.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://jwt.nanxinkj.top

cmd > out.log 2>&1
来源：http://khw.sufxvd.cn

[R40] 追加写日志
来源：http://igb.sufxvd.cn

echo "log" >> out.log
来源：http://jqg.tanke756.top

[R41] 丢弃输出
来源：http://dhu.tanke756.top

cmd >/dev/null 2>&1
来源：http://duf.yuxming.cn

[R42] 输入重定向
来源：http://nyx.zdqjudy.top

wc -l < a.txt
来源：http://pmb.ybcxt.top

[R43] 按名字查找文件
来源：http://eek.yfazqb.com

find . -name "*.log" -type f
来源：http://fut.vehdjk.com

[R44] 按修改时间查找
来源：http://zur.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://sbq.shuidangran.top

[R45] 批量删除
来源：http://hvc.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://sju.cucudq.cn

[R46] 递归替换文件内容
来源：http://scc.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mmn.wangdashe.top

[R47] sed 单行替换
来源：http://nkw.pycfn.com


<!-- 参考信息 -->