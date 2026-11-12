代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xgu.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://gio.jqgfzy.top

[P07] 防抖与节流
来源：http://pak.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://std.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://vnu.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzu.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdf.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://knf.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ska.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rpv.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cnm.fengsongda.top

[P08] 处理浮点精度问题
来源：http://gzm.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xae.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ymy.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pir.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nmz.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aog.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cwk.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sop.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lyd.hammf.cn

================================================================================
来源：http://uow.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eux.xingfuxueyuan.xyz

================================================================================
来源：http://bvz.pycfn.com

[Q01] 创建表
来源：http://jfm.kuanghao11.cn

CREATE TABLE users (
来源：http://ctw.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xkh.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://kph.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://wri.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ypx.ctjpmb.com

);
来源：http://awl.xuanzx.com

[Q02] 创建带外键的表
来源：http://aed.vehdjk.com

CREATE TABLE orders (
来源：http://lxx.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vmw.vqdsnc.cn

user_id INT NOT NULL,
来源：http://uds.jianghu66.top

amount DECIMAL(10, 2),
来源：http://khg.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qwy.fengsongda.top

);
来源：http://hgn.vqdsnc.cn

[Q03] 增加列
来源：http://lag.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://goy.shangyingyoupin.top

[Q04] 修改列类型
来源：http://oks.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://inj.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://yob.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://grl.yongpay.top

[Q06] 删除列
来源：http://ssv.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://neq.yanxiufei.cn

[Q07] 删除表
来源：http://aaa.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://dwd.fengsongda.top

[Q08] 创建普通索引
来源：http://lxi.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hou.yueranfly.top

[Q09] 创建唯一索引
来源：http://qvz.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hxg.jqgufenzy.top

[Q10] 插入单行
来源：http://jvm.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://peh.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://bvd.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ewy.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://hri.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://idi.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yyl.yj20258.top

[Q13] 忽略重复插入
来源：http://fnd.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://frj.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://qxx.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgz.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rrp.jlsjyb.cn

[Q15] 查询全部
来源：http://zih.shuidangran.top

SELECT * FROM users;
来源：http://wvm.wangdashe.top

[Q16] 查询指定列
来源：http://jww.nwbrower.top

SELECT id, name FROM users;
来源：http://ter.jinqigufen.top

[Q17] 条件查询
来源：http://aoi.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://txo.chenzaomai.com

[Q18] 模糊匹配
来源：http://oxs.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://det.mhx1999.top

[Q19] 范围查询
来源：http://tzg.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ijt.guowangkeji.top

[Q20] IN 列表
来源：http://vcm.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pug.fktsv.cn

[Q21] 空值判断
来源：http://ozc.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mft.snrcjt.cn

[Q22] 排序
来源：http://tlt.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eau.nwbrower.top

[Q23] 分页
来源：http://kry.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ufh.vehdjk.com

[Q24] 去重
来源：http://qbh.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://xje.jinqigufen.top

[Q25] 只取前 N 条
来源：http://sjg.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ezp.jiagoushi.top

[Q26] 计数
来源：http://rmf.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://edi.zdbjq.cn

[Q27] 条件计数
来源：http://uqx.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jke.chenjidiqi.icu

[Q28] 求和与平均
来源：http://dfh.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sos.meibo888.top

[Q29] 最大最小值
来源：http://ldg.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pyh.0kj1m.cn

[Q30] 分组统计
来源：http://kgt.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ixg.zhoulong.xyz

[Q31] 分组后过滤
来源：http://ftn.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvk.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://bqj.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lxj.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hso.sjlbkw.cn

[Q33] 多列分组
来源：http://qum.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://awi.dashuyun.cn

[Q34] 每组取第一条
来源：http://yng.jiagoushi.top

SELECT * FROM (
来源：http://dio.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wbd.zhoulong.xyz

) t WHERE rn = 1;
来源：http://ury.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://wvr.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hbw.yongpay.top

[Q36] 左连接
来源：http://gii.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wan.nanxuanxn.top

[Q37] 右连接
来源：http://ecb.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ani.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jpm.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jsf.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://bct.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fjv.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://val.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jli.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rrk.nwbrower.top

[Q41] 多表连接
来源：http://iiy.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lzg.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://nsi.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://tnv.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://fxu.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://gyn.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ftp.andypj.xyz

[Q43] 标量子查询
来源：http://avc.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yjk.zhixingplan.top

[Q44] IN 子查询
来源：http://txg.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lcb.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://seu.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgk.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://wgs.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gev.zdbjq.cn

[Q47] 与平均值比较
来源：http://qou.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qdd.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://bwq.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fre.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://iwu.tian-w.cn

[Q49] 更新单行
来源：http://eak.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gve.andypj.xyz

[Q50] 批量更新
来源：http://lyo.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://weu.ivvv.top

[Q51] 用子查询更新
来源：http://tsg.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rbt.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://ecr.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://ecu.yuxming.cn

[Q53] 按条件删除
来源：http://osc.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fxn.daxiang520.top

[Q54] 清空表
来源：http://okm.yfazqb.com

TRUNCATE TABLE logs;
来源：http://tbm.ydzc1.top

[Q55] 排名（并列占位）
来源：http://zeg.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eaf.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://nea.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sth.zdbjq.cn

[Q57] 行号
来源：http://lpe.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qjq.meibo888.top

[Q58] 累计求和
来源：http://xux.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kvw.xuanzx.com

[Q59] 分组内累计
来源：http://tlu.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dcw.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://dmd.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xse.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nwi.guowangkeji.top

[Q61] 移动平均
来源：http://bkh.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xsa.iojbl.cn

[Q62] 分组占比
来源：http://hhw.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://itz.0kj1m.cn

[Q63] 开启事务
来源：http://evr.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wlo.cheryme.top

[Q64] 提交事务
来源：http://muf.wangshuangyany.cn

COMMIT;
来源：http://ipg.shangyingyoupin.top

[Q65] 回滚事务
来源：http://sfu.yanxiufei.cn

ROLLBACK;
来源：http://qqp.zdqjudy.top

[Q66] 行锁查询
来源：http://gxq.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://onu.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://jjz.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bzl.jinqigufen.top

[Q68] 保存点
来源：http://apw.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://aat.guowangkeji.top

ROLLBACK TO sp1;
来源：http://jub.guannengcc.top

[Q69] 查看执行计划
来源：http://xyh.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uzi.jqgufenzy.top

[Q70] 更新统计信息
来源：http://fht.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://fqd.iojbl.cn

[Q71] 查看建表语句
来源：http://rpk.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zpu.sufxvd.cn

[Q72] 查看索引
来源：http://unn.jiagoushi.top

SHOW INDEX FROM users;
来源：http://ydp.kuanghao11.cn

[Q73] 查看表状态
来源：http://zvm.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ssh.redwolf501.top

[Q74] 强制使用索引
来源：http://quy.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yuh.dashuyun.cn

[Q75] 日期格式化
来源：http://ttt.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ebn.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://swz.xuetiantiany.cn

[Q76] 按天统计
来源：http://rog.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ids.hesvh.cn

[Q77] 时间加减
来源：http://jff.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mho.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://vze.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bqr.svipenyu.cn

[Q79] 字符串拼接
来源：http://hnj.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ooh.cdnleiting.top

[Q80] 字符串截取
来源：http://zqq.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kwx.jiagoushi.top

[Q81] 字符串替换
来源：http://hjm.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qoi.yj20258.top

[Q82] 字符长度与字节长度
来源：http://nnh.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ltj.hnqzz.top

[Q83] 大小写转换
来源：http://sxt.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bct.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://xck.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://fwe.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://ntp.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyp.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://coa.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gvq.jianghu66.top

[Q87] JSON 字段做条件
来源：http://fms.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xkn.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://fya.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pgc.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jmv.fengsongda.top

[Q89] 判断表是否存在
来源：http://fue.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tye.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://bdu.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bxw.dashuyun.cn

================================================================================
来源：http://ohe.chenjidiqi.icu

R. Bash 专题
来源：http://uhg.gaohongyu789.top

================================================================================
来源：http://vks.tarul.cn

[R01] shebang 与严格模式
来源：http://ltx.bbcook.cn

#!/usr/bin/env bash
来源：http://wmq.hnqzz.top

set -euo pipefail
来源：http://vdh.havefunace.top

[R02] 变量赋值与使用
来源：http://eer.gogol.net.cn

name="Tom"; echo "$name"
来源：http://zlr.shanyushiyangkeji.top

[R03] 只读变量
来源：http://ogc.cqqwz.cn

readonly PI=3.14
来源：http://yze.sufxvd.cn

[R04] 位置参数
来源：http://mes.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vgx.gaohongyu789.top

[R05] 参数默认值
来源：http://bup.jinghuilouyu.cn

name="${1:-default}"
来源：http://kfa.cucudq.cn

[R06] 判断命令是否存在
来源：http://und.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cqb.shuidangran.top

[R07] if 判断文件
来源：http://bkz.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yne.jinqigufen.top

[R08] 数值比较
来源：http://boi.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oyb.hfpthk.cn

[R09] 字符串比较
来源：http://aex.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://slr.jqgfzy.top

[R10] 正则匹配
来源：http://jus.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ztn.hywenlv.cn

[R11] case 多分支
来源：http://tij.zhaomingkeji.xyz

case "$1" in
来源：http://axm.fehbvm.com

start) echo "启动" ;;
来源：http://tfp.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://jxy.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://zqe.iojbl.cn

esac
来源：http://mil.zycfv.cn

[R12] for 遍历文件
来源：http://wry.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://kdz.zdqjudy.top

[R13] for 计数循环
来源：http://dey.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://hei.uphjek.com

[R14] C 风格 for
来源：http://gxt.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aaw.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://dzq.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jec.zhoulong.xyz

[R16] until 等待条件
来源：http://xlm.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://buv.sysykeji.top

[R17] 数组定义与取值
来源：http://vuk.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://fpc.birdmap.top

[R18] 遍历数组
来源：http://pkw.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ako.tianlin.xyz

[R19] 数组长度
来源：http://jla.chenzaomai.com

echo "${#arr[@]}"
来源：http://crw.hammf.cn

[R20] 关联数组（字典）
来源：http://kcy.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://asb.hywenlv.cn

[R21] 字符串长度
来源：http://ctx.xylfe.cn

echo "${#s}"
来源：http://rcj.sysykeji.top

[R22] 截取子串
来源：http://jyi.jinqigufen.top

echo "${s:0:5}"
来源：http://vnf.ybcxt.top

[R23] 字符串替换
来源：http://qyl.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kof.hcnkem.com

[R24] 大小写转换
来源：http://fvq.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqi.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://pur.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lxz.vqdsnc.cn

[R26] 命令替换
来源：http://bml.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://lqp.sufxvd.cn

[R27] 算术展开
来源：http://hdl.yuxming.cn

echo $((1 + 2 * 3))
来源：http://sbs.sjlbkw.cn

[R28] 浮点运算
来源：http://thk.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://vrk.shangyingyoupin.top

[R29] 定义函数
来源：http://zak.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xjv.cucudq.cn

[R30] 函数返回状态码
来源：http://eqm.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://isp.sysykeji.top

[R31] 局部变量
来源：http://aip.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://thd.dianchejie.cn

[R32] 参数个数校验
来源：http://zzg.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lcu.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://zum.snrcjt.cn


<!-- 参考信息 -->