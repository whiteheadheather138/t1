代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gua.yuanzhike.top

[Q05] 重命名列
来源：http://wmn.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xbs.hongshengwenyu.top

[Q06] 删除列
来源：http://edj.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gus.gaohongyu789.top

[Q07] 删除表
来源：http://pdx.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://rip.tianlin.xyz

[Q08] 创建普通索引
来源：http://npg.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://efi.316326.xyz

[Q09] 创建唯一索引
来源：http://tnk.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://udg.wangshuangyany.cn

[Q10] 插入单行
来源：http://aob.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rxx.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://coi.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uwl.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://yhz.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://wja.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rsy.hfpthk.cn

[Q13] 忽略重复插入
来源：http://taf.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nyd.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://ldp.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://phj.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://evy.meibo888.top

[Q15] 查询全部
来源：http://xab.zycfv.cn

SELECT * FROM users;
来源：http://ooy.xylfe.cn

[Q16] 查询指定列
来源：http://gmw.ivvv.top

SELECT id, name FROM users;
来源：http://oau.guannengcc.top

[Q17] 条件查询
来源：http://ine.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qwa.ivvv.top

[Q18] 模糊匹配
来源：http://vob.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpd.xylfe.cn

[Q19] 范围查询
来源：http://aqz.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lpd.mhx1999.top

[Q20] IN 列表
来源：http://amm.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mpl.hysaishi.cn

[Q21] 空值判断
来源：http://wbc.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ysd.fktsv.cn

[Q22] 排序
来源：http://mgb.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xgd.zdqjudy.top

[Q23] 分页
来源：http://uen.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://knz.hfpthk.cn

[Q24] 去重
来源：http://ncd.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://wdb.sufxvd.cn

[Q25] 只取前 N 条
来源：http://wmt.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gui.ywan-chungtsiang.top

[Q26] 计数
来源：http://xej.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://ljb.316326.xyz

[Q27] 条件计数
来源：http://zxd.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zfg.feifeiyinyue.top

[Q28] 求和与平均
来源：http://vpd.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kph.chenlongwang.top

[Q29] 最大最小值
来源：http://tdd.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://jme.hysaishi.cn

[Q30] 分组统计
来源：http://vpk.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pok.yuxming.cn

[Q31] 分组后过滤
来源：http://fqr.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yql.epnwcf.com

[Q32] 分组拼接字符串
来源：http://hlp.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfc.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pxy.dashuyun.cn

[Q33] 多列分组
来源：http://lma.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qpb.quarkkingdee.top

[Q34] 每组取第一条
来源：http://vgk.havefunace.top

SELECT * FROM (
来源：http://aek.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vgc.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://hns.yj20258888.top

[Q35] 内连接
来源：http://wko.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mwh.shuidangran.top

[Q36] 左连接
来源：http://xtj.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twr.smart0.xyz

[Q37] 右连接
来源：http://chm.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://adz.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wbr.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uhs.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://pqq.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://fka.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ayz.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xpm.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://flx.yuanzhike.top

[Q41] 多表连接
来源：http://sqi.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qgn.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://oeo.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://coi.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://yqu.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://wqq.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zsv.ydjk.org.cn

[Q43] 标量子查询
来源：http://rcv.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aub.hysaishi.cn

[Q44] IN 子查询
来源：http://bop.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bry.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://dub.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jky.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://coz.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ssp.haohaochexian.top

[Q47] 与平均值比较
来源：http://nml.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gxf.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://ygi.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nsw.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://lhh.fengsongda.top

[Q49] 更新单行
来源：http://qmz.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nkm.ppjwa.cn

[Q50] 批量更新
来源：http://arh.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yuf.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://tag.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tno.bbcook.cn

[Q52] 删除指定行
来源：http://aqb.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://los.xylfe.cn

[Q53] 按条件删除
来源：http://vox.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dcn.9152youxi.cn

[Q54] 清空表
来源：http://brf.epnwcf.com

TRUNCATE TABLE logs;
来源：http://qpw.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://yey.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fop.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://bkn.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dmf.xziqi.cn

[Q57] 行号
来源：http://vli.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ytz.kuanghao11.cn

[Q58] 累计求和
来源：http://gau.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pao.chenlongwang.top

[Q59] 分组内累计
来源：http://lug.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ylw.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://yzl.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ybb.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqo.yonumen.top

[Q61] 移动平均
来源：http://xek.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://znr.yfazqb.com

[Q62] 分组占比
来源：http://the.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tuj.redwolf501.top

[Q63] 开启事务
来源：http://cyx.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://yhl.dashuyun.cn

[Q64] 提交事务
来源：http://jry.shangyingyoupin.top

COMMIT;
来源：http://nyd.wangshuangyany.cn

[Q65] 回滚事务
来源：http://uhs.0kj1m.cn

ROLLBACK;
来源：http://txj.yvedp.cn

[Q66] 行锁查询
来源：http://ygh.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fnl.smart0.xyz

[Q67] 设置隔离级别
来源：http://att.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://skz.quarkkingdee.top

[Q68] 保存点
来源：http://ocw.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://hpk.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://dqr.aibaodan.cn

[Q69] 查看执行计划
来源：http://ydm.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://afz.uphjek.com

[Q70] 更新统计信息
来源：http://clo.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://wwh.yj20258888.top

[Q71] 查看建表语句
来源：http://lhg.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lvz.shuidangran.top

[Q72] 查看索引
来源：http://zvh.dianchejie.cn

SHOW INDEX FROM users;
来源：http://cwz.fengsongda.top

[Q73] 查看表状态
来源：http://vlc.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vtu.sxryk.cn

[Q74] 强制使用索引
来源：http://lki.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://avt.vqdsnc.cn

[Q75] 日期格式化
来源：http://iqx.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://seb.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ubr.hfpthk.cn

[Q76] 按天统计
来源：http://dok.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ant.havefunace.top

[Q77] 时间加减
来源：http://xhe.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bgk.bjfxy.top

[Q78] 当前时间
来源：http://efp.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ohq.jqgfzy.top

[Q79] 字符串拼接
来源：http://vzf.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ngz.xylfe.cn

[Q80] 字符串截取
来源：http://srk.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mbs.chenlongwang.top

[Q81] 字符串替换
来源：http://wfe.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aqp.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://exq.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eyf.yj20258888.top

[Q83] 大小写转换
来源：http://jlp.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://euw.tanke756.top

[Q84] 去除首尾空格
来源：http://caq.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://ayk.xinyue.icu

[Q85] 数值取整
来源：http://qzo.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wpy.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://rje.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wue.tanke756.top

[Q87] JSON 字段做条件
来源：http://ies.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hqz.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://jap.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://irm.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qzp.chenzaomai.com

[Q89] 判断表是否存在
来源：http://inr.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sis.ydjk.org.cn

[Q90] 生成序号列
来源：http://hqm.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://umd.xylfe.cn

================================================================================
来源：http://kam.xziqi.cn

R. Bash 专题
来源：http://bns.jinqigufen.top

================================================================================
来源：http://nlg.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://hwa.nwbrower.top

#!/usr/bin/env bash
来源：http://fra.xingfuxueyuan.xyz

set -euo pipefail
来源：http://okn.ppjwa.cn

[R02] 变量赋值与使用
来源：http://dpz.chenzaomai.com

name="Tom"; echo "$name"
来源：http://fhk.yfazqb.com

[R03] 只读变量
来源：http://xrx.0kj1m.cn

readonly PI=3.14
来源：http://aik.shzxlz.cn

[R04] 位置参数
来源：http://xzk.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ylp.ctjpmb.com

[R05] 参数默认值
来源：http://ppo.cashguo.top

name="${1:-default}"
来源：http://aig.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://kmv.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rlb.jianghu66.top

[R07] if 判断文件
来源：http://pbu.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fam.uphjek.com

[R08] 数值比较
来源：http://yqu.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hkr.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://nhd.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wcb.zdbjq.cn

[R10] 正则匹配
来源：http://vnx.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ils.bjfxy.top

[R11] case 多分支
来源：http://hsu.epnwcf.com

case "$1" in
来源：http://xpo.tarul.cn

start) echo "启动" ;;
来源：http://ugx.epnwcf.com

stop)  echo "停止" ;;
来源：http://jvo.yuxming.cn

*)     echo "未知命令" ;;
来源：http://zfl.sweek.top

esac
来源：http://dly.yj20258.top

[R12] for 遍历文件
来源：http://pfk.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://cwg.fehbvm.com

[R13] for 计数循环
来源：http://zvs.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://gmx.meibo888.top

[R14] C 风格 for
来源：http://bph.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cgz.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://dyu.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nqf.hysaishi.cn

[R16] until 等待条件
来源：http://zxu.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ozw.smart0.xyz

[R17] 数组定义与取值
来源：http://ktz.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://yld.jinqigufen.top

[R18] 遍历数组
来源：http://ecn.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ouq.cheryme.top

[R19] 数组长度
来源：http://xqw.vqdsnc.cn

echo "${#arr[@]}"
来源：http://rpi.zdbjq.cn

[R20] 关联数组（字典）
来源：http://jyf.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pki.yj202588.top

[R21] 字符串长度
来源：http://hjh.birdmap.top

echo "${#s}"
来源：http://usw.jianghu66.top

[R22] 截取子串
来源：http://tvr.redwolf501.top

echo "${s:0:5}"
来源：http://qci.shuidangran.top

[R23] 字符串替换
来源：http://iip.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xun.guowangkeji.top

[R24] 大小写转换
来源：http://znc.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://zdt.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://bzf.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ipu.hnxiangtu.top

[R26] 命令替换
来源：http://apn.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://nao.yj20258.top

[R27] 算术展开
来源：http://bof.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://auo.redwolf501.top

[R28] 浮点运算
来源：http://zsr.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://hyf.andypj.xyz

[R29] 定义函数
来源：http://rer.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lph.sxryk.cn

[R30] 函数返回状态码
来源：http://xac.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://ppb.shangyingyoupin.top

[R31] 局部变量
来源：http://rsn.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://xdy.zdbjq.cn

[R32] 参数个数校验
来源：http://waq.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bto.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://yyv.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ylq.fehbvm.com

[R34] 退出时清理
来源：http://byw.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://acf.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://epi.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ame.zhixingplan.top

[R36] 并发执行多个任务
来源：http://mtb.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qqn.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://cso.jqgfzy.top

files=$(ls -1)
来源：http://mix.fktsv.cn

[R38] 管道串联
来源：http://vcw.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://tge.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://niq.hnqzz.top

cmd > out.log 2>&1
来源：http://rvi.hnqzz.top

[R40] 追加写日志
来源：http://lwr.wangdashe.top

echo "log" >> out.log
来源：http://nuz.sjlbkw.cn

[R41] 丢弃输出
来源：http://egy.yvedp.cn

cmd >/dev/null 2>&1
来源：http://jqc.kuanghao11.cn

[R42] 输入重定向
来源：http://pmw.0kj1m.cn

wc -l < a.txt
来源：http://dxz.meibo888.top

[R43] 按名字查找文件
来源：http://eyx.pycfn.com

find . -name "*.log" -type f
来源：http://hff.316326.xyz

[R44] 按修改时间查找
来源：http://xxk.yuanzhike.top

find . -mtime -7 -type f
来源：http://yeh.xziqi.cn

[R45] 批量删除
来源：http://bnl.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://mco.xuanzx.com

[R46] 递归替换文件内容
来源：http://gkv.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fee.cdnleiting.top

[R47] sed 单行替换
来源：http://rrw.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://uas.tianlin.xyz

[R48] awk 取指定列
来源：http://obm.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://ire.yvedp.cn

[R49] awk 带条件
来源：http://mgc.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ton.kuanghao11.cn

[R50] awk 求和
来源：http://bcc.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ilf.ivvv.top

[R51] 排序去重取前几
来源：http://ieb.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oqd.tanke756.top

[R52] 统计行数
来源：http://jdl.feifeiyinyue.top

wc -l a.txt
来源：http://iiu.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://fzc.yj20258.top


<!-- 参考信息 -->