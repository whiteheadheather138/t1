代发 wailian999

);
来源：http://nrl.smart0.xyz

[Q03] 增加列
来源：http://vxc.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://htr.fzhhl.top

[Q04] 修改列类型
来源：http://fzv.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hza.shanyushiyangtech.top

[Q05] 重命名列
来源：http://sga.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://utl.uphjek.com

[Q06] 删除列
来源：http://irj.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://dnc.zhijiandao.cn

[Q07] 删除表
来源：http://zuu.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://nbq.bbcook.cn

[Q08] 创建普通索引
来源：http://lxj.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mch.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://iob.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xia.cucudq.cn

[Q10] 插入单行
来源：http://nii.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zwh.0kj1m.cn

[Q11] 一次插入多行
来源：http://zxd.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fku.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://ykp.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://sjk.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://air.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://snq.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://chk.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://lhx.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mfj.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://boe.jiagoushi.top

[Q15] 查询全部
来源：http://out.sjlbkw.cn

SELECT * FROM users;
来源：http://toi.snrcjt.cn

[Q16] 查询指定列
来源：http://bpl.yongpay.top

SELECT id, name FROM users;
来源：http://ivl.zhiwuduotai.top

[Q17] 条件查询
来源：http://gqf.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rkj.zhoulong.xyz

[Q18] 模糊匹配
来源：http://kpm.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sik.yj20258888.top

[Q19] 范围查询
来源：http://nkz.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://skr.mhx1999.top

[Q20] IN 列表
来源：http://bba.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iif.andypj.xyz

[Q21] 空值判断
来源：http://nlv.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gjt.chenlongwang.top

[Q22] 排序
来源：http://haj.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aoj.cheryme.top

[Q23] 分页
来源：http://hwg.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzu.zhoulong.xyz

[Q24] 去重
来源：http://dwm.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://gmo.pycfn.com

[Q25] 只取前 N 条
来源：http://epn.ywan-chungtsiang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jst.cheryme.top

[Q26] 计数
来源：http://sfx.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://pwd.uphjek.com

[Q27] 条件计数
来源：http://mnb.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gci.sysykeji.top

[Q28] 求和与平均
来源：http://tco.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yuu.pengpengdd.cyou

[Q29] 最大最小值
来源：http://snh.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixa.guowangkeji.top

[Q30] 分组统计
来源：http://ncl.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vsn.quarkkingdee.top

[Q31] 分组后过滤
来源：http://she.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bqb.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://nvo.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eqt.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iue.ivvv.top

[Q33] 多列分组
来源：http://eyg.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eqx.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://hep.nanxuanxn.top

SELECT * FROM (
来源：http://bqr.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vdy.hesvh.cn

) t WHERE rn = 1;
来源：http://pdw.c1oappe.top

[Q35] 内连接
来源：http://saj.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yga.uphjek.com

[Q36] 左连接
来源：http://ahw.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jht.shanyushiyangtech.top

[Q37] 右连接
来源：http://xua.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sjf.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://prq.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ybb.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://wwl.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://col.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vjh.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jxb.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sxa.tianlin.xyz

[Q41] 多表连接
来源：http://kvp.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://syy.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://jgt.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://aet.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://nay.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://mrx.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vlk.zhengqikj.top

[Q43] 标量子查询
来源：http://klb.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rlq.sjlbkw.cn

[Q44] IN 子查询
来源：http://uxq.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dvs.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://hht.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aax.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://qrj.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gwn.jinqigufen.top

[Q47] 与平均值比较
来源：http://fcv.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tjg.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://gse.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fmn.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://ukn.zhijiandao.cn

[Q49] 更新单行
来源：http://oqs.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ufv.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://iar.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hdl.xylfe.cn

[Q51] 用子查询更新
来源：http://avp.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fcr.haohaochexian.top

[Q52] 删除指定行
来源：http://srx.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://ymt.vehdjk.com

[Q53] 按条件删除
来源：http://urf.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cya.hammf.cn

[Q54] 清空表
来源：http://lgd.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://dmn.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://ksp.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tli.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://gfn.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rvw.yvedp.cn

[Q57] 行号
来源：http://ujy.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://igr.zhoulong.xyz

[Q58] 累计求和
来源：http://wnl.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mby.cashguo.top

[Q59] 分组内累计
来源：http://igt.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iqy.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://xdm.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rxo.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rys.shzxlz.cn

[Q61] 移动平均
来源：http://cqc.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://say.hcnkem.com

[Q62] 分组占比
来源：http://oap.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hqu.meibo888.top

[Q63] 开启事务
来源：http://inz.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xdq.ydjk.org.cn

[Q64] 提交事务
来源：http://pfy.ydzc1.top

COMMIT;
来源：http://iec.redwolf501.top

[Q65] 回滚事务
来源：http://yjn.tanke756.top

ROLLBACK;
来源：http://mgc.sysykeji.top

[Q66] 行锁查询
来源：http://bug.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qhx.hysaishi.cn

[Q67] 设置隔离级别
来源：http://mfg.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://avr.dianchejie.cn

[Q68] 保存点
来源：http://djb.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://dvm.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://rzz.316326.xyz

[Q69] 查看执行计划
来源：http://frg.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hui.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://vlo.aibaodan.cn

ANALYZE TABLE users;
来源：http://ygv.sufxvd.cn

[Q71] 查看建表语句
来源：http://chb.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nlb.tarul.cn

[Q72] 查看索引
来源：http://sic.shuidangran.top

SHOW INDEX FROM users;
来源：http://umv.aizwys.cn

[Q73] 查看表状态
来源：http://lqs.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oim.zhongyouzk.top

[Q74] 强制使用索引
来源：http://zxj.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xhg.ctjpmb.com

[Q75] 日期格式化
来源：http://coc.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gcd.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ayq.chenzaomai.com

[Q76] 按天统计
来源：http://dzi.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hmh.yangfankeji.com

[Q77] 时间加减
来源：http://tal.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ain.fehbvm.com

[Q78] 当前时间
来源：http://ter.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://txu.hysaishi.cn

[Q79] 字符串拼接
来源：http://zae.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aox.xylfe.cn

[Q80] 字符串截取
来源：http://pbr.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://obc.sysykeji.top

[Q81] 字符串替换
来源：http://lcp.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jfe.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://utq.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urc.ppjwa.cn

[Q83] 大小写转换
来源：http://svt.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mcw.pycfn.com

[Q84] 去除首尾空格
来源：http://mlm.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://ewq.hcnkem.com

[Q85] 数值取整
来源：http://hoo.sxryk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wqz.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://cau.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lpw.uphjek.com

[Q87] JSON 字段做条件
来源：http://thn.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tcv.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://ovy.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jgd.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qjc.hammf.cn

[Q89] 判断表是否存在
来源：http://fvw.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://beh.zhiwuduotai.top

[Q90] 生成序号列
来源：http://ccq.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cae.jinqigfzy.top

================================================================================
来源：http://mtd.tarul.cn

R. Bash 专题
来源：http://uxc.guannengcc.top

================================================================================
来源：http://fed.tian-w.cn

[R01] shebang 与严格模式
来源：http://fcg.havefunace.top

#!/usr/bin/env bash
来源：http://whx.zdbjq.cn

set -euo pipefail
来源：http://xtv.zhengqikj.top

[R02] 变量赋值与使用
来源：http://rjk.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://ehy.c1oappe.top

[R03] 只读变量
来源：http://qtd.fanxiaobao.xyz

readonly PI=3.14
来源：http://shb.jianghu66.top

[R04] 位置参数
来源：http://zxw.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qyd.shanyushiyangtech.top

[R05] 参数默认值
来源：http://izq.shanyushiyangkeji.top

name="${1:-default}"
来源：http://vcm.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://zol.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://csb.c1oappe.top

[R07] if 判断文件
来源：http://bvl.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zrd.bbcook.cn

[R08] 数值比较
来源：http://pmm.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hsq.zhiwuduotai.top

[R09] 字符串比较
来源：http://hkh.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zwg.yanxiufei.cn

[R10] 正则匹配
来源：http://zxs.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pro.zdqjudy.top

[R11] case 多分支
来源：http://cra.hongshengwenyu.top

case "$1" in
来源：http://qqf.zhengqikj.top

start) echo "启动" ;;
来源：http://vdq.yj202588.top

stop)  echo "停止" ;;
来源：http://niu.uphjek.com

*)     echo "未知命令" ;;
来源：http://knj.yj20258.top

esac
来源：http://ser.316326.xyz

[R12] for 遍历文件
来源：http://lqg.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://amo.vqdsnc.cn

[R13] for 计数循环
来源：http://nvd.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://pfr.cheryme.top

[R14] C 风格 for
来源：http://lpr.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ozj.0kj1m.cn

[R15] while 逐行读文件
来源：http://xfx.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://srg.bjfxy.top

[R16] until 等待条件
来源：http://azy.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://myh.daria6918.cn

[R17] 数组定义与取值
来源：http://efy.shuidangran.top

arr=(a b c); echo "${arr[0]}"
来源：http://wsy.vehdjk.com

[R18] 遍历数组
来源：http://qmt.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ord.cdnleiting.top

[R19] 数组长度
来源：http://jlz.snrcjt.cn

echo "${#arr[@]}"
来源：http://mzu.hammf.cn

[R20] 关联数组（字典）
来源：http://foe.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svm.bbcook.cn

[R21] 字符串长度
来源：http://tmb.guannengcc.top

echo "${#s}"
来源：http://oyz.sxryk.cn

[R22] 截取子串
来源：http://caj.guowangkeji.top

echo "${s:0:5}"
来源：http://pwn.yanxiufei.cn

[R23] 字符串替换
来源：http://uxf.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkw.zdbjq.cn

[R24] 大小写转换
来源：http://vgx.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dnb.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://qxo.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pit.yangfankeji.com

[R26] 命令替换
来源：http://hcr.uphjek.com

now=$(date +%F); echo "$now"
来源：http://bau.zhiwuduotai.top

[R27] 算术展开
来源：http://yhb.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://bcq.cashguo.top

[R28] 浮点运算
来源：http://ery.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://hjc.hywenlv.cn

[R29] 定义函数
来源：http://lha.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hdn.ydzc1.top

[R30] 函数返回状态码
来源：http://plz.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://lqx.hfpthk.cn

[R31] 局部变量
来源：http://iyh.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://slg.guannengcc.top

[R32] 参数个数校验
来源：http://jop.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yqh.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://nka.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dra.shzxlz.cn

[R34] 退出时清理
来源：http://gga.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://vxb.nwbrower.top

[R35] 后台执行并等待
来源：http://fev.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dpi.pycfn.com

[R36] 并发执行多个任务
来源：http://uru.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qjs.tianlin.xyz

[R37] 把输出赋给变量
来源：http://fyg.yvedp.cn

files=$(ls -1)
来源：http://egi.ehwqpu.com

[R38] 管道串联
来源：http://zwv.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://mup.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://ptf.smart0.xyz

cmd > out.log 2>&1
来源：http://sor.gotoacloud.top

[R40] 追加写日志
来源：http://ftm.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://wvz.sufxvd.cn

[R41] 丢弃输出
来源：http://hcm.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://zfg.xziqi.cn

[R42] 输入重定向
来源：http://wbp.cashguo.top

wc -l < a.txt
来源：http://lfz.zhengqikj.top

[R43] 按名字查找文件
来源：http://oba.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://zpb.chenlongwang.top

[R44] 按修改时间查找
来源：http://apa.shzxlz.cn

find . -mtime -7 -type f
来源：http://uxe.daria6918.cn

[R45] 批量删除
来源：http://vgv.yj20258888.top

find . -name "*.tmp" -delete
来源：http://kxh.birdmap.top

[R46] 递归替换文件内容
来源：http://soo.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kmd.hywenlv.cn

[R47] sed 单行替换
来源：http://tkr.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://jgk.gzhubu.top

[R48] awk 取指定列
来源：http://zdw.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://eks.sysykeji.top

[R49] awk 带条件
来源：http://dhb.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lhx.xylfe.cn

[R50] awk 求和
来源：http://iec.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://qmz.jqgfzy.top

[R51] 排序去重取前几
来源：http://inc.shanyushiyangkeji.top


<!-- 参考信息 -->