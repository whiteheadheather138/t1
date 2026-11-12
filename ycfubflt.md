代发 wailian999

);
来源：http://gkf.mhx1999.top

[Q03] 增加列
来源：http://dpz.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ago.aibaodan.cn

[Q04] 修改列类型
来源：http://pdy.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hyr.fanxiaobao.xyz

[Q05] 重命名列
来源：http://bwn.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qpb.hysaishi.cn

[Q06] 删除列
来源：http://ect.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://tjd.52xcode.cn

[Q07] 删除表
来源：http://vyc.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://ohg.gogol.net.cn

[Q08] 创建普通索引
来源：http://isx.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://drt.fktsv.cn

[Q09] 创建唯一索引
来源：http://ujr.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://llh.aibaodan.cn

[Q10] 插入单行
来源：http://pkm.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eme.yj20258.top

[Q11] 一次插入多行
来源：http://edh.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sdh.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://cku.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://gfn.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gpa.mhx1999.top

[Q13] 忽略重复插入
来源：http://gxi.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xxk.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://zyh.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgc.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dtx.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://mqa.quarkkingdee.top

SELECT * FROM users;
来源：http://xuv.epnwcf.com

[Q16] 查询指定列
来源：http://qwi.ctjpmb.com

SELECT id, name FROM users;
来源：http://dgs.zdbjq.cn

[Q17] 条件查询
来源：http://lim.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbh.tian-w.cn

[Q18] 模糊匹配
来源：http://slv.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wob.ivvv.top

[Q19] 范围查询
来源：http://cgi.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mzv.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://dws.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lzx.fengsongda.top

[Q21] 空值判断
来源：http://lap.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ypc.quarkkingdee.top

[Q22] 排序
来源：http://mlp.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bcz.snrcjt.cn

[Q23] 分页
来源：http://njg.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sah.ppjwa.cn

[Q24] 去重
来源：http://rya.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://mrq.yonumen.top

[Q25] 只取前 N 条
来源：http://nih.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pzq.havefunace.top

[Q26] 计数
来源：http://imb.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://hra.tanke756.top

[Q27] 条件计数
来源：http://dfp.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgp.cqqwz.cn

[Q28] 求和与平均
来源：http://sit.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hjm.bjfxy.top

[Q29] 最大最小值
来源：http://zxr.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uzr.uphjek.com

[Q30] 分组统计
来源：http://xjq.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xpb.chenlongwang.top

[Q31] 分组后过滤
来源：http://dsd.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gxv.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://xkr.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xjg.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qym.nwbrower.top

[Q33] 多列分组
来源：http://wjc.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xgx.snrcjt.cn

[Q34] 每组取第一条
来源：http://nqv.wangshuangyany.cn

SELECT * FROM (
来源：http://swj.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rie.yuanzhike.top

) t WHERE rn = 1;
来源：http://isg.epnwcf.com

[Q35] 内连接
来源：http://hsp.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vmv.haohaochexian.top

[Q36] 左连接
来源：http://qkq.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yrx.hnxiangtu.top

[Q37] 右连接
来源：http://cji.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xqi.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://znt.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ezv.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://ofi.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nzh.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqy.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://duc.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ovo.aibaodan.cn

[Q41] 多表连接
来源：http://kqy.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zwg.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://nmc.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://zzm.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://cst.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://xqv.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kde.quarkkingdee.top

[Q43] 标量子查询
来源：http://yfl.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yni.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://cwf.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcc.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://cvi.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://leo.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://mmp.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvd.havefunace.top

[Q47] 与平均值比较
来源：http://itw.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cdr.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://mqh.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vsr.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://egd.sufxvd.cn

[Q49] 更新单行
来源：http://fjt.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kfe.hesvh.cn

[Q50] 批量更新
来源：http://sae.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fho.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://wja.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yba.xziqi.cn

[Q52] 删除指定行
来源：http://cfn.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://waz.iojbl.cn

[Q53] 按条件删除
来源：http://veb.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fgn.jinyuanbaomall.cn

[Q54] 清空表
来源：http://slv.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://jjc.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://uzt.fehbvm.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://liv.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://zir.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dfv.gzhubu.top

[Q57] 行号
来源：http://vlv.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ddh.zhengqikj.top

[Q58] 累计求和
来源：http://luh.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gxp.redwolf501.top

[Q59] 分组内累计
来源：http://okz.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zho.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://ulf.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aiv.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://awr.dashuyun.cn

[Q61] 移动平均
来源：http://oqs.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mde.tian-w.cn

[Q62] 分组占比
来源：http://hkw.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tlh.shangyingyoupin.top

[Q63] 开启事务
来源：http://rxn.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xfg.ydjk.org.cn

[Q64] 提交事务
来源：http://jdz.yueranfly.top

COMMIT;
来源：http://rjg.yongpay.top

[Q65] 回滚事务
来源：http://zwz.zdbjq.cn

ROLLBACK;
来源：http://fbc.yuxming.cn

[Q66] 行锁查询
来源：http://hah.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fuz.yj20258888.top

[Q67] 设置隔离级别
来源：http://eku.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ykj.vqdsnc.cn

[Q68] 保存点
来源：http://rel.ybcxt.top

SAVEPOINT sp1;
来源：http://nhq.chenzaomai.com

ROLLBACK TO sp1;
来源：http://vvp.aibaodan.cn

[Q69] 查看执行计划
来源：http://cya.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vvr.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://nxw.zycfv.cn

ANALYZE TABLE users;
来源：http://ogc.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://ifp.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iri.zdbjq.cn

[Q72] 查看索引
来源：http://gdr.haohaochexian.top

SHOW INDEX FROM users;
来源：http://pfe.yvedp.cn

[Q73] 查看表状态
来源：http://owy.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://otz.hnqzz.top

[Q74] 强制使用索引
来源：http://mdt.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ouc.tianlin.xyz

[Q75] 日期格式化
来源：http://cpj.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://npx.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vkv.xuetiantiany.cn

[Q76] 按天统计
来源：http://jug.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xkm.0kj1m.cn

[Q77] 时间加减
来源：http://brd.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yxd.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://fbj.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zse.zhoulong.xyz

[Q79] 字符串拼接
来源：http://wva.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ywh.gzhubu.top

[Q80] 字符串截取
来源：http://hjp.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://npp.sjlbkw.cn

[Q81] 字符串替换
来源：http://scm.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hxk.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://lhu.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zyv.jqgufenzy.top

[Q83] 大小写转换
来源：http://twt.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tko.sxryk.cn

[Q84] 去除首尾空格
来源：http://pqj.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://jsa.daxiang520.top

[Q85] 数值取整
来源：http://xwt.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wjp.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://ezz.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uny.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://dfq.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gsl.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://nee.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gic.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fnq.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://ied.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bkt.hnxiangtu.top

[Q90] 生成序号列
来源：http://jow.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nrx.sxryk.cn

================================================================================
来源：http://tqo.hcnkem.com

R. Bash 专题
来源：http://wrj.jiagoushi.top

================================================================================
来源：http://jpb.0kj1m.cn

[R01] shebang 与严格模式
来源：http://nvg.tarul.cn

#!/usr/bin/env bash
来源：http://amg.kuanghao11.cn

set -euo pipefail
来源：http://jpd.yuxming.cn

[R02] 变量赋值与使用
来源：http://znh.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://wds.hongshengwenyu.top

[R03] 只读变量
来源：http://pqo.aibaodan.cn

readonly PI=3.14
来源：http://ycc.sysykeji.top

[R04] 位置参数
来源：http://ucn.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cit.shuidangran.top

[R05] 参数默认值
来源：http://xyh.xuanzx.com

name="${1:-default}"
来源：http://inu.0kj1m.cn

[R06] 判断命令是否存在
来源：http://xaw.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ewc.redwolf501.top

[R07] if 判断文件
来源：http://wqo.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jyy.shzxlz.cn

[R08] 数值比较
来源：http://frt.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://goq.cashguo.top

[R09] 字符串比较
来源：http://ksh.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://prn.nanxinkj.top

[R10] 正则匹配
来源：http://mfv.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zpj.ydzc1.top

[R11] case 多分支
来源：http://xip.uphjek.com

case "$1" in
来源：http://kud.52xcode.cn

start) echo "启动" ;;
来源：http://baq.yonumen.top

stop)  echo "停止" ;;
来源：http://faf.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://hes.svipenyu.cn

esac
来源：http://lck.yfazqb.com

[R12] for 遍历文件
来源：http://uuj.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://mhp.tian-w.cn

[R13] for 计数循环
来源：http://lce.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://pub.chenzaomai.com

[R14] C 风格 for
来源：http://izg.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pcl.aizwys.cn

[R15] while 逐行读文件
来源：http://app.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mnv.cashguo.top

[R16] until 等待条件
来源：http://nzp.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nuw.dianchejie.cn

[R17] 数组定义与取值
来源：http://tns.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://fxa.shanyushiyangtech.top

[R18] 遍历数组
来源：http://ncb.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eje.zhiwuduotai.top

[R19] 数组长度
来源：http://lwd.fzhhl.top

echo "${#arr[@]}"
来源：http://rxw.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://hdd.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ech.9152youxi.cn

[R21] 字符串长度
来源：http://irn.hywenlv.cn

echo "${#s}"
来源：http://lgq.cdnleiting.top

[R22] 截取子串
来源：http://vnf.c1oappe.top

echo "${s:0:5}"
来源：http://gmj.meibo888.top

[R23] 字符串替换
来源：http://rmx.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mia.jinqigufen.top

[R24] 大小写转换
来源：http://uup.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ohy.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://int.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jrq.redwolf501.top

[R26] 命令替换
来源：http://thj.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://rkr.c1oappe.top

[R27] 算术展开
来源：http://zan.bbcook.cn

echo $((1 + 2 * 3))
来源：http://woo.quarkkingdee.top

[R28] 浮点运算
来源：http://het.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://zgw.cdnleiting.top

[R29] 定义函数
来源：http://zvl.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lmo.gotoacloud.top

[R30] 函数返回状态码
来源：http://lgq.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://rsx.zdbjq.cn

[R31] 局部变量
来源：http://eea.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://xxh.pycfn.com

[R32] 参数个数校验
来源：http://jhr.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jeo.hammf.cn

[R33] 捕获错误并提示行号
来源：http://mgm.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vzm.hnxiangtu.top

[R34] 退出时清理
来源：http://woq.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://psq.pycfn.com

[R35] 后台执行并等待
来源：http://ngg.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iif.yueranfly.top

[R36] 并发执行多个任务
来源：http://xhj.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ehp.zhengqikj.top

[R37] 把输出赋给变量
来源：http://cqc.haohaochexian.top

files=$(ls -1)
来源：http://viy.uphjek.com

[R38] 管道串联
来源：http://soo.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://zim.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://cfh.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://lrk.aibaodan.cn

[R40] 追加写日志
来源：http://fwk.mhx1999.top

echo "log" >> out.log
来源：http://lxh.svipenyu.cn

[R41] 丢弃输出
来源：http://dic.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://rsw.ivvv.top

[R42] 输入重定向
来源：http://syz.xylfe.cn

wc -l < a.txt
来源：http://jnl.jiagoushi.top

[R43] 按名字查找文件
来源：http://xmj.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://okk.dianchejie.cn

[R44] 按修改时间查找
来源：http://bvb.xylfe.cn

find . -mtime -7 -type f
来源：http://xgg.gzhubu.top

[R45] 批量删除
来源：http://wyk.daxiang520.top

find . -name "*.tmp" -delete
来源：http://dwt.jyoumei.cn

[R46] 递归替换文件内容
来源：http://wdt.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ekz.sjlbkw.cn

[R47] sed 单行替换
来源：http://toe.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mkh.guowangkeji.top

[R48] awk 取指定列
来源：http://qdb.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://crw.yonumen.top

[R49] awk 带条件
来源：http://ufu.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://skg.9152youxi.cn

[R50] awk 求和
来源：http://zoq.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tms.aizwys.cn

[R51] 排序去重取前几
来源：http://qip.xuetiantiany.cn


<!-- 参考信息 -->