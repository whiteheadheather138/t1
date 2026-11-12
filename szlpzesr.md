代发 wailian999

);
来源：http://zac.andypj.xyz

[Q03] 增加列
来源：http://qtu.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqc.zhiwuduotai.top

[Q04] 修改列类型
来源：http://rep.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iuc.vqdsnc.cn

[Q05] 重命名列
来源：http://uya.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lfp.sufxvd.cn

[Q06] 删除列
来源：http://sjq.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uqb.shuidangran.top

[Q07] 删除表
来源：http://pkf.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://xpp.zhixingplan.top

[Q08] 创建普通索引
来源：http://ohl.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lai.yonumen.top

[Q09] 创建唯一索引
来源：http://pjp.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lkp.vqdsnc.cn

[Q10] 插入单行
来源：http://rbq.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ych.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://pfz.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gvo.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://ohv.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cie.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mwi.gotoacloud.top

[Q13] 忽略重复插入
来源：http://lja.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mdc.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://wor.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gny.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yow.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://mfz.c1oappe.top

SELECT * FROM users;
来源：http://bxa.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://dlf.yj20258.top

SELECT id, name FROM users;
来源：http://esc.cqqwz.cn

[Q17] 条件查询
来源：http://iqx.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://glq.sxryk.cn

[Q18] 模糊匹配
来源：http://ewx.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jcr.fktsv.cn

[Q19] 范围查询
来源：http://vfp.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vco.wangdashe.top

[Q20] IN 列表
来源：http://oic.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nto.daria6918.cn

[Q21] 空值判断
来源：http://haa.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://quf.ctjpmb.com

[Q22] 排序
来源：http://wvn.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uhd.yuxming.cn

[Q23] 分页
来源：http://mue.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wpg.jinyuanbaomall.cn

[Q24] 去重
来源：http://jof.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://fuh.mhx1999.top

[Q25] 只取前 N 条
来源：http://ssr.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sit.cheryme.top

[Q26] 计数
来源：http://mds.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://vhu.cashguo.top

[Q27] 条件计数
来源：http://qrr.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dpp.zhixingplan.top

[Q28] 求和与平均
来源：http://jyl.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wvg.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://lcr.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://eob.316326.xyz

[Q30] 分组统计
来源：http://tdr.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qai.ivvv.top

[Q31] 分组后过滤
来源：http://brl.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://egw.zycfv.cn

[Q32] 分组拼接字符串
来源：http://oir.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://evv.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ckr.hfpthk.cn

[Q33] 多列分组
来源：http://pfg.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fqr.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://ckz.yj20258888.top

SELECT * FROM (
来源：http://weq.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zni.0kj1m.cn

) t WHERE rn = 1;
来源：http://owu.andypj.xyz

[Q35] 内连接
来源：http://stn.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iri.hesvh.cn

[Q36] 左连接
来源：http://kwi.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jqp.gaohongyu789.top

[Q37] 右连接
来源：http://uwn.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://btk.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://mno.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lsq.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://cqv.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gae.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xlm.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://brg.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ltz.haohaochexian.top

[Q41] 多表连接
来源：http://dkr.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tqb.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://fpm.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://odm.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://gux.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://nvc.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mnl.xinyue.icu

[Q43] 标量子查询
来源：http://pcz.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ffx.xuetiantiany.cn

[Q44] IN 子查询
来源：http://aib.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iur.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://jqc.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cff.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sws.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fbu.meibo888.top

[Q47] 与平均值比较
来源：http://lrz.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mgo.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://mbb.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mwe.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://nuj.shuidangran.top

[Q49] 更新单行
来源：http://nbn.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rtx.fzhhl.top

[Q50] 批量更新
来源：http://xql.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dxa.fzhhl.top

[Q51] 用子查询更新
来源：http://pzo.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://boq.nwbrower.top

[Q52] 删除指定行
来源：http://rzq.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://vgd.sysykeji.top

[Q53] 按条件删除
来源：http://rra.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kbo.ydjk.org.cn

[Q54] 清空表
来源：http://hyw.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://ifw.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://war.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eyg.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://xtg.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jej.haohaochexian.top

[Q57] 行号
来源：http://skb.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zmh.smart0.xyz

[Q58] 累计求和
来源：http://jhj.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yrw.xziqi.cn

[Q59] 分组内累计
来源：http://ssy.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dwu.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://cja.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://woe.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bso.dianchejie.cn

[Q61] 移动平均
来源：http://ycq.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oyj.ctjpmb.com

[Q62] 分组占比
来源：http://vke.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eqk.cucudq.cn

[Q63] 开启事务
来源：http://ylt.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wxc.daxiang520.top

[Q64] 提交事务
来源：http://dmf.gaohongyu789.top

COMMIT;
来源：http://qma.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://yla.fanxiaobao.xyz

ROLLBACK;
来源：http://xyl.uphjek.com

[Q66] 行锁查询
来源：http://xws.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kai.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://unv.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zvj.fktsv.cn

[Q68] 保存点
来源：http://ccr.gotoacloud.top

SAVEPOINT sp1;
来源：http://tey.aizwys.cn

ROLLBACK TO sp1;
来源：http://xvv.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://xuf.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ybs.yfazqb.com

[Q70] 更新统计信息
来源：http://gui.gogol.net.cn

ANALYZE TABLE users;
来源：http://roz.yonumen.top

[Q71] 查看建表语句
来源：http://axi.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wwv.yanxiufei.cn

[Q72] 查看索引
来源：http://bxh.hfpthk.cn

SHOW INDEX FROM users;
来源：http://gbr.tarul.cn

[Q73] 查看表状态
来源：http://wgm.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yru.smart0.xyz

[Q74] 强制使用索引
来源：http://ypm.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gfi.iojbl.cn

[Q75] 日期格式化
来源：http://jhv.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nfd.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://unt.havefunace.top

[Q76] 按天统计
来源：http://ciq.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hff.zhengqikj.top

[Q77] 时间加减
来源：http://bid.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://juk.jyoumei.cn

[Q78] 当前时间
来源：http://oxt.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://taf.birdmap.top

[Q79] 字符串拼接
来源：http://vlx.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xxj.zhijiandao.cn

[Q80] 字符串截取
来源：http://pws.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nbz.yuxming.cn

[Q81] 字符串替换
来源：http://vhp.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vup.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://qhq.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://csk.jqgfzy.top

[Q83] 大小写转换
来源：http://web.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rst.chenzaomai.com

[Q84] 去除首尾空格
来源：http://klj.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://ckx.nanxinkj.top

[Q85] 数值取整
来源：http://bcv.aibaodan.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://smb.yonumen.top

[Q86] 读取 JSON 字段
来源：http://sbj.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fcf.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://epf.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qag.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://ccv.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yyc.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://snz.yuanzhike.top

[Q89] 判断表是否存在
来源：http://ari.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ogk.tianlin.xyz

[Q90] 生成序号列
来源：http://wfv.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ytu.shangyingyoupin.top

================================================================================
来源：http://yns.nanxinkj.top

R. Bash 专题
来源：http://lpn.hfpthk.cn

================================================================================
来源：http://mze.yuanzhike.top

[R01] shebang 与严格模式
来源：http://rpk.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://zrb.yonumen.top

set -euo pipefail
来源：http://tvc.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://yqf.fengsongda.top

name="Tom"; echo "$name"
来源：http://zoq.sufxvd.cn

[R03] 只读变量
来源：http://kdk.gogol.net.cn

readonly PI=3.14
来源：http://ccn.mhx1999.top

[R04] 位置参数
来源：http://fqs.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://opr.cqqwz.cn

[R05] 参数默认值
来源：http://tni.yfazqb.com

name="${1:-default}"
来源：http://zot.epnwcf.com

[R06] 判断命令是否存在
来源：http://xgs.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://guh.jinghuilouyu.cn

[R07] if 判断文件
来源：http://dua.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wxy.sweek.top

[R08] 数值比较
来源：http://wiq.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dur.ydjk.org.cn

[R09] 字符串比较
来源：http://dyn.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lzq.quarkkingdee.top

[R10] 正则匹配
来源：http://ehs.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qwd.svipenyu.cn

[R11] case 多分支
来源：http://msn.mhx1999.top

case "$1" in
来源：http://xjv.yfazqb.com

start) echo "启动" ;;
来源：http://jqw.ivvv.top

stop)  echo "停止" ;;
来源：http://ipi.yvedp.cn

*)     echo "未知命令" ;;
来源：http://hsg.sweek.top

esac
来源：http://jvh.sxryk.cn

[R12] for 遍历文件
来源：http://fez.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://bcz.nanxuanxn.top

[R13] for 计数循环
来源：http://bpk.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://gyg.cheryme.top

[R14] C 风格 for
来源：http://eeo.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kyb.aibaodan.cn

[R15] while 逐行读文件
来源：http://mfs.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://etp.c1oappe.top

[R16] until 等待条件
来源：http://wac.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tps.52xcode.cn

[R17] 数组定义与取值
来源：http://ree.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://ldt.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://ltt.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mil.sufxvd.cn

[R19] 数组长度
来源：http://bfv.yuxming.cn

echo "${#arr[@]}"
来源：http://yxf.c1oappe.top

[R20] 关联数组（字典）
来源：http://ftc.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://crm.uphjek.com

[R21] 字符串长度
来源：http://jwe.jyoumei.cn

echo "${#s}"
来源：http://mht.epnwcf.com

[R22] 截取子串
来源：http://ytt.wangshuangyany.cn

echo "${s:0:5}"
来源：http://hcc.sxryk.cn

[R23] 字符串替换
来源：http://llc.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zbe.sweek.top

[R24] 大小写转换
来源：http://owm.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://fbr.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://nxk.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xrp.gzhubu.top

[R26] 命令替换
来源：http://zpy.yj20258.top

now=$(date +%F); echo "$now"
来源：http://zib.cqqwz.cn

[R27] 算术展开
来源：http://zoa.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://kio.yanxiufei.cn

[R28] 浮点运算
来源：http://nrk.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://hit.chenzaomai.com

[R29] 定义函数
来源：http://rys.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cep.andypj.xyz

[R30] 函数返回状态码
来源：http://cbe.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://pka.xuanzx.com

[R31] 局部变量
来源：http://tgm.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://uba.cdnleiting.top

[R32] 参数个数校验
来源：http://wtl.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://obt.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://cnl.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wux.ybcxt.top

[R34] 退出时清理
来源：http://wjv.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://pfd.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://rqr.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://far.ybcxt.top

[R36] 并发执行多个任务
来源：http://ytw.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sjm.yuanzhike.top

[R37] 把输出赋给变量
来源：http://xiy.shangyingyoupin.top

files=$(ls -1)
来源：http://pos.xylfe.cn

[R38] 管道串联
来源：http://hfr.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://teb.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://yxl.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://jkr.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://qka.dashuyun.cn

echo "log" >> out.log
来源：http://dok.jyoumei.cn

[R41] 丢弃输出
来源：http://qax.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://tun.yuxming.cn

[R42] 输入重定向
来源：http://uuu.yueranfly.top

wc -l < a.txt
来源：http://qwf.hammf.cn

[R43] 按名字查找文件
来源：http://wlu.jqgufenzy.top

find . -name "*.log" -type f
来源：http://khp.wangdashe.top

[R44] 按修改时间查找
来源：http://zpb.hammf.cn

find . -mtime -7 -type f
来源：http://der.jqgfzy.top

[R45] 批量删除
来源：http://tff.xuanzx.com

find . -name "*.tmp" -delete
来源：http://naw.hnqzz.top

[R46] 递归替换文件内容
来源：http://pvg.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qqq.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://teo.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://xsd.ybcxt.top

[R48] awk 取指定列
来源：http://hgv.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://vov.0kj1m.cn

[R49] awk 带条件
来源：http://xns.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pyu.tanke756.top

[R50] awk 求和
来源：http://eqn.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://zee.yangfankeji.com

[R51] 排序去重取前几
来源：http://uch.sweek.top


<!-- 参考信息 -->