代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ygr.ehwqpu.com

TS:   if (x == null) {}
来源：http://vlo.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mvz.guannengcc.top

Go:   if x == nil {}
来源：http://eik.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pqv.yueranfly.top

C#:   if (x is null) {}
来源：http://otj.c1oappe.top

[P07] 防抖与节流
来源：http://zdr.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://afq.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://thy.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jba.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qur.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jev.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fkl.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://iol.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vhx.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://wzr.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://utv.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lls.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dub.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ydu.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ulb.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zmb.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vnc.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lhv.hongshengwenyu.top

================================================================================
来源：http://vcw.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://abq.jinqigfzy.top

================================================================================
来源：http://bxe.hongshengwenyu.top

[Q01] 创建表
来源：http://udt.yfazqb.com

CREATE TABLE users (
来源：http://wlv.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vgm.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://pey.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://xlh.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tcp.aizwys.cn

);
来源：http://jau.redwolf501.top

[Q02] 创建带外键的表
来源：http://ntd.chenzaomai.com

CREATE TABLE orders (
来源：http://sjh.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rig.yuxming.cn

user_id INT NOT NULL,
来源：http://yyj.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://xia.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pjy.jianghu66.top

);
来源：http://jzc.fengsongda.top

[Q03] 增加列
来源：http://cnk.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qyf.shuidangran.top

[Q04] 修改列类型
来源：http://lgk.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nfk.bjfxy.top

[Q05] 重命名列
来源：http://kas.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://awm.yueranfly.top

[Q06] 删除列
来源：http://kfx.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jfc.jinghuilouyu.cn

[Q07] 删除表
来源：http://oyx.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://wyi.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://sqg.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ntn.sxryk.cn

[Q09] 创建唯一索引
来源：http://lpu.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lan.meibo888.top

[Q10] 插入单行
来源：http://bdp.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qlv.ivvv.top

[Q11] 一次插入多行
来源：http://brj.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fxq.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://gcu.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://nkz.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ixv.chenlongwang.top

[Q13] 忽略重复插入
来源：http://vzf.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ujj.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://vsp.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oiu.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bco.xinyue.icu

[Q15] 查询全部
来源：http://cpo.yj20258888.top

SELECT * FROM users;
来源：http://suz.hywenlv.cn

[Q16] 查询指定列
来源：http://hrq.zycfv.cn

SELECT id, name FROM users;
来源：http://mom.jqgfzy.top

[Q17] 条件查询
来源：http://hka.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oof.gotoacloud.top

[Q18] 模糊匹配
来源：http://jju.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yhw.hysaishi.cn

[Q19] 范围查询
来源：http://syu.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hfd.hammf.cn

[Q20] IN 列表
来源：http://agp.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ozp.cashguo.top

[Q21] 空值判断
来源：http://mpc.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mdn.jlsjyb.cn

[Q22] 排序
来源：http://psc.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hbq.zdqjudy.top

[Q23] 分页
来源：http://fsc.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vpr.smart0.xyz

[Q24] 去重
来源：http://kfn.shangyingyoupin.top

SELECT DISTINCT city FROM users;
来源：http://rdz.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://wyr.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qvl.ehwqpu.com

[Q26] 计数
来源：http://yet.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://qap.zdbjq.cn

[Q27] 条件计数
来源：http://yvm.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tld.jiagoushi.top

[Q28] 求和与平均
来源：http://qqi.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zxc.haohaochexian.top

[Q29] 最大最小值
来源：http://vuz.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bmk.yangfankeji.com

[Q30] 分组统计
来源：http://lkw.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gnn.yj20258.top

[Q31] 分组后过滤
来源：http://wnm.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hwj.yvedp.cn

[Q32] 分组拼接字符串
来源：http://nae.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hsy.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mkt.9152youxi.cn

[Q33] 多列分组
来源：http://wej.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sup.yvedp.cn

[Q34] 每组取第一条
来源：http://qoi.epnwcf.com

SELECT * FROM (
来源：http://llz.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cvm.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://rpx.fehbvm.com

[Q35] 内连接
来源：http://xtj.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yoc.fengsongda.top

[Q36] 左连接
来源：http://utf.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://trc.sxryk.cn

[Q37] 右连接
来源：http://pwg.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fya.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://tnj.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kxv.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://tzj.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tlo.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ivk.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qxv.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jor.gaohongyu789.top

[Q41] 多表连接
来源：http://zsv.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://kvg.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://rpu.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://wsw.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://yku.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://dnq.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hap.tarul.cn

[Q43] 标量子查询
来源：http://mkf.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://krg.aibaodan.cn

[Q44] IN 子查询
来源：http://nut.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lbh.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://kyk.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tlg.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hrw.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jwr.hywenlv.cn

[Q47] 与平均值比较
来源：http://oox.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bfo.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://fvu.fzhhl.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hyu.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://aaj.redwolf501.top

[Q49] 更新单行
来源：http://cup.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kyq.jyoumei.cn

[Q50] 批量更新
来源：http://ohp.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bpx.zycfv.cn

[Q51] 用子查询更新
来源：http://bje.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xnz.vqdsnc.cn

[Q52] 删除指定行
来源：http://frj.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://lav.hesvh.cn

[Q53] 按条件删除
来源：http://bsa.yanxiufei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qen.pycfn.com

[Q54] 清空表
来源：http://oxz.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://guu.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://afs.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uby.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://pvw.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://unx.yfazqb.com

[Q57] 行号
来源：http://tib.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://byp.zhongyouzk.top

[Q58] 累计求和
来源：http://dsa.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kyk.hnqzz.top

[Q59] 分组内累计
来源：http://kce.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://evg.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://jor.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kcz.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://llg.zhoulong.xyz

[Q61] 移动平均
来源：http://uka.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nli.ehwqpu.com

[Q62] 分组占比
来源：http://iiq.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uox.yongpay.top

[Q63] 开启事务
来源：http://enj.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://buk.cucudq.cn

[Q64] 提交事务
来源：http://srv.jinghuilouyu.cn

COMMIT;
来源：http://mpy.zdbjq.cn

[Q65] 回滚事务
来源：http://pos.tanke756.top

ROLLBACK;
来源：http://ofq.jlsjyb.cn

[Q66] 行锁查询
来源：http://gbb.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jhh.iojbl.cn

[Q67] 设置隔离级别
来源：http://zvt.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xck.aibaodan.cn

[Q68] 保存点
来源：http://utb.meibo888.top

SAVEPOINT sp1;
来源：http://yvg.pycfn.com

ROLLBACK TO sp1;
来源：http://qah.tanke756.top

[Q69] 查看执行计划
来源：http://jxj.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ems.aibaodan.cn

[Q70] 更新统计信息
来源：http://zmd.yj20258.top

ANALYZE TABLE users;
来源：http://jwt.yonumen.top

[Q71] 查看建表语句
来源：http://opv.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://low.shzxlz.cn

[Q72] 查看索引
来源：http://ssy.iojbl.cn

SHOW INDEX FROM users;
来源：http://nde.tian-w.cn

[Q73] 查看表状态
来源：http://ulr.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://twi.c1oappe.top

[Q74] 强制使用索引
来源：http://fwp.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kbr.jianghu66.top

[Q75] 日期格式化
来源：http://ayj.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oxe.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ajy.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://gmh.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fzv.shuidangran.top

[Q77] 时间加减
来源：http://anp.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cfw.yonumen.top

[Q78] 当前时间
来源：http://amh.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nyt.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://ooz.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://naw.birdmap.top

[Q80] 字符串截取
来源：http://wvw.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jdx.xziqi.cn

[Q81] 字符串替换
来源：http://jbg.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hix.havefunace.top

[Q82] 字符长度与字节长度
来源：http://unc.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fft.dianchejie.cn

[Q83] 大小写转换
来源：http://mii.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vlt.fehbvm.com

[Q84] 去除首尾空格
来源：http://lyd.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://vhj.quarkkingdee.top

[Q85] 数值取整
来源：http://mrn.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fgk.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://mng.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rrx.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://pfj.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vvi.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://fjt.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vdj.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cjp.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://yae.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkz.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://dwf.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qmi.yfazqb.com

================================================================================
来源：http://ibo.jinqigufen.top

R. Bash 专题
来源：http://hfu.zhixingplan.top

================================================================================
来源：http://ykr.yj202588.top

[R01] shebang 与严格模式
来源：http://eef.kuanghao11.cn

#!/usr/bin/env bash
来源：http://ali.cashguo.top

set -euo pipefail
来源：http://rhk.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://dlr.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://fiq.fengsongda.top

[R03] 只读变量
来源：http://ast.hongshengwenyu.top

readonly PI=3.14
来源：http://ceh.yonumen.top

[R04] 位置参数
来源：http://upd.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://flz.hysaishi.cn

[R05] 参数默认值
来源：http://omr.yuanzhike.top

name="${1:-default}"
来源：http://rca.yongpay.top

[R06] 判断命令是否存在
来源：http://zgv.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oel.xylfe.cn

[R07] if 判断文件
来源：http://umc.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wiw.jinghuilouyu.cn

[R08] 数值比较
来源：http://qrt.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://smy.fengsongda.top

[R09] 字符串比较
来源：http://bua.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://svg.zhiwuduotai.top

[R10] 正则匹配
来源：http://xvy.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aiq.ydzc1.top

[R11] case 多分支
来源：http://xna.vqdsnc.cn

case "$1" in
来源：http://omi.yonumen.top

start) echo "启动" ;;
来源：http://cnj.316326.xyz

stop)  echo "停止" ;;
来源：http://ucs.hnqzz.top

*)     echo "未知命令" ;;
来源：http://zwr.hfpthk.cn

esac
来源：http://lss.aizwys.cn

[R12] for 遍历文件
来源：http://mdo.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://ivy.jqgfzy.top

[R13] for 计数循环
来源：http://mkd.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://ida.zdqjudy.top

[R14] C 风格 for
来源：http://elp.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iwh.xinyue.icu

[R15] while 逐行读文件
来源：http://snc.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ymo.cashguo.top

[R16] until 等待条件
来源：http://ujf.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://alz.nwbrower.top

[R17] 数组定义与取值
来源：http://bsz.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://xwv.zhiwuduotai.top

[R18] 遍历数组
来源：http://jxo.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujw.andypj.xyz

[R19] 数组长度
来源：http://ixp.zhongyouzk.top

echo "${#arr[@]}"
来源：http://brq.52xcode.cn

[R20] 关联数组（字典）
来源：http://dqm.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfz.sxryk.cn

[R21] 字符串长度
来源：http://aik.chenzaomai.com

echo "${#s}"
来源：http://gva.ivvv.top

[R22] 截取子串
来源：http://oyj.xziqi.cn

echo "${s:0:5}"
来源：http://oky.haohaochexian.top

[R23] 字符串替换
来源：http://nyo.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itv.jqgfzy.top

[R24] 大小写转换
来源：http://mwp.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://xgs.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://syi.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://phs.smart0.xyz

[R26] 命令替换
来源：http://gvq.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://zsv.hnqzz.top

[R27] 算术展开
来源：http://apj.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://abe.havefunace.top

[R28] 浮点运算
来源：http://glp.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://snb.zhiwuduotai.top

[R29] 定义函数
来源：http://fhw.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vxb.c1oappe.top

[R30] 函数返回状态码
来源：http://wxm.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://nva.redwolf501.top

[R31] 局部变量
来源：http://upc.hcnkem.com


<!-- 参考信息 -->