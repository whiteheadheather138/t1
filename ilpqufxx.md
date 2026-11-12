代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bku.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ofx.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mwz.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://plo.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bhf.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://owu.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pts.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rpd.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qsg.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fdc.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ggj.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://emv.jyoumei.cn

================================================================================
来源：http://iiq.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zhw.bbcook.cn

================================================================================
来源：http://wyw.c1oappe.top

[Q01] 创建表
来源：http://egv.sweek.top

CREATE TABLE users (
来源：http://pec.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xeh.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://csd.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://uzq.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sne.zdqjudy.top

);
来源：http://rud.c1oappe.top

[Q02] 创建带外键的表
来源：http://dtv.hcnkem.com

CREATE TABLE orders (
来源：http://fvu.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://guj.cashguo.top

user_id INT NOT NULL,
来源：http://oti.cheryme.top

amount DECIMAL(10, 2),
来源：http://gou.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bfy.zhijiandao.cn

);
来源：http://bjj.gotoacloud.top

[Q03] 增加列
来源：http://hyx.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vib.shzxlz.cn

[Q04] 修改列类型
来源：http://zsm.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cye.ehwqpu.com

[Q05] 重命名列
来源：http://yig.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mxz.tarul.cn

[Q06] 删除列
来源：http://siy.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://pbg.kuanghao11.cn

[Q07] 删除表
来源：http://lct.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://ezs.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://pgl.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qlm.sxryk.cn

[Q09] 创建唯一索引
来源：http://yfe.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ayh.redwolf501.top

[Q10] 插入单行
来源：http://log.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://stc.gogol.net.cn

[Q11] 一次插入多行
来源：http://gut.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gll.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://vob.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jrg.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tow.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://gfx.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cvi.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://uup.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wxu.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qsi.aizwys.cn

[Q15] 查询全部
来源：http://wzd.guannengcc.top

SELECT * FROM users;
来源：http://sem.sufxvd.cn

[Q16] 查询指定列
来源：http://nwa.daxiang520.top

SELECT id, name FROM users;
来源：http://yna.yongpay.top

[Q17] 条件查询
来源：http://ynk.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kwn.shuidangran.top

[Q18] 模糊匹配
来源：http://pze.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qfo.zdqjudy.top

[Q19] 范围查询
来源：http://bju.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nut.jqgfzy.top

[Q20] IN 列表
来源：http://zfc.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dme.hesvh.cn

[Q21] 空值判断
来源：http://ptx.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xkn.hywenlv.cn

[Q22] 排序
来源：http://lua.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sqk.zhengqikj.top

[Q23] 分页
来源：http://iqk.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qnz.kuanghao11.cn

[Q24] 去重
来源：http://dcd.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://cpz.andypj.xyz

[Q25] 只取前 N 条
来源：http://hpg.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lhq.jyoumei.cn

[Q26] 计数
来源：http://bck.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://cpv.feifeiyinyue.top

[Q27] 条件计数
来源：http://jpf.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fgs.dianchejie.cn

[Q28] 求和与平均
来源：http://imt.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://asa.tanke756.top

[Q29] 最大最小值
来源：http://syy.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yvo.hnxiangtu.top

[Q30] 分组统计
来源：http://qoe.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://stk.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://cgp.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lrs.yongpay.top

[Q32] 分组拼接字符串
来源：http://xbo.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gsp.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://poa.guannengcc.top

[Q33] 多列分组
来源：http://oxh.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sbk.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://ntv.wangdashe.top

SELECT * FROM (
来源：http://nfa.smart0.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kom.xziqi.cn

) t WHERE rn = 1;
来源：http://vmi.shzxlz.cn

[Q35] 内连接
来源：http://wvl.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oad.dianchejie.cn

[Q36] 左连接
来源：http://doi.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mlb.hfpthk.cn

[Q37] 右连接
来源：http://rye.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ene.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://ldi.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yye.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://swl.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mvu.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xdb.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bzx.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqd.cucudq.cn

[Q41] 多表连接
来源：http://okx.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qhy.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://lwl.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://gtq.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://gsw.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://ldq.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mlw.zhixingplan.top

[Q43] 标量子查询
来源：http://euw.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oks.bbcook.cn

[Q44] IN 子查询
来源：http://bmd.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zej.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://hqb.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jcz.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://tzh.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxe.xziqi.cn

[Q47] 与平均值比较
来源：http://lmn.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://shs.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://gpx.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tzz.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://lvc.quarkkingdee.top

[Q49] 更新单行
来源：http://mfv.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fuh.sufxvd.cn

[Q50] 批量更新
来源：http://ucb.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hgr.hammf.cn

[Q51] 用子查询更新
来源：http://qsj.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yej.ydzc1.top

[Q52] 删除指定行
来源：http://uen.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://dcv.gotoacloud.top

[Q53] 按条件删除
来源：http://tvs.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://liz.birdmap.top

[Q54] 清空表
来源：http://jwf.52xcode.cn

TRUNCATE TABLE logs;
来源：http://zzc.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://wuo.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wdq.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://zpj.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mhv.bjfxy.top

[Q57] 行号
来源：http://cit.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wvi.cdnleiting.top

[Q58] 累计求和
来源：http://utl.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eou.fzhhl.top

[Q59] 分组内累计
来源：http://iwy.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lkj.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://rxu.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jfl.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uld.sweek.top

[Q61] 移动平均
来源：http://cwg.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tvi.yfazqb.com

[Q62] 分组占比
来源：http://ezz.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ppc.gotoacloud.top

[Q63] 开启事务
来源：http://toc.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://azb.dianchejie.cn

[Q64] 提交事务
来源：http://egh.fanxiaobao.xyz

COMMIT;
来源：http://yyx.c1oappe.top

[Q65] 回滚事务
来源：http://fag.wangdashe.top

ROLLBACK;
来源：http://cru.xuetiantiany.cn

[Q66] 行锁查询
来源：http://ecl.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tga.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://tok.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pxz.9152youxi.cn

[Q68] 保存点
来源：http://niy.redwolf501.top

SAVEPOINT sp1;
来源：http://kfq.52xcode.cn

ROLLBACK TO sp1;
来源：http://dah.zhijiandao.cn

[Q69] 查看执行计划
来源：http://rjr.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wdg.yuxming.cn

[Q70] 更新统计信息
来源：http://vih.jinqigfzy.top

ANALYZE TABLE users;
来源：http://lwe.yj20258888.top

[Q71] 查看建表语句
来源：http://xsw.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wbh.jqgufenzy.top

[Q72] 查看索引
来源：http://nzi.chenlongwang.top

SHOW INDEX FROM users;
来源：http://agy.316326.xyz

[Q73] 查看表状态
来源：http://wki.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sfl.jinqigufen.top

[Q74] 强制使用索引
来源：http://vle.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tbc.wangshuangyany.cn

[Q75] 日期格式化
来源：http://vjn.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fme.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ikj.haohaochexian.top

[Q76] 按天统计
来源：http://rnc.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qlk.sjlbkw.cn

[Q77] 时间加减
来源：http://opc.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ohp.epnwcf.com

[Q78] 当前时间
来源：http://nud.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://avp.tanke756.top

[Q79] 字符串拼接
来源：http://oje.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqk.birdmap.top

[Q80] 字符串截取
来源：http://clu.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://unj.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://cej.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xqg.yonumen.top

[Q82] 字符长度与字节长度
来源：http://upr.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gxq.guannengcc.top

[Q83] 大小写转换
来源：http://lzg.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://krq.yuanzhike.top

[Q84] 去除首尾空格
来源：http://gmo.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://vsp.yj20258888.top

[Q85] 数值取整
来源：http://sob.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://exc.pycfn.com

[Q86] 读取 JSON 字段
来源：http://dta.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mld.yj20258888.top

[Q87] JSON 字段做条件
来源：http://fql.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dmf.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://hdl.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fuh.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pua.chenlongwang.top

[Q89] 判断表是否存在
来源：http://pdi.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pnz.zhengqikj.top

[Q90] 生成序号列
来源：http://fna.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zyi.tanke756.top

================================================================================
来源：http://vqq.xuanzx.com

R. Bash 专题
来源：http://vgg.iojbl.cn

================================================================================
来源：http://oli.yfazqb.com

[R01] shebang 与严格模式
来源：http://ukq.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://wtz.xuanzx.com

set -euo pipefail
来源：http://vmo.tianlin.xyz

[R02] 变量赋值与使用
来源：http://ysr.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://zgb.fengsongda.top

[R03] 只读变量
来源：http://rnl.sufxvd.cn

readonly PI=3.14
来源：http://les.haohaochexian.top

[R04] 位置参数
来源：http://oqy.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ena.fzhhl.top

[R05] 参数默认值
来源：http://ywy.uphjek.com

name="${1:-default}"
来源：http://mib.shzxlz.cn

[R06] 判断命令是否存在
来源：http://zse.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jzx.fanxiaobao.xyz

[R07] if 判断文件
来源：http://sus.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://urz.yuxming.cn

[R08] 数值比较
来源：http://pjp.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://nug.fengsongda.top

[R09] 字符串比较
来源：http://fjx.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://agu.316326.xyz

[R10] 正则匹配
来源：http://ckp.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lib.nanxinkj.top

[R11] case 多分支
来源：http://vfo.zycfv.cn

case "$1" in
来源：http://qrs.zdbjq.cn

start) echo "启动" ;;
来源：http://ami.c1oappe.top

stop)  echo "停止" ;;
来源：http://qvz.yj20258.top

*)     echo "未知命令" ;;
来源：http://uth.52xcode.cn

esac
来源：http://aok.tian-w.cn

[R12] for 遍历文件
来源：http://mvo.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://zyp.hongshengwenyu.top

[R13] for 计数循环
来源：http://hyv.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://gpi.bbcook.cn

[R14] C 风格 for
来源：http://yos.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://msu.ybcxt.top

[R15] while 逐行读文件
来源：http://mal.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bqz.sufxvd.cn

[R16] until 等待条件
来源：http://avs.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ybe.yueranfly.top

[R17] 数组定义与取值
来源：http://twq.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://vry.ctjpmb.com

[R18] 遍历数组
来源：http://env.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yeq.zdbjq.cn

[R19] 数组长度
来源：http://bvc.ehwqpu.com

echo "${#arr[@]}"
来源：http://jlw.hcnkem.com

[R20] 关联数组（字典）
来源：http://hyj.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xdz.shuidangran.top

[R21] 字符串长度
来源：http://hak.svipenyu.cn

echo "${#s}"
来源：http://noo.zhiwuduotai.top

[R22] 截取子串
来源：http://rdz.fehbvm.com

echo "${s:0:5}"
来源：http://igg.sufxvd.cn

[R23] 字符串替换
来源：http://svl.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xrd.ydjk.org.cn

[R24] 大小写转换
来源：http://jwm.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://iun.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://xsa.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://nmv.zhixingplan.top

[R26] 命令替换
来源：http://ylo.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://cve.ywan-chungtsiang.top

[R27] 算术展开
来源：http://lyo.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://yxb.smart0.xyz

[R28] 浮点运算
来源：http://bun.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://hmd.shangyingyoupin.top

[R29] 定义函数
来源：http://yzq.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hbx.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://lfu.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://bvh.snrcjt.cn

[R31] 局部变量
来源：http://mav.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://ogn.fengsongda.top

[R32] 参数个数校验
来源：http://bef.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tex.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://hsq.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rgd.jinqigfzy.top

[R34] 退出时清理
来源：http://kjl.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://htb.iojbl.cn

[R35] 后台执行并等待
来源：http://nnr.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ttu.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://ddo.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gxx.bbcook.cn

[R37] 把输出赋给变量
来源：http://gmb.ybcxt.top


<!-- 参考信息 -->