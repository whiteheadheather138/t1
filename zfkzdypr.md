代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wvl.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwy.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oww.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xhm.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hsk.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wns.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uld.cashguo.top

[P08] 处理浮点精度问题
来源：http://gzr.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pjp.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rfx.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ipb.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sdz.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vrt.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nuo.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jgb.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wfb.vehdjk.com

================================================================================
来源：http://pnc.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://voa.gzhubu.top

================================================================================
来源：http://iax.zhiwuduotai.top

[Q01] 创建表
来源：http://stj.zhiwuduotai.top

CREATE TABLE users (
来源：http://vzr.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zmd.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://itz.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://rip.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cmn.jyoumei.cn

);
来源：http://xyd.shuidangran.top

[Q02] 创建带外键的表
来源：http://cqo.tian-w.cn

CREATE TABLE orders (
来源：http://qze.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyj.jiagoushi.top

user_id INT NOT NULL,
来源：http://ecw.iojbl.cn

amount DECIMAL(10, 2),
来源：http://evj.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iiw.zhongyouzk.top

);
来源：http://pdq.hywenlv.cn

[Q03] 增加列
来源：http://tfm.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hpq.xuetiantiany.cn

[Q04] 修改列类型
来源：http://opq.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uap.316326.xyz

[Q05] 重命名列
来源：http://zbs.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mdf.zhiwuduotai.top

[Q06] 删除列
来源：http://jjw.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cnt.quarkkingdee.top

[Q07] 删除表
来源：http://udj.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://din.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://bin.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mbc.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://atd.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gwi.sufxvd.cn

[Q10] 插入单行
来源：http://qpk.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uwa.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://lgr.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pen.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://hmw.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ojh.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrf.hammf.cn

[Q13] 忽略重复插入
来源：http://wrp.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nbo.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://nff.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jcs.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pjr.zhengqikj.top

[Q15] 查询全部
来源：http://nhp.sjlbkw.cn

SELECT * FROM users;
来源：http://cjm.yanxiufei.cn

[Q16] 查询指定列
来源：http://xwm.tanke756.top

SELECT id, name FROM users;
来源：http://osq.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://lig.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://htj.jlsjyb.cn

[Q18] 模糊匹配
来源：http://shr.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://app.guannengcc.top

[Q19] 范围查询
来源：http://yfz.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rkn.dashuyun.cn

[Q20] IN 列表
来源：http://vdc.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hvr.zycfv.cn

[Q21] 空值判断
来源：http://mzm.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mjx.jinghuilouyu.cn

[Q22] 排序
来源：http://uie.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://crq.aizwys.cn

[Q23] 分页
来源：http://imo.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hhi.cheryme.top

[Q24] 去重
来源：http://sji.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://uqk.ivvv.top

[Q25] 只取前 N 条
来源：http://xap.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kvk.chenlongwang.top

[Q26] 计数
来源：http://wui.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://umu.iojbl.cn

[Q27] 条件计数
来源：http://rwz.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ikk.cqqwz.cn

[Q28] 求和与平均
来源：http://qio.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ndv.zhengqikj.top

[Q29] 最大最小值
来源：http://xvo.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nak.snrcjt.cn

[Q30] 分组统计
来源：http://tub.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nhh.tian-w.cn

[Q31] 分组后过滤
来源：http://pev.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nmb.fzhhl.top

[Q32] 分组拼接字符串
来源：http://rba.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ejj.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hak.bbcook.cn

[Q33] 多列分组
来源：http://tmf.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://teg.cdnleiting.top

[Q34] 每组取第一条
来源：http://jcr.jlsjyb.cn

SELECT * FROM (
来源：http://yyp.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mpw.andypj.xyz

) t WHERE rn = 1;
来源：http://bho.yuxming.cn

[Q35] 内连接
来源：http://zip.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ebk.shanyushiyangkeji.top

[Q36] 左连接
来源：http://jpg.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://asi.aizwys.cn

[Q37] 右连接
来源：http://xky.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xpt.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://jze.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://otf.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://blu.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://csp.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://npm.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fqj.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wga.jqgfzy.top

[Q41] 多表连接
来源：http://hxc.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sje.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://box.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://xnk.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://fis.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://okv.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pgg.xuetiantiany.cn

[Q43] 标量子查询
来源：http://ofe.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://coy.cheryme.top

[Q44] IN 子查询
来源：http://vin.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hzh.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://vsx.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vku.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://eqy.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pao.dianchejie.cn

[Q47] 与平均值比较
来源：http://kbb.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dbk.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://joy.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nqu.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://pqj.316326.xyz

[Q49] 更新单行
来源：http://hyv.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zhx.hammf.cn

[Q50] 批量更新
来源：http://izd.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://taf.svipenyu.cn

[Q51] 用子查询更新
来源：http://cjd.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cxj.yvedp.cn

[Q52] 删除指定行
来源：http://cdw.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://lly.hcnkem.com

[Q53] 按条件删除
来源：http://mfe.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://psk.xziqi.cn

[Q54] 清空表
来源：http://yzp.yuxming.cn

TRUNCATE TABLE logs;
来源：http://yyv.sxryk.cn

[Q55] 排名（并列占位）
来源：http://gka.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uea.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://xiy.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bcq.fzhhl.top

[Q57] 行号
来源：http://cph.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qwe.tarul.cn

[Q58] 累计求和
来源：http://hdn.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jap.ehwqpu.com

[Q59] 分组内累计
来源：http://inz.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ihc.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://mta.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mis.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://snw.hcnkem.com

[Q61] 移动平均
来源：http://ork.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hlk.mhx1999.top

[Q62] 分组占比
来源：http://dve.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sob.quarkkingdee.top

[Q63] 开启事务
来源：http://sjb.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mfc.wangshuangyany.cn

[Q64] 提交事务
来源：http://rzk.cheryme.top

COMMIT;
来源：http://hpt.nwbrower.top

[Q65] 回滚事务
来源：http://srt.jinqigfzy.top

ROLLBACK;
来源：http://asn.fehbvm.com

[Q66] 行锁查询
来源：http://nqv.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uyv.wangdashe.top

[Q67] 设置隔离级别
来源：http://jwl.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ywa.sysykeji.top

[Q68] 保存点
来源：http://epg.nwbrower.top

SAVEPOINT sp1;
来源：http://rbg.ydzc1.top

ROLLBACK TO sp1;
来源：http://ncn.yvedp.cn

[Q69] 查看执行计划
来源：http://aee.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ili.sufxvd.cn

[Q70] 更新统计信息
来源：http://ivb.zhoulong.xyz

ANALYZE TABLE users;
来源：http://xwk.ehwqpu.com

[Q71] 查看建表语句
来源：http://zts.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zfj.9152youxi.cn

[Q72] 查看索引
来源：http://ljt.yj202588.top

SHOW INDEX FROM users;
来源：http://bqb.zhixingplan.top

[Q73] 查看表状态
来源：http://key.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://mno.zhoulong.xyz

[Q74] 强制使用索引
来源：http://ifr.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zau.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://sqw.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mad.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qox.jqgufenzy.top

[Q76] 按天统计
来源：http://emh.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fpu.yanxiufei.cn

[Q77] 时间加减
来源：http://qcw.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nln.tian-w.cn

[Q78] 当前时间
来源：http://ksi.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qxt.tianlin.xyz

[Q79] 字符串拼接
来源：http://yqz.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://swz.c1oappe.top

[Q80] 字符串截取
来源：http://fub.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ndc.haohaochexian.top

[Q81] 字符串替换
来源：http://avv.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mtc.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://sfq.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bdc.zhengqikj.top

[Q83] 大小写转换
来源：http://tju.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://utu.ybcxt.top

[Q84] 去除首尾空格
来源：http://bxr.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://tdk.aizwys.cn

[Q85] 数值取整
来源：http://dvz.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ofu.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://kka.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eid.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://bbd.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vcu.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://fcy.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rvj.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rtq.c1oappe.top

[Q89] 判断表是否存在
来源：http://xvt.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hyp.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://yar.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://chc.9152youxi.cn

================================================================================
来源：http://pno.hesvh.cn

R. Bash 专题
来源：http://rlr.shanyushiyangkeji.top

================================================================================
来源：http://qle.daxiang520.top

[R01] shebang 与严格模式
来源：http://wgz.bbcook.cn

#!/usr/bin/env bash
来源：http://bil.svipenyu.cn

set -euo pipefail
来源：http://lyf.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://ong.316326.xyz

name="Tom"; echo "$name"
来源：http://rne.tian-w.cn

[R03] 只读变量
来源：http://uqr.gzhubu.top

readonly PI=3.14
来源：http://thd.9152youxi.cn

[R04] 位置参数
来源：http://asj.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lpt.yueranfly.top

[R05] 参数默认值
来源：http://hss.tian-w.cn

name="${1:-default}"
来源：http://gjv.52xcode.cn

[R06] 判断命令是否存在
来源：http://bsz.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ozy.shanyushiyangtech.top

[R07] if 判断文件
来源：http://pjd.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nmd.kuanghao11.cn

[R08] 数值比较
来源：http://dlf.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jdb.shzxlz.cn

[R09] 字符串比较
来源：http://sjj.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lug.jinqigfzy.top

[R10] 正则匹配
来源：http://imu.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gmz.iojbl.cn

[R11] case 多分支
来源：http://ybf.gotoacloud.top

case "$1" in
来源：http://iqf.hysaishi.cn

start) echo "启动" ;;
来源：http://lho.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://uqg.daria6918.cn

*)     echo "未知命令" ;;
来源：http://uve.daria6918.cn

esac
来源：http://jjq.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://upk.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://vnm.sysykeji.top

[R13] for 计数循环
来源：http://tyl.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://jyi.ybcxt.top

[R14] C 风格 for
来源：http://ynf.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zap.fehbvm.com

[R15] while 逐行读文件
来源：http://kxa.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cec.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://cxt.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lbk.fehbvm.com

[R17] 数组定义与取值
来源：http://uai.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://bvl.andypj.xyz

[R18] 遍历数组
来源：http://igf.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mwr.svipenyu.cn

[R19] 数组长度
来源：http://fow.yj202588.top

echo "${#arr[@]}"
来源：http://mku.guannengcc.top

[R20] 关联数组（字典）
来源：http://zjk.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kkg.zhijiandao.cn

[R21] 字符串长度
来源：http://vdg.aizwys.cn

echo "${#s}"
来源：http://kll.zhoulong.xyz

[R22] 截取子串
来源：http://gcx.yangfankeji.com

echo "${s:0:5}"
来源：http://zre.yonumen.top

[R23] 字符串替换
来源：http://koq.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ftf.xuanzx.com

[R24] 大小写转换
来源：http://luy.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://mwl.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://smh.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ugn.xziqi.cn

[R26] 命令替换
来源：http://rma.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://jyx.fengsongda.top

[R27] 算术展开
来源：http://ffl.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://rdl.gaohongyu789.top

[R28] 浮点运算
来源：http://jit.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://jug.snrcjt.cn

[R29] 定义函数
来源：http://jus.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tox.aizwys.cn

[R30] 函数返回状态码
来源：http://vuh.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://qgd.snrcjt.cn

[R31] 局部变量
来源：http://psf.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://aat.yvedp.cn

[R32] 参数个数校验
来源：http://oxc.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcm.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://hco.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vqo.bbcook.cn

[R34] 退出时清理
来源：http://ofr.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://yrs.xuanzx.com

[R35] 后台执行并等待
来源：http://fho.316326.xyz


<!-- 参考信息 -->