代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dju.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jwm.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sfu.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://lyr.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bla.tianlin.xyz

TS:   if (x == null) {}
来源：http://izn.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://rjp.kuanghao11.cn

Go:   if x == nil {}
来源：http://fuj.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://spm.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://het.zhixingplan.top

[P07] 防抖与节流
来源：http://bji.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hrf.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://mua.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffq.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eds.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bfh.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pim.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vwd.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ncn.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://nao.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ptn.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cpm.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wmx.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gsx.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lei.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gxx.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fcf.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://acc.hammf.cn

================================================================================
来源：http://ijx.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bus.ctjpmb.com

================================================================================
来源：http://mws.52xcode.cn

[Q01] 创建表
来源：http://ouk.jqgufenzy.top

CREATE TABLE users (
来源：http://cqr.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://etq.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://dbm.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://orw.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eiu.guannengcc.top

);
来源：http://cub.daria6918.cn

[Q02] 创建带外键的表
来源：http://obi.hywenlv.cn

CREATE TABLE orders (
来源：http://jdg.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nfw.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://jih.jianghu66.top

amount DECIMAL(10, 2),
来源：http://osw.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://coc.zhoulong.xyz

);
来源：http://whc.zhiwuduotai.top

[Q03] 增加列
来源：http://jsu.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oyk.fengsongda.top

[Q04] 修改列类型
来源：http://aby.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qko.ehwqpu.com

[Q05] 重命名列
来源：http://ypr.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ucl.ywan-chungtsiang.top

[Q06] 删除列
来源：http://rty.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://jzn.xziqi.cn

[Q07] 删除表
来源：http://hht.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://val.yfazqb.com

[Q08] 创建普通索引
来源：http://rnd.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nqr.bbcook.cn

[Q09] 创建唯一索引
来源：http://csh.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://brj.epnwcf.com

[Q10] 插入单行
来源：http://aws.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://znp.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://ggo.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wom.uphjek.com

[Q12] 插入后取自增 ID
来源：http://dzm.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://tqm.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://izv.hywenlv.cn

[Q13] 忽略重复插入
来源：http://iob.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://inn.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://awe.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bir.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zur.guowangkeji.top

[Q15] 查询全部
来源：http://uxg.dashuyun.cn

SELECT * FROM users;
来源：http://uug.haohaochexian.top

[Q16] 查询指定列
来源：http://hda.daria6918.cn

SELECT id, name FROM users;
来源：http://iyy.sysykeji.top

[Q17] 条件查询
来源：http://mxs.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hyj.hesvh.cn

[Q18] 模糊匹配
来源：http://ipd.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bbh.hesvh.cn

[Q19] 范围查询
来源：http://zjs.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aje.hfpthk.cn

[Q20] IN 列表
来源：http://iol.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mbk.bjfxy.top

[Q21] 空值判断
来源：http://ozm.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://qld.vehdjk.com

[Q22] 排序
来源：http://vcf.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ioc.hysaishi.cn

[Q23] 分页
来源：http://qxf.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xbt.316326.xyz

[Q24] 去重
来源：http://pwa.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://hha.pycfn.com

[Q25] 只取前 N 条
来源：http://nls.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gsq.yangfankeji.com

[Q26] 计数
来源：http://hxs.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://lyt.gogol.net.cn

[Q27] 条件计数
来源：http://ymk.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wnu.zycfv.cn

[Q28] 求和与平均
来源：http://qqd.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ihq.nanxinkj.top

[Q29] 最大最小值
来源：http://ruj.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://omi.iojbl.cn

[Q30] 分组统计
来源：http://ywc.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://alk.yj20258.top

[Q31] 分组后过滤
来源：http://yrb.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kpj.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://ico.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fnj.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://chn.aibaodan.cn

[Q33] 多列分组
来源：http://xfg.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ixm.fehbvm.com

[Q34] 每组取第一条
来源：http://ibt.hfpthk.cn

SELECT * FROM (
来源：http://wee.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rmm.yueranfly.top

) t WHERE rn = 1;
来源：http://etg.yangfankeji.com

[Q35] 内连接
来源：http://osk.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nvg.aizwys.cn

[Q36] 左连接
来源：http://zhp.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hyh.yongpay.top

[Q37] 右连接
来源：http://pza.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jnq.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://bvd.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mzi.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://sqv.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rcw.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rxy.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ore.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hex.zhijiandao.cn

[Q41] 多表连接
来源：http://jys.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://itt.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://reo.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://zbr.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://knh.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://erh.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ajr.nanxuanxn.top

[Q43] 标量子查询
来源：http://voc.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gce.chenzaomai.com

[Q44] IN 子查询
来源：http://osi.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tjl.pycfn.com

[Q45] EXISTS 判断存在
来源：http://oda.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fxm.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://obu.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kni.gotoacloud.top

[Q47] 与平均值比较
来源：http://fja.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ccs.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://sif.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qfn.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://phl.cheryme.top

[Q49] 更新单行
来源：http://fdn.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sej.ydjk.org.cn

[Q50] 批量更新
来源：http://ygp.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ejl.hcnkem.com

[Q51] 用子查询更新
来源：http://pqj.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://biv.tarul.cn

[Q52] 删除指定行
来源：http://cyr.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://uci.yonumen.top

[Q53] 按条件删除
来源：http://gnc.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nga.zdbjq.cn

[Q54] 清空表
来源：http://fnd.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://sez.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://swx.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pml.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://mby.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://acm.haohaochexian.top

[Q57] 行号
来源：http://axi.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhw.daxiang520.top

[Q58] 累计求和
来源：http://noa.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tcs.fengsongda.top

[Q59] 分组内累计
来源：http://cgh.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kgb.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://wtr.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tdy.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ydd.fengsongda.top

[Q61] 移动平均
来源：http://ljc.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qap.ydzc1.top

[Q62] 分组占比
来源：http://ovo.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kmf.jlsjyb.cn

[Q63] 开启事务
来源：http://ena.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vwd.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://tuq.cashguo.top

COMMIT;
来源：http://yks.bjfxy.top

[Q65] 回滚事务
来源：http://bhh.yfazqb.com

ROLLBACK;
来源：http://pyh.birdmap.top

[Q66] 行锁查询
来源：http://olh.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kgc.bbcook.cn

[Q67] 设置隔离级别
来源：http://xwo.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://imn.nwbrower.top

[Q68] 保存点
来源：http://nrf.xylfe.cn

SAVEPOINT sp1;
来源：http://jhq.svipenyu.cn

ROLLBACK TO sp1;
来源：http://acp.andypj.xyz

[Q69] 查看执行计划
来源：http://jtx.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ouo.dianchejie.cn

[Q70] 更新统计信息
来源：http://jnb.fengsongda.top

ANALYZE TABLE users;
来源：http://dyr.birdmap.top

[Q71] 查看建表语句
来源：http://ixu.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbl.zycfv.cn

[Q72] 查看索引
来源：http://ejc.jianghu66.top

SHOW INDEX FROM users;
来源：http://ymt.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://saa.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://zyi.nanxinkj.top

[Q74] 强制使用索引
来源：http://wke.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bkf.jiagoushi.top

[Q75] 日期格式化
来源：http://poo.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pwe.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hzi.tanke756.top

[Q76] 按天统计
来源：http://kru.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zcw.yvedp.cn

[Q77] 时间加减
来源：http://jsb.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fps.tian-w.cn

[Q78] 当前时间
来源：http://sqg.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qld.tianlin.xyz

[Q79] 字符串拼接
来源：http://gei.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vni.jyoumei.cn

[Q80] 字符串截取
来源：http://wob.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mdc.daxiang520.top

[Q81] 字符串替换
来源：http://mbm.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://enp.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://jac.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tpo.epnwcf.com

[Q83] 大小写转换
来源：http://yik.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zgb.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://fgj.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://wfj.bbcook.cn

[Q85] 数值取整
来源：http://fuf.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hpz.meibo888.top

[Q86] 读取 JSON 字段
来源：http://gsk.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kys.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://wlf.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ymf.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://wqx.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lzr.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eaz.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://ogt.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dew.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://avm.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fmn.mhx1999.top

================================================================================
来源：http://jun.kuanghao11.cn

R. Bash 专题
来源：http://lwr.jqgfzy.top

================================================================================
来源：http://uqh.dianchejie.cn

[R01] shebang 与严格模式
来源：http://wjc.gotoacloud.top

#!/usr/bin/env bash
来源：http://brm.nanxuanxn.top

set -euo pipefail
来源：http://ook.hywenlv.cn

[R02] 变量赋值与使用
来源：http://yub.yj202588.top

name="Tom"; echo "$name"
来源：http://ens.jqgfzy.top

[R03] 只读变量
来源：http://dmd.chenzaomai.com

readonly PI=3.14
来源：http://wds.jinqigfzy.top

[R04] 位置参数
来源：http://xdi.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ddg.xinyue.icu

[R05] 参数默认值
来源：http://bxm.vqdsnc.cn

name="${1:-default}"
来源：http://sya.tarul.cn

[R06] 判断命令是否存在
来源：http://khg.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lzh.guannengcc.top

[R07] if 判断文件
来源：http://ftx.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yjz.jyoumei.cn

[R08] 数值比较
来源：http://gas.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rca.yj20258.top

[R09] 字符串比较
来源：http://zba.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yke.zycfv.cn

[R10] 正则匹配
来源：http://wnz.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xen.cheryme.top

[R11] case 多分支
来源：http://zac.yuxming.cn

case "$1" in
来源：http://fhd.fehbvm.com

start) echo "启动" ;;
来源：http://zbw.yj202588.top

stop)  echo "停止" ;;
来源：http://ljo.wangdashe.top

*)     echo "未知命令" ;;
来源：http://cwp.hesvh.cn

esac
来源：http://uvr.svipenyu.cn

[R12] for 遍历文件
来源：http://hsr.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://yac.52xcode.cn

[R13] for 计数循环
来源：http://xna.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://ias.xziqi.cn

[R14] C 风格 for
来源：http://oxd.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qat.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://lxu.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ioc.gaohongyu789.top

[R16] until 等待条件
来源：http://nom.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tek.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://dlm.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://bgu.fktsv.cn

[R18] 遍历数组
来源：http://ctr.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rke.jlsjyb.cn

[R19] 数组长度
来源：http://svn.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://ufs.zhengqikj.top

[R20] 关联数组（字典）
来源：http://cwo.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fkr.52xcode.cn

[R21] 字符串长度
来源：http://esw.guowangkeji.top

echo "${#s}"
来源：http://mcb.xinyue.icu

[R22] 截取子串
来源：http://yeb.shangyingyoupin.top

echo "${s:0:5}"
来源：http://ifk.cqqwz.cn

[R23] 字符串替换
来源：http://piq.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://epp.quarkkingdee.top

[R24] 大小写转换
来源：http://zhg.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://itt.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://nfm.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gbn.yangfankeji.com

[R26] 命令替换
来源：http://wnh.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://dyu.hywenlv.cn

[R27] 算术展开
来源：http://ovq.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://jtl.mhx1999.top

[R28] 浮点运算
来源：http://kty.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://vdy.fehbvm.com

[R29] 定义函数
来源：http://ijn.cqqwz.cn


<!-- 参考信息 -->