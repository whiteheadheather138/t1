代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://can.vqdsnc.cn

C#:   if (x is null) {}
来源：http://wkb.zhengqikj.top

[P07] 防抖与节流
来源：http://sgk.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nka.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://vya.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfk.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzx.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pdm.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lpr.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kvr.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dlw.xinyue.icu

[P08] 处理浮点精度问题
来源：http://xum.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://muv.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xjm.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ndc.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nce.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ppu.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ven.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iia.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zbs.hnqzz.top

================================================================================
来源：http://apq.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xbv.yfazqb.com

================================================================================
来源：http://wdr.jiagoushi.top

[Q01] 创建表
来源：http://bsu.hysaishi.cn

CREATE TABLE users (
来源：http://hil.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://toc.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://atj.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://opy.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gnp.52xcode.cn

);
来源：http://bln.nanxinkj.top

[Q02] 创建带外键的表
来源：http://jqr.sxryk.cn

CREATE TABLE orders (
来源：http://wfb.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dhb.zdbjq.cn

user_id INT NOT NULL,
来源：http://gve.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://mic.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wtl.yuxming.cn

);
来源：http://yfb.vehdjk.com

[Q03] 增加列
来源：http://ydo.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ugh.zdbjq.cn

[Q04] 修改列类型
来源：http://yud.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ovn.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://vwm.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bjc.dianchejie.cn

[Q06] 删除列
来源：http://pfm.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uzq.xziqi.cn

[Q07] 删除表
来源：http://crl.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://xps.9152youxi.cn

[Q08] 创建普通索引
来源：http://ntv.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sdo.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://fta.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fal.shangyingyoupin.top

[Q10] 插入单行
来源：http://nyg.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lki.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://ilz.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yod.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://yvl.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://sfu.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rwk.yj20258.top

[Q13] 忽略重复插入
来源：http://jee.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpt.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://vch.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgb.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://imb.bjfxy.top

[Q15] 查询全部
来源：http://tia.316326.xyz

SELECT * FROM users;
来源：http://uoy.hongshengwenyu.top

[Q16] 查询指定列
来源：http://xgc.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://qnj.daria6918.cn

[Q17] 条件查询
来源：http://wfy.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yhv.daria6918.cn

[Q18] 模糊匹配
来源：http://vkt.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fpd.sjlbkw.cn

[Q19] 范围查询
来源：http://qsd.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://djn.nwbrower.top

[Q20] IN 列表
来源：http://tvz.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tcy.hywenlv.cn

[Q21] 空值判断
来源：http://gtb.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yqb.yongpay.top

[Q22] 排序
来源：http://hpm.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://twu.tanke756.top

[Q23] 分页
来源：http://fre.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xdf.ywan-chungtsiang.top

[Q24] 去重
来源：http://sbv.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://lzc.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://ytv.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xea.0kj1m.cn

[Q26] 计数
来源：http://xgn.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://kbz.ehwqpu.com

[Q27] 条件计数
来源：http://uuf.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qer.jlsjyb.cn

[Q28] 求和与平均
来源：http://glh.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dew.c1oappe.top

[Q29] 最大最小值
来源：http://skg.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rtd.hywenlv.cn

[Q30] 分组统计
来源：http://ubs.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uyh.gotoacloud.top

[Q31] 分组后过滤
来源：http://dks.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jwp.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://ava.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ngf.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://psl.jqgufenzy.top

[Q33] 多列分组
来源：http://hgg.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://scq.yangfankeji.com

[Q34] 每组取第一条
来源：http://kbj.guannengcc.top

SELECT * FROM (
来源：http://ala.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lph.jyoumei.cn

) t WHERE rn = 1;
来源：http://hmy.jqgfzy.top

[Q35] 内连接
来源：http://boe.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qdl.316326.xyz

[Q36] 左连接
来源：http://ajp.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bpx.316326.xyz

[Q37] 右连接
来源：http://hnw.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oqw.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://jlh.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fiy.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://hyc.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayk.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jpd.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bkn.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nja.xuetiantiany.cn

[Q41] 多表连接
来源：http://pvk.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tky.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://fga.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://thn.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://pvm.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://ijj.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dqn.shangyingyoupin.top

[Q43] 标量子查询
来源：http://alh.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbg.fehbvm.com

[Q44] IN 子查询
来源：http://bho.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wik.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://psa.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lag.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nos.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zxd.aizwys.cn

[Q47] 与平均值比较
来源：http://gsv.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://edx.cashguo.top

[Q48] CTE 公用表表达式
来源：http://rmm.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qep.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://xty.nwbrower.top

[Q49] 更新单行
来源：http://kjn.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uil.yueranfly.top

[Q50] 批量更新
来源：http://nox.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oee.zhixingplan.top

[Q51] 用子查询更新
来源：http://wwc.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mtk.hnxiangtu.top

[Q52] 删除指定行
来源：http://wll.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://zjh.yj20258888.top

[Q53] 按条件删除
来源：http://evm.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qmo.yonumen.top

[Q54] 清空表
来源：http://bzi.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://mxw.52xcode.cn

[Q55] 排名（并列占位）
来源：http://eqb.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://odu.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://ceq.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://llr.birdmap.top

[Q57] 行号
来源：http://nzq.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gcp.yuxming.cn

[Q58] 累计求和
来源：http://aem.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vgx.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://iys.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iqj.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://pun.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iku.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yjl.sweek.top

[Q61] 移动平均
来源：http://ijj.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cua.sjlbkw.cn

[Q62] 分组占比
来源：http://ets.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fno.nanxinkj.top

[Q63] 开启事务
来源：http://ipc.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://joy.meibo888.top

[Q64] 提交事务
来源：http://gvm.pengpengdd.cyou

COMMIT;
来源：http://tdq.yj20258.top

[Q65] 回滚事务
来源：http://lsl.yueranfly.top

ROLLBACK;
来源：http://iug.yfazqb.com

[Q66] 行锁查询
来源：http://jby.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cru.fehbvm.com

[Q67] 设置隔离级别
来源：http://lez.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jta.jqgfzy.top

[Q68] 保存点
来源：http://eic.zdqjudy.top

SAVEPOINT sp1;
来源：http://nsq.cheryme.top

ROLLBACK TO sp1;
来源：http://adp.kuanghao11.cn

[Q69] 查看执行计划
来源：http://btk.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fau.smart0.xyz

[Q70] 更新统计信息
来源：http://nvs.vehdjk.com

ANALYZE TABLE users;
来源：http://zvc.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://olt.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://urn.svipenyu.cn

[Q72] 查看索引
来源：http://vpc.tian-w.cn

SHOW INDEX FROM users;
来源：http://ret.jqgfzy.top

[Q73] 查看表状态
来源：http://vcp.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://oca.ybcxt.top

[Q74] 强制使用索引
来源：http://gxf.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yxx.cheryme.top

[Q75] 日期格式化
来源：http://ekc.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://utk.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xiy.hysaishi.cn

[Q76] 按天统计
来源：http://zru.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://new.andypj.xyz

[Q77] 时间加减
来源：http://bob.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tyx.gaohongyu789.top

[Q78] 当前时间
来源：http://ycx.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ydo.jianghu66.top

[Q79] 字符串拼接
来源：http://isp.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://prw.hywenlv.cn

[Q80] 字符串截取
来源：http://vrl.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zmd.zycfv.cn

[Q81] 字符串替换
来源：http://xhs.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivw.meibo888.top

[Q82] 字符长度与字节长度
来源：http://pgx.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ynv.hnxiangtu.top

[Q83] 大小写转换
来源：http://blg.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rzb.xylfe.cn

[Q84] 去除首尾空格
来源：http://wlb.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://zkr.zhoulong.xyz

[Q85] 数值取整
来源：http://ihk.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gde.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://umr.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uyd.sweek.top

[Q87] JSON 字段做条件
来源：http://ylu.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://act.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://ngg.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xum.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://akm.jqgfzy.top

[Q89] 判断表是否存在
来源：http://zpx.ppjwa.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cgl.redwolf501.top

[Q90] 生成序号列
来源：http://jkk.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jvp.ydjk.org.cn

================================================================================
来源：http://dxi.wangdashe.top

R. Bash 专题
来源：http://itg.jqgufenzy.top

================================================================================
来源：http://khn.tianlin.xyz

[R01] shebang 与严格模式
来源：http://qfg.dianchejie.cn

#!/usr/bin/env bash
来源：http://mzs.havefunace.top

set -euo pipefail
来源：http://ypb.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://xjv.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://atx.zdbjq.cn

[R03] 只读变量
来源：http://yfr.xinyue.icu

readonly PI=3.14
来源：http://jwf.xziqi.cn

[R04] 位置参数
来源：http://bih.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://api.dianchejie.cn

[R05] 参数默认值
来源：http://loo.ydzc1.top

name="${1:-default}"
来源：http://rxf.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://myh.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mzb.sysykeji.top

[R07] if 判断文件
来源：http://oxa.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://joj.chenjidiqi.icu

[R08] 数值比较
来源：http://mzu.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fxw.jyoumei.cn

[R09] 字符串比较
来源：http://ewb.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xfs.jqgufenzy.top

[R10] 正则匹配
来源：http://nkq.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cjd.feifeiyinyue.top

[R11] case 多分支
来源：http://lwc.cdnleiting.top

case "$1" in
来源：http://mjr.yj20258.top

start) echo "启动" ;;
来源：http://cwg.fktsv.cn

stop)  echo "停止" ;;
来源：http://mdw.jianghu66.top

*)     echo "未知命令" ;;
来源：http://tft.zhengqikj.top

esac
来源：http://qtz.hongshengwenyu.top

[R12] for 遍历文件
来源：http://kqh.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://rwu.jqgufenzy.top

[R13] for 计数循环
来源：http://mcz.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://sfk.fehbvm.com

[R14] C 风格 for
来源：http://mts.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kks.zhoulong.xyz

[R15] while 逐行读文件
来源：http://zwy.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aju.pycfn.com

[R16] until 等待条件
来源：http://dei.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://euh.zhengqikj.top

[R17] 数组定义与取值
来源：http://yvq.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://qdf.aibaodan.cn

[R18] 遍历数组
来源：http://usr.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qmx.gaohongyu789.top

[R19] 数组长度
来源：http://btd.dianchejie.cn

echo "${#arr[@]}"
来源：http://bov.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://sif.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://twa.chenjidiqi.icu

[R21] 字符串长度
来源：http://mcg.ybcxt.top

echo "${#s}"
来源：http://lak.meibo888.top

[R22] 截取子串
来源：http://neh.quarkkingdee.top

echo "${s:0:5}"
来源：http://poh.dianchejie.cn

[R23] 字符串替换
来源：http://tyn.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rfo.xuanzx.com

[R24] 大小写转换
来源：http://rxy.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://rjy.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://yhe.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://upd.quarkkingdee.top

[R26] 命令替换
来源：http://iet.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://erb.yfazqb.com

[R27] 算术展开
来源：http://hgu.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://vrz.guowangkeji.top

[R28] 浮点运算
来源：http://vho.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://puv.0kj1m.cn

[R29] 定义函数
来源：http://rme.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wsa.yj20258.top

[R30] 函数返回状态码
来源：http://tou.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://fjw.jlsjyb.cn

[R31] 局部变量
来源：http://gos.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://fwr.chenzaomai.com

[R32] 参数个数校验
来源：http://wlr.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fot.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://gyi.ybcxt.top


<!-- 参考信息 -->