代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dnj.sweek.top

[Q05] 重命名列
来源：http://vvv.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldf.pycfn.com

[Q06] 删除列
来源：http://ptq.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ovs.hnqzz.top

[Q07] 删除表
来源：http://zsj.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://dxn.52xcode.cn

[Q08] 创建普通索引
来源：http://ryj.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://zku.gotoacloud.top

[Q09] 创建唯一索引
来源：http://xzg.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vwk.nanxuanxn.top

[Q10] 插入单行
来源：http://hjg.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://obe.bbcook.cn

[Q11] 一次插入多行
来源：http://sds.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vcv.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://mbz.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://uuw.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zli.52xcode.cn

[Q13] 忽略重复插入
来源：http://uav.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mao.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://irf.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://toj.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ibz.dianchejie.cn

[Q15] 查询全部
来源：http://nja.0kj1m.cn

SELECT * FROM users;
来源：http://hyl.bbcook.cn

[Q16] 查询指定列
来源：http://ube.yonumen.top

SELECT id, name FROM users;
来源：http://gxk.xziqi.cn

[Q17] 条件查询
来源：http://rbl.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://onv.wangdashe.top

[Q18] 模糊匹配
来源：http://bgn.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdz.dianchejie.cn

[Q19] 范围查询
来源：http://xkg.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zfl.yfazqb.com

[Q20] IN 列表
来源：http://ssn.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nsl.zycfv.cn

[Q21] 空值判断
来源：http://ijp.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://klm.tarul.cn

[Q22] 排序
来源：http://ibd.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tfm.yfazqb.com

[Q23] 分页
来源：http://ufv.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yta.nwbrower.top

[Q24] 去重
来源：http://lqm.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://lcp.mhx1999.top

[Q25] 只取前 N 条
来源：http://quo.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oqk.pengpengdd.cyou

[Q26] 计数
来源：http://mdm.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://aag.yongpay.top

[Q27] 条件计数
来源：http://dtn.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lym.yj202588.top

[Q28] 求和与平均
来源：http://ltx.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wiu.cashguo.top

[Q29] 最大最小值
来源：http://jzn.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hfx.bjfxy.top

[Q30] 分组统计
来源：http://tzs.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vca.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://zdf.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rpt.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://avq.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lim.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://myx.hywenlv.cn

[Q33] 多列分组
来源：http://zbj.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mgz.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://zoa.vehdjk.com

SELECT * FROM (
来源：http://kxw.smart0.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://szs.jqgfzy.top

) t WHERE rn = 1;
来源：http://xcf.tianlin.xyz

[Q35] 内连接
来源：http://nzo.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hns.fanxiaobao.xyz

[Q36] 左连接
来源：http://bvt.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tmh.cashguo.top

[Q37] 右连接
来源：http://cev.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tao.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dir.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kiv.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://nkt.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dwc.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pli.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://szt.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mgc.zhixingplan.top

[Q41] 多表连接
来源：http://abj.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ipx.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://hjm.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://frr.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://jfl.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://nmb.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mwf.andypj.xyz

[Q43] 标量子查询
来源：http://wfw.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xfw.dianchejie.cn

[Q44] IN 子查询
来源：http://tfb.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jio.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://itp.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhr.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sxn.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pof.hammf.cn

[Q47] 与平均值比较
来源：http://yqp.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nbi.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://omb.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzm.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://rbf.dianchejie.cn

[Q49] 更新单行
来源：http://els.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gaq.gaohongyu789.top

[Q50] 批量更新
来源：http://vxa.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nly.yangfankeji.com

[Q51] 用子查询更新
来源：http://rqx.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aoc.meibo888.top

[Q52] 删除指定行
来源：http://pwk.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://uoa.cheryme.top

[Q53] 按条件删除
来源：http://xcp.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xda.zhaomingkeji.xyz

[Q54] 清空表
来源：http://zjm.epnwcf.com

TRUNCATE TABLE logs;
来源：http://srr.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://wot.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://udn.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://xvl.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fkv.fanxiaobao.xyz

[Q57] 行号
来源：http://tom.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qfl.nanxuanxn.top

[Q58] 累计求和
来源：http://fdv.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pio.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://gar.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xkt.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://hac.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zua.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://njs.uphjek.com

[Q61] 移动平均
来源：http://jul.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eny.jiagoushi.top

[Q62] 分组占比
来源：http://myy.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pga.jlsjyb.cn

[Q63] 开启事务
来源：http://pgk.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wvf.jinghuilouyu.cn

[Q64] 提交事务
来源：http://rbu.tian-w.cn

COMMIT;
来源：http://ipq.meibo888.top

[Q65] 回滚事务
来源：http://own.iojbl.cn

ROLLBACK;
来源：http://egp.sweek.top

[Q66] 行锁查询
来源：http://kww.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://whr.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://mui.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mjn.sysykeji.top

[Q68] 保存点
来源：http://wak.hammf.cn

SAVEPOINT sp1;
来源：http://ztx.sufxvd.cn

ROLLBACK TO sp1;
来源：http://ogc.yonumen.top

[Q69] 查看执行计划
来源：http://hlw.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wym.jlsjyb.cn

[Q70] 更新统计信息
来源：http://cyr.yvedp.cn

ANALYZE TABLE users;
来源：http://ejz.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://giz.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xma.quarkkingdee.top

[Q72] 查看索引
来源：http://hyr.yvedp.cn

SHOW INDEX FROM users;
来源：http://ihd.zhoulong.xyz

[Q73] 查看表状态
来源：http://ywq.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oyw.snrcjt.cn

[Q74] 强制使用索引
来源：http://kwv.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vib.fehbvm.com

[Q75] 日期格式化
来源：http://qjc.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nky.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nlh.yongpay.top

[Q76] 按天统计
来源：http://lxk.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dxz.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://dlj.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tfk.c1oappe.top

[Q78] 当前时间
来源：http://qbl.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ssh.gotoacloud.top

[Q79] 字符串拼接
来源：http://uda.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nne.hesvh.cn

[Q80] 字符串截取
来源：http://exv.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gvx.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://ssx.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cxb.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://crf.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yhy.epnwcf.com

[Q83] 大小写转换
来源：http://xou.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pkz.sweek.top

[Q84] 去除首尾空格
来源：http://von.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://sog.chenlongwang.top

[Q85] 数值取整
来源：http://fia.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zot.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://aug.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uid.nwbrower.top

[Q87] JSON 字段做条件
来源：http://wuh.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dwf.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://smn.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://frs.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iyz.sufxvd.cn

[Q89] 判断表是否存在
来源：http://bwp.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xzq.fzhhl.top

[Q90] 生成序号列
来源：http://bcr.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oxx.yfazqb.com

================================================================================
来源：http://qpa.wangdashe.top

R. Bash 专题
来源：http://lby.xuetiantiany.cn

================================================================================
来源：http://idz.hfpthk.cn

[R01] shebang 与严格模式
来源：http://mvi.52xcode.cn

#!/usr/bin/env bash
来源：http://nxr.uphjek.com

set -euo pipefail
来源：http://cwg.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://amp.yj202588.top

name="Tom"; echo "$name"
来源：http://psc.gaohongyu789.top

[R03] 只读变量
来源：http://cgk.nwbrower.top

readonly PI=3.14
来源：http://moi.316326.xyz

[R04] 位置参数
来源：http://mey.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://spy.hongshengwenyu.top

[R05] 参数默认值
来源：http://wid.jiagoushi.top

name="${1:-default}"
来源：http://dbp.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://rir.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qoy.hammf.cn

[R07] if 判断文件
来源：http://dnw.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vqa.shanyushiyangkeji.top

[R08] 数值比较
来源：http://gor.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jno.hammf.cn

[R09] 字符串比较
来源：http://flk.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hky.sufxvd.cn

[R10] 正则匹配
来源：http://amv.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ozs.xziqi.cn

[R11] case 多分支
来源：http://mej.shanyushiyangtech.top

case "$1" in
来源：http://kcp.pycfn.com

start) echo "启动" ;;
来源：http://ygm.smart0.xyz

stop)  echo "停止" ;;
来源：http://jgs.hammf.cn

*)     echo "未知命令" ;;
来源：http://xta.ivvv.top

esac
来源：http://lit.hnxiangtu.top

[R12] for 遍历文件
来源：http://wjq.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://ywi.jinqigfzy.top

[R13] for 计数循环
来源：http://bqu.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://ldc.tarul.cn

[R14] C 风格 for
来源：http://csa.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cmo.jinqigfzy.top

[R15] while 逐行读文件
来源：http://cho.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mxl.jyoumei.cn

[R16] until 等待条件
来源：http://bqd.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qbj.hnxiangtu.top

[R17] 数组定义与取值
来源：http://dnf.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wpy.snrcjt.cn

[R18] 遍历数组
来源：http://ddn.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://trc.jinqigfzy.top

[R19] 数组长度
来源：http://gol.epnwcf.com

echo "${#arr[@]}"
来源：http://smt.0kj1m.cn

[R20] 关联数组（字典）
来源：http://ahs.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rkv.bjfxy.top

[R21] 字符串长度
来源：http://obc.yongpay.top

echo "${#s}"
来源：http://qrv.cdnleiting.top

[R22] 截取子串
来源：http://owc.guannengcc.top

echo "${s:0:5}"
来源：http://vkq.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://aqe.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://odo.nwbrower.top

[R24] 大小写转换
来源：http://dtv.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://igf.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://ejr.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jjy.xziqi.cn

[R26] 命令替换
来源：http://rri.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://awu.hnqzz.top

[R27] 算术展开
来源：http://zcv.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://cgq.cashguo.top

[R28] 浮点运算
来源：http://oko.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://oau.dianchejie.cn

[R29] 定义函数
来源：http://hll.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wra.yj20258888.top

[R30] 函数返回状态码
来源：http://azg.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://cih.vqdsnc.cn

[R31] 局部变量
来源：http://lvw.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://zro.hesvh.cn

[R32] 参数个数校验
来源：http://zcb.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mug.meibo888.top

[R33] 捕获错误并提示行号
来源：http://lxm.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jga.9152youxi.cn

[R34] 退出时清理
来源：http://wmm.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jrq.tianlin.xyz

[R35] 后台执行并等待
来源：http://crb.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jmj.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://nsx.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kbj.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://dva.pycfn.com

files=$(ls -1)
来源：http://gft.zhaomingkeji.xyz

[R38] 管道串联
来源：http://emn.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://qau.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://zpr.yj20258888.top

cmd > out.log 2>&1
来源：http://yya.vqdsnc.cn

[R40] 追加写日志
来源：http://pur.jianghu66.top

echo "log" >> out.log
来源：http://eat.kuanghao11.cn

[R41] 丢弃输出
来源：http://cxt.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://odz.jinghuilouyu.cn

[R42] 输入重定向
来源：http://utx.cheryme.top

wc -l < a.txt
来源：http://snw.hammf.cn

[R43] 按名字查找文件
来源：http://hzt.jqgfzy.top

find . -name "*.log" -type f
来源：http://egj.pycfn.com

[R44] 按修改时间查找
来源：http://jtj.nanxuanxn.top

find . -mtime -7 -type f
来源：http://edp.jinghuilouyu.cn

[R45] 批量删除
来源：http://xke.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://xnl.bbcook.cn

[R46] 递归替换文件内容
来源：http://fdu.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kfm.zdbjq.cn

[R47] sed 单行替换
来源：http://sbq.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://cko.xziqi.cn

[R48] awk 取指定列
来源：http://ibq.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://gik.zdbjq.cn

[R49] awk 带条件
来源：http://nob.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://guq.gotoacloud.top

[R50] awk 求和
来源：http://ssw.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://iaa.jqgfzy.top

[R51] 排序去重取前几
来源：http://hpb.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://krj.zhoulong.xyz

[R52] 统计行数
来源：http://oma.fengsongda.top

wc -l a.txt
来源：http://nwm.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://boe.ivvv.top


<!-- 参考信息 -->