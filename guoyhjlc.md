代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mmg.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hxf.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://isd.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://axf.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kqv.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://etf.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bzy.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bqu.zhongyouzk.top

================================================================================
来源：http://hxr.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hit.52xcode.cn

================================================================================
来源：http://rgh.xuanzx.com

[Q01] 创建表
来源：http://ihq.yuxming.cn

CREATE TABLE users (
来源：http://ihr.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqn.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://eai.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://xii.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gli.hnxiangtu.top

);
来源：http://ztz.zhengqikj.top

[Q02] 创建带外键的表
来源：http://dsd.sjlbkw.cn

CREATE TABLE orders (
来源：http://vwz.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://odu.tarul.cn

user_id INT NOT NULL,
来源：http://mag.52xcode.cn

amount DECIMAL(10, 2),
来源：http://tbx.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eyk.jqgfzy.top

);
来源：http://bww.xziqi.cn

[Q03] 增加列
来源：http://wea.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ote.dianchejie.cn

[Q04] 修改列类型
来源：http://qjr.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dgr.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://vhp.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zsw.zycfv.cn

[Q06] 删除列
来源：http://pmh.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://mee.jianghu66.top

[Q07] 删除表
来源：http://jyi.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://sju.kuanghao11.cn

[Q08] 创建普通索引
来源：http://zqt.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vuw.ctjpmb.com

[Q09] 创建唯一索引
来源：http://bad.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lyd.sysykeji.top

[Q10] 插入单行
来源：http://inh.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uzn.haohaochexian.top

[Q11] 一次插入多行
来源：http://cnd.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fxk.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://ixp.tanke756.top

INSERT INTO users (name) VALUES ('C');
来源：http://bpz.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gov.fengsongda.top

[Q13] 忽略重复插入
来源：http://fgy.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://acl.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://fxg.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dfe.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kgd.haohaochexian.top

[Q15] 查询全部
来源：http://ldk.gogol.net.cn

SELECT * FROM users;
来源：http://pyl.haohaochexian.top

[Q16] 查询指定列
来源：http://mdg.chenzaomai.com

SELECT id, name FROM users;
来源：http://rsj.c1oappe.top

[Q17] 条件查询
来源：http://sia.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lkv.aibaodan.cn

[Q18] 模糊匹配
来源：http://dgf.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ysp.fanxiaobao.xyz

[Q19] 范围查询
来源：http://dma.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fhb.jiagoushi.top

[Q20] IN 列表
来源：http://vag.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vmf.ybcxt.top

[Q21] 空值判断
来源：http://vxq.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jzh.pengpengdd.cyou

[Q22] 排序
来源：http://axs.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xtx.guannengcc.top

[Q23] 分页
来源：http://png.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nry.ppjwa.cn

[Q24] 去重
来源：http://cdy.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://cpd.guowangkeji.top

[Q25] 只取前 N 条
来源：http://zln.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://crs.xziqi.cn

[Q26] 计数
来源：http://jci.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://ggm.ehwqpu.com

[Q27] 条件计数
来源：http://zdb.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pnx.haohaochexian.top

[Q28] 求和与平均
来源：http://wjx.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hlq.hnxiangtu.top

[Q29] 最大最小值
来源：http://gyw.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qyb.pycfn.com

[Q30] 分组统计
来源：http://pcb.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vjt.daxiang520.top

[Q31] 分组后过滤
来源：http://azt.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zfk.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://qmk.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxf.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://twp.zhongyouzk.top

[Q33] 多列分组
来源：http://jpp.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zav.52xcode.cn

[Q34] 每组取第一条
来源：http://ifw.birdmap.top

SELECT * FROM (
来源：http://izc.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wcq.chenzaomai.com

) t WHERE rn = 1;
来源：http://lbr.ivvv.top

[Q35] 内连接
来源：http://ddg.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wxf.guowangkeji.top

[Q36] 左连接
来源：http://lhj.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rjq.ywan-chungtsiang.top

[Q37] 右连接
来源：http://ovg.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvz.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hpk.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vtr.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://mwh.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://szf.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xri.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hni.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yot.0kj1m.cn

[Q41] 多表连接
来源：http://zjb.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xmr.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://haz.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://prr.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://ulf.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://hgm.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lby.yangfankeji.com

[Q43] 标量子查询
来源：http://ubb.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tuj.ybcxt.top

[Q44] IN 子查询
来源：http://qfs.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ztm.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://ovn.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ykn.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://ydq.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmt.yonumen.top

[Q47] 与平均值比较
来源：http://twt.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nmu.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://fbx.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pkg.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://ygm.hnqzz.top

[Q49] 更新单行
来源：http://ftc.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fnq.sweek.top

[Q50] 批量更新
来源：http://wai.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rsk.cashguo.top

[Q51] 用子查询更新
来源：http://sqn.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tle.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://yza.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://vhc.zhixingplan.top

[Q53] 按条件删除
来源：http://tfa.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kvc.yueranfly.top

[Q54] 清空表
来源：http://qoi.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://zzl.gzhubu.top

[Q55] 排名（并列占位）
来源：http://zdk.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yvr.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://kpn.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://und.pycfn.com

[Q57] 行号
来源：http://qxc.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wdp.shanyushiyangtech.top

[Q58] 累计求和
来源：http://ywm.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uoc.hfpthk.cn

[Q59] 分组内累计
来源：http://afk.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rma.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://cwc.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iob.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ube.jinqigufen.top

[Q61] 移动平均
来源：http://opa.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zar.fehbvm.com

[Q62] 分组占比
来源：http://jtp.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bkq.jiagoushi.top

[Q63] 开启事务
来源：http://uij.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ztv.ctjpmb.com

[Q64] 提交事务
来源：http://evs.hcnkem.com

COMMIT;
来源：http://pzp.havefunace.top

[Q65] 回滚事务
来源：http://xau.0kj1m.cn

ROLLBACK;
来源：http://wlo.fengsongda.top

[Q66] 行锁查询
来源：http://jcf.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vxl.9152youxi.cn

[Q67] 设置隔离级别
来源：http://wvw.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kkd.52xcode.cn

[Q68] 保存点
来源：http://reg.daxiang520.top

SAVEPOINT sp1;
来源：http://xcf.yuanzhike.top

ROLLBACK TO sp1;
来源：http://bcn.fktsv.cn

[Q69] 查看执行计划
来源：http://qzl.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jgc.nanxinkj.top

[Q70] 更新统计信息
来源：http://zcm.daria6918.cn

ANALYZE TABLE users;
来源：http://pfl.xinyue.icu

[Q71] 查看建表语句
来源：http://lke.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oep.dashuyun.cn

[Q72] 查看索引
来源：http://ypn.tianlin.xyz

SHOW INDEX FROM users;
来源：http://nej.chenzaomai.com

[Q73] 查看表状态
来源：http://abb.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fzl.nwbrower.top

[Q74] 强制使用索引
来源：http://fgq.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://djo.shuidangran.top

[Q75] 日期格式化
来源：http://uqu.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xjo.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qwa.mhx1999.top

[Q76] 按天统计
来源：http://ypi.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bcx.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://yds.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ffb.sysykeji.top

[Q78] 当前时间
来源：http://mzz.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hru.yuanzhike.top

[Q79] 字符串拼接
来源：http://luw.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uzc.zycfv.cn

[Q80] 字符串截取
来源：http://zmu.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qkn.uphjek.com

[Q81] 字符串替换
来源：http://ale.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qfp.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://ijs.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gbb.daria6918.cn

[Q83] 大小写转换
来源：http://lyd.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nui.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://ejj.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://foy.hcnkem.com

[Q85] 数值取整
来源：http://ijt.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://viz.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://sdc.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cuw.hesvh.cn

[Q87] JSON 字段做条件
来源：http://kfi.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://prh.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://uwf.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yaf.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qek.jinqigufen.top

[Q89] 判断表是否存在
来源：http://coy.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pbk.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://uxv.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dqm.feifeiyinyue.top

================================================================================
来源：http://bdh.bjfxy.top

R. Bash 专题
来源：http://gbg.tianlin.xyz

================================================================================
来源：http://hte.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://yfb.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://wgz.andypj.xyz

set -euo pipefail
来源：http://bfk.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://jgb.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://akj.smart0.xyz

[R03] 只读变量
来源：http://wky.tanke756.top

readonly PI=3.14
来源：http://uvb.hnxiangtu.top

[R04] 位置参数
来源：http://mwz.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zrb.52xcode.cn

[R05] 参数默认值
来源：http://ejs.hongshengwenyu.top

name="${1:-default}"
来源：http://dmp.fehbvm.com

[R06] 判断命令是否存在
来源：http://lin.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://axi.xuetiantiany.cn

[R07] if 判断文件
来源：http://fyb.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ubs.xuanzx.com

[R08] 数值比较
来源：http://ztw.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ttn.kuanghao11.cn

[R09] 字符串比较
来源：http://nsh.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jiw.yuanzhike.top

[R10] 正则匹配
来源：http://udb.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rnd.redwolf501.top

[R11] case 多分支
来源：http://mge.birdmap.top

case "$1" in
来源：http://gwm.sysykeji.top

start) echo "启动" ;;
来源：http://ioc.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://tye.tanke756.top

*)     echo "未知命令" ;;
来源：http://jhk.sxryk.cn

esac
来源：http://uac.hnxiangtu.top

[R12] for 遍历文件
来源：http://dft.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://lgh.chenzaomai.com

[R13] for 计数循环
来源：http://ymr.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://gzs.haohaochexian.top

[R14] C 风格 for
来源：http://dry.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://shc.redwolf501.top

[R15] while 逐行读文件
来源：http://bat.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://alm.sxryk.cn

[R16] until 等待条件
来源：http://oih.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://umm.sufxvd.cn

[R17] 数组定义与取值
来源：http://zov.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://sgz.cdnleiting.top

[R18] 遍历数组
来源：http://yos.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qup.sxryk.cn

[R19] 数组长度
来源：http://wza.daxiang520.top

echo "${#arr[@]}"
来源：http://mso.daria6918.cn

[R20] 关联数组（字典）
来源：http://zjg.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wlj.gaohongyu789.top

[R21] 字符串长度
来源：http://hfp.tarul.cn

echo "${#s}"
来源：http://ypv.vqdsnc.cn

[R22] 截取子串
来源：http://ayu.yj20258888.top

echo "${s:0:5}"
来源：http://rsr.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://khx.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://guu.smart0.xyz

[R24] 大小写转换
来源：http://sph.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lac.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://ebm.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://esm.dianchejie.cn

[R26] 命令替换
来源：http://csb.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://kpq.yangfankeji.com

[R27] 算术展开
来源：http://ibh.pycfn.com

echo $((1 + 2 * 3))
来源：http://heh.redwolf501.top

[R28] 浮点运算
来源：http://fdd.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://qok.dianchejie.cn

[R29] 定义函数
来源：http://mmv.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sqc.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://nik.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://cuf.shuidangran.top

[R31] 局部变量
来源：http://vyj.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://ssu.chenzaomai.com

[R32] 参数个数校验
来源：http://pma.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zid.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://fnc.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kpm.zycfv.cn

[R34] 退出时清理
来源：http://ijr.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mty.mhx1999.top

[R35] 后台执行并等待
来源：http://uoi.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nek.yueranfly.top

[R36] 并发执行多个任务
来源：http://mfy.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pac.daxiang520.top

[R37] 把输出赋给变量
来源：http://ker.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://aqw.yonumen.top

[R38] 管道串联
来源：http://lzw.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://tru.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://vnb.jiagoushi.top


<!-- 参考信息 -->