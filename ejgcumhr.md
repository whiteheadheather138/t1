代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggn.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jhz.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yit.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://tkj.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nlt.jinqigfzy.top

TS:   if (x == null) {}
来源：http://tkz.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hid.cdnleiting.top

Go:   if x == nil {}
来源：http://zhj.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jcn.vehdjk.com

C#:   if (x is null) {}
来源：http://ner.epnwcf.com

[P07] 防抖与节流
来源：http://dsg.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://imp.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://egy.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewe.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpn.zhixingplan.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mtm.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xxg.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://utv.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://owh.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://fju.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kvc.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dmo.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nft.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hzg.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wyo.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tmr.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oac.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hfx.ywan-chungtsiang.top

================================================================================
来源：http://zcm.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://suu.c1oappe.top

================================================================================
来源：http://pgv.hcnkem.com

[Q01] 创建表
来源：http://cbs.hnqzz.top

CREATE TABLE users (
来源：http://bzo.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ays.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://jys.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://frx.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nvn.jinyuanbaomall.cn

);
来源：http://nwo.xylfe.cn

[Q02] 创建带外键的表
来源：http://huo.ivvv.top

CREATE TABLE orders (
来源：http://njq.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://prd.mhx1999.top

user_id INT NOT NULL,
来源：http://jkv.ybcxt.top

amount DECIMAL(10, 2),
来源：http://grl.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sjy.ivvv.top

);
来源：http://xmd.feifeiyinyue.top

[Q03] 增加列
来源：http://cxo.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://szm.cheryme.top

[Q04] 修改列类型
来源：http://lav.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ugo.fzhhl.top

[Q05] 重命名列
来源：http://jku.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chb.dashuyun.cn

[Q06] 删除列
来源：http://giq.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://ndt.quarkkingdee.top

[Q07] 删除表
来源：http://wrd.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://udh.tian-w.cn

[Q08] 创建普通索引
来源：http://wbr.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://kwi.jianghu66.top

[Q09] 创建唯一索引
来源：http://vff.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vkm.hywenlv.cn

[Q10] 插入单行
来源：http://vhs.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ler.ppjwa.cn

[Q11] 一次插入多行
来源：http://tzs.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcy.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://ryg.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://xrv.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gze.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://aca.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://reh.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://ltr.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ukz.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bhx.xylfe.cn

[Q15] 查询全部
来源：http://ayp.birdmap.top

SELECT * FROM users;
来源：http://hds.pengpengdd.cyou

[Q16] 查询指定列
来源：http://dsl.jiagoushi.top

SELECT id, name FROM users;
来源：http://jdr.zhongyouzk.top

[Q17] 条件查询
来源：http://pyf.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fwg.tianlin.xyz

[Q18] 模糊匹配
来源：http://nwi.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wle.ydjk.org.cn

[Q19] 范围查询
来源：http://jfu.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gei.zhongyouzk.top

[Q20] IN 列表
来源：http://szc.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nsw.snrcjt.cn

[Q21] 空值判断
来源：http://huy.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sav.fanxiaobao.xyz

[Q22] 排序
来源：http://vkf.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bjt.jqgfzy.top

[Q23] 分页
来源：http://jpy.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xhy.daria6918.cn

[Q24] 去重
来源：http://ies.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://owh.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://xyg.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uoz.yj20258.top

[Q26] 计数
来源：http://tfy.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://wzi.sysykeji.top

[Q27] 条件计数
来源：http://iej.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lzc.yueranfly.top

[Q28] 求和与平均
来源：http://pnk.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dgt.shuidangran.top

[Q29] 最大最小值
来源：http://wex.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nyb.yj20258888.top

[Q30] 分组统计
来源：http://qmo.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybx.zhengqikj.top

[Q31] 分组后过滤
来源：http://pxw.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xgu.vehdjk.com

[Q32] 分组拼接字符串
来源：http://ffa.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aqp.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sce.ydzc1.top

[Q33] 多列分组
来源：http://azt.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hhr.fengsongda.top

[Q34] 每组取第一条
来源：http://rpf.hfpthk.cn

SELECT * FROM (
来源：http://djh.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://new.jqgfzy.top

) t WHERE rn = 1;
来源：http://oni.smart0.xyz

[Q35] 内连接
来源：http://fhu.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mqx.hesvh.cn

[Q36] 左连接
来源：http://jhd.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eyk.cashguo.top

[Q37] 右连接
来源：http://lgg.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hnv.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://avg.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://llf.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://gry.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qwg.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vsj.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uoj.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ohh.tarul.cn

[Q41] 多表连接
来源：http://upf.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://csj.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://fru.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://xkt.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://bfv.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://nyh.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ffz.yj202588.top

[Q43] 标量子查询
来源：http://gos.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dci.guannengcc.top

[Q44] IN 子查询
来源：http://dbe.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dyl.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://ltx.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yna.nanxinkj.top

[Q46] NOT EXISTS 判断不存在
来源：http://jig.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://phu.ehwqpu.com

[Q47] 与平均值比较
来源：http://vnz.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ssc.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://dvv.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qie.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ggd.gzhubu.top

[Q49] 更新单行
来源：http://ntd.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ilf.jyoumei.cn

[Q50] 批量更新
来源：http://wfn.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yuz.cucudq.cn

[Q51] 用子查询更新
来源：http://cgx.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nlr.sysykeji.top

[Q52] 删除指定行
来源：http://wbp.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://sfo.xziqi.cn

[Q53] 按条件删除
来源：http://oha.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrm.andypj.xyz

[Q54] 清空表
来源：http://zpn.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://nmr.shuidangran.top

[Q55] 排名（并列占位）
来源：http://ytl.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uoj.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://xtq.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bbv.jinqigfzy.top

[Q57] 行号
来源：http://vpt.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://okn.9152youxi.cn

[Q58] 累计求和
来源：http://cky.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iop.smart0.xyz

[Q59] 分组内累计
来源：http://zdo.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dev.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://guz.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bng.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zmo.hfpthk.cn

[Q61] 移动平均
来源：http://wcg.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://slq.zycfv.cn

[Q62] 分组占比
来源：http://zjr.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zts.zhoulong.xyz

[Q63] 开启事务
来源：http://pop.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wxk.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://hvx.jinqigufen.top

COMMIT;
来源：http://buv.ydzc1.top

[Q65] 回滚事务
来源：http://yhz.shangyingyoupin.top

ROLLBACK;
来源：http://kge.zhiwuduotai.top

[Q66] 行锁查询
来源：http://jam.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ejn.svipenyu.cn

[Q67] 设置隔离级别
来源：http://ufb.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bbq.jyoumei.cn

[Q68] 保存点
来源：http://nyd.shuidangran.top

SAVEPOINT sp1;
来源：http://mby.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://gox.zhoulong.xyz

[Q69] 查看执行计划
来源：http://aww.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xcl.sufxvd.cn

[Q70] 更新统计信息
来源：http://vlj.hammf.cn

ANALYZE TABLE users;
来源：http://nnt.hysaishi.cn

[Q71] 查看建表语句
来源：http://jfu.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bts.yongpay.top

[Q72] 查看索引
来源：http://ilp.smart0.xyz

SHOW INDEX FROM users;
来源：http://skw.sufxvd.cn

[Q73] 查看表状态
来源：http://fas.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vzm.xylfe.cn

[Q74] 强制使用索引
来源：http://zkz.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vtk.fzhhl.top

[Q75] 日期格式化
来源：http://aix.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://glm.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dnh.gaohongyu789.top

[Q76] 按天统计
来源：http://fes.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://evq.hywenlv.cn

[Q77] 时间加减
来源：http://kpi.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bjm.yanxiufei.cn

[Q78] 当前时间
来源：http://pcf.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jxe.quarkkingdee.top

[Q79] 字符串拼接
来源：http://abp.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkf.yueranfly.top

[Q80] 字符串截取
来源：http://axg.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pkl.daxiang520.top

[Q81] 字符串替换
来源：http://hhc.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bhw.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://pru.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qqu.yangfankeji.com

[Q83] 大小写转换
来源：http://svg.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sph.xziqi.cn

[Q84] 去除首尾空格
来源：http://znv.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://kxp.hammf.cn

[Q85] 数值取整
来源：http://kim.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gix.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://lgs.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ayd.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://kbb.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mkp.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://tsf.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tkf.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mbr.ctjpmb.com

[Q89] 判断表是否存在
来源：http://psn.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mov.gogol.net.cn

[Q90] 生成序号列
来源：http://bry.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ibz.yuxming.cn

================================================================================
来源：http://vgv.52xcode.cn

R. Bash 专题
来源：http://ueu.zhoulong.xyz

================================================================================
来源：http://brr.sufxvd.cn

[R01] shebang 与严格模式
来源：http://msq.birdmap.top

#!/usr/bin/env bash
来源：http://kmu.nwbrower.top

set -euo pipefail
来源：http://khd.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://who.andypj.xyz

name="Tom"; echo "$name"
来源：http://fzk.sxryk.cn

[R03] 只读变量
来源：http://cte.ehwqpu.com

readonly PI=3.14
来源：http://len.yanxiufei.cn

[R04] 位置参数
来源：http://ngo.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uaa.zhongyouzk.top

[R05] 参数默认值
来源：http://ehx.zdbjq.cn

name="${1:-default}"
来源：http://ebn.ctjpmb.com

[R06] 判断命令是否存在
来源：http://gdv.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://arh.wangshuangyany.cn

[R07] if 判断文件
来源：http://jvp.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kss.quarkkingdee.top

[R08] 数值比较
来源：http://epc.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://btb.zycfv.cn

[R09] 字符串比较
来源：http://snv.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qfr.fehbvm.com

[R10] 正则匹配
来源：http://jxv.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sjf.pengpengdd.cyou

[R11] case 多分支
来源：http://wjr.ehwqpu.com

case "$1" in
来源：http://yhi.zycfv.cn

start) echo "启动" ;;
来源：http://wtb.yongpay.top

stop)  echo "停止" ;;
来源：http://ocl.ybcxt.top

*)     echo "未知命令" ;;
来源：http://yck.havefunace.top

esac
来源：http://snj.c1oappe.top

[R12] for 遍历文件
来源：http://nls.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://sor.ydzc1.top

[R13] for 计数循环
来源：http://rsc.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://wnv.zhongyouzk.top

[R14] C 风格 for
来源：http://ooe.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jpt.sweek.top

[R15] while 逐行读文件
来源：http://cyu.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fyk.ppjwa.cn

[R16] until 等待条件
来源：http://suj.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dnw.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://lud.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ffu.tarul.cn

[R18] 遍历数组
来源：http://ust.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hkt.pengpengdd.cyou

[R19] 数组长度
来源：http://eow.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://rsz.sysykeji.top

[R20] 关联数组（字典）
来源：http://nrk.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gdd.xuetiantiany.cn

[R21] 字符串长度
来源：http://mwo.yueranfly.top

echo "${#s}"
来源：http://anu.hysaishi.cn

[R22] 截取子串
来源：http://fvg.wangshuangyany.cn

echo "${s:0:5}"
来源：http://lff.xuanzx.com

[R23] 字符串替换
来源：http://edz.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mjm.zhiwuduotai.top

[R24] 大小写转换
来源：http://ovg.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://lqf.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://rrs.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eny.hnxiangtu.top

[R26] 命令替换
来源：http://dou.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://niq.shuidangran.top

[R27] 算术展开
来源：http://abk.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://iro.yuxming.cn

[R28] 浮点运算
来源：http://dek.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://oei.uphjek.com

[R29] 定义函数
来源：http://nsk.yj20258888.top


<!-- 参考信息 -->