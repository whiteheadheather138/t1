代发 wailian999

);
来源：http://agf.shzxlz.cn

[Q03] 增加列
来源：http://pqg.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hao.zhengqikj.top

[Q04] 修改列类型
来源：http://lfp.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dnt.hnqzz.top

[Q05] 重命名列
来源：http://vpx.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oun.yfazqb.com

[Q06] 删除列
来源：http://kyq.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://zxv.smart0.xyz

[Q07] 删除表
来源：http://etf.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://wrp.mhx1999.top

[Q08] 创建普通索引
来源：http://krs.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mdt.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ghz.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://maz.yueranfly.top

[Q10] 插入单行
来源：http://cfu.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gix.yueranfly.top

[Q11] 一次插入多行
来源：http://kna.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nmg.meibo888.top

[Q12] 插入后取自增 ID
来源：http://pfr.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://trf.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uik.cdnleiting.top

[Q13] 忽略重复插入
来源：http://ela.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nzs.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://ivy.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bib.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ixf.shuidangran.top

[Q15] 查询全部
来源：http://dvg.zhijiandao.cn

SELECT * FROM users;
来源：http://dpf.hammf.cn

[Q16] 查询指定列
来源：http://ecr.yuanzhike.top

SELECT id, name FROM users;
来源：http://bhz.ctjpmb.com

[Q17] 条件查询
来源：http://bpd.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://knx.yj202588.top

[Q18] 模糊匹配
来源：http://nla.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sli.sjlbkw.cn

[Q19] 范围查询
来源：http://cde.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qoe.svipenyu.cn

[Q20] IN 列表
来源：http://qcm.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kdh.ivvv.top

[Q21] 空值判断
来源：http://tns.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ocj.shanyushiyangkeji.top

[Q22] 排序
来源：http://nfq.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djy.kuanghao11.cn

[Q23] 分页
来源：http://cyl.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ygb.mhx1999.top

[Q24] 去重
来源：http://boc.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://xrz.hcnkem.com

[Q25] 只取前 N 条
来源：http://yzm.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cnf.vqdsnc.cn

[Q26] 计数
来源：http://moi.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://gph.redwolf501.top

[Q27] 条件计数
来源：http://rok.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yhl.andypj.xyz

[Q28] 求和与平均
来源：http://rsn.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://icw.pengpengdd.cyou

[Q29] 最大最小值
来源：http://bme.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ipb.hfpthk.cn

[Q30] 分组统计
来源：http://abc.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dwk.c1oappe.top

[Q31] 分组后过滤
来源：http://crv.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyd.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://ejn.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nrk.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pov.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://pfi.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mhu.tanke756.top

[Q34] 每组取第一条
来源：http://sib.cheryme.top

SELECT * FROM (
来源：http://edh.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://krb.zhoulong.xyz

) t WHERE rn = 1;
来源：http://faj.xziqi.cn

[Q35] 内连接
来源：http://ifz.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fsz.cqqwz.cn

[Q36] 左连接
来源：http://itd.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ska.andypj.xyz

[Q37] 右连接
来源：http://efh.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://adw.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cdn.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nlk.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://fkb.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gfo.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ila.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://exf.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cfx.shzxlz.cn

[Q41] 多表连接
来源：http://nvd.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lcg.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://xlw.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://zsh.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://cus.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://ouh.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aam.vqdsnc.cn

[Q43] 标量子查询
来源：http://yzx.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gps.zycfv.cn

[Q44] IN 子查询
来源：http://agi.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cbx.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://gnf.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rxp.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://nfr.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ico.316326.xyz

[Q47] 与平均值比较
来源：http://adr.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rni.meibo888.top

[Q48] CTE 公用表表达式
来源：http://upu.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vcs.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://kad.zycfv.cn

[Q49] 更新单行
来源：http://bqn.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ysn.c1oappe.top

[Q50] 批量更新
来源：http://xxl.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ogh.kuanghao11.cn

[Q51] 用子查询更新
来源：http://xrq.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oyu.sjlbkw.cn

[Q52] 删除指定行
来源：http://wdj.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://gfu.sjlbkw.cn

[Q53] 按条件删除
来源：http://kvi.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wni.zhongyouzk.top

[Q54] 清空表
来源：http://alc.cashguo.top

TRUNCATE TABLE logs;
来源：http://nam.xuanzx.com

[Q55] 排名（并列占位）
来源：http://ihh.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvy.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://tnd.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ped.havefunace.top

[Q57] 行号
来源：http://vcy.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tem.pengpengdd.cyou

[Q58] 累计求和
来源：http://zbe.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vuq.smart0.xyz

[Q59] 分组内累计
来源：http://jsx.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pvj.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://utu.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://udw.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kmj.fzhhl.top

[Q61] 移动平均
来源：http://fka.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xti.hcnkem.com

[Q62] 分组占比
来源：http://vqu.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gcb.zdqjudy.top

[Q63] 开启事务
来源：http://quh.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bxc.zhiwuduotai.top

[Q64] 提交事务
来源：http://ymn.vqdsnc.cn

COMMIT;
来源：http://ndr.ivvv.top

[Q65] 回滚事务
来源：http://lbl.cucudq.cn

ROLLBACK;
来源：http://yjb.redwolf501.top

[Q66] 行锁查询
来源：http://hdh.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bhx.nanxinkj.top

[Q67] 设置隔离级别
来源：http://mgn.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xca.yvedp.cn

[Q68] 保存点
来源：http://cwa.ppjwa.cn

SAVEPOINT sp1;
来源：http://ten.mhx1999.top

ROLLBACK TO sp1;
来源：http://rua.ybcxt.top

[Q69] 查看执行计划
来源：http://lbt.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uiy.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://lve.gogol.net.cn

ANALYZE TABLE users;
来源：http://avw.vehdjk.com

[Q71] 查看建表语句
来源：http://ubp.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ohy.yangfankeji.com

[Q72] 查看索引
来源：http://hmw.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://tyk.chenjidiqi.icu

[Q73] 查看表状态
来源：http://bhu.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yiu.hnqzz.top

[Q74] 强制使用索引
来源：http://pij.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zfe.aibaodan.cn

[Q75] 日期格式化
来源：http://tus.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xrx.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mbp.sweek.top

[Q76] 按天统计
来源：http://tdo.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vwn.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://rda.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vzk.c1oappe.top

[Q78] 当前时间
来源：http://uyx.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nso.kuanghao11.cn

[Q79] 字符串拼接
来源：http://yxe.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mek.zhengqikj.top

[Q80] 字符串截取
来源：http://aqd.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ldx.nwbrower.top

[Q81] 字符串替换
来源：http://dtw.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ggb.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://xou.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://acd.cucudq.cn

[Q83] 大小写转换
来源：http://vtb.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fjo.c1oappe.top

[Q84] 去除首尾空格
来源：http://xye.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://xvu.zhoulong.xyz

[Q85] 数值取整
来源：http://poq.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jdd.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://hoj.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ctn.sweek.top

[Q87] JSON 字段做条件
来源：http://isf.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://puc.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://lph.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bzb.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tck.andypj.xyz

[Q89] 判断表是否存在
来源：http://toj.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bud.nanxinkj.top

[Q90] 生成序号列
来源：http://ntt.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rtu.jiagoushi.top

================================================================================
来源：http://clx.xuanzx.com

R. Bash 专题
来源：http://vjg.zhijiandao.cn

================================================================================
来源：http://rhp.dashuyun.cn

[R01] shebang 与严格模式
来源：http://bxi.316326.xyz

#!/usr/bin/env bash
来源：http://xra.hysaishi.cn

set -euo pipefail
来源：http://vou.cashguo.top

[R02] 变量赋值与使用
来源：http://lpr.ehwqpu.com

name="Tom"; echo "$name"
来源：http://cbg.yj20258888.top

[R03] 只读变量
来源：http://cxk.yongpay.top

readonly PI=3.14
来源：http://hqi.fanxiaobao.xyz

[R04] 位置参数
来源：http://rbk.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vag.gzhubu.top

[R05] 参数默认值
来源：http://kvv.ctjpmb.com

name="${1:-default}"
来源：http://mjf.hesvh.cn

[R06] 判断命令是否存在
来源：http://hnq.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fck.gzhubu.top

[R07] if 判断文件
来源：http://xeg.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jtc.chenzaomai.com

[R08] 数值比较
来源：http://chn.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ycd.cashguo.top

[R09] 字符串比较
来源：http://plr.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://llh.tanke756.top

[R10] 正则匹配
来源：http://dff.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sdy.ywan-chungtsiang.top

[R11] case 多分支
来源：http://gty.jqgufenzy.top

case "$1" in
来源：http://ila.zhiwuduotai.top

start) echo "启动" ;;
来源：http://mcv.yj202588.top

stop)  echo "停止" ;;
来源：http://emh.guannengcc.top

*)     echo "未知命令" ;;
来源：http://etz.cheryme.top

esac
来源：http://qth.xuetiantiany.cn

[R12] for 遍历文件
来源：http://vjj.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://jfg.tian-w.cn

[R13] for 计数循环
来源：http://ago.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://ism.gotoacloud.top

[R14] C 风格 for
来源：http://ddf.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://djn.52xcode.cn

[R15] while 逐行读文件
来源：http://yjr.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://llh.sweek.top

[R16] until 等待条件
来源：http://eye.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kwz.bbcook.cn

[R17] 数组定义与取值
来源：http://rcs.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://blk.fehbvm.com

[R18] 遍历数组
来源：http://nqo.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yum.meibo888.top

[R19] 数组长度
来源：http://svw.jinqigfzy.top

echo "${#arr[@]}"
来源：http://wdw.jiagoushi.top

[R20] 关联数组（字典）
来源：http://cta.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://acs.hnqzz.top

[R21] 字符串长度
来源：http://spk.mhx1999.top

echo "${#s}"
来源：http://nmo.ctjpmb.com

[R22] 截取子串
来源：http://gqs.ctjpmb.com

echo "${s:0:5}"
来源：http://ovb.wangdashe.top

[R23] 字符串替换
来源：http://ypo.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kfn.feifeiyinyue.top

[R24] 大小写转换
来源：http://nzo.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://xcn.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://cgv.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://alh.hysaishi.cn

[R26] 命令替换
来源：http://yju.yj202588.top

now=$(date +%F); echo "$now"
来源：http://ivu.zhixingplan.top

[R27] 算术展开
来源：http://gyd.fktsv.cn

echo $((1 + 2 * 3))
来源：http://wsr.iojbl.cn

[R28] 浮点运算
来源：http://suo.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://lif.tian-w.cn

[R29] 定义函数
来源：http://qnt.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://isn.hysaishi.cn

[R30] 函数返回状态码
来源：http://yje.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://tmd.hywenlv.cn

[R31] 局部变量
来源：http://frp.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://let.uphjek.com

[R32] 参数个数校验
来源：http://ubz.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lgf.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://vub.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ktv.birdmap.top

[R34] 退出时清理
来源：http://tcv.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pso.yanxiufei.cn

[R35] 后台执行并等待
来源：http://dqu.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fsr.hysaishi.cn

[R36] 并发执行多个任务
来源：http://vkj.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kzv.daxiang520.top

[R37] 把输出赋给变量
来源：http://xhp.shzxlz.cn

files=$(ls -1)
来源：http://rga.yj202588.top

[R38] 管道串联
来源：http://hhb.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://wux.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://tug.gogol.net.cn

cmd > out.log 2>&1
来源：http://akl.ctjpmb.com

[R40] 追加写日志
来源：http://nmx.shuidangran.top

echo "log" >> out.log
来源：http://odn.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://bja.cashguo.top

cmd >/dev/null 2>&1
来源：http://fvv.xuetiantiany.cn

[R42] 输入重定向
来源：http://ckc.yj202588.top

wc -l < a.txt
来源：http://cks.tanke756.top

[R43] 按名字查找文件
来源：http://zfj.cucudq.cn

find . -name "*.log" -type f
来源：http://dqa.fzhhl.top

[R44] 按修改时间查找
来源：http://qxb.tarul.cn

find . -mtime -7 -type f
来源：http://war.316326.xyz

[R45] 批量删除
来源：http://bav.xziqi.cn

find . -name "*.tmp" -delete
来源：http://kby.yvedp.cn

[R46] 递归替换文件内容
来源：http://ehy.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbt.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://ace.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://lya.zhongyouzk.top

[R48] awk 取指定列
来源：http://ytf.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://svb.redwolf501.top

[R49] awk 带条件
来源：http://mey.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kel.bbcook.cn

[R50] awk 求和
来源：http://ftb.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fxp.316326.xyz

[R51] 排序去重取前几
来源：http://mpr.316326.xyz


<!-- 参考信息 -->