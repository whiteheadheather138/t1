代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eru.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ujp.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yio.wangshuangyany.cn

Ruby: a == b
来源：http://okg.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tpb.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ani.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uwe.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://beg.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rvq.bjfxy.top

TS:   if (x == null) {}
来源：http://aua.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ati.cqqwz.cn

Go:   if x == nil {}
来源：http://nqt.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hxm.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://hkw.bbcook.cn

[P07] 防抖与节流
来源：http://dei.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sah.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://xki.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://stf.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsg.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yif.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://duk.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pdb.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yyf.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://dyq.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zzt.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ign.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://viu.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lha.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gvh.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bqp.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hwx.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://exp.gotoacloud.top

================================================================================
来源：http://qyj.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohx.guowangkeji.top

================================================================================
来源：http://xkh.hesvh.cn

[Q01] 创建表
来源：http://dtk.tanke756.top

CREATE TABLE users (
来源：http://tut.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rcc.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://gxm.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://otq.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eda.fanxiaobao.xyz

);
来源：http://niy.fengsongda.top

[Q02] 创建带外键的表
来源：http://tyx.daxiang520.top

CREATE TABLE orders (
来源：http://dwc.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hxw.sweek.top

user_id INT NOT NULL,
来源：http://ozb.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://zaq.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cxp.hcnkem.com

);
来源：http://gvw.pengpengdd.cyou

[Q03] 增加列
来源：http://kji.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://klx.zhoulong.xyz

[Q04] 修改列类型
来源：http://csj.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jpy.shzxlz.cn

[Q05] 重命名列
来源：http://xio.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lah.sufxvd.cn

[Q06] 删除列
来源：http://gyi.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pwa.jinghuilouyu.cn

[Q07] 删除表
来源：http://aqm.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://ise.zdbjq.cn

[Q08] 创建普通索引
来源：http://dzl.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ewt.pycfn.com

[Q09] 创建唯一索引
来源：http://bsi.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gee.jlsjyb.cn

[Q10] 插入单行
来源：http://isv.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dvh.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://rxj.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tvx.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://zgs.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wmd.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mmo.fengsongda.top

[Q13] 忽略重复插入
来源：http://hng.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqt.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://xmt.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uen.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fwy.zhijiandao.cn

[Q15] 查询全部
来源：http://nqx.shuidangran.top

SELECT * FROM users;
来源：http://iay.daxiang520.top

[Q16] 查询指定列
来源：http://ynk.shuidangran.top

SELECT id, name FROM users;
来源：http://vlc.vehdjk.com

[Q17] 条件查询
来源：http://dsa.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://etz.cheryme.top

[Q18] 模糊匹配
来源：http://knf.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hnp.jinghuilouyu.cn

[Q19] 范围查询
来源：http://tao.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wjl.epnwcf.com

[Q20] IN 列表
来源：http://jer.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eaz.cashguo.top

[Q21] 空值判断
来源：http://lbs.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://csf.vqdsnc.cn

[Q22] 排序
来源：http://vvy.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sag.sjlbkw.cn

[Q23] 分页
来源：http://kai.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bed.xziqi.cn

[Q24] 去重
来源：http://nss.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://wjs.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://fox.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://huq.52xcode.cn

[Q26] 计数
来源：http://uny.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://vfh.vehdjk.com

[Q27] 条件计数
来源：http://cmr.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://flj.snrcjt.cn

[Q28] 求和与平均
来源：http://fkd.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uvc.fengsongda.top

[Q29] 最大最小值
来源：http://zit.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bcp.xuanzx.com

[Q30] 分组统计
来源：http://lpm.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://axk.iojbl.cn

[Q31] 分组后过滤
来源：http://pfl.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xow.fehbvm.com

[Q32] 分组拼接字符串
来源：http://ejz.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sto.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yuz.ybcxt.top

[Q33] 多列分组
来源：http://fsp.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://trc.smart0.xyz

[Q34] 每组取第一条
来源：http://fsi.vehdjk.com

SELECT * FROM (
来源：http://icg.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rhx.yuanzhike.top

) t WHERE rn = 1;
来源：http://lbk.vehdjk.com

[Q35] 内连接
来源：http://ypz.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://egq.havefunace.top

[Q36] 左连接
来源：http://gpn.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://umt.chenjidiqi.icu

[Q37] 右连接
来源：http://ygu.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggq.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://eby.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mak.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://yhh.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdo.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gmw.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yif.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://abn.hfpthk.cn

[Q41] 多表连接
来源：http://gfs.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://vme.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://dzk.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://vnu.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://vxy.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://hng.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pvv.daria6918.cn

[Q43] 标量子查询
来源：http://bfg.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dxe.mhx1999.top

[Q44] IN 子查询
来源：http://arc.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rmk.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://nsi.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eel.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://dkc.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jrq.gogol.net.cn

[Q47] 与平均值比较
来源：http://bjw.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ygy.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://ojv.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://krp.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://epa.xylfe.cn

[Q49] 更新单行
来源：http://ljk.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://obt.zhijiandao.cn

[Q50] 批量更新
来源：http://zlb.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qad.ctjpmb.com

[Q51] 用子查询更新
来源：http://jun.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tso.yj202588.top

[Q52] 删除指定行
来源：http://xcz.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://eda.jqgfzy.top

[Q53] 按条件删除
来源：http://uzf.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cnh.shanyushiyangtech.top

[Q54] 清空表
来源：http://hco.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://cwo.hesvh.cn

[Q55] 排名（并列占位）
来源：http://jhr.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vpn.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://iam.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tfm.fanxiaobao.xyz

[Q57] 行号
来源：http://szd.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gms.wangshuangyany.cn

[Q58] 累计求和
来源：http://xju.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ntv.tianlin.xyz

[Q59] 分组内累计
来源：http://dsg.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sfq.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://clw.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://arn.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jgu.kuanghao11.cn

[Q61] 移动平均
来源：http://inb.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rad.hesvh.cn

[Q62] 分组占比
来源：http://fci.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qjt.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://qfi.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ukw.aibaodan.cn

[Q64] 提交事务
来源：http://gul.ppjwa.cn

COMMIT;
来源：http://yih.chenjidiqi.icu

[Q65] 回滚事务
来源：http://ljh.fengsongda.top

ROLLBACK;
来源：http://lrm.wangdashe.top

[Q66] 行锁查询
来源：http://uai.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vxv.tarul.cn

[Q67] 设置隔离级别
来源：http://fat.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lch.vehdjk.com

[Q68] 保存点
来源：http://fmu.sjlbkw.cn

SAVEPOINT sp1;
来源：http://dto.yvedp.cn

ROLLBACK TO sp1;
来源：http://qvc.bjfxy.top

[Q69] 查看执行计划
来源：http://gip.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ixr.yangfankeji.com

[Q70] 更新统计信息
来源：http://kfb.xuanzx.com

ANALYZE TABLE users;
来源：http://cmh.gotoacloud.top

[Q71] 查看建表语句
来源：http://paz.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pvz.dashuyun.cn

[Q72] 查看索引
来源：http://iwl.316326.xyz

SHOW INDEX FROM users;
来源：http://vuf.mhx1999.top

[Q73] 查看表状态
来源：http://hmi.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ane.yfazqb.com

[Q74] 强制使用索引
来源：http://acv.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xwz.yuxming.cn

[Q75] 日期格式化
来源：http://zys.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hcc.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hhl.chenlongwang.top

[Q76] 按天统计
来源：http://ddq.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iac.nanxinkj.top

[Q77] 时间加减
来源：http://kpc.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aig.birdmap.top

[Q78] 当前时间
来源：http://nuu.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kxn.yvedp.cn

[Q79] 字符串拼接
来源：http://ufz.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gzp.gogol.net.cn

[Q80] 字符串截取
来源：http://jrc.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sdu.epnwcf.com

[Q81] 字符串替换
来源：http://xoy.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dyr.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://xsp.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fcx.hysaishi.cn

[Q83] 大小写转换
来源：http://owr.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sim.yangfankeji.com

[Q84] 去除首尾空格
来源：http://iid.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://xzt.redwolf501.top

[Q85] 数值取整
来源：http://yef.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bxz.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://acr.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ccg.ybcxt.top

[Q87] JSON 字段做条件
来源：http://yqu.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://upd.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://tuz.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ava.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wny.cdnleiting.top

[Q89] 判断表是否存在
来源：http://nzk.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ljg.zhengqikj.top

[Q90] 生成序号列
来源：http://knu.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnc.zhijiandao.cn

================================================================================
来源：http://krn.yj20258.top

R. Bash 专题
来源：http://iaw.chenzaomai.com

================================================================================
来源：http://mta.fehbvm.com

[R01] shebang 与严格模式
来源：http://kjs.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://yza.xuanzx.com

set -euo pipefail
来源：http://nti.hcnkem.com

[R02] 变量赋值与使用
来源：http://rxm.yuxming.cn

name="Tom"; echo "$name"
来源：http://ghn.zdqjudy.top

[R03] 只读变量
来源：http://xaa.tanke756.top

readonly PI=3.14
来源：http://byg.smart0.xyz

[R04] 位置参数
来源：http://fyo.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nlc.zhoulong.xyz

[R05] 参数默认值
来源：http://kvx.jinyuanbaomall.cn

name="${1:-default}"
来源：http://fqh.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://smq.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fce.cdnleiting.top

[R07] if 判断文件
来源：http://eud.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://glp.xinyue.icu

[R08] 数值比较
来源：http://bzz.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lyf.birdmap.top

[R09] 字符串比较
来源：http://xgm.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tgp.zhiwuduotai.top

[R10] 正则匹配
来源：http://lhu.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rpq.yvedp.cn

[R11] case 多分支
来源：http://smw.mhx1999.top

case "$1" in
来源：http://xhn.fehbvm.com

start) echo "启动" ;;
来源：http://pad.cheryme.top

stop)  echo "停止" ;;
来源：http://mba.c1oappe.top

*)     echo "未知命令" ;;
来源：http://gje.mhx1999.top

esac
来源：http://qbw.sjlbkw.cn

[R12] for 遍历文件
来源：http://osu.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://yij.svipenyu.cn

[R13] for 计数循环
来源：http://mdu.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://mpa.fehbvm.com

[R14] C 风格 for
来源：http://eaf.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tce.316326.xyz

[R15] while 逐行读文件
来源：http://dsc.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ajk.daxiang520.top

[R16] until 等待条件
来源：http://bsk.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://acp.zhijiandao.cn

[R17] 数组定义与取值
来源：http://vxz.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qpb.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://pjz.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uip.sysykeji.top

[R19] 数组长度
来源：http://uvt.quarkkingdee.top

echo "${#arr[@]}"
来源：http://yzz.hammf.cn

[R20] 关联数组（字典）
来源：http://jkp.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://asf.jiagoushi.top

[R21] 字符串长度
来源：http://wbb.aibaodan.cn

echo "${#s}"
来源：http://bzk.ivvv.top

[R22] 截取子串
来源：http://ing.yj20258888.top

echo "${s:0:5}"
来源：http://cje.fengsongda.top

[R23] 字符串替换
来源：http://toq.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iwm.haohaochexian.top

[R24] 大小写转换
来源：http://vaz.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://byv.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://phi.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://wti.xylfe.cn

[R26] 命令替换
来源：http://mce.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://epe.birdmap.top

[R27] 算术展开
来源：http://swk.fanxiaobao.xyz


<!-- 参考信息 -->