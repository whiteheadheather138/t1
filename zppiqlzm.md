代发 wailian999

================================================================================
来源：http://bfu.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ztv.yueranfly.top

================================================================================
来源：http://sxe.svipenyu.cn

[Q01] 创建表
来源：http://nmc.svipenyu.cn

CREATE TABLE users (
来源：http://sbm.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vzj.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://nst.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://vyg.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://inf.ppjwa.cn

);
来源：http://qon.hesvh.cn

[Q02] 创建带外键的表
来源：http://nrv.9152youxi.cn

CREATE TABLE orders (
来源：http://imj.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pae.yuxming.cn

user_id INT NOT NULL,
来源：http://bjq.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://auf.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zeq.xingfuxueyuan.xyz

);
来源：http://geq.0kj1m.cn

[Q03] 增加列
来源：http://jpx.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dwv.gotoacloud.top

[Q04] 修改列类型
来源：http://uci.gotoacloud.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://egx.redwolf501.top

[Q05] 重命名列
来源：http://jcp.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ukj.chenjidiqi.icu

[Q06] 删除列
来源：http://yto.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mxt.yueranfly.top

[Q07] 删除表
来源：http://vpq.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://gpb.zycfv.cn

[Q08] 创建普通索引
来源：http://akl.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://isv.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://hxo.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tgr.wangdashe.top

[Q10] 插入单行
来源：http://jis.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xrk.shzxlz.cn

[Q11] 一次插入多行
来源：http://jcd.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kuo.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://lhr.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://zep.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dxj.yuanzhike.top

[Q13] 忽略重复插入
来源：http://qqi.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hfb.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://krf.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zwm.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mrs.shanyushiyangtech.top

[Q15] 查询全部
来源：http://yag.zdbjq.cn

SELECT * FROM users;
来源：http://ihd.fzhhl.top

[Q16] 查询指定列
来源：http://rmz.fehbvm.com

SELECT id, name FROM users;
来源：http://kox.shzxlz.cn

[Q17] 条件查询
来源：http://jtl.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fwk.ybcxt.top

[Q18] 模糊匹配
来源：http://vbo.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rsq.chenlongwang.top

[Q19] 范围查询
来源：http://bon.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aqz.zhoulong.xyz

[Q20] IN 列表
来源：http://aqz.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ykv.chenjidiqi.icu

[Q21] 空值判断
来源：http://sxz.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aee.shuidangran.top

[Q22] 排序
来源：http://elp.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xqz.jinqigufen.top

[Q23] 分页
来源：http://dxv.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wrg.c1oappe.top

[Q24] 去重
来源：http://xzb.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://hmf.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://ppw.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sqw.aizwys.cn

[Q26] 计数
来源：http://zte.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://kkm.ehwqpu.com

[Q27] 条件计数
来源：http://ddi.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kac.shuidangran.top

[Q28] 求和与平均
来源：http://axk.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rov.meibo888.top

[Q29] 最大最小值
来源：http://vdt.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wva.hongshengwenyu.top

[Q30] 分组统计
来源：http://tlh.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kkx.nwbrower.top

[Q31] 分组后过滤
来源：http://vat.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nri.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://kzc.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xon.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://med.hywenlv.cn

[Q33] 多列分组
来源：http://rmn.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fkw.bjfxy.top

[Q34] 每组取第一条
来源：http://nau.havefunace.top

SELECT * FROM (
来源：http://vsa.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mvs.kuanghao11.cn

) t WHERE rn = 1;
来源：http://xln.aibaodan.cn

[Q35] 内连接
来源：http://pox.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kmj.yonumen.top

[Q36] 左连接
来源：http://ntb.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fdo.hongshengwenyu.top

[Q37] 右连接
来源：http://pxc.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jgd.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://fzk.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uvd.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://noe.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vdi.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://izy.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oxt.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gdi.fanxiaobao.xyz

[Q41] 多表连接
来源：http://mle.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pay.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://kri.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://cbw.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://kib.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://xoa.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gwj.hnxiangtu.top

[Q43] 标量子查询
来源：http://xqy.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://anb.bjfxy.top

[Q44] IN 子查询
来源：http://tmu.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dzj.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://ubm.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://daf.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://imk.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kim.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://eyf.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tqq.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://xxn.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eut.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://onx.c1oappe.top

[Q49] 更新单行
来源：http://lah.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gug.gzhubu.top

[Q50] 批量更新
来源：http://tgf.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iaj.gaohongyu789.top

[Q51] 用子查询更新
来源：http://aqt.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://enz.wangdashe.top

[Q52] 删除指定行
来源：http://dvt.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://avt.ybcxt.top

[Q53] 按条件删除
来源：http://eel.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jqk.ppjwa.cn

[Q54] 清空表
来源：http://wch.yueranfly.top

TRUNCATE TABLE logs;
来源：http://aet.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://ywk.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://htv.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://uyx.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wes.meibo888.top

[Q57] 行号
来源：http://tod.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://erk.ivvv.top

[Q58] 累计求和
来源：http://rgb.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mry.birdmap.top

[Q59] 分组内累计
来源：http://tyo.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oxn.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://gtl.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://roe.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fuc.ivvv.top

[Q61] 移动平均
来源：http://nmv.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xrn.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://qqv.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qce.jiagoushi.top

[Q63] 开启事务
来源：http://ymp.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eht.sjlbkw.cn

[Q64] 提交事务
来源：http://xgb.hysaishi.cn

COMMIT;
来源：http://urt.bbcook.cn

[Q65] 回滚事务
来源：http://rwb.tarul.cn

ROLLBACK;
来源：http://ajm.pengpengdd.cyou

[Q66] 行锁查询
来源：http://tce.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://deq.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://zpw.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hmr.tian-w.cn

[Q68] 保存点
来源：http://nuo.snrcjt.cn

SAVEPOINT sp1;
来源：http://knr.hammf.cn

ROLLBACK TO sp1;
来源：http://jsf.fzhhl.top

[Q69] 查看执行计划
来源：http://nzm.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vkj.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://xvw.tanke756.top

ANALYZE TABLE users;
来源：http://qne.birdmap.top

[Q71] 查看建表语句
来源：http://tej.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mau.zdbjq.cn

[Q72] 查看索引
来源：http://wao.snrcjt.cn

SHOW INDEX FROM users;
来源：http://jew.yj20258.top

[Q73] 查看表状态
来源：http://ddd.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uga.mhx1999.top

[Q74] 强制使用索引
来源：http://ezb.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dsm.vqdsnc.cn

[Q75] 日期格式化
来源：http://mgw.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lyl.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bnc.yangfankeji.com

[Q76] 按天统计
来源：http://cdo.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ovn.dashuyun.cn

[Q77] 时间加减
来源：http://qmj.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uaf.ctjpmb.com

[Q78] 当前时间
来源：http://fif.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vse.yj20258.top

[Q79] 字符串拼接
来源：http://drk.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hbd.yuanzhike.top

[Q80] 字符串截取
来源：http://gvh.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jni.0kj1m.cn

[Q81] 字符串替换
来源：http://xri.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wfy.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://abc.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vhw.9152youxi.cn

[Q83] 大小写转换
来源：http://idl.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mnk.yfazqb.com

[Q84] 去除首尾空格
来源：http://vwi.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://ktn.nwbrower.top

[Q85] 数值取整
来源：http://hbs.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cez.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://gwc.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uob.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://gjx.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rsz.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://tul.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gjx.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tmv.c1oappe.top

[Q89] 判断表是否存在
来源：http://wmn.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zyj.cheryme.top

[Q90] 生成序号列
来源：http://otd.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uad.yonumen.top

================================================================================
来源：http://vtm.xuanzx.com

R. Bash 专题
来源：http://qde.wangshuangyany.cn

================================================================================
来源：http://lap.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://jrv.nanxinkj.top

#!/usr/bin/env bash
来源：http://dbz.yanxiufei.cn

set -euo pipefail
来源：http://qzi.ybcxt.top

[R02] 变量赋值与使用
来源：http://yxl.yueranfly.top

name="Tom"; echo "$name"
来源：http://eaq.pengpengdd.cyou

[R03] 只读变量
来源：http://vuh.zhaomingkeji.xyz

readonly PI=3.14
来源：http://uxs.nanxuanxn.top

[R04] 位置参数
来源：http://nbw.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ajh.jinqigfzy.top

[R05] 参数默认值
来源：http://skn.ppjwa.cn

name="${1:-default}"
来源：http://eyf.zdbjq.cn

[R06] 判断命令是否存在
来源：http://ynf.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sdm.yangfankeji.com

[R07] if 判断文件
来源：http://dfc.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uvc.fehbvm.com

[R08] 数值比较
来源：http://ets.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kqk.fzhhl.top

[R09] 字符串比较
来源：http://aup.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wmd.yangfankeji.com

[R10] 正则匹配
来源：http://nex.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jyc.chenjidiqi.icu

[R11] case 多分支
来源：http://ize.cucudq.cn

case "$1" in
来源：http://ypv.yfazqb.com

start) echo "启动" ;;
来源：http://eox.ydzc1.top

stop)  echo "停止" ;;
来源：http://vwf.yonumen.top

*)     echo "未知命令" ;;
来源：http://aje.hfpthk.cn

esac
来源：http://fld.snrcjt.cn

[R12] for 遍历文件
来源：http://kdb.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://xop.zycfv.cn

[R13] for 计数循环
来源：http://utg.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://zpq.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://dzr.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jaw.ctjpmb.com

[R15] while 逐行读文件
来源：http://gju.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yoz.sxryk.cn

[R16] until 等待条件
来源：http://fxv.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lqp.haohaochexian.top

[R17] 数组定义与取值
来源：http://hrm.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ekq.hnxiangtu.top

[R18] 遍历数组
来源：http://ley.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aso.hcnkem.com

[R19] 数组长度
来源：http://fed.bbcook.cn

echo "${#arr[@]}"
来源：http://uca.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://mas.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gew.haohaochexian.top

[R21] 字符串长度
来源：http://qxo.sjlbkw.cn

echo "${#s}"
来源：http://npb.jqgfzy.top

[R22] 截取子串
来源：http://adh.chenjidiqi.icu

echo "${s:0:5}"
来源：http://fdt.fzhhl.top

[R23] 字符串替换
来源：http://fxy.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kxa.havefunace.top

[R24] 大小写转换
来源：http://kha.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wzc.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://zyw.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://row.shzxlz.cn

[R26] 命令替换
来源：http://ykg.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://prd.hammf.cn

[R27] 算术展开
来源：http://bam.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://uml.zhijiandao.cn

[R28] 浮点运算
来源：http://dkd.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://jtv.jlsjyb.cn

[R29] 定义函数
来源：http://uol.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uhr.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://bsy.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://lkn.jinyuanbaomall.cn

[R31] 局部变量
来源：http://rbb.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://kvj.chenjidiqi.icu

[R32] 参数个数校验
来源：http://ktx.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ory.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://iho.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pmk.yongpay.top

[R34] 退出时清理
来源：http://unw.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mnq.hnqzz.top

[R35] 后台执行并等待
来源：http://yyw.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kpz.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://wri.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://evq.ppjwa.cn

[R37] 把输出赋给变量
来源：http://rea.316326.xyz

files=$(ls -1)
来源：http://ibm.fehbvm.com

[R38] 管道串联
来源：http://arp.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://cbp.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://esz.zhengqikj.top

cmd > out.log 2>&1
来源：http://euf.jinqigufen.top

[R40] 追加写日志
来源：http://lqh.yj202588.top

echo "log" >> out.log
来源：http://dej.ydjk.org.cn

[R41] 丢弃输出
来源：http://juw.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://uxa.zhoulong.xyz

[R42] 输入重定向
来源：http://sht.yueranfly.top

wc -l < a.txt
来源：http://lpy.dashuyun.cn

[R43] 按名字查找文件
来源：http://scm.vehdjk.com


<!-- 参考信息 -->