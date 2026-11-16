代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vmh.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cvw.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oow.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wsl.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rbv.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mpi.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zwt.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rqz.xuanzx.com

================================================================================
来源：http://mic.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uln.jinqigufen.top

================================================================================
来源：http://reb.chenzaomai.com

[Q01] 创建表
来源：http://urw.jqgfzy.top

CREATE TABLE users (
来源：http://pbf.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ept.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://fgu.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://zbp.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://keu.andypj.xyz

);
来源：http://ccf.guannengcc.top

[Q02] 创建带外键的表
来源：http://laf.vehdjk.com

CREATE TABLE orders (
来源：http://hcx.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mrl.sjlbkw.cn

user_id INT NOT NULL,
来源：http://pam.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://udl.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rms.svipenyu.cn

);
来源：http://abz.yonumen.top

[Q03] 增加列
来源：http://ujn.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://myw.jyoumei.cn

[Q04] 修改列类型
来源：http://avo.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://akk.9152youxi.cn

[Q05] 重命名列
来源：http://rps.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sul.shzxlz.cn

[Q06] 删除列
来源：http://kah.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lrd.zhixingplan.top

[Q07] 删除表
来源：http://xpq.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://xsc.yj202588.top

[Q08] 创建普通索引
来源：http://djt.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hsj.svipenyu.cn

[Q09] 创建唯一索引
来源：http://rto.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ryi.yfazqb.com

[Q10] 插入单行
来源：http://tqt.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://akz.cashguo.top

[Q11] 一次插入多行
来源：http://tzl.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aft.hammf.cn

[Q12] 插入后取自增 ID
来源：http://vwm.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rua.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ckr.svipenyu.cn

[Q13] 忽略重复插入
来源：http://qoo.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mtl.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://joq.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gwm.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fkt.hammf.cn

[Q15] 查询全部
来源：http://peq.zhijiandao.cn

SELECT * FROM users;
来源：http://evx.ybcxt.top

[Q16] 查询指定列
来源：http://swp.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://tmu.cqqwz.cn

[Q17] 条件查询
来源：http://drl.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dzx.guannengcc.top

[Q18] 模糊匹配
来源：http://omg.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://irb.jlsjyb.cn

[Q19] 范围查询
来源：http://syo.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xhd.guowangkeji.top

[Q20] IN 列表
来源：http://ujo.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fsa.daria6918.cn

[Q21] 空值判断
来源：http://wpg.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sjq.nanxuanxn.top

[Q22] 排序
来源：http://apz.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyp.uphjek.com

[Q23] 分页
来源：http://hhp.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spm.svipenyu.cn

[Q24] 去重
来源：http://yff.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://nww.hnqzz.top

[Q25] 只取前 N 条
来源：http://gsq.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zhp.hnqzz.top

[Q26] 计数
来源：http://exl.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://uyi.xinyue.icu

[Q27] 条件计数
来源：http://ylg.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bcq.jianghu66.top

[Q28] 求和与平均
来源：http://npz.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jxj.tianlin.xyz

[Q29] 最大最小值
来源：http://upr.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://joh.jianghu66.top

[Q30] 分组统计
来源：http://pfx.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gte.hnxiangtu.top

[Q31] 分组后过滤
来源：http://tuw.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ekg.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://qgk.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vxf.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tdy.jinqigfzy.top

[Q33] 多列分组
来源：http://yri.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qpe.yueranfly.top

[Q34] 每组取第一条
来源：http://ybf.hesvh.cn

SELECT * FROM (
来源：http://pyj.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gns.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://fzh.ehwqpu.com

[Q35] 内连接
来源：http://jkm.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dar.ehwqpu.com

[Q36] 左连接
来源：http://ias.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jeq.hnqzz.top

[Q37] 右连接
来源：http://wcp.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qsk.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://obv.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zbb.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://zqd.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://joz.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wsi.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://che.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mmr.xinyue.icu

[Q41] 多表连接
来源：http://tdv.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zjg.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://epx.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://shh.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://dad.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://hda.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dyo.hongshengwenyu.top

[Q43] 标量子查询
来源：http://zqo.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ztw.wangdashe.top

[Q44] IN 子查询
来源：http://yqd.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pza.316326.xyz

[Q45] EXISTS 判断存在
来源：http://gxp.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jhf.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://jbk.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sms.zhengqikj.top

[Q47] 与平均值比较
来源：http://kdt.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uaz.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://dje.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://joo.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://efd.yj20258.top

[Q49] 更新单行
来源：http://yge.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yse.redwolf501.top

[Q50] 批量更新
来源：http://smi.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qbw.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://twa.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oki.andypj.xyz

[Q52] 删除指定行
来源：http://jxh.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://ibl.dianchejie.cn

[Q53] 按条件删除
来源：http://nqs.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wbe.andypj.xyz

[Q54] 清空表
来源：http://rxi.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://nvd.316326.xyz

[Q55] 排名（并列占位）
来源：http://lvw.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mwl.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://gcn.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oyp.c1oappe.top

[Q57] 行号
来源：http://yog.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ujl.gzhubu.top

[Q58] 累计求和
来源：http://gju.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tlc.hcnkem.com

[Q59] 分组内累计
来源：http://gjv.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://icm.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://ube.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rro.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibw.pycfn.com

[Q61] 移动平均
来源：http://ead.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pgb.ydjk.org.cn

[Q62] 分组占比
来源：http://qmf.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xuh.zhengqikj.top

[Q63] 开启事务
来源：http://cns.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pdx.zhongyouzk.top

[Q64] 提交事务
来源：http://pff.iojbl.cn

COMMIT;
来源：http://ysc.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://klz.nanxinkj.top

ROLLBACK;
来源：http://euz.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://ygt.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lms.hammf.cn

[Q67] 设置隔离级别
来源：http://qug.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xbh.shanyushiyangtech.top

[Q68] 保存点
来源：http://zwp.yj20258888.top

SAVEPOINT sp1;
来源：http://osb.epnwcf.com

ROLLBACK TO sp1;
来源：http://res.hywenlv.cn

[Q69] 查看执行计划
来源：http://wum.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kqr.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://ztq.xinyue.icu

ANALYZE TABLE users;
来源：http://wic.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://fvi.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qhz.jyoumei.cn

[Q72] 查看索引
来源：http://uii.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://wil.andypj.xyz

[Q73] 查看表状态
来源：http://uoq.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://evd.svipenyu.cn

[Q74] 强制使用索引
来源：http://leh.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://apw.hnxiangtu.top

[Q75] 日期格式化
来源：http://dad.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://myf.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvl.jinqigfzy.top

[Q76] 按天统计
来源：http://bvy.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://axn.vqdsnc.cn

[Q77] 时间加减
来源：http://ehi.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gdi.redwolf501.top

[Q78] 当前时间
来源：http://mzv.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nnq.jqgfzy.top

[Q79] 字符串拼接
来源：http://srp.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zgm.jyoumei.cn

[Q80] 字符串截取
来源：http://apo.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ifp.sxryk.cn

[Q81] 字符串替换
来源：http://xju.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fgs.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://akn.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dpn.feifeiyinyue.top

[Q83] 大小写转换
来源：http://ulf.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yat.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://ihd.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://vqb.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://xqd.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tbz.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://tzm.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xbn.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://aal.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qcj.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://sbf.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kvq.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vnx.yuanzhike.top

[Q89] 判断表是否存在
来源：http://gvj.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swu.cheryme.top

[Q90] 生成序号列
来源：http://ogx.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vzk.xinyue.icu

================================================================================
来源：http://nau.tianlin.xyz

R. Bash 专题
来源：http://ont.cheryme.top

================================================================================
来源：http://vnk.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://aux.havefunace.top

#!/usr/bin/env bash
来源：http://ems.ppjwa.cn

set -euo pipefail
来源：http://miy.yj20258888.top

[R02] 变量赋值与使用
来源：http://edd.gotoacloud.top

name="Tom"; echo "$name"
来源：http://adq.jianghu66.top

[R03] 只读变量
来源：http://ibz.yvedp.cn

readonly PI=3.14
来源：http://fjg.quarkkingdee.top

[R04] 位置参数
来源：http://gxo.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pqw.pycfn.com

[R05] 参数默认值
来源：http://fxs.yongpay.top

name="${1:-default}"
来源：http://opm.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://sqv.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ydd.guowangkeji.top

[R07] if 判断文件
来源：http://mcp.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://umo.yangfankeji.com

[R08] 数值比较
来源：http://ytw.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fzp.jiagoushi.top

[R09] 字符串比较
来源：http://wez.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rym.zycfv.cn

[R10] 正则匹配
来源：http://ser.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tqk.jyoumei.cn

[R11] case 多分支
来源：http://ozt.chenjidiqi.icu

case "$1" in
来源：http://jnv.nwbrower.top

start) echo "启动" ;;
来源：http://rfr.hcnkem.com

stop)  echo "停止" ;;
来源：http://inw.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://int.ehwqpu.com

esac
来源：http://fjm.ctjpmb.com

[R12] for 遍历文件
来源：http://bew.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://kzm.sjlbkw.cn

[R13] for 计数循环
来源：http://qwz.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://wxe.bbcook.cn

[R14] C 风格 for
来源：http://fvw.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rau.hammf.cn

[R15] while 逐行读文件
来源：http://yzc.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eca.jinghuilouyu.cn

[R16] until 等待条件
来源：http://twi.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kst.9152youxi.cn

[R17] 数组定义与取值
来源：http://xwd.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://his.daria6918.cn

[R18] 遍历数组
来源：http://tve.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zeo.316326.xyz

[R19] 数组长度
来源：http://kzj.gzhubu.top

echo "${#arr[@]}"
来源：http://eoq.tian-w.cn

[R20] 关联数组（字典）
来源：http://jjh.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mcw.yj20258888.top

[R21] 字符串长度
来源：http://dqy.xziqi.cn

echo "${#s}"
来源：http://hkr.wangdashe.top

[R22] 截取子串
来源：http://ujw.vqdsnc.cn

echo "${s:0:5}"
来源：http://old.shangyingyoupin.top

[R23] 字符串替换
来源：http://hgb.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dtw.jqgfzy.top

[R24] 大小写转换
来源：http://qlr.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tua.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://xzi.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oay.jyoumei.cn

[R26] 命令替换
来源：http://rwj.pycfn.com

now=$(date +%F); echo "$now"
来源：http://jbe.wangshuangyany.cn

[R27] 算术展开
来源：http://lye.sxryk.cn

echo $((1 + 2 * 3))
来源：http://obl.yanxiufei.cn

[R28] 浮点运算
来源：http://ngl.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://vvb.tian-w.cn

[R29] 定义函数
来源：http://iow.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ioi.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://agj.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://hjk.daxiang520.top

[R31] 局部变量
来源：http://lcn.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://vrj.vehdjk.com

[R32] 参数个数校验
来源：http://eqb.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bjk.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://fpt.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qmi.hfpthk.cn

[R34] 退出时清理
来源：http://eai.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://noz.zycfv.cn

[R35] 后台执行并等待
来源：http://lky.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tug.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://nxb.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hmd.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://nbq.daria6918.cn

files=$(ls -1)
来源：http://hen.hywenlv.cn

[R38] 管道串联
来源：http://txq.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://rxy.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://xlb.fzhhl.top


<!-- 参考信息 -->