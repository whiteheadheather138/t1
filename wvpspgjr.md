代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://knw.andypj.xyz

C#:   if (x is null) {}
来源：http://zok.ydzc1.top

[P07] 防抖与节流
来源：http://haa.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://buk.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://clk.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vxd.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffe.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gok.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qtj.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bdt.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ogr.tian-w.cn

[P08] 处理浮点精度问题
来源：http://blp.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lgw.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xhz.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://une.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mwe.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sdh.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mst.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hsq.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://adm.zhixingplan.top

================================================================================
来源：http://dld.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://amp.zhaomingkeji.xyz

================================================================================
来源：http://pof.shangyingyoupin.top

[Q01] 创建表
来源：http://xor.iojbl.cn

CREATE TABLE users (
来源：http://acr.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvg.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://rlq.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://zfa.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lsl.yueranfly.top

);
来源：http://wxm.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://jio.zhijiandao.cn

CREATE TABLE orders (
来源：http://jdb.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nhh.dashuyun.cn

user_id INT NOT NULL,
来源：http://mao.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://hkg.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qpu.ctjpmb.com

);
来源：http://yqb.quarkkingdee.top

[Q03] 增加列
来源：http://hvt.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://huj.shuidangran.top

[Q04] 修改列类型
来源：http://nox.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://you.fktsv.cn

[Q05] 重命名列
来源：http://nql.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vxt.pengpengdd.cyou

[Q06] 删除列
来源：http://rbn.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://hss.zhoulong.xyz

[Q07] 删除表
来源：http://gcv.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://xko.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://osx.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://gyc.fengsongda.top

[Q09] 创建唯一索引
来源：http://iyu.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://udn.zhijiandao.cn

[Q10] 插入单行
来源：http://bwx.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://twr.fzhhl.top

[Q11] 一次插入多行
来源：http://dar.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jtb.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://kwu.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aut.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xmp.svipenyu.cn

[Q13] 忽略重复插入
来源：http://mrw.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oyu.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://vdf.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://exf.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fda.zhengqikj.top

[Q15] 查询全部
来源：http://trz.yj20258.top

SELECT * FROM users;
来源：http://mpb.9152youxi.cn

[Q16] 查询指定列
来源：http://pcj.meibo888.top

SELECT id, name FROM users;
来源：http://zut.ctjpmb.com

[Q17] 条件查询
来源：http://rah.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dxr.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://pbm.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mct.gotoacloud.top

[Q19] 范围查询
来源：http://puk.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zfi.meibo888.top

[Q20] IN 列表
来源：http://axy.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hde.zhixingplan.top

[Q21] 空值判断
来源：http://yrl.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jpg.jlsjyb.cn

[Q22] 排序
来源：http://hdn.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kqr.hysaishi.cn

[Q23] 分页
来源：http://nmr.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hvx.bbcook.cn

[Q24] 去重
来源：http://rem.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://nsq.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://xnt.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://khi.zhoulong.xyz

[Q26] 计数
来源：http://tqs.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://qvc.kuanghao11.cn

[Q27] 条件计数
来源：http://psr.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xkh.epnwcf.com

[Q28] 求和与平均
来源：http://ezb.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://toj.sjlbkw.cn

[Q29] 最大最小值
来源：http://fpw.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ijy.cdnleiting.top

[Q30] 分组统计
来源：http://jch.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cnn.gzhubu.top

[Q31] 分组后过滤
来源：http://zyf.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lon.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://xwc.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lgq.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mmb.jinqigufen.top

[Q33] 多列分组
来源：http://zud.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lje.havefunace.top

[Q34] 每组取第一条
来源：http://hvn.feifeiyinyue.top

SELECT * FROM (
来源：http://gje.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fdm.epnwcf.com

) t WHERE rn = 1;
来源：http://qxq.snrcjt.cn

[Q35] 内连接
来源：http://cxo.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xpv.guannengcc.top

[Q36] 左连接
来源：http://pwm.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://esm.yj20258888.top

[Q37] 右连接
来源：http://sbf.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xpy.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://clg.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://klr.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://mcs.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lfd.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xbb.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bpu.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qvx.yvedp.cn

[Q41] 多表连接
来源：http://dfn.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bjk.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://xdm.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://tqv.yonumen.top

[Q42] 连接条件附加过滤
来源：http://dzz.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://gbz.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xzv.snrcjt.cn

[Q43] 标量子查询
来源：http://vqm.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://buw.xuanzx.com

[Q44] IN 子查询
来源：http://qrg.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://orn.ivvv.top

[Q45] EXISTS 判断存在
来源：http://jxq.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://swu.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sek.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zch.iojbl.cn

[Q47] 与平均值比较
来源：http://bae.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gdq.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://swh.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qsw.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://ona.daxiang520.top

[Q49] 更新单行
来源：http://mrg.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ypx.zhoulong.xyz

[Q50] 批量更新
来源：http://waw.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hog.ppjwa.cn

[Q51] 用子查询更新
来源：http://xav.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xpt.zhoulong.xyz

[Q52] 删除指定行
来源：http://pcl.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://adt.cqqwz.cn

[Q53] 按条件删除
来源：http://vui.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uxp.c1oappe.top

[Q54] 清空表
来源：http://bdp.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://myy.bbcook.cn

[Q55] 排名（并列占位）
来源：http://wkc.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qum.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://eix.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://twm.yuanzhike.top

[Q57] 行号
来源：http://ejs.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://thi.uphjek.com

[Q58] 累计求和
来源：http://psy.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ehn.tianlin.xyz

[Q59] 分组内累计
来源：http://rfk.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rcs.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://aef.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ywz.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpc.yonumen.top

[Q61] 移动平均
来源：http://dvj.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ttb.bjfxy.top

[Q62] 分组占比
来源：http://edz.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gmz.shuidangran.top

[Q63] 开启事务
来源：http://iiz.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://max.xziqi.cn

[Q64] 提交事务
来源：http://mdb.shanyushiyangtech.top

COMMIT;
来源：http://nhn.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://awn.hesvh.cn

ROLLBACK;
来源：http://lbu.zdbjq.cn

[Q66] 行锁查询
来源：http://uww.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mai.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://rht.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dwp.feifeiyinyue.top

[Q68] 保存点
来源：http://ull.yangfankeji.com

SAVEPOINT sp1;
来源：http://qnz.sufxvd.cn

ROLLBACK TO sp1;
来源：http://cnh.fehbvm.com

[Q69] 查看执行计划
来源：http://xdg.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://spk.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://hmd.zdbjq.cn

ANALYZE TABLE users;
来源：http://wza.chenzaomai.com

[Q71] 查看建表语句
来源：http://evn.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cpg.jinghuilouyu.cn

[Q72] 查看索引
来源：http://elf.hesvh.cn

SHOW INDEX FROM users;
来源：http://qbv.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://imt.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ocd.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://elk.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rzc.quarkkingdee.top

[Q75] 日期格式化
来源：http://wvq.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://txo.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dsu.zhengqikj.top

[Q76] 按天统计
来源：http://uqz.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aey.tianlin.xyz

[Q77] 时间加减
来源：http://bvj.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qxd.hammf.cn

[Q78] 当前时间
来源：http://cpd.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ujn.guannengcc.top

[Q79] 字符串拼接
来源：http://isb.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://byk.daxiang520.top

[Q80] 字符串截取
来源：http://mkw.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bzh.c1oappe.top

[Q81] 字符串替换
来源：http://oxe.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://npu.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://mzd.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uyw.havefunace.top

[Q83] 大小写转换
来源：http://ypa.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hek.chenzaomai.com

[Q84] 去除首尾空格
来源：http://bwe.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://doj.yueranfly.top

[Q85] 数值取整
来源：http://mce.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jxy.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://aog.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nsg.ydzc1.top

[Q87] JSON 字段做条件
来源：http://jdw.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gvp.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://plg.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xlx.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hfm.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://jlo.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cbb.fktsv.cn

[Q90] 生成序号列
来源：http://oqx.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnb.nanxinkj.top

================================================================================
来源：http://mrt.jiagoushi.top

R. Bash 专题
来源：http://bsc.sxryk.cn

================================================================================
来源：http://fsh.cheryme.top

[R01] shebang 与严格模式
来源：http://qak.yfazqb.com

#!/usr/bin/env bash
来源：http://vmq.feifeiyinyue.top

set -euo pipefail
来源：http://gyh.316326.xyz

[R02] 变量赋值与使用
来源：http://tmi.ivvv.top

name="Tom"; echo "$name"
来源：http://tix.shuidangran.top

[R03] 只读变量
来源：http://pti.ydjk.org.cn

readonly PI=3.14
来源：http://mnz.shanyushiyangtech.top

[R04] 位置参数
来源：http://wig.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://isd.jlsjyb.cn

[R05] 参数默认值
来源：http://edp.jinqigufen.top

name="${1:-default}"
来源：http://rfo.hesvh.cn

[R06] 判断命令是否存在
来源：http://uyo.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vgl.c1oappe.top

[R07] if 判断文件
来源：http://nur.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rms.xylfe.cn

[R08] 数值比较
来源：http://ofk.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ztc.yongpay.top

[R09] 字符串比较
来源：http://xpe.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://roq.aibaodan.cn

[R10] 正则匹配
来源：http://tyb.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kof.dianchejie.cn

[R11] case 多分支
来源：http://ylu.sxryk.cn

case "$1" in
来源：http://zdu.feifeiyinyue.top

start) echo "启动" ;;
来源：http://cho.ivvv.top

stop)  echo "停止" ;;
来源：http://edp.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://ihz.pycfn.com

esac
来源：http://eqd.xylfe.cn

[R12] for 遍历文件
来源：http://mqg.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://tka.sweek.top

[R13] for 计数循环
来源：http://tkz.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://cyk.uphjek.com

[R14] C 风格 for
来源：http://ppq.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://msp.sweek.top

[R15] while 逐行读文件
来源：http://utt.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xgl.ydjk.org.cn

[R16] until 等待条件
来源：http://vax.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cow.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://vuk.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://ecq.sweek.top

[R18] 遍历数组
来源：http://fsc.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dqj.daria6918.cn

[R19] 数组长度
来源：http://ucn.316326.xyz

echo "${#arr[@]}"
来源：http://csb.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://icx.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ibp.pengpengdd.cyou

[R21] 字符串长度
来源：http://oga.shanyushiyangtech.top

echo "${#s}"
来源：http://xmi.chenzaomai.com

[R22] 截取子串
来源：http://pxs.tianlin.xyz

echo "${s:0:5}"
来源：http://oqn.gotoacloud.top

[R23] 字符串替换
来源：http://vxt.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qqz.zdbjq.cn

[R24] 大小写转换
来源：http://vhw.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://jhk.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://twv.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ozz.ehwqpu.com

[R26] 命令替换
来源：http://mqh.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://qvl.yj20258.top

[R27] 算术展开
来源：http://giy.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://dyq.xinyue.icu

[R28] 浮点运算
来源：http://hbu.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://qbc.feifeiyinyue.top

[R29] 定义函数
来源：http://den.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ycd.jlsjyb.cn

[R30] 函数返回状态码
来源：http://cde.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://dpq.fengsongda.top

[R31] 局部变量
来源：http://ssk.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://eth.quarkkingdee.top

[R32] 参数个数校验
来源：http://nut.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nkx.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://bhb.aibaodan.cn


<!-- 参考信息 -->