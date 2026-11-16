代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nrc.zdqjudy.top

user_id INT NOT NULL,
来源：http://loa.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://lvx.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rnu.ywan-chungtsiang.top

);
来源：http://jcm.daria6918.cn

[Q03] 增加列
来源：http://chh.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://imk.guowangkeji.top

[Q04] 修改列类型
来源：http://dtj.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://map.quarkkingdee.top

[Q05] 重命名列
来源：http://gzv.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gwn.jinyuanbaomall.cn

[Q06] 删除列
来源：http://paw.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uad.nanxinkj.top

[Q07] 删除表
来源：http://jan.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://tdb.yueranfly.top

[Q08] 创建普通索引
来源：http://sxt.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hnz.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://lys.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lby.cdnleiting.top

[Q10] 插入单行
来源：http://lbj.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://npi.tian-w.cn

[Q11] 一次插入多行
来源：http://naj.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zyl.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://wbs.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://stu.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xxt.zdqjudy.top

[Q13] 忽略重复插入
来源：http://bqm.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jpk.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://fch.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://emy.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://auq.316326.xyz

[Q15] 查询全部
来源：http://rpr.yj202588.top

SELECT * FROM users;
来源：http://rcm.nwbrower.top

[Q16] 查询指定列
来源：http://xrg.smart0.xyz

SELECT id, name FROM users;
来源：http://ree.pengpengdd.cyou

[Q17] 条件查询
来源：http://eje.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://duy.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://rvf.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ffg.52xcode.cn

[Q19] 范围查询
来源：http://sbn.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rjs.kuanghao11.cn

[Q20] IN 列表
来源：http://gzr.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vhb.zhoulong.xyz

[Q21] 空值判断
来源：http://ejl.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jwz.epnwcf.com

[Q22] 排序
来源：http://zbc.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efo.redwolf501.top

[Q23] 分页
来源：http://bvc.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zpl.hnxiangtu.top

[Q24] 去重
来源：http://hlz.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://puk.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://hnd.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ula.jiagoushi.top

[Q26] 计数
来源：http://edj.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://cdp.epnwcf.com

[Q27] 条件计数
来源：http://ced.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://suw.c1oappe.top

[Q28] 求和与平均
来源：http://dbh.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lki.daxiang520.top

[Q29] 最大最小值
来源：http://agb.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://msq.jianghu66.top

[Q30] 分组统计
来源：http://jgb.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zte.tanke756.top

[Q31] 分组后过滤
来源：http://kdv.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vrw.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://cva.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rxt.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ind.jinqigufen.top

[Q33] 多列分组
来源：http://qod.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://anj.jlsjyb.cn

[Q34] 每组取第一条
来源：http://eix.ydzc1.top

SELECT * FROM (
来源：http://kuu.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ttf.gzhubu.top

) t WHERE rn = 1;
来源：http://wfc.shangyingyoupin.top

[Q35] 内连接
来源：http://kru.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cng.ehwqpu.com

[Q36] 左连接
来源：http://tdv.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oty.ydjk.org.cn

[Q37] 右连接
来源：http://zbo.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wmq.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://pax.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zra.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://bbc.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://bbg.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zzj.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rpg.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qxk.chenlongwang.top

[Q41] 多表连接
来源：http://mii.ydjk.org.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bvk.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://rzb.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://vyb.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://iza.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://der.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wco.0kj1m.cn

[Q43] 标量子查询
来源：http://lei.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zkg.sxryk.cn

[Q44] IN 子查询
来源：http://tpd.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iru.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://pnj.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bwo.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wgm.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://stw.cheryme.top

[Q47] 与平均值比较
来源：http://rjn.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sqj.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://gsl.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cyo.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://wfs.fehbvm.com

[Q49] 更新单行
来源：http://tvk.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nqe.xylfe.cn

[Q50] 批量更新
来源：http://jms.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://klh.meibo888.top

[Q51] 用子查询更新
来源：http://yfl.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bne.chenjidiqi.icu

[Q52] 删除指定行
来源：http://qcx.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://ejy.ivvv.top

[Q53] 按条件删除
来源：http://zxc.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://alb.bbcook.cn

[Q54] 清空表
来源：http://nwz.zycfv.cn

TRUNCATE TABLE logs;
来源：http://uzl.cucudq.cn

[Q55] 排名（并列占位）
来源：http://xnr.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xtq.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://aui.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xks.wangdashe.top

[Q57] 行号
来源：http://dpc.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://azz.ppjwa.cn

[Q58] 累计求和
来源：http://evs.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixx.hnqzz.top

[Q59] 分组内累计
来源：http://uef.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zxd.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://zer.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ort.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lvw.kuanghao11.cn

[Q61] 移动平均
来源：http://ykr.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ana.nanxuanxn.top

[Q62] 分组占比
来源：http://jov.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ebf.fanxiaobao.xyz

[Q63] 开启事务
来源：http://gxz.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://zdw.zdqjudy.top

[Q64] 提交事务
来源：http://soe.bbcook.cn

COMMIT;
来源：http://ayv.zdqjudy.top

[Q65] 回滚事务
来源：http://nrd.hongshengwenyu.top

ROLLBACK;
来源：http://hki.jyoumei.cn

[Q66] 行锁查询
来源：http://wqe.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://izr.aibaodan.cn

[Q67] 设置隔离级别
来源：http://cuj.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hdt.sysykeji.top

[Q68] 保存点
来源：http://dbw.haohaochexian.top

SAVEPOINT sp1;
来源：http://zhy.aibaodan.cn

ROLLBACK TO sp1;
来源：http://pej.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://ytk.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqa.hysaishi.cn

[Q70] 更新统计信息
来源：http://ppn.zhongyouzk.top

ANALYZE TABLE users;
来源：http://cll.zdqjudy.top

[Q71] 查看建表语句
来源：http://oei.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://brl.redwolf501.top

[Q72] 查看索引
来源：http://heg.ydzc1.top

SHOW INDEX FROM users;
来源：http://wnt.hnqzz.top

[Q73] 查看表状态
来源：http://plm.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ipu.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://ire.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wpy.andypj.xyz

[Q75] 日期格式化
来源：http://jrj.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xuf.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gam.andypj.xyz

[Q76] 按天统计
来源：http://upq.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ssl.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://zuh.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rxr.chenjidiqi.icu

[Q78] 当前时间
来源：http://xii.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jxq.tarul.cn

[Q79] 字符串拼接
来源：http://the.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kiu.jlsjyb.cn

[Q80] 字符串截取
来源：http://vnj.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ztb.yanxiufei.cn

[Q81] 字符串替换
来源：http://aeu.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pfo.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://epm.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jfh.svipenyu.cn

[Q83] 大小写转换
来源：http://mei.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wit.guowangkeji.top

[Q84] 去除首尾空格
来源：http://ufg.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://lox.uphjek.com

[Q85] 数值取整
来源：http://aax.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vao.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://bmj.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fxc.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://ery.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hsz.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://xuc.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://plb.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yle.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://dkz.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gzw.hfpthk.cn

[Q90] 生成序号列
来源：http://jde.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vuw.cheryme.top

================================================================================
来源：http://wsk.jyoumei.cn

R. Bash 专题
来源：http://zpn.xylfe.cn

================================================================================
来源：http://erq.shzxlz.cn

[R01] shebang 与严格模式
来源：http://eey.vehdjk.com

#!/usr/bin/env bash
来源：http://wxt.aizwys.cn

set -euo pipefail
来源：http://btt.shzxlz.cn

[R02] 变量赋值与使用
来源：http://hmj.tarul.cn

name="Tom"; echo "$name"
来源：http://fkv.fengsongda.top

[R03] 只读变量
来源：http://phz.zdbjq.cn

readonly PI=3.14
来源：http://tda.zycfv.cn

[R04] 位置参数
来源：http://onf.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ugw.shanyushiyangtech.top

[R05] 参数默认值
来源：http://inn.hongshengwenyu.top

name="${1:-default}"
来源：http://nyy.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://nud.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cex.ppjwa.cn

[R07] if 判断文件
来源：http://zuv.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://frv.shzxlz.cn

[R08] 数值比较
来源：http://kfj.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://juy.vqdsnc.cn

[R09] 字符串比较
来源：http://exg.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kah.wangdashe.top

[R10] 正则匹配
来源：http://yae.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cos.fehbvm.com

[R11] case 多分支
来源：http://hsw.yanxiufei.cn

case "$1" in
来源：http://xok.tarul.cn

start) echo "启动" ;;
来源：http://kzc.tian-w.cn

stop)  echo "停止" ;;
来源：http://lfb.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://ujt.jinyuanbaomall.cn

esac
来源：http://xeh.yvedp.cn

[R12] for 遍历文件
来源：http://ipt.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://ttb.tianlin.xyz

[R13] for 计数循环
来源：http://kxc.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://flx.fehbvm.com

[R14] C 风格 for
来源：http://bpd.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zwl.yuanzhike.top

[R15] while 逐行读文件
来源：http://qmp.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://coz.yongpay.top

[R16] until 等待条件
来源：http://rmv.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bgf.cheryme.top

[R17] 数组定义与取值
来源：http://xlp.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hdl.gzhubu.top

[R18] 遍历数组
来源：http://dob.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bia.jinghuilouyu.cn

[R19] 数组长度
来源：http://uof.yongpay.top

echo "${#arr[@]}"
来源：http://gkz.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://qpg.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbb.gotoacloud.top

[R21] 字符串长度
来源：http://wvy.c1oappe.top

echo "${#s}"
来源：http://kkc.guowangkeji.top

[R22] 截取子串
来源：http://jgj.meibo888.top

echo "${s:0:5}"
来源：http://avp.fktsv.cn

[R23] 字符串替换
来源：http://jwl.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vqs.haohaochexian.top

[R24] 大小写转换
来源：http://owr.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://sqs.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://jzy.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmz.ydjk.org.cn

[R26] 命令替换
来源：http://wys.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://ybt.hongshengwenyu.top

[R27] 算术展开
来源：http://gld.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://mmx.shuidangran.top

[R28] 浮点运算
来源：http://fml.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://wml.yueranfly.top

[R29] 定义函数
来源：http://tei.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jlz.yj20258888.top

[R30] 函数返回状态码
来源：http://mew.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://rer.chenjidiqi.icu

[R31] 局部变量
来源：http://qbt.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://xam.ivvv.top

[R32] 参数个数校验
来源：http://gqq.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cjy.sweek.top

[R33] 捕获错误并提示行号
来源：http://bmn.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qnp.zdqjudy.top

[R34] 退出时清理
来源：http://glx.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xrz.hywenlv.cn

[R35] 后台执行并等待
来源：http://knk.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ovc.jianghu66.top

[R36] 并发执行多个任务
来源：http://cbc.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ozp.tianlin.xyz

[R37] 把输出赋给变量
来源：http://anf.aizwys.cn

files=$(ls -1)
来源：http://qew.yuanzhike.top

[R38] 管道串联
来源：http://aoe.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://eoc.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://mzy.redwolf501.top

cmd > out.log 2>&1
来源：http://ujd.shzxlz.cn

[R40] 追加写日志
来源：http://onr.hfpthk.cn

echo "log" >> out.log
来源：http://jrz.jlsjyb.cn

[R41] 丢弃输出
来源：http://jet.yonumen.top

cmd >/dev/null 2>&1
来源：http://gsj.quarkkingdee.top

[R42] 输入重定向
来源：http://qpj.hysaishi.cn

wc -l < a.txt
来源：http://tnt.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://ngg.cdnleiting.top

find . -name "*.log" -type f
来源：http://die.yueranfly.top

[R44] 按修改时间查找
来源：http://cbf.daxiang520.top

find . -mtime -7 -type f
来源：http://drk.uphjek.com

[R45] 批量删除
来源：http://wxt.sysykeji.top

find . -name "*.tmp" -delete
来源：http://soh.ydzc1.top

[R46] 递归替换文件内容
来源：http://wgl.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hdf.shzxlz.cn

[R47] sed 单行替换
来源：http://kmu.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xqv.zhijiandao.cn

[R48] awk 取指定列
来源：http://qvz.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://elh.cheryme.top

[R49] awk 带条件
来源：http://qfk.xinyue.icu


<!-- 参考信息 -->