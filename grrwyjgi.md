代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ndd.52xcode.cn

C#:   if (x is null) {}
来源：http://xkl.ppjwa.cn

[P07] 防抖与节流
来源：http://bjy.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dab.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://zem.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nce.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://goh.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qxb.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wyr.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hpr.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oss.andypj.xyz

[P08] 处理浮点精度问题
来源：http://raw.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bdu.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dps.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oyc.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hcc.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xpe.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://agn.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqf.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qtw.sysykeji.top

================================================================================
来源：http://riu.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://shz.fanxiaobao.xyz

================================================================================
来源：http://pqr.hesvh.cn

[Q01] 创建表
来源：http://hqi.shangyingyoupin.top

CREATE TABLE users (
来源：http://zun.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jcq.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://anc.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://bpv.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ipu.gaohongyu789.top

);
来源：http://grf.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://bms.nanxinkj.top

CREATE TABLE orders (
来源：http://mec.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://doi.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://gay.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://zvp.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://neq.guowangkeji.top

);
来源：http://tdt.yvedp.cn

[Q03] 增加列
来源：http://ehr.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kud.nanxuanxn.top

[Q04] 修改列类型
来源：http://vjo.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jtg.dashuyun.cn

[Q05] 重命名列
来源：http://hoy.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://llr.guannengcc.top

[Q06] 删除列
来源：http://tqu.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pmp.gotoacloud.top

[Q07] 删除表
来源：http://xyw.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ruo.hysaishi.cn

[Q08] 创建普通索引
来源：http://gct.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gyk.andypj.xyz

[Q09] 创建唯一索引
来源：http://ehj.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yko.sxryk.cn

[Q10] 插入单行
来源：http://axp.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vpc.hywenlv.cn

[Q11] 一次插入多行
来源：http://pxb.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kxv.yongpay.top

[Q12] 插入后取自增 ID
来源：http://sne.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kzg.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://toa.epnwcf.com

[Q13] 忽略重复插入
来源：http://hal.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xbz.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://djp.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wgd.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vcb.52xcode.cn

[Q15] 查询全部
来源：http://nwa.yj20258.top

SELECT * FROM users;
来源：http://sqn.zdbjq.cn

[Q16] 查询指定列
来源：http://cgs.kuanghao11.cn

SELECT id, name FROM users;
来源：http://mji.fanxiaobao.xyz

[Q17] 条件查询
来源：http://avn.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ptu.ehwqpu.com

[Q18] 模糊匹配
来源：http://kbq.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uij.snrcjt.cn

[Q19] 范围查询
来源：http://yfq.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bme.birdmap.top

[Q20] IN 列表
来源：http://vzq.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uun.ydzc1.top

[Q21] 空值判断
来源：http://aqb.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qrk.xingfuxueyuan.xyz

[Q22] 排序
来源：http://qav.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dlt.xziqi.cn

[Q23] 分页
来源：http://gob.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ukc.guowangkeji.top

[Q24] 去重
来源：http://hci.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://zdr.jyoumei.cn

[Q25] 只取前 N 条
来源：http://hhi.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xmr.fengsongda.top

[Q26] 计数
来源：http://fuz.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://rdw.shanyushiyangtech.top

[Q27] 条件计数
来源：http://jsy.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yvx.zhiwuduotai.top

[Q28] 求和与平均
来源：http://osd.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rgx.zdqjudy.top

[Q29] 最大最小值
来源：http://fhr.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://vnc.hnqzz.top

[Q30] 分组统计
来源：http://uic.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://thc.yangfankeji.com

[Q31] 分组后过滤
来源：http://rqm.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://evh.jianghu66.top

[Q32] 分组拼接字符串
来源：http://wau.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fkk.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hms.ydzc1.top

[Q33] 多列分组
来源：http://uqc.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://adm.fehbvm.com

[Q34] 每组取第一条
来源：http://tty.meibo888.top

SELECT * FROM (
来源：http://rnq.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://knj.9152youxi.cn

) t WHERE rn = 1;
来源：http://mxe.pycfn.com

[Q35] 内连接
来源：http://nav.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tym.bbcook.cn

[Q36] 左连接
来源：http://hby.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hwp.iojbl.cn

[Q37] 右连接
来源：http://bsc.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://frq.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://omx.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vvu.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://idd.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bna.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://itg.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://avv.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lvq.sufxvd.cn

[Q41] 多表连接
来源：http://cdz.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nks.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://mkn.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://kto.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://cxb.birdmap.top

SELECT u.name, o.amount FROM users u
来源：http://dqo.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uig.tanke756.top

[Q43] 标量子查询
来源：http://jwt.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cey.ppjwa.cn

[Q44] IN 子查询
来源：http://epx.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jlz.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://bvk.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fcd.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://hun.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ldo.hywenlv.cn

[Q47] 与平均值比较
来源：http://igr.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wxe.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://gij.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://enp.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://oyd.gogol.net.cn

[Q49] 更新单行
来源：http://rnc.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gct.jyoumei.cn

[Q50] 批量更新
来源：http://pop.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xix.tanke756.top

[Q51] 用子查询更新
来源：http://cdj.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tlh.zhiwuduotai.top

[Q52] 删除指定行
来源：http://ssd.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://evq.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://agd.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qlx.xylfe.cn

[Q54] 清空表
来源：http://lwv.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://vli.shuidangran.top

[Q55] 排名（并列占位）
来源：http://mbd.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jhv.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://qnb.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wie.xuanzx.com

[Q57] 行号
来源：http://vdi.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wcb.9152youxi.cn

[Q58] 累计求和
来源：http://vtm.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ijq.tian-w.cn

[Q59] 分组内累计
来源：http://qvx.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yqc.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://loe.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwi.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://shk.jqgfzy.top

[Q61] 移动平均
来源：http://qfd.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dvl.hcnkem.com

[Q62] 分组占比
来源：http://afl.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mbc.wangdashe.top

[Q63] 开启事务
来源：http://yyu.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://xbs.birdmap.top

[Q64] 提交事务
来源：http://odl.xylfe.cn

COMMIT;
来源：http://xan.havefunace.top

[Q65] 回滚事务
来源：http://xzd.tanke756.top

ROLLBACK;
来源：http://zcg.cucudq.cn

[Q66] 行锁查询
来源：http://dou.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ezt.redwolf501.top

[Q67] 设置隔离级别
来源：http://frc.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://boo.tarul.cn

[Q68] 保存点
来源：http://kio.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://wpn.fktsv.cn

ROLLBACK TO sp1;
来源：http://mwf.cheryme.top

[Q69] 查看执行计划
来源：http://nhm.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rbo.haohaochexian.top

[Q70] 更新统计信息
来源：http://kod.haohaochexian.top

ANALYZE TABLE users;
来源：http://hib.daxiang520.top

[Q71] 查看建表语句
来源：http://ffr.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ijw.52xcode.cn

[Q72] 查看索引
来源：http://vze.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://mkc.svipenyu.cn

[Q73] 查看表状态
来源：http://ewj.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fmj.cqqwz.cn

[Q74] 强制使用索引
来源：http://jwy.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cnd.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://xlq.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rca.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cac.shangyingyoupin.top

[Q76] 按天统计
来源：http://usc.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uwp.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://yuu.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xul.bjfxy.top

[Q78] 当前时间
来源：http://dga.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dal.epnwcf.com

[Q79] 字符串拼接
来源：http://umg.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qgg.jinqigfzy.top

[Q80] 字符串截取
来源：http://aet.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rsd.shzxlz.cn

[Q81] 字符串替换
来源：http://iyy.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zxv.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://ygz.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oix.shuidangran.top

[Q83] 大小写转换
来源：http://axm.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zrm.sxryk.cn

[Q84] 去除首尾空格
来源：http://oar.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://kzj.fktsv.cn

[Q85] 数值取整
来源：http://aiw.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nwu.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://rpm.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://faf.hcnkem.com

[Q87] JSON 字段做条件
来源：http://bfc.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ocf.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://vyz.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://esm.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hxv.andypj.xyz

[Q89] 判断表是否存在
来源：http://pqa.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cvs.cqqwz.cn

[Q90] 生成序号列
来源：http://dmo.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://odt.hongshengwenyu.top

================================================================================
来源：http://xtp.ydjk.org.cn

R. Bash 专题
来源：http://seg.guowangkeji.top

================================================================================
来源：http://hqy.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://lse.smart0.xyz

#!/usr/bin/env bash
来源：http://mrl.zhixingplan.top

set -euo pipefail
来源：http://lva.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://ecd.bbcook.cn

name="Tom"; echo "$name"
来源：http://ban.hongshengwenyu.top

[R03] 只读变量
来源：http://ldf.fengsongda.top

readonly PI=3.14
来源：http://hqm.yongpay.top

[R04] 位置参数
来源：http://nqr.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yat.sjlbkw.cn

[R05] 参数默认值
来源：http://jmv.hnqzz.top

name="${1:-default}"
来源：http://lqp.dianchejie.cn

[R06] 判断命令是否存在
来源：http://dyf.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yls.nanxinkj.top

[R07] if 判断文件
来源：http://xzu.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dii.316326.xyz

[R08] 数值比较
来源：http://egh.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ebp.birdmap.top

[R09] 字符串比较
来源：http://pie.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xok.yuanzhike.top

[R10] 正则匹配
来源：http://srp.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kss.zycfv.cn

[R11] case 多分支
来源：http://psa.fzhhl.top

case "$1" in
来源：http://upy.yueranfly.top

start) echo "启动" ;;
来源：http://usl.yj202588.top

stop)  echo "停止" ;;
来源：http://wqk.ydzc1.top

*)     echo "未知命令" ;;
来源：http://tzi.xylfe.cn

esac
来源：http://xrv.epnwcf.com

[R12] for 遍历文件
来源：http://lyc.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://hhd.hongshengwenyu.top

[R13] for 计数循环
来源：http://voc.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://awi.iojbl.cn

[R14] C 风格 for
来源：http://vvq.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://inx.shuidangran.top

[R15] while 逐行读文件
来源：http://bxv.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ydl.yonumen.top

[R16] until 等待条件
来源：http://cdf.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bnq.yueranfly.top

[R17] 数组定义与取值
来源：http://sop.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ahw.sufxvd.cn

[R18] 遍历数组
来源：http://sec.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ejk.meibo888.top

[R19] 数组长度
来源：http://pdn.yangfankeji.com

echo "${#arr[@]}"
来源：http://bjp.cashguo.top

[R20] 关联数组（字典）
来源：http://jug.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://red.yj202588.top

[R21] 字符串长度
来源：http://rka.tarul.cn

echo "${#s}"
来源：http://bkh.vqdsnc.cn

[R22] 截取子串
来源：http://ser.epnwcf.com

echo "${s:0:5}"
来源：http://yaj.316326.xyz

[R23] 字符串替换
来源：http://ies.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tjy.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://zev.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://jzj.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://qjg.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wqw.fengsongda.top

[R26] 命令替换
来源：http://hxw.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://jsj.quarkkingdee.top

[R27] 算术展开
来源：http://ltz.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://jzv.0kj1m.cn

[R28] 浮点运算
来源：http://esr.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://kzr.zhixingplan.top

[R29] 定义函数
来源：http://oyd.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ile.xinyue.icu

[R30] 函数返回状态码
来源：http://ksc.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://omg.ppjwa.cn

[R31] 局部变量
来源：http://eod.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://dop.zhixingplan.top

[R32] 参数个数校验
来源：http://lqa.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://typ.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://owa.jiagoushi.top


<!-- 参考信息 -->