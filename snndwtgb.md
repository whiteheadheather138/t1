代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kyn.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://isb.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eji.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ocm.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hwu.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dpq.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fgl.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://amp.yanxiufei.cn

================================================================================
来源：http://cxn.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://afv.zdbjq.cn

================================================================================
来源：http://vdp.zdbjq.cn

[Q01] 创建表
来源：http://rwo.havefunace.top

CREATE TABLE users (
来源：http://dqz.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yao.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://arp.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://nxq.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hta.ywan-chungtsiang.top

);
来源：http://ktu.fktsv.cn

[Q02] 创建带外键的表
来源：http://rne.zdqjudy.top

CREATE TABLE orders (
来源：http://jfp.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hxs.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://ggi.cucudq.cn

amount DECIMAL(10, 2),
来源：http://doi.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ncb.bjfxy.top

);
来源：http://eeh.ywan-chungtsiang.top

[Q03] 增加列
来源：http://vlf.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://coz.52xcode.cn

[Q04] 修改列类型
来源：http://yuy.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yrk.yj20258888.top

[Q05] 重命名列
来源：http://vgj.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vql.jlsjyb.cn

[Q06] 删除列
来源：http://fcq.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://htz.jqgufenzy.top

[Q07] 删除表
来源：http://tjr.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://yuo.jinqigufen.top

[Q08] 创建普通索引
来源：http://lez.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://akv.vehdjk.com

[Q09] 创建唯一索引
来源：http://oeh.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://txj.wangdashe.top

[Q10] 插入单行
来源：http://gxq.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://umt.zhijiandao.cn

[Q11] 一次插入多行
来源：http://lbv.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nfo.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://arp.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://ynz.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibr.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://yew.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fgm.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://top.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bxm.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pbq.0kj1m.cn

[Q15] 查询全部
来源：http://cln.jinqigufen.top

SELECT * FROM users;
来源：http://qut.tarul.cn

[Q16] 查询指定列
来源：http://vtv.zhongyouzk.top

SELECT id, name FROM users;
来源：http://kra.yueranfly.top

[Q17] 条件查询
来源：http://xdb.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pby.xinyue.icu

[Q18] 模糊匹配
来源：http://huk.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://joo.cqqwz.cn

[Q19] 范围查询
来源：http://hzz.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aox.316326.xyz

[Q20] IN 列表
来源：http://xmq.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qja.cashguo.top

[Q21] 空值判断
来源：http://utl.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mfq.hongshengwenyu.top

[Q22] 排序
来源：http://tup.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vqd.pengpengdd.cyou

[Q23] 分页
来源：http://nje.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gao.gzhubu.top

[Q24] 去重
来源：http://qwf.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://qvy.aibaodan.cn

[Q25] 只取前 N 条
来源：http://dif.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kjh.yangfankeji.com

[Q26] 计数
来源：http://uce.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://ppa.xuanzx.com

[Q27] 条件计数
来源：http://wwv.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yso.yuanzhike.top

[Q28] 求和与平均
来源：http://hbr.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eiq.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://deh.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fhs.havefunace.top

[Q30] 分组统计
来源：http://rqu.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ypc.wangdashe.top

[Q31] 分组后过滤
来源：http://dlo.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tez.316326.xyz

[Q32] 分组拼接字符串
来源：http://jct.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ion.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://til.quarkkingdee.top

[Q33] 多列分组
来源：http://itp.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bwp.ppjwa.cn

[Q34] 每组取第一条
来源：http://lhv.gotoacloud.top

SELECT * FROM (
来源：http://xio.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wwt.redwolf501.top

) t WHERE rn = 1;
来源：http://pkz.tarul.cn

[Q35] 内连接
来源：http://sal.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xkg.hammf.cn

[Q36] 左连接
来源：http://lfs.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://igl.hesvh.cn

[Q37] 右连接
来源：http://han.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mai.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://zwx.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://alr.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://jtd.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ewn.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zlo.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qat.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dee.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://krn.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lqj.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://nwc.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://odv.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://dwb.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://tyd.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://unb.shangyingyoupin.top

[Q43] 标量子查询
来源：http://kng.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fbd.sysykeji.top

[Q44] IN 子查询
来源：http://ckn.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wph.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://deh.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uev.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://qyy.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xru.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://jds.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://inb.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://pni.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xmp.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://ire.yfazqb.com

[Q49] 更新单行
来源：http://aix.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fqi.redwolf501.top

[Q50] 批量更新
来源：http://scr.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://djv.nwbrower.top

[Q51] 用子查询更新
来源：http://lxx.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://igz.hnxiangtu.top

[Q52] 删除指定行
来源：http://dnc.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://lwi.xuanzx.com

[Q53] 按条件删除
来源：http://uix.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wxl.daxiang520.top

[Q54] 清空表
来源：http://zbl.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://paw.fktsv.cn

[Q55] 排名（并列占位）
来源：http://fbt.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://avv.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://cck.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fiq.aizwys.cn

[Q57] 行号
来源：http://koj.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lvf.zdqjudy.top

[Q58] 累计求和
来源：http://qee.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tix.hysaishi.cn

[Q59] 分组内累计
来源：http://kll.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kua.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://gcj.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mzy.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zql.mhx1999.top

[Q61] 移动平均
来源：http://fsi.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyn.epnwcf.com

[Q62] 分组占比
来源：http://fwe.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kvl.xylfe.cn

[Q63] 开启事务
来源：http://ggz.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xms.zhongyouzk.top

[Q64] 提交事务
来源：http://kyy.shzxlz.cn

COMMIT;
来源：http://yxt.xuanzx.com

[Q65] 回滚事务
来源：http://cmg.quarkkingdee.top

ROLLBACK;
来源：http://ubz.yueranfly.top

[Q66] 行锁查询
来源：http://tre.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tnk.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://dre.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cbv.uphjek.com

[Q68] 保存点
来源：http://usc.yfazqb.com

SAVEPOINT sp1;
来源：http://ysc.cashguo.top

ROLLBACK TO sp1;
来源：http://fce.shzxlz.cn

[Q69] 查看执行计划
来源：http://xyo.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://piq.nanxuanxn.top

[Q70] 更新统计信息
来源：http://mwd.iojbl.cn

ANALYZE TABLE users;
来源：http://ihz.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://tus.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uzu.fehbvm.com

[Q72] 查看索引
来源：http://qxg.nwbrower.top

SHOW INDEX FROM users;
来源：http://wxs.fehbvm.com

[Q73] 查看表状态
来源：http://yry.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kdo.c1oappe.top

[Q74] 强制使用索引
来源：http://lmg.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://acc.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://qkj.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qnb.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jfz.sufxvd.cn

[Q76] 按天统计
来源：http://qyb.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxk.chenzaomai.com

[Q77] 时间加减
来源：http://wdi.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cpr.yfazqb.com

[Q78] 当前时间
来源：http://syq.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://neg.shzxlz.cn

[Q79] 字符串拼接
来源：http://teo.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chu.zhixingplan.top

[Q80] 字符串截取
来源：http://oir.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwo.yvedp.cn

[Q81] 字符串替换
来源：http://ixl.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ezr.havefunace.top

[Q82] 字符长度与字节长度
来源：http://vfp.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pjq.xylfe.cn

[Q83] 大小写转换
来源：http://pbm.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gxe.316326.xyz

[Q84] 去除首尾空格
来源：http://zbp.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://zlp.epnwcf.com

[Q85] 数值取整
来源：http://oxj.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hzq.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://tfh.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zrf.mhx1999.top

[Q87] JSON 字段做条件
来源：http://bau.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxx.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://exg.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://luu.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hqf.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://gbj.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ety.yj202588.top

[Q90] 生成序号列
来源：http://jhp.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nnd.uphjek.com

================================================================================
来源：http://lrh.yuxming.cn

R. Bash 专题
来源：http://hcv.gotoacloud.top

================================================================================
来源：http://qrw.snrcjt.cn

[R01] shebang 与严格模式
来源：http://nww.yj20258.top

#!/usr/bin/env bash
来源：http://icv.jiagoushi.top

set -euo pipefail
来源：http://der.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://pyj.zdbjq.cn

name="Tom"; echo "$name"
来源：http://oyz.xziqi.cn

[R03] 只读变量
来源：http://cmo.jyoumei.cn

readonly PI=3.14
来源：http://evx.fzhhl.top

[R04] 位置参数
来源：http://krc.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ygl.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://trx.cucudq.cn

name="${1:-default}"
来源：http://urr.yj20258888.top

[R06] 判断命令是否存在
来源：http://wnt.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jsh.hammf.cn

[R07] if 判断文件
来源：http://zat.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ica.redwolf501.top

[R08] 数值比较
来源：http://mse.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cjq.hcnkem.com

[R09] 字符串比较
来源：http://wim.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xsc.hcnkem.com

[R10] 正则匹配
来源：http://hxo.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yoh.nanxuanxn.top

[R11] case 多分支
来源：http://cdw.uphjek.com

case "$1" in
来源：http://cuw.feifeiyinyue.top

start) echo "启动" ;;
来源：http://iky.cheryme.top

stop)  echo "停止" ;;
来源：http://jqs.redwolf501.top

*)     echo "未知命令" ;;
来源：http://knj.tian-w.cn

esac
来源：http://nnc.andypj.xyz

[R12] for 遍历文件
来源：http://zvp.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://efz.cucudq.cn

[R13] for 计数循环
来源：http://nrv.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://rhj.hywenlv.cn

[R14] C 风格 for
来源：http://zso.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hwy.tian-w.cn

[R15] while 逐行读文件
来源：http://mit.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xmr.sxryk.cn

[R16] until 等待条件
来源：http://dfd.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jlz.yvedp.cn

[R17] 数组定义与取值
来源：http://ake.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://nlk.52xcode.cn

[R18] 遍历数组
来源：http://kpx.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fff.kuanghao11.cn

[R19] 数组长度
来源：http://vaa.kuanghao11.cn

echo "${#arr[@]}"
来源：http://sso.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://ezc.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ate.epnwcf.com

[R21] 字符串长度
来源：http://rmx.sjlbkw.cn

echo "${#s}"
来源：http://zam.havefunace.top

[R22] 截取子串
来源：http://med.zhengqikj.top

echo "${s:0:5}"
来源：http://doq.hnqzz.top

[R23] 字符串替换
来源：http://gpn.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ksz.feifeiyinyue.top

[R24] 大小写转换
来源：http://mkf.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://yzm.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://njt.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wkz.zhiwuduotai.top

[R26] 命令替换
来源：http://uvd.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://upx.uphjek.com

[R27] 算术展开
来源：http://eey.andypj.xyz

echo $((1 + 2 * 3))
来源：http://vbx.zdqjudy.top

[R28] 浮点运算
来源：http://cvu.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://ipf.ydzc1.top

[R29] 定义函数
来源：http://rni.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rkk.cdnleiting.top

[R30] 函数返回状态码
来源：http://zeh.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vlw.xuanzx.com

[R31] 局部变量
来源：http://ovh.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://jcx.gotoacloud.top

[R32] 参数个数校验
来源：http://sno.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fir.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://ltv.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dpb.jlsjyb.cn

[R34] 退出时清理
来源：http://lnt.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://vww.chenlongwang.top

[R35] 后台执行并等待
来源：http://fxk.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zmg.chenzaomai.com

[R36] 并发执行多个任务
来源：http://mig.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://web.c1oappe.top

[R37] 把输出赋给变量
来源：http://ynz.hnxiangtu.top

files=$(ls -1)
来源：http://vpd.jiagoushi.top

[R38] 管道串联
来源：http://itm.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://xee.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://wes.cdnleiting.top


<!-- 参考信息 -->