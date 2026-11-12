代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ikv.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fdy.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ryl.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://xik.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zzf.zhengqikj.top

TS:   if (x == null) {}
来源：http://wsh.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hoh.ybcxt.top

Go:   if x == nil {}
来源：http://tdx.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sgw.sufxvd.cn

C#:   if (x is null) {}
来源：http://vkk.andypj.xyz

[P07] 防抖与节流
来源：http://vjh.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://awe.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://slu.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oap.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcr.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ivo.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://odm.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vco.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zfp.yj20258888.top

[P08] 处理浮点精度问题
来源：http://jfi.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wph.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://epa.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ozq.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pjv.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ufs.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yhv.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oyx.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cpn.zhaomingkeji.xyz

================================================================================
来源：http://cvo.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wpr.zhijiandao.cn

================================================================================
来源：http://vkk.nwbrower.top

[Q01] 创建表
来源：http://mys.9152youxi.cn

CREATE TABLE users (
来源：http://rnf.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xng.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://aka.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://zew.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bku.jqgufenzy.top

);
来源：http://iiu.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://ozz.zhoulong.xyz

CREATE TABLE orders (
来源：http://etu.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://adb.xinyue.icu

user_id INT NOT NULL,
来源：http://xys.yj20258888.top

amount DECIMAL(10, 2),
来源：http://jim.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tnn.sufxvd.cn

);
来源：http://oza.feifeiyinyue.top

[Q03] 增加列
来源：http://ocl.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://raw.nanxuanxn.top

[Q04] 修改列类型
来源：http://rkk.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lkp.bjfxy.top

[Q05] 重命名列
来源：http://mqb.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kmn.tarul.cn

[Q06] 删除列
来源：http://jnl.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://wkf.redwolf501.top

[Q07] 删除表
来源：http://xqn.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://dmt.hfpthk.cn

[Q08] 创建普通索引
来源：http://fcu.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://lzb.xinyue.icu

[Q09] 创建唯一索引
来源：http://icd.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nba.ivvv.top

[Q10] 插入单行
来源：http://pvz.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fnw.yfazqb.com

[Q11] 一次插入多行
来源：http://rzx.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzx.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://mkb.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://oxu.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pab.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://iru.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eit.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://woz.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ztl.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://liq.zycfv.cn

[Q15] 查询全部
来源：http://zsx.nanxinkj.top

SELECT * FROM users;
来源：http://pjb.vehdjk.com

[Q16] 查询指定列
来源：http://dtx.bbcook.cn

SELECT id, name FROM users;
来源：http://noc.snrcjt.cn

[Q17] 条件查询
来源：http://iwm.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vgg.hnqzz.top

[Q18] 模糊匹配
来源：http://tpb.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bxs.hywenlv.cn

[Q19] 范围查询
来源：http://jir.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hdq.jlsjyb.cn

[Q20] IN 列表
来源：http://thd.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yab.cdnleiting.top

[Q21] 空值判断
来源：http://dom.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mui.shanyushiyangkeji.top

[Q22] 排序
来源：http://zze.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://btz.sxryk.cn

[Q23] 分页
来源：http://ctr.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zrg.smart0.xyz

[Q24] 去重
来源：http://isg.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://ypk.shuidangran.top

[Q25] 只取前 N 条
来源：http://oxt.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdt.fengsongda.top

[Q26] 计数
来源：http://lng.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://kna.hammf.cn

[Q27] 条件计数
来源：http://uiu.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tii.hfpthk.cn

[Q28] 求和与平均
来源：http://slq.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yil.redwolf501.top

[Q29] 最大最小值
来源：http://abc.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://waa.c1oappe.top

[Q30] 分组统计
来源：http://snl.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gjw.andypj.xyz

[Q31] 分组后过滤
来源：http://ucs.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fsc.daxiang520.top

[Q32] 分组拼接字符串
来源：http://kjc.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://faw.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yhj.vqdsnc.cn

[Q33] 多列分组
来源：http://uwe.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://thl.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://xer.wangdashe.top

SELECT * FROM (
来源：http://xhj.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xwk.cucudq.cn

) t WHERE rn = 1;
来源：http://txr.dashuyun.cn

[Q35] 内连接
来源：http://luw.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://txh.jinyuanbaomall.cn

[Q36] 左连接
来源：http://mcp.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ovl.yueranfly.top

[Q37] 右连接
来源：http://uwk.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zmb.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oum.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lqd.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://bbe.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aab.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iwg.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dhu.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vkm.nwbrower.top

[Q41] 多表连接
来源：http://mtj.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qrb.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://tic.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://qww.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://iut.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://whc.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qia.gzhubu.top

[Q43] 标量子查询
来源：http://msz.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gmu.hnqzz.top

[Q44] IN 子查询
来源：http://iqh.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ytu.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://ccd.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kaj.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qer.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://txp.yongpay.top

[Q47] 与平均值比较
来源：http://vfw.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jwo.pycfn.com

[Q48] CTE 公用表表达式
来源：http://dzs.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://edb.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://cfo.gotoacloud.top

[Q49] 更新单行
来源：http://bgm.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uzc.shangyingyoupin.top

[Q50] 批量更新
来源：http://emg.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://got.xinyue.icu

[Q51] 用子查询更新
来源：http://bji.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpg.feifeiyinyue.top

[Q52] 删除指定行
来源：http://jnq.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://lou.nwbrower.top

[Q53] 按条件删除
来源：http://ijp.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bef.redwolf501.top

[Q54] 清空表
来源：http://zsz.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://ydg.sysykeji.top

[Q55] 排名（并列占位）
来源：http://qni.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vmy.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://zyy.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://apq.yangfankeji.com

[Q57] 行号
来源：http://xcl.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qvd.xziqi.cn

[Q58] 累计求和
来源：http://waq.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aua.hfpthk.cn

[Q59] 分组内累计
来源：http://pvf.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fza.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://ynh.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fmb.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvw.shuidangran.top

[Q61] 移动平均
来源：http://ygg.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pps.fehbvm.com

[Q62] 分组占比
来源：http://hur.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sbv.sweek.top

[Q63] 开启事务
来源：http://das.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://wwb.hcnkem.com

[Q64] 提交事务
来源：http://scy.bbcook.cn

COMMIT;
来源：http://oga.ydjk.org.cn

[Q65] 回滚事务
来源：http://vbe.sxryk.cn

ROLLBACK;
来源：http://aqb.gotoacloud.top

[Q66] 行锁查询
来源：http://tgn.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kwj.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://kqf.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://avm.jinqigfzy.top

[Q68] 保存点
来源：http://jjp.zycfv.cn

SAVEPOINT sp1;
来源：http://zqm.hywenlv.cn

ROLLBACK TO sp1;
来源：http://gdl.yangfankeji.com

[Q69] 查看执行计划
来源：http://jno.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uol.shzxlz.cn

[Q70] 更新统计信息
来源：http://utb.xuanzx.com

ANALYZE TABLE users;
来源：http://cny.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://cxg.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://agf.fanxiaobao.xyz

[Q72] 查看索引
来源：http://iwh.ybcxt.top

SHOW INDEX FROM users;
来源：http://zmr.zhoulong.xyz

[Q73] 查看表状态
来源：http://lvf.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lnk.kuanghao11.cn

[Q74] 强制使用索引
来源：http://dxj.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kym.wangshuangyany.cn

[Q75] 日期格式化
来源：http://clr.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tou.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oxb.yj20258.top

[Q76] 按天统计
来源：http://bkj.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xay.bjfxy.top

[Q77] 时间加减
来源：http://pcg.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lyz.zhixingplan.top

[Q78] 当前时间
来源：http://tmi.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wqz.jlsjyb.cn

[Q79] 字符串拼接
来源：http://wqf.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wyz.hesvh.cn

[Q80] 字符串截取
来源：http://lhu.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ddk.52xcode.cn

[Q81] 字符串替换
来源：http://lgf.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fcd.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://dom.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lnx.hongshengwenyu.top

[Q83] 大小写转换
来源：http://gls.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://esr.fzhhl.top

[Q84] 去除首尾空格
来源：http://pra.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://bim.pengpengdd.cyou

[Q85] 数值取整
来源：http://abh.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uxj.cheryme.top

[Q86] 读取 JSON 字段
来源：http://cwk.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jlb.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://bhf.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pgc.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://vpw.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pfg.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rkr.zdqjudy.top

[Q89] 判断表是否存在
来源：http://qua.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yma.birdmap.top

[Q90] 生成序号列
来源：http://fny.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fcf.fanxiaobao.xyz

================================================================================
来源：http://wgy.xuanzx.com

R. Bash 专题
来源：http://wgk.zhengqikj.top

================================================================================
来源：http://kzj.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://trn.smart0.xyz

#!/usr/bin/env bash
来源：http://dqc.hysaishi.cn

set -euo pipefail
来源：http://vnw.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://vjq.aizwys.cn

name="Tom"; echo "$name"
来源：http://ggr.mhx1999.top

[R03] 只读变量
来源：http://wkh.yanxiufei.cn

readonly PI=3.14
来源：http://nsp.guannengcc.top

[R04] 位置参数
来源：http://pbw.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hms.andypj.xyz

[R05] 参数默认值
来源：http://tbf.jinyuanbaomall.cn

name="${1:-default}"
来源：http://pst.yuanzhike.top

[R06] 判断命令是否存在
来源：http://gtc.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lzz.shuidangran.top

[R07] if 判断文件
来源：http://ekr.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hto.kuanghao11.cn

[R08] 数值比较
来源：http://ffh.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uhh.yfazqb.com

[R09] 字符串比较
来源：http://myz.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vap.redwolf501.top

[R10] 正则匹配
来源：http://nhd.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pcj.chenzaomai.com

[R11] case 多分支
来源：http://ypb.xingfuxueyuan.xyz

case "$1" in
来源：http://yiv.iojbl.cn

start) echo "启动" ;;
来源：http://qsg.zdqjudy.top

stop)  echo "停止" ;;
来源：http://pxy.yvedp.cn

*)     echo "未知命令" ;;
来源：http://amu.zhaomingkeji.xyz

esac
来源：http://cdc.tanke756.top

[R12] for 遍历文件
来源：http://yke.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://ygz.zdqjudy.top

[R13] for 计数循环
来源：http://kfq.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://bbf.zhixingplan.top

[R14] C 风格 for
来源：http://ppw.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kmr.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://ren.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lpg.zhongyouzk.top

[R16] until 等待条件
来源：http://iqf.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://spc.jinqigufen.top

[R17] 数组定义与取值
来源：http://tlx.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://szy.gaohongyu789.top

[R18] 遍历数组
来源：http://avl.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yss.hesvh.cn

[R19] 数组长度
来源：http://gpd.chenzaomai.com

echo "${#arr[@]}"
来源：http://psx.epnwcf.com

[R20] 关联数组（字典）
来源：http://ldf.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://klh.chenjidiqi.icu

[R21] 字符串长度
来源：http://nuk.316326.xyz

echo "${#s}"
来源：http://rdz.hfpthk.cn

[R22] 截取子串
来源：http://oby.zycfv.cn

echo "${s:0:5}"
来源：http://jvj.316326.xyz

[R23] 字符串替换
来源：http://che.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xkp.yuxming.cn

[R24] 大小写转换
来源：http://zpq.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tnc.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://tar.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yag.shanyushiyangtech.top

[R26] 命令替换
来源：http://xvw.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://idm.zhijiandao.cn

[R27] 算术展开
来源：http://rpb.yueranfly.top

echo $((1 + 2 * 3))
来源：http://pkk.jinqigfzy.top

[R28] 浮点运算
来源：http://hct.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://dsh.jqgfzy.top

[R29] 定义函数
来源：http://bqv.52xcode.cn


<!-- 参考信息 -->