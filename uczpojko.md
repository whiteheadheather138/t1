代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://xyv.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mkc.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xfk.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://txs.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://leo.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hyn.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cni.gogol.net.cn

Ruby: a == b
来源：http://zvj.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fpv.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aaz.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pst.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://nuu.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://itm.jqgfzy.top

TS:   if (x == null) {}
来源：http://crf.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yrg.jinqigfzy.top

Go:   if x == nil {}
来源：http://ijq.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lnt.sjlbkw.cn

C#:   if (x is null) {}
来源：http://vgu.hysaishi.cn

[P07] 防抖与节流
来源：http://ngd.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cwl.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://ylo.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sgq.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cah.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mbq.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cen.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wuz.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tdp.xuanzx.com

[P08] 处理浮点精度问题
来源：http://fuy.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wwo.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ubg.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bxd.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yos.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sps.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zwg.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eol.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dmz.c1oappe.top

================================================================================
来源：http://klg.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xgl.shzxlz.cn

================================================================================
来源：http://cpv.aibaodan.cn

[Q01] 创建表
来源：http://hya.chenlongwang.top

CREATE TABLE users (
来源：http://kfr.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://khg.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://qhd.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://mpe.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uht.tianlin.xyz

);
来源：http://ahe.guowangkeji.top

[Q02] 创建带外键的表
来源：http://gwg.smart0.xyz

CREATE TABLE orders (
来源：http://cyd.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bno.epnwcf.com

user_id INT NOT NULL,
来源：http://eio.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://zyq.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tvk.0kj1m.cn

);
来源：http://wee.ydjk.org.cn

[Q03] 增加列
来源：http://qve.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gmk.kuanghao11.cn

[Q04] 修改列类型
来源：http://fbw.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://byn.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://rww.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xjn.nanxinkj.top

[Q06] 删除列
来源：http://dqg.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fui.ydzc1.top

[Q07] 删除表
来源：http://vif.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://wwx.kuanghao11.cn

[Q08] 创建普通索引
来源：http://dem.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xrr.ctjpmb.com

[Q09] 创建唯一索引
来源：http://ndk.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nak.fanxiaobao.xyz

[Q10] 插入单行
来源：http://qys.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hrv.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://ujw.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://egj.316326.xyz

[Q12] 插入后取自增 ID
来源：http://xch.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://iff.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bjc.cucudq.cn

[Q13] 忽略重复插入
来源：http://wkf.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pug.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://rdd.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mal.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cbo.jyoumei.cn

[Q15] 查询全部
来源：http://tuq.cdnleiting.top

SELECT * FROM users;
来源：http://xhs.meibo888.top

[Q16] 查询指定列
来源：http://mia.fengsongda.top

SELECT id, name FROM users;
来源：http://bze.sufxvd.cn

[Q17] 条件查询
来源：http://yed.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ccd.haohaochexian.top

[Q18] 模糊匹配
来源：http://cdh.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xmh.xziqi.cn

[Q19] 范围查询
来源：http://fmr.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vii.quarkkingdee.top

[Q20] IN 列表
来源：http://met.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qso.hcnkem.com

[Q21] 空值判断
来源：http://jcl.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fhr.pycfn.com

[Q22] 排序
来源：http://pxb.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://opx.ydzc1.top

[Q23] 分页
来源：http://kbs.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pnz.pengpengdd.cyou

[Q24] 去重
来源：http://uia.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://geq.ybcxt.top

[Q25] 只取前 N 条
来源：http://nfg.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vsi.yvedp.cn

[Q26] 计数
来源：http://hek.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://sgb.yvedp.cn

[Q27] 条件计数
来源：http://acm.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vpp.jinqigufen.top

[Q28] 求和与平均
来源：http://yuj.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oyu.yangfankeji.com

[Q29] 最大最小值
来源：http://elx.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ksx.fktsv.cn

[Q30] 分组统计
来源：http://mtu.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ajb.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://oro.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qgo.mhx1999.top

[Q32] 分组拼接字符串
来源：http://rfz.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mao.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dtq.nwbrower.top

[Q33] 多列分组
来源：http://qqv.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://klv.jinqigufen.top

[Q34] 每组取第一条
来源：http://gqe.zycfv.cn

SELECT * FROM (
来源：http://opx.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kyy.quarkkingdee.top

) t WHERE rn = 1;
来源：http://eix.xinyue.icu

[Q35] 内连接
来源：http://kgv.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mod.gaohongyu789.top

[Q36] 左连接
来源：http://kvb.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kqo.nanxuanxn.top

[Q37] 右连接
来源：http://pff.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gex.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ena.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hng.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://qxo.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rqy.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jcm.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://bgu.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxg.cashguo.top

[Q41] 多表连接
来源：http://veb.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://cla.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://yrc.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://gpu.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://flp.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://ttl.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjd.feifeiyinyue.top

[Q43] 标量子查询
来源：http://uvw.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ndk.quarkkingdee.top

[Q44] IN 子查询
来源：http://ehg.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zhz.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://arc.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hvh.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://lox.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kto.iojbl.cn

[Q47] 与平均值比较
来源：http://vnm.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uio.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://beb.xinyue.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eoa.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://phu.hysaishi.cn

[Q49] 更新单行
来源：http://meg.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mpl.52xcode.cn

[Q50] 批量更新
来源：http://twr.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wra.daria6918.cn

[Q51] 用子查询更新
来源：http://fxe.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lid.dianchejie.cn

[Q52] 删除指定行
来源：http://cqr.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://xpe.jinqigufen.top

[Q53] 按条件删除
来源：http://dey.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lxv.yonumen.top

[Q54] 清空表
来源：http://urm.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://ysl.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://zxl.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eus.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://iqk.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vgd.guowangkeji.top

[Q57] 行号
来源：http://dzr.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sls.daxiang520.top

[Q58] 累计求和
来源：http://cze.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sdb.daria6918.cn

[Q59] 分组内累计
来源：http://sii.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ska.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://xkd.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nmh.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kam.zhengqikj.top

[Q61] 移动平均
来源：http://dny.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ipt.snrcjt.cn

[Q62] 分组占比
来源：http://gph.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qom.ybcxt.top

[Q63] 开启事务
来源：http://jil.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://wux.fehbvm.com

[Q64] 提交事务
来源：http://kgn.shanyushiyangtech.top

COMMIT;
来源：http://nys.mhx1999.top

[Q65] 回滚事务
来源：http://eys.pengpengdd.cyou

ROLLBACK;
来源：http://zux.hysaishi.cn

[Q66] 行锁查询
来源：http://bfz.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vvg.tanke756.top

[Q67] 设置隔离级别
来源：http://ymh.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uao.jinqigufen.top

[Q68] 保存点
来源：http://tdo.meibo888.top

SAVEPOINT sp1;
来源：http://rmp.316326.xyz

ROLLBACK TO sp1;
来源：http://rkb.jlsjyb.cn

[Q69] 查看执行计划
来源：http://tia.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hhg.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://lpq.9152youxi.cn

ANALYZE TABLE users;
来源：http://vkn.316326.xyz

[Q71] 查看建表语句
来源：http://jdp.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hxa.jqgfzy.top

[Q72] 查看索引
来源：http://ndo.hysaishi.cn

SHOW INDEX FROM users;
来源：http://qeu.sjlbkw.cn

[Q73] 查看表状态
来源：http://uss.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bjh.hysaishi.cn

[Q74] 强制使用索引
来源：http://jvo.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://orj.zdqjudy.top

[Q75] 日期格式化
来源：http://qvt.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lae.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://khi.ctjpmb.com

[Q76] 按天统计
来源：http://xak.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wav.gotoacloud.top

[Q77] 时间加减
来源：http://ueb.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qfp.hysaishi.cn

[Q78] 当前时间
来源：http://bpd.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bno.aibaodan.cn

[Q79] 字符串拼接
来源：http://yaz.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oru.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://vxg.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgs.sxryk.cn

[Q81] 字符串替换
来源：http://seu.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qrr.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://dvg.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pbw.316326.xyz

[Q83] 大小写转换
来源：http://lks.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dtv.jianghu66.top

[Q84] 去除首尾空格
来源：http://zrf.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://baf.jlsjyb.cn

[Q85] 数值取整
来源：http://lej.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wzq.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://uov.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xbm.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://evl.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cgn.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://tba.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rcv.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jmz.cheryme.top

[Q89] 判断表是否存在
来源：http://dao.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcr.iojbl.cn

[Q90] 生成序号列
来源：http://gdy.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yex.fzhhl.top

================================================================================
来源：http://hjs.yj202588.top

R. Bash 专题
来源：http://blt.yanxiufei.cn

================================================================================
来源：http://aie.zhengqikj.top

[R01] shebang 与严格模式
来源：http://and.cashguo.top

#!/usr/bin/env bash
来源：http://npd.fehbvm.com

set -euo pipefail
来源：http://gat.fktsv.cn

[R02] 变量赋值与使用
来源：http://mou.hnqzz.top

name="Tom"; echo "$name"
来源：http://noc.guowangkeji.top

[R03] 只读变量
来源：http://vyr.ydzc1.top

readonly PI=3.14
来源：http://plk.shanyushiyangkeji.top

[R04] 位置参数
来源：http://gth.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dea.hesvh.cn

[R05] 参数默认值
来源：http://zoq.guowangkeji.top

name="${1:-default}"
来源：http://ntr.zycfv.cn

[R06] 判断命令是否存在
来源：http://mrw.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://coq.nwbrower.top

[R07] if 判断文件
来源：http://wrq.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wyb.yj20258.top

[R08] 数值比较
来源：http://qcj.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://avn.chenjidiqi.icu

[R09] 字符串比较
来源：http://ehu.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jje.shzxlz.cn

[R10] 正则匹配
来源：http://hnz.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tqf.yonumen.top

[R11] case 多分支
来源：http://ohc.nanxuanxn.top

case "$1" in
来源：http://cql.yanxiufei.cn

start) echo "启动" ;;
来源：http://lxn.nwbrower.top

stop)  echo "停止" ;;
来源：http://pcr.sysykeji.top

*)     echo "未知命令" ;;
来源：http://dov.sxryk.cn

esac
来源：http://fpa.jiagoushi.top

[R12] for 遍历文件
来源：http://sdb.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://uso.yj20258.top

[R13] for 计数循环
来源：http://qmz.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://fvu.ppjwa.cn

[R14] C 风格 for
来源：http://ois.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iad.meibo888.top

[R15] while 逐行读文件
来源：http://kzu.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nox.bjfxy.top

[R16] until 等待条件
来源：http://ewf.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gtv.jinqigfzy.top

[R17] 数组定义与取值
来源：http://lsk.shuidangran.top

arr=(a b c); echo "${arr[0]}"
来源：http://qgd.fktsv.cn

[R18] 遍历数组
来源：http://cjv.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://she.jinqigufen.top

[R19] 数组长度
来源：http://xkc.tian-w.cn

echo "${#arr[@]}"
来源：http://tgc.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://sma.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kiu.c1oappe.top

[R21] 字符串长度
来源：http://oqs.yangfankeji.com

echo "${#s}"
来源：http://lwl.snrcjt.cn

[R22] 截取子串
来源：http://any.wangdashe.top

echo "${s:0:5}"
来源：http://fvf.chenlongwang.top

[R23] 字符串替换
来源：http://arj.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gwd.gogol.net.cn

[R24] 大小写转换
来源：http://sdy.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://eff.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://thg.zhoulong.xyz


<!-- 参考信息 -->