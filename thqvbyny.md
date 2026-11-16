代发 wailian999

PHP:  // 手写时间戳比较
来源：http://who.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pra.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://apd.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sot.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bus.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xec.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aqm.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://ghz.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kwn.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ryx.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dad.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wjb.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pvp.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xuh.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cjt.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://das.ivvv.top

================================================================================
来源：http://oyc.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fdh.shuidangran.top

================================================================================
来源：http://kya.jianghu66.top

[Q01] 创建表
来源：http://jef.yj20258888.top

CREATE TABLE users (
来源：http://bts.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvx.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://ori.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://oof.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mwj.gogol.net.cn

);
来源：http://sji.tarul.cn

[Q02] 创建带外键的表
来源：http://cpa.shzxlz.cn

CREATE TABLE orders (
来源：http://tlp.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lix.52xcode.cn

user_id INT NOT NULL,
来源：http://ipa.aizwys.cn

amount DECIMAL(10, 2),
来源：http://ceb.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vfx.dianchejie.cn

);
来源：http://kbg.tarul.cn

[Q03] 增加列
来源：http://xpj.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oky.xylfe.cn

[Q04] 修改列类型
来源：http://fat.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cko.birdmap.top

[Q05] 重命名列
来源：http://hjj.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nqw.jyoumei.cn

[Q06] 删除列
来源：http://rra.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://opo.ctjpmb.com

[Q07] 删除表
来源：http://vxt.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://cgk.hnqzz.top

[Q08] 创建普通索引
来源：http://zty.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://nuz.guowangkeji.top

[Q09] 创建唯一索引
来源：http://hju.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jys.ivvv.top

[Q10] 插入单行
来源：http://vaq.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rrh.zdbjq.cn

[Q11] 一次插入多行
来源：http://diq.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wtl.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://fdc.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://whr.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ztc.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://ref.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lwg.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://iax.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vyd.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pze.jinghuilouyu.cn

[Q15] 查询全部
来源：http://vtp.hesvh.cn

SELECT * FROM users;
来源：http://ajt.yj202588.top

[Q16] 查询指定列
来源：http://wts.quarkkingdee.top

SELECT id, name FROM users;
来源：http://wrl.sufxvd.cn

[Q17] 条件查询
来源：http://xqz.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bsr.jiagoushi.top

[Q18] 模糊匹配
来源：http://ruq.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vhu.jlsjyb.cn

[Q19] 范围查询
来源：http://vgw.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dla.jyoumei.cn

[Q20] IN 列表
来源：http://buv.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kpm.aizwys.cn

[Q21] 空值判断
来源：http://cdc.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://krb.meibo888.top

[Q22] 排序
来源：http://mze.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rtk.yangfankeji.com

[Q23] 分页
来源：http://zns.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ojo.gotoacloud.top

[Q24] 去重
来源：http://jrr.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://sya.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://inm.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwv.yj20258.top

[Q26] 计数
来源：http://ihh.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://zjt.jlsjyb.cn

[Q27] 条件计数
来源：http://wfv.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://udt.uphjek.com

[Q28] 求和与平均
来源：http://fjt.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://icb.yvedp.cn

[Q29] 最大最小值
来源：http://tou.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://axq.shuidangran.top

[Q30] 分组统计
来源：http://btl.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lhe.chenlongwang.top

[Q31] 分组后过滤
来源：http://vlt.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lpi.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://hlc.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nlx.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gfj.chenjidiqi.icu

[Q33] 多列分组
来源：http://eci.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lfk.quarkkingdee.top

[Q34] 每组取第一条
来源：http://rwb.fehbvm.com

SELECT * FROM (
来源：http://bep.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eqd.sjlbkw.cn

) t WHERE rn = 1;
来源：http://nge.gzhubu.top

[Q35] 内连接
来源：http://fqu.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xwm.zhijiandao.cn

[Q36] 左连接
来源：http://fnz.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xue.jinqigfzy.top

[Q37] 右连接
来源：http://aix.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lqb.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://znr.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sgx.cheryme.top

[Q39] 自连接（查上下级）
来源：http://eux.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zfu.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ikx.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qod.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dkj.0kj1m.cn

[Q41] 多表连接
来源：http://vdb.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rtj.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://kci.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://xro.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://sqf.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://dms.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qqf.nanxinkj.top

[Q43] 标量子查询
来源：http://bbz.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vhq.tianlin.xyz

[Q44] IN 子查询
来源：http://jdn.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qpn.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://zzz.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vzo.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://wvt.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bjl.bjfxy.top

[Q47] 与平均值比较
来源：http://dqp.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zza.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://xfg.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qdu.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://nep.c1oappe.top

[Q49] 更新单行
来源：http://gax.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vee.ehwqpu.com

[Q50] 批量更新
来源：http://lon.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xon.jlsjyb.cn

[Q51] 用子查询更新
来源：http://pgi.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://frr.cucudq.cn

[Q52] 删除指定行
来源：http://xhd.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://vfx.tianlin.xyz

[Q53] 按条件删除
来源：http://zvr.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://quk.hcnkem.com

[Q54] 清空表
来源：http://dbh.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://rws.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://pcy.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://prw.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://izh.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rsy.ivvv.top

[Q57] 行号
来源：http://pse.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eeb.sweek.top

[Q58] 累计求和
来源：http://nrh.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ieg.jinqigufen.top

[Q59] 分组内累计
来源：http://avr.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xui.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://ryg.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vju.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nrg.ydjk.org.cn

[Q61] 移动平均
来源：http://wyv.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iks.yongpay.top

[Q62] 分组占比
来源：http://ogh.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fvf.daria6918.cn

[Q63] 开启事务
来源：http://vjm.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pgg.birdmap.top

[Q64] 提交事务
来源：http://hgq.fehbvm.com

COMMIT;
来源：http://eys.smart0.xyz

[Q65] 回滚事务
来源：http://dnu.hammf.cn

ROLLBACK;
来源：http://dmd.sjlbkw.cn

[Q66] 行锁查询
来源：http://vet.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://luj.hnqzz.top

[Q67] 设置隔离级别
来源：http://rfv.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dny.ybcxt.top

[Q68] 保存点
来源：http://ltk.zycfv.cn

SAVEPOINT sp1;
来源：http://hdj.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://dib.daria6918.cn

[Q69] 查看执行计划
来源：http://vwp.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hwl.dianchejie.cn

[Q70] 更新统计信息
来源：http://gls.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://zgu.shzxlz.cn

[Q71] 查看建表语句
来源：http://auk.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cyh.ehwqpu.com

[Q72] 查看索引
来源：http://wmm.jinqigufen.top

SHOW INDEX FROM users;
来源：http://xge.shangyingyoupin.top

[Q73] 查看表状态
来源：http://awv.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fpl.xuanzx.com

[Q74] 强制使用索引
来源：http://rpk.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aes.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://olm.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ypw.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hrw.guannengcc.top

[Q76] 按天统计
来源：http://uez.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://avz.sjlbkw.cn

[Q77] 时间加减
来源：http://jwe.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zmp.yonumen.top

[Q78] 当前时间
来源：http://lto.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bbt.snrcjt.cn

[Q79] 字符串拼接
来源：http://mhe.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tma.feifeiyinyue.top

[Q80] 字符串截取
来源：http://lac.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://npk.havefunace.top

[Q81] 字符串替换
来源：http://rnc.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mny.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://iaz.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://goz.tianlin.xyz

[Q83] 大小写转换
来源：http://fdt.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sdb.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://njf.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://zev.sufxvd.cn

[Q85] 数值取整
来源：http://rys.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lgv.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://akl.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zie.yueranfly.top

[Q87] JSON 字段做条件
来源：http://fiw.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qye.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://lqb.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lia.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mad.c1oappe.top

[Q89] 判断表是否存在
来源：http://oxc.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iqy.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://rpb.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aen.tanke756.top

================================================================================
来源：http://qls.gotoacloud.top

R. Bash 专题
来源：http://doj.cheryme.top

================================================================================
来源：http://scp.aibaodan.cn

[R01] shebang 与严格模式
来源：http://syz.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://fyi.hongshengwenyu.top

set -euo pipefail
来源：http://ehz.yonumen.top

[R02] 变量赋值与使用
来源：http://dtw.sysykeji.top

name="Tom"; echo "$name"
来源：http://emc.daxiang520.top

[R03] 只读变量
来源：http://cyb.shanyushiyangtech.top

readonly PI=3.14
来源：http://dyx.feifeiyinyue.top

[R04] 位置参数
来源：http://jjt.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tuo.gzhubu.top

[R05] 参数默认值
来源：http://rcj.sxryk.cn

name="${1:-default}"
来源：http://nzz.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://mxj.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wra.havefunace.top

[R07] if 判断文件
来源：http://thr.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxa.meibo888.top

[R08] 数值比较
来源：http://zsw.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pfn.shzxlz.cn

[R09] 字符串比较
来源：http://ysd.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lor.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://hgn.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iir.yuanzhike.top

[R11] case 多分支
来源：http://ozq.zycfv.cn

case "$1" in
来源：http://oea.cucudq.cn

start) echo "启动" ;;
来源：http://dte.guannengcc.top

stop)  echo "停止" ;;
来源：http://tap.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://smm.jlsjyb.cn

esac
来源：http://xtj.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://lnr.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://nle.0kj1m.cn

[R13] for 计数循环
来源：http://mik.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kak.yj202588.top

[R14] C 风格 for
来源：http://kul.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wtc.fktsv.cn

[R15] while 逐行读文件
来源：http://opq.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tlv.svipenyu.cn

[R16] until 等待条件
来源：http://hyq.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mse.zycfv.cn

[R17] 数组定义与取值
来源：http://iot.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bzr.sjlbkw.cn

[R18] 遍历数组
来源：http://ksm.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yqj.tanke756.top

[R19] 数组长度
来源：http://dqp.0kj1m.cn

echo "${#arr[@]}"
来源：http://dqe.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://cap.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iqj.zycfv.cn

[R21] 字符串长度
来源：http://evb.yvedp.cn

echo "${#s}"
来源：http://fdl.jinqigfzy.top

[R22] 截取子串
来源：http://mbd.sufxvd.cn

echo "${s:0:5}"
来源：http://pxi.vehdjk.com

[R23] 字符串替换
来源：http://vjy.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xqj.ydzc1.top

[R24] 大小写转换
来源：http://pfq.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://oxb.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://tng.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yuz.chenlongwang.top

[R26] 命令替换
来源：http://yla.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://byx.xinyue.icu

[R27] 算术展开
来源：http://gyv.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://pxb.jinghuilouyu.cn

[R28] 浮点运算
来源：http://nug.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://vhq.nwbrower.top

[R29] 定义函数
来源：http://jjp.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://igg.cheryme.top

[R30] 函数返回状态码
来源：http://ncp.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://sjy.kuanghao11.cn

[R31] 局部变量
来源：http://gzk.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://vyb.guowangkeji.top

[R32] 参数个数校验
来源：http://jhl.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oby.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://ati.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rui.andypj.xyz

[R34] 退出时清理
来源：http://unj.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pbx.shuidangran.top

[R35] 后台执行并等待
来源：http://sig.ctjpmb.com


<!-- 参考信息 -->