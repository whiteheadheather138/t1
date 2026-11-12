代发 wailian999

);
来源：http://fnb.tian-w.cn

[Q03] 增加列
来源：http://twe.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ayc.shuidangran.top

[Q04] 修改列类型
来源：http://cxe.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zpw.fzhhl.top

[Q05] 重命名列
来源：http://ugy.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oyx.hfpthk.cn

[Q06] 删除列
来源：http://dej.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gxc.jinyuanbaomall.cn

[Q07] 删除表
来源：http://jza.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://bqg.ybcxt.top

[Q08] 创建普通索引
来源：http://jsr.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xtc.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://gsu.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oeh.haohaochexian.top

[Q10] 插入单行
来源：http://eqb.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lcm.xylfe.cn

[Q11] 一次插入多行
来源：http://kba.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jea.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://iqm.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://weq.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ynl.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://mjq.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tzx.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://war.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mrl.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rji.hesvh.cn

[Q15] 查询全部
来源：http://ujj.yanxiufei.cn

SELECT * FROM users;
来源：http://rvy.52xcode.cn

[Q16] 查询指定列
来源：http://rcp.nanxinkj.top

SELECT id, name FROM users;
来源：http://juh.sxryk.cn

[Q17] 条件查询
来源：http://mvi.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ibh.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://jsk.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://isn.cqqwz.cn

[Q19] 范围查询
来源：http://efn.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dlx.zdbjq.cn

[Q20] IN 列表
来源：http://ayw.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mys.vqdsnc.cn

[Q21] 空值判断
来源：http://zjz.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://flg.xinyue.icu

[Q22] 排序
来源：http://fsz.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zpt.jinqigfzy.top

[Q23] 分页
来源：http://qpd.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cfx.yongpay.top

[Q24] 去重
来源：http://pdh.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://pbh.uphjek.com

[Q25] 只取前 N 条
来源：http://bnx.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uvy.pengpengdd.cyou

[Q26] 计数
来源：http://pfr.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://cim.yuxming.cn

[Q27] 条件计数
来源：http://rhf.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nus.tianlin.xyz

[Q28] 求和与平均
来源：http://rcu.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://szg.cheryme.top

[Q29] 最大最小值
来源：http://oja.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xkp.cashguo.top

[Q30] 分组统计
来源：http://xha.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sbm.hnxiangtu.top

[Q31] 分组后过滤
来源：http://veq.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ctt.c1oappe.top

[Q32] 分组拼接字符串
来源：http://ayj.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pkw.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gva.gogol.net.cn

[Q33] 多列分组
来源：http://myu.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmg.meibo888.top

[Q34] 每组取第一条
来源：http://nko.mhx1999.top

SELECT * FROM (
来源：http://oqq.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zmi.gaohongyu789.top

) t WHERE rn = 1;
来源：http://vao.sweek.top

[Q35] 内连接
来源：http://qvy.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://knl.daxiang520.top

[Q36] 左连接
来源：http://ird.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bqk.ybcxt.top

[Q37] 右连接
来源：http://nvj.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fzk.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zeg.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://crl.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://lmw.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ran.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ygw.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bnx.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vov.xziqi.cn

[Q41] 多表连接
来源：http://gae.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zcm.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://qic.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://rzv.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://fyt.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://sms.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gew.svipenyu.cn

[Q43] 标量子查询
来源：http://mlk.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ieg.hysaishi.cn

[Q44] IN 子查询
来源：http://bff.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hna.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://gvd.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zif.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://kwn.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ogz.nanxinkj.top

[Q47] 与平均值比较
来源：http://izr.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://muw.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://ukv.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgm.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://nao.zhoulong.xyz

[Q49] 更新单行
来源：http://hgb.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dib.vqdsnc.cn

[Q50] 批量更新
来源：http://oly.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nsm.fzhhl.top

[Q51] 用子查询更新
来源：http://nps.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xrb.fktsv.cn

[Q52] 删除指定行
来源：http://pos.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://ykb.ctjpmb.com

[Q53] 按条件删除
来源：http://rss.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://boy.ctjpmb.com

[Q54] 清空表
来源：http://grb.nwbrower.top

TRUNCATE TABLE logs;
来源：http://igh.xylfe.cn

[Q55] 排名（并列占位）
来源：http://gem.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iin.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://fcp.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jgz.mhx1999.top

[Q57] 行号
来源：http://ebi.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sot.jinghuilouyu.cn

[Q58] 累计求和
来源：http://cmp.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tze.shangyingyoupin.top

[Q59] 分组内累计
来源：http://rgs.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ldx.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://dak.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yzq.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csw.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://idg.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eaj.xuetiantiany.cn

[Q62] 分组占比
来源：http://shv.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aan.dianchejie.cn

[Q63] 开启事务
来源：http://ozs.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ysx.yangfankeji.com

[Q64] 提交事务
来源：http://bot.ydzc1.top

COMMIT;
来源：http://vej.yongpay.top

[Q65] 回滚事务
来源：http://xsz.sxryk.cn

ROLLBACK;
来源：http://iqs.fktsv.cn

[Q66] 行锁查询
来源：http://ufy.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tvo.hnxiangtu.top

[Q67] 设置隔离级别
来源：http://qmd.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rfy.jinghuilouyu.cn

[Q68] 保存点
来源：http://uxz.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://ohx.mhx1999.top

ROLLBACK TO sp1;
来源：http://com.hammf.cn

[Q69] 查看执行计划
来源：http://tkx.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mzv.jlsjyb.cn

[Q70] 更新统计信息
来源：http://axv.nwbrower.top

ANALYZE TABLE users;
来源：http://xvx.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://btv.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oiw.quarkkingdee.top

[Q72] 查看索引
来源：http://uoj.dashuyun.cn

SHOW INDEX FROM users;
来源：http://zsu.cqqwz.cn

[Q73] 查看表状态
来源：http://lzh.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wfd.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://hcx.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://brx.dianchejie.cn

[Q75] 日期格式化
来源：http://mek.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ucn.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://emr.sufxvd.cn

[Q76] 按天统计
来源：http://jhq.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qvo.zhijiandao.cn

[Q77] 时间加减
来源：http://nkb.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhp.mhx1999.top

[Q78] 当前时间
来源：http://kaq.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxx.hnqzz.top

[Q79] 字符串拼接
来源：http://tzi.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://van.jqgufenzy.top

[Q80] 字符串截取
来源：http://vlk.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kes.epnwcf.com

[Q81] 字符串替换
来源：http://zgs.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zte.tanke756.top

[Q82] 字符长度与字节长度
来源：http://ifa.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dfy.sjlbkw.cn

[Q83] 大小写转换
来源：http://jwv.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mal.zdqjudy.top

[Q84] 去除首尾空格
来源：http://imq.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://lmm.yonumen.top

[Q85] 数值取整
来源：http://mvj.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ybv.yonumen.top

[Q86] 读取 JSON 字段
来源：http://usy.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ewx.fktsv.cn

[Q87] JSON 字段做条件
来源：http://oip.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ifo.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://coa.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dcx.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://top.0kj1m.cn

[Q89] 判断表是否存在
来源：http://axj.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yee.nanxinkj.top

[Q90] 生成序号列
来源：http://rad.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ley.dashuyun.cn

================================================================================
来源：http://ong.daxiang520.top

R. Bash 专题
来源：http://zbc.jqgufenzy.top

================================================================================
来源：http://brv.bbcook.cn

[R01] shebang 与严格模式
来源：http://qhv.yonumen.top

#!/usr/bin/env bash
来源：http://lmq.tian-w.cn

set -euo pipefail
来源：http://fxc.fktsv.cn

[R02] 变量赋值与使用
来源：http://ohi.dashuyun.cn

name="Tom"; echo "$name"
来源：http://eoa.52xcode.cn

[R03] 只读变量
来源：http://gwr.bjfxy.top

readonly PI=3.14
来源：http://xdl.daria6918.cn

[R04] 位置参数
来源：http://nfr.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ido.uphjek.com

[R05] 参数默认值
来源：http://hbm.nanxuanxn.top

name="${1:-default}"
来源：http://imi.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://hbp.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eqy.yj20258888.top

[R07] if 判断文件
来源：http://xig.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://stv.ctjpmb.com

[R08] 数值比较
来源：http://egh.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pnj.pengpengdd.cyou

[R09] 字符串比较
来源：http://aqr.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zeo.guowangkeji.top

[R10] 正则匹配
来源：http://ntv.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fhh.bjfxy.top

[R11] case 多分支
来源：http://mon.guowangkeji.top

case "$1" in
来源：http://meu.haohaochexian.top

start) echo "启动" ;;
来源：http://mjg.shzxlz.cn

stop)  echo "停止" ;;
来源：http://amf.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://pzk.yvedp.cn

esac
来源：http://awm.cucudq.cn

[R12] for 遍历文件
来源：http://chk.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://tia.xuanzx.com

[R13] for 计数循环
来源：http://xzd.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vxm.hysaishi.cn

[R14] C 风格 for
来源：http://wtt.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ogd.cheryme.top

[R15] while 逐行读文件
来源：http://yiz.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dbf.yonumen.top

[R16] until 等待条件
来源：http://wqv.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oyk.yj20258.top

[R17] 数组定义与取值
来源：http://xkf.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fzg.wangshuangyany.cn

[R18] 遍历数组
来源：http://lrd.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xxb.shuidangran.top

[R19] 数组长度
来源：http://yvu.vehdjk.com

echo "${#arr[@]}"
来源：http://kpm.zhixingplan.top

[R20] 关联数组（字典）
来源：http://jsz.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bcg.hnxiangtu.top

[R21] 字符串长度
来源：http://uxr.9152youxi.cn

echo "${#s}"
来源：http://zyj.fehbvm.com

[R22] 截取子串
来源：http://paa.sxryk.cn

echo "${s:0:5}"
来源：http://jic.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://suv.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ijs.fzhhl.top

[R24] 大小写转换
来源：http://ifp.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jun.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://egy.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xhe.mhx1999.top

[R26] 命令替换
来源：http://mld.yj202588.top

now=$(date +%F); echo "$now"
来源：http://jkr.sjlbkw.cn

[R27] 算术展开
来源：http://ouc.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://eag.kuanghao11.cn

[R28] 浮点运算
来源：http://tdp.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://nde.jlsjyb.cn

[R29] 定义函数
来源：http://bsr.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zkz.redwolf501.top

[R30] 函数返回状态码
来源：http://nen.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://cjk.mhx1999.top

[R31] 局部变量
来源：http://yel.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://xdo.hnxiangtu.top

[R32] 参数个数校验
来源：http://ekk.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://toj.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://bhp.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zdn.ybcxt.top

[R34] 退出时清理
来源：http://kcn.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://prx.tarul.cn

[R35] 后台执行并等待
来源：http://lyd.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ktj.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://qwd.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://acp.hesvh.cn

[R37] 把输出赋给变量
来源：http://aun.tianlin.xyz

files=$(ls -1)
来源：http://txv.zdbjq.cn

[R38] 管道串联
来源：http://nvc.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://vsx.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://qcj.yj202588.top

cmd > out.log 2>&1
来源：http://snx.zhoulong.xyz

[R40] 追加写日志
来源：http://owa.kuanghao11.cn

echo "log" >> out.log
来源：http://oun.jqgufenzy.top

[R41] 丢弃输出
来源：http://mpf.uphjek.com

cmd >/dev/null 2>&1
来源：http://psx.yueranfly.top

[R42] 输入重定向
来源：http://lfq.sjlbkw.cn

wc -l < a.txt
来源：http://wqq.yuxming.cn

[R43] 按名字查找文件
来源：http://jtj.jiagoushi.top

find . -name "*.log" -type f
来源：http://kbf.yueranfly.top

[R44] 按修改时间查找
来源：http://ecc.fengsongda.top

find . -mtime -7 -type f
来源：http://wdc.sufxvd.cn

[R45] 批量删除
来源：http://yro.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://uui.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://quy.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pnl.xylfe.cn

[R47] sed 单行替换
来源：http://hlo.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rjx.yanxiufei.cn

[R48] awk 取指定列
来源：http://axl.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://mda.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://urk.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ana.haohaochexian.top

[R50] awk 求和
来源：http://qdr.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gal.ehwqpu.com

[R51] 排序去重取前几
来源：http://ykm.ydjk.org.cn


<!-- 参考信息 -->