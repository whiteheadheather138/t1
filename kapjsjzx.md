代发 wailian999

PHP:  // 手写时间戳比较
来源：http://zxa.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvl.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nub.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jar.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mpl.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://ich.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://phe.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://ecw.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ynn.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://laz.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mpd.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dws.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nfs.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uxi.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fgi.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://edw.zhengqikj.top

================================================================================
来源：http://ivs.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pcr.hysaishi.cn

================================================================================
来源：http://mag.xinyue.icu

[Q01] 创建表
来源：http://xkn.epnwcf.com

CREATE TABLE users (
来源：http://bjq.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sjj.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://lhg.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://xzw.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://slf.yfazqb.com

);
来源：http://ipv.svipenyu.cn

[Q02] 创建带外键的表
来源：http://lsk.hammf.cn

CREATE TABLE orders (
来源：http://vho.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpu.svipenyu.cn

user_id INT NOT NULL,
来源：http://yud.smart0.xyz

amount DECIMAL(10, 2),
来源：http://jnp.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aln.chenjidiqi.icu

);
来源：http://fdw.sysykeji.top

[Q03] 增加列
来源：http://sod.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rnt.yuxming.cn

[Q04] 修改列类型
来源：http://hse.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ekc.fzhhl.top

[Q05] 重命名列
来源：http://iow.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zwo.cqqwz.cn

[Q06] 删除列
来源：http://nts.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cks.kuanghao11.cn

[Q07] 删除表
来源：http://fdv.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://hau.fktsv.cn

[Q08] 创建普通索引
来源：http://rim.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nkq.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://lkg.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jmv.shzxlz.cn

[Q10] 插入单行
来源：http://fcp.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mrr.zdqjudy.top

[Q11] 一次插入多行
来源：http://cph.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kza.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://hhv.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://ipt.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uru.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://kdt.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dra.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://dfa.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ckl.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hqx.cdnleiting.top

[Q15] 查询全部
来源：http://fxj.sufxvd.cn

SELECT * FROM users;
来源：http://nhe.52xcode.cn

[Q16] 查询指定列
来源：http://xwh.ppjwa.cn

SELECT id, name FROM users;
来源：http://obv.sweek.top

[Q17] 条件查询
来源：http://doh.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://khr.yj202588.top

[Q18] 模糊匹配
来源：http://vcv.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cpw.yvedp.cn

[Q19] 范围查询
来源：http://yvf.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zwt.jinqigfzy.top

[Q20] IN 列表
来源：http://nji.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wxr.kuanghao11.cn

[Q21] 空值判断
来源：http://muy.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mbe.yj20258888.top

[Q22] 排序
来源：http://mwg.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kki.yj20258.top

[Q23] 分页
来源：http://gfe.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://emh.tian-w.cn

[Q24] 去重
来源：http://jvh.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://ski.gogol.net.cn

[Q25] 只取前 N 条
来源：http://yur.yj20258888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdx.bbcook.cn

[Q26] 计数
来源：http://ltt.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://gej.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://sip.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ddt.9152youxi.cn

[Q28] 求和与平均
来源：http://mdv.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bat.cheryme.top

[Q29] 最大最小值
来源：http://vrd.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vec.daria6918.cn

[Q30] 分组统计
来源：http://avl.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dkq.hesvh.cn

[Q31] 分组后过滤
来源：http://nts.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zjf.cheryme.top

[Q32] 分组拼接字符串
来源：http://wrp.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://asl.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mql.jinqigufen.top

[Q33] 多列分组
来源：http://vsm.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fhz.ydjk.org.cn

[Q34] 每组取第一条
来源：http://vmo.bbcook.cn

SELECT * FROM (
来源：http://gvu.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ixx.zycfv.cn

) t WHERE rn = 1;
来源：http://mtu.nwbrower.top

[Q35] 内连接
来源：http://tht.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzb.xuanzx.com

[Q36] 左连接
来源：http://pgg.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gle.uphjek.com

[Q37] 右连接
来源：http://hry.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pau.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bdf.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lcq.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://rnd.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ram.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kbm.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://deg.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hlb.zdbjq.cn

[Q41] 多表连接
来源：http://vvb.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://guv.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://tyr.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://edm.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://cyj.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://lyp.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://szk.yj20258888.top

[Q43] 标量子查询
来源：http://eve.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rtw.fehbvm.com

[Q44] IN 子查询
来源：http://mea.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cuh.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://bui.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vnq.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dcq.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mnq.fktsv.cn

[Q47] 与平均值比较
来源：http://fth.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kmr.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://apw.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tgm.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://kvg.birdmap.top

[Q49] 更新单行
来源：http://ebu.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gmz.hongshengwenyu.top

[Q50] 批量更新
来源：http://rpe.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fjk.tian-w.cn

[Q51] 用子查询更新
来源：http://dlm.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cfm.bjfxy.top

[Q52] 删除指定行
来源：http://vxn.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://kze.ydjk.org.cn

[Q53] 按条件删除
来源：http://lad.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://smx.xuanzx.com

[Q54] 清空表
来源：http://dnt.pycfn.com

TRUNCATE TABLE logs;
来源：http://arh.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://jwt.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xak.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://tly.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jcd.wangshuangyany.cn

[Q57] 行号
来源：http://jia.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fdw.jinghuilouyu.cn

[Q58] 累计求和
来源：http://xhd.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rlz.vqdsnc.cn

[Q59] 分组内累计
来源：http://crp.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://upn.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://utv.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pby.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kkl.gzhubu.top

[Q61] 移动平均
来源：http://xqj.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://omy.ydjk.org.cn

[Q62] 分组占比
来源：http://iyr.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://byy.bbcook.cn

[Q63] 开启事务
来源：http://xqu.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://alb.shanyushiyangtech.top

[Q64] 提交事务
来源：http://sra.smart0.xyz

COMMIT;
来源：http://cax.hongshengwenyu.top

[Q65] 回滚事务
来源：http://pte.nanxinkj.top

ROLLBACK;
来源：http://wqq.hywenlv.cn

[Q66] 行锁查询
来源：http://tya.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ztb.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://mdb.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uzg.ybcxt.top

[Q68] 保存点
来源：http://bqx.snrcjt.cn

SAVEPOINT sp1;
来源：http://bbi.jyoumei.cn

ROLLBACK TO sp1;
来源：http://wxy.fehbvm.com

[Q69] 查看执行计划
来源：http://jjw.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ixl.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://bah.nanxuanxn.top

ANALYZE TABLE users;
来源：http://rog.zhengqikj.top

[Q71] 查看建表语句
来源：http://czb.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hck.shzxlz.cn

[Q72] 查看索引
来源：http://syw.guowangkeji.top

SHOW INDEX FROM users;
来源：http://wrg.0kj1m.cn

[Q73] 查看表状态
来源：http://ejd.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jox.meibo888.top

[Q74] 强制使用索引
来源：http://lte.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ina.yj20258.top

[Q75] 日期格式化
来源：http://gdk.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iml.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cal.zhongyouzk.top

[Q76] 按天统计
来源：http://vwn.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rib.haohaochexian.top

[Q77] 时间加减
来源：http://csu.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xfj.c1oappe.top

[Q78] 当前时间
来源：http://wbc.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pcp.smart0.xyz

[Q79] 字符串拼接
来源：http://njv.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cqa.jqgfzy.top

[Q80] 字符串截取
来源：http://yfm.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gxx.yfazqb.com

[Q81] 字符串替换
来源：http://afh.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vnl.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://ofi.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://apz.yj20258888.top

[Q83] 大小写转换
来源：http://dvu.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bup.redwolf501.top

[Q84] 去除首尾空格
来源：http://ghe.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://ofi.chenlongwang.top

[Q85] 数值取整
来源：http://jus.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pqg.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://ciy.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uef.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://ybj.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uzi.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://ddt.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ask.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://edb.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://ayj.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ayq.meibo888.top

[Q90] 生成序号列
来源：http://tsv.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cxc.xylfe.cn

================================================================================
来源：http://krj.redwolf501.top

R. Bash 专题
来源：http://abf.tanke756.top

================================================================================
来源：http://vvw.fengsongda.top

[R01] shebang 与严格模式
来源：http://qce.xuanzx.com

#!/usr/bin/env bash
来源：http://dli.pycfn.com

set -euo pipefail
来源：http://xes.tarul.cn

[R02] 变量赋值与使用
来源：http://nrg.shuidangran.top

name="Tom"; echo "$name"
来源：http://fyc.kuanghao11.cn

[R03] 只读变量
来源：http://vus.yj20258888.top

readonly PI=3.14
来源：http://ihz.zdbjq.cn

[R04] 位置参数
来源：http://vpa.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zil.yongpay.top

[R05] 参数默认值
来源：http://pki.shangyingyoupin.top

name="${1:-default}"
来源：http://bqh.jiagoushi.top

[R06] 判断命令是否存在
来源：http://fxo.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dgg.ehwqpu.com

[R07] if 判断文件
来源：http://hwy.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nfp.jinqigfzy.top

[R08] 数值比较
来源：http://qjj.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lpy.zycfv.cn

[R09] 字符串比较
来源：http://dsp.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://diz.hnxiangtu.top

[R10] 正则匹配
来源：http://qag.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ccc.c1oappe.top

[R11] case 多分支
来源：http://pbk.daria6918.cn

case "$1" in
来源：http://hfh.zhixingplan.top

start) echo "启动" ;;
来源：http://xwg.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://vgt.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://vrr.316326.xyz

esac
来源：http://vkm.jinqigfzy.top

[R12] for 遍历文件
来源：http://qjq.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://bdu.hywenlv.cn

[R13] for 计数循环
来源：http://cyv.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://nvo.yangfankeji.com

[R14] C 风格 for
来源：http://syy.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zmf.nanxinkj.top

[R15] while 逐行读文件
来源：http://rev.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lcu.zhoulong.xyz

[R16] until 等待条件
来源：http://efx.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zyw.chenzaomai.com

[R17] 数组定义与取值
来源：http://utx.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://mhp.xylfe.cn

[R18] 遍历数组
来源：http://pef.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://psh.yongpay.top

[R19] 数组长度
来源：http://epm.ydzc1.top

echo "${#arr[@]}"
来源：http://zqd.ybcxt.top

[R20] 关联数组（字典）
来源：http://sks.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://afd.52xcode.cn

[R21] 字符串长度
来源：http://wwz.fengsongda.top

echo "${#s}"
来源：http://rdv.yj20258888.top

[R22] 截取子串
来源：http://xup.redwolf501.top

echo "${s:0:5}"
来源：http://plb.meibo888.top

[R23] 字符串替换
来源：http://hyk.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkf.svipenyu.cn

[R24] 大小写转换
来源：http://adr.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://qwu.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://tiy.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vkj.guowangkeji.top

[R26] 命令替换
来源：http://tzi.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://cgl.zhoulong.xyz

[R27] 算术展开
来源：http://qqd.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://etg.cqqwz.cn

[R28] 浮点运算
来源：http://rvo.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://xyk.shzxlz.cn

[R29] 定义函数
来源：http://mvn.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hna.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://jam.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://eop.ivvv.top

[R31] 局部变量
来源：http://uza.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://rua.jinqigfzy.top

[R32] 参数个数校验
来源：http://izf.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uak.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://fmo.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qwu.cheryme.top

[R34] 退出时清理
来源：http://vkr.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://urv.havefunace.top

[R35] 后台执行并等待
来源：http://agi.zhongyouzk.top


<!-- 参考信息 -->