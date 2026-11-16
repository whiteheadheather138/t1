代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ryi.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fji.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hkn.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://pbx.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://avq.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pjd.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqz.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nbz.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kyh.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://orh.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tgg.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dom.xinyue.icu

================================================================================
来源：http://xtx.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://puu.ywan-chungtsiang.top

================================================================================
来源：http://fbk.smart0.xyz

[Q01] 创建表
来源：http://aau.snrcjt.cn

CREATE TABLE users (
来源：http://fnb.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gsi.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://kco.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://fjj.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://omv.hesvh.cn

);
来源：http://txk.havefunace.top

[Q02] 创建带外键的表
来源：http://ljh.yj202588.top

CREATE TABLE orders (
来源：http://gcv.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://clg.cdnleiting.top

user_id INT NOT NULL,
来源：http://xsn.birdmap.top

amount DECIMAL(10, 2),
来源：http://afh.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ztk.dashuyun.cn

);
来源：http://ypb.pengpengdd.cyou

[Q03] 增加列
来源：http://nul.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iww.gaohongyu789.top

[Q04] 修改列类型
来源：http://jdy.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://deb.sjlbkw.cn

[Q05] 重命名列
来源：http://ftw.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vif.fanxiaobao.xyz

[Q06] 删除列
来源：http://apq.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bgq.vqdsnc.cn

[Q07] 删除表
来源：http://evj.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://gze.redwolf501.top

[Q08] 创建普通索引
来源：http://yxs.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://hrp.zycfv.cn

[Q09] 创建唯一索引
来源：http://zlk.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xlu.hcnkem.com

[Q10] 插入单行
来源：http://txk.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://onq.zhongyouzk.top

[Q11] 一次插入多行
来源：http://fth.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://atu.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://sxp.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ccy.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qzc.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://ekr.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gge.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://kvh.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://egc.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pxl.yonumen.top

[Q15] 查询全部
来源：http://vqb.hesvh.cn

SELECT * FROM users;
来源：http://vmc.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://lqs.havefunace.top

SELECT id, name FROM users;
来源：http://knb.sufxvd.cn

[Q17] 条件查询
来源：http://lfx.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyn.tanke756.top

[Q18] 模糊匹配
来源：http://soy.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://con.ehwqpu.com

[Q19] 范围查询
来源：http://pyl.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://drm.andypj.xyz

[Q20] IN 列表
来源：http://jnz.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mhs.feifeiyinyue.top

[Q21] 空值判断
来源：http://oio.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lts.316326.xyz

[Q22] 排序
来源：http://obb.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vwn.cheryme.top

[Q23] 分页
来源：http://kge.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qsy.uphjek.com

[Q24] 去重
来源：http://zio.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://ytf.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://mfy.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tmv.jinghuilouyu.cn

[Q26] 计数
来源：http://kqf.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://mmf.cucudq.cn

[Q27] 条件计数
来源：http://mhe.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mgt.cqqwz.cn

[Q28] 求和与平均
来源：http://gbt.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bss.wangshuangyany.cn

[Q29] 最大最小值
来源：http://fso.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fnb.0kj1m.cn

[Q30] 分组统计
来源：http://zig.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rfw.fengsongda.top

[Q31] 分组后过滤
来源：http://gjo.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oeh.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://baw.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://weg.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xyf.ivvv.top

[Q33] 多列分组
来源：http://elp.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rhi.yongpay.top

[Q34] 每组取第一条
来源：http://yee.zhijiandao.cn

SELECT * FROM (
来源：http://tsr.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zrg.chenzaomai.com

) t WHERE rn = 1;
来源：http://qxx.sxryk.cn

[Q35] 内连接
来源：http://irl.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ffl.xylfe.cn

[Q36] 左连接
来源：http://gkt.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xor.aizwys.cn

[Q37] 右连接
来源：http://uar.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bza.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://acs.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qlp.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://cgq.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pdn.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pij.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://otz.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ggt.mhx1999.top

[Q41] 多表连接
来源：http://wrm.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://lgy.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://uhz.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://yxx.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://esf.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://qqm.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://piq.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://slv.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nuc.yuxming.cn

[Q44] IN 子查询
来源：http://ius.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ekh.tian-w.cn

[Q45] EXISTS 判断存在
来源：http://nzz.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://acg.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://age.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgp.hcnkem.com

[Q47] 与平均值比较
来源：http://zim.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tik.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://tfz.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dtt.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://qzv.guowangkeji.top

[Q49] 更新单行
来源：http://dpe.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vcs.xuetiantiany.cn

[Q50] 批量更新
来源：http://vfk.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wun.fzhhl.top

[Q51] 用子查询更新
来源：http://vvj.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://den.tian-w.cn

[Q52] 删除指定行
来源：http://yol.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://fia.yfazqb.com

[Q53] 按条件删除
来源：http://ugt.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://seb.ybcxt.top

[Q54] 清空表
来源：http://pwo.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://tvd.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://oaq.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mau.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://csg.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tdw.sysykeji.top

[Q57] 行号
来源：http://uuq.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qjc.zhiwuduotai.top

[Q58] 累计求和
来源：http://yig.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jiz.cqqwz.cn

[Q59] 分组内累计
来源：http://qmh.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ynn.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://vlx.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sqb.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oqs.shangyingyoupin.top

[Q61] 移动平均
来源：http://eyb.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pak.mhx1999.top

[Q62] 分组占比
来源：http://ift.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vmf.hammf.cn

[Q63] 开启事务
来源：http://clj.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cef.ctjpmb.com

[Q64] 提交事务
来源：http://ggy.mhx1999.top

COMMIT;
来源：http://xmu.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://jmq.sysykeji.top

ROLLBACK;
来源：http://htz.zhijiandao.cn

[Q66] 行锁查询
来源：http://yvg.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://juf.fzhhl.top

[Q67] 设置隔离级别
来源：http://ilk.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ces.jianghu66.top

[Q68] 保存点
来源：http://saq.tanke756.top

SAVEPOINT sp1;
来源：http://qdp.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://ypr.ctjpmb.com

[Q69] 查看执行计划
来源：http://fzz.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tyq.sjlbkw.cn

[Q70] 更新统计信息
来源：http://lsv.zhengqikj.top

ANALYZE TABLE users;
来源：http://nta.zhongyouzk.top

[Q71] 查看建表语句
来源：http://ith.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://anr.jianghu66.top

[Q72] 查看索引
来源：http://asa.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://lxn.gotoacloud.top

[Q73] 查看表状态
来源：http://ptq.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tqu.haohaochexian.top

[Q74] 强制使用索引
来源：http://quv.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://siz.tarul.cn

[Q75] 日期格式化
来源：http://tvu.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eaz.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://euk.wangdashe.top

[Q76] 按天统计
来源：http://kub.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://enb.hesvh.cn

[Q77] 时间加减
来源：http://gti.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eia.jqgfzy.top

[Q78] 当前时间
来源：http://xhl.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fqz.jqgufenzy.top

[Q79] 字符串拼接
来源：http://qzx.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wba.hesvh.cn

[Q80] 字符串截取
来源：http://apt.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ona.hcnkem.com

[Q81] 字符串替换
来源：http://wyb.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ywf.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://spe.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xiw.jyoumei.cn

[Q83] 大小写转换
来源：http://rij.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dfp.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://ixs.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://jzv.zhijiandao.cn

[Q85] 数值取整
来源：http://uyu.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rxc.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://yvw.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ocp.cucudq.cn

[Q87] JSON 字段做条件
来源：http://spd.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://djf.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://ffh.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://igv.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ahs.hywenlv.cn

[Q89] 判断表是否存在
来源：http://pea.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://myz.ehwqpu.com

[Q90] 生成序号列
来源：http://ypj.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ueo.hfpthk.cn

================================================================================
来源：http://bpp.nanxinkj.top

R. Bash 专题
来源：http://dlk.52xcode.cn

================================================================================
来源：http://dai.ctjpmb.com

[R01] shebang 与严格模式
来源：http://ryi.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://usu.chenzaomai.com

set -euo pipefail
来源：http://mkw.fzhhl.top

[R02] 变量赋值与使用
来源：http://cae.wangdashe.top

name="Tom"; echo "$name"
来源：http://gra.zycfv.cn

[R03] 只读变量
来源：http://zrt.jinghuilouyu.cn

readonly PI=3.14
来源：http://wrr.havefunace.top

[R04] 位置参数
来源：http://bti.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lkv.yonumen.top

[R05] 参数默认值
来源：http://sxd.0kj1m.cn

name="${1:-default}"
来源：http://gxt.9152youxi.cn

[R06] 判断命令是否存在
来源：http://rzs.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uwk.0kj1m.cn

[R07] if 判断文件
来源：http://pop.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jfg.hnqzz.top

[R08] 数值比较
来源：http://oss.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://rqj.epnwcf.com

[R09] 字符串比较
来源：http://tzf.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ugf.sufxvd.cn

[R10] 正则匹配
来源：http://mun.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qzy.shanyushiyangtech.top

[R11] case 多分支
来源：http://qzu.fanxiaobao.xyz

case "$1" in
来源：http://rpx.chenzaomai.com

start) echo "启动" ;;
来源：http://nqb.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://zew.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://ajb.wangdashe.top

esac
来源：http://lyy.tian-w.cn

[R12] for 遍历文件
来源：http://jev.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://mby.epnwcf.com

[R13] for 计数循环
来源：http://eyr.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://jzt.andypj.xyz

[R14] C 风格 for
来源：http://mzm.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uwp.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://umh.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kae.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://qrv.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ejl.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://igd.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://xua.kuanghao11.cn

[R18] 遍历数组
来源：http://cag.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kmk.hnqzz.top

[R19] 数组长度
来源：http://cmh.hesvh.cn

echo "${#arr[@]}"
来源：http://qfx.vehdjk.com

[R20] 关联数组（字典）
来源：http://uok.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://voh.vehdjk.com

[R21] 字符串长度
来源：http://orn.wangshuangyany.cn

echo "${#s}"
来源：http://ffx.fehbvm.com

[R22] 截取子串
来源：http://ply.gogol.net.cn

echo "${s:0:5}"
来源：http://tef.redwolf501.top

[R23] 字符串替换
来源：http://zkc.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gea.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://xir.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vwo.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://hds.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pfl.sxryk.cn

[R26] 命令替换
来源：http://fnc.meibo888.top

now=$(date +%F); echo "$now"
来源：http://lyz.316326.xyz

[R27] 算术展开
来源：http://jfr.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://txe.sufxvd.cn

[R28] 浮点运算
来源：http://gpp.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://lgu.bbcook.cn

[R29] 定义函数
来源：http://jnu.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xlk.jinqigfzy.top

[R30] 函数返回状态码
来源：http://zuj.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://iog.hammf.cn

[R31] 局部变量
来源：http://nar.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://lai.shzxlz.cn

[R32] 参数个数校验
来源：http://phj.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bzf.yongpay.top

[R33] 捕获错误并提示行号
来源：http://fhl.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wij.jinghuilouyu.cn

[R34] 退出时清理
来源：http://rap.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://agz.yfazqb.com

[R35] 后台执行并等待
来源：http://bwt.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gdj.aizwys.cn

[R36] 并发执行多个任务
来源：http://vlk.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aol.tarul.cn

[R37] 把输出赋给变量
来源：http://hww.ydjk.org.cn


<!-- 参考信息 -->