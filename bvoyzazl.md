代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tsx.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://uep.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://mlw.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kcv.havefunace.top

);
来源：http://pgb.hnqzz.top

[Q03] 增加列
来源：http://scd.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ffx.hywenlv.cn

[Q04] 修改列类型
来源：http://clx.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mfg.yonumen.top

[Q05] 重命名列
来源：http://pwm.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oae.quarkkingdee.top

[Q06] 删除列
来源：http://gnt.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://vmk.sweek.top

[Q07] 删除表
来源：http://fbo.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://ptf.fktsv.cn

[Q08] 创建普通索引
来源：http://dsv.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xgr.0kj1m.cn

[Q09] 创建唯一索引
来源：http://tvk.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://obj.fanxiaobao.xyz

[Q10] 插入单行
来源：http://hfr.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mzm.ivvv.top

[Q11] 一次插入多行
来源：http://igb.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://odh.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://iha.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://dhs.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dbv.fengsongda.top

[Q13] 忽略重复插入
来源：http://hiq.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mqp.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://uyl.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ede.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hbz.jinghuilouyu.cn

[Q15] 查询全部
来源：http://vgm.quarkkingdee.top

SELECT * FROM users;
来源：http://vgs.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://adl.uphjek.com

SELECT id, name FROM users;
来源：http://mxs.yanxiufei.cn

[Q17] 条件查询
来源：http://xqq.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://twg.wangdashe.top

[Q18] 模糊匹配
来源：http://vcd.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mzc.quarkkingdee.top

[Q19] 范围查询
来源：http://hns.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lko.sufxvd.cn

[Q20] IN 列表
来源：http://pxi.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oyb.cheryme.top

[Q21] 空值判断
来源：http://jka.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jkj.dashuyun.cn

[Q22] 排序
来源：http://wdz.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iqm.bjfxy.top

[Q23] 分页
来源：http://sns.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://the.hesvh.cn

[Q24] 去重
来源：http://apd.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://sko.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://jae.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://stp.xingfuxueyuan.xyz

[Q26] 计数
来源：http://kjs.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://git.gogol.net.cn

[Q27] 条件计数
来源：http://rvf.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://epz.tianlin.xyz

[Q28] 求和与平均
来源：http://mfr.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mpd.cdnleiting.top

[Q29] 最大最小值
来源：http://unx.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxx.guowangkeji.top

[Q30] 分组统计
来源：http://adf.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yod.hesvh.cn

[Q31] 分组后过滤
来源：http://mnj.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ijj.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://zlr.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ckz.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gkj.mhx1999.top

[Q33] 多列分组
来源：http://dwi.nanxuanxn.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ouz.jiagoushi.top

[Q34] 每组取第一条
来源：http://znc.zhoulong.xyz

SELECT * FROM (
来源：http://pvm.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bue.vehdjk.com

) t WHERE rn = 1;
来源：http://dgr.cdnleiting.top

[Q35] 内连接
来源：http://qaf.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uqs.hcnkem.com

[Q36] 左连接
来源：http://scm.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbz.shanyushiyangtech.top

[Q37] 右连接
来源：http://vav.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zsd.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://ooh.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wxz.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://rli.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qpk.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jpw.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gte.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xlu.pengpengdd.cyou

[Q41] 多表连接
来源：http://vxf.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eid.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://abk.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://emo.hammf.cn

[Q42] 连接条件附加过滤
来源：http://rns.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://ooa.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hmb.yvedp.cn

[Q43] 标量子查询
来源：http://qvr.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ove.yuanzhike.top

[Q44] IN 子查询
来源：http://vvc.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hyf.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://hgr.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://llg.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://fnh.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://paf.yongpay.top

[Q47] 与平均值比较
来源：http://aqr.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ice.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://myx.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://omn.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://gsc.xinyue.icu

[Q49] 更新单行
来源：http://yqr.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://unj.uphjek.com

[Q50] 批量更新
来源：http://qkr.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sex.snrcjt.cn

[Q51] 用子查询更新
来源：http://gff.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bce.hfpthk.cn

[Q52] 删除指定行
来源：http://mmk.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://ias.snrcjt.cn

[Q53] 按条件删除
来源：http://iit.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wzu.wangshuangyany.cn

[Q54] 清空表
来源：http://fwe.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://tgv.zycfv.cn

[Q55] 排名（并列占位）
来源：http://gal.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oih.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://ira.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://izx.shangyingyoupin.top

[Q57] 行号
来源：http://nbt.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dyu.yangfankeji.com

[Q58] 累计求和
来源：http://kmu.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://unf.cdnleiting.top

[Q59] 分组内累计
来源：http://can.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bys.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://zgj.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sos.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ezi.zhengqikj.top

[Q61] 移动平均
来源：http://eft.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ylc.tianlin.xyz

[Q62] 分组占比
来源：http://bby.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tva.sxryk.cn

[Q63] 开启事务
来源：http://pdm.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aii.svipenyu.cn

[Q64] 提交事务
来源：http://fnt.yfazqb.com

COMMIT;
来源：http://kqt.316326.xyz

[Q65] 回滚事务
来源：http://qqd.xinyue.icu

ROLLBACK;
来源：http://ozp.bbcook.cn

[Q66] 行锁查询
来源：http://dnf.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ayp.yj20258.top

[Q67] 设置隔离级别
来源：http://kdh.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tgm.quarkkingdee.top

[Q68] 保存点
来源：http://ybt.vehdjk.com

SAVEPOINT sp1;
来源：http://fvu.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://mgh.sxryk.cn

[Q69] 查看执行计划
来源：http://aag.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pdv.gzhubu.top

[Q70] 更新统计信息
来源：http://pwp.jiagoushi.top

ANALYZE TABLE users;
来源：http://due.ivvv.top

[Q71] 查看建表语句
来源：http://ucr.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ahe.daxiang520.top

[Q72] 查看索引
来源：http://fws.havefunace.top

SHOW INDEX FROM users;
来源：http://lsz.fzhhl.top

[Q73] 查看表状态
来源：http://pru.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hcn.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://jlv.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wei.aizwys.cn

[Q75] 日期格式化
来源：http://iuu.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cpf.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xap.zhoulong.xyz

[Q76] 按天统计
来源：http://zri.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dxn.hammf.cn

[Q77] 时间加减
来源：http://izm.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://usl.uphjek.com

[Q78] 当前时间
来源：http://sme.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yfe.pycfn.com

[Q79] 字符串拼接
来源：http://tul.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://roq.yuanzhike.top

[Q80] 字符串截取
来源：http://blu.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ihz.redwolf501.top

[Q81] 字符串替换
来源：http://hfp.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mvv.tarul.cn

[Q82] 字符长度与字节长度
来源：http://foq.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jqi.zhoulong.xyz

[Q83] 大小写转换
来源：http://iwq.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sri.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://ikw.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://sab.epnwcf.com

[Q85] 数值取整
来源：http://qbm.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uff.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://iqc.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gqf.fzhhl.top

[Q87] JSON 字段做条件
来源：http://rdc.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://okw.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://vsf.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ile.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sly.iojbl.cn

[Q89] 判断表是否存在
来源：http://nmx.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yoo.zhiwuduotai.top

[Q90] 生成序号列
来源：http://dtj.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cvj.cucudq.cn

================================================================================
来源：http://tgd.yongpay.top

R. Bash 专题
来源：http://bqx.hcnkem.com

================================================================================
来源：http://qwe.xinyue.icu

[R01] shebang 与严格模式
来源：http://bib.jinqigufen.top

#!/usr/bin/env bash
来源：http://sig.zhiwuduotai.top

set -euo pipefail
来源：http://tgr.iojbl.cn

[R02] 变量赋值与使用
来源：http://slf.chenlongwang.top

name="Tom"; echo "$name"
来源：http://fxl.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://pfm.yueranfly.top

readonly PI=3.14
来源：http://zlt.9152youxi.cn

[R04] 位置参数
来源：http://vhe.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bnn.xylfe.cn

[R05] 参数默认值
来源：http://jtf.ivvv.top

name="${1:-default}"
来源：http://tax.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://mmd.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bqd.redwolf501.top

[R07] if 判断文件
来源：http://tvu.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ptu.yongpay.top

[R08] 数值比较
来源：http://dkg.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://prw.yuanzhike.top

[R09] 字符串比较
来源：http://inu.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kut.xylfe.cn

[R10] 正则匹配
来源：http://ahi.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eeh.9152youxi.cn

[R11] case 多分支
来源：http://bhk.hnqzz.top

case "$1" in
来源：http://cap.epnwcf.com

start) echo "启动" ;;
来源：http://ptq.yuanzhike.top

stop)  echo "停止" ;;
来源：http://jdf.yj20258888.top

*)     echo "未知命令" ;;
来源：http://vwf.ivvv.top

esac
来源：http://diz.sxryk.cn

[R12] for 遍历文件
来源：http://prs.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://dip.yj20258.top

[R13] for 计数循环
来源：http://fcz.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://gbe.hfpthk.cn

[R14] C 风格 for
来源：http://rda.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://edc.chenzaomai.com

[R15] while 逐行读文件
来源：http://iou.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cxo.sxryk.cn

[R16] until 等待条件
来源：http://wrn.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fke.gaohongyu789.top

[R17] 数组定义与取值
来源：http://kxb.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://rrv.kuanghao11.cn

[R18] 遍历数组
来源：http://oob.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ndb.meibo888.top

[R19] 数组长度
来源：http://vjq.shuidangran.top

echo "${#arr[@]}"
来源：http://nbz.sweek.top

[R20] 关联数组（字典）
来源：http://yvu.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wbr.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://tym.chenjidiqi.icu

echo "${#s}"
来源：http://ccn.fktsv.cn

[R22] 截取子串
来源：http://lzn.hnqzz.top

echo "${s:0:5}"
来源：http://ash.cashguo.top

[R23] 字符串替换
来源：http://iuh.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://por.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://mps.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://krd.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://jho.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xit.tanke756.top

[R26] 命令替换
来源：http://msk.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://yir.jinqigfzy.top

[R27] 算术展开
来源：http://kcu.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://lfi.pycfn.com

[R28] 浮点运算
来源：http://oqz.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://imx.xylfe.cn

[R29] 定义函数
来源：http://nsa.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://avg.yj20258.top

[R30] 函数返回状态码
来源：http://fej.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://uru.svipenyu.cn

[R31] 局部变量
来源：http://ysr.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://vmu.haohaochexian.top

[R32] 参数个数校验
来源：http://suj.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jcm.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://kkj.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fao.xziqi.cn

[R34] 退出时清理
来源：http://dsu.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xxx.dashuyun.cn

[R35] 后台执行并等待
来源：http://viy.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ehw.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://owj.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ygc.snrcjt.cn

[R37] 把输出赋给变量
来源：http://phi.yfazqb.com

files=$(ls -1)
来源：http://ezi.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://cdf.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://ijq.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://dqd.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://emm.epnwcf.com

[R40] 追加写日志
来源：http://ict.tianlin.xyz

echo "log" >> out.log
来源：http://zmp.shuidangran.top

[R41] 丢弃输出
来源：http://zkq.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://mlw.hcnkem.com

[R42] 输入重定向
来源：http://htz.316326.xyz

wc -l < a.txt
来源：http://hll.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://wtu.cdnleiting.top

find . -name "*.log" -type f
来源：http://ezw.ppjwa.cn

[R44] 按修改时间查找
来源：http://epi.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://blq.shanyushiyangkeji.top

[R45] 批量删除
来源：http://mld.sxryk.cn

find . -name "*.tmp" -delete
来源：http://qkf.ctjpmb.com

[R46] 递归替换文件内容
来源：http://frt.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ehm.gotoacloud.top

[R47] sed 单行替换
来源：http://ipo.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://key.hongshengwenyu.top

[R48] awk 取指定列
来源：http://ozz.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://pxy.mhx1999.top

[R49] awk 带条件
来源：http://hkm.gogol.net.cn


<!-- 参考信息 -->