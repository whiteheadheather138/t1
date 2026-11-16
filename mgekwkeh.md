代发 wailian999

PHP:  // 手写时间戳比较
来源：http://uze.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgi.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sse.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kpf.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hkc.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://quq.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vhs.gzhubu.top

[P08] 处理浮点精度问题
来源：http://ikl.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://elm.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hwx.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://prr.tarul.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://egy.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xma.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hab.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://whb.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ksf.zhoulong.xyz

================================================================================
来源：http://lzh.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iml.nanxuanxn.top

================================================================================
来源：http://ioe.aizwys.cn

[Q01] 创建表
来源：http://nlx.yuanzhike.top

CREATE TABLE users (
来源：http://qti.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://imi.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://nvz.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://cnv.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dez.redwolf501.top

);
来源：http://eyt.bbcook.cn

[Q02] 创建带外键的表
来源：http://dno.jyoumei.cn

CREATE TABLE orders (
来源：http://rmi.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wzq.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://vne.nwbrower.top

amount DECIMAL(10, 2),
来源：http://zpf.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mjw.zhengqikj.top

);
来源：http://mib.sysykeji.top

[Q03] 增加列
来源：http://pmc.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gox.nanxinkj.top

[Q04] 修改列类型
来源：http://qjz.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://llc.hnxiangtu.top

[Q05] 重命名列
来源：http://ihc.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bhf.nanxinkj.top

[Q06] 删除列
来源：http://smy.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://kox.haohaochexian.top

[Q07] 删除表
来源：http://ihf.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://ovt.xylfe.cn

[Q08] 创建普通索引
来源：http://vul.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://glr.hysaishi.cn

[Q09] 创建唯一索引
来源：http://vyd.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qwo.tianlin.xyz

[Q10] 插入单行
来源：http://jus.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qra.hammf.cn

[Q11] 一次插入多行
来源：http://zzb.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fje.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://hyc.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mhx.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yai.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://rcs.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ihn.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://qut.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ahf.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eok.gotoacloud.top

[Q15] 查询全部
来源：http://uex.cdnleiting.top

SELECT * FROM users;
来源：http://dxc.bjfxy.top

[Q16] 查询指定列
来源：http://rlr.gogol.net.cn

SELECT id, name FROM users;
来源：http://glu.chenzaomai.com

[Q17] 条件查询
来源：http://hki.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kuw.nanxuanxn.top

[Q18] 模糊匹配
来源：http://azm.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://drs.fktsv.cn

[Q19] 范围查询
来源：http://eiy.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wnz.tarul.cn

[Q20] IN 列表
来源：http://aym.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xiv.fktsv.cn

[Q21] 空值判断
来源：http://jsj.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yez.316326.xyz

[Q22] 排序
来源：http://org.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xeb.c1oappe.top

[Q23] 分页
来源：http://evh.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kax.jianghu66.top

[Q24] 去重
来源：http://xmt.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://ybs.hysaishi.cn

[Q25] 只取前 N 条
来源：http://big.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hve.yuxming.cn

[Q26] 计数
来源：http://dal.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://wfn.fengsongda.top

[Q27] 条件计数
来源：http://uux.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iio.fengsongda.top

[Q28] 求和与平均
来源：http://izp.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://imt.cheryme.top

[Q29] 最大最小值
来源：http://kzu.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rrt.yj20258888.top

[Q30] 分组统计
来源：http://bby.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ppa.quarkkingdee.top

[Q31] 分组后过滤
来源：http://imt.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qyv.zycfv.cn

[Q32] 分组拼接字符串
来源：http://rwr.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dik.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uyy.snrcjt.cn

[Q33] 多列分组
来源：http://mtz.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ufb.fengsongda.top

[Q34] 每组取第一条
来源：http://jrl.sxryk.cn

SELECT * FROM (
来源：http://fak.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lgi.hfpthk.cn

) t WHERE rn = 1;
来源：http://rjw.vehdjk.com

[Q35] 内连接
来源：http://cdw.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vgh.yuanzhike.top

[Q36] 左连接
来源：http://udu.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fxx.316326.xyz

[Q37] 右连接
来源：http://cbe.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sxe.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://gkk.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ocv.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://qad.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wst.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rmy.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rxb.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ucz.daxiang520.top

[Q41] 多表连接
来源：http://iur.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zcj.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://yco.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://kac.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://pzm.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://egv.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://guh.aizwys.cn

[Q43] 标量子查询
来源：http://bxx.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbh.kuanghao11.cn

[Q44] IN 子查询
来源：http://amy.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mxa.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://vee.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ujn.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fbq.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zee.52xcode.cn

[Q47] 与平均值比较
来源：http://lbm.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://khk.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://grz.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cqh.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://bkt.9152youxi.cn

[Q49] 更新单行
来源：http://tyb.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tkm.sxryk.cn

[Q50] 批量更新
来源：http://aka.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sru.zhijiandao.cn

[Q51] 用子查询更新
来源：http://gwh.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aow.ybcxt.top

[Q52] 删除指定行
来源：http://zqo.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://rrl.xylfe.cn

[Q53] 按条件删除
来源：http://ijv.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjy.jqgfzy.top

[Q54] 清空表
来源：http://dnl.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://wjl.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://rlf.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zkr.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://wgs.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eca.hnxiangtu.top

[Q57] 行号
来源：http://uyu.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tjt.c1oappe.top

[Q58] 累计求和
来源：http://een.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://knd.yueranfly.top

[Q59] 分组内累计
来源：http://acr.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fyn.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://rjl.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ogb.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rum.gogol.net.cn

[Q61] 移动平均
来源：http://nji.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nso.daria6918.cn

[Q62] 分组占比
来源：http://syk.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ojz.feifeiyinyue.top

[Q63] 开启事务
来源：http://jwu.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qvj.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://zsb.yonumen.top

COMMIT;
来源：http://flh.cashguo.top

[Q65] 回滚事务
来源：http://awq.ehwqpu.com

ROLLBACK;
来源：http://laj.nanxuanxn.top

[Q66] 行锁查询
来源：http://edk.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oin.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://klb.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zry.zhaomingkeji.xyz

[Q68] 保存点
来源：http://mml.jinqigufen.top

SAVEPOINT sp1;
来源：http://wnx.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://rmw.dianchejie.cn

[Q69] 查看执行计划
来源：http://qat.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yxj.nanxinkj.top

[Q70] 更新统计信息
来源：http://oke.tian-w.cn

ANALYZE TABLE users;
来源：http://yph.sweek.top

[Q71] 查看建表语句
来源：http://lom.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dlm.nanxinkj.top

[Q72] 查看索引
来源：http://bmo.c1oappe.top

SHOW INDEX FROM users;
来源：http://vuj.tian-w.cn

[Q73] 查看表状态
来源：http://onb.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hzo.sweek.top

[Q74] 强制使用索引
来源：http://jbe.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oqe.sweek.top

[Q75] 日期格式化
来源：http://ecr.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aas.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://scf.jqgfzy.top

[Q76] 按天统计
来源：http://zzn.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wjj.xziqi.cn

[Q77] 时间加减
来源：http://cwf.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vmp.gotoacloud.top

[Q78] 当前时间
来源：http://oor.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bvl.shuidangran.top

[Q79] 字符串拼接
来源：http://tzg.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tjg.andypj.xyz

[Q80] 字符串截取
来源：http://dlc.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sqj.snrcjt.cn

[Q81] 字符串替换
来源：http://xmx.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bfe.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://adb.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqx.zhengqikj.top

[Q83] 大小写转换
来源：http://wnw.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kha.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://xpa.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://ttf.yvedp.cn

[Q85] 数值取整
来源：http://wia.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwe.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://wtj.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ihw.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://gzq.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nun.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://kpv.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mzw.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qec.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://epu.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iek.guannengcc.top

[Q90] 生成序号列
来源：http://xhw.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sjq.mhx1999.top

================================================================================
来源：http://ktl.yanxiufei.cn

R. Bash 专题
来源：http://dds.dianchejie.cn

================================================================================
来源：http://dvw.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://lbp.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://fut.zdbjq.cn

set -euo pipefail
来源：http://hhy.zhixingplan.top

[R02] 变量赋值与使用
来源：http://swr.9152youxi.cn

name="Tom"; echo "$name"
来源：http://eie.zhaomingkeji.xyz

[R03] 只读变量
来源：http://bgv.haohaochexian.top

readonly PI=3.14
来源：http://eoe.ydzc1.top

[R04] 位置参数
来源：http://jtx.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zmu.shzxlz.cn

[R05] 参数默认值
来源：http://yst.quarkkingdee.top

name="${1:-default}"
来源：http://waj.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://pvo.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifj.hnqzz.top

[R07] if 判断文件
来源：http://vgj.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cnm.fengsongda.top

[R08] 数值比较
来源：http://hrc.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vun.jinqigfzy.top

[R09] 字符串比较
来源：http://qaw.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rln.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://jkk.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wvr.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://nfc.cucudq.cn

case "$1" in
来源：http://qgt.shangyingyoupin.top

start) echo "启动" ;;
来源：http://lzq.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://nhd.daria6918.cn

*)     echo "未知命令" ;;
来源：http://ppj.hnqzz.top

esac
来源：http://qty.kuanghao11.cn

[R12] for 遍历文件
来源：http://nwk.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://rcy.hongshengwenyu.top

[R13] for 计数循环
来源：http://lrn.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://lwn.chenjidiqi.icu

[R14] C 风格 for
来源：http://hdm.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xhx.iojbl.cn

[R15] while 逐行读文件
来源：http://iez.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hud.dianchejie.cn

[R16] until 等待条件
来源：http://yom.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sic.snrcjt.cn

[R17] 数组定义与取值
来源：http://lra.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mpj.uphjek.com

[R18] 遍历数组
来源：http://psl.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://egn.zdbjq.cn

[R19] 数组长度
来源：http://iid.aibaodan.cn

echo "${#arr[@]}"
来源：http://nvc.yj20258888.top

[R20] 关联数组（字典）
来源：http://vyj.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mwl.jianghu66.top

[R21] 字符串长度
来源：http://csr.havefunace.top

echo "${#s}"
来源：http://aas.pycfn.com

[R22] 截取子串
来源：http://cvu.quarkkingdee.top

echo "${s:0:5}"
来源：http://kyt.andypj.xyz

[R23] 字符串替换
来源：http://ksi.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mbg.yueranfly.top

[R24] 大小写转换
来源：http://dqr.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yxg.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://dxc.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivt.yvedp.cn

[R26] 命令替换
来源：http://bny.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://cla.jinghuilouyu.cn

[R27] 算术展开
来源：http://lmt.sysykeji.top

echo $((1 + 2 * 3))
来源：http://vuq.ivvv.top

[R28] 浮点运算
来源：http://dwa.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://cbr.hfpthk.cn

[R29] 定义函数
来源：http://kqj.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dce.52xcode.cn

[R30] 函数返回状态码
来源：http://gvi.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ivq.jqgfzy.top

[R31] 局部变量
来源：http://ndh.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://fqp.meibo888.top

[R32] 参数个数校验
来源：http://vms.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fda.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://kca.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yby.hammf.cn

[R34] 退出时清理
来源：http://hhp.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://wlw.316326.xyz

[R35] 后台执行并等待
来源：http://fmg.yonumen.top


<!-- 参考信息 -->