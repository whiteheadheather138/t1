代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gdn.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nvp.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pqs.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wyl.316326.xyz

================================================================================
来源：http://raa.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ery.yj20258.top

================================================================================
来源：http://zak.vqdsnc.cn

[Q01] 创建表
来源：http://vhr.ctjpmb.com

CREATE TABLE users (
来源：http://qxt.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mys.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://qja.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://zdg.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://axv.nanxuanxn.top

);
来源：http://qxl.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://spq.chenlongwang.top

CREATE TABLE orders (
来源：http://bcg.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zmr.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://ejv.hammf.cn

amount DECIMAL(10, 2),
来源：http://zsh.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmx.tianlin.xyz

);
来源：http://nly.cqqwz.cn

[Q03] 增加列
来源：http://ktc.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hqj.zhengqikj.top

[Q04] 修改列类型
来源：http://fmi.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fyx.nanxinkj.top

[Q05] 重命名列
来源：http://wjt.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://djh.chenzaomai.com

[Q06] 删除列
来源：http://dlc.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://itm.uphjek.com

[Q07] 删除表
来源：http://hij.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://jgd.0kj1m.cn

[Q08] 创建普通索引
来源：http://scy.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ceo.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://qvu.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gwc.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://biy.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nsk.redwolf501.top

[Q11] 一次插入多行
来源：http://yyq.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://thr.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://yro.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cqy.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nya.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://lyd.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://akt.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://uji.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://acy.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qjy.yj20258888.top

[Q15] 查询全部
来源：http://vqx.yvedp.cn

SELECT * FROM users;
来源：http://qys.shzxlz.cn

[Q16] 查询指定列
来源：http://etl.xinyue.icu

SELECT id, name FROM users;
来源：http://oxs.jiagoushi.top

[Q17] 条件查询
来源：http://wvv.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zgk.fktsv.cn

[Q18] 模糊匹配
来源：http://wkv.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqr.wangshuangyany.cn

[Q19] 范围查询
来源：http://yxt.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ues.nwbrower.top

[Q20] IN 列表
来源：http://ewq.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hit.sufxvd.cn

[Q21] 空值判断
来源：http://qjo.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://fuw.zhengqikj.top

[Q22] 排序
来源：http://hwm.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mjd.iojbl.cn

[Q23] 分页
来源：http://gsu.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fmt.nanxinkj.top

[Q24] 去重
来源：http://bnt.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://cfa.yj202588.top

[Q25] 只取前 N 条
来源：http://huo.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lsx.9152youxi.cn

[Q26] 计数
来源：http://rni.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://acx.yueranfly.top

[Q27] 条件计数
来源：http://yof.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rhe.aibaodan.cn

[Q28] 求和与平均
来源：http://kno.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zlx.yongpay.top

[Q29] 最大最小值
来源：http://nys.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wcu.pycfn.com

[Q30] 分组统计
来源：http://ibp.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izl.xuanzx.com

[Q31] 分组后过滤
来源：http://rek.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nwz.havefunace.top

[Q32] 分组拼接字符串
来源：http://vzx.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qqq.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yul.tian-w.cn

[Q33] 多列分组
来源：http://ioy.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xah.yvedp.cn

[Q34] 每组取第一条
来源：http://svu.feifeiyinyue.top

SELECT * FROM (
来源：http://mcq.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ybe.zhengqikj.top

) t WHERE rn = 1;
来源：http://xjp.fzhhl.top

[Q35] 内连接
来源：http://htl.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pcd.fktsv.cn

[Q36] 左连接
来源：http://osz.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kiy.svipenyu.cn

[Q37] 右连接
来源：http://ecu.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://apr.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nvr.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yjc.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://kgp.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kuq.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cxx.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wge.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rwp.cheryme.top

[Q41] 多表连接
来源：http://tfb.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fji.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://ilf.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://xug.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://nqb.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://ejp.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qro.mhx1999.top

[Q43] 标量子查询
来源：http://igk.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oxk.zhiwuduotai.top

[Q44] IN 子查询
来源：http://cdc.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruz.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://muv.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ycq.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vyn.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://svs.jianghu66.top

[Q47] 与平均值比较
来源：http://uje.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://obh.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://xoa.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jbh.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://sit.gzhubu.top

[Q49] 更新单行
来源：http://wup.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ygf.guannengcc.top

[Q50] 批量更新
来源：http://sez.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qja.yueranfly.top

[Q51] 用子查询更新
来源：http://fea.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ccc.jyoumei.cn

[Q52] 删除指定行
来源：http://uwi.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://lix.redwolf501.top

[Q53] 按条件删除
来源：http://wyo.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wrj.bjfxy.top

[Q54] 清空表
来源：http://sor.yueranfly.top

TRUNCATE TABLE logs;
来源：http://hvs.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://uhg.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pts.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://iwt.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nyq.quarkkingdee.top

[Q57] 行号
来源：http://tox.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lrx.chenjidiqi.icu

[Q58] 累计求和
来源：http://nft.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wsl.fzhhl.top

[Q59] 分组内累计
来源：http://zqu.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hvw.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://ffd.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zfk.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://axz.jianghu66.top

[Q61] 移动平均
来源：http://edi.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://psp.wangshuangyany.cn

[Q62] 分组占比
来源：http://jcd.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://adz.tianlin.xyz

[Q63] 开启事务
来源：http://hlo.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://afm.yfazqb.com

[Q64] 提交事务
来源：http://ltx.gzhubu.top

COMMIT;
来源：http://koc.mhx1999.top

[Q65] 回滚事务
来源：http://ndi.yvedp.cn

ROLLBACK;
来源：http://umg.ivvv.top

[Q66] 行锁查询
来源：http://lzs.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jlx.hcnkem.com

[Q67] 设置隔离级别
来源：http://eqy.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ayt.zhijiandao.cn

[Q68] 保存点
来源：http://ibw.tian-w.cn

SAVEPOINT sp1;
来源：http://pyo.fzhhl.top

ROLLBACK TO sp1;
来源：http://drp.316326.xyz

[Q69] 查看执行计划
来源：http://qht.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rbn.guannengcc.top

[Q70] 更新统计信息
来源：http://uaq.tanke756.top

ANALYZE TABLE users;
来源：http://ndd.tianlin.xyz

[Q71] 查看建表语句
来源：http://ufb.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xuz.c1oappe.top

[Q72] 查看索引
来源：http://idz.zdqjudy.top

SHOW INDEX FROM users;
来源：http://odt.nanxuanxn.top

[Q73] 查看表状态
来源：http://scj.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ile.yongpay.top

[Q74] 强制使用索引
来源：http://nzx.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://enk.hnqzz.top

[Q75] 日期格式化
来源：http://eif.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbg.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pkr.shuidangran.top

[Q76] 按天统计
来源：http://xde.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yed.yonumen.top

[Q77] 时间加减
来源：http://aek.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lof.shzxlz.cn

[Q78] 当前时间
来源：http://lic.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mst.0kj1m.cn

[Q79] 字符串拼接
来源：http://ebr.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://woh.chenzaomai.com

[Q80] 字符串截取
来源：http://igi.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://arx.sysykeji.top

[Q81] 字符串替换
来源：http://bih.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rfr.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://icv.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ull.chenlongwang.top

[Q83] 大小写转换
来源：http://kdm.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ajv.9152youxi.cn

[Q84] 去除首尾空格
来源：http://mww.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://rre.xuanzx.com

[Q85] 数值取整
来源：http://qrq.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fvp.316326.xyz

[Q86] 读取 JSON 字段
来源：http://jly.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dzm.bjfxy.top

[Q87] JSON 字段做条件
来源：http://krm.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yxy.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://vtj.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yzb.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kjy.hysaishi.cn

[Q89] 判断表是否存在
来源：http://kxn.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mjw.c1oappe.top

[Q90] 生成序号列
来源：http://leb.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bqu.cheryme.top

================================================================================
来源：http://gxa.sjlbkw.cn

R. Bash 专题
来源：http://vkv.yj20258888.top

================================================================================
来源：http://huq.svipenyu.cn

[R01] shebang 与严格模式
来源：http://crd.xziqi.cn

#!/usr/bin/env bash
来源：http://ihz.c1oappe.top

set -euo pipefail
来源：http://zvm.dashuyun.cn

[R02] 变量赋值与使用
来源：http://qgy.fehbvm.com

name="Tom"; echo "$name"
来源：http://bks.tarul.cn

[R03] 只读变量
来源：http://ziy.zhongyouzk.top

readonly PI=3.14
来源：http://whk.0kj1m.cn

[R04] 位置参数
来源：http://gln.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sqx.guannengcc.top

[R05] 参数默认值
来源：http://ubq.ivvv.top

name="${1:-default}"
来源：http://hsl.ppjwa.cn

[R06] 判断命令是否存在
来源：http://rwm.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzk.sjlbkw.cn

[R07] if 判断文件
来源：http://lvo.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vtg.cucudq.cn

[R08] 数值比较
来源：http://kdg.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nyf.smart0.xyz

[R09] 字符串比较
来源：http://afu.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gab.feifeiyinyue.top

[R10] 正则匹配
来源：http://odb.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zly.jlsjyb.cn

[R11] case 多分支
来源：http://mkm.xuetiantiany.cn

case "$1" in
来源：http://cez.dashuyun.cn

start) echo "启动" ;;
来源：http://xez.ehwqpu.com

stop)  echo "停止" ;;
来源：http://fvn.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://eoq.zhongyouzk.top

esac
来源：http://xfe.jqgufenzy.top

[R12] for 遍历文件
来源：http://rao.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://wua.sxryk.cn

[R13] for 计数循环
来源：http://zfx.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://qgx.mhx1999.top

[R14] C 风格 for
来源：http://ysz.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yzi.tarul.cn

[R15] while 逐行读文件
来源：http://bpf.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iml.cashguo.top

[R16] until 等待条件
来源：http://mzf.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ltf.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://phh.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yad.zdbjq.cn

[R18] 遍历数组
来源：http://aaq.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lvb.yuanzhike.top

[R19] 数组长度
来源：http://mva.xziqi.cn

echo "${#arr[@]}"
来源：http://mfy.xuanzx.com

[R20] 关联数组（字典）
来源：http://bsf.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://scb.dianchejie.cn

[R21] 字符串长度
来源：http://ykd.zdqjudy.top

echo "${#s}"
来源：http://xgw.gogol.net.cn

[R22] 截取子串
来源：http://ctp.dianchejie.cn

echo "${s:0:5}"
来源：http://jnz.iojbl.cn

[R23] 字符串替换
来源：http://orx.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tvf.xuanzx.com

[R24] 大小写转换
来源：http://zat.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://txc.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://jrx.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jgx.smart0.xyz

[R26] 命令替换
来源：http://vpc.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://jup.zhoulong.xyz

[R27] 算术展开
来源：http://pva.xylfe.cn

echo $((1 + 2 * 3))
来源：http://yrs.sysykeji.top

[R28] 浮点运算
来源：http://jjy.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://utt.mhx1999.top

[R29] 定义函数
来源：http://ugp.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sbu.wangdashe.top

[R30] 函数返回状态码
来源：http://xzr.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://new.feifeiyinyue.top

[R31] 局部变量
来源：http://our.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://pit.zhongyouzk.top

[R32] 参数个数校验
来源：http://qst.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://buf.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://ing.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jya.chenlongwang.top

[R34] 退出时清理
来源：http://lkn.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://inn.yj20258.top

[R35] 后台执行并等待
来源：http://qkw.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zcq.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://tkp.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zet.yj20258888.top

[R37] 把输出赋给变量
来源：http://jtm.cheryme.top

files=$(ls -1)
来源：http://bvx.fzhhl.top

[R38] 管道串联
来源：http://vop.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://kna.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://hps.zycfv.cn

cmd > out.log 2>&1
来源：http://nbt.iojbl.cn

[R40] 追加写日志
来源：http://uam.hnxiangtu.top

echo "log" >> out.log
来源：http://got.hesvh.cn

[R41] 丢弃输出
来源：http://otn.0kj1m.cn


<!-- 参考信息 -->