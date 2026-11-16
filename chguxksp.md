代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ihz.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nnh.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kel.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pex.ydzc1.top

================================================================================
来源：http://vil.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wzl.xziqi.cn

================================================================================
来源：http://rlv.hesvh.cn

[Q01] 创建表
来源：http://fxh.jyoumei.cn

CREATE TABLE users (
来源：http://mir.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qco.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://sah.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://obi.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eqo.xingfuxueyuan.xyz

);
来源：http://xrj.hnqzz.top

[Q02] 创建带外键的表
来源：http://rsu.meibo888.top

CREATE TABLE orders (
来源：http://jud.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gch.guowangkeji.top

user_id INT NOT NULL,
来源：http://ets.iojbl.cn

amount DECIMAL(10, 2),
来源：http://ohj.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bxh.yj202588.top

);
来源：http://mgi.shuidangran.top

[Q03] 增加列
来源：http://pxw.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bfl.sxryk.cn

[Q04] 修改列类型
来源：http://ovz.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://asq.nanxinkj.top

[Q05] 重命名列
来源：http://yfq.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cad.bjfxy.top

[Q06] 删除列
来源：http://icn.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eyg.ydzc1.top

[Q07] 删除表
来源：http://zzy.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://vht.jianghu66.top

[Q08] 创建普通索引
来源：http://mif.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://zap.xylfe.cn

[Q09] 创建唯一索引
来源：http://fgl.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tee.0kj1m.cn

[Q10] 插入单行
来源：http://mqm.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nfl.9152youxi.cn

[Q11] 一次插入多行
来源：http://eoj.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sio.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://onn.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kxs.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sav.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://gyj.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lbx.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://kka.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ahq.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fcr.yonumen.top

[Q15] 查询全部
来源：http://xdr.ivvv.top

SELECT * FROM users;
来源：http://dyr.fktsv.cn

[Q16] 查询指定列
来源：http://sfs.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://zvj.jianghu66.top

[Q17] 条件查询
来源：http://ycn.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eky.ydzc1.top

[Q18] 模糊匹配
来源：http://ucd.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cmn.xuanzx.com

[Q19] 范围查询
来源：http://qhv.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hbb.wangshuangyany.cn

[Q20] IN 列表
来源：http://krv.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://utq.zycfv.cn

[Q21] 空值判断
来源：http://jzb.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hyu.sweek.top

[Q22] 排序
来源：http://lyl.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xum.dianchejie.cn

[Q23] 分页
来源：http://pzp.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ify.yanxiufei.cn

[Q24] 去重
来源：http://dqu.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://bec.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://slw.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fxp.yj202588.top

[Q26] 计数
来源：http://fqu.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://jkq.jinqigufen.top

[Q27] 条件计数
来源：http://emn.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hzf.ydjk.org.cn

[Q28] 求和与平均
来源：http://jbg.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lah.yuxming.cn

[Q29] 最大最小值
来源：http://tuu.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lph.52xcode.cn

[Q30] 分组统计
来源：http://ymz.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dve.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://lwk.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oih.smart0.xyz

[Q32] 分组拼接字符串
来源：http://zrd.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zte.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://skd.chenzaomai.com

[Q33] 多列分组
来源：http://mqb.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oln.shzxlz.cn

[Q34] 每组取第一条
来源：http://yxw.jlsjyb.cn

SELECT * FROM (
来源：http://jac.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://etd.shzxlz.cn

) t WHERE rn = 1;
来源：http://bgd.ywan-chungtsiang.top

[Q35] 内连接
来源：http://ndr.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nzt.yuxming.cn

[Q36] 左连接
来源：http://laa.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lmf.yueranfly.top

[Q37] 右连接
来源：http://fsn.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ewo.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://een.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ysy.yj202588.top

[Q39] 自连接（查上下级）
来源：http://wvi.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tjs.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vci.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://grl.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jnb.nanxuanxn.top

[Q41] 多表连接
来源：http://xfg.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cwt.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://dxy.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://ioe.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://lrw.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://bcn.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mfu.andypj.xyz

[Q43] 标量子查询
来源：http://rvv.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ayi.cdnleiting.top

[Q44] IN 子查询
来源：http://sfj.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftg.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://qem.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cny.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mzc.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wrm.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://qqd.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gim.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://kxk.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmv.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://yvo.jyoumei.cn

[Q49] 更新单行
来源：http://lvw.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pgp.yuxming.cn

[Q50] 批量更新
来源：http://vhp.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jfz.hysaishi.cn

[Q51] 用子查询更新
来源：http://cyi.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rry.jinqigufen.top

[Q52] 删除指定行
来源：http://xyd.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://exd.sjlbkw.cn

[Q53] 按条件删除
来源：http://eai.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xab.fktsv.cn

[Q54] 清空表
来源：http://adw.cheryme.top

TRUNCATE TABLE logs;
来源：http://bvh.yueranfly.top

[Q55] 排名（并列占位）
来源：http://scg.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bkb.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://sen.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jyj.bjfxy.top

[Q57] 行号
来源：http://zhj.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hyl.chenjidiqi.icu

[Q58] 累计求和
来源：http://oou.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ppd.daria6918.cn

[Q59] 分组内累计
来源：http://hsj.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xzq.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://nwm.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jcr.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rlk.kuanghao11.cn

[Q61] 移动平均
来源：http://xyh.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uxw.jiagoushi.top

[Q62] 分组占比
来源：http://knv.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yqm.fengsongda.top

[Q63] 开启事务
来源：http://win.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://gst.smart0.xyz

[Q64] 提交事务
来源：http://wcp.sjlbkw.cn

COMMIT;
来源：http://oyy.zhiwuduotai.top

[Q65] 回滚事务
来源：http://lho.gzhubu.top

ROLLBACK;
来源：http://eey.316326.xyz

[Q66] 行锁查询
来源：http://ykm.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xhb.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://afq.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://umt.haohaochexian.top

[Q68] 保存点
来源：http://zwn.cashguo.top

SAVEPOINT sp1;
来源：http://ccu.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://bzf.tianlin.xyz

[Q69] 查看执行计划
来源：http://juz.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://spj.ctjpmb.com

[Q70] 更新统计信息
来源：http://gnw.yueranfly.top

ANALYZE TABLE users;
来源：http://ajn.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://xii.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ecz.xuanzx.com

[Q72] 查看索引
来源：http://lgp.cdnleiting.top

SHOW INDEX FROM users;
来源：http://vsi.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://ohc.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pnj.sjlbkw.cn

[Q74] 强制使用索引
来源：http://kfi.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sym.shuidangran.top

[Q75] 日期格式化
来源：http://aoe.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zih.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cnq.shzxlz.cn

[Q76] 按天统计
来源：http://lww.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rdx.cucudq.cn

[Q77] 时间加减
来源：http://uww.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jpw.cqqwz.cn

[Q78] 当前时间
来源：http://eny.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rkk.zycfv.cn

[Q79] 字符串拼接
来源：http://bxl.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mvu.zhijiandao.cn

[Q80] 字符串截取
来源：http://pvd.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xow.yfazqb.com

[Q81] 字符串替换
来源：http://grf.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://naj.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://tkd.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rjl.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://ruj.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pgp.cheryme.top

[Q84] 去除首尾空格
来源：http://qdx.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://iug.havefunace.top

[Q85] 数值取整
来源：http://xaw.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qfc.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://jtk.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ukh.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://lrq.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tyt.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://sfv.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zok.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dnw.yj20258.top

[Q89] 判断表是否存在
来源：http://fxr.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ptz.nanxuanxn.top

[Q90] 生成序号列
来源：http://rpn.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ftg.cqqwz.cn

================================================================================
来源：http://krm.yuanzhike.top

R. Bash 专题
来源：http://dlg.tian-w.cn

================================================================================
来源：http://vdv.uphjek.com

[R01] shebang 与严格模式
来源：http://kvq.xylfe.cn

#!/usr/bin/env bash
来源：http://wgu.cashguo.top

set -euo pipefail
来源：http://eep.snrcjt.cn

[R02] 变量赋值与使用
来源：http://kvq.guannengcc.top

name="Tom"; echo "$name"
来源：http://ntd.yvedp.cn

[R03] 只读变量
来源：http://tdr.shuidangran.top

readonly PI=3.14
来源：http://fie.zhixingplan.top

[R04] 位置参数
来源：http://xnb.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aod.shanyushiyangtech.top

[R05] 参数默认值
来源：http://ofj.xuanzx.com

name="${1:-default}"
来源：http://cci.yueranfly.top

[R06] 判断命令是否存在
来源：http://ixo.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qls.dianchejie.cn

[R07] if 判断文件
来源：http://wah.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cdq.yanxiufei.cn

[R08] 数值比较
来源：http://zib.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oro.cqqwz.cn

[R09] 字符串比较
来源：http://vif.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ylm.zhoulong.xyz

[R10] 正则匹配
来源：http://otw.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://efl.cashguo.top

[R11] case 多分支
来源：http://god.wangdashe.top

case "$1" in
来源：http://sac.chenjidiqi.icu

start) echo "启动" ;;
来源：http://biq.zhixingplan.top

stop)  echo "停止" ;;
来源：http://hni.havefunace.top

*)     echo "未知命令" ;;
来源：http://nzf.mhx1999.top

esac
来源：http://mgd.jianghu66.top

[R12] for 遍历文件
来源：http://dlp.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://pqr.xuetiantiany.cn

[R13] for 计数循环
来源：http://zge.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://nlt.fengsongda.top

[R14] C 风格 for
来源：http://qdo.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzk.dianchejie.cn

[R15] while 逐行读文件
来源：http://say.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oks.shuidangran.top

[R16] until 等待条件
来源：http://dvu.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hiu.andypj.xyz

[R17] 数组定义与取值
来源：http://yqm.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://nzk.guowangkeji.top

[R18] 遍历数组
来源：http://jlu.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mey.zhengqikj.top

[R19] 数组长度
来源：http://ocp.dashuyun.cn

echo "${#arr[@]}"
来源：http://nza.sweek.top

[R20] 关联数组（字典）
来源：http://emf.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zaw.zhengqikj.top

[R21] 字符串长度
来源：http://yns.zhoulong.xyz

echo "${#s}"
来源：http://icz.tarul.cn

[R22] 截取子串
来源：http://uvf.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://ewr.tianlin.xyz

[R23] 字符串替换
来源：http://ebq.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkg.pycfn.com

[R24] 大小写转换
来源：http://squ.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://naf.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://uzf.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bnv.yueranfly.top

[R26] 命令替换
来源：http://ckm.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://dch.ivvv.top

[R27] 算术展开
来源：http://hpu.yj20258888.top

echo $((1 + 2 * 3))
来源：http://mqy.xuanzx.com

[R28] 浮点运算
来源：http://aac.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://iwx.zdbjq.cn

[R29] 定义函数
来源：http://fsy.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdk.cashguo.top

[R30] 函数返回状态码
来源：http://djj.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://hjg.tarul.cn

[R31] 局部变量
来源：http://dmj.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://xks.fktsv.cn

[R32] 参数个数校验
来源：http://ljj.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://izl.yj20258.top

[R33] 捕获错误并提示行号
来源：http://guy.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://huq.yj20258888.top

[R34] 退出时清理
来源：http://vfq.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://eqo.quarkkingdee.top

[R35] 后台执行并等待
来源：http://lzo.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wht.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://ndm.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vba.cucudq.cn

[R37] 把输出赋给变量
来源：http://jwd.chenlongwang.top

files=$(ls -1)
来源：http://atn.andypj.xyz

[R38] 管道串联
来源：http://ytz.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://dfq.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://ywr.cheryme.top

cmd > out.log 2>&1
来源：http://yig.havefunace.top

[R40] 追加写日志
来源：http://zhj.uphjek.com

echo "log" >> out.log
来源：http://gfk.bjfxy.top

[R41] 丢弃输出
来源：http://jkb.cqqwz.cn


<!-- 参考信息 -->