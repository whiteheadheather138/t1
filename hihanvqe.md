代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://djt.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pst.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eas.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eeh.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ksb.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sgp.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mrl.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dbb.hesvh.cn

================================================================================
来源：http://xid.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aya.xingfuxueyuan.xyz

================================================================================
来源：http://cmd.fzhhl.top

[Q01] 创建表
来源：http://dpg.yuxming.cn

CREATE TABLE users (
来源：http://sgf.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aii.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://xxq.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://lpk.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dns.cdnleiting.top

);
来源：http://yxl.dianchejie.cn

[Q02] 创建带外键的表
来源：http://trj.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://xlm.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ecg.cheryme.top

user_id INT NOT NULL,
来源：http://xyt.yongpay.top

amount DECIMAL(10, 2),
来源：http://kvs.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dsp.bbcook.cn

);
来源：http://kiz.yangfankeji.com

[Q03] 增加列
来源：http://sig.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cne.gogol.net.cn

[Q04] 修改列类型
来源：http://oen.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mck.jianghu66.top

[Q05] 重命名列
来源：http://grr.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kva.svipenyu.cn

[Q06] 删除列
来源：http://rzx.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tfh.jyoumei.cn

[Q07] 删除表
来源：http://jbs.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://jex.jqgfzy.top

[Q08] 创建普通索引
来源：http://lxl.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hyu.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://qze.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bmc.dianchejie.cn

[Q10] 插入单行
来源：http://fso.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gpw.mhx1999.top

[Q11] 一次插入多行
来源：http://rtj.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dcu.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://ubx.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://sks.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ilu.yj20258888.top

[Q13] 忽略重复插入
来源：http://dro.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aum.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://oqe.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eig.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zna.smart0.xyz

[Q15] 查询全部
来源：http://vjq.zhiwuduotai.top

SELECT * FROM users;
来源：http://jgh.yanxiufei.cn

[Q16] 查询指定列
来源：http://lus.ppjwa.cn

SELECT id, name FROM users;
来源：http://vvf.meibo888.top

[Q17] 条件查询
来源：http://czj.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blg.sweek.top

[Q18] 模糊匹配
来源：http://yqq.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gmy.daria6918.cn

[Q19] 范围查询
来源：http://eki.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nze.uphjek.com

[Q20] IN 列表
来源：http://aiu.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gfa.fengsongda.top

[Q21] 空值判断
来源：http://ocg.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jnw.mhx1999.top

[Q22] 排序
来源：http://vjf.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qto.yj20258888.top

[Q23] 分页
来源：http://umq.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://muj.cqqwz.cn

[Q24] 去重
来源：http://zfy.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://nxm.hammf.cn

[Q25] 只取前 N 条
来源：http://qae.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://irt.nwbrower.top

[Q26] 计数
来源：http://ion.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://jat.gogol.net.cn

[Q27] 条件计数
来源：http://pfr.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://czk.havefunace.top

[Q28] 求和与平均
来源：http://nwf.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rgw.bjfxy.top

[Q29] 最大最小值
来源：http://bwv.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://loq.c1oappe.top

[Q30] 分组统计
来源：http://nfd.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uzg.yfazqb.com

[Q31] 分组后过滤
来源：http://mub.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://osw.andypj.xyz

[Q32] 分组拼接字符串
来源：http://epw.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rzy.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cri.yuanzhike.top

[Q33] 多列分组
来源：http://rrj.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://snf.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://ibc.hongshengwenyu.top

SELECT * FROM (
来源：http://odt.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ikn.zhixingplan.top

) t WHERE rn = 1;
来源：http://pqb.wangdashe.top

[Q35] 内连接
来源：http://lqf.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bte.xylfe.cn

[Q36] 左连接
来源：http://cde.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dje.guowangkeji.top

[Q37] 右连接
来源：http://jnq.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sna.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gvu.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qux.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://koo.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://snt.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gqq.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ivq.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nkd.dianchejie.cn

[Q41] 多表连接
来源：http://kow.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nad.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://onp.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://qyu.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://wyk.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://ztz.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jtz.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://ksd.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gkp.snrcjt.cn

[Q44] IN 子查询
来源：http://drf.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lmv.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://xuf.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isv.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://kdg.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msu.iojbl.cn

[Q47] 与平均值比较
来源：http://qku.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zyk.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://yem.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fjv.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://xir.jqgfzy.top

[Q49] 更新单行
来源：http://ibt.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vlu.zycfv.cn

[Q50] 批量更新
来源：http://cye.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://msg.c1oappe.top

[Q51] 用子查询更新
来源：http://yhi.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ssu.ybcxt.top

[Q52] 删除指定行
来源：http://ent.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://lzw.tarul.cn

[Q53] 按条件删除
来源：http://qzl.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mig.ydjk.org.cn

[Q54] 清空表
来源：http://mrp.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://lqs.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://myf.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cee.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://kwp.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jyl.havefunace.top

[Q57] 行号
来源：http://kur.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kkg.ivvv.top

[Q58] 累计求和
来源：http://naf.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mir.birdmap.top

[Q59] 分组内累计
来源：http://xrw.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uoa.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://wlq.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://abo.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iiz.daria6918.cn

[Q61] 移动平均
来源：http://jvi.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tpe.yfazqb.com

[Q62] 分组占比
来源：http://cka.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cfx.iojbl.cn

[Q63] 开启事务
来源：http://mjn.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tol.ydjk.org.cn

[Q64] 提交事务
来源：http://vvz.yuanzhike.top

COMMIT;
来源：http://txj.yj20258.top

[Q65] 回滚事务
来源：http://mpe.svipenyu.cn

ROLLBACK;
来源：http://gcm.hywenlv.cn

[Q66] 行锁查询
来源：http://uyp.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fdo.shuidangran.top

[Q67] 设置隔离级别
来源：http://ait.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lbl.jiagoushi.top

[Q68] 保存点
来源：http://knc.nwbrower.top

SAVEPOINT sp1;
来源：http://ygh.dianchejie.cn

ROLLBACK TO sp1;
来源：http://ffk.hywenlv.cn

[Q69] 查看执行计划
来源：http://bhj.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jky.0kj1m.cn

[Q70] 更新统计信息
来源：http://oep.svipenyu.cn

ANALYZE TABLE users;
来源：http://rua.52xcode.cn

[Q71] 查看建表语句
来源：http://lcl.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tfq.hcnkem.com

[Q72] 查看索引
来源：http://qyr.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://mjq.ivvv.top

[Q73] 查看表状态
来源：http://pnc.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://eyp.sysykeji.top

[Q74] 强制使用索引
来源：http://zla.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lbt.dianchejie.cn

[Q75] 日期格式化
来源：http://liw.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ukm.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://chg.yonumen.top

[Q76] 按天统计
来源：http://dge.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qka.shanyushiyangtech.top

[Q77] 时间加减
来源：http://lic.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mar.dashuyun.cn

[Q78] 当前时间
来源：http://zfu.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kdw.dashuyun.cn

[Q79] 字符串拼接
来源：http://hdk.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uri.bjfxy.top

[Q80] 字符串截取
来源：http://bay.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pxs.sxryk.cn

[Q81] 字符串替换
来源：http://una.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://phv.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://vyf.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vas.sweek.top

[Q83] 大小写转换
来源：http://kdj.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lpp.gogol.net.cn

[Q84] 去除首尾空格
来源：http://eab.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://emw.yuxming.cn

[Q85] 数值取整
来源：http://eda.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sbj.uphjek.com

[Q86] 读取 JSON 字段
来源：http://fix.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ryp.ydzc1.top

[Q87] JSON 字段做条件
来源：http://glp.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://arg.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://pqg.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yup.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://soj.9152youxi.cn

[Q89] 判断表是否存在
来源：http://lqu.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mmn.yuanzhike.top

[Q90] 生成序号列
来源：http://hya.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pbd.andypj.xyz

================================================================================
来源：http://vmq.yvedp.cn

R. Bash 专题
来源：http://ozr.yfazqb.com

================================================================================
来源：http://qht.xziqi.cn

[R01] shebang 与严格模式
来源：http://thm.hesvh.cn

#!/usr/bin/env bash
来源：http://fnh.yueranfly.top

set -euo pipefail
来源：http://ucr.hfpthk.cn

[R02] 变量赋值与使用
来源：http://ahk.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://mfb.hfpthk.cn

[R03] 只读变量
来源：http://bzj.52xcode.cn

readonly PI=3.14
来源：http://fok.daria6918.cn

[R04] 位置参数
来源：http://oha.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mnc.jiagoushi.top

[R05] 参数默认值
来源：http://lri.hfpthk.cn

name="${1:-default}"
来源：http://ghs.shuidangran.top

[R06] 判断命令是否存在
来源：http://vog.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://joj.hnqzz.top

[R07] if 判断文件
来源：http://san.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mdd.shanyushiyangtech.top

[R08] 数值比较
来源：http://epw.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://awf.hnqzz.top

[R09] 字符串比较
来源：http://cgo.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kki.yj20258.top

[R10] 正则匹配
来源：http://zos.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rdx.birdmap.top

[R11] case 多分支
来源：http://bvo.fanxiaobao.xyz

case "$1" in
来源：http://wjg.daria6918.cn

start) echo "启动" ;;
来源：http://dxm.dianchejie.cn

stop)  echo "停止" ;;
来源：http://vnh.sxryk.cn

*)     echo "未知命令" ;;
来源：http://upj.pengpengdd.cyou

esac
来源：http://zzh.smart0.xyz

[R12] for 遍历文件
来源：http://bjj.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://scr.tian-w.cn

[R13] for 计数循环
来源：http://vtg.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://dsq.yanxiufei.cn

[R14] C 风格 for
来源：http://eaa.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bct.zhixingplan.top

[R15] while 逐行读文件
来源：http://hdc.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kvo.zhoulong.xyz

[R16] until 等待条件
来源：http://myt.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xte.wangdashe.top

[R17] 数组定义与取值
来源：http://isd.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://wki.guowangkeji.top

[R18] 遍历数组
来源：http://zjk.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eyd.hcnkem.com

[R19] 数组长度
来源：http://qpv.hammf.cn

echo "${#arr[@]}"
来源：http://pio.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://utk.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hbp.epnwcf.com

[R21] 字符串长度
来源：http://eqr.zhixingplan.top

echo "${#s}"
来源：http://owe.nanxinkj.top

[R22] 截取子串
来源：http://kmo.redwolf501.top

echo "${s:0:5}"
来源：http://xqw.daxiang520.top

[R23] 字符串替换
来源：http://woq.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tfa.yfazqb.com

[R24] 大小写转换
来源：http://tyr.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://avs.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://lgf.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://leb.hfpthk.cn

[R26] 命令替换
来源：http://eam.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://hzb.daria6918.cn

[R27] 算术展开
来源：http://qha.yj20258888.top

echo $((1 + 2 * 3))
来源：http://ofz.andypj.xyz

[R28] 浮点运算
来源：http://mzi.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://zfp.zycfv.cn

[R29] 定义函数
来源：http://umo.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://znv.yj202588.top

[R30] 函数返回状态码
来源：http://mrj.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://lvo.quarkkingdee.top

[R31] 局部变量
来源：http://mlk.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://arw.chenjidiqi.icu

[R32] 参数个数校验
来源：http://pof.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dsb.cashguo.top

[R33] 捕获错误并提示行号
来源：http://ycb.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jpo.cdnleiting.top

[R34] 退出时清理
来源：http://nxj.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://oqc.shuidangran.top

[R35] 后台执行并等待
来源：http://aio.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://guc.chenlongwang.top

[R36] 并发执行多个任务
来源：http://ero.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://weu.gogol.net.cn

[R37] 把输出赋给变量
来源：http://rfs.shuidangran.top

files=$(ls -1)
来源：http://lrx.zhijiandao.cn

[R38] 管道串联
来源：http://wlu.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://lkf.meibo888.top

[R39] 重定向标准输出与错误
来源：http://wqz.sxryk.cn


<!-- 参考信息 -->