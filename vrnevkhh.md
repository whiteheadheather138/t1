代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bat.zdqjudy.top

TS:   if (x == null) {}
来源：http://azh.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jhk.xziqi.cn

Go:   if x == nil {}
来源：http://uvx.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wxv.ybcxt.top

C#:   if (x is null) {}
来源：http://onh.ybcxt.top

[P07] 防抖与节流
来源：http://qjj.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mys.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://gnu.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ocs.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxf.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rjy.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zur.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dpf.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ntb.sweek.top

[P08] 处理浮点精度问题
来源：http://ckp.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ftl.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vtr.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xhr.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cvt.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nhp.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gjx.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ndk.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tlp.chenzaomai.com

================================================================================
来源：http://wnj.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yxb.shanyushiyangtech.top

================================================================================
来源：http://qhq.vqdsnc.cn

[Q01] 创建表
来源：http://yuc.0kj1m.cn

CREATE TABLE users (
来源：http://btf.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bet.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://hat.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://igm.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ifk.fengsongda.top

);
来源：http://rgt.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://wxl.zhongyouzk.top

CREATE TABLE orders (
来源：http://uuf.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://amw.cucudq.cn

user_id INT NOT NULL,
来源：http://btv.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://mca.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tue.zhaomingkeji.xyz

);
来源：http://hfb.fengsongda.top

[Q03] 增加列
来源：http://idr.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ytl.gogol.net.cn

[Q04] 修改列类型
来源：http://xwz.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fna.hnxiangtu.top

[Q05] 重命名列
来源：http://dtj.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wsm.vqdsnc.cn

[Q06] 删除列
来源：http://jxa.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://nrh.jinghuilouyu.cn

[Q07] 删除表
来源：http://sec.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://uzm.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://ybw.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://geg.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://nin.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kfl.feifeiyinyue.top

[Q10] 插入单行
来源：http://urr.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xbm.aizwys.cn

[Q11] 一次插入多行
来源：http://tas.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bwu.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://njr.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xzt.hammf.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://twu.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://tvh.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wej.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://uuy.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xto.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mzn.zhixingplan.top

[Q15] 查询全部
来源：http://clz.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://bth.jinqigufen.top

[Q16] 查询指定列
来源：http://bui.yueranfly.top

SELECT id, name FROM users;
来源：http://geg.pengpengdd.cyou

[Q17] 条件查询
来源：http://imc.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xso.ivvv.top

[Q18] 模糊匹配
来源：http://lcf.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mgo.hammf.cn

[Q19] 范围查询
来源：http://rem.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://enb.redwolf501.top

[Q20] IN 列表
来源：http://qrs.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hwr.zdqjudy.top

[Q21] 空值判断
来源：http://lif.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ish.vqdsnc.cn

[Q22] 排序
来源：http://mjm.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kgo.jianghu66.top

[Q23] 分页
来源：http://iuf.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tch.ybcxt.top

[Q24] 去重
来源：http://bpr.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://plo.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://foi.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xzl.jlsjyb.cn

[Q26] 计数
来源：http://pur.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://vhs.shanyushiyangtech.top

[Q27] 条件计数
来源：http://nze.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mvn.zhongyouzk.top

[Q28] 求和与平均
来源：http://krn.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mwh.andypj.xyz

[Q29] 最大最小值
来源：http://wpx.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iqo.meibo888.top

[Q30] 分组统计
来源：http://drg.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcx.jinqigufen.top

[Q31] 分组后过滤
来源：http://ycb.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cwq.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://ncw.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mub.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ngv.svipenyu.cn

[Q33] 多列分组
来源：http://rru.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://isq.bbcook.cn

[Q34] 每组取第一条
来源：http://viy.tarul.cn

SELECT * FROM (
来源：http://edv.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ida.fktsv.cn

) t WHERE rn = 1;
来源：http://wqg.nanxinkj.top

[Q35] 内连接
来源：http://vkj.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ayb.nanxinkj.top

[Q36] 左连接
来源：http://doj.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yav.jinqigfzy.top

[Q37] 右连接
来源：http://nvr.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qkl.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://dzd.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tav.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://vrk.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mbo.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fal.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ydu.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fgp.sxryk.cn

[Q41] 多表连接
来源：http://yyg.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fkg.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://lsf.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://icu.uphjek.com

[Q42] 连接条件附加过滤
来源：http://awl.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://dld.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mam.hesvh.cn

[Q43] 标量子查询
来源：http://bcl.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tss.dashuyun.cn

[Q44] IN 子查询
来源：http://dug.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zho.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://nuw.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lfp.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://txb.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ify.ppjwa.cn

[Q47] 与平均值比较
来源：http://gjc.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dsp.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://vdq.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ucd.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://pdq.9152youxi.cn

[Q49] 更新单行
来源：http://xwv.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pbl.haohaochexian.top

[Q50] 批量更新
来源：http://czz.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lrl.jiagoushi.top

[Q51] 用子查询更新
来源：http://qnx.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xxf.snrcjt.cn

[Q52] 删除指定行
来源：http://nmt.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://xyl.feifeiyinyue.top

[Q53] 按条件删除
来源：http://rga.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kwt.cheryme.top

[Q54] 清空表
来源：http://ivl.sysykeji.top

TRUNCATE TABLE logs;
来源：http://xtb.tarul.cn

[Q55] 排名（并列占位）
来源：http://mge.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fys.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://blb.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://srs.jyoumei.cn

[Q57] 行号
来源：http://ysj.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fcb.hongshengwenyu.top

[Q58] 累计求和
来源：http://izt.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hji.aibaodan.cn

[Q59] 分组内累计
来源：http://itf.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sqj.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://rns.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://otz.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://exy.hammf.cn

[Q61] 移动平均
来源：http://dty.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://goo.fengsongda.top

[Q62] 分组占比
来源：http://esl.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://egf.gaohongyu789.top

[Q63] 开启事务
来源：http://vnm.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vxg.hesvh.cn

[Q64] 提交事务
来源：http://znh.redwolf501.top

COMMIT;
来源：http://kks.jianghu66.top

[Q65] 回滚事务
来源：http://crq.jinqigufen.top

ROLLBACK;
来源：http://ozo.tian-w.cn

[Q66] 行锁查询
来源：http://ott.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hmx.aizwys.cn

[Q67] 设置隔离级别
来源：http://ebi.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyh.nanxinkj.top

[Q68] 保存点
来源：http://raj.jqgufenzy.top

SAVEPOINT sp1;
来源：http://goe.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://zku.ctjpmb.com

[Q69] 查看执行计划
来源：http://awb.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bug.haohaochexian.top

[Q70] 更新统计信息
来源：http://joy.aizwys.cn

ANALYZE TABLE users;
来源：http://zsb.hfpthk.cn

[Q71] 查看建表语句
来源：http://yzx.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwr.aibaodan.cn

[Q72] 查看索引
来源：http://rfb.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://iic.tarul.cn

[Q73] 查看表状态
来源：http://ugt.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://upy.cucudq.cn

[Q74] 强制使用索引
来源：http://mne.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dmw.vehdjk.com

[Q75] 日期格式化
来源：http://qqx.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ukl.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hvh.snrcjt.cn

[Q76] 按天统计
来源：http://iar.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://msj.epnwcf.com

[Q77] 时间加减
来源：http://nag.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fwr.chenjidiqi.icu

[Q78] 当前时间
来源：http://qox.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qyt.bjfxy.top

[Q79] 字符串拼接
来源：http://mtj.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ptv.shzxlz.cn

[Q80] 字符串截取
来源：http://fll.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kvp.zhoulong.xyz

[Q81] 字符串替换
来源：http://sag.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fzf.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://mwi.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xjd.pengpengdd.cyou

[Q83] 大小写转换
来源：http://bzl.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eso.yuanzhike.top

[Q84] 去除首尾空格
来源：http://rvv.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://ewo.dashuyun.cn

[Q85] 数值取整
来源：http://cwa.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://olm.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://dby.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pob.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://ryy.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ges.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://bej.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://axy.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fqp.jiagoushi.top

[Q89] 判断表是否存在
来源：http://pkj.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://viv.cdnleiting.top

[Q90] 生成序号列
来源：http://zxr.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tnd.ydzc1.top

================================================================================
来源：http://kjx.gogol.net.cn

R. Bash 专题
来源：http://lsl.jinqigfzy.top

================================================================================
来源：http://ygp.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://ysh.shzxlz.cn

#!/usr/bin/env bash
来源：http://zth.zhongyouzk.top

set -euo pipefail
来源：http://lec.xuanzx.com

[R02] 变量赋值与使用
来源：http://bmj.cdnleiting.top

name="Tom"; echo "$name"
来源：http://jfj.sjlbkw.cn

[R03] 只读变量
来源：http://wdk.jqgufenzy.top

readonly PI=3.14
来源：http://wyr.chenlongwang.top

[R04] 位置参数
来源：http://ivu.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dpy.aizwys.cn

[R05] 参数默认值
来源：http://fal.zycfv.cn

name="${1:-default}"
来源：http://zli.9152youxi.cn

[R06] 判断命令是否存在
来源：http://set.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cvp.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://bdy.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ssc.nanxuanxn.top

[R08] 数值比较
来源：http://isa.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://epd.ppjwa.cn

[R09] 字符串比较
来源：http://jke.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qyr.tian-w.cn

[R10] 正则匹配
来源：http://sjk.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ijg.yonumen.top

[R11] case 多分支
来源：http://bpk.sysykeji.top

case "$1" in
来源：http://hxe.52xcode.cn

start) echo "启动" ;;
来源：http://ceb.yangfankeji.com

stop)  echo "停止" ;;
来源：http://dpq.redwolf501.top

*)     echo "未知命令" ;;
来源：http://vtb.jinqigfzy.top

esac
来源：http://ufj.pycfn.com

[R12] for 遍历文件
来源：http://cix.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://mxz.gotoacloud.top

[R13] for 计数循环
来源：http://yzi.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://dqk.sysykeji.top

[R14] C 风格 for
来源：http://zqd.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wpd.uphjek.com

[R15] while 逐行读文件
来源：http://blh.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yyl.c1oappe.top

[R16] until 等待条件
来源：http://kth.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cye.sysykeji.top

[R17] 数组定义与取值
来源：http://icx.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://byn.epnwcf.com

[R18] 遍历数组
来源：http://rrm.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://siu.gotoacloud.top

[R19] 数组长度
来源：http://dsm.birdmap.top

echo "${#arr[@]}"
来源：http://xbf.dianchejie.cn

[R20] 关联数组（字典）
来源：http://dfq.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wqk.gzhubu.top

[R21] 字符串长度
来源：http://hma.jiagoushi.top

echo "${#s}"
来源：http://xii.fanxiaobao.xyz

[R22] 截取子串
来源：http://pii.yangfankeji.com

echo "${s:0:5}"
来源：http://kmo.chenjidiqi.icu

[R23] 字符串替换
来源：http://qub.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://psn.52xcode.cn

[R24] 大小写转换
来源：http://rqk.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mva.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://uzn.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uyg.hammf.cn

[R26] 命令替换
来源：http://ija.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://kcu.yj202588.top

[R27] 算术展开
来源：http://qtq.fktsv.cn

echo $((1 + 2 * 3))
来源：http://tnh.epnwcf.com

[R28] 浮点运算
来源：http://gsq.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://opo.yanxiufei.cn

[R29] 定义函数
来源：http://ree.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qlo.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://uks.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://xwm.nanxinkj.top

[R31] 局部变量
来源：http://lhd.tanke756.top


<!-- 参考信息 -->