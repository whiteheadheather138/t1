代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://odv.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ylq.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://okx.fktsv.cn

[P08] 处理浮点精度问题
来源：http://ojr.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kku.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kye.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vwd.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vdq.sxryk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vgh.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ves.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tks.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qoy.sysykeji.top

================================================================================
来源：http://nfm.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edl.hongshengwenyu.top

================================================================================
来源：http://qkl.fehbvm.com

[Q01] 创建表
来源：http://nxt.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://xun.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://szp.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://uqc.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://gtb.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ktk.hnqzz.top

);
来源：http://vkh.pycfn.com

[Q02] 创建带外键的表
来源：http://qrf.zhixingplan.top

CREATE TABLE orders (
来源：http://utt.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zqa.aibaodan.cn

user_id INT NOT NULL,
来源：http://wae.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://bpz.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://srr.shanyushiyangtech.top

);
来源：http://kqr.ywan-chungtsiang.top

[Q03] 增加列
来源：http://imj.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pkv.ppjwa.cn

[Q04] 修改列类型
来源：http://irh.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bma.yueranfly.top

[Q05] 重命名列
来源：http://bnx.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vrx.hfpthk.cn

[Q06] 删除列
来源：http://hrl.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kfe.havefunace.top

[Q07] 删除表
来源：http://lgr.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://siz.aibaodan.cn

[Q08] 创建普通索引
来源：http://cjk.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gpj.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://mxl.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehl.cucudq.cn

[Q10] 插入单行
来源：http://tib.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ihp.yuxming.cn

[Q11] 一次插入多行
来源：http://ell.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wfm.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://scr.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lan.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cbe.yj20258.top

[Q13] 忽略重复插入
来源：http://jzv.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lzw.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://zfx.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kjd.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ocz.jlsjyb.cn

[Q15] 查询全部
来源：http://nus.xziqi.cn

SELECT * FROM users;
来源：http://qkm.9152youxi.cn

[Q16] 查询指定列
来源：http://sjf.shzxlz.cn

SELECT id, name FROM users;
来源：http://csz.zhongyouzk.top

[Q17] 条件查询
来源：http://lmc.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xub.wangdashe.top

[Q18] 模糊匹配
来源：http://awr.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tet.xuetiantiany.cn

[Q19] 范围查询
来源：http://dfj.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rgf.zdqjudy.top

[Q20] IN 列表
来源：http://oal.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bfx.zhixingplan.top

[Q21] 空值判断
来源：http://asu.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://far.hnqzz.top

[Q22] 排序
来源：http://cqy.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qdm.zhoulong.xyz

[Q23] 分页
来源：http://hdo.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ldr.chenzaomai.com

[Q24] 去重
来源：http://yta.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://fpm.dashuyun.cn

[Q25] 只取前 N 条
来源：http://ohf.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bgs.yuxming.cn

[Q26] 计数
来源：http://zdq.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://ung.hfpthk.cn

[Q27] 条件计数
来源：http://uen.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xdy.yonumen.top

[Q28] 求和与平均
来源：http://xni.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xdb.jqgfzy.top

[Q29] 最大最小值
来源：http://nqa.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bwi.yj20258.top

[Q30] 分组统计
来源：http://dxn.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zfd.9152youxi.cn

[Q31] 分组后过滤
来源：http://kus.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://npx.bjfxy.top

[Q32] 分组拼接字符串
来源：http://enb.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tor.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://enk.hfpthk.cn

[Q33] 多列分组
来源：http://fys.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zop.shzxlz.cn

[Q34] 每组取第一条
来源：http://pvn.hnqzz.top

SELECT * FROM (
来源：http://nwz.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nqt.yueranfly.top

) t WHERE rn = 1;
来源：http://dcp.gotoacloud.top

[Q35] 内连接
来源：http://nyk.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uow.fanxiaobao.xyz

[Q36] 左连接
来源：http://qxr.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rea.xziqi.cn

[Q37] 右连接
来源：http://vck.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ucp.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ypk.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gos.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://xey.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ijs.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yju.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lmu.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qsw.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://mpz.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://frp.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://gpn.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://fam.ivvv.top

[Q42] 连接条件附加过滤
来源：http://axb.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://crt.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fer.snrcjt.cn

[Q43] 标量子查询
来源：http://jix.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jiy.dashuyun.cn

[Q44] IN 子查询
来源：http://qjv.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pmc.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://ylt.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aop.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://xcx.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://njy.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://wts.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tvn.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://hip.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://prz.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://ixa.sxryk.cn

[Q49] 更新单行
来源：http://zla.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ooz.xuanzx.com

[Q50] 批量更新
来源：http://ngk.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dlq.zhijiandao.cn

[Q51] 用子查询更新
来源：http://upw.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zyq.uphjek.com

[Q52] 删除指定行
来源：http://kew.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://dez.zhoulong.xyz

[Q53] 按条件删除
来源：http://hey.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nuq.chenzaomai.com

[Q54] 清空表
来源：http://afo.cucudq.cn

TRUNCATE TABLE logs;
来源：http://nxu.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://xhk.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gpe.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://rif.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iqo.zhengqikj.top

[Q57] 行号
来源：http://tls.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sgb.shangyingyoupin.top

[Q58] 累计求和
来源：http://wom.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ost.yonumen.top

[Q59] 分组内累计
来源：http://ooi.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yxt.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://kzn.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cng.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gfb.hysaishi.cn

[Q61] 移动平均
来源：http://wzr.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qyc.yongpay.top

[Q62] 分组占比
来源：http://gyl.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://txr.zdqjudy.top

[Q63] 开启事务
来源：http://kps.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pwx.vqdsnc.cn

[Q64] 提交事务
来源：http://tnz.daxiang520.top

COMMIT;
来源：http://ylm.bjfxy.top

[Q65] 回滚事务
来源：http://fzi.sweek.top

ROLLBACK;
来源：http://bid.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://yur.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ztn.smart0.xyz

[Q67] 设置隔离级别
来源：http://msy.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nre.fktsv.cn

[Q68] 保存点
来源：http://btp.uphjek.com

SAVEPOINT sp1;
来源：http://tdd.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://mjv.shuidangran.top

[Q69] 查看执行计划
来源：http://ycx.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tsm.cucudq.cn

[Q70] 更新统计信息
来源：http://tkw.wangdashe.top

ANALYZE TABLE users;
来源：http://mik.chenlongwang.top

[Q71] 查看建表语句
来源：http://ntw.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hwq.andypj.xyz

[Q72] 查看索引
来源：http://sxf.chenzaomai.com

SHOW INDEX FROM users;
来源：http://aoi.aibaodan.cn

[Q73] 查看表状态
来源：http://ogi.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tuh.vehdjk.com

[Q74] 强制使用索引
来源：http://zck.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ojy.jianghu66.top

[Q75] 日期格式化
来源：http://fqg.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kbk.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://prw.aizwys.cn

[Q76] 按天统计
来源：http://pxh.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://afh.feifeiyinyue.top

[Q77] 时间加减
来源：http://jce.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yry.dianchejie.cn

[Q78] 当前时间
来源：http://hwx.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ckv.xziqi.cn

[Q79] 字符串拼接
来源：http://mhk.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://avy.ydjk.org.cn

[Q80] 字符串截取
来源：http://vaq.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dic.jiagoushi.top

[Q81] 字符串替换
来源：http://bzz.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mev.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://jxp.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oef.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://esd.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rjq.yfazqb.com

[Q84] 去除首尾空格
来源：http://tpy.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://mwx.jqgfzy.top

[Q85] 数值取整
来源：http://zqa.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqa.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://vtd.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ptp.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://fxj.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ttg.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://hgg.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibf.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nbh.cqqwz.cn

[Q89] 判断表是否存在
来源：http://wkc.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://izs.hongshengwenyu.top

[Q90] 生成序号列
来源：http://one.hfpthk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kfc.vqdsnc.cn

================================================================================
来源：http://qny.c1oappe.top

R. Bash 专题
来源：http://sls.shzxlz.cn

================================================================================
来源：http://icl.birdmap.top

[R01] shebang 与严格模式
来源：http://elf.ppjwa.cn

#!/usr/bin/env bash
来源：http://yss.sxryk.cn

set -euo pipefail
来源：http://qyx.shuidangran.top

[R02] 变量赋值与使用
来源：http://vmr.wangdashe.top

name="Tom"; echo "$name"
来源：http://ljz.jlsjyb.cn

[R03] 只读变量
来源：http://cfq.zhijiandao.cn

readonly PI=3.14
来源：http://ocp.gotoacloud.top

[R04] 位置参数
来源：http://xkw.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://woa.zycfv.cn

[R05] 参数默认值
来源：http://cgr.hnqzz.top

name="${1:-default}"
来源：http://fhe.zycfv.cn

[R06] 判断命令是否存在
来源：http://foe.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gpq.52xcode.cn

[R07] if 判断文件
来源：http://chf.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gix.wangshuangyany.cn

[R08] 数值比较
来源：http://mrx.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rll.fehbvm.com

[R09] 字符串比较
来源：http://yho.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pta.hfpthk.cn

[R10] 正则匹配
来源：http://jhf.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jdf.quarkkingdee.top

[R11] case 多分支
来源：http://vim.wangshuangyany.cn

case "$1" in
来源：http://rcf.yongpay.top

start) echo "启动" ;;
来源：http://ytg.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://ehp.yj20258.top

*)     echo "未知命令" ;;
来源：http://wpm.shzxlz.cn

esac
来源：http://qah.aizwys.cn

[R12] for 遍历文件
来源：http://feo.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://rtp.fzhhl.top

[R13] for 计数循环
来源：http://esu.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://oev.hnxiangtu.top

[R14] C 风格 for
来源：http://esg.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pdy.redwolf501.top

[R15] while 逐行读文件
来源：http://mym.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qow.zhengqikj.top

[R16] until 等待条件
来源：http://aiy.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lix.epnwcf.com

[R17] 数组定义与取值
来源：http://rxz.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://huh.xinyue.icu

[R18] 遍历数组
来源：http://sek.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://beq.gogol.net.cn

[R19] 数组长度
来源：http://kam.jinqigufen.top

echo "${#arr[@]}"
来源：http://voq.yuxming.cn

[R20] 关联数组（字典）
来源：http://vxo.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bqe.daria6918.cn

[R21] 字符串长度
来源：http://msn.havefunace.top

echo "${#s}"
来源：http://hgr.jqgfzy.top

[R22] 截取子串
来源：http://zsf.nanxinkj.top

echo "${s:0:5}"
来源：http://hzu.hfpthk.cn

[R23] 字符串替换
来源：http://vse.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nfk.ivvv.top

[R24] 大小写转换
来源：http://jiv.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hhv.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://sja.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mnx.9152youxi.cn

[R26] 命令替换
来源：http://qzt.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://slv.jianghu66.top

[R27] 算术展开
来源：http://txe.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://mkx.chenjidiqi.icu

[R28] 浮点运算
来源：http://lea.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://ywf.sxryk.cn

[R29] 定义函数
来源：http://omg.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djr.zhixingplan.top

[R30] 函数返回状态码
来源：http://aoa.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://kum.hysaishi.cn

[R31] 局部变量
来源：http://yjl.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://imj.zhixingplan.top

[R32] 参数个数校验
来源：http://jcr.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ghp.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://cnr.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bit.jyoumei.cn

[R34] 退出时清理
来源：http://kxw.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://dgy.hnqzz.top

[R35] 后台执行并等待
来源：http://ctz.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lgg.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://jpi.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gqd.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://xcn.sxryk.cn


<!-- 参考信息 -->