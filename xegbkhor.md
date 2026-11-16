代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hhm.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ixl.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://agl.haohaochexian.top

Ruby: a == b
来源：http://vgu.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gzj.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ljz.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tfg.havefunace.top

PHP:  if (empty($x)) {}
来源：http://osp.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vmx.yj20258888.top

TS:   if (x == null) {}
来源：http://oxm.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://svx.jinqigufen.top

Go:   if x == nil {}
来源：http://bvl.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cwi.yj20258.top

C#:   if (x is null) {}
来源：http://urc.yuanzhike.top

[P07] 防抖与节流
来源：http://lhk.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xyq.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://lku.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zss.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lyu.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fjo.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kgw.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://lpu.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uzb.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://vrg.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fps.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://atc.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ycg.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hmg.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wtl.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xyu.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kdm.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jyz.yvedp.cn

================================================================================
来源：http://bow.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wyo.yuxming.cn

================================================================================
来源：http://eqc.vehdjk.com

[Q01] 创建表
来源：http://psa.iojbl.cn

CREATE TABLE users (
来源：http://jre.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kmg.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://ssi.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://hql.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rww.snrcjt.cn

);
来源：http://tdc.havefunace.top

[Q02] 创建带外键的表
来源：http://ahz.yvedp.cn

CREATE TABLE orders (
来源：http://udl.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mbb.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://ykm.yfazqb.com

amount DECIMAL(10, 2),
来源：http://fzy.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpq.vqdsnc.cn

);
来源：http://mce.jyoumei.cn

[Q03] 增加列
来源：http://nen.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qns.gzhubu.top

[Q04] 修改列类型
来源：http://qqj.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ouo.52xcode.cn

[Q05] 重命名列
来源：http://rue.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rrk.smart0.xyz

[Q06] 删除列
来源：http://kff.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vfp.wangshuangyany.cn

[Q07] 删除表
来源：http://srb.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://mlz.zhoulong.xyz

[Q08] 创建普通索引
来源：http://uio.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xzv.cashguo.top

[Q09] 创建唯一索引
来源：http://mdu.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mtq.jqgfzy.top

[Q10] 插入单行
来源：http://hnd.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ule.nanxuanxn.top

[Q11] 一次插入多行
来源：http://grd.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mfj.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://tys.tanke756.top

INSERT INTO users (name) VALUES ('C');
来源：http://coj.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fgh.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://nhs.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vdk.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://lly.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://due.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnq.hongshengwenyu.top

[Q15] 查询全部
来源：http://irq.havefunace.top

SELECT * FROM users;
来源：http://nry.meibo888.top

[Q16] 查询指定列
来源：http://gbw.meibo888.top

SELECT id, name FROM users;
来源：http://glb.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://gkf.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csw.jqgfzy.top

[Q18] 模糊匹配
来源：http://kos.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dqs.fehbvm.com

[Q19] 范围查询
来源：http://hpq.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hgg.tianlin.xyz

[Q20] IN 列表
来源：http://qgz.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hgb.52xcode.cn

[Q21] 空值判断
来源：http://vsq.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ijg.9152youxi.cn

[Q22] 排序
来源：http://hkc.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tqf.sxryk.cn

[Q23] 分页
来源：http://iwu.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lsz.xuanzx.com

[Q24] 去重
来源：http://ile.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://xqh.zhengqikj.top

[Q25] 只取前 N 条
来源：http://vzp.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bts.zhongyouzk.top

[Q26] 计数
来源：http://hns.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://uft.fanxiaobao.xyz

[Q27] 条件计数
来源：http://sis.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://epe.yvedp.cn

[Q28] 求和与平均
来源：http://gwz.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ebw.fengsongda.top

[Q29] 最大最小值
来源：http://rnl.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zpa.haohaochexian.top

[Q30] 分组统计
来源：http://fky.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cht.gotoacloud.top

[Q31] 分组后过滤
来源：http://fhi.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hnp.ydzc1.top

[Q32] 分组拼接字符串
来源：http://cdb.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dqs.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dkx.fzhhl.top

[Q33] 多列分组
来源：http://dbr.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tpk.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://dga.zhixingplan.top

SELECT * FROM (
来源：http://vnf.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bsq.yj20258.top

) t WHERE rn = 1;
来源：http://eye.ehwqpu.com

[Q35] 内连接
来源：http://vci.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sei.iojbl.cn

[Q36] 左连接
来源：http://wvk.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wrz.shanyushiyangkeji.top

[Q37] 右连接
来源：http://nga.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jbq.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://wfo.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bhl.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://zhi.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nsh.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://trv.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vxp.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://utc.feifeiyinyue.top

[Q41] 多表连接
来源：http://vii.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bcl.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://yzd.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://vyc.yj202588.top

[Q42] 连接条件附加过滤
来源：http://qil.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://odo.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dhq.snrcjt.cn

[Q43] 标量子查询
来源：http://hwx.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dax.bjfxy.top

[Q44] IN 子查询
来源：http://vep.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jjw.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://wmf.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xul.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lek.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cit.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://zpp.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ugi.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://mou.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pff.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://kgh.jinghuilouyu.cn

[Q49] 更新单行
来源：http://zct.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dfu.gaohongyu789.top

[Q50] 批量更新
来源：http://xmb.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cet.uphjek.com

[Q51] 用子查询更新
来源：http://tgj.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fzl.jianghu66.top

[Q52] 删除指定行
来源：http://vli.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://jfd.nanxuanxn.top

[Q53] 按条件删除
来源：http://ihq.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hmd.chenzaomai.com

[Q54] 清空表
来源：http://mbt.vehdjk.com

TRUNCATE TABLE logs;
来源：http://zdi.pycfn.com

[Q55] 排名（并列占位）
来源：http://hhe.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jmz.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://dqz.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rak.yj20258888.top

[Q57] 行号
来源：http://zsf.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mih.yj202588.top

[Q58] 累计求和
来源：http://zwc.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lao.bbcook.cn

[Q59] 分组内累计
来源：http://fjm.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bzf.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://vxq.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qge.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cmv.uphjek.com

[Q61] 移动平均
来源：http://ezj.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qqx.tanke756.top

[Q62] 分组占比
来源：http://nnm.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ugz.yueranfly.top

[Q63] 开启事务
来源：http://boy.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ktg.snrcjt.cn

[Q64] 提交事务
来源：http://xsg.quarkkingdee.top

COMMIT;
来源：http://jpa.svipenyu.cn

[Q65] 回滚事务
来源：http://ucc.c1oappe.top

ROLLBACK;
来源：http://rsu.fktsv.cn

[Q66] 行锁查询
来源：http://kbl.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bbb.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://ctx.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mvc.chenzaomai.com

[Q68] 保存点
来源：http://gcw.c1oappe.top

SAVEPOINT sp1;
来源：http://sna.zhengqikj.top

ROLLBACK TO sp1;
来源：http://gkz.guannengcc.top

[Q69] 查看执行计划
来源：http://tbl.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qtt.9152youxi.cn

[Q70] 更新统计信息
来源：http://nyu.birdmap.top

ANALYZE TABLE users;
来源：http://cvq.chenlongwang.top

[Q71] 查看建表语句
来源：http://xdn.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hsq.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://eio.yfazqb.com

SHOW INDEX FROM users;
来源：http://fxa.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://hvw.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mpf.chenzaomai.com

[Q74] 强制使用索引
来源：http://xlm.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hdh.shangyingyoupin.top

[Q75] 日期格式化
来源：http://zif.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vja.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xjx.yuxming.cn

[Q76] 按天统计
来源：http://mgp.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zwn.shanyushiyangtech.top

[Q77] 时间加减
来源：http://cpy.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dqk.andypj.xyz

[Q78] 当前时间
来源：http://uqm.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gls.ybcxt.top

[Q79] 字符串拼接
来源：http://mih.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pza.sysykeji.top

[Q80] 字符串截取
来源：http://yaz.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kxj.fehbvm.com

[Q81] 字符串替换
来源：http://psk.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hee.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://ezb.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mzr.zhixingplan.top

[Q83] 大小写转换
来源：http://evm.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ivq.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://skc.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://cqa.quarkkingdee.top

[Q85] 数值取整
来源：http://jdq.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fun.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://xle.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qcf.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://wxx.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://urj.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://qwa.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://anf.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lpd.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://jpu.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jst.zdbjq.cn

[Q90] 生成序号列
来源：http://gxk.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xui.sweek.top

================================================================================
来源：http://wvn.shanyushiyangkeji.top

R. Bash 专题
来源：http://sgx.cqqwz.cn

================================================================================
来源：http://jaz.zhixingplan.top

[R01] shebang 与严格模式
来源：http://hxf.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://dvr.snrcjt.cn

set -euo pipefail
来源：http://bip.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://ttd.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://epb.shangyingyoupin.top

[R03] 只读变量
来源：http://ebw.jinyuanbaomall.cn

readonly PI=3.14
来源：http://dtk.sufxvd.cn

[R04] 位置参数
来源：http://dxc.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qlt.bbcook.cn

[R05] 参数默认值
来源：http://moh.tian-w.cn

name="${1:-default}"
来源：http://klx.iojbl.cn

[R06] 判断命令是否存在
来源：http://fko.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://plc.cdnleiting.top

[R07] if 判断文件
来源：http://wws.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://obq.vqdsnc.cn

[R08] 数值比较
来源：http://xlx.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mbx.gzhubu.top

[R09] 字符串比较
来源：http://jof.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ton.zdbjq.cn

[R10] 正则匹配
来源：http://brw.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xmq.hfpthk.cn

[R11] case 多分支
来源：http://moh.sxryk.cn

case "$1" in
来源：http://ujc.hnqzz.top

start) echo "启动" ;;
来源：http://qwj.yuanzhike.top

stop)  echo "停止" ;;
来源：http://hsb.tian-w.cn

*)     echo "未知命令" ;;
来源：http://hej.andypj.xyz

esac
来源：http://mzh.haohaochexian.top

[R12] for 遍历文件
来源：http://xis.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://vob.xziqi.cn

[R13] for 计数循环
来源：http://hce.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://onx.hcnkem.com

[R14] C 风格 for
来源：http://pfk.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cjz.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://kqp.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wzq.chenlongwang.top

[R16] until 等待条件
来源：http://frl.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dqa.snrcjt.cn

[R17] 数组定义与取值
来源：http://okf.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dns.fzhhl.top

[R18] 遍历数组
来源：http://tpg.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dmw.fengsongda.top

[R19] 数组长度
来源：http://yto.ppjwa.cn

echo "${#arr[@]}"
来源：http://hwc.hywenlv.cn

[R20] 关联数组（字典）
来源：http://pux.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://utz.snrcjt.cn

[R21] 字符串长度
来源：http://ais.nwbrower.top

echo "${#s}"
来源：http://ppl.andypj.xyz

[R22] 截取子串
来源：http://stf.yj202588.top

echo "${s:0:5}"
来源：http://ott.guowangkeji.top

[R23] 字符串替换
来源：http://ivw.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nrx.yj20258888.top

[R24] 大小写转换
来源：http://ykd.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://drl.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://iev.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fvd.redwolf501.top

[R26] 命令替换
来源：http://mma.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://von.ivvv.top

[R27] 算术展开
来源：http://fcz.vqdsnc.cn


<!-- 参考信息 -->