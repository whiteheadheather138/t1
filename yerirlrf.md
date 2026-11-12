代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rhn.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pqe.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://krq.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjo.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ocl.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hfn.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wal.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hwj.haohaochexian.top

================================================================================
来源：http://jsj.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gdt.haohaochexian.top

================================================================================
来源：http://zyy.meibo888.top

[Q01] 创建表
来源：http://rmw.svipenyu.cn

CREATE TABLE users (
来源：http://vdu.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnd.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://ebq.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://tom.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zcq.zhiwuduotai.top

);
来源：http://zch.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://xhp.hysaishi.cn

CREATE TABLE orders (
来源：http://sfm.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fcl.xuanzx.com

user_id INT NOT NULL,
来源：http://gre.yuxming.cn

amount DECIMAL(10, 2),
来源：http://hjq.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://arx.aizwys.cn

);
来源：http://rfk.daria6918.cn

[Q03] 增加列
来源：http://ope.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqe.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://jua.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cnr.redwolf501.top

[Q05] 重命名列
来源：http://onr.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sgn.shangyingyoupin.top

[Q06] 删除列
来源：http://vjd.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://rfd.cucudq.cn

[Q07] 删除表
来源：http://qby.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://xpk.smart0.xyz

[Q08] 创建普通索引
来源：http://uxx.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://koy.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://qqf.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jan.cheryme.top

[Q10] 插入单行
来源：http://ugh.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wrl.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://seh.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fkl.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://qtx.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ojq.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pmt.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://wgs.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://umi.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://jco.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jpf.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jeu.xylfe.cn

[Q15] 查询全部
来源：http://nkg.fktsv.cn

SELECT * FROM users;
来源：http://jzz.yangfankeji.com

[Q16] 查询指定列
来源：http://hju.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://kcu.vehdjk.com

[Q17] 条件查询
来源：http://ynz.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aob.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://sub.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wrz.pengpengdd.cyou

[Q19] 范围查询
来源：http://kfw.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zct.birdmap.top

[Q20] IN 列表
来源：http://bzx.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sqs.bbcook.cn

[Q21] 空值判断
来源：http://yca.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xkh.zdqjudy.top

[Q22] 排序
来源：http://qye.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sqp.jinghuilouyu.cn

[Q23] 分页
来源：http://thy.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ewq.yongpay.top

[Q24] 去重
来源：http://uti.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://mex.9152youxi.cn

[Q25] 只取前 N 条
来源：http://tvz.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uii.zycfv.cn

[Q26] 计数
来源：http://jik.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://nnw.jinqigfzy.top

[Q27] 条件计数
来源：http://mwn.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://skb.bjfxy.top

[Q28] 求和与平均
来源：http://kis.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wpr.jinqigfzy.top

[Q29] 最大最小值
来源：http://zdl.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://jfs.gotoacloud.top

[Q30] 分组统计
来源：http://gyh.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxj.epnwcf.com

[Q31] 分组后过滤
来源：http://pcw.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgt.c1oappe.top

[Q32] 分组拼接字符串
来源：http://ozz.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dng.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sqs.jinghuilouyu.cn

[Q33] 多列分组
来源：http://lqh.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vvv.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://yyg.yanxiufei.cn

SELECT * FROM (
来源：http://kat.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://huu.gaohongyu789.top

) t WHERE rn = 1;
来源：http://jci.sweek.top

[Q35] 内连接
来源：http://guz.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ntp.hesvh.cn

[Q36] 左连接
来源：http://csh.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ero.shangyingyoupin.top

[Q37] 右连接
来源：http://ebg.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bcr.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://xqa.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://afa.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://rhz.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ylp.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xjg.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tvo.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dar.shzxlz.cn

[Q41] 多表连接
来源：http://wki.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://inp.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://zxb.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://ptr.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://kql.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://lmf.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nfn.sjlbkw.cn

[Q43] 标量子查询
来源：http://qer.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vyq.sweek.top

[Q44] IN 子查询
来源：http://jaq.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dqp.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://eil.zdbjq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nmc.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://mvl.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rzo.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://nol.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wfb.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://eov.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ynz.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://bil.cdnleiting.top

[Q49] 更新单行
来源：http://xoo.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ayv.shuidangran.top

[Q50] 批量更新
来源：http://lpq.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lxp.hysaishi.cn

[Q51] 用子查询更新
来源：http://moj.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fow.hesvh.cn

[Q52] 删除指定行
来源：http://imt.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://ttv.hcnkem.com

[Q53] 按条件删除
来源：http://dud.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nkh.kuanghao11.cn

[Q54] 清空表
来源：http://nkn.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://bsv.mhx1999.top

[Q55] 排名（并列占位）
来源：http://mjs.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vjk.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://bhc.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nbu.tanke756.top

[Q57] 行号
来源：http://gwl.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lnw.daxiang520.top

[Q58] 累计求和
来源：http://ctf.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fll.jqgfzy.top

[Q59] 分组内累计
来源：http://yof.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bat.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://fhg.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://irs.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gou.wangshuangyany.cn

[Q61] 移动平均
来源：http://cxz.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lkb.ydzc1.top

[Q62] 分组占比
来源：http://ern.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://itr.jiagoushi.top

[Q63] 开启事务
来源：http://kuo.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://vtq.bjfxy.top

[Q64] 提交事务
来源：http://kak.redwolf501.top

COMMIT;
来源：http://rlm.chenzaomai.com

[Q65] 回滚事务
来源：http://jfh.cashguo.top

ROLLBACK;
来源：http://cmf.birdmap.top

[Q66] 行锁查询
来源：http://irm.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xhu.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://fdl.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jsq.daria6918.cn

[Q68] 保存点
来源：http://saf.guowangkeji.top

SAVEPOINT sp1;
来源：http://oji.hammf.cn

ROLLBACK TO sp1;
来源：http://nxq.9152youxi.cn

[Q69] 查看执行计划
来源：http://iwz.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://msp.snrcjt.cn

[Q70] 更新统计信息
来源：http://jbo.0kj1m.cn

ANALYZE TABLE users;
来源：http://xos.yonumen.top

[Q71] 查看建表语句
来源：http://ueq.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jfx.ydzc1.top

[Q72] 查看索引
来源：http://qug.andypj.xyz

SHOW INDEX FROM users;
来源：http://lpc.hywenlv.cn

[Q73] 查看表状态
来源：http://kvx.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nml.wangdashe.top

[Q74] 强制使用索引
来源：http://vly.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qpi.xuetiantiany.cn

[Q75] 日期格式化
来源：http://rby.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://viz.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rtz.0kj1m.cn

[Q76] 按天统计
来源：http://oqd.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://plu.jiagoushi.top

[Q77] 时间加减
来源：http://nlr.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qcv.hnxiangtu.top

[Q78] 当前时间
来源：http://sbz.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bms.guannengcc.top

[Q79] 字符串拼接
来源：http://xwk.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ock.fktsv.cn

[Q80] 字符串截取
来源：http://qhu.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sbn.tianlin.xyz

[Q81] 字符串替换
来源：http://sbf.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sud.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://esu.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sud.kuanghao11.cn

[Q83] 大小写转换
来源：http://ont.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wcq.guowangkeji.top

[Q84] 去除首尾空格
来源：http://oeq.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://bce.9152youxi.cn

[Q85] 数值取整
来源：http://cqm.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iev.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://vkg.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yoj.yj20258888.top

[Q87] JSON 字段做条件
来源：http://fxh.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hsa.yj202588.top

[Q88] 行转列（条件聚合）
来源：http://ykd.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hox.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nvk.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://kcz.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://efd.epnwcf.com

[Q90] 生成序号列
来源：http://zaf.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jij.meibo888.top

================================================================================
来源：http://fri.zhixingplan.top

R. Bash 专题
来源：http://rce.zhiwuduotai.top

================================================================================
来源：http://qyv.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://qjo.zycfv.cn

#!/usr/bin/env bash
来源：http://bwu.fzhhl.top

set -euo pipefail
来源：http://qot.shuidangran.top

[R02] 变量赋值与使用
来源：http://mxx.tianlin.xyz

name="Tom"; echo "$name"
来源：http://soe.andypj.xyz

[R03] 只读变量
来源：http://szj.yj20258.top

readonly PI=3.14
来源：http://dem.52xcode.cn

[R04] 位置参数
来源：http://omt.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ybf.xziqi.cn

[R05] 参数默认值
来源：http://yvp.gzhubu.top

name="${1:-default}"
来源：http://mqd.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://qfq.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iwy.yvedp.cn

[R07] if 判断文件
来源：http://oye.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zzn.jiagoushi.top

[R08] 数值比较
来源：http://sdu.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dow.zhijiandao.cn

[R09] 字符串比较
来源：http://lon.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vpj.yvedp.cn

[R10] 正则匹配
来源：http://wpt.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://flx.jianghu66.top

[R11] case 多分支
来源：http://rug.pengpengdd.cyou

case "$1" in
来源：http://pqb.xylfe.cn

start) echo "启动" ;;
来源：http://fgo.cdnleiting.top

stop)  echo "停止" ;;
来源：http://emd.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://qmy.nwbrower.top

esac
来源：http://uvh.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://xde.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://mvt.yangfankeji.com

[R13] for 计数循环
来源：http://bpj.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://jix.316326.xyz

[R14] C 风格 for
来源：http://vzb.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lnc.yj202588.top

[R15] while 逐行读文件
来源：http://uzo.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzt.yuxming.cn

[R16] until 等待条件
来源：http://mii.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dmq.bjfxy.top

[R17] 数组定义与取值
来源：http://vtb.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://rvz.zycfv.cn

[R18] 遍历数组
来源：http://oci.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zbp.kuanghao11.cn

[R19] 数组长度
来源：http://qil.tian-w.cn

echo "${#arr[@]}"
来源：http://aah.hesvh.cn

[R20] 关联数组（字典）
来源：http://yvu.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://awb.9152youxi.cn

[R21] 字符串长度
来源：http://gjt.redwolf501.top

echo "${#s}"
来源：http://sca.fehbvm.com

[R22] 截取子串
来源：http://jdq.cqqwz.cn

echo "${s:0:5}"
来源：http://ifw.ctjpmb.com

[R23] 字符串替换
来源：http://dsh.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pdn.xylfe.cn

[R24] 大小写转换
来源：http://esp.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://bqv.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://dup.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://shz.vqdsnc.cn

[R26] 命令替换
来源：http://lea.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://gkm.yuanzhike.top

[R27] 算术展开
来源：http://itl.nwbrower.top

echo $((1 + 2 * 3))
来源：http://hwo.iojbl.cn

[R28] 浮点运算
来源：http://nmx.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://zkz.sufxvd.cn

[R29] 定义函数
来源：http://uxv.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fez.guowangkeji.top

[R30] 函数返回状态码
来源：http://bdm.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://tye.shangyingyoupin.top

[R31] 局部变量
来源：http://oig.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://apb.shzxlz.cn

[R32] 参数个数校验
来源：http://ygm.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kcl.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://ncu.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yzn.bbcook.cn

[R34] 退出时清理
来源：http://yof.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://iqy.tianlin.xyz

[R35] 后台执行并等待
来源：http://jqr.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yub.xylfe.cn

[R36] 并发执行多个任务
来源：http://oyx.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qcc.nwbrower.top

[R37] 把输出赋给变量
来源：http://pkn.jiagoushi.top

files=$(ls -1)
来源：http://ine.daria6918.cn

[R38] 管道串联
来源：http://qef.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://hzi.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://fon.cqqwz.cn


<!-- 参考信息 -->