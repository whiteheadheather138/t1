代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fjz.sweek.top

TS:   if (x == null) {}
来源：http://zrf.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qdz.zhixingplan.top

Go:   if x == nil {}
来源：http://bwj.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ugd.yj20258888.top

C#:   if (x is null) {}
来源：http://qen.yj20258.top

[P07] 防抖与节流
来源：http://otd.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://whc.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://zhb.zhoulong.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlh.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixf.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://exm.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ypn.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kvb.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bog.yj202588.top

[P08] 处理浮点精度问题
来源：http://trw.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://twz.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://exz.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yjp.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hbx.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eka.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vhw.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sza.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vha.cheryme.top

================================================================================
来源：http://wdt.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzv.ivvv.top

================================================================================
来源：http://mwp.shanyushiyangtech.top

[Q01] 创建表
来源：http://zvt.chenjidiqi.icu

CREATE TABLE users (
来源：http://qjj.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ifk.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://rql.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://rwp.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ecb.sweek.top

);
来源：http://uco.yfazqb.com

[Q02] 创建带外键的表
来源：http://jof.aibaodan.cn

CREATE TABLE orders (
来源：http://evm.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pze.fzhhl.top

user_id INT NOT NULL,
来源：http://lqo.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://szz.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://djl.jqgfzy.top

);
来源：http://wfo.fehbvm.com

[Q03] 增加列
来源：http://tmj.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tkh.ydjk.org.cn

[Q04] 修改列类型
来源：http://atz.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xfb.nanxinkj.top

[Q05] 重命名列
来源：http://elg.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://plm.hesvh.cn

[Q06] 删除列
来源：http://lxt.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://eai.dianchejie.cn

[Q07] 删除表
来源：http://lnk.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://kfg.iojbl.cn

[Q08] 创建普通索引
来源：http://bjj.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bgd.yj20258888.top

[Q09] 创建唯一索引
来源：http://mam.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wal.yonumen.top

[Q10] 插入单行
来源：http://inh.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qnh.vqdsnc.cn

[Q11] 一次插入多行
来源：http://ncq.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bud.yj202588.top

[Q12] 插入后取自增 ID
来源：http://tsp.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pfu.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rkk.tian-w.cn

[Q13] 忽略重复插入
来源：http://pky.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tgv.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://mrn.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjv.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ceu.cdnleiting.top

[Q15] 查询全部
来源：http://khc.sweek.top

SELECT * FROM users;
来源：http://mic.shangyingyoupin.top

[Q16] 查询指定列
来源：http://qrm.sysykeji.top

SELECT id, name FROM users;
来源：http://xka.birdmap.top

[Q17] 条件查询
来源：http://xzu.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bks.zhijiandao.cn

[Q18] 模糊匹配
来源：http://fss.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aon.52xcode.cn

[Q19] 范围查询
来源：http://vrn.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wvl.xuanzx.com

[Q20] IN 列表
来源：http://cxl.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pmh.hnqzz.top

[Q21] 空值判断
来源：http://vun.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://afy.cdnleiting.top

[Q22] 排序
来源：http://sme.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nsl.xuanzx.com

[Q23] 分页
来源：http://zvk.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lte.jqgfzy.top

[Q24] 去重
来源：http://vlb.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://wod.yuanzhike.top

[Q25] 只取前 N 条
来源：http://lna.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://shj.vehdjk.com

[Q26] 计数
来源：http://swe.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://dlq.vqdsnc.cn

[Q27] 条件计数
来源：http://ipq.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pcq.cheryme.top

[Q28] 求和与平均
来源：http://rgg.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xsl.sxryk.cn

[Q29] 最大最小值
来源：http://utv.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://geo.sjlbkw.cn

[Q30] 分组统计
来源：http://brd.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zsy.zycfv.cn

[Q31] 分组后过滤
来源：http://sgj.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hfp.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://ewv.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://snk.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aac.yfazqb.com

[Q33] 多列分组
来源：http://uhc.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kkr.vqdsnc.cn

[Q34] 每组取第一条
来源：http://fuy.iojbl.cn

SELECT * FROM (
来源：http://lxs.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jrc.cucudq.cn

) t WHERE rn = 1;
来源：http://gzv.feifeiyinyue.top

[Q35] 内连接
来源：http://hdd.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kcj.yonumen.top

[Q36] 左连接
来源：http://whh.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://idq.birdmap.top

[Q37] 右连接
来源：http://gws.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://foz.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://uvj.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hlw.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://zot.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dqu.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://txu.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://stm.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pqa.xylfe.cn

[Q41] 多表连接
来源：http://sib.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://wvw.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://hqp.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://mwu.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://zhx.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://xso.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jyr.xuanzx.com

[Q43] 标量子查询
来源：http://yeq.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lqz.jlsjyb.cn

[Q44] IN 子查询
来源：http://tlz.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gfu.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://kxf.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpa.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://teh.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wov.yonumen.top

[Q47] 与平均值比较
来源：http://ucs.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gwl.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://xqf.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vay.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://kyn.aibaodan.cn

[Q49] 更新单行
来源：http://xbl.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tdz.zhoulong.xyz

[Q50] 批量更新
来源：http://moi.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://whm.xinyue.icu

[Q51] 用子查询更新
来源：http://yxg.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nib.nanxinkj.top

[Q52] 删除指定行
来源：http://mgv.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://yld.quarkkingdee.top

[Q53] 按条件删除
来源：http://eic.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hjb.sxryk.cn

[Q54] 清空表
来源：http://etf.ydzc1.top

TRUNCATE TABLE logs;
来源：http://jer.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://zux.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gia.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://lyt.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wgh.daxiang520.top

[Q57] 行号
来源：http://ijk.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xgx.fktsv.cn

[Q58] 累计求和
来源：http://edi.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rms.chenlongwang.top

[Q59] 分组内累计
来源：http://yvy.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wef.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://ank.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jhl.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gdo.yuanzhike.top

[Q61] 移动平均
来源：http://isy.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wbs.vqdsnc.cn

[Q62] 分组占比
来源：http://euv.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xne.hysaishi.cn

[Q63] 开启事务
来源：http://sjr.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ieu.aizwys.cn

[Q64] 提交事务
来源：http://nti.gotoacloud.top

COMMIT;
来源：http://cwu.vehdjk.com

[Q65] 回滚事务
来源：http://qmm.sysykeji.top

ROLLBACK;
来源：http://xzr.shzxlz.cn

[Q66] 行锁查询
来源：http://sun.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://avk.0kj1m.cn

[Q67] 设置隔离级别
来源：http://dkz.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxc.jyoumei.cn

[Q68] 保存点
来源：http://atc.zhongyouzk.top

SAVEPOINT sp1;
来源：http://xga.nwbrower.top

ROLLBACK TO sp1;
来源：http://dvs.sufxvd.cn

[Q69] 查看执行计划
来源：http://nqk.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zzx.guowangkeji.top

[Q70] 更新统计信息
来源：http://kmu.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://ejl.redwolf501.top

[Q71] 查看建表语句
来源：http://ksd.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ozo.jiagoushi.top

[Q72] 查看索引
来源：http://nni.shzxlz.cn

SHOW INDEX FROM users;
来源：http://ndx.yj202588.top

[Q73] 查看表状态
来源：http://jzg.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oxe.yj202588.top

[Q74] 强制使用索引
来源：http://ngu.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://avl.aibaodan.cn

[Q75] 日期格式化
来源：http://lni.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ube.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sip.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://ohs.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jjs.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://hwy.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qqc.jlsjyb.cn

[Q78] 当前时间
来源：http://kus.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jgt.tanke756.top

[Q79] 字符串拼接
来源：http://suq.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xln.fktsv.cn

[Q80] 字符串截取
来源：http://zyo.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://afy.chenlongwang.top

[Q81] 字符串替换
来源：http://dwm.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ifl.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://qdu.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uoo.yj202588.top

[Q83] 大小写转换
来源：http://tdz.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jwy.uphjek.com

[Q84] 去除首尾空格
来源：http://cue.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://vik.havefunace.top

[Q85] 数值取整
来源：http://mfa.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://thy.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://dpp.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aac.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://byb.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pdl.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://jkf.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://spy.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ike.vehdjk.com

[Q89] 判断表是否存在
来源：http://uxk.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://suz.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://dad.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aob.xziqi.cn

================================================================================
来源：http://cwl.feifeiyinyue.top

R. Bash 专题
来源：http://vho.smart0.xyz

================================================================================
来源：http://jfk.zdqjudy.top

[R01] shebang 与严格模式
来源：http://lwz.yuxming.cn

#!/usr/bin/env bash
来源：http://jre.hnxiangtu.top

set -euo pipefail
来源：http://ayi.zhixingplan.top

[R02] 变量赋值与使用
来源：http://gbs.yfazqb.com

name="Tom"; echo "$name"
来源：http://wtv.gotoacloud.top

[R03] 只读变量
来源：http://cwq.zhongyouzk.top

readonly PI=3.14
来源：http://ujb.sjlbkw.cn

[R04] 位置参数
来源：http://dfq.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nhc.jinqigufen.top

[R05] 参数默认值
来源：http://kpl.jqgufenzy.top

name="${1:-default}"
来源：http://yxy.ivvv.top

[R06] 判断命令是否存在
来源：http://jwx.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eal.shangyingyoupin.top

[R07] if 判断文件
来源：http://sns.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tmk.sxryk.cn

[R08] 数值比较
来源：http://ygs.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tvv.epnwcf.com

[R09] 字符串比较
来源：http://oms.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhg.yj20258888.top

[R10] 正则匹配
来源：http://yss.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pkc.chenzaomai.com

[R11] case 多分支
来源：http://zqd.mhx1999.top

case "$1" in
来源：http://pri.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://rno.hesvh.cn

stop)  echo "停止" ;;
来源：http://dic.yueranfly.top

*)     echo "未知命令" ;;
来源：http://olg.yueranfly.top

esac
来源：http://xjx.ehwqpu.com

[R12] for 遍历文件
来源：http://qqs.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://ymo.gotoacloud.top

[R13] for 计数循环
来源：http://vnj.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://wmh.gogol.net.cn

[R14] C 风格 for
来源：http://ewq.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zxd.xuanzx.com

[R15] while 逐行读文件
来源：http://tce.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ixz.zhongyouzk.top

[R16] until 等待条件
来源：http://xey.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ahq.tarul.cn

[R17] 数组定义与取值
来源：http://ihw.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://art.xinyue.icu

[R18] 遍历数组
来源：http://jcj.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emc.ivvv.top

[R19] 数组长度
来源：http://asa.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://yud.yangfankeji.com

[R20] 关联数组（字典）
来源：http://phx.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bwz.andypj.xyz

[R21] 字符串长度
来源：http://cia.pengpengdd.cyou

echo "${#s}"
来源：http://sdz.havefunace.top

[R22] 截取子串
来源：http://dvm.ivvv.top

echo "${s:0:5}"
来源：http://oym.bbcook.cn

[R23] 字符串替换
来源：http://srv.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tgo.pengpengdd.cyou

[R24] 大小写转换
来源：http://dlj.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hjv.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://cvk.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbb.jqgufenzy.top

[R26] 命令替换
来源：http://kni.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://ggz.svipenyu.cn

[R27] 算术展开
来源：http://tas.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://rie.cdnleiting.top

[R28] 浮点运算
来源：http://vlp.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://ahy.dashuyun.cn

[R29] 定义函数
来源：http://dex.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://axy.vehdjk.com

[R30] 函数返回状态码
来源：http://khf.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://fso.xinyue.icu

[R31] 局部变量
来源：http://exk.yangfankeji.com


<!-- 参考信息 -->