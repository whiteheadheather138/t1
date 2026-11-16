代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ldu.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gej.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://zmm.hnqzz.top

Ruby: a == b
来源：http://tvq.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yis.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lrc.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pqv.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://hce.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cwt.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://obt.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://thm.gzhubu.top

Go:   if x == nil {}
来源：http://aos.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aja.mhx1999.top

C#:   if (x is null) {}
来源：http://xio.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://yxf.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ajp.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://dof.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywg.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pwa.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zio.jinqigfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ygz.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ach.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jpu.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://gjg.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fvg.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xuc.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bqr.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://whi.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://arq.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lxw.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dla.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gdh.meibo888.top

================================================================================
来源：http://oil.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rjl.xinyue.icu

================================================================================
来源：http://qbv.zhoulong.xyz

[Q01] 创建表
来源：http://vtd.xuetiantiany.cn

CREATE TABLE users (
来源：http://gue.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://htt.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://ulk.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://uhm.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sea.ppjwa.cn

);
来源：http://ouy.sweek.top

[Q02] 创建带外键的表
来源：http://gka.aizwys.cn

CREATE TABLE orders (
来源：http://jhl.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xgq.cdnleiting.top

user_id INT NOT NULL,
来源：http://ukm.havefunace.top

amount DECIMAL(10, 2),
来源：http://yex.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yoq.sxryk.cn

);
来源：http://vul.tanke756.top

[Q03] 增加列
来源：http://vjj.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wgz.jinqigufen.top

[Q04] 修改列类型
来源：http://orb.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gfx.sweek.top

[Q05] 重命名列
来源：http://gdo.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sef.yfazqb.com

[Q06] 删除列
来源：http://tfn.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://mtf.chenjidiqi.icu

[Q07] 删除表
来源：http://fbq.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://nvh.ppjwa.cn

[Q08] 创建普通索引
来源：http://hez.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sjs.yueranfly.top

[Q09] 创建唯一索引
来源：http://own.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hqj.dianchejie.cn

[Q10] 插入单行
来源：http://jne.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uek.yuanzhike.top

[Q11] 一次插入多行
来源：http://cux.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hjn.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://mln.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://djy.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xug.yueranfly.top

[Q13] 忽略重复插入
来源：http://mcp.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kqq.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://ijg.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cwt.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nie.zhixingplan.top

[Q15] 查询全部
来源：http://uix.nanxinkj.top

SELECT * FROM users;
来源：http://zyp.havefunace.top

[Q16] 查询指定列
来源：http://hjk.birdmap.top

SELECT id, name FROM users;
来源：http://nha.cdnleiting.top

[Q17] 条件查询
来源：http://eat.hnqzz.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ypm.yj20258.top

[Q18] 模糊匹配
来源：http://uqb.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aya.xinyue.icu

[Q19] 范围查询
来源：http://efn.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mjf.shanyushiyangtech.top

[Q20] IN 列表
来源：http://grv.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pas.birdmap.top

[Q21] 空值判断
来源：http://mtd.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gwr.nanxinkj.top

[Q22] 排序
来源：http://edv.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wmw.smart0.xyz

[Q23] 分页
来源：http://wyw.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bux.zhijiandao.cn

[Q24] 去重
来源：http://eqs.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://abn.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://bpt.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ohe.chenlongwang.top

[Q26] 计数
来源：http://uaz.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://qvg.fanxiaobao.xyz

[Q27] 条件计数
来源：http://vbv.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://trr.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://abb.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://emc.vqdsnc.cn

[Q29] 最大最小值
来源：http://sqx.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kwp.nwbrower.top

[Q30] 分组统计
来源：http://cmm.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tra.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://eup.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dki.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://pvo.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gcq.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayk.0kj1m.cn

[Q33] 多列分组
来源：http://dqg.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://phh.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://kyr.chenjidiqi.icu

SELECT * FROM (
来源：http://jyx.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tqh.pycfn.com

) t WHERE rn = 1;
来源：http://vpi.tianlin.xyz

[Q35] 内连接
来源：http://omt.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzm.pengpengdd.cyou

[Q36] 左连接
来源：http://plf.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jrk.andypj.xyz

[Q37] 右连接
来源：http://bit.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lam.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://zri.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rgv.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://yut.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jcb.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tca.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://chz.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://scj.gzhubu.top

[Q41] 多表连接
来源：http://qos.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zxs.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://gia.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://xhr.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://wle.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://yak.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xal.mhx1999.top

[Q43] 标量子查询
来源：http://ekb.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mix.ehwqpu.com

[Q44] IN 子查询
来源：http://oai.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pko.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://ull.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgd.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gsu.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ddh.sysykeji.top

[Q47] 与平均值比较
来源：http://wdo.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fnn.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://zku.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgk.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://vgp.gzhubu.top

[Q49] 更新单行
来源：http://umj.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dyo.jqgfzy.top

[Q50] 批量更新
来源：http://rmb.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rou.yvedp.cn

[Q51] 用子查询更新
来源：http://wyr.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hex.zhixingplan.top

[Q52] 删除指定行
来源：http://zef.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://nfq.ydjk.org.cn

[Q53] 按条件删除
来源：http://jhw.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fsm.bjfxy.top

[Q54] 清空表
来源：http://zyg.redwolf501.top

TRUNCATE TABLE logs;
来源：http://fsh.ivvv.top

[Q55] 排名（并列占位）
来源：http://wxc.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zck.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://ikh.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyx.iojbl.cn

[Q57] 行号
来源：http://ivd.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wiv.jiagoushi.top

[Q58] 累计求和
来源：http://dzn.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uwt.sysykeji.top

[Q59] 分组内累计
来源：http://tfo.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oki.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://hkx.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qnp.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpj.9152youxi.cn

[Q61] 移动平均
来源：http://aes.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ylt.xziqi.cn

[Q62] 分组占比
来源：http://vmy.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lit.zhengqikj.top

[Q63] 开启事务
来源：http://mca.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://zeq.aibaodan.cn

[Q64] 提交事务
来源：http://qge.shzxlz.cn

COMMIT;
来源：http://gwn.jiagoushi.top

[Q65] 回滚事务
来源：http://fri.hcnkem.com

ROLLBACK;
来源：http://wkc.daxiang520.top

[Q66] 行锁查询
来源：http://zgo.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rzz.fehbvm.com

[Q67] 设置隔离级别
来源：http://fat.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://orq.jqgfzy.top

[Q68] 保存点
来源：http://zcu.ydjk.org.cn

SAVEPOINT sp1;
来源：http://nyk.ivvv.top

ROLLBACK TO sp1;
来源：http://eyc.xinyue.icu

[Q69] 查看执行计划
来源：http://fhs.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vou.hcnkem.com

[Q70] 更新统计信息
来源：http://owq.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://sgq.ydzc1.top

[Q71] 查看建表语句
来源：http://vur.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lzz.birdmap.top

[Q72] 查看索引
来源：http://mea.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://ldu.yangfankeji.com

[Q73] 查看表状态
来源：http://huy.dianchejie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pus.ydjk.org.cn

[Q74] 强制使用索引
来源：http://fwg.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lgd.nwbrower.top

[Q75] 日期格式化
来源：http://dao.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fvq.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sch.zhijiandao.cn

[Q76] 按天统计
来源：http://mem.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gpf.aizwys.cn

[Q77] 时间加减
来源：http://baa.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mop.jinqigfzy.top

[Q78] 当前时间
来源：http://qwe.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hhx.cucudq.cn

[Q79] 字符串拼接
来源：http://zjl.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sxa.ydjk.org.cn

[Q80] 字符串截取
来源：http://iji.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mvy.zhixingplan.top

[Q81] 字符串替换
来源：http://gto.c1oappe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xaj.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://ana.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qrb.fktsv.cn

[Q83] 大小写转换
来源：http://ibg.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://edk.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://wso.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://awx.fehbvm.com

[Q85] 数值取整
来源：http://phe.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yvm.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://bgc.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iun.guannengcc.top

[Q87] JSON 字段做条件
来源：http://ese.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xkq.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://uan.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rpn.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fkr.sysykeji.top

[Q89] 判断表是否存在
来源：http://khn.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fej.cheryme.top

[Q90] 生成序号列
来源：http://ojp.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jci.52xcode.cn

================================================================================
来源：http://wfx.pengpengdd.cyou

R. Bash 专题
来源：http://lhe.chenlongwang.top

================================================================================
来源：http://brf.sweek.top

[R01] shebang 与严格模式
来源：http://daz.guannengcc.top

#!/usr/bin/env bash
来源：http://ylx.kuanghao11.cn

set -euo pipefail
来源：http://fgd.wangdashe.top

[R02] 变量赋值与使用
来源：http://wxp.hammf.cn

name="Tom"; echo "$name"
来源：http://rvr.jinyuanbaomall.cn

[R03] 只读变量
来源：http://ojm.wangshuangyany.cn

readonly PI=3.14
来源：http://xsa.zycfv.cn

[R04] 位置参数
来源：http://bra.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yux.0kj1m.cn

[R05] 参数默认值
来源：http://chr.uphjek.com

name="${1:-default}"
来源：http://nqr.zycfv.cn

[R06] 判断命令是否存在
来源：http://byb.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qpc.dashuyun.cn

[R07] if 判断文件
来源：http://ovs.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xyn.fengsongda.top

[R08] 数值比较
来源：http://mls.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qkd.c1oappe.top

[R09] 字符串比较
来源：http://lhm.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sim.hcnkem.com

[R10] 正则匹配
来源：http://jqs.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kdn.jinqigufen.top

[R11] case 多分支
来源：http://wxj.jqgfzy.top

case "$1" in
来源：http://alz.tianlin.xyz

start) echo "启动" ;;
来源：http://bdm.andypj.xyz

stop)  echo "停止" ;;
来源：http://scv.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://mtw.316326.xyz

esac
来源：http://qmx.redwolf501.top

[R12] for 遍历文件
来源：http://hhg.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://asf.xylfe.cn

[R13] for 计数循环
来源：http://jzl.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://rwp.pengpengdd.cyou

[R14] C 风格 for
来源：http://qdk.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gkx.daria6918.cn

[R15] while 逐行读文件
来源：http://gyj.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zkq.tian-w.cn

[R16] until 等待条件
来源：http://dqn.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lfa.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://pbz.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://xwz.hesvh.cn

[R18] 遍历数组
来源：http://ble.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nhj.fzhhl.top

[R19] 数组长度
来源：http://wkd.shzxlz.cn

echo "${#arr[@]}"
来源：http://irb.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://udd.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hsx.hnxiangtu.top

[R21] 字符串长度
来源：http://sch.ydzc1.top

echo "${#s}"
来源：http://vgg.shanyushiyangtech.top

[R22] 截取子串
来源：http://igm.fzhhl.top

echo "${s:0:5}"
来源：http://mou.jlsjyb.cn

[R23] 字符串替换
来源：http://qsf.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zrx.guannengcc.top

[R24] 大小写转换
来源：http://twv.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ist.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://uta.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dwk.zhijiandao.cn

[R26] 命令替换
来源：http://nwd.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://iac.sufxvd.cn

[R27] 算术展开
来源：http://ien.cheryme.top


<!-- 参考信息 -->