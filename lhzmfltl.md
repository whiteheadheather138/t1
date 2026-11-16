代发 wailian999

PHP:  // 手写时间戳比较
来源：http://ziz.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fer.gaohongyu789.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qli.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nxl.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pzb.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://shh.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vtj.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://uiu.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iwi.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yir.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ywp.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xfk.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yhu.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pgf.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fxf.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://evo.ppjwa.cn

================================================================================
来源：http://ltg.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vvj.zhijiandao.cn

================================================================================
来源：http://nfu.feifeiyinyue.top

[Q01] 创建表
来源：http://hvg.zhiwuduotai.top

CREATE TABLE users (
来源：http://hnu.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzb.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://nbj.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://mfv.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://enn.fehbvm.com

);
来源：http://chg.uphjek.com

[Q02] 创建带外键的表
来源：http://gsg.birdmap.top

CREATE TABLE orders (
来源：http://rqf.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gck.zycfv.cn

user_id INT NOT NULL,
来源：http://lmy.jianghu66.top

amount DECIMAL(10, 2),
来源：http://pzv.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pbj.birdmap.top

);
来源：http://yud.bjfxy.top

[Q03] 增加列
来源：http://xdi.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyt.316326.xyz

[Q04] 修改列类型
来源：http://wpu.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uss.wangdashe.top

[Q05] 重命名列
来源：http://und.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pwm.yvedp.cn

[Q06] 删除列
来源：http://uzf.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://xio.mhx1999.top

[Q07] 删除表
来源：http://qyo.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://lxx.yanxiufei.cn

[Q08] 创建普通索引
来源：http://dkh.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ntq.tarul.cn

[Q09] 创建唯一索引
来源：http://vxu.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wts.vehdjk.com

[Q10] 插入单行
来源：http://zhp.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mtf.haohaochexian.top

[Q11] 一次插入多行
来源：http://pyu.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://izh.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://lmk.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://qpy.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zna.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://aih.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yqt.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://jox.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lgn.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dnh.hongshengwenyu.top

[Q15] 查询全部
来源：http://ghq.vehdjk.com

SELECT * FROM users;
来源：http://mkv.yueranfly.top

[Q16] 查询指定列
来源：http://lym.dianchejie.cn

SELECT id, name FROM users;
来源：http://zyn.0kj1m.cn

[Q17] 条件查询
来源：http://pey.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vdv.hammf.cn

[Q18] 模糊匹配
来源：http://ffz.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aqz.9152youxi.cn

[Q19] 范围查询
来源：http://gfc.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xgt.jinqigfzy.top

[Q20] IN 列表
来源：http://exp.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oex.zhongyouzk.top

[Q21] 空值判断
来源：http://swx.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://htk.xingfuxueyuan.xyz

[Q22] 排序
来源：http://mja.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rij.gzhubu.top

[Q23] 分页
来源：http://jtt.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uzi.andypj.xyz

[Q24] 去重
来源：http://qfl.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://tgg.jyoumei.cn

[Q25] 只取前 N 条
来源：http://fch.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jzx.zhongyouzk.top

[Q26] 计数
来源：http://vzy.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://bqp.cdnleiting.top

[Q27] 条件计数
来源：http://cro.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pvq.tanke756.top

[Q28] 求和与平均
来源：http://gcg.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dgz.jiagoushi.top

[Q29] 最大最小值
来源：http://qgl.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uvo.jqgfzy.top

[Q30] 分组统计
来源：http://yro.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sog.haohaochexian.top

[Q31] 分组后过滤
来源：http://mhw.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dpo.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://nrf.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://stl.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://isc.ehwqpu.com

[Q33] 多列分组
来源：http://zfp.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qkq.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://ihz.zdqjudy.top

SELECT * FROM (
来源：http://ame.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rec.yvedp.cn

) t WHERE rn = 1;
来源：http://bjq.hesvh.cn

[Q35] 内连接
来源：http://xcx.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://olo.hysaishi.cn

[Q36] 左连接
来源：http://nak.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yfq.9152youxi.cn

[Q37] 右连接
来源：http://itw.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nbv.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://gxt.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gli.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://nmk.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oim.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ktb.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pgr.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rzd.shzxlz.cn

[Q41] 多表连接
来源：http://dxo.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hoi.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://oiu.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://eyn.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://wxd.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://oss.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nsc.hongshengwenyu.top

[Q43] 标量子查询
来源：http://epm.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qzv.xuetiantiany.cn

[Q44] IN 子查询
来源：http://ful.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ffu.tanke756.top

[Q45] EXISTS 判断存在
来源：http://bra.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gzl.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cti.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iff.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://ysh.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://syw.birdmap.top

[Q48] CTE 公用表表达式
来源：http://yuh.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sen.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://rlb.pengpengdd.cyou

[Q49] 更新单行
来源：http://qvk.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ifd.epnwcf.com

[Q50] 批量更新
来源：http://gzp.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zhp.andypj.xyz

[Q51] 用子查询更新
来源：http://izb.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oua.yongpay.top

[Q52] 删除指定行
来源：http://njo.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://uql.cdnleiting.top

[Q53] 按条件删除
来源：http://xlu.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vxg.ybcxt.top

[Q54] 清空表
来源：http://llo.xylfe.cn

TRUNCATE TABLE logs;
来源：http://wvw.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://irn.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pum.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://fwb.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvy.cqqwz.cn

[Q57] 行号
来源：http://sni.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sku.tanke756.top

[Q58] 累计求和
来源：http://rvb.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vwi.andypj.xyz

[Q59] 分组内累计
来源：http://sld.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://msa.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://uey.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://avl.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bxg.hammf.cn

[Q61] 移动平均
来源：http://tsu.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jzg.yuanzhike.top

[Q62] 分组占比
来源：http://xlg.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hdy.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://ent.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dwa.cashguo.top

[Q64] 提交事务
来源：http://qgg.fengsongda.top

COMMIT;
来源：http://uis.xylfe.cn

[Q65] 回滚事务
来源：http://vwq.cucudq.cn

ROLLBACK;
来源：http://bfm.hammf.cn

[Q66] 行锁查询
来源：http://ouf.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://stq.xziqi.cn

[Q67] 设置隔离级别
来源：http://vzf.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brc.zhaomingkeji.xyz

[Q68] 保存点
来源：http://phg.jqgufenzy.top

SAVEPOINT sp1;
来源：http://gyz.yj20258.top

ROLLBACK TO sp1;
来源：http://fnp.fktsv.cn

[Q69] 查看执行计划
来源：http://dsm.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tzw.zhijiandao.cn

[Q70] 更新统计信息
来源：http://evb.bjfxy.top

ANALYZE TABLE users;
来源：http://bpq.aibaodan.cn

[Q71] 查看建表语句
来源：http://mrr.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bxq.hnqzz.top

[Q72] 查看索引
来源：http://ndu.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://qug.tarul.cn

[Q73] 查看表状态
来源：http://lvr.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oyi.chenzaomai.com

[Q74] 强制使用索引
来源：http://gks.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vgg.jqgufenzy.top

[Q75] 日期格式化
来源：http://ovj.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vzs.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://udn.yonumen.top

[Q76] 按天统计
来源：http://dpm.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hln.jinghuilouyu.cn

[Q77] 时间加减
来源：http://qxx.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pub.hesvh.cn

[Q78] 当前时间
来源：http://noy.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ebw.yj20258888.top

[Q79] 字符串拼接
来源：http://fkl.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tdy.fktsv.cn

[Q80] 字符串截取
来源：http://zga.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qoz.hnxiangtu.top

[Q81] 字符串替换
来源：http://hmy.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dsb.yj20258.top

[Q82] 字符长度与字节长度
来源：http://yuh.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bkw.cheryme.top

[Q83] 大小写转换
来源：http://cen.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mab.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://ool.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://djy.ydjk.org.cn

[Q85] 数值取整
来源：http://qxx.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eth.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://qix.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mul.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ylo.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dar.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://sqr.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gye.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bkv.yueranfly.top

[Q89] 判断表是否存在
来源：http://ats.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwt.nwbrower.top

[Q90] 生成序号列
来源：http://grg.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://alo.pengpengdd.cyou

================================================================================
来源：http://xtx.fanxiaobao.xyz

R. Bash 专题
来源：http://quc.ydjk.org.cn

================================================================================
来源：http://lqp.yj20258888.top

[R01] shebang 与严格模式
来源：http://qxt.dianchejie.cn

#!/usr/bin/env bash
来源：http://yuf.nanxuanxn.top

set -euo pipefail
来源：http://qbg.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://gfu.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://che.jyoumei.cn

[R03] 只读变量
来源：http://ecc.svipenyu.cn

readonly PI=3.14
来源：http://mrj.sweek.top

[R04] 位置参数
来源：http://ujn.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iau.iojbl.cn

[R05] 参数默认值
来源：http://jke.52xcode.cn

name="${1:-default}"
来源：http://jrf.daxiang520.top

[R06] 判断命令是否存在
来源：http://pew.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibw.yangfankeji.com

[R07] if 判断文件
来源：http://gov.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rsg.yonumen.top

[R08] 数值比较
来源：http://lgg.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rtb.iojbl.cn

[R09] 字符串比较
来源：http://ltw.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ert.52xcode.cn

[R10] 正则匹配
来源：http://qxq.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qph.bjfxy.top

[R11] case 多分支
来源：http://gmx.cashguo.top

case "$1" in
来源：http://bnm.nanxinkj.top

start) echo "启动" ;;
来源：http://rbh.mhx1999.top

stop)  echo "停止" ;;
来源：http://ten.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://jaj.0kj1m.cn

esac
来源：http://pos.fktsv.cn

[R12] for 遍历文件
来源：http://bpn.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://djv.jqgufenzy.top

[R13] for 计数循环
来源：http://wld.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://stg.zhengqikj.top

[R14] C 风格 for
来源：http://jlx.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qyo.jqgufenzy.top

[R15] while 逐行读文件
来源：http://sbv.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bgs.bbcook.cn

[R16] until 等待条件
来源：http://zmf.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qzv.smart0.xyz

[R17] 数组定义与取值
来源：http://coe.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uwj.cucudq.cn

[R18] 遍历数组
来源：http://aww.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hdr.fanxiaobao.xyz

[R19] 数组长度
来源：http://xin.fehbvm.com

echo "${#arr[@]}"
来源：http://wgf.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://uuo.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qcj.guannengcc.top

[R21] 字符串长度
来源：http://xhc.vqdsnc.cn

echo "${#s}"
来源：http://mlo.zhoulong.xyz

[R22] 截取子串
来源：http://psg.nanxinkj.top

echo "${s:0:5}"
来源：http://sfc.xinyue.icu

[R23] 字符串替换
来源：http://mgr.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ccv.quarkkingdee.top

[R24] 大小写转换
来源：http://uff.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wuc.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://zlo.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbn.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://smw.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://uda.ybcxt.top

[R27] 算术展开
来源：http://evj.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://xoi.chenlongwang.top

[R28] 浮点运算
来源：http://pah.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://aoh.yj20258.top

[R29] 定义函数
来源：http://zvo.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xnl.jyoumei.cn

[R30] 函数返回状态码
来源：http://mqn.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://cui.yj20258888.top

[R31] 局部变量
来源：http://cgb.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://bml.hesvh.cn

[R32] 参数个数校验
来源：http://ufs.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nrj.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://hpq.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hei.fktsv.cn

[R34] 退出时清理
来源：http://cck.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dia.xuanzx.com

[R35] 后台执行并等待
来源：http://uff.chenjidiqi.icu


<!-- 参考信息 -->