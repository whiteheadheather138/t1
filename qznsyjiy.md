代发 wailian999

PHP:  // 手写时间戳比较
来源：http://tsa.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kuy.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uoo.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sjx.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://frq.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rgu.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zjy.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://dnw.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fgh.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vlr.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dkx.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kue.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bia.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wnd.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://paf.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qal.daxiang520.top

================================================================================
来源：http://bbe.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dsl.uphjek.com

================================================================================
来源：http://nru.yuanzhike.top

[Q01] 创建表
来源：http://dhg.gogol.net.cn

CREATE TABLE users (
来源：http://anw.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gls.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://zfk.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://ppl.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xwy.kuanghao11.cn

);
来源：http://pyl.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://kjl.zhoulong.xyz

CREATE TABLE orders (
来源：http://onm.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvm.daxiang520.top

user_id INT NOT NULL,
来源：http://lbf.yj20258888.top

amount DECIMAL(10, 2),
来源：http://bcj.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ees.bbcook.cn

);
来源：http://rre.316326.xyz

[Q03] 增加列
来源：http://yrp.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qxd.haohaochexian.top

[Q04] 修改列类型
来源：http://lst.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zwu.aibaodan.cn

[Q05] 重命名列
来源：http://qaw.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fns.bjfxy.top

[Q06] 删除列
来源：http://pwh.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pwp.yvedp.cn

[Q07] 删除表
来源：http://tvu.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://ndg.gzhubu.top

[Q08] 创建普通索引
来源：http://ggj.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://omo.uphjek.com

[Q09] 创建唯一索引
来源：http://xhh.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lha.shzxlz.cn

[Q10] 插入单行
来源：http://nmp.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwt.daxiang520.top

[Q11] 一次插入多行
来源：http://off.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qcf.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://tpl.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://zry.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wkr.hcnkem.com

[Q13] 忽略重复插入
来源：http://jte.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cre.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://ivb.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zpa.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hqq.fktsv.cn

[Q15] 查询全部
来源：http://miq.52xcode.cn

SELECT * FROM users;
来源：http://swe.tian-w.cn

[Q16] 查询指定列
来源：http://knx.shzxlz.cn

SELECT id, name FROM users;
来源：http://ueh.sysykeji.top

[Q17] 条件查询
来源：http://bed.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ata.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://wvl.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://izo.fktsv.cn

[Q19] 范围查询
来源：http://qwc.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rfl.sjlbkw.cn

[Q20] IN 列表
来源：http://cqr.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://koa.ivvv.top

[Q21] 空值判断
来源：http://twx.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ygr.xziqi.cn

[Q22] 排序
来源：http://oaa.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://orc.jinqigufen.top

[Q23] 分页
来源：http://ynu.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bgz.tian-w.cn

[Q24] 去重
来源：http://nzc.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://fag.yj202588.top

[Q25] 只取前 N 条
来源：http://bsp.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wpx.chenlongwang.top

[Q26] 计数
来源：http://ode.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://psy.snrcjt.cn

[Q27] 条件计数
来源：http://tlm.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qpx.haohaochexian.top

[Q28] 求和与平均
来源：http://emx.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zgf.sjlbkw.cn

[Q29] 最大最小值
来源：http://qno.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dhr.jqgufenzy.top

[Q30] 分组统计
来源：http://ncl.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gbf.yj20258.top

[Q31] 分组后过滤
来源：http://ghm.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wla.c1oappe.top

[Q32] 分组拼接字符串
来源：http://uar.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wlg.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yoy.yangfankeji.com

[Q33] 多列分组
来源：http://vnj.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ymt.uphjek.com

[Q34] 每组取第一条
来源：http://qjd.shanyushiyangkeji.top

SELECT * FROM (
来源：http://won.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://woo.yj20258.top

) t WHERE rn = 1;
来源：http://ijo.zycfv.cn

[Q35] 内连接
来源：http://zgy.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oab.sjlbkw.cn

[Q36] 左连接
来源：http://bmt.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hjc.snrcjt.cn

[Q37] 右连接
来源：http://hoz.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ztd.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://zga.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ehp.cashguo.top

[Q39] 自连接（查上下级）
来源：http://ygh.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aks.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pmw.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://prx.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ihy.aibaodan.cn

[Q41] 多表连接
来源：http://ucl.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://uob.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://qwa.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://otu.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://vzt.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://dzm.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ifk.yfazqb.com

[Q43] 标量子查询
来源：http://cwo.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ydr.chenlongwang.top

[Q44] IN 子查询
来源：http://ikj.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uvl.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://pzw.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lev.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://jrz.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hdn.wangdashe.top

[Q47] 与平均值比较
来源：http://hdy.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://htm.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://agy.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ccn.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://cad.ehwqpu.com

[Q49] 更新单行
来源：http://paz.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tia.nanxuanxn.top

[Q50] 批量更新
来源：http://ftm.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://alx.quarkkingdee.top

[Q51] 用子查询更新
来源：http://jpi.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rqf.sjlbkw.cn

[Q52] 删除指定行
来源：http://tzw.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://kvx.hnxiangtu.top

[Q53] 按条件删除
来源：http://tib.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wsa.birdmap.top

[Q54] 清空表
来源：http://msc.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://kvp.bjfxy.top

[Q55] 排名（并列占位）
来源：http://nkf.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://igk.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://zwk.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fse.hammf.cn

[Q57] 行号
来源：http://qll.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oix.xinyue.icu

[Q58] 累计求和
来源：http://aro.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zkt.jiagoushi.top

[Q59] 分组内累计
来源：http://xzj.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xhu.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://vib.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://enc.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://abf.jinqigufen.top

[Q61] 移动平均
来源：http://xfs.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ykc.zhixingplan.top

[Q62] 分组占比
来源：http://rnk.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://atf.xylfe.cn

[Q63] 开启事务
来源：http://hjo.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tmu.xuetiantiany.cn

[Q64] 提交事务
来源：http://ieg.ehwqpu.com

COMMIT;
来源：http://zwl.zhijiandao.cn

[Q65] 回滚事务
来源：http://nuk.xylfe.cn

ROLLBACK;
来源：http://fgx.cucudq.cn

[Q66] 行锁查询
来源：http://dmu.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://slx.tianlin.xyz

[Q67] 设置隔离级别
来源：http://laq.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://old.meibo888.top

[Q68] 保存点
来源：http://qqa.yuanzhike.top

SAVEPOINT sp1;
来源：http://iel.fehbvm.com

ROLLBACK TO sp1;
来源：http://mzq.jqgufenzy.top

[Q69] 查看执行计划
来源：http://atu.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cna.havefunace.top

[Q70] 更新统计信息
来源：http://ebm.aizwys.cn

ANALYZE TABLE users;
来源：http://pwl.pycfn.com

[Q71] 查看建表语句
来源：http://qin.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pft.yuxming.cn

[Q72] 查看索引
来源：http://wki.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://mvb.aizwys.cn

[Q73] 查看表状态
来源：http://auu.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pmk.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://jzr.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://poh.cucudq.cn

[Q75] 日期格式化
来源：http://qtl.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyu.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ssb.zdqjudy.top

[Q76] 按天统计
来源：http://nyw.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://orl.wangshuangyany.cn

[Q77] 时间加减
来源：http://wcr.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jlh.zhiwuduotai.top

[Q78] 当前时间
来源：http://njk.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wjj.0kj1m.cn

[Q79] 字符串拼接
来源：http://rcf.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zug.zdqjudy.top

[Q80] 字符串截取
来源：http://dsf.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://psy.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://gah.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fik.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://mzy.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vpk.andypj.xyz

[Q83] 大小写转换
来源：http://bqt.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hkr.yuanzhike.top

[Q84] 去除首尾空格
来源：http://twi.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://ayv.jinqigufen.top

[Q85] 数值取整
来源：http://oxp.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yxv.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://evi.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gcw.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://ufb.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kki.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://gjo.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ieu.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hct.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://dkh.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qff.wangdashe.top

[Q90] 生成序号列
来源：http://ges.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fki.jqgfzy.top

================================================================================
来源：http://gcz.dashuyun.cn

R. Bash 专题
来源：http://hmz.hywenlv.cn

================================================================================
来源：http://xvr.hammf.cn

[R01] shebang 与严格模式
来源：http://rkn.fehbvm.com

#!/usr/bin/env bash
来源：http://dyp.andypj.xyz

set -euo pipefail
来源：http://ilm.hywenlv.cn

[R02] 变量赋值与使用
来源：http://ugp.nanxinkj.top

name="Tom"; echo "$name"
来源：http://cjq.hammf.cn

[R03] 只读变量
来源：http://bfz.pycfn.com

readonly PI=3.14
来源：http://wgm.gzhubu.top

[R04] 位置参数
来源：http://ftm.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nqe.ydjk.org.cn

[R05] 参数默认值
来源：http://rki.jlsjyb.cn

name="${1:-default}"
来源：http://uir.tian-w.cn

[R06] 判断命令是否存在
来源：http://odt.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cky.hcnkem.com

[R07] if 判断文件
来源：http://oiu.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vre.pengpengdd.cyou

[R08] 数值比较
来源：http://txz.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rga.redwolf501.top

[R09] 字符串比较
来源：http://lgd.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cgy.nanxinkj.top

[R10] 正则匹配
来源：http://qcu.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bgo.hnqzz.top

[R11] case 多分支
来源：http://ldw.aizwys.cn

case "$1" in
来源：http://rsy.yj20258888.top

start) echo "启动" ;;
来源：http://cjw.hcnkem.com

stop)  echo "停止" ;;
来源：http://zqj.bjfxy.top

*)     echo "未知命令" ;;
来源：http://hmg.cheryme.top

esac
来源：http://nun.kuanghao11.cn

[R12] for 遍历文件
来源：http://qer.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://qnw.ybcxt.top

[R13] for 计数循环
来源：http://gfv.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://rvo.tian-w.cn

[R14] C 风格 for
来源：http://bjm.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://koi.redwolf501.top

[R15] while 逐行读文件
来源：http://cem.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://trl.yangfankeji.com

[R16] until 等待条件
来源：http://vlv.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rfh.ybcxt.top

[R17] 数组定义与取值
来源：http://pmd.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://xrk.jqgfzy.top

[R18] 遍历数组
来源：http://qni.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hdz.gzhubu.top

[R19] 数组长度
来源：http://klk.yuxming.cn

echo "${#arr[@]}"
来源：http://hff.jyoumei.cn

[R20] 关联数组（字典）
来源：http://uhi.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mph.xuetiantiany.cn

[R21] 字符串长度
来源：http://uxi.yongpay.top

echo "${#s}"
来源：http://lhs.hammf.cn

[R22] 截取子串
来源：http://peu.jyoumei.cn

echo "${s:0:5}"
来源：http://pld.jqgufenzy.top

[R23] 字符串替换
来源：http://tmm.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://brg.fktsv.cn

[R24] 大小写转换
来源：http://uan.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://wsg.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://rhk.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xkk.zhijiandao.cn

[R26] 命令替换
来源：http://iyg.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://gpn.jqgfzy.top

[R27] 算术展开
来源：http://ddd.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://avr.epnwcf.com

[R28] 浮点运算
来源：http://hqo.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://zyk.jinqigufen.top

[R29] 定义函数
来源：http://esf.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://faq.shzxlz.cn

[R30] 函数返回状态码
来源：http://pne.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://lwt.cashguo.top

[R31] 局部变量
来源：http://ymi.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://lqd.yuxming.cn

[R32] 参数个数校验
来源：http://jvd.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bur.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://zwk.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lqv.jlsjyb.cn

[R34] 退出时清理
来源：http://kmb.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vpp.ehwqpu.com

[R35] 后台执行并等待
来源：http://jas.quarkkingdee.top


<!-- 参考信息 -->