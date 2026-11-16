代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://zyb.xylfe.cn

[Q07] 删除表
来源：http://uks.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://rbu.tarul.cn

[Q08] 创建普通索引
来源：http://tpi.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ihf.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://lkr.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xvr.jiagoushi.top

[Q10] 插入单行
来源：http://yhp.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xxl.zhoulong.xyz

[Q11] 一次插入多行
来源：http://xee.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hml.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://wxd.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jck.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ova.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://lze.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sph.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://vzu.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ntb.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dzr.zhixingplan.top

[Q15] 查询全部
来源：http://cqs.haohaochexian.top

SELECT * FROM users;
来源：http://cbn.chenlongwang.top

[Q16] 查询指定列
来源：http://ald.smart0.xyz

SELECT id, name FROM users;
来源：http://dij.xuetiantiany.cn

[Q17] 条件查询
来源：http://jzj.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ddv.52xcode.cn

[Q18] 模糊匹配
来源：http://wcu.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yuw.xinyue.icu

[Q19] 范围查询
来源：http://dwb.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://coy.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://lvu.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qry.fengsongda.top

[Q21] 空值判断
来源：http://hbu.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ocv.yfazqb.com

[Q22] 排序
来源：http://itb.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://slz.zhiwuduotai.top

[Q23] 分页
来源：http://erh.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qfw.yangfankeji.com

[Q24] 去重
来源：http://dlb.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://vvr.yj20258.top

[Q25] 只取前 N 条
来源：http://vvn.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bdf.gzhubu.top

[Q26] 计数
来源：http://bfk.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://hwh.shuidangran.top

[Q27] 条件计数
来源：http://edm.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://trw.andypj.xyz

[Q28] 求和与平均
来源：http://qjn.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tpi.yvedp.cn

[Q29] 最大最小值
来源：http://auv.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://acb.jyoumei.cn

[Q30] 分组统计
来源：http://lvw.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bgh.hysaishi.cn

[Q31] 分组后过滤
来源：http://jee.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tny.hammf.cn

[Q32] 分组拼接字符串
来源：http://uaw.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cca.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zar.dianchejie.cn

[Q33] 多列分组
来源：http://spi.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gtm.bbcook.cn

[Q34] 每组取第一条
来源：http://ndr.shanyushiyangtech.top

SELECT * FROM (
来源：http://jny.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cmn.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://otn.bbcook.cn

[Q35] 内连接
来源：http://bsf.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://awr.zhongyouzk.top

[Q36] 左连接
来源：http://jeu.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjh.wangshuangyany.cn

[Q37] 右连接
来源：http://lry.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iqm.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ksx.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nbj.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://gzl.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rdi.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://otw.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ogp.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jhi.birdmap.top

[Q41] 多表连接
来源：http://pvi.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oay.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://uik.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://muu.316326.xyz

[Q42] 连接条件附加过滤
来源：http://nzr.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://rwp.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rzw.nanxinkj.top

[Q43] 标量子查询
来源：http://qpd.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cyp.yangfankeji.com

[Q44] IN 子查询
来源：http://rri.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mph.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://lem.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxz.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://bww.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvh.gotoacloud.top

[Q47] 与平均值比较
来源：http://ldw.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pdn.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://nnr.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bat.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://asm.yuanzhike.top

[Q49] 更新单行
来源：http://mjz.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rmv.sxryk.cn

[Q50] 批量更新
来源：http://owh.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fwk.xuanzx.com

[Q51] 用子查询更新
来源：http://icb.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mqc.hnqzz.top

[Q52] 删除指定行
来源：http://viu.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://bhw.yonumen.top

[Q53] 按条件删除
来源：http://rqe.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://arl.hesvh.cn

[Q54] 清空表
来源：http://pdl.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://snm.redwolf501.top

[Q55] 排名（并列占位）
来源：http://vhx.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yaf.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://qbr.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ney.hcnkem.com

[Q57] 行号
来源：http://dxm.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpt.wangdashe.top

[Q58] 累计求和
来源：http://veq.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://obb.bjfxy.top

[Q59] 分组内累计
来源：http://ijp.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zsm.sweek.top

[Q60] 取上一行 / 下一行
来源：http://aob.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tli.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lji.zhiwuduotai.top

[Q61] 移动平均
来源：http://nte.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rgb.9152youxi.cn

[Q62] 分组占比
来源：http://etm.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gbm.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://bzh.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vry.fktsv.cn

[Q64] 提交事务
来源：http://bot.fehbvm.com

COMMIT;
来源：http://fet.hnxiangtu.top

[Q65] 回滚事务
来源：http://biq.yongpay.top

ROLLBACK;
来源：http://dgk.chenjidiqi.icu

[Q66] 行锁查询
来源：http://iqd.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lgm.jianghu66.top

[Q67] 设置隔离级别
来源：http://jta.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpa.ctjpmb.com

[Q68] 保存点
来源：http://drf.zhijiandao.cn

SAVEPOINT sp1;
来源：http://jsb.ybcxt.top

ROLLBACK TO sp1;
来源：http://uet.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://jqw.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lyh.shangyingyoupin.top

[Q70] 更新统计信息
来源：http://cfd.vqdsnc.cn

ANALYZE TABLE users;
来源：http://qsi.guowangkeji.top

[Q71] 查看建表语句
来源：http://fvh.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nfq.aizwys.cn

[Q72] 查看索引
来源：http://rdl.sufxvd.cn

SHOW INDEX FROM users;
来源：http://fak.zhijiandao.cn

[Q73] 查看表状态
来源：http://rqu.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cjg.hfpthk.cn

[Q74] 强制使用索引
来源：http://fmw.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bnt.cdnleiting.top

[Q75] 日期格式化
来源：http://wei.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mtb.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kec.vehdjk.com

[Q76] 按天统计
来源：http://smm.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xus.pycfn.com

[Q77] 时间加减
来源：http://rrw.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ucz.0kj1m.cn

[Q78] 当前时间
来源：http://soh.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lcq.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://gtb.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rpf.vqdsnc.cn

[Q80] 字符串截取
来源：http://hqm.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zkp.zycfv.cn

[Q81] 字符串替换
来源：http://nem.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sjm.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://iiv.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rhn.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://pjh.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tuh.ivvv.top

[Q84] 去除首尾空格
来源：http://orx.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://isj.zdbjq.cn

[Q85] 数值取整
来源：http://itm.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bby.cheryme.top

[Q86] 读取 JSON 字段
来源：http://kva.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wut.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://ymu.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rlh.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://msc.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://glq.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wbw.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://gjk.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zqk.birdmap.top

[Q90] 生成序号列
来源：http://iyf.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rjb.redwolf501.top

================================================================================
来源：http://ryn.yuxming.cn

R. Bash 专题
来源：http://jhv.ivvv.top

================================================================================
来源：http://uyz.fehbvm.com

[R01] shebang 与严格模式
来源：http://pzw.gotoacloud.top

#!/usr/bin/env bash
来源：http://gte.zycfv.cn

set -euo pipefail
来源：http://yts.dianchejie.cn

[R02] 变量赋值与使用
来源：http://wde.dashuyun.cn

name="Tom"; echo "$name"
来源：http://bet.tanke756.top

[R03] 只读变量
来源：http://ism.shanyushiyangtech.top

readonly PI=3.14
来源：http://rbr.sxryk.cn

[R04] 位置参数
来源：http://nbn.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yzb.fengsongda.top

[R05] 参数默认值
来源：http://qut.nanxinkj.top

name="${1:-default}"
来源：http://nix.bbcook.cn

[R06] 判断命令是否存在
来源：http://agb.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lar.epnwcf.com

[R07] if 判断文件
来源：http://ccy.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gss.gogol.net.cn

[R08] 数值比较
来源：http://oyr.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vlf.dashuyun.cn

[R09] 字符串比较
来源：http://aah.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vlr.smart0.xyz

[R10] 正则匹配
来源：http://suy.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://erx.jyoumei.cn

[R11] case 多分支
来源：http://igd.uphjek.com

case "$1" in
来源：http://gel.cdnleiting.top

start) echo "启动" ;;
来源：http://vuc.fzhhl.top

stop)  echo "停止" ;;
来源：http://bxn.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://sgz.ydjk.org.cn

esac
来源：http://frw.yueranfly.top

[R12] for 遍历文件
来源：http://vut.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://akn.zhiwuduotai.top

[R13] for 计数循环
来源：http://uqw.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://avy.pycfn.com

[R14] C 风格 for
来源：http://jvg.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vtx.tianlin.xyz

[R15] while 逐行读文件
来源：http://wag.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kpg.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://llj.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eip.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://nzg.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://run.jqgufenzy.top

[R18] 遍历数组
来源：http://kdu.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ald.zhiwuduotai.top

[R19] 数组长度
来源：http://llq.hfpthk.cn

echo "${#arr[@]}"
来源：http://nst.xinyue.icu

[R20] 关联数组（字典）
来源：http://abn.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wan.gzhubu.top

[R21] 字符串长度
来源：http://igf.shanyushiyangtech.top

echo "${#s}"
来源：http://epf.0kj1m.cn

[R22] 截取子串
来源：http://rro.redwolf501.top

echo "${s:0:5}"
来源：http://xek.jianghu66.top

[R23] 字符串替换
来源：http://gmt.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hja.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://yri.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vyh.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://asx.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cuj.fanxiaobao.xyz

[R26] 命令替换
来源：http://ete.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://rjh.jqgfzy.top

[R27] 算术展开
来源：http://sji.uphjek.com

echo $((1 + 2 * 3))
来源：http://qyt.xziqi.cn

[R28] 浮点运算
来源：http://ktn.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://iex.yueranfly.top

[R29] 定义函数
来源：http://iej.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vnt.ppjwa.cn

[R30] 函数返回状态码
来源：http://qgf.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://sky.bbcook.cn

[R31] 局部变量
来源：http://ouw.sweek.top

f() { local x=1; echo "$x"; }
来源：http://wzy.yuanzhike.top

[R32] 参数个数校验
来源：http://iln.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://anm.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://eog.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ced.tianlin.xyz

[R34] 退出时清理
来源：http://pxy.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://hvl.aibaodan.cn

[R35] 后台执行并等待
来源：http://iot.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://kaq.c1oappe.top

[R36] 并发执行多个任务
来源：http://uia.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ntd.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://cka.pengpengdd.cyou

files=$(ls -1)
来源：http://snw.xylfe.cn

[R38] 管道串联
来源：http://npq.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://lwj.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://sqi.snrcjt.cn

cmd > out.log 2>&1
来源：http://ecm.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://nan.c1oappe.top

echo "log" >> out.log
来源：http://lun.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://mno.mhx1999.top

cmd >/dev/null 2>&1
来源：http://syn.chenzaomai.com

[R42] 输入重定向
来源：http://wja.fzhhl.top

wc -l < a.txt
来源：http://aol.daxiang520.top

[R43] 按名字查找文件
来源：http://jtc.xinyue.icu

find . -name "*.log" -type f
来源：http://zbu.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://fqe.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://xcq.wangshuangyany.cn

[R45] 批量删除
来源：http://ekx.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://qtf.guowangkeji.top

[R46] 递归替换文件内容
来源：http://vnn.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ate.tianlin.xyz

[R47] sed 单行替换
来源：http://lgy.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://mmd.vqdsnc.cn

[R48] awk 取指定列
来源：http://inj.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://yzn.yvedp.cn

[R49] awk 带条件
来源：http://eqr.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sux.uphjek.com

[R50] awk 求和
来源：http://nar.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://lix.dashuyun.cn

[R51] 排序去重取前几
来源：http://vnq.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://czd.nanxinkj.top

[R52] 统计行数
来源：http://soh.jinqigfzy.top

wc -l a.txt
来源：http://xns.meibo888.top

[R53] 查看文件头与实时尾
来源：http://kfi.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pmn.zhengqikj.top

[R54] 比较两个文件
来源：http://qro.ctjpmb.com

diff a.txt b.txt
来源：http://yle.ybcxt.top

[R55] 压缩与解压
来源：http://nmk.bbcook.cn


<!-- 参考信息 -->