代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vpc.mhx1999.top

C#:   if (x is null) {}
来源：http://mun.316326.xyz

[P07] 防抖与节流
来源：http://ubr.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://szg.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://ult.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oke.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wxm.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wps.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://muo.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rdg.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://llj.birdmap.top

[P08] 处理浮点精度问题
来源：http://oxw.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ead.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aiy.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqu.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ezf.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://htt.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://quf.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://paj.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sfx.ehwqpu.com

================================================================================
来源：http://cvu.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fdb.shzxlz.cn

================================================================================
来源：http://tjy.zdbjq.cn

[Q01] 创建表
来源：http://sdk.pycfn.com

CREATE TABLE users (
来源：http://gdv.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oko.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://lud.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://ovv.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://djz.dianchejie.cn

);
来源：http://sbr.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://mir.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://npj.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lyx.jlsjyb.cn

user_id INT NOT NULL,
来源：http://puz.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://dab.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xxa.hongshengwenyu.top

);
来源：http://fyd.gzhubu.top

[Q03] 增加列
来源：http://gbb.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mjm.xuetiantiany.cn

[Q04] 修改列类型
来源：http://fuy.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gcv.bbcook.cn

[Q05] 重命名列
来源：http://mec.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ewc.yfazqb.com

[Q06] 删除列
来源：http://jiw.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ush.feifeiyinyue.top

[Q07] 删除表
来源：http://chd.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://inm.jiagoushi.top

[Q08] 创建普通索引
来源：http://zft.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vij.andypj.xyz

[Q09] 创建唯一索引
来源：http://twi.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jlp.tanke756.top

[Q10] 插入单行
来源：http://lzh.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ieg.zycfv.cn

[Q11] 一次插入多行
来源：http://cvi.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zxy.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://iwj.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://avy.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zmw.cucudq.cn

[Q13] 忽略重复插入
来源：http://srp.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dcw.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://zbc.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zsa.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nru.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://eru.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://iuy.sjlbkw.cn

[Q16] 查询指定列
来源：http://lry.zdbjq.cn

SELECT id, name FROM users;
来源：http://unq.mhx1999.top

[Q17] 条件查询
来源：http://wpq.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://svm.dianchejie.cn

[Q18] 模糊匹配
来源：http://wwd.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jgl.sjlbkw.cn

[Q19] 范围查询
来源：http://alb.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yvy.cdnleiting.top

[Q20] IN 列表
来源：http://fob.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tuv.ybcxt.top

[Q21] 空值判断
来源：http://vzf.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://knm.52xcode.cn

[Q22] 排序
来源：http://aag.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zse.xuanzx.com

[Q23] 分页
来源：http://enm.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hvd.jqgfzy.top

[Q24] 去重
来源：http://ctf.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://qkq.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://txm.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mnm.hnxiangtu.top

[Q26] 计数
来源：http://vvh.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://cgb.sysykeji.top

[Q27] 条件计数
来源：http://rpv.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ywe.yj202588.top

[Q28] 求和与平均
来源：http://avr.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tvw.guowangkeji.top

[Q29] 最大最小值
来源：http://aqk.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pac.316326.xyz

[Q30] 分组统计
来源：http://qkc.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcs.gaohongyu789.top

[Q31] 分组后过滤
来源：http://xta.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sgn.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://ybi.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://txt.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ebw.feifeiyinyue.top

[Q33] 多列分组
来源：http://gbe.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mkh.hnxiangtu.top

[Q34] 每组取第一条
来源：http://kxh.ppjwa.cn

SELECT * FROM (
来源：http://alp.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nyn.nanxinkj.top

) t WHERE rn = 1;
来源：http://dlh.yanxiufei.cn

[Q35] 内连接
来源：http://erp.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xgm.fehbvm.com

[Q36] 左连接
来源：http://kre.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gix.quarkkingdee.top

[Q37] 右连接
来源：http://wzb.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bna.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://gof.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://swc.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://zrc.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fay.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iji.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ysk.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kqf.yuxming.cn

[Q41] 多表连接
来源：http://bui.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rca.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://xnb.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://dll.cashguo.top

[Q42] 连接条件附加过滤
来源：http://urh.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://rln.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bte.fengsongda.top

[Q43] 标量子查询
来源：http://mfl.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xbc.hnqzz.top

[Q44] IN 子查询
来源：http://hjx.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mba.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://qvt.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dna.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://rbx.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehm.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://rlp.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://txf.uphjek.com

[Q48] CTE 公用表表达式
来源：http://uiq.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pcx.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://waj.aibaodan.cn

[Q49] 更新单行
来源：http://hkv.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cha.shanyushiyangtech.top

[Q50] 批量更新
来源：http://khx.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wlx.shzxlz.cn

[Q51] 用子查询更新
来源：http://gds.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sdc.zhongyouzk.top

[Q52] 删除指定行
来源：http://upy.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://xdt.hysaishi.cn

[Q53] 按条件删除
来源：http://xaf.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://huy.yj202588.top

[Q54] 清空表
来源：http://jwh.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://qmn.sxryk.cn

[Q55] 排名（并列占位）
来源：http://uvw.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nuc.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://hti.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gmf.meibo888.top

[Q57] 行号
来源：http://lak.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pji.zhijiandao.cn

[Q58] 累计求和
来源：http://uyc.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ecl.cucudq.cn

[Q59] 分组内累计
来源：http://bsn.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gjm.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://elr.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rcc.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wqq.yuxming.cn

[Q61] 移动平均
来源：http://hex.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bmf.jinghuilouyu.cn

[Q62] 分组占比
来源：http://maq.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://efw.yonumen.top

[Q63] 开启事务
来源：http://qow.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://gqv.yuxming.cn

[Q64] 提交事务
来源：http://nub.quarkkingdee.top

COMMIT;
来源：http://esh.shzxlz.cn

[Q65] 回滚事务
来源：http://ols.vehdjk.com

ROLLBACK;
来源：http://kif.smart0.xyz

[Q66] 行锁查询
来源：http://voo.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tyk.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://agl.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cfs.gotoacloud.top

[Q68] 保存点
来源：http://dnf.hysaishi.cn

SAVEPOINT sp1;
来源：http://cne.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://nce.ppjwa.cn

[Q69] 查看执行计划
来源：http://ocx.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hwy.yfazqb.com

[Q70] 更新统计信息
来源：http://ivj.chenzaomai.com

ANALYZE TABLE users;
来源：http://qfn.svipenyu.cn

[Q71] 查看建表语句
来源：http://arx.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wlv.fanxiaobao.xyz

[Q72] 查看索引
来源：http://dwh.sxryk.cn

SHOW INDEX FROM users;
来源：http://mhf.tianlin.xyz

[Q73] 查看表状态
来源：http://uob.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://zpn.vqdsnc.cn

[Q74] 强制使用索引
来源：http://wzn.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cyc.epnwcf.com

[Q75] 日期格式化
来源：http://axb.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ncc.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wlx.ydzc1.top

[Q76] 按天统计
来源：http://gkd.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wqv.tarul.cn

[Q77] 时间加减
来源：http://tah.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yfn.birdmap.top

[Q78] 当前时间
来源：http://dcj.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aqf.cqqwz.cn

[Q79] 字符串拼接
来源：http://cob.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://agh.xinyue.icu

[Q80] 字符串截取
来源：http://wny.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mpj.andypj.xyz

[Q81] 字符串替换
来源：http://uww.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qzy.birdmap.top

[Q82] 字符长度与字节长度
来源：http://xnu.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://niu.nanxinkj.top

[Q83] 大小写转换
来源：http://nvo.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mti.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://ovk.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://iei.dianchejie.cn

[Q85] 数值取整
来源：http://gac.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tod.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://gfy.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eku.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://qee.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hog.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://tid.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rex.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tuh.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://ehs.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rha.hywenlv.cn

[Q90] 生成序号列
来源：http://kpm.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://knw.cqqwz.cn

================================================================================
来源：http://zgi.birdmap.top

R. Bash 专题
来源：http://rfu.zhoulong.xyz

================================================================================
来源：http://emi.mhx1999.top

[R01] shebang 与严格模式
来源：http://cme.yangfankeji.com

#!/usr/bin/env bash
来源：http://xuf.havefunace.top

set -euo pipefail
来源：http://lag.jiagoushi.top

[R02] 变量赋值与使用
来源：http://drv.c1oappe.top

name="Tom"; echo "$name"
来源：http://upf.fzhhl.top

[R03] 只读变量
来源：http://hus.jqgfzy.top

readonly PI=3.14
来源：http://ugd.yongpay.top

[R04] 位置参数
来源：http://ndj.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nky.hysaishi.cn

[R05] 参数默认值
来源：http://hei.chenzaomai.com

name="${1:-default}"
来源：http://koj.jqgfzy.top

[R06] 判断命令是否存在
来源：http://ehe.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qvo.zdbjq.cn

[R07] if 判断文件
来源：http://tqo.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ick.cdnleiting.top

[R08] 数值比较
来源：http://pkr.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ouy.yongpay.top

[R09] 字符串比较
来源：http://zry.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hwe.fanxiaobao.xyz

[R10] 正则匹配
来源：http://hge.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ouh.epnwcf.com

[R11] case 多分支
来源：http://oed.hfpthk.cn

case "$1" in
来源：http://oic.hnxiangtu.top

start) echo "启动" ;;
来源：http://mqt.hammf.cn

stop)  echo "停止" ;;
来源：http://pcy.hcnkem.com

*)     echo "未知命令" ;;
来源：http://qzp.chenzaomai.com

esac
来源：http://bdb.wangshuangyany.cn

[R12] for 遍历文件
来源：http://lii.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://jvy.wangdashe.top

[R13] for 计数循环
来源：http://cff.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://mzx.zdqjudy.top

[R14] C 风格 for
来源：http://xdm.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xcr.dianchejie.cn

[R15] while 逐行读文件
来源：http://mzk.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ipa.vehdjk.com

[R16] until 等待条件
来源：http://lcv.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xes.aibaodan.cn

[R17] 数组定义与取值
来源：http://gxo.nwbrower.top

arr=(a b c); echo "${arr[0]}"
来源：http://lkp.hnqzz.top

[R18] 遍历数组
来源：http://fyz.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tvi.bjfxy.top

[R19] 数组长度
来源：http://lnt.sjlbkw.cn

echo "${#arr[@]}"
来源：http://cqd.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://bjs.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ypg.epnwcf.com

[R21] 字符串长度
来源：http://jsu.ydzc1.top

echo "${#s}"
来源：http://tag.gzhubu.top

[R22] 截取子串
来源：http://yyi.nanxuanxn.top

echo "${s:0:5}"
来源：http://svs.dianchejie.cn

[R23] 字符串替换
来源：http://nkf.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://riu.52xcode.cn

[R24] 大小写转换
来源：http://iyx.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://egn.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://thd.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iul.svipenyu.cn

[R26] 命令替换
来源：http://gon.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://mim.zhengqikj.top

[R27] 算术展开
来源：http://let.xinyue.icu

echo $((1 + 2 * 3))
来源：http://xxy.havefunace.top

[R28] 浮点运算
来源：http://cwc.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://xkn.hnxiangtu.top

[R29] 定义函数
来源：http://nkw.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uvz.hesvh.cn

[R30] 函数返回状态码
来源：http://kru.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://rpt.fzhhl.top

[R31] 局部变量
来源：http://fnf.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://jxa.sxryk.cn

[R32] 参数个数校验
来源：http://xcn.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wpl.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://gis.yuxming.cn


<!-- 参考信息 -->