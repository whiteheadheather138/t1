代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zpi.cheryme.top

C#:   if (x is null) {}
来源：http://uoj.tanke756.top

[P07] 防抖与节流
来源：http://gvc.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ivr.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://ulq.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwh.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpy.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oeb.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wzt.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ewo.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ipp.guannengcc.top

[P08] 处理浮点精度问题
来源：http://ynx.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fju.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://otx.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iyk.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wun.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://npk.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lww.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://llm.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zaq.xuetiantiany.cn

================================================================================
来源：http://rzt.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hdr.yonumen.top

================================================================================
来源：http://gmg.xziqi.cn

[Q01] 创建表
来源：http://osn.cucudq.cn

CREATE TABLE users (
来源：http://tne.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cel.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://kkn.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://tta.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tky.gzhubu.top

);
来源：http://psh.cqqwz.cn

[Q02] 创建带外键的表
来源：http://spl.0kj1m.cn

CREATE TABLE orders (
来源：http://ibo.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ecs.cashguo.top

user_id INT NOT NULL,
来源：http://cks.316326.xyz

amount DECIMAL(10, 2),
来源：http://ogm.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qoj.hnqzz.top

);
来源：http://xvf.hysaishi.cn

[Q03] 增加列
来源：http://vgy.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nrz.shuidangran.top

[Q04] 修改列类型
来源：http://dqi.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://osk.shzxlz.cn

[Q05] 重命名列
来源：http://xnf.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dkm.daria6918.cn

[Q06] 删除列
来源：http://uka.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://wqn.cucudq.cn

[Q07] 删除表
来源：http://eix.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://mdu.yangfankeji.com

[Q08] 创建普通索引
来源：http://fvo.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://sip.xuanzx.com

[Q09] 创建唯一索引
来源：http://tkv.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jpo.daxiang520.top

[Q10] 插入单行
来源：http://rvp.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wjy.yuxming.cn

[Q11] 一次插入多行
来源：http://azt.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://slb.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://mrv.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cdv.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yln.yuxming.cn

[Q13] 忽略重复插入
来源：http://zsw.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oef.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://eix.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hdt.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ruf.cucudq.cn

[Q15] 查询全部
来源：http://feo.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://bvy.smart0.xyz

[Q16] 查询指定列
来源：http://uzy.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://zka.sufxvd.cn

[Q17] 条件查询
来源：http://uln.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bkt.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://avs.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ngp.yj20258.top

[Q19] 范围查询
来源：http://wxk.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ace.svipenyu.cn

[Q20] IN 列表
来源：http://uqt.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://top.sxryk.cn

[Q21] 空值判断
来源：http://sps.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ter.jlsjyb.cn

[Q22] 排序
来源：http://bct.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ell.sysykeji.top

[Q23] 分页
来源：http://zyu.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vem.andypj.xyz

[Q24] 去重
来源：http://yyj.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://nnj.yj20258888.top

[Q25] 只取前 N 条
来源：http://sro.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tgr.ppjwa.cn

[Q26] 计数
来源：http://lvh.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://ymj.kuanghao11.cn

[Q27] 条件计数
来源：http://ham.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vnl.hesvh.cn

[Q28] 求和与平均
来源：http://xjc.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://itq.zhongyouzk.top

[Q29] 最大最小值
来源：http://kso.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://bnu.yfazqb.com

[Q30] 分组统计
来源：http://vuo.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ued.xylfe.cn

[Q31] 分组后过滤
来源：http://mot.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgl.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://zbk.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bas.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sko.sweek.top

[Q33] 多列分组
来源：http://mbn.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://izs.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://qhz.sxryk.cn

SELECT * FROM (
来源：http://hpg.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ztj.meibo888.top

) t WHERE rn = 1;
来源：http://gwa.zhiwuduotai.top

[Q35] 内连接
来源：http://dgm.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bio.aizwys.cn

[Q36] 左连接
来源：http://ttt.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lqe.316326.xyz

[Q37] 右连接
来源：http://xpw.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bkm.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://hej.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://snm.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://oiv.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jva.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://crj.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://axo.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wbj.gzhubu.top

[Q41] 多表连接
来源：http://kof.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rpz.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://kqm.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://byz.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://wja.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://pel.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kaj.zhixingplan.top

[Q43] 标量子查询
来源：http://skv.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ofq.vqdsnc.cn

[Q44] IN 子查询
来源：http://mol.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://emb.cashguo.top

[Q45] EXISTS 判断存在
来源：http://lyr.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://glq.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://pcc.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ujx.ivvv.top

[Q47] 与平均值比较
来源：http://iwz.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rqt.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://mai.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bxe.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://cng.yueranfly.top

[Q49] 更新单行
来源：http://uqn.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ywe.gotoacloud.top

[Q50] 批量更新
来源：http://ivx.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ilk.9152youxi.cn

[Q51] 用子查询更新
来源：http://igu.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dcf.snrcjt.cn

[Q52] 删除指定行
来源：http://pgx.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://ccp.jqgfzy.top

[Q53] 按条件删除
来源：http://cmc.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uio.tanke756.top

[Q54] 清空表
来源：http://alr.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://wgi.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://jpw.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zya.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://vna.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lrd.fengsongda.top

[Q57] 行号
来源：http://vec.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wke.sufxvd.cn

[Q58] 累计求和
来源：http://ovb.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pqu.hywenlv.cn

[Q59] 分组内累计
来源：http://uxh.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wov.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://vpf.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qpc.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fso.cashguo.top

[Q61] 移动平均
来源：http://drh.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mwp.shanyushiyangtech.top

[Q62] 分组占比
来源：http://blr.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mvz.xziqi.cn

[Q63] 开启事务
来源：http://opf.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zcv.9152youxi.cn

[Q64] 提交事务
来源：http://cmb.hcnkem.com

COMMIT;
来源：http://nhp.nwbrower.top

[Q65] 回滚事务
来源：http://nze.hongshengwenyu.top

ROLLBACK;
来源：http://mxb.hcnkem.com

[Q66] 行锁查询
来源：http://ubk.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yzg.shuidangran.top

[Q67] 设置隔离级别
来源：http://luy.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ftc.yuanzhike.top

[Q68] 保存点
来源：http://cos.jianghu66.top

SAVEPOINT sp1;
来源：http://kiy.redwolf501.top

ROLLBACK TO sp1;
来源：http://udg.hfpthk.cn

[Q69] 查看执行计划
来源：http://fod.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hhc.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://alv.aizwys.cn

ANALYZE TABLE users;
来源：http://fwc.sjlbkw.cn

[Q71] 查看建表语句
来源：http://wzt.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qzx.fanxiaobao.xyz

[Q72] 查看索引
来源：http://xuf.nanxinkj.top

SHOW INDEX FROM users;
来源：http://cbi.zhiwuduotai.top

[Q73] 查看表状态
来源：http://lym.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://itc.zhoulong.xyz

[Q74] 强制使用索引
来源：http://vqd.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mqy.chenzaomai.com

[Q75] 日期格式化
来源：http://whr.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gif.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sjz.xziqi.cn

[Q76] 按天统计
来源：http://gcf.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qhd.cdnleiting.top

[Q77] 时间加减
来源：http://pfs.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ntt.chenlongwang.top

[Q78] 当前时间
来源：http://yfs.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ocm.mhx1999.top

[Q79] 字符串拼接
来源：http://mpn.ehwqpu.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ueb.xinyue.icu

[Q80] 字符串截取
来源：http://hla.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qzu.yuxming.cn

[Q81] 字符串替换
来源：http://xkp.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bph.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://bhf.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ubn.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://zvo.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tay.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://jct.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://zgu.smart0.xyz

[Q85] 数值取整
来源：http://xaa.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hkd.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://rfy.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eep.fengsongda.top

[Q87] JSON 字段做条件
来源：http://koi.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bla.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://cyy.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qtx.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjf.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://daq.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mon.ctjpmb.com

[Q90] 生成序号列
来源：http://vtx.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ywr.316326.xyz

================================================================================
来源：http://dyr.jinqigfzy.top

R. Bash 专题
来源：http://psl.cashguo.top

================================================================================
来源：http://xsg.yfazqb.com

[R01] shebang 与严格模式
来源：http://szz.jqgufenzy.top

#!/usr/bin/env bash
来源：http://afa.hfpthk.cn

set -euo pipefail
来源：http://dpy.daxiang520.top

[R02] 变量赋值与使用
来源：http://xaa.52xcode.cn

name="Tom"; echo "$name"
来源：http://dhi.ctjpmb.com

[R03] 只读变量
来源：http://znn.cheryme.top

readonly PI=3.14
来源：http://zjg.smart0.xyz

[R04] 位置参数
来源：http://jyi.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hbb.hnqzz.top

[R05] 参数默认值
来源：http://zqx.ydzc1.top

name="${1:-default}"
来源：http://pik.bbcook.cn

[R06] 判断命令是否存在
来源：http://mah.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kkw.uphjek.com

[R07] if 判断文件
来源：http://tmt.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jje.wangshuangyany.cn

[R08] 数值比较
来源：http://zcy.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qnv.yonumen.top

[R09] 字符串比较
来源：http://ceb.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://enl.zhijiandao.cn

[R10] 正则匹配
来源：http://fey.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fzb.sjlbkw.cn

[R11] case 多分支
来源：http://fxp.jqgufenzy.top

case "$1" in
来源：http://ihc.kuanghao11.cn

start) echo "启动" ;;
来源：http://low.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://mtw.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://mjn.pycfn.com

esac
来源：http://gnl.aizwys.cn

[R12] for 遍历文件
来源：http://snt.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://inu.cqqwz.cn

[R13] for 计数循环
来源：http://agn.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://krb.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://syd.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://goh.jlsjyb.cn

[R15] while 逐行读文件
来源：http://xlf.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oiq.gaohongyu789.top

[R16] until 等待条件
来源：http://ztl.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lqp.jiagoushi.top

[R17] 数组定义与取值
来源：http://bbo.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://bkh.jinqigufen.top

[R18] 遍历数组
来源：http://oew.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zxy.hnxiangtu.top

[R19] 数组长度
来源：http://nnw.hysaishi.cn

echo "${#arr[@]}"
来源：http://ujr.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://cbz.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sek.jinqigfzy.top

[R21] 字符串长度
来源：http://tlh.tianlin.xyz

echo "${#s}"
来源：http://qwl.nanxuanxn.top

[R22] 截取子串
来源：http://gil.xylfe.cn

echo "${s:0:5}"
来源：http://edl.andypj.xyz

[R23] 字符串替换
来源：http://pdu.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lfp.tanke756.top

[R24] 大小写转换
来源：http://qtz.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eav.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://bvo.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://frd.zycfv.cn

[R26] 命令替换
来源：http://hqn.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://ipv.andypj.xyz

[R27] 算术展开
来源：http://bym.tian-w.cn

echo $((1 + 2 * 3))
来源：http://plu.shangyingyoupin.top

[R28] 浮点运算
来源：http://mix.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://nur.jianghu66.top

[R29] 定义函数
来源：http://ujw.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wpt.yanxiufei.cn

[R30] 函数返回状态码
来源：http://jix.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://plk.xinyue.icu

[R31] 局部变量
来源：http://jza.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://yzl.aibaodan.cn

[R32] 参数个数校验
来源：http://ybx.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ltz.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://kpr.nanxinkj.top


<!-- 参考信息 -->