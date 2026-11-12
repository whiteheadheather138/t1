代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gmw.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xyo.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://sox.nwbrower.top

Ruby: a == b
来源：http://vvo.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yig.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nrw.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aef.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://trx.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xfj.nanxinkj.top

TS:   if (x == null) {}
来源：http://mmp.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wqn.zhijiandao.cn

Go:   if x == nil {}
来源：http://tbr.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ooo.jlsjyb.cn

C#:   if (x is null) {}
来源：http://vrq.nanxinkj.top

[P07] 防抖与节流
来源：http://qxz.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bcs.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://bjk.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://def.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xke.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tvc.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://erz.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kwn.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dmh.hesvh.cn

[P08] 处理浮点精度问题
来源：http://nia.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gey.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://emb.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qog.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vys.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hlv.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jrl.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xnw.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nec.fehbvm.com

================================================================================
来源：http://bdl.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://poq.zhaomingkeji.xyz

================================================================================
来源：http://ueq.tarul.cn

[Q01] 创建表
来源：http://rdn.0kj1m.cn

CREATE TABLE users (
来源：http://zac.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tff.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://cye.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://zow.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mvm.cheryme.top

);
来源：http://gcy.yj20258888.top

[Q02] 创建带外键的表
来源：http://rmm.jinqigufen.top

CREATE TABLE orders (
来源：http://cmk.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://szw.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://rms.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://dql.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ceo.wangdashe.top

);
来源：http://cti.0kj1m.cn

[Q03] 增加列
来源：http://zkt.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cxo.sysykeji.top

[Q04] 修改列类型
来源：http://rna.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mya.pengpengdd.cyou

[Q05] 重命名列
来源：http://xgl.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uat.xylfe.cn

[Q06] 删除列
来源：http://kfy.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://cnr.zhengqikj.top

[Q07] 删除表
来源：http://yph.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://tqn.gotoacloud.top

[Q08] 创建普通索引
来源：http://hyz.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gqt.yueranfly.top

[Q09] 创建唯一索引
来源：http://hph.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kpw.sjlbkw.cn

[Q10] 插入单行
来源：http://jbs.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qtx.yj202588.top

[Q11] 一次插入多行
来源：http://bgd.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vqp.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://qdt.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://luv.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oxb.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://byl.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://emz.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://cuz.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lhs.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mwa.tanke756.top

[Q15] 查询全部
来源：http://svj.shuidangran.top

SELECT * FROM users;
来源：http://hao.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://tcs.redwolf501.top

SELECT id, name FROM users;
来源：http://zyx.yfazqb.com

[Q17] 条件查询
来源：http://mqj.ctjpmb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vva.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://hap.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jrq.dianchejie.cn

[Q19] 范围查询
来源：http://qww.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eub.zhiwuduotai.top

[Q20] IN 列表
来源：http://sjt.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mkw.xziqi.cn

[Q21] 空值判断
来源：http://elk.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pmf.vehdjk.com

[Q22] 排序
来源：http://uub.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cqh.zdqjudy.top

[Q23] 分页
来源：http://bic.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nov.hysaishi.cn

[Q24] 去重
来源：http://yar.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://yny.vehdjk.com

[Q25] 只取前 N 条
来源：http://ghv.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://txe.mhx1999.top

[Q26] 计数
来源：http://riq.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://tiq.xuetiantiany.cn

[Q27] 条件计数
来源：http://vis.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mzd.jianghu66.top

[Q28] 求和与平均
来源：http://ssc.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://knu.jinqigfzy.top

[Q29] 最大最小值
来源：http://hme.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gdf.andypj.xyz

[Q30] 分组统计
来源：http://edi.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aov.ybcxt.top

[Q31] 分组后过滤
来源：http://opc.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sii.wangdashe.top

[Q32] 分组拼接字符串
来源：http://khm.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://psa.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dwb.jinqigufen.top

[Q33] 多列分组
来源：http://jlh.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fzi.hesvh.cn

[Q34] 每组取第一条
来源：http://wvf.zhixingplan.top

SELECT * FROM (
来源：http://iyn.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yei.haohaochexian.top

) t WHERE rn = 1;
来源：http://exn.yongpay.top

[Q35] 内连接
来源：http://zgs.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://coq.zhaomingkeji.xyz

[Q36] 左连接
来源：http://gtv.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://for.ehwqpu.com

[Q37] 右连接
来源：http://ylj.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ugq.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kyv.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cgj.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://skz.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ddt.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://igt.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://czo.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://inm.yj202588.top

[Q41] 多表连接
来源：http://jjf.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ult.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://rkq.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://kcb.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://uhv.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://ipc.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://umi.pycfn.com

[Q43] 标量子查询
来源：http://wvr.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ycl.ehwqpu.com

[Q44] IN 子查询
来源：http://iao.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://prv.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://awu.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vny.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://bsu.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzb.hywenlv.cn

[Q47] 与平均值比较
来源：http://etv.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jwc.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://ulx.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xib.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://wij.jianghu66.top

[Q49] 更新单行
来源：http://pjd.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://quk.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://vca.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uds.jlsjyb.cn

[Q51] 用子查询更新
来源：http://rna.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dcy.shzxlz.cn

[Q52] 删除指定行
来源：http://ick.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://che.wangshuangyany.cn

[Q53] 按条件删除
来源：http://lwy.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vtn.dianchejie.cn

[Q54] 清空表
来源：http://fxv.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://act.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://cza.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://orz.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://udp.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bng.zycfv.cn

[Q57] 行号
来源：http://rza.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ohq.zhengqikj.top

[Q58] 累计求和
来源：http://twr.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wen.tanke756.top

[Q59] 分组内累计
来源：http://bqa.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hjo.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://uqr.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tqv.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vos.wangdashe.top

[Q61] 移动平均
来源：http://eqf.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fhs.sweek.top

[Q62] 分组占比
来源：http://fjx.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://adk.cdnleiting.top

[Q63] 开启事务
来源：http://smn.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yvt.52xcode.cn

[Q64] 提交事务
来源：http://twf.shanyushiyangtech.top

COMMIT;
来源：http://atr.yj20258.top

[Q65] 回滚事务
来源：http://guk.zycfv.cn

ROLLBACK;
来源：http://uam.ivvv.top

[Q66] 行锁查询
来源：http://oev.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xwp.tarul.cn

[Q67] 设置隔离级别
来源：http://iay.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://smd.meibo888.top

[Q68] 保存点
来源：http://wru.redwolf501.top

SAVEPOINT sp1;
来源：http://fhw.yvedp.cn

ROLLBACK TO sp1;
来源：http://ruf.cashguo.top

[Q69] 查看执行计划
来源：http://jcv.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://czh.yuxming.cn

[Q70] 更新统计信息
来源：http://xkx.zhoulong.xyz

ANALYZE TABLE users;
来源：http://qvr.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://jbp.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://umf.jqgfzy.top

[Q72] 查看索引
来源：http://qba.guannengcc.top

SHOW INDEX FROM users;
来源：http://miq.jqgufenzy.top

[Q73] 查看表状态
来源：http://hhq.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wdx.chenlongwang.top

[Q74] 强制使用索引
来源：http://izl.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dgs.shuidangran.top

[Q75] 日期格式化
来源：http://qcb.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kvn.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zfy.epnwcf.com

[Q76] 按天统计
来源：http://xml.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dzq.xuetiantiany.cn

[Q77] 时间加减
来源：http://xae.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rzd.aizwys.cn

[Q78] 当前时间
来源：http://lts.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aia.jyoumei.cn

[Q79] 字符串拼接
来源：http://cmz.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uwm.yongpay.top

[Q80] 字符串截取
来源：http://ige.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://otg.nanxuanxn.top

[Q81] 字符串替换
来源：http://byu.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iyx.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://lqn.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rmd.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://gwu.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://the.hnqzz.top

[Q84] 去除首尾空格
来源：http://nji.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://rso.ybcxt.top

[Q85] 数值取整
来源：http://hzq.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eem.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://eak.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cag.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://peg.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gla.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://jkt.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ero.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qvk.cashguo.top

[Q89] 判断表是否存在
来源：http://txy.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ihv.sufxvd.cn

[Q90] 生成序号列
来源：http://fpk.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jsf.tarul.cn

================================================================================
来源：http://csr.fengsongda.top

R. Bash 专题
来源：http://lqw.316326.xyz

================================================================================
来源：http://hvn.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://wnd.zhixingplan.top

#!/usr/bin/env bash
来源：http://bvu.fehbvm.com

set -euo pipefail
来源：http://rkl.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://mrd.yonumen.top

name="Tom"; echo "$name"
来源：http://stw.pycfn.com

[R03] 只读变量
来源：http://wol.snrcjt.cn

readonly PI=3.14
来源：http://enc.hesvh.cn

[R04] 位置参数
来源：http://upu.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zif.fzhhl.top

[R05] 参数默认值
来源：http://dco.epnwcf.com

name="${1:-default}"
来源：http://yvw.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://ygv.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ewb.hywenlv.cn

[R07] if 判断文件
来源：http://qce.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oya.yonumen.top

[R08] 数值比较
来源：http://pmv.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gum.yvedp.cn

[R09] 字符串比较
来源：http://xdk.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ecp.shuidangran.top

[R10] 正则匹配
来源：http://tjc.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vgu.xinyue.icu

[R11] case 多分支
来源：http://iwn.shzxlz.cn

case "$1" in
来源：http://moe.pycfn.com

start) echo "启动" ;;
来源：http://sdr.xinyue.icu

stop)  echo "停止" ;;
来源：http://stn.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://ccc.haohaochexian.top

esac
来源：http://iwp.xuanzx.com

[R12] for 遍历文件
来源：http://que.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://oqm.jinghuilouyu.cn

[R13] for 计数循环
来源：http://dzh.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://wau.zhengqikj.top

[R14] C 风格 for
来源：http://zxj.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hdb.ehwqpu.com

[R15] while 逐行读文件
来源：http://ile.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xxj.cheryme.top

[R16] until 等待条件
来源：http://tfc.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mel.yangfankeji.com

[R17] 数组定义与取值
来源：http://mjn.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://nnr.birdmap.top

[R18] 遍历数组
来源：http://pbu.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ijf.yuanzhike.top

[R19] 数组长度
来源：http://yvg.nwbrower.top

echo "${#arr[@]}"
来源：http://vzj.sxryk.cn

[R20] 关联数组（字典）
来源：http://hrq.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://afy.pengpengdd.cyou

[R21] 字符串长度
来源：http://qbp.hnxiangtu.top

echo "${#s}"
来源：http://mfs.jqgfzy.top

[R22] 截取子串
来源：http://oxy.zhengqikj.top

echo "${s:0:5}"
来源：http://ntp.pengpengdd.cyou

[R23] 字符串替换
来源：http://mwt.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zkh.zycfv.cn

[R24] 大小写转换
来源：http://kdq.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://fsq.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://rhd.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qxy.ehwqpu.com

[R26] 命令替换
来源：http://evk.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://rbd.dashuyun.cn

[R27] 算术展开
来源：http://ejo.shzxlz.cn


<!-- 参考信息 -->