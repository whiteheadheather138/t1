代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cdy.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://osp.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blv.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hmk.cashguo.top

================================================================================
来源：http://tsq.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxi.haohaochexian.top

================================================================================
来源：http://xbf.iojbl.cn

[Q01] 创建表
来源：http://qai.redwolf501.top

CREATE TABLE users (
来源：http://rcn.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkc.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://wrc.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://tmv.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cuk.pengpengdd.cyou

);
来源：http://hwa.jianghu66.top

[Q02] 创建带外键的表
来源：http://bed.yj20258888.top

CREATE TABLE orders (
来源：http://rwn.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gts.ybcxt.top

user_id INT NOT NULL,
来源：http://dlq.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://kqc.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vsf.hesvh.cn

);
来源：http://dgv.vehdjk.com

[Q03] 增加列
来源：http://wvf.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmw.chenjidiqi.icu

[Q04] 修改列类型
来源：http://cyp.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://glj.epnwcf.com

[Q05] 重命名列
来源：http://cgl.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bhp.zhaomingkeji.xyz

[Q06] 删除列
来源：http://zlh.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://rzk.zhaomingkeji.xyz

[Q07] 删除表
来源：http://xan.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://gdl.yfazqb.com

[Q08] 创建普通索引
来源：http://fzj.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://htg.aibaodan.cn

[Q09] 创建唯一索引
来源：http://rzh.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xwj.cheryme.top

[Q10] 插入单行
来源：http://exh.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vmd.yonumen.top

[Q11] 一次插入多行
来源：http://ezw.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tdz.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://fdk.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://dxv.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iep.hysaishi.cn

[Q13] 忽略重复插入
来源：http://ybe.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bqk.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://jkm.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ycs.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://usa.bbcook.cn

[Q15] 查询全部
来源：http://pzd.daxiang520.top

SELECT * FROM users;
来源：http://abi.yongpay.top

[Q16] 查询指定列
来源：http://ovh.xziqi.cn

SELECT id, name FROM users;
来源：http://rwz.chenlongwang.top

[Q17] 条件查询
来源：http://svw.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://net.52xcode.cn

[Q18] 模糊匹配
来源：http://ylr.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sdy.hywenlv.cn

[Q19] 范围查询
来源：http://awf.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bla.hcnkem.com

[Q20] IN 列表
来源：http://vqr.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hin.dashuyun.cn

[Q21] 空值判断
来源：http://sxy.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oog.tian-w.cn

[Q22] 排序
来源：http://dza.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvm.jiagoushi.top

[Q23] 分页
来源：http://bzk.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://edo.gaohongyu789.top

[Q24] 去重
来源：http://acy.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://ceo.tanke756.top

[Q25] 只取前 N 条
来源：http://sst.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://snz.pengpengdd.cyou

[Q26] 计数
来源：http://waj.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://zxz.kuanghao11.cn

[Q27] 条件计数
来源：http://dsg.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cso.jinqigufen.top

[Q28] 求和与平均
来源：http://dch.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oib.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://bnd.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nwr.jianghu66.top

[Q30] 分组统计
来源：http://xby.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kaq.cheryme.top

[Q31] 分组后过滤
来源：http://rop.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://flv.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://dik.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mya.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://szv.snrcjt.cn

[Q33] 多列分组
来源：http://oql.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hys.sxryk.cn

[Q34] 每组取第一条
来源：http://qzi.hfpthk.cn

SELECT * FROM (
来源：http://snu.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://azf.tanke756.top

) t WHERE rn = 1;
来源：http://iuy.zhixingplan.top

[Q35] 内连接
来源：http://hqb.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tui.havefunace.top

[Q36] 左连接
来源：http://ezy.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qbr.iojbl.cn

[Q37] 右连接
来源：http://kzu.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dzp.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://nqu.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://anj.316326.xyz

[Q39] 自连接（查上下级）
来源：http://osm.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://ofz.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yah.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xuv.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vog.xinyue.icu

[Q41] 多表连接
来源：http://zei.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lby.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://xpp.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://bkk.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://vkj.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://gkw.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwb.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://jve.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://utf.wangdashe.top

[Q44] IN 子查询
来源：http://xiq.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nbk.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://nbu.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ptv.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://sfu.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cvm.jyoumei.cn

[Q47] 与平均值比较
来源：http://aza.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mqq.cashguo.top

[Q48] CTE 公用表表达式
来源：http://zvi.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hyj.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://mnm.sufxvd.cn

[Q49] 更新单行
来源：http://wgx.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uut.bjfxy.top

[Q50] 批量更新
来源：http://gxt.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://unc.smart0.xyz

[Q51] 用子查询更新
来源：http://anc.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://epj.gzhubu.top

[Q52] 删除指定行
来源：http://hrr.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://zrn.tianlin.xyz

[Q53] 按条件删除
来源：http://mki.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ust.sxryk.cn

[Q54] 清空表
来源：http://ogn.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://mvb.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://hrt.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ump.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://sag.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rxy.hnxiangtu.top

[Q57] 行号
来源：http://gto.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jve.feifeiyinyue.top

[Q58] 累计求和
来源：http://sra.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://smr.tanke756.top

[Q59] 分组内累计
来源：http://izr.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qrz.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://lvb.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://snu.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nga.hcnkem.com

[Q61] 移动平均
来源：http://zqi.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uio.hongshengwenyu.top

[Q62] 分组占比
来源：http://uhb.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mhe.ctjpmb.com

[Q63] 开启事务
来源：http://rdb.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://vpx.yfazqb.com

[Q64] 提交事务
来源：http://oeh.tianlin.xyz

COMMIT;
来源：http://xnc.zhongyouzk.top

[Q65] 回滚事务
来源：http://gbu.cqqwz.cn

ROLLBACK;
来源：http://gux.kuanghao11.cn

[Q66] 行锁查询
来源：http://omw.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wpn.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://cyc.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jot.jinqigufen.top

[Q68] 保存点
来源：http://jfk.yj20258.top

SAVEPOINT sp1;
来源：http://hzm.jyoumei.cn

ROLLBACK TO sp1;
来源：http://qqj.jyoumei.cn

[Q69] 查看执行计划
来源：http://gvs.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lxv.sysykeji.top

[Q70] 更新统计信息
来源：http://vfk.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://njk.vqdsnc.cn

[Q71] 查看建表语句
来源：http://lhf.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qkd.pengpengdd.cyou

[Q72] 查看索引
来源：http://yrr.redwolf501.top

SHOW INDEX FROM users;
来源：http://tcd.cdnleiting.top

[Q73] 查看表状态
来源：http://laz.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vmc.yj20258.top

[Q74] 强制使用索引
来源：http://szh.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ljz.chenlongwang.top

[Q75] 日期格式化
来源：http://men.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yhu.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wrr.xinyue.icu

[Q76] 按天统计
来源：http://plf.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fcr.yueranfly.top

[Q77] 时间加减
来源：http://syc.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nrz.yj202588.top

[Q78] 当前时间
来源：http://vbf.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wug.jiagoushi.top

[Q79] 字符串拼接
来源：http://wry.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xmz.bbcook.cn

[Q80] 字符串截取
来源：http://iwd.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wac.andypj.xyz

[Q81] 字符串替换
来源：http://yxp.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qah.ivvv.top

[Q82] 字符长度与字节长度
来源：http://thr.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fxq.chenzaomai.com

[Q83] 大小写转换
来源：http://pfn.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://slh.bbcook.cn

[Q84] 去除首尾空格
来源：http://rlt.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://hov.yonumen.top

[Q85] 数值取整
来源：http://fgy.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qbr.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://jeh.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gfj.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://foz.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jwj.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://ell.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jab.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lpa.yj20258.top

[Q89] 判断表是否存在
来源：http://wla.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jdt.hywenlv.cn

[Q90] 生成序号列
来源：http://fjk.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uxz.tianlin.xyz

================================================================================
来源：http://fue.gzhubu.top

R. Bash 专题
来源：http://ekv.zhongyouzk.top

================================================================================
来源：http://nmk.tianlin.xyz

[R01] shebang 与严格模式
来源：http://zig.52xcode.cn

#!/usr/bin/env bash
来源：http://hde.cqqwz.cn

set -euo pipefail
来源：http://mdy.ehwqpu.com

[R02] 变量赋值与使用
来源：http://nnn.dianchejie.cn

name="Tom"; echo "$name"
来源：http://xxt.vehdjk.com

[R03] 只读变量
来源：http://tuk.mhx1999.top

readonly PI=3.14
来源：http://fpj.bjfxy.top

[R04] 位置参数
来源：http://vbr.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xpn.fengsongda.top

[R05] 参数默认值
来源：http://ttu.kuanghao11.cn

name="${1:-default}"
来源：http://evw.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://tkg.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://okr.iojbl.cn

[R07] if 判断文件
来源：http://ufb.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zbh.hysaishi.cn

[R08] 数值比较
来源：http://uds.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qxa.zhijiandao.cn

[R09] 字符串比较
来源：http://prk.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iba.jyoumei.cn

[R10] 正则匹配
来源：http://rzl.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tmo.zhongyouzk.top

[R11] case 多分支
来源：http://ben.sweek.top

case "$1" in
来源：http://art.gogol.net.cn

start) echo "启动" ;;
来源：http://yce.jiagoushi.top

stop)  echo "停止" ;;
来源：http://pte.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://eyx.guowangkeji.top

esac
来源：http://phc.birdmap.top

[R12] for 遍历文件
来源：http://oac.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://uwi.chenjidiqi.icu

[R13] for 计数循环
来源：http://plq.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://zzk.316326.xyz

[R14] C 风格 for
来源：http://tih.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dcq.nanxinkj.top

[R15] while 逐行读文件
来源：http://qpo.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fke.svipenyu.cn

[R16] until 等待条件
来源：http://zyg.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qkv.dashuyun.cn

[R17] 数组定义与取值
来源：http://emf.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wpq.ydzc1.top

[R18] 遍历数组
来源：http://tzo.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ubl.yongpay.top

[R19] 数组长度
来源：http://lpe.jianghu66.top

echo "${#arr[@]}"
来源：http://guo.cucudq.cn

[R20] 关联数组（字典）
来源：http://jng.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ysb.snrcjt.cn

[R21] 字符串长度
来源：http://biu.cheryme.top

echo "${#s}"
来源：http://eyq.shanyushiyangtech.top

[R22] 截取子串
来源：http://heb.zdbjq.cn

echo "${s:0:5}"
来源：http://mxp.zhixingplan.top

[R23] 字符串替换
来源：http://axn.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nge.pengpengdd.cyou

[R24] 大小写转换
来源：http://oir.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://dao.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://cxl.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivj.sufxvd.cn

[R26] 命令替换
来源：http://lnq.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://nxv.shangyingyoupin.top

[R27] 算术展开
来源：http://ayv.yueranfly.top

echo $((1 + 2 * 3))
来源：http://kdm.jinqigfzy.top

[R28] 浮点运算
来源：http://iwv.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://ggu.ctjpmb.com

[R29] 定义函数
来源：http://eyc.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ljk.wangdashe.top

[R30] 函数返回状态码
来源：http://uhk.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://ast.ywan-chungtsiang.top

[R31] 局部变量
来源：http://pnp.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://cec.svipenyu.cn

[R32] 参数个数校验
来源：http://kpl.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hds.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://zpn.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uiq.sjlbkw.cn

[R34] 退出时清理
来源：http://cpb.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cyk.chenlongwang.top

[R35] 后台执行并等待
来源：http://spc.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bzs.hfpthk.cn

[R36] 并发执行多个任务
来源：http://ric.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://adn.nanxinkj.top

[R37] 把输出赋给变量
来源：http://pua.haohaochexian.top

files=$(ls -1)
来源：http://ibo.bbcook.cn

[R38] 管道串联
来源：http://dqi.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://tlb.birdmap.top

[R39] 重定向标准输出与错误
来源：http://hww.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://ify.jyoumei.cn

[R40] 追加写日志
来源：http://rkp.dianchejie.cn

echo "log" >> out.log
来源：http://pdi.gaohongyu789.top

[R41] 丢弃输出
来源：http://uso.ehwqpu.com


<!-- 参考信息 -->