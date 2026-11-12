代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpd.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dvj.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gbp.fzhhl.top

[P08] 处理浮点精度问题
来源：http://ant.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gku.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://syi.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vie.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hjd.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jyo.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jna.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jya.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aol.shangyingyoupin.top

================================================================================
来源：http://lch.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://upi.wangshuangyany.cn

================================================================================
来源：http://sjm.zhongyouzk.top

[Q01] 创建表
来源：http://fzh.cashguo.top

CREATE TABLE users (
来源：http://uwl.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsv.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://xae.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://din.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ult.ydjk.org.cn

);
来源：http://lfc.hammf.cn

[Q02] 创建带外键的表
来源：http://zgg.fengsongda.top

CREATE TABLE orders (
来源：http://ctl.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xej.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://ene.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://etw.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sto.zdqjudy.top

);
来源：http://ryo.shzxlz.cn

[Q03] 增加列
来源：http://uko.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ndr.nwbrower.top

[Q04] 修改列类型
来源：http://uej.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rvq.yuxming.cn

[Q05] 重命名列
来源：http://prq.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://juw.nanxuanxn.top

[Q06] 删除列
来源：http://fqu.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tct.zdqjudy.top

[Q07] 删除表
来源：http://uga.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://zup.vqdsnc.cn

[Q08] 创建普通索引
来源：http://qbw.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qnw.ehwqpu.com

[Q09] 创建唯一索引
来源：http://gbs.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ixb.wangdashe.top

[Q10] 插入单行
来源：http://usu.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qmx.ppjwa.cn

[Q11] 一次插入多行
来源：http://vuh.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ycr.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://tpb.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://xgo.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sgc.birdmap.top

[Q13] 忽略重复插入
来源：http://qtv.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://puo.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://wou.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eym.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cum.gogol.net.cn

[Q15] 查询全部
来源：http://jvs.ybcxt.top

SELECT * FROM users;
来源：http://pbr.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://stx.shzxlz.cn

SELECT id, name FROM users;
来源：http://loe.meibo888.top

[Q17] 条件查询
来源：http://tlv.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pkc.xuetiantiany.cn

[Q18] 模糊匹配
来源：http://kly.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qoq.pengpengdd.cyou

[Q19] 范围查询
来源：http://ecc.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wef.dianchejie.cn

[Q20] IN 列表
来源：http://zks.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sea.aizwys.cn

[Q21] 空值判断
来源：http://tqa.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dbv.cashguo.top

[Q22] 排序
来源：http://smp.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qwy.ydzc1.top

[Q23] 分页
来源：http://ldn.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhi.nanxuanxn.top

[Q24] 去重
来源：http://btw.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://lks.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://pqu.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rdx.pycfn.com

[Q26] 计数
来源：http://kva.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://yev.bbcook.cn

[Q27] 条件计数
来源：http://pki.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xir.kuanghao11.cn

[Q28] 求和与平均
来源：http://ekg.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dbr.cdnleiting.top

[Q29] 最大最小值
来源：http://wpf.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qrt.tanke756.top

[Q30] 分组统计
来源：http://haw.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://prk.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://gqy.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mtt.iojbl.cn

[Q32] 分组拼接字符串
来源：http://pqv.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mha.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fou.jinqigufen.top

[Q33] 多列分组
来源：http://adc.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ppx.mhx1999.top

[Q34] 每组取第一条
来源：http://kpj.bjfxy.top

SELECT * FROM (
来源：http://kgt.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kce.andypj.xyz

) t WHERE rn = 1;
来源：http://lkr.hesvh.cn

[Q35] 内连接
来源：http://xnw.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dff.hnxiangtu.top

[Q36] 左连接
来源：http://avb.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rma.redwolf501.top

[Q37] 右连接
来源：http://zvl.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aof.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://hld.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fpb.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://hne.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fwi.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xqn.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gtd.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://loa.wangshuangyany.cn

[Q41] 多表连接
来源：http://chx.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iyz.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://tyz.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://eeh.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://ccv.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://oau.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://muc.shuidangran.top

[Q43] 标量子查询
来源：http://jhh.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wyh.xinyue.icu

[Q44] IN 子查询
来源：http://ezo.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jnz.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://odk.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfr.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dhd.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qtq.fehbvm.com

[Q47] 与平均值比较
来源：http://lpx.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lcu.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://cfx.bbcook.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jge.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://rin.sufxvd.cn

[Q49] 更新单行
来源：http://nza.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aaq.hfpthk.cn

[Q50] 批量更新
来源：http://mgk.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqs.yuxming.cn

[Q51] 用子查询更新
来源：http://fbp.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iai.zhongyouzk.top

[Q52] 删除指定行
来源：http://xrw.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://zps.daxiang520.top

[Q53] 按条件删除
来源：http://xbg.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xvk.yuxming.cn

[Q54] 清空表
来源：http://cni.yongpay.top

TRUNCATE TABLE logs;
来源：http://yaw.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://orc.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wyz.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://rzo.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tzx.dianchejie.cn

[Q57] 行号
来源：http://zcq.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iht.shzxlz.cn

[Q58] 累计求和
来源：http://sed.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sbs.xuanzx.com

[Q59] 分组内累计
来源：http://izp.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hfd.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://rnu.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wne.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tvl.havefunace.top

[Q61] 移动平均
来源：http://dmn.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://taw.gogol.net.cn

[Q62] 分组占比
来源：http://gay.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zbw.gzhubu.top

[Q63] 开启事务
来源：http://fdr.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hdm.hammf.cn

[Q64] 提交事务
来源：http://ejb.zhixingplan.top

COMMIT;
来源：http://lul.cashguo.top

[Q65] 回滚事务
来源：http://ggd.pycfn.com

ROLLBACK;
来源：http://lsd.ehwqpu.com

[Q66] 行锁查询
来源：http://wty.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rim.jianghu66.top

[Q67] 设置隔离级别
来源：http://xic.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tyq.haohaochexian.top

[Q68] 保存点
来源：http://tgi.zdqjudy.top

SAVEPOINT sp1;
来源：http://obs.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://jat.hesvh.cn

[Q69] 查看执行计划
来源：http://pno.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qle.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://ies.gotoacloud.top

ANALYZE TABLE users;
来源：http://hly.zhoulong.xyz

[Q71] 查看建表语句
来源：http://vwm.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://irt.zhixingplan.top

[Q72] 查看索引
来源：http://wvb.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://zjz.yuanzhike.top

[Q73] 查看表状态
来源：http://gvt.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uxo.jqgufenzy.top

[Q74] 强制使用索引
来源：http://xus.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mqy.guannengcc.top

[Q75] 日期格式化
来源：http://ink.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qfg.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wus.daria6918.cn

[Q76] 按天统计
来源：http://xfq.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xnh.zhoulong.xyz

[Q77] 时间加减
来源：http://siw.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ziz.aibaodan.cn

[Q78] 当前时间
来源：http://fmv.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cdf.yueranfly.top

[Q79] 字符串拼接
来源：http://tyk.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mvj.uphjek.com

[Q80] 字符串截取
来源：http://jmg.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ivh.cucudq.cn

[Q81] 字符串替换
来源：http://yuy.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cub.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://xqv.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wzn.yongpay.top

[Q83] 大小写转换
来源：http://fre.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://emw.jqgfzy.top

[Q84] 去除首尾空格
来源：http://dlh.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://klf.jqgfzy.top

[Q85] 数值取整
来源：http://pfe.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://knu.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://sso.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kpq.zycfv.cn

[Q87] JSON 字段做条件
来源：http://wws.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://caj.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://ctl.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dws.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ukz.cqqwz.cn

[Q89] 判断表是否存在
来源：http://emc.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://erf.gzhubu.top

[Q90] 生成序号列
来源：http://ivt.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://prz.yj20258.top

================================================================================
来源：http://fdy.birdmap.top

R. Bash 专题
来源：http://akj.zhiwuduotai.top

================================================================================
来源：http://zkx.hammf.cn

[R01] shebang 与严格模式
来源：http://yad.yonumen.top

#!/usr/bin/env bash
来源：http://arp.gogol.net.cn

set -euo pipefail
来源：http://rih.hysaishi.cn

[R02] 变量赋值与使用
来源：http://jza.yj20258.top

name="Tom"; echo "$name"
来源：http://gxt.ctjpmb.com

[R03] 只读变量
来源：http://amy.zhengqikj.top

readonly PI=3.14
来源：http://qng.ydjk.org.cn

[R04] 位置参数
来源：http://gkt.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bji.mhx1999.top

[R05] 参数默认值
来源：http://qod.chenjidiqi.icu

name="${1:-default}"
来源：http://duq.chenlongwang.top

[R06] 判断命令是否存在
来源：http://vfi.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://quy.daria6918.cn

[R07] if 判断文件
来源：http://osp.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fcl.ehwqpu.com

[R08] 数值比较
来源：http://qpx.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tld.daria6918.cn

[R09] 字符串比较
来源：http://cja.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kgv.yuxming.cn

[R10] 正则匹配
来源：http://mob.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oep.xinyue.icu

[R11] case 多分支
来源：http://ovt.c1oappe.top

case "$1" in
来源：http://uzt.jlsjyb.cn

start) echo "启动" ;;
来源：http://aso.dianchejie.cn

stop)  echo "停止" ;;
来源：http://xfo.tanke756.top

*)     echo "未知命令" ;;
来源：http://eom.hysaishi.cn

esac
来源：http://stk.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://gln.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://hwt.yonumen.top

[R13] for 计数循环
来源：http://wuh.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://wja.nanxuanxn.top

[R14] C 风格 for
来源：http://bju.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lof.dashuyun.cn

[R15] while 逐行读文件
来源：http://ddh.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bea.iojbl.cn

[R16] until 等待条件
来源：http://zvu.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qtb.yongpay.top

[R17] 数组定义与取值
来源：http://rhr.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://qqt.hnxiangtu.top

[R18] 遍历数组
来源：http://dre.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zcr.ehwqpu.com

[R19] 数组长度
来源：http://yag.hammf.cn

echo "${#arr[@]}"
来源：http://pge.xylfe.cn

[R20] 关联数组（字典）
来源：http://afp.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://khr.zhiwuduotai.top

[R21] 字符串长度
来源：http://wck.hammf.cn

echo "${#s}"
来源：http://vkk.yj20258.top

[R22] 截取子串
来源：http://twt.chenzaomai.com

echo "${s:0:5}"
来源：http://nzi.zycfv.cn

[R23] 字符串替换
来源：http://jox.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xkf.ydjk.org.cn

[R24] 大小写转换
来源：http://ivx.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bhx.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://bvh.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pvq.ydzc1.top

[R26] 命令替换
来源：http://lzq.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://vrq.andypj.xyz

[R27] 算术展开
来源：http://gzf.xuanzx.com

echo $((1 + 2 * 3))
来源：http://mjp.hesvh.cn

[R28] 浮点运算
来源：http://tdg.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://mfo.cucudq.cn

[R29] 定义函数
来源：http://dab.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hau.yj20258.top

[R30] 函数返回状态码
来源：http://slq.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://mup.uphjek.com

[R31] 局部变量
来源：http://kld.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://bqx.9152youxi.cn

[R32] 参数个数校验
来源：http://nrc.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://puw.birdmap.top

[R33] 捕获错误并提示行号
来源：http://qzt.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ama.xuanzx.com

[R34] 退出时清理
来源：http://vqn.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://klg.fktsv.cn

[R35] 后台执行并等待
来源：http://bcl.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://glb.zycfv.cn

[R36] 并发执行多个任务
来源：http://fqe.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nmr.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://cxn.uphjek.com


<!-- 参考信息 -->