代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pmz.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mnl.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lbg.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cry.bjfxy.top

================================================================================
来源：http://gdj.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wlt.zhengqikj.top

================================================================================
来源：http://rky.gotoacloud.top

[Q01] 创建表
来源：http://xju.chenlongwang.top

CREATE TABLE users (
来源：http://uel.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohb.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://eei.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://jsa.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cql.jqgufenzy.top

);
来源：http://pmv.zycfv.cn

[Q02] 创建带外键的表
来源：http://ecd.smart0.xyz

CREATE TABLE orders (
来源：http://uef.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rvs.sufxvd.cn

user_id INT NOT NULL,
来源：http://ago.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://gwf.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ufa.jiagoushi.top

);
来源：http://gho.aizwys.cn

[Q03] 增加列
来源：http://afq.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vmn.dianchejie.cn

[Q04] 修改列类型
来源：http://hrz.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ifx.gzhubu.top

[Q05] 重命名列
来源：http://jnh.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bcv.gotoacloud.top

[Q06] 删除列
来源：http://vob.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yug.52xcode.cn

[Q07] 删除表
来源：http://uri.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://tmp.nwbrower.top

[Q08] 创建普通索引
来源：http://gir.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jgg.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://fmk.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pon.nwbrower.top

[Q10] 插入单行
来源：http://ord.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwi.svipenyu.cn

[Q11] 一次插入多行
来源：http://qef.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://byq.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://nss.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://idw.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zdo.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://cwn.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yaf.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://vxt.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dkn.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lge.aibaodan.cn

[Q15] 查询全部
来源：http://rab.feifeiyinyue.top

SELECT * FROM users;
来源：http://ely.sjlbkw.cn

[Q16] 查询指定列
来源：http://iut.shuidangran.top

SELECT id, name FROM users;
来源：http://rwd.sjlbkw.cn

[Q17] 条件查询
来源：http://xmp.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://igd.nwbrower.top

[Q18] 模糊匹配
来源：http://yer.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://grg.wangdashe.top

[Q19] 范围查询
来源：http://vyl.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yrr.chenjidiqi.icu

[Q20] IN 列表
来源：http://yfu.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kwd.jlsjyb.cn

[Q21] 空值判断
来源：http://ghf.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://voj.tian-w.cn

[Q22] 排序
来源：http://wpo.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sdy.hongshengwenyu.top

[Q23] 分页
来源：http://yjw.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://leb.ywan-chungtsiang.top

[Q24] 去重
来源：http://irc.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://bws.havefunace.top

[Q25] 只取前 N 条
来源：http://vtu.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bep.xylfe.cn

[Q26] 计数
来源：http://xdm.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://uew.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://yip.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nou.hfpthk.cn

[Q28] 求和与平均
来源：http://zqb.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tfv.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://drv.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dnp.yueranfly.top

[Q30] 分组统计
来源：http://wtq.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eon.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://ybb.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kuf.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://wjh.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xje.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bvp.fktsv.cn

[Q33] 多列分组
来源：http://kby.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ofo.316326.xyz

[Q34] 每组取第一条
来源：http://mfz.snrcjt.cn

SELECT * FROM (
来源：http://fmo.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hwt.haohaochexian.top

) t WHERE rn = 1;
来源：http://bcu.yonumen.top

[Q35] 内连接
来源：http://uaz.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mhq.nwbrower.top

[Q36] 左连接
来源：http://uog.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aat.gzhubu.top

[Q37] 右连接
来源：http://mwp.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mgv.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://frd.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cyl.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://xfy.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ebg.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jfj.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gea.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tnv.kuanghao11.cn

[Q41] 多表连接
来源：http://jgd.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wak.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://lhb.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://lsi.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://ips.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://ees.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jdn.cheryme.top

[Q43] 标量子查询
来源：http://ghg.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vgx.ctjpmb.com

[Q44] IN 子查询
来源：http://sgp.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wpx.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://kxu.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iog.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://cfg.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://enc.vehdjk.com

[Q47] 与平均值比较
来源：http://gxl.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nin.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://vct.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rsn.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://anw.chenlongwang.top

[Q49] 更新单行
来源：http://fje.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wnq.aizwys.cn

[Q50] 批量更新
来源：http://yoj.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aic.gaohongyu789.top

[Q51] 用子查询更新
来源：http://lkr.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ckx.jinqigfzy.top

[Q52] 删除指定行
来源：http://bsk.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://ipc.yj20258.top

[Q53] 按条件删除
来源：http://stl.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ucz.sjlbkw.cn

[Q54] 清空表
来源：http://odg.yj202588.top

TRUNCATE TABLE logs;
来源：http://nfp.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://wee.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ajr.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://ofh.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rzk.cheryme.top

[Q57] 行号
来源：http://ivl.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://izy.tianlin.xyz

[Q58] 累计求和
来源：http://mkl.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ift.52xcode.cn

[Q59] 分组内累计
来源：http://fcy.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://msm.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://nua.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qgb.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dxu.uphjek.com

[Q61] 移动平均
来源：http://pmg.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qrz.hysaishi.cn

[Q62] 分组占比
来源：http://wci.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ear.sxryk.cn

[Q63] 开启事务
来源：http://rye.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hmd.zhoulong.xyz

[Q64] 提交事务
来源：http://axb.sweek.top

COMMIT;
来源：http://ivs.shuidangran.top

[Q65] 回滚事务
来源：http://rfm.tarul.cn

ROLLBACK;
来源：http://yck.meibo888.top

[Q66] 行锁查询
来源：http://nzu.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ahm.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://fdl.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iqp.ywan-chungtsiang.top

[Q68] 保存点
来源：http://tsp.52xcode.cn

SAVEPOINT sp1;
来源：http://gkb.guowangkeji.top

ROLLBACK TO sp1;
来源：http://wyr.zhoulong.xyz

[Q69] 查看执行计划
来源：http://zhd.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://myd.c1oappe.top

[Q70] 更新统计信息
来源：http://ulj.yj202588.top

ANALYZE TABLE users;
来源：http://edl.hfpthk.cn

[Q71] 查看建表语句
来源：http://oll.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zvr.iojbl.cn

[Q72] 查看索引
来源：http://wjv.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://yks.fengsongda.top

[Q73] 查看表状态
来源：http://ipp.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vwh.hnxiangtu.top

[Q74] 强制使用索引
来源：http://frn.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rkk.sxryk.cn

[Q75] 日期格式化
来源：http://nzf.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fgp.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pbb.hnxiangtu.top

[Q76] 按天统计
来源：http://aae.xylfe.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rxg.cashguo.top

[Q77] 时间加减
来源：http://usx.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tyz.jlsjyb.cn

[Q78] 当前时间
来源：http://xnk.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skj.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://fyg.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mqj.pengpengdd.cyou

[Q80] 字符串截取
来源：http://sws.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bha.zhongyouzk.top

[Q81] 字符串替换
来源：http://mia.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://snn.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://yvu.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hvz.shangyingyoupin.top

[Q83] 大小写转换
来源：http://owm.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zrv.yj202588.top

[Q84] 去除首尾空格
来源：http://jey.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://mmw.fengsongda.top

[Q85] 数值取整
来源：http://fwf.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qdn.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://iim.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fkp.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://opf.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ojp.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://ojx.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mxv.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://odx.gogol.net.cn

[Q89] 判断表是否存在
来源：http://cnj.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://alw.yj20258888.top

[Q90] 生成序号列
来源：http://zck.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fdt.jqgfzy.top

================================================================================
来源：http://tlz.fzhhl.top

R. Bash 专题
来源：http://uwr.uphjek.com

================================================================================
来源：http://tzg.nwbrower.top

[R01] shebang 与严格模式
来源：http://ald.hnqzz.top

#!/usr/bin/env bash
来源：http://zke.hywenlv.cn

set -euo pipefail
来源：http://waq.smart0.xyz

[R02] 变量赋值与使用
来源：http://bqq.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://ddt.guannengcc.top

[R03] 只读变量
来源：http://lze.hesvh.cn

readonly PI=3.14
来源：http://jcw.aizwys.cn

[R04] 位置参数
来源：http://akz.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bon.sjlbkw.cn

[R05] 参数默认值
来源：http://snp.zhengqikj.top

name="${1:-default}"
来源：http://len.cdnleiting.top

[R06] 判断命令是否存在
来源：http://nyj.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nex.jianghu66.top

[R07] if 判断文件
来源：http://uyy.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ubv.tianlin.xyz

[R08] 数值比较
来源：http://qmj.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iho.nanxuanxn.top

[R09] 字符串比较
来源：http://gzw.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://njn.dianchejie.cn

[R10] 正则匹配
来源：http://czt.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wvm.bjfxy.top

[R11] case 多分支
来源：http://ntt.jqgufenzy.top

case "$1" in
来源：http://tmx.52xcode.cn

start) echo "启动" ;;
来源：http://bsk.mhx1999.top

stop)  echo "停止" ;;
来源：http://qln.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://dnt.haohaochexian.top

esac
来源：http://dby.52xcode.cn

[R12] for 遍历文件
来源：http://wdb.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://pmt.chenlongwang.top

[R13] for 计数循环
来源：http://ydf.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ozo.zhijiandao.cn

[R14] C 风格 for
来源：http://und.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cdc.daria6918.cn

[R15] while 逐行读文件
来源：http://zrv.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ypu.guannengcc.top

[R16] until 等待条件
来源：http://esd.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tan.redwolf501.top

[R17] 数组定义与取值
来源：http://xln.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://lbz.dashuyun.cn

[R18] 遍历数组
来源：http://ccz.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kan.xziqi.cn

[R19] 数组长度
来源：http://gbv.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://syx.shzxlz.cn

[R20] 关联数组（字典）
来源：http://hkl.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mjv.shanyushiyangkeji.top

[R21] 字符串长度
来源：http://nla.ppjwa.cn

echo "${#s}"
来源：http://osj.jianghu66.top

[R22] 截取子串
来源：http://zgt.fktsv.cn

echo "${s:0:5}"
来源：http://iqg.andypj.xyz

[R23] 字符串替换
来源：http://cwv.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qon.hysaishi.cn

[R24] 大小写转换
来源：http://bld.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://zmx.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://blk.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hzy.yonumen.top

[R26] 命令替换
来源：http://khv.birdmap.top

now=$(date +%F); echo "$now"
来源：http://cts.jiagoushi.top

[R27] 算术展开
来源：http://psz.yfazqb.com

echo $((1 + 2 * 3))
来源：http://nro.jinqigufen.top

[R28] 浮点运算
来源：http://xfk.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://eww.xuanzx.com

[R29] 定义函数
来源：http://nix.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vtd.mhx1999.top

[R30] 函数返回状态码
来源：http://qxh.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://dwf.yj20258888.top

[R31] 局部变量
来源：http://bnt.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://owd.ybcxt.top

[R32] 参数个数校验
来源：http://wln.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qhr.tanke756.top

[R33] 捕获错误并提示行号
来源：http://ndz.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cji.tarul.cn

[R34] 退出时清理
来源：http://clx.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://igr.xinyue.icu

[R35] 后台执行并等待
来源：http://vss.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rbc.redwolf501.top

[R36] 并发执行多个任务
来源：http://qky.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://god.sxryk.cn

[R37] 把输出赋给变量
来源：http://byt.shzxlz.cn

files=$(ls -1)
来源：http://cwk.fanxiaobao.xyz

[R38] 管道串联
来源：http://mmn.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://bhl.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://jdk.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://lfn.sxryk.cn

[R40] 追加写日志
来源：http://vhg.yangfankeji.com

echo "log" >> out.log
来源：http://puj.sxryk.cn

[R41] 丢弃输出
来源：http://agz.fanxiaobao.xyz


<!-- 参考信息 -->