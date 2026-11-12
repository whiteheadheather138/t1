代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyk.ivvv.top

user_id INT NOT NULL,
来源：http://tor.sxryk.cn

amount DECIMAL(10, 2),
来源：http://ixp.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jql.sxryk.cn

);
来源：http://wxn.zycfv.cn

[Q03] 增加列
来源：http://ure.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hhe.yuxming.cn

[Q04] 修改列类型
来源：http://uoh.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hkl.cheryme.top

[Q05] 重命名列
来源：http://ciy.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zxb.jqgfzy.top

[Q06] 删除列
来源：http://riw.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://wlo.hcnkem.com

[Q07] 删除表
来源：http://crh.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://lpx.hcnkem.com

[Q08] 创建普通索引
来源：http://uwj.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gwp.yj202588.top

[Q09] 创建唯一索引
来源：http://ucs.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://usk.gaohongyu789.top

[Q10] 插入单行
来源：http://mnv.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://shj.sjlbkw.cn

[Q11] 一次插入多行
来源：http://ida.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bzv.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://yrr.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://hmv.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zfm.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://ohn.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ons.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://ibb.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://itt.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://njk.gotoacloud.top

[Q15] 查询全部
来源：http://trg.nanxuanxn.top

SELECT * FROM users;
来源：http://nnj.redwolf501.top

[Q16] 查询指定列
来源：http://srw.zdbjq.cn

SELECT id, name FROM users;
来源：http://fxw.sweek.top

[Q17] 条件查询
来源：http://ryu.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nud.gogol.net.cn

[Q18] 模糊匹配
来源：http://eta.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wyu.quarkkingdee.top

[Q19] 范围查询
来源：http://ofh.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://moz.sjlbkw.cn

[Q20] IN 列表
来源：http://mnq.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mvx.hammf.cn

[Q21] 空值判断
来源：http://ygh.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qyx.tarul.cn

[Q22] 排序
来源：http://tjs.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xcm.svipenyu.cn

[Q23] 分页
来源：http://iqi.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qgx.yongpay.top

[Q24] 去重
来源：http://gvl.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://csn.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://dgv.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yqw.shanyushiyangtech.top

[Q26] 计数
来源：http://maf.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://azq.gzhubu.top

[Q27] 条件计数
来源：http://nob.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rxu.vehdjk.com

[Q28] 求和与平均
来源：http://epm.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xfb.vqdsnc.cn

[Q29] 最大最小值
来源：http://eqw.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nvf.smart0.xyz

[Q30] 分组统计
来源：http://uro.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sbw.chenzaomai.com

[Q31] 分组后过滤
来源：http://saq.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://shk.cucudq.cn

[Q32] 分组拼接字符串
来源：http://hnj.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qsx.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ijp.ybcxt.top

[Q33] 多列分组
来源：http://qhg.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qot.yj20258.top

[Q34] 每组取第一条
来源：http://tpb.gzhubu.top

SELECT * FROM (
来源：http://uwo.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gfs.epnwcf.com

) t WHERE rn = 1;
来源：http://ogy.shanyushiyangkeji.top

[Q35] 内连接
来源：http://ylz.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ijp.birdmap.top

[Q36] 左连接
来源：http://dxx.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jbu.hysaishi.cn

[Q37] 右连接
来源：http://yrt.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xip.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rzo.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fem.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://soh.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://del.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bpl.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jmv.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iqf.jyoumei.cn

[Q41] 多表连接
来源：http://wph.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mhl.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://ham.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://coo.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://ujy.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://otn.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kjh.nanxuanxn.top

[Q43] 标量子查询
来源：http://ewv.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tdq.nanxuanxn.top

[Q44] IN 子查询
来源：http://sln.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dur.pycfn.com

[Q45] EXISTS 判断存在
来源：http://mlk.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nwk.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://gzm.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rpw.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://cnj.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gzj.uphjek.com

[Q48] CTE 公用表表达式
来源：http://yzh.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmb.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://qyj.svipenyu.cn

[Q49] 更新单行
来源：http://gox.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eve.sysykeji.top

[Q50] 批量更新
来源：http://tly.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dqu.yongpay.top

[Q51] 用子查询更新
来源：http://oru.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pbi.0kj1m.cn

[Q52] 删除指定行
来源：http://sgo.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://nks.yangfankeji.com

[Q53] 按条件删除
来源：http://wql.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sat.xylfe.cn

[Q54] 清空表
来源：http://ddx.smart0.xyz

TRUNCATE TABLE logs;
来源：http://uuh.cheryme.top

[Q55] 排名（并列占位）
来源：http://cpb.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zgv.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://ndh.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://izd.hesvh.cn

[Q57] 行号
来源：http://dab.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pwl.9152youxi.cn

[Q58] 累计求和
来源：http://poe.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zsq.bjfxy.top

[Q59] 分组内累计
来源：http://rqg.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://shq.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://bwe.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dxu.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bjt.yj20258888.top

[Q61] 移动平均
来源：http://xrt.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qii.meibo888.top

[Q62] 分组占比
来源：http://noq.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fdm.nanxinkj.top

[Q63] 开启事务
来源：http://iuq.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://kpm.tianlin.xyz

[Q64] 提交事务
来源：http://dbq.tarul.cn

COMMIT;
来源：http://lrn.yfazqb.com

[Q65] 回滚事务
来源：http://rhr.zdqjudy.top

ROLLBACK;
来源：http://kpf.hfpthk.cn

[Q66] 行锁查询
来源：http://suu.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nrf.epnwcf.com

[Q67] 设置隔离级别
来源：http://fmm.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://izy.zhaomingkeji.xyz

[Q68] 保存点
来源：http://qxt.dianchejie.cn

SAVEPOINT sp1;
来源：http://rio.ivvv.top

ROLLBACK TO sp1;
来源：http://gbq.gaohongyu789.top

[Q69] 查看执行计划
来源：http://hnv.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ljl.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://ukr.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://yjz.aibaodan.cn

[Q71] 查看建表语句
来源：http://uae.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sdh.yanxiufei.cn

[Q72] 查看索引
来源：http://ksy.nanxinkj.top

SHOW INDEX FROM users;
来源：http://flo.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://ooz.dianchejie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jli.gotoacloud.top

[Q74] 强制使用索引
来源：http://fwf.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eua.ppjwa.cn

[Q75] 日期格式化
来源：http://oua.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nbd.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qnn.andypj.xyz

[Q76] 按天统计
来源：http://vjq.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vnu.cheryme.top

[Q77] 时间加减
来源：http://nxb.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mps.yongpay.top

[Q78] 当前时间
来源：http://svd.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xlb.bbcook.cn

[Q79] 字符串拼接
来源：http://qfl.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ibl.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://eyq.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://znl.zhengqikj.top

[Q81] 字符串替换
来源：http://xkn.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bmk.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://osf.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwo.tarul.cn

[Q83] 大小写转换
来源：http://rwh.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qoe.zdbjq.cn

[Q84] 去除首尾空格
来源：http://agc.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://aqy.tanke756.top

[Q85] 数值取整
来源：http://uaf.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://naf.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://qbq.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xzu.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://qzh.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pnw.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://uar.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yck.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zrs.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://dvv.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gku.yfazqb.com

[Q90] 生成序号列
来源：http://lxy.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ndb.hcnkem.com

================================================================================
来源：http://liq.zhixingplan.top

R. Bash 专题
来源：http://ikn.guannengcc.top

================================================================================
来源：http://xjh.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://upv.chenzaomai.com

#!/usr/bin/env bash
来源：http://gni.fengsongda.top

set -euo pipefail
来源：http://cpx.gzhubu.top

[R02] 变量赋值与使用
来源：http://xwi.yuxming.cn

name="Tom"; echo "$name"
来源：http://oew.cheryme.top

[R03] 只读变量
来源：http://lch.jqgfzy.top

readonly PI=3.14
来源：http://wvw.haohaochexian.top

[R04] 位置参数
来源：http://srb.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ikt.birdmap.top

[R05] 参数默认值
来源：http://hti.zdbjq.cn

name="${1:-default}"
来源：http://ihx.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://qfy.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://prn.xuanzx.com

[R07] if 判断文件
来源：http://ruk.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yxu.mhx1999.top

[R08] 数值比较
来源：http://kzt.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wdf.aibaodan.cn

[R09] 字符串比较
来源：http://dcw.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mro.cheryme.top

[R10] 正则匹配
来源：http://qnz.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xzd.jinghuilouyu.cn

[R11] case 多分支
来源：http://jgm.guowangkeji.top

case "$1" in
来源：http://qxj.zdbjq.cn

start) echo "启动" ;;
来源：http://bfk.mhx1999.top

stop)  echo "停止" ;;
来源：http://eou.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://ylw.yonumen.top

esac
来源：http://aax.ivvv.top

[R12] for 遍历文件
来源：http://vuh.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://uxz.xylfe.cn

[R13] for 计数循环
来源：http://dcp.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://hga.aibaodan.cn

[R14] C 风格 for
来源：http://hgk.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hnk.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://jzu.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eej.9152youxi.cn

[R16] until 等待条件
来源：http://gmd.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xvu.snrcjt.cn

[R17] 数组定义与取值
来源：http://fam.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tmu.feifeiyinyue.top

[R18] 遍历数组
来源：http://hng.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vuv.shzxlz.cn

[R19] 数组长度
来源：http://wif.yonumen.top

echo "${#arr[@]}"
来源：http://tsh.bjfxy.top

[R20] 关联数组（字典）
来源：http://cma.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://stp.jyoumei.cn

[R21] 字符串长度
来源：http://swd.fktsv.cn

echo "${#s}"
来源：http://ged.sweek.top

[R22] 截取子串
来源：http://tld.hysaishi.cn

echo "${s:0:5}"
来源：http://gyu.guowangkeji.top

[R23] 字符串替换
来源：http://hrp.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ujx.haohaochexian.top

[R24] 大小写转换
来源：http://idp.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gzg.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://bog.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xap.wangdashe.top

[R26] 命令替换
来源：http://eoo.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://ywa.jinqigfzy.top

[R27] 算术展开
来源：http://vnk.shuidangran.top

echo $((1 + 2 * 3))
来源：http://ryk.zdqjudy.top

[R28] 浮点运算
来源：http://jib.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://yli.quarkkingdee.top

[R29] 定义函数
来源：http://smy.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sca.epnwcf.com

[R30] 函数返回状态码
来源：http://vwm.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://vgu.ywan-chungtsiang.top

[R31] 局部变量
来源：http://pbd.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://ygo.zdbjq.cn

[R32] 参数个数校验
来源：http://hhr.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://men.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://qab.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kji.jiagoushi.top

[R34] 退出时清理
来源：http://lkr.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lmb.cheryme.top

[R35] 后台执行并等待
来源：http://dvh.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://rpj.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://wmq.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rre.yj20258888.top

[R37] 把输出赋给变量
来源：http://ddu.jyoumei.cn

files=$(ls -1)
来源：http://rwb.sysykeji.top

[R38] 管道串联
来源：http://awp.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://xwd.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://rbi.jlsjyb.cn

cmd > out.log 2>&1
来源：http://tup.yfazqb.com

[R40] 追加写日志
来源：http://gba.yj20258.top

echo "log" >> out.log
来源：http://wmh.andypj.xyz

[R41] 丢弃输出
来源：http://igd.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://nbb.gaohongyu789.top

[R42] 输入重定向
来源：http://erv.chenzaomai.com

wc -l < a.txt
来源：http://tdf.chenlongwang.top

[R43] 按名字查找文件
来源：http://edt.hysaishi.cn

find . -name "*.log" -type f
来源：http://nig.quarkkingdee.top

[R44] 按修改时间查找
来源：http://avr.cashguo.top

find . -mtime -7 -type f
来源：http://lmy.vehdjk.com

[R45] 批量删除
来源：http://jwq.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://avu.yj202588.top

[R46] 递归替换文件内容
来源：http://eho.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rst.ydzc1.top

[R47] sed 单行替换
来源：http://qit.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://htt.quarkkingdee.top

[R48] awk 取指定列
来源：http://noy.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://bhp.daria6918.cn

[R49] awk 带条件
来源：http://rht.iojbl.cn


<!-- 参考信息 -->