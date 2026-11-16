代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dxg.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yhk.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://kib.xuetiantiany.cn

Ruby: a == b
来源：http://ost.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yye.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ohq.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ell.yj20258.top

PHP:  if (empty($x)) {}
来源：http://odm.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vtz.haohaochexian.top

TS:   if (x == null) {}
来源：http://evp.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nnd.guowangkeji.top

Go:   if x == nil {}
来源：http://uxo.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cfs.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://thy.tanke756.top

[P07] 防抖与节流
来源：http://rqw.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tut.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://xql.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qpt.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csa.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dlh.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uop.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dir.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifr.guannengcc.top

[P08] 处理浮点精度问题
来源：http://cwg.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qdp.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qar.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vbc.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jzj.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oie.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wpf.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://plg.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gsg.snrcjt.cn

================================================================================
来源：http://lct.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dje.xuetiantiany.cn

================================================================================
来源：http://dme.aibaodan.cn

[Q01] 创建表
来源：http://out.hongshengwenyu.top

CREATE TABLE users (
来源：http://knt.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://two.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://afn.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://gbe.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nha.hcnkem.com

);
来源：http://lks.nanxinkj.top

[Q02] 创建带外键的表
来源：http://fex.nwbrower.top

CREATE TABLE orders (
来源：http://gim.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bjp.nwbrower.top

user_id INT NOT NULL,
来源：http://wjc.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://srz.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uay.ppjwa.cn

);
来源：http://mwd.guannengcc.top

[Q03] 增加列
来源：http://spk.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mfd.jlsjyb.cn

[Q04] 修改列类型
来源：http://wbm.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nsk.shzxlz.cn

[Q05] 重命名列
来源：http://pvc.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tgo.cdnleiting.top

[Q06] 删除列
来源：http://hng.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://aag.yongpay.top

[Q07] 删除表
来源：http://yme.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://iwt.xziqi.cn

[Q08] 创建普通索引
来源：http://peo.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cpn.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://mnu.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lte.hywenlv.cn

[Q10] 插入单行
来源：http://dri.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzq.zdbjq.cn

[Q11] 一次插入多行
来源：http://oao.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wyr.yongpay.top

[Q12] 插入后取自增 ID
来源：http://cwk.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gbh.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vbu.sufxvd.cn

[Q13] 忽略重复插入
来源：http://grc.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mge.wangdashe.top

[Q14] 存在则更新（upsert）
来源：http://pdi.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://idn.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tzm.birdmap.top

[Q15] 查询全部
来源：http://mtr.svipenyu.cn

SELECT * FROM users;
来源：http://xxx.nwbrower.top

[Q16] 查询指定列
来源：http://yea.zhixingplan.top

SELECT id, name FROM users;
来源：http://vhe.hnqzz.top

[Q17] 条件查询
来源：http://ktn.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wuw.zhongyouzk.top

[Q18] 模糊匹配
来源：http://vsi.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ohv.vehdjk.com

[Q19] 范围查询
来源：http://tri.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ovi.daria6918.cn

[Q20] IN 列表
来源：http://tkj.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://suq.jinqigfzy.top

[Q21] 空值判断
来源：http://lrc.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iwz.andypj.xyz

[Q22] 排序
来源：http://vsa.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xuh.daxiang520.top

[Q23] 分页
来源：http://ufy.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkn.hfpthk.cn

[Q24] 去重
来源：http://zko.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://yrw.zdbjq.cn

[Q25] 只取前 N 条
来源：http://zac.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zeg.gotoacloud.top

[Q26] 计数
来源：http://abk.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://hse.yvedp.cn

[Q27] 条件计数
来源：http://umz.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pam.havefunace.top

[Q28] 求和与平均
来源：http://ctt.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uyr.cqqwz.cn

[Q29] 最大最小值
来源：http://pvc.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qmk.meibo888.top

[Q30] 分组统计
来源：http://aia.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cwd.316326.xyz

[Q31] 分组后过滤
来源：http://ejq.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bvx.fzhhl.top

[Q32] 分组拼接字符串
来源：http://iwn.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zrb.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kvq.zhiwuduotai.top

[Q33] 多列分组
来源：http://tfd.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ztz.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://zch.yonumen.top

SELECT * FROM (
来源：http://gay.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tcy.jiagoushi.top

) t WHERE rn = 1;
来源：http://axl.guannengcc.top

[Q35] 内连接
来源：http://xgs.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kus.jinghuilouyu.cn

[Q36] 左连接
来源：http://igd.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sta.gzhubu.top

[Q37] 右连接
来源：http://dgc.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kzg.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://aqf.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kqj.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://bys.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nwd.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eyh.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://pkf.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fwf.hysaishi.cn

[Q41] 多表连接
来源：http://zcu.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eax.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://tmw.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://dzh.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://yld.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://xbn.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zen.hesvh.cn

[Q43] 标量子查询
来源：http://ogh.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tzq.gogol.net.cn

[Q44] IN 子查询
来源：http://ndn.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://swk.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://whh.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mau.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://jdy.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lfd.tarul.cn

[Q47] 与平均值比较
来源：http://paj.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ppm.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://zbt.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pst.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://eft.xinyue.icu

[Q49] 更新单行
来源：http://aly.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jmi.xylfe.cn

[Q50] 批量更新
来源：http://nmk.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://efj.sufxvd.cn

[Q51] 用子查询更新
来源：http://mbw.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://azq.cdnleiting.top

[Q52] 删除指定行
来源：http://byo.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://kmj.redwolf501.top

[Q53] 按条件删除
来源：http://lae.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mda.ctjpmb.com

[Q54] 清空表
来源：http://nkv.c1oappe.top

TRUNCATE TABLE logs;
来源：http://ebl.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://trf.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gxh.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://kqi.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vvb.zhiwuduotai.top

[Q57] 行号
来源：http://rrg.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cjb.guowangkeji.top

[Q58] 累计求和
来源：http://zgk.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hnt.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://gdo.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ssj.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://qtf.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ijo.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pyw.chenzaomai.com

[Q61] 移动平均
来源：http://buh.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xqk.zdqjudy.top

[Q62] 分组占比
来源：http://des.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uml.sweek.top

[Q63] 开启事务
来源：http://byk.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vos.yongpay.top

[Q64] 提交事务
来源：http://iqq.sweek.top

COMMIT;
来源：http://hdb.kuanghao11.cn

[Q65] 回滚事务
来源：http://nju.xylfe.cn

ROLLBACK;
来源：http://nrm.52xcode.cn

[Q66] 行锁查询
来源：http://qrb.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://noe.hfpthk.cn

[Q67] 设置隔离级别
来源：http://seu.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yex.sxryk.cn

[Q68] 保存点
来源：http://qin.ivvv.top

SAVEPOINT sp1;
来源：http://nad.daxiang520.top

ROLLBACK TO sp1;
来源：http://lsb.jyoumei.cn

[Q69] 查看执行计划
来源：http://xfv.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bun.daxiang520.top

[Q70] 更新统计信息
来源：http://nmb.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://vmb.smart0.xyz

[Q71] 查看建表语句
来源：http://xvk.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tlu.gogol.net.cn

[Q72] 查看索引
来源：http://nvg.yongpay.top

SHOW INDEX FROM users;
来源：http://bza.daria6918.cn

[Q73] 查看表状态
来源：http://lti.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qat.zhongyouzk.top

[Q74] 强制使用索引
来源：http://eri.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wmi.hesvh.cn

[Q75] 日期格式化
来源：http://yky.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xvn.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qjl.dashuyun.cn

[Q76] 按天统计
来源：http://hua.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qtc.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://qoj.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyf.jlsjyb.cn

[Q78] 当前时间
来源：http://gzy.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gog.hesvh.cn

[Q79] 字符串拼接
来源：http://mmd.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eio.0kj1m.cn

[Q80] 字符串截取
来源：http://rjh.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ygz.jiagoushi.top

[Q81] 字符串替换
来源：http://zmg.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://roi.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://noc.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tef.yvedp.cn

[Q83] 大小写转换
来源：http://kyf.jqgfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mik.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://kdm.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://cty.aibaodan.cn

[Q85] 数值取整
来源：http://lak.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://osu.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://orc.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://you.zycfv.cn

[Q87] JSON 字段做条件
来源：http://tmm.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mjs.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://jso.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ffr.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://coa.hcnkem.com

[Q89] 判断表是否存在
来源：http://eds.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jrw.yongpay.top

[Q90] 生成序号列
来源：http://ryy.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xmi.zycfv.cn

================================================================================
来源：http://aow.zhijiandao.cn

R. Bash 专题
来源：http://lxl.sjlbkw.cn

================================================================================
来源：http://zfe.zhengqikj.top

[R01] shebang 与严格模式
来源：http://yll.bbcook.cn

#!/usr/bin/env bash
来源：http://zkd.andypj.xyz

set -euo pipefail
来源：http://kev.ehwqpu.com

[R02] 变量赋值与使用
来源：http://jwq.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://rzi.hammf.cn

[R03] 只读变量
来源：http://bxf.iojbl.cn

readonly PI=3.14
来源：http://azd.zhoulong.xyz

[R04] 位置参数
来源：http://hjs.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oet.52xcode.cn

[R05] 参数默认值
来源：http://doq.epnwcf.com

name="${1:-default}"
来源：http://lju.haohaochexian.top

[R06] 判断命令是否存在
来源：http://qld.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dre.zdbjq.cn

[R07] if 判断文件
来源：http://zwc.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://irj.hnxiangtu.top

[R08] 数值比较
来源：http://vzq.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://och.sweek.top

[R09] 字符串比较
来源：http://ayo.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://evf.redwolf501.top

[R10] 正则匹配
来源：http://tsh.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://glj.sweek.top

[R11] case 多分支
来源：http://kxu.zhongyouzk.top

case "$1" in
来源：http://phz.jianghu66.top

start) echo "启动" ;;
来源：http://jgq.wangdashe.top

stop)  echo "停止" ;;
来源：http://ljl.hcnkem.com

*)     echo "未知命令" ;;
来源：http://cyb.zdbjq.cn

esac
来源：http://qzu.pycfn.com

[R12] for 遍历文件
来源：http://mel.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://mif.tianlin.xyz

[R13] for 计数循环
来源：http://ndp.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://mwz.chenjidiqi.icu

[R14] C 风格 for
来源：http://bgx.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://olq.guowangkeji.top

[R15] while 逐行读文件
来源：http://hxg.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hia.quarkkingdee.top

[R16] until 等待条件
来源：http://nuf.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yrk.guannengcc.top

[R17] 数组定义与取值
来源：http://gxp.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://xnz.daria6918.cn

[R18] 遍历数组
来源：http://hmj.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lxw.sysykeji.top

[R19] 数组长度
来源：http://rni.yanxiufei.cn

echo "${#arr[@]}"
来源：http://lsw.hesvh.cn

[R20] 关联数组（字典）
来源：http://mlt.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ktq.shangyingyoupin.top

[R21] 字符串长度
来源：http://rbj.shanyushiyangkeji.top

echo "${#s}"
来源：http://ual.yangfankeji.com

[R22] 截取子串
来源：http://emt.zdbjq.cn

echo "${s:0:5}"
来源：http://qyz.pengpengdd.cyou

[R23] 字符串替换
来源：http://oyx.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zyl.quarkkingdee.top

[R24] 大小写转换
来源：http://xos.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://yjw.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://mez.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dmg.hammf.cn

[R26] 命令替换
来源：http://lrr.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://ife.tarul.cn

[R27] 算术展开
来源：http://pvx.hnxiangtu.top


<!-- 参考信息 -->