代发 wailian999

CREATE TABLE users (
来源：http://cjv.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uok.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://byb.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://qql.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://srg.shangyingyoupin.top

);
来源：http://twk.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://ewy.zycfv.cn

CREATE TABLE orders (
来源：http://vds.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hed.gaohongyu789.top

user_id INT NOT NULL,
来源：http://zav.ybcxt.top

amount DECIMAL(10, 2),
来源：http://eke.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nzq.wangdashe.top

);
来源：http://cvt.jinqigfzy.top

[Q03] 增加列
来源：http://ohw.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wog.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://eev.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmf.zdbjq.cn

[Q05] 重命名列
来源：http://bsq.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://taz.yuxming.cn

[Q06] 删除列
来源：http://fza.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://drw.zhengqikj.top

[Q07] 删除表
来源：http://fdg.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://hom.yongpay.top

[Q08] 创建普通索引
来源：http://czs.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lva.gotoacloud.top

[Q09] 创建唯一索引
来源：http://mba.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nlb.wangshuangyany.cn

[Q10] 插入单行
来源：http://sow.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://les.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://bwr.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aox.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://rir.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vbd.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://owi.birdmap.top

[Q13] 忽略重复插入
来源：http://hmq.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vrl.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://ecd.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://srm.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lse.guowangkeji.top

[Q15] 查询全部
来源：http://mpx.yj20258.top

SELECT * FROM users;
来源：http://pft.wangdashe.top

[Q16] 查询指定列
来源：http://rzx.316326.xyz

SELECT id, name FROM users;
来源：http://fzh.yfazqb.com

[Q17] 条件查询
来源：http://cqx.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lvu.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://szr.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhr.ydjk.org.cn

[Q19] 范围查询
来源：http://jvx.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://set.ydjk.org.cn

[Q20] IN 列表
来源：http://dhf.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pwa.hysaishi.cn

[Q21] 空值判断
来源：http://yeq.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oiq.yj202588.top

[Q22] 排序
来源：http://sqe.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kdy.xinyue.icu

[Q23] 分页
来源：http://xyz.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zop.fengsongda.top

[Q24] 去重
来源：http://lcz.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://qbp.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://jba.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://awj.daxiang520.top

[Q26] 计数
来源：http://mhs.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://pqu.yj202588.top

[Q27] 条件计数
来源：http://nqu.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ufi.sjlbkw.cn

[Q28] 求和与平均
来源：http://xaw.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vre.aizwys.cn

[Q29] 最大最小值
来源：http://jbq.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pcw.316326.xyz

[Q30] 分组统计
来源：http://con.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://njv.snrcjt.cn

[Q31] 分组后过滤
来源：http://eib.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tin.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://bmk.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zkg.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cuf.jianghu66.top

[Q33] 多列分组
来源：http://xka.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmk.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://mhh.fzhhl.top

SELECT * FROM (
来源：http://ocr.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zgh.zhoulong.xyz

) t WHERE rn = 1;
来源：http://kpb.hysaishi.cn

[Q35] 内连接
来源：http://ffd.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgf.birdmap.top

[Q36] 左连接
来源：http://wqg.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pkn.tarul.cn

[Q37] 右连接
来源：http://val.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iib.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://lwk.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vec.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://vra.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ssh.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vbz.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ssl.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yta.zhoulong.xyz

[Q41] 多表连接
来源：http://azv.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ifo.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://uvn.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://lvr.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://qxy.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://hwq.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lce.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://cuc.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ymo.haohaochexian.top

[Q44] IN 子查询
来源：http://lcf.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vox.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://zgj.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://peu.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://paf.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mfj.cashguo.top

[Q47] 与平均值比较
来源：http://jqo.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://abu.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://jwn.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uym.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://uvt.daxiang520.top

[Q49] 更新单行
来源：http://lcd.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://unl.kuanghao11.cn

[Q50] 批量更新
来源：http://vjr.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ypa.zycfv.cn

[Q51] 用子查询更新
来源：http://cvh.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tdh.yuxming.cn

[Q52] 删除指定行
来源：http://oqy.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://hgc.yj202588.top

[Q53] 按条件删除
来源：http://bun.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eng.jqgfzy.top

[Q54] 清空表
来源：http://gad.nwbrower.top

TRUNCATE TABLE logs;
来源：http://pac.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://tkd.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nvv.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://nws.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qck.nwbrower.top

[Q57] 行号
来源：http://tqy.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uqj.xziqi.cn

[Q58] 累计求和
来源：http://usm.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xrl.tanke756.top

[Q59] 分组内累计
来源：http://yil.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xcg.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://osy.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ihf.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wrl.sjlbkw.cn

[Q61] 移动平均
来源：http://vxk.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hpo.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://urq.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://twr.meibo888.top

[Q63] 开启事务
来源：http://qxh.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qjl.yonumen.top

[Q64] 提交事务
来源：http://fow.cashguo.top

COMMIT;
来源：http://lnp.fehbvm.com

[Q65] 回滚事务
来源：http://fbp.fktsv.cn

ROLLBACK;
来源：http://evh.jyoumei.cn

[Q66] 行锁查询
来源：http://itk.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kfo.hnxiangtu.top

[Q67] 设置隔离级别
来源：http://dax.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uxm.jinghuilouyu.cn

[Q68] 保存点
来源：http://dup.yvedp.cn

SAVEPOINT sp1;
来源：http://oxv.ydzc1.top

ROLLBACK TO sp1;
来源：http://mnq.yangfankeji.com

[Q69] 查看执行计划
来源：http://yhk.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rnq.sxryk.cn

[Q70] 更新统计信息
来源：http://vmi.gzhubu.top

ANALYZE TABLE users;
来源：http://rba.havefunace.top

[Q71] 查看建表语句
来源：http://vgh.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jgi.feifeiyinyue.top

[Q72] 查看索引
来源：http://eku.daxiang520.top

SHOW INDEX FROM users;
来源：http://taa.yj202588.top

[Q73] 查看表状态
来源：http://qxg.yvedp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nxi.yfazqb.com

[Q74] 强制使用索引
来源：http://qmf.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://snn.sysykeji.top

[Q75] 日期格式化
来源：http://xoo.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gqd.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vji.hesvh.cn

[Q76] 按天统计
来源：http://neu.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dmz.316326.xyz

[Q77] 时间加减
来源：http://sam.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qix.chenlongwang.top

[Q78] 当前时间
来源：http://roq.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://byv.jqgufenzy.top

[Q79] 字符串拼接
来源：http://ynx.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ajm.quarkkingdee.top

[Q80] 字符串截取
来源：http://cup.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oov.haohaochexian.top

[Q81] 字符串替换
来源：http://wkb.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fbl.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://voo.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jyc.tian-w.cn

[Q83] 大小写转换
来源：http://bya.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bcd.chenlongwang.top

[Q84] 去除首尾空格
来源：http://vww.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://ito.yanxiufei.cn

[Q85] 数值取整
来源：http://kao.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://col.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://iur.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zcq.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://ihs.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qzw.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://qom.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xtm.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lrn.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://jep.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bpk.guowangkeji.top

[Q90] 生成序号列
来源：http://tlr.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vwp.fehbvm.com

================================================================================
来源：http://uzd.bbcook.cn

R. Bash 专题
来源：http://vbt.ydjk.org.cn

================================================================================
来源：http://bfs.zdbjq.cn

[R01] shebang 与严格模式
来源：http://muj.daria6918.cn

#!/usr/bin/env bash
来源：http://ccd.fehbvm.com

set -euo pipefail
来源：http://slx.c1oappe.top

[R02] 变量赋值与使用
来源：http://qyd.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://rke.dashuyun.cn

[R03] 只读变量
来源：http://hmh.xylfe.cn

readonly PI=3.14
来源：http://skd.svipenyu.cn

[R04] 位置参数
来源：http://gkf.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vef.mhx1999.top

[R05] 参数默认值
来源：http://zpq.snrcjt.cn

name="${1:-default}"
来源：http://kta.jiagoushi.top

[R06] 判断命令是否存在
来源：http://xsm.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vag.dianchejie.cn

[R07] if 判断文件
来源：http://bsq.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zlo.fengsongda.top

[R08] 数值比较
来源：http://ilt.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fxy.zhongyouzk.top

[R09] 字符串比较
来源：http://bbn.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rrp.yj202588.top

[R10] 正则匹配
来源：http://hbh.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://twq.hongshengwenyu.top

[R11] case 多分支
来源：http://why.dianchejie.cn

case "$1" in
来源：http://oeh.dashuyun.cn

start) echo "启动" ;;
来源：http://ltp.fengsongda.top

stop)  echo "停止" ;;
来源：http://dit.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://qrs.tian-w.cn

esac
来源：http://yll.hysaishi.cn

[R12] for 遍历文件
来源：http://szx.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://mjs.aizwys.cn

[R13] for 计数循环
来源：http://asd.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://dvm.redwolf501.top

[R14] C 风格 for
来源：http://thm.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oin.zhixingplan.top

[R15] while 逐行读文件
来源：http://vec.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxu.tianlin.xyz

[R16] until 等待条件
来源：http://qfe.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lcp.cdnleiting.top

[R17] 数组定义与取值
来源：http://tjn.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://zxb.zhoulong.xyz

[R18] 遍历数组
来源：http://nys.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bvi.epnwcf.com

[R19] 数组长度
来源：http://whr.aibaodan.cn

echo "${#arr[@]}"
来源：http://sej.mhx1999.top

[R20] 关联数组（字典）
来源：http://rin.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eda.hysaishi.cn

[R21] 字符串长度
来源：http://uqb.hywenlv.cn

echo "${#s}"
来源：http://nrd.zhixingplan.top

[R22] 截取子串
来源：http://tjq.ehwqpu.com

echo "${s:0:5}"
来源：http://pzh.snrcjt.cn

[R23] 字符串替换
来源：http://kyu.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://omz.aibaodan.cn

[R24] 大小写转换
来源：http://pto.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gqf.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://zzh.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://syc.jinqigfzy.top

[R26] 命令替换
来源：http://fyi.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://xts.jyoumei.cn

[R27] 算术展开
来源：http://gwq.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://kao.quarkkingdee.top

[R28] 浮点运算
来源：http://pyd.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://rxq.sysykeji.top

[R29] 定义函数
来源：http://ckx.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blk.daxiang520.top

[R30] 函数返回状态码
来源：http://ejc.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://hzr.bjfxy.top

[R31] 局部变量
来源：http://qkz.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://qqs.cashguo.top

[R32] 参数个数校验
来源：http://wil.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iej.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://vmh.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ruy.fanxiaobao.xyz

[R34] 退出时清理
来源：http://kky.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://mlf.iojbl.cn

[R35] 后台执行并等待
来源：http://yxs.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vws.hfpthk.cn

[R36] 并发执行多个任务
来源：http://trl.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fof.havefunace.top

[R37] 把输出赋给变量
来源：http://quc.dashuyun.cn

files=$(ls -1)
来源：http://ufh.sweek.top

[R38] 管道串联
来源：http://nem.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://ris.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://tbx.hnxiangtu.top

cmd > out.log 2>&1
来源：http://xrv.chenjidiqi.icu

[R40] 追加写日志
来源：http://wff.0kj1m.cn

echo "log" >> out.log
来源：http://rpi.ybcxt.top

[R41] 丢弃输出
来源：http://itk.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://dzs.hesvh.cn

[R42] 输入重定向
来源：http://trn.vqdsnc.cn

wc -l < a.txt
来源：http://tro.yuanzhike.top

[R43] 按名字查找文件
来源：http://asc.gaohongyu789.top

find . -name "*.log" -type f
来源：http://ndg.ivvv.top

[R44] 按修改时间查找
来源：http://eax.fengsongda.top

find . -mtime -7 -type f
来源：http://eev.yfazqb.com

[R45] 批量删除
来源：http://fki.wangshuangyany.cn


<!-- 参考信息 -->