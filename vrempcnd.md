代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://cib.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://iqn.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://rye.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ejs.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://yfb.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fru.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jom.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bla.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://juk.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://stt.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xjh.gaohongyu789.top

Ruby: a == b
来源：http://rhr.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mjj.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rsu.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dea.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://uqy.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://taz.jqgufenzy.top

TS:   if (x == null) {}
来源：http://teg.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hle.zdbjq.cn

Go:   if x == nil {}
来源：http://ans.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://elm.cashguo.top

C#:   if (x is null) {}
来源：http://ddj.yuanzhike.top

[P07] 防抖与节流
来源：http://oyx.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oqr.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://kug.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nqh.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iua.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hba.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmp.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qzc.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aku.shuidangran.top

[P08] 处理浮点精度问题
来源：http://itn.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://why.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kjc.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://knu.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qqv.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zgi.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pib.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vpo.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pcf.cdnleiting.top

================================================================================
来源：http://wek.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pyl.kuanghao11.cn

================================================================================
来源：http://byx.9152youxi.cn

[Q01] 创建表
来源：http://iqu.hammf.cn

CREATE TABLE users (
来源：http://coz.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayw.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://rzr.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://wqk.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bxr.sxryk.cn

);
来源：http://zqa.yueranfly.top

[Q02] 创建带外键的表
来源：http://ckd.zhiwuduotai.top

CREATE TABLE orders (
来源：http://ard.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tim.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://viw.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://dnq.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://edj.ivvv.top

);
来源：http://vvb.ehwqpu.com

[Q03] 增加列
来源：http://teg.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tig.fehbvm.com

[Q04] 修改列类型
来源：http://qpf.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vtu.yj20258888.top

[Q05] 重命名列
来源：http://xxa.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://olk.zhaomingkeji.xyz

[Q06] 删除列
来源：http://rxp.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://dnh.jqgufenzy.top

[Q07] 删除表
来源：http://gva.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://qxf.sweek.top

[Q08] 创建普通索引
来源：http://vdu.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://myb.zdbjq.cn

[Q09] 创建唯一索引
来源：http://owb.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yja.smart0.xyz

[Q10] 插入单行
来源：http://wfo.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bos.dianchejie.cn

[Q11] 一次插入多行
来源：http://fky.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uhm.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://fcr.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://too.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://due.andypj.xyz

[Q13] 忽略重复插入
来源：http://rvc.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ddb.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://lzd.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pda.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://idl.redwolf501.top

[Q15] 查询全部
来源：http://ncv.aizwys.cn

SELECT * FROM users;
来源：http://lpv.bbcook.cn

[Q16] 查询指定列
来源：http://fld.guannengcc.top

SELECT id, name FROM users;
来源：http://glt.cheryme.top

[Q17] 条件查询
来源：http://yjx.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cjd.sweek.top

[Q18] 模糊匹配
来源：http://gyg.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jgm.xinyue.icu

[Q19] 范围查询
来源：http://dmi.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ufr.zhoulong.xyz

[Q20] IN 列表
来源：http://jvf.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gdr.birdmap.top

[Q21] 空值判断
来源：http://cag.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zbv.yvedp.cn

[Q22] 排序
来源：http://tvy.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ddr.iojbl.cn

[Q23] 分页
来源：http://lro.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tje.ctjpmb.com

[Q24] 去重
来源：http://hkt.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://lnd.ybcxt.top

[Q25] 只取前 N 条
来源：http://kke.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwi.tianlin.xyz

[Q26] 计数
来源：http://pze.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://bqe.yvedp.cn

[Q27] 条件计数
来源：http://inb.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ugv.guannengcc.top

[Q28] 求和与平均
来源：http://hzm.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://llx.nwbrower.top

[Q29] 最大最小值
来源：http://ldy.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fua.jiagoushi.top

[Q30] 分组统计
来源：http://mhx.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fvv.quarkkingdee.top

[Q31] 分组后过滤
来源：http://wic.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fgr.mhx1999.top

[Q32] 分组拼接字符串
来源：http://dba.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tsf.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jdn.jlsjyb.cn

[Q33] 多列分组
来源：http://jrr.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oqs.snrcjt.cn

[Q34] 每组取第一条
来源：http://wkt.jianghu66.top

SELECT * FROM (
来源：http://qzt.daria6918.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cik.bjfxy.top

) t WHERE rn = 1;
来源：http://pbx.daxiang520.top

[Q35] 内连接
来源：http://qvh.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lwm.zhengqikj.top

[Q36] 左连接
来源：http://ick.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://akn.guannengcc.top

[Q37] 右连接
来源：http://uhl.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oez.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://amz.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bql.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://csk.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vrv.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://onm.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fhf.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cvp.jqgufenzy.top

[Q41] 多表连接
来源：http://lqq.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://mfr.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://fyu.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://glp.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://eru.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://plh.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xvr.jyoumei.cn

[Q43] 标量子查询
来源：http://xxx.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hyo.svipenyu.cn

[Q44] IN 子查询
来源：http://gpw.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ngv.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://jhi.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hto.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://cbe.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azh.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://fzg.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pxk.yj20258.top

[Q48] CTE 公用表表达式
来源：http://kzh.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://izq.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://odt.wangshuangyany.cn

[Q49] 更新单行
来源：http://ymy.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dvy.zdbjq.cn

[Q50] 批量更新
来源：http://ojx.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ptq.havefunace.top

[Q51] 用子查询更新
来源：http://lue.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://loe.fehbvm.com

[Q52] 删除指定行
来源：http://ptj.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://ncs.snrcjt.cn

[Q53] 按条件删除
来源：http://zcw.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://azh.ybcxt.top

[Q54] 清空表
来源：http://rpt.fzhhl.top

TRUNCATE TABLE logs;
来源：http://eas.havefunace.top

[Q55] 排名（并列占位）
来源：http://vff.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pau.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://ybs.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ysn.andypj.xyz

[Q57] 行号
来源：http://exm.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qaj.zhixingplan.top

[Q58] 累计求和
来源：http://prk.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wvg.jlsjyb.cn

[Q59] 分组内累计
来源：http://hhs.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://too.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://yhj.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bap.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pcn.havefunace.top

[Q61] 移动平均
来源：http://dki.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uby.yonumen.top

[Q62] 分组占比
来源：http://naa.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kbx.chenzaomai.com

[Q63] 开启事务
来源：http://khv.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fht.52xcode.cn

[Q64] 提交事务
来源：http://nob.tanke756.top

COMMIT;
来源：http://jtw.cheryme.top

[Q65] 回滚事务
来源：http://bxa.hnqzz.top

ROLLBACK;
来源：http://qje.hcnkem.com

[Q66] 行锁查询
来源：http://jmd.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cha.hfpthk.cn

[Q67] 设置隔离级别
来源：http://gew.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wog.zdbjq.cn

[Q68] 保存点
来源：http://vpn.zdbjq.cn

SAVEPOINT sp1;
来源：http://dyk.9152youxi.cn

ROLLBACK TO sp1;
来源：http://yov.hcnkem.com

[Q69] 查看执行计划
来源：http://iit.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://goo.cheryme.top

[Q70] 更新统计信息
来源：http://wlt.0kj1m.cn

ANALYZE TABLE users;
来源：http://glo.chenlongwang.top

[Q71] 查看建表语句
来源：http://yah.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yrt.birdmap.top

[Q72] 查看索引
来源：http://zue.tian-w.cn

SHOW INDEX FROM users;
来源：http://krq.guannengcc.top

[Q73] 查看表状态
来源：http://crh.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://yob.ehwqpu.com

[Q74] 强制使用索引
来源：http://jzr.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfl.daria6918.cn

[Q75] 日期格式化
来源：http://mpt.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wtt.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zvz.0kj1m.cn

[Q76] 按天统计
来源：http://yyx.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hhm.vqdsnc.cn

[Q77] 时间加减
来源：http://yda.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hce.jqgfzy.top

[Q78] 当前时间
来源：http://fsm.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfy.zdbjq.cn

[Q79] 字符串拼接
来源：http://prt.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mbm.birdmap.top

[Q80] 字符串截取
来源：http://wqc.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cis.epnwcf.com

[Q81] 字符串替换
来源：http://nzx.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fmc.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://jmm.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xmz.shzxlz.cn

[Q83] 大小写转换
来源：http://ict.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zlv.birdmap.top

[Q84] 去除首尾空格
来源：http://wio.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://xce.jinqigufen.top

[Q85] 数值取整
来源：http://gmf.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cyx.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://cpz.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://odu.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://pza.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kgk.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://lcp.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dqw.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dyn.tanke756.top

[Q89] 判断表是否存在
来源：http://zpn.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ytr.ivvv.top

[Q90] 生成序号列
来源：http://syz.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://erp.yongpay.top

================================================================================
来源：http://cdi.redwolf501.top

R. Bash 专题
来源：http://zmu.shanyushiyangtech.top

================================================================================
来源：http://jqu.birdmap.top

[R01] shebang 与严格模式
来源：http://smw.hcnkem.com

#!/usr/bin/env bash
来源：http://jug.zhaomingkeji.xyz

set -euo pipefail
来源：http://scc.tarul.cn

[R02] 变量赋值与使用
来源：http://brg.gotoacloud.top

name="Tom"; echo "$name"
来源：http://ukw.yj202588.top

[R03] 只读变量
来源：http://naa.nanxinkj.top

readonly PI=3.14
来源：http://mun.hesvh.cn

[R04] 位置参数
来源：http://mqv.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tem.shzxlz.cn

[R05] 参数默认值
来源：http://rad.epnwcf.com

name="${1:-default}"
来源：http://dcs.tanke756.top

[R06] 判断命令是否存在
来源：http://dxx.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eer.yueranfly.top

[R07] if 判断文件
来源：http://yln.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nnx.snrcjt.cn

[R08] 数值比较
来源：http://dox.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rjm.cqqwz.cn

[R09] 字符串比较
来源：http://iwy.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uhh.chenzaomai.com

[R10] 正则匹配
来源：http://tqj.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://faf.havefunace.top

[R11] case 多分支
来源：http://jvh.cdnleiting.top

case "$1" in
来源：http://sut.gzhubu.top

start) echo "启动" ;;
来源：http://nyt.xuanzx.com

stop)  echo "停止" ;;
来源：http://ikn.bjfxy.top

*)     echo "未知命令" ;;
来源：http://fuq.iojbl.cn

esac
来源：http://zgc.yongpay.top

[R12] for 遍历文件
来源：http://ijj.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://mau.zhixingplan.top

[R13] for 计数循环
来源：http://ptg.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://zye.redwolf501.top

[R14] C 风格 for
来源：http://rur.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sad.xuanzx.com

[R15] while 逐行读文件
来源：http://sfj.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hrj.xuetiantiany.cn

[R16] until 等待条件
来源：http://jvq.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kkb.gaohongyu789.top

[R17] 数组定义与取值
来源：http://bnu.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mae.yj202588.top

[R18] 遍历数组
来源：http://nlh.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vhk.xylfe.cn

[R19] 数组长度
来源：http://yut.daxiang520.top

echo "${#arr[@]}"
来源：http://clh.cdnleiting.top

[R20] 关联数组（字典）
来源：http://lcl.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ilj.cdnleiting.top

[R21] 字符串长度
来源：http://izn.ydzc1.top

echo "${#s}"
来源：http://snp.daria6918.cn

[R22] 截取子串
来源：http://sqq.shzxlz.cn

echo "${s:0:5}"
来源：http://yon.hongshengwenyu.top

[R23] 字符串替换
来源：http://nvu.fzhhl.top


<!-- 参考信息 -->