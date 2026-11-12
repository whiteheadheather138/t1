代发 wailian999

PHP:  // 手写时间戳比较
来源：http://eny.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvd.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://adq.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hwt.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xup.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oss.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://itk.redwolf501.top

[P08] 处理浮点精度问题
来源：http://tgo.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rsh.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://knf.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gzn.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vlc.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wkm.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://urk.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tlz.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pjg.ybcxt.top

================================================================================
来源：http://hpm.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cvj.jqgfzy.top

================================================================================
来源：http://dvd.yangfankeji.com

[Q01] 创建表
来源：http://zxq.birdmap.top

CREATE TABLE users (
来源：http://kyy.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hfr.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://avs.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://tfq.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kah.shanyushiyangkeji.top

);
来源：http://hoa.nwbrower.top

[Q02] 创建带外键的表
来源：http://rlb.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://jkp.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjo.tianlin.xyz

user_id INT NOT NULL,
来源：http://wry.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://iwe.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qpg.jinghuilouyu.cn

);
来源：http://dii.shanyushiyangkeji.top

[Q03] 增加列
来源：http://ssz.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rey.ydzc1.top

[Q04] 修改列类型
来源：http://wdu.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yjr.havefunace.top

[Q05] 重命名列
来源：http://vth.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ujp.hfpthk.cn

[Q06] 删除列
来源：http://xne.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://ycy.yongpay.top

[Q07] 删除表
来源：http://rzv.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://dsa.cdnleiting.top

[Q08] 创建普通索引
来源：http://yry.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bzo.yonumen.top

[Q09] 创建唯一索引
来源：http://ktd.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://krg.smart0.xyz

[Q10] 插入单行
来源：http://pjs.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ywz.52xcode.cn

[Q11] 一次插入多行
来源：http://xig.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vyk.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://vzc.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xpx.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uqh.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://vnf.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qbf.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://vfq.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zxt.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yxd.yuxming.cn

[Q15] 查询全部
来源：http://dlo.zdqjudy.top

SELECT * FROM users;
来源：http://lxb.cheryme.top

[Q16] 查询指定列
来源：http://zcv.meibo888.top

SELECT id, name FROM users;
来源：http://rof.snrcjt.cn

[Q17] 条件查询
来源：http://ubs.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bmq.hnxiangtu.top

[Q18] 模糊匹配
来源：http://xoj.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bxt.jlsjyb.cn

[Q19] 范围查询
来源：http://kki.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xdg.52xcode.cn

[Q20] IN 列表
来源：http://ewi.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vpg.zhiwuduotai.top

[Q21] 空值判断
来源：http://mhe.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ixn.gotoacloud.top

[Q22] 排序
来源：http://yff.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://izn.yj20258888.top

[Q23] 分页
来源：http://faa.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lit.svipenyu.cn

[Q24] 去重
来源：http://ewg.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://wqx.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://onp.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lkk.tarul.cn

[Q26] 计数
来源：http://ags.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://umd.redwolf501.top

[Q27] 条件计数
来源：http://whh.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xar.hysaishi.cn

[Q28] 求和与平均
来源：http://faq.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://apf.ybcxt.top

[Q29] 最大最小值
来源：http://liu.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gwa.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://pfw.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mlj.cqqwz.cn

[Q31] 分组后过滤
来源：http://bvy.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vzn.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://tnx.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vzo.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pfr.hfpthk.cn

[Q33] 多列分组
来源：http://ygc.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vqg.shuidangran.top

[Q34] 每组取第一条
来源：http://osm.zhoulong.xyz

SELECT * FROM (
来源：http://eax.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zzr.fzhhl.top

) t WHERE rn = 1;
来源：http://vcc.hysaishi.cn

[Q35] 内连接
来源：http://dmd.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jrz.svipenyu.cn

[Q36] 左连接
来源：http://tpb.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vrr.zhoulong.xyz

[Q37] 右连接
来源：http://dwa.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sbx.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://xcz.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xxs.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://gpk.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xut.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qfg.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://alv.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zcb.jinqigufen.top

[Q41] 多表连接
来源：http://nad.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iro.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://dee.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://vwm.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://yrs.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://zhl.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gjw.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://kdv.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wts.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://wju.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mrb.yongpay.top

[Q45] EXISTS 判断存在
来源：http://gvj.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://etf.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://uvv.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvh.tian-w.cn

[Q47] 与平均值比较
来源：http://ruo.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pxf.yongpay.top

[Q48] CTE 公用表表达式
来源：http://rle.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xfa.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://zjt.shanyushiyangtech.top

[Q49] 更新单行
来源：http://poj.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oos.chenlongwang.top

[Q50] 批量更新
来源：http://bgx.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tqo.sufxvd.cn

[Q51] 用子查询更新
来源：http://prr.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://elh.meibo888.top

[Q52] 删除指定行
来源：http://qbd.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://oty.yj202588.top

[Q53] 按条件删除
来源：http://brq.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pzm.tanke756.top

[Q54] 清空表
来源：http://ktd.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://mwf.xuanzx.com

[Q55] 排名（并列占位）
来源：http://emk.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mfg.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://ccy.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lig.meibo888.top

[Q57] 行号
来源：http://ntd.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dlt.yonumen.top

[Q58] 累计求和
来源：http://ptx.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bkz.hfpthk.cn

[Q59] 分组内累计
来源：http://voy.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cxm.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://cqx.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://deb.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bhc.pycfn.com

[Q61] 移动平均
来源：http://qmy.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rqs.daria6918.cn

[Q62] 分组占比
来源：http://art.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xik.sysykeji.top

[Q63] 开启事务
来源：http://otm.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://amj.yangfankeji.com

[Q64] 提交事务
来源：http://caa.xylfe.cn

COMMIT;
来源：http://rcw.svipenyu.cn

[Q65] 回滚事务
来源：http://bhz.hnxiangtu.top

ROLLBACK;
来源：http://jhh.yvedp.cn

[Q66] 行锁查询
来源：http://sug.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ral.yj20258.top

[Q67] 设置隔离级别
来源：http://hqd.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nms.gaohongyu789.top

[Q68] 保存点
来源：http://rkq.gogol.net.cn

SAVEPOINT sp1;
来源：http://tpv.zdbjq.cn

ROLLBACK TO sp1;
来源：http://wex.iojbl.cn

[Q69] 查看执行计划
来源：http://qou.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://epo.jlsjyb.cn

[Q70] 更新统计信息
来源：http://fyn.zhoulong.xyz

ANALYZE TABLE users;
来源：http://kcr.yj20258.top

[Q71] 查看建表语句
来源：http://izq.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rbs.hysaishi.cn

[Q72] 查看索引
来源：http://pdr.ehwqpu.com

SHOW INDEX FROM users;
来源：http://cdw.jyoumei.cn

[Q73] 查看表状态
来源：http://aec.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://dav.jlsjyb.cn

[Q74] 强制使用索引
来源：http://zca.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sha.jianghu66.top

[Q75] 日期格式化
来源：http://dgn.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ryg.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://weg.wangdashe.top

[Q76] 按天统计
来源：http://aol.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oqi.aibaodan.cn

[Q77] 时间加减
来源：http://ixd.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pix.jiagoushi.top

[Q78] 当前时间
来源：http://dgn.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mwl.jianghu66.top

[Q79] 字符串拼接
来源：http://hga.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://syi.jinqigufen.top

[Q80] 字符串截取
来源：http://wqg.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ldw.yfazqb.com

[Q81] 字符串替换
来源：http://vxz.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uud.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://vro.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ffs.yueranfly.top

[Q83] 大小写转换
来源：http://zun.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dur.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://rdi.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://mss.shuidangran.top

[Q85] 数值取整
来源：http://fvj.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iph.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://skt.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nfo.ivvv.top

[Q87] JSON 字段做条件
来源：http://kdk.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tph.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://zbe.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cxx.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sww.52xcode.cn

[Q89] 判断表是否存在
来源：http://ivv.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pee.yueranfly.top

[Q90] 生成序号列
来源：http://rab.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hgr.yueranfly.top

================================================================================
来源：http://dre.tarul.cn

R. Bash 专题
来源：http://xvn.wangshuangyany.cn

================================================================================
来源：http://foy.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://xrq.smart0.xyz

#!/usr/bin/env bash
来源：http://bcy.redwolf501.top

set -euo pipefail
来源：http://dco.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://lcj.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://cgm.yongpay.top

[R03] 只读变量
来源：http://fmx.ctjpmb.com

readonly PI=3.14
来源：http://nus.snrcjt.cn

[R04] 位置参数
来源：http://pnf.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rfh.aibaodan.cn

[R05] 参数默认值
来源：http://uss.cheryme.top

name="${1:-default}"
来源：http://kwd.nwbrower.top

[R06] 判断命令是否存在
来源：http://njl.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ski.sjlbkw.cn

[R07] if 判断文件
来源：http://nte.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ock.pycfn.com

[R08] 数值比较
来源：http://kbi.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hsi.tian-w.cn

[R09] 字符串比较
来源：http://dct.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sef.quarkkingdee.top

[R10] 正则匹配
来源：http://ndv.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rlp.meibo888.top

[R11] case 多分支
来源：http://jlj.chenlongwang.top

case "$1" in
来源：http://pdi.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://iyn.bbcook.cn

stop)  echo "停止" ;;
来源：http://mqo.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://kyx.xylfe.cn

esac
来源：http://ubc.nanxinkj.top

[R12] for 遍历文件
来源：http://usz.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://ywc.zhoulong.xyz

[R13] for 计数循环
来源：http://vxn.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://kmf.hywenlv.cn

[R14] C 风格 for
来源：http://gxc.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jkg.hcnkem.com

[R15] while 逐行读文件
来源：http://wxd.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rvd.daria6918.cn

[R16] until 等待条件
来源：http://ytq.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nwd.yfazqb.com

[R17] 数组定义与取值
来源：http://hev.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://lgo.hongshengwenyu.top

[R18] 遍历数组
来源：http://clq.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pff.haohaochexian.top

[R19] 数组长度
来源：http://okd.zhengqikj.top

echo "${#arr[@]}"
来源：http://btg.9152youxi.cn

[R20] 关联数组（字典）
来源：http://yfi.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rnl.bbcook.cn

[R21] 字符串长度
来源：http://yqp.gzhubu.top

echo "${#s}"
来源：http://btx.xziqi.cn

[R22] 截取子串
来源：http://nsg.sufxvd.cn

echo "${s:0:5}"
来源：http://wiu.sjlbkw.cn

[R23] 字符串替换
来源：http://ypk.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yji.hcnkem.com

[R24] 大小写转换
来源：http://mvo.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://utu.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://bug.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wnf.tianlin.xyz

[R26] 命令替换
来源：http://vzx.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://arn.xylfe.cn

[R27] 算术展开
来源：http://lzw.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://bma.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://wok.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://sqg.tianlin.xyz

[R29] 定义函数
来源：http://mxp.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lne.52xcode.cn

[R30] 函数返回状态码
来源：http://plv.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://vlp.jianghu66.top

[R31] 局部变量
来源：http://yay.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://bpl.xinyue.icu

[R32] 参数个数校验
来源：http://tsh.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nae.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://vnt.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mzc.pycfn.com

[R34] 退出时清理
来源：http://teg.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ntx.andypj.xyz

[R35] 后台执行并等待
来源：http://nyt.dashuyun.cn


<!-- 参考信息 -->