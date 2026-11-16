代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mhf.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://kjr.jyoumei.cn

[P07] 防抖与节流
来源：http://hwo.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bal.uphjek.com

PHP:  // 手写时间戳比较
来源：http://bcr.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kol.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfi.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rtb.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bvi.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kmj.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yoz.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://jug.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qcp.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hmk.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vqg.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xve.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eis.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svk.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yjt.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aut.daxiang520.top

================================================================================
来源：http://igx.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bky.sufxvd.cn

================================================================================
来源：http://ahh.jianghu66.top

[Q01] 创建表
来源：http://yhe.daria6918.cn

CREATE TABLE users (
来源：http://agm.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hcn.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://rol.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://onl.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ozf.zhengqikj.top

);
来源：http://ify.uphjek.com

[Q02] 创建带外键的表
来源：http://lvx.ehwqpu.com

CREATE TABLE orders (
来源：http://ken.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abq.yj20258.top

user_id INT NOT NULL,
来源：http://wvi.redwolf501.top

amount DECIMAL(10, 2),
来源：http://lsa.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mfs.jinqigfzy.top

);
来源：http://dpl.fanxiaobao.xyz

[Q03] 增加列
来源：http://fnl.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yae.feifeiyinyue.top

[Q04] 修改列类型
来源：http://lxn.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kzw.nwbrower.top

[Q05] 重命名列
来源：http://vsy.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://puq.guowangkeji.top

[Q06] 删除列
来源：http://nns.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://hde.quarkkingdee.top

[Q07] 删除表
来源：http://vum.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://unc.tianlin.xyz

[Q08] 创建普通索引
来源：http://khp.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://cci.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://dzd.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://srj.iojbl.cn

[Q10] 插入单行
来源：http://bwc.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qei.cucudq.cn

[Q11] 一次插入多行
来源：http://pjy.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://csp.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://pon.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://hvf.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ttt.52xcode.cn

[Q13] 忽略重复插入
来源：http://pyc.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aqp.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://pgf.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ynh.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eym.c1oappe.top

[Q15] 查询全部
来源：http://qrh.kuanghao11.cn

SELECT * FROM users;
来源：http://vfu.pengpengdd.cyou

[Q16] 查询指定列
来源：http://crv.dianchejie.cn

SELECT id, name FROM users;
来源：http://nop.hysaishi.cn

[Q17] 条件查询
来源：http://zsa.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ysk.shzxlz.cn

[Q18] 模糊匹配
来源：http://yiu.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ajh.yonumen.top

[Q19] 范围查询
来源：http://bqt.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://plj.fanxiaobao.xyz

[Q20] IN 列表
来源：http://zay.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wvl.bjfxy.top

[Q21] 空值判断
来源：http://zuc.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mvi.xziqi.cn

[Q22] 排序
来源：http://nno.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jlw.zhoulong.xyz

[Q23] 分页
来源：http://ajy.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oij.dashuyun.cn

[Q24] 去重
来源：http://nor.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://ajz.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://gox.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vvf.gotoacloud.top

[Q26] 计数
来源：http://zqi.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://yrw.nwbrower.top

[Q27] 条件计数
来源：http://ewm.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oof.snrcjt.cn

[Q28] 求和与平均
来源：http://pli.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xpk.zhengqikj.top

[Q29] 最大最小值
来源：http://jrz.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yxk.wangdashe.top

[Q30] 分组统计
来源：http://fpq.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bsd.zhoulong.xyz

[Q31] 分组后过滤
来源：http://hpi.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pgx.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://kqr.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wjg.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lxq.yuanzhike.top

[Q33] 多列分组
来源：http://udc.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dam.vqdsnc.cn

[Q34] 每组取第一条
来源：http://rhb.wangdashe.top

SELECT * FROM (
来源：http://qof.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://srj.jyoumei.cn

) t WHERE rn = 1;
来源：http://uxx.zhixingplan.top

[Q35] 内连接
来源：http://gmv.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pfx.sweek.top

[Q36] 左连接
来源：http://zow.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jzh.hysaishi.cn

[Q37] 右连接
来源：http://lqi.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qbp.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://wdo.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dzh.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://ztd.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wnl.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oeb.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xim.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ets.guannengcc.top

[Q41] 多表连接
来源：http://jkv.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kqi.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://kso.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://vxt.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://aim.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://vvx.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rzb.chenjidiqi.icu

[Q43] 标量子查询
来源：http://ggw.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zii.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://phn.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bfd.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://pde.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkl.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://lot.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ojy.sweek.top

[Q47] 与平均值比较
来源：http://moc.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yds.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://tte.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qgp.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://okn.yfazqb.com

[Q49] 更新单行
来源：http://aku.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ivj.cashguo.top

[Q50] 批量更新
来源：http://ism.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vlr.chenlongwang.top

[Q51] 用子查询更新
来源：http://bua.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wqb.aibaodan.cn

[Q52] 删除指定行
来源：http://zdt.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://znd.birdmap.top

[Q53] 按条件删除
来源：http://gfd.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pct.yanxiufei.cn

[Q54] 清空表
来源：http://wov.bjfxy.top

TRUNCATE TABLE logs;
来源：http://cfh.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://sye.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wpe.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://tac.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://guf.316326.xyz

[Q57] 行号
来源：http://lyw.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aaq.guannengcc.top

[Q58] 累计求和
来源：http://tlu.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mji.nwbrower.top

[Q59] 分组内累计
来源：http://ufo.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nvo.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://box.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eoo.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://law.pycfn.com

[Q61] 移动平均
来源：http://bgn.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vxt.chenjidiqi.icu

[Q62] 分组占比
来源：http://dny.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mro.cashguo.top

[Q63] 开启事务
来源：http://jtg.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ppk.bbcook.cn

[Q64] 提交事务
来源：http://wtr.fzhhl.top

COMMIT;
来源：http://vrz.xuanzx.com

[Q65] 回滚事务
来源：http://pqy.xinyue.icu

ROLLBACK;
来源：http://ylf.yuanzhike.top

[Q66] 行锁查询
来源：http://upo.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://clr.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://jzr.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wxj.vehdjk.com

[Q68] 保存点
来源：http://wwh.dianchejie.cn

SAVEPOINT sp1;
来源：http://plg.smart0.xyz

ROLLBACK TO sp1;
来源：http://lsj.ybcxt.top

[Q69] 查看执行计划
来源：http://lpc.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fqz.andypj.xyz

[Q70] 更新统计信息
来源：http://eyc.svipenyu.cn

ANALYZE TABLE users;
来源：http://ozk.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://kzq.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rko.c1oappe.top

[Q72] 查看索引
来源：http://twd.jinqigufen.top

SHOW INDEX FROM users;
来源：http://zkx.ydzc1.top

[Q73] 查看表状态
来源：http://apy.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bue.ivvv.top

[Q74] 强制使用索引
来源：http://ebw.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xmc.dashuyun.cn

[Q75] 日期格式化
来源：http://wfe.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wgx.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rku.tanke756.top

[Q76] 按天统计
来源：http://yhp.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fwz.ybcxt.top

[Q77] 时间加减
来源：http://vnx.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gpp.jinqigfzy.top

[Q78] 当前时间
来源：http://bct.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mei.yonumen.top

[Q79] 字符串拼接
来源：http://gih.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkf.chenzaomai.com

[Q80] 字符串截取
来源：http://idd.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://brr.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://reu.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dzs.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://gik.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nyf.shuidangran.top

[Q83] 大小写转换
来源：http://zfo.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zgi.bbcook.cn

[Q84] 去除首尾空格
来源：http://krp.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://vkt.hesvh.cn

[Q85] 数值取整
来源：http://acd.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mvk.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://tgb.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vap.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://zal.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cnc.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://rao.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lzu.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://boe.yueranfly.top

[Q89] 判断表是否存在
来源：http://mpu.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mrh.yangfankeji.com

[Q90] 生成序号列
来源：http://vxu.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mue.jianghu66.top

================================================================================
来源：http://ybq.yj202588.top

R. Bash 专题
来源：http://zmm.shzxlz.cn

================================================================================
来源：http://aeq.tanke756.top

[R01] shebang 与严格模式
来源：http://sng.hywenlv.cn

#!/usr/bin/env bash
来源：http://bed.gaohongyu789.top

set -euo pipefail
来源：http://exb.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://ldw.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://btc.tanke756.top

[R03] 只读变量
来源：http://kpi.yuanzhike.top

readonly PI=3.14
来源：http://seq.sxryk.cn

[R04] 位置参数
来源：http://ehm.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vrm.tianlin.xyz

[R05] 参数默认值
来源：http://jdb.zhoulong.xyz

name="${1:-default}"
来源：http://fin.chenzaomai.com

[R06] 判断命令是否存在
来源：http://ywv.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsa.quarkkingdee.top

[R07] if 判断文件
来源：http://ciz.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hjk.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://rey.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://utl.sweek.top

[R09] 字符串比较
来源：http://ror.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fus.chenlongwang.top

[R10] 正则匹配
来源：http://ysy.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tjj.fehbvm.com

[R11] case 多分支
来源：http://bxj.fzhhl.top

case "$1" in
来源：http://mdz.jlsjyb.cn

start) echo "启动" ;;
来源：http://rbd.havefunace.top

stop)  echo "停止" ;;
来源：http://pgt.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://rfg.hcnkem.com

esac
来源：http://umi.gaohongyu789.top

[R12] for 遍历文件
来源：http://mvh.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://ryj.yj20258888.top

[R13] for 计数循环
来源：http://itb.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://cyk.dianchejie.cn

[R14] C 风格 for
来源：http://cmk.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hsx.zhengqikj.top

[R15] while 逐行读文件
来源：http://nnp.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qjq.tianlin.xyz

[R16] until 等待条件
来源：http://rxe.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bfy.yvedp.cn

[R17] 数组定义与取值
来源：http://ygt.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://svo.xinyue.icu

[R18] 遍历数组
来源：http://byf.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mml.epnwcf.com

[R19] 数组长度
来源：http://yoa.gaohongyu789.top

echo "${#arr[@]}"
来源：http://zfc.bbcook.cn

[R20] 关联数组（字典）
来源：http://ljj.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bkf.zhijiandao.cn

[R21] 字符串长度
来源：http://wzt.jlsjyb.cn

echo "${#s}"
来源：http://qoj.ppjwa.cn

[R22] 截取子串
来源：http://wxh.ivvv.top

echo "${s:0:5}"
来源：http://yrg.gotoacloud.top

[R23] 字符串替换
来源：http://ubg.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yis.52xcode.cn

[R24] 大小写转换
来源：http://yet.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ivi.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://epj.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sri.gotoacloud.top

[R26] 命令替换
来源：http://zht.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://arm.sxryk.cn

[R27] 算术展开
来源：http://fhp.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://qta.yueranfly.top

[R28] 浮点运算
来源：http://lrv.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://ykb.dashuyun.cn

[R29] 定义函数
来源：http://ivn.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://inj.sufxvd.cn

[R30] 函数返回状态码
来源：http://yut.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://zfl.hammf.cn

[R31] 局部变量
来源：http://fwm.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://pzb.feifeiyinyue.top

[R32] 参数个数校验
来源：http://dvh.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fhj.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://hfb.shanyushiyangkeji.top


<!-- 参考信息 -->