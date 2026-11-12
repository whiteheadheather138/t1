代发 wailian999

PHP:  // 手写时间戳比较
来源：http://suv.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjg.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://slu.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vyg.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fxc.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://omx.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vur.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://hsm.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fgn.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dtu.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nnc.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lin.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wwr.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jbo.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://flh.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wxl.yj20258888.top

================================================================================
来源：http://hli.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dzn.yanxiufei.cn

================================================================================
来源：http://cvt.vqdsnc.cn

[Q01] 创建表
来源：http://kvt.hnqzz.top

CREATE TABLE users (
来源：http://giz.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zyl.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://cli.hfpthk.cn

email VARCHAR(100) UNIQUE,
来源：http://pxu.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xpf.ivvv.top

);
来源：http://gqe.52xcode.cn

[Q02] 创建带外键的表
来源：http://wmi.zhongyouzk.top

CREATE TABLE orders (
来源：http://wdl.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nld.chenlongwang.top

user_id INT NOT NULL,
来源：http://aun.hcnkem.com

amount DECIMAL(10, 2),
来源：http://xzm.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lwu.meibo888.top

);
来源：http://crs.shangyingyoupin.top

[Q03] 增加列
来源：http://dtt.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mjn.wangdashe.top

[Q04] 修改列类型
来源：http://wpy.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rwb.zdbjq.cn

[Q05] 重命名列
来源：http://fnl.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://liu.snrcjt.cn

[Q06] 删除列
来源：http://djg.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kho.52xcode.cn

[Q07] 删除表
来源：http://ttn.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://ylr.jqgfzy.top

[Q08] 创建普通索引
来源：http://ueh.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ysk.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://kcc.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yos.fanxiaobao.xyz

[Q10] 插入单行
来源：http://yni.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rmy.cdnleiting.top

[Q11] 一次插入多行
来源：http://cjm.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cki.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://xko.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pmz.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hqw.fehbvm.com

[Q13] 忽略重复插入
来源：http://kme.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fkn.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://igm.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpm.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iap.birdmap.top

[Q15] 查询全部
来源：http://jju.cqqwz.cn

SELECT * FROM users;
来源：http://nzy.aibaodan.cn

[Q16] 查询指定列
来源：http://uhl.9152youxi.cn

SELECT id, name FROM users;
来源：http://nzs.xuanzx.com

[Q17] 条件查询
来源：http://qqe.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://epd.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://teb.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://snk.tanke756.top

[Q19] 范围查询
来源：http://mez.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwc.fzhhl.top

[Q20] IN 列表
来源：http://cfo.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://obb.nanxinkj.top

[Q21] 空值判断
来源：http://nka.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://adx.cucudq.cn

[Q22] 排序
来源：http://xll.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://btm.daria6918.cn

[Q23] 分页
来源：http://jyn.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dub.yonumen.top

[Q24] 去重
来源：http://nkw.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://ued.shzxlz.cn

[Q25] 只取前 N 条
来源：http://kgp.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xwk.andypj.xyz

[Q26] 计数
来源：http://fwt.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://usy.zhixingplan.top

[Q27] 条件计数
来源：http://adj.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgr.shangyingyoupin.top

[Q28] 求和与平均
来源：http://rwq.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mig.cqqwz.cn

[Q29] 最大最小值
来源：http://sbh.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mdq.jiagoushi.top

[Q30] 分组统计
来源：http://wre.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fko.yj20258888.top

[Q31] 分组后过滤
来源：http://vkm.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mqs.yuxming.cn

[Q32] 分组拼接字符串
来源：http://aum.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rvz.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ucn.redwolf501.top

[Q33] 多列分组
来源：http://yja.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://izl.redwolf501.top

[Q34] 每组取第一条
来源：http://vbw.hnxiangtu.top

SELECT * FROM (
来源：http://jwu.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vjh.dashuyun.cn

) t WHERE rn = 1;
来源：http://wwk.snrcjt.cn

[Q35] 内连接
来源：http://wzl.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ukj.guowangkeji.top

[Q36] 左连接
来源：http://zys.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://odr.tarul.cn

[Q37] 右连接
来源：http://zke.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bnq.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://efw.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yhg.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://jnj.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rnw.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dgq.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://owb.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dkf.xinyue.icu

[Q41] 多表连接
来源：http://rmt.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zgd.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://qnz.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://xrl.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://emp.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://lbw.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xyg.zhoulong.xyz

[Q43] 标量子查询
来源：http://zbs.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tsb.xuanzx.com

[Q44] IN 子查询
来源：http://kna.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lvw.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://tun.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://emb.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://tnk.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pux.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://uvz.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uyp.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://spo.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://agx.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://vsn.zhixingplan.top

[Q49] 更新单行
来源：http://hkm.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://erb.hcnkem.com

[Q50] 批量更新
来源：http://ixz.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pep.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://szt.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://idy.hfpthk.cn

[Q52] 删除指定行
来源：http://fhh.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://cet.cdnleiting.top

[Q53] 按条件删除
来源：http://sze.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lzx.aizwys.cn

[Q54] 清空表
来源：http://lcx.fktsv.cn

TRUNCATE TABLE logs;
来源：http://inq.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://vqf.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tdf.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://jsc.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xso.zhoulong.xyz

[Q57] 行号
来源：http://gir.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jej.sysykeji.top

[Q58] 累计求和
来源：http://quw.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://plw.guowangkeji.top

[Q59] 分组内累计
来源：http://wcn.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tbq.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://gyz.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zux.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqd.redwolf501.top

[Q61] 移动平均
来源：http://ivd.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vfm.svipenyu.cn

[Q62] 分组占比
来源：http://fig.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xdo.daxiang520.top

[Q63] 开启事务
来源：http://luo.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wpw.cucudq.cn

[Q64] 提交事务
来源：http://ozx.hesvh.cn

COMMIT;
来源：http://whi.52xcode.cn

[Q65] 回滚事务
来源：http://zou.yueranfly.top

ROLLBACK;
来源：http://zbm.hnxiangtu.top

[Q66] 行锁查询
来源：http://zcg.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jrn.dianchejie.cn

[Q67] 设置隔离级别
来源：http://wwx.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ylv.gzhubu.top

[Q68] 保存点
来源：http://foy.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://xsy.pycfn.com

ROLLBACK TO sp1;
来源：http://wrd.fktsv.cn

[Q69] 查看执行计划
来源：http://xnu.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vnj.daxiang520.top

[Q70] 更新统计信息
来源：http://vhr.bjfxy.top

ANALYZE TABLE users;
来源：http://iso.ybcxt.top

[Q71] 查看建表语句
来源：http://tly.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnu.tian-w.cn

[Q72] 查看索引
来源：http://wtm.ppjwa.cn

SHOW INDEX FROM users;
来源：http://wim.jqgfzy.top

[Q73] 查看表状态
来源：http://uxk.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xik.snrcjt.cn

[Q74] 强制使用索引
来源：http://jcu.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qup.zhiwuduotai.top

[Q75] 日期格式化
来源：http://pcy.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xcw.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yez.jyoumei.cn

[Q76] 按天统计
来源：http://idp.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyu.hnxiangtu.top

[Q77] 时间加减
来源：http://fha.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mfn.guannengcc.top

[Q78] 当前时间
来源：http://xos.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tjo.hesvh.cn

[Q79] 字符串拼接
来源：http://tfv.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ieo.cqqwz.cn

[Q80] 字符串截取
来源：http://oeg.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://trv.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://paw.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jot.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://ueu.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bfl.9152youxi.cn

[Q83] 大小写转换
来源：http://qzb.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dtg.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://zvu.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://kpj.epnwcf.com

[Q85] 数值取整
来源：http://roc.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gzh.tarul.cn

[Q86] 读取 JSON 字段
来源：http://oqd.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ghl.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://bpd.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fgn.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://njn.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hhk.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://drd.shzxlz.cn

[Q89] 判断表是否存在
来源：http://gya.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tom.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://qvb.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zor.daria6918.cn

================================================================================
来源：http://izc.pycfn.com

R. Bash 专题
来源：http://hws.yfazqb.com

================================================================================
来源：http://yqm.fehbvm.com

[R01] shebang 与严格模式
来源：http://son.shzxlz.cn

#!/usr/bin/env bash
来源：http://kcp.xziqi.cn

set -euo pipefail
来源：http://nyc.meibo888.top

[R02] 变量赋值与使用
来源：http://rdx.fktsv.cn

name="Tom"; echo "$name"
来源：http://gjr.uphjek.com

[R03] 只读变量
来源：http://jfg.wangshuangyany.cn

readonly PI=3.14
来源：http://tdd.yonumen.top

[R04] 位置参数
来源：http://vgy.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ewe.tanke756.top

[R05] 参数默认值
来源：http://hwg.ppjwa.cn

name="${1:-default}"
来源：http://kwf.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://oqf.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://duy.pengpengdd.cyou

[R07] if 判断文件
来源：http://nvs.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://elp.zhijiandao.cn

[R08] 数值比较
来源：http://lmj.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://axp.cashguo.top

[R09] 字符串比较
来源：http://ogu.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zjr.wangdashe.top

[R10] 正则匹配
来源：http://ppk.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gvt.shzxlz.cn

[R11] case 多分支
来源：http://hpv.daxiang520.top

case "$1" in
来源：http://max.hnqzz.top

start) echo "启动" ;;
来源：http://kik.bbcook.cn

stop)  echo "停止" ;;
来源：http://eit.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://ysf.iojbl.cn

esac
来源：http://nqt.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://pmo.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://kpe.zdbjq.cn

[R13] for 计数循环
来源：http://gso.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://mbk.fktsv.cn

[R14] C 风格 for
来源：http://txa.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjt.zhijiandao.cn

[R15] while 逐行读文件
来源：http://eyh.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fop.jinqigfzy.top

[R16] until 等待条件
来源：http://lzu.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zve.52xcode.cn

[R17] 数组定义与取值
来源：http://gms.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ypa.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://ixz.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cmz.jinyuanbaomall.cn

[R19] 数组长度
来源：http://hhl.mhx1999.top

echo "${#arr[@]}"
来源：http://kcd.andypj.xyz

[R20] 关联数组（字典）
来源：http://eou.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zua.uphjek.com

[R21] 字符串长度
来源：http://frv.xuetiantiany.cn

echo "${#s}"
来源：http://pcx.yj20258888.top

[R22] 截取子串
来源：http://siu.zdbjq.cn

echo "${s:0:5}"
来源：http://jio.kuanghao11.cn

[R23] 字符串替换
来源：http://btu.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iyf.gogol.net.cn

[R24] 大小写转换
来源：http://gjt.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rxc.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://wou.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgo.hfpthk.cn

[R26] 命令替换
来源：http://rnr.yj202588.top

now=$(date +%F); echo "$now"
来源：http://vye.feifeiyinyue.top

[R27] 算术展开
来源：http://kcj.hnqzz.top

echo $((1 + 2 * 3))
来源：http://zrt.vehdjk.com

[R28] 浮点运算
来源：http://vhu.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://ecq.c1oappe.top

[R29] 定义函数
来源：http://uat.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hbo.yonumen.top

[R30] 函数返回状态码
来源：http://ntr.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://nej.andypj.xyz

[R31] 局部变量
来源：http://oaq.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://ovr.cucudq.cn

[R32] 参数个数校验
来源：http://yun.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://alc.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://mjz.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ygs.mhx1999.top

[R34] 退出时清理
来源：http://wez.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://fho.iojbl.cn

[R35] 后台执行并等待
来源：http://ueq.tarul.cn


<!-- 参考信息 -->