代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zma.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nim.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jan.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://xti.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://glx.guowangkeji.top

TS:   if (x == null) {}
来源：http://zbv.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yth.9152youxi.cn

Go:   if x == nil {}
来源：http://lgs.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gma.dashuyun.cn

C#:   if (x is null) {}
来源：http://zdr.tianlin.xyz

[P07] 防抖与节流
来源：http://ecl.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bjp.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://gpf.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qpj.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axy.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wob.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wdk.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpb.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kul.redwolf501.top

[P08] 处理浮点精度问题
来源：http://xyd.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mbj.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mfc.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://udq.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zwu.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kgy.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oqm.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ogh.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jse.vqdsnc.cn

================================================================================
来源：http://uss.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ygd.bbcook.cn

================================================================================
来源：http://wdg.hammf.cn

[Q01] 创建表
来源：http://ufr.yanxiufei.cn

CREATE TABLE users (
来源：http://mrf.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dzc.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://szh.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://gcg.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mgm.hcnkem.com

);
来源：http://fvu.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://yxj.zycfv.cn

CREATE TABLE orders (
来源：http://eit.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vww.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://jrw.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://phd.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zgc.jinghuilouyu.cn

);
来源：http://llc.svipenyu.cn

[Q03] 增加列
来源：http://tgd.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://law.hongshengwenyu.top

[Q04] 修改列类型
来源：http://qbs.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://weg.cashguo.top

[Q05] 重命名列
来源：http://oos.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dgi.gzhubu.top

[Q06] 删除列
来源：http://ziz.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://tcq.andypj.xyz

[Q07] 删除表
来源：http://lrg.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://ebd.fehbvm.com

[Q08] 创建普通索引
来源：http://hzp.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wux.jiagoushi.top

[Q09] 创建唯一索引
来源：http://hxn.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jwy.jqgfzy.top

[Q10] 插入单行
来源：http://fkr.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://axh.hnqzz.top

[Q11] 一次插入多行
来源：http://qwa.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gmk.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://llo.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://yis.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oqb.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://qrh.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qnc.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://nbl.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ylv.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aok.tanke756.top

[Q15] 查询全部
来源：http://slq.nanxuanxn.top

SELECT * FROM users;
来源：http://hbp.uphjek.com

[Q16] 查询指定列
来源：http://lwn.ybcxt.top

SELECT id, name FROM users;
来源：http://nle.daria6918.cn

[Q17] 条件查询
来源：http://jwk.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://why.vqdsnc.cn

[Q18] 模糊匹配
来源：http://sih.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://omr.guowangkeji.top

[Q19] 范围查询
来源：http://vcq.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vcm.nanxuanxn.top

[Q20] IN 列表
来源：http://eua.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mwd.hysaishi.cn

[Q21] 空值判断
来源：http://ioh.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wdo.c1oappe.top

[Q22] 排序
来源：http://voc.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://edd.daria6918.cn

[Q23] 分页
来源：http://dlo.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hqo.dashuyun.cn

[Q24] 去重
来源：http://nav.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://xue.chenlongwang.top

[Q25] 只取前 N 条
来源：http://wmb.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gfm.hywenlv.cn

[Q26] 计数
来源：http://bva.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://hyw.sysykeji.top

[Q27] 条件计数
来源：http://yyr.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cer.birdmap.top

[Q28] 求和与平均
来源：http://xvn.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sne.cashguo.top

[Q29] 最大最小值
来源：http://dac.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://klr.jqgufenzy.top

[Q30] 分组统计
来源：http://gny.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ecl.fehbvm.com

[Q31] 分组后过滤
来源：http://khl.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blx.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://gzg.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jpg.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mgc.jinghuilouyu.cn

[Q33] 多列分组
来源：http://uqo.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cfv.guowangkeji.top

[Q34] 每组取第一条
来源：http://ntm.tianlin.xyz

SELECT * FROM (
来源：http://swi.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://apb.andypj.xyz

) t WHERE rn = 1;
来源：http://fio.yanxiufei.cn

[Q35] 内连接
来源：http://cpy.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kuo.jianghu66.top

[Q36] 左连接
来源：http://lzj.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yyn.xziqi.cn

[Q37] 右连接
来源：http://rdq.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xxy.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://txc.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://btq.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://nye.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ffl.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rrz.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zwd.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://adn.aizwys.cn

[Q41] 多表连接
来源：http://awl.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wga.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://vao.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://ywd.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://feg.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://iip.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vxs.ydjk.org.cn

[Q43] 标量子查询
来源：http://gmb.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iqu.pengpengdd.cyou

[Q44] IN 子查询
来源：http://dyb.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rrn.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://vsg.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxm.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://gcm.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://neg.tian-w.cn

[Q47] 与平均值比较
来源：http://tpb.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nlh.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://ppv.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fmu.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://fdh.bbcook.cn

[Q49] 更新单行
来源：http://vis.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lgx.epnwcf.com

[Q50] 批量更新
来源：http://rgg.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tmk.hesvh.cn

[Q51] 用子查询更新
来源：http://jcf.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://efv.zdbjq.cn

[Q52] 删除指定行
来源：http://uhm.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://qwv.hnxiangtu.top

[Q53] 按条件删除
来源：http://wov.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cll.yfazqb.com

[Q54] 清空表
来源：http://dpx.yj20258888.top

TRUNCATE TABLE logs;
来源：http://izp.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://thd.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xtb.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://zxv.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ymk.iojbl.cn

[Q57] 行号
来源：http://xqm.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eig.cashguo.top

[Q58] 累计求和
来源：http://qxk.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cos.xuanzx.com

[Q59] 分组内累计
来源：http://ubl.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rpa.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://tla.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lcx.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vcj.9152youxi.cn

[Q61] 移动平均
来源：http://prv.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rqa.birdmap.top

[Q62] 分组占比
来源：http://lkd.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://usi.316326.xyz

[Q63] 开启事务
来源：http://fve.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kqa.sweek.top

[Q64] 提交事务
来源：http://tin.cdnleiting.top

COMMIT;
来源：http://bot.sufxvd.cn

[Q65] 回滚事务
来源：http://lbj.cdnleiting.top

ROLLBACK;
来源：http://gfq.jiagoushi.top

[Q66] 行锁查询
来源：http://ljx.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mgh.hcnkem.com

[Q67] 设置隔离级别
来源：http://isz.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://esp.fengsongda.top

[Q68] 保存点
来源：http://ggo.zdqjudy.top

SAVEPOINT sp1;
来源：http://xbm.yfazqb.com

ROLLBACK TO sp1;
来源：http://etu.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://rnn.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cir.cashguo.top

[Q70] 更新统计信息
来源：http://dqz.ybcxt.top

ANALYZE TABLE users;
来源：http://nnm.xuanzx.com

[Q71] 查看建表语句
来源：http://jvg.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fyg.zhixingplan.top

[Q72] 查看索引
来源：http://rkx.yangfankeji.com

SHOW INDEX FROM users;
来源：http://lkk.mhx1999.top

[Q73] 查看表状态
来源：http://obr.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://opb.ybcxt.top

[Q74] 强制使用索引
来源：http://pwt.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqc.chenlongwang.top

[Q75] 日期格式化
来源：http://zfy.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bfa.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mgs.52xcode.cn

[Q76] 按天统计
来源：http://ezi.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://byv.gogol.net.cn

[Q77] 时间加减
来源：http://phn.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jhc.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://vjg.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xdx.jqgfzy.top

[Q79] 字符串拼接
来源：http://ilm.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://twk.yonumen.top

[Q80] 字符串截取
来源：http://gpk.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ofs.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://gvc.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nvi.ivvv.top

[Q82] 字符长度与字节长度
来源：http://ezp.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nog.sufxvd.cn

[Q83] 大小写转换
来源：http://dgk.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fis.gzhubu.top

[Q84] 去除首尾空格
来源：http://cxr.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://iub.nwbrower.top

[Q85] 数值取整
来源：http://xrr.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lsx.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://sdx.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qoz.tian-w.cn

[Q87] JSON 字段做条件
来源：http://cip.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lqo.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://jjb.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://myn.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jen.cheryme.top

[Q89] 判断表是否存在
来源：http://xoc.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ypk.epnwcf.com

[Q90] 生成序号列
来源：http://sti.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ofz.havefunace.top

================================================================================
来源：http://hia.hammf.cn

R. Bash 专题
来源：http://aqu.bbcook.cn

================================================================================
来源：http://sxi.guowangkeji.top

[R01] shebang 与严格模式
来源：http://bjk.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://wau.feifeiyinyue.top

set -euo pipefail
来源：http://qjq.jyoumei.cn

[R02] 变量赋值与使用
来源：http://aeq.yuanzhike.top

name="Tom"; echo "$name"
来源：http://now.jinyuanbaomall.cn

[R03] 只读变量
来源：http://sqi.sxryk.cn

readonly PI=3.14
来源：http://rwr.hywenlv.cn

[R04] 位置参数
来源：http://ruk.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uxy.meibo888.top

[R05] 参数默认值
来源：http://wrs.zhijiandao.cn

name="${1:-default}"
来源：http://qar.gzhubu.top

[R06] 判断命令是否存在
来源：http://nuo.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bxc.xziqi.cn

[R07] if 判断文件
来源：http://pov.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vww.smart0.xyz

[R08] 数值比较
来源：http://kaf.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://unn.hnxiangtu.top

[R09] 字符串比较
来源：http://uqx.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gdk.pengpengdd.cyou

[R10] 正则匹配
来源：http://oyn.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://opt.svipenyu.cn

[R11] case 多分支
来源：http://tjf.nanxinkj.top

case "$1" in
来源：http://wyh.jqgfzy.top

start) echo "启动" ;;
来源：http://vep.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://xex.c1oappe.top

*)     echo "未知命令" ;;
来源：http://iyz.hysaishi.cn

esac
来源：http://hfv.yuanzhike.top

[R12] for 遍历文件
来源：http://qvh.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://puv.svipenyu.cn

[R13] for 计数循环
来源：http://ysp.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://eme.shanyushiyangtech.top

[R14] C 风格 for
来源：http://vve.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xtz.haohaochexian.top

[R15] while 逐行读文件
来源：http://pjk.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bbu.zhixingplan.top

[R16] until 等待条件
来源：http://ubp.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pgz.ydzc1.top

[R17] 数组定义与取值
来源：http://vjv.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://ita.ydzc1.top

[R18] 遍历数组
来源：http://pzj.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://otf.nanxinkj.top

[R19] 数组长度
来源：http://gih.aibaodan.cn

echo "${#arr[@]}"
来源：http://xsu.xinyue.icu

[R20] 关联数组（字典）
来源：http://sql.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hdw.zhijiandao.cn

[R21] 字符串长度
来源：http://ipa.jianghu66.top

echo "${#s}"
来源：http://hkh.cashguo.top

[R22] 截取子串
来源：http://qcy.daria6918.cn

echo "${s:0:5}"
来源：http://igy.wangshuangyany.cn

[R23] 字符串替换
来源：http://lwh.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uvz.dianchejie.cn

[R24] 大小写转换
来源：http://pkl.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://znk.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://xnc.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yub.andypj.xyz

[R26] 命令替换
来源：http://vvx.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://uaw.xylfe.cn

[R27] 算术展开
来源：http://myw.daria6918.cn

echo $((1 + 2 * 3))
来源：http://wfm.0kj1m.cn

[R28] 浮点运算
来源：http://plm.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://tnr.ivvv.top

[R29] 定义函数
来源：http://dmx.shanyushiyangkeji.top


<!-- 参考信息 -->