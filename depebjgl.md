代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fqu.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bzu.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mwr.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vct.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qoj.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://chq.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kpt.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmu.gzhubu.top

================================================================================
来源：http://wnw.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fpm.tian-w.cn

================================================================================
来源：http://gyy.sufxvd.cn

[Q01] 创建表
来源：http://acf.fzhhl.top

CREATE TABLE users (
来源：http://gnm.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsc.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://suv.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://baj.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zgw.fktsv.cn

);
来源：http://grq.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://ijh.cashguo.top

CREATE TABLE orders (
来源：http://ioq.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dds.sufxvd.cn

user_id INT NOT NULL,
来源：http://ygz.yueranfly.top

amount DECIMAL(10, 2),
来源：http://vxq.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fqa.dashuyun.cn

);
来源：http://wnt.aibaodan.cn

[Q03] 增加列
来源：http://hyb.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://glb.shzxlz.cn

[Q04] 修改列类型
来源：http://ezj.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ztt.hcnkem.com

[Q05] 重命名列
来源：http://knl.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cee.dashuyun.cn

[Q06] 删除列
来源：http://lsu.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://kjf.ydzc1.top

[Q07] 删除表
来源：http://jni.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://yjq.hnqzz.top

[Q08] 创建普通索引
来源：http://arr.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ezw.iojbl.cn

[Q09] 创建唯一索引
来源：http://wjw.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ymi.zhoulong.xyz

[Q10] 插入单行
来源：http://jua.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tmz.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://ygi.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://txm.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://mdy.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://wxt.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wyx.hammf.cn

[Q13] 忽略重复插入
来源：http://gwx.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gnh.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://nrr.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cie.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fhu.xinyue.icu

[Q15] 查询全部
来源：http://kfa.tanke756.top

SELECT * FROM users;
来源：http://uua.guannengcc.top

[Q16] 查询指定列
来源：http://icr.zhijiandao.cn

SELECT id, name FROM users;
来源：http://gib.jiagoushi.top

[Q17] 条件查询
来源：http://ziu.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pid.snrcjt.cn

[Q18] 模糊匹配
来源：http://zku.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zgr.zhiwuduotai.top

[Q19] 范围查询
来源：http://ftd.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pjw.jlsjyb.cn

[Q20] IN 列表
来源：http://fes.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rtt.jiagoushi.top

[Q21] 空值判断
来源：http://imi.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://efr.zhoulong.xyz

[Q22] 排序
来源：http://zot.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oxl.fanxiaobao.xyz

[Q23] 分页
来源：http://wqa.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uza.316326.xyz

[Q24] 去重
来源：http://rid.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://aai.ivvv.top

[Q25] 只取前 N 条
来源：http://eed.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://crg.zhengqikj.top

[Q26] 计数
来源：http://gzy.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://fmr.gotoacloud.top

[Q27] 条件计数
来源：http://hrt.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qyj.xuanzx.com

[Q28] 求和与平均
来源：http://vhi.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kez.zhixingplan.top

[Q29] 最大最小值
来源：http://nyn.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gzp.zycfv.cn

[Q30] 分组统计
来源：http://hju.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sxk.zycfv.cn

[Q31] 分组后过滤
来源：http://hwc.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bvd.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://djv.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uya.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mjw.jinqigufen.top

[Q33] 多列分组
来源：http://elt.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zdd.jinqigfzy.top

[Q34] 每组取第一条
来源：http://xhz.gogol.net.cn

SELECT * FROM (
来源：http://ehd.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://chu.zhoulong.xyz

) t WHERE rn = 1;
来源：http://auf.fzhhl.top

[Q35] 内连接
来源：http://zyy.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iyu.pycfn.com

[Q36] 左连接
来源：http://nll.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pwd.ywan-chungtsiang.top

[Q37] 右连接
来源：http://djf.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://enf.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pam.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qqn.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://jwr.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pwl.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hhh.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://igq.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ryz.hfpthk.cn

[Q41] 多表连接
来源：http://tho.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://bth.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://lmu.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://kic.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://cyl.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://sbc.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vnn.ctjpmb.com

[Q43] 标量子查询
来源：http://tdy.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://euw.zdbjq.cn

[Q44] IN 子查询
来源：http://jmr.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qjr.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://tcm.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hlg.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://jlk.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ysc.cqqwz.cn

[Q47] 与平均值比较
来源：http://ndf.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ulq.316326.xyz

[Q48] CTE 公用表表达式
来源：http://kfa.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qns.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://mwl.cqqwz.cn

[Q49] 更新单行
来源：http://tcb.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uaq.jiagoushi.top

[Q50] 批量更新
来源：http://pqo.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vwa.0kj1m.cn

[Q51] 用子查询更新
来源：http://gyg.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jtb.chenjidiqi.icu

[Q52] 删除指定行
来源：http://jzl.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://zaw.ydzc1.top

[Q53] 按条件删除
来源：http://tkj.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ojc.52xcode.cn

[Q54] 清空表
来源：http://kyy.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://nsm.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://joa.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ufy.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://epu.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mdh.zhengqikj.top

[Q57] 行号
来源：http://jgb.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gls.meibo888.top

[Q58] 累计求和
来源：http://gpg.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qve.9152youxi.cn

[Q59] 分组内累计
来源：http://fji.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tjx.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://jye.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://syy.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://edq.daria6918.cn

[Q61] 移动平均
来源：http://acl.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ryc.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://ter.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dzm.vqdsnc.cn

[Q63] 开启事务
来源：http://bgk.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tdh.jinqigufen.top

[Q64] 提交事务
来源：http://euf.fehbvm.com

COMMIT;
来源：http://omb.vqdsnc.cn

[Q65] 回滚事务
来源：http://pce.daria6918.cn

ROLLBACK;
来源：http://hzi.hnqzz.top

[Q66] 行锁查询
来源：http://yjf.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fge.cucudq.cn

[Q67] 设置隔离级别
来源：http://oad.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zoc.nanxuanxn.top

[Q68] 保存点
来源：http://div.zhengqikj.top

SAVEPOINT sp1;
来源：http://acm.sufxvd.cn

ROLLBACK TO sp1;
来源：http://uhu.nwbrower.top

[Q69] 查看执行计划
来源：http://naz.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ijp.jlsjyb.cn

[Q70] 更新统计信息
来源：http://nhm.quarkkingdee.top

ANALYZE TABLE users;
来源：http://oxu.gotoacloud.top

[Q71] 查看建表语句
来源：http://rgu.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iaq.smart0.xyz

[Q72] 查看索引
来源：http://mya.jiagoushi.top

SHOW INDEX FROM users;
来源：http://jfr.hongshengwenyu.top

[Q73] 查看表状态
来源：http://mpb.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://reh.jqgfzy.top

[Q74] 强制使用索引
来源：http://smd.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dys.fengsongda.top

[Q75] 日期格式化
来源：http://stp.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://syp.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pdl.hnqzz.top

[Q76] 按天统计
来源：http://kxf.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gsy.haohaochexian.top

[Q77] 时间加减
来源：http://lzi.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://erz.jianghu66.top

[Q78] 当前时间
来源：http://nrj.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ctk.cashguo.top

[Q79] 字符串拼接
来源：http://ygs.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kak.hfpthk.cn

[Q80] 字符串截取
来源：http://ghv.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://agx.shzxlz.cn

[Q81] 字符串替换
来源：http://tfr.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zus.yj20258.top

[Q82] 字符长度与字节长度
来源：http://rgg.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xpk.9152youxi.cn

[Q83] 大小写转换
来源：http://gco.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xol.cdnleiting.top

[Q84] 去除首尾空格
来源：http://bul.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://fdq.redwolf501.top

[Q85] 数值取整
来源：http://mwm.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jld.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://qwy.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jyk.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://vrq.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qjy.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://lns.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zvu.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kmg.guannengcc.top

[Q89] 判断表是否存在
来源：http://hbd.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://opq.9152youxi.cn

[Q90] 生成序号列
来源：http://wzi.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fwn.zhaomingkeji.xyz

================================================================================
来源：http://yho.meibo888.top

R. Bash 专题
来源：http://hhd.daria6918.cn

================================================================================
来源：http://lsu.havefunace.top

[R01] shebang 与严格模式
来源：http://clt.sweek.top

#!/usr/bin/env bash
来源：http://yjp.cucudq.cn

set -euo pipefail
来源：http://dmi.hywenlv.cn

[R02] 变量赋值与使用
来源：http://lty.chenlongwang.top

name="Tom"; echo "$name"
来源：http://csl.hcnkem.com

[R03] 只读变量
来源：http://vje.sxryk.cn

readonly PI=3.14
来源：http://qap.tian-w.cn

[R04] 位置参数
来源：http://zfb.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://srq.jlsjyb.cn

[R05] 参数默认值
来源：http://kbg.ydzc1.top

name="${1:-default}"
来源：http://orq.svipenyu.cn

[R06] 判断命令是否存在
来源：http://kxs.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oeq.uphjek.com

[R07] if 判断文件
来源：http://xmg.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://slf.zhiwuduotai.top

[R08] 数值比较
来源：http://smz.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://azn.cucudq.cn

[R09] 字符串比较
来源：http://yze.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://knq.snrcjt.cn

[R10] 正则匹配
来源：http://tls.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pio.shuidangran.top

[R11] case 多分支
来源：http://jfe.tarul.cn

case "$1" in
来源：http://hyw.ppjwa.cn

start) echo "启动" ;;
来源：http://eib.cdnleiting.top

stop)  echo "停止" ;;
来源：http://idx.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://lml.jiagoushi.top

esac
来源：http://xkq.sufxvd.cn

[R12] for 遍历文件
来源：http://zur.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://mcn.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://aso.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://yzu.jinqigfzy.top

[R14] C 风格 for
来源：http://txd.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aai.nanxuanxn.top

[R15] while 逐行读文件
来源：http://yav.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kvf.pengpengdd.cyou

[R16] until 等待条件
来源：http://lqq.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://avn.zhoulong.xyz

[R17] 数组定义与取值
来源：http://hyr.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vno.andypj.xyz

[R18] 遍历数组
来源：http://fxe.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oia.yueranfly.top

[R19] 数组长度
来源：http://sff.hfpthk.cn

echo "${#arr[@]}"
来源：http://uld.zhixingplan.top

[R20] 关联数组（字典）
来源：http://vag.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yrn.zhijiandao.cn

[R21] 字符串长度
来源：http://hmh.guannengcc.top

echo "${#s}"
来源：http://fmx.hfpthk.cn

[R22] 截取子串
来源：http://xdi.havefunace.top

echo "${s:0:5}"
来源：http://cpe.shangyingyoupin.top

[R23] 字符串替换
来源：http://upv.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fng.zdqjudy.top

[R24] 大小写转换
来源：http://ffv.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://nsn.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ubk.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iwx.tian-w.cn

[R26] 命令替换
来源：http://qxp.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://vvo.zdbjq.cn

[R27] 算术展开
来源：http://nmx.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://pkg.ctjpmb.com

[R28] 浮点运算
来源：http://lip.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://acn.kuanghao11.cn

[R29] 定义函数
来源：http://rhj.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://llu.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://oso.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://rgd.shzxlz.cn

[R31] 局部变量
来源：http://vec.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://zqn.gzhubu.top

[R32] 参数个数校验
来源：http://dkv.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gvg.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://fjj.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mtx.hnqzz.top

[R34] 退出时清理
来源：http://mar.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hwa.hywenlv.cn

[R35] 后台执行并等待
来源：http://kby.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gxp.cashguo.top

[R36] 并发执行多个任务
来源：http://rwz.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://snn.fzhhl.top

[R37] 把输出赋给变量
来源：http://bqw.316326.xyz

files=$(ls -1)
来源：http://dak.zhijiandao.cn

[R38] 管道串联
来源：http://wfq.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://zas.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://gjh.cqqwz.cn


<!-- 参考信息 -->