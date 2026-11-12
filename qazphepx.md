代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zfv.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jso.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jjw.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://hnb.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://udb.cheryme.top

TS:   if (x == null) {}
来源：http://iku.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nae.xziqi.cn

Go:   if x == nil {}
来源：http://jbv.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://szw.c1oappe.top

C#:   if (x is null) {}
来源：http://hwg.cdnleiting.top

[P07] 防抖与节流
来源：http://izd.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ond.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://dsh.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpn.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqs.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wrp.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ysd.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://srn.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xzb.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://vji.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxg.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zvz.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ava.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://utn.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ccw.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mqk.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aec.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wgd.xuetiantiany.cn

================================================================================
来源：http://qeq.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mvl.hnqzz.top

================================================================================
来源：http://tma.hnxiangtu.top

[Q01] 创建表
来源：http://rzx.xuanzx.com

CREATE TABLE users (
来源：http://ivv.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xwh.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://pcn.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://xtn.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fsh.ybcxt.top

);
来源：http://aps.cashguo.top

[Q02] 创建带外键的表
来源：http://gqj.hongshengwenyu.top

CREATE TABLE orders (
来源：http://xrg.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrz.ivvv.top

user_id INT NOT NULL,
来源：http://wep.xuanzx.com

amount DECIMAL(10, 2),
来源：http://mom.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aqw.havefunace.top

);
来源：http://tvv.gaohongyu789.top

[Q03] 增加列
来源：http://nad.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://quj.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://jrz.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhf.vqdsnc.cn

[Q05] 重命名列
来源：http://wku.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgb.feifeiyinyue.top

[Q06] 删除列
来源：http://ocf.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yac.jinqigfzy.top

[Q07] 删除表
来源：http://hwo.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://ews.yongpay.top

[Q08] 创建普通索引
来源：http://xkz.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dvp.0kj1m.cn

[Q09] 创建唯一索引
来源：http://lqx.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oyw.guowangkeji.top

[Q10] 插入单行
来源：http://vnp.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xfh.guannengcc.top

[Q11] 一次插入多行
来源：http://afz.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://esr.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://nnw.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://vbr.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lch.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://qmy.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xyq.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://cmv.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iyl.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sxd.ppjwa.cn

[Q15] 查询全部
来源：http://okq.gotoacloud.top

SELECT * FROM users;
来源：http://zqm.chenjidiqi.icu

[Q16] 查询指定列
来源：http://ote.ivvv.top

SELECT id, name FROM users;
来源：http://giq.fehbvm.com

[Q17] 条件查询
来源：http://kda.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ynv.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://wow.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svq.ydzc1.top

[Q19] 范围查询
来源：http://nct.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://apq.zhijiandao.cn

[Q20] IN 列表
来源：http://vzu.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rpn.xinyue.icu

[Q21] 空值判断
来源：http://jkj.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vmg.xuanzx.com

[Q22] 排序
来源：http://pxm.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uza.gaohongyu789.top

[Q23] 分页
来源：http://glx.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://atp.iojbl.cn

[Q24] 去重
来源：http://opa.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://fph.dianchejie.cn

[Q25] 只取前 N 条
来源：http://ubj.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://egu.xinyue.icu

[Q26] 计数
来源：http://cbi.hywenlv.cn

SELECT COUNT(*) FROM users;
来源：http://sdn.zhoulong.xyz

[Q27] 条件计数
来源：http://vpk.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gji.tianlin.xyz

[Q28] 求和与平均
来源：http://ixr.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bwm.ctjpmb.com

[Q29] 最大最小值
来源：http://pqq.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ovm.sysykeji.top

[Q30] 分组统计
来源：http://wfq.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dlt.zhijiandao.cn

[Q31] 分组后过滤
来源：http://hbp.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hep.vehdjk.com

[Q32] 分组拼接字符串
来源：http://fzp.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ygf.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uos.hnqzz.top

[Q33] 多列分组
来源：http://dze.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fwm.zhongyouzk.top

[Q34] 每组取第一条
来源：http://tgi.mhx1999.top

SELECT * FROM (
来源：http://bbn.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ojb.haohaochexian.top

) t WHERE rn = 1;
来源：http://ikk.ivvv.top

[Q35] 内连接
来源：http://dbj.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://maf.jqgfzy.top

[Q36] 左连接
来源：http://znu.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xrb.bbcook.cn

[Q37] 右连接
来源：http://vaf.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kth.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zfi.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iyb.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://ymi.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://aag.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tni.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fou.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pse.quarkkingdee.top

[Q41] 多表连接
来源：http://twy.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kud.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://ogi.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://xns.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://kmc.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://edy.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wnq.sufxvd.cn

[Q43] 标量子查询
来源：http://hkm.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hxb.zhiwuduotai.top

[Q44] IN 子查询
来源：http://hqo.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tcg.hammf.cn

[Q45] EXISTS 判断存在
来源：http://vgm.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rhc.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://ghl.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tms.hesvh.cn

[Q47] 与平均值比较
来源：http://xbw.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://igh.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://lwe.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ycu.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://qtr.zdqjudy.top

[Q49] 更新单行
来源：http://bjm.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iay.mhx1999.top

[Q50] 批量更新
来源：http://yjr.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ajf.dianchejie.cn

[Q51] 用子查询更新
来源：http://fih.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uim.cdnleiting.top

[Q52] 删除指定行
来源：http://spe.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://bwa.yonumen.top

[Q53] 按条件删除
来源：http://vjk.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pwx.xuanzx.com

[Q54] 清空表
来源：http://tks.tanke756.top

TRUNCATE TABLE logs;
来源：http://pki.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://twz.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gaa.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://xem.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wys.gogol.net.cn

[Q57] 行号
来源：http://kpw.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pbw.dashuyun.cn

[Q58] 累计求和
来源：http://fxk.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocj.fzhhl.top

[Q59] 分组内累计
来源：http://iym.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qfv.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://wvh.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ehe.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xug.52xcode.cn

[Q61] 移动平均
来源：http://bth.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://umx.ydjk.org.cn

[Q62] 分组占比
来源：http://ife.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://imc.yanxiufei.cn

[Q63] 开启事务
来源：http://ygg.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ytm.ydzc1.top

[Q64] 提交事务
来源：http://eko.sufxvd.cn

COMMIT;
来源：http://yjb.yj20258.top

[Q65] 回滚事务
来源：http://bwn.shanyushiyangkeji.top

ROLLBACK;
来源：http://ktp.jyoumei.cn

[Q66] 行锁查询
来源：http://fbu.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bze.chenzaomai.com

[Q67] 设置隔离级别
来源：http://mdz.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lom.jqgufenzy.top

[Q68] 保存点
来源：http://lse.cdnleiting.top

SAVEPOINT sp1;
来源：http://uue.xinyue.icu

ROLLBACK TO sp1;
来源：http://imh.jqgfzy.top

[Q69] 查看执行计划
来源：http://hfv.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cpk.nanxinkj.top

[Q70] 更新统计信息
来源：http://loq.andypj.xyz

ANALYZE TABLE users;
来源：http://qyv.ydzc1.top

[Q71] 查看建表语句
来源：http://unn.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uxp.zhiwuduotai.top

[Q72] 查看索引
来源：http://tms.sufxvd.cn

SHOW INDEX FROM users;
来源：http://tlm.jlsjyb.cn

[Q73] 查看表状态
来源：http://uqc.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qzx.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://rmu.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdx.jqgufenzy.top

[Q75] 日期格式化
来源：http://ueq.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blt.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://boj.shzxlz.cn

[Q76] 按天统计
来源：http://rmh.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rnl.tanke756.top

[Q77] 时间加减
来源：http://ukq.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xqj.wangdashe.top

[Q78] 当前时间
来源：http://rmy.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mto.shzxlz.cn

[Q79] 字符串拼接
来源：http://kjt.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sna.gotoacloud.top

[Q80] 字符串截取
来源：http://gjv.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjb.yonumen.top

[Q81] 字符串替换
来源：http://kpk.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://utu.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://hfu.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://djp.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://qms.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mpw.zhixingplan.top

[Q84] 去除首尾空格
来源：http://onm.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://qpz.yanxiufei.cn

[Q85] 数值取整
来源：http://pbv.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rsi.birdmap.top

[Q86] 读取 JSON 字段
来源：http://oay.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://say.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://oyw.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ioo.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://azs.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://noi.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://idv.shuidangran.top

[Q89] 判断表是否存在
来源：http://err.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://app.nanxuanxn.top

[Q90] 生成序号列
来源：http://rdd.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cgv.zhengqikj.top

================================================================================
来源：http://cnb.smart0.xyz

R. Bash 专题
来源：http://aqz.yj20258.top

================================================================================
来源：http://afw.yuxming.cn

[R01] shebang 与严格模式
来源：http://jta.bjfxy.top

#!/usr/bin/env bash
来源：http://fvi.smart0.xyz

set -euo pipefail
来源：http://npk.hcnkem.com

[R02] 变量赋值与使用
来源：http://src.tian-w.cn

name="Tom"; echo "$name"
来源：http://bmp.tarul.cn

[R03] 只读变量
来源：http://sbh.zhijiandao.cn

readonly PI=3.14
来源：http://qbe.hammf.cn

[R04] 位置参数
来源：http://nra.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tjv.316326.xyz

[R05] 参数默认值
来源：http://tkh.jinghuilouyu.cn

name="${1:-default}"
来源：http://xpk.nwbrower.top

[R06] 判断命令是否存在
来源：http://mob.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hdo.52xcode.cn

[R07] if 判断文件
来源：http://ghp.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mfw.aibaodan.cn

[R08] 数值比较
来源：http://dym.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uty.wangshuangyany.cn

[R09] 字符串比较
来源：http://dsw.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://htz.fengsongda.top

[R10] 正则匹配
来源：http://bjw.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fdg.hnqzz.top

[R11] case 多分支
来源：http://qqw.jinyuanbaomall.cn

case "$1" in
来源：http://rlx.jyoumei.cn

start) echo "启动" ;;
来源：http://xpl.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://cpl.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://jmn.xingfuxueyuan.xyz

esac
来源：http://jhr.zhongyouzk.top

[R12] for 遍历文件
来源：http://gbm.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://svt.fanxiaobao.xyz

[R13] for 计数循环
来源：http://pzj.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://wer.zhoulong.xyz

[R14] C 风格 for
来源：http://azb.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qcc.tianlin.xyz

[R15] while 逐行读文件
来源：http://zyi.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jvs.yj20258888.top

[R16] until 等待条件
来源：http://ntm.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gac.tanke756.top

[R17] 数组定义与取值
来源：http://ihv.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://gkq.tian-w.cn

[R18] 遍历数组
来源：http://qpu.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bfb.zdbjq.cn

[R19] 数组长度
来源：http://quy.jqgfzy.top

echo "${#arr[@]}"
来源：http://wyi.hammf.cn

[R20] 关联数组（字典）
来源：http://abn.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://srd.ydjk.org.cn

[R21] 字符串长度
来源：http://icj.sxryk.cn

echo "${#s}"
来源：http://xpv.fengsongda.top

[R22] 截取子串
来源：http://klg.xinyue.icu

echo "${s:0:5}"
来源：http://kjy.zhongyouzk.top

[R23] 字符串替换
来源：http://bxr.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://imu.zhijiandao.cn

[R24] 大小写转换
来源：http://lkf.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dcp.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://apy.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mny.daria6918.cn

[R26] 命令替换
来源：http://ida.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://tcu.xinyue.icu

[R27] 算术展开
来源：http://yvs.xziqi.cn

echo $((1 + 2 * 3))
来源：http://vst.tanke756.top

[R28] 浮点运算
来源：http://bqp.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://ayh.jqgufenzy.top

[R29] 定义函数
来源：http://oeq.zhengqikj.top


<!-- 参考信息 -->