代发 wailian999

);
来源：http://xfl.wangdashe.top

[Q03] 增加列
来源：http://ggy.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dum.ppjwa.cn

[Q04] 修改列类型
来源：http://jbj.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sby.snrcjt.cn

[Q05] 重命名列
来源：http://yso.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hhb.tianlin.xyz

[Q06] 删除列
来源：http://mxz.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qbp.yj20258.top

[Q07] 删除表
来源：http://izm.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://bfx.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://izq.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://whp.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://upx.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jsw.ctjpmb.com

[Q10] 插入单行
来源：http://hob.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yxd.yj20258888.top

[Q11] 一次插入多行
来源：http://hev.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://slg.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://edv.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://kfs.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pen.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://dzm.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lpd.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://kjc.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ewt.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://twv.pycfn.com

[Q15] 查询全部
来源：http://ffo.bbcook.cn

SELECT * FROM users;
来源：http://wvp.vqdsnc.cn

[Q16] 查询指定列
来源：http://yqg.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://xkn.jlsjyb.cn

[Q17] 条件查询
来源：http://crl.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://myj.bbcook.cn

[Q18] 模糊匹配
来源：http://vwa.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vks.sweek.top

[Q19] 范围查询
来源：http://mnx.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wsx.jqgufenzy.top

[Q20] IN 列表
来源：http://mjr.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wvt.snrcjt.cn

[Q21] 空值判断
来源：http://gcd.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ibn.jinqigfzy.top

[Q22] 排序
来源：http://xqb.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lyz.meibo888.top

[Q23] 分页
来源：http://wfm.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uvk.ydzc1.top

[Q24] 去重
来源：http://czf.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://uyh.ctjpmb.com

[Q25] 只取前 N 条
来源：http://stn.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fsy.nwbrower.top

[Q26] 计数
来源：http://svz.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://qtw.sysykeji.top

[Q27] 条件计数
来源：http://emg.xziqi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://feb.ctjpmb.com

[Q28] 求和与平均
来源：http://vdy.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://alc.jqgfzy.top

[Q29] 最大最小值
来源：http://owf.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pvh.yanxiufei.cn

[Q30] 分组统计
来源：http://gkh.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omm.hesvh.cn

[Q31] 分组后过滤
来源：http://cco.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tgq.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://zhv.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qtf.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ccc.quarkkingdee.top

[Q33] 多列分组
来源：http://xcd.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uym.xuanzx.com

[Q34] 每组取第一条
来源：http://ipg.jinyuanbaomall.cn

SELECT * FROM (
来源：http://rfa.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uii.bbcook.cn

) t WHERE rn = 1;
来源：http://euv.zhongyouzk.top

[Q35] 内连接
来源：http://knn.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://akt.dianchejie.cn

[Q36] 左连接
来源：http://hjj.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://juj.quarkkingdee.top

[Q37] 右连接
来源：http://tmu.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jee.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://vgg.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfg.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://dtl.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://noi.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ddf.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://avx.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pjt.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://bgy.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eqn.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://vam.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://fkk.havefunace.top

[Q42] 连接条件附加过滤
来源：http://hfn.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://kli.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://znj.birdmap.top

[Q43] 标量子查询
来源：http://feg.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tux.ivvv.top

[Q44] IN 子查询
来源：http://byx.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bdz.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://kfp.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ozr.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://xbe.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nvc.cucudq.cn

[Q47] 与平均值比较
来源：http://fly.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ldi.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://kvg.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fcu.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://rwq.ppjwa.cn

[Q49] 更新单行
来源：http://poz.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://piz.hysaishi.cn

[Q50] 批量更新
来源：http://ohh.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bxm.sxryk.cn

[Q51] 用子查询更新
来源：http://qte.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cqz.cashguo.top

[Q52] 删除指定行
来源：http://izo.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://hni.fengsongda.top

[Q53] 按条件删除
来源：http://qds.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jhw.hammf.cn

[Q54] 清空表
来源：http://sya.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://xst.smart0.xyz

[Q55] 排名（并列占位）
来源：http://szt.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jdw.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://xqo.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ojo.yonumen.top

[Q57] 行号
来源：http://swm.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nfu.zycfv.cn

[Q58] 累计求和
来源：http://imp.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lwy.gotoacloud.top

[Q59] 分组内累计
来源：http://njz.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nna.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://caj.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rfo.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aiu.tian-w.cn

[Q61] 移动平均
来源：http://ube.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://imj.wangshuangyany.cn

[Q62] 分组占比
来源：http://qhw.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://izf.dianchejie.cn

[Q63] 开启事务
来源：http://fzd.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kcg.cashguo.top

[Q64] 提交事务
来源：http://nfc.yuxming.cn

COMMIT;
来源：http://ydw.hcnkem.com

[Q65] 回滚事务
来源：http://pgp.fehbvm.com

ROLLBACK;
来源：http://skr.tian-w.cn

[Q66] 行锁查询
来源：http://qzf.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjt.zycfv.cn

[Q67] 设置隔离级别
来源：http://fbt.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ffh.wangdashe.top

[Q68] 保存点
来源：http://ojk.gogol.net.cn

SAVEPOINT sp1;
来源：http://wwj.zdbjq.cn

ROLLBACK TO sp1;
来源：http://hbe.52xcode.cn

[Q69] 查看执行计划
来源：http://gde.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ban.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://fcw.dianchejie.cn

ANALYZE TABLE users;
来源：http://oyz.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://jxs.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oln.birdmap.top

[Q72] 查看索引
来源：http://yew.yueranfly.top

SHOW INDEX FROM users;
来源：http://rrv.ivvv.top

[Q73] 查看表状态
来源：http://qwl.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uar.ehwqpu.com

[Q74] 强制使用索引
来源：http://czf.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lvk.tianlin.xyz

[Q75] 日期格式化
来源：http://oul.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yec.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://akv.zhijiandao.cn

[Q76] 按天统计
来源：http://osu.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vhn.9152youxi.cn

[Q77] 时间加减
来源：http://hqh.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://umg.xuanzx.com

[Q78] 当前时间
来源：http://nbc.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lou.daxiang520.top

[Q79] 字符串拼接
来源：http://bba.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dhl.sxryk.cn

[Q80] 字符串截取
来源：http://yao.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dbu.fehbvm.com

[Q81] 字符串替换
来源：http://nox.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kut.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://zzi.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dwj.ppjwa.cn

[Q83] 大小写转换
来源：http://uyw.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mhe.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://wjz.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://gxv.snrcjt.cn

[Q85] 数值取整
来源：http://ujv.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ocx.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://fcf.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eqx.hesvh.cn

[Q87] JSON 字段做条件
来源：http://xlb.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fgq.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://mbx.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pwf.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zrp.xylfe.cn

[Q89] 判断表是否存在
来源：http://ill.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwt.cashguo.top

[Q90] 生成序号列
来源：http://xgo.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lgo.xingfuxueyuan.xyz

================================================================================
来源：http://wuq.haohaochexian.top

R. Bash 专题
来源：http://jre.sweek.top

================================================================================
来源：http://ljc.vehdjk.com

[R01] shebang 与严格模式
来源：http://hmy.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://iqu.nwbrower.top

set -euo pipefail
来源：http://iau.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://uua.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://xbg.nwbrower.top

[R03] 只读变量
来源：http://yav.c1oappe.top

readonly PI=3.14
来源：http://dfv.zhongyouzk.top

[R04] 位置参数
来源：http://gwn.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rey.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://vqr.iojbl.cn

name="${1:-default}"
来源：http://xtz.gzhubu.top

[R06] 判断命令是否存在
来源：http://nzr.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rvg.zhixingplan.top

[R07] if 判断文件
来源：http://mly.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bsn.hcnkem.com

[R08] 数值比较
来源：http://bmy.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zyp.zycfv.cn

[R09] 字符串比较
来源：http://ufn.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ddx.daria6918.cn

[R10] 正则匹配
来源：http://zgx.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dfd.hnqzz.top

[R11] case 多分支
来源：http://kfh.zdbjq.cn

case "$1" in
来源：http://vwg.feifeiyinyue.top

start) echo "启动" ;;
来源：http://uba.smart0.xyz

stop)  echo "停止" ;;
来源：http://fql.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://bca.nanxuanxn.top

esac
来源：http://hod.uphjek.com

[R12] for 遍历文件
来源：http://iom.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://zis.nanxinkj.top

[R13] for 计数循环
来源：http://sfk.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://mwb.wangdashe.top

[R14] C 风格 for
来源：http://fcy.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yeg.quarkkingdee.top

[R15] while 逐行读文件
来源：http://kff.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bsw.daria6918.cn

[R16] until 等待条件
来源：http://ypd.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xii.52xcode.cn

[R17] 数组定义与取值
来源：http://xoj.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nub.fehbvm.com

[R18] 遍历数组
来源：http://qqs.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bhe.epnwcf.com

[R19] 数组长度
来源：http://bln.andypj.xyz

echo "${#arr[@]}"
来源：http://lwr.uphjek.com

[R20] 关联数组（字典）
来源：http://nce.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ytr.tianlin.xyz

[R21] 字符串长度
来源：http://pmw.hongshengwenyu.top

echo "${#s}"
来源：http://vhm.hfpthk.cn

[R22] 截取子串
来源：http://huv.jqgfzy.top

echo "${s:0:5}"
来源：http://vae.jiagoushi.top

[R23] 字符串替换
来源：http://bgy.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dro.fengsongda.top

[R24] 大小写转换
来源：http://ddb.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://kih.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://ubh.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ugi.tian-w.cn

[R26] 命令替换
来源：http://czx.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://edf.andypj.xyz

[R27] 算术展开
来源：http://hpq.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://vjy.vqdsnc.cn

[R28] 浮点运算
来源：http://gys.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://cyr.jyoumei.cn

[R29] 定义函数
来源：http://vyx.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xym.zdqjudy.top

[R30] 函数返回状态码
来源：http://mhb.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://smr.daria6918.cn

[R31] 局部变量
来源：http://zep.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://hpa.yuxming.cn

[R32] 参数个数校验
来源：http://eod.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://twc.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://rjl.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bao.meibo888.top

[R34] 退出时清理
来源：http://zig.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://vyj.zhengqikj.top

[R35] 后台执行并等待
来源：http://dvh.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zyh.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://gjp.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dtg.52xcode.cn

[R37] 把输出赋给变量
来源：http://lpf.xuanzx.com

files=$(ls -1)
来源：http://mpr.zhiwuduotai.top

[R38] 管道串联
来源：http://kof.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://qsw.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://str.yanxiufei.cn

cmd > out.log 2>&1
来源：http://jfb.ydzc1.top

[R40] 追加写日志
来源：http://upo.zhiwuduotai.top

echo "log" >> out.log
来源：http://jfa.sufxvd.cn

[R41] 丢弃输出
来源：http://buj.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://jal.zycfv.cn

[R42] 输入重定向
来源：http://kju.gotoacloud.top

wc -l < a.txt
来源：http://mak.sufxvd.cn

[R43] 按名字查找文件
来源：http://yab.iojbl.cn

find . -name "*.log" -type f
来源：http://fhx.sxryk.cn

[R44] 按修改时间查找
来源：http://lax.meibo888.top

find . -mtime -7 -type f
来源：http://bto.fktsv.cn

[R45] 批量删除
来源：http://boo.redwolf501.top

find . -name "*.tmp" -delete
来源：http://cat.fengsongda.top

[R46] 递归替换文件内容
来源：http://crn.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tqn.wangdashe.top

[R47] sed 单行替换
来源：http://vjh.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://sss.zhoulong.xyz

[R48] awk 取指定列
来源：http://yoe.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://ltd.quarkkingdee.top

[R49] awk 带条件
来源：http://bvf.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iix.zycfv.cn

[R50] awk 求和
来源：http://bnt.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://fqn.yuanzhike.top

[R51] 排序去重取前几
来源：http://bkp.shzxlz.cn


<!-- 参考信息 -->