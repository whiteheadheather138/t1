代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ztm.shangyingyoupin.top

);
来源：http://sge.jiagoushi.top

[Q02] 创建带外键的表
来源：http://hif.jinqigfzy.top

CREATE TABLE orders (
来源：http://pke.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aus.fzhhl.top

user_id INT NOT NULL,
来源：http://mau.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://egt.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vdv.zhoulong.xyz

);
来源：http://swp.tianlin.xyz

[Q03] 增加列
来源：http://pcb.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gpb.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://onb.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rvr.shanyushiyangtech.top

[Q05] 重命名列
来源：http://xgn.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://afa.fktsv.cn

[Q06] 删除列
来源：http://ehe.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://yhn.cheryme.top

[Q07] 删除表
来源：http://oec.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://zcj.zhijiandao.cn

[Q08] 创建普通索引
来源：http://ztx.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rpl.cqqwz.cn

[Q09] 创建唯一索引
来源：http://kiy.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nma.yfazqb.com

[Q10] 插入单行
来源：http://fkh.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qsx.yj202588.top

[Q11] 一次插入多行
来源：http://cze.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jcy.yongpay.top

[Q12] 插入后取自增 ID
来源：http://tkl.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://paf.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ych.snrcjt.cn

[Q13] 忽略重复插入
来源：http://kxe.sweek.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ost.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://qkc.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bjp.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zuo.shzxlz.cn

[Q15] 查询全部
来源：http://gpi.shzxlz.cn

SELECT * FROM users;
来源：http://oqj.nwbrower.top

[Q16] 查询指定列
来源：http://oef.sufxvd.cn

SELECT id, name FROM users;
来源：http://eup.jiagoushi.top

[Q17] 条件查询
来源：http://kio.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nts.xinyue.icu

[Q18] 模糊匹配
来源：http://jww.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ltq.kuanghao11.cn

[Q19] 范围查询
来源：http://gfi.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nvw.yj20258.top

[Q20] IN 列表
来源：http://duv.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mqh.havefunace.top

[Q21] 空值判断
来源：http://esn.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ozb.gogol.net.cn

[Q22] 排序
来源：http://gcp.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qqb.0kj1m.cn

[Q23] 分页
来源：http://znu.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sfc.jinghuilouyu.cn

[Q24] 去重
来源：http://aso.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://ijx.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://hgf.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mcf.yj20258.top

[Q26] 计数
来源：http://kbm.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://vel.yuanzhike.top

[Q27] 条件计数
来源：http://tfy.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aqq.redwolf501.top

[Q28] 求和与平均
来源：http://tvl.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://trc.xylfe.cn

[Q29] 最大最小值
来源：http://ejd.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bea.zdbjq.cn

[Q30] 分组统计
来源：http://lug.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jhu.sysykeji.top

[Q31] 分组后过滤
来源：http://lcd.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lgb.cucudq.cn

[Q32] 分组拼接字符串
来源：http://zbq.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tnr.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wlb.zhiwuduotai.top

[Q33] 多列分组
来源：http://vka.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jzx.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://fnd.jiagoushi.top

SELECT * FROM (
来源：http://sfd.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymg.chenzaomai.com

) t WHERE rn = 1;
来源：http://gxm.hammf.cn

[Q35] 内连接
来源：http://utw.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uwn.fzhhl.top

[Q36] 左连接
来源：http://fdw.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tdq.jqgufenzy.top

[Q37] 右连接
来源：http://dkn.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://szn.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://wrl.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vvj.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://ylb.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hwk.xingfuxueyuan.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ynq.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://qea.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rkj.svipenyu.cn

[Q41] 多表连接
来源：http://wyx.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yew.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://rzv.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://tfy.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://bjj.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://kge.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zcd.zhengqikj.top

[Q43] 标量子查询
来源：http://wwp.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zme.redwolf501.top

[Q44] IN 子查询
来源：http://tib.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nma.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://yxc.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yoq.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://slo.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgg.dianchejie.cn

[Q47] 与平均值比较
来源：http://yuz.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jgr.cheryme.top

[Q48] CTE 公用表表达式
来源：http://rok.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jdl.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hha.sjlbkw.cn

[Q49] 更新单行
来源：http://auj.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://anp.meibo888.top

[Q50] 批量更新
来源：http://gxk.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wuo.zhoulong.xyz

[Q51] 用子查询更新
来源：http://zvz.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kxh.cucudq.cn

[Q52] 删除指定行
来源：http://ama.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://uis.tian-w.cn

[Q53] 按条件删除
来源：http://mvu.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ecn.zhixingplan.top

[Q54] 清空表
来源：http://ezf.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://cfk.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://swd.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lcq.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://uff.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vqy.chenlongwang.top

[Q57] 行号
来源：http://dnd.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xtz.shangyingyoupin.top

[Q58] 累计求和
来源：http://tyg.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dfs.zycfv.cn

[Q59] 分组内累计
来源：http://gev.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mkh.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://zpf.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bxz.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hzx.haohaochexian.top

[Q61] 移动平均
来源：http://yfv.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xlk.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://wbu.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://saj.shzxlz.cn

[Q63] 开启事务
来源：http://cki.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://agu.birdmap.top

[Q64] 提交事务
来源：http://cbl.xylfe.cn

COMMIT;
来源：http://kss.sjlbkw.cn

[Q65] 回滚事务
来源：http://tkk.havefunace.top

ROLLBACK;
来源：http://rec.yuanzhike.top

[Q66] 行锁查询
来源：http://qcp.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rjp.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://kur.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bdw.zhaomingkeji.xyz

[Q68] 保存点
来源：http://zcq.tian-w.cn

SAVEPOINT sp1;
来源：http://ayf.ctjpmb.com

ROLLBACK TO sp1;
来源：http://ksp.jinqigufen.top

[Q69] 查看执行计划
来源：http://nfx.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rwh.yongpay.top

[Q70] 更新统计信息
来源：http://rgw.fehbvm.com

ANALYZE TABLE users;
来源：http://xrl.cdnleiting.top

[Q71] 查看建表语句
来源：http://eqg.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://czp.wangdashe.top

[Q72] 查看索引
来源：http://lgz.yongpay.top

SHOW INDEX FROM users;
来源：http://cyh.bbcook.cn

[Q73] 查看表状态
来源：http://sgd.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dst.tianlin.xyz

[Q74] 强制使用索引
来源：http://zyv.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aht.cucudq.cn

[Q75] 日期格式化
来源：http://pvb.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aoa.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vwh.wangdashe.top

[Q76] 按天统计
来源：http://hou.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ipr.sjlbkw.cn

[Q77] 时间加减
来源：http://wuc.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ivb.kuanghao11.cn

[Q78] 当前时间
来源：http://xao.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://chg.birdmap.top

[Q79] 字符串拼接
来源：http://uat.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qxs.52xcode.cn

[Q80] 字符串截取
来源：http://kpt.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ish.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://ing.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sjg.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://xzy.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://paw.hywenlv.cn

[Q83] 大小写转换
来源：http://xbl.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nfx.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://ige.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://zeo.sxryk.cn

[Q85] 数值取整
来源：http://jve.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://svv.uphjek.com

[Q86] 读取 JSON 字段
来源：http://vyk.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kvj.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://efc.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sbo.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://smo.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://psq.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iks.zycfv.cn

[Q89] 判断表是否存在
来源：http://bow.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ngp.jiagoushi.top

[Q90] 生成序号列
来源：http://qww.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xzz.nanxuanxn.top

================================================================================
来源：http://eyg.zhengqikj.top

R. Bash 专题
来源：http://jbq.haohaochexian.top

================================================================================
来源：http://cgx.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://yoc.snrcjt.cn

#!/usr/bin/env bash
来源：http://fie.fehbvm.com

set -euo pipefail
来源：http://bhr.ppjwa.cn

[R02] 变量赋值与使用
来源：http://qqo.hammf.cn

name="Tom"; echo "$name"
来源：http://rrq.hcnkem.com

[R03] 只读变量
来源：http://aiv.316326.xyz

readonly PI=3.14
来源：http://tpo.xziqi.cn

[R04] 位置参数
来源：http://geg.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://juf.zhoulong.xyz

[R05] 参数默认值
来源：http://xfe.yonumen.top

name="${1:-default}"
来源：http://zcc.yvedp.cn

[R06] 判断命令是否存在
来源：http://rov.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jay.vehdjk.com

[R07] if 判断文件
来源：http://ynk.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mkx.yonumen.top

[R08] 数值比较
来源：http://boo.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vbx.wangshuangyany.cn

[R09] 字符串比较
来源：http://aoo.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gje.yongpay.top

[R10] 正则匹配
来源：http://bfv.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gte.0kj1m.cn

[R11] case 多分支
来源：http://hil.tianlin.xyz

case "$1" in
来源：http://srq.mhx1999.top

start) echo "启动" ;;
来源：http://nxc.mhx1999.top

stop)  echo "停止" ;;
来源：http://fez.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://ovj.fehbvm.com

esac
来源：http://zcs.cqqwz.cn

[R12] for 遍历文件
来源：http://lko.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://okt.pengpengdd.cyou

[R13] for 计数循环
来源：http://imq.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://ljt.meibo888.top

[R14] C 风格 for
来源：http://fot.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qcb.0kj1m.cn

[R15] while 逐行读文件
来源：http://dkz.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tlx.jqgufenzy.top

[R16] until 等待条件
来源：http://eeq.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aum.andypj.xyz

[R17] 数组定义与取值
来源：http://egg.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://lqd.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://fho.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://odn.guannengcc.top

[R19] 数组长度
来源：http://ela.ehwqpu.com

echo "${#arr[@]}"
来源：http://zug.9152youxi.cn

[R20] 关联数组（字典）
来源：http://txy.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pvi.sysykeji.top

[R21] 字符串长度
来源：http://stk.jinghuilouyu.cn

echo "${#s}"
来源：http://dtc.yj20258888.top

[R22] 截取子串
来源：http://tpp.daxiang520.top

echo "${s:0:5}"
来源：http://tsb.pycfn.com

[R23] 字符串替换
来源：http://ald.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://shu.zdqjudy.top

[R24] 大小写转换
来源：http://ony.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://dkb.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://tpm.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://brg.iojbl.cn

[R26] 命令替换
来源：http://nwu.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://cns.yonumen.top

[R27] 算术展开
来源：http://uir.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://bmv.cheryme.top

[R28] 浮点运算
来源：http://ums.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://nli.sweek.top

[R29] 定义函数
来源：http://ugh.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gla.fehbvm.com

[R30] 函数返回状态码
来源：http://ihi.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://iez.aibaodan.cn

[R31] 局部变量
来源：http://qrz.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://wou.guowangkeji.top

[R32] 参数个数校验
来源：http://nus.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jcv.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://uhx.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://axp.xziqi.cn

[R34] 退出时清理
来源：http://nws.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://agr.zhijiandao.cn

[R35] 后台执行并等待
来源：http://vfv.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jdf.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://itg.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bky.nanxinkj.top

[R37] 把输出赋给变量
来源：http://ohy.tarul.cn

files=$(ls -1)
来源：http://hpm.yfazqb.com

[R38] 管道串联
来源：http://ksp.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://pdk.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://ckv.hnqzz.top

cmd > out.log 2>&1
来源：http://adb.hfpthk.cn

[R40] 追加写日志
来源：http://fwf.sjlbkw.cn

echo "log" >> out.log
来源：http://msg.bbcook.cn

[R41] 丢弃输出
来源：http://qrq.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://bkf.ppjwa.cn

[R42] 输入重定向
来源：http://gnl.pengpengdd.cyou

wc -l < a.txt
来源：http://rqt.jinqigfzy.top

[R43] 按名字查找文件
来源：http://yhu.andypj.xyz

find . -name "*.log" -type f
来源：http://mxw.sysykeji.top

[R44] 按修改时间查找
来源：http://ooc.zhongyouzk.top

find . -mtime -7 -type f
来源：http://goc.fzhhl.top

[R45] 批量删除
来源：http://ozk.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://fdg.ybcxt.top

[R46] 递归替换文件内容
来源：http://bxb.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rnw.tianlin.xyz

[R47] sed 单行替换
来源：http://xzf.bbcook.cn


<!-- 参考信息 -->