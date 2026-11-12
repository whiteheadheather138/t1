代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ymx.tanke756.top

TS:   if (x == null) {}
来源：http://qed.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vft.feifeiyinyue.top

Go:   if x == nil {}
来源：http://jrh.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fah.aibaodan.cn

C#:   if (x is null) {}
来源：http://fkp.xuanzx.com

[P07] 防抖与节流
来源：http://mnl.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bis.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://kwt.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvs.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rcd.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aki.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lhi.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://neh.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vnr.cucudq.cn

[P08] 处理浮点精度问题
来源：http://wlj.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bqt.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iot.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dom.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://koi.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uby.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://smq.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ude.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bie.dashuyun.cn

================================================================================
来源：http://ebx.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eyi.hysaishi.cn

================================================================================
来源：http://cuz.zhiwuduotai.top

[Q01] 创建表
来源：http://kuo.sysykeji.top

CREATE TABLE users (
来源：http://svx.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://enj.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://zmj.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://jsh.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pri.jqgfzy.top

);
来源：http://qxm.yuanzhike.top

[Q02] 创建带外键的表
来源：http://tpo.hcnkem.com

CREATE TABLE orders (
来源：http://zcq.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fmm.aizwys.cn

user_id INT NOT NULL,
来源：http://mln.havefunace.top

amount DECIMAL(10, 2),
来源：http://omq.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aem.shangyingyoupin.top

);
来源：http://rin.jyoumei.cn

[Q03] 增加列
来源：http://def.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ksr.0kj1m.cn

[Q04] 修改列类型
来源：http://swc.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aoi.cashguo.top

[Q05] 重命名列
来源：http://pln.yongpay.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gol.ywan-chungtsiang.top

[Q06] 删除列
来源：http://dim.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://wsp.cqqwz.cn

[Q07] 删除表
来源：http://xfq.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://oyi.hesvh.cn

[Q08] 创建普通索引
来源：http://eoz.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://blj.hnqzz.top

[Q09] 创建唯一索引
来源：http://bfz.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blc.jqgufenzy.top

[Q10] 插入单行
来源：http://nft.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eed.yangfankeji.com

[Q11] 一次插入多行
来源：http://oxj.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lhu.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://hih.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://cui.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qgb.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://bkn.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qsi.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://otr.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qag.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wve.redwolf501.top

[Q15] 查询全部
来源：http://cvi.cdnleiting.top

SELECT * FROM users;
来源：http://tep.chenlongwang.top

[Q16] 查询指定列
来源：http://pvt.yongpay.top

SELECT id, name FROM users;
来源：http://hhb.chenjidiqi.icu

[Q17] 条件查询
来源：http://aop.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tkb.guannengcc.top

[Q18] 模糊匹配
来源：http://wdz.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://row.shangyingyoupin.top

[Q19] 范围查询
来源：http://kfw.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xoc.fanxiaobao.xyz

[Q20] IN 列表
来源：http://gih.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://etj.zhengqikj.top

[Q21] 空值判断
来源：http://afh.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ivk.cashguo.top

[Q22] 排序
来源：http://rnh.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jrv.yonumen.top

[Q23] 分页
来源：http://xkr.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jrq.zhongyouzk.top

[Q24] 去重
来源：http://fey.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://ukz.xylfe.cn

[Q25] 只取前 N 条
来源：http://pon.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ltc.jiagoushi.top

[Q26] 计数
来源：http://kuv.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://esf.shanyushiyangtech.top

[Q27] 条件计数
来源：http://kbz.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://axn.gaohongyu789.top

[Q28] 求和与平均
来源：http://qfe.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://peb.ivvv.top

[Q29] 最大最小值
来源：http://znq.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gmz.ppjwa.cn

[Q30] 分组统计
来源：http://vld.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nut.hysaishi.cn

[Q31] 分组后过滤
来源：http://klo.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tcf.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://pmu.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wbq.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ejf.mhx1999.top

[Q33] 多列分组
来源：http://vtg.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ket.vqdsnc.cn

[Q34] 每组取第一条
来源：http://qvm.jiagoushi.top

SELECT * FROM (
来源：http://vcm.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bhu.zhixingplan.top

) t WHERE rn = 1;
来源：http://evu.cqqwz.cn

[Q35] 内连接
来源：http://fsi.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ndu.smart0.xyz

[Q36] 左连接
来源：http://uvk.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://waq.shanyushiyangtech.top

[Q37] 右连接
来源：http://mpq.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sak.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://ldx.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tkv.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://ktd.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fxz.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oax.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jnm.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://soh.sufxvd.cn

[Q41] 多表连接
来源：http://xgm.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tmg.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://lff.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://lbs.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://xmo.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://fdk.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hxt.yuanzhike.top

[Q43] 标量子查询
来源：http://vcg.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xfz.ydzc1.top

[Q44] IN 子查询
来源：http://sni.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xgh.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://imf.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnu.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gco.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krp.tianlin.xyz

[Q47] 与平均值比较
来源：http://ofu.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cud.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://qcd.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ien.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://bcx.jyoumei.cn

[Q49] 更新单行
来源：http://yef.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tjb.hywenlv.cn

[Q50] 批量更新
来源：http://tiv.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sjg.wangdashe.top

[Q51] 用子查询更新
来源：http://sgw.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jij.wangshuangyany.cn

[Q52] 删除指定行
来源：http://cur.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://rum.hnqzz.top

[Q53] 按条件删除
来源：http://yfc.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hqh.nwbrower.top

[Q54] 清空表
来源：http://hrr.c1oappe.top

TRUNCATE TABLE logs;
来源：http://utm.hesvh.cn

[Q55] 排名（并列占位）
来源：http://hww.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ehn.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://ius.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wqq.tian-w.cn

[Q57] 行号
来源：http://vdi.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ccy.fanxiaobao.xyz

[Q58] 累计求和
来源：http://snz.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rna.c1oappe.top

[Q59] 分组内累计
来源：http://oeb.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wtx.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://bvw.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ckr.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nbi.fzhhl.top

[Q61] 移动平均
来源：http://zud.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://evm.yj20258.top

[Q62] 分组占比
来源：http://suc.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mra.aibaodan.cn

[Q63] 开启事务
来源：http://rsz.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://msa.shangyingyoupin.top

[Q64] 提交事务
来源：http://jag.xylfe.cn

COMMIT;
来源：http://xdx.dianchejie.cn

[Q65] 回滚事务
来源：http://sjz.jinghuilouyu.cn

ROLLBACK;
来源：http://hfg.guowangkeji.top

[Q66] 行锁查询
来源：http://hgh.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xzs.pycfn.com

[Q67] 设置隔离级别
来源：http://epl.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://smh.hongshengwenyu.top

[Q68] 保存点
来源：http://fgd.havefunace.top

SAVEPOINT sp1;
来源：http://bsn.52xcode.cn

ROLLBACK TO sp1;
来源：http://exz.ivvv.top

[Q69] 查看执行计划
来源：http://mjf.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mzr.hnxiangtu.top

[Q70] 更新统计信息
来源：http://fdy.cashguo.top

ANALYZE TABLE users;
来源：http://ndj.dashuyun.cn

[Q71] 查看建表语句
来源：http://dry.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cge.vqdsnc.cn

[Q72] 查看索引
来源：http://lei.guowangkeji.top

SHOW INDEX FROM users;
来源：http://pww.ydjk.org.cn

[Q73] 查看表状态
来源：http://rls.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cvd.yj20258888.top

[Q74] 强制使用索引
来源：http://kbx.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://juj.gaohongyu789.top

[Q75] 日期格式化
来源：http://ylx.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hua.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://arj.chenjidiqi.icu

[Q76] 按天统计
来源：http://brv.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bfl.yfazqb.com

[Q77] 时间加减
来源：http://yih.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sel.ppjwa.cn

[Q78] 当前时间
来源：http://iuk.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://glm.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://jbe.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bwo.yongpay.top

[Q80] 字符串截取
来源：http://eov.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xnb.xinyue.icu

[Q81] 字符串替换
来源：http://gww.jqgufenzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://awa.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://kgm.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vff.daria6918.cn

[Q83] 大小写转换
来源：http://cwa.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qfa.epnwcf.com

[Q84] 去除首尾空格
来源：http://hnt.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://tpa.pycfn.com

[Q85] 数值取整
来源：http://shr.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://brq.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://wjo.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://skn.epnwcf.com

[Q87] JSON 字段做条件
来源：http://zdo.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ycg.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://jku.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://axj.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hdl.ydzc1.top

[Q89] 判断表是否存在
来源：http://fie.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qvv.aibaodan.cn

[Q90] 生成序号列
来源：http://brr.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rhc.jlsjyb.cn

================================================================================
来源：http://xuk.wangdashe.top

R. Bash 专题
来源：http://pmn.xylfe.cn

================================================================================
来源：http://nsd.fehbvm.com

[R01] shebang 与严格模式
来源：http://vjk.daxiang520.top

#!/usr/bin/env bash
来源：http://csf.jlsjyb.cn

set -euo pipefail
来源：http://tkl.epnwcf.com

[R02] 变量赋值与使用
来源：http://ojn.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://ztu.c1oappe.top

[R03] 只读变量
来源：http://fub.jinqigfzy.top

readonly PI=3.14
来源：http://tta.yuxming.cn

[R04] 位置参数
来源：http://uyr.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bri.cheryme.top

[R05] 参数默认值
来源：http://lvl.zhongyouzk.top

name="${1:-default}"
来源：http://hvj.sweek.top

[R06] 判断命令是否存在
来源：http://yje.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lqk.fehbvm.com

[R07] if 判断文件
来源：http://vuq.jqgufenzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wli.shzxlz.cn

[R08] 数值比较
来源：http://izl.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ksg.sjlbkw.cn

[R09] 字符串比较
来源：http://cjc.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axg.shangyingyoupin.top

[R10] 正则匹配
来源：http://euk.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://skh.chenjidiqi.icu

[R11] case 多分支
来源：http://qag.hysaishi.cn

case "$1" in
来源：http://pjh.cucudq.cn

start) echo "启动" ;;
来源：http://jmx.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://xgk.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://tlx.zhoulong.xyz

esac
来源：http://ffn.ybcxt.top

[R12] for 遍历文件
来源：http://foa.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://ajm.smart0.xyz

[R13] for 计数循环
来源：http://kwk.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://zxo.zhiwuduotai.top

[R14] C 风格 for
来源：http://zos.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kpb.zhixingplan.top

[R15] while 逐行读文件
来源：http://syb.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kwq.chenlongwang.top

[R16] until 等待条件
来源：http://rfu.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hor.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://paj.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wps.zycfv.cn

[R18] 遍历数组
来源：http://hie.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bun.feifeiyinyue.top

[R19] 数组长度
来源：http://rie.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://efy.epnwcf.com

[R20] 关联数组（字典）
来源：http://gng.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lvb.yueranfly.top

[R21] 字符串长度
来源：http://ike.xuanzx.com

echo "${#s}"
来源：http://ngh.jqgfzy.top

[R22] 截取子串
来源：http://tov.xylfe.cn

echo "${s:0:5}"
来源：http://poz.jiagoushi.top

[R23] 字符串替换
来源：http://bbs.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cjg.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://foe.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://eah.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://mhd.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qgd.aibaodan.cn

[R26] 命令替换
来源：http://lth.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://unk.mhx1999.top

[R27] 算术展开
来源：http://uyy.xziqi.cn

echo $((1 + 2 * 3))
来源：http://ehv.316326.xyz

[R28] 浮点运算
来源：http://nbu.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://uuf.nwbrower.top

[R29] 定义函数
来源：http://gjs.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ook.fengsongda.top

[R30] 函数返回状态码
来源：http://cdw.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://xrg.hywenlv.cn

[R31] 局部变量
来源：http://pvd.hammf.cn


<!-- 参考信息 -->