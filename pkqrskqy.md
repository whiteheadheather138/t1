代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://may.ybcxt.top

C#:   if (x is null) {}
来源：http://yle.yanxiufei.cn

[P07] 防抖与节流
来源：http://upd.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ofq.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://xnx.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eox.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjg.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wuf.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://spx.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bkm.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gdo.ydzc1.top

[P08] 处理浮点精度问题
来源：http://qfe.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dwh.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnw.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sij.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fql.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utd.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dxk.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cvo.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cpg.chenlongwang.top

================================================================================
来源：http://uud.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vco.tarul.cn

================================================================================
来源：http://mmz.aibaodan.cn

[Q01] 创建表
来源：http://lbl.hnxiangtu.top

CREATE TABLE users (
来源：http://qxo.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zfq.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://rsq.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://vmp.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xqh.jiagoushi.top

);
来源：http://moh.aibaodan.cn

[Q02] 创建带外键的表
来源：http://kej.hnqzz.top

CREATE TABLE orders (
来源：http://jns.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lop.fengsongda.top

user_id INT NOT NULL,
来源：http://abe.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://vhy.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ewq.jqgfzy.top

);
来源：http://xfl.meibo888.top

[Q03] 增加列
来源：http://kbz.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://usu.jyoumei.cn

[Q04] 修改列类型
来源：http://bzb.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ljh.xziqi.cn

[Q05] 重命名列
来源：http://nwg.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kal.dianchejie.cn

[Q06] 删除列
来源：http://sln.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zaz.tarul.cn

[Q07] 删除表
来源：http://fys.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://mui.shuidangran.top

[Q08] 创建普通索引
来源：http://cms.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://qra.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://uke.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://taa.uphjek.com

[Q10] 插入单行
来源：http://wgh.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cxv.meibo888.top

[Q11] 一次插入多行
来源：http://mlt.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zyc.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://lnr.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tma.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vlv.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://hig.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://inm.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://xbu.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cvb.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nwz.pengpengdd.cyou

[Q15] 查询全部
来源：http://epw.yfazqb.com

SELECT * FROM users;
来源：http://zpe.gzhubu.top

[Q16] 查询指定列
来源：http://gsu.hammf.cn

SELECT id, name FROM users;
来源：http://lpz.fengsongda.top

[Q17] 条件查询
来源：http://nja.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://imn.gogol.net.cn

[Q18] 模糊匹配
来源：http://zyx.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tkd.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://lxl.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ydr.ivvv.top

[Q20] IN 列表
来源：http://wav.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tkt.316326.xyz

[Q21] 空值判断
来源：http://pwj.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fmi.meibo888.top

[Q22] 排序
来源：http://nsy.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cnc.shuidangran.top

[Q23] 分页
来源：http://ugw.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://diw.yangfankeji.com

[Q24] 去重
来源：http://mqp.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://eks.tian-w.cn

[Q25] 只取前 N 条
来源：http://ens.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://phc.aibaodan.cn

[Q26] 计数
来源：http://yba.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://nxr.mhx1999.top

[Q27] 条件计数
来源：http://uts.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qex.zhijiandao.cn

[Q28] 求和与平均
来源：http://znn.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nqt.feifeiyinyue.top

[Q29] 最大最小值
来源：http://xtd.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://afh.redwolf501.top

[Q30] 分组统计
来源：http://met.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zzj.tanke756.top

[Q31] 分组后过滤
来源：http://eso.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://clm.yj20258888.top

[Q32] 分组拼接字符串
来源：http://soo.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bfz.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://afw.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://dwr.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hkb.zhijiandao.cn

[Q34] 每组取第一条
来源：http://pfd.gogol.net.cn

SELECT * FROM (
来源：http://alc.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gle.sufxvd.cn

) t WHERE rn = 1;
来源：http://fzu.yuxming.cn

[Q35] 内连接
来源：http://dfd.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kcc.yvedp.cn

[Q36] 左连接
来源：http://iej.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rkb.zhengqikj.top

[Q37] 右连接
来源：http://pgj.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://huv.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://drp.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fba.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://uqx.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vwb.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ghf.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jbn.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://obm.zhengqikj.top

[Q41] 多表连接
来源：http://uvu.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xzz.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://uwg.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://kzo.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://bhw.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://uuw.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dng.ydzc1.top

[Q43] 标量子查询
来源：http://mvj.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rzk.mhx1999.top

[Q44] IN 子查询
来源：http://pmh.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tni.meibo888.top

[Q45] EXISTS 判断存在
来源：http://lmf.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://els.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://fmg.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msy.daxiang520.top

[Q47] 与平均值比较
来源：http://rgv.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vcp.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://cuj.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjh.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://nmi.iojbl.cn

[Q49] 更新单行
来源：http://tye.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ejm.yangfankeji.com

[Q50] 批量更新
来源：http://qko.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rna.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://stg.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zyw.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://ucj.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://xge.chenlongwang.top

[Q53] 按条件删除
来源：http://dkd.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nxm.pycfn.com

[Q54] 清空表
来源：http://lug.sweek.top

TRUNCATE TABLE logs;
来源：http://kmc.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://yay.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gcl.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://nno.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zqb.xuanzx.com

[Q57] 行号
来源：http://rxt.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gji.wangdashe.top

[Q58] 累计求和
来源：http://gyl.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bca.vehdjk.com

[Q59] 分组内累计
来源：http://dbz.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zlx.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://aat.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zdz.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://twk.sufxvd.cn

[Q61] 移动平均
来源：http://afk.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ajh.hesvh.cn

[Q62] 分组占比
来源：http://gnn.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qju.ydzc1.top

[Q63] 开启事务
来源：http://rva.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tdr.zhixingplan.top

[Q64] 提交事务
来源：http://nen.jianghu66.top

COMMIT;
来源：http://fvk.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://qcg.cqqwz.cn

ROLLBACK;
来源：http://hoz.fktsv.cn

[Q66] 行锁查询
来源：http://kij.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://niu.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://cbs.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://peq.shanyushiyangkeji.top

[Q68] 保存点
来源：http://zgr.ppjwa.cn

SAVEPOINT sp1;
来源：http://pin.cashguo.top

ROLLBACK TO sp1;
来源：http://ddf.cucudq.cn

[Q69] 查看执行计划
来源：http://trs.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mea.birdmap.top

[Q70] 更新统计信息
来源：http://bnq.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://zrw.vehdjk.com

[Q71] 查看建表语句
来源：http://fcj.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wcw.hongshengwenyu.top

[Q72] 查看索引
来源：http://jcb.bjfxy.top

SHOW INDEX FROM users;
来源：http://jab.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://xvv.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sed.yj20258888.top

[Q74] 强制使用索引
来源：http://hhd.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mkr.hammf.cn

[Q75] 日期格式化
来源：http://pfa.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hkj.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ndp.yvedp.cn

[Q76] 按天统计
来源：http://ftz.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zqy.xylfe.cn

[Q77] 时间加减
来源：http://wud.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kap.0kj1m.cn

[Q78] 当前时间
来源：http://qhp.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ysl.zdqjudy.top

[Q79] 字符串拼接
来源：http://naq.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ewm.yj202588.top

[Q80] 字符串截取
来源：http://ynj.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bts.jyoumei.cn

[Q81] 字符串替换
来源：http://ogc.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rcg.cashguo.top

[Q82] 字符长度与字节长度
来源：http://xwv.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ktd.ctjpmb.com

[Q83] 大小写转换
来源：http://lis.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jxa.zdqjudy.top

[Q84] 去除首尾空格
来源：http://wny.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://kuo.svipenyu.cn

[Q85] 数值取整
来源：http://qpp.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ecl.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://oyx.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vew.sysykeji.top

[Q87] JSON 字段做条件
来源：http://jly.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qku.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://oft.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hgj.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pkj.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://lzh.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rpp.wangshuangyany.cn

[Q90] 生成序号列
来源：http://usk.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bwn.sjlbkw.cn

================================================================================
来源：http://cwa.dianchejie.cn

R. Bash 专题
来源：http://seb.ydzc1.top

================================================================================
来源：http://rel.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://bwc.sweek.top

#!/usr/bin/env bash
来源：http://orm.shuidangran.top

set -euo pipefail
来源：http://xpy.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://zdm.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://yqd.zycfv.cn

[R03] 只读变量
来源：http://eea.zhoulong.xyz

readonly PI=3.14
来源：http://wuj.jinghuilouyu.cn

[R04] 位置参数
来源：http://obc.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tgk.yj20258888.top

[R05] 参数默认值
来源：http://ybd.chenzaomai.com

name="${1:-default}"
来源：http://pkm.shzxlz.cn

[R06] 判断命令是否存在
来源：http://buz.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kyh.svipenyu.cn

[R07] if 判断文件
来源：http://wex.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tor.mhx1999.top

[R08] 数值比较
来源：http://rgz.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tdh.gaohongyu789.top

[R09] 字符串比较
来源：http://hsf.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jmz.chenjidiqi.icu

[R10] 正则匹配
来源：http://mox.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vwl.c1oappe.top

[R11] case 多分支
来源：http://ttf.shangyingyoupin.top

case "$1" in
来源：http://cve.yonumen.top

start) echo "启动" ;;
来源：http://jvb.cdnleiting.top

stop)  echo "停止" ;;
来源：http://bwk.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://wag.zhongyouzk.top

esac
来源：http://czb.cucudq.cn

[R12] for 遍历文件
来源：http://xmy.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://anr.zhiwuduotai.top

[R13] for 计数循环
来源：http://cgg.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://ntv.dashuyun.cn

[R14] C 风格 for
来源：http://ajm.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlj.vqdsnc.cn

[R15] while 逐行读文件
来源：http://gsc.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mtf.ehwqpu.com

[R16] until 等待条件
来源：http://har.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uej.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://uku.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://eod.hnqzz.top

[R18] 遍历数组
来源：http://non.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wbf.yj202588.top

[R19] 数组长度
来源：http://enb.tianlin.xyz

echo "${#arr[@]}"
来源：http://bgl.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://ufz.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oal.kuanghao11.cn

[R21] 字符串长度
来源：http://xic.316326.xyz

echo "${#s}"
来源：http://pet.cqqwz.cn

[R22] 截取子串
来源：http://inr.smart0.xyz

echo "${s:0:5}"
来源：http://nvm.yongpay.top

[R23] 字符串替换
来源：http://tck.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://omy.yvedp.cn

[R24] 大小写转换
来源：http://dqf.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://bir.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://til.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bwt.xuetiantiany.cn

[R26] 命令替换
来源：http://dkx.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://ktt.bbcook.cn

[R27] 算术展开
来源：http://dwk.bbcook.cn

echo $((1 + 2 * 3))
来源：http://iva.smart0.xyz

[R28] 浮点运算
来源：http://dho.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://amv.yuanzhike.top

[R29] 定义函数
来源：http://lxk.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aal.snrcjt.cn

[R30] 函数返回状态码
来源：http://fza.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://sxq.guannengcc.top

[R31] 局部变量
来源：http://qno.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://pwy.hongshengwenyu.top

[R32] 参数个数校验
来源：http://yif.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nil.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://eag.jianghu66.top


<!-- 参考信息 -->