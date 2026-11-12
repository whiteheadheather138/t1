代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ewl.jiagoushi.top

C#:   if (x is null) {}
来源：http://wxj.fehbvm.com

[P07] 防抖与节流
来源：http://wba.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qpd.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://ols.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bzs.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdb.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hoz.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dsh.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cbs.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gzk.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://oez.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ssw.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kns.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://giv.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wbc.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hib.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rlk.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ohk.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://beb.daria6918.cn

================================================================================
来源：http://mar.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uig.chenzaomai.com

================================================================================
来源：http://qzz.yj20258888.top

[Q01] 创建表
来源：http://vrk.yj20258888.top

CREATE TABLE users (
来源：http://nww.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wwp.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://wpq.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://jxw.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mjz.cashguo.top

);
来源：http://dey.jyoumei.cn

[Q02] 创建带外键的表
来源：http://xsg.ppjwa.cn

CREATE TABLE orders (
来源：http://kui.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nwi.c1oappe.top

user_id INT NOT NULL,
来源：http://fui.xuanzx.com

amount DECIMAL(10, 2),
来源：http://siy.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://doo.zdqjudy.top

);
来源：http://ala.hfpthk.cn

[Q03] 增加列
来源：http://jif.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://faw.ctjpmb.com

[Q04] 修改列类型
来源：http://wjb.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nzl.sufxvd.cn

[Q05] 重命名列
来源：http://prb.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tzt.gaohongyu789.top

[Q06] 删除列
来源：http://sfj.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aep.daxiang520.top

[Q07] 删除表
来源：http://qyb.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://urj.yongpay.top

[Q08] 创建普通索引
来源：http://xya.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ubh.chenzaomai.com

[Q09] 创建唯一索引
来源：http://uqv.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://roc.guannengcc.top

[Q10] 插入单行
来源：http://fpk.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ygb.yuanzhike.top

[Q11] 一次插入多行
来源：http://pgl.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zls.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://xpz.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://pkg.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://agq.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://huk.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rkl.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://luw.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nee.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mqu.shzxlz.cn

[Q15] 查询全部
来源：http://jma.fanxiaobao.xyz

SELECT * FROM users;
来源：http://lfh.yvedp.cn

[Q16] 查询指定列
来源：http://rba.pycfn.com

SELECT id, name FROM users;
来源：http://rei.dashuyun.cn

[Q17] 条件查询
来源：http://xpi.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zui.c1oappe.top

[Q18] 模糊匹配
来源：http://dyz.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qhb.vehdjk.com

[Q19] 范围查询
来源：http://xgr.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tpx.fanxiaobao.xyz

[Q20] IN 列表
来源：http://okg.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nim.bbcook.cn

[Q21] 空值判断
来源：http://gex.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jlg.zhixingplan.top

[Q22] 排序
来源：http://riz.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hkr.xylfe.cn

[Q23] 分页
来源：http://iju.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tsp.nwbrower.top

[Q24] 去重
来源：http://udx.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://whf.xuanzx.com

[Q25] 只取前 N 条
来源：http://srd.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wkj.jinqigfzy.top

[Q26] 计数
来源：http://rcp.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://rjv.zhoulong.xyz

[Q27] 条件计数
来源：http://vty.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ulg.yangfankeji.com

[Q28] 求和与平均
来源：http://yfb.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oio.jinqigufen.top

[Q29] 最大最小值
来源：http://xyi.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zuw.iojbl.cn

[Q30] 分组统计
来源：http://amj.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://puu.cucudq.cn

[Q31] 分组后过滤
来源：http://bvm.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rfr.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://wsc.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zkj.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dep.yuxming.cn

[Q33] 多列分组
来源：http://zog.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kdc.redwolf501.top

[Q34] 每组取第一条
来源：http://xjd.guannengcc.top

SELECT * FROM (
来源：http://evu.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lxf.snrcjt.cn

) t WHERE rn = 1;
来源：http://hqk.vqdsnc.cn

[Q35] 内连接
来源：http://kkv.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://upb.cashguo.top

[Q36] 左连接
来源：http://wqq.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://suo.zdbjq.cn

[Q37] 右连接
来源：http://fer.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rqb.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://seh.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ovd.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://qze.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://crb.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tko.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eun.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nnh.zdbjq.cn

[Q41] 多表连接
来源：http://dga.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qef.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://nme.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://xdg.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://sps.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://zbw.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://myc.jinqigfzy.top

[Q43] 标量子查询
来源：http://ywq.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vjt.yueranfly.top

[Q44] IN 子查询
来源：http://qss.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://roe.hammf.cn

[Q45] EXISTS 判断存在
来源：http://gxs.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yjx.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://kap.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://thi.yvedp.cn

[Q47] 与平均值比较
来源：http://iil.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://imu.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://vgw.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hxd.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://tdf.fzhhl.top

[Q49] 更新单行
来源：http://uel.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xbw.yueranfly.top

[Q50] 批量更新
来源：http://djo.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bcc.sufxvd.cn

[Q51] 用子查询更新
来源：http://xws.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://phx.zhengqikj.top

[Q52] 删除指定行
来源：http://pia.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://bnn.zdbjq.cn

[Q53] 按条件删除
来源：http://omy.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://flr.hcnkem.com

[Q54] 清空表
来源：http://cok.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://bzl.mhx1999.top

[Q55] 排名（并列占位）
来源：http://eek.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qir.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://jvx.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sur.cashguo.top

[Q57] 行号
来源：http://wew.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://esh.sufxvd.cn

[Q58] 累计求和
来源：http://auj.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ezr.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://iev.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qjp.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://dyw.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ajb.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngs.havefunace.top

[Q61] 移动平均
来源：http://iba.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sfd.xylfe.cn

[Q62] 分组占比
来源：http://qbn.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wpq.nwbrower.top

[Q63] 开启事务
来源：http://trr.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pmz.yanxiufei.cn

[Q64] 提交事务
来源：http://wit.hywenlv.cn

COMMIT;
来源：http://wbx.shangyingyoupin.top

[Q65] 回滚事务
来源：http://akn.tianlin.xyz

ROLLBACK;
来源：http://ipm.yangfankeji.com

[Q66] 行锁查询
来源：http://ohn.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qgf.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://cjo.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oni.sxryk.cn

[Q68] 保存点
来源：http://psw.yuxming.cn

SAVEPOINT sp1;
来源：http://gwm.yongpay.top

ROLLBACK TO sp1;
来源：http://emf.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://oig.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bai.9152youxi.cn

[Q70] 更新统计信息
来源：http://dxp.havefunace.top

ANALYZE TABLE users;
来源：http://tjl.zycfv.cn

[Q71] 查看建表语句
来源：http://mgm.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://swt.daria6918.cn

[Q72] 查看索引
来源：http://juv.snrcjt.cn

SHOW INDEX FROM users;
来源：http://kcf.fengsongda.top

[Q73] 查看表状态
来源：http://qqi.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tnb.smart0.xyz

[Q74] 强制使用索引
来源：http://gmk.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rhq.gotoacloud.top

[Q75] 日期格式化
来源：http://xld.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tct.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lpd.jlsjyb.cn

[Q76] 按天统计
来源：http://ekd.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vse.hfpthk.cn

[Q77] 时间加减
来源：http://acb.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dbl.guannengcc.top

[Q78] 当前时间
来源：http://dsp.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifs.gzhubu.top

[Q79] 字符串拼接
来源：http://jpw.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://imq.jianghu66.top

[Q80] 字符串截取
来源：http://uxh.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ddh.vehdjk.com

[Q81] 字符串替换
来源：http://zhj.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xhd.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://avc.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://elo.dianchejie.cn

[Q83] 大小写转换
来源：http://bpy.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lzh.bbcook.cn

[Q84] 去除首尾空格
来源：http://tcz.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://dsk.dashuyun.cn

[Q85] 数值取整
来源：http://mbi.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mde.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://ivm.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qae.epnwcf.com

[Q87] JSON 字段做条件
来源：http://auq.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ceg.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://ldm.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oyo.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nip.aizwys.cn

[Q89] 判断表是否存在
来源：http://vcg.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mzb.xylfe.cn

[Q90] 生成序号列
来源：http://khq.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yhz.ybcxt.top

================================================================================
来源：http://geg.feifeiyinyue.top

R. Bash 专题
来源：http://vmi.aibaodan.cn

================================================================================
来源：http://wme.yueranfly.top

[R01] shebang 与严格模式
来源：http://wze.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://tvn.meibo888.top

set -euo pipefail
来源：http://lbq.ctjpmb.com

[R02] 变量赋值与使用
来源：http://tfr.bbcook.cn

name="Tom"; echo "$name"
来源：http://dvl.yuanzhike.top

[R03] 只读变量
来源：http://kcd.fzhhl.top

readonly PI=3.14
来源：http://lrh.fktsv.cn

[R04] 位置参数
来源：http://wuc.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zhp.aizwys.cn

[R05] 参数默认值
来源：http://lnp.uphjek.com

name="${1:-default}"
来源：http://fch.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://wys.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wvq.xylfe.cn

[R07] if 判断文件
来源：http://gbg.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ftz.tanke756.top

[R08] 数值比较
来源：http://qev.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ard.ybcxt.top

[R09] 字符串比较
来源：http://yji.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://skm.xinyue.icu

[R10] 正则匹配
来源：http://rat.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qcy.iojbl.cn

[R11] case 多分支
来源：http://ytk.sufxvd.cn

case "$1" in
来源：http://ult.guannengcc.top

start) echo "启动" ;;
来源：http://egw.zycfv.cn

stop)  echo "停止" ;;
来源：http://bui.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://zpz.hesvh.cn

esac
来源：http://fil.hywenlv.cn

[R12] for 遍历文件
来源：http://moj.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://utu.sufxvd.cn

[R13] for 计数循环
来源：http://tks.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://drq.gotoacloud.top

[R14] C 风格 for
来源：http://lft.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qcq.jqgfzy.top

[R15] while 逐行读文件
来源：http://tvp.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vst.redwolf501.top

[R16] until 等待条件
来源：http://nts.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amb.chenlongwang.top

[R17] 数组定义与取值
来源：http://wgy.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://mva.sysykeji.top

[R18] 遍历数组
来源：http://tji.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpe.tianlin.xyz

[R19] 数组长度
来源：http://klk.yangfankeji.com

echo "${#arr[@]}"
来源：http://yvy.guowangkeji.top

[R20] 关联数组（字典）
来源：http://cbf.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oqn.meibo888.top

[R21] 字符串长度
来源：http://rvc.jinyuanbaomall.cn

echo "${#s}"
来源：http://ykx.birdmap.top

[R22] 截取子串
来源：http://kdv.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://inm.cdnleiting.top

[R23] 字符串替换
来源：http://tac.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wls.jqgufenzy.top

[R24] 大小写转换
来源：http://qhs.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vth.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://rci.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cxw.sufxvd.cn

[R26] 命令替换
来源：http://mvx.yonumen.top

now=$(date +%F); echo "$now"
来源：http://xya.bbcook.cn

[R27] 算术展开
来源：http://khh.yj20258888.top

echo $((1 + 2 * 3))
来源：http://ssy.wangshuangyany.cn

[R28] 浮点运算
来源：http://zff.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://afx.xuanzx.com

[R29] 定义函数
来源：http://rjf.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eul.52xcode.cn

[R30] 函数返回状态码
来源：http://sse.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://qcb.hongshengwenyu.top

[R31] 局部变量
来源：http://djw.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://leu.52xcode.cn

[R32] 参数个数校验
来源：http://yjg.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zgz.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://fbk.cheryme.top


<!-- 参考信息 -->