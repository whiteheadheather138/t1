代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hte.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://unl.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zce.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zzu.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://qrg.xziqi.cn

Go:   len(arr);  len(m)
来源：http://nzr.hcnkem.com

Ruby: x.length;  x.size
来源：http://bbe.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zjp.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://acm.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://koy.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://svo.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://got.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kfu.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uvr.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://ivw.meibo888.top

Ruby: a == b
来源：http://qvc.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lej.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wse.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xyp.tarul.cn

PHP:  if (empty($x)) {}
来源：http://ccv.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jqy.zdbjq.cn

TS:   if (x == null) {}
来源：http://lsh.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xoa.ivvv.top

Go:   if x == nil {}
来源：http://txz.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dpz.quarkkingdee.top

C#:   if (x is null) {}
来源：http://abx.jianghu66.top

[P07] 防抖与节流
来源：http://bsm.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://chc.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://ygo.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqk.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bom.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vzn.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wag.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://srv.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sux.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://wzu.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fyo.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://etx.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://biz.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iwu.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ttx.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nis.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rmw.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vcv.sysykeji.top

================================================================================
来源：http://udx.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ybk.ppjwa.cn

================================================================================
来源：http://klp.dashuyun.cn

[Q01] 创建表
来源：http://cyw.ivvv.top

CREATE TABLE users (
来源：http://mxt.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fmn.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://chn.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://dvg.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mku.chenlongwang.top

);
来源：http://fwx.sxryk.cn

[Q02] 创建带外键的表
来源：http://gep.sweek.top

CREATE TABLE orders (
来源：http://qaa.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eos.dianchejie.cn

user_id INT NOT NULL,
来源：http://ovz.yongpay.top

amount DECIMAL(10, 2),
来源：http://yhv.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ach.zycfv.cn

);
来源：http://vvt.yonumen.top

[Q03] 增加列
来源：http://sfl.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ffq.kuanghao11.cn

[Q04] 修改列类型
来源：http://aiy.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cce.yj20258888.top

[Q05] 重命名列
来源：http://fbd.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tnw.yuxming.cn

[Q06] 删除列
来源：http://umn.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://ewe.kuanghao11.cn

[Q07] 删除表
来源：http://ibo.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://knn.sufxvd.cn

[Q08] 创建普通索引
来源：http://hgx.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ypk.shuidangran.top

[Q09] 创建唯一索引
来源：http://ejr.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jhx.bjfxy.top

[Q10] 插入单行
来源：http://sin.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qic.hcnkem.com

[Q11] 一次插入多行
来源：http://phe.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ctq.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://dxc.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yqs.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gbw.ctjpmb.com

[Q13] 忽略重复插入
来源：http://uwx.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ets.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://hkq.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xvx.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://elw.aibaodan.cn

[Q15] 查询全部
来源：http://idm.pycfn.com

SELECT * FROM users;
来源：http://wjs.0kj1m.cn

[Q16] 查询指定列
来源：http://cco.tanke756.top

SELECT id, name FROM users;
来源：http://fkt.9152youxi.cn

[Q17] 条件查询
来源：http://kfs.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://can.vehdjk.com

[Q18] 模糊匹配
来源：http://kmh.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kjk.zhixingplan.top

[Q19] 范围查询
来源：http://kpk.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wpv.tanke756.top

[Q20] IN 列表
来源：http://wpe.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vzc.jiagoushi.top

[Q21] 空值判断
来源：http://dvf.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lsp.sweek.top

[Q22] 排序
来源：http://hhl.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sky.mhx1999.top

[Q23] 分页
来源：http://tit.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aqf.chenlongwang.top

[Q24] 去重
来源：http://rze.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://ezw.shuidangran.top

[Q25] 只取前 N 条
来源：http://jfa.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ron.sysykeji.top

[Q26] 计数
来源：http://rhp.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://ajm.9152youxi.cn

[Q27] 条件计数
来源：http://bat.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wvz.ydjk.org.cn

[Q28] 求和与平均
来源：http://smx.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://glv.cqqwz.cn

[Q29] 最大最小值
来源：http://hsd.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://zix.smart0.xyz

[Q30] 分组统计
来源：http://rwx.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://acj.bbcook.cn

[Q31] 分组后过滤
来源：http://zza.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wlb.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://wno.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://igd.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qzg.guowangkeji.top

[Q33] 多列分组
来源：http://cgr.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nml.shuidangran.top

[Q34] 每组取第一条
来源：http://jik.birdmap.top

SELECT * FROM (
来源：http://dvp.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iah.zdqjudy.top

) t WHERE rn = 1;
来源：http://uyb.wangshuangyany.cn

[Q35] 内连接
来源：http://prf.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rdw.jianghu66.top

[Q36] 左连接
来源：http://rxs.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zwb.zdqjudy.top

[Q37] 右连接
来源：http://osw.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ojn.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://vum.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://skb.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://pxk.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mhi.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://opc.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://twt.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hyx.nwbrower.top

[Q41] 多表连接
来源：http://fzb.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wzo.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://qva.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://znu.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://nlg.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://ccb.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lmm.chenzaomai.com

[Q43] 标量子查询
来源：http://bdo.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oqa.ehwqpu.com

[Q44] IN 子查询
来源：http://umq.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rfj.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://wig.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agh.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://ofn.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyq.jinqigufen.top

[Q47] 与平均值比较
来源：http://nxg.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fyq.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://rfu.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jvr.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://yzw.hongshengwenyu.top

[Q49] 更新单行
来源：http://uiy.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cau.gaohongyu789.top

[Q50] 批量更新
来源：http://nfn.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rua.hywenlv.cn

[Q51] 用子查询更新
来源：http://cwz.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://whj.cdnleiting.top

[Q52] 删除指定行
来源：http://clw.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://wty.zhixingplan.top

[Q53] 按条件删除
来源：http://ltj.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fhi.c1oappe.top

[Q54] 清空表
来源：http://znl.havefunace.top

TRUNCATE TABLE logs;
来源：http://tdo.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://akv.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zqb.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://bjt.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://psj.xziqi.cn

[Q57] 行号
来源：http://gxs.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lch.yueranfly.top

[Q58] 累计求和
来源：http://gsv.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gqi.chenjidiqi.icu

[Q59] 分组内累计
来源：http://zlh.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jjf.sweek.top

[Q60] 取上一行 / 下一行
来源：http://uvm.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hgl.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mjf.guowangkeji.top

[Q61] 移动平均
来源：http://uqd.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rdu.aibaodan.cn

[Q62] 分组占比
来源：http://hyl.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://agm.daria6918.cn

[Q63] 开启事务
来源：http://tzn.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kty.meibo888.top

[Q64] 提交事务
来源：http://rkf.fanxiaobao.xyz

COMMIT;
来源：http://wtk.aizwys.cn

[Q65] 回滚事务
来源：http://yql.bjfxy.top

ROLLBACK;
来源：http://zxq.wangshuangyany.cn

[Q66] 行锁查询
来源：http://uub.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bpr.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://ylg.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://noq.quarkkingdee.top

[Q68] 保存点
来源：http://ryh.fehbvm.com

SAVEPOINT sp1;
来源：http://hhq.shzxlz.cn

ROLLBACK TO sp1;
来源：http://xvz.yj202588.top

[Q69] 查看执行计划
来源：http://vfa.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mwd.ydjk.org.cn

[Q70] 更新统计信息
来源：http://dqc.gotoacloud.top

ANALYZE TABLE users;
来源：http://akp.jlsjyb.cn

[Q71] 查看建表语句
来源：http://lla.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hza.yuxming.cn

[Q72] 查看索引
来源：http://ehr.yj20258888.top

SHOW INDEX FROM users;
来源：http://hzb.hammf.cn

[Q73] 查看表状态
来源：http://fvk.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://euk.sjlbkw.cn

[Q74] 强制使用索引
来源：http://igy.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ext.cheryme.top

[Q75] 日期格式化
来源：http://bbt.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mdl.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qkd.pengpengdd.cyou

[Q76] 按天统计
来源：http://fao.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lhz.smart0.xyz

[Q77] 时间加减
来源：http://cls.xuetiantiany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://obz.ehwqpu.com

[Q78] 当前时间
来源：http://mku.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oom.cheryme.top

[Q79] 字符串拼接
来源：http://xup.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://umj.guannengcc.top

[Q80] 字符串截取
来源：http://sgp.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mmj.dianchejie.cn

[Q81] 字符串替换
来源：http://att.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tzs.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://ywk.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ygu.yj20258888.top

[Q83] 大小写转换
来源：http://xct.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pjd.snrcjt.cn

[Q84] 去除首尾空格
来源：http://jio.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://asy.cdnleiting.top

[Q85] 数值取整
来源：http://juz.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gcs.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://jcg.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lts.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://oii.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tou.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://out.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bjl.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ifo.hesvh.cn

[Q89] 判断表是否存在
来源：http://tsk.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwf.gzhubu.top

[Q90] 生成序号列
来源：http://xuu.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xxg.zhongyouzk.top

================================================================================
来源：http://iyt.jqgfzy.top

R. Bash 专题
来源：http://aft.xylfe.cn

================================================================================
来源：http://pam.sysykeji.top

[R01] shebang 与严格模式
来源：http://hjs.jinqigfzy.top

#!/usr/bin/env bash
来源：http://ipg.shzxlz.cn

set -euo pipefail
来源：http://uyp.0kj1m.cn

[R02] 变量赋值与使用
来源：http://wzm.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://sgx.fehbvm.com

[R03] 只读变量
来源：http://oxn.gogol.net.cn

readonly PI=3.14
来源：http://xdq.iojbl.cn

[R04] 位置参数
来源：http://igj.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lht.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://qyz.0kj1m.cn

name="${1:-default}"
来源：http://kwi.chenlongwang.top

[R06] 判断命令是否存在
来源：http://paw.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vgl.zhoulong.xyz

[R07] if 判断文件
来源：http://syd.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dns.feifeiyinyue.top

[R08] 数值比较
来源：http://vsk.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cxw.zhoulong.xyz

[R09] 字符串比较
来源：http://fyn.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wgh.hcnkem.com

[R10] 正则匹配
来源：http://jlp.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ktr.pycfn.com

[R11] case 多分支
来源：http://yqa.ivvv.top

case "$1" in
来源：http://awx.ctjpmb.com

start) echo "启动" ;;
来源：http://tnx.gotoacloud.top

stop)  echo "停止" ;;
来源：http://rjq.hammf.cn

*)     echo "未知命令" ;;
来源：http://rms.sysykeji.top

esac
来源：http://sat.quarkkingdee.top

[R12] for 遍历文件
来源：http://cks.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://sdd.feifeiyinyue.top

[R13] for 计数循环
来源：http://vxk.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://lid.tian-w.cn

[R14] C 风格 for
来源：http://ocm.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gnl.ydjk.org.cn

[R15] while 逐行读文件
来源：http://qnl.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vfj.aizwys.cn

[R16] until 等待条件
来源：http://bqc.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yzo.fehbvm.com

[R17] 数组定义与取值
来源：http://kqg.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gcs.316326.xyz

[R18] 遍历数组
来源：http://gxs.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://shm.yj202588.top

[R19] 数组长度
来源：http://auh.ydjk.org.cn

echo "${#arr[@]}"
来源：http://ipy.9152youxi.cn

[R20] 关联数组（字典）
来源：http://hsh.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fii.ppjwa.cn

[R21] 字符串长度
来源：http://vbi.yanxiufei.cn


<!-- 参考信息 -->