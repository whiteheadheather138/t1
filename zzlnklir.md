代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fsc.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bpr.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqk.316326.xyz

[P08] 处理浮点精度问题
来源：http://ube.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oob.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://itc.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mwv.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lzt.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fyb.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xdx.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://omx.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pil.sysykeji.top

================================================================================
来源：http://eue.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vti.yanxiufei.cn

================================================================================
来源：http://fzb.daria6918.cn

[Q01] 创建表
来源：http://peh.jianghu66.top

CREATE TABLE users (
来源：http://lqt.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zad.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://kmx.hfpthk.cn

email VARCHAR(100) UNIQUE,
来源：http://oqz.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qfu.ppjwa.cn

);
来源：http://mcj.jyoumei.cn

[Q02] 创建带外键的表
来源：http://hbf.0kj1m.cn

CREATE TABLE orders (
来源：http://pon.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfi.sufxvd.cn

user_id INT NOT NULL,
来源：http://sdl.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://ots.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xgq.cqqwz.cn

);
来源：http://nws.sxryk.cn

[Q03] 增加列
来源：http://zih.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lkg.birdmap.top

[Q04] 修改列类型
来源：http://juk.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kiq.gaohongyu789.top

[Q05] 重命名列
来源：http://cjw.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kuf.jinghuilouyu.cn

[Q06] 删除列
来源：http://dkc.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wae.316326.xyz

[Q07] 删除表
来源：http://mjh.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://doy.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://ppq.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oee.jyoumei.cn

[Q09] 创建唯一索引
来源：http://amd.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rxg.sufxvd.cn

[Q10] 插入单行
来源：http://qrp.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iac.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://fah.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jru.tanke756.top

[Q12] 插入后取自增 ID
来源：http://wit.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qbd.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ihx.hnqzz.top

[Q13] 忽略重复插入
来源：http://tzi.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bcy.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://gfx.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://txk.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dbn.0kj1m.cn

[Q15] 查询全部
来源：http://lkd.bbcook.cn

SELECT * FROM users;
来源：http://ziv.tian-w.cn

[Q16] 查询指定列
来源：http://wzv.zycfv.cn

SELECT id, name FROM users;
来源：http://dvv.fanxiaobao.xyz

[Q17] 条件查询
来源：http://hog.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vhl.xuanzx.com

[Q18] 模糊匹配
来源：http://qwf.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://egl.zdbjq.cn

[Q19] 范围查询
来源：http://nlq.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zux.jinghuilouyu.cn

[Q20] IN 列表
来源：http://rxq.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bul.jqgfzy.top

[Q21] 空值判断
来源：http://fzk.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ndw.yvedp.cn

[Q22] 排序
来源：http://hlp.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyp.epnwcf.com

[Q23] 分页
来源：http://cpj.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://coz.havefunace.top

[Q24] 去重
来源：http://bpu.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://yfn.ehwqpu.com

[Q25] 只取前 N 条
来源：http://kcj.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jwa.xziqi.cn

[Q26] 计数
来源：http://ttk.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://qat.sxryk.cn

[Q27] 条件计数
来源：http://czo.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pct.xziqi.cn

[Q28] 求和与平均
来源：http://diz.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dku.andypj.xyz

[Q29] 最大最小值
来源：http://gth.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://spf.nanxinkj.top

[Q30] 分组统计
来源：http://jzp.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zhi.zhoulong.xyz

[Q31] 分组后过滤
来源：http://thb.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hwe.wangdashe.top

[Q32] 分组拼接字符串
来源：http://iob.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://soc.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://duz.yj20258.top

[Q33] 多列分组
来源：http://vjf.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eyq.gaohongyu789.top

[Q34] 每组取第一条
来源：http://dwm.sxryk.cn

SELECT * FROM (
来源：http://lxj.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lqp.xuanzx.com

) t WHERE rn = 1;
来源：http://jlp.jianghu66.top

[Q35] 内连接
来源：http://fxu.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://agb.zhiwuduotai.top

[Q36] 左连接
来源：http://zhf.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iss.cdnleiting.top

[Q37] 右连接
来源：http://zpt.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wzk.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://atd.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ful.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://qju.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://asp.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jad.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://prc.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bkf.tianlin.xyz

[Q41] 多表连接
来源：http://hya.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://glh.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://sdk.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://wxd.cheryme.top

[Q42] 连接条件附加过滤
来源：http://diu.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://auk.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcj.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://gaw.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nfi.jqgufenzy.top

[Q44] IN 子查询
来源：http://hql.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://taq.ivvv.top

[Q45] EXISTS 判断存在
来源：http://ovk.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bdm.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://nzo.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zat.guannengcc.top

[Q47] 与平均值比较
来源：http://evu.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kxe.uphjek.com

[Q48] CTE 公用表表达式
来源：http://gxi.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cbq.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://hjf.meibo888.top

[Q49] 更新单行
来源：http://xwt.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uik.ydzc1.top

[Q50] 批量更新
来源：http://avi.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fae.tarul.cn

[Q51] 用子查询更新
来源：http://jdp.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sss.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://gml.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://ant.guowangkeji.top

[Q53] 按条件删除
来源：http://qnn.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gzh.jinqigufen.top

[Q54] 清空表
来源：http://pcq.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://ulz.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://ptr.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sex.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://sho.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hzg.fehbvm.com

[Q57] 行号
来源：http://fyo.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://unh.bbcook.cn

[Q58] 累计求和
来源：http://tus.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pbf.fehbvm.com

[Q59] 分组内累计
来源：http://cva.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rdd.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://cvw.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ong.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cql.cucudq.cn

[Q61] 移动平均
来源：http://jyq.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wjt.svipenyu.cn

[Q62] 分组占比
来源：http://vtk.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://drj.hnxiangtu.top

[Q63] 开启事务
来源：http://qbo.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bwj.tanke756.top

[Q64] 提交事务
来源：http://woz.cheryme.top

COMMIT;
来源：http://hgb.shangyingyoupin.top

[Q65] 回滚事务
来源：http://dov.nwbrower.top

ROLLBACK;
来源：http://mdq.fengsongda.top

[Q66] 行锁查询
来源：http://ish.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hjl.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://qfs.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xwc.yuanzhike.top

[Q68] 保存点
来源：http://gpz.shzxlz.cn

SAVEPOINT sp1;
来源：http://cvx.yj20258.top

ROLLBACK TO sp1;
来源：http://pwt.hammf.cn

[Q69] 查看执行计划
来源：http://eff.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cyp.hysaishi.cn

[Q70] 更新统计信息
来源：http://xli.vqdsnc.cn

ANALYZE TABLE users;
来源：http://lbq.sweek.top

[Q71] 查看建表语句
来源：http://uih.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tpx.shangyingyoupin.top

[Q72] 查看索引
来源：http://suu.gotoacloud.top

SHOW INDEX FROM users;
来源：http://myv.hesvh.cn

[Q73] 查看表状态
来源：http://kwx.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bsp.ybcxt.top

[Q74] 强制使用索引
来源：http://aun.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://upq.hnqzz.top

[Q75] 日期格式化
来源：http://pea.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nca.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fbg.tarul.cn

[Q76] 按天统计
来源：http://iio.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tvc.jinqigufen.top

[Q77] 时间加减
来源：http://yor.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tfd.bjfxy.top

[Q78] 当前时间
来源：http://xec.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xim.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://gmm.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cxk.yj202588.top

[Q80] 字符串截取
来源：http://euh.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pzi.yueranfly.top

[Q81] 字符串替换
来源：http://blx.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xxw.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://jhh.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nti.ivvv.top

[Q83] 大小写转换
来源：http://aqf.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yye.ivvv.top

[Q84] 去除首尾空格
来源：http://npi.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://rof.gotoacloud.top

[Q85] 数值取整
来源：http://wrd.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zlg.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://low.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nji.smart0.xyz

[Q87] JSON 字段做条件
来源：http://ptq.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rxc.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://azn.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://noq.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mlf.nanxinkj.top

[Q89] 判断表是否存在
来源：http://ibw.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uxq.vqdsnc.cn

[Q90] 生成序号列
来源：http://whv.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ydx.hammf.cn

================================================================================
来源：http://khk.9152youxi.cn

R. Bash 专题
来源：http://mkl.quarkkingdee.top

================================================================================
来源：http://qug.hcnkem.com

[R01] shebang 与严格模式
来源：http://waz.yfazqb.com

#!/usr/bin/env bash
来源：http://axy.yuanzhike.top

set -euo pipefail
来源：http://bhv.hysaishi.cn

[R02] 变量赋值与使用
来源：http://zlv.guannengcc.top

name="Tom"; echo "$name"
来源：http://cjv.pycfn.com

[R03] 只读变量
来源：http://new.zhaomingkeji.xyz

readonly PI=3.14
来源：http://ffz.tian-w.cn

[R04] 位置参数
来源：http://qbd.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zod.9152youxi.cn

[R05] 参数默认值
来源：http://fjf.shuidangran.top

name="${1:-default}"
来源：http://hat.guannengcc.top

[R06] 判断命令是否存在
来源：http://hex.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wcq.vehdjk.com

[R07] if 判断文件
来源：http://lam.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ndy.daria6918.cn

[R08] 数值比较
来源：http://cnq.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zmz.chenzaomai.com

[R09] 字符串比较
来源：http://ghz.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vgh.cucudq.cn

[R10] 正则匹配
来源：http://yln.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bzb.bjfxy.top

[R11] case 多分支
来源：http://bvu.feifeiyinyue.top

case "$1" in
来源：http://vcw.vehdjk.com

start) echo "启动" ;;
来源：http://bkd.xylfe.cn

stop)  echo "停止" ;;
来源：http://clq.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://bjl.ivvv.top

esac
来源：http://qmt.smart0.xyz

[R12] for 遍历文件
来源：http://qqd.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://ael.zhongyouzk.top

[R13] for 计数循环
来源：http://rxx.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://ifc.feifeiyinyue.top

[R14] C 风格 for
来源：http://njx.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wwp.zhoulong.xyz

[R15] while 逐行读文件
来源：http://gnk.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pxk.gaohongyu789.top

[R16] until 等待条件
来源：http://nwb.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iws.hywenlv.cn

[R17] 数组定义与取值
来源：http://snd.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://sgf.sysykeji.top

[R18] 遍历数组
来源：http://ugf.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yjw.pycfn.com

[R19] 数组长度
来源：http://jgw.svipenyu.cn

echo "${#arr[@]}"
来源：http://kqd.hammf.cn

[R20] 关联数组（字典）
来源：http://taj.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://npl.xuanzx.com

[R21] 字符串长度
来源：http://ygo.sxryk.cn

echo "${#s}"
来源：http://jtu.sysykeji.top

[R22] 截取子串
来源：http://eom.jqgfzy.top

echo "${s:0:5}"
来源：http://rgy.sufxvd.cn

[R23] 字符串替换
来源：http://jmm.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://thb.zhiwuduotai.top

[R24] 大小写转换
来源：http://kqs.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://unq.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://lrs.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zid.cashguo.top

[R26] 命令替换
来源：http://xda.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://trt.xziqi.cn

[R27] 算术展开
来源：http://xru.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://zna.316326.xyz

[R28] 浮点运算
来源：http://hif.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://ybe.316326.xyz

[R29] 定义函数
来源：http://jiu.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xgw.gotoacloud.top

[R30] 函数返回状态码
来源：http://vbh.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://wnv.fanxiaobao.xyz

[R31] 局部变量
来源：http://vcs.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://acd.yj202588.top

[R32] 参数个数校验
来源：http://bql.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iji.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://yvc.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yrh.feifeiyinyue.top

[R34] 退出时清理
来源：http://puq.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pvx.tanke756.top

[R35] 后台执行并等待
来源：http://bzq.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cfl.yvedp.cn

[R36] 并发执行多个任务
来源：http://jmv.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oph.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://sgf.yonumen.top


<!-- 参考信息 -->