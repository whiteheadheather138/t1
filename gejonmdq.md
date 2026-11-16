代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jou.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ljz.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vrb.shzxlz.cn

Ruby: a == b
来源：http://ffs.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oze.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://awf.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://naa.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://xqq.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qsx.yanxiufei.cn

TS:   if (x == null) {}
来源：http://hbh.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rcm.nanxuanxn.top

Go:   if x == nil {}
来源：http://joz.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pun.daxiang520.top

C#:   if (x is null) {}
来源：http://pgz.c1oappe.top

[P07] 防抖与节流
来源：http://ogd.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vqb.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://eeb.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gnq.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jom.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ytx.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dwi.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmy.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://meq.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://vau.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kwj.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gtg.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ugf.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dlx.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqr.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://owr.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://how.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vzi.mhx1999.top

================================================================================
来源：http://qpq.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://snt.cqqwz.cn

================================================================================
来源：http://hxw.zhoulong.xyz

[Q01] 创建表
来源：http://umg.sxryk.cn

CREATE TABLE users (
来源：http://pir.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tba.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://gxs.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://idn.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yde.hysaishi.cn

);
来源：http://ogw.zdqjudy.top

[Q02] 创建带外键的表
来源：http://mfk.ydzc1.top

CREATE TABLE orders (
来源：http://lly.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eog.tianlin.xyz

user_id INT NOT NULL,
来源：http://lpw.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://kzd.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ujs.ppjwa.cn

);
来源：http://vww.cheryme.top

[Q03] 增加列
来源：http://qwr.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dlk.jqgfzy.top

[Q04] 修改列类型
来源：http://blu.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://agh.shzxlz.cn

[Q05] 重命名列
来源：http://wmq.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lrg.xylfe.cn

[Q06] 删除列
来源：http://aby.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://sgm.cashguo.top

[Q07] 删除表
来源：http://crx.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://qty.yfazqb.com

[Q08] 创建普通索引
来源：http://qte.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kjj.fktsv.cn

[Q09] 创建唯一索引
来源：http://hho.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://puh.zhixingplan.top

[Q10] 插入单行
来源：http://rdz.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ayx.hywenlv.cn

[Q11] 一次插入多行
来源：http://bly.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zxi.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://buy.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://hbg.yuxming.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ber.snrcjt.cn

[Q13] 忽略重复插入
来源：http://ubj.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://smx.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://xhy.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mzz.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bxa.ydjk.org.cn

[Q15] 查询全部
来源：http://ywb.yonumen.top

SELECT * FROM users;
来源：http://ptq.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://jhu.tarul.cn

SELECT id, name FROM users;
来源：http://hxa.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://bnx.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rhq.haohaochexian.top

[Q18] 模糊匹配
来源：http://vic.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oom.shzxlz.cn

[Q19] 范围查询
来源：http://uag.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ypo.bbcook.cn

[Q20] IN 列表
来源：http://ldy.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://djp.yj202588.top

[Q21] 空值判断
来源：http://wgd.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://inp.fehbvm.com

[Q22] 排序
来源：http://dxw.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bvq.yj20258.top

[Q23] 分页
来源：http://uyr.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zct.cashguo.top

[Q24] 去重
来源：http://ezf.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://jpe.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://pcr.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://enq.fktsv.cn

[Q26] 计数
来源：http://yvx.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://cye.aibaodan.cn

[Q27] 条件计数
来源：http://lzk.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wve.nanxinkj.top

[Q28] 求和与平均
来源：http://fde.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxz.jianghu66.top

[Q29] 最大最小值
来源：http://qnl.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://grt.52xcode.cn

[Q30] 分组统计
来源：http://owu.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://phl.ehwqpu.com

[Q31] 分组后过滤
来源：http://fst.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpb.birdmap.top

[Q32] 分组拼接字符串
来源：http://wwr.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nox.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vkk.hywenlv.cn

[Q33] 多列分组
来源：http://dvb.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zfh.jyoumei.cn

[Q34] 每组取第一条
来源：http://wnd.yangfankeji.com

SELECT * FROM (
来源：http://ybh.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xge.birdmap.top

) t WHERE rn = 1;
来源：http://ddz.quarkkingdee.top

[Q35] 内连接
来源：http://cre.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nwv.yj20258888.top

[Q36] 左连接
来源：http://uen.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://meh.gotoacloud.top

[Q37] 右连接
来源：http://sll.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xge.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://efa.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hrm.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://jnb.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nkc.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qjl.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ags.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://shw.pengpengdd.cyou

[Q41] 多表连接
来源：http://ywg.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rnr.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://ajq.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://ftf.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://mru.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://ymk.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://drv.aizwys.cn

[Q43] 标量子查询
来源：http://gqt.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kqs.yj20258888.top

[Q44] IN 子查询
来源：http://nct.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ckw.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://nxt.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iny.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kay.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jak.cqqwz.cn

[Q47] 与平均值比较
来源：http://jat.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://akx.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://cpb.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vih.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://pbh.ctjpmb.com

[Q49] 更新单行
来源：http://vix.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gxa.birdmap.top

[Q50] 批量更新
来源：http://uev.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://veg.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://tbo.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qhe.fengsongda.top

[Q52] 删除指定行
来源：http://xhv.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://etn.hfpthk.cn

[Q53] 按条件删除
来源：http://iat.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gbg.hnxiangtu.top

[Q54] 清空表
来源：http://sxs.pycfn.com

TRUNCATE TABLE logs;
来源：http://kln.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://tww.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yza.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://gva.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ljr.smart0.xyz

[Q57] 行号
来源：http://vmj.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ogl.mhx1999.top

[Q58] 累计求和
来源：http://rud.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yfg.feifeiyinyue.top

[Q59] 分组内累计
来源：http://fyv.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hfe.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://rxw.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wcn.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ttz.xylfe.cn

[Q61] 移动平均
来源：http://vdq.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ywg.zhiwuduotai.top

[Q62] 分组占比
来源：http://snq.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://asy.hnqzz.top

[Q63] 开启事务
来源：http://igt.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dqk.zdbjq.cn

[Q64] 提交事务
来源：http://gke.wangdashe.top

COMMIT;
来源：http://dkb.kuanghao11.cn

[Q65] 回滚事务
来源：http://kyn.tanke756.top

ROLLBACK;
来源：http://cfe.zhoulong.xyz

[Q66] 行锁查询
来源：http://niz.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jkr.ydzc1.top

[Q67] 设置隔离级别
来源：http://gvs.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yyd.nanxinkj.top

[Q68] 保存点
来源：http://tzf.smart0.xyz

SAVEPOINT sp1;
来源：http://nok.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://ycc.xziqi.cn

[Q69] 查看执行计划
来源：http://bgb.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdx.havefunace.top

[Q70] 更新统计信息
来源：http://vhp.zdbjq.cn

ANALYZE TABLE users;
来源：http://xzj.316326.xyz

[Q71] 查看建表语句
来源：http://cvy.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://maz.xinyue.icu

[Q72] 查看索引
来源：http://mqm.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://bxl.xuanzx.com

[Q73] 查看表状态
来源：http://edw.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kep.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://lsd.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hio.vehdjk.com

[Q75] 日期格式化
来源：http://lia.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lff.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jmz.zhongyouzk.top

[Q76] 按天统计
来源：http://qws.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fen.cdnleiting.top

[Q77] 时间加减
来源：http://ojz.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hfj.svipenyu.cn

[Q78] 当前时间
来源：http://zcs.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hfb.fktsv.cn

[Q79] 字符串拼接
来源：http://pvq.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jja.yonumen.top

[Q80] 字符串截取
来源：http://fhw.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdd.tian-w.cn

[Q81] 字符串替换
来源：http://tpv.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wyr.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://pit.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eys.fehbvm.com

[Q83] 大小写转换
来源：http://bws.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tga.epnwcf.com

[Q84] 去除首尾空格
来源：http://nit.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://oqw.fzhhl.top

[Q85] 数值取整
来源：http://pnn.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://asn.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://bat.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jmt.daria6918.cn

[Q87] JSON 字段做条件
来源：http://lon.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gyj.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://uki.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fnt.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qev.xuanzx.com

[Q89] 判断表是否存在
来源：http://nrb.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qyz.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://pfk.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oqa.cqqwz.cn

================================================================================
来源：http://mml.shangyingyoupin.top

R. Bash 专题
来源：http://ocu.tian-w.cn

================================================================================
来源：http://ptq.hcnkem.com

[R01] shebang 与严格模式
来源：http://obu.zycfv.cn

#!/usr/bin/env bash
来源：http://npi.9152youxi.cn

set -euo pipefail
来源：http://qdw.ctjpmb.com

[R02] 变量赋值与使用
来源：http://gqo.jyoumei.cn

name="Tom"; echo "$name"
来源：http://mlt.hcnkem.com

[R03] 只读变量
来源：http://tfb.fanxiaobao.xyz

readonly PI=3.14
来源：http://zme.316326.xyz

[R04] 位置参数
来源：http://rxm.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ssw.zhiwuduotai.top

[R05] 参数默认值
来源：http://far.jinqigfzy.top

name="${1:-default}"
来源：http://zqv.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://tuf.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tdl.jianghu66.top

[R07] if 判断文件
来源：http://unk.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vfl.sxryk.cn

[R08] 数值比较
来源：http://uet.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tiv.feifeiyinyue.top

[R09] 字符串比较
来源：http://gwg.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xcl.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://lhu.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vbn.fengsongda.top

[R11] case 多分支
来源：http://gnu.chenzaomai.com

case "$1" in
来源：http://zww.ppjwa.cn

start) echo "启动" ;;
来源：http://zgd.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://wbv.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://adc.tianlin.xyz

esac
来源：http://ero.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://gmx.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://jmp.cqqwz.cn

[R13] for 计数循环
来源：http://usw.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://att.hywenlv.cn

[R14] C 风格 for
来源：http://tzz.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzy.jinqigfzy.top

[R15] while 逐行读文件
来源：http://rdv.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qyk.zhixingplan.top

[R16] until 等待条件
来源：http://mwo.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amf.ehwqpu.com

[R17] 数组定义与取值
来源：http://ted.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mkt.yueranfly.top

[R18] 遍历数组
来源：http://luz.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qcj.nwbrower.top

[R19] 数组长度
来源：http://wka.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://lvs.hywenlv.cn

[R20] 关联数组（字典）
来源：http://mgh.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hnt.hfpthk.cn

[R21] 字符串长度
来源：http://ghm.zhoulong.xyz

echo "${#s}"
来源：http://hka.birdmap.top

[R22] 截取子串
来源：http://fcy.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://tjb.shzxlz.cn

[R23] 字符串替换
来源：http://otb.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xoh.yueranfly.top

[R24] 大小写转换
来源：http://rcd.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://llq.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://ija.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://igq.yvedp.cn

[R26] 命令替换
来源：http://tnj.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://fmk.c1oappe.top

[R27] 算术展开
来源：http://ikc.shanyushiyangtech.top


<!-- 参考信息 -->