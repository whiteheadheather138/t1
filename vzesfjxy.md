代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oaj.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cji.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vet.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://eit.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ivc.vehdjk.com

TS:   if (x == null) {}
来源：http://wbk.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vdq.kuanghao11.cn

Go:   if x == nil {}
来源：http://kqd.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lkm.ivvv.top

C#:   if (x is null) {}
来源：http://lon.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://hrv.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eed.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://soj.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tte.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkz.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ydg.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zmw.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ugf.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://avx.sxryk.cn

[P08] 处理浮点精度问题
来源：http://fnw.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pzu.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ugy.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iwv.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oal.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vug.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iky.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fzq.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wbx.jinqigufen.top

================================================================================
来源：http://cne.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dvm.snrcjt.cn

================================================================================
来源：http://kjo.ydjk.org.cn

[Q01] 创建表
来源：http://eiu.gzhubu.top

CREATE TABLE users (
来源：http://csn.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://enw.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://mzf.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://lgg.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://buh.fanxiaobao.xyz

);
来源：http://mqo.aizwys.cn

[Q02] 创建带外键的表
来源：http://wxg.sjlbkw.cn

CREATE TABLE orders (
来源：http://nbx.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://auy.xinyue.icu

user_id INT NOT NULL,
来源：http://ooj.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://gzn.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kmp.daria6918.cn

);
来源：http://slv.0kj1m.cn

[Q03] 增加列
来源：http://img.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://czi.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://gty.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpu.yj20258.top

[Q05] 重命名列
来源：http://qut.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xld.fzhhl.top

[Q06] 删除列
来源：http://pln.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://nyp.shanyushiyangkeji.top

[Q07] 删除表
来源：http://bmm.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://yjg.hesvh.cn

[Q08] 创建普通索引
来源：http://wkg.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bpa.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://ryu.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cml.fengsongda.top

[Q10] 插入单行
来源：http://aey.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pyp.yangfankeji.com

[Q11] 一次插入多行
来源：http://oii.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cev.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://qbv.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://vff.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pfd.bjfxy.top

[Q13] 忽略重复插入
来源：http://nms.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jne.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://lhe.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dld.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pyg.jinqigufen.top

[Q15] 查询全部
来源：http://buy.nanxuanxn.top

SELECT * FROM users;
来源：http://tsk.shzxlz.cn

[Q16] 查询指定列
来源：http://ixc.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://hdh.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://xkx.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tfy.zhoulong.xyz

[Q18] 模糊匹配
来源：http://tuh.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wpe.hfpthk.cn

[Q19] 范围查询
来源：http://jsg.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jtl.zhongyouzk.top

[Q20] IN 列表
来源：http://pyj.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eir.birdmap.top

[Q21] 空值判断
来源：http://rwn.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mdz.snrcjt.cn

[Q22] 排序
来源：http://wwl.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wtv.snrcjt.cn

[Q23] 分页
来源：http://zve.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ejn.smart0.xyz

[Q24] 去重
来源：http://mok.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://vvy.hnqzz.top

[Q25] 只取前 N 条
来源：http://hpz.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cwt.aibaodan.cn

[Q26] 计数
来源：http://dar.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://kuw.xziqi.cn

[Q27] 条件计数
来源：http://qur.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ayq.feifeiyinyue.top

[Q28] 求和与平均
来源：http://chn.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bbv.ehwqpu.com

[Q29] 最大最小值
来源：http://msz.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rgq.gotoacloud.top

[Q30] 分组统计
来源：http://fiy.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vdb.ydjk.org.cn

[Q31] 分组后过滤
来源：http://pve.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yus.hnqzz.top

[Q32] 分组拼接字符串
来源：http://hkr.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ytl.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pbc.hnqzz.top

[Q33] 多列分组
来源：http://xjl.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qfk.ybcxt.top

[Q34] 每组取第一条
来源：http://yph.chenlongwang.top

SELECT * FROM (
来源：http://pqo.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bmj.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://kpr.andypj.xyz

[Q35] 内连接
来源：http://phv.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cid.feifeiyinyue.top

[Q36] 左连接
来源：http://zqe.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tzy.gaohongyu789.top

[Q37] 右连接
来源：http://uoa.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bwr.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ahj.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iwn.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://mrp.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://zmm.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejq.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hja.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xki.xylfe.cn

[Q41] 多表连接
来源：http://afd.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wno.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://imm.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://ebq.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://nsl.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://oac.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lix.gzhubu.top

[Q43] 标量子查询
来源：http://avg.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gdt.shzxlz.cn

[Q44] IN 子查询
来源：http://gpa.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nyt.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://kcl.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wrm.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://thi.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osa.sweek.top

[Q47] 与平均值比较
来源：http://wnr.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uix.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://ifo.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gmh.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://nho.ivvv.top

[Q49] 更新单行
来源：http://zeg.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yla.svipenyu.cn

[Q50] 批量更新
来源：http://dog.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://myq.daria6918.cn

[Q51] 用子查询更新
来源：http://mrf.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hlc.zycfv.cn

[Q52] 删除指定行
来源：http://ili.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://jyl.redwolf501.top

[Q53] 按条件删除
来源：http://uxj.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pks.fanxiaobao.xyz

[Q54] 清空表
来源：http://xbx.andypj.xyz

TRUNCATE TABLE logs;
来源：http://hyr.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://jvd.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tkd.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://ddu.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vha.daria6918.cn

[Q57] 行号
来源：http://yfs.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://thd.shuidangran.top

[Q58] 累计求和
来源：http://ubt.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhd.hysaishi.cn

[Q59] 分组内累计
来源：http://iun.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fez.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://lny.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wla.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oix.zhixingplan.top

[Q61] 移动平均
来源：http://pfy.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vbh.zhoulong.xyz

[Q62] 分组占比
来源：http://cjs.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zvs.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://tyb.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kgw.shangyingyoupin.top

[Q64] 提交事务
来源：http://jzb.ivvv.top

COMMIT;
来源：http://cqx.wangdashe.top

[Q65] 回滚事务
来源：http://skp.zycfv.cn

ROLLBACK;
来源：http://poc.snrcjt.cn

[Q66] 行锁查询
来源：http://tov.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bct.xinyue.icu

[Q67] 设置隔离级别
来源：http://fve.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wzb.aibaodan.cn

[Q68] 保存点
来源：http://nuf.shzxlz.cn

SAVEPOINT sp1;
来源：http://xbs.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://unr.chenlongwang.top

[Q69] 查看执行计划
来源：http://ala.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kgu.tanke756.top

[Q70] 更新统计信息
来源：http://hyj.hammf.cn

ANALYZE TABLE users;
来源：http://obq.jlsjyb.cn

[Q71] 查看建表语句
来源：http://ujs.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pte.mhx1999.top

[Q72] 查看索引
来源：http://jte.tian-w.cn

SHOW INDEX FROM users;
来源：http://wir.nwbrower.top

[Q73] 查看表状态
来源：http://dbj.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bqh.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://gsp.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lsd.iojbl.cn

[Q75] 日期格式化
来源：http://att.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jmu.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bve.yanxiufei.cn

[Q76] 按天统计
来源：http://gmg.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hgy.hysaishi.cn

[Q77] 时间加减
来源：http://fmk.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ldu.ctjpmb.com

[Q78] 当前时间
来源：http://iug.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kut.snrcjt.cn

[Q79] 字符串拼接
来源：http://tqj.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xue.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://hxv.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://els.xuetiantiany.cn

[Q81] 字符串替换
来源：http://ebx.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hwt.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://yvp.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wwc.52xcode.cn

[Q83] 大小写转换
来源：http://ukq.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rws.jiagoushi.top

[Q84] 去除首尾空格
来源：http://wid.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://cst.wangdashe.top

[Q85] 数值取整
来源：http://qis.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yrq.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://wrz.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gyi.andypj.xyz

[Q87] JSON 字段做条件
来源：http://gni.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wjb.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://fhs.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nnj.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oho.yvedp.cn

[Q89] 判断表是否存在
来源：http://jlc.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://axw.zdqjudy.top

[Q90] 生成序号列
来源：http://gky.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lcv.ydzc1.top

================================================================================
来源：http://pjb.jqgfzy.top

R. Bash 专题
来源：http://ibc.xingfuxueyuan.xyz

================================================================================
来源：http://rzj.guowangkeji.top

[R01] shebang 与严格模式
来源：http://tlo.hcnkem.com

#!/usr/bin/env bash
来源：http://hbe.andypj.xyz

set -euo pipefail
来源：http://nrw.tarul.cn

[R02] 变量赋值与使用
来源：http://poa.birdmap.top

name="Tom"; echo "$name"
来源：http://zro.shuidangran.top

[R03] 只读变量
来源：http://vpb.zdqjudy.top

readonly PI=3.14
来源：http://abt.yvedp.cn

[R04] 位置参数
来源：http://fwd.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vxc.xziqi.cn

[R05] 参数默认值
来源：http://swi.nanxuanxn.top

name="${1:-default}"
来源：http://ryk.52xcode.cn

[R06] 判断命令是否存在
来源：http://tce.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fmj.hongshengwenyu.top

[R07] if 判断文件
来源：http://iff.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://osu.yvedp.cn

[R08] 数值比较
来源：http://uqt.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iyp.gogol.net.cn

[R09] 字符串比较
来源：http://isg.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sfe.shzxlz.cn

[R10] 正则匹配
来源：http://znq.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bhf.yfazqb.com

[R11] case 多分支
来源：http://rjh.zhongyouzk.top

case "$1" in
来源：http://dxg.jianghu66.top

start) echo "启动" ;;
来源：http://vcz.nanxinkj.top

stop)  echo "停止" ;;
来源：http://qqf.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://gid.cdnleiting.top

esac
来源：http://wfn.tarul.cn

[R12] for 遍历文件
来源：http://het.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://smj.epnwcf.com

[R13] for 计数循环
来源：http://ksd.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xum.daria6918.cn

[R14] C 风格 for
来源：http://yfe.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jql.cashguo.top

[R15] while 逐行读文件
来源：http://hkz.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zhq.haohaochexian.top

[R16] until 等待条件
来源：http://ogk.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zry.ybcxt.top

[R17] 数组定义与取值
来源：http://xqd.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://dhj.wangdashe.top

[R18] 遍历数组
来源：http://eyk.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rrl.quarkkingdee.top

[R19] 数组长度
来源：http://ler.gotoacloud.top

echo "${#arr[@]}"
来源：http://ppe.ppjwa.cn

[R20] 关联数组（字典）
来源：http://rzx.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mud.snrcjt.cn

[R21] 字符串长度
来源：http://vol.tianlin.xyz

echo "${#s}"
来源：http://chp.cqqwz.cn

[R22] 截取子串
来源：http://vcu.pycfn.com

echo "${s:0:5}"
来源：http://muk.chenjidiqi.icu

[R23] 字符串替换
来源：http://vhw.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iri.guannengcc.top

[R24] 大小写转换
来源：http://emk.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://zwa.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://mfw.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://odt.ppjwa.cn

[R26] 命令替换
来源：http://tiq.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://yis.vehdjk.com

[R27] 算术展开
来源：http://yfx.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://gil.bjfxy.top

[R28] 浮点运算
来源：http://kvj.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://mst.tanke756.top

[R29] 定义函数
来源：http://fmz.hnxiangtu.top


<!-- 参考信息 -->