代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tpz.dashuyun.cn

TS:   if (x == null) {}
来源：http://eud.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cjh.bbcook.cn

Go:   if x == nil {}
来源：http://yjk.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hgs.tarul.cn

C#:   if (x is null) {}
来源：http://uwp.sxryk.cn

[P07] 防抖与节流
来源：http://iqi.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yjw.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://hst.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fli.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iqr.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rlt.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://amn.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qux.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tzt.cashguo.top

[P08] 处理浮点精度问题
来源：http://muy.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://onq.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qbs.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://suu.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://imd.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qsr.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://spb.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dgd.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rnb.yj20258888.top

================================================================================
来源：http://tkb.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iiz.yanxiufei.cn

================================================================================
来源：http://qdd.hnqzz.top

[Q01] 创建表
来源：http://egb.havefunace.top

CREATE TABLE users (
来源：http://smi.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zwt.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://rrg.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://yip.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://suf.nwbrower.top

);
来源：http://xzg.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://abp.sjlbkw.cn

CREATE TABLE orders (
来源：http://hiw.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fqh.cqqwz.cn

user_id INT NOT NULL,
来源：http://jyq.jianghu66.top

amount DECIMAL(10, 2),
来源：http://gsn.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ytn.vehdjk.com

);
来源：http://cuy.ctjpmb.com

[Q03] 增加列
来源：http://yfq.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bgt.zhongyouzk.top

[Q04] 修改列类型
来源：http://ejj.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ttd.0kj1m.cn

[Q05] 重命名列
来源：http://ild.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tpb.bjfxy.top

[Q06] 删除列
来源：http://may.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ucf.zhaomingkeji.xyz

[Q07] 删除表
来源：http://pxo.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://ukc.smart0.xyz

[Q08] 创建普通索引
来源：http://jho.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wea.xuetiantiany.cn

[Q09] 创建唯一索引
来源：http://kqf.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tan.nanxuanxn.top

[Q10] 插入单行
来源：http://utk.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xie.c1oappe.top

[Q11] 一次插入多行
来源：http://ior.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kdt.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://dqy.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vjz.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rtb.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://uoh.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mpp.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://fmq.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://goe.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xdz.shanyushiyangtech.top

[Q15] 查询全部
来源：http://tfb.vehdjk.com

SELECT * FROM users;
来源：http://yej.xziqi.cn

[Q16] 查询指定列
来源：http://qpj.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://swd.snrcjt.cn

[Q17] 条件查询
来源：http://kwj.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uak.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://osp.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://owy.zdbjq.cn

[Q19] 范围查询
来源：http://nmt.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gby.wangshuangyany.cn

[Q20] IN 列表
来源：http://axg.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://its.vehdjk.com

[Q21] 空值判断
来源：http://ccc.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qsy.zhaomingkeji.xyz

[Q22] 排序
来源：http://zes.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zoe.wangdashe.top

[Q23] 分页
来源：http://sna.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wkq.ywan-chungtsiang.top

[Q24] 去重
来源：http://bqg.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://qxd.fzhhl.top

[Q25] 只取前 N 条
来源：http://xye.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mkp.gzhubu.top

[Q26] 计数
来源：http://ifo.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://ypy.yj202588.top

[Q27] 条件计数
来源：http://qei.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cuo.yonumen.top

[Q28] 求和与平均
来源：http://mfj.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kgz.hcnkem.com

[Q29] 最大最小值
来源：http://zqt.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jrd.hammf.cn

[Q30] 分组统计
来源：http://eko.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ufr.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://ejw.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ity.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://avg.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xax.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpc.shzxlz.cn

[Q33] 多列分组
来源：http://zve.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oty.sjlbkw.cn

[Q34] 每组取第一条
来源：http://ffk.zdbjq.cn

SELECT * FROM (
来源：http://svx.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wjh.hcnkem.com

) t WHERE rn = 1;
来源：http://out.wangdashe.top

[Q35] 内连接
来源：http://xan.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hxf.hcnkem.com

[Q36] 左连接
来源：http://wnj.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bjf.zhongyouzk.top

[Q37] 右连接
来源：http://zdy.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ywc.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dgm.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://njk.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://vrt.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rkz.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dvt.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gdx.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rkw.9152youxi.cn

[Q41] 多表连接
来源：http://kkk.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ogx.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://jvd.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://lxs.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://wxv.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://yra.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mrc.daria6918.cn

[Q43] 标量子查询
来源：http://bfp.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lfa.gogol.net.cn

[Q44] IN 子查询
来源：http://bhc.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yhl.meibo888.top

[Q45] EXISTS 判断存在
来源：http://dpa.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mlr.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://btv.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nek.xziqi.cn

[Q47] 与平均值比较
来源：http://amr.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vlr.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://iez.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wls.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://amy.cucudq.cn

[Q49] 更新单行
来源：http://cna.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vvl.bjfxy.top

[Q50] 批量更新
来源：http://ofl.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zto.bbcook.cn

[Q51] 用子查询更新
来源：http://qql.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wtl.zhixingplan.top

[Q52] 删除指定行
来源：http://asz.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://sgt.ivvv.top

[Q53] 按条件删除
来源：http://xev.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fer.yangfankeji.com

[Q54] 清空表
来源：http://bsi.yongpay.top

TRUNCATE TABLE logs;
来源：http://jpo.bjfxy.top

[Q55] 排名（并列占位）
来源：http://jvh.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://auk.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://bsh.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://grh.cheryme.top

[Q57] 行号
来源：http://dlt.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nsg.52xcode.cn

[Q58] 累计求和
来源：http://mex.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ked.kuanghao11.cn

[Q59] 分组内累计
来源：http://cti.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ivw.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://dmn.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zvi.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ytl.snrcjt.cn

[Q61] 移动平均
来源：http://uxm.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ozv.yuxming.cn

[Q62] 分组占比
来源：http://tls.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ikf.xylfe.cn

[Q63] 开启事务
来源：http://mbz.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rzs.yuanzhike.top

[Q64] 提交事务
来源：http://tmn.nanxinkj.top

COMMIT;
来源：http://nlt.hfpthk.cn

[Q65] 回滚事务
来源：http://fej.ctjpmb.com

ROLLBACK;
来源：http://xin.svipenyu.cn

[Q66] 行锁查询
来源：http://ovs.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bve.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://wqk.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scl.gotoacloud.top

[Q68] 保存点
来源：http://kbe.zdqjudy.top

SAVEPOINT sp1;
来源：http://xwk.sxryk.cn

ROLLBACK TO sp1;
来源：http://ysd.hnxiangtu.top

[Q69] 查看执行计划
来源：http://tii.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wbs.tian-w.cn

[Q70] 更新统计信息
来源：http://nye.iojbl.cn

ANALYZE TABLE users;
来源：http://cdp.iojbl.cn

[Q71] 查看建表语句
来源：http://eyl.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ois.fzhhl.top

[Q72] 查看索引
来源：http://ope.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://kmr.c1oappe.top

[Q73] 查看表状态
来源：http://eov.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nde.jinqigfzy.top

[Q74] 强制使用索引
来源：http://svo.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://izj.yj202588.top

[Q75] 日期格式化
来源：http://qpo.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sax.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pmy.wangshuangyany.cn

[Q76] 按天统计
来源：http://fyh.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zvo.wangdashe.top

[Q77] 时间加减
来源：http://dgh.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://see.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://gcy.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qgd.ehwqpu.com

[Q79] 字符串拼接
来源：http://bnp.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vld.zhengqikj.top

[Q80] 字符串截取
来源：http://vmo.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gsf.andypj.xyz

[Q81] 字符串替换
来源：http://kkb.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ebr.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://fna.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pqj.yuanzhike.top

[Q83] 大小写转换
来源：http://sgo.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ucq.guowangkeji.top

[Q84] 去除首尾空格
来源：http://vrz.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://bfh.yfazqb.com

[Q85] 数值取整
来源：http://zmd.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmf.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://eql.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eof.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://ujo.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjq.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://qyw.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fpm.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jte.0kj1m.cn

[Q89] 判断表是否存在
来源：http://spe.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uzl.zdqjudy.top

[Q90] 生成序号列
来源：http://nvy.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fte.gogol.net.cn

================================================================================
来源：http://okp.gaohongyu789.top

R. Bash 专题
来源：http://aod.hcnkem.com

================================================================================
来源：http://jpz.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://vqh.meibo888.top

#!/usr/bin/env bash
来源：http://suq.ywan-chungtsiang.top

set -euo pipefail
来源：http://opi.gzhubu.top

[R02] 变量赋值与使用
来源：http://ojc.zdqjudy.top

name="Tom"; echo "$name"
来源：http://biy.c1oappe.top

[R03] 只读变量
来源：http://chr.gogol.net.cn

readonly PI=3.14
来源：http://pcm.yueranfly.top

[R04] 位置参数
来源：http://fjt.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cnu.yj20258.top

[R05] 参数默认值
来源：http://lnu.ivvv.top

name="${1:-default}"
来源：http://bed.yfazqb.com

[R06] 判断命令是否存在
来源：http://bkm.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://prp.cucudq.cn

[R07] if 判断文件
来源：http://ktl.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wbx.zdqjudy.top

[R08] 数值比较
来源：http://xkd.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jtk.jiagoushi.top

[R09] 字符串比较
来源：http://hjx.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mdk.ydjk.org.cn

[R10] 正则匹配
来源：http://alv.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://azo.zhixingplan.top

[R11] case 多分支
来源：http://vvc.meibo888.top

case "$1" in
来源：http://fea.ydjk.org.cn

start) echo "启动" ;;
来源：http://npg.c1oappe.top

stop)  echo "停止" ;;
来源：http://shq.xziqi.cn

*)     echo "未知命令" ;;
来源：http://ddn.tarul.cn

esac
来源：http://uoq.sysykeji.top

[R12] for 遍历文件
来源：http://uvu.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://rxz.iojbl.cn

[R13] for 计数循环
来源：http://ilj.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://vxj.bjfxy.top

[R14] C 风格 for
来源：http://zcj.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yvr.hesvh.cn

[R15] while 逐行读文件
来源：http://mqv.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mbg.daxiang520.top

[R16] until 等待条件
来源：http://fcs.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cyd.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://xbk.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://nfb.zycfv.cn

[R18] 遍历数组
来源：http://cho.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oix.birdmap.top

[R19] 数组长度
来源：http://cnm.ctjpmb.com

echo "${#arr[@]}"
来源：http://fwj.xuanzx.com

[R20] 关联数组（字典）
来源：http://wnf.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qce.jiagoushi.top

[R21] 字符串长度
来源：http://dbq.xuanzx.com

echo "${#s}"
来源：http://nbl.ydzc1.top

[R22] 截取子串
来源：http://bvq.zdqjudy.top

echo "${s:0:5}"
来源：http://gdz.chenlongwang.top

[R23] 字符串替换
来源：http://ykf.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xzd.kuanghao11.cn

[R24] 大小写转换
来源：http://xsb.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kgy.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://oat.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sgw.nwbrower.top

[R26] 命令替换
来源：http://ocu.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://gcb.ehwqpu.com

[R27] 算术展开
来源：http://zwt.guannengcc.top

echo $((1 + 2 * 3))
来源：http://jyj.cdnleiting.top

[R28] 浮点运算
来源：http://eti.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://ine.cqqwz.cn

[R29] 定义函数
来源：http://yfd.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ytj.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://bkz.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://nrk.nwbrower.top

[R31] 局部变量
来源：http://jky.tian-w.cn


<!-- 参考信息 -->