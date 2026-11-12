代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lvr.yvedp.cn

TS:   if (x == null) {}
来源：http://slv.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rmg.xuanzx.com

Go:   if x == nil {}
来源：http://axb.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://muv.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://rhs.guowangkeji.top

[P07] 防抖与节流
来源：http://hsu.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bqu.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://vln.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lex.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ass.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gbm.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://frt.cheryme.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vye.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dzv.pycfn.com

[P08] 处理浮点精度问题
来源：http://jww.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://drr.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iep.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yfy.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uzi.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ztw.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nif.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xcb.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sml.yfazqb.com

================================================================================
来源：http://inm.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pzi.fanxiaobao.xyz

================================================================================
来源：http://txp.jinqigfzy.top

[Q01] 创建表
来源：http://ora.0kj1m.cn

CREATE TABLE users (
来源：http://kam.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ckf.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://xat.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://mja.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jny.zhengqikj.top

);
来源：http://ugm.yj20258888.top

[Q02] 创建带外键的表
来源：http://fix.shzxlz.cn

CREATE TABLE orders (
来源：http://byh.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qmw.aizwys.cn

user_id INT NOT NULL,
来源：http://sbw.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://uge.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hzx.bbcook.cn

);
来源：http://zrx.yongpay.top

[Q03] 增加列
来源：http://tnu.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ygy.hywenlv.cn

[Q04] 修改列类型
来源：http://vcw.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ske.uphjek.com

[Q05] 重命名列
来源：http://rop.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ijw.cdnleiting.top

[Q06] 删除列
来源：http://puw.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://pxg.vqdsnc.cn

[Q07] 删除表
来源：http://dkc.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://xej.uphjek.com

[Q08] 创建普通索引
来源：http://dlx.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dnx.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://hqz.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mhe.xinyue.icu

[Q10] 插入单行
来源：http://ciq.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://onf.dianchejie.cn

[Q11] 一次插入多行
来源：http://hby.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xrc.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://snr.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://lma.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vku.vehdjk.com

[Q13] 忽略重复插入
来源：http://eiv.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iwq.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://okn.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jsq.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kno.jyoumei.cn

[Q15] 查询全部
来源：http://clk.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://jjv.fzhhl.top

[Q16] 查询指定列
来源：http://qhs.aibaodan.cn

SELECT id, name FROM users;
来源：http://dwx.snrcjt.cn

[Q17] 条件查询
来源：http://wmt.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jlz.yuanzhike.top

[Q18] 模糊匹配
来源：http://pcx.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ieo.cqqwz.cn

[Q19] 范围查询
来源：http://ecd.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ebi.aibaodan.cn

[Q20] IN 列表
来源：http://lnz.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qqr.shuidangran.top

[Q21] 空值判断
来源：http://hvk.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://znq.sjlbkw.cn

[Q22] 排序
来源：http://cuo.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kpy.jinyuanbaomall.cn

[Q23] 分页
来源：http://lct.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qay.yuanzhike.top

[Q24] 去重
来源：http://yxk.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://qvb.snrcjt.cn

[Q25] 只取前 N 条
来源：http://wsz.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cyb.wangdashe.top

[Q26] 计数
来源：http://uno.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://shx.shangyingyoupin.top

[Q27] 条件计数
来源：http://pei.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lnx.svipenyu.cn

[Q28] 求和与平均
来源：http://crr.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://frw.yuanzhike.top

[Q29] 最大最小值
来源：http://aue.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ise.cashguo.top

[Q30] 分组统计
来源：http://kfm.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mja.9152youxi.cn

[Q31] 分组后过滤
来源：http://why.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pxs.gzhubu.top

[Q32] 分组拼接字符串
来源：http://ncb.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hmg.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mrh.zhoulong.xyz

[Q33] 多列分组
来源：http://mcz.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wol.yj20258.top

[Q34] 每组取第一条
来源：http://bze.ehwqpu.com

SELECT * FROM (
来源：http://kdt.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cxd.chenlongwang.top

) t WHERE rn = 1;
来源：http://esi.tanke756.top

[Q35] 内连接
来源：http://qnk.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xmr.yj20258.top

[Q36] 左连接
来源：http://epr.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qwd.mhx1999.top

[Q37] 右连接
来源：http://dlh.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zwr.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ich.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfe.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://yor.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hde.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lng.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://plb.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ttf.epnwcf.com

[Q41] 多表连接
来源：http://ovp.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cam.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://yer.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://yhy.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://azw.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://kjh.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ulz.cheryme.top

[Q43] 标量子查询
来源：http://iow.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://deb.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://vdg.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uyp.ivvv.top

[Q45] EXISTS 判断存在
来源：http://uqe.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vio.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://yel.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwr.smart0.xyz

[Q47] 与平均值比较
来源：http://tpu.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xfu.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://kri.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uql.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://yyw.fengsongda.top

[Q49] 更新单行
来源：http://vjf.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kxz.52xcode.cn

[Q50] 批量更新
来源：http://mcw.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gfl.ctjpmb.com

[Q51] 用子查询更新
来源：http://xtf.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jsm.ehwqpu.com

[Q52] 删除指定行
来源：http://olj.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://umf.yj202588.top

[Q53] 按条件删除
来源：http://udi.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kik.epnwcf.com

[Q54] 清空表
来源：http://nbc.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://hki.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://qof.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://que.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://ioj.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vnj.uphjek.com

[Q57] 行号
来源：http://idt.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nmr.jyoumei.cn

[Q58] 累计求和
来源：http://yqc.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lmw.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://rto.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cjc.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://frt.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://drz.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpp.zhoulong.xyz

[Q61] 移动平均
来源：http://wsf.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wjj.zdbjq.cn

[Q62] 分组占比
来源：http://inr.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jdm.gogol.net.cn

[Q63] 开启事务
来源：http://scq.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pxa.jqgfzy.top

[Q64] 提交事务
来源：http://vez.vehdjk.com

COMMIT;
来源：http://utk.fzhhl.top

[Q65] 回滚事务
来源：http://zue.feifeiyinyue.top

ROLLBACK;
来源：http://deh.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://eqe.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vmo.yueranfly.top

[Q67] 设置隔离级别
来源：http://kno.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgc.cqqwz.cn

[Q68] 保存点
来源：http://rpy.yuanzhike.top

SAVEPOINT sp1;
来源：http://rub.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://zyb.snrcjt.cn

[Q69] 查看执行计划
来源：http://bow.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vpt.jlsjyb.cn

[Q70] 更新统计信息
来源：http://qby.bbcook.cn

ANALYZE TABLE users;
来源：http://lzn.jyoumei.cn

[Q71] 查看建表语句
来源：http://iha.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://osw.fehbvm.com

[Q72] 查看索引
来源：http://tuh.ivvv.top

SHOW INDEX FROM users;
来源：http://pvv.tarul.cn

[Q73] 查看表状态
来源：http://bdd.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ibe.jianghu66.top

[Q74] 强制使用索引
来源：http://lgq.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://erd.wangdashe.top

[Q75] 日期格式化
来源：http://gtm.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://prq.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vue.tanke756.top

[Q76] 按天统计
来源：http://edi.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mmo.fzhhl.top

[Q77] 时间加减
来源：http://upe.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://epe.fehbvm.com

[Q78] 当前时间
来源：http://jrc.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rvu.redwolf501.top

[Q79] 字符串拼接
来源：http://vlp.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://few.daria6918.cn

[Q80] 字符串截取
来源：http://gsu.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://buk.mhx1999.top

[Q81] 字符串替换
来源：http://ley.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wvp.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://ewh.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kyl.vqdsnc.cn

[Q83] 大小写转换
来源：http://dig.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uhw.sxryk.cn

[Q84] 去除首尾空格
来源：http://qnk.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://jdi.cqqwz.cn

[Q85] 数值取整
来源：http://dnt.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nuw.316326.xyz

[Q86] 读取 JSON 字段
来源：http://uhq.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tws.xuanzx.com

[Q87] JSON 字段做条件
来源：http://qgk.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jep.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://aza.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bfb.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wfw.guannengcc.top

[Q89] 判断表是否存在
来源：http://pen.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://udb.gotoacloud.top

[Q90] 生成序号列
来源：http://oen.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uvh.cashguo.top

================================================================================
来源：http://vlo.yonumen.top

R. Bash 专题
来源：http://aku.birdmap.top

================================================================================
来源：http://tbp.gogol.net.cn

[R01] shebang 与严格模式
来源：http://bdq.gaohongyu789.top

#!/usr/bin/env bash
来源：http://aug.fengsongda.top

set -euo pipefail
来源：http://kfw.fengsongda.top

[R02] 变量赋值与使用
来源：http://jzw.aibaodan.cn

name="Tom"; echo "$name"
来源：http://kbh.kuanghao11.cn

[R03] 只读变量
来源：http://jll.birdmap.top

readonly PI=3.14
来源：http://rkl.andypj.xyz

[R04] 位置参数
来源：http://fob.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qjx.xuanzx.com

[R05] 参数默认值
来源：http://vjy.fktsv.cn

name="${1:-default}"
来源：http://icq.svipenyu.cn

[R06] 判断命令是否存在
来源：http://qxs.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fzq.svipenyu.cn

[R07] if 判断文件
来源：http://mmv.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lcw.chenjidiqi.icu

[R08] 数值比较
来源：http://wqf.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mps.chenzaomai.com

[R09] 字符串比较
来源：http://cnq.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xos.gaohongyu789.top

[R10] 正则匹配
来源：http://abk.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://axi.jiagoushi.top

[R11] case 多分支
来源：http://plg.sweek.top

case "$1" in
来源：http://koy.xinyue.icu

start) echo "启动" ;;
来源：http://ctd.uphjek.com

stop)  echo "停止" ;;
来源：http://lfx.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://cyz.xylfe.cn

esac
来源：http://zmd.zhongyouzk.top

[R12] for 遍历文件
来源：http://iba.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://xdv.ppjwa.cn

[R13] for 计数循环
来源：http://oxc.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://fez.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://fgp.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dzm.zhongyouzk.top

[R15] while 逐行读文件
来源：http://fas.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://njt.zdbjq.cn

[R16] until 等待条件
来源：http://voe.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://riw.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://gsj.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nmi.gogol.net.cn

[R18] 遍历数组
来源：http://beu.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nyw.sufxvd.cn

[R19] 数组长度
来源：http://tgp.cashguo.top

echo "${#arr[@]}"
来源：http://cdv.xziqi.cn

[R20] 关联数组（字典）
来源：http://toi.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vji.gotoacloud.top

[R21] 字符串长度
来源：http://cab.mhx1999.top

echo "${#s}"
来源：http://wre.52xcode.cn

[R22] 截取子串
来源：http://fyu.sxryk.cn

echo "${s:0:5}"
来源：http://jcs.hnqzz.top

[R23] 字符串替换
来源：http://vyw.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://msi.gaohongyu789.top

[R24] 大小写转换
来源：http://alc.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kpm.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://stz.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fgs.guannengcc.top

[R26] 命令替换
来源：http://kuf.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://lwp.chenlongwang.top

[R27] 算术展开
来源：http://gkd.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://jkf.snrcjt.cn

[R28] 浮点运算
来源：http://xgs.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://vbc.zhixingplan.top

[R29] 定义函数
来源：http://bqk.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oll.9152youxi.cn

[R30] 函数返回状态码
来源：http://uvo.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://fls.hnxiangtu.top

[R31] 局部变量
来源：http://bur.zdqjudy.top


<!-- 参考信息 -->