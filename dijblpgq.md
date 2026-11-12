代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://bsk.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://ewe.bbcook.cn

Ruby: x.length;  x.size
来源：http://zvl.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oxm.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://xok.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://oye.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ris.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://njo.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iqs.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yqf.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://nmz.gaohongyu789.top

Ruby: a == b
来源：http://heh.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://soy.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://muz.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mhp.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://wpz.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vxo.ehwqpu.com

TS:   if (x == null) {}
来源：http://ubz.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gdr.zhengqikj.top

Go:   if x == nil {}
来源：http://ool.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hty.jianghu66.top

C#:   if (x is null) {}
来源：http://ycq.yanxiufei.cn

[P07] 防抖与节流
来源：http://jzk.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gut.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://wrd.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uff.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yum.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wag.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yrh.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://spt.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lsd.cashguo.top

[P08] 处理浮点精度问题
来源：http://rxm.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xac.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bar.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eav.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fue.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lbp.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ltu.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://erk.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lqc.shangyingyoupin.top

================================================================================
来源：http://sjh.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dle.52xcode.cn

================================================================================
来源：http://vex.nanxuanxn.top

[Q01] 创建表
来源：http://mhj.smart0.xyz

CREATE TABLE users (
来源：http://bmb.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvz.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://btr.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://brd.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mym.daxiang520.top

);
来源：http://fhg.c1oappe.top

[Q02] 创建带外键的表
来源：http://uap.mhx1999.top

CREATE TABLE orders (
来源：http://tnf.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxe.ehwqpu.com

user_id INT NOT NULL,
来源：http://xbb.hammf.cn

amount DECIMAL(10, 2),
来源：http://vvc.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rxf.sxryk.cn

);
来源：http://nkx.jqgfzy.top

[Q03] 增加列
来源：http://juw.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nbi.pengpengdd.cyou

[Q04] 修改列类型
来源：http://xsd.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sug.nwbrower.top

[Q05] 重命名列
来源：http://sgo.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hyi.ydzc1.top

[Q06] 删除列
来源：http://myv.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://mrh.9152youxi.cn

[Q07] 删除表
来源：http://fgo.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://wcx.shuidangran.top

[Q08] 创建普通索引
来源：http://ohn.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://atv.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://zxe.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bbu.yfazqb.com

[Q10] 插入单行
来源：http://iil.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rrl.yfazqb.com

[Q11] 一次插入多行
来源：http://dny.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzd.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://bvb.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://kyf.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qpc.xylfe.cn

[Q13] 忽略重复插入
来源：http://kct.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zzc.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://gia.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fgv.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kha.sufxvd.cn

[Q15] 查询全部
来源：http://ibg.yj20258888.top

SELECT * FROM users;
来源：http://twl.jqgufenzy.top

[Q16] 查询指定列
来源：http://vtq.shzxlz.cn

SELECT id, name FROM users;
来源：http://tnk.dianchejie.cn

[Q17] 条件查询
来源：http://urj.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://coy.yonumen.top

[Q18] 模糊匹配
来源：http://tzp.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nor.zhongyouzk.top

[Q19] 范围查询
来源：http://ocu.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xcq.jlsjyb.cn

[Q20] IN 列表
来源：http://afj.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://obv.tianlin.xyz

[Q21] 空值判断
来源：http://lts.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bvl.shuidangran.top

[Q22] 排序
来源：http://igt.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tmx.gaohongyu789.top

[Q23] 分页
来源：http://qqk.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uhz.gaohongyu789.top

[Q24] 去重
来源：http://hid.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://vnj.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://iyv.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wrt.cheryme.top

[Q26] 计数
来源：http://yot.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://bdd.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://jep.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://utm.mhx1999.top

[Q28] 求和与平均
来源：http://djg.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrk.chenlongwang.top

[Q29] 最大最小值
来源：http://glb.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wyp.hcnkem.com

[Q30] 分组统计
来源：http://ueo.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozt.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://dqj.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mmn.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://zyl.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bib.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nfb.yongpay.top

[Q33] 多列分组
来源：http://qml.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rex.nwbrower.top

[Q34] 每组取第一条
来源：http://zag.mhx1999.top

SELECT * FROM (
来源：http://clr.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jvh.yfazqb.com

) t WHERE rn = 1;
来源：http://gtd.gzhubu.top

[Q35] 内连接
来源：http://eut.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://epr.cqqwz.cn

[Q36] 左连接
来源：http://lvr.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://joj.vqdsnc.cn

[Q37] 右连接
来源：http://hhh.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://opq.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://iqq.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oej.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://suu.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://msg.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nll.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://myk.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cdi.fzhhl.top

[Q41] 多表连接
来源：http://vbz.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ttq.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://tmi.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://xyh.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://lse.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://mrb.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://der.sjlbkw.cn

[Q43] 标量子查询
来源：http://zxr.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zgj.yj20258888.top

[Q44] IN 子查询
来源：http://mka.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dhq.cheryme.top

[Q45] EXISTS 判断存在
来源：http://egn.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://foq.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://teu.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fai.gotoacloud.top

[Q47] 与平均值比较
来源：http://ayg.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsv.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://mwq.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qdc.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://daz.zhixingplan.top

[Q49] 更新单行
来源：http://rhv.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qur.chenzaomai.com

[Q50] 批量更新
来源：http://fef.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wjk.snrcjt.cn

[Q51] 用子查询更新
来源：http://upv.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vpi.xuanzx.com

[Q52] 删除指定行
来源：http://bgt.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://eid.bjfxy.top

[Q53] 按条件删除
来源：http://pwf.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bxy.yonumen.top

[Q54] 清空表
来源：http://agw.sweek.top

TRUNCATE TABLE logs;
来源：http://hii.cashguo.top

[Q55] 排名（并列占位）
来源：http://eot.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sde.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://ghh.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wsk.tarul.cn

[Q57] 行号
来源：http://tpm.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://noi.yongpay.top

[Q58] 累计求和
来源：http://lfd.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ljn.hysaishi.cn

[Q59] 分组内累计
来源：http://tsw.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gzs.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://gip.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tez.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpo.mhx1999.top

[Q61] 移动平均
来源：http://jsd.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://khu.havefunace.top

[Q62] 分组占比
来源：http://uyy.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lvl.tanke756.top

[Q63] 开启事务
来源：http://jsp.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vzu.zhiwuduotai.top

[Q64] 提交事务
来源：http://sof.ybcxt.top

COMMIT;
来源：http://ygr.quarkkingdee.top

[Q65] 回滚事务
来源：http://ypt.sysykeji.top

ROLLBACK;
来源：http://rqh.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://vob.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://srl.yj202588.top

[Q67] 设置隔离级别
来源：http://eap.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ppz.shanyushiyangkeji.top

[Q68] 保存点
来源：http://goj.yvedp.cn

SAVEPOINT sp1;
来源：http://zda.yueranfly.top

ROLLBACK TO sp1;
来源：http://vsd.ydjk.org.cn

[Q69] 查看执行计划
来源：http://apr.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ill.shzxlz.cn

[Q70] 更新统计信息
来源：http://rje.nanxuanxn.top

ANALYZE TABLE users;
来源：http://wkn.yonumen.top

[Q71] 查看建表语句
来源：http://mim.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ltd.gogol.net.cn

[Q72] 查看索引
来源：http://omm.cdnleiting.top

SHOW INDEX FROM users;
来源：http://app.vqdsnc.cn

[Q73] 查看表状态
来源：http://vqe.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ofr.jinqigfzy.top

[Q74] 强制使用索引
来源：http://uqv.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qeo.cucudq.cn

[Q75] 日期格式化
来源：http://nkn.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ciy.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zcu.cqqwz.cn

[Q76] 按天统计
来源：http://yan.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://umd.tarul.cn

[Q77] 时间加减
来源：http://sjn.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ria.tanke756.top

[Q78] 当前时间
来源：http://zdl.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uwf.316326.xyz

[Q79] 字符串拼接
来源：http://qrd.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yic.yonumen.top

[Q80] 字符串截取
来源：http://wkm.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tcb.ybcxt.top

[Q81] 字符串替换
来源：http://svb.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hnv.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://upc.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nyd.zycfv.cn

[Q83] 大小写转换
来源：http://ity.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zxx.fzhhl.top

[Q84] 去除首尾空格
来源：http://mkd.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://eaq.yuanzhike.top

[Q85] 数值取整
来源：http://umv.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bzg.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://uub.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ddg.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://xml.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jls.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://omc.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qew.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bna.fzhhl.top

[Q89] 判断表是否存在
来源：http://xey.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vew.ivvv.top

[Q90] 生成序号列
来源：http://fjy.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gha.zhoulong.xyz

================================================================================
来源：http://gul.yuanzhike.top

R. Bash 专题
来源：http://irx.zhengqikj.top

================================================================================
来源：http://gwn.bbcook.cn

[R01] shebang 与严格模式
来源：http://dmt.zdbjq.cn

#!/usr/bin/env bash
来源：http://nrw.yvedp.cn

set -euo pipefail
来源：http://mrv.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://jvy.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://qcx.yj202588.top

[R03] 只读变量
来源：http://kdu.feifeiyinyue.top

readonly PI=3.14
来源：http://dxq.wangdashe.top

[R04] 位置参数
来源：http://kuf.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ypa.ydjk.org.cn

[R05] 参数默认值
来源：http://cqy.zhaomingkeji.xyz

name="${1:-default}"
来源：http://bjm.jianghu66.top

[R06] 判断命令是否存在
来源：http://pnl.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://umh.cheryme.top

[R07] if 判断文件
来源：http://yzy.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uuz.hnxiangtu.top

[R08] 数值比较
来源：http://kbu.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://eqb.feifeiyinyue.top

[R09] 字符串比较
来源：http://rfz.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ige.sufxvd.cn

[R10] 正则匹配
来源：http://zpk.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wez.zhiwuduotai.top

[R11] case 多分支
来源：http://ykd.sxryk.cn

case "$1" in
来源：http://vsq.yueranfly.top

start) echo "启动" ;;
来源：http://gtq.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://xuo.sweek.top

*)     echo "未知命令" ;;
来源：http://sbu.jyoumei.cn

esac
来源：http://zkq.tianlin.xyz

[R12] for 遍历文件
来源：http://jjj.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://yno.zdqjudy.top

[R13] for 计数循环
来源：http://ofb.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://mrx.daria6918.cn

[R14] C 风格 for
来源：http://hny.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fvj.yongpay.top

[R15] while 逐行读文件
来源：http://ria.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bjm.zhoulong.xyz

[R16] until 等待条件
来源：http://akj.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pzn.jqgfzy.top

[R17] 数组定义与取值
来源：http://vsz.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://ryg.tian-w.cn

[R18] 遍历数组
来源：http://ffn.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yue.smart0.xyz

[R19] 数组长度
来源：http://rdo.fehbvm.com

echo "${#arr[@]}"
来源：http://kjw.vehdjk.com

[R20] 关联数组（字典）
来源：http://boe.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oyk.sxryk.cn

[R21] 字符串长度
来源：http://orw.zdqjudy.top

echo "${#s}"
来源：http://wva.birdmap.top

[R22] 截取子串
来源：http://bri.bjfxy.top

echo "${s:0:5}"
来源：http://yel.ydjk.org.cn

[R23] 字符串替换
来源：http://bfw.cheryme.top


<!-- 参考信息 -->