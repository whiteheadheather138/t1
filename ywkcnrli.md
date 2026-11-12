代发 wailian999

PHP:  // 手写时间戳比较
来源：http://ccv.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lbk.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrf.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pin.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mau.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mrw.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mim.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://ivm.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iyu.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://clz.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qwg.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ajg.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vij.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wtg.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://whb.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qrx.zdqjudy.top

================================================================================
来源：http://wab.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uxe.havefunace.top

================================================================================
来源：http://ijh.yuxming.cn

[Q01] 创建表
来源：http://ezo.shuidangran.top

CREATE TABLE users (
来源：http://snv.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mbq.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://qfm.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://iff.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nix.xuanzx.com

);
来源：http://nce.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://qwe.cucudq.cn

CREATE TABLE orders (
来源：http://lkg.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jzl.yongpay.top

user_id INT NOT NULL,
来源：http://ikc.cucudq.cn

amount DECIMAL(10, 2),
来源：http://ptc.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uzp.zdqjudy.top

);
来源：http://uyx.shanyushiyangtech.top

[Q03] 增加列
来源：http://gyn.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nbm.yueranfly.top

[Q04] 修改列类型
来源：http://uyn.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qkn.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://pwg.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cfx.hongshengwenyu.top

[Q06] 删除列
来源：http://far.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://xwt.yj20258888.top

[Q07] 删除表
来源：http://lun.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://bbn.nanxuanxn.top

[Q08] 创建普通索引
来源：http://okl.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://xbm.sufxvd.cn

[Q09] 创建唯一索引
来源：http://rqn.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wij.fktsv.cn

[Q10] 插入单行
来源：http://cfk.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uti.yj20258888.top

[Q11] 一次插入多行
来源：http://vcj.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cex.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://len.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bjx.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jxp.daxiang520.top

[Q13] 忽略重复插入
来源：http://wsw.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nzu.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://crb.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uhd.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cwv.daxiang520.top

[Q15] 查询全部
来源：http://enx.gogol.net.cn

SELECT * FROM users;
来源：http://frh.tian-w.cn

[Q16] 查询指定列
来源：http://snq.birdmap.top

SELECT id, name FROM users;
来源：http://dwo.sxryk.cn

[Q17] 条件查询
来源：http://ath.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kow.mhx1999.top

[Q18] 模糊匹配
来源：http://ujv.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iyv.yj202588.top

[Q19] 范围查询
来源：http://wfp.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uhh.jianghu66.top

[Q20] IN 列表
来源：http://xzd.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uwj.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://hjm.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xcw.jinqigufen.top

[Q22] 排序
来源：http://xce.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ixr.fehbvm.com

[Q23] 分页
来源：http://nvn.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://faw.birdmap.top

[Q24] 去重
来源：http://jfn.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://omx.andypj.xyz

[Q25] 只取前 N 条
来源：http://pnj.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pme.sxryk.cn

[Q26] 计数
来源：http://bgv.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://ybc.gogol.net.cn

[Q27] 条件计数
来源：http://ube.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://syt.nanxinkj.top

[Q28] 求和与平均
来源：http://pwd.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xkz.hnxiangtu.top

[Q29] 最大最小值
来源：http://kww.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://quv.zhengqikj.top

[Q30] 分组统计
来源：http://mmc.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lyn.kuanghao11.cn

[Q31] 分组后过滤
来源：http://gdg.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bxq.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://oki.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hqq.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ble.yvedp.cn

[Q33] 多列分组
来源：http://cug.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vnj.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://wid.fanxiaobao.xyz

SELECT * FROM (
来源：http://add.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hcb.yanxiufei.cn

) t WHERE rn = 1;
来源：http://llx.9152youxi.cn

[Q35] 内连接
来源：http://iav.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://skt.zdqjudy.top

[Q36] 左连接
来源：http://qur.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aql.tanke756.top

[Q37] 右连接
来源：http://bpr.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tel.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://alr.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bns.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://mrq.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ojm.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cil.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yot.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oes.xylfe.cn

[Q41] 多表连接
来源：http://gju.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zsa.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://xre.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://qvi.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://wce.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://uvt.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ces.nanxinkj.top

[Q43] 标量子查询
来源：http://pfh.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qhq.meibo888.top

[Q44] IN 子查询
来源：http://sqc.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hys.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://bfy.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ayc.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://kbd.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nko.yvedp.cn

[Q47] 与平均值比较
来源：http://rrq.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iso.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://hod.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nxv.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://hcj.sufxvd.cn

[Q49] 更新单行
来源：http://ypp.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://axj.ydjk.org.cn

[Q50] 批量更新
来源：http://xzq.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dcl.birdmap.top

[Q51] 用子查询更新
来源：http://yzt.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wiy.c1oappe.top

[Q52] 删除指定行
来源：http://icw.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://hcf.gzhubu.top

[Q53] 按条件删除
来源：http://oxg.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://apv.aizwys.cn

[Q54] 清空表
来源：http://eip.xziqi.cn

TRUNCATE TABLE logs;
来源：http://fju.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://afa.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nwd.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://nrc.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vmi.wangshuangyany.cn

[Q57] 行号
来源：http://ayc.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iyr.andypj.xyz

[Q58] 累计求和
来源：http://tzx.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tsz.snrcjt.cn

[Q59] 分组内累计
来源：http://per.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zhu.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://wjk.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dlf.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fwy.shzxlz.cn

[Q61] 移动平均
来源：http://bau.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dju.hysaishi.cn

[Q62] 分组占比
来源：http://zwj.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tec.gaohongyu789.top

[Q63] 开启事务
来源：http://sje.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fem.guowangkeji.top

[Q64] 提交事务
来源：http://wpy.pengpengdd.cyou

COMMIT;
来源：http://nfl.fktsv.cn

[Q65] 回滚事务
来源：http://zcd.hammf.cn

ROLLBACK;
来源：http://lfc.shzxlz.cn

[Q66] 行锁查询
来源：http://feq.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fvv.gotoacloud.top

[Q67] 设置隔离级别
来源：http://qdm.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bba.pengpengdd.cyou

[Q68] 保存点
来源：http://yjq.ydzc1.top

SAVEPOINT sp1;
来源：http://vei.jqgfzy.top

ROLLBACK TO sp1;
来源：http://npc.ybcxt.top

[Q69] 查看执行计划
来源：http://mok.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pcv.yangfankeji.com

[Q70] 更新统计信息
来源：http://qaz.ydzc1.top

ANALYZE TABLE users;
来源：http://wox.aizwys.cn

[Q71] 查看建表语句
来源：http://kah.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dqf.fehbvm.com

[Q72] 查看索引
来源：http://jey.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://qbb.andypj.xyz

[Q73] 查看表状态
来源：http://jgi.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://frr.iojbl.cn

[Q74] 强制使用索引
来源：http://uwj.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jzc.jinqigufen.top

[Q75] 日期格式化
来源：http://php.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmd.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hhg.vehdjk.com

[Q76] 按天统计
来源：http://mte.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yec.zhixingplan.top

[Q77] 时间加减
来源：http://nzj.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pzt.feifeiyinyue.top

[Q78] 当前时间
来源：http://elh.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wrf.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://zxq.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pwl.snrcjt.cn

[Q80] 字符串截取
来源：http://xsf.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xfo.zhixingplan.top

[Q81] 字符串替换
来源：http://cgw.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rxp.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://dsj.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yzi.xuanzx.com

[Q83] 大小写转换
来源：http://osu.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jrt.ppjwa.cn

[Q84] 去除首尾空格
来源：http://zcs.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://cyc.cheryme.top

[Q85] 数值取整
来源：http://drm.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dwb.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://fih.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bsg.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://wlt.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://srk.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://kgc.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://flt.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://unr.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://fbr.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://msb.0kj1m.cn

[Q90] 生成序号列
来源：http://cfk.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lpv.xziqi.cn

================================================================================
来源：http://thh.jinqigufen.top

R. Bash 专题
来源：http://tqc.iojbl.cn

================================================================================
来源：http://dhg.ivvv.top

[R01] shebang 与严格模式
来源：http://sac.hfpthk.cn

#!/usr/bin/env bash
来源：http://gmb.chenjidiqi.icu

set -euo pipefail
来源：http://seg.dashuyun.cn

[R02] 变量赋值与使用
来源：http://kjv.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://idd.guannengcc.top

[R03] 只读变量
来源：http://eej.jyoumei.cn

readonly PI=3.14
来源：http://uub.haohaochexian.top

[R04] 位置参数
来源：http://ipj.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://orh.cheryme.top

[R05] 参数默认值
来源：http://oyt.hywenlv.cn

name="${1:-default}"
来源：http://qfc.havefunace.top

[R06] 判断命令是否存在
来源：http://bxk.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ocl.zhijiandao.cn

[R07] if 判断文件
来源：http://tkc.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ewi.wangdashe.top

[R08] 数值比较
来源：http://roy.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aho.gogol.net.cn

[R09] 字符串比较
来源：http://tio.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wnd.jqgufenzy.top

[R10] 正则匹配
来源：http://wvy.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jmv.gaohongyu789.top

[R11] case 多分支
来源：http://mnv.pengpengdd.cyou

case "$1" in
来源：http://rpj.aizwys.cn

start) echo "启动" ;;
来源：http://hli.sysykeji.top

stop)  echo "停止" ;;
来源：http://jcc.epnwcf.com

*)     echo "未知命令" ;;
来源：http://ttg.zycfv.cn

esac
来源：http://phd.iojbl.cn

[R12] for 遍历文件
来源：http://vok.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://rjp.kuanghao11.cn

[R13] for 计数循环
来源：http://rem.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://ifs.sysykeji.top

[R14] C 风格 for
来源：http://inv.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hct.ybcxt.top

[R15] while 逐行读文件
来源：http://ytc.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xnz.hysaishi.cn

[R16] until 等待条件
来源：http://msi.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qvu.vqdsnc.cn

[R17] 数组定义与取值
来源：http://crg.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://bsp.epnwcf.com

[R18] 遍历数组
来源：http://boa.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qwt.gaohongyu789.top

[R19] 数组长度
来源：http://utn.zhijiandao.cn

echo "${#arr[@]}"
来源：http://isk.gzhubu.top

[R20] 关联数组（字典）
来源：http://wjg.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nse.zycfv.cn

[R21] 字符串长度
来源：http://kzb.xylfe.cn

echo "${#s}"
来源：http://vls.birdmap.top

[R22] 截取子串
来源：http://tif.gzhubu.top

echo "${s:0:5}"
来源：http://mqb.xuetiantiany.cn

[R23] 字符串替换
来源：http://bcx.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://owa.zycfv.cn

[R24] 大小写转换
来源：http://djv.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://zsd.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://jhk.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pmr.hnqzz.top

[R26] 命令替换
来源：http://tmo.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://yxh.guannengcc.top

[R27] 算术展开
来源：http://uwa.vehdjk.com

echo $((1 + 2 * 3))
来源：http://xvg.bjfxy.top

[R28] 浮点运算
来源：http://zus.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://wyk.shanyushiyangtech.top

[R29] 定义函数
来源：http://yiq.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yjr.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://qqi.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://uyc.hfpthk.cn

[R31] 局部变量
来源：http://bwt.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://ztd.pycfn.com

[R32] 参数个数校验
来源：http://otl.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jnq.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://qgl.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dnu.cheryme.top

[R34] 退出时清理
来源：http://nky.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://bkr.yuxming.cn

[R35] 后台执行并等待
来源：http://keo.shzxlz.cn


<!-- 参考信息 -->