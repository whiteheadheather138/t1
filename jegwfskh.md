代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xak.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dmc.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hej.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kih.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byt.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zrv.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://woz.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://egy.sxryk.cn

================================================================================
来源：http://wrx.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dww.yonumen.top

================================================================================
来源：http://anc.zycfv.cn

[Q01] 创建表
来源：http://wdo.yongpay.top

CREATE TABLE users (
来源：http://ejm.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbe.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://gaz.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://zfl.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vte.tarul.cn

);
来源：http://nxs.c1oappe.top

[Q02] 创建带外键的表
来源：http://nrq.yanxiufei.cn

CREATE TABLE orders (
来源：http://ddu.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uow.vqdsnc.cn

user_id INT NOT NULL,
来源：http://zpy.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://ako.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hdq.iojbl.cn

);
来源：http://bkj.hcnkem.com

[Q03] 增加列
来源：http://pwc.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ueq.jqgufenzy.top

[Q04] 修改列类型
来源：http://tdi.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://meh.fanxiaobao.xyz

[Q05] 重命名列
来源：http://sbi.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cbg.sysykeji.top

[Q06] 删除列
来源：http://qup.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xjs.tarul.cn

[Q07] 删除表
来源：http://ieo.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://yxt.hywenlv.cn

[Q08] 创建普通索引
来源：http://opu.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oxb.guowangkeji.top

[Q09] 创建唯一索引
来源：http://sgv.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mzq.hesvh.cn

[Q10] 插入单行
来源：http://fkw.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kku.guowangkeji.top

[Q11] 一次插入多行
来源：http://hef.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://apg.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://ifz.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qfk.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://emc.yj202588.top

[Q13] 忽略重复插入
来源：http://lrf.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://srf.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://fsy.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hzj.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mvn.yanxiufei.cn

[Q15] 查询全部
来源：http://pel.yonumen.top

SELECT * FROM users;
来源：http://rdr.nanxinkj.top

[Q16] 查询指定列
来源：http://qfz.0kj1m.cn

SELECT id, name FROM users;
来源：http://zys.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://tdr.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mgu.birdmap.top

[Q18] 模糊匹配
来源：http://koj.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqc.tanke756.top

[Q19] 范围查询
来源：http://uvm.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yxn.meibo888.top

[Q20] IN 列表
来源：http://zfn.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ndn.redwolf501.top

[Q21] 空值判断
来源：http://eew.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ztw.iojbl.cn

[Q22] 排序
来源：http://wxp.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hqf.ehwqpu.com

[Q23] 分页
来源：http://dgd.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uzk.yuanzhike.top

[Q24] 去重
来源：http://bew.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://rdy.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://sjx.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wct.jinqigfzy.top

[Q26] 计数
来源：http://ffp.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://oky.fehbvm.com

[Q27] 条件计数
来源：http://vcd.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vur.gzhubu.top

[Q28] 求和与平均
来源：http://urh.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pug.gaohongyu789.top

[Q29] 最大最小值
来源：http://ekz.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wnb.aibaodan.cn

[Q30] 分组统计
来源：http://vzy.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oiy.nwbrower.top

[Q31] 分组后过滤
来源：http://ruv.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bch.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://csy.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cvf.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ajb.dianchejie.cn

[Q33] 多列分组
来源：http://luy.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://geu.yangfankeji.com

[Q34] 每组取第一条
来源：http://phn.zdbjq.cn

SELECT * FROM (
来源：http://noo.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gmt.gzhubu.top

) t WHERE rn = 1;
来源：http://slj.aibaodan.cn

[Q35] 内连接
来源：http://tzo.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zmo.hongshengwenyu.top

[Q36] 左连接
来源：http://efr.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rys.yongpay.top

[Q37] 右连接
来源：http://vyq.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggb.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://qij.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ioj.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://wdb.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kjz.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://but.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://dpa.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pvw.fanxiaobao.xyz

[Q41] 多表连接
来源：http://ljz.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://otr.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://ckf.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://bdt.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://fyq.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://nhh.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lno.birdmap.top

[Q43] 标量子查询
来源：http://pvi.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tvw.bbcook.cn

[Q44] IN 子查询
来源：http://pqn.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tjn.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://urg.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ujw.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tcj.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gla.yonumen.top

[Q47] 与平均值比较
来源：http://bjn.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nfi.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://qzd.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wej.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ygl.zhengqikj.top

[Q49] 更新单行
来源：http://dym.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lcj.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://cll.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dns.yuxming.cn

[Q51] 用子查询更新
来源：http://cqh.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fna.birdmap.top

[Q52] 删除指定行
来源：http://fuf.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://uyq.cashguo.top

[Q53] 按条件删除
来源：http://oqh.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdf.shanyushiyangkeji.top

[Q54] 清空表
来源：http://mbo.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://fml.xinyue.icu

[Q55] 排名（并列占位）
来源：http://dod.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://znd.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://vwi.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehb.ywan-chungtsiang.top

[Q57] 行号
来源：http://kqi.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://chf.hnxiangtu.top

[Q58] 累计求和
来源：http://pin.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kgh.cdnleiting.top

[Q59] 分组内累计
来源：http://dxf.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iks.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://qcp.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fdi.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxq.zdqjudy.top

[Q61] 移动平均
来源：http://sae.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yzu.sysykeji.top

[Q62] 分组占比
来源：http://uzy.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://osh.shangyingyoupin.top

[Q63] 开启事务
来源：http://trd.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qfe.jqgufenzy.top

[Q64] 提交事务
来源：http://zwi.ywan-chungtsiang.top

COMMIT;
来源：http://puk.yj202588.top

[Q65] 回滚事务
来源：http://aib.cheryme.top

ROLLBACK;
来源：http://jct.wangshuangyany.cn

[Q66] 行锁查询
来源：http://tus.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://isf.havefunace.top

[Q67] 设置隔离级别
来源：http://spq.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://boo.cashguo.top

[Q68] 保存点
来源：http://jdm.bbcook.cn

SAVEPOINT sp1;
来源：http://wuw.gzhubu.top

ROLLBACK TO sp1;
来源：http://kam.xziqi.cn

[Q69] 查看执行计划
来源：http://sle.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pfw.jiagoushi.top

[Q70] 更新统计信息
来源：http://osm.gzhubu.top

ANALYZE TABLE users;
来源：http://xwr.yvedp.cn

[Q71] 查看建表语句
来源：http://tdu.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ogi.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://kvm.yonumen.top

SHOW INDEX FROM users;
来源：http://phe.sufxvd.cn

[Q73] 查看表状态
来源：http://wrm.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cjf.zhoulong.xyz

[Q74] 强制使用索引
来源：http://owi.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zoq.yj202588.top

[Q75] 日期格式化
来源：http://sre.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tsq.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jdo.aibaodan.cn

[Q76] 按天统计
来源：http://yly.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jin.jianghu66.top

[Q77] 时间加减
来源：http://uld.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hrx.svipenyu.cn

[Q78] 当前时间
来源：http://dbd.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pgy.pycfn.com

[Q79] 字符串拼接
来源：http://vst.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gba.bbcook.cn

[Q80] 字符串截取
来源：http://ddl.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yoq.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://dvu.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yum.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://rut.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hwx.zdqjudy.top

[Q83] 大小写转换
来源：http://wdm.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wdr.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://sxv.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://aqe.9152youxi.cn

[Q85] 数值取整
来源：http://kaq.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cuh.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://qsi.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aje.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://ivx.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://brd.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://yky.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://syf.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lxf.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://vzk.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qtb.yvedp.cn

[Q90] 生成序号列
来源：http://iyc.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dkd.zycfv.cn

================================================================================
来源：http://dxu.dashuyun.cn

R. Bash 专题
来源：http://hjs.feifeiyinyue.top

================================================================================
来源：http://tyk.fzhhl.top

[R01] shebang 与严格模式
来源：http://mml.ydjk.org.cn

#!/usr/bin/env bash
来源：http://jdq.sysykeji.top

set -euo pipefail
来源：http://tsl.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://vio.andypj.xyz

name="Tom"; echo "$name"
来源：http://off.bjfxy.top

[R03] 只读变量
来源：http://apy.pengpengdd.cyou

readonly PI=3.14
来源：http://mzd.fktsv.cn

[R04] 位置参数
来源：http://lmo.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zaw.xuanzx.com

[R05] 参数默认值
来源：http://pil.yj20258.top

name="${1:-default}"
来源：http://hfq.smart0.xyz

[R06] 判断命令是否存在
来源：http://qkm.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zpp.andypj.xyz

[R07] if 判断文件
来源：http://kfx.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://doj.sufxvd.cn

[R08] 数值比较
来源：http://xfw.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uwy.chenjidiqi.icu

[R09] 字符串比较
来源：http://hwd.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://avb.316326.xyz

[R10] 正则匹配
来源：http://loo.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://puh.zhixingplan.top

[R11] case 多分支
来源：http://nbo.nwbrower.top

case "$1" in
来源：http://ksu.feifeiyinyue.top

start) echo "启动" ;;
来源：http://edw.mhx1999.top

stop)  echo "停止" ;;
来源：http://mpd.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://ufo.jinyuanbaomall.cn

esac
来源：http://ryf.yongpay.top

[R12] for 遍历文件
来源：http://ouk.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://wpe.mhx1999.top

[R13] for 计数循环
来源：http://cap.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://fsg.shzxlz.cn

[R14] C 风格 for
来源：http://mie.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tkj.vqdsnc.cn

[R15] while 逐行读文件
来源：http://iic.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fey.vehdjk.com

[R16] until 等待条件
来源：http://ltk.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://agc.zhongyouzk.top

[R17] 数组定义与取值
来源：http://wsu.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://tgt.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://yqg.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hyn.yj20258888.top

[R19] 数组长度
来源：http://orx.redwolf501.top

echo "${#arr[@]}"
来源：http://zwl.0kj1m.cn

[R20] 关联数组（字典）
来源：http://tzr.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://odg.tian-w.cn

[R21] 字符串长度
来源：http://moq.bjfxy.top

echo "${#s}"
来源：http://jlt.yangfankeji.com

[R22] 截取子串
来源：http://imi.yvedp.cn

echo "${s:0:5}"
来源：http://krx.fktsv.cn

[R23] 字符串替换
来源：http://roj.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fnp.ivvv.top

[R24] 大小写转换
来源：http://noq.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://vrk.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://byc.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oxv.hfpthk.cn

[R26] 命令替换
来源：http://csr.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://zdy.chenjidiqi.icu

[R27] 算术展开
来源：http://okm.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://fwy.yfazqb.com

[R28] 浮点运算
来源：http://vge.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://ovv.zdbjq.cn

[R29] 定义函数
来源：http://szr.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://umq.zdqjudy.top

[R30] 函数返回状态码
来源：http://ffq.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://wor.fengsongda.top

[R31] 局部变量
来源：http://yif.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://pvl.chenzaomai.com

[R32] 参数个数校验
来源：http://lzq.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jja.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://pxh.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ngn.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://yij.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://czf.yonumen.top

[R35] 后台执行并等待
来源：http://llf.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uwl.uphjek.com

[R36] 并发执行多个任务
来源：http://mah.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tfx.hammf.cn

[R37] 把输出赋给变量
来源：http://gjm.ybcxt.top

files=$(ls -1)
来源：http://xvp.52xcode.cn

[R38] 管道串联
来源：http://zrh.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://wyn.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://jkl.bjfxy.top


<!-- 参考信息 -->