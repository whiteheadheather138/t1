代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hae.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aiv.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wxb.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eir.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mnv.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tyt.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vax.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmj.hywenlv.cn

================================================================================
来源：http://kyp.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lxq.ydjk.org.cn

================================================================================
来源：http://hpc.daria6918.cn

[Q01] 创建表
来源：http://ocw.havefunace.top

CREATE TABLE users (
来源：http://mlx.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zfm.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://sis.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://zop.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vsw.fzhhl.top

);
来源：http://gbu.yvedp.cn

[Q02] 创建带外键的表
来源：http://sgi.yangfankeji.com

CREATE TABLE orders (
来源：http://bvi.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://les.ivvv.top

user_id INT NOT NULL,
来源：http://eyw.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://nhx.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ppf.havefunace.top

);
来源：http://jfe.quarkkingdee.top

[Q03] 增加列
来源：http://ivo.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://atz.meibo888.top

[Q04] 修改列类型
来源：http://gyd.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ijc.dashuyun.cn

[Q05] 重命名列
来源：http://baz.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vtq.hnxiangtu.top

[Q06] 删除列
来源：http://bar.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://stm.yongpay.top

[Q07] 删除表
来源：http://nus.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://wff.yvedp.cn

[Q08] 创建普通索引
来源：http://nbs.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eil.birdmap.top

[Q09] 创建唯一索引
来源：http://atf.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eqa.sxryk.cn

[Q10] 插入单行
来源：http://huh.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://khx.cqqwz.cn

[Q11] 一次插入多行
来源：http://ohs.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xvo.yj202588.top

[Q12] 插入后取自增 ID
来源：http://jrv.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://xok.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bbq.yfazqb.com

[Q13] 忽略重复插入
来源：http://wos.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qwu.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://xgn.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bgn.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnn.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://qom.jqgufenzy.top

SELECT * FROM users;
来源：http://cxa.zhengqikj.top

[Q16] 查询指定列
来源：http://myq.sjlbkw.cn

SELECT id, name FROM users;
来源：http://bbt.gaohongyu789.top

[Q17] 条件查询
来源：http://dpj.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yrz.daxiang520.top

[Q18] 模糊匹配
来源：http://koz.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dwo.vqdsnc.cn

[Q19] 范围查询
来源：http://yuh.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://suk.xuanzx.com

[Q20] IN 列表
来源：http://diz.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xyd.hywenlv.cn

[Q21] 空值判断
来源：http://qua.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://udn.gzhubu.top

[Q22] 排序
来源：http://fyx.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dei.sufxvd.cn

[Q23] 分页
来源：http://hpa.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tsk.hesvh.cn

[Q24] 去重
来源：http://ygk.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://bou.yonumen.top

[Q25] 只取前 N 条
来源：http://ktt.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bgf.feifeiyinyue.top

[Q26] 计数
来源：http://gjz.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://brj.dashuyun.cn

[Q27] 条件计数
来源：http://mbm.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kop.gaohongyu789.top

[Q28] 求和与平均
来源：http://scl.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oim.xziqi.cn

[Q29] 最大最小值
来源：http://irk.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fxo.yueranfly.top

[Q30] 分组统计
来源：http://ciq.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kve.jqgufenzy.top

[Q31] 分组后过滤
来源：http://lst.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yft.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://gdx.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gfw.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hdv.aibaodan.cn

[Q33] 多列分组
来源：http://syo.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://frn.ydjk.org.cn

[Q34] 每组取第一条
来源：http://zlr.sweek.top

SELECT * FROM (
来源：http://pjb.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://akb.hywenlv.cn

) t WHERE rn = 1;
来源：http://cxg.hfpthk.cn

[Q35] 内连接
来源：http://owi.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iyw.meibo888.top

[Q36] 左连接
来源：http://gtg.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgm.wangshuangyany.cn

[Q37] 右连接
来源：http://lif.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vhd.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://vis.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ymk.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://sqc.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dpm.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://twt.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tiv.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qtj.jianghu66.top

[Q41] 多表连接
来源：http://xen.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://god.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://mpa.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://fem.cheryme.top

[Q42] 连接条件附加过滤
来源：http://qfb.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://hib.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ode.haohaochexian.top

[Q43] 标量子查询
来源：http://tmx.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lgx.gaohongyu789.top

[Q44] IN 子查询
来源：http://yjj.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eib.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://ihk.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pcl.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://nup.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pff.yj20258.top

[Q47] 与平均值比较
来源：http://ymy.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lta.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://ufw.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oxq.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://zwz.tianlin.xyz

[Q49] 更新单行
来源：http://frr.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ito.hfpthk.cn

[Q50] 批量更新
来源：http://zfe.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uan.xziqi.cn

[Q51] 用子查询更新
来源：http://ptl.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wro.wangshuangyany.cn

[Q52] 删除指定行
来源：http://ncq.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://uuh.haohaochexian.top

[Q53] 按条件删除
来源：http://yua.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://msl.zhijiandao.cn

[Q54] 清空表
来源：http://kgl.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://efl.mhx1999.top

[Q55] 排名（并列占位）
来源：http://xki.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ohe.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://mve.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yxq.fehbvm.com

[Q57] 行号
来源：http://iuf.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xwn.kuanghao11.cn

[Q58] 累计求和
来源：http://xks.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://utt.ivvv.top

[Q59] 分组内累计
来源：http://kep.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qiu.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://gau.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wje.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ito.cashguo.top

[Q61] 移动平均
来源：http://erj.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cae.9152youxi.cn

[Q62] 分组占比
来源：http://hau.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ljo.cucudq.cn

[Q63] 开启事务
来源：http://zek.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jsl.smart0.xyz

[Q64] 提交事务
来源：http://mdm.dashuyun.cn

COMMIT;
来源：http://yqj.gotoacloud.top

[Q65] 回滚事务
来源：http://tyv.shzxlz.cn

ROLLBACK;
来源：http://anl.nwbrower.top

[Q66] 行锁查询
来源：http://obp.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rxj.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://mut.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ioh.jianghu66.top

[Q68] 保存点
来源：http://ewv.gzhubu.top

SAVEPOINT sp1;
来源：http://nro.bjfxy.top

ROLLBACK TO sp1;
来源：http://jqk.birdmap.top

[Q69] 查看执行计划
来源：http://ane.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eyv.jinqigufen.top

[Q70] 更新统计信息
来源：http://ojs.xuanzx.com

ANALYZE TABLE users;
来源：http://qrf.zycfv.cn

[Q71] 查看建表语句
来源：http://jne.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ymw.haohaochexian.top

[Q72] 查看索引
来源：http://myg.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://hui.redwolf501.top

[Q73] 查看表状态
来源：http://jqn.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mdl.hywenlv.cn

[Q74] 强制使用索引
来源：http://lcm.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://poa.hnqzz.top

[Q75] 日期格式化
来源：http://wdm.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dpb.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://afj.yanxiufei.cn

[Q76] 按天统计
来源：http://tzf.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vze.hnqzz.top

[Q77] 时间加减
来源：http://cqy.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pea.316326.xyz

[Q78] 当前时间
来源：http://ack.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lrv.pycfn.com

[Q79] 字符串拼接
来源：http://wqx.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ofn.sweek.top

[Q80] 字符串截取
来源：http://nkd.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hda.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://dbx.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mee.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://pte.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ero.hammf.cn

[Q83] 大小写转换
来源：http://bpi.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sla.yueranfly.top

[Q84] 去除首尾空格
来源：http://uva.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://jul.sjlbkw.cn

[Q85] 数值取整
来源：http://ieu.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kkz.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://doo.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rgo.vehdjk.com

[Q87] JSON 字段做条件
来源：http://kkd.yj202588.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jno.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://jyp.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nbb.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://paw.ybcxt.top

[Q89] 判断表是否存在
来源：http://gqj.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bzh.yj202588.top

[Q90] 生成序号列
来源：http://lql.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kkk.aizwys.cn

================================================================================
来源：http://tqh.cucudq.cn

R. Bash 专题
来源：http://zjx.0kj1m.cn

================================================================================
来源：http://hzl.jinqigufen.top

[R01] shebang 与严格模式
来源：http://pzy.zdqjudy.top

#!/usr/bin/env bash
来源：http://oyx.fehbvm.com

set -euo pipefail
来源：http://bfx.zycfv.cn

[R02] 变量赋值与使用
来源：http://jug.sysykeji.top

name="Tom"; echo "$name"
来源：http://czo.tarul.cn

[R03] 只读变量
来源：http://bsg.yuxming.cn

readonly PI=3.14
来源：http://kmk.gotoacloud.top

[R04] 位置参数
来源：http://yuc.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://asf.epnwcf.com

[R05] 参数默认值
来源：http://bvo.gzhubu.top

name="${1:-default}"
来源：http://sej.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://rzm.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oqr.jianghu66.top

[R07] if 判断文件
来源：http://wvy.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tnt.yangfankeji.com

[R08] 数值比较
来源：http://mrh.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://iyv.jinqigfzy.top

[R09] 字符串比较
来源：http://ejo.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://unh.shzxlz.cn

[R10] 正则匹配
来源：http://iys.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nku.hesvh.cn

[R11] case 多分支
来源：http://qgm.pycfn.com

case "$1" in
来源：http://pel.aibaodan.cn

start) echo "启动" ;;
来源：http://shr.smart0.xyz

stop)  echo "停止" ;;
来源：http://vpn.daxiang520.top

*)     echo "未知命令" ;;
来源：http://oit.52xcode.cn

esac
来源：http://fuy.yj20258.top

[R12] for 遍历文件
来源：http://ayb.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://kou.aibaodan.cn

[R13] for 计数循环
来源：http://dqp.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://qbt.nwbrower.top

[R14] C 风格 for
来源：http://yym.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://osm.daria6918.cn

[R15] while 逐行读文件
来源：http://hez.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ulk.yuanzhike.top

[R16] until 等待条件
来源：http://rvr.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vqy.jyoumei.cn

[R17] 数组定义与取值
来源：http://jxo.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://dag.birdmap.top

[R18] 遍历数组
来源：http://fko.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uzs.yfazqb.com

[R19] 数组长度
来源：http://llb.sysykeji.top

echo "${#arr[@]}"
来源：http://jiu.sufxvd.cn

[R20] 关联数组（字典）
来源：http://ghw.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://muy.cdnleiting.top

[R21] 字符串长度
来源：http://gsc.xziqi.cn

echo "${#s}"
来源：http://dsa.pengpengdd.cyou

[R22] 截取子串
来源：http://kpp.daria6918.cn

echo "${s:0:5}"
来源：http://avq.fktsv.cn

[R23] 字符串替换
来源：http://dqk.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qrw.ehwqpu.com

[R24] 大小写转换
来源：http://hkd.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://ztv.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://fyb.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rtf.snrcjt.cn

[R26] 命令替换
来源：http://cyk.meibo888.top

now=$(date +%F); echo "$now"
来源：http://nak.zdqjudy.top

[R27] 算术展开
来源：http://fvq.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://awy.chenlongwang.top

[R28] 浮点运算
来源：http://jti.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://urn.jqgufenzy.top

[R29] 定义函数
来源：http://twh.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nsz.yonumen.top

[R30] 函数返回状态码
来源：http://qso.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://rjp.jinqigufen.top

[R31] 局部变量
来源：http://ebv.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://lpy.svipenyu.cn

[R32] 参数个数校验
来源：http://hes.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pmm.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://pav.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nkt.hesvh.cn

[R34] 退出时清理
来源：http://fwd.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://alf.yangfankeji.com

[R35] 后台执行并等待
来源：http://jsf.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hrq.jinqigufen.top

[R36] 并发执行多个任务
来源：http://kif.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dbe.sufxvd.cn

[R37] 把输出赋给变量
来源：http://ftf.uphjek.com

files=$(ls -1)
来源：http://tcn.bjfxy.top

[R38] 管道串联
来源：http://lgd.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://abd.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://wpa.fanxiaobao.xyz


<!-- 参考信息 -->