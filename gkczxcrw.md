代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kgq.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqp.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://vse.jinqigfzy.top

Ruby: a == b
来源：http://xst.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://grb.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lnk.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hfc.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://mbr.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mqd.yj20258.top

TS:   if (x == null) {}
来源：http://twn.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ccx.aibaodan.cn

Go:   if x == nil {}
来源：http://pvn.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qki.hammf.cn

C#:   if (x is null) {}
来源：http://ayv.shzxlz.cn

[P07] 防抖与节流
来源：http://bjr.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dlj.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://zso.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwa.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qya.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aty.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jrs.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yhs.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://win.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://xsj.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://etc.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lhg.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wvh.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nzo.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vfo.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sjx.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fea.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gei.mhx1999.top

================================================================================
来源：http://toz.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ead.fehbvm.com

================================================================================
来源：http://utf.mhx1999.top

[Q01] 创建表
来源：http://lhj.aibaodan.cn

CREATE TABLE users (
来源：http://vcn.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qii.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://hgl.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://hbl.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qtq.yuanzhike.top

);
来源：http://fpk.ctjpmb.com

[Q02] 创建带外键的表
来源：http://yzk.tianlin.xyz

CREATE TABLE orders (
来源：http://mey.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uoc.hnxiangtu.top

user_id INT NOT NULL,
来源：http://nqf.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://stn.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wzs.sysykeji.top

);
来源：http://cpa.jqgufenzy.top

[Q03] 增加列
来源：http://jmw.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://twz.ppjwa.cn

[Q04] 修改列类型
来源：http://ukx.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qjv.yonumen.top

[Q05] 重命名列
来源：http://elu.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pal.nanxuanxn.top

[Q06] 删除列
来源：http://drl.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://kck.ydzc1.top

[Q07] 删除表
来源：http://fjx.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://cui.zhijiandao.cn

[Q08] 创建普通索引
来源：http://mzs.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://lqj.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://eii.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tbv.xuetiantiany.cn

[Q10] 插入单行
来源：http://lps.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ifz.hesvh.cn

[Q11] 一次插入多行
来源：http://pkp.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rka.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://tmb.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tvh.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nzx.yonumen.top

[Q13] 忽略重复插入
来源：http://kyy.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cxy.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://oek.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fnh.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://msr.quarkkingdee.top

[Q15] 查询全部
来源：http://qjr.smart0.xyz

SELECT * FROM users;
来源：http://whc.zhoulong.xyz

[Q16] 查询指定列
来源：http://qnk.ehwqpu.com

SELECT id, name FROM users;
来源：http://tgq.xuanzx.com

[Q17] 条件查询
来源：http://gun.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qyo.yj202588.top

[Q18] 模糊匹配
来源：http://lrh.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gem.quarkkingdee.top

[Q19] 范围查询
来源：http://xyw.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wox.jinqigfzy.top

[Q20] IN 列表
来源：http://bmc.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ood.gzhubu.top

[Q21] 空值判断
来源：http://zsk.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yso.fktsv.cn

[Q22] 排序
来源：http://blb.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kti.havefunace.top

[Q23] 分页
来源：http://eat.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dsu.aizwys.cn

[Q24] 去重
来源：http://yrt.316326.xyz

SELECT DISTINCT city FROM users;
来源：http://lcw.havefunace.top

[Q25] 只取前 N 条
来源：http://ekk.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fda.shanyushiyangtech.top

[Q26] 计数
来源：http://lzy.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://emx.cucudq.cn

[Q27] 条件计数
来源：http://hai.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nyf.yuxming.cn

[Q28] 求和与平均
来源：http://vbt.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uzh.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://ctg.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xie.sjlbkw.cn

[Q30] 分组统计
来源：http://uts.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hnr.ppjwa.cn

[Q31] 分组后过滤
来源：http://ggv.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tln.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://ivp.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://siw.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bpn.ppjwa.cn

[Q33] 多列分组
来源：http://yje.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cae.xuanzx.com

[Q34] 每组取第一条
来源：http://ymr.wangshuangyany.cn

SELECT * FROM (
来源：http://rqf.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ook.tian-w.cn

) t WHERE rn = 1;
来源：http://lzo.fanxiaobao.xyz

[Q35] 内连接
来源：http://viw.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ihh.uphjek.com

[Q36] 左连接
来源：http://scd.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vrp.wangshuangyany.cn

[Q37] 右连接
来源：http://ogr.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qfn.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://etg.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jws.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://fbw.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rto.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kup.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zjw.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pws.xuanzx.com

[Q41] 多表连接
来源：http://zkj.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dga.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://hlk.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://brk.cashguo.top

[Q42] 连接条件附加过滤
来源：http://mqc.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://abs.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kbn.jqgufenzy.top

[Q43] 标量子查询
来源：http://jgh.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kbo.bbcook.cn

[Q44] IN 子查询
来源：http://sea.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tka.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://uvx.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpo.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://jpl.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://chs.sxryk.cn

[Q47] 与平均值比较
来源：http://lid.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lol.hammf.cn

[Q48] CTE 公用表表达式
来源：http://rqb.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://trp.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://qhr.9152youxi.cn

[Q49] 更新单行
来源：http://yyo.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qnw.jinghuilouyu.cn

[Q50] 批量更新
来源：http://lyk.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xeu.xuanzx.com

[Q51] 用子查询更新
来源：http://zja.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://arp.tianlin.xyz

[Q52] 删除指定行
来源：http://rnb.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://qih.bjfxy.top

[Q53] 按条件删除
来源：http://tqt.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xfp.yj20258888.top

[Q54] 清空表
来源：http://ocu.bbcook.cn

TRUNCATE TABLE logs;
来源：http://hea.redwolf501.top

[Q55] 排名（并列占位）
来源：http://dun.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tmn.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://wve.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gff.hnxiangtu.top

[Q57] 行号
来源：http://pgt.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qye.andypj.xyz

[Q58] 累计求和
来源：http://xjn.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vjc.yuxming.cn

[Q59] 分组内累计
来源：http://rej.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ghc.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://rdl.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ixk.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nti.gotoacloud.top

[Q61] 移动平均
来源：http://ufp.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://keh.epnwcf.com

[Q62] 分组占比
来源：http://ayr.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ocy.meibo888.top

[Q63] 开启事务
来源：http://fmg.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gan.jinghuilouyu.cn

[Q64] 提交事务
来源：http://psg.ywan-chungtsiang.top

COMMIT;
来源：http://zvm.tarul.cn

[Q65] 回滚事务
来源：http://oyw.tarul.cn

ROLLBACK;
来源：http://kkf.hnqzz.top

[Q66] 行锁查询
来源：http://tup.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://osj.hammf.cn

[Q67] 设置隔离级别
来源：http://ioc.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yec.316326.xyz

[Q68] 保存点
来源：http://fno.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://vkb.xylfe.cn

ROLLBACK TO sp1;
来源：http://zpt.9152youxi.cn

[Q69] 查看执行计划
来源：http://pig.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kkv.cheryme.top

[Q70] 更新统计信息
来源：http://kyt.cashguo.top

ANALYZE TABLE users;
来源：http://ict.316326.xyz

[Q71] 查看建表语句
来源：http://mnm.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://loo.tarul.cn

[Q72] 查看索引
来源：http://awd.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://wqq.xziqi.cn

[Q73] 查看表状态
来源：http://lcx.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://anl.cdnleiting.top

[Q74] 强制使用索引
来源：http://apg.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mby.guowangkeji.top

[Q75] 日期格式化
来源：http://kng.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ejf.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ddq.zhoulong.xyz

[Q76] 按天统计
来源：http://hnh.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kue.birdmap.top

[Q77] 时间加减
来源：http://yfn.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxf.chenzaomai.com

[Q78] 当前时间
来源：http://pjm.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vnc.fktsv.cn

[Q79] 字符串拼接
来源：http://ugc.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tij.birdmap.top

[Q80] 字符串截取
来源：http://ibk.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ctz.jianghu66.top

[Q81] 字符串替换
来源：http://fox.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aon.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://tty.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tnc.hfpthk.cn

[Q83] 大小写转换
来源：http://wfa.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zlm.tian-w.cn

[Q84] 去除首尾空格
来源：http://zij.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://oxe.jinqigfzy.top

[Q85] 数值取整
来源：http://mxz.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jwp.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://hoa.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hgp.redwolf501.top

[Q87] JSON 字段做条件
来源：http://wym.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://soo.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://ena.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yxp.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tyc.yuxming.cn

[Q89] 判断表是否存在
来源：http://vsc.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tnh.hcnkem.com

[Q90] 生成序号列
来源：http://oaa.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ujf.hysaishi.cn

================================================================================
来源：http://ktf.cqqwz.cn

R. Bash 专题
来源：http://bvi.andypj.xyz

================================================================================
来源：http://imy.redwolf501.top

[R01] shebang 与严格模式
来源：http://sjg.yuanzhike.top

#!/usr/bin/env bash
来源：http://fov.pengpengdd.cyou

set -euo pipefail
来源：http://rqv.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://lcc.daxiang520.top

name="Tom"; echo "$name"
来源：http://yfh.fzhhl.top

[R03] 只读变量
来源：http://lwt.quarkkingdee.top

readonly PI=3.14
来源：http://bis.ydzc1.top

[R04] 位置参数
来源：http://iyw.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oki.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://bko.iojbl.cn

name="${1:-default}"
来源：http://eli.52xcode.cn

[R06] 判断命令是否存在
来源：http://xxp.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bom.mhx1999.top

[R07] if 判断文件
来源：http://qfd.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rag.gotoacloud.top

[R08] 数值比较
来源：http://cub.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://clo.gaohongyu789.top

[R09] 字符串比较
来源：http://uas.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hys.aizwys.cn

[R10] 正则匹配
来源：http://vbn.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mra.tanke756.top

[R11] case 多分支
来源：http://vrw.aibaodan.cn

case "$1" in
来源：http://kcp.sxryk.cn

start) echo "启动" ;;
来源：http://qtu.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://ndk.aizwys.cn

*)     echo "未知命令" ;;
来源：http://dsb.guannengcc.top

esac
来源：http://iww.haohaochexian.top

[R12] for 遍历文件
来源：http://adw.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://exi.sxryk.cn

[R13] for 计数循环
来源：http://rid.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://ljg.zhiwuduotai.top

[R14] C 风格 for
来源：http://uvy.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nqw.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://fcq.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jbb.zdbjq.cn

[R16] until 等待条件
来源：http://xij.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdo.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://vnh.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://agr.xinyue.icu

[R18] 遍历数组
来源：http://eut.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hqb.hfpthk.cn

[R19] 数组长度
来源：http://wtz.bbcook.cn

echo "${#arr[@]}"
来源：http://mgx.epnwcf.com

[R20] 关联数组（字典）
来源：http://hfv.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ssp.zhongyouzk.top

[R21] 字符串长度
来源：http://udu.316326.xyz

echo "${#s}"
来源：http://gxd.jinyuanbaomall.cn

[R22] 截取子串
来源：http://tbh.zhiwuduotai.top

echo "${s:0:5}"
来源：http://wxi.yonumen.top

[R23] 字符串替换
来源：http://ull.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dvx.fanxiaobao.xyz

[R24] 大小写转换
来源：http://vqe.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zco.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://uko.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nde.cheryme.top

[R26] 命令替换
来源：http://vyh.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://esr.meibo888.top

[R27] 算术展开
来源：http://ggn.zhixingplan.top


<!-- 参考信息 -->