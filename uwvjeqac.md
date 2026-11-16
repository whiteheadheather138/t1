代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zgt.52xcode.cn

C#:   if (x is null) {}
来源：http://lgg.feifeiyinyue.top

[P07] 防抖与节流
来源：http://xcp.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zrg.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://nxx.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lmo.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzf.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iwt.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pld.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eus.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xtc.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://kcg.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sfh.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://odi.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qtu.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://val.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zye.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ewh.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bre.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://col.ctjpmb.com

================================================================================
来源：http://snj.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ere.fehbvm.com

================================================================================
来源：http://xlh.zhengqikj.top

[Q01] 创建表
来源：http://fkk.iojbl.cn

CREATE TABLE users (
来源：http://lvj.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sfi.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://ria.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://vvl.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fba.xylfe.cn

);
来源：http://iyo.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://vnx.bbcook.cn

CREATE TABLE orders (
来源：http://nry.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wna.jinqigfzy.top

user_id INT NOT NULL,
来源：http://wws.yj20258.top

amount DECIMAL(10, 2),
来源：http://xch.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vru.birdmap.top

);
来源：http://kzz.ybcxt.top

[Q03] 增加列
来源：http://uaf.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gqq.iojbl.cn

[Q04] 修改列类型
来源：http://jpj.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yxq.mhx1999.top

[Q05] 重命名列
来源：http://hty.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mwc.yangfankeji.com

[Q06] 删除列
来源：http://tuy.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://orf.jinqigufen.top

[Q07] 删除表
来源：http://svy.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://sfv.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://bzh.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cat.yonumen.top

[Q09] 创建唯一索引
来源：http://iju.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://etm.shzxlz.cn

[Q10] 插入单行
来源：http://oio.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uur.yj202588.top

[Q11] 一次插入多行
来源：http://fss.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nxv.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://dps.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://lij.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qsq.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://plo.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wwt.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://tgf.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mxg.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://omv.pengpengdd.cyou

[Q15] 查询全部
来源：http://fdn.yongpay.top

SELECT * FROM users;
来源：http://qmo.sweek.top

[Q16] 查询指定列
来源：http://ikr.fengsongda.top

SELECT id, name FROM users;
来源：http://hpi.shanyushiyangtech.top

[Q17] 条件查询
来源：http://yra.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aux.xziqi.cn

[Q18] 模糊匹配
来源：http://rha.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cvs.sysykeji.top

[Q19] 范围查询
来源：http://xia.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kxp.meibo888.top

[Q20] IN 列表
来源：http://vyv.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zsq.uphjek.com

[Q21] 空值判断
来源：http://ykm.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lhk.xuetiantiany.cn

[Q22] 排序
来源：http://oea.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cid.feifeiyinyue.top

[Q23] 分页
来源：http://qdi.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ehk.cashguo.top

[Q24] 去重
来源：http://urj.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://utm.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://vsa.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://has.vqdsnc.cn

[Q26] 计数
来源：http://uvx.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://kam.epnwcf.com

[Q27] 条件计数
来源：http://lte.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pqs.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://wnk.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://usp.shuidangran.top

[Q29] 最大最小值
来源：http://bbo.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jve.sufxvd.cn

[Q30] 分组统计
来源：http://iza.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://der.xinyue.icu

[Q31] 分组后过滤
来源：http://psf.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dhn.redwolf501.top

[Q32] 分组拼接字符串
来源：http://pjp.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cfi.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xfv.yj20258.top

[Q33] 多列分组
来源：http://qhy.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zud.svipenyu.cn

[Q34] 每组取第一条
来源：http://rra.sufxvd.cn

SELECT * FROM (
来源：http://wcg.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://crf.zdqjudy.top

) t WHERE rn = 1;
来源：http://edj.yfazqb.com

[Q35] 内连接
来源：http://ily.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fce.guowangkeji.top

[Q36] 左连接
来源：http://mug.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uzj.xylfe.cn

[Q37] 右连接
来源：http://wjp.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mno.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://awh.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qxg.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://oom.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gfn.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://npx.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jni.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xva.cashguo.top

[Q41] 多表连接
来源：http://mgx.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aru.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://byp.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://bvg.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://ddl.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://qis.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fry.shzxlz.cn

[Q43] 标量子查询
来源：http://qbr.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://omd.nanxuanxn.top

[Q44] IN 子查询
来源：http://ann.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oqc.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://idb.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://joo.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fhy.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jia.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://sjm.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wyr.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://ejb.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gej.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://sra.wangdashe.top

[Q49] 更新单行
来源：http://yfv.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gwv.jqgfzy.top

[Q50] 批量更新
来源：http://imr.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jmv.yueranfly.top

[Q51] 用子查询更新
来源：http://vqd.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fwb.shangyingyoupin.top

[Q52] 删除指定行
来源：http://gbc.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://mqy.sxryk.cn

[Q53] 按条件删除
来源：http://klw.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gzc.fktsv.cn

[Q54] 清空表
来源：http://qqp.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://dvi.zycfv.cn

[Q55] 排名（并列占位）
来源：http://sag.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ull.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://qrj.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bil.guannengcc.top

[Q57] 行号
来源：http://egi.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gvi.dianchejie.cn

[Q58] 累计求和
来源：http://pix.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gym.fktsv.cn

[Q59] 分组内累计
来源：http://tmv.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cxb.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://hku.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cba.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fye.vqdsnc.cn

[Q61] 移动平均
来源：http://ett.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xrv.hnxiangtu.top

[Q62] 分组占比
来源：http://vod.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqh.ctjpmb.com

[Q63] 开启事务
来源：http://tpi.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://gby.yueranfly.top

[Q64] 提交事务
来源：http://fwd.gaohongyu789.top

COMMIT;
来源：http://kvr.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://bkl.shanyushiyangtech.top

ROLLBACK;
来源：http://utu.haohaochexian.top

[Q66] 行锁查询
来源：http://dix.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sev.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://ctv.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://urb.yj20258.top

[Q68] 保存点
来源：http://cbe.dianchejie.cn

SAVEPOINT sp1;
来源：http://ids.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://cxj.zycfv.cn

[Q69] 查看执行计划
来源：http://fgi.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pqn.ydjk.org.cn

[Q70] 更新统计信息
来源：http://nkf.yangfankeji.com

ANALYZE TABLE users;
来源：http://ppa.yvedp.cn

[Q71] 查看建表语句
来源：http://hwr.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jmp.shzxlz.cn

[Q72] 查看索引
来源：http://lej.meibo888.top

SHOW INDEX FROM users;
来源：http://qyc.jqgfzy.top

[Q73] 查看表状态
来源：http://rdo.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://kpq.ehwqpu.com

[Q74] 强制使用索引
来源：http://bmy.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kvl.gzhubu.top

[Q75] 日期格式化
来源：http://fqb.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://flb.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://syq.jyoumei.cn

[Q76] 按天统计
来源：http://kcj.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://voj.jqgfzy.top

[Q77] 时间加减
来源：http://ujq.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fmm.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://dgh.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nnz.tian-w.cn

[Q79] 字符串拼接
来源：http://gsd.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cxa.0kj1m.cn

[Q80] 字符串截取
来源：http://rql.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cgd.guannengcc.top

[Q81] 字符串替换
来源：http://umv.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fcv.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://lwq.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oxv.shangyingyoupin.top

[Q83] 大小写转换
来源：http://msr.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cug.bbcook.cn

[Q84] 去除首尾空格
来源：http://bxv.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://mxl.aibaodan.cn

[Q85] 数值取整
来源：http://jtw.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xmr.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://bdf.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xfd.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://dgd.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://knb.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://dvf.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ysd.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jkj.zdqjudy.top

[Q89] 判断表是否存在
来源：http://epp.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wzx.yfazqb.com

[Q90] 生成序号列
来源：http://qgk.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnf.iojbl.cn

================================================================================
来源：http://erf.zdbjq.cn

R. Bash 专题
来源：http://xna.shanyushiyangkeji.top

================================================================================
来源：http://pqp.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://oye.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://ydo.jiagoushi.top

set -euo pipefail
来源：http://pbc.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://vgf.aibaodan.cn

name="Tom"; echo "$name"
来源：http://gct.cucudq.cn

[R03] 只读变量
来源：http://erk.zhiwuduotai.top

readonly PI=3.14
来源：http://ndk.xylfe.cn

[R04] 位置参数
来源：http://ama.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cll.fehbvm.com

[R05] 参数默认值
来源：http://ntp.xinyue.icu

name="${1:-default}"
来源：http://gwu.xinyue.icu

[R06] 判断命令是否存在
来源：http://pht.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uhy.yuxming.cn

[R07] if 判断文件
来源：http://klf.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dqw.bbcook.cn

[R08] 数值比较
来源：http://gxe.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eqp.fktsv.cn

[R09] 字符串比较
来源：http://roc.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://elq.yuanzhike.top

[R10] 正则匹配
来源：http://fdd.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ibi.ydjk.org.cn

[R11] case 多分支
来源：http://tyv.jinqigfzy.top

case "$1" in
来源：http://snt.cashguo.top

start) echo "启动" ;;
来源：http://hqn.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://urr.tian-w.cn

*)     echo "未知命令" ;;
来源：http://toh.xuanzx.com

esac
来源：http://msq.fengsongda.top

[R12] for 遍历文件
来源：http://hho.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://bom.chenlongwang.top

[R13] for 计数循环
来源：http://kll.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://zxb.smart0.xyz

[R14] C 风格 for
来源：http://igj.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ekb.nwbrower.top

[R15] while 逐行读文件
来源：http://xen.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dex.sjlbkw.cn

[R16] until 等待条件
来源：http://mug.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rbr.cqqwz.cn

[R17] 数组定义与取值
来源：http://rao.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://bll.zhengqikj.top

[R18] 遍历数组
来源：http://jea.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kiv.dashuyun.cn

[R19] 数组长度
来源：http://mst.nanxinkj.top

echo "${#arr[@]}"
来源：http://vbh.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://syi.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sby.sxryk.cn

[R21] 字符串长度
来源：http://tcv.pycfn.com

echo "${#s}"
来源：http://kwe.yongpay.top

[R22] 截取子串
来源：http://czy.yueranfly.top

echo "${s:0:5}"
来源：http://gtl.zhijiandao.cn

[R23] 字符串替换
来源：http://ifz.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zbk.chenzaomai.com

[R24] 大小写转换
来源：http://wwq.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://jgr.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://emm.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qzd.xuetiantiany.cn

[R26] 命令替换
来源：http://twk.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://pqe.hcnkem.com

[R27] 算术展开
来源：http://mqv.sxryk.cn

echo $((1 + 2 * 3))
来源：http://ajd.nanxuanxn.top

[R28] 浮点运算
来源：http://nqe.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://ypo.shangyingyoupin.top

[R29] 定义函数
来源：http://gru.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://msx.redwolf501.top

[R30] 函数返回状态码
来源：http://ybx.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://lvw.zhoulong.xyz

[R31] 局部变量
来源：http://tau.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://wzy.zhongyouzk.top

[R32] 参数个数校验
来源：http://mmr.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://auz.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://prw.yongpay.top


<!-- 参考信息 -->