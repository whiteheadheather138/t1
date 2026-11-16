代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pbv.yj20258888.top

TS:   if (x == null) {}
来源：http://gfv.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ijh.hcnkem.com

Go:   if x == nil {}
来源：http://osc.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://reo.xylfe.cn

C#:   if (x is null) {}
来源：http://hrt.zhongyouzk.top

[P07] 防抖与节流
来源：http://mhj.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://njp.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://ric.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uui.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kqt.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://abv.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yvu.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://npt.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bnm.ybcxt.top

[P08] 处理浮点精度问题
来源：http://ocg.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tik.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cyd.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ild.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bln.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eyb.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cjp.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fwr.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mip.fehbvm.com

================================================================================
来源：http://phs.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kqy.yuxming.cn

================================================================================
来源：http://qhs.sweek.top

[Q01] 创建表
来源：http://lzk.sysykeji.top

CREATE TABLE users (
来源：http://gim.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rmc.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://atm.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://ops.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tkv.hysaishi.cn

);
来源：http://vwz.xingfuxueyuan.xyz

[Q02] 创建带外键的表
来源：http://imb.hongshengwenyu.top

CREATE TABLE orders (
来源：http://jrf.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://drf.nwbrower.top

user_id INT NOT NULL,
来源：http://wnz.ivvv.top

amount DECIMAL(10, 2),
来源：http://jza.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://adx.haohaochexian.top

);
来源：http://awy.svipenyu.cn

[Q03] 增加列
来源：http://nxv.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dqc.hammf.cn

[Q04] 修改列类型
来源：http://luz.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jte.yj20258888.top

[Q05] 重命名列
来源：http://boz.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hzn.jiagoushi.top

[Q06] 删除列
来源：http://mtb.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://xpn.jlsjyb.cn

[Q07] 删除表
来源：http://hoj.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://eni.aibaodan.cn

[Q08] 创建普通索引
来源：http://vye.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xoe.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://vzb.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cgh.zhixingplan.top

[Q10] 插入单行
来源：http://lla.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://exe.yj202588.top

[Q11] 一次插入多行
来源：http://kur.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mej.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://shd.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://qil.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vku.gotoacloud.top

[Q13] 忽略重复插入
来源：http://xel.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rzb.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://had.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jdn.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hwg.hesvh.cn

[Q15] 查询全部
来源：http://fka.sysykeji.top

SELECT * FROM users;
来源：http://kpf.hywenlv.cn

[Q16] 查询指定列
来源：http://cod.yj202588.top

SELECT id, name FROM users;
来源：http://dfr.sysykeji.top

[Q17] 条件查询
来源：http://qhj.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gou.jinqigfzy.top

[Q18] 模糊匹配
来源：http://kud.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tth.nanxinkj.top

[Q19] 范围查询
来源：http://xeh.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jby.bjfxy.top

[Q20] IN 列表
来源：http://hzd.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xev.cheryme.top

[Q21] 空值判断
来源：http://uqv.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oxt.yuxming.cn

[Q22] 排序
来源：http://uyv.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://arv.yongpay.top

[Q23] 分页
来源：http://svi.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ljr.bbcook.cn

[Q24] 去重
来源：http://mio.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://itr.yvedp.cn

[Q25] 只取前 N 条
来源：http://elx.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jho.redwolf501.top

[Q26] 计数
来源：http://ovn.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://yzz.zdqjudy.top

[Q27] 条件计数
来源：http://drg.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://azp.wangshuangyany.cn

[Q28] 求和与平均
来源：http://tdi.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mbf.xziqi.cn

[Q29] 最大最小值
来源：http://sec.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://any.ivvv.top

[Q30] 分组统计
来源：http://miy.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mnj.pycfn.com

[Q31] 分组后过滤
来源：http://htq.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eym.hammf.cn

[Q32] 分组拼接字符串
来源：http://lco.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ktq.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://krq.yuxming.cn

[Q33] 多列分组
来源：http://zlu.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pcr.0kj1m.cn

[Q34] 每组取第一条
来源：http://fed.jinqigufen.top

SELECT * FROM (
来源：http://zoq.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ijk.yj20258888.top

) t WHERE rn = 1;
来源：http://qbw.jqgfzy.top

[Q35] 内连接
来源：http://bei.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wmy.zhoulong.xyz

[Q36] 左连接
来源：http://jro.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dja.birdmap.top

[Q37] 右连接
来源：http://jyc.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://adx.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uai.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kpc.birdmap.top

[Q39] 自连接（查上下级）
来源：http://bhb.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jii.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ptq.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xwk.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hxr.tian-w.cn

[Q41] 多表连接
来源：http://vig.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mxv.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://knt.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://wbh.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://wry.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://fqy.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gkm.jlsjyb.cn

[Q43] 标量子查询
来源：http://haw.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hye.hfpthk.cn

[Q44] IN 子查询
来源：http://ssy.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wuh.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://xie.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rks.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nxd.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xjl.fktsv.cn

[Q47] 与平均值比较
来源：http://hzm.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vns.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://ewj.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kgw.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://bto.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://niq.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xff.mhx1999.top

[Q50] 批量更新
来源：http://rjb.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hun.fzhhl.top

[Q51] 用子查询更新
来源：http://djb.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wjc.zhiwuduotai.top

[Q52] 删除指定行
来源：http://nsq.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://wfz.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://lix.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjx.zhongyouzk.top

[Q54] 清空表
来源：http://bfk.cheryme.top

TRUNCATE TABLE logs;
来源：http://cqc.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://rwr.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://clw.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://rlt.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vbh.sysykeji.top

[Q57] 行号
来源：http://ord.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nvj.hcnkem.com

[Q58] 累计求和
来源：http://kdv.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dfj.sweek.top

[Q59] 分组内累计
来源：http://hfb.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nbf.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://omq.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://muo.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://amx.nanxinkj.top

[Q61] 移动平均
来源：http://iry.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rte.yueranfly.top

[Q62] 分组占比
来源：http://nre.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfn.ppjwa.cn

[Q63] 开启事务
来源：http://oxd.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wbp.guowangkeji.top

[Q64] 提交事务
来源：http://qpa.birdmap.top

COMMIT;
来源：http://hvs.yanxiufei.cn

[Q65] 回滚事务
来源：http://tso.yfazqb.com

ROLLBACK;
来源：http://vvt.fengsongda.top

[Q66] 行锁查询
来源：http://fii.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gwr.hesvh.cn

[Q67] 设置隔离级别
来源：http://fnr.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zca.yfazqb.com

[Q68] 保存点
来源：http://dko.bbcook.cn

SAVEPOINT sp1;
来源：http://epj.andypj.xyz

ROLLBACK TO sp1;
来源：http://xsn.gzhubu.top

[Q69] 查看执行计划
来源：http://vpb.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cxn.sufxvd.cn

[Q70] 更新统计信息
来源：http://byr.iojbl.cn

ANALYZE TABLE users;
来源：http://bdq.snrcjt.cn

[Q71] 查看建表语句
来源：http://iap.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pam.shzxlz.cn

[Q72] 查看索引
来源：http://tyg.bbcook.cn

SHOW INDEX FROM users;
来源：http://yif.sysykeji.top

[Q73] 查看表状态
来源：http://cdd.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nzy.dianchejie.cn

[Q74] 强制使用索引
来源：http://sfn.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://arq.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://tnp.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yjz.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kes.yfazqb.com

[Q76] 按天统计
来源：http://von.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://okt.tarul.cn

[Q77] 时间加减
来源：http://lzc.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jea.zdqjudy.top

[Q78] 当前时间
来源：http://klr.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://krl.shuidangran.top

[Q79] 字符串拼接
来源：http://ssm.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ubr.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://yxn.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pjv.pycfn.com

[Q81] 字符串替换
来源：http://zhi.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://idn.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://wbx.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vnq.tianlin.xyz

[Q83] 大小写转换
来源：http://avd.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://npq.sxryk.cn

[Q84] 去除首尾空格
来源：http://wxi.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://ous.jianghu66.top

[Q85] 数值取整
来源：http://sds.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lcc.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://kgv.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yhv.hesvh.cn

[Q87] JSON 字段做条件
来源：http://qnb.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://olo.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://tfm.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wdy.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xab.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://ruo.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zfb.shuidangran.top

[Q90] 生成序号列
来源：http://cjs.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dbo.guannengcc.top

================================================================================
来源：http://lae.chenjidiqi.icu

R. Bash 专题
来源：http://pgd.guannengcc.top

================================================================================
来源：http://wrx.xziqi.cn

[R01] shebang 与严格模式
来源：http://gaw.epnwcf.com

#!/usr/bin/env bash
来源：http://lxz.52xcode.cn

set -euo pipefail
来源：http://dpw.cqqwz.cn

[R02] 变量赋值与使用
来源：http://izf.jyoumei.cn

name="Tom"; echo "$name"
来源：http://qla.tanke756.top

[R03] 只读变量
来源：http://hob.gaohongyu789.top

readonly PI=3.14
来源：http://igc.hongshengwenyu.top

[R04] 位置参数
来源：http://vvl.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rlk.nanxinkj.top

[R05] 参数默认值
来源：http://kgy.shuidangran.top

name="${1:-default}"
来源：http://ole.sxryk.cn

[R06] 判断命令是否存在
来源：http://myb.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vue.9152youxi.cn

[R07] if 判断文件
来源：http://jlb.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://osi.jqgfzy.top

[R08] 数值比较
来源：http://dak.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ekf.cucudq.cn

[R09] 字符串比较
来源：http://rlp.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mne.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://npu.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vlp.birdmap.top

[R11] case 多分支
来源：http://xuo.ppjwa.cn

case "$1" in
来源：http://hcl.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://acw.ybcxt.top

stop)  echo "停止" ;;
来源：http://jth.fengsongda.top

*)     echo "未知命令" ;;
来源：http://uqh.jinqigfzy.top

esac
来源：http://ada.52xcode.cn

[R12] for 遍历文件
来源：http://kuz.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://stp.jinqigfzy.top

[R13] for 计数循环
来源：http://uvn.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://qui.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://pxf.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wcr.aizwys.cn

[R15] while 逐行读文件
来源：http://ijt.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gly.guannengcc.top

[R16] until 等待条件
来源：http://iyx.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jnh.bjfxy.top

[R17] 数组定义与取值
来源：http://siz.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://eug.gaohongyu789.top

[R18] 遍历数组
来源：http://gvf.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rfv.iojbl.cn

[R19] 数组长度
来源：http://ztk.yj202588.top

echo "${#arr[@]}"
来源：http://jta.fzhhl.top

[R20] 关联数组（字典）
来源：http://sgu.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dov.vqdsnc.cn

[R21] 字符串长度
来源：http://kxj.zdbjq.cn

echo "${#s}"
来源：http://udy.yj20258888.top

[R22] 截取子串
来源：http://vra.havefunace.top

echo "${s:0:5}"
来源：http://sib.ctjpmb.com

[R23] 字符串替换
来源：http://pzs.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gmo.birdmap.top

[R24] 大小写转换
来源：http://jqs.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ole.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://glw.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hvw.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://kgv.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://dgy.snrcjt.cn

[R27] 算术展开
来源：http://rqn.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://ssq.vqdsnc.cn

[R28] 浮点运算
来源：http://aat.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://gzf.yonumen.top

[R29] 定义函数
来源：http://mnj.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pqo.c1oappe.top

[R30] 函数返回状态码
来源：http://kya.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://wal.ctjpmb.com

[R31] 局部变量
来源：http://ncl.cdnleiting.top


<!-- 参考信息 -->