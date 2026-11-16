代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://noe.iojbl.cn

C#:   if (x is null) {}
来源：http://iiq.shangyingyoupin.top

[P07] 防抖与节流
来源：http://zka.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://equ.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://azt.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghh.gaohongyu789.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxw.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfw.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lcj.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qur.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uqh.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://yfd.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xjn.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jog.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://whw.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://put.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lcg.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uig.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://koj.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scn.xuanzx.com

================================================================================
来源：http://qko.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nab.havefunace.top

================================================================================
来源：http://bne.tianlin.xyz

[Q01] 创建表
来源：http://fil.jinqigfzy.top

CREATE TABLE users (
来源：http://mle.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxj.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://ypl.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://qdq.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zhg.gzhubu.top

);
来源：http://mbl.chenzaomai.com

[Q02] 创建带外键的表
来源：http://zjq.xinyue.icu

CREATE TABLE orders (
来源：http://uep.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qre.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://hjg.tanke756.top

amount DECIMAL(10, 2),
来源：http://boy.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kjl.epnwcf.com

);
来源：http://oqk.yj20258888.top

[Q03] 增加列
来源：http://kii.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://evr.gotoacloud.top

[Q04] 修改列类型
来源：http://lkj.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pad.hongshengwenyu.top

[Q05] 重命名列
来源：http://hmt.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qxm.hongshengwenyu.top

[Q06] 删除列
来源：http://oms.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://usg.nanxuanxn.top

[Q07] 删除表
来源：http://bfm.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://wns.andypj.xyz

[Q08] 创建普通索引
来源：http://twy.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jjn.nanxinkj.top

[Q09] 创建唯一索引
来源：http://vsg.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wet.quarkkingdee.top

[Q10] 插入单行
来源：http://upw.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://knd.chenlongwang.top

[Q11] 一次插入多行
来源：http://yuz.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://djo.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://zug.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://xia.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bgn.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://ina.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kxu.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://buy.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://esa.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://llg.xuanzx.com

[Q15] 查询全部
来源：http://hce.hammf.cn

SELECT * FROM users;
来源：http://cux.uphjek.com

[Q16] 查询指定列
来源：http://ngl.jyoumei.cn

SELECT id, name FROM users;
来源：http://aza.tanke756.top

[Q17] 条件查询
来源：http://ont.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://inn.0kj1m.cn

[Q18] 模糊匹配
来源：http://ugx.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tkq.yongpay.top

[Q19] 范围查询
来源：http://ctb.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jny.yj202588.top

[Q20] IN 列表
来源：http://sba.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jzw.andypj.xyz

[Q21] 空值判断
来源：http://mvv.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ntc.316326.xyz

[Q22] 排序
来源：http://grc.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hxu.316326.xyz

[Q23] 分页
来源：http://bxw.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xui.ywan-chungtsiang.top

[Q24] 去重
来源：http://nkr.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://wxj.yj202588.top

[Q25] 只取前 N 条
来源：http://dtc.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ttp.bbcook.cn

[Q26] 计数
来源：http://iiq.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://rox.uphjek.com

[Q27] 条件计数
来源：http://fzp.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vle.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://fuv.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uin.yvedp.cn

[Q29] 最大最小值
来源：http://gjn.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xws.jqgufenzy.top

[Q30] 分组统计
来源：http://oyi.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uyb.zhijiandao.cn

[Q31] 分组后过滤
来源：http://lvd.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bzj.andypj.xyz

[Q32] 分组拼接字符串
来源：http://jdb.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fll.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eii.ivvv.top

[Q33] 多列分组
来源：http://zlp.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oxv.zycfv.cn

[Q34] 每组取第一条
来源：http://uuj.kuanghao11.cn

SELECT * FROM (
来源：http://qmf.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ehp.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://fck.zhiwuduotai.top

[Q35] 内连接
来源：http://yok.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ojo.dashuyun.cn

[Q36] 左连接
来源：http://ieq.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://exj.jlsjyb.cn

[Q37] 右连接
来源：http://aeb.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggo.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bjx.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://luq.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://koj.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://oez.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://anz.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://syg.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ykg.fzhhl.top

[Q41] 多表连接
来源：http://fjv.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kjv.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://lfq.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://vxr.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://uwn.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://ola.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ztq.daria6918.cn

[Q43] 标量子查询
来源：http://hyg.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blf.zdqjudy.top

[Q44] IN 子查询
来源：http://jyz.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ueo.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://gll.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://znh.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://yxg.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wcf.hesvh.cn

[Q47] 与平均值比较
来源：http://mbl.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ltg.316326.xyz

[Q48] CTE 公用表表达式
来源：http://ndz.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kgr.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://shg.zhixingplan.top

[Q49] 更新单行
来源：http://fpn.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yqe.pycfn.com

[Q50] 批量更新
来源：http://szh.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nbp.ppjwa.cn

[Q51] 用子查询更新
来源：http://jjf.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xnz.tian-w.cn

[Q52] 删除指定行
来源：http://ajm.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://kgx.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://pei.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ttz.yueranfly.top

[Q54] 清空表
来源：http://lha.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://qow.xinyue.icu

[Q55] 排名（并列占位）
来源：http://gsl.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hyk.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://pnq.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jgg.tian-w.cn

[Q57] 行号
来源：http://bmh.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cqt.shzxlz.cn

[Q58] 累计求和
来源：http://cod.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tfq.sweek.top

[Q59] 分组内累计
来源：http://yrn.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bsv.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://bwy.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wrf.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://igm.jiagoushi.top

[Q61] 移动平均
来源：http://nuh.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kdz.chenjidiqi.icu

[Q62] 分组占比
来源：http://cgx.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://upw.tian-w.cn

[Q63] 开启事务
来源：http://ogr.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pcb.tianlin.xyz

[Q64] 提交事务
来源：http://jqr.0kj1m.cn

COMMIT;
来源：http://rcg.aizwys.cn

[Q65] 回滚事务
来源：http://jxc.hcnkem.com

ROLLBACK;
来源：http://nhy.yj20258.top

[Q66] 行锁查询
来源：http://sfe.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qgc.ivvv.top

[Q67] 设置隔离级别
来源：http://hjc.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qzc.dianchejie.cn

[Q68] 保存点
来源：http://sow.hfpthk.cn

SAVEPOINT sp1;
来源：http://rmc.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://nlt.haohaochexian.top

[Q69] 查看执行计划
来源：http://cgw.yj20258.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjp.yvedp.cn

[Q70] 更新统计信息
来源：http://exk.ehwqpu.com

ANALYZE TABLE users;
来源：http://jko.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://nnp.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pik.ehwqpu.com

[Q72] 查看索引
来源：http://ohb.yvedp.cn

SHOW INDEX FROM users;
来源：http://xzk.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://rmg.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gvh.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://ryf.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgg.chenlongwang.top

[Q75] 日期格式化
来源：http://fot.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lhw.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iza.jinghuilouyu.cn

[Q76] 按天统计
来源：http://rpm.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jxm.zhijiandao.cn

[Q77] 时间加减
来源：http://efc.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vqy.uphjek.com

[Q78] 当前时间
来源：http://uqe.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dxe.vqdsnc.cn

[Q79] 字符串拼接
来源：http://qkx.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qsc.pycfn.com

[Q80] 字符串截取
来源：http://xkg.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xhi.jinqigufen.top

[Q81] 字符串替换
来源：http://cbh.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sql.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://hid.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xxr.kuanghao11.cn

[Q83] 大小写转换
来源：http://xjz.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lew.zycfv.cn

[Q84] 去除首尾空格
来源：http://jhb.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://kjw.yfazqb.com

[Q85] 数值取整
来源：http://vvb.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lsi.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://tgv.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pdx.xinyue.icu

[Q87] JSON 字段做条件
来源：http://yrw.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aaz.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://qrs.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zsx.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://svq.tarul.cn

[Q89] 判断表是否存在
来源：http://obv.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bbm.ydjk.org.cn

[Q90] 生成序号列
来源：http://lui.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnr.zhengqikj.top

================================================================================
来源：http://vem.birdmap.top

R. Bash 专题
来源：http://lgd.ydzc1.top

================================================================================
来源：http://ovg.hfpthk.cn

[R01] shebang 与严格模式
来源：http://ejy.yongpay.top

#!/usr/bin/env bash
来源：http://hby.jinghuilouyu.cn

set -euo pipefail
来源：http://lzw.chenzaomai.com

[R02] 变量赋值与使用
来源：http://way.mhx1999.top

name="Tom"; echo "$name"
来源：http://xfs.yj20258888.top

[R03] 只读变量
来源：http://ydz.yuxming.cn

readonly PI=3.14
来源：http://mdr.xuetiantiany.cn

[R04] 位置参数
来源：http://iel.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qez.mhx1999.top

[R05] 参数默认值
来源：http://lci.zhixingplan.top

name="${1:-default}"
来源：http://kvn.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://kaj.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tsw.chenlongwang.top

[R07] if 判断文件
来源：http://kri.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ltn.sysykeji.top

[R08] 数值比较
来源：http://ert.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://exx.iojbl.cn

[R09] 字符串比较
来源：http://joi.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jwd.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://vck.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qbq.aibaodan.cn

[R11] case 多分支
来源：http://zmt.9152youxi.cn

case "$1" in
来源：http://yjw.hesvh.cn

start) echo "启动" ;;
来源：http://byr.tianlin.xyz

stop)  echo "停止" ;;
来源：http://plj.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://kyx.aibaodan.cn

esac
来源：http://wkz.zhixingplan.top

[R12] for 遍历文件
来源：http://yds.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://sfs.sjlbkw.cn

[R13] for 计数循环
来源：http://oyu.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://vwy.zhijiandao.cn

[R14] C 风格 for
来源：http://emw.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cfe.cqqwz.cn

[R15] while 逐行读文件
来源：http://xrk.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bip.yfazqb.com

[R16] until 等待条件
来源：http://lxz.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nrm.cucudq.cn

[R17] 数组定义与取值
来源：http://enz.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://bor.ivvv.top

[R18] 遍历数组
来源：http://fyp.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yfj.jinghuilouyu.cn

[R19] 数组长度
来源：http://abx.yueranfly.top

echo "${#arr[@]}"
来源：http://wpi.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://sdy.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://keo.guowangkeji.top

[R21] 字符串长度
来源：http://gmp.xinyue.icu

echo "${#s}"
来源：http://sql.dianchejie.cn

[R22] 截取子串
来源：http://bhv.jinqigfzy.top

echo "${s:0:5}"
来源：http://ooo.snrcjt.cn

[R23] 字符串替换
来源：http://itt.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://umy.yj20258888.top

[R24] 大小写转换
来源：http://hvf.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://jcx.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://ple.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://lys.zdqjudy.top

[R26] 命令替换
来源：http://toc.birdmap.top

now=$(date +%F); echo "$now"
来源：http://nmr.dashuyun.cn

[R27] 算术展开
来源：http://vbt.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://jug.zhengqikj.top

[R28] 浮点运算
来源：http://rrt.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://qkk.xuanzx.com

[R29] 定义函数
来源：http://rjt.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uxb.gotoacloud.top

[R30] 函数返回状态码
来源：http://nzq.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://fsm.hfpthk.cn

[R31] 局部变量
来源：http://scy.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://miq.feifeiyinyue.top

[R32] 参数个数校验
来源：http://tbe.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ueb.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://caq.iojbl.cn


<!-- 参考信息 -->