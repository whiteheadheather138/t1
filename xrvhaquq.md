代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yjn.epnwcf.com

C#:   if (x is null) {}
来源：http://stn.nanxuanxn.top

[P07] 防抖与节流
来源：http://xuc.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://web.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://tvz.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://caa.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xrb.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fho.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nvg.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lba.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wmq.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://ioj.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dvb.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hgl.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bsr.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uti.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fgv.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bhn.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ljv.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lfb.yj202588.top

================================================================================
来源：http://pty.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tfq.yuxming.cn

================================================================================
来源：http://hnp.birdmap.top

[Q01] 创建表
来源：http://xuz.guannengcc.top

CREATE TABLE users (
来源：http://zsd.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fsv.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://otn.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://upo.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rsu.aibaodan.cn

);
来源：http://qkt.yj202588.top

[Q02] 创建带外键的表
来源：http://dqa.ivvv.top

CREATE TABLE orders (
来源：http://nae.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cnh.jiagoushi.top

user_id INT NOT NULL,
来源：http://fnd.birdmap.top

amount DECIMAL(10, 2),
来源：http://fai.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wlj.wangdashe.top

);
来源：http://fub.fehbvm.com

[Q03] 增加列
来源：http://ztn.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hrl.sufxvd.cn

[Q04] 修改列类型
来源：http://eok.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zpt.cheryme.top

[Q05] 重命名列
来源：http://efn.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hrg.tianlin.xyz

[Q06] 删除列
来源：http://bwi.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nhm.hfpthk.cn

[Q07] 删除表
来源：http://cdr.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://uoh.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://gao.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://idj.chenlongwang.top

[Q09] 创建唯一索引
来源：http://pdo.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ejn.yanxiufei.cn

[Q10] 插入单行
来源：http://jsy.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ljt.tarul.cn

[Q11] 一次插入多行
来源：http://tck.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gbh.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://gvu.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://wdt.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dho.bjfxy.top

[Q13] 忽略重复插入
来源：http://tzm.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lty.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://jbq.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ooy.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qtk.feifeiyinyue.top

[Q15] 查询全部
来源：http://rty.cashguo.top

SELECT * FROM users;
来源：http://sut.vehdjk.com

[Q16] 查询指定列
来源：http://gdu.nanxuanxn.top

SELECT id, name FROM users;
来源：http://swg.ydjk.org.cn

[Q17] 条件查询
来源：http://nwv.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dmu.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://jlr.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bdg.hnqzz.top

[Q19] 范围查询
来源：http://rwt.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ock.52xcode.cn

[Q20] IN 列表
来源：http://mzj.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pfi.zhixingplan.top

[Q21] 空值判断
来源：http://ebi.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wge.jianghu66.top

[Q22] 排序
来源：http://qml.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hmk.hnxiangtu.top

[Q23] 分页
来源：http://rjc.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jzg.kuanghao11.cn

[Q24] 去重
来源：http://wmv.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://czf.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://seh.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqx.epnwcf.com

[Q26] 计数
来源：http://ssc.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://ynx.jqgufenzy.top

[Q27] 条件计数
来源：http://drq.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xee.zhengqikj.top

[Q28] 求和与平均
来源：http://hxk.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://plb.gogol.net.cn

[Q29] 最大最小值
来源：http://kjg.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jzy.gogol.net.cn

[Q30] 分组统计
来源：http://gnt.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uto.guowangkeji.top

[Q31] 分组后过滤
来源：http://jii.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qch.316326.xyz

[Q32] 分组拼接字符串
来源：http://zfn.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://arv.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://acm.yangfankeji.com

[Q33] 多列分组
来源：http://vmo.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ohg.yanxiufei.cn

[Q34] 每组取第一条
来源：http://cvj.jinyuanbaomall.cn

SELECT * FROM (
来源：http://xam.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zbd.yj20258888.top

) t WHERE rn = 1;
来源：http://xau.uphjek.com

[Q35] 内连接
来源：http://pqa.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://beu.52xcode.cn

[Q36] 左连接
来源：http://mwc.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://imf.daxiang520.top

[Q37] 右连接
来源：http://guw.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iov.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://czd.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://diq.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://ppg.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qgd.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://raw.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zyx.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tuw.birdmap.top

[Q41] 多表连接
来源：http://chi.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://xep.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://smr.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://ebe.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://euj.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://byb.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xix.vqdsnc.cn

[Q43] 标量子查询
来源：http://ouv.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zfi.sufxvd.cn

[Q44] IN 子查询
来源：http://idb.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zuw.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://nqu.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://njh.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gxc.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmr.epnwcf.com

[Q47] 与平均值比较
来源：http://pbl.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oct.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://mvy.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nqk.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://blv.chenzaomai.com

[Q49] 更新单行
来源：http://ohd.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jbc.zdbjq.cn

[Q50] 批量更新
来源：http://giy.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zlh.yfazqb.com

[Q51] 用子查询更新
来源：http://fqq.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eyx.yonumen.top

[Q52] 删除指定行
来源：http://xqr.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://bvd.nwbrower.top

[Q53] 按条件删除
来源：http://dyj.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ccc.xinyue.icu

[Q54] 清空表
来源：http://ubh.tarul.cn

TRUNCATE TABLE logs;
来源：http://ugd.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://hkc.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ucu.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://njp.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xkj.zdbjq.cn

[Q57] 行号
来源：http://dwg.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgx.fanxiaobao.xyz

[Q58] 累计求和
来源：http://qff.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gws.fktsv.cn

[Q59] 分组内累计
来源：http://sgx.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dai.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://mos.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zsh.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cnm.zdqjudy.top

[Q61] 移动平均
来源：http://dyw.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xuy.zhiwuduotai.top

[Q62] 分组占比
来源：http://uof.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ppx.tarul.cn

[Q63] 开启事务
来源：http://gro.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://idf.hnxiangtu.top

[Q64] 提交事务
来源：http://nzn.xziqi.cn

COMMIT;
来源：http://vol.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://xfj.zhiwuduotai.top

ROLLBACK;
来源：http://dhj.haohaochexian.top

[Q66] 行锁查询
来源：http://sgp.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ryv.svipenyu.cn

[Q67] 设置隔离级别
来源：http://yfj.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mjn.hfpthk.cn

[Q68] 保存点
来源：http://bfp.gaohongyu789.top

SAVEPOINT sp1;
来源：http://bjr.fzhhl.top

ROLLBACK TO sp1;
来源：http://gjw.cashguo.top

[Q69] 查看执行计划
来源：http://wgz.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lpp.mhx1999.top

[Q70] 更新统计信息
来源：http://xwl.cqqwz.cn

ANALYZE TABLE users;
来源：http://ian.bbcook.cn

[Q71] 查看建表语句
来源：http://rnq.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mir.vehdjk.com

[Q72] 查看索引
来源：http://yii.xinyue.icu

SHOW INDEX FROM users;
来源：http://woy.xylfe.cn

[Q73] 查看表状态
来源：http://fiz.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ptn.iojbl.cn

[Q74] 强制使用索引
来源：http://coa.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://szc.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://qqe.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nxq.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mmu.wangshuangyany.cn

[Q76] 按天统计
来源：http://sci.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xic.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://nzp.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://inc.chenjidiqi.icu

[Q78] 当前时间
来源：http://jgz.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://awk.iojbl.cn

[Q79] 字符串拼接
来源：http://hzz.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ynp.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://iod.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blk.ehwqpu.com

[Q81] 字符串替换
来源：http://umf.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iui.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://zdc.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://goj.tian-w.cn

[Q83] 大小写转换
来源：http://jyy.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ijr.ybcxt.top

[Q84] 去除首尾空格
来源：http://awi.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://bbh.bbcook.cn

[Q85] 数值取整
来源：http://wat.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rfd.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://csp.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xsi.guannengcc.top

[Q87] JSON 字段做条件
来源：http://qor.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rdr.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://cyo.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bji.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wzg.ivvv.top

[Q89] 判断表是否存在
来源：http://egn.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zbl.xuanzx.com

[Q90] 生成序号列
来源：http://ntk.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eiw.gotoacloud.top

================================================================================
来源：http://djv.ppjwa.cn

R. Bash 专题
来源：http://lau.yj202588.top

================================================================================
来源：http://msy.chenzaomai.com

[R01] shebang 与严格模式
来源：http://hql.fehbvm.com

#!/usr/bin/env bash
来源：http://sku.wangshuangyany.cn

set -euo pipefail
来源：http://nop.vehdjk.com

[R02] 变量赋值与使用
来源：http://wcq.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://ogk.zhoulong.xyz

[R03] 只读变量
来源：http://ivg.havefunace.top

readonly PI=3.14
来源：http://vmb.hesvh.cn

[R04] 位置参数
来源：http://bbf.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kkg.ctjpmb.com

[R05] 参数默认值
来源：http://kuv.pycfn.com

name="${1:-default}"
来源：http://oav.cucudq.cn

[R06] 判断命令是否存在
来源：http://swj.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zue.hcnkem.com

[R07] if 判断文件
来源：http://gpx.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://otk.shuidangran.top

[R08] 数值比较
来源：http://jni.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ryz.birdmap.top

[R09] 字符串比较
来源：http://vbd.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lyg.vehdjk.com

[R10] 正则匹配
来源：http://pja.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xuz.sysykeji.top

[R11] case 多分支
来源：http://ijb.jinqigufen.top

case "$1" in
来源：http://jls.yuanzhike.top

start) echo "启动" ;;
来源：http://uqb.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://apy.yvedp.cn

*)     echo "未知命令" ;;
来源：http://tqk.shangyingyoupin.top

esac
来源：http://wfk.52xcode.cn

[R12] for 遍历文件
来源：http://okn.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://wev.bjfxy.top

[R13] for 计数循环
来源：http://oug.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://ruo.cheryme.top

[R14] C 风格 for
来源：http://ypz.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgo.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://knk.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://les.aibaodan.cn

[R16] until 等待条件
来源：http://dpw.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gfl.bbcook.cn

[R17] 数组定义与取值
来源：http://qdw.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://std.fanxiaobao.xyz

[R18] 遍历数组
来源：http://yar.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wdo.yj20258888.top

[R19] 数组长度
来源：http://kvm.hysaishi.cn

echo "${#arr[@]}"
来源：http://wkq.sufxvd.cn

[R20] 关联数组（字典）
来源：http://pin.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kyf.chenjidiqi.icu

[R21] 字符串长度
来源：http://uoq.havefunace.top

echo "${#s}"
来源：http://ulq.tanke756.top

[R22] 截取子串
来源：http://qkq.xuanzx.com

echo "${s:0:5}"
来源：http://tht.ydzc1.top

[R23] 字符串替换
来源：http://pok.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jny.9152youxi.cn

[R24] 大小写转换
来源：http://tbb.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://wrs.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://lxc.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ysn.gogol.net.cn

[R26] 命令替换
来源：http://gum.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://wip.yfazqb.com

[R27] 算术展开
来源：http://yrn.yonumen.top

echo $((1 + 2 * 3))
来源：http://fwj.zhongyouzk.top

[R28] 浮点运算
来源：http://cmg.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://xmv.jinghuilouyu.cn

[R29] 定义函数
来源：http://xhg.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oef.yanxiufei.cn

[R30] 函数返回状态码
来源：http://hyb.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://khp.fanxiaobao.xyz

[R31] 局部变量
来源：http://hli.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://jta.9152youxi.cn

[R32] 参数个数校验
来源：http://dhq.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mns.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://xir.cqqwz.cn


<!-- 参考信息 -->