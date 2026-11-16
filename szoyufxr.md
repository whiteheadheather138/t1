代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tca.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://twj.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tsb.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xkb.jinqigufen.top

================================================================================
来源：http://emn.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zct.chenzaomai.com

================================================================================
来源：http://mkp.xziqi.cn

[Q01] 创建表
来源：http://zfg.birdmap.top

CREATE TABLE users (
来源：http://zba.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrp.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://jid.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://ipn.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ryn.hesvh.cn

);
来源：http://azk.haohaochexian.top

[Q02] 创建带外键的表
来源：http://pdk.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://eql.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozi.ctjpmb.com

user_id INT NOT NULL,
来源：http://lyr.havefunace.top

amount DECIMAL(10, 2),
来源：http://yly.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wfo.xziqi.cn

);
来源：http://rpu.chenlongwang.top

[Q03] 增加列
来源：http://rar.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://npf.chenzaomai.com

[Q04] 修改列类型
来源：http://kej.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rcv.zhiwuduotai.top

[Q05] 重命名列
来源：http://lae.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://syp.cqqwz.cn

[Q06] 删除列
来源：http://pcj.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://qaw.ehwqpu.com

[Q07] 删除表
来源：http://nca.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://yen.hysaishi.cn

[Q08] 创建普通索引
来源：http://lkv.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qag.fzhhl.top

[Q09] 创建唯一索引
来源：http://tfe.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zsc.zhongyouzk.top

[Q10] 插入单行
来源：http://bbs.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fkg.xziqi.cn

[Q11] 一次插入多行
来源：http://ydb.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mzj.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://vfz.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://sqz.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ual.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://lvt.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ycr.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://jgy.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iux.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vwc.iojbl.cn

[Q15] 查询全部
来源：http://cgf.jqgufenzy.top

SELECT * FROM users;
来源：http://iol.wangshuangyany.cn

[Q16] 查询指定列
来源：http://kem.fengsongda.top

SELECT id, name FROM users;
来源：http://nyu.bbcook.cn

[Q17] 条件查询
来源：http://dwu.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://inj.zhongyouzk.top

[Q18] 模糊匹配
来源：http://bvw.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rpc.fengsongda.top

[Q19] 范围查询
来源：http://nfv.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nhh.jiagoushi.top

[Q20] IN 列表
来源：http://sjp.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://igp.cqqwz.cn

[Q21] 空值判断
来源：http://nrb.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cor.yanxiufei.cn

[Q22] 排序
来源：http://cba.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pzu.vqdsnc.cn

[Q23] 分页
来源：http://crq.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kok.hammf.cn

[Q24] 去重
来源：http://bwv.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://frl.shzxlz.cn

[Q25] 只取前 N 条
来源：http://dus.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aen.gzhubu.top

[Q26] 计数
来源：http://srr.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://sev.fengsongda.top

[Q27] 条件计数
来源：http://knq.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmj.havefunace.top

[Q28] 求和与平均
来源：http://cxs.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ncp.jqgufenzy.top

[Q29] 最大最小值
来源：http://ndf.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rcm.zdbjq.cn

[Q30] 分组统计
来源：http://zdy.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xih.ppjwa.cn

[Q31] 分组后过滤
来源：http://ckk.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iot.smart0.xyz

[Q32] 分组拼接字符串
来源：http://hqu.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oiq.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uar.gogol.net.cn

[Q33] 多列分组
来源：http://ros.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://amf.cheryme.top

[Q34] 每组取第一条
来源：http://cpc.cqqwz.cn

SELECT * FROM (
来源：http://zyp.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oqb.yangfankeji.com

) t WHERE rn = 1;
来源：http://ipt.hesvh.cn

[Q35] 内连接
来源：http://hbv.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlw.hongshengwenyu.top

[Q36] 左连接
来源：http://urc.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hpt.yanxiufei.cn

[Q37] 右连接
来源：http://ahs.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ofo.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://jbw.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hoo.uphjek.com

[Q39] 自连接（查上下级）
来源：http://tmx.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ioz.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jow.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kmp.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ahg.zdqjudy.top

[Q41] 多表连接
来源：http://lbw.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://alj.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://jey.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://zkz.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://jef.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://uke.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lar.gotoacloud.top

[Q43] 标量子查询
来源：http://bgm.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rqr.iojbl.cn

[Q44] IN 子查询
来源：http://rej.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cct.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://wzu.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xtp.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://yuz.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqc.sxryk.cn

[Q47] 与平均值比较
来源：http://ipj.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://skd.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://bmz.hammf.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://boo.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://nng.sysykeji.top

[Q49] 更新单行
来源：http://hwh.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dbm.cheryme.top

[Q50] 批量更新
来源：http://ilw.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lrj.xylfe.cn

[Q51] 用子查询更新
来源：http://dgp.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fsl.cheryme.top

[Q52] 删除指定行
来源：http://iun.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://bac.sjlbkw.cn

[Q53] 按条件删除
来源：http://vgt.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pjj.cdnleiting.top

[Q54] 清空表
来源：http://lfa.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://dqv.hesvh.cn

[Q55] 排名（并列占位）
来源：http://jaw.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zyh.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://rvv.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gcp.yj20258.top

[Q57] 行号
来源：http://csl.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oyq.nanxinkj.top

[Q58] 累计求和
来源：http://evh.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://enw.cdnleiting.top

[Q59] 分组内累计
来源：http://gsh.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bvv.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://hkq.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vfb.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mji.hongshengwenyu.top

[Q61] 移动平均
来源：http://bby.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qrh.nanxuanxn.top

[Q62] 分组占比
来源：http://rhh.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nsn.zhengqikj.top

[Q63] 开启事务
来源：http://esj.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jjs.9152youxi.cn

[Q64] 提交事务
来源：http://pff.jinyuanbaomall.cn

COMMIT;
来源：http://bkg.cheryme.top

[Q65] 回滚事务
来源：http://zyk.zhiwuduotai.top

ROLLBACK;
来源：http://zsc.jqgfzy.top

[Q66] 行锁查询
来源：http://fhs.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://psu.ybcxt.top

[Q67] 设置隔离级别
来源：http://wfr.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://err.yuanzhike.top

[Q68] 保存点
来源：http://rea.sweek.top

SAVEPOINT sp1;
来源：http://bqb.aibaodan.cn

ROLLBACK TO sp1;
来源：http://eeg.nanxuanxn.top

[Q69] 查看执行计划
来源：http://rqw.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qem.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://ifv.daria6918.cn

ANALYZE TABLE users;
来源：http://hcm.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://nvh.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qwz.xuanzx.com

[Q72] 查看索引
来源：http://wva.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://iac.wangdashe.top

[Q73] 查看表状态
来源：http://jmi.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qzz.jyoumei.cn

[Q74] 强制使用索引
来源：http://kuw.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bky.shangyingyoupin.top

[Q75] 日期格式化
来源：http://lvp.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ojw.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ugo.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://nty.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://quh.sysykeji.top

[Q77] 时间加减
来源：http://hfy.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tvs.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://yby.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cce.cheryme.top

[Q79] 字符串拼接
来源：http://ptq.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zeo.cqqwz.cn

[Q80] 字符串截取
来源：http://wud.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jyf.vehdjk.com

[Q81] 字符串替换
来源：http://jlf.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pxp.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://fsa.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iuu.tarul.cn

[Q83] 大小写转换
来源：http://kzx.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tst.chenlongwang.top

[Q84] 去除首尾空格
来源：http://nze.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://wcp.shangyingyoupin.top

[Q85] 数值取整
来源：http://rbw.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hbc.birdmap.top

[Q86] 读取 JSON 字段
来源：http://tjj.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uoc.316326.xyz

[Q87] JSON 字段做条件
来源：http://snu.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzs.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://gvg.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vqp.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tlm.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://nrq.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uaz.jiagoushi.top

[Q90] 生成序号列
来源：http://ipn.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ftu.fzhhl.top

================================================================================
来源：http://jrm.yj20258888.top

R. Bash 专题
来源：http://xez.havefunace.top

================================================================================
来源：http://ipv.gotoacloud.top

[R01] shebang 与严格模式
来源：http://lmd.c1oappe.top

#!/usr/bin/env bash
来源：http://zmr.redwolf501.top

set -euo pipefail
来源：http://efq.tianlin.xyz

[R02] 变量赋值与使用
来源：http://tfs.jyoumei.cn

name="Tom"; echo "$name"
来源：http://cyb.shangyingyoupin.top

[R03] 只读变量
来源：http://gan.wangshuangyany.cn

readonly PI=3.14
来源：http://yav.redwolf501.top

[R04] 位置参数
来源：http://whk.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://odj.fehbvm.com

[R05] 参数默认值
来源：http://gqf.guowangkeji.top

name="${1:-default}"
来源：http://wxb.cdnleiting.top

[R06] 判断命令是否存在
来源：http://tum.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eay.smart0.xyz

[R07] if 判断文件
来源：http://xuz.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://obp.sysykeji.top

[R08] 数值比较
来源：http://kbs.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dku.cucudq.cn

[R09] 字符串比较
来源：http://dfr.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lvi.jiagoushi.top

[R10] 正则匹配
来源：http://qir.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://agy.haohaochexian.top

[R11] case 多分支
来源：http://srz.cdnleiting.top

case "$1" in
来源：http://uil.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://cve.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://yxb.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://hos.hnqzz.top

esac
来源：http://sbm.wangshuangyany.cn

[R12] for 遍历文件
来源：http://uub.dianchejie.cn

for f in *.txt; do echo "$f"; done
来源：http://ytp.xylfe.cn

[R13] for 计数循环
来源：http://fkp.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://yij.chenzaomai.com

[R14] C 风格 for
来源：http://hee.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ron.shuidangran.top

[R15] while 逐行读文件
来源：http://mjx.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://har.hywenlv.cn

[R16] until 等待条件
来源：http://ncp.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wbv.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://kxr.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://bsx.bjfxy.top

[R18] 遍历数组
来源：http://epu.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zlx.sxryk.cn

[R19] 数组长度
来源：http://oiw.shuidangran.top

echo "${#arr[@]}"
来源：http://hpy.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://zwt.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cnj.shzxlz.cn

[R21] 字符串长度
来源：http://lmb.birdmap.top

echo "${#s}"
来源：http://jjb.sjlbkw.cn

[R22] 截取子串
来源：http://yjq.aizwys.cn

echo "${s:0:5}"
来源：http://ldi.yanxiufei.cn

[R23] 字符串替换
来源：http://lsb.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gdy.tianlin.xyz

[R24] 大小写转换
来源：http://rye.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bdl.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://vmz.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mrc.ctjpmb.com

[R26] 命令替换
来源：http://guc.uphjek.com

now=$(date +%F); echo "$now"
来源：http://crb.pycfn.com

[R27] 算术展开
来源：http://kqa.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://gsp.meibo888.top

[R28] 浮点运算
来源：http://ebh.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://bli.gzhubu.top

[R29] 定义函数
来源：http://saj.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ckl.cheryme.top

[R30] 函数返回状态码
来源：http://pwq.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://bao.quarkkingdee.top

[R31] 局部变量
来源：http://enp.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://yjl.nwbrower.top

[R32] 参数个数校验
来源：http://mva.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dhz.cashguo.top

[R33] 捕获错误并提示行号
来源：http://wtl.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rvk.svipenyu.cn

[R34] 退出时清理
来源：http://xgi.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xpd.ydzc1.top

[R35] 后台执行并等待
来源：http://zcb.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://elp.jinqigufen.top

[R36] 并发执行多个任务
来源：http://uyb.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ryc.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://tpp.jqgufenzy.top

files=$(ls -1)
来源：http://loy.gaohongyu789.top

[R38] 管道串联
来源：http://gkr.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://gqv.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://iet.gzhubu.top

cmd > out.log 2>&1
来源：http://iut.hnxiangtu.top

[R40] 追加写日志
来源：http://cmo.yfazqb.com

echo "log" >> out.log
来源：http://xwh.sufxvd.cn

[R41] 丢弃输出
来源：http://kjv.tianlin.xyz


<!-- 参考信息 -->