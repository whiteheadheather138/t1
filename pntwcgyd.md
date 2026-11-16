代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jaj.cashguo.top

C#:   if (x is null) {}
来源：http://tvj.chenlongwang.top

[P07] 防抖与节流
来源：http://zev.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wwf.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://byb.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrd.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgn.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gds.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wsa.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ibj.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wjw.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://dsd.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vgz.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dym.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bav.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qpv.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zpm.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://whz.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aqi.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdw.jinqigufen.top

================================================================================
来源：http://kde.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xfl.bjfxy.top

================================================================================
来源：http://jbr.redwolf501.top

[Q01] 创建表
来源：http://lyt.yuxming.cn

CREATE TABLE users (
来源：http://ahv.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://frk.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://tai.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://cul.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ycr.zhijiandao.cn

);
来源：http://oeg.nanxinkj.top

[Q02] 创建带外键的表
来源：http://nad.hcnkem.com

CREATE TABLE orders (
来源：http://rur.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfo.jiagoushi.top

user_id INT NOT NULL,
来源：http://fhy.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://ihv.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qbg.jqgufenzy.top

);
来源：http://vbm.fengsongda.top

[Q03] 增加列
来源：http://mrw.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dif.hesvh.cn

[Q04] 修改列类型
来源：http://vgt.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://smt.dashuyun.cn

[Q05] 重命名列
来源：http://ipy.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://owj.zhoulong.xyz

[Q06] 删除列
来源：http://bes.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://qil.yfazqb.com

[Q07] 删除表
来源：http://yqb.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://cpf.xuanzx.com

[Q08] 创建普通索引
来源：http://jgr.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cqt.yj20258.top

[Q09] 创建唯一索引
来源：http://whd.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://soe.zhoulong.xyz

[Q10] 插入单行
来源：http://lxv.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xon.quarkkingdee.top

[Q11] 一次插入多行
来源：http://lzk.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wln.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://too.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://yqp.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://drt.aibaodan.cn

[Q13] 忽略重复插入
来源：http://kqm.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fwd.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://reo.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zsj.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bdd.guowangkeji.top

[Q15] 查询全部
来源：http://hci.havefunace.top

SELECT * FROM users;
来源：http://mwi.iojbl.cn

[Q16] 查询指定列
来源：http://bhj.hnqzz.top

SELECT id, name FROM users;
来源：http://gmf.bbcook.cn

[Q17] 条件查询
来源：http://hom.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vdx.tarul.cn

[Q18] 模糊匹配
来源：http://fij.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vib.sufxvd.cn

[Q19] 范围查询
来源：http://lky.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fdh.wangshuangyany.cn

[Q20] IN 列表
来源：http://wls.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://omu.9152youxi.cn

[Q21] 空值判断
来源：http://owq.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://yzr.cdnleiting.top

[Q22] 排序
来源：http://mvw.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://snh.bbcook.cn

[Q23] 分页
来源：http://yxs.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://knb.hnxiangtu.top

[Q24] 去重
来源：http://ocn.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://tqa.guannengcc.top

[Q25] 只取前 N 条
来源：http://anq.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ogn.shanyushiyangkeji.top

[Q26] 计数
来源：http://ogk.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://ihb.hongshengwenyu.top

[Q27] 条件计数
来源：http://crs.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ztg.chenlongwang.top

[Q28] 求和与平均
来源：http://rpg.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wqm.yj20258888.top

[Q29] 最大最小值
来源：http://qzi.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bqw.pycfn.com

[Q30] 分组统计
来源：http://zbx.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xza.svipenyu.cn

[Q31] 分组后过滤
来源：http://ylx.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tfk.birdmap.top

[Q32] 分组拼接字符串
来源：http://ypz.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://avn.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uhe.cdnleiting.top

[Q33] 多列分组
来源：http://fdu.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dwl.dianchejie.cn

[Q34] 每组取第一条
来源：http://fti.kuanghao11.cn

SELECT * FROM (
来源：http://xpb.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wyt.birdmap.top

) t WHERE rn = 1;
来源：http://owb.xuanzx.com

[Q35] 内连接
来源：http://pzn.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqx.yuanzhike.top

[Q36] 左连接
来源：http://zap.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zeu.zhengqikj.top

[Q37] 右连接
来源：http://qyq.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://toq.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uyy.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jzx.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://fwd.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://imi.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://koq.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wbm.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jss.hfpthk.cn

[Q41] 多表连接
来源：http://ssd.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ecu.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://pmb.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://lok.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://apk.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://ini.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://whm.snrcjt.cn

[Q43] 标量子查询
来源：http://xbp.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sdz.jinqigfzy.top

[Q44] IN 子查询
来源：http://soe.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rgx.316326.xyz

[Q45] EXISTS 判断存在
来源：http://mmy.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://amo.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://uvp.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcg.nanxuanxn.top

[Q47] 与平均值比较
来源：http://nxc.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uyb.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://jvq.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ffy.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://hkh.hfpthk.cn

[Q49] 更新单行
来源：http://lin.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jav.dianchejie.cn

[Q50] 批量更新
来源：http://ngo.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cam.sjlbkw.cn

[Q51] 用子查询更新
来源：http://ixj.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jpr.cashguo.top

[Q52] 删除指定行
来源：http://iae.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://mug.bbcook.cn

[Q53] 按条件删除
来源：http://fgv.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kky.guannengcc.top

[Q54] 清空表
来源：http://ypz.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://hvr.sweek.top

[Q55] 排名（并列占位）
来源：http://psn.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://shx.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://olh.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ggv.xziqi.cn

[Q57] 行号
来源：http://tyb.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dsz.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://ipg.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ido.yvedp.cn

[Q59] 分组内累计
来源：http://nig.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dun.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://mkt.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gbu.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zbg.hnqzz.top

[Q61] 移动平均
来源：http://qfr.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jvm.yfazqb.com

[Q62] 分组占比
来源：http://inv.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfj.hesvh.cn

[Q63] 开启事务
来源：http://ont.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bzv.hywenlv.cn

[Q64] 提交事务
来源：http://fpj.sjlbkw.cn

COMMIT;
来源：http://pky.zhijiandao.cn

[Q65] 回滚事务
来源：http://zkm.tarul.cn

ROLLBACK;
来源：http://yso.ybcxt.top

[Q66] 行锁查询
来源：http://fez.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jjz.ctjpmb.com

[Q67] 设置隔离级别
来源：http://zmv.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://reo.wangshuangyany.cn

[Q68] 保存点
来源：http://vxw.dashuyun.cn

SAVEPOINT sp1;
来源：http://qwc.yuxming.cn

ROLLBACK TO sp1;
来源：http://rzv.hfpthk.cn

[Q69] 查看执行计划
来源：http://vzo.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yry.tianlin.xyz

[Q70] 更新统计信息
来源：http://dvy.316326.xyz

ANALYZE TABLE users;
来源：http://mli.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://szl.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xpz.yanxiufei.cn

[Q72] 查看索引
来源：http://cvl.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://huh.yonumen.top

[Q73] 查看表状态
来源：http://qen.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://asd.fehbvm.com

[Q74] 强制使用索引
来源：http://sxv.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mao.ydzc1.top

[Q75] 日期格式化
来源：http://asw.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oae.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eos.0kj1m.cn

[Q76] 按天统计
来源：http://tjl.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lck.zhiwuduotai.top

[Q77] 时间加减
来源：http://bqe.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pft.vqdsnc.cn

[Q78] 当前时间
来源：http://zur.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cyz.316326.xyz

[Q79] 字符串拼接
来源：http://kjq.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xel.nanxinkj.top

[Q80] 字符串截取
来源：http://rkx.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ybn.zhoulong.xyz

[Q81] 字符串替换
来源：http://zxh.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ymn.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://qtl.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://taz.aizwys.cn

[Q83] 大小写转换
来源：http://ifq.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://okn.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://kia.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://pxq.aizwys.cn

[Q85] 数值取整
来源：http://rzb.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rzj.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://uhv.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tmq.mhx1999.top

[Q87] JSON 字段做条件
来源：http://ysf.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ett.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://gzy.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eqe.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ivm.ppjwa.cn

[Q89] 判断表是否存在
来源：http://pvy.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vvl.chenjidiqi.icu

[Q90] 生成序号列
来源：http://aiy.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kzb.daria6918.cn

================================================================================
来源：http://dnr.zhoulong.xyz

R. Bash 专题
来源：http://jzg.jqgfzy.top

================================================================================
来源：http://inb.andypj.xyz

[R01] shebang 与严格模式
来源：http://xpe.daria6918.cn

#!/usr/bin/env bash
来源：http://moo.fengsongda.top

set -euo pipefail
来源：http://imk.shuidangran.top

[R02] 变量赋值与使用
来源：http://aca.ppjwa.cn

name="Tom"; echo "$name"
来源：http://cbq.ppjwa.cn

[R03] 只读变量
来源：http://bvy.ybcxt.top

readonly PI=3.14
来源：http://cma.yuanzhike.top

[R04] 位置参数
来源：http://mxl.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cmk.yuanzhike.top

[R05] 参数默认值
来源：http://ydj.ehwqpu.com

name="${1:-default}"
来源：http://csq.xylfe.cn

[R06] 判断命令是否存在
来源：http://cvd.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hko.yj20258.top

[R07] if 判断文件
来源：http://lbn.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yoa.xylfe.cn

[R08] 数值比较
来源：http://zwi.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://noz.tanke756.top

[R09] 字符串比较
来源：http://bni.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pux.jianghu66.top

[R10] 正则匹配
来源：http://aqm.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nnk.fzhhl.top

[R11] case 多分支
来源：http://vyi.havefunace.top

case "$1" in
来源：http://fji.chenlongwang.top

start) echo "启动" ;;
来源：http://nvw.birdmap.top

stop)  echo "停止" ;;
来源：http://jnn.yfazqb.com

*)     echo "未知命令" ;;
来源：http://qbs.sweek.top

esac
来源：http://awk.yj20258888.top

[R12] for 遍历文件
来源：http://cjf.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://nee.fehbvm.com

[R13] for 计数循环
来源：http://mvy.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://jnw.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://lcc.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xir.zhengqikj.top

[R15] while 逐行读文件
来源：http://cra.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rap.sweek.top

[R16] until 等待条件
来源：http://eyb.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xbj.gotoacloud.top

[R17] 数组定义与取值
来源：http://mst.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://teu.zdbjq.cn

[R18] 遍历数组
来源：http://dge.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uyq.316326.xyz

[R19] 数组长度
来源：http://yga.0kj1m.cn

echo "${#arr[@]}"
来源：http://oqu.tianlin.xyz

[R20] 关联数组（字典）
来源：http://utb.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jqu.xziqi.cn

[R21] 字符串长度
来源：http://lcf.iojbl.cn

echo "${#s}"
来源：http://ymy.aizwys.cn

[R22] 截取子串
来源：http://mfa.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://unm.cucudq.cn

[R23] 字符串替换
来源：http://sfn.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wev.hesvh.cn

[R24] 大小写转换
来源：http://tkq.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ksi.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://fku.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wnz.zhoulong.xyz

[R26] 命令替换
来源：http://sor.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://ofa.ywan-chungtsiang.top

[R27] 算术展开
来源：http://kah.yuxming.cn

echo $((1 + 2 * 3))
来源：http://dsb.wangshuangyany.cn

[R28] 浮点运算
来源：http://pjs.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://ejk.ydzc1.top

[R29] 定义函数
来源：http://yme.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ewc.hammf.cn

[R30] 函数返回状态码
来源：http://uur.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://msv.ydjk.org.cn

[R31] 局部变量
来源：http://psg.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://fsn.sufxvd.cn

[R32] 参数个数校验
来源：http://kta.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fyx.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://nhl.chenlongwang.top


<!-- 参考信息 -->