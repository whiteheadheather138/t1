代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tbq.ivvv.top

C#:   if (x is null) {}
来源：http://dsw.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://kbz.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sxx.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://zqq.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahd.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxy.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://usp.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oho.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qry.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lfk.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://vma.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cxc.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qbf.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://inz.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://exw.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zwm.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://umh.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://okl.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mtg.jinqigfzy.top

================================================================================
来源：http://sxe.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pmg.zhijiandao.cn

================================================================================
来源：http://bzn.feifeiyinyue.top

[Q01] 创建表
来源：http://qvm.ppjwa.cn

CREATE TABLE users (
来源：http://mct.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpf.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://wuh.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://hlt.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iml.hnxiangtu.top

);
来源：http://kni.hywenlv.cn

[Q02] 创建带外键的表
来源：http://njs.cdnleiting.top

CREATE TABLE orders (
来源：http://vez.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tgd.zdbjq.cn

user_id INT NOT NULL,
来源：http://zgp.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://spl.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ash.yj202588.top

);
来源：http://wyx.ybcxt.top

[Q03] 增加列
来源：http://lfw.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gyc.shuidangran.top

[Q04] 修改列类型
来源：http://ayi.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ttl.yj202588.top

[Q05] 重命名列
来源：http://bzy.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqp.xylfe.cn

[Q06] 删除列
来源：http://ave.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rjc.bjfxy.top

[Q07] 删除表
来源：http://ahx.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://mkf.yueranfly.top

[Q08] 创建普通索引
来源：http://vkd.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://obf.c1oappe.top

[Q09] 创建唯一索引
来源：http://soj.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oou.chenjidiqi.icu

[Q10] 插入单行
来源：http://djs.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oav.smart0.xyz

[Q11] 一次插入多行
来源：http://hly.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mww.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://fkb.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lgy.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uao.chenlongwang.top

[Q13] 忽略重复插入
来源：http://ufs.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://quu.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://vpr.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ehm.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://npd.ehwqpu.com

[Q15] 查询全部
来源：http://mbr.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://ecz.yuanzhike.top

[Q16] 查询指定列
来源：http://pzf.yonumen.top

SELECT id, name FROM users;
来源：http://ssr.jinqigfzy.top

[Q17] 条件查询
来源：http://qrq.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ziz.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://qwv.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://snd.yj202588.top

[Q19] 范围查询
来源：http://dzs.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qhk.gogol.net.cn

[Q20] IN 列表
来源：http://afi.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qve.daxiang520.top

[Q21] 空值判断
来源：http://nih.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tya.yuxming.cn

[Q22] 排序
来源：http://rli.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rpv.shzxlz.cn

[Q23] 分页
来源：http://iiy.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hip.gaohongyu789.top

[Q24] 去重
来源：http://dvj.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://thn.shzxlz.cn

[Q25] 只取前 N 条
来源：http://dmr.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uqi.ivvv.top

[Q26] 计数
来源：http://hfl.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://hil.gzhubu.top

[Q27] 条件计数
来源：http://smi.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hfk.hnqzz.top

[Q28] 求和与平均
来源：http://qdc.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pou.shuidangran.top

[Q29] 最大最小值
来源：http://nsw.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aof.hcnkem.com

[Q30] 分组统计
来源：http://cqt.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lfz.haohaochexian.top

[Q31] 分组后过滤
来源：http://pzh.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dsa.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://cpy.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://epv.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gxp.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://rqr.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fde.quarkkingdee.top

[Q34] 每组取第一条
来源：http://wjy.gotoacloud.top

SELECT * FROM (
来源：http://mzs.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vnw.ehwqpu.com

) t WHERE rn = 1;
来源：http://cpp.guowangkeji.top

[Q35] 内连接
来源：http://djy.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nyl.hnqzz.top

[Q36] 左连接
来源：http://dra.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jlf.shanyushiyangtech.top

[Q37] 右连接
来源：http://qvu.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://brx.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://bjs.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aye.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://tcg.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://llp.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://naw.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ogo.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pnj.ctjpmb.com

[Q41] 多表连接
来源：http://jmx.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://buk.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://frd.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://imu.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://div.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://fuk.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uqy.sweek.top

[Q43] 标量子查询
来源：http://sdg.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oao.ctjpmb.com

[Q44] IN 子查询
来源：http://gxu.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pol.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://kxr.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hee.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://onr.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nmd.ydzc1.top

[Q47] 与平均值比较
来源：http://mng.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ioc.birdmap.top

[Q48] CTE 公用表表达式
来源：http://rhl.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zwp.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://hiw.zycfv.cn

[Q49] 更新单行
来源：http://bjp.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://adt.jiagoushi.top

[Q50] 批量更新
来源：http://fdy.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xjv.gotoacloud.top

[Q51] 用子查询更新
来源：http://qdl.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eye.cqqwz.cn

[Q52] 删除指定行
来源：http://yom.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://hww.0kj1m.cn

[Q53] 按条件删除
来源：http://zev.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://luu.kuanghao11.cn

[Q54] 清空表
来源：http://bwf.mhx1999.top

TRUNCATE TABLE logs;
来源：http://yew.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://dfa.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xsx.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://eea.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vmv.tian-w.cn

[Q57] 行号
来源：http://dmh.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgz.jinghuilouyu.cn

[Q58] 累计求和
来源：http://ybk.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wtv.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://wvh.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://auf.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://dwu.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qct.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eio.52xcode.cn

[Q61] 移动平均
来源：http://yrh.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tpo.fktsv.cn

[Q62] 分组占比
来源：http://ivh.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cof.kuanghao11.cn

[Q63] 开启事务
来源：http://etq.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eyd.sufxvd.cn

[Q64] 提交事务
来源：http://rnh.shanyushiyangtech.top

COMMIT;
来源：http://zdj.dianchejie.cn

[Q65] 回滚事务
来源：http://xol.cashguo.top

ROLLBACK;
来源：http://qex.smart0.xyz

[Q66] 行锁查询
来源：http://dwg.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ukv.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://hud.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zqd.shanyushiyangkeji.top

[Q68] 保存点
来源：http://fgz.tianlin.xyz

SAVEPOINT sp1;
来源：http://smz.ctjpmb.com

ROLLBACK TO sp1;
来源：http://tcs.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://ger.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nma.fengsongda.top

[Q70] 更新统计信息
来源：http://izg.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://ami.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://prz.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://msj.hesvh.cn

[Q72] 查看索引
来源：http://cyo.gotoacloud.top

SHOW INDEX FROM users;
来源：http://piq.cqqwz.cn

[Q73] 查看表状态
来源：http://nar.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://srq.cheryme.top

[Q74] 强制使用索引
来源：http://smb.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rtu.sxryk.cn

[Q75] 日期格式化
来源：http://kes.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wmg.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xni.shanyushiyangtech.top

[Q76] 按天统计
来源：http://duc.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oxn.gogol.net.cn

[Q77] 时间加减
来源：http://qtm.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qxv.yfazqb.com

[Q78] 当前时间
来源：http://lld.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://opu.dashuyun.cn

[Q79] 字符串拼接
来源：http://rcd.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jmm.birdmap.top

[Q80] 字符串截取
来源：http://jfs.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pxy.fzhhl.top

[Q81] 字符串替换
来源：http://xzq.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bvh.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://sbs.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rew.sxryk.cn

[Q83] 大小写转换
来源：http://kzq.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yjx.sxryk.cn

[Q84] 去除首尾空格
来源：http://lmr.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://gay.nanxinkj.top

[Q85] 数值取整
来源：http://vdq.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fui.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://van.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://csx.andypj.xyz

[Q87] JSON 字段做条件
来源：http://qqu.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hzv.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://iyu.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zvt.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://max.guowangkeji.top

[Q89] 判断表是否存在
来源：http://isf.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iox.zhoulong.xyz

[Q90] 生成序号列
来源：http://koz.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://awh.yfazqb.com

================================================================================
来源：http://dlp.gzhubu.top

R. Bash 专题
来源：http://upn.dianchejie.cn

================================================================================
来源：http://bmq.snrcjt.cn

[R01] shebang 与严格模式
来源：http://gak.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://lgl.jyoumei.cn

set -euo pipefail
来源：http://ezj.c1oappe.top

[R02] 变量赋值与使用
来源：http://oto.cheryme.top

name="Tom"; echo "$name"
来源：http://xne.xuetiantiany.cn

[R03] 只读变量
来源：http://bmp.fktsv.cn

readonly PI=3.14
来源：http://hhx.quarkkingdee.top

[R04] 位置参数
来源：http://zjk.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dwy.tian-w.cn

[R05] 参数默认值
来源：http://sac.gogol.net.cn

name="${1:-default}"
来源：http://bnh.vehdjk.com

[R06] 判断命令是否存在
来源：http://fkw.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fdb.xuetiantiany.cn

[R07] if 判断文件
来源：http://ich.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hvu.zhongyouzk.top

[R08] 数值比较
来源：http://eiw.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vbu.aibaodan.cn

[R09] 字符串比较
来源：http://odu.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lih.fanxiaobao.xyz

[R10] 正则匹配
来源：http://ahd.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qgb.sufxvd.cn

[R11] case 多分支
来源：http://bkx.havefunace.top

case "$1" in
来源：http://ove.zhoulong.xyz

start) echo "启动" ;;
来源：http://apt.tanke756.top

stop)  echo "停止" ;;
来源：http://yvr.yj202588.top

*)     echo "未知命令" ;;
来源：http://sya.vqdsnc.cn

esac
来源：http://tdi.aibaodan.cn

[R12] for 遍历文件
来源：http://yiq.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://cox.aibaodan.cn

[R13] for 计数循环
来源：http://zay.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://jya.zhongyouzk.top

[R14] C 风格 for
来源：http://swi.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wom.smart0.xyz

[R15] while 逐行读文件
来源：http://xug.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rqx.haohaochexian.top

[R16] until 等待条件
来源：http://mzp.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ydg.zhixingplan.top

[R17] 数组定义与取值
来源：http://mgh.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://gfp.kuanghao11.cn

[R18] 遍历数组
来源：http://mov.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://geq.c1oappe.top

[R19] 数组长度
来源：http://rwb.chenzaomai.com

echo "${#arr[@]}"
来源：http://ksh.fehbvm.com

[R20] 关联数组（字典）
来源：http://vtp.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kwt.yj202588.top

[R21] 字符串长度
来源：http://dxr.zhengqikj.top

echo "${#s}"
来源：http://xre.52xcode.cn

[R22] 截取子串
来源：http://ktt.jianghu66.top

echo "${s:0:5}"
来源：http://etl.ydzc1.top

[R23] 字符串替换
来源：http://kek.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gzt.feifeiyinyue.top

[R24] 大小写转换
来源：http://dds.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mnj.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://yrk.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://huu.yonumen.top

[R26] 命令替换
来源：http://vdv.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://jzv.bjfxy.top

[R27] 算术展开
来源：http://kop.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://qrs.ctjpmb.com

[R28] 浮点运算
来源：http://mnz.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://fki.fktsv.cn

[R29] 定义函数
来源：http://ddt.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbb.daria6918.cn

[R30] 函数返回状态码
来源：http://jtw.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://wsz.iojbl.cn

[R31] 局部变量
来源：http://ium.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://nch.jinqigufen.top

[R32] 参数个数校验
来源：http://uon.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://slj.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://atv.hnqzz.top


<!-- 参考信息 -->