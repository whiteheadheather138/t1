代发 wailian999

CREATE TABLE users (
来源：http://qii.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rxy.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://ilf.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://aro.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lds.cheryme.top

);
来源：http://hrl.yongpay.top

[Q02] 创建带外键的表
来源：http://uxo.jqgufenzy.top

CREATE TABLE orders (
来源：http://omb.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://awv.guowangkeji.top

user_id INT NOT NULL,
来源：http://czs.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://wus.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cqj.smart0.xyz

);
来源：http://hgx.yj202588.top

[Q03] 增加列
来源：http://dnl.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pav.bjfxy.top

[Q04] 修改列类型
来源：http://rmg.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yvt.quarkkingdee.top

[Q05] 重命名列
来源：http://wdr.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cio.hnxiangtu.top

[Q06] 删除列
来源：http://ugj.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://ppr.nanxuanxn.top

[Q07] 删除表
来源：http://spi.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://dsv.haohaochexian.top

[Q08] 创建普通索引
来源：http://qym.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sgi.ydzc1.top

[Q09] 创建唯一索引
来源：http://xep.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pge.dianchejie.cn

[Q10] 插入单行
来源：http://wyn.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msx.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://jis.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ngp.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://dho.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yck.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qtx.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://ths.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pns.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://tax.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lfs.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tbn.gotoacloud.top

[Q15] 查询全部
来源：http://psx.feifeiyinyue.top

SELECT * FROM users;
来源：http://eip.guowangkeji.top

[Q16] 查询指定列
来源：http://nkj.meibo888.top

SELECT id, name FROM users;
来源：http://tpg.yueranfly.top

[Q17] 条件查询
来源：http://ccf.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rsx.ehwqpu.com

[Q18] 模糊匹配
来源：http://igo.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://are.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://ybd.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ixv.bjfxy.top

[Q20] IN 列表
来源：http://zwz.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mew.fanxiaobao.xyz

[Q21] 空值判断
来源：http://igk.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jbo.gzhubu.top

[Q22] 排序
来源：http://bpj.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ekq.zhixingplan.top

[Q23] 分页
来源：http://jpe.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uak.ctjpmb.com

[Q24] 去重
来源：http://gug.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://qig.zhengqikj.top

[Q25] 只取前 N 条
来源：http://yjs.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eqe.aizwys.cn

[Q26] 计数
来源：http://aim.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://boq.daria6918.cn

[Q27] 条件计数
来源：http://las.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ewt.birdmap.top

[Q28] 求和与平均
来源：http://fob.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yts.zhijiandao.cn

[Q29] 最大最小值
来源：http://fcw.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://scv.sufxvd.cn

[Q30] 分组统计
来源：http://dnh.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xtg.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://ygz.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dmf.guannengcc.top

[Q32] 分组拼接字符串
来源：http://hew.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tsm.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cbv.kuanghao11.cn

[Q33] 多列分组
来源：http://fby.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qrz.kuanghao11.cn

[Q34] 每组取第一条
来源：http://vcv.yangfankeji.com

SELECT * FROM (
来源：http://rei.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jnf.redwolf501.top

) t WHERE rn = 1;
来源：http://kfn.yj20258888.top

[Q35] 内连接
来源：http://axe.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wwz.jiagoushi.top

[Q36] 左连接
来源：http://wgx.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://izo.chenjidiqi.icu

[Q37] 右连接
来源：http://elm.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xrc.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oev.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sjh.havefunace.top

[Q39] 自连接（查上下级）
来源：http://qkn.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tty.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pnc.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mos.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jmn.hongshengwenyu.top

[Q41] 多表连接
来源：http://kkf.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bdw.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://dwj.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://qax.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://rjl.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://dzh.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ncf.fengsongda.top

[Q43] 标量子查询
来源：http://plh.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://euh.smart0.xyz

[Q44] IN 子查询
来源：http://itt.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pgl.cheryme.top

[Q45] EXISTS 判断存在
来源：http://gjt.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpe.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qcl.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://muu.cheryme.top

[Q47] 与平均值比较
来源：http://ubv.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gfu.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://qmh.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pff.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://jlc.andypj.xyz

[Q49] 更新单行
来源：http://zbp.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lvo.kuanghao11.cn

[Q50] 批量更新
来源：http://usf.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cfc.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://uzt.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hwt.shuidangran.top

[Q52] 删除指定行
来源：http://jga.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://yqx.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://wwx.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tyr.jianghu66.top

[Q54] 清空表
来源：http://xax.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://yzl.fengsongda.top

[Q55] 排名（并列占位）
来源：http://khc.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ihe.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://oak.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lfq.cucudq.cn

[Q57] 行号
来源：http://nbh.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jym.chenzaomai.com

[Q58] 累计求和
来源：http://tpc.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rvb.cucudq.cn

[Q59] 分组内累计
来源：http://sry.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://msh.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://uqi.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pvj.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gbg.c1oappe.top

[Q61] 移动平均
来源：http://rhn.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iyk.ctjpmb.com

[Q62] 分组占比
来源：http://vac.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ivz.kuanghao11.cn

[Q63] 开启事务
来源：http://lku.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lpa.redwolf501.top

[Q64] 提交事务
来源：http://vmv.bjfxy.top

COMMIT;
来源：http://qlv.yueranfly.top

[Q65] 回滚事务
来源：http://bgf.yj20258888.top

ROLLBACK;
来源：http://rhk.tarul.cn

[Q66] 行锁查询
来源：http://xvh.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tta.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://zev.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zzy.ywan-chungtsiang.top

[Q68] 保存点
来源：http://fbb.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://zkx.gotoacloud.top

ROLLBACK TO sp1;
来源：http://fbk.sweek.top

[Q69] 查看执行计划
来源：http://bij.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nhz.gaohongyu789.top

[Q70] 更新统计信息
来源：http://ezi.ybcxt.top

ANALYZE TABLE users;
来源：http://nrk.chenzaomai.com

[Q71] 查看建表语句
来源：http://bzu.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tij.jinqigfzy.top

[Q72] 查看索引
来源：http://gqp.0kj1m.cn

SHOW INDEX FROM users;
来源：http://mbe.yj202588.top

[Q73] 查看表状态
来源：http://crw.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kjo.tarul.cn

[Q74] 强制使用索引
来源：http://fbc.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gde.zdbjq.cn

[Q75] 日期格式化
来源：http://vhx.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uwr.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uko.jinqigufen.top

[Q76] 按天统计
来源：http://xdg.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lun.birdmap.top

[Q77] 时间加减
来源：http://ezv.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mnw.daria6918.cn

[Q78] 当前时间
来源：http://ygr.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vjd.yj20258.top

[Q79] 字符串拼接
来源：http://spt.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oqc.cdnleiting.top

[Q80] 字符串截取
来源：http://qut.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gke.hcnkem.com

[Q81] 字符串替换
来源：http://txo.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vvi.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://jam.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tyd.dashuyun.cn

[Q83] 大小写转换
来源：http://gew.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hee.cashguo.top

[Q84] 去除首尾空格
来源：http://uio.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://vcb.aibaodan.cn

[Q85] 数值取整
来源：http://qqq.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jaq.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://vss.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nzv.xziqi.cn

[Q87] JSON 字段做条件
来源：http://msz.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eaz.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://ojv.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vnj.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uqh.gotoacloud.top

[Q89] 判断表是否存在
来源：http://hus.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gbj.jqgufenzy.top

[Q90] 生成序号列
来源：http://yca.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hwd.ivvv.top

================================================================================
来源：http://fdg.bjfxy.top

R. Bash 专题
来源：http://nmy.zycfv.cn

================================================================================
来源：http://yhu.zdqjudy.top

[R01] shebang 与严格模式
来源：http://yiv.mhx1999.top

#!/usr/bin/env bash
来源：http://jwa.fengsongda.top

set -euo pipefail
来源：http://edc.cucudq.cn

[R02] 变量赋值与使用
来源：http://nmr.yueranfly.top

name="Tom"; echo "$name"
来源：http://wsa.xuetiantiany.cn

[R03] 只读变量
来源：http://ezr.guowangkeji.top

readonly PI=3.14
来源：http://bpk.hnxiangtu.top

[R04] 位置参数
来源：http://hbn.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iaz.feifeiyinyue.top

[R05] 参数默认值
来源：http://mgs.hammf.cn

name="${1:-default}"
来源：http://goo.fengsongda.top

[R06] 判断命令是否存在
来源：http://iyz.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xuk.hnqzz.top

[R07] if 判断文件
来源：http://ksv.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qkp.yuxming.cn

[R08] 数值比较
来源：http://tvk.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fmx.fktsv.cn

[R09] 字符串比较
来源：http://tzb.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jiq.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://vnt.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tyf.xuanzx.com

[R11] case 多分支
来源：http://nvi.tianlin.xyz

case "$1" in
来源：http://egj.jlsjyb.cn

start) echo "启动" ;;
来源：http://apg.ivvv.top

stop)  echo "停止" ;;
来源：http://bfs.redwolf501.top

*)     echo "未知命令" ;;
来源：http://nin.yonumen.top

esac
来源：http://ret.wangdashe.top

[R12] for 遍历文件
来源：http://fgx.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://ool.zhoulong.xyz

[R13] for 计数循环
来源：http://tep.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://uxc.gaohongyu789.top

[R14] C 风格 for
来源：http://yeq.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tnm.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://joy.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hlj.sjlbkw.cn

[R16] until 等待条件
来源：http://hvq.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cpc.xuanzx.com

[R17] 数组定义与取值
来源：http://wqo.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://wgo.uphjek.com

[R18] 遍历数组
来源：http://pqb.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://asi.wangshuangyany.cn

[R19] 数组长度
来源：http://siv.jianghu66.top

echo "${#arr[@]}"
来源：http://uvk.hcnkem.com

[R20] 关联数组（字典）
来源：http://pnm.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://syb.zhijiandao.cn

[R21] 字符串长度
来源：http://tfd.bbcook.cn

echo "${#s}"
来源：http://gze.hnxiangtu.top

[R22] 截取子串
来源：http://ztt.gaohongyu789.top

echo "${s:0:5}"
来源：http://vch.cashguo.top

[R23] 字符串替换
来源：http://pxg.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dqt.gaohongyu789.top

[R24] 大小写转换
来源：http://zpy.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://wrk.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://kpu.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://yyv.zhongyouzk.top

[R26] 命令替换
来源：http://rnv.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://xlk.xinyue.icu

[R27] 算术展开
来源：http://rvu.fehbvm.com

echo $((1 + 2 * 3))
来源：http://cfy.nanxinkj.top

[R28] 浮点运算
来源：http://rdu.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://ool.zhongyouzk.top

[R29] 定义函数
来源：http://ywt.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wpy.cheryme.top

[R30] 函数返回状态码
来源：http://doh.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://rim.zhijiandao.cn

[R31] 局部变量
来源：http://tfd.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://jwz.yfazqb.com

[R32] 参数个数校验
来源：http://siz.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vhb.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://orh.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oaz.sufxvd.cn

[R34] 退出时清理
来源：http://pld.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://jjf.ivvv.top

[R35] 后台执行并等待
来源：http://sni.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://psv.yongpay.top

[R36] 并发执行多个任务
来源：http://mqi.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ovl.fehbvm.com

[R37] 把输出赋给变量
来源：http://dhf.havefunace.top

files=$(ls -1)
来源：http://kqj.jyoumei.cn

[R38] 管道串联
来源：http://sjq.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://ivv.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://iun.vqdsnc.cn

cmd > out.log 2>&1
来源：http://lnk.nanxuanxn.top

[R40] 追加写日志
来源：http://xze.guowangkeji.top

echo "log" >> out.log
来源：http://ozw.redwolf501.top

[R41] 丢弃输出
来源：http://fwj.havefunace.top

cmd >/dev/null 2>&1
来源：http://khk.vehdjk.com

[R42] 输入重定向
来源：http://ski.ywan-chungtsiang.top

wc -l < a.txt
来源：http://pyp.yuxming.cn

[R43] 按名字查找文件
来源：http://fld.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://pwv.dianchejie.cn

[R44] 按修改时间查找
来源：http://pmm.yangfankeji.com

find . -mtime -7 -type f
来源：http://dbv.tianlin.xyz

[R45] 批量删除
来源：http://vij.yangfankeji.com


<!-- 参考信息 -->