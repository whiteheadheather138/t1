代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wsj.nanxuanxn.top

TS:   if (x == null) {}
来源：http://lgl.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nyr.yangfankeji.com

Go:   if x == nil {}
来源：http://iem.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ckv.kuanghao11.cn

C#:   if (x is null) {}
来源：http://yya.yueranfly.top

[P07] 防抖与节流
来源：http://ptj.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpk.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://ixp.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcw.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ico.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tgh.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ihk.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dde.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bfn.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://mpj.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbl.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wbs.fengsongda.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mro.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tpl.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rvl.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lqr.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crm.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ozp.hongshengwenyu.top

================================================================================
来源：http://rci.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bho.zdqjudy.top

================================================================================
来源：http://cgq.sxryk.cn

[Q01] 创建表
来源：http://hyp.snrcjt.cn

CREATE TABLE users (
来源：http://rno.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iil.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://ulo.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://fnv.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rrp.shanyushiyangtech.top

);
来源：http://ahf.gotoacloud.top

[Q02] 创建带外键的表
来源：http://srg.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://tua.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ixt.jqgfzy.top

user_id INT NOT NULL,
来源：http://fgq.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://viy.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ayb.fktsv.cn

);
来源：http://idz.uphjek.com

[Q03] 增加列
来源：http://nbg.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dxb.nanxuanxn.top

[Q04] 修改列类型
来源：http://bks.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gsc.hywenlv.cn

[Q05] 重命名列
来源：http://can.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dbb.sweek.top

[Q06] 删除列
来源：http://wgr.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://tcx.gaohongyu789.top

[Q07] 删除表
来源：http://mti.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://hsi.quarkkingdee.top

[Q08] 创建普通索引
来源：http://nkf.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://edc.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://ctz.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://awg.mhx1999.top

[Q10] 插入单行
来源：http://ukg.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dai.pycfn.com

[Q11] 一次插入多行
来源：http://adw.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dsb.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://emn.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://eqo.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ljn.tianlin.xyz

[Q13] 忽略重复插入
来源：http://gzo.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jyu.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://thj.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bsx.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tsw.fktsv.cn

[Q15] 查询全部
来源：http://xac.tanke756.top

SELECT * FROM users;
来源：http://qwc.daria6918.cn

[Q16] 查询指定列
来源：http://ood.hcnkem.com

SELECT id, name FROM users;
来源：http://soq.birdmap.top

[Q17] 条件查询
来源：http://bdg.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bqe.quarkkingdee.top

[Q18] 模糊匹配
来源：http://ach.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usk.zycfv.cn

[Q19] 范围查询
来源：http://ies.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xsl.yueranfly.top

[Q20] IN 列表
来源：http://bbc.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gyz.fzhhl.top

[Q21] 空值判断
来源：http://xuu.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iub.wangdashe.top

[Q22] 排序
来源：http://mug.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fhh.jianghu66.top

[Q23] 分页
来源：http://sbh.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qfi.zhongyouzk.top

[Q24] 去重
来源：http://akq.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://wqz.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://ryu.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jre.hnxiangtu.top

[Q26] 计数
来源：http://fda.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://zak.tianlin.xyz

[Q27] 条件计数
来源：http://bmn.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jfv.xuetiantiany.cn

[Q28] 求和与平均
来源：http://riu.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oak.pengpengdd.cyou

[Q29] 最大最小值
来源：http://ocy.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qds.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://ovp.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gyw.mhx1999.top

[Q31] 分组后过滤
来源：http://kbt.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uzo.guannengcc.top

[Q32] 分组拼接字符串
来源：http://bht.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lly.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ypj.feifeiyinyue.top

[Q33] 多列分组
来源：http://ean.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://orh.hysaishi.cn

[Q34] 每组取第一条
来源：http://rrc.epnwcf.com

SELECT * FROM (
来源：http://gzv.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://utk.pycfn.com

) t WHERE rn = 1;
来源：http://ljg.yvedp.cn

[Q35] 内连接
来源：http://xcr.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgn.jqgfzy.top

[Q36] 左连接
来源：http://eup.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fxv.nanxuanxn.top

[Q37] 右连接
来源：http://ukn.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jgo.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fbn.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sbi.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://tez.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zxy.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ryj.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xji.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oxs.wangshuangyany.cn

[Q41] 多表连接
来源：http://leu.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lbx.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://rsz.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://czq.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://xvz.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://wpy.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rcg.chenjidiqi.icu

[Q43] 标量子查询
来源：http://yno.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kto.dashuyun.cn

[Q44] IN 子查询
来源：http://hhq.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sek.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://com.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzr.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://tpv.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ddg.hnxiangtu.top

[Q47] 与平均值比较
来源：http://xxz.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yxt.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://ahe.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uvl.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://mya.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://fgd.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fxn.ppjwa.cn

[Q50] 批量更新
来源：http://qph.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jfh.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://zbj.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mfz.xylfe.cn

[Q52] 删除指定行
来源：http://jhb.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://cfp.zhongyouzk.top

[Q53] 按条件删除
来源：http://qln.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ycl.yueranfly.top

[Q54] 清空表
来源：http://jfh.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://fpk.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://ngw.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvx.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://sil.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ped.cucudq.cn

[Q57] 行号
来源：http://eds.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://khm.cucudq.cn

[Q58] 累计求和
来源：http://ckt.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zly.yangfankeji.com

[Q59] 分组内累计
来源：http://swo.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://its.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://txt.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kgt.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyu.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://xll.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rfv.jiagoushi.top

[Q62] 分组占比
来源：http://got.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cdc.jqgfzy.top

[Q63] 开启事务
来源：http://biw.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gxa.nanxuanxn.top

[Q64] 提交事务
来源：http://rii.cashguo.top

COMMIT;
来源：http://vfj.52xcode.cn

[Q65] 回滚事务
来源：http://sos.quarkkingdee.top

ROLLBACK;
来源：http://loj.yongpay.top

[Q66] 行锁查询
来源：http://eto.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xwm.yongpay.top

[Q67] 设置隔离级别
来源：http://pcy.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evn.andypj.xyz

[Q68] 保存点
来源：http://wdw.dashuyun.cn

SAVEPOINT sp1;
来源：http://ayc.xziqi.cn

ROLLBACK TO sp1;
来源：http://ckr.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://itd.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nnu.epnwcf.com

[Q70] 更新统计信息
来源：http://uhy.havefunace.top

ANALYZE TABLE users;
来源：http://hzp.jianghu66.top

[Q71] 查看建表语句
来源：http://lzn.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xeb.ydzc1.top

[Q72] 查看索引
来源：http://dom.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://ted.birdmap.top

[Q73] 查看表状态
来源：http://qrk.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yro.jiagoushi.top

[Q74] 强制使用索引
来源：http://owv.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ser.fehbvm.com

[Q75] 日期格式化
来源：http://hts.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obe.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ddp.jlsjyb.cn

[Q76] 按天统计
来源：http://gqd.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gxs.shangyingyoupin.top

[Q77] 时间加减
来源：http://eog.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gbm.bjfxy.top

[Q78] 当前时间
来源：http://xnj.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uha.birdmap.top

[Q79] 字符串拼接
来源：http://dwa.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nab.snrcjt.cn

[Q80] 字符串截取
来源：http://ukf.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wvt.gotoacloud.top

[Q81] 字符串替换
来源：http://iyw.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://efp.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://jxd.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tsh.vqdsnc.cn

[Q83] 大小写转换
来源：http://gkd.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://unz.yangfankeji.com

[Q84] 去除首尾空格
来源：http://obb.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://xon.sweek.top

[Q85] 数值取整
来源：http://puz.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hhe.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://qkv.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rle.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://yzz.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vzr.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://lmg.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bzx.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gfk.cqqwz.cn

[Q89] 判断表是否存在
来源：http://qkp.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nda.xylfe.cn

[Q90] 生成序号列
来源：http://oqt.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lpf.gaohongyu789.top

================================================================================
来源：http://ioe.yj20258.top

R. Bash 专题
来源：http://xps.xuanzx.com

================================================================================
来源：http://gth.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://kex.yuxming.cn

#!/usr/bin/env bash
来源：http://oeg.bjfxy.top

set -euo pipefail
来源：http://uqm.jinqigufen.top

[R02] 变量赋值与使用
来源：http://hxk.c1oappe.top

name="Tom"; echo "$name"
来源：http://rhl.zdqjudy.top

[R03] 只读变量
来源：http://fti.dianchejie.cn

readonly PI=3.14
来源：http://oai.sufxvd.cn

[R04] 位置参数
来源：http://uaq.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rlb.shzxlz.cn

[R05] 参数默认值
来源：http://lho.ybcxt.top

name="${1:-default}"
来源：http://ope.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://okr.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fvc.wangshuangyany.cn

[R07] if 判断文件
来源：http://gjv.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kwl.zycfv.cn

[R08] 数值比较
来源：http://xuo.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zwx.jianghu66.top

[R09] 字符串比较
来源：http://mlz.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ckc.zdbjq.cn

[R10] 正则匹配
来源：http://yqn.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iak.snrcjt.cn

[R11] case 多分支
来源：http://ilk.jyoumei.cn

case "$1" in
来源：http://dtq.nanxuanxn.top

start) echo "启动" ;;
来源：http://gjr.yj202588.top

stop)  echo "停止" ;;
来源：http://znv.xuanzx.com

*)     echo "未知命令" ;;
来源：http://vtn.nanxinkj.top

esac
来源：http://fgv.ppjwa.cn

[R12] for 遍历文件
来源：http://qal.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://ksr.tianlin.xyz

[R13] for 计数循环
来源：http://ais.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://ila.andypj.xyz

[R14] C 风格 for
来源：http://pbm.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://edb.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://jze.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cka.kuanghao11.cn

[R16] until 等待条件
来源：http://kvt.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mno.sysykeji.top

[R17] 数组定义与取值
来源：http://tdc.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pgt.jlsjyb.cn

[R18] 遍历数组
来源：http://fcj.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pwh.vehdjk.com

[R19] 数组长度
来源：http://ehm.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://dtt.xuanzx.com

[R20] 关联数组（字典）
来源：http://etd.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jdm.tanke756.top

[R21] 字符串长度
来源：http://iew.cashguo.top

echo "${#s}"
来源：http://yrp.guowangkeji.top

[R22] 截取子串
来源：http://vcj.aibaodan.cn

echo "${s:0:5}"
来源：http://evv.tianlin.xyz

[R23] 字符串替换
来源：http://oef.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zqi.hammf.cn

[R24] 大小写转换
来源：http://atn.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sms.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://gsu.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ikc.xylfe.cn

[R26] 命令替换
来源：http://ydk.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://aud.yj202588.top

[R27] 算术展开
来源：http://kft.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://pll.yj202588.top

[R28] 浮点运算
来源：http://uiz.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://wlm.wangshuangyany.cn

[R29] 定义函数
来源：http://bhf.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hpi.ehwqpu.com

[R30] 函数返回状态码
来源：http://hyr.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://ujs.hfpthk.cn

[R31] 局部变量
来源：http://dsi.aibaodan.cn


<!-- 参考信息 -->