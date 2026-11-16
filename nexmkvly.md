代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lpg.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tii.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ufz.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://pxo.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vbj.yueranfly.top

TS:   if (x == null) {}
来源：http://fut.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ecq.hnqzz.top

Go:   if x == nil {}
来源：http://tun.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hom.redwolf501.top

C#:   if (x is null) {}
来源：http://une.redwolf501.top

[P07] 防抖与节流
来源：http://vsz.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wgx.316326.xyz

PHP:  // 手写时间戳比较
来源：http://rex.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzn.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkv.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ynt.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lyq.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wvo.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iqo.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://oiy.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ekr.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lfz.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zki.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rid.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://knr.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yut.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ctr.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ckc.nanxinkj.top

================================================================================
来源：http://wkt.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://irb.sysykeji.top

================================================================================
来源：http://ehz.jiagoushi.top

[Q01] 创建表
来源：http://ntd.jinqigfzy.top

CREATE TABLE users (
来源：http://exx.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ymo.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://hby.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://wvu.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xmw.jinqigfzy.top

);
来源：http://gly.havefunace.top

[Q02] 创建带外键的表
来源：http://hye.dashuyun.cn

CREATE TABLE orders (
来源：http://ski.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mjk.yangfankeji.com

user_id INT NOT NULL,
来源：http://nij.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://gum.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://paw.epnwcf.com

);
来源：http://cve.shanyushiyangtech.top

[Q03] 增加列
来源：http://lbk.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qyo.fehbvm.com

[Q04] 修改列类型
来源：http://qyd.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qzd.guowangkeji.top

[Q05] 重命名列
来源：http://snp.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ygt.xuetiantiany.cn

[Q06] 删除列
来源：http://abx.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ksb.yuxming.cn

[Q07] 删除表
来源：http://sam.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://ewp.guannengcc.top

[Q08] 创建普通索引
来源：http://kxd.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://sqg.andypj.xyz

[Q09] 创建唯一索引
来源：http://uit.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://etw.hesvh.cn

[Q10] 插入单行
来源：http://cfc.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://loz.ybcxt.top

[Q11] 一次插入多行
来源：http://jcb.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gld.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://gzi.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://unz.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jam.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://boz.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwz.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://dpc.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hnx.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mdx.ydzc1.top

[Q15] 查询全部
来源：http://uec.guannengcc.top

SELECT * FROM users;
来源：http://rgx.bbcook.cn

[Q16] 查询指定列
来源：http://yld.yanxiufei.cn

SELECT id, name FROM users;
来源：http://nqn.yfazqb.com

[Q17] 条件查询
来源：http://gjc.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gcn.andypj.xyz

[Q18] 模糊匹配
来源：http://tnd.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qql.hesvh.cn

[Q19] 范围查询
来源：http://bxp.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://foi.svipenyu.cn

[Q20] IN 列表
来源：http://sbk.hnqzz.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ydg.nanxinkj.top

[Q21] 空值判断
来源：http://hgq.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sho.gotoacloud.top

[Q22] 排序
来源：http://ovj.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://frn.xuetiantiany.cn

[Q23] 分页
来源：http://myr.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jcj.hysaishi.cn

[Q24] 去重
来源：http://hws.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://kfu.daxiang520.top

[Q25] 只取前 N 条
来源：http://oyc.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wiu.meibo888.top

[Q26] 计数
来源：http://twm.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://qvi.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://sdy.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vob.tarul.cn

[Q28] 求和与平均
来源：http://ivy.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qtc.guannengcc.top

[Q29] 最大最小值
来源：http://wsf.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nay.hfpthk.cn

[Q30] 分组统计
来源：http://qra.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ljl.xinyue.icu

[Q31] 分组后过滤
来源：http://usc.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvn.yvedp.cn

[Q32] 分组拼接字符串
来源：http://rho.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uig.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hcb.yongpay.top

[Q33] 多列分组
来源：http://glk.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kpr.zdqjudy.top

[Q34] 每组取第一条
来源：http://wwf.9152youxi.cn

SELECT * FROM (
来源：http://loq.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://joi.ehwqpu.com

) t WHERE rn = 1;
来源：http://qka.zycfv.cn

[Q35] 内连接
来源：http://zxn.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jay.yvedp.cn

[Q36] 左连接
来源：http://cxt.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wwr.ppjwa.cn

[Q37] 右连接
来源：http://blp.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vzb.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dml.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kaw.meibo888.top

[Q39] 自连接（查上下级）
来源：http://oqn.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jim.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aer.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://edo.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tpl.shangyingyoupin.top

[Q41] 多表连接
来源：http://rwr.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://znu.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://dcr.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://rfs.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://iay.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://ezn.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xdq.tianlin.xyz

[Q43] 标量子查询
来源：http://uvd.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vfp.0kj1m.cn

[Q44] IN 子查询
来源：http://yyb.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qll.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://izc.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zms.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://ngc.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://voy.jinqigufen.top

[Q47] 与平均值比较
来源：http://kwj.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ldw.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://zim.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dqf.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://wtz.shuidangran.top

[Q49] 更新单行
来源：http://ova.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bmf.jiagoushi.top

[Q50] 批量更新
来源：http://ykl.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pyg.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://uem.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qlb.cucudq.cn

[Q52] 删除指定行
来源：http://iwv.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://lre.sweek.top

[Q53] 按条件删除
来源：http://wci.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjm.fehbvm.com

[Q54] 清空表
来源：http://eir.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://mkj.ybcxt.top

[Q55] 排名（并列占位）
来源：http://nsf.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kap.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://ufw.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hda.yfazqb.com

[Q57] 行号
来源：http://ixx.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nmr.chenjidiqi.icu

[Q58] 累计求和
来源：http://zee.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rxu.ivvv.top

[Q59] 分组内累计
来源：http://vsi.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bok.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://ifo.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fnm.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ead.zhiwuduotai.top

[Q61] 移动平均
来源：http://lkg.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zrw.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://zdy.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ham.dashuyun.cn

[Q63] 开启事务
来源：http://sse.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fsx.shzxlz.cn

[Q64] 提交事务
来源：http://uwj.yangfankeji.com

COMMIT;
来源：http://efh.daxiang520.top

[Q65] 回滚事务
来源：http://cyj.0kj1m.cn

ROLLBACK;
来源：http://plg.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://gfq.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xps.tian-w.cn

[Q67] 设置隔离级别
来源：http://ryn.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://opt.cqqwz.cn

[Q68] 保存点
来源：http://mua.jlsjyb.cn

SAVEPOINT sp1;
来源：http://vht.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://ysu.hesvh.cn

[Q69] 查看执行计划
来源：http://wel.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dht.dashuyun.cn

[Q70] 更新统计信息
来源：http://pse.zhixingplan.top

ANALYZE TABLE users;
来源：http://pat.hammf.cn

[Q71] 查看建表语句
来源：http://uzl.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eft.52xcode.cn

[Q72] 查看索引
来源：http://qwh.zdbjq.cn

SHOW INDEX FROM users;
来源：http://whp.uphjek.com

[Q73] 查看表状态
来源：http://hsq.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ysg.chenzaomai.com

[Q74] 强制使用索引
来源：http://wit.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ecj.sxryk.cn

[Q75] 日期格式化
来源：http://wid.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dcy.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gvr.wangshuangyany.cn

[Q76] 按天统计
来源：http://est.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://flo.feifeiyinyue.top

[Q77] 时间加减
来源：http://eng.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qgz.ehwqpu.com

[Q78] 当前时间
来源：http://juz.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://thp.iojbl.cn

[Q79] 字符串拼接
来源：http://kqa.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wnx.ydjk.org.cn

[Q80] 字符串截取
来源：http://jjb.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bpw.yonumen.top

[Q81] 字符串替换
来源：http://zib.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://acx.birdmap.top

[Q82] 字符长度与字节长度
来源：http://lrw.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xli.sufxvd.cn

[Q83] 大小写转换
来源：http://azc.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bhu.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://lmt.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://qtb.aizwys.cn

[Q85] 数值取整
来源：http://wue.aibaodan.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yjr.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://oem.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kat.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://txf.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rki.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://rgt.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yha.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ukm.aizwys.cn

[Q89] 判断表是否存在
来源：http://sqd.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hjl.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://omw.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pse.chenjidiqi.icu

================================================================================
来源：http://hqp.cucudq.cn

R. Bash 专题
来源：http://ylg.uphjek.com

================================================================================
来源：http://oqd.bbcook.cn

[R01] shebang 与严格模式
来源：http://cqm.redwolf501.top

#!/usr/bin/env bash
来源：http://jfh.dianchejie.cn

set -euo pipefail
来源：http://tyc.birdmap.top

[R02] 变量赋值与使用
来源：http://iie.hammf.cn

name="Tom"; echo "$name"
来源：http://irk.daxiang520.top

[R03] 只读变量
来源：http://sgl.sysykeji.top

readonly PI=3.14
来源：http://gaf.svipenyu.cn

[R04] 位置参数
来源：http://vld.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wly.0kj1m.cn

[R05] 参数默认值
来源：http://dka.aizwys.cn

name="${1:-default}"
来源：http://tcw.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://bar.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gbv.fktsv.cn

[R07] if 判断文件
来源：http://dje.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://opz.guowangkeji.top

[R08] 数值比较
来源：http://qcm.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pdh.hfpthk.cn

[R09] 字符串比较
来源：http://wjx.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://quc.fanxiaobao.xyz

[R10] 正则匹配
来源：http://iqt.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uux.haohaochexian.top

[R11] case 多分支
来源：http://zzm.ydjk.org.cn

case "$1" in
来源：http://xsg.9152youxi.cn

start) echo "启动" ;;
来源：http://lyt.dianchejie.cn

stop)  echo "停止" ;;
来源：http://mde.pycfn.com

*)     echo "未知命令" ;;
来源：http://mmu.fengsongda.top

esac
来源：http://jpg.yfazqb.com

[R12] for 遍历文件
来源：http://bbz.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://qxu.hammf.cn

[R13] for 计数循环
来源：http://sya.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://del.yueranfly.top

[R14] C 风格 for
来源：http://xwu.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qwg.wangdashe.top

[R15] while 逐行读文件
来源：http://tqz.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hrt.feifeiyinyue.top

[R16] until 等待条件
来源：http://jcj.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wll.tarul.cn

[R17] 数组定义与取值
来源：http://nhi.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://sfs.zhongyouzk.top

[R18] 遍历数组
来源：http://rfj.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xbi.zhijiandao.cn

[R19] 数组长度
来源：http://zuq.sxryk.cn

echo "${#arr[@]}"
来源：http://gmr.ctjpmb.com

[R20] 关联数组（字典）
来源：http://qaz.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rqg.sweek.top

[R21] 字符串长度
来源：http://zht.xuetiantiany.cn

echo "${#s}"
来源：http://iom.yangfankeji.com

[R22] 截取子串
来源：http://tlo.shzxlz.cn

echo "${s:0:5}"
来源：http://rop.sweek.top

[R23] 字符串替换
来源：http://jwt.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oel.ctjpmb.com

[R24] 大小写转换
来源：http://imo.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aod.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://vrv.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vsg.bbcook.cn

[R26] 命令替换
来源：http://pcs.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://fsz.xylfe.cn

[R27] 算术展开
来源：http://vnj.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://hyg.jqgfzy.top

[R28] 浮点运算
来源：http://rdj.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://ycv.bjfxy.top

[R29] 定义函数
来源：http://flt.jlsjyb.cn


<!-- 参考信息 -->