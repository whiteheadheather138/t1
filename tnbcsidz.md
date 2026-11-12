代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oic.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oyq.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://nbp.zdbjq.cn

Ruby: a == b
来源：http://klv.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aml.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mwj.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://smv.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://yio.gotoacloud.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yaj.c1oappe.top

TS:   if (x == null) {}
来源：http://yaf.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iuu.yfazqb.com

Go:   if x == nil {}
来源：http://eww.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hex.fzhhl.top

C#:   if (x is null) {}
来源：http://ocy.cheryme.top

[P07] 防抖与节流
来源：http://tsf.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bgf.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://tse.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pui.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://biw.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ekp.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://moj.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wnk.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ivi.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://tga.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mzq.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bre.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xhr.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vbd.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qfk.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kbg.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zxt.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pip.yonumen.top

================================================================================
来源：http://qkf.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lqd.sxryk.cn

================================================================================
来源：http://cmp.cdnleiting.top

[Q01] 创建表
来源：http://vrd.shzxlz.cn

CREATE TABLE users (
来源：http://oqk.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhz.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://wdm.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://gez.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jqh.meibo888.top

);
来源：http://vrn.xziqi.cn

[Q02] 创建带外键的表
来源：http://odb.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://kzs.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hao.epnwcf.com

user_id INT NOT NULL,
来源：http://hje.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://vwz.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zls.yvedp.cn

);
来源：http://ete.zdbjq.cn

[Q03] 增加列
来源：http://zts.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://alu.tian-w.cn

[Q04] 修改列类型
来源：http://xmm.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gjg.jianghu66.top

[Q05] 重命名列
来源：http://zoq.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nfy.bjfxy.top

[Q06] 删除列
来源：http://xhr.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://dte.zhongyouzk.top

[Q07] 删除表
来源：http://ytq.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://djz.hnqzz.top

[Q08] 创建普通索引
来源：http://xte.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://don.xziqi.cn

[Q09] 创建唯一索引
来源：http://cup.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xrl.gogol.net.cn

[Q10] 插入单行
来源：http://jzl.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ijv.ydzc1.top

[Q11] 一次插入多行
来源：http://bcx.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sos.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://liw.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://hfw.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cvn.hysaishi.cn

[Q13] 忽略重复插入
来源：http://xdo.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dpy.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://koj.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xeb.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://suc.mhx1999.top

[Q15] 查询全部
来源：http://cnu.52xcode.cn

SELECT * FROM users;
来源：http://dxq.hcnkem.com

[Q16] 查询指定列
来源：http://syz.daxiang520.top

SELECT id, name FROM users;
来源：http://thd.xuanzx.com

[Q17] 条件查询
来源：http://gjn.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uvv.gaohongyu789.top

[Q18] 模糊匹配
来源：http://hyq.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fep.havefunace.top

[Q19] 范围查询
来源：http://ohf.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://icb.ydjk.org.cn

[Q20] IN 列表
来源：http://wqd.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gst.aizwys.cn

[Q21] 空值判断
来源：http://ten.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dtc.zycfv.cn

[Q22] 排序
来源：http://qzq.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nbk.52xcode.cn

[Q23] 分页
来源：http://oil.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tff.svipenyu.cn

[Q24] 去重
来源：http://bkv.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://jba.chenzaomai.com

[Q25] 只取前 N 条
来源：http://fkt.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ame.xinyue.icu

[Q26] 计数
来源：http://noo.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://ady.fktsv.cn

[Q27] 条件计数
来源：http://bfh.xziqi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jon.zhiwuduotai.top

[Q28] 求和与平均
来源：http://gkg.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yav.wangshuangyany.cn

[Q29] 最大最小值
来源：http://hyx.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zsu.0kj1m.cn

[Q30] 分组统计
来源：http://yps.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://llf.yj202588.top

[Q31] 分组后过滤
来源：http://zrf.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://onu.yj202588.top

[Q32] 分组拼接字符串
来源：http://jfj.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qci.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wjs.chenjidiqi.icu

[Q33] 多列分组
来源：http://qih.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bam.ehwqpu.com

[Q34] 每组取第一条
来源：http://mhc.gotoacloud.top

SELECT * FROM (
来源：http://zip.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ieq.hcnkem.com

) t WHERE rn = 1;
来源：http://pvh.yj20258.top

[Q35] 内连接
来源：http://azv.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ixm.hammf.cn

[Q36] 左连接
来源：http://ksd.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zlq.jqgfzy.top

[Q37] 右连接
来源：http://xsz.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://frg.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://hto.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lrv.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://umh.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lyg.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xev.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lbi.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hvl.316326.xyz

[Q41] 多表连接
来源：http://aia.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://neb.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://urt.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://ahx.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://ckq.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://pnm.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aul.hongshengwenyu.top

[Q43] 标量子查询
来源：http://pee.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ohs.cheryme.top

[Q44] IN 子查询
来源：http://ydl.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ppy.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://ogx.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qto.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://cng.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cmu.sjlbkw.cn

[Q47] 与平均值比较
来源：http://man.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zem.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://tik.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qct.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://qkt.jinqigufen.top

[Q49] 更新单行
来源：http://fyz.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://orl.pengpengdd.cyou

[Q50] 批量更新
来源：http://uns.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://woz.cqqwz.cn

[Q51] 用子查询更新
来源：http://tdy.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ltv.fengsongda.top

[Q52] 删除指定行
来源：http://irm.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://mpd.jiagoushi.top

[Q53] 按条件删除
来源：http://crk.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lxi.kuanghao11.cn

[Q54] 清空表
来源：http://nix.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://tgx.daria6918.cn

[Q55] 排名（并列占位）
来源：http://kfj.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://owo.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://zpd.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oqt.epnwcf.com

[Q57] 行号
来源：http://kwq.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jnh.wangdashe.top

[Q58] 累计求和
来源：http://hal.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rjk.hongshengwenyu.top

[Q59] 分组内累计
来源：http://ooq.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jsi.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://yox.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rrc.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sip.pengpengdd.cyou

[Q61] 移动平均
来源：http://ysd.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wkn.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://ruj.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mhc.sjlbkw.cn

[Q63] 开启事务
来源：http://fzu.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dwn.cashguo.top

[Q64] 提交事务
来源：http://gjm.yj20258888.top

COMMIT;
来源：http://esn.ybcxt.top

[Q65] 回滚事务
来源：http://upp.yvedp.cn

ROLLBACK;
来源：http://trb.sweek.top

[Q66] 行锁查询
来源：http://ibl.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pjn.hnqzz.top

[Q67] 设置隔离级别
来源：http://hfy.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vrv.yangfankeji.com

[Q68] 保存点
来源：http://jsz.yueranfly.top

SAVEPOINT sp1;
来源：http://ftb.yj20258.top

ROLLBACK TO sp1;
来源：http://qse.hesvh.cn

[Q69] 查看执行计划
来源：http://wqe.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qzx.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://gnz.zhengqikj.top

ANALYZE TABLE users;
来源：http://udw.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://lcq.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fmn.ctjpmb.com

[Q72] 查看索引
来源：http://cwp.yuanzhike.top

SHOW INDEX FROM users;
来源：http://stz.guannengcc.top

[Q73] 查看表状态
来源：http://bom.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://efk.bjfxy.top

[Q74] 强制使用索引
来源：http://hzi.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://skh.jqgfzy.top

[Q75] 日期格式化
来源：http://oqf.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kca.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eim.hfpthk.cn

[Q76] 按天统计
来源：http://qjl.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mdt.hnxiangtu.top

[Q77] 时间加减
来源：http://iwe.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://opa.xuetiantiany.cn

[Q78] 当前时间
来源：http://ecx.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zmv.jqgufenzy.top

[Q79] 字符串拼接
来源：http://rfg.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hmo.jianghu66.top

[Q80] 字符串截取
来源：http://ked.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ust.aizwys.cn

[Q81] 字符串替换
来源：http://igm.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dny.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://awv.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://clk.chenjidiqi.icu

[Q83] 大小写转换
来源：http://nsq.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fvl.yj20258888.top

[Q84] 去除首尾空格
来源：http://lzn.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://ngk.jqgfzy.top

[Q85] 数值取整
来源：http://yhp.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdg.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://vvy.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://knn.ivvv.top

[Q87] JSON 字段做条件
来源：http://cmj.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rno.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://bsz.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://efr.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pgs.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://hsy.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkr.yongpay.top

[Q90] 生成序号列
来源：http://wmu.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://utv.jinghuilouyu.cn

================================================================================
来源：http://yov.gaohongyu789.top

R. Bash 专题
来源：http://bxe.vehdjk.com

================================================================================
来源：http://lms.9152youxi.cn

[R01] shebang 与严格模式
来源：http://lgk.52xcode.cn

#!/usr/bin/env bash
来源：http://usk.cheryme.top

set -euo pipefail
来源：http://owf.9152youxi.cn

[R02] 变量赋值与使用
来源：http://sto.fktsv.cn

name="Tom"; echo "$name"
来源：http://hoi.jianghu66.top

[R03] 只读变量
来源：http://hsl.vehdjk.com

readonly PI=3.14
来源：http://tkb.haohaochexian.top

[R04] 位置参数
来源：http://cbf.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cgt.feifeiyinyue.top

[R05] 参数默认值
来源：http://sxx.feifeiyinyue.top

name="${1:-default}"
来源：http://jlc.tanke756.top

[R06] 判断命令是否存在
来源：http://gft.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kfl.zhiwuduotai.top

[R07] if 判断文件
来源：http://jdk.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tlz.yfazqb.com

[R08] 数值比较
来源：http://lob.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pyw.gaohongyu789.top

[R09] 字符串比较
来源：http://ebv.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://szb.zhoulong.xyz

[R10] 正则匹配
来源：http://nrg.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nle.ydzc1.top

[R11] case 多分支
来源：http://gxx.xuanzx.com

case "$1" in
来源：http://psz.hammf.cn

start) echo "启动" ;;
来源：http://gii.tarul.cn

stop)  echo "停止" ;;
来源：http://gjs.vehdjk.com

*)     echo "未知命令" ;;
来源：http://wca.cqqwz.cn

esac
来源：http://gjn.hnxiangtu.top

[R12] for 遍历文件
来源：http://nzq.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://ebe.hnxiangtu.top

[R13] for 计数循环
来源：http://ler.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://dcz.meibo888.top

[R14] C 风格 for
来源：http://spu.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wkq.bbcook.cn

[R15] while 逐行读文件
来源：http://qkn.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bgj.sxryk.cn

[R16] until 等待条件
来源：http://afa.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aml.daxiang520.top

[R17] 数组定义与取值
来源：http://oia.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ytc.9152youxi.cn

[R18] 遍历数组
来源：http://wwj.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wln.sufxvd.cn

[R19] 数组长度
来源：http://kni.zdbjq.cn

echo "${#arr[@]}"
来源：http://isq.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://otx.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://euq.jinqigufen.top

[R21] 字符串长度
来源：http://tvg.dashuyun.cn

echo "${#s}"
来源：http://uxb.fehbvm.com

[R22] 截取子串
来源：http://aui.yj202588.top

echo "${s:0:5}"
来源：http://rtg.shangyingyoupin.top

[R23] 字符串替换
来源：http://vnb.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://liv.hywenlv.cn

[R24] 大小写转换
来源：http://ago.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://mfz.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://rdx.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eff.yuxming.cn

[R26] 命令替换
来源：http://jon.havefunace.top

now=$(date +%F); echo "$now"
来源：http://afd.zhongyouzk.top

[R27] 算术展开
来源：http://rxy.zhaomingkeji.xyz


<!-- 参考信息 -->