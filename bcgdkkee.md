代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xcj.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cgo.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://imk.yueranfly.top

[P08] 处理浮点精度问题
来源：http://dzd.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bkt.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://slv.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://als.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzi.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kte.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qra.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eaf.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yaz.mhx1999.top

================================================================================
来源：http://nuv.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dyf.epnwcf.com

================================================================================
来源：http://dbd.wangshuangyany.cn

[Q01] 创建表
来源：http://gqz.hnqzz.top

CREATE TABLE users (
来源：http://uaf.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tce.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://dli.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://xdy.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://koh.ppjwa.cn

);
来源：http://tav.nwbrower.top

[Q02] 创建带外键的表
来源：http://qfe.xziqi.cn

CREATE TABLE orders (
来源：http://eux.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://noh.jqgfzy.top

user_id INT NOT NULL,
来源：http://bib.wangdashe.top

amount DECIMAL(10, 2),
来源：http://tbk.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tsy.mhx1999.top

);
来源：http://zmb.tian-w.cn

[Q03] 增加列
来源：http://slg.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjr.sysykeji.top

[Q04] 修改列类型
来源：http://xuz.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mcr.meibo888.top

[Q05] 重命名列
来源：http://ebp.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jxy.zhijiandao.cn

[Q06] 删除列
来源：http://dbs.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jht.yfazqb.com

[Q07] 删除表
来源：http://wtf.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://jib.guowangkeji.top

[Q08] 创建普通索引
来源：http://cfz.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nrb.vehdjk.com

[Q09] 创建唯一索引
来源：http://aks.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gsr.zhongyouzk.top

[Q10] 插入单行
来源：http://tsn.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wkz.hammf.cn

[Q11] 一次插入多行
来源：http://vxb.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iph.uphjek.com

[Q12] 插入后取自增 ID
来源：http://www.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://qha.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ysh.yuxming.cn

[Q13] 忽略重复插入
来源：http://qcv.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sax.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://xvu.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://azq.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsv.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://euw.gzhubu.top

SELECT * FROM users;
来源：http://fen.xylfe.cn

[Q16] 查询指定列
来源：http://uph.cheryme.top

SELECT id, name FROM users;
来源：http://ovf.daria6918.cn

[Q17] 条件查询
来源：http://mnu.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cnt.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://duh.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqw.fehbvm.com

[Q19] 范围查询
来源：http://iqp.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gbq.yj20258.top

[Q20] IN 列表
来源：http://wor.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dgz.yfazqb.com

[Q21] 空值判断
来源：http://eth.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://clo.shangyingyoupin.top

[Q22] 排序
来源：http://ivn.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rxe.sysykeji.top

[Q23] 分页
来源：http://aul.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvd.daria6918.cn

[Q24] 去重
来源：http://asg.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://vtk.fzhhl.top

[Q25] 只取前 N 条
来源：http://ozj.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wau.yangfankeji.com

[Q26] 计数
来源：http://oxo.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://gbw.havefunace.top

[Q27] 条件计数
来源：http://ejn.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ote.shzxlz.cn

[Q28] 求和与平均
来源：http://bdq.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rgo.hfpthk.cn

[Q29] 最大最小值
来源：http://dgv.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jmj.daria6918.cn

[Q30] 分组统计
来源：http://vyr.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wmo.xinyue.icu

[Q31] 分组后过滤
来源：http://laq.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xvm.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://sss.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gbx.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zvp.vqdsnc.cn

[Q33] 多列分组
来源：http://kcw.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jkt.0kj1m.cn

[Q34] 每组取第一条
来源：http://isa.jinqigufen.top

SELECT * FROM (
来源：http://vsa.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jah.hammf.cn

) t WHERE rn = 1;
来源：http://jse.shanyushiyangkeji.top

[Q35] 内连接
来源：http://umy.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hkz.hysaishi.cn

[Q36] 左连接
来源：http://mel.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wzg.hfpthk.cn

[Q37] 右连接
来源：http://gyu.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iiy.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dpn.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://atm.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://elu.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://enc.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kds.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nom.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgu.fengsongda.top

[Q41] 多表连接
来源：http://dwv.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kfa.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://dwx.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://jxn.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://jdb.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://gns.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ift.ehwqpu.com

[Q43] 标量子查询
来源：http://khc.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://twj.svipenyu.cn

[Q44] IN 子查询
来源：http://hpv.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nho.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://hkz.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gev.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wwc.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exs.aizwys.cn

[Q47] 与平均值比较
来源：http://xrg.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yxf.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://waf.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wiw.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://tqc.ydjk.org.cn

[Q49] 更新单行
来源：http://taw.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://era.birdmap.top

[Q50] 批量更新
来源：http://iyq.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kre.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://cmv.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jjx.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://fll.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://fji.hcnkem.com

[Q53] 按条件删除
来源：http://kxm.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://shx.yuxming.cn

[Q54] 清空表
来源：http://cjq.hammf.cn

TRUNCATE TABLE logs;
来源：http://evt.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://kgk.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sty.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://zgj.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xxu.bbcook.cn

[Q57] 行号
来源：http://ayq.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eeo.52xcode.cn

[Q58] 累计求和
来源：http://wcv.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dbp.fengsongda.top

[Q59] 分组内累计
来源：http://mak.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tky.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://uzc.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qrv.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gho.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://hnx.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rnw.c1oappe.top

[Q62] 分组占比
来源：http://tgj.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ooz.svipenyu.cn

[Q63] 开启事务
来源：http://fgb.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wlt.yj202588.top

[Q64] 提交事务
来源：http://hcg.shanyushiyangkeji.top

COMMIT;
来源：http://odv.jiagoushi.top

[Q65] 回滚事务
来源：http://sbw.pycfn.com

ROLLBACK;
来源：http://ids.guowangkeji.top

[Q66] 行锁查询
来源：http://qaq.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hsb.guowangkeji.top

[Q67] 设置隔离级别
来源：http://mfg.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iio.jianghu66.top

[Q68] 保存点
来源：http://zwq.quarkkingdee.top

SAVEPOINT sp1;
来源：http://nho.hammf.cn

ROLLBACK TO sp1;
来源：http://ens.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://qqj.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ave.shuidangran.top

[Q70] 更新统计信息
来源：http://rln.jqgufenzy.top

ANALYZE TABLE users;
来源：http://ami.sxryk.cn

[Q71] 查看建表语句
来源：http://lmy.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dmv.gzhubu.top

[Q72] 查看索引
来源：http://svz.cdnleiting.top

SHOW INDEX FROM users;
来源：http://irp.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://wwm.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kua.svipenyu.cn

[Q74] 强制使用索引
来源：http://voi.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ffr.kuanghao11.cn

[Q75] 日期格式化
来源：http://ivg.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://edg.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ydz.jinghuilouyu.cn

[Q76] 按天统计
来源：http://bbx.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ohk.birdmap.top

[Q77] 时间加减
来源：http://iwe.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yak.jyoumei.cn

[Q78] 当前时间
来源：http://wez.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://myv.chenlongwang.top

[Q79] 字符串拼接
来源：http://vmq.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ihc.sxryk.cn

[Q80] 字符串截取
来源：http://lcf.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pba.daria6918.cn

[Q81] 字符串替换
来源：http://qjr.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cfy.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://hcc.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://waz.nanxuanxn.top

[Q83] 大小写转换
来源：http://dbv.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zmf.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://zdd.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://yti.bjfxy.top

[Q85] 数值取整
来源：http://aeh.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lmc.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://dow.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dye.havefunace.top

[Q87] JSON 字段做条件
来源：http://cro.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eyi.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://mpr.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xcq.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ocp.ydzc1.top

[Q89] 判断表是否存在
来源：http://yxx.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uwy.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://ezv.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wdu.uphjek.com

================================================================================
来源：http://ygr.tian-w.cn

R. Bash 专题
来源：http://prm.zhijiandao.cn

================================================================================
来源：http://vxr.yj20258888.top

[R01] shebang 与严格模式
来源：http://fqj.hnqzz.top

#!/usr/bin/env bash
来源：http://ppc.zhongyouzk.top

set -euo pipefail
来源：http://gzs.tianlin.xyz

[R02] 变量赋值与使用
来源：http://bwj.ybcxt.top

name="Tom"; echo "$name"
来源：http://ukl.jqgfzy.top

[R03] 只读变量
来源：http://utt.chenlongwang.top

readonly PI=3.14
来源：http://ymb.bjfxy.top

[R04] 位置参数
来源：http://fdc.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://utf.shuidangran.top

[R05] 参数默认值
来源：http://wko.guannengcc.top

name="${1:-default}"
来源：http://klm.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://yyz.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcm.jiagoushi.top

[R07] if 判断文件
来源：http://jwg.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhx.zhengqikj.top

[R08] 数值比较
来源：http://bkp.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cxt.0kj1m.cn

[R09] 字符串比较
来源：http://rtm.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ayd.xuetiantiany.cn

[R10] 正则匹配
来源：http://ait.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://poc.aibaodan.cn

[R11] case 多分支
来源：http://xya.daria6918.cn

case "$1" in
来源：http://lzo.cucudq.cn

start) echo "启动" ;;
来源：http://yqf.zdbjq.cn

stop)  echo "停止" ;;
来源：http://cbg.fzhhl.top

*)     echo "未知命令" ;;
来源：http://prc.daxiang520.top

esac
来源：http://kxq.52xcode.cn

[R12] for 遍历文件
来源：http://bhs.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://gbg.vqdsnc.cn

[R13] for 计数循环
来源：http://wwn.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://pga.9152youxi.cn

[R14] C 风格 for
来源：http://ker.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rll.ydjk.org.cn

[R15] while 逐行读文件
来源：http://xgi.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://inc.daxiang520.top

[R16] until 等待条件
来源：http://wiv.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vut.ydjk.org.cn

[R17] 数组定义与取值
来源：http://zoe.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://qjr.chenlongwang.top

[R18] 遍历数组
来源：http://zbw.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dew.cdnleiting.top

[R19] 数组长度
来源：http://ukf.ctjpmb.com

echo "${#arr[@]}"
来源：http://kxr.jianghu66.top

[R20] 关联数组（字典）
来源：http://vvn.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hel.ydjk.org.cn

[R21] 字符串长度
来源：http://twb.yuanzhike.top

echo "${#s}"
来源：http://aff.gogol.net.cn

[R22] 截取子串
来源：http://qiu.pycfn.com

echo "${s:0:5}"
来源：http://tty.andypj.xyz

[R23] 字符串替换
来源：http://pqy.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pjr.jqgufenzy.top

[R24] 大小写转换
来源：http://zpx.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://edk.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://eio.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nvb.sweek.top

[R26] 命令替换
来源：http://odq.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://iga.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://gqm.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://zkv.zycfv.cn

[R28] 浮点运算
来源：http://had.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://zke.pengpengdd.cyou

[R29] 定义函数
来源：http://zuw.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://etv.hesvh.cn

[R30] 函数返回状态码
来源：http://ttb.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://xmw.ybcxt.top

[R31] 局部变量
来源：http://qpo.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://ahp.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://dew.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xmj.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://ncg.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hbe.vehdjk.com

[R34] 退出时清理
来源：http://err.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nke.uphjek.com

[R35] 后台执行并等待
来源：http://gbd.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://kxe.aibaodan.cn

[R36] 并发执行多个任务
来源：http://dju.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yod.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://xkn.ehwqpu.com


<!-- 参考信息 -->