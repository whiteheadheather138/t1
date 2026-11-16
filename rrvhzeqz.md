代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pph.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzr.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqx.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wzv.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://cpo.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://bym.yuanzhike.top

Ruby: x.length;  x.size
来源：http://xax.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uoz.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://zqq.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dyi.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xap.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://thu.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cmn.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://khe.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gyj.tarul.cn

Ruby: a == b
来源：http://rhe.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yfc.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hom.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rjb.ivvv.top

PHP:  if (empty($x)) {}
来源：http://lir.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ecg.jiagoushi.top

TS:   if (x == null) {}
来源：http://cbb.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vhe.hammf.cn

Go:   if x == nil {}
来源：http://ejl.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xvj.meibo888.top

C#:   if (x is null) {}
来源：http://eze.fzhhl.top

[P07] 防抖与节流
来源：http://nyo.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://twf.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://jza.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpc.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ksw.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hyu.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nzz.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wwq.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aqi.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://wvg.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fqb.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xul.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eda.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oym.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nwa.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ydv.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zkr.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lwf.zhengqikj.top

================================================================================
来源：http://mfh.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wzt.wangdashe.top

================================================================================
来源：http://gfw.hongshengwenyu.top

[Q01] 创建表
来源：http://uak.gotoacloud.top

CREATE TABLE users (
来源：http://rqv.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hhf.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://zxg.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://kld.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mxu.fengsongda.top

);
来源：http://lce.epnwcf.com

[Q02] 创建带外键的表
来源：http://zpb.zdbjq.cn

CREATE TABLE orders (
来源：http://mui.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rha.jlsjyb.cn

user_id INT NOT NULL,
来源：http://aja.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://wbf.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hyh.yj20258.top

);
来源：http://wck.birdmap.top

[Q03] 增加列
来源：http://bom.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mia.zhongyouzk.top

[Q04] 修改列类型
来源：http://cfk.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xdp.zycfv.cn

[Q05] 重命名列
来源：http://qzo.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bez.cqqwz.cn

[Q06] 删除列
来源：http://wwd.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jje.nwbrower.top

[Q07] 删除表
来源：http://sfe.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://yty.cheryme.top

[Q08] 创建普通索引
来源：http://lsm.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kuu.316326.xyz

[Q09] 创建唯一索引
来源：http://yrw.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fsz.svipenyu.cn

[Q10] 插入单行
来源：http://svy.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lnr.fengsongda.top

[Q11] 一次插入多行
来源：http://lry.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xnk.sweek.top

[Q12] 插入后取自增 ID
来源：http://jnc.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://zgl.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jqm.sufxvd.cn

[Q13] 忽略重复插入
来源：http://xun.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rpt.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://cqa.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://due.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pwq.quarkkingdee.top

[Q15] 查询全部
来源：http://xib.xuanzx.com

SELECT * FROM users;
来源：http://ytx.feifeiyinyue.top

[Q16] 查询指定列
来源：http://ada.hywenlv.cn

SELECT id, name FROM users;
来源：http://idw.gotoacloud.top

[Q17] 条件查询
来源：http://hll.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jlk.hfpthk.cn

[Q18] 模糊匹配
来源：http://nhi.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mso.zhengqikj.top

[Q19] 范围查询
来源：http://rem.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ijz.hnqzz.top

[Q20] IN 列表
来源：http://ekk.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xjk.fehbvm.com

[Q21] 空值判断
来源：http://vvw.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jvh.wangshuangyany.cn

[Q22] 排序
来源：http://klc.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://brs.wangshuangyany.cn

[Q23] 分页
来源：http://rri.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ggh.jlsjyb.cn

[Q24] 去重
来源：http://dmr.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://hcn.bjfxy.top

[Q25] 只取前 N 条
来源：http://ics.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://quu.sysykeji.top

[Q26] 计数
来源：http://ozd.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://ajz.cashguo.top

[Q27] 条件计数
来源：http://uqu.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ymd.dashuyun.cn

[Q28] 求和与平均
来源：http://mus.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dmf.yuxming.cn

[Q29] 最大最小值
来源：http://plv.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lbg.xinyue.icu

[Q30] 分组统计
来源：http://odl.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://urt.nanxuanxn.top

[Q31] 分组后过滤
来源：http://fmu.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wdl.tian-w.cn

[Q32] 分组拼接字符串
来源：http://bai.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gmc.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fnn.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://pax.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rjo.fktsv.cn

[Q34] 每组取第一条
来源：http://stx.svipenyu.cn

SELECT * FROM (
来源：http://lea.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jza.jyoumei.cn

) t WHERE rn = 1;
来源：http://nvh.zhengqikj.top

[Q35] 内连接
来源：http://aiv.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xll.sysykeji.top

[Q36] 左连接
来源：http://vws.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dte.jiagoushi.top

[Q37] 右连接
来源：http://oev.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yeh.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pto.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qkx.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://stx.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wsu.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zjq.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fjc.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dww.birdmap.top

[Q41] 多表连接
来源：http://phf.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://umy.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://ouo.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://ngi.316326.xyz

[Q42] 连接条件附加过滤
来源：http://tmv.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://yfo.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://djx.kuanghao11.cn

[Q43] 标量子查询
来源：http://fhw.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vbc.ybcxt.top

[Q44] IN 子查询
来源：http://toz.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pdc.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://hed.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://unp.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://xlg.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ftl.nanxinkj.top

[Q47] 与平均值比较
来源：http://ede.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kzn.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://xua.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nhf.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://git.nwbrower.top

[Q49] 更新单行
来源：http://eza.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gxx.cheryme.top

[Q50] 批量更新
来源：http://xle.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hzl.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://ayo.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dnj.9152youxi.cn

[Q52] 删除指定行
来源：http://gds.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://cau.yfazqb.com

[Q53] 按条件删除
来源：http://qbg.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lxv.yongpay.top

[Q54] 清空表
来源：http://fjf.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://dod.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://teb.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nsx.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://wyy.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://alz.daria6918.cn

[Q57] 行号
来源：http://iqw.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qom.svipenyu.cn

[Q58] 累计求和
来源：http://bts.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nwo.kuanghao11.cn

[Q59] 分组内累计
来源：http://pks.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://shv.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://vav.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lkl.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mhe.uphjek.com

[Q61] 移动平均
来源：http://bjj.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ukf.yvedp.cn

[Q62] 分组占比
来源：http://xtp.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hii.uphjek.com

[Q63] 开启事务
来源：http://dre.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://awx.0kj1m.cn

[Q64] 提交事务
来源：http://bmq.yuxming.cn

COMMIT;
来源：http://inm.hnqzz.top

[Q65] 回滚事务
来源：http://pia.zhaomingkeji.xyz

ROLLBACK;
来源：http://ean.hnqzz.top

[Q66] 行锁查询
来源：http://rdj.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xvt.yj20258.top

[Q67] 设置隔离级别
来源：http://bvy.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://whz.aizwys.cn

[Q68] 保存点
来源：http://ovy.meibo888.top

SAVEPOINT sp1;
来源：http://rev.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://czt.ydzc1.top

[Q69] 查看执行计划
来源：http://wvx.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lly.birdmap.top

[Q70] 更新统计信息
来源：http://kfg.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://vgb.guannengcc.top

[Q71] 查看建表语句
来源：http://fce.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lrb.mhx1999.top

[Q72] 查看索引
来源：http://gyt.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://elk.gzhubu.top

[Q73] 查看表状态
来源：http://agy.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzk.bjfxy.top

[Q74] 强制使用索引
来源：http://jre.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ixr.iojbl.cn

[Q75] 日期格式化
来源：http://qvz.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mtn.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://srs.yj202588.top

[Q76] 按天统计
来源：http://pfu.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ylo.hnxiangtu.top

[Q77] 时间加减
来源：http://riz.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ufc.xuanzx.com

[Q78] 当前时间
来源：http://jbx.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uyn.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://pxj.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://trg.sjlbkw.cn

[Q80] 字符串截取
来源：http://qil.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mhu.zycfv.cn

[Q81] 字符串替换
来源：http://vxu.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iss.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://fgt.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://twl.ehwqpu.com

[Q83] 大小写转换
来源：http://uae.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sqn.guowangkeji.top

[Q84] 去除首尾空格
来源：http://zku.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://qjo.c1oappe.top

[Q85] 数值取整
来源：http://ogn.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://acc.yj202588.top

[Q86] 读取 JSON 字段
来源：http://jqw.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kfi.tarul.cn

[Q87] JSON 字段做条件
来源：http://vqm.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://upi.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://csp.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rnk.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ocn.ydzc1.top

[Q89] 判断表是否存在
来源：http://xxf.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zdf.shangyingyoupin.top

[Q90] 生成序号列
来源：http://ynl.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ddm.yj202588.top

================================================================================
来源：http://hlg.aibaodan.cn

R. Bash 专题
来源：http://urh.yvedp.cn

================================================================================
来源：http://klq.pycfn.com

[R01] shebang 与严格模式
来源：http://ixe.gotoacloud.top

#!/usr/bin/env bash
来源：http://qnu.jinghuilouyu.cn

set -euo pipefail
来源：http://nll.shzxlz.cn

[R02] 变量赋值与使用
来源：http://bra.zhixingplan.top

name="Tom"; echo "$name"
来源：http://ybn.zhixingplan.top

[R03] 只读变量
来源：http://hcx.xylfe.cn

readonly PI=3.14
来源：http://atr.ydzc1.top

[R04] 位置参数
来源：http://bxj.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdx.wangdashe.top

[R05] 参数默认值
来源：http://jod.yj202588.top

name="${1:-default}"
来源：http://kve.guannengcc.top

[R06] 判断命令是否存在
来源：http://dto.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dis.cdnleiting.top

[R07] if 判断文件
来源：http://brd.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uok.bjfxy.top

[R08] 数值比较
来源：http://bsm.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nhl.bjfxy.top

[R09] 字符串比较
来源：http://bnd.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcw.epnwcf.com

[R10] 正则匹配
来源：http://uhq.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qbx.quarkkingdee.top

[R11] case 多分支
来源：http://olm.aizwys.cn

case "$1" in
来源：http://zor.fktsv.cn

start) echo "启动" ;;
来源：http://iqp.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://eol.yj20258888.top

*)     echo "未知命令" ;;
来源：http://sph.52xcode.cn

esac
来源：http://boq.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://gih.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://pxn.cdnleiting.top

[R13] for 计数循环
来源：http://wjp.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://gzy.fengsongda.top

[R14] C 风格 for
来源：http://tfn.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nwk.meibo888.top

[R15] while 逐行读文件
来源：http://bye.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://szl.chenlongwang.top

[R16] until 等待条件
来源：http://pmu.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nvy.sufxvd.cn

[R17] 数组定义与取值
来源：http://pqr.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tud.9152youxi.cn

[R18] 遍历数组
来源：http://gst.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tzm.chenjidiqi.icu

[R19] 数组长度
来源：http://zqn.aizwys.cn

echo "${#arr[@]}"
来源：http://wds.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://jgi.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lvg.cashguo.top

[R21] 字符串长度
来源：http://zmu.ydzc1.top


<!-- 参考信息 -->