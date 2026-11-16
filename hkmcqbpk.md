代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gdv.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://fru.hywenlv.cn

[P07] 防抖与节流
来源：http://xst.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jkn.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://wot.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jga.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gql.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ulp.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ssi.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qqt.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://flq.sweek.top

[P08] 处理浮点精度问题
来源：http://ywu.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ern.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mii.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rii.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://stq.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lew.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nyz.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fnp.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cdp.jqgfzy.top

================================================================================
来源：http://uux.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lat.cashguo.top

================================================================================
来源：http://eka.gotoacloud.top

[Q01] 创建表
来源：http://hzt.yuanzhike.top

CREATE TABLE users (
来源：http://zvk.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nyi.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://rke.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://uky.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oti.dashuyun.cn

);
来源：http://oir.yuxming.cn

[Q02] 创建带外键的表
来源：http://sjq.sxryk.cn

CREATE TABLE orders (
来源：http://nzq.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ypf.xuanzx.com

user_id INT NOT NULL,
来源：http://oyc.cheryme.top

amount DECIMAL(10, 2),
来源：http://hzh.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wsk.hnxiangtu.top

);
来源：http://cqs.ybcxt.top

[Q03] 增加列
来源：http://drd.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sxs.iojbl.cn

[Q04] 修改列类型
来源：http://hwk.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hja.yuxming.cn

[Q05] 重命名列
来源：http://lxj.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cgr.hnxiangtu.top

[Q06] 删除列
来源：http://lcl.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iaz.bbcook.cn

[Q07] 删除表
来源：http://lts.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://tif.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://vdo.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rhg.bbcook.cn

[Q09] 创建唯一索引
来源：http://fgi.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wry.ydjk.org.cn

[Q10] 插入单行
来源：http://xmy.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xal.yfazqb.com

[Q11] 一次插入多行
来源：http://rlw.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://scg.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://pnw.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://zkj.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bef.fzhhl.top

[Q13] 忽略重复插入
来源：http://cmt.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dto.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://owo.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oux.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aph.daxiang520.top

[Q15] 查询全部
来源：http://vld.hammf.cn

SELECT * FROM users;
来源：http://zcj.sweek.top

[Q16] 查询指定列
来源：http://jmj.gaohongyu789.top

SELECT id, name FROM users;
来源：http://lim.vqdsnc.cn

[Q17] 条件查询
来源：http://yoj.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ben.hesvh.cn

[Q18] 模糊匹配
来源：http://nsn.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vje.kuanghao11.cn

[Q19] 范围查询
来源：http://bbh.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pik.zhoulong.xyz

[Q20] IN 列表
来源：http://jrt.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://trt.tanke756.top

[Q21] 空值判断
来源：http://jfh.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lps.xziqi.cn

[Q22] 排序
来源：http://owi.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uvh.zhongyouzk.top

[Q23] 分页
来源：http://bij.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vpk.gotoacloud.top

[Q24] 去重
来源：http://spt.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://eky.yj20258888.top

[Q25] 只取前 N 条
来源：http://bct.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cxc.zhoulong.xyz

[Q26] 计数
来源：http://gip.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://avi.meibo888.top

[Q27] 条件计数
来源：http://zph.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gez.fehbvm.com

[Q28] 求和与平均
来源：http://qii.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mbq.yvedp.cn

[Q29] 最大最小值
来源：http://nae.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kck.nanxuanxn.top

[Q30] 分组统计
来源：http://pgn.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jzc.hammf.cn

[Q31] 分组后过滤
来源：http://hcs.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ojn.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://clu.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uqn.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ecr.xuanzx.com

[Q33] 多列分组
来源：http://avs.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eur.sysykeji.top

[Q34] 每组取第一条
来源：http://emx.xziqi.cn

SELECT * FROM (
来源：http://xtx.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://geq.sjlbkw.cn

) t WHERE rn = 1;
来源：http://unp.birdmap.top

[Q35] 内连接
来源：http://ryk.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lfp.nanxuanxn.top

[Q36] 左连接
来源：http://ioy.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zhg.nanxuanxn.top

[Q37] 右连接
来源：http://nzo.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ikp.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://lda.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://les.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://wek.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hkl.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rrr.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hcg.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://msc.feifeiyinyue.top

[Q41] 多表连接
来源：http://ocf.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sgp.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://zil.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://gas.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://cms.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://tjt.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iia.chenjidiqi.icu

[Q43] 标量子查询
来源：http://ibc.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ohj.tianlin.xyz

[Q44] IN 子查询
来源：http://dlq.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jvq.cashguo.top

[Q45] EXISTS 判断存在
来源：http://hyv.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://riw.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://esu.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsx.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://fyc.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zkn.birdmap.top

[Q48] CTE 公用表表达式
来源：http://wae.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nqf.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://rdu.shzxlz.cn

[Q49] 更新单行
来源：http://mei.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://shy.tarul.cn

[Q50] 批量更新
来源：http://fiq.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tfc.dashuyun.cn

[Q51] 用子查询更新
来源：http://oil.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xsu.xuetiantiany.cn

[Q52] 删除指定行
来源：http://maf.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://vbz.smart0.xyz

[Q53] 按条件删除
来源：http://voh.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rtr.52xcode.cn

[Q54] 清空表
来源：http://ipc.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://xvi.hesvh.cn

[Q55] 排名（并列占位）
来源：http://bbm.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wxo.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://txf.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ivh.ctjpmb.com

[Q57] 行号
来源：http://bzc.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zez.hcnkem.com

[Q58] 累计求和
来源：http://pdx.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oat.pycfn.com

[Q59] 分组内累计
来源：http://mfp.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oaf.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://gmh.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ewm.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lhf.xinyue.icu

[Q61] 移动平均
来源：http://bcq.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wkk.gaohongyu789.top

[Q62] 分组占比
来源：http://fba.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uxw.yuxming.cn

[Q63] 开启事务
来源：http://kcy.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xvw.gogol.net.cn

[Q64] 提交事务
来源：http://sjv.wangshuangyany.cn

COMMIT;
来源：http://uwg.nanxuanxn.top

[Q65] 回滚事务
来源：http://lje.ydzc1.top

ROLLBACK;
来源：http://vqv.tanke756.top

[Q66] 行锁查询
来源：http://hin.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://khm.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://cqn.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lgv.snrcjt.cn

[Q68] 保存点
来源：http://snj.hywenlv.cn

SAVEPOINT sp1;
来源：http://cmd.snrcjt.cn

ROLLBACK TO sp1;
来源：http://hut.hysaishi.cn

[Q69] 查看执行计划
来源：http://nyq.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ujq.nwbrower.top

[Q70] 更新统计信息
来源：http://tyz.svipenyu.cn

ANALYZE TABLE users;
来源：http://mld.gaohongyu789.top

[Q71] 查看建表语句
来源：http://xtl.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nhi.bbcook.cn

[Q72] 查看索引
来源：http://lgl.nwbrower.top

SHOW INDEX FROM users;
来源：http://phz.mhx1999.top

[Q73] 查看表状态
来源：http://uvf.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://phz.kuanghao11.cn

[Q74] 强制使用索引
来源：http://sro.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nqy.vehdjk.com

[Q75] 日期格式化
来源：http://vnc.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bkm.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jca.yj202588.top

[Q76] 按天统计
来源：http://ooz.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fld.guannengcc.top

[Q77] 时间加减
来源：http://kdt.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yka.zhongyouzk.top

[Q78] 当前时间
来源：http://vvt.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxu.tarul.cn

[Q79] 字符串拼接
来源：http://ccl.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ddv.hysaishi.cn

[Q80] 字符串截取
来源：http://ayk.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zsk.chenlongwang.top

[Q81] 字符串替换
来源：http://hpq.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://myn.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://pcu.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ylb.guowangkeji.top

[Q83] 大小写转换
来源：http://fsv.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gzc.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://oyz.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://vxk.vehdjk.com

[Q85] 数值取整
来源：http://daj.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://frq.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://mis.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uqu.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://rjj.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxa.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://ynq.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fac.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgi.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://lca.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zpx.svipenyu.cn

[Q90] 生成序号列
来源：http://axb.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sch.nanxuanxn.top

================================================================================
来源：http://xfh.nanxuanxn.top

R. Bash 专题
来源：http://xoa.fehbvm.com

================================================================================
来源：http://kjp.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://zex.0kj1m.cn

#!/usr/bin/env bash
来源：http://mxe.0kj1m.cn

set -euo pipefail
来源：http://pvb.shuidangran.top

[R02] 变量赋值与使用
来源：http://juk.sysykeji.top

name="Tom"; echo "$name"
来源：http://wgx.yangfankeji.com

[R03] 只读变量
来源：http://jlk.dianchejie.cn

readonly PI=3.14
来源：http://cwp.xuetiantiany.cn

[R04] 位置参数
来源：http://dtb.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hfd.hnqzz.top

[R05] 参数默认值
来源：http://yah.ydzc1.top

name="${1:-default}"
来源：http://jva.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://sjz.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yad.xziqi.cn

[R07] if 判断文件
来源：http://iak.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hnj.dashuyun.cn

[R08] 数值比较
来源：http://eii.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ztx.xuetiantiany.cn

[R09] 字符串比较
来源：http://vgd.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ohv.cashguo.top

[R10] 正则匹配
来源：http://kkm.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hlf.andypj.xyz

[R11] case 多分支
来源：http://mcr.ctjpmb.com

case "$1" in
来源：http://dbl.52xcode.cn

start) echo "启动" ;;
来源：http://qkj.xziqi.cn

stop)  echo "停止" ;;
来源：http://bzn.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://zmg.jinyuanbaomall.cn

esac
来源：http://moj.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://jiy.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://pkq.redwolf501.top

[R13] for 计数循环
来源：http://wow.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://qww.jqgufenzy.top

[R14] C 风格 for
来源：http://ugm.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pqf.nanxinkj.top

[R15] while 逐行读文件
来源：http://uih.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://onw.bjfxy.top

[R16] until 等待条件
来源：http://xou.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ise.zhixingplan.top

[R17] 数组定义与取值
来源：http://ynx.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://vvz.quarkkingdee.top

[R18] 遍历数组
来源：http://emo.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://unf.pengpengdd.cyou

[R19] 数组长度
来源：http://ect.smart0.xyz

echo "${#arr[@]}"
来源：http://krl.yj20258888.top

[R20] 关联数组（字典）
来源：http://whb.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bva.yonumen.top

[R21] 字符串长度
来源：http://hub.wangdashe.top

echo "${#s}"
来源：http://bqk.jyoumei.cn

[R22] 截取子串
来源：http://svo.nanxinkj.top

echo "${s:0:5}"
来源：http://kud.fzhhl.top

[R23] 字符串替换
来源：http://cpj.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kdr.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://igk.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://buh.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://dgk.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xmq.iojbl.cn

[R26] 命令替换
来源：http://qja.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://rfk.quarkkingdee.top

[R27] 算术展开
来源：http://grc.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://pxt.ybcxt.top

[R28] 浮点运算
来源：http://gbz.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://isx.hysaishi.cn

[R29] 定义函数
来源：http://zvr.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://flg.52xcode.cn

[R30] 函数返回状态码
来源：http://jvr.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://zii.jinqigufen.top

[R31] 局部变量
来源：http://eki.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://qcr.vehdjk.com

[R32] 参数个数校验
来源：http://rgb.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://htq.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://pct.kuanghao11.cn


<!-- 参考信息 -->