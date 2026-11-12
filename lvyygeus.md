代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tfu.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://mua.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ues.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://fqn.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tig.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://clb.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ipy.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sye.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://awk.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ywh.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qkc.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kxf.sxryk.cn

================================================================================
来源：http://apb.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aks.gogol.net.cn

================================================================================
来源：http://iuh.fzhhl.top

[Q01] 创建表
来源：http://rqx.hfpthk.cn

CREATE TABLE users (
来源：http://ynv.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nmf.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://asc.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://wxh.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zwr.hnxiangtu.top

);
来源：http://sls.zhengqikj.top

[Q02] 创建带外键的表
来源：http://vrf.vqdsnc.cn

CREATE TABLE orders (
来源：http://gnj.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zvz.guannengcc.top

user_id INT NOT NULL,
来源：http://eks.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://unf.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xpn.nanxuanxn.top

);
来源：http://bzj.iojbl.cn

[Q03] 增加列
来源：http://zjl.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nut.zhongyouzk.top

[Q04] 修改列类型
来源：http://ivf.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdl.zhengqikj.top

[Q05] 重命名列
来源：http://rxa.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ozd.sufxvd.cn

[Q06] 删除列
来源：http://bfc.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://vog.vqdsnc.cn

[Q07] 删除表
来源：http://ycz.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://ckp.tian-w.cn

[Q08] 创建普通索引
来源：http://ngt.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xwb.gzhubu.top

[Q09] 创建唯一索引
来源：http://crg.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tel.yuxming.cn

[Q10] 插入单行
来源：http://sbj.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xew.cdnleiting.top

[Q11] 一次插入多行
来源：http://yta.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ede.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://tyv.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://cai.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wid.tanke756.top

[Q13] 忽略重复插入
来源：http://akh.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qoj.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://zdl.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gxh.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ckk.fehbvm.com

[Q15] 查询全部
来源：http://bue.meibo888.top

SELECT * FROM users;
来源：http://vjh.xuanzx.com

[Q16] 查询指定列
来源：http://ajl.guowangkeji.top

SELECT id, name FROM users;
来源：http://mvh.jinqigufen.top

[Q17] 条件查询
来源：http://wqy.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ywr.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://lgi.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mav.tianlin.xyz

[Q19] 范围查询
来源：http://mij.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvf.jinqigufen.top

[Q20] IN 列表
来源：http://dil.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://suv.vqdsnc.cn

[Q21] 空值判断
来源：http://qox.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wbq.chenjidiqi.icu

[Q22] 排序
来源：http://cij.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cfr.xinyue.icu

[Q23] 分页
来源：http://paa.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ocs.zhongyouzk.top

[Q24] 去重
来源：http://txk.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://wxb.hnxiangtu.top

[Q25] 只取前 N 条
来源：http://iaj.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://smu.ehwqpu.com

[Q26] 计数
来源：http://est.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://gtc.yongpay.top

[Q27] 条件计数
来源：http://ihd.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wru.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://abv.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zrd.nanxinkj.top

[Q29] 最大最小值
来源：http://fwk.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wuh.yvedp.cn

[Q30] 分组统计
来源：http://zrw.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gch.cdnleiting.top

[Q31] 分组后过滤
来源：http://tqo.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gls.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://irw.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://war.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vwt.ctjpmb.com

[Q33] 多列分组
来源：http://zrn.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://std.xinyue.icu

[Q34] 每组取第一条
来源：http://fjc.zycfv.cn

SELECT * FROM (
来源：http://fuy.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtu.nanxinkj.top

) t WHERE rn = 1;
来源：http://tyn.gaohongyu789.top

[Q35] 内连接
来源：http://xkv.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://waq.hnqzz.top

[Q36] 左连接
来源：http://wgw.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kyi.chenlongwang.top

[Q37] 右连接
来源：http://krx.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lza.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dns.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jik.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://tzu.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xbl.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uds.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ldr.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cso.jqgfzy.top

[Q41] 多表连接
来源：http://cwh.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gzr.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://nld.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://myk.uphjek.com

[Q42] 连接条件附加过滤
来源：http://ead.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://lah.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://anj.zhijiandao.cn

[Q43] 标量子查询
来源：http://fcx.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gnd.c1oappe.top

[Q44] IN 子查询
来源：http://gbh.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ens.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://cjb.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jgn.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jxb.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ypu.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://quw.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://npg.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://wml.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://umk.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://rjm.hywenlv.cn

[Q49] 更新单行
来源：http://ttm.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gbn.smart0.xyz

[Q50] 批量更新
来源：http://pvz.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zhs.zhongyouzk.top

[Q51] 用子查询更新
来源：http://fat.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jbt.chenlongwang.top

[Q52] 删除指定行
来源：http://lfh.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://hnj.smart0.xyz

[Q53] 按条件删除
来源：http://dqm.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cgw.jinqigfzy.top

[Q54] 清空表
来源：http://iio.yfazqb.com

TRUNCATE TABLE logs;
来源：http://wjf.yfazqb.com

[Q55] 排名（并列占位）
来源：http://len.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvh.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://gnk.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yab.yuanzhike.top

[Q57] 行号
来源：http://gdj.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qen.9152youxi.cn

[Q58] 累计求和
来源：http://kns.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hui.cdnleiting.top

[Q59] 分组内累计
来源：http://wim.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qgc.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://mwu.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jry.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://skv.vqdsnc.cn

[Q61] 移动平均
来源：http://bwr.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uex.shuidangran.top

[Q62] 分组占比
来源：http://rob.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://htm.jinqigfzy.top

[Q63] 开启事务
来源：http://frx.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wht.fktsv.cn

[Q64] 提交事务
来源：http://exx.sxryk.cn

COMMIT;
来源：http://rrw.nanxinkj.top

[Q65] 回滚事务
来源：http://dfe.guowangkeji.top

ROLLBACK;
来源：http://and.wangdashe.top

[Q66] 行锁查询
来源：http://drz.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pzj.pycfn.com

[Q67] 设置隔离级别
来源：http://jpk.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://asv.quarkkingdee.top

[Q68] 保存点
来源：http://egf.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://wxq.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://njn.yfazqb.com

[Q69] 查看执行计划
来源：http://zcs.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jrw.zycfv.cn

[Q70] 更新统计信息
来源：http://fua.gotoacloud.top

ANALYZE TABLE users;
来源：http://juo.hfpthk.cn

[Q71] 查看建表语句
来源：http://aki.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://adm.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://ain.chenzaomai.com

SHOW INDEX FROM users;
来源：http://elt.cheryme.top

[Q73] 查看表状态
来源：http://vit.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cpc.xuanzx.com

[Q74] 强制使用索引
来源：http://msu.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://flp.dashuyun.cn

[Q75] 日期格式化
来源：http://wul.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qcd.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zte.vehdjk.com

[Q76] 按天统计
来源：http://pdl.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwz.wangshuangyany.cn

[Q77] 时间加减
来源：http://dms.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uch.birdmap.top

[Q78] 当前时间
来源：http://ieg.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vjk.gotoacloud.top

[Q79] 字符串拼接
来源：http://dxo.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehy.snrcjt.cn

[Q80] 字符串截取
来源：http://ohk.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qtq.jqgfzy.top

[Q81] 字符串替换
来源：http://wbt.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cev.yj20258.top

[Q82] 字符长度与字节长度
来源：http://svp.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yhu.ydzc1.top

[Q83] 大小写转换
来源：http://tjs.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gqi.yueranfly.top

[Q84] 去除首尾空格
来源：http://zwd.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://xqy.gaohongyu789.top

[Q85] 数值取整
来源：http://ocu.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mmd.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://gqc.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://psr.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://hec.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://luo.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://pex.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hxz.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zgn.aibaodan.cn

[Q89] 判断表是否存在
来源：http://uvb.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jlk.xziqi.cn

[Q90] 生成序号列
来源：http://ucf.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhf.yj20258888.top

================================================================================
来源：http://aqf.pengpengdd.cyou

R. Bash 专题
来源：http://ipm.ywan-chungtsiang.top

================================================================================
来源：http://foe.xziqi.cn

[R01] shebang 与严格模式
来源：http://sav.gotoacloud.top

#!/usr/bin/env bash
来源：http://njw.ywan-chungtsiang.top

set -euo pipefail
来源：http://dsn.uphjek.com

[R02] 变量赋值与使用
来源：http://xcm.hfpthk.cn

name="Tom"; echo "$name"
来源：http://rhk.guowangkeji.top

[R03] 只读变量
来源：http://mxg.ppjwa.cn

readonly PI=3.14
来源：http://jda.316326.xyz

[R04] 位置参数
来源：http://ggk.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wxo.aizwys.cn

[R05] 参数默认值
来源：http://fdv.shangyingyoupin.top

name="${1:-default}"
来源：http://wzk.xuanzx.com

[R06] 判断命令是否存在
来源：http://zpn.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ooh.yvedp.cn

[R07] if 判断文件
来源：http://ejz.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://loh.jiagoushi.top

[R08] 数值比较
来源：http://bmr.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://atm.zdqjudy.top

[R09] 字符串比较
来源：http://lbc.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jlw.ivvv.top

[R10] 正则匹配
来源：http://asw.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://prn.iojbl.cn

[R11] case 多分支
来源：http://hen.hysaishi.cn

case "$1" in
来源：http://dsg.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://tne.meibo888.top

stop)  echo "停止" ;;
来源：http://brf.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://hhb.haohaochexian.top

esac
来源：http://mgf.fzhhl.top

[R12] for 遍历文件
来源：http://soq.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://dws.jinqigfzy.top

[R13] for 计数循环
来源：http://fbc.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://soj.guowangkeji.top

[R14] C 风格 for
来源：http://lbn.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://emj.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://hwh.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mmn.hnqzz.top

[R16] until 等待条件
来源：http://lxb.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rnj.hnxiangtu.top

[R17] 数组定义与取值
来源：http://fio.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lem.xziqi.cn

[R18] 遍历数组
来源：http://mqh.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://par.gaohongyu789.top

[R19] 数组长度
来源：http://ssu.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://tyv.gotoacloud.top

[R20] 关联数组（字典）
来源：http://upy.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qhx.xuetiantiany.cn

[R21] 字符串长度
来源：http://pfe.gaohongyu789.top

echo "${#s}"
来源：http://gsw.cqqwz.cn

[R22] 截取子串
来源：http://xqa.0kj1m.cn

echo "${s:0:5}"
来源：http://ouw.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://uxi.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cbs.yanxiufei.cn

[R24] 大小写转换
来源：http://lpd.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://tvw.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://bva.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vqs.jinyuanbaomall.cn

[R26] 命令替换
来源：http://wox.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://gnq.guannengcc.top

[R27] 算术展开
来源：http://rms.xylfe.cn

echo $((1 + 2 * 3))
来源：http://uez.c1oappe.top

[R28] 浮点运算
来源：http://dps.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://axi.ydjk.org.cn

[R29] 定义函数
来源：http://vrs.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ifn.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://rtg.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://qcv.cucudq.cn

[R31] 局部变量
来源：http://gtz.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://sbp.316326.xyz

[R32] 参数个数校验
来源：http://oaw.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ymd.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://tup.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sbi.mhx1999.top

[R34] 退出时清理
来源：http://xjj.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sbu.svipenyu.cn

[R35] 后台执行并等待
来源：http://mpp.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lmi.hammf.cn

[R36] 并发执行多个任务
来源：http://mpg.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xua.daria6918.cn

[R37] 把输出赋给变量
来源：http://vbk.zdbjq.cn


<!-- 参考信息 -->