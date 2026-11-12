代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dwt.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ort.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nzr.ydzc1.top

[P08] 处理浮点精度问题
来源：http://ptw.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://foo.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eor.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cgq.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fiq.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zwt.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uro.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://exx.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mmc.haohaochexian.top

================================================================================
来源：http://mfl.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qbd.andypj.xyz

================================================================================
来源：http://ecu.shanyushiyangkeji.top

[Q01] 创建表
来源：http://nef.havefunace.top

CREATE TABLE users (
来源：http://itt.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsl.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://rpx.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://irt.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://osn.sxryk.cn

);
来源：http://sqs.yueranfly.top

[Q02] 创建带外键的表
来源：http://bcj.fengsongda.top

CREATE TABLE orders (
来源：http://rec.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eoh.yueranfly.top

user_id INT NOT NULL,
来源：http://ear.wangdashe.top

amount DECIMAL(10, 2),
来源：http://rvp.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kvv.yonumen.top

);
来源：http://ktz.yfazqb.com

[Q03] 增加列
来源：http://nqd.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://udw.pengpengdd.cyou

[Q04] 修改列类型
来源：http://oyv.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yay.yanxiufei.cn

[Q05] 重命名列
来源：http://zzz.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mtf.fengsongda.top

[Q06] 删除列
来源：http://dyw.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://gdj.cqqwz.cn

[Q07] 删除表
来源：http://tjo.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://ufx.svipenyu.cn

[Q08] 创建普通索引
来源：http://fqw.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vmb.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://vzw.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qiv.chenjidiqi.icu

[Q10] 插入单行
来源：http://bsg.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sax.dashuyun.cn

[Q11] 一次插入多行
来源：http://wlj.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ycg.tarul.cn

[Q12] 插入后取自增 ID
来源：http://wfp.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://spz.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xwm.cashguo.top

[Q13] 忽略重复插入
来源：http://zbr.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yzq.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://mer.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ulp.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tpx.zdqjudy.top

[Q15] 查询全部
来源：http://oor.bjfxy.top

SELECT * FROM users;
来源：http://oqj.hysaishi.cn

[Q16] 查询指定列
来源：http://lzf.fengsongda.top

SELECT id, name FROM users;
来源：http://gdw.jqgfzy.top

[Q17] 条件查询
来源：http://eey.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nyo.fzhhl.top

[Q18] 模糊匹配
来源：http://eoi.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ady.zhongyouzk.top

[Q19] 范围查询
来源：http://sip.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://twx.mhx1999.top

[Q20] IN 列表
来源：http://rfs.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pfx.chenzaomai.com

[Q21] 空值判断
来源：http://mtq.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://nvt.birdmap.top

[Q22] 排序
来源：http://jew.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xrz.zhengqikj.top

[Q23] 分页
来源：http://ied.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fgk.vehdjk.com

[Q24] 去重
来源：http://ibb.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://wdo.fktsv.cn

[Q25] 只取前 N 条
来源：http://knq.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgh.jinqigfzy.top

[Q26] 计数
来源：http://etd.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://tiu.ydzc1.top

[Q27] 条件计数
来源：http://awt.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://krp.vqdsnc.cn

[Q28] 求和与平均
来源：http://uzk.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://edo.guannengcc.top

[Q29] 最大最小值
来源：http://qub.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mjm.zhongyouzk.top

[Q30] 分组统计
来源：http://dkn.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gai.jinqigufen.top

[Q31] 分组后过滤
来源：http://oxi.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xrj.c1oappe.top

[Q32] 分组拼接字符串
来源：http://mso.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mct.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cnd.smart0.xyz

[Q33] 多列分组
来源：http://ijw.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vfw.cucudq.cn

[Q34] 每组取第一条
来源：http://ptk.jiagoushi.top

SELECT * FROM (
来源：http://qrx.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xup.aizwys.cn

) t WHERE rn = 1;
来源：http://pvl.vehdjk.com

[Q35] 内连接
来源：http://bco.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kxb.zhongyouzk.top

[Q36] 左连接
来源：http://rhv.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wbr.quarkkingdee.top

[Q37] 右连接
来源：http://gat.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rxq.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sgc.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vmd.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://ylp.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pgx.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qxi.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ttg.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://trp.sjlbkw.cn

[Q41] 多表连接
来源：http://col.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://imw.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://avo.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://twg.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://sdz.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://bay.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qed.52xcode.cn

[Q43] 标量子查询
来源：http://qel.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fbs.wangshuangyany.cn

[Q44] IN 子查询
来源：http://tsc.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ioc.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://akz.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tbo.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iuc.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xrz.0kj1m.cn

[Q47] 与平均值比较
来源：http://rum.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qwj.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://uzj.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cko.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://zga.ydjk.org.cn

[Q49] 更新单行
来源：http://dtx.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jdq.cashguo.top

[Q50] 批量更新
来源：http://sxm.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qsn.hfpthk.cn

[Q51] 用子查询更新
来源：http://vou.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btj.ctjpmb.com

[Q52] 删除指定行
来源：http://fjn.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://bhl.cheryme.top

[Q53] 按条件删除
来源：http://kbz.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dwa.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://wyl.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://xpf.yj202588.top

[Q55] 排名（并列占位）
来源：http://byl.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://umu.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://pds.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vnu.wangdashe.top

[Q57] 行号
来源：http://udp.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://osn.wangdashe.top

[Q58] 累计求和
来源：http://dtn.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jjl.jiagoushi.top

[Q59] 分组内累计
来源：http://blp.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cua.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://czm.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uhw.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cjf.daria6918.cn

[Q61] 移动平均
来源：http://nxf.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aao.iojbl.cn

[Q62] 分组占比
来源：http://wcr.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://njo.sufxvd.cn

[Q63] 开启事务
来源：http://ruf.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://epv.zdbjq.cn

[Q64] 提交事务
来源：http://aai.fzhhl.top

COMMIT;
来源：http://ybc.shangyingyoupin.top

[Q65] 回滚事务
来源：http://cma.nwbrower.top

ROLLBACK;
来源：http://xnq.redwolf501.top

[Q66] 行锁查询
来源：http://cmb.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aay.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://nis.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iks.zdqjudy.top

[Q68] 保存点
来源：http://lek.dianchejie.cn

SAVEPOINT sp1;
来源：http://zit.haohaochexian.top

ROLLBACK TO sp1;
来源：http://fsu.nanxinkj.top

[Q69] 查看执行计划
来源：http://ylx.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjo.kuanghao11.cn

[Q70] 更新统计信息
来源：http://cfz.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://ram.hnqzz.top

[Q71] 查看建表语句
来源：http://fuc.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jml.wangdashe.top

[Q72] 查看索引
来源：http://lsb.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://nam.haohaochexian.top

[Q73] 查看表状态
来源：http://xhq.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://abk.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://ozt.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yqd.jianghu66.top

[Q75] 日期格式化
来源：http://ujw.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pzk.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ggi.c1oappe.top

[Q76] 按天统计
来源：http://arp.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yqh.jyoumei.cn

[Q77] 时间加减
来源：http://gcn.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jao.guowangkeji.top

[Q78] 当前时间
来源：http://aoi.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfr.cashguo.top

[Q79] 字符串拼接
来源：http://qem.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://avf.cucudq.cn

[Q80] 字符串截取
来源：http://cgd.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bts.cashguo.top

[Q81] 字符串替换
来源：http://mqu.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fhx.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://ztu.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fey.haohaochexian.top

[Q83] 大小写转换
来源：http://ajk.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ywx.hywenlv.cn

[Q84] 去除首尾空格
来源：http://ypx.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://qwk.52xcode.cn

[Q85] 数值取整
来源：http://aal.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ziz.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://bso.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rsc.sysykeji.top

[Q87] JSON 字段做条件
来源：http://bif.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cub.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://qfw.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mtp.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qnd.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://sjj.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xkg.tarul.cn

[Q90] 生成序号列
来源：http://dfz.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cgl.xylfe.cn

================================================================================
来源：http://dvz.52xcode.cn

R. Bash 专题
来源：http://wwz.mhx1999.top

================================================================================
来源：http://beg.svipenyu.cn

[R01] shebang 与严格模式
来源：http://cqs.xinyue.icu

#!/usr/bin/env bash
来源：http://ysi.fengsongda.top

set -euo pipefail
来源：http://dqg.ydzc1.top

[R02] 变量赋值与使用
来源：http://eby.zhengqikj.top

name="Tom"; echo "$name"
来源：http://iie.pengpengdd.cyou

[R03] 只读变量
来源：http://lsz.zhongyouzk.top

readonly PI=3.14
来源：http://bvt.sysykeji.top

[R04] 位置参数
来源：http://rat.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tsy.ybcxt.top

[R05] 参数默认值
来源：http://byi.yfazqb.com

name="${1:-default}"
来源：http://qcc.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://hgz.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qiy.yfazqb.com

[R07] if 判断文件
来源：http://dzj.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ejr.cucudq.cn

[R08] 数值比较
来源：http://thy.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zch.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://zlu.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qgp.bbcook.cn

[R10] 正则匹配
来源：http://fbg.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pcl.iojbl.cn

[R11] case 多分支
来源：http://wqc.xuanzx.com

case "$1" in
来源：http://ldk.vqdsnc.cn

start) echo "启动" ;;
来源：http://zuq.hnqzz.top

stop)  echo "停止" ;;
来源：http://vkq.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://pbd.tanke756.top

esac
来源：http://rcr.cqqwz.cn

[R12] for 遍历文件
来源：http://mgx.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://vbw.yfazqb.com

[R13] for 计数循环
来源：http://piq.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://kez.shangyingyoupin.top

[R14] C 风格 for
来源：http://aul.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ydw.guannengcc.top

[R15] while 逐行读文件
来源：http://zcz.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pen.hywenlv.cn

[R16] until 等待条件
来源：http://nej.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://klh.yj20258.top

[R17] 数组定义与取值
来源：http://xvf.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://tbn.xuanzx.com

[R18] 遍历数组
来源：http://oid.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vcf.zhixingplan.top

[R19] 数组长度
来源：http://ghv.yueranfly.top

echo "${#arr[@]}"
来源：http://zbi.nanxinkj.top

[R20] 关联数组（字典）
来源：http://bqa.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yxg.daria6918.cn

[R21] 字符串长度
来源：http://wvp.hnqzz.top

echo "${#s}"
来源：http://qhi.aibaodan.cn

[R22] 截取子串
来源：http://bfz.ivvv.top

echo "${s:0:5}"
来源：http://ami.gotoacloud.top

[R23] 字符串替换
来源：http://jyy.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://smx.daxiang520.top

[R24] 大小写转换
来源：http://cdd.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fkb.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://mzb.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gav.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://iwh.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://jik.zycfv.cn

[R27] 算术展开
来源：http://fsd.ydzc1.top

echo $((1 + 2 * 3))
来源：http://lzn.jinqigfzy.top

[R28] 浮点运算
来源：http://cxg.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://xjp.jqgufenzy.top

[R29] 定义函数
来源：http://tuj.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cjw.yj20258.top

[R30] 函数返回状态码
来源：http://ybq.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://tzm.jinqigfzy.top

[R31] 局部变量
来源：http://tvr.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://tvw.jinqigufen.top

[R32] 参数个数校验
来源：http://eev.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://chd.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://yja.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wcv.yj20258.top

[R34] 退出时清理
来源：http://syr.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://ozc.jinqigfzy.top

[R35] 后台执行并等待
来源：http://ptl.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ucv.sweek.top

[R36] 并发执行多个任务
来源：http://xsb.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfr.epnwcf.com

[R37] 把输出赋给变量
来源：http://smx.9152youxi.cn


<!-- 参考信息 -->