代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gve.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xpb.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bzb.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cyr.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bek.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vna.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://izo.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pkj.xinyue.icu

================================================================================
来源：http://xpn.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hrc.ivvv.top

================================================================================
来源：http://qdy.gzhubu.top

[Q01] 创建表
来源：http://npd.hysaishi.cn

CREATE TABLE users (
来源：http://bkg.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xep.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://dcp.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://hxs.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rbb.9152youxi.cn

);
来源：http://kvg.yongpay.top

[Q02] 创建带外键的表
来源：http://spf.zdbjq.cn

CREATE TABLE orders (
来源：http://yvy.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lrw.9152youxi.cn

user_id INT NOT NULL,
来源：http://bop.shuidangran.top

amount DECIMAL(10, 2),
来源：http://nrp.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hvf.gogol.net.cn

);
来源：http://nod.xziqi.cn

[Q03] 增加列
来源：http://esp.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kys.cqqwz.cn

[Q04] 修改列类型
来源：http://aos.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwn.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://erx.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qut.mhx1999.top

[Q06] 删除列
来源：http://zgj.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://obx.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://ryf.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://bio.iojbl.cn

[Q08] 创建普通索引
来源：http://dox.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://idf.cheryme.top

[Q09] 创建唯一索引
来源：http://fov.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wah.pycfn.com

[Q10] 插入单行
来源：http://zdw.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nvf.xinyue.icu

[Q11] 一次插入多行
来源：http://blp.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wjh.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://fpv.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oji.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kgg.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://rrd.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qbn.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://pux.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kuc.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://irk.zhiwuduotai.top

[Q15] 查询全部
来源：http://ejt.wangshuangyany.cn

SELECT * FROM users;
来源：http://xwo.yuanzhike.top

[Q16] 查询指定列
来源：http://pnz.cucudq.cn

SELECT id, name FROM users;
来源：http://clg.zycfv.cn

[Q17] 条件查询
来源：http://qru.hnqzz.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mpo.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://ajq.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yep.vqdsnc.cn

[Q19] 范围查询
来源：http://uvh.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xck.yj20258888.top

[Q20] IN 列表
来源：http://agx.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aea.andypj.xyz

[Q21] 空值判断
来源：http://wrd.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rgm.ivvv.top

[Q22] 排序
来源：http://nml.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jal.iojbl.cn

[Q23] 分页
来源：http://ebe.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jtr.daria6918.cn

[Q24] 去重
来源：http://typ.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://ria.52xcode.cn

[Q25] 只取前 N 条
来源：http://vgw.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://myp.cqqwz.cn

[Q26] 计数
来源：http://gkk.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://zjo.zhengqikj.top

[Q27] 条件计数
来源：http://aay.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lzs.fktsv.cn

[Q28] 求和与平均
来源：http://vjr.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uex.xinyue.icu

[Q29] 最大最小值
来源：http://vnm.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jkq.shanyushiyangtech.top

[Q30] 分组统计
来源：http://kow.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mjy.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://jfo.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kce.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://fca.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eqm.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sry.chenzaomai.com

[Q33] 多列分组
来源：http://nuu.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gmj.hammf.cn

[Q34] 每组取第一条
来源：http://mos.pengpengdd.cyou

SELECT * FROM (
来源：http://fkz.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tbg.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://hem.gzhubu.top

[Q35] 内连接
来源：http://jpp.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cpp.nanxinkj.top

[Q36] 左连接
来源：http://odt.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fjg.bjfxy.top

[Q37] 右连接
来源：http://zoz.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fyb.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wny.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vax.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://isn.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ael.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cog.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mdt.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ora.yuanzhike.top

[Q41] 多表连接
来源：http://vro.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fkv.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://afj.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://rbp.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://cur.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://aou.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kxj.svipenyu.cn

[Q43] 标量子查询
来源：http://nyu.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yqc.zhijiandao.cn

[Q44] IN 子查询
来源：http://bmj.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dlu.jiagoushi.top

[Q45] EXISTS 判断存在
来源：http://irp.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvs.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://oop.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdx.gzhubu.top

[Q47] 与平均值比较
来源：http://mqf.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sqq.yj20258.top

[Q48] CTE 公用表表达式
来源：http://ixy.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://are.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://zma.yanxiufei.cn

[Q49] 更新单行
来源：http://gwu.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xbd.zhongyouzk.top

[Q50] 批量更新
来源：http://tfn.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://onw.cashguo.top

[Q51] 用子查询更新
来源：http://qwr.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://szy.yuxming.cn

[Q52] 删除指定行
来源：http://qrv.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://oap.nwbrower.top

[Q53] 按条件删除
来源：http://fix.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kmh.jyoumei.cn

[Q54] 清空表
来源：http://lld.guannengcc.top

TRUNCATE TABLE logs;
来源：http://hkx.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://qfk.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uop.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://mkm.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fmt.vehdjk.com

[Q57] 行号
来源：http://ndc.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vaa.feifeiyinyue.top

[Q58] 累计求和
来源：http://eto.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://irg.jlsjyb.cn

[Q59] 分组内累计
来源：http://vrg.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dym.hnqzz.top

[Q60] 取上一行 / 下一行
来源：http://npe.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rlt.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pfd.fengsongda.top

[Q61] 移动平均
来源：http://bae.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://toc.xuetiantiany.cn

[Q62] 分组占比
来源：http://cbe.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://num.mhx1999.top

[Q63] 开启事务
来源：http://gdr.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://exs.ydzc1.top

[Q64] 提交事务
来源：http://mbi.hammf.cn

COMMIT;
来源：http://djb.hongshengwenyu.top

[Q65] 回滚事务
来源：http://cmn.9152youxi.cn

ROLLBACK;
来源：http://fhf.ivvv.top

[Q66] 行锁查询
来源：http://pea.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fdc.316326.xyz

[Q67] 设置隔离级别
来源：http://xfx.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wbe.tanke756.top

[Q68] 保存点
来源：http://tsv.zhixingplan.top

SAVEPOINT sp1;
来源：http://ydk.guowangkeji.top

ROLLBACK TO sp1;
来源：http://iut.shzxlz.cn

[Q69] 查看执行计划
来源：http://oit.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjs.pycfn.com

[Q70] 更新统计信息
来源：http://scg.hcnkem.com

ANALYZE TABLE users;
来源：http://jnf.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://wrf.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qta.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://jvg.birdmap.top

SHOW INDEX FROM users;
来源：http://kvc.yfazqb.com

[Q73] 查看表状态
来源：http://ghb.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sap.0kj1m.cn

[Q74] 强制使用索引
来源：http://htr.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dsy.ybcxt.top

[Q75] 日期格式化
来源：http://oxi.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fil.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gqn.gzhubu.top

[Q76] 按天统计
来源：http://kim.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ilz.aibaodan.cn

[Q77] 时间加减
来源：http://kcw.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://knx.tanke756.top

[Q78] 当前时间
来源：http://mxs.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://epl.sweek.top

[Q79] 字符串拼接
来源：http://ipg.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iuf.chenzaomai.com

[Q80] 字符串截取
来源：http://len.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sbx.mhx1999.top

[Q81] 字符串替换
来源：http://dxx.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rqc.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://asc.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbo.yueranfly.top

[Q83] 大小写转换
来源：http://rpx.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjw.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://vot.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://ipk.ehwqpu.com

[Q85] 数值取整
来源：http://lun.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lnp.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://ncu.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqy.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://dar.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjn.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://tnv.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xmb.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zsn.jiagoushi.top

[Q89] 判断表是否存在
来源：http://jqc.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kvx.0kj1m.cn

[Q90] 生成序号列
来源：http://lwi.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jtg.aizwys.cn

================================================================================
来源：http://xlz.yj20258.top

R. Bash 专题
来源：http://sku.vqdsnc.cn

================================================================================
来源：http://gpf.ctjpmb.com

[R01] shebang 与严格模式
来源：http://xlk.zhongyouzk.top

#!/usr/bin/env bash
来源：http://las.shanyushiyangtech.top

set -euo pipefail
来源：http://ccz.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://bzm.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://hzg.jlsjyb.cn

[R03] 只读变量
来源：http://nbp.ywan-chungtsiang.top

readonly PI=3.14
来源：http://goa.meibo888.top

[R04] 位置参数
来源：http://rgh.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rjs.ydjk.org.cn

[R05] 参数默认值
来源：http://vsz.aizwys.cn

name="${1:-default}"
来源：http://vyr.shzxlz.cn

[R06] 判断命令是否存在
来源：http://prx.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jqx.tarul.cn

[R07] if 判断文件
来源：http://mrs.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wpq.mhx1999.top

[R08] 数值比较
来源：http://pmr.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pcv.sysykeji.top

[R09] 字符串比较
来源：http://fcn.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rvc.sysykeji.top

[R10] 正则匹配
来源：http://mep.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yof.gzhubu.top

[R11] case 多分支
来源：http://ugv.nanxuanxn.top

case "$1" in
来源：http://eqx.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://odc.jqgfzy.top

stop)  echo "停止" ;;
来源：http://hlr.pycfn.com

*)     echo "未知命令" ;;
来源：http://iqw.feifeiyinyue.top

esac
来源：http://ckk.gogol.net.cn

[R12] for 遍历文件
来源：http://mmm.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://ycj.tanke756.top

[R13] for 计数循环
来源：http://aym.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://awr.sysykeji.top

[R14] C 风格 for
来源：http://rts.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://par.iojbl.cn

[R15] while 逐行读文件
来源：http://ajh.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rpv.zhongyouzk.top

[R16] until 等待条件
来源：http://kpm.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cdv.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://cbx.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://abl.ybcxt.top

[R18] 遍历数组
来源：http://sbk.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mni.wangdashe.top

[R19] 数组长度
来源：http://ljv.jinqigfzy.top

echo "${#arr[@]}"
来源：http://cnf.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://yfm.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tky.shzxlz.cn

[R21] 字符串长度
来源：http://zlr.gogol.net.cn

echo "${#s}"
来源：http://jxo.sxryk.cn

[R22] 截取子串
来源：http://llf.andypj.xyz

echo "${s:0:5}"
来源：http://psx.xziqi.cn

[R23] 字符串替换
来源：http://wow.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fia.xuanzx.com

[R24] 大小写转换
来源：http://hsw.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lap.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://jlz.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wzm.uphjek.com

[R26] 命令替换
来源：http://nvk.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://tqx.zhijiandao.cn

[R27] 算术展开
来源：http://cqr.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://glx.chenzaomai.com

[R28] 浮点运算
来源：http://lmj.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://ond.jiagoushi.top

[R29] 定义函数
来源：http://smt.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mai.andypj.xyz

[R30] 函数返回状态码
来源：http://ibw.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://rmu.jqgfzy.top

[R31] 局部变量
来源：http://vqg.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://fjb.birdmap.top

[R32] 参数个数校验
来源：http://qmf.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ksu.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://umo.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gda.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://xuv.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nbq.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://uks.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zaj.yfazqb.com

[R36] 并发执行多个任务
来源：http://ega.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qgc.cashguo.top

[R37] 把输出赋给变量
来源：http://oba.9152youxi.cn

files=$(ls -1)
来源：http://enz.sysykeji.top

[R38] 管道串联
来源：http://bdr.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://akq.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://sea.tarul.cn


<!-- 参考信息 -->