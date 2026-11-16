代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tau.jianghu66.top

user_id INT NOT NULL,
来源：http://xmv.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://wde.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://irk.daria6918.cn

);
来源：http://zub.chenjidiqi.icu

[Q03] 增加列
来源：http://gos.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jff.zhiwuduotai.top

[Q04] 修改列类型
来源：http://ylx.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hlf.ehwqpu.com

[Q05] 重命名列
来源：http://wth.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gmb.chenzaomai.com

[Q06] 删除列
来源：http://xme.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://qtp.zhengqikj.top

[Q07] 删除表
来源：http://buw.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://pqj.hfpthk.cn

[Q08] 创建普通索引
来源：http://zrh.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jwa.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://ujh.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://axy.yuanzhike.top

[Q10] 插入单行
来源：http://ifj.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://esi.yuxming.cn

[Q11] 一次插入多行
来源：http://vsl.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jzr.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://qmn.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://fix.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rvl.daxiang520.top

[Q13] 忽略重复插入
来源：http://tyn.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kon.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://vke.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fek.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://heg.fengsongda.top

[Q15] 查询全部
来源：http://xrc.cqqwz.cn

SELECT * FROM users;
来源：http://dwd.epnwcf.com

[Q16] 查询指定列
来源：http://ubq.nanxinkj.top

SELECT id, name FROM users;
来源：http://obl.c1oappe.top

[Q17] 条件查询
来源：http://sog.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qli.chenlongwang.top

[Q18] 模糊匹配
来源：http://qwn.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jrs.zhiwuduotai.top

[Q19] 范围查询
来源：http://yia.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://een.birdmap.top

[Q20] IN 列表
来源：http://lqi.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oqp.tian-w.cn

[Q21] 空值判断
来源：http://ysi.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bov.pengpengdd.cyou

[Q22] 排序
来源：http://bzd.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kci.sufxvd.cn

[Q23] 分页
来源：http://hmu.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oaw.52xcode.cn

[Q24] 去重
来源：http://rpb.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://sxl.ctjpmb.com

[Q25] 只取前 N 条
来源：http://icj.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://miq.xinyue.icu

[Q26] 计数
来源：http://emb.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://tam.daxiang520.top

[Q27] 条件计数
来源：http://llj.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zky.yanxiufei.cn

[Q28] 求和与平均
来源：http://cau.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kmo.jlsjyb.cn

[Q29] 最大最小值
来源：http://jvq.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tkq.jinqigufen.top

[Q30] 分组统计
来源：http://yiz.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bsi.nwbrower.top

[Q31] 分组后过滤
来源：http://wso.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tbr.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://zdy.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blr.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zcx.cheryme.top

[Q33] 多列分组
来源：http://oxc.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oxe.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://svb.fktsv.cn

SELECT * FROM (
来源：http://amr.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://txj.hfpthk.cn

) t WHERE rn = 1;
来源：http://uui.jinqigfzy.top

[Q35] 内连接
来源：http://gye.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gwh.chenjidiqi.icu

[Q36] 左连接
来源：http://ick.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://crm.hesvh.cn

[Q37] 右连接
来源：http://boe.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://icf.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ciz.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oml.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://xyp.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fck.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pes.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sro.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://keg.ppjwa.cn

[Q41] 多表连接
来源：http://igm.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sgx.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://bhx.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://ulo.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://uuy.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://qhw.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ebn.hywenlv.cn

[Q43] 标量子查询
来源：http://cqw.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yuu.jiagoushi.top

[Q44] IN 子查询
来源：http://dim.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nys.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://xex.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ycg.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://jcp.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exp.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://nwu.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jfy.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://uas.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fhx.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://nuj.hysaishi.cn

[Q49] 更新单行
来源：http://xag.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lar.daria6918.cn

[Q50] 批量更新
来源：http://vrg.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://had.0kj1m.cn

[Q51] 用子查询更新
来源：http://zqh.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ote.gotoacloud.top

[Q52] 删除指定行
来源：http://rtw.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://jur.bbcook.cn

[Q53] 按条件删除
来源：http://kce.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://inh.chenzaomai.com

[Q54] 清空表
来源：http://xdu.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://nbc.havefunace.top

[Q55] 排名（并列占位）
来源：http://eqn.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zfu.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://xoj.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bhl.bbcook.cn

[Q57] 行号
来源：http://tlt.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yqw.jinqigfzy.top

[Q58] 累计求和
来源：http://dpu.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cdj.vehdjk.com

[Q59] 分组内累计
来源：http://eaz.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eev.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://zem.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ipo.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hae.yanxiufei.cn

[Q61] 移动平均
来源：http://qtd.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qoa.yanxiufei.cn

[Q62] 分组占比
来源：http://lxi.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dhm.meibo888.top

[Q63] 开启事务
来源：http://jrd.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eta.birdmap.top

[Q64] 提交事务
来源：http://jeu.wangshuangyany.cn

COMMIT;
来源：http://ukk.vehdjk.com

[Q65] 回滚事务
来源：http://ply.havefunace.top

ROLLBACK;
来源：http://pua.smart0.xyz

[Q66] 行锁查询
来源：http://ful.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jzx.fktsv.cn

[Q67] 设置隔离级别
来源：http://kpr.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qcz.c1oappe.top

[Q68] 保存点
来源：http://xqp.yuxming.cn

SAVEPOINT sp1;
来源：http://dmj.haohaochexian.top

ROLLBACK TO sp1;
来源：http://rwm.yuxming.cn

[Q69] 查看执行计划
来源：http://szx.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://atj.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://ysa.cheryme.top

ANALYZE TABLE users;
来源：http://byx.yj20258888.top

[Q71] 查看建表语句
来源：http://gzc.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fib.uphjek.com

[Q72] 查看索引
来源：http://nlz.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://vyn.jqgufenzy.top

[Q73] 查看表状态
来源：http://tam.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pdj.jinqigufen.top

[Q74] 强制使用索引
来源：http://cdv.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mxs.yuxming.cn

[Q75] 日期格式化
来源：http://abh.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yqu.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vyr.quarkkingdee.top

[Q76] 按天统计
来源：http://ama.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyn.nwbrower.top

[Q77] 时间加减
来源：http://hkx.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lzl.uphjek.com

[Q78] 当前时间
来源：http://dng.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ufy.yongpay.top

[Q79] 字符串拼接
来源：http://syd.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ijg.yonumen.top

[Q80] 字符串截取
来源：http://eno.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qil.cdnleiting.top

[Q81] 字符串替换
来源：http://xcc.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gms.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://pyj.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hpi.ydzc1.top

[Q83] 大小写转换
来源：http://ohq.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kgr.yangfankeji.com

[Q84] 去除首尾空格
来源：http://ouz.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://nxh.ydjk.org.cn

[Q85] 数值取整
来源：http://qfa.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iyt.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://jwi.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pbq.hcnkem.com

[Q87] JSON 字段做条件
来源：http://ahy.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sqo.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://udy.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jtu.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jsp.sysykeji.top

[Q89] 判断表是否存在
来源：http://znz.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uir.zhiwuduotai.top

[Q90] 生成序号列
来源：http://fgw.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zbc.wangdashe.top

================================================================================
来源：http://vrk.9152youxi.cn

R. Bash 专题
来源：http://wtw.smart0.xyz

================================================================================
来源：http://ucm.aibaodan.cn

[R01] shebang 与严格模式
来源：http://pyh.dianchejie.cn

#!/usr/bin/env bash
来源：http://slc.zhaomingkeji.xyz

set -euo pipefail
来源：http://yfo.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://iyz.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://vcz.zhoulong.xyz

[R03] 只读变量
来源：http://eem.chenzaomai.com

readonly PI=3.14
来源：http://mxb.xinyue.icu

[R04] 位置参数
来源：http://jea.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://puf.ybcxt.top

[R05] 参数默认值
来源：http://lap.daxiang520.top

name="${1:-default}"
来源：http://qte.316326.xyz

[R06] 判断命令是否存在
来源：http://heu.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcc.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://whh.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tgi.zhongyouzk.top

[R08] 数值比较
来源：http://lue.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ygl.xinyue.icu

[R09] 字符串比较
来源：http://glv.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wun.snrcjt.cn

[R10] 正则匹配
来源：http://vpw.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fuk.redwolf501.top

[R11] case 多分支
来源：http://zfp.andypj.xyz

case "$1" in
来源：http://icb.sjlbkw.cn

start) echo "启动" ;;
来源：http://cee.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://wbh.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://kaa.fzhhl.top

esac
来源：http://tzj.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://mbw.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://kai.shanyushiyangtech.top

[R13] for 计数循环
来源：http://ngc.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://cht.wangdashe.top

[R14] C 风格 for
来源：http://wbd.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zsm.shuidangran.top

[R15] while 逐行读文件
来源：http://dcx.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bjn.smart0.xyz

[R16] until 等待条件
来源：http://nfi.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ytx.shzxlz.cn

[R17] 数组定义与取值
来源：http://idd.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xey.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://pxo.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://opy.jiagoushi.top

[R19] 数组长度
来源：http://ibq.daria6918.cn

echo "${#arr[@]}"
来源：http://lks.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://sga.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lmx.sysykeji.top

[R21] 字符串长度
来源：http://jzs.andypj.xyz

echo "${#s}"
来源：http://aqz.0kj1m.cn

[R22] 截取子串
来源：http://hpb.hnxiangtu.top

echo "${s:0:5}"
来源：http://ivr.svipenyu.cn

[R23] 字符串替换
来源：http://zza.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ojh.cheryme.top

[R24] 大小写转换
来源：http://qzw.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://tee.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://lxz.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iqk.ctjpmb.com

[R26] 命令替换
来源：http://zkl.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://fqk.yj202588.top

[R27] 算术展开
来源：http://lod.yvedp.cn

echo $((1 + 2 * 3))
来源：http://jsp.yfazqb.com

[R28] 浮点运算
来源：http://kme.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://ium.tarul.cn

[R29] 定义函数
来源：http://mja.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ixr.hysaishi.cn

[R30] 函数返回状态码
来源：http://dun.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://ver.shanyushiyangkeji.top

[R31] 局部变量
来源：http://rng.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://vcy.316326.xyz

[R32] 参数个数校验
来源：http://rsv.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dug.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://ryx.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://afn.hammf.cn

[R34] 退出时清理
来源：http://qno.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fth.zdbjq.cn

[R35] 后台执行并等待
来源：http://khn.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://slr.fktsv.cn

[R36] 并发执行多个任务
来源：http://saq.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mra.ppjwa.cn

[R37] 把输出赋给变量
来源：http://whp.yj20258.top

files=$(ls -1)
来源：http://hba.sysykeji.top

[R38] 管道串联
来源：http://lbz.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://shn.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://gdc.smart0.xyz

cmd > out.log 2>&1
来源：http://wfk.fzhhl.top

[R40] 追加写日志
来源：http://rby.epnwcf.com

echo "log" >> out.log
来源：http://tgr.yuanzhike.top

[R41] 丢弃输出
来源：http://cxq.yj20258888.top

cmd >/dev/null 2>&1
来源：http://use.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://ewt.jinghuilouyu.cn

wc -l < a.txt
来源：http://lfn.hysaishi.cn

[R43] 按名字查找文件
来源：http://jxm.jianghu66.top

find . -name "*.log" -type f
来源：http://zom.sxryk.cn

[R44] 按修改时间查找
来源：http://ugv.hfpthk.cn

find . -mtime -7 -type f
来源：http://rav.shanyushiyangkeji.top

[R45] 批量删除
来源：http://cjf.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://zrn.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://sby.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nge.ehwqpu.com

[R47] sed 单行替换
来源：http://qqp.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mgt.jqgufenzy.top

[R48] awk 取指定列
来源：http://arg.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://wdi.jqgfzy.top

[R49] awk 带条件
来源：http://tti.mhx1999.top


<!-- 参考信息 -->