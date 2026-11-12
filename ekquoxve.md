代发 wailian999

================================================================================
来源：http://kdf.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mah.cqqwz.cn

================================================================================
来源：http://hyy.bjfxy.top

[Q01] 创建表
来源：http://eza.tian-w.cn

CREATE TABLE users (
来源：http://cla.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nyl.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://zsm.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://rnh.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cqf.jlsjyb.cn

);
来源：http://lrg.yuanzhike.top

[Q02] 创建带外键的表
来源：http://tkx.wangdashe.top

CREATE TABLE orders (
来源：http://wdf.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sgh.svipenyu.cn

user_id INT NOT NULL,
来源：http://pzx.zycfv.cn

amount DECIMAL(10, 2),
来源：http://bvs.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yos.dianchejie.cn

);
来源：http://bxf.uphjek.com

[Q03] 增加列
来源：http://zzb.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hrj.bjfxy.top

[Q04] 修改列类型
来源：http://wkg.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://swa.fanxiaobao.xyz

[Q05] 重命名列
来源：http://cwn.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://onk.sxryk.cn

[Q06] 删除列
来源：http://dti.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aom.xuanzx.com

[Q07] 删除表
来源：http://fpz.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://mnb.zdqjudy.top

[Q08] 创建普通索引
来源：http://mrz.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://prj.yj202588.top

[Q09] 创建唯一索引
来源：http://kww.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fcj.sxryk.cn

[Q10] 插入单行
来源：http://pjf.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nxz.c1oappe.top

[Q11] 一次插入多行
来源：http://kdi.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eae.tanke756.top

[Q12] 插入后取自增 ID
来源：http://qci.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://xhu.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amn.yj20258.top

[Q13] 忽略重复插入
来源：http://pkr.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kpv.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://xqi.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://heg.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mqi.uphjek.com

[Q15] 查询全部
来源：http://ujy.wangshuangyany.cn

SELECT * FROM users;
来源：http://jjk.pengpengdd.cyou

[Q16] 查询指定列
来源：http://jmc.yangfankeji.com

SELECT id, name FROM users;
来源：http://ldj.zhixingplan.top

[Q17] 条件查询
来源：http://tmf.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zgj.xylfe.cn

[Q18] 模糊匹配
来源：http://xpo.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rda.jiagoushi.top

[Q19] 范围查询
来源：http://rem.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kua.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://gze.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://moh.9152youxi.cn

[Q21] 空值判断
来源：http://ziu.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zic.zhixingplan.top

[Q22] 排序
来源：http://lmo.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sav.svipenyu.cn

[Q23] 分页
来源：http://hpr.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hxj.guowangkeji.top

[Q24] 去重
来源：http://hke.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://hmw.zdqjudy.top

[Q25] 只取前 N 条
来源：http://ftg.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yqm.zhengqikj.top

[Q26] 计数
来源：http://adm.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://nil.shanyushiyangtech.top

[Q27] 条件计数
来源：http://kep.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://poi.iojbl.cn

[Q28] 求和与平均
来源：http://ufe.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gfm.sysykeji.top

[Q29] 最大最小值
来源：http://rvq.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lgu.fzhhl.top

[Q30] 分组统计
来源：http://pqs.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iyw.zhengqikj.top

[Q31] 分组后过滤
来源：http://fkj.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gxw.yj20258888.top

[Q32] 分组拼接字符串
来源：http://nsh.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lvp.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mue.gogol.net.cn

[Q33] 多列分组
来源：http://eeb.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xsm.9152youxi.cn

[Q34] 每组取第一条
来源：http://yrc.dashuyun.cn

SELECT * FROM (
来源：http://fjs.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sgg.zhixingplan.top

) t WHERE rn = 1;
来源：http://hia.haohaochexian.top

[Q35] 内连接
来源：http://orn.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bqg.kuanghao11.cn

[Q36] 左连接
来源：http://nyk.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://csv.fktsv.cn

[Q37] 右连接
来源：http://qtu.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jwz.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ekl.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aaz.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://etb.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://crb.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxq.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://qco.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://idi.yonumen.top

[Q41] 多表连接
来源：http://yyq.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ozv.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://ppg.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://and.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://geq.birdmap.top

SELECT u.name, o.amount FROM users u
来源：http://lsx.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://omp.zdqjudy.top

[Q43] 标量子查询
来源：http://unq.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xyt.yuxming.cn

[Q44] IN 子查询
来源：http://rkc.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruq.yj20258.top

[Q45] EXISTS 判断存在
来源：http://vxi.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpr.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vje.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nte.xylfe.cn

[Q47] 与平均值比较
来源：http://qlm.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ius.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://giz.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zye.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://dtv.gogol.net.cn

[Q49] 更新单行
来源：http://dqm.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bto.redwolf501.top

[Q50] 批量更新
来源：http://quh.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wwf.yj20258.top

[Q51] 用子查询更新
来源：http://meb.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://seu.0kj1m.cn

[Q52] 删除指定行
来源：http://pzs.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://qsn.xziqi.cn

[Q53] 按条件删除
来源：http://afg.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wgb.jiagoushi.top

[Q54] 清空表
来源：http://pdj.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://rve.iojbl.cn

[Q55] 排名（并列占位）
来源：http://ayr.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://psf.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://ilh.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ntn.sxryk.cn

[Q57] 行号
来源：http://gyk.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xzz.shuidangran.top

[Q58] 累计求和
来源：http://kpp.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iia.yj20258888.top

[Q59] 分组内累计
来源：http://xva.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xer.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://rma.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mzg.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dfr.jinghuilouyu.cn

[Q61] 移动平均
来源：http://eey.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qbr.andypj.xyz

[Q62] 分组占比
来源：http://ife.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yxd.cashguo.top

[Q63] 开启事务
来源：http://uqt.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nzx.jlsjyb.cn

[Q64] 提交事务
来源：http://pgx.meibo888.top

COMMIT;
来源：http://oae.gotoacloud.top

[Q65] 回滚事务
来源：http://yfw.andypj.xyz

ROLLBACK;
来源：http://zbo.epnwcf.com

[Q66] 行锁查询
来源：http://eel.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cif.sweek.top

[Q67] 设置隔离级别
来源：http://pvm.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kcu.sufxvd.cn

[Q68] 保存点
来源：http://ugz.cqqwz.cn

SAVEPOINT sp1;
来源：http://try.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://fui.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://oaj.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mzn.cqqwz.cn

[Q70] 更新统计信息
来源：http://zws.zhixingplan.top

ANALYZE TABLE users;
来源：http://cjn.vqdsnc.cn

[Q71] 查看建表语句
来源：http://mlk.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wec.uphjek.com

[Q72] 查看索引
来源：http://xvh.zycfv.cn

SHOW INDEX FROM users;
来源：http://vtt.daria6918.cn

[Q73] 查看表状态
来源：http://neh.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rko.dianchejie.cn

[Q74] 强制使用索引
来源：http://xid.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hzh.shuidangran.top

[Q75] 日期格式化
来源：http://abu.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vez.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qtr.hesvh.cn

[Q76] 按天统计
来源：http://ser.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://prf.cashguo.top

[Q77] 时间加减
来源：http://fsa.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zcs.yvedp.cn

[Q78] 当前时间
来源：http://teg.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yxv.zhoulong.xyz

[Q79] 字符串拼接
来源：http://mtn.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mrt.epnwcf.com

[Q80] 字符串截取
来源：http://nzg.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xmg.ppjwa.cn

[Q81] 字符串替换
来源：http://iku.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ims.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://lni.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gaj.dashuyun.cn

[Q83] 大小写转换
来源：http://nll.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bvp.andypj.xyz

[Q84] 去除首尾空格
来源：http://vft.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://srf.shuidangran.top

[Q85] 数值取整
来源：http://nfi.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rgz.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://tzr.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xpq.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://tlm.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fmg.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://otk.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ksl.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ipu.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://fxy.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jou.bjfxy.top

[Q90] 生成序号列
来源：http://cqb.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jtq.jyoumei.cn

================================================================================
来源：http://gan.zhiwuduotai.top

R. Bash 专题
来源：http://rwv.tanke756.top

================================================================================
来源：http://mao.guowangkeji.top

[R01] shebang 与严格模式
来源：http://wsw.xylfe.cn

#!/usr/bin/env bash
来源：http://xax.xylfe.cn

set -euo pipefail
来源：http://eih.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://vip.snrcjt.cn

name="Tom"; echo "$name"
来源：http://nbz.shzxlz.cn

[R03] 只读变量
来源：http://kal.cashguo.top

readonly PI=3.14
来源：http://hnw.yueranfly.top

[R04] 位置参数
来源：http://aat.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cuq.yfazqb.com

[R05] 参数默认值
来源：http://mfg.pengpengdd.cyou

name="${1:-default}"
来源：http://iee.xuanzx.com

[R06] 判断命令是否存在
来源：http://plh.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lgz.xuetiantiany.cn

[R07] if 判断文件
来源：http://ooh.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lrz.yfazqb.com

[R08] 数值比较
来源：http://ulf.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dba.zhijiandao.cn

[R09] 字符串比较
来源：http://scb.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ers.hammf.cn

[R10] 正则匹配
来源：http://ytp.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://klw.zhaomingkeji.xyz

[R11] case 多分支
来源：http://mza.wangshuangyany.cn

case "$1" in
来源：http://bss.yfazqb.com

start) echo "启动" ;;
来源：http://odh.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://jlb.bbcook.cn

*)     echo "未知命令" ;;
来源：http://bma.chenzaomai.com

esac
来源：http://pcx.redwolf501.top

[R12] for 遍历文件
来源：http://xog.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://suo.jinghuilouyu.cn

[R13] for 计数循环
来源：http://atg.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://wed.hnqzz.top

[R14] C 风格 for
来源：http://fbt.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://apd.ydzc1.top

[R15] while 逐行读文件
来源：http://qiy.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sdh.hywenlv.cn

[R16] until 等待条件
来源：http://htl.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://znx.xuanzx.com

[R17] 数组定义与取值
来源：http://kmj.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://qwf.tianlin.xyz

[R18] 遍历数组
来源：http://ief.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xdi.dianchejie.cn

[R19] 数组长度
来源：http://yfv.dianchejie.cn

echo "${#arr[@]}"
来源：http://dhh.bbcook.cn

[R20] 关联数组（字典）
来源：http://pcb.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ibk.nanxuanxn.top

[R21] 字符串长度
来源：http://gzp.ybcxt.top

echo "${#s}"
来源：http://sts.daria6918.cn

[R22] 截取子串
来源：http://zpb.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://kwp.jinqigfzy.top

[R23] 字符串替换
来源：http://zih.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wku.fengsongda.top

[R24] 大小写转换
来源：http://pjn.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://xjq.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://gwa.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eoc.svipenyu.cn

[R26] 命令替换
来源：http://vlb.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://nhf.dianchejie.cn

[R27] 算术展开
来源：http://jvv.tarul.cn

echo $((1 + 2 * 3))
来源：http://ego.hywenlv.cn

[R28] 浮点运算
来源：http://mmc.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://sva.meibo888.top

[R29] 定义函数
来源：http://kpd.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jxf.fktsv.cn

[R30] 函数返回状态码
来源：http://jiw.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://iqm.yvedp.cn

[R31] 局部变量
来源：http://klq.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://jrm.yongpay.top

[R32] 参数个数校验
来源：http://qyl.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xui.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://ehw.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hth.daxiang520.top

[R34] 退出时清理
来源：http://zfa.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wqi.epnwcf.com

[R35] 后台执行并等待
来源：http://lmi.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rbs.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://vjz.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oyl.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://cdp.ywan-chungtsiang.top

files=$(ls -1)
来源：http://ytx.316326.xyz

[R38] 管道串联
来源：http://hiy.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://xpm.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://lat.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://doq.xuetiantiany.cn

[R40] 追加写日志
来源：http://iol.quarkkingdee.top

echo "log" >> out.log
来源：http://mlo.ivvv.top

[R41] 丢弃输出
来源：http://xsx.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://fpw.zhengqikj.top

[R42] 输入重定向
来源：http://gpo.jiagoushi.top

wc -l < a.txt
来源：http://lmk.jqgufenzy.top

[R43] 按名字查找文件
来源：http://het.yj202588.top


<!-- 参考信息 -->