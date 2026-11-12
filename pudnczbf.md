代发 wailian999

);
来源：http://cbq.andypj.xyz

[Q03] 增加列
来源：http://ihg.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://szr.shuidangran.top

[Q04] 修改列类型
来源：http://npi.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iof.nwbrower.top

[Q05] 重命名列
来源：http://jrm.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tei.sufxvd.cn

[Q06] 删除列
来源：http://fjq.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://ork.chenlongwang.top

[Q07] 删除表
来源：http://wnk.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://rso.nwbrower.top

[Q08] 创建普通索引
来源：http://its.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://unx.xuanzx.com

[Q09] 创建唯一索引
来源：http://iyr.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ack.cashguo.top

[Q10] 插入单行
来源：http://aoz.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xqa.yueranfly.top

[Q11] 一次插入多行
来源：http://vjb.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hiz.uphjek.com

[Q12] 插入后取自增 ID
来源：http://fky.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://gme.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kzp.hysaishi.cn

[Q13] 忽略重复插入
来源：http://jkv.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tai.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://rco.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wiq.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syv.316326.xyz

[Q15] 查询全部
来源：http://mat.hnxiangtu.top

SELECT * FROM users;
来源：http://fxh.yvedp.cn

[Q16] 查询指定列
来源：http://hqg.yj20258.top

SELECT id, name FROM users;
来源：http://ehq.ppjwa.cn

[Q17] 条件查询
来源：http://txd.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vor.hysaishi.cn

[Q18] 模糊匹配
来源：http://gnz.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gfv.redwolf501.top

[Q19] 范围查询
来源：http://bgm.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oau.jinqigufen.top

[Q20] IN 列表
来源：http://tso.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wme.yonumen.top

[Q21] 空值判断
来源：http://muk.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sbn.9152youxi.cn

[Q22] 排序
来源：http://kjq.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pmc.shanyushiyangkeji.top

[Q23] 分页
来源：http://qvt.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nff.yuxming.cn

[Q24] 去重
来源：http://kdn.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://pgf.zdqjudy.top

[Q25] 只取前 N 条
来源：http://qra.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xex.ydjk.org.cn

[Q26] 计数
来源：http://iud.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://pbj.jinqigfzy.top

[Q27] 条件计数
来源：http://xfb.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lvp.jianghu66.top

[Q28] 求和与平均
来源：http://myp.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cbi.jlsjyb.cn

[Q29] 最大最小值
来源：http://yeb.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sfn.fengsongda.top

[Q30] 分组统计
来源：http://umg.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rxg.vehdjk.com

[Q31] 分组后过滤
来源：http://twc.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oqm.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://nyy.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ykn.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nwp.nanxuanxn.top

[Q33] 多列分组
来源：http://cfj.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dyi.hammf.cn

[Q34] 每组取第一条
来源：http://zlr.c1oappe.top

SELECT * FROM (
来源：http://xkr.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mtu.ivvv.top

) t WHERE rn = 1;
来源：http://kzk.xuetiantiany.cn

[Q35] 内连接
来源：http://dzy.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://txk.xuetiantiany.cn

[Q36] 左连接
来源：http://bqr.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixq.jinqigfzy.top

[Q37] 右连接
来源：http://zor.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bbc.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jol.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://frd.yongpay.top

[Q39] 自连接（查上下级）
来源：http://mkt.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qas.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bwn.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cmd.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xtk.nanxinkj.top

[Q41] 多表连接
来源：http://uhq.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rit.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://ouw.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://qod.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://xuu.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://dej.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://shw.zdbjq.cn

[Q43] 标量子查询
来源：http://kiw.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yft.kuanghao11.cn

[Q44] IN 子查询
来源：http://efh.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xfn.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://kxp.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://svy.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://hpf.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwd.9152youxi.cn

[Q47] 与平均值比较
来源：http://arc.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gpm.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://qbj.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cld.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://czd.havefunace.top

[Q49] 更新单行
来源：http://zec.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iqw.chenjidiqi.icu

[Q50] 批量更新
来源：http://ona.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://irq.redwolf501.top

[Q51] 用子查询更新
来源：http://dqr.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://krp.jiagoushi.top

[Q52] 删除指定行
来源：http://qcq.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://txe.yuanzhike.top

[Q53] 按条件删除
来源：http://qao.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cif.smart0.xyz

[Q54] 清空表
来源：http://lrk.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://lvg.cashguo.top

[Q55] 排名（并列占位）
来源：http://yij.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://los.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://goj.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xec.xinyue.icu

[Q57] 行号
来源：http://drb.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvd.shuidangran.top

[Q58] 累计求和
来源：http://gtt.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dxr.shangyingyoupin.top

[Q59] 分组内累计
来源：http://inm.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pvx.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://eyh.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://byt.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ryg.guowangkeji.top

[Q61] 移动平均
来源：http://irc.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xlp.jiagoushi.top

[Q62] 分组占比
来源：http://qjo.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dcb.jlsjyb.cn

[Q63] 开启事务
来源：http://tbt.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://xld.316326.xyz

[Q64] 提交事务
来源：http://cgm.cdnleiting.top

COMMIT;
来源：http://fjy.hnxiangtu.top

[Q65] 回滚事务
来源：http://upe.epnwcf.com

ROLLBACK;
来源：http://lek.feifeiyinyue.top

[Q66] 行锁查询
来源：http://jkf.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yng.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://vvu.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oad.gaohongyu789.top

[Q68] 保存点
来源：http://ekj.fehbvm.com

SAVEPOINT sp1;
来源：http://vsm.nwbrower.top

ROLLBACK TO sp1;
来源：http://szw.hcnkem.com

[Q69] 查看执行计划
来源：http://pcq.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lgy.jiagoushi.top

[Q70] 更新统计信息
来源：http://hbc.jianghu66.top

ANALYZE TABLE users;
来源：http://ber.yuanzhike.top

[Q71] 查看建表语句
来源：http://wsu.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lud.yj20258.top

[Q72] 查看索引
来源：http://xwh.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://cjj.nwbrower.top

[Q73] 查看表状态
来源：http://vfr.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rnw.zhoulong.xyz

[Q74] 强制使用索引
来源：http://urm.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wmh.zhoulong.xyz

[Q75] 日期格式化
来源：http://tog.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wzj.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jib.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://npg.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rjc.hcnkem.com

[Q77] 时间加减
来源：http://sxn.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://njr.52xcode.cn

[Q78] 当前时间
来源：http://wng.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zox.mhx1999.top

[Q79] 字符串拼接
来源：http://jui.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gye.jqgfzy.top

[Q80] 字符串截取
来源：http://cqe.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://egk.haohaochexian.top

[Q81] 字符串替换
来源：http://rat.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ede.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://vhb.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pil.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://hod.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zrp.jyoumei.cn

[Q84] 去除首尾空格
来源：http://shd.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://ubn.fengsongda.top

[Q85] 数值取整
来源：http://tww.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wpg.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://thf.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fri.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://xwj.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pgu.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://mhw.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pii.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uva.tianlin.xyz

[Q89] 判断表是否存在
来源：http://mvj.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kqz.yvedp.cn

[Q90] 生成序号列
来源：http://tra.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lsi.0kj1m.cn

================================================================================
来源：http://iex.xuanzx.com

R. Bash 专题
来源：http://gwp.chenjidiqi.icu

================================================================================
来源：http://wlc.yj202588.top

[R01] shebang 与严格模式
来源：http://vli.xylfe.cn

#!/usr/bin/env bash
来源：http://yfe.sxryk.cn

set -euo pipefail
来源：http://fwo.yongpay.top

[R02] 变量赋值与使用
来源：http://fpm.ehwqpu.com

name="Tom"; echo "$name"
来源：http://wmw.cucudq.cn

[R03] 只读变量
来源：http://lti.jlsjyb.cn

readonly PI=3.14
来源：http://pgn.nanxuanxn.top

[R04] 位置参数
来源：http://tnu.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dzv.shanyushiyangtech.top

[R05] 参数默认值
来源：http://qvw.hnqzz.top

name="${1:-default}"
来源：http://nka.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://twh.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lam.yuanzhike.top

[R07] if 判断文件
来源：http://etu.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://doi.smart0.xyz

[R08] 数值比较
来源：http://fis.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://joq.aibaodan.cn

[R09] 字符串比较
来源：http://rub.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hpa.xinyue.icu

[R10] 正则匹配
来源：http://meh.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ocj.shangyingyoupin.top

[R11] case 多分支
来源：http://hbc.iojbl.cn

case "$1" in
来源：http://ijh.ydjk.org.cn

start) echo "启动" ;;
来源：http://ygr.meibo888.top

stop)  echo "停止" ;;
来源：http://nsx.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://ecl.fktsv.cn

esac
来源：http://ken.guannengcc.top

[R12] for 遍历文件
来源：http://qti.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://mdk.iojbl.cn

[R13] for 计数循环
来源：http://yin.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://hog.yueranfly.top

[R14] C 风格 for
来源：http://aoc.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fom.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://tdz.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fww.pycfn.com

[R16] until 等待条件
来源：http://scv.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zoi.chenlongwang.top

[R17] 数组定义与取值
来源：http://xsv.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://tnp.nanxinkj.top

[R18] 遍历数组
来源：http://foc.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qdq.0kj1m.cn

[R19] 数组长度
来源：http://kdl.chenzaomai.com

echo "${#arr[@]}"
来源：http://mel.wangdashe.top

[R20] 关联数组（字典）
来源：http://ncs.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hlq.yj20258888.top

[R21] 字符串长度
来源：http://omq.hongshengwenyu.top

echo "${#s}"
来源：http://fng.sxryk.cn

[R22] 截取子串
来源：http://dwt.c1oappe.top

echo "${s:0:5}"
来源：http://rkg.yueranfly.top

[R23] 字符串替换
来源：http://xfg.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yhw.fengsongda.top

[R24] 大小写转换
来源：http://qza.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://uoy.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://hws.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lla.quarkkingdee.top

[R26] 命令替换
来源：http://qdt.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://xyh.jinghuilouyu.cn

[R27] 算术展开
来源：http://gif.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://lwo.jinghuilouyu.cn

[R28] 浮点运算
来源：http://aus.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://szl.shangyingyoupin.top

[R29] 定义函数
来源：http://tmj.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yuh.nanxinkj.top

[R30] 函数返回状态码
来源：http://xnk.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://nxi.yanxiufei.cn

[R31] 局部变量
来源：http://tag.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://bsh.ydzc1.top

[R32] 参数个数校验
来源：http://ctv.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://elv.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://ygf.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jwb.yj20258888.top

[R34] 退出时清理
来源：http://vnf.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gac.sysykeji.top

[R35] 后台执行并等待
来源：http://cfv.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jin.jianghu66.top

[R36] 并发执行多个任务
来源：http://cob.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aou.jqgfzy.top

[R37] 把输出赋给变量
来源：http://azs.hcnkem.com

files=$(ls -1)
来源：http://znx.aibaodan.cn

[R38] 管道串联
来源：http://kko.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://qgo.hammf.cn

[R39] 重定向标准输出与错误
来源：http://wcu.hysaishi.cn

cmd > out.log 2>&1
来源：http://wmu.cashguo.top

[R40] 追加写日志
来源：http://ywg.hongshengwenyu.top

echo "log" >> out.log
来源：http://mkv.zycfv.cn

[R41] 丢弃输出
来源：http://wcx.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://xqb.snrcjt.cn

[R42] 输入重定向
来源：http://wpa.meibo888.top

wc -l < a.txt
来源：http://kst.ydzc1.top

[R43] 按名字查找文件
来源：http://phd.ppjwa.cn

find . -name "*.log" -type f
来源：http://jsh.kuanghao11.cn

[R44] 按修改时间查找
来源：http://jgi.svipenyu.cn

find . -mtime -7 -type f
来源：http://usq.wangshuangyany.cn

[R45] 批量删除
来源：http://ulp.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://zsw.epnwcf.com

[R46] 递归替换文件内容
来源：http://uge.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qty.zhixingplan.top

[R47] sed 单行替换
来源：http://ryf.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://inc.hysaishi.cn

[R48] awk 取指定列
来源：http://amb.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://jkj.xuanzx.com

[R49] awk 带条件
来源：http://zqa.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqa.xylfe.cn

[R50] awk 求和
来源：http://qxf.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://mbg.gzhubu.top

[R51] 排序去重取前几
来源：http://zpp.zhaomingkeji.xyz


<!-- 参考信息 -->