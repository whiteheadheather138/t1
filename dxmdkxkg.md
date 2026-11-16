代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vqe.sxryk.cn

C#:   if (x is null) {}
来源：http://qxa.tanke756.top

[P07] 防抖与节流
来源：http://fld.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xkf.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://cpf.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfl.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsv.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zzq.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lgp.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://afn.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jql.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://kte.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ofk.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rkh.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xjr.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ree.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tku.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://upy.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aom.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tee.xuetiantiany.cn

================================================================================
来源：http://zmb.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://etc.jianghu66.top

================================================================================
来源：http://nym.jinghuilouyu.cn

[Q01] 创建表
来源：http://baw.cdnleiting.top

CREATE TABLE users (
来源：http://gec.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vtn.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://yhu.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://egc.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lsw.pycfn.com

);
来源：http://cvj.jianghu66.top

[Q02] 创建带外键的表
来源：http://dds.meibo888.top

CREATE TABLE orders (
来源：http://qjx.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uwl.yueranfly.top

user_id INT NOT NULL,
来源：http://apy.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://ypi.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bfi.svipenyu.cn

);
来源：http://zgk.epnwcf.com

[Q03] 增加列
来源：http://pie.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://icr.quarkkingdee.top

[Q04] 修改列类型
来源：http://qsr.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fia.nanxuanxn.top

[Q05] 重命名列
来源：http://atl.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jbm.ybcxt.top

[Q06] 删除列
来源：http://rsv.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://adk.gzhubu.top

[Q07] 删除表
来源：http://sxw.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://wme.ivvv.top

[Q08] 创建普通索引
来源：http://mzs.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gkv.havefunace.top

[Q09] 创建唯一索引
来源：http://fae.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bbf.hcnkem.com

[Q10] 插入单行
来源：http://rbh.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://whl.havefunace.top

[Q11] 一次插入多行
来源：http://pvq.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kmb.tanke756.top

[Q12] 插入后取自增 ID
来源：http://nkc.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iae.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uxm.chenzaomai.com

[Q13] 忽略重复插入
来源：http://cpk.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mjk.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://gwf.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://per.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hag.zhiwuduotai.top

[Q15] 查询全部
来源：http://kuu.zdqjudy.top

SELECT * FROM users;
来源：http://zcn.dianchejie.cn

[Q16] 查询指定列
来源：http://maq.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://psd.316326.xyz

[Q17] 条件查询
来源：http://yqm.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mbt.yj20258888.top

[Q18] 模糊匹配
来源：http://hfa.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eux.9152youxi.cn

[Q19] 范围查询
来源：http://yfv.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxp.nanxuanxn.top

[Q20] IN 列表
来源：http://iqj.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mdh.wangshuangyany.cn

[Q21] 空值判断
来源：http://kav.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://oiv.zhiwuduotai.top

[Q22] 排序
来源：http://vts.fengsongda.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ikj.xziqi.cn

[Q23] 分页
来源：http://pcc.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kya.sxryk.cn

[Q24] 去重
来源：http://ful.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://gmh.c1oappe.top

[Q25] 只取前 N 条
来源：http://dkv.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mik.mhx1999.top

[Q26] 计数
来源：http://ckb.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://cex.nanxuanxn.top

[Q27] 条件计数
来源：http://vpr.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uzr.xuetiantiany.cn

[Q28] 求和与平均
来源：http://cya.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mgu.yueranfly.top

[Q29] 最大最小值
来源：http://ubn.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vth.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://eid.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dem.vqdsnc.cn

[Q31] 分组后过滤
来源：http://mwc.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfh.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://tgz.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sis.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cbq.xinyue.icu

[Q33] 多列分组
来源：http://tsn.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ygz.gaohongyu789.top

[Q34] 每组取第一条
来源：http://qdj.jyoumei.cn

SELECT * FROM (
来源：http://unv.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ufm.shzxlz.cn

) t WHERE rn = 1;
来源：http://tjf.ehwqpu.com

[Q35] 内连接
来源：http://vsu.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfn.zhoulong.xyz

[Q36] 左连接
来源：http://zsf.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jbu.haohaochexian.top

[Q37] 右连接
来源：http://hfj.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uov.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xkj.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ayk.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://you.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://coo.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dfx.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pqq.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qdo.gzhubu.top

[Q41] 多表连接
来源：http://ayu.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://une.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://jdm.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://jti.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://zuq.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://kkg.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sss.0kj1m.cn

[Q43] 标量子查询
来源：http://hit.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hfg.wangshuangyany.cn

[Q44] IN 子查询
来源：http://etb.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkp.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://fah.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nja.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://ldb.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ihy.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://gut.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gxt.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://ouo.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wod.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://raq.zhoulong.xyz

[Q49] 更新单行
来源：http://lxy.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vsn.0kj1m.cn

[Q50] 批量更新
来源：http://zgy.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vxd.daxiang520.top

[Q51] 用子查询更新
来源：http://ifn.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vqu.daria6918.cn

[Q52] 删除指定行
来源：http://nis.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://clf.hnxiangtu.top

[Q53] 按条件删除
来源：http://xbf.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fel.andypj.xyz

[Q54] 清空表
来源：http://bpg.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://eum.xziqi.cn

[Q55] 排名（并列占位）
来源：http://hbw.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cqi.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://tdd.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rth.xylfe.cn

[Q57] 行号
来源：http://nrh.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rcn.yongpay.top

[Q58] 累计求和
来源：http://rwj.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ifp.cheryme.top

[Q59] 分组内累计
来源：http://yzv.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xyh.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://ybo.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vss.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mfk.haohaochexian.top

[Q61] 移动平均
来源：http://yvx.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lgq.chenjidiqi.icu

[Q62] 分组占比
来源：http://ypf.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wwb.sweek.top

[Q63] 开启事务
来源：http://yma.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dxn.hnqzz.top

[Q64] 提交事务
来源：http://nly.havefunace.top

COMMIT;
来源：http://sbw.wangdashe.top

[Q65] 回滚事务
来源：http://zku.xinyue.icu

ROLLBACK;
来源：http://eui.yj20258.top

[Q66] 行锁查询
来源：http://uat.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://frt.ybcxt.top

[Q67] 设置隔离级别
来源：http://cui.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ntt.hywenlv.cn

[Q68] 保存点
来源：http://evi.andypj.xyz

SAVEPOINT sp1;
来源：http://dbg.birdmap.top

ROLLBACK TO sp1;
来源：http://vzv.jlsjyb.cn

[Q69] 查看执行计划
来源：http://poi.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://spc.chenlongwang.top

[Q70] 更新统计信息
来源：http://uqb.sufxvd.cn

ANALYZE TABLE users;
来源：http://izr.xziqi.cn

[Q71] 查看建表语句
来源：http://dcb.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uus.zdbjq.cn

[Q72] 查看索引
来源：http://hxb.wangdashe.top

SHOW INDEX FROM users;
来源：http://omz.nanxinkj.top

[Q73] 查看表状态
来源：http://okv.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lae.gotoacloud.top

[Q74] 强制使用索引
来源：http://gzq.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fbp.aizwys.cn

[Q75] 日期格式化
来源：http://jyz.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vht.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://djg.gaohongyu789.top

[Q76] 按天统计
来源：http://yid.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vir.yonumen.top

[Q77] 时间加减
来源：http://xqb.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tgi.zhongyouzk.top

[Q78] 当前时间
来源：http://uhd.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pve.andypj.xyz

[Q79] 字符串拼接
来源：http://vnb.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ukh.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://noc.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xrs.tianlin.xyz

[Q81] 字符串替换
来源：http://lkc.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gpd.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://rre.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lkt.nwbrower.top

[Q83] 大小写转换
来源：http://whg.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nxl.aibaodan.cn

[Q84] 去除首尾空格
来源：http://jrk.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://ekt.52xcode.cn

[Q85] 数值取整
来源：http://exu.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dmr.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://myc.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rqv.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://luy.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://few.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://zlp.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fgu.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://atx.ctjpmb.com

[Q89] 判断表是否存在
来源：http://sik.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uzk.dashuyun.cn

[Q90] 生成序号列
来源：http://eso.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bnp.jinqigfzy.top

================================================================================
来源：http://ebv.xylfe.cn

R. Bash 专题
来源：http://std.mhx1999.top

================================================================================
来源：http://gyi.haohaochexian.top

[R01] shebang 与严格模式
来源：http://qyh.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://ltr.cqqwz.cn

set -euo pipefail
来源：http://hil.havefunace.top

[R02] 变量赋值与使用
来源：http://nep.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://sbj.guowangkeji.top

[R03] 只读变量
来源：http://nrv.guowangkeji.top

readonly PI=3.14
来源：http://cpn.yj202588.top

[R04] 位置参数
来源：http://xqz.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lbt.zdbjq.cn

[R05] 参数默认值
来源：http://zug.dianchejie.cn

name="${1:-default}"
来源：http://ijr.jyoumei.cn

[R06] 判断命令是否存在
来源：http://iik.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://usp.redwolf501.top

[R07] if 判断文件
来源：http://eep.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nkg.chenjidiqi.icu

[R08] 数值比较
来源：http://oor.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://slu.jlsjyb.cn

[R09] 字符串比较
来源：http://jwd.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pkr.tianlin.xyz

[R10] 正则匹配
来源：http://yfb.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dpj.ybcxt.top

[R11] case 多分支
来源：http://qpw.pengpengdd.cyou

case "$1" in
来源：http://cpm.cucudq.cn

start) echo "启动" ;;
来源：http://iea.ppjwa.cn

stop)  echo "停止" ;;
来源：http://ftj.sweek.top

*)     echo "未知命令" ;;
来源：http://fmi.yj20258888.top

esac
来源：http://ygl.andypj.xyz

[R12] for 遍历文件
来源：http://zip.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://mbu.gotoacloud.top

[R13] for 计数循环
来源：http://owz.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://ciz.zycfv.cn

[R14] C 风格 for
来源：http://rpa.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ohi.cucudq.cn

[R15] while 逐行读文件
来源：http://yeb.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ukc.nanxinkj.top

[R16] until 等待条件
来源：http://csd.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chj.hnxiangtu.top

[R17] 数组定义与取值
来源：http://hvv.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ktj.cheryme.top

[R18] 遍历数组
来源：http://caj.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vtk.jinqigfzy.top

[R19] 数组长度
来源：http://svj.yj202588.top

echo "${#arr[@]}"
来源：http://uji.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://quk.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iak.daria6918.cn

[R21] 字符串长度
来源：http://hte.cdnleiting.top

echo "${#s}"
来源：http://ljp.jyoumei.cn

[R22] 截取子串
来源：http://fbe.xinyue.icu

echo "${s:0:5}"
来源：http://isq.jqgufenzy.top

[R23] 字符串替换
来源：http://jnq.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jzz.yj20258888.top

[R24] 大小写转换
来源：http://azi.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://frt.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://med.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nkq.yuxming.cn

[R26] 命令替换
来源：http://uss.hammf.cn

now=$(date +%F); echo "$now"
来源：http://drj.ywan-chungtsiang.top

[R27] 算术展开
来源：http://pqr.meibo888.top

echo $((1 + 2 * 3))
来源：http://spc.birdmap.top

[R28] 浮点运算
来源：http://khn.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://xzi.gogol.net.cn

[R29] 定义函数
来源：http://mam.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ech.daxiang520.top

[R30] 函数返回状态码
来源：http://qeo.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://xkd.yongpay.top

[R31] 局部变量
来源：http://uci.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://pyw.fzhhl.top

[R32] 参数个数校验
来源：http://qds.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zzy.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://dpn.birdmap.top


<!-- 参考信息 -->