代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bjr.nanxinkj.top

C#:   if (x is null) {}
来源：http://eoj.ydzc1.top

[P07] 防抖与节流
来源：http://ulz.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://coq.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://pjp.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pez.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jtu.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qkw.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tow.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://baz.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://knf.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://gdc.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mjq.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uvv.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sbg.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jjs.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://trm.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://umy.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yaj.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bdo.aibaodan.cn

================================================================================
来源：http://wvj.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bjt.dianchejie.cn

================================================================================
来源：http://iab.uphjek.com

[Q01] 创建表
来源：http://txo.tarul.cn

CREATE TABLE users (
来源：http://ont.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qbz.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://vxp.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://iuc.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wzd.ppjwa.cn

);
来源：http://ypb.xinyue.icu

[Q02] 创建带外键的表
来源：http://wvi.cucudq.cn

CREATE TABLE orders (
来源：http://osg.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://icz.ppjwa.cn

user_id INT NOT NULL,
来源：http://wks.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://wsy.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cos.shzxlz.cn

);
来源：http://axe.yuxming.cn

[Q03] 增加列
来源：http://vdk.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wnt.sweek.top

[Q04] 修改列类型
来源：http://buu.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jeo.jiagoushi.top

[Q05] 重命名列
来源：http://wai.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qax.jqgufenzy.top

[Q06] 删除列
来源：http://uqa.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://exs.nanxuanxn.top

[Q07] 删除表
来源：http://qai.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://lqj.aibaodan.cn

[Q08] 创建普通索引
来源：http://aup.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lxi.haohaochexian.top

[Q09] 创建唯一索引
来源：http://qun.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oih.guannengcc.top

[Q10] 插入单行
来源：http://vtk.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nin.yanxiufei.cn

[Q11] 一次插入多行
来源：http://vqp.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ygn.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://hch.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://pfm.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cwa.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://wmq.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zju.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://art.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ksr.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wfz.epnwcf.com

[Q15] 查询全部
来源：http://xil.nanxinkj.top

SELECT * FROM users;
来源：http://lht.52xcode.cn

[Q16] 查询指定列
来源：http://gjs.shzxlz.cn

SELECT id, name FROM users;
来源：http://jrx.zdqjudy.top

[Q17] 条件查询
来源：http://gik.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tkm.nanxinkj.top

[Q18] 模糊匹配
来源：http://rlm.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cvi.zhijiandao.cn

[Q19] 范围查询
来源：http://kbv.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zlu.zhoulong.xyz

[Q20] IN 列表
来源：http://kzx.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tci.jyoumei.cn

[Q21] 空值判断
来源：http://zux.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mln.316326.xyz

[Q22] 排序
来源：http://jrj.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fpz.xuetiantiany.cn

[Q23] 分页
来源：http://tin.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qkm.jlsjyb.cn

[Q24] 去重
来源：http://acv.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://xso.jiagoushi.top

[Q25] 只取前 N 条
来源：http://fgz.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://acc.jiagoushi.top

[Q26] 计数
来源：http://yvj.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://spl.yuxming.cn

[Q27] 条件计数
来源：http://fps.cdnleiting.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ghe.jyoumei.cn

[Q28] 求和与平均
来源：http://utr.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://umb.shzxlz.cn

[Q29] 最大最小值
来源：http://wxb.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hcy.ppjwa.cn

[Q30] 分组统计
来源：http://bik.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sry.snrcjt.cn

[Q31] 分组后过滤
来源：http://xhn.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nar.52xcode.cn

[Q32] 分组拼接字符串
来源：http://jlq.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cxc.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qle.gzhubu.top

[Q33] 多列分组
来源：http://him.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mje.vqdsnc.cn

[Q34] 每组取第一条
来源：http://ukj.jianghu66.top

SELECT * FROM (
来源：http://zoe.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgo.gotoacloud.top

) t WHERE rn = 1;
来源：http://yns.shanyushiyangtech.top

[Q35] 内连接
来源：http://omk.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://otl.52xcode.cn

[Q36] 左连接
来源：http://wpt.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eyc.hammf.cn

[Q37] 右连接
来源：http://itz.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ieb.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://wih.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qqd.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://ung.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uns.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cqm.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uuc.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xrz.hammf.cn

[Q41] 多表连接
来源：http://ahu.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xsw.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://wyq.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://pzc.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://mbr.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://ehk.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://grv.guowangkeji.top

[Q43] 标量子查询
来源：http://yso.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oui.cheryme.top

[Q44] IN 子查询
来源：http://dxp.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://erq.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://tkm.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxq.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fsf.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbt.tian-w.cn

[Q47] 与平均值比较
来源：http://ley.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wgd.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://ild.hammf.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gtb.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://fpq.yj20258888.top

[Q49] 更新单行
来源：http://ata.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ylh.sxryk.cn

[Q50] 批量更新
来源：http://qfb.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wkc.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://ltd.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kau.gzhubu.top

[Q52] 删除指定行
来源：http://eiz.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://yuf.chenlongwang.top

[Q53] 按条件删除
来源：http://wff.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ybs.ivvv.top

[Q54] 清空表
来源：http://pgw.hammf.cn

TRUNCATE TABLE logs;
来源：http://xcx.sweek.top

[Q55] 排名（并列占位）
来源：http://rmr.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wga.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://wpp.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tpy.fanxiaobao.xyz

[Q57] 行号
来源：http://zsx.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mhp.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://bqs.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dls.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://ilt.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://egh.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://rnm.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bmo.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nal.meibo888.top

[Q61] 移动平均
来源：http://blo.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vcn.hammf.cn

[Q62] 分组占比
来源：http://qnu.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://akl.zhoulong.xyz

[Q63] 开启事务
来源：http://mvh.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://djm.sjlbkw.cn

[Q64] 提交事务
来源：http://idh.gaohongyu789.top

COMMIT;
来源：http://aaq.guowangkeji.top

[Q65] 回滚事务
来源：http://ibc.wangdashe.top

ROLLBACK;
来源：http://spr.zhijiandao.cn

[Q66] 行锁查询
来源：http://fqw.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oqj.tanke756.top

[Q67] 设置隔离级别
来源：http://uli.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jeb.redwolf501.top

[Q68] 保存点
来源：http://gxl.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://dsl.gogol.net.cn

ROLLBACK TO sp1;
来源：http://maa.yj20258888.top

[Q69] 查看执行计划
来源：http://zzn.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://siy.mhx1999.top

[Q70] 更新统计信息
来源：http://rwm.zycfv.cn

ANALYZE TABLE users;
来源：http://crz.ppjwa.cn

[Q71] 查看建表语句
来源：http://wvk.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fdi.yj20258888.top

[Q72] 查看索引
来源：http://vco.nwbrower.top

SHOW INDEX FROM users;
来源：http://kyy.yvedp.cn

[Q73] 查看表状态
来源：http://nfm.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ibl.epnwcf.com

[Q74] 强制使用索引
来源：http://miy.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://new.cdnleiting.top

[Q75] 日期格式化
来源：http://mgu.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wgh.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lfw.gzhubu.top

[Q76] 按天统计
来源：http://nlt.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://irh.uphjek.com

[Q77] 时间加减
来源：http://rco.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cxp.jqgufenzy.top

[Q78] 当前时间
来源：http://goh.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iln.hysaishi.cn

[Q79] 字符串拼接
来源：http://xen.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bfy.hnxiangtu.top

[Q80] 字符串截取
来源：http://jhu.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fow.havefunace.top

[Q81] 字符串替换
来源：http://kst.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cev.uphjek.com

[Q82] 字符长度与字节长度
来源：http://gkg.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://faz.jianghu66.top

[Q83] 大小写转换
来源：http://cqj.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmh.daxiang520.top

[Q84] 去除首尾空格
来源：http://pay.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://sbo.jqgfzy.top

[Q85] 数值取整
来源：http://usy.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ulg.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://mxh.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zrt.andypj.xyz

[Q87] JSON 字段做条件
来源：http://zuv.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lxx.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://gov.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://orr.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lrx.hesvh.cn

[Q89] 判断表是否存在
来源：http://whc.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dzm.jinqigufen.top

[Q90] 生成序号列
来源：http://wgc.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://znp.feifeiyinyue.top

================================================================================
来源：http://mdb.fktsv.cn

R. Bash 专题
来源：http://uax.mhx1999.top

================================================================================
来源：http://abp.tian-w.cn

[R01] shebang 与严格模式
来源：http://hfj.shzxlz.cn

#!/usr/bin/env bash
来源：http://bwd.xuetiantiany.cn

set -euo pipefail
来源：http://niu.zdqjudy.top

[R02] 变量赋值与使用
来源：http://jnk.52xcode.cn

name="Tom"; echo "$name"
来源：http://djy.chenjidiqi.icu

[R03] 只读变量
来源：http://kgr.haohaochexian.top

readonly PI=3.14
来源：http://xfj.vqdsnc.cn

[R04] 位置参数
来源：http://qmb.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.jyoumei.cn

[R05] 参数默认值
来源：http://spp.zhixingplan.top

name="${1:-default}"
来源：http://ota.hywenlv.cn

[R06] 判断命令是否存在
来源：http://yoj.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xlq.tarul.cn

[R07] if 判断文件
来源：http://qlh.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://enn.hcnkem.com

[R08] 数值比较
来源：http://ata.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vao.yuanzhike.top

[R09] 字符串比较
来源：http://thc.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yqq.xuanzx.com

[R10] 正则匹配
来源：http://aof.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dns.haohaochexian.top

[R11] case 多分支
来源：http://ibq.ppjwa.cn

case "$1" in
来源：http://yom.zdqjudy.top

start) echo "启动" ;;
来源：http://uxe.yueranfly.top

stop)  echo "停止" ;;
来源：http://val.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://gxe.ywan-chungtsiang.top

esac
来源：http://gak.fehbvm.com

[R12] for 遍历文件
来源：http://ntu.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://tio.bbcook.cn

[R13] for 计数循环
来源：http://pzs.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://hac.jinghuilouyu.cn

[R14] C 风格 for
来源：http://irm.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tss.zycfv.cn

[R15] while 逐行读文件
来源：http://kuv.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sin.jlsjyb.cn

[R16] until 等待条件
来源：http://qdg.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jnw.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://iqw.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fec.dianchejie.cn

[R18] 遍历数组
来源：http://any.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pua.yuxming.cn

[R19] 数组长度
来源：http://xbf.xziqi.cn

echo "${#arr[@]}"
来源：http://zjx.cdnleiting.top

[R20] 关联数组（字典）
来源：http://zqy.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lds.sweek.top

[R21] 字符串长度
来源：http://xpt.9152youxi.cn

echo "${#s}"
来源：http://kea.shzxlz.cn

[R22] 截取子串
来源：http://gpf.cdnleiting.top

echo "${s:0:5}"
来源：http://zho.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://ygr.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dlh.fktsv.cn

[R24] 大小写转换
来源：http://ozg.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fzs.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://kuo.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qfd.dianchejie.cn

[R26] 命令替换
来源：http://omh.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://bxn.xziqi.cn

[R27] 算术展开
来源：http://gvx.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://edn.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://pns.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://qnp.hesvh.cn

[R29] 定义函数
来源：http://vrv.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fyt.hcnkem.com

[R30] 函数返回状态码
来源：http://zbh.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://rjr.zycfv.cn

[R31] 局部变量
来源：http://jvb.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://bwv.ydzc1.top

[R32] 参数个数校验
来源：http://gzg.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yvt.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://sik.aibaodan.cn


<!-- 参考信息 -->