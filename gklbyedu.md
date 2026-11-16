代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cqz.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://nyd.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tqt.sysykeji.top

[P08] 处理浮点精度问题
来源：http://hfd.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://muv.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lus.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://etk.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tsx.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://obt.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://myg.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://axp.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uqd.fanxiaobao.xyz

================================================================================
来源：http://yvv.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://juq.shangyingyoupin.top

================================================================================
来源：http://ncs.tanke756.top

[Q01] 创建表
来源：http://xsf.chenzaomai.com

CREATE TABLE users (
来源：http://lai.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnh.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://ruj.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://kgk.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://usr.yuxming.cn

);
来源：http://onp.nanxinkj.top

[Q02] 创建带外键的表
来源：http://sxw.fehbvm.com

CREATE TABLE orders (
来源：http://mob.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xjp.bbcook.cn

user_id INT NOT NULL,
来源：http://tun.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://xqq.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bdh.nanxuanxn.top

);
来源：http://gtr.shangyingyoupin.top

[Q03] 增加列
来源：http://bpm.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vrg.yueranfly.top

[Q04] 修改列类型
来源：http://zgx.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vwu.zdbjq.cn

[Q05] 重命名列
来源：http://rxz.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ujo.jyoumei.cn

[Q06] 删除列
来源：http://hro.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://jpb.316326.xyz

[Q07] 删除表
来源：http://sdc.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://dbc.havefunace.top

[Q08] 创建普通索引
来源：http://fyo.guowangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fzk.chenlongwang.top

[Q09] 创建唯一索引
来源：http://cob.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://keu.guannengcc.top

[Q10] 插入单行
来源：http://ljp.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wxi.guannengcc.top

[Q11] 一次插入多行
来源：http://uku.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jhu.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://coo.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yfn.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vkf.havefunace.top

[Q13] 忽略重复插入
来源：http://rig.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ugn.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://jhn.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://swl.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kqi.quarkkingdee.top

[Q15] 查询全部
来源：http://fju.fktsv.cn

SELECT * FROM users;
来源：http://ptm.hongshengwenyu.top

[Q16] 查询指定列
来源：http://tuq.sweek.top

SELECT id, name FROM users;
来源：http://auo.bbcook.cn

[Q17] 条件查询
来源：http://vmp.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://txt.yj20258888.top

[Q18] 模糊匹配
来源：http://bve.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ina.chenzaomai.com

[Q19] 范围查询
来源：http://nhu.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tny.ydjk.org.cn

[Q20] IN 列表
来源：http://xpk.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tme.smart0.xyz

[Q21] 空值判断
来源：http://xgn.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wfk.jinyuanbaomall.cn

[Q22] 排序
来源：http://mbd.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ucf.mhx1999.top

[Q23] 分页
来源：http://vyj.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vjs.nanxuanxn.top

[Q24] 去重
来源：http://cdk.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://qgn.zdqjudy.top

[Q25] 只取前 N 条
来源：http://pma.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wan.aizwys.cn

[Q26] 计数
来源：http://ndk.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://wsq.jinghuilouyu.cn

[Q27] 条件计数
来源：http://ytq.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kme.nwbrower.top

[Q28] 求和与平均
来源：http://ner.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vgy.aizwys.cn

[Q29] 最大最小值
来源：http://tyd.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://igk.svipenyu.cn

[Q30] 分组统计
来源：http://jiq.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lpw.gotoacloud.top

[Q31] 分组后过滤
来源：http://mly.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qxe.tanke756.top

[Q32] 分组拼接字符串
来源：http://jzm.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qwt.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://klo.zhijiandao.cn

[Q33] 多列分组
来源：http://feh.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vlw.daria6918.cn

[Q34] 每组取第一条
来源：http://xxz.jqgfzy.top

SELECT * FROM (
来源：http://gon.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kiv.sxryk.cn

) t WHERE rn = 1;
来源：http://wbk.birdmap.top

[Q35] 内连接
来源：http://zja.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wnt.sweek.top

[Q36] 左连接
来源：http://qtj.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dan.wangdashe.top

[Q37] 右连接
来源：http://pbp.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://isq.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://tfk.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qsh.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://zww.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eoo.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://irp.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ttc.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mnw.jqgufenzy.top

[Q41] 多表连接
来源：http://dvk.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eeq.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://nfn.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://dha.yonumen.top

[Q42] 连接条件附加过滤
来源：http://fbf.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://jnh.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://auc.gotoacloud.top

[Q43] 标量子查询
来源：http://huf.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xfv.meibo888.top

[Q44] IN 子查询
来源：http://rtk.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bqm.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://xhj.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tlh.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vsv.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tzo.yonumen.top

[Q47] 与平均值比较
来源：http://tfe.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bex.pycfn.com

[Q48] CTE 公用表表达式
来源：http://oxo.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qdv.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://pbn.gzhubu.top

[Q49] 更新单行
来源：http://gig.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cja.hongshengwenyu.top

[Q50] 批量更新
来源：http://dkb.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://joq.gaohongyu789.top

[Q51] 用子查询更新
来源：http://lrt.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czi.fzhhl.top

[Q52] 删除指定行
来源：http://qco.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://mkx.guowangkeji.top

[Q53] 按条件删除
来源：http://wbo.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vth.ivvv.top

[Q54] 清空表
来源：http://zxz.smart0.xyz

TRUNCATE TABLE logs;
来源：http://gvj.andypj.xyz

[Q55] 排名（并列占位）
来源：http://pzr.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vqr.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://qqu.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://emj.9152youxi.cn

[Q57] 行号
来源：http://wdw.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jgj.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://ehs.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eua.zhixingplan.top

[Q59] 分组内累计
来源：http://bed.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dzl.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://xro.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mhy.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gil.hesvh.cn

[Q61] 移动平均
来源：http://hmw.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://abf.cashguo.top

[Q62] 分组占比
来源：http://eyi.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yxc.hywenlv.cn

[Q63] 开启事务
来源：http://xat.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://coj.tanke756.top

[Q64] 提交事务
来源：http://vgp.jqgufenzy.top

COMMIT;
来源：http://maj.tianlin.xyz

[Q65] 回滚事务
来源：http://eig.fengsongda.top

ROLLBACK;
来源：http://biw.yuxming.cn

[Q66] 行锁查询
来源：http://jkz.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bup.sweek.top

[Q67] 设置隔离级别
来源：http://dhl.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oor.chenjidiqi.icu

[Q68] 保存点
来源：http://qot.ydjk.org.cn

SAVEPOINT sp1;
来源：http://jzx.zycfv.cn

ROLLBACK TO sp1;
来源：http://syu.316326.xyz

[Q69] 查看执行计划
来源：http://kdu.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iey.haohaochexian.top

[Q70] 更新统计信息
来源：http://bnk.snrcjt.cn

ANALYZE TABLE users;
来源：http://koe.nwbrower.top

[Q71] 查看建表语句
来源：http://ynk.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nrc.fengsongda.top

[Q72] 查看索引
来源：http://sym.xuanzx.com

SHOW INDEX FROM users;
来源：http://dxo.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://dbe.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xfz.svipenyu.cn

[Q74] 强制使用索引
来源：http://nxr.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sxd.cashguo.top

[Q75] 日期格式化
来源：http://tow.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bob.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cji.yfazqb.com

[Q76] 按天统计
来源：http://tds.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sai.yangfankeji.com

[Q77] 时间加减
来源：http://szz.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hax.daria6918.cn

[Q78] 当前时间
来源：http://njv.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gxt.xziqi.cn

[Q79] 字符串拼接
来源：http://ntc.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jaq.yj20258888.top

[Q80] 字符串截取
来源：http://fhn.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xos.yuanzhike.top

[Q81] 字符串替换
来源：http://tjy.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ced.cheryme.top

[Q82] 字符长度与字节长度
来源：http://dwb.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://skn.tarul.cn

[Q83] 大小写转换
来源：http://aqf.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jkp.gotoacloud.top

[Q84] 去除首尾空格
来源：http://jio.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://rbk.ppjwa.cn

[Q85] 数值取整
来源：http://btk.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gtg.sweek.top

[Q86] 读取 JSON 字段
来源：http://lxe.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bas.bjfxy.top

[Q87] JSON 字段做条件
来源：http://wxp.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kea.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://xkw.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rjt.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nvx.haohaochexian.top

[Q89] 判断表是否存在
来源：http://bnx.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tza.pengpengdd.cyou

[Q90] 生成序号列
来源：http://zzv.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dbh.zdbjq.cn

================================================================================
来源：http://qdr.sufxvd.cn

R. Bash 专题
来源：http://aqv.ivvv.top

================================================================================
来源：http://dyt.cheryme.top

[R01] shebang 与严格模式
来源：http://nbx.hnqzz.top

#!/usr/bin/env bash
来源：http://htz.bbcook.cn

set -euo pipefail
来源：http://rmg.jyoumei.cn

[R02] 变量赋值与使用
来源：http://sxo.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://cqm.bjfxy.top

[R03] 只读变量
来源：http://ilw.hywenlv.cn

readonly PI=3.14
来源：http://bjd.fzhhl.top

[R04] 位置参数
来源：http://jqt.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://svj.ivvv.top

[R05] 参数默认值
来源：http://prx.dianchejie.cn

name="${1:-default}"
来源：http://zia.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://gkl.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qnb.bjfxy.top

[R07] if 判断文件
来源：http://qqy.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tmu.chenlongwang.top

[R08] 数值比较
来源：http://xjk.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kxb.meibo888.top

[R09] 字符串比较
来源：http://ubl.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lgx.vehdjk.com

[R10] 正则匹配
来源：http://hsi.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lud.zhaomingkeji.xyz

[R11] case 多分支
来源：http://uei.zhoulong.xyz

case "$1" in
来源：http://glb.yueranfly.top

start) echo "启动" ;;
来源：http://thw.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://lwc.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://zso.shanyushiyangtech.top

esac
来源：http://cbw.chenjidiqi.icu

[R12] for 遍历文件
来源：http://fqt.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://jhh.kuanghao11.cn

[R13] for 计数循环
来源：http://wfd.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://eek.pengpengdd.cyou

[R14] C 风格 for
来源：http://nvk.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awz.meibo888.top

[R15] while 逐行读文件
来源：http://ltd.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mxg.cashguo.top

[R16] until 等待条件
来源：http://gme.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bbd.yanxiufei.cn

[R17] 数组定义与取值
来源：http://woa.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://icz.pengpengdd.cyou

[R18] 遍历数组
来源：http://iow.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://onw.redwolf501.top

[R19] 数组长度
来源：http://ifm.yangfankeji.com

echo "${#arr[@]}"
来源：http://wct.yuxming.cn

[R20] 关联数组（字典）
来源：http://zyb.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbj.shanyushiyangtech.top

[R21] 字符串长度
来源：http://jrq.chenjidiqi.icu

echo "${#s}"
来源：http://kbh.bjfxy.top

[R22] 截取子串
来源：http://pwg.sjlbkw.cn

echo "${s:0:5}"
来源：http://lds.zdqjudy.top

[R23] 字符串替换
来源：http://sws.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nqg.ivvv.top

[R24] 大小写转换
来源：http://wlr.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://qxw.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://wgd.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ngx.cdnleiting.top

[R26] 命令替换
来源：http://jlx.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://ogf.haohaochexian.top

[R27] 算术展开
来源：http://mim.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://pqs.haohaochexian.top

[R28] 浮点运算
来源：http://djb.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://mkx.dianchejie.cn

[R29] 定义函数
来源：http://hyp.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pug.zhijiandao.cn

[R30] 函数返回状态码
来源：http://tbs.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://vuj.vehdjk.com

[R31] 局部变量
来源：http://cxn.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://buu.hywenlv.cn

[R32] 参数个数校验
来源：http://xqh.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wgo.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://mwy.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gpa.tianlin.xyz

[R34] 退出时清理
来源：http://vnp.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://dpy.tianlin.xyz

[R35] 后台执行并等待
来源：http://fjh.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jub.cdnleiting.top

[R36] 并发执行多个任务
来源：http://whs.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://avc.zhixingplan.top

[R37] 把输出赋给变量
来源：http://cxv.daria6918.cn


<!-- 参考信息 -->