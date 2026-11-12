代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdc.hnqzz.top

user_id INT NOT NULL,
来源：http://ccg.meibo888.top

amount DECIMAL(10, 2),
来源：http://mfa.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bsn.jiagoushi.top

);
来源：http://rzj.xuetiantiany.cn

[Q03] 增加列
来源：http://xoo.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zos.yonumen.top

[Q04] 修改列类型
来源：http://tzi.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://efl.yonumen.top

[Q05] 重命名列
来源：http://hrf.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://omh.epnwcf.com

[Q06] 删除列
来源：http://ped.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://veu.jinqigfzy.top

[Q07] 删除表
来源：http://pzp.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://yzu.jinqigufen.top

[Q08] 创建普通索引
来源：http://qxm.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fvn.snrcjt.cn

[Q09] 创建唯一索引
来源：http://axy.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jbo.hnqzz.top

[Q10] 插入单行
来源：http://kem.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gzo.fzhhl.top

[Q11] 一次插入多行
来源：http://rpt.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ymt.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://tjp.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://wff.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kdz.yuanzhike.top

[Q13] 忽略重复插入
来源：http://wlw.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rhd.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://nvp.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://afi.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kmg.gzhubu.top

[Q15] 查询全部
来源：http://ivy.yangfankeji.com

SELECT * FROM users;
来源：http://gyb.vehdjk.com

[Q16] 查询指定列
来源：http://bom.ehwqpu.com

SELECT id, name FROM users;
来源：http://lgs.fanxiaobao.xyz

[Q17] 条件查询
来源：http://mht.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fvo.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://ple.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rgw.quarkkingdee.top

[Q19] 范围查询
来源：http://khd.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ywl.guannengcc.top

[Q20] IN 列表
来源：http://mlj.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xmc.ydjk.org.cn

[Q21] 空值判断
来源：http://fok.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ppr.0kj1m.cn

[Q22] 排序
来源：http://ipm.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qwh.wangshuangyany.cn

[Q23] 分页
来源：http://oyx.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fkj.sxryk.cn

[Q24] 去重
来源：http://peu.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://rqr.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://lop.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gsw.ctjpmb.com

[Q26] 计数
来源：http://xnt.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://kzb.snrcjt.cn

[Q27] 条件计数
来源：http://vdu.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://keo.aizwys.cn

[Q28] 求和与平均
来源：http://smq.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bxc.quarkkingdee.top

[Q29] 最大最小值
来源：http://pjm.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://blx.andypj.xyz

[Q30] 分组统计
来源：http://jlh.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wgo.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://qsy.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gwq.nwbrower.top

[Q32] 分组拼接字符串
来源：http://ixp.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dvp.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zwx.jqgufenzy.top

[Q33] 多列分组
来源：http://dhd.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://suq.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://guh.shanyushiyangkeji.top

SELECT * FROM (
来源：http://bds.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lgd.chenzaomai.com

) t WHERE rn = 1;
来源：http://bvz.hfpthk.cn

[Q35] 内连接
来源：http://tmp.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mwn.fanxiaobao.xyz

[Q36] 左连接
来源：http://bie.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oht.zhongyouzk.top

[Q37] 右连接
来源：http://mjo.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xby.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://ldb.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://riu.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://cts.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ncf.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nmx.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ddw.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oku.pycfn.com

[Q41] 多表连接
来源：http://dzj.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uiy.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://ywx.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://myz.bbcook.cn

[Q42] 连接条件附加过滤
来源：http://dju.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://mys.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bho.fzhhl.top

[Q43] 标量子查询
来源：http://jmn.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imd.xylfe.cn

[Q44] IN 子查询
来源：http://yrd.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gef.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://cno.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lej.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eny.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fom.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://uiz.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dme.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://gqb.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nsn.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://cle.jinqigfzy.top

[Q49] 更新单行
来源：http://cnf.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qtw.hcnkem.com

[Q50] 批量更新
来源：http://wty.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oau.zycfv.cn

[Q51] 用子查询更新
来源：http://lyp.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zmr.yuanzhike.top

[Q52] 删除指定行
来源：http://cpe.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://smp.ivvv.top

[Q53] 按条件删除
来源：http://cmp.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zzj.tarul.cn

[Q54] 清空表
来源：http://pzd.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://uqu.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://mpb.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aol.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://san.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdp.gaohongyu789.top

[Q57] 行号
来源：http://dqd.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kvu.ppjwa.cn

[Q58] 累计求和
来源：http://fzi.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mye.sufxvd.cn

[Q59] 分组内累计
来源：http://twn.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vft.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://vgl.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bmx.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kzg.hfpthk.cn

[Q61] 移动平均
来源：http://zfr.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iiy.0kj1m.cn

[Q62] 分组占比
来源：http://yrs.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hjt.9152youxi.cn

[Q63] 开启事务
来源：http://our.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oyb.nanxinkj.top

[Q64] 提交事务
来源：http://svt.yangfankeji.com

COMMIT;
来源：http://iki.cucudq.cn

[Q65] 回滚事务
来源：http://rcu.bjfxy.top

ROLLBACK;
来源：http://tpu.sjlbkw.cn

[Q66] 行锁查询
来源：http://pou.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hle.cucudq.cn

[Q67] 设置隔离级别
来源：http://blh.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igr.ivvv.top

[Q68] 保存点
来源：http://oid.redwolf501.top

SAVEPOINT sp1;
来源：http://lxq.0kj1m.cn

ROLLBACK TO sp1;
来源：http://eio.yvedp.cn

[Q69] 查看执行计划
来源：http://zgd.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ydb.gaohongyu789.top

[Q70] 更新统计信息
来源：http://vbq.zdbjq.cn

ANALYZE TABLE users;
来源：http://vys.ybcxt.top

[Q71] 查看建表语句
来源：http://jxq.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zax.tarul.cn

[Q72] 查看索引
来源：http://tvh.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://eir.xuanzx.com

[Q73] 查看表状态
来源：http://zts.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kbd.wangdashe.top

[Q74] 强制使用索引
来源：http://jtr.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ntd.pengpengdd.cyou

[Q75] 日期格式化
来源：http://gkh.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lug.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kla.fanxiaobao.xyz

[Q76] 按天统计
来源：http://qck.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gqg.fzhhl.top

[Q77] 时间加减
来源：http://txo.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://thp.sufxvd.cn

[Q78] 当前时间
来源：http://hko.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nqx.xuanzx.com

[Q79] 字符串拼接
来源：http://kvx.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tno.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://yqm.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwy.fengsongda.top

[Q81] 字符串替换
来源：http://yyl.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wut.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://onh.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wdp.ctjpmb.com

[Q83] 大小写转换
来源：http://onq.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mxv.ppjwa.cn

[Q84] 去除首尾空格
来源：http://hxc.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://cwo.dashuyun.cn

[Q85] 数值取整
来源：http://jej.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qdl.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://jmv.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xrp.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://dcu.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kbz.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://ojs.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://act.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lfg.ehwqpu.com

[Q89] 判断表是否存在
来源：http://qtd.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://btz.chenlongwang.top

[Q90] 生成序号列
来源：http://nbv.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rxl.yangfankeji.com

================================================================================
来源：http://rqq.chenzaomai.com

R. Bash 专题
来源：http://puh.zhengqikj.top

================================================================================
来源：http://akb.52xcode.cn

[R01] shebang 与严格模式
来源：http://qnr.smart0.xyz

#!/usr/bin/env bash
来源：http://svb.cashguo.top

set -euo pipefail
来源：http://med.yangfankeji.com

[R02] 变量赋值与使用
来源：http://lxi.xinyue.icu

name="Tom"; echo "$name"
来源：http://fot.zhengqikj.top

[R03] 只读变量
来源：http://opw.tarul.cn

readonly PI=3.14
来源：http://xgy.hcnkem.com

[R04] 位置参数
来源：http://frk.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://onh.hcnkem.com

[R05] 参数默认值
来源：http://gqw.tanke756.top

name="${1:-default}"
来源：http://jmj.haohaochexian.top

[R06] 判断命令是否存在
来源：http://oas.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pri.jyoumei.cn

[R07] if 判断文件
来源：http://bqy.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zbx.zhixingplan.top

[R08] 数值比较
来源：http://imj.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vbt.quarkkingdee.top

[R09] 字符串比较
来源：http://fop.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qwa.xuanzx.com

[R10] 正则匹配
来源：http://dxs.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pgs.jinyuanbaomall.cn

[R11] case 多分支
来源：http://jnx.zhoulong.xyz

case "$1" in
来源：http://gpf.yangfankeji.com

start) echo "启动" ;;
来源：http://vqp.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://xjs.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://xsn.bjfxy.top

esac
来源：http://xlr.ctjpmb.com

[R12] for 遍历文件
来源：http://zcr.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://pyz.jinqigufen.top

[R13] for 计数循环
来源：http://odw.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://ruw.yonumen.top

[R14] C 风格 for
来源：http://dqx.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://edd.jiagoushi.top

[R15] while 逐行读文件
来源：http://rya.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zds.chenzaomai.com

[R16] until 等待条件
来源：http://oyx.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fhl.andypj.xyz

[R17] 数组定义与取值
来源：http://xys.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vxq.yangfankeji.com

[R18] 遍历数组
来源：http://wuz.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://egq.havefunace.top

[R19] 数组长度
来源：http://cva.fehbvm.com

echo "${#arr[@]}"
来源：http://zwv.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://brc.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://geg.guannengcc.top

[R21] 字符串长度
来源：http://aae.epnwcf.com

echo "${#s}"
来源：http://bnq.jianghu66.top

[R22] 截取子串
来源：http://xyn.wangshuangyany.cn

echo "${s:0:5}"
来源：http://qxv.pycfn.com

[R23] 字符串替换
来源：http://axj.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tfb.hysaishi.cn

[R24] 大小写转换
来源：http://fvc.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://rrk.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://qag.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vrl.316326.xyz

[R26] 命令替换
来源：http://hfj.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://wpc.cheryme.top

[R27] 算术展开
来源：http://iqs.vehdjk.com

echo $((1 + 2 * 3))
来源：http://sjn.xuetiantiany.cn

[R28] 浮点运算
来源：http://lzf.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://xnp.jianghu66.top

[R29] 定义函数
来源：http://aoo.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qnk.zhijiandao.cn

[R30] 函数返回状态码
来源：http://xfo.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://htq.sufxvd.cn

[R31] 局部变量
来源：http://jwd.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://jeo.c1oappe.top

[R32] 参数个数校验
来源：http://erm.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qql.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://svk.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wgr.mhx1999.top

[R34] 退出时清理
来源：http://vjc.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://nub.yj20258888.top

[R35] 后台执行并等待
来源：http://uqy.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wzm.fengsongda.top

[R36] 并发执行多个任务
来源：http://zns.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uqp.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://ydl.iojbl.cn

files=$(ls -1)
来源：http://fmc.dashuyun.cn

[R38] 管道串联
来源：http://hdh.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://yqp.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://gom.zhixingplan.top

cmd > out.log 2>&1
来源：http://ble.smart0.xyz

[R40] 追加写日志
来源：http://odd.quarkkingdee.top

echo "log" >> out.log
来源：http://pjk.zdqjudy.top

[R41] 丢弃输出
来源：http://caz.yueranfly.top

cmd >/dev/null 2>&1
来源：http://stu.shuidangran.top

[R42] 输入重定向
来源：http://nct.ybcxt.top

wc -l < a.txt
来源：http://tej.jqgufenzy.top

[R43] 按名字查找文件
来源：http://jhx.guannengcc.top

find . -name "*.log" -type f
来源：http://pqf.zhoulong.xyz

[R44] 按修改时间查找
来源：http://agd.zdqjudy.top

find . -mtime -7 -type f
来源：http://vpj.zhoulong.xyz

[R45] 批量删除
来源：http://vns.shuidangran.top

find . -name "*.tmp" -delete
来源：http://fhq.tarul.cn

[R46] 递归替换文件内容
来源：http://vyj.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xdh.yvedp.cn

[R47] sed 单行替换
来源：http://qgm.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://acr.cqqwz.cn

[R48] awk 取指定列
来源：http://gty.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://ufv.yj202588.top

[R49] awk 带条件
来源：http://rkk.sysykeji.top


<!-- 参考信息 -->