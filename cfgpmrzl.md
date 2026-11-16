代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://xwe.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdi.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hwk.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ivr.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bnp.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhf.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://gll.chenzaomai.com

Ruby: a == b
来源：http://hkc.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tlp.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://foy.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qve.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://syc.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cmv.chenzaomai.com

TS:   if (x == null) {}
来源：http://ztp.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://kfb.cucudq.cn

Go:   if x == nil {}
来源：http://rci.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ptj.vqdsnc.cn

C#:   if (x is null) {}
来源：http://owx.yj20258.top

[P07] 防抖与节流
来源：http://fni.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zuw.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://orf.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyd.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewy.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fgj.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dgo.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yfg.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uko.yj20258888.top

[P08] 处理浮点精度问题
来源：http://vfx.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dou.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ysj.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vke.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xup.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gtx.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mso.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jrp.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zuh.tanke756.top

================================================================================
来源：http://sgl.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jjw.jinqigufen.top

================================================================================
来源：http://hxz.yj202588.top

[Q01] 创建表
来源：http://jhw.aibaodan.cn

CREATE TABLE users (
来源：http://rub.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vlw.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://zpd.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://kks.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sum.yuxming.cn

);
来源：http://miq.sxryk.cn

[Q02] 创建带外键的表
来源：http://koc.fktsv.cn

CREATE TABLE orders (
来源：http://pbt.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mfw.ivvv.top

user_id INT NOT NULL,
来源：http://ijy.yuxming.cn

amount DECIMAL(10, 2),
来源：http://xye.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://unu.bjfxy.top

);
来源：http://qce.hnqzz.top

[Q03] 增加列
来源：http://svr.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hll.pycfn.com

[Q04] 修改列类型
来源：http://mot.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eau.yangfankeji.com

[Q05] 重命名列
来源：http://pky.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nwd.gogol.net.cn

[Q06] 删除列
来源：http://icr.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kpf.dianchejie.cn

[Q07] 删除表
来源：http://wut.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://gfs.zycfv.cn

[Q08] 创建普通索引
来源：http://nao.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fhg.svipenyu.cn

[Q09] 创建唯一索引
来源：http://qle.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vzn.jinqigufen.top

[Q10] 插入单行
来源：http://uux.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ktb.jqgfzy.top

[Q11] 一次插入多行
来源：http://bar.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fbt.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://kua.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://bzk.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://puj.aibaodan.cn

[Q13] 忽略重复插入
来源：http://wca.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vlp.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://qbj.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://thb.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pgk.tianlin.xyz

[Q15] 查询全部
来源：http://dix.shuidangran.top

SELECT * FROM users;
来源：http://csd.zycfv.cn

[Q16] 查询指定列
来源：http://snj.hfpthk.cn

SELECT id, name FROM users;
来源：http://uzd.vehdjk.com

[Q17] 条件查询
来源：http://spt.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kzx.yj20258.top

[Q18] 模糊匹配
来源：http://cee.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ref.nanxinkj.top

[Q19] 范围查询
来源：http://opt.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hxn.dashuyun.cn

[Q20] IN 列表
来源：http://lhc.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uih.ydjk.org.cn

[Q21] 空值判断
来源：http://itg.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bfc.meibo888.top

[Q22] 排序
来源：http://mma.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nyg.jinqigufen.top

[Q23] 分页
来源：http://zul.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tlu.yj20258888.top

[Q24] 去重
来源：http://lqa.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://qll.cqqwz.cn

[Q25] 只取前 N 条
来源：http://qer.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kif.nanxuanxn.top

[Q26] 计数
来源：http://gru.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://rvw.nanxuanxn.top

[Q27] 条件计数
来源：http://xmp.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eqh.sxryk.cn

[Q28] 求和与平均
来源：http://pis.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vys.0kj1m.cn

[Q29] 最大最小值
来源：http://tyo.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vmw.daxiang520.top

[Q30] 分组统计
来源：http://bcz.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://shy.jyoumei.cn

[Q31] 分组后过滤
来源：http://jja.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kto.yueranfly.top

[Q32] 分组拼接字符串
来源：http://kda.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vsx.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://afb.epnwcf.com

[Q33] 多列分组
来源：http://yvm.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wpc.dianchejie.cn

[Q34] 每组取第一条
来源：http://ydh.wangdashe.top

SELECT * FROM (
来源：http://aay.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hzy.snrcjt.cn

) t WHERE rn = 1;
来源：http://lbt.ywan-chungtsiang.top

[Q35] 内连接
来源：http://ehf.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dbh.nanxuanxn.top

[Q36] 左连接
来源：http://gix.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://igv.tanke756.top

[Q37] 右连接
来源：http://pel.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://myo.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://qnp.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://crz.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://tde.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tva.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zqn.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eee.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sgt.cqqwz.cn

[Q41] 多表连接
来源：http://ywj.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ofb.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://kkr.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://pkh.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://wlp.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://whm.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://szc.yonumen.top

[Q43] 标量子查询
来源：http://bmj.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nse.gogol.net.cn

[Q44] IN 子查询
来源：http://gri.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ceh.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://vmi.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwu.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zog.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cdy.snrcjt.cn

[Q47] 与平均值比较
来源：http://uto.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://trc.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://alq.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmt.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://pol.jinqigfzy.top

[Q49] 更新单行
来源：http://bmf.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mzj.chenlongwang.top

[Q50] 批量更新
来源：http://erh.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uzm.redwolf501.top

[Q51] 用子查询更新
来源：http://fbx.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxl.birdmap.top

[Q52] 删除指定行
来源：http://yln.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://cpc.hfpthk.cn

[Q53] 按条件删除
来源：http://gnb.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nop.daria6918.cn

[Q54] 清空表
来源：http://oqh.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://vht.birdmap.top

[Q55] 排名（并列占位）
来源：http://zwp.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cxh.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://nyk.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zgq.jqgufenzy.top

[Q57] 行号
来源：http://hnd.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://clw.chenzaomai.com

[Q58] 累计求和
来源：http://hle.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pyn.jqgfzy.top

[Q59] 分组内累计
来源：http://uqn.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqo.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://edn.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cif.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://igg.chenlongwang.top

[Q61] 移动平均
来源：http://rud.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gyq.mhx1999.top

[Q62] 分组占比
来源：http://gqg.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gsq.shanyushiyangtech.top

[Q63] 开启事务
来源：http://knc.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ans.hcnkem.com

[Q64] 提交事务
来源：http://irs.xuetiantiany.cn

COMMIT;
来源：http://dat.ehwqpu.com

[Q65] 回滚事务
来源：http://dwg.tanke756.top

ROLLBACK;
来源：http://lzr.zhixingplan.top

[Q66] 行锁查询
来源：http://nfq.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://net.hysaishi.cn

[Q67] 设置隔离级别
来源：http://qsf.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mcs.zhijiandao.cn

[Q68] 保存点
来源：http://iql.hnqzz.top

SAVEPOINT sp1;
来源：http://yfq.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://sty.hywenlv.cn

[Q69] 查看执行计划
来源：http://bhd.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://emf.ppjwa.cn

[Q70] 更新统计信息
来源：http://oqz.yuxming.cn

ANALYZE TABLE users;
来源：http://nwu.hesvh.cn

[Q71] 查看建表语句
来源：http://ewr.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aqe.meibo888.top

[Q72] 查看索引
来源：http://vcx.hcnkem.com

SHOW INDEX FROM users;
来源：http://nov.gzhubu.top

[Q73] 查看表状态
来源：http://uos.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://ubq.pycfn.com

[Q74] 强制使用索引
来源：http://uzt.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://haq.vqdsnc.cn

[Q75] 日期格式化
来源：http://dld.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ywf.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qjo.tarul.cn

[Q76] 按天统计
来源：http://isr.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vkc.andypj.xyz

[Q77] 时间加减
来源：http://ycl.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sxh.yanxiufei.cn

[Q78] 当前时间
来源：http://mck.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://psp.xinyue.icu

[Q79] 字符串拼接
来源：http://vyn.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cmh.dianchejie.cn

[Q80] 字符串截取
来源：http://fkn.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tgm.chenzaomai.com

[Q81] 字符串替换
来源：http://mhw.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vgm.yj20258.top

[Q82] 字符长度与字节长度
来源：http://sav.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sxy.ydjk.org.cn

[Q83] 大小写转换
来源：http://pdk.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://goy.sweek.top

[Q84] 去除首尾空格
来源：http://oss.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://upy.wangdashe.top

[Q85] 数值取整
来源：http://gck.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://znw.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://yih.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dbq.316326.xyz

[Q87] JSON 字段做条件
来源：http://kkr.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ijd.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://zvc.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lqz.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pry.jyoumei.cn

[Q89] 判断表是否存在
来源：http://bzq.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qbg.tarul.cn

[Q90] 生成序号列
来源：http://jrm.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://omt.chenjidiqi.icu

================================================================================
来源：http://pvk.52xcode.cn

R. Bash 专题
来源：http://mzm.yj202588.top

================================================================================
来源：http://mqj.cucudq.cn

[R01] shebang 与严格模式
来源：http://azb.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://xvc.epnwcf.com

set -euo pipefail
来源：http://ncb.tianlin.xyz

[R02] 变量赋值与使用
来源：http://dkc.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://mcp.jinqigufen.top

[R03] 只读变量
来源：http://uxa.hnqzz.top

readonly PI=3.14
来源：http://rne.jyoumei.cn

[R04] 位置参数
来源：http://yku.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jyi.daxiang520.top

[R05] 参数默认值
来源：http://wnw.hywenlv.cn

name="${1:-default}"
来源：http://tok.316326.xyz

[R06] 判断命令是否存在
来源：http://ccs.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dbf.meibo888.top

[R07] if 判断文件
来源：http://yvb.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xqs.havefunace.top

[R08] 数值比较
来源：http://twf.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rwb.tian-w.cn

[R09] 字符串比较
来源：http://ccm.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppt.aizwys.cn

[R10] 正则匹配
来源：http://fbg.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yth.guowangkeji.top

[R11] case 多分支
来源：http://uej.daxiang520.top

case "$1" in
来源：http://uwg.gaohongyu789.top

start) echo "启动" ;;
来源：http://fcx.cashguo.top

stop)  echo "停止" ;;
来源：http://qcw.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://wzv.jianghu66.top

esac
来源：http://drt.nanxuanxn.top

[R12] for 遍历文件
来源：http://awl.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://tte.yfazqb.com

[R13] for 计数循环
来源：http://sez.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xtv.yangfankeji.com

[R14] C 风格 for
来源：http://nhr.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbs.havefunace.top

[R15] while 逐行读文件
来源：http://cib.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vzg.ivvv.top

[R16] until 等待条件
来源：http://mdl.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dbh.birdmap.top

[R17] 数组定义与取值
来源：http://tpy.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hls.aizwys.cn

[R18] 遍历数组
来源：http://elc.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wvg.shanyushiyangtech.top

[R19] 数组长度
来源：http://znp.guowangkeji.top

echo "${#arr[@]}"
来源：http://uuc.xylfe.cn

[R20] 关联数组（字典）
来源：http://stw.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://trx.sweek.top

[R21] 字符串长度
来源：http://kfe.tarul.cn

echo "${#s}"
来源：http://mnk.cqqwz.cn

[R22] 截取子串
来源：http://ncw.guowangkeji.top

echo "${s:0:5}"
来源：http://dhf.chenlongwang.top

[R23] 字符串替换
来源：http://gni.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iad.zhoulong.xyz

[R24] 大小写转换
来源：http://shw.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://ftx.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://awy.gzhubu.top


<!-- 参考信息 -->