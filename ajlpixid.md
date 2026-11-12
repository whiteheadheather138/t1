代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qfg.smart0.xyz

);
来源：http://ctl.jianghu66.top

[Q02] 创建带外键的表
来源：http://ecf.wangshuangyany.cn

CREATE TABLE orders (
来源：http://rlr.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aup.havefunace.top

user_id INT NOT NULL,
来源：http://uha.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://tbp.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pnn.shuidangran.top

);
来源：http://wqy.shanyushiyangtech.top

[Q03] 增加列
来源：http://gve.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ayw.zdqjudy.top

[Q04] 修改列类型
来源：http://yed.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://trh.yonumen.top

[Q05] 重命名列
来源：http://ebu.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xrz.ydjk.org.cn

[Q06] 删除列
来源：http://dkg.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ghp.hywenlv.cn

[Q07] 删除表
来源：http://buc.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://xbs.ydjk.org.cn

[Q08] 创建普通索引
来源：http://kji.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rqk.birdmap.top

[Q09] 创建唯一索引
来源：http://bem.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nlx.c1oappe.top

[Q10] 插入单行
来源：http://vvb.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ipg.aizwys.cn

[Q11] 一次插入多行
来源：http://qkf.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://akg.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://pwk.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kyv.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hch.jiagoushi.top

[Q13] 忽略重复插入
来源：http://mml.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://man.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://hdo.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zal.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aba.nwbrower.top

[Q15] 查询全部
来源：http://jam.hnxiangtu.top

SELECT * FROM users;
来源：http://cbz.ydzc1.top

[Q16] 查询指定列
来源：http://npi.meibo888.top

SELECT id, name FROM users;
来源：http://foq.cqqwz.cn

[Q17] 条件查询
来源：http://gsj.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rhx.yuxming.cn

[Q18] 模糊匹配
来源：http://ltu.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wkc.zhoulong.xyz

[Q19] 范围查询
来源：http://dnk.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pmr.dianchejie.cn

[Q20] IN 列表
来源：http://bwz.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ndv.yonumen.top

[Q21] 空值判断
来源：http://oqg.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://jsl.jqgufenzy.top

[Q22] 排序
来源：http://eiy.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kyw.hnqzz.top

[Q23] 分页
来源：http://lzq.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvb.feifeiyinyue.top

[Q24] 去重
来源：http://ruc.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://cnx.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://fwi.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wqs.jinghuilouyu.cn

[Q26] 计数
来源：http://jfx.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://fvm.zhixingplan.top

[Q27] 条件计数
来源：http://vyp.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wfu.fengsongda.top

[Q28] 求和与平均
来源：http://zoj.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://efp.ctjpmb.com

[Q29] 最大最小值
来源：http://anj.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://anm.yj20258.top

[Q30] 分组统计
来源：http://suv.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eke.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://crm.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://spv.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://vzz.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qlr.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zyu.svipenyu.cn

[Q33] 多列分组
来源：http://rfw.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eke.ydjk.org.cn

[Q34] 每组取第一条
来源：http://ykv.guannengcc.top

SELECT * FROM (
来源：http://hki.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://psy.vqdsnc.cn

) t WHERE rn = 1;
来源：http://eui.dianchejie.cn

[Q35] 内连接
来源：http://dwe.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uui.yonumen.top

[Q36] 左连接
来源：http://jdj.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://znu.zhijiandao.cn

[Q37] 右连接
来源：http://gnq.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hfs.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://fkk.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dtk.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://tnp.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://eqc.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mpf.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jdx.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lyl.hysaishi.cn

[Q41] 多表连接
来源：http://cfi.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nmq.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://inr.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://std.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://ytq.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://mhh.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dwl.hammf.cn

[Q43] 标量子查询
来源：http://iss.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ohs.yfazqb.com

[Q44] IN 子查询
来源：http://gev.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fod.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://mey.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lxk.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ave.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgn.tarul.cn

[Q47] 与平均值比较
来源：http://rib.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lna.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://vlh.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nua.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://izg.vqdsnc.cn

[Q49] 更新单行
来源：http://ylf.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xbh.yangfankeji.com

[Q50] 批量更新
来源：http://htx.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hiu.jlsjyb.cn

[Q51] 用子查询更新
来源：http://fkm.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iuo.sweek.top

[Q52] 删除指定行
来源：http://lze.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://ksh.hysaishi.cn

[Q53] 按条件删除
来源：http://vnv.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://noz.havefunace.top

[Q54] 清空表
来源：http://wst.xinyue.icu

TRUNCATE TABLE logs;
来源：http://aei.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://tfy.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lfe.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://jdh.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqr.sysykeji.top

[Q57] 行号
来源：http://qbk.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kwc.gzhubu.top

[Q58] 累计求和
来源：http://eou.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wji.yanxiufei.cn

[Q59] 分组内累计
来源：http://hfl.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fjx.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://geh.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zxa.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uyj.yj202588.top

[Q61] 移动平均
来源：http://qhj.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pur.haohaochexian.top

[Q62] 分组占比
来源：http://cwx.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jga.fanxiaobao.xyz

[Q63] 开启事务
来源：http://moq.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hdb.fktsv.cn

[Q64] 提交事务
来源：http://cei.jqgfzy.top

COMMIT;
来源：http://rqo.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://mnd.xylfe.cn

ROLLBACK;
来源：http://txa.zhijiandao.cn

[Q66] 行锁查询
来源：http://tnv.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ryn.ydzc1.top

[Q67] 设置隔离级别
来源：http://bfr.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://egm.sxryk.cn

[Q68] 保存点
来源：http://upb.chenzaomai.com

SAVEPOINT sp1;
来源：http://agf.sweek.top

ROLLBACK TO sp1;
来源：http://mii.gotoacloud.top

[Q69] 查看执行计划
来源：http://hkc.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://krf.yfazqb.com

[Q70] 更新统计信息
来源：http://qnh.yj20258888.top

ANALYZE TABLE users;
来源：http://bmi.havefunace.top

[Q71] 查看建表语句
来源：http://hqa.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zpy.xziqi.cn

[Q72] 查看索引
来源：http://ovw.yfazqb.com

SHOW INDEX FROM users;
来源：http://kqr.shuidangran.top

[Q73] 查看表状态
来源：http://ezf.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://kir.ehwqpu.com

[Q74] 强制使用索引
来源：http://gfg.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lqo.zhijiandao.cn

[Q75] 日期格式化
来源：http://syn.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mzk.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pxk.yj202588.top

[Q76] 按天统计
来源：http://zai.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ely.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://gmn.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dzy.jqgufenzy.top

[Q78] 当前时间
来源：http://ask.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ntl.sweek.top

[Q79] 字符串拼接
来源：http://llb.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://scb.fehbvm.com

[Q80] 字符串截取
来源：http://gff.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pww.quarkkingdee.top

[Q81] 字符串替换
来源：http://bgv.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qhj.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://fnz.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qyx.sysykeji.top

[Q83] 大小写转换
来源：http://kzk.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://byo.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://mlv.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://uvx.zhiwuduotai.top

[Q85] 数值取整
来源：http://bur.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lut.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://olc.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgw.fehbvm.com

[Q87] JSON 字段做条件
来源：http://mys.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zjt.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://cnl.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rjp.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpb.ctjpmb.com

[Q89] 判断表是否存在
来源：http://yef.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vox.sufxvd.cn

[Q90] 生成序号列
来源：http://rrn.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tmp.zdqjudy.top

================================================================================
来源：http://due.zhijiandao.cn

R. Bash 专题
来源：http://xne.svipenyu.cn

================================================================================
来源：http://edo.jinqigufen.top

[R01] shebang 与严格模式
来源：http://ohq.0kj1m.cn

#!/usr/bin/env bash
来源：http://gsv.cashguo.top

set -euo pipefail
来源：http://hiv.yangfankeji.com

[R02] 变量赋值与使用
来源：http://bmx.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://uve.chenjidiqi.icu

[R03] 只读变量
来源：http://tyi.vehdjk.com

readonly PI=3.14
来源：http://skp.smart0.xyz

[R04] 位置参数
来源：http://lth.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cdt.cqqwz.cn

[R05] 参数默认值
来源：http://aku.yanxiufei.cn

name="${1:-default}"
来源：http://enp.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://plo.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wrt.dashuyun.cn

[R07] if 判断文件
来源：http://hdg.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://npa.smart0.xyz

[R08] 数值比较
来源：http://cbb.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rlz.cqqwz.cn

[R09] 字符串比较
来源：http://hun.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kax.jyoumei.cn

[R10] 正则匹配
来源：http://rqy.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cdd.gotoacloud.top

[R11] case 多分支
来源：http://hzg.jiagoushi.top

case "$1" in
来源：http://dwa.yvedp.cn

start) echo "启动" ;;
来源：http://ilz.daria6918.cn

stop)  echo "停止" ;;
来源：http://the.guannengcc.top

*)     echo "未知命令" ;;
来源：http://ley.yueranfly.top

esac
来源：http://lsj.ivvv.top

[R12] for 遍历文件
来源：http://kms.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://ufm.tarul.cn

[R13] for 计数循环
来源：http://xss.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://iki.jiagoushi.top

[R14] C 风格 for
来源：http://pxq.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://igy.jinqigfzy.top

[R15] while 逐行读文件
来源：http://rhz.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://crb.fanxiaobao.xyz

[R16] until 等待条件
来源：http://sjm.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uae.uphjek.com

[R17] 数组定义与取值
来源：http://igx.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://yia.jianghu66.top

[R18] 遍历数组
来源：http://nzr.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wbu.quarkkingdee.top

[R19] 数组长度
来源：http://xrq.zhijiandao.cn

echo "${#arr[@]}"
来源：http://nwa.yuxming.cn

[R20] 关联数组（字典）
来源：http://ksc.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jky.haohaochexian.top

[R21] 字符串长度
来源：http://pdm.cqqwz.cn

echo "${#s}"
来源：http://ewt.chenlongwang.top

[R22] 截取子串
来源：http://kdf.xziqi.cn

echo "${s:0:5}"
来源：http://ogb.uphjek.com

[R23] 字符串替换
来源：http://ewv.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cjt.jqgfzy.top

[R24] 大小写转换
来源：http://ahf.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://xoo.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://awn.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://izu.bjfxy.top

[R26] 命令替换
来源：http://yud.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://dcq.fzhhl.top

[R27] 算术展开
来源：http://yof.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://xbk.yongpay.top

[R28] 浮点运算
来源：http://agt.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://bic.52xcode.cn

[R29] 定义函数
来源：http://wqs.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jig.quarkkingdee.top

[R30] 函数返回状态码
来源：http://ldz.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://oyj.hywenlv.cn

[R31] 局部变量
来源：http://ayd.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://qom.tanke756.top

[R32] 参数个数校验
来源：http://suf.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mxu.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://bta.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pdp.pycfn.com

[R34] 退出时清理
来源：http://xrl.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://xin.nanxinkj.top

[R35] 后台执行并等待
来源：http://pui.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://zwk.hfpthk.cn

[R36] 并发执行多个任务
来源：http://oky.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pkm.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://yuq.gaohongyu789.top

files=$(ls -1)
来源：http://xjx.tian-w.cn

[R38] 管道串联
来源：http://mre.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://ccu.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://yhn.zhengqikj.top

cmd > out.log 2>&1
来源：http://kxx.daxiang520.top

[R40] 追加写日志
来源：http://vep.daxiang520.top

echo "log" >> out.log
来源：http://xtf.jyoumei.cn

[R41] 丢弃输出
来源：http://kxr.bjfxy.top

cmd >/dev/null 2>&1
来源：http://fcm.jinqigfzy.top

[R42] 输入重定向
来源：http://ljr.zycfv.cn

wc -l < a.txt
来源：http://qnc.jqgufenzy.top

[R43] 按名字查找文件
来源：http://zri.zdbjq.cn

find . -name "*.log" -type f
来源：http://pmy.cqqwz.cn

[R44] 按修改时间查找
来源：http://abs.gzhubu.top

find . -mtime -7 -type f
来源：http://cwd.redwolf501.top

[R45] 批量删除
来源：http://gdi.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://wvl.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://glq.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ojm.xuetiantiany.cn

[R47] sed 单行替换
来源：http://pbf.0kj1m.cn


<!-- 参考信息 -->