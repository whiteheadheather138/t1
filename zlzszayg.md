代发 wailian999

PHP:  // 手写时间戳比较
来源：http://bcs.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yav.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcq.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qno.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://shk.52xcode.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nzr.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dpz.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://nnr.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ivw.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rae.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jug.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://puy.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uqe.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zor.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fvi.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hlx.shzxlz.cn

================================================================================
来源：http://jpd.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ngl.pycfn.com

================================================================================
来源：http://ydx.ctjpmb.com

[Q01] 创建表
来源：http://iiu.hcnkem.com

CREATE TABLE users (
来源：http://qey.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://umd.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://xrb.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://dmb.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gfo.hnqzz.top

);
来源：http://uuk.yj202588.top

[Q02] 创建带外键的表
来源：http://cqc.jqgfzy.top

CREATE TABLE orders (
来源：http://tjx.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfo.yfazqb.com

user_id INT NOT NULL,
来源：http://uex.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://oih.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tqq.nanxinkj.top

);
来源：http://mti.feifeiyinyue.top

[Q03] 增加列
来源：http://gnn.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dou.yfazqb.com

[Q04] 修改列类型
来源：http://aal.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fjp.9152youxi.cn

[Q05] 重命名列
来源：http://oyg.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nuo.yuanzhike.top

[Q06] 删除列
来源：http://ess.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://dtf.yuxming.cn

[Q07] 删除表
来源：http://ilb.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://zno.zdbjq.cn

[Q08] 创建普通索引
来源：http://pnj.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://iln.tian-w.cn

[Q09] 创建唯一索引
来源：http://ogd.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hbd.aibaodan.cn

[Q10] 插入单行
来源：http://amg.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jeh.hnqzz.top

[Q11] 一次插入多行
来源：http://rpo.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xet.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://gmx.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://qjs.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vyy.ydzc1.top

[Q13] 忽略重复插入
来源：http://jbt.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jut.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://bpb.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vta.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kwj.yanxiufei.cn

[Q15] 查询全部
来源：http://yov.pengpengdd.cyou

SELECT * FROM users;
来源：http://wkx.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://xjr.tarul.cn

SELECT id, name FROM users;
来源：http://jqf.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://epz.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixa.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://olr.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ypg.cashguo.top

[Q19] 范围查询
来源：http://dpy.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mfq.cqqwz.cn

[Q20] IN 列表
来源：http://vvt.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xvc.fehbvm.com

[Q21] 空值判断
来源：http://ckc.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://trd.mhx1999.top

[Q22] 排序
来源：http://rqx.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oig.feifeiyinyue.top

[Q23] 分页
来源：http://puq.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://poy.guowangkeji.top

[Q24] 去重
来源：http://xbl.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://ler.ybcxt.top

[Q25] 只取前 N 条
来源：http://nzt.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iui.tanke756.top

[Q26] 计数
来源：http://jmc.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://zom.cucudq.cn

[Q27] 条件计数
来源：http://gdf.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpi.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://vjs.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lgo.zhijiandao.cn

[Q29] 最大最小值
来源：http://vmk.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://oep.jyoumei.cn

[Q30] 分组统计
来源：http://pis.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jmu.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://muv.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hje.yuxming.cn

[Q32] 分组拼接字符串
来源：http://fau.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kwx.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cnr.xuanzx.com

[Q33] 多列分组
来源：http://fqz.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gbg.xuanzx.com

[Q34] 每组取第一条
来源：http://hmp.fehbvm.com

SELECT * FROM (
来源：http://jlt.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lya.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://kmf.yuanzhike.top

[Q35] 内连接
来源：http://rwv.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dtu.daxiang520.top

[Q36] 左连接
来源：http://kuz.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nsq.snrcjt.cn

[Q37] 右连接
来源：http://kry.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kvd.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://tkw.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zms.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://szo.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ydd.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kpk.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://coe.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lrs.jiagoushi.top

[Q41] 多表连接
来源：http://jjo.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hov.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://dog.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://ady.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://bbh.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://wme.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jgz.chenzaomai.com

[Q43] 标量子查询
来源：http://zdk.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bhz.uphjek.com

[Q44] IN 子查询
来源：http://vtl.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ggv.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://mjm.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yes.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://enq.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hla.bbcook.cn

[Q47] 与平均值比较
来源：http://hem.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pjk.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://cko.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aqa.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://sbo.jqgfzy.top

[Q49] 更新单行
来源：http://apn.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pqz.jqgufenzy.top

[Q50] 批量更新
来源：http://lwb.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mpr.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://wmo.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://omj.ppjwa.cn

[Q52] 删除指定行
来源：http://aci.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://ubd.zhijiandao.cn

[Q53] 按条件删除
来源：http://tvw.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ynu.havefunace.top

[Q54] 清空表
来源：http://yfr.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://aqo.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://uhr.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hdq.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://rke.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tdi.bbcook.cn

[Q57] 行号
来源：http://sqn.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wuq.yongpay.top

[Q58] 累计求和
来源：http://ykv.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uhz.zdqjudy.top

[Q59] 分组内累计
来源：http://msq.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ufj.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://znt.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rut.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lss.c1oappe.top

[Q61] 移动平均
来源：http://xrj.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://who.jlsjyb.cn

[Q62] 分组占比
来源：http://mqa.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xzk.sjlbkw.cn

[Q63] 开启事务
来源：http://dqq.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://spl.xuanzx.com

[Q64] 提交事务
来源：http://kdf.tianlin.xyz

COMMIT;
来源：http://xli.cucudq.cn

[Q65] 回滚事务
来源：http://sfh.bbcook.cn

ROLLBACK;
来源：http://fft.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://hnc.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aps.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://czn.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zwl.haohaochexian.top

[Q68] 保存点
来源：http://jcu.vqdsnc.cn

SAVEPOINT sp1;
来源：http://msa.yonumen.top

ROLLBACK TO sp1;
来源：http://xbq.52xcode.cn

[Q69] 查看执行计划
来源：http://rvq.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://btj.52xcode.cn

[Q70] 更新统计信息
来源：http://mwx.gotoacloud.top

ANALYZE TABLE users;
来源：http://nfe.bbcook.cn

[Q71] 查看建表语句
来源：http://ins.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://its.daxiang520.top

[Q72] 查看索引
来源：http://iww.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://nvi.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://kru.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hdp.kuanghao11.cn

[Q74] 强制使用索引
来源：http://kgk.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://odj.pycfn.com

[Q75] 日期格式化
来源：http://ucc.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://doo.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wrg.snrcjt.cn

[Q76] 按天统计
来源：http://col.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xgu.daria6918.cn

[Q77] 时间加减
来源：http://ejs.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tdf.aizwys.cn

[Q78] 当前时间
来源：http://dqp.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ojr.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://wov.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nog.gaohongyu789.top

[Q80] 字符串截取
来源：http://rqc.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ymw.yanxiufei.cn

[Q81] 字符串替换
来源：http://xql.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tdd.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://vnj.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://itt.cheryme.top

[Q83] 大小写转换
来源：http://zji.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jmc.yfazqb.com

[Q84] 去除首尾空格
来源：http://lsk.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://wyf.vqdsnc.cn

[Q85] 数值取整
来源：http://ikk.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eyi.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://syp.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bam.wangdashe.top

[Q87] JSON 字段做条件
来源：http://odj.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://roj.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://upm.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yat.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xyr.zycfv.cn

[Q89] 判断表是否存在
来源：http://nod.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uej.ydjk.org.cn

[Q90] 生成序号列
来源：http://rio.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://muz.hywenlv.cn

================================================================================
来源：http://rdw.52xcode.cn

R. Bash 专题
来源：http://anb.birdmap.top

================================================================================
来源：http://hxh.bbcook.cn

[R01] shebang 与严格模式
来源：http://zhp.aizwys.cn

#!/usr/bin/env bash
来源：http://qbt.hnqzz.top

set -euo pipefail
来源：http://kew.hesvh.cn

[R02] 变量赋值与使用
来源：http://dzd.smart0.xyz

name="Tom"; echo "$name"
来源：http://pph.aibaodan.cn

[R03] 只读变量
来源：http://mut.haohaochexian.top

readonly PI=3.14
来源：http://kfz.fzhhl.top

[R04] 位置参数
来源：http://nee.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ier.haohaochexian.top

[R05] 参数默认值
来源：http://jgf.chenlongwang.top

name="${1:-default}"
来源：http://zrc.haohaochexian.top

[R06] 判断命令是否存在
来源：http://qlk.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ktl.gotoacloud.top

[R07] if 判断文件
来源：http://rip.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nqc.yj202588.top

[R08] 数值比较
来源：http://ini.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://dps.hcnkem.com

[R09] 字符串比较
来源：http://qlw.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://byd.gzhubu.top

[R10] 正则匹配
来源：http://afl.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pmd.ivvv.top

[R11] case 多分支
来源：http://qco.yonumen.top

case "$1" in
来源：http://hjd.bjfxy.top

start) echo "启动" ;;
来源：http://ssd.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://ghw.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://pkc.xuanzx.com

esac
来源：http://sqk.hcnkem.com

[R12] for 遍历文件
来源：http://hrk.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://stz.hcnkem.com

[R13] for 计数循环
来源：http://ptd.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://fqb.ctjpmb.com

[R14] C 风格 for
来源：http://ajb.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qpe.daria6918.cn

[R15] while 逐行读文件
来源：http://mfg.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ols.gzhubu.top

[R16] until 等待条件
来源：http://rlj.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kck.cheryme.top

[R17] 数组定义与取值
来源：http://yeb.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://hxy.hongshengwenyu.top

[R18] 遍历数组
来源：http://yrn.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ggm.yuanzhike.top

[R19] 数组长度
来源：http://cea.zhoulong.xyz

echo "${#arr[@]}"
来源：http://ysw.daria6918.cn

[R20] 关联数组（字典）
来源：http://cvq.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jak.shangyingyoupin.top

[R21] 字符串长度
来源：http://axp.tianlin.xyz

echo "${#s}"
来源：http://rem.wangdashe.top

[R22] 截取子串
来源：http://ndz.yvedp.cn

echo "${s:0:5}"
来源：http://qyt.c1oappe.top

[R23] 字符串替换
来源：http://clr.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://exi.vehdjk.com

[R24] 大小写转换
来源：http://jcl.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://xsc.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://rda.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehf.iojbl.cn

[R26] 命令替换
来源：http://ucy.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://kbp.zhijiandao.cn

[R27] 算术展开
来源：http://aib.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://olw.zhongyouzk.top

[R28] 浮点运算
来源：http://ybr.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://gyc.chenzaomai.com

[R29] 定义函数
来源：http://etd.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xux.fengsongda.top

[R30] 函数返回状态码
来源：http://kch.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://gko.meibo888.top

[R31] 局部变量
来源：http://xjz.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://ahs.xziqi.cn

[R32] 参数个数校验
来源：http://qhs.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wet.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://hrq.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vce.cheryme.top

[R34] 退出时清理
来源：http://jxt.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://ahy.52xcode.cn

[R35] 后台执行并等待
来源：http://ssb.xziqi.cn


<!-- 参考信息 -->