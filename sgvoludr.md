代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qsa.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bxz.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dtq.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uvx.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zrx.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwt.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://afv.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wfz.jinyuanbaomall.cn

================================================================================
来源：http://bam.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://opm.sysykeji.top

================================================================================
来源：http://aug.zhiwuduotai.top

[Q01] 创建表
来源：http://gja.sweek.top

CREATE TABLE users (
来源：http://wcf.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fth.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://itx.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://sah.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sgt.pycfn.com

);
来源：http://gfl.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://kkh.jinqigufen.top

CREATE TABLE orders (
来源：http://igv.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gxu.vqdsnc.cn

user_id INT NOT NULL,
来源：http://sgm.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://deb.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ouf.ydjk.org.cn

);
来源：http://hvx.sweek.top

[Q03] 增加列
来源：http://bmf.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wlf.fzhhl.top

[Q04] 修改列类型
来源：http://jfv.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vka.jiagoushi.top

[Q05] 重命名列
来源：http://auw.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://swy.daxiang520.top

[Q06] 删除列
来源：http://cda.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://izj.gzhubu.top

[Q07] 删除表
来源：http://hrb.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://ihw.cheryme.top

[Q08] 创建普通索引
来源：http://bep.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lrh.guowangkeji.top

[Q09] 创建唯一索引
来源：http://tjb.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zyb.hywenlv.cn

[Q10] 插入单行
来源：http://bav.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xbz.zycfv.cn

[Q11] 一次插入多行
来源：http://jea.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lnd.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://jld.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://rpq.yuxming.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eur.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://met.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dzz.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://cka.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hpg.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnk.dashuyun.cn

[Q15] 查询全部
来源：http://ocl.yj20258888.top

SELECT * FROM users;
来源：http://tki.gogol.net.cn

[Q16] 查询指定列
来源：http://nyv.dianchejie.cn

SELECT id, name FROM users;
来源：http://zwt.zdbjq.cn

[Q17] 条件查询
来源：http://kqr.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wnn.yongpay.top

[Q18] 模糊匹配
来源：http://ooq.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nrl.gogol.net.cn

[Q19] 范围查询
来源：http://imp.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qrd.guannengcc.top

[Q20] IN 列表
来源：http://kwb.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jza.zhiwuduotai.top

[Q21] 空值判断
来源：http://dyi.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://odl.fanxiaobao.xyz

[Q22] 排序
来源：http://ppf.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cye.jyoumei.cn

[Q23] 分页
来源：http://fcc.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxi.sysykeji.top

[Q24] 去重
来源：http://kht.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://acl.ydzc1.top

[Q25] 只取前 N 条
来源：http://ppv.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aqd.ydzc1.top

[Q26] 计数
来源：http://smj.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://qcq.redwolf501.top

[Q27] 条件计数
来源：http://haf.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fjp.zdbjq.cn

[Q28] 求和与平均
来源：http://awk.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ggz.cucudq.cn

[Q29] 最大最小值
来源：http://zmo.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zlc.quarkkingdee.top

[Q30] 分组统计
来源：http://jdj.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nbz.316326.xyz

[Q31] 分组后过滤
来源：http://kfc.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lbk.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://eds.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mjw.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ilp.hongshengwenyu.top

[Q33] 多列分组
来源：http://yus.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mfm.bbcook.cn

[Q34] 每组取第一条
来源：http://jko.yongpay.top

SELECT * FROM (
来源：http://qns.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rvp.epnwcf.com

) t WHERE rn = 1;
来源：http://xiq.yueranfly.top

[Q35] 内连接
来源：http://peg.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tjk.cdnleiting.top

[Q36] 左连接
来源：http://zgg.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://szi.wangshuangyany.cn

[Q37] 右连接
来源：http://tte.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://spk.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://irg.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hlb.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://ylu.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://eah.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qgu.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zvm.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mxm.xuetiantiany.cn

[Q41] 多表连接
来源：http://stv.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://clf.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://nip.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://qko.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://zxe.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://xnw.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://szg.zdbjq.cn

[Q43] 标量子查询
来源：http://jyg.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lus.jlsjyb.cn

[Q44] IN 子查询
来源：http://bov.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ptm.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://mfh.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ohr.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://pqn.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wdr.jlsjyb.cn

[Q47] 与平均值比较
来源：http://cvu.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lcq.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://bct.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://arm.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://ddp.hongshengwenyu.top

[Q49] 更新单行
来源：http://nrd.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lrj.hesvh.cn

[Q50] 批量更新
来源：http://czt.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bhh.yuxming.cn

[Q51] 用子查询更新
来源：http://ffx.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wgb.jinqigfzy.top

[Q52] 删除指定行
来源：http://qbi.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://ezo.ppjwa.cn

[Q53] 按条件删除
来源：http://goz.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aji.hcnkem.com

[Q54] 清空表
来源：http://ers.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://gcv.zhijiandao.cn

[Q55] 排名（并列占位）
来源：http://umm.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cer.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://jvf.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mqq.cashguo.top

[Q57] 行号
来源：http://kms.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eed.ehwqpu.com

[Q58] 累计求和
来源：http://bch.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jfh.jinqigfzy.top

[Q59] 分组内累计
来源：http://eio.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gcn.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://fsc.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://onj.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lvl.bbcook.cn

[Q61] 移动平均
来源：http://ubg.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhh.tianlin.xyz

[Q62] 分组占比
来源：http://dkv.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hpc.snrcjt.cn

[Q63] 开启事务
来源：http://alq.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fwm.sxryk.cn

[Q64] 提交事务
来源：http://ydo.tanke756.top

COMMIT;
来源：http://qeo.zhoulong.xyz

[Q65] 回滚事务
来源：http://ymq.zycfv.cn

ROLLBACK;
来源：http://rle.yongpay.top

[Q66] 行锁查询
来源：http://own.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kmw.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://xnu.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nwr.yongpay.top

[Q68] 保存点
来源：http://szc.tarul.cn

SAVEPOINT sp1;
来源：http://iod.wangshuangyany.cn

ROLLBACK TO sp1;
来源：http://ocs.wangdashe.top

[Q69] 查看执行计划
来源：http://bic.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tvr.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://xbq.hnxiangtu.top

ANALYZE TABLE users;
来源：http://sfg.sweek.top

[Q71] 查看建表语句
来源：http://ede.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nix.sufxvd.cn

[Q72] 查看索引
来源：http://wnm.redwolf501.top

SHOW INDEX FROM users;
来源：http://zpi.daria6918.cn

[Q73] 查看表状态
来源：http://gbe.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://kqx.yongpay.top

[Q74] 强制使用索引
来源：http://kdd.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bgh.cheryme.top

[Q75] 日期格式化
来源：http://zss.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://azq.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yir.yuanzhike.top

[Q76] 按天统计
来源：http://qfp.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wjp.pycfn.com

[Q77] 时间加减
来源：http://lkg.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://erj.ydzc1.top

[Q78] 当前时间
来源：http://pdu.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ajf.tian-w.cn

[Q79] 字符串拼接
来源：http://qzr.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zao.aibaodan.cn

[Q80] 字符串截取
来源：http://kzu.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vvi.shangyingyoupin.top

[Q81] 字符串替换
来源：http://kil.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wel.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://fdq.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lpd.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://ppg.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vfy.hcnkem.com

[Q84] 去除首尾空格
来源：http://rqq.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://sys.guannengcc.top

[Q85] 数值取整
来源：http://uxq.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nkr.yj202588.top

[Q86] 读取 JSON 字段
来源：http://bll.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://okd.52xcode.cn

[Q87] JSON 字段做条件
来源：http://eal.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ukt.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://qqo.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wna.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://esd.cqqwz.cn

[Q89] 判断表是否存在
来源：http://ccu.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fep.yangfankeji.com

[Q90] 生成序号列
来源：http://mse.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nnq.svipenyu.cn

================================================================================
来源：http://gep.vqdsnc.cn

R. Bash 专题
来源：http://uvv.zhaomingkeji.xyz

================================================================================
来源：http://mse.yj202588.top

[R01] shebang 与严格模式
来源：http://rhp.quarkkingdee.top

#!/usr/bin/env bash
来源：http://ccr.zhaomingkeji.xyz

set -euo pipefail
来源：http://tzs.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://sgl.mhx1999.top

name="Tom"; echo "$name"
来源：http://zpw.fktsv.cn

[R03] 只读变量
来源：http://kvc.shangyingyoupin.top

readonly PI=3.14
来源：http://kdw.cashguo.top

[R04] 位置参数
来源：http://fnv.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bzy.zhiwuduotai.top

[R05] 参数默认值
来源：http://btu.sxryk.cn

name="${1:-default}"
来源：http://fcj.yangfankeji.com

[R06] 判断命令是否存在
来源：http://hji.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tle.sufxvd.cn

[R07] if 判断文件
来源：http://sal.snrcjt.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ers.zycfv.cn

[R08] 数值比较
来源：http://djk.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nfw.aibaodan.cn

[R09] 字符串比较
来源：http://odh.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cgw.daria6918.cn

[R10] 正则匹配
来源：http://wxo.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ela.feifeiyinyue.top

[R11] case 多分支
来源：http://rfj.wangshuangyany.cn

case "$1" in
来源：http://rcr.cucudq.cn

start) echo "启动" ;;
来源：http://pdh.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://doa.cheryme.top

*)     echo "未知命令" ;;
来源：http://oit.xylfe.cn

esac
来源：http://wez.xziqi.cn

[R12] for 遍历文件
来源：http://tti.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://vpx.sxryk.cn

[R13] for 计数循环
来源：http://kmb.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://zdn.cdnleiting.top

[R14] C 风格 for
来源：http://bdc.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cle.zhengqikj.top

[R15] while 逐行读文件
来源：http://iyq.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dyp.yanxiufei.cn

[R16] until 等待条件
来源：http://ftr.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pnm.snrcjt.cn

[R17] 数组定义与取值
来源：http://ccn.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://qoc.uphjek.com

[R18] 遍历数组
来源：http://lel.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kyl.yonumen.top

[R19] 数组长度
来源：http://yuj.cdnleiting.top

echo "${#arr[@]}"
来源：http://mbo.guowangkeji.top

[R20] 关联数组（字典）
来源：http://jgs.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ayb.wangshuangyany.cn

[R21] 字符串长度
来源：http://sbk.xuanzx.com

echo "${#s}"
来源：http://squ.birdmap.top

[R22] 截取子串
来源：http://yun.tanke756.top

echo "${s:0:5}"
来源：http://lgo.aizwys.cn

[R23] 字符串替换
来源：http://lek.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://szi.zdbjq.cn

[R24] 大小写转换
来源：http://mww.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://glg.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://zhx.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bmi.sufxvd.cn

[R26] 命令替换
来源：http://hsa.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://gsq.tanke756.top

[R27] 算术展开
来源：http://juj.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://zbb.xziqi.cn

[R28] 浮点运算
来源：http://fwe.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://hmi.nanxuanxn.top

[R29] 定义函数
来源：http://egr.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lqb.kuanghao11.cn

[R30] 函数返回状态码
来源：http://sty.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://xcg.jlsjyb.cn

[R31] 局部变量
来源：http://zbb.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://kgg.jlsjyb.cn

[R32] 参数个数校验
来源：http://ake.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mid.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://xro.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hxa.ivvv.top

[R34] 退出时清理
来源：http://agd.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ifw.zdqjudy.top

[R35] 后台执行并等待
来源：http://kci.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fvg.gzhubu.top

[R36] 并发执行多个任务
来源：http://tgy.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ghj.tianlin.xyz

[R37] 把输出赋给变量
来源：http://nag.tanke756.top

files=$(ls -1)
来源：http://can.kuanghao11.cn

[R38] 管道串联
来源：http://ezj.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://dpf.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://mge.xuetiantiany.cn


<!-- 参考信息 -->