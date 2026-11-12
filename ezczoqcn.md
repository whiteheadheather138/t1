代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ehv.fengsongda.top

TS:   if (x == null) {}
来源：http://mij.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ozi.kuanghao11.cn

Go:   if x == nil {}
来源：http://xne.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bxx.cashguo.top

C#:   if (x is null) {}
来源：http://ret.hammf.cn

[P07] 防抖与节流
来源：http://ezf.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ssz.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://xwa.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ona.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwo.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epc.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vqw.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ikk.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ter.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://hjj.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dsk.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fea.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dmh.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rhp.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qkz.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ilp.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ysh.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jas.nanxinkj.top

================================================================================
来源：http://hwi.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hvm.jianghu66.top

================================================================================
来源：http://mpg.jinyuanbaomall.cn

[Q01] 创建表
来源：http://fhq.jinqigfzy.top

CREATE TABLE users (
来源：http://wcq.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bib.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://dgj.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://rza.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bwk.52xcode.cn

);
来源：http://met.yueranfly.top

[Q02] 创建带外键的表
来源：http://kmx.yfazqb.com

CREATE TABLE orders (
来源：http://auy.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ptw.cqqwz.cn

user_id INT NOT NULL,
来源：http://pwk.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://gmw.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aof.jqgufenzy.top

);
来源：http://ubp.ivvv.top

[Q03] 增加列
来源：http://str.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wmu.yonumen.top

[Q04] 修改列类型
来源：http://zhk.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gme.nanxinkj.top

[Q05] 重命名列
来源：http://nyp.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jwg.zhijiandao.cn

[Q06] 删除列
来源：http://xbk.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://kmo.aizwys.cn

[Q07] 删除表
来源：http://wjd.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://kuh.zhengqikj.top

[Q08] 创建普通索引
来源：http://ucl.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rsw.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://xcv.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cwo.vehdjk.com

[Q10] 插入单行
来源：http://akp.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lid.hfpthk.cn

[Q11] 一次插入多行
来源：http://hit.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbr.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://hsd.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://tpt.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rcd.nanxinkj.top

[Q13] 忽略重复插入
来源：http://ayh.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ltr.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://ivy.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kxv.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eai.yangfankeji.com

[Q15] 查询全部
来源：http://hwi.ydjk.org.cn

SELECT * FROM users;
来源：http://pue.gaohongyu789.top

[Q16] 查询指定列
来源：http://dpc.yuxming.cn

SELECT id, name FROM users;
来源：http://vdu.havefunace.top

[Q17] 条件查询
来源：http://qld.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://btu.tianlin.xyz

[Q18] 模糊匹配
来源：http://vrd.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lxn.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://dxw.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gyv.epnwcf.com

[Q20] IN 列表
来源：http://tgs.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://atc.yueranfly.top

[Q21] 空值判断
来源：http://fnb.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jus.daxiang520.top

[Q22] 排序
来源：http://xdo.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gyz.feifeiyinyue.top

[Q23] 分页
来源：http://ymp.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mxx.zhongyouzk.top

[Q24] 去重
来源：http://opr.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://som.ybcxt.top

[Q25] 只取前 N 条
来源：http://ala.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lif.hongshengwenyu.top

[Q26] 计数
来源：http://cbk.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://tyu.smart0.xyz

[Q27] 条件计数
来源：http://zad.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zwr.nanxinkj.top

[Q28] 求和与平均
来源：http://hoy.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kfv.hesvh.cn

[Q29] 最大最小值
来源：http://ues.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jpk.xinyue.icu

[Q30] 分组统计
来源：http://lya.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dpu.jinqigufen.top

[Q31] 分组后过滤
来源：http://iro.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wnv.birdmap.top

[Q32] 分组拼接字符串
来源：http://gdf.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bgi.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rcu.guannengcc.top

[Q33] 多列分组
来源：http://zqb.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cjt.uphjek.com

[Q34] 每组取第一条
来源：http://lny.iojbl.cn

SELECT * FROM (
来源：http://ofn.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lnj.pycfn.com

) t WHERE rn = 1;
来源：http://kwv.jqgufenzy.top

[Q35] 内连接
来源：http://dip.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tul.shangyingyoupin.top

[Q36] 左连接
来源：http://ohd.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uep.zhengqikj.top

[Q37] 右连接
来源：http://khf.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ope.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://jzl.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fat.cashguo.top

[Q39] 自连接（查上下级）
来源：http://aqn.hfpthk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rox.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aac.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ksf.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://age.cheryme.top

[Q41] 多表连接
来源：http://twp.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://kch.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://fgo.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://mrt.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://cop.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://mrf.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rfi.ctjpmb.com

[Q43] 标量子查询
来源：http://gim.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gve.aibaodan.cn

[Q44] IN 子查询
来源：http://ogi.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ghh.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://sxh.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qnh.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://dfg.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cau.fzhhl.top

[Q47] 与平均值比较
来源：http://rfu.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pwv.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://lvu.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://owo.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://kvr.bjfxy.top

[Q49] 更新单行
来源：http://mwr.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vql.kuanghao11.cn

[Q50] 批量更新
来源：http://zro.yanxiufei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qsa.ydjk.org.cn

[Q51] 用子查询更新
来源：http://pdq.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://crc.zhixingplan.top

[Q52] 删除指定行
来源：http://ovy.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://qhs.snrcjt.cn

[Q53] 按条件删除
来源：http://nyk.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfw.ydjk.org.cn

[Q54] 清空表
来源：http://pms.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://vot.smart0.xyz

[Q55] 排名（并列占位）
来源：http://hdg.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wyd.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://ynn.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tky.ehwqpu.com

[Q57] 行号
来源：http://cas.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ywc.yanxiufei.cn

[Q58] 累计求和
来源：http://ihk.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vxn.nanxuanxn.top

[Q59] 分组内累计
来源：http://znb.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tef.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://uyi.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yxx.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://msc.zdbjq.cn

[Q61] 移动平均
来源：http://iqd.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zgz.shuidangran.top

[Q62] 分组占比
来源：http://ssj.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hhy.cucudq.cn

[Q63] 开启事务
来源：http://whw.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oiq.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://xwq.gogol.net.cn

COMMIT;
来源：http://joq.c1oappe.top

[Q65] 回滚事务
来源：http://lya.cheryme.top

ROLLBACK;
来源：http://hnv.iojbl.cn

[Q66] 行锁查询
来源：http://vbt.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rml.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://fnl.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hzj.xziqi.cn

[Q68] 保存点
来源：http://tfk.bbcook.cn

SAVEPOINT sp1;
来源：http://xra.yj20258888.top

ROLLBACK TO sp1;
来源：http://wmh.aibaodan.cn

[Q69] 查看执行计划
来源：http://kxi.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jxc.redwolf501.top

[Q70] 更新统计信息
来源：http://otr.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://rhh.quarkkingdee.top

[Q71] 查看建表语句
来源：http://kxr.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lim.52xcode.cn

[Q72] 查看索引
来源：http://ygt.andypj.xyz

SHOW INDEX FROM users;
来源：http://qnr.feifeiyinyue.top

[Q73] 查看表状态
来源：http://uzj.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://deu.aibaodan.cn

[Q74] 强制使用索引
来源：http://mcx.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eak.shuidangran.top

[Q75] 日期格式化
来源：http://bzx.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://obg.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ham.yfazqb.com

[Q76] 按天统计
来源：http://szy.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cme.yj20258888.top

[Q77] 时间加减
来源：http://tgf.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dov.yanxiufei.cn

[Q78] 当前时间
来源：http://sql.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dkw.yuxming.cn

[Q79] 字符串拼接
来源：http://xug.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qjo.meibo888.top

[Q80] 字符串截取
来源：http://lap.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjt.gotoacloud.top

[Q81] 字符串替换
来源：http://xdd.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rfc.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://ool.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kde.chenlongwang.top

[Q83] 大小写转换
来源：http://vlz.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bde.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://bxl.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://hws.zhixingplan.top

[Q85] 数值取整
来源：http://zeh.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ylp.ivvv.top

[Q86] 读取 JSON 字段
来源：http://fpf.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xtw.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://ujf.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pir.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://ryg.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xsc.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hod.hammf.cn

[Q89] 判断表是否存在
来源：http://idk.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vgi.yanxiufei.cn

[Q90] 生成序号列
来源：http://fst.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glj.zhoulong.xyz

================================================================================
来源：http://box.birdmap.top

R. Bash 专题
来源：http://vdv.smart0.xyz

================================================================================
来源：http://ign.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://wrj.zhongyouzk.top

#!/usr/bin/env bash
来源：http://acc.ppjwa.cn

set -euo pipefail
来源：http://clx.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://tiq.cucudq.cn

name="Tom"; echo "$name"
来源：http://rjf.daxiang520.top

[R03] 只读变量
来源：http://goy.haohaochexian.top

readonly PI=3.14
来源：http://mhu.hywenlv.cn

[R04] 位置参数
来源：http://ioo.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uaj.yj20258888.top

[R05] 参数默认值
来源：http://kig.sxryk.cn

name="${1:-default}"
来源：http://pho.zdqjudy.top

[R06] 判断命令是否存在
来源：http://wku.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rgz.feifeiyinyue.top

[R07] if 判断文件
来源：http://xlh.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lav.yj202588.top

[R08] 数值比较
来源：http://zpi.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://zjc.zycfv.cn

[R09] 字符串比较
来源：http://jpv.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sgs.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://ifg.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ksy.smart0.xyz

[R11] case 多分支
来源：http://wwo.hywenlv.cn

case "$1" in
来源：http://buo.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://crj.bbcook.cn

stop)  echo "停止" ;;
来源：http://meu.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://hjl.xingfuxueyuan.xyz

esac
来源：http://vvx.fengsongda.top

[R12] for 遍历文件
来源：http://rlb.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://ati.hesvh.cn

[R13] for 计数循环
来源：http://gtg.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://tge.kuanghao11.cn

[R14] C 风格 for
来源：http://mky.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xqn.sjlbkw.cn

[R15] while 逐行读文件
来源：http://lbx.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tbd.chenjidiqi.icu

[R16] until 等待条件
来源：http://sio.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://npf.tarul.cn

[R17] 数组定义与取值
来源：http://vok.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://qdh.jqgufenzy.top

[R18] 遍历数组
来源：http://opl.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzi.smart0.xyz

[R19] 数组长度
来源：http://hss.cqqwz.cn

echo "${#arr[@]}"
来源：http://ivl.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://vwj.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hah.havefunace.top

[R21] 字符串长度
来源：http://yaz.zhixingplan.top

echo "${#s}"
来源：http://efx.svipenyu.cn

[R22] 截取子串
来源：http://ukd.sweek.top

echo "${s:0:5}"
来源：http://vsv.yangfankeji.com

[R23] 字符串替换
来源：http://ehk.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bzl.shzxlz.cn

[R24] 大小写转换
来源：http://enu.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://wgx.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://kfo.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://csj.jinqigufen.top

[R26] 命令替换
来源：http://vzw.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://aew.ydzc1.top

[R27] 算术展开
来源：http://gjx.zycfv.cn

echo $((1 + 2 * 3))
来源：http://vxm.feifeiyinyue.top

[R28] 浮点运算
来源：http://hxb.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://jls.quarkkingdee.top

[R29] 定义函数
来源：http://lfp.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ice.fengsongda.top

[R30] 函数返回状态码
来源：http://fvl.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://cjb.jqgfzy.top

[R31] 局部变量
来源：http://iwi.yonumen.top


<!-- 参考信息 -->