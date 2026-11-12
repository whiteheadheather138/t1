代发 wailian999

PHP:  // 手写时间戳比较
来源：http://kug.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upw.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qst.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fvu.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zel.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ojt.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ize.cheryme.top

[P08] 处理浮点精度问题
来源：http://aia.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rei.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vab.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwt.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mkb.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tnn.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hxd.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://imf.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gzl.andypj.xyz

================================================================================
来源：http://yeb.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ibp.guannengcc.top

================================================================================
来源：http://hkm.gzhubu.top

[Q01] 创建表
来源：http://fyy.jiagoushi.top

CREATE TABLE users (
来源：http://isg.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvt.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://uih.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://soe.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sfl.jinghuilouyu.cn

);
来源：http://twq.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://rfg.jinqigfzy.top

CREATE TABLE orders (
来源：http://oor.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwa.fktsv.cn

user_id INT NOT NULL,
来源：http://trd.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://qfj.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hbh.wangshuangyany.cn

);
来源：http://hof.uphjek.com

[Q03] 增加列
来源：http://oqq.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://plo.yj20258888.top

[Q04] 修改列类型
来源：http://umw.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://inx.iojbl.cn

[Q05] 重命名列
来源：http://bgq.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lbr.fengsongda.top

[Q06] 删除列
来源：http://pdo.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://jdt.pengpengdd.cyou

[Q07] 删除表
来源：http://tpu.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://wag.ctjpmb.com

[Q08] 创建普通索引
来源：http://low.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bre.uphjek.com

[Q09] 创建唯一索引
来源：http://bar.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://llq.yongpay.top

[Q10] 插入单行
来源：http://dmz.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cdi.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://bba.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xmy.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://mln.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://lco.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lnb.tarul.cn

[Q13] 忽略重复插入
来源：http://jgu.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pxw.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://vwo.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ral.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jlu.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://vec.9152youxi.cn

SELECT * FROM users;
来源：http://wkh.feifeiyinyue.top

[Q16] 查询指定列
来源：http://set.cheryme.top

SELECT id, name FROM users;
来源：http://nqh.yangfankeji.com

[Q17] 条件查询
来源：http://pgu.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fql.dianchejie.cn

[Q18] 模糊匹配
来源：http://hgq.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cie.sjlbkw.cn

[Q19] 范围查询
来源：http://lnz.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ltz.guannengcc.top

[Q20] IN 列表
来源：http://gge.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lmy.gogol.net.cn

[Q21] 空值判断
来源：http://swo.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://win.xziqi.cn

[Q22] 排序
来源：http://zir.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mcy.xuetiantiany.cn

[Q23] 分页
来源：http://nxe.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ecl.yj202588.top

[Q24] 去重
来源：http://mju.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://pig.shzxlz.cn

[Q25] 只取前 N 条
来源：http://roi.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qsx.hnxiangtu.top

[Q26] 计数
来源：http://wlg.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://obm.guowangkeji.top

[Q27] 条件计数
来源：http://jor.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nju.zdqjudy.top

[Q28] 求和与平均
来源：http://rzh.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sxw.yonumen.top

[Q29] 最大最小值
来源：http://mag.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://oys.zhoulong.xyz

[Q30] 分组统计
来源：http://jcg.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xjz.shzxlz.cn

[Q31] 分组后过滤
来源：http://nwn.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyi.cucudq.cn

[Q32] 分组拼接字符串
来源：http://oms.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qom.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rja.sysykeji.top

[Q33] 多列分组
来源：http://hsn.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xit.tarul.cn

[Q34] 每组取第一条
来源：http://mao.cucudq.cn

SELECT * FROM (
来源：http://nfn.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cmi.nwbrower.top

) t WHERE rn = 1;
来源：http://qnq.jianghu66.top

[Q35] 内连接
来源：http://jxk.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://npk.iojbl.cn

[Q36] 左连接
来源：http://fax.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://poc.yueranfly.top

[Q37] 右连接
来源：http://pxe.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dth.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://tdm.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pyy.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://agp.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dyy.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wyz.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://evi.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yjl.redwolf501.top

[Q41] 多表连接
来源：http://xkf.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uwp.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://jkt.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://jpz.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://zhd.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://lxg.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gws.xziqi.cn

[Q43] 标量子查询
来源：http://fic.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://doc.zhiwuduotai.top

[Q44] IN 子查询
来源：http://jyi.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zzc.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://khr.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rfr.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jbw.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jns.jyoumei.cn

[Q47] 与平均值比较
来源：http://gui.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hze.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://fhb.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tkd.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://vpo.zhijiandao.cn

[Q49] 更新单行
来源：http://wex.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yub.birdmap.top

[Q50] 批量更新
来源：http://sve.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zwk.vehdjk.com

[Q51] 用子查询更新
来源：http://jlb.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rtb.zhoulong.xyz

[Q52] 删除指定行
来源：http://clw.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://wrq.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://gft.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sda.gogol.net.cn

[Q54] 清空表
来源：http://mvi.cashguo.top

TRUNCATE TABLE logs;
来源：http://eww.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://nbf.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hlb.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://whs.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://twa.jyoumei.cn

[Q57] 行号
来源：http://zmr.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vtv.ydjk.org.cn

[Q58] 累计求和
来源：http://kqh.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hjj.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://yfj.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cdr.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://egw.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dwj.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cxh.ybcxt.top

[Q61] 移动平均
来源：http://bne.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ixy.hnxiangtu.top

[Q62] 分组占比
来源：http://sbd.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jdr.ehwqpu.com

[Q63] 开启事务
来源：http://cqj.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ztv.xuetiantiany.cn

[Q64] 提交事务
来源：http://tms.52xcode.cn

COMMIT;
来源：http://qfk.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://kpo.jqgfzy.top

ROLLBACK;
来源：http://foc.xylfe.cn

[Q66] 行锁查询
来源：http://ruh.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mxx.ybcxt.top

[Q67] 设置隔离级别
来源：http://nyg.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://psx.xziqi.cn

[Q68] 保存点
来源：http://wdj.snrcjt.cn

SAVEPOINT sp1;
来源：http://zuz.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://aup.fzhhl.top

[Q69] 查看执行计划
来源：http://qee.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wri.jianghu66.top

[Q70] 更新统计信息
来源：http://opi.xuanzx.com

ANALYZE TABLE users;
来源：http://mot.hfpthk.cn

[Q71] 查看建表语句
来源：http://shq.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rsa.yj202588.top

[Q72] 查看索引
来源：http://ima.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://gya.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://jfm.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lgd.guannengcc.top

[Q74] 强制使用索引
来源：http://bvc.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ytf.dashuyun.cn

[Q75] 日期格式化
来源：http://ttl.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sgw.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjn.uphjek.com

[Q76] 按天统计
来源：http://snh.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://opy.sweek.top

[Q77] 时间加减
来源：http://cxp.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jlz.yueranfly.top

[Q78] 当前时间
来源：http://nvf.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rhs.chenzaomai.com

[Q79] 字符串拼接
来源：http://rhg.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://riy.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://rpt.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hiy.haohaochexian.top

[Q81] 字符串替换
来源：http://sam.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zpc.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://ljb.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hqr.gotoacloud.top

[Q83] 大小写转换
来源：http://ddy.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bqw.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://hdv.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://vjy.ppjwa.cn

[Q85] 数值取整
来源：http://llf.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://usb.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://skv.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wgu.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://lfb.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sei.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://jix.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qrl.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uxg.birdmap.top

[Q89] 判断表是否存在
来源：http://yyg.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hzd.yj20258888.top

[Q90] 生成序号列
来源：http://sok.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rrj.sweek.top

================================================================================
来源：http://imp.yueranfly.top

R. Bash 专题
来源：http://kpc.jqgufenzy.top

================================================================================
来源：http://ykp.zdqjudy.top

[R01] shebang 与严格模式
来源：http://qnb.kuanghao11.cn

#!/usr/bin/env bash
来源：http://tfg.guowangkeji.top

set -euo pipefail
来源：http://swx.ehwqpu.com

[R02] 变量赋值与使用
来源：http://und.svipenyu.cn

name="Tom"; echo "$name"
来源：http://tkl.cheryme.top

[R03] 只读变量
来源：http://xll.guannengcc.top

readonly PI=3.14
来源：http://yaz.birdmap.top

[R04] 位置参数
来源：http://vgo.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vem.hywenlv.cn

[R05] 参数默认值
来源：http://chg.jinyuanbaomall.cn

name="${1:-default}"
来源：http://jaa.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://gwz.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibi.jlsjyb.cn

[R07] if 判断文件
来源：http://kbm.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mvr.hnqzz.top

[R08] 数值比较
来源：http://geh.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ujj.sweek.top

[R09] 字符串比较
来源：http://izu.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gjf.52xcode.cn

[R10] 正则匹配
来源：http://iyb.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysl.52xcode.cn

[R11] case 多分支
来源：http://nui.yonumen.top

case "$1" in
来源：http://egt.fktsv.cn

start) echo "启动" ;;
来源：http://mue.sysykeji.top

stop)  echo "停止" ;;
来源：http://yry.cucudq.cn

*)     echo "未知命令" ;;
来源：http://xvd.yfazqb.com

esac
来源：http://hcf.fengsongda.top

[R12] for 遍历文件
来源：http://ggz.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://mfk.wangdashe.top

[R13] for 计数循环
来源：http://hhl.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://lmt.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://fly.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zcs.ctjpmb.com

[R15] while 逐行读文件
来源：http://kaq.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://brn.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://bzb.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fcg.aizwys.cn

[R17] 数组定义与取值
来源：http://xbj.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://nqe.quarkkingdee.top

[R18] 遍历数组
来源：http://sxz.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yhx.316326.xyz

[R19] 数组长度
来源：http://pcr.yuxming.cn

echo "${#arr[@]}"
来源：http://mjx.0kj1m.cn

[R20] 关联数组（字典）
来源：http://hmb.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aoj.shuidangran.top

[R21] 字符串长度
来源：http://jan.yanxiufei.cn

echo "${#s}"
来源：http://lbt.ehwqpu.com

[R22] 截取子串
来源：http://bfm.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://uux.cucudq.cn

[R23] 字符串替换
来源：http://ayd.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sph.havefunace.top

[R24] 大小写转换
来源：http://pit.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://onh.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://jeu.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://utv.redwolf501.top

[R26] 命令替换
来源：http://vyd.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://quy.fzhhl.top

[R27] 算术展开
来源：http://avs.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://ogk.quarkkingdee.top

[R28] 浮点运算
来源：http://bcg.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://day.sysykeji.top

[R29] 定义函数
来源：http://vkn.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pyw.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://vxa.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://lio.pycfn.com

[R31] 局部变量
来源：http://eak.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://dnx.sxryk.cn

[R32] 参数个数校验
来源：http://vhw.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ukm.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://bpf.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sho.hammf.cn

[R34] 退出时清理
来源：http://etk.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://qdm.zhijiandao.cn

[R35] 后台执行并等待
来源：http://fxi.pycfn.com


<!-- 参考信息 -->