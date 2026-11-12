代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ozo.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rti.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://etg.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://olf.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cia.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fld.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aju.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://axo.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tfq.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bfb.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://klf.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdn.xuanzx.com

================================================================================
来源：http://aqn.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lmy.c1oappe.top

================================================================================
来源：http://atu.smart0.xyz

[Q01] 创建表
来源：http://qbn.c1oappe.top

CREATE TABLE users (
来源：http://ebm.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqi.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://mwo.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://voz.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sys.havefunace.top

);
来源：http://tce.svipenyu.cn

[Q02] 创建带外键的表
来源：http://vsh.cucudq.cn

CREATE TABLE orders (
来源：http://vdq.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tpp.xziqi.cn

user_id INT NOT NULL,
来源：http://kji.cucudq.cn

amount DECIMAL(10, 2),
来源：http://eii.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xxf.mhx1999.top

);
来源：http://uqu.zhoulong.xyz

[Q03] 增加列
来源：http://sbe.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ixk.cheryme.top

[Q04] 修改列类型
来源：http://ovw.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://grc.jiagoushi.top

[Q05] 重命名列
来源：http://lgt.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eas.sysykeji.top

[Q06] 删除列
来源：http://elg.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://apg.bbcook.cn

[Q07] 删除表
来源：http://hws.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://mme.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://hjf.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ekh.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://zrf.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fke.shanyushiyangtech.top

[Q10] 插入单行
来源：http://sfm.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pbx.cqqwz.cn

[Q11] 一次插入多行
来源：http://lcd.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://osq.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://tez.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://vvl.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gmw.cheryme.top

[Q13] 忽略重复插入
来源：http://kuu.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dzv.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://wwh.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gsn.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lpt.gaohongyu789.top

[Q15] 查询全部
来源：http://ady.redwolf501.top

SELECT * FROM users;
来源：http://tgf.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://hkd.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://xpv.zdqjudy.top

[Q17] 条件查询
来源：http://asf.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lwm.zdqjudy.top

[Q18] 模糊匹配
来源：http://bfa.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ljt.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://kfx.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aya.vqdsnc.cn

[Q20] IN 列表
来源：http://nck.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gls.zdbjq.cn

[Q21] 空值判断
来源：http://rsh.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://obk.xuetiantiany.cn

[Q22] 排序
来源：http://fyn.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://txb.xziqi.cn

[Q23] 分页
来源：http://mnw.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qhe.yj20258.top

[Q24] 去重
来源：http://mov.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://srq.nanxinkj.top

[Q25] 只取前 N 条
来源：http://cjd.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vjj.hysaishi.cn

[Q26] 计数
来源：http://mwv.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://wmb.vehdjk.com

[Q27] 条件计数
来源：http://ton.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://buv.hammf.cn

[Q28] 求和与平均
来源：http://qrt.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://inh.chenlongwang.top

[Q29] 最大最小值
来源：http://soh.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nsy.bbcook.cn

[Q30] 分组统计
来源：http://zlv.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ewg.jiagoushi.top

[Q31] 分组后过滤
来源：http://iwm.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vde.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://wpj.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oyq.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yfi.quarkkingdee.top

[Q33] 多列分组
来源：http://ool.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tub.dianchejie.cn

[Q34] 每组取第一条
来源：http://eyg.shanyushiyangtech.top

SELECT * FROM (
来源：http://oeb.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mzo.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://lym.yonumen.top

[Q35] 内连接
来源：http://hnf.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zmm.sweek.top

[Q36] 左连接
来源：http://sls.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjj.jinghuilouyu.cn

[Q37] 右连接
来源：http://lym.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mae.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://rcp.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oak.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://lfg.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nja.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ugh.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sbl.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bau.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://cdg.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://xvx.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://vtj.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ghu.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://ihf.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://hao.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jzo.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://tef.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kas.pycfn.com

[Q44] IN 子查询
来源：http://ghh.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xif.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://aks.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qvh.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://sim.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ezf.guannengcc.top

[Q47] 与平均值比较
来源：http://hlu.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ndp.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://kbn.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rom.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://frr.ehwqpu.com

[Q49] 更新单行
来源：http://jiu.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nob.havefunace.top

[Q50] 批量更新
来源：http://jgv.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://drb.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://qay.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wep.ivvv.top

[Q52] 删除指定行
来源：http://bgd.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://zyd.ybcxt.top

[Q53] 按条件删除
来源：http://hzy.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zoi.xuetiantiany.cn

[Q54] 清空表
来源：http://cna.daria6918.cn

TRUNCATE TABLE logs;
来源：http://eip.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://gmj.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://toh.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://sfa.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jlp.vqdsnc.cn

[Q57] 行号
来源：http://yeq.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pey.jqgfzy.top

[Q58] 累计求和
来源：http://clw.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sio.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://jdn.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nls.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://cwg.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vqw.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kfw.vqdsnc.cn

[Q61] 移动平均
来源：http://hvs.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ccm.iojbl.cn

[Q62] 分组占比
来源：http://jin.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ioy.yongpay.top

[Q63] 开启事务
来源：http://gsm.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://her.daxiang520.top

[Q64] 提交事务
来源：http://apv.havefunace.top

COMMIT;
来源：http://qie.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://khd.xinyue.icu

ROLLBACK;
来源：http://goi.sysykeji.top

[Q66] 行锁查询
来源：http://hon.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qgg.fzhhl.top

[Q67] 设置隔离级别
来源：http://zvf.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jel.guannengcc.top

[Q68] 保存点
来源：http://bxp.tian-w.cn

SAVEPOINT sp1;
来源：http://dyj.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://mfk.zhixingplan.top

[Q69] 查看执行计划
来源：http://ieg.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jxs.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://msu.jianghu66.top

ANALYZE TABLE users;
来源：http://qoh.sjlbkw.cn

[Q71] 查看建表语句
来源：http://fgw.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ava.yangfankeji.com

[Q72] 查看索引
来源：http://mwj.cqqwz.cn

SHOW INDEX FROM users;
来源：http://vep.gaohongyu789.top

[Q73] 查看表状态
来源：http://lxx.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hhy.cqqwz.cn

[Q74] 强制使用索引
来源：http://oju.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rvq.mhx1999.top

[Q75] 日期格式化
来源：http://jrs.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vbv.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hff.xuanzx.com

[Q76] 按天统计
来源：http://iru.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gej.fehbvm.com

[Q77] 时间加减
来源：http://igy.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wre.gzhubu.top

[Q78] 当前时间
来源：http://yhf.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gwd.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://wai.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mue.zycfv.cn

[Q80] 字符串截取
来源：http://pdx.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bjr.ybcxt.top

[Q81] 字符串替换
来源：http://nez.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vxv.yj20258.top

[Q82] 字符长度与字节长度
来源：http://nkx.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rgv.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://hho.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vzd.wangdashe.top

[Q84] 去除首尾空格
来源：http://txp.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://sea.ehwqpu.com

[Q85] 数值取整
来源：http://emg.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rez.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://qdg.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hyj.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://uiz.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gei.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://zlk.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jsw.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nkk.zdbjq.cn

[Q89] 判断表是否存在
来源：http://wsk.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dur.jinqigufen.top

[Q90] 生成序号列
来源：http://bhm.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vkq.chenzaomai.com

================================================================================
来源：http://tqx.fengsongda.top

R. Bash 专题
来源：http://uem.yongpay.top

================================================================================
来源：http://ujw.shuidangran.top

[R01] shebang 与严格模式
来源：http://dxe.tanke756.top

#!/usr/bin/env bash
来源：http://imp.zycfv.cn

set -euo pipefail
来源：http://zhj.hesvh.cn

[R02] 变量赋值与使用
来源：http://qts.yongpay.top

name="Tom"; echo "$name"
来源：http://bwv.zhoulong.xyz

[R03] 只读变量
来源：http://mid.kuanghao11.cn

readonly PI=3.14
来源：http://uma.hammf.cn

[R04] 位置参数
来源：http://lnm.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kem.jyoumei.cn

[R05] 参数默认值
来源：http://oop.ehwqpu.com

name="${1:-default}"
来源：http://bsh.guowangkeji.top

[R06] 判断命令是否存在
来源：http://ulk.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hlz.yvedp.cn

[R07] if 判断文件
来源：http://mzi.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://suh.xuetiantiany.cn

[R08] 数值比较
来源：http://nop.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qsy.daria6918.cn

[R09] 字符串比较
来源：http://tei.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yrg.guowangkeji.top

[R10] 正则匹配
来源：http://kus.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://twm.cheryme.top

[R11] case 多分支
来源：http://jkh.gzhubu.top

case "$1" in
来源：http://umm.iojbl.cn

start) echo "启动" ;;
来源：http://gbe.birdmap.top

stop)  echo "停止" ;;
来源：http://ixa.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://dtx.pengpengdd.cyou

esac
来源：http://sbh.yongpay.top

[R12] for 遍历文件
来源：http://apl.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://mkj.zhijiandao.cn

[R13] for 计数循环
来源：http://ogk.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ykc.quarkkingdee.top

[R14] C 风格 for
来源：http://xsj.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cxi.zycfv.cn

[R15] while 逐行读文件
来源：http://mfh.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://znd.aizwys.cn

[R16] until 等待条件
来源：http://azx.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bwe.hammf.cn

[R17] 数组定义与取值
来源：http://jxs.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://vpu.gogol.net.cn

[R18] 遍历数组
来源：http://rwp.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pfh.jinqigufen.top

[R19] 数组长度
来源：http://sow.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://kdt.snrcjt.cn

[R20] 关联数组（字典）
来源：http://yhn.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://utm.svipenyu.cn

[R21] 字符串长度
来源：http://hsb.gaohongyu789.top

echo "${#s}"
来源：http://ppu.fehbvm.com

[R22] 截取子串
来源：http://zfb.svipenyu.cn

echo "${s:0:5}"
来源：http://qca.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://qhm.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rvm.sjlbkw.cn

[R24] 大小写转换
来源：http://qwi.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://hgx.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://deh.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dlr.ppjwa.cn

[R26] 命令替换
来源：http://qgi.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://dqq.yuanzhike.top

[R27] 算术展开
来源：http://hxv.ydzc1.top

echo $((1 + 2 * 3))
来源：http://vwi.shanyushiyangtech.top

[R28] 浮点运算
来源：http://ogm.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://jbk.fzhhl.top

[R29] 定义函数
来源：http://bmi.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://grn.jyoumei.cn

[R30] 函数返回状态码
来源：http://nbi.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://fxw.sweek.top

[R31] 局部变量
来源：http://ixd.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://rff.cucudq.cn

[R32] 参数个数校验
来源：http://ypn.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cnz.cashguo.top

[R33] 捕获错误并提示行号
来源：http://mqs.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zoo.quarkkingdee.top

[R34] 退出时清理
来源：http://epy.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qka.0kj1m.cn

[R35] 后台执行并等待
来源：http://bsf.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mts.chenzaomai.com

[R36] 并发执行多个任务
来源：http://wwf.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hit.hnqzz.top

[R37] 把输出赋给变量
来源：http://kea.nwbrower.top


<!-- 参考信息 -->