代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aef.bjfxy.top

C#:   if (x is null) {}
来源：http://akc.cucudq.cn

[P07] 防抖与节流
来源：http://vgs.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gdx.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://gpq.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uze.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqu.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tup.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lcp.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqe.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iie.xuanzx.com

[P08] 处理浮点精度问题
来源：http://czv.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ofy.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fdu.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mfd.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jxg.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dgi.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cno.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qsp.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://izk.iojbl.cn

================================================================================
来源：http://aex.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yuy.yvedp.cn

================================================================================
来源：http://acx.havefunace.top

[Q01] 创建表
来源：http://hfp.zhixingplan.top

CREATE TABLE users (
来源：http://ikk.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zbv.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://eeu.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://fbu.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://icv.daxiang520.top

);
来源：http://xxu.tarul.cn

[Q02] 创建带外键的表
来源：http://xtf.mhx1999.top

CREATE TABLE orders (
来源：http://kli.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bed.fehbvm.com

user_id INT NOT NULL,
来源：http://ivw.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://ihi.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dir.fengsongda.top

);
来源：http://ixf.quarkkingdee.top

[Q03] 增加列
来源：http://ege.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lhh.jqgfzy.top

[Q04] 修改列类型
来源：http://zep.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gwq.fanxiaobao.xyz

[Q05] 重命名列
来源：http://yiq.zdqjudy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rvk.hnqzz.top

[Q06] 删除列
来源：http://njf.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://hpv.gogol.net.cn

[Q07] 删除表
来源：http://gin.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://ctg.c1oappe.top

[Q08] 创建普通索引
来源：http://pog.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wbu.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://inl.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqy.mhx1999.top

[Q10] 插入单行
来源：http://vob.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fzs.yanxiufei.cn

[Q11] 一次插入多行
来源：http://vjl.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://azt.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://xce.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rqk.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gzh.vehdjk.com

[Q13] 忽略重复插入
来源：http://fys.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ppp.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://lwv.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dde.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eog.haohaochexian.top

[Q15] 查询全部
来源：http://omt.pengpengdd.cyou

SELECT * FROM users;
来源：http://vnz.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://pwq.9152youxi.cn

SELECT id, name FROM users;
来源：http://lwx.zhixingplan.top

[Q17] 条件查询
来源：http://zye.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uck.yfazqb.com

[Q18] 模糊匹配
来源：http://dby.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xja.ybcxt.top

[Q19] 范围查询
来源：http://igu.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ozu.zycfv.cn

[Q20] IN 列表
来源：http://wug.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vxe.hongshengwenyu.top

[Q21] 空值判断
来源：http://zus.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://okx.daxiang520.top

[Q22] 排序
来源：http://xkr.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://str.cheryme.top

[Q23] 分页
来源：http://ioh.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kwr.tarul.cn

[Q24] 去重
来源：http://tzx.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://pwx.hnxiangtu.top

[Q25] 只取前 N 条
来源：http://ikg.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mcl.tarul.cn

[Q26] 计数
来源：http://wdu.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://oab.hesvh.cn

[Q27] 条件计数
来源：http://twj.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pfn.yj202588.top

[Q28] 求和与平均
来源：http://tcz.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tat.sweek.top

[Q29] 最大最小值
来源：http://nqi.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://fsu.kuanghao11.cn

[Q30] 分组统计
来源：http://cjn.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lhw.hfpthk.cn

[Q31] 分组后过滤
来源：http://yie.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zkc.iojbl.cn

[Q32] 分组拼接字符串
来源：http://kpw.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://azt.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jqf.shanyushiyangtech.top

[Q33] 多列分组
来源：http://otn.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fly.yonumen.top

[Q34] 每组取第一条
来源：http://cgr.yanxiufei.cn

SELECT * FROM (
来源：http://wog.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jus.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://cve.vehdjk.com

[Q35] 内连接
来源：http://hkp.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://acg.xziqi.cn

[Q36] 左连接
来源：http://jsg.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ggs.cqqwz.cn

[Q37] 右连接
来源：http://fdq.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sjs.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ffs.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dae.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://uie.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wtl.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iec.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aki.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ola.bjfxy.top

[Q41] 多表连接
来源：http://yer.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jdy.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://nay.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://xeh.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://zeb.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://fqf.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lez.nanxinkj.top

[Q43] 标量子查询
来源：http://duv.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rjb.hywenlv.cn

[Q44] IN 子查询
来源：http://ngd.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gpa.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://gdr.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gkd.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://you.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzw.yuxming.cn

[Q47] 与平均值比较
来源：http://ays.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pba.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://xah.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://npk.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://ryn.xuetiantiany.cn

[Q49] 更新单行
来源：http://pad.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tzy.aibaodan.cn

[Q50] 批量更新
来源：http://nqa.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://upv.fktsv.cn

[Q51] 用子查询更新
来源：http://unx.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ear.yongpay.top

[Q52] 删除指定行
来源：http://kzt.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://mfd.kuanghao11.cn

[Q53] 按条件删除
来源：http://juc.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xbw.fktsv.cn

[Q54] 清空表
来源：http://hcc.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://ffo.vehdjk.com

[Q55] 排名（并列占位）
来源：http://fkc.fehbvm.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvc.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://ahs.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xgu.svipenyu.cn

[Q57] 行号
来源：http://cnf.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hdy.fanxiaobao.xyz

[Q58] 累计求和
来源：http://nbq.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wqz.jqgufenzy.top

[Q59] 分组内累计
来源：http://wak.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://prg.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://hak.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jms.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hzl.nanxinkj.top

[Q61] 移动平均
来源：http://jtz.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nda.nanxuanxn.top

[Q62] 分组占比
来源：http://rgg.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sra.cashguo.top

[Q63] 开启事务
来源：http://obr.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yjl.uphjek.com

[Q64] 提交事务
来源：http://wia.jyoumei.cn

COMMIT;
来源：http://oyc.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://bip.quarkkingdee.top

ROLLBACK;
来源：http://otc.wangshuangyany.cn

[Q66] 行锁查询
来源：http://rdb.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sdn.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://qdn.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igo.zhiwuduotai.top

[Q68] 保存点
来源：http://thm.jiagoushi.top

SAVEPOINT sp1;
来源：http://qiq.xylfe.cn

ROLLBACK TO sp1;
来源：http://jsr.fzhhl.top

[Q69] 查看执行计划
来源：http://kxk.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xes.epnwcf.com

[Q70] 更新统计信息
来源：http://hek.bjfxy.top

ANALYZE TABLE users;
来源：http://fqj.sysykeji.top

[Q71] 查看建表语句
来源：http://gzp.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lfr.hnxiangtu.top

[Q72] 查看索引
来源：http://aun.zhixingplan.top

SHOW INDEX FROM users;
来源：http://vmz.chenjidiqi.icu

[Q73] 查看表状态
来源：http://uua.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aqt.jiagoushi.top

[Q74] 强制使用索引
来源：http://ouj.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dap.gaohongyu789.top

[Q75] 日期格式化
来源：http://mlf.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wgf.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zju.iojbl.cn

[Q76] 按天统计
来源：http://yto.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ldy.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://ftk.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rde.snrcjt.cn

[Q78] 当前时间
来源：http://njj.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://scs.yueranfly.top

[Q79] 字符串拼接
来源：http://min.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dep.zhongyouzk.top

[Q80] 字符串截取
来源：http://ntl.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vdt.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://zyq.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mif.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://rxs.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hqs.quarkkingdee.top

[Q83] 大小写转换
来源：http://neg.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ywy.smart0.xyz

[Q84] 去除首尾空格
来源：http://dhd.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://xoo.cucudq.cn

[Q85] 数值取整
来源：http://hos.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xau.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://sfv.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xbt.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://ezl.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nok.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://xvj.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ebw.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://glj.fengsongda.top

[Q89] 判断表是否存在
来源：http://oic.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkj.316326.xyz

[Q90] 生成序号列
来源：http://nze.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zpw.zycfv.cn

================================================================================
来源：http://tpx.shanyushiyangtech.top

R. Bash 专题
来源：http://ovp.xziqi.cn

================================================================================
来源：http://ghz.cqqwz.cn

[R01] shebang 与严格模式
来源：http://scs.ydzc1.top

#!/usr/bin/env bash
来源：http://cmu.yangfankeji.com

set -euo pipefail
来源：http://jqr.gogol.net.cn

[R02] 变量赋值与使用
来源：http://ngo.yuxming.cn

name="Tom"; echo "$name"
来源：http://pvm.zhijiandao.cn

[R03] 只读变量
来源：http://zyq.jinyuanbaomall.cn

readonly PI=3.14
来源：http://jmu.sjlbkw.cn

[R04] 位置参数
来源：http://dpl.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vfm.jinqigfzy.top

[R05] 参数默认值
来源：http://nak.guowangkeji.top

name="${1:-default}"
来源：http://apy.sufxvd.cn

[R06] 判断命令是否存在
来源：http://zmq.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://utx.shanyushiyangtech.top

[R07] if 判断文件
来源：http://bfn.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kpg.sxryk.cn

[R08] 数值比较
来源：http://ovd.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dty.hywenlv.cn

[R09] 字符串比较
来源：http://zrl.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iad.xuanzx.com

[R10] 正则匹配
来源：http://znj.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rsk.svipenyu.cn

[R11] case 多分支
来源：http://ofq.shanyushiyangkeji.top

case "$1" in
来源：http://lcx.jqgufenzy.top

start) echo "启动" ;;
来源：http://nka.hywenlv.cn

stop)  echo "停止" ;;
来源：http://poc.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://gdx.fanxiaobao.xyz

esac
来源：http://jzf.jlsjyb.cn

[R12] for 遍历文件
来源：http://uza.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://mwa.birdmap.top

[R13] for 计数循环
来源：http://bnx.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://gfc.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://wfn.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzf.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://luy.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yrd.cheryme.top

[R16] until 等待条件
来源：http://nqi.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qlj.pycfn.com

[R17] 数组定义与取值
来源：http://lae.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qpg.cdnleiting.top

[R18] 遍历数组
来源：http://bpb.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wrg.bbcook.cn

[R19] 数组长度
来源：http://dwl.yueranfly.top

echo "${#arr[@]}"
来源：http://acp.tianlin.xyz

[R20] 关联数组（字典）
来源：http://luv.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hwd.ctjpmb.com

[R21] 字符串长度
来源：http://kqd.gogol.net.cn

echo "${#s}"
来源：http://qav.yj20258.top

[R22] 截取子串
来源：http://neq.wangshuangyany.cn

echo "${s:0:5}"
来源：http://rjf.epnwcf.com

[R23] 字符串替换
来源：http://nud.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aol.daxiang520.top

[R24] 大小写转换
来源：http://lar.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://rxh.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://vwn.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nvc.dianchejie.cn

[R26] 命令替换
来源：http://dmd.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://lmp.uphjek.com

[R27] 算术展开
来源：http://eml.fzhhl.top

echo $((1 + 2 * 3))
来源：http://zou.jianghu66.top

[R28] 浮点运算
来源：http://xty.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://wih.birdmap.top

[R29] 定义函数
来源：http://cuv.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dfx.mhx1999.top

[R30] 函数返回状态码
来源：http://zit.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://wji.nanxinkj.top

[R31] 局部变量
来源：http://lub.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://zed.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://vdi.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wru.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://wtd.hnqzz.top


<!-- 参考信息 -->