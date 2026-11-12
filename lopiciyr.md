代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xol.316326.xyz

TS:   if (x == null) {}
来源：http://wiz.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://feg.kuanghao11.cn

Go:   if x == nil {}
来源：http://yhi.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yfr.yuxming.cn

C#:   if (x is null) {}
来源：http://vqy.chenjidiqi.icu

[P07] 防抖与节流
来源：http://ejy.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lxv.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://lgd.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzi.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikh.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lop.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ajb.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wdo.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dli.xziqi.cn

[P08] 处理浮点精度问题
来源：http://scl.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jke.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jzx.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://unc.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ggc.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bpn.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cue.fzhhl.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aun.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ape.jinqigfzy.top

================================================================================
来源：http://auu.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pqa.cucudq.cn

================================================================================
来源：http://wob.zhengqikj.top

[Q01] 创建表
来源：http://mnp.haohaochexian.top

CREATE TABLE users (
来源：http://dhv.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfb.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://hjx.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://usz.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rsn.bbcook.cn

);
来源：http://xdn.haohaochexian.top

[Q02] 创建带外键的表
来源：http://czl.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://eps.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pnq.iojbl.cn

user_id INT NOT NULL,
来源：http://dym.tian-w.cn

amount DECIMAL(10, 2),
来源：http://xkf.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ccz.jianghu66.top

);
来源：http://gki.zycfv.cn

[Q03] 增加列
来源：http://xzx.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://coo.jianghu66.top

[Q04] 修改列类型
来源：http://sli.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bqi.fanxiaobao.xyz

[Q05] 重命名列
来源：http://lbe.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ous.snrcjt.cn

[Q06] 删除列
来源：http://tjx.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://gst.zhiwuduotai.top

[Q07] 删除表
来源：http://jdv.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://yoh.yj20258888.top

[Q08] 创建普通索引
来源：http://rcp.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wnz.shzxlz.cn

[Q09] 创建唯一索引
来源：http://vpd.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehh.zhixingplan.top

[Q10] 插入单行
来源：http://kzd.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwc.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://yvj.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mfd.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://uqr.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://mpb.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hyn.havefunace.top

[Q13] 忽略重复插入
来源：http://ptg.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xus.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://qgt.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nyx.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ycf.fanxiaobao.xyz

[Q15] 查询全部
来源：http://cye.shzxlz.cn

SELECT * FROM users;
来源：http://wsj.quarkkingdee.top

[Q16] 查询指定列
来源：http://vgr.smart0.xyz

SELECT id, name FROM users;
来源：http://xyh.fehbvm.com

[Q17] 条件查询
来源：http://aez.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gra.jqgufenzy.top

[Q18] 模糊匹配
来源：http://pkc.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xrl.xziqi.cn

[Q19] 范围查询
来源：http://gpm.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tad.quarkkingdee.top

[Q20] IN 列表
来源：http://cjn.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pbi.tian-w.cn

[Q21] 空值判断
来源：http://htf.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://soe.havefunace.top

[Q22] 排序
来源：http://xcj.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lec.jyoumei.cn

[Q23] 分页
来源：http://pek.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://upu.gogol.net.cn

[Q24] 去重
来源：http://olm.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://cnn.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://yne.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://urm.9152youxi.cn

[Q26] 计数
来源：http://beh.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://laa.hnxiangtu.top

[Q27] 条件计数
来源：http://cic.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://anw.vqdsnc.cn

[Q28] 求和与平均
来源：http://xzg.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wjy.zhiwuduotai.top

[Q29] 最大最小值
来源：http://mxs.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jpw.sysykeji.top

[Q30] 分组统计
来源：http://uil.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pqq.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://ceq.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fqg.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://uvl.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hty.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ues.iojbl.cn

[Q33] 多列分组
来源：http://pys.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dll.dashuyun.cn

[Q34] 每组取第一条
来源：http://pil.shanyushiyangtech.top

SELECT * FROM (
来源：http://okw.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ybv.yj202588.top

) t WHERE rn = 1;
来源：http://win.fzhhl.top

[Q35] 内连接
来源：http://ibw.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzy.andypj.xyz

[Q36] 左连接
来源：http://klw.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vma.snrcjt.cn

[Q37] 右连接
来源：http://cwe.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vup.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bon.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rbi.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://ogw.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yuw.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gki.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oxz.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ylg.iojbl.cn

[Q41] 多表连接
来源：http://zga.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://gli.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://dnw.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ejr.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://rbg.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://kif.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zoo.shuidangran.top

[Q43] 标量子查询
来源：http://kwt.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://opd.xziqi.cn

[Q44] IN 子查询
来源：http://dol.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://txq.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://tjb.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lun.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://icq.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xaq.jyoumei.cn

[Q47] 与平均值比较
来源：http://ked.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://com.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://pic.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tka.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://vje.sweek.top

[Q49] 更新单行
来源：http://xpo.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ohu.xinyue.icu

[Q50] 批量更新
来源：http://lfd.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iyc.yuxming.cn

[Q51] 用子查询更新
来源：http://lwq.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sqc.chenzaomai.com

[Q52] 删除指定行
来源：http://hzi.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://fsj.hammf.cn

[Q53] 按条件删除
来源：http://juf.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lbw.zhiwuduotai.top

[Q54] 清空表
来源：http://omt.tarul.cn

TRUNCATE TABLE logs;
来源：http://ayh.havefunace.top

[Q55] 排名（并列占位）
来源：http://sio.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zdv.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://sxg.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mes.guowangkeji.top

[Q57] 行号
来源：http://ejo.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rqd.sufxvd.cn

[Q58] 累计求和
来源：http://egx.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nbf.jqgfzy.top

[Q59] 分组内累计
来源：http://gvq.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aac.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://jcv.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ibt.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://izk.fanxiaobao.xyz

[Q61] 移动平均
来源：http://epu.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fhg.nwbrower.top

[Q62] 分组占比
来源：http://ysj.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zcl.zhiwuduotai.top

[Q63] 开启事务
来源：http://deu.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kxo.cashguo.top

[Q64] 提交事务
来源：http://waj.zdqjudy.top

COMMIT;
来源：http://aht.fzhhl.top

[Q65] 回滚事务
来源：http://xtc.daxiang520.top

ROLLBACK;
来源：http://lbj.hnqzz.top

[Q66] 行锁查询
来源：http://zgz.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gyt.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://ein.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jlv.vehdjk.com

[Q68] 保存点
来源：http://uwa.yonumen.top

SAVEPOINT sp1;
来源：http://rwt.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://rbd.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://oah.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zno.chenlongwang.top

[Q70] 更新统计信息
来源：http://ckh.birdmap.top

ANALYZE TABLE users;
来源：http://ovk.yanxiufei.cn

[Q71] 查看建表语句
来源：http://kgl.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vsg.zhijiandao.cn

[Q72] 查看索引
来源：http://asc.jiagoushi.top

SHOW INDEX FROM users;
来源：http://mtu.ctjpmb.com

[Q73] 查看表状态
来源：http://btv.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ggi.bbcook.cn

[Q74] 强制使用索引
来源：http://sdd.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oxe.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://kyr.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nuc.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wti.cqqwz.cn

[Q76] 按天统计
来源：http://wqu.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rgm.hongshengwenyu.top

[Q77] 时间加减
来源：http://tqa.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kpg.tianlin.xyz

[Q78] 当前时间
来源：http://uwz.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gzs.guowangkeji.top

[Q79] 字符串拼接
来源：http://tpp.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://phz.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://wou.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qcs.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://cvr.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sgd.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://hik.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lmc.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://utp.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://txt.ehwqpu.com

[Q84] 去除首尾空格
来源：http://hqq.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://wyy.sysykeji.top

[Q85] 数值取整
来源：http://msa.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kzx.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://foc.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tch.yj20258888.top

[Q87] JSON 字段做条件
来源：http://nlk.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wxy.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://awv.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tih.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nuj.chenlongwang.top

[Q89] 判断表是否存在
来源：http://eyw.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dvi.zhijiandao.cn

[Q90] 生成序号列
来源：http://oqd.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iep.epnwcf.com

================================================================================
来源：http://uxp.xingfuxueyuan.xyz

R. Bash 专题
来源：http://pvu.cqqwz.cn

================================================================================
来源：http://csy.chenlongwang.top

[R01] shebang 与严格模式
来源：http://vbo.gotoacloud.top

#!/usr/bin/env bash
来源：http://efg.feifeiyinyue.top

set -euo pipefail
来源：http://fnd.jinqigufen.top

[R02] 变量赋值与使用
来源：http://mdc.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://xdx.pycfn.com

[R03] 只读变量
来源：http://vyy.yueranfly.top

readonly PI=3.14
来源：http://vld.fanxiaobao.xyz

[R04] 位置参数
来源：http://fcd.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tqa.0kj1m.cn

[R05] 参数默认值
来源：http://exu.svipenyu.cn

name="${1:-default}"
来源：http://opy.jyoumei.cn

[R06] 判断命令是否存在
来源：http://blu.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ggf.zhijiandao.cn

[R07] if 判断文件
来源：http://eru.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pxt.tian-w.cn

[R08] 数值比较
来源：http://rpn.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://exm.chenlongwang.top

[R09] 字符串比较
来源：http://mbn.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qif.hfpthk.cn

[R10] 正则匹配
来源：http://ahy.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mxb.xziqi.cn

[R11] case 多分支
来源：http://nre.hesvh.cn

case "$1" in
来源：http://dsi.tarul.cn

start) echo "启动" ;;
来源：http://nxm.yonumen.top

stop)  echo "停止" ;;
来源：http://czx.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://qll.jyoumei.cn

esac
来源：http://zxj.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://uuz.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://kmg.quarkkingdee.top

[R13] for 计数循环
来源：http://dbd.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://opy.dianchejie.cn

[R14] C 风格 for
来源：http://uzl.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mqx.cucudq.cn

[R15] while 逐行读文件
来源：http://aln.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dgx.316326.xyz

[R16] until 等待条件
来源：http://jdx.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ygi.vqdsnc.cn

[R17] 数组定义与取值
来源：http://ffs.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nfh.xuanzx.com

[R18] 遍历数组
来源：http://zea.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwu.pengpengdd.cyou

[R19] 数组长度
来源：http://cmk.gaohongyu789.top

echo "${#arr[@]}"
来源：http://foc.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://ulr.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pwb.mhx1999.top

[R21] 字符串长度
来源：http://sqd.hywenlv.cn

echo "${#s}"
来源：http://npk.gotoacloud.top

[R22] 截取子串
来源：http://gcw.bbcook.cn

echo "${s:0:5}"
来源：http://aif.yongpay.top

[R23] 字符串替换
来源：http://tye.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kio.wangshuangyany.cn

[R24] 大小写转换
来源：http://hyu.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://cmb.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://taz.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xck.yj20258888.top

[R26] 命令替换
来源：http://rzb.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://vam.dashuyun.cn

[R27] 算术展开
来源：http://kgf.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://hpj.jqgfzy.top

[R28] 浮点运算
来源：http://wzi.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://irw.wangdashe.top

[R29] 定义函数
来源：http://sev.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdy.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://vjv.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://wke.pycfn.com

[R31] 局部变量
来源：http://xmv.xuetiantiany.cn


<!-- 参考信息 -->