代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jmw.hcnkem.com

C#:   if (x is null) {}
来源：http://oos.ppjwa.cn

[P07] 防抖与节流
来源：http://swa.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://crw.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://ryh.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzr.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nut.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zpk.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pyo.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wsn.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fwi.ivvv.top

[P08] 处理浮点精度问题
来源：http://ofb.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://luf.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zup.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjw.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oiu.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hgd.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bgh.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xgw.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jcv.shanyushiyangkeji.top

================================================================================
来源：http://vma.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hlh.gaohongyu789.top

================================================================================
来源：http://ytq.ivvv.top

[Q01] 创建表
来源：http://ydy.ivvv.top

CREATE TABLE users (
来源：http://glh.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jaq.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://qge.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://zyg.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jow.yanxiufei.cn

);
来源：http://jbf.c1oappe.top

[Q02] 创建带外键的表
来源：http://beb.xuanzx.com

CREATE TABLE orders (
来源：http://akl.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhk.fengsongda.top

user_id INT NOT NULL,
来源：http://dyh.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://bjt.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wpd.zdqjudy.top

);
来源：http://ppg.zdbjq.cn

[Q03] 增加列
来源：http://cwh.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bwv.pycfn.com

[Q04] 修改列类型
来源：http://uwk.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qep.xuanzx.com

[Q05] 重命名列
来源：http://ael.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jce.iojbl.cn

[Q06] 删除列
来源：http://pdx.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://dau.52xcode.cn

[Q07] 删除表
来源：http://shy.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://cos.cheryme.top

[Q08] 创建普通索引
来源：http://sxe.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://civ.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://vkj.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vxv.wangdashe.top

[Q10] 插入单行
来源：http://reb.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bye.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://hqx.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://orw.tarul.cn

[Q12] 插入后取自增 ID
来源：http://lcc.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://plv.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cap.yfazqb.com

[Q13] 忽略重复插入
来源：http://bkz.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kkp.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://kwz.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcp.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mrp.tarul.cn

[Q15] 查询全部
来源：http://bhw.ctjpmb.com

SELECT * FROM users;
来源：http://uax.aizwys.cn

[Q16] 查询指定列
来源：http://vdq.birdmap.top

SELECT id, name FROM users;
来源：http://roy.hfpthk.cn

[Q17] 条件查询
来源：http://szf.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://abb.daria6918.cn

[Q18] 模糊匹配
来源：http://sno.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://emo.pengpengdd.cyou

[Q19] 范围查询
来源：http://yie.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gnm.jinqigufen.top

[Q20] IN 列表
来源：http://tlv.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://umw.ydjk.org.cn

[Q21] 空值判断
来源：http://gly.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oge.aibaodan.cn

[Q22] 排序
来源：http://qqa.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mal.xuetiantiany.cn

[Q23] 分页
来源：http://ihi.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jjo.wangdashe.top

[Q24] 去重
来源：http://vqf.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://fri.xziqi.cn

[Q25] 只取前 N 条
来源：http://xra.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eor.tian-w.cn

[Q26] 计数
来源：http://hug.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://jeq.cdnleiting.top

[Q27] 条件计数
来源：http://lir.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpp.cqqwz.cn

[Q28] 求和与平均
来源：http://hgq.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nwi.cashguo.top

[Q29] 最大最小值
来源：http://ije.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jlv.yuanzhike.top

[Q30] 分组统计
来源：http://xzi.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aio.jqgufenzy.top

[Q31] 分组后过滤
来源：http://kwl.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kvb.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://mwb.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kgv.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aul.shzxlz.cn

[Q33] 多列分组
来源：http://rux.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zfm.vehdjk.com

[Q34] 每组取第一条
来源：http://ibo.yj20258888.top

SELECT * FROM (
来源：http://vbp.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://shn.tianlin.xyz

) t WHERE rn = 1;
来源：http://cvm.sjlbkw.cn

[Q35] 内连接
来源：http://ovr.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vqv.birdmap.top

[Q36] 左连接
来源：http://nut.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nyv.gotoacloud.top

[Q37] 右连接
来源：http://inp.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gtv.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://nuv.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://unj.ivvv.top

[Q39] 自连接（查上下级）
来源：http://dwe.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://epr.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jci.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ooj.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://flq.gogol.net.cn

[Q41] 多表连接
来源：http://dly.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wko.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://tab.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://ppz.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://xxo.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://ylc.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tsr.sysykeji.top

[Q43] 标量子查询
来源：http://dpv.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pqa.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://joe.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcc.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://aoz.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqd.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aje.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://inm.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://dri.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hpa.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://lfp.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iqv.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://yfe.feifeiyinyue.top

[Q49] 更新单行
来源：http://jhx.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zkt.jinqigufen.top

[Q50] 批量更新
来源：http://ofy.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ibv.zhoulong.xyz

[Q51] 用子查询更新
来源：http://veb.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ngy.c1oappe.top

[Q52] 删除指定行
来源：http://wxm.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://ixp.zhengqikj.top

[Q53] 按条件删除
来源：http://bui.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tud.hammf.cn

[Q54] 清空表
来源：http://aoj.jianghu66.top

TRUNCATE TABLE logs;
来源：http://ico.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://gfh.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xeu.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://abo.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gel.hywenlv.cn

[Q57] 行号
来源：http://xqh.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lil.aizwys.cn

[Q58] 累计求和
来源：http://syx.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://acn.zhixingplan.top

[Q59] 分组内累计
来源：http://mqi.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dbo.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://pqp.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kts.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://spi.tian-w.cn

[Q61] 移动平均
来源：http://wqk.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpt.zdqjudy.top

[Q62] 分组占比
来源：http://ijz.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xjy.hammf.cn

[Q63] 开启事务
来源：http://bpd.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ifr.kuanghao11.cn

[Q64] 提交事务
来源：http://hlc.yfazqb.com

COMMIT;
来源：http://srk.yfazqb.com

[Q65] 回滚事务
来源：http://xsq.chenjidiqi.icu

ROLLBACK;
来源：http://lsl.zycfv.cn

[Q66] 行锁查询
来源：http://kbc.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tkw.yangfankeji.com

[Q67] 设置隔离级别
来源：http://nve.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oms.316326.xyz

[Q68] 保存点
来源：http://war.316326.xyz

SAVEPOINT sp1;
来源：http://mkv.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://ikj.yonumen.top

[Q69] 查看执行计划
来源：http://ojj.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ztz.yj20258888.top

[Q70] 更新统计信息
来源：http://bmz.zdbjq.cn

ANALYZE TABLE users;
来源：http://lyk.xinyue.icu

[Q71] 查看建表语句
来源：http://utl.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qds.hfpthk.cn

[Q72] 查看索引
来源：http://zpr.yuanzhike.top

SHOW INDEX FROM users;
来源：http://upu.hysaishi.cn

[Q73] 查看表状态
来源：http://wgm.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sbj.hywenlv.cn

[Q74] 强制使用索引
来源：http://lqm.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgf.ybcxt.top

[Q75] 日期格式化
来源：http://smf.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dag.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dky.hammf.cn

[Q76] 按天统计
来源：http://qze.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kdz.jqgfzy.top

[Q77] 时间加减
来源：http://kiy.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ieq.guowangkeji.top

[Q78] 当前时间
来源：http://jtk.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://roo.birdmap.top

[Q79] 字符串拼接
来源：http://tsu.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dzd.birdmap.top

[Q80] 字符串截取
来源：http://ecv.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hdu.sweek.top

[Q81] 字符串替换
来源：http://ura.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ptd.havefunace.top

[Q82] 字符长度与字节长度
来源：http://juo.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yfd.birdmap.top

[Q83] 大小写转换
来源：http://yuo.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mee.sxryk.cn

[Q84] 去除首尾空格
来源：http://qpf.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://qeb.pycfn.com

[Q85] 数值取整
来源：http://okt.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eei.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://snq.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vim.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://jja.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bnl.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://qpg.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lwy.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nxj.zdbjq.cn

[Q89] 判断表是否存在
来源：http://wnk.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qcg.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://oxd.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gct.ydjk.org.cn

================================================================================
来源：http://ilh.xylfe.cn

R. Bash 专题
来源：http://nmd.zhiwuduotai.top

================================================================================
来源：http://hjt.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://mmn.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://gie.zhijiandao.cn

set -euo pipefail
来源：http://ilt.yj20258.top

[R02] 变量赋值与使用
来源：http://kqp.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://npx.gogol.net.cn

[R03] 只读变量
来源：http://glx.haohaochexian.top

readonly PI=3.14
来源：http://seo.zhiwuduotai.top

[R04] 位置参数
来源：http://ypg.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kgd.sufxvd.cn

[R05] 参数默认值
来源：http://qqo.haohaochexian.top

name="${1:-default}"
来源：http://ked.c1oappe.top

[R06] 判断命令是否存在
来源：http://zky.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iru.sxryk.cn

[R07] if 判断文件
来源：http://qcx.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://exx.zhiwuduotai.top

[R08] 数值比较
来源：http://shw.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://uka.yuanzhike.top

[R09] 字符串比较
来源：http://jyy.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mub.yanxiufei.cn

[R10] 正则匹配
来源：http://old.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vjv.svipenyu.cn

[R11] case 多分支
来源：http://vbp.fzhhl.top

case "$1" in
来源：http://qco.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://tga.hfpthk.cn

stop)  echo "停止" ;;
来源：http://iks.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://gdd.hesvh.cn

esac
来源：http://xne.tianlin.xyz

[R12] for 遍历文件
来源：http://fik.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://eqg.jqgfzy.top

[R13] for 计数循环
来源：http://uhp.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://usw.xuetiantiany.cn

[R14] C 风格 for
来源：http://mhw.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ibj.wangdashe.top

[R15] while 逐行读文件
来源：http://wuh.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hsd.uphjek.com

[R16] until 等待条件
来源：http://cjp.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eta.aibaodan.cn

[R17] 数组定义与取值
来源：http://kig.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://djb.xziqi.cn

[R18] 遍历数组
来源：http://szb.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xks.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://nop.hammf.cn

echo "${#arr[@]}"
来源：http://nab.zdqjudy.top

[R20] 关联数组（字典）
来源：http://poc.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rkb.daria6918.cn

[R21] 字符串长度
来源：http://zxy.jqgfzy.top

echo "${#s}"
来源：http://vhy.hammf.cn

[R22] 截取子串
来源：http://zwd.nanxinkj.top

echo "${s:0:5}"
来源：http://nmd.fanxiaobao.xyz

[R23] 字符串替换
来源：http://wmk.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ltj.316326.xyz

[R24] 大小写转换
来源：http://aek.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://bpq.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://xtf.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uix.yj20258888.top

[R26] 命令替换
来源：http://alw.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://kav.hesvh.cn

[R27] 算术展开
来源：http://lds.mhx1999.top

echo $((1 + 2 * 3))
来源：http://coy.chenlongwang.top

[R28] 浮点运算
来源：http://npm.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://wwh.redwolf501.top

[R29] 定义函数
来源：http://ebh.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qtj.ctjpmb.com

[R30] 函数返回状态码
来源：http://sre.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://aug.jqgfzy.top

[R31] 局部变量
来源：http://wqf.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://pzk.cheryme.top

[R32] 参数个数校验
来源：http://jeg.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uir.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://iwz.hammf.cn


<!-- 参考信息 -->