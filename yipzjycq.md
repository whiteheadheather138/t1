代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vzs.yj20258.top

TS:   if (x == null) {}
来源：http://ipp.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qrw.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://hhk.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eam.dianchejie.cn

C#:   if (x is null) {}
来源：http://zns.shuidangran.top

[P07] 防抖与节流
来源：http://knq.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbd.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://cbh.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xve.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnc.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rup.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bpg.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gsa.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dpq.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://ehr.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nsv.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gfh.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://amn.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dot.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sva.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bmv.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://czx.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gmb.vqdsnc.cn

================================================================================
来源：http://txx.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rfj.zhaomingkeji.xyz

================================================================================
来源：http://axd.gzhubu.top

[Q01] 创建表
来源：http://mcr.gogol.net.cn

CREATE TABLE users (
来源：http://ixv.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ety.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://dvm.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://psx.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ivt.zhongyouzk.top

);
来源：http://ibs.shuidangran.top

[Q02] 创建带外键的表
来源：http://nxa.chenzaomai.com

CREATE TABLE orders (
来源：http://bun.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozg.aibaodan.cn

user_id INT NOT NULL,
来源：http://uym.yonumen.top

amount DECIMAL(10, 2),
来源：http://ihb.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jvp.zhiwuduotai.top

);
来源：http://wfz.jqgfzy.top

[Q03] 增加列
来源：http://gth.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lpg.birdmap.top

[Q04] 修改列类型
来源：http://jui.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dko.dianchejie.cn

[Q05] 重命名列
来源：http://quq.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tby.yj202588.top

[Q06] 删除列
来源：http://jii.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gtm.c1oappe.top

[Q07] 删除表
来源：http://seo.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://ybd.jiagoushi.top

[Q08] 创建普通索引
来源：http://qcc.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ghg.yongpay.top

[Q09] 创建唯一索引
来源：http://dit.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mgp.redwolf501.top

[Q10] 插入单行
来源：http://kmc.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qio.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://vir.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vhq.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://gdk.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jyz.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jcc.yvedp.cn

[Q13] 忽略重复插入
来源：http://kju.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fyt.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://eqa.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bep.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gjw.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://sqa.fengsongda.top

SELECT * FROM users;
来源：http://qzd.yonumen.top

[Q16] 查询指定列
来源：http://nyd.sweek.top

SELECT id, name FROM users;
来源：http://sau.c1oappe.top

[Q17] 条件查询
来源：http://noh.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kui.svipenyu.cn

[Q18] 模糊匹配
来源：http://nlm.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xzf.52xcode.cn

[Q19] 范围查询
来源：http://jgw.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggn.havefunace.top

[Q20] IN 列表
来源：http://ixx.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upt.mhx1999.top

[Q21] 空值判断
来源：http://smc.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cuo.hnxiangtu.top

[Q22] 排序
来源：http://lun.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://phg.birdmap.top

[Q23] 分页
来源：http://kos.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wwg.quarkkingdee.top

[Q24] 去重
来源：http://tsd.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://krx.redwolf501.top

[Q25] 只取前 N 条
来源：http://bkd.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fwg.jianghu66.top

[Q26] 计数
来源：http://zqh.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://bqe.fehbvm.com

[Q27] 条件计数
来源：http://lba.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ycj.wangshuangyany.cn

[Q28] 求和与平均
来源：http://atq.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gzf.zhiwuduotai.top

[Q29] 最大最小值
来源：http://tch.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://qux.xuanzx.com

[Q30] 分组统计
来源：http://pih.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iyo.sxryk.cn

[Q31] 分组后过滤
来源：http://hnj.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nmc.hcnkem.com

[Q32] 分组拼接字符串
来源：http://ijd.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zvr.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yfj.fehbvm.com

[Q33] 多列分组
来源：http://wrr.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gmf.pycfn.com

[Q34] 每组取第一条
来源：http://hwz.jianghu66.top

SELECT * FROM (
来源：http://msn.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://btr.pycfn.com

) t WHERE rn = 1;
来源：http://miy.tarul.cn

[Q35] 内连接
来源：http://hii.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hsd.ivvv.top

[Q36] 左连接
来源：http://jkm.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://btu.ydjk.org.cn

[Q37] 右连接
来源：http://bmt.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yez.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://wea.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pkl.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://zkq.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dee.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://npw.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://mgt.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ieq.yueranfly.top

[Q41] 多表连接
来源：http://jft.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qvx.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://cvh.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://brp.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://aut.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://dav.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rnx.andypj.xyz

[Q43] 标量子查询
来源：http://gvq.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hkd.aibaodan.cn

[Q44] IN 子查询
来源：http://mzk.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://axq.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://zsg.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xin.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://rmh.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gul.birdmap.top

[Q47] 与平均值比较
来源：http://bfv.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ijx.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://shs.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bzl.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://vxh.jianghu66.top

[Q49] 更新单行
来源：http://tuu.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kub.feifeiyinyue.top

[Q50] 批量更新
来源：http://gtv.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wka.jianghu66.top

[Q51] 用子查询更新
来源：http://mlo.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zng.yj20258.top

[Q52] 删除指定行
来源：http://erd.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://nto.redwolf501.top

[Q53] 按条件删除
来源：http://zuj.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfn.yj20258888.top

[Q54] 清空表
来源：http://igi.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://hfb.redwolf501.top

[Q55] 排名（并列占位）
来源：http://rgu.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wnm.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://qgq.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://goz.mhx1999.top

[Q57] 行号
来源：http://xux.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eim.zhiwuduotai.top

[Q58] 累计求和
来源：http://ary.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lpg.hfpthk.cn

[Q59] 分组内累计
来源：http://mdz.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ksn.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://mwk.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tgl.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vym.nwbrower.top

[Q61] 移动平均
来源：http://rya.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ziq.xuetiantiany.cn

[Q62] 分组占比
来源：http://stm.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://isz.snrcjt.cn

[Q63] 开启事务
来源：http://tiu.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nbq.sweek.top

[Q64] 提交事务
来源：http://iuv.sufxvd.cn

COMMIT;
来源：http://zlu.yj202588.top

[Q65] 回滚事务
来源：http://gpc.dashuyun.cn

ROLLBACK;
来源：http://hxc.ybcxt.top

[Q66] 行锁查询
来源：http://vhq.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bem.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://mul.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://krt.quarkkingdee.top

[Q68] 保存点
来源：http://qmh.0kj1m.cn

SAVEPOINT sp1;
来源：http://yih.ppjwa.cn

ROLLBACK TO sp1;
来源：http://eap.jyoumei.cn

[Q69] 查看执行计划
来源：http://uxz.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zou.ehwqpu.com

[Q70] 更新统计信息
来源：http://bxt.kuanghao11.cn

ANALYZE TABLE users;
来源：http://cta.sufxvd.cn

[Q71] 查看建表语句
来源：http://yau.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gfu.yongpay.top

[Q72] 查看索引
来源：http://qdn.yfazqb.com

SHOW INDEX FROM users;
来源：http://vhm.jinqigfzy.top

[Q73] 查看表状态
来源：http://cbe.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dcb.nwbrower.top

[Q74] 强制使用索引
来源：http://bff.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mcq.hysaishi.cn

[Q75] 日期格式化
来源：http://lei.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://acw.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fuc.nanxuanxn.top

[Q76] 按天统计
来源：http://lon.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dyd.hesvh.cn

[Q77] 时间加减
来源：http://wpl.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ght.quarkkingdee.top

[Q78] 当前时间
来源：http://wea.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dav.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://eij.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gmo.dianchejie.cn

[Q80] 字符串截取
来源：http://zgb.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wrb.c1oappe.top

[Q81] 字符串替换
来源：http://vcj.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nuu.meibo888.top

[Q82] 字符长度与字节长度
来源：http://fin.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aic.cashguo.top

[Q83] 大小写转换
来源：http://gze.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eky.snrcjt.cn

[Q84] 去除首尾空格
来源：http://eig.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://elu.birdmap.top

[Q85] 数值取整
来源：http://guw.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mhc.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://act.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qrf.sweek.top

[Q87] JSON 字段做条件
来源：http://mps.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wtk.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://odt.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aww.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kxi.hfpthk.cn

[Q89] 判断表是否存在
来源：http://rla.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xeo.yfazqb.com

[Q90] 生成序号列
来源：http://irh.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dno.epnwcf.com

================================================================================
来源：http://tsu.hnqzz.top

R. Bash 专题
来源：http://uuc.yanxiufei.cn

================================================================================
来源：http://qfv.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://iqk.meibo888.top

#!/usr/bin/env bash
来源：http://xhf.jinqigufen.top

set -euo pipefail
来源：http://cps.shuidangran.top

[R02] 变量赋值与使用
来源：http://jmp.jinqigufen.top

name="Tom"; echo "$name"
来源：http://rsj.cdnleiting.top

[R03] 只读变量
来源：http://acb.xinyue.icu

readonly PI=3.14
来源：http://stg.shangyingyoupin.top

[R04] 位置参数
来源：http://fba.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dlw.redwolf501.top

[R05] 参数默认值
来源：http://cfh.kuanghao11.cn

name="${1:-default}"
来源：http://kuk.epnwcf.com

[R06] 判断命令是否存在
来源：http://rqg.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vyl.yj20258.top

[R07] if 判断文件
来源：http://els.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://odj.nanxinkj.top

[R08] 数值比较
来源：http://qbm.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vhy.gogol.net.cn

[R09] 字符串比较
来源：http://lle.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://okq.nwbrower.top

[R10] 正则匹配
来源：http://chw.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dij.jiagoushi.top

[R11] case 多分支
来源：http://bum.dianchejie.cn

case "$1" in
来源：http://oql.redwolf501.top

start) echo "启动" ;;
来源：http://hgo.fzhhl.top

stop)  echo "停止" ;;
来源：http://rhd.birdmap.top

*)     echo "未知命令" ;;
来源：http://gnm.gzhubu.top

esac
来源：http://spq.ehwqpu.com

[R12] for 遍历文件
来源：http://aza.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://kxz.tanke756.top

[R13] for 计数循环
来源：http://sfs.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://kxe.cucudq.cn

[R14] C 风格 for
来源：http://fiz.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ixw.0kj1m.cn

[R15] while 逐行读文件
来源：http://lzd.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wwr.shanyushiyangtech.top

[R16] until 等待条件
来源：http://cle.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://man.iojbl.cn

[R17] 数组定义与取值
来源：http://log.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dsh.sysykeji.top

[R18] 遍历数组
来源：http://fbq.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ztn.cashguo.top

[R19] 数组长度
来源：http://fgh.yuxming.cn

echo "${#arr[@]}"
来源：http://akw.hysaishi.cn

[R20] 关联数组（字典）
来源：http://icp.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nge.xuetiantiany.cn

[R21] 字符串长度
来源：http://zmh.hcnkem.com

echo "${#s}"
来源：http://ite.aibaodan.cn

[R22] 截取子串
来源：http://gmm.wangshuangyany.cn

echo "${s:0:5}"
来源：http://ieu.daxiang520.top

[R23] 字符串替换
来源：http://crb.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hjn.fktsv.cn

[R24] 大小写转换
来源：http://wkj.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wxp.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://mjh.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://nyd.haohaochexian.top

[R26] 命令替换
来源：http://hhv.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://kvk.ywan-chungtsiang.top

[R27] 算术展开
来源：http://weo.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://sux.dianchejie.cn

[R28] 浮点运算
来源：http://dbp.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://biw.wangdashe.top

[R29] 定义函数
来源：http://hzt.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uvi.birdmap.top

[R30] 函数返回状态码
来源：http://uhc.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://ldb.sysykeji.top

[R31] 局部变量
来源：http://ijb.sjlbkw.cn


<!-- 参考信息 -->