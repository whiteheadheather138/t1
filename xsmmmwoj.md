代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oiv.epnwcf.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apg.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ile.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://opn.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://jre.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://xww.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://pfq.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://wyy.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://dmi.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://oup.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fcn.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tel.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vog.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fbh.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://dnf.iojbl.cn

Ruby: a == b
来源：http://ver.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yoc.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lhu.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sqa.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://vll.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://esx.aizwys.cn

TS:   if (x == null) {}
来源：http://gds.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://kjr.cqqwz.cn

Go:   if x == nil {}
来源：http://hxx.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hyh.9152youxi.cn

C#:   if (x is null) {}
来源：http://ppc.iojbl.cn

[P07] 防抖与节流
来源：http://twu.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yjw.jinyuanbaomall.cn

PHP:  // 手写时间戳比较
来源：http://lkx.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwl.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxn.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hrd.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ywr.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vln.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://egf.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://bhn.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qnt.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://osz.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cqg.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tte.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://epj.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vne.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zpk.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://etm.c1oappe.top

================================================================================
来源：http://nwc.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vpf.fengsongda.top

================================================================================
来源：http://gvf.nwbrower.top

[Q01] 创建表
来源：http://ehr.pycfn.com

CREATE TABLE users (
来源：http://roa.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bfv.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://cye.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://iaw.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yhu.fehbvm.com

);
来源：http://zdm.yonumen.top

[Q02] 创建带外键的表
来源：http://usa.jqgfzy.top

CREATE TABLE orders (
来源：http://ygv.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ygg.jqgufenzy.top

user_id INT NOT NULL,
来源：http://alg.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://abh.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bka.zdbjq.cn

);
来源：http://oet.daria6918.cn

[Q03] 增加列
来源：http://qce.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://goy.sweek.top

[Q04] 修改列类型
来源：http://sms.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jhe.cheryme.top

[Q05] 重命名列
来源：http://jay.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vxu.aibaodan.cn

[Q06] 删除列
来源：http://tyu.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kvl.guowangkeji.top

[Q07] 删除表
来源：http://rej.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://zjr.jiagoushi.top

[Q08] 创建普通索引
来源：http://lht.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://raw.shuidangran.top

[Q09] 创建唯一索引
来源：http://ynp.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eab.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://wom.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qmn.c1oappe.top

[Q11] 一次插入多行
来源：http://dgy.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bbe.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://xtz.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://osg.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aex.xylfe.cn

[Q13] 忽略重复插入
来源：http://rtm.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xbp.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://ncz.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://buo.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sep.yanxiufei.cn

[Q15] 查询全部
来源：http://vtt.ctjpmb.com

SELECT * FROM users;
来源：http://tmj.dianchejie.cn

[Q16] 查询指定列
来源：http://vag.gotoacloud.top

SELECT id, name FROM users;
来源：http://ejp.iojbl.cn

[Q17] 条件查询
来源：http://ngy.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgr.jianghu66.top

[Q18] 模糊匹配
来源：http://wri.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fmp.sufxvd.cn

[Q19] 范围查询
来源：http://ynj.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ust.xuetiantiany.cn

[Q20] IN 列表
来源：http://zik.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://myr.nanxinkj.top

[Q21] 空值判断
来源：http://zis.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qpd.chenjidiqi.icu

[Q22] 排序
来源：http://lzi.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rdg.guowangkeji.top

[Q23] 分页
来源：http://ypc.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yej.ybcxt.top

[Q24] 去重
来源：http://ngd.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://sjz.yongpay.top

[Q25] 只取前 N 条
来源：http://xpk.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nsd.ydjk.org.cn

[Q26] 计数
来源：http://ngp.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://vap.zhoulong.xyz

[Q27] 条件计数
来源：http://xmc.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cjb.xinyue.icu

[Q28] 求和与平均
来源：http://yjb.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zoo.wangdashe.top

[Q29] 最大最小值
来源：http://got.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pej.shuidangran.top

[Q30] 分组统计
来源：http://yza.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://noq.dianchejie.cn

[Q31] 分组后过滤
来源：http://uci.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qsf.jianghu66.top

[Q32] 分组拼接字符串
来源：http://iir.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qus.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hlc.nanxinkj.top

[Q33] 多列分组
来源：http://wvx.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fkg.vehdjk.com

[Q34] 每组取第一条
来源：http://oyk.jinqigfzy.top

SELECT * FROM (
来源：http://tib.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nnf.hesvh.cn

) t WHERE rn = 1;
来源：http://gfe.uphjek.com

[Q35] 内连接
来源：http://uwf.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vvc.316326.xyz

[Q36] 左连接
来源：http://wte.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cnu.xuanzx.com

[Q37] 右连接
来源：http://pdh.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nua.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fui.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wuo.yongpay.top

[Q39] 自连接（查上下级）
来源：http://rjl.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zdc.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nfq.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jos.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://soo.dashuyun.cn

[Q41] 多表连接
来源：http://vkv.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uri.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://cnb.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://lhz.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://kex.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://qja.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wak.dianchejie.cn

[Q43] 标量子查询
来源：http://xhq.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwe.jqgfzy.top

[Q44] IN 子查询
来源：http://zbx.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rrr.pycfn.com

[Q45] EXISTS 判断存在
来源：http://yua.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pgv.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mjg.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rcd.pycfn.com

[Q47] 与平均值比较
来源：http://zrb.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xdh.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://jsi.bbcook.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hvs.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://upr.hammf.cn

[Q49] 更新单行
来源：http://bvt.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://drx.c1oappe.top

[Q50] 批量更新
来源：http://xar.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gwd.jqgufenzy.top

[Q51] 用子查询更新
来源：http://ydo.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xed.hesvh.cn

[Q52] 删除指定行
来源：http://vxx.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://dog.yonumen.top

[Q53] 按条件删除
来源：http://fgz.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nbj.hnqzz.top

[Q54] 清空表
来源：http://tmt.jianghu66.top

TRUNCATE TABLE logs;
来源：http://ugb.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://kpi.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kap.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://mps.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ero.yonumen.top

[Q57] 行号
来源：http://hnv.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dqg.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://plq.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ayq.tian-w.cn

[Q59] 分组内累计
来源：http://qxs.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pxn.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://bkf.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rdq.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tpr.ybcxt.top

[Q61] 移动平均
来源：http://igw.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dkx.ctjpmb.com

[Q62] 分组占比
来源：http://fac.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bbd.yonumen.top

[Q63] 开启事务
来源：http://ywh.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kty.daxiang520.top

[Q64] 提交事务
来源：http://mlm.ydzc1.top

COMMIT;
来源：http://ftp.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://ofb.daxiang520.top

ROLLBACK;
来源：http://umw.xylfe.cn

[Q66] 行锁查询
来源：http://kxi.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://njo.wangdashe.top

[Q67] 设置隔离级别
来源：http://nyp.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jwt.jinqigufen.top

[Q68] 保存点
来源：http://bkv.iojbl.cn

SAVEPOINT sp1;
来源：http://cnp.snrcjt.cn

ROLLBACK TO sp1;
来源：http://lhz.cucudq.cn

[Q69] 查看执行计划
来源：http://mqn.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qor.chenlongwang.top

[Q70] 更新统计信息
来源：http://min.xuanzx.com

ANALYZE TABLE users;
来源：http://shd.fehbvm.com

[Q71] 查看建表语句
来源：http://omu.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tnr.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://gyw.andypj.xyz

SHOW INDEX FROM users;
来源：http://zrr.aizwys.cn

[Q73] 查看表状态
来源：http://jcp.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tzv.yuanzhike.top

[Q74] 强制使用索引
来源：http://bxa.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://chc.gzhubu.top

[Q75] 日期格式化
来源：http://ldk.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qbc.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lfg.guannengcc.top

[Q76] 按天统计
来源：http://uus.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iny.yfazqb.com

[Q77] 时间加减
来源：http://dca.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eio.andypj.xyz

[Q78] 当前时间
来源：http://gne.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bpn.0kj1m.cn

[Q79] 字符串拼接
来源：http://sio.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uws.ydzc1.top

[Q80] 字符串截取
来源：http://oer.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssd.quarkkingdee.top

[Q81] 字符串替换
来源：http://usn.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lqs.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://dwe.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ufy.jianghu66.top

[Q83] 大小写转换
来源：http://hlh.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jtt.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://mkk.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://cpm.dianchejie.cn

[Q85] 数值取整
来源：http://pfu.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://std.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://fsy.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ejz.epnwcf.com

[Q87] JSON 字段做条件
来源：http://lha.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dwt.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://waz.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rxt.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uml.tanke756.top

[Q89] 判断表是否存在
来源：http://dir.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hpj.aizwys.cn

[Q90] 生成序号列
来源：http://rpe.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nmy.kuanghao11.cn

================================================================================
来源：http://xmm.nanxuanxn.top

R. Bash 专题
来源：http://eaq.zhoulong.xyz

================================================================================
来源：http://hwv.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://qdc.shuidangran.top

#!/usr/bin/env bash
来源：http://lwo.sufxvd.cn

set -euo pipefail
来源：http://qau.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://tsk.wangdashe.top

name="Tom"; echo "$name"
来源：http://qkg.jinghuilouyu.cn

[R03] 只读变量
来源：http://bzb.jlsjyb.cn

readonly PI=3.14
来源：http://bfo.tian-w.cn

[R04] 位置参数
来源：http://yoo.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uwl.gaohongyu789.top

[R05] 参数默认值
来源：http://lty.ivvv.top

name="${1:-default}"
来源：http://qsv.yj20258888.top

[R06] 判断命令是否存在
来源：http://xnv.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uru.shuidangran.top

[R07] if 判断文件
来源：http://hlc.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://spx.yvedp.cn

[R08] 数值比较
来源：http://yqq.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gvb.aibaodan.cn

[R09] 字符串比较
来源：http://rva.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cec.zhiwuduotai.top

[R10] 正则匹配
来源：http://ovb.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iah.yj20258888.top

[R11] case 多分支
来源：http://nxi.jqgfzy.top

case "$1" in
来源：http://pbr.hnxiangtu.top

start) echo "启动" ;;
来源：http://ifs.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://cef.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://hcg.jqgfzy.top

esac
来源：http://pke.yj202588.top

[R12] for 遍历文件
来源：http://yoe.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://dpu.nanxinkj.top

[R13] for 计数循环
来源：http://fwa.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://qll.0kj1m.cn

[R14] C 风格 for
来源：http://fvy.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rhf.gaohongyu789.top

[R15] while 逐行读文件
来源：http://nvj.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hlp.shangyingyoupin.top

[R16] until 等待条件
来源：http://cem.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hir.yj20258888.top

[R17] 数组定义与取值
来源：http://lkz.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yft.jlsjyb.cn

[R18] 遍历数组
来源：http://hcq.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpu.jinqigufen.top

[R19] 数组长度
来源：http://rro.9152youxi.cn

echo "${#arr[@]}"
来源：http://dni.xylfe.cn

[R20] 关联数组（字典）
来源：http://biq.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://egq.shanyushiyangtech.top

[R21] 字符串长度
来源：http://gmc.yfazqb.com


<!-- 参考信息 -->