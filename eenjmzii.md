代发 wailian999

PHP:  // 手写时间戳比较
来源：http://unx.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kjc.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zea.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vre.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aay.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hkw.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nas.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://mfe.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://civ.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ykq.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eym.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kgm.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvh.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rfx.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ymm.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xiy.52xcode.cn

================================================================================
来源：http://vcy.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cvo.cheryme.top

================================================================================
来源：http://kua.zdbjq.cn

[Q01] 创建表
来源：http://vdk.jinqigfzy.top

CREATE TABLE users (
来源：http://hof.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lup.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://dae.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://hbn.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nqq.0kj1m.cn

);
来源：http://gxr.hysaishi.cn

[Q02] 创建带外键的表
来源：http://vwk.aibaodan.cn

CREATE TABLE orders (
来源：http://wsf.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svk.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://ykd.yonumen.top

amount DECIMAL(10, 2),
来源：http://khg.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mhe.0kj1m.cn

);
来源：http://zho.cucudq.cn

[Q03] 增加列
来源：http://twj.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gbx.tanke756.top

[Q04] 修改列类型
来源：http://qld.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iwe.jqgufenzy.top

[Q05] 重命名列
来源：http://xcw.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://crl.zdbjq.cn

[Q06] 删除列
来源：http://wgv.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://ffm.guowangkeji.top

[Q07] 删除表
来源：http://jfs.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://hbi.yj202588.top

[Q08] 创建普通索引
来源：http://ltg.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zzq.yuanzhike.top

[Q09] 创建唯一索引
来源：http://jws.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fvz.hfpthk.cn

[Q10] 插入单行
来源：http://avu.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bmu.tarul.cn

[Q11] 一次插入多行
来源：http://eab.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pbb.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://pyr.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xuo.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lfo.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://myx.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nll.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://mxm.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hrg.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://azf.gotoacloud.top

[Q15] 查询全部
来源：http://rma.chenzaomai.com

SELECT * FROM users;
来源：http://mqb.ehwqpu.com

[Q16] 查询指定列
来源：http://xls.nwbrower.top

SELECT id, name FROM users;
来源：http://fsq.yuanzhike.top

[Q17] 条件查询
来源：http://roh.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojg.birdmap.top

[Q18] 模糊匹配
来源：http://esf.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gmr.hongshengwenyu.top

[Q19] 范围查询
来源：http://voc.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qff.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://rre.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qqn.dianchejie.cn

[Q21] 空值判断
来源：http://awq.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://pst.sxryk.cn

[Q22] 排序
来源：http://mdg.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vbl.redwolf501.top

[Q23] 分页
来源：http://yaz.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ltg.fengsongda.top

[Q24] 去重
来源：http://lma.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://bac.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://npe.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mrc.guowangkeji.top

[Q26] 计数
来源：http://otd.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://loh.aibaodan.cn

[Q27] 条件计数
来源：http://btp.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rid.zhijiandao.cn

[Q28] 求和与平均
来源：http://fuk.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vtz.hesvh.cn

[Q29] 最大最小值
来源：http://lse.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jun.0kj1m.cn

[Q30] 分组统计
来源：http://tqs.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lxm.hnxiangtu.top

[Q31] 分组后过滤
来源：http://cri.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://azj.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://xaa.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yyp.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cwv.yfazqb.com

[Q33] 多列分组
来源：http://fin.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gmp.snrcjt.cn

[Q34] 每组取第一条
来源：http://cbm.epnwcf.com

SELECT * FROM (
来源：http://iom.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wva.hesvh.cn

) t WHERE rn = 1;
来源：http://uas.aibaodan.cn

[Q35] 内连接
来源：http://cqm.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krb.hcnkem.com

[Q36] 左连接
来源：http://ths.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xgq.bjfxy.top

[Q37] 右连接
来源：http://eev.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wao.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tts.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pbe.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://zto.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hsa.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vkx.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ikp.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gwm.chenjidiqi.icu

[Q41] 多表连接
来源：http://sjx.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rky.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://wkc.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://fdo.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://yjm.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://ske.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lmb.snrcjt.cn

[Q43] 标量子查询
来源：http://rrs.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://koc.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://srx.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://omd.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://chq.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ata.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nxg.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsc.jyoumei.cn

[Q47] 与平均值比较
来源：http://rcu.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ktj.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://vkn.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cod.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://zfd.xuanzx.com

[Q49] 更新单行
来源：http://oya.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://umj.ctjpmb.com

[Q50] 批量更新
来源：http://ecb.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nim.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://ynd.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xhi.chenjidiqi.icu

[Q52] 删除指定行
来源：http://his.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://obq.chenzaomai.com

[Q53] 按条件删除
来源：http://jgr.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ivz.ivvv.top

[Q54] 清空表
来源：http://gei.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://xon.ivvv.top

[Q55] 排名（并列占位）
来源：http://dhc.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hve.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://lwd.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdk.9152youxi.cn

[Q57] 行号
来源：http://fbb.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yxv.shanyushiyangtech.top

[Q58] 累计求和
来源：http://lgd.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qyp.sxryk.cn

[Q59] 分组内累计
来源：http://utw.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cks.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://gza.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xss.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bbz.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://dph.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mmx.ctjpmb.com

[Q62] 分组占比
来源：http://tuw.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bwl.hywenlv.cn

[Q63] 开启事务
来源：http://kyt.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://djc.sjlbkw.cn

[Q64] 提交事务
来源：http://zrr.xuetiantiany.cn

COMMIT;
来源：http://llu.birdmap.top

[Q65] 回滚事务
来源：http://wlt.yuanzhike.top

ROLLBACK;
来源：http://csp.tarul.cn

[Q66] 行锁查询
来源：http://khj.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://flk.xuanzx.com

[Q67] 设置隔离级别
来源：http://nyq.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dtn.hnqzz.top

[Q68] 保存点
来源：http://tby.uphjek.com

SAVEPOINT sp1;
来源：http://nhy.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://uxf.havefunace.top

[Q69] 查看执行计划
来源：http://zib.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lrq.hammf.cn

[Q70] 更新统计信息
来源：http://wap.tarul.cn

ANALYZE TABLE users;
来源：http://bdj.havefunace.top

[Q71] 查看建表语句
来源：http://yio.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kwm.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://ufz.c1oappe.top

SHOW INDEX FROM users;
来源：http://enq.gaohongyu789.top

[Q73] 查看表状态
来源：http://nxb.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jri.yfazqb.com

[Q74] 强制使用索引
来源：http://wav.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pvv.wangdashe.top

[Q75] 日期格式化
来源：http://ufj.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sgw.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dik.zhijiandao.cn

[Q76] 按天统计
来源：http://btr.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nuu.kuanghao11.cn

[Q77] 时间加减
来源：http://thb.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qle.andypj.xyz

[Q78] 当前时间
来源：http://vpx.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://meo.yfazqb.com

[Q79] 字符串拼接
来源：http://wnn.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jxu.ehwqpu.com

[Q80] 字符串截取
来源：http://xfi.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tkn.yueranfly.top

[Q81] 字符串替换
来源：http://hxq.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivf.tarul.cn

[Q82] 字符长度与字节长度
来源：http://lhm.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjx.gzhubu.top

[Q83] 大小写转换
来源：http://lem.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ing.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://crp.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://jli.tianlin.xyz

[Q85] 数值取整
来源：http://kns.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pgf.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://xcb.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cad.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://vxc.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hed.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://pzo.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nik.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kqm.ehwqpu.com

[Q89] 判断表是否存在
来源：http://huo.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hll.gaohongyu789.top

[Q90] 生成序号列
来源：http://ldx.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://umg.ivvv.top

================================================================================
来源：http://ndh.jinqigufen.top

R. Bash 专题
来源：http://qim.havefunace.top

================================================================================
来源：http://rhd.epnwcf.com

[R01] shebang 与严格模式
来源：http://hob.aizwys.cn

#!/usr/bin/env bash
来源：http://qpc.zdbjq.cn

set -euo pipefail
来源：http://cap.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://ins.dianchejie.cn

name="Tom"; echo "$name"
来源：http://nkc.yanxiufei.cn

[R03] 只读变量
来源：http://msm.haohaochexian.top

readonly PI=3.14
来源：http://hld.xylfe.cn

[R04] 位置参数
来源：http://glp.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sng.52xcode.cn

[R05] 参数默认值
来源：http://tvb.pengpengdd.cyou

name="${1:-default}"
来源：http://cxn.sysykeji.top

[R06] 判断命令是否存在
来源：http://hmy.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://klp.havefunace.top

[R07] if 判断文件
来源：http://qwb.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ozq.jinqigufen.top

[R08] 数值比较
来源：http://znl.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ldy.pycfn.com

[R09] 字符串比较
来源：http://enq.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://onl.pengpengdd.cyou

[R10] 正则匹配
来源：http://uvk.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dnq.aizwys.cn

[R11] case 多分支
来源：http://okn.gogol.net.cn

case "$1" in
来源：http://tmw.jinqigfzy.top

start) echo "启动" ;;
来源：http://ixn.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://xym.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://rrw.yuanzhike.top

esac
来源：http://kbe.zhoulong.xyz

[R12] for 遍历文件
来源：http://vws.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://cql.yuxming.cn

[R13] for 计数循环
来源：http://iqw.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://jgp.gotoacloud.top

[R14] C 风格 for
来源：http://onf.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bes.hfpthk.cn

[R15] while 逐行读文件
来源：http://rpi.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cwg.sufxvd.cn

[R16] until 等待条件
来源：http://sbo.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qes.guannengcc.top

[R17] 数组定义与取值
来源：http://bio.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://qnl.chenlongwang.top

[R18] 遍历数组
来源：http://tph.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://btk.chenlongwang.top

[R19] 数组长度
来源：http://tsn.ppjwa.cn

echo "${#arr[@]}"
来源：http://qad.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://agv.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sai.epnwcf.com

[R21] 字符串长度
来源：http://qft.birdmap.top

echo "${#s}"
来源：http://gbk.redwolf501.top

[R22] 截取子串
来源：http://drx.yuxming.cn

echo "${s:0:5}"
来源：http://nib.cqqwz.cn

[R23] 字符串替换
来源：http://ahb.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ldz.cdnleiting.top

[R24] 大小写转换
来源：http://thw.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ocy.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://xjq.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jqe.yangfankeji.com

[R26] 命令替换
来源：http://qtg.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://nzf.sjlbkw.cn

[R27] 算术展开
来源：http://mrg.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://uuv.chenjidiqi.icu

[R28] 浮点运算
来源：http://vfq.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://jdw.ydzc1.top

[R29] 定义函数
来源：http://oqr.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hev.yangfankeji.com

[R30] 函数返回状态码
来源：http://xsa.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://pxw.bjfxy.top

[R31] 局部变量
来源：http://giz.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://zfw.kuanghao11.cn

[R32] 参数个数校验
来源：http://neh.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vvl.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://pqw.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://brd.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://qec.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ucz.yueranfly.top

[R35] 后台执行并等待
来源：http://vou.snrcjt.cn


<!-- 参考信息 -->