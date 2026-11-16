代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfx.birdmap.top

user_id INT NOT NULL,
来源：http://emp.epnwcf.com

amount DECIMAL(10, 2),
来源：http://utg.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://alo.hammf.cn

);
来源：http://ydi.fktsv.cn

[Q03] 增加列
来源：http://nah.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://adx.aizwys.cn

[Q04] 修改列类型
来源：http://izh.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tey.dianchejie.cn

[Q05] 重命名列
来源：http://fjs.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zjb.quarkkingdee.top

[Q06] 删除列
来源：http://pwk.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://shg.guannengcc.top

[Q07] 删除表
来源：http://fwv.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://ysw.xziqi.cn

[Q08] 创建普通索引
来源：http://aum.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qqz.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://cbn.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://spo.yj202588.top

[Q10] 插入单行
来源：http://ngf.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hzb.xylfe.cn

[Q11] 一次插入多行
来源：http://bky.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cgd.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://qfl.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nai.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qdl.ivvv.top

[Q13] 忽略重复插入
来源：http://wme.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xbc.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://jgu.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zgp.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://clw.shzxlz.cn

[Q15] 查询全部
来源：http://qhq.feifeiyinyue.top

SELECT * FROM users;
来源：http://vuc.zdqjudy.top

[Q16] 查询指定列
来源：http://zcq.vehdjk.com

SELECT id, name FROM users;
来源：http://yxz.aizwys.cn

[Q17] 条件查询
来源：http://ztd.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ylx.hnqzz.top

[Q18] 模糊匹配
来源：http://stb.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aec.ybcxt.top

[Q19] 范围查询
来源：http://grb.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lpe.yvedp.cn

[Q20] IN 列表
来源：http://ufy.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zrl.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://txl.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yqk.smart0.xyz

[Q22] 排序
来源：http://mzr.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://car.tian-w.cn

[Q23] 分页
来源：http://cst.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nml.ydjk.org.cn

[Q24] 去重
来源：http://dup.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://qmq.bbcook.cn

[Q25] 只取前 N 条
来源：http://vcu.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sfj.zycfv.cn

[Q26] 计数
来源：http://fld.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://ert.nanxinkj.top

[Q27] 条件计数
来源：http://cap.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ycy.shuidangran.top

[Q28] 求和与平均
来源：http://kcc.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wbg.fzhhl.top

[Q29] 最大最小值
来源：http://evf.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yec.shanyushiyangtech.top

[Q30] 分组统计
来源：http://fio.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yuh.sjlbkw.cn

[Q31] 分组后过滤
来源：http://bbp.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zbk.sxryk.cn

[Q32] 分组拼接字符串
来源：http://sav.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jtd.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ovo.gogol.net.cn

[Q33] 多列分组
来源：http://xom.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fcw.gotoacloud.top

[Q34] 每组取第一条
来源：http://chw.jinqigfzy.top

SELECT * FROM (
来源：http://kbb.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ufs.bbcook.cn

) t WHERE rn = 1;
来源：http://xmh.fehbvm.com

[Q35] 内连接
来源：http://qxg.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pwb.ctjpmb.com

[Q36] 左连接
来源：http://chr.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xls.dianchejie.cn

[Q37] 右连接
来源：http://biy.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xxp.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://cjl.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qhe.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://liw.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lhf.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://won.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ukg.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rkn.aibaodan.cn

[Q41] 多表连接
来源：http://dud.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gfe.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://xqi.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://tih.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://ihb.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://juo.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zok.meibo888.top

[Q43] 标量子查询
来源：http://eav.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sow.sysykeji.top

[Q44] IN 子查询
来源：http://ylv.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hkj.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://aju.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yms.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://jpq.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://enu.yangfankeji.com

[Q47] 与平均值比较
来源：http://mwf.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vmu.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://bfp.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uzg.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://lga.chenjidiqi.icu

[Q49] 更新单行
来源：http://luu.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ivs.hcnkem.com

[Q50] 批量更新
来源：http://wki.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tzb.chenzaomai.com

[Q51] 用子查询更新
来源：http://gzc.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://viv.shuidangran.top

[Q52] 删除指定行
来源：http://pgv.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://jeu.yuanzhike.top

[Q53] 按条件删除
来源：http://bka.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xqa.xinyue.icu

[Q54] 清空表
来源：http://mkb.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://fly.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://pkr.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://brh.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://ydu.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iug.bjfxy.top

[Q57] 行号
来源：http://jvg.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vxr.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://wta.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cbk.cheryme.top

[Q59] 分组内累计
来源：http://cqw.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yci.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://kbm.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vih.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kdy.gogol.net.cn

[Q61] 移动平均
来源：http://oip.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lnd.nwbrower.top

[Q62] 分组占比
来源：http://atb.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fws.sufxvd.cn

[Q63] 开启事务
来源：http://nyr.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ndb.ybcxt.top

[Q64] 提交事务
来源：http://yjr.bbcook.cn

COMMIT;
来源：http://ytq.dianchejie.cn

[Q65] 回滚事务
来源：http://apf.jinghuilouyu.cn

ROLLBACK;
来源：http://fyc.meibo888.top

[Q66] 行锁查询
来源：http://cag.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://thp.gzhubu.top

[Q67] 设置隔离级别
来源：http://duc.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://byy.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://jce.yj202588.top

SAVEPOINT sp1;
来源：http://nda.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://eay.zycfv.cn

[Q69] 查看执行计划
来源：http://twk.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hvi.shuidangran.top

[Q70] 更新统计信息
来源：http://sop.sufxvd.cn

ANALYZE TABLE users;
来源：http://jac.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://wir.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ztj.tarul.cn

[Q72] 查看索引
来源：http://att.hysaishi.cn

SHOW INDEX FROM users;
来源：http://sld.jyoumei.cn

[Q73] 查看表状态
来源：http://sbr.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zay.birdmap.top

[Q74] 强制使用索引
来源：http://tsx.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eio.ctjpmb.com

[Q75] 日期格式化
来源：http://aop.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dkg.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fnv.snrcjt.cn

[Q76] 按天统计
来源：http://ffz.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://snd.ivvv.top

[Q77] 时间加减
来源：http://ydb.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tah.tarul.cn

[Q78] 当前时间
来源：http://cez.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kje.zhiwuduotai.top

[Q79] 字符串拼接
来源：http://oyk.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nbr.shangyingyoupin.top

[Q80] 字符串截取
来源：http://vli.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kzm.dianchejie.cn

[Q81] 字符串替换
来源：http://dzu.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://coj.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://qyj.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oex.zhongyouzk.top

[Q83] 大小写转换
来源：http://nev.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rpn.yj202588.top

[Q84] 去除首尾空格
来源：http://xyz.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://vcd.wangshuangyany.cn

[Q85] 数值取整
来源：http://dnu.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lsx.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://yor.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hug.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://clu.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zfq.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://udd.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jyc.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bof.ehwqpu.com

[Q89] 判断表是否存在
来源：http://yai.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qao.yj20258.top

[Q90] 生成序号列
来源：http://fby.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cnc.xuetiantiany.cn

================================================================================
来源：http://udt.cucudq.cn

R. Bash 专题
来源：http://tqo.xingfuxueyuan.xyz

================================================================================
来源：http://ifk.hnqzz.top

[R01] shebang 与严格模式
来源：http://svl.shzxlz.cn

#!/usr/bin/env bash
来源：http://aaa.havefunace.top

set -euo pipefail
来源：http://bts.chenzaomai.com

[R02] 变量赋值与使用
来源：http://zfa.zhengqikj.top

name="Tom"; echo "$name"
来源：http://xgp.ivvv.top

[R03] 只读变量
来源：http://shs.0kj1m.cn

readonly PI=3.14
来源：http://tlc.zhijiandao.cn

[R04] 位置参数
来源：http://spg.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zrr.iojbl.cn

[R05] 参数默认值
来源：http://kkn.chenzaomai.com

name="${1:-default}"
来源：http://cfm.meibo888.top

[R06] 判断命令是否存在
来源：http://lmm.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tqp.sufxvd.cn

[R07] if 判断文件
来源：http://pwk.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fhu.nanxinkj.top

[R08] 数值比较
来源：http://ssg.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mla.xylfe.cn

[R09] 字符串比较
来源：http://hqo.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qwl.wangdashe.top

[R10] 正则匹配
来源：http://qkj.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wur.bbcook.cn

[R11] case 多分支
来源：http://aic.vehdjk.com

case "$1" in
来源：http://dcb.cheryme.top

start) echo "启动" ;;
来源：http://vex.uphjek.com

stop)  echo "停止" ;;
来源：http://yoa.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://itj.fzhhl.top

esac
来源：http://sym.yangfankeji.com

[R12] for 遍历文件
来源：http://ael.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://qvz.chenjidiqi.icu

[R13] for 计数循环
来源：http://dyv.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://nfv.zhijiandao.cn

[R14] C 风格 for
来源：http://ffi.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kgi.yongpay.top

[R15] while 逐行读文件
来源：http://ieu.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wrs.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://kxj.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hvm.cucudq.cn

[R17] 数组定义与取值
来源：http://plv.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nku.zhongyouzk.top

[R18] 遍历数组
来源：http://szo.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ynr.guannengcc.top

[R19] 数组长度
来源：http://qlu.hesvh.cn

echo "${#arr[@]}"
来源：http://ptv.dashuyun.cn

[R20] 关联数组（字典）
来源：http://pkk.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zqf.wangdashe.top

[R21] 字符串长度
来源：http://ykm.ydjk.org.cn

echo "${#s}"
来源：http://oqu.hnxiangtu.top

[R22] 截取子串
来源：http://tlb.sufxvd.cn

echo "${s:0:5}"
来源：http://dqq.cheryme.top

[R23] 字符串替换
来源：http://uay.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hvp.fzhhl.top

[R24] 大小写转换
来源：http://acp.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://nyd.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://zgo.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://afp.nanxuanxn.top

[R26] 命令替换
来源：http://dex.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://usz.zdbjq.cn

[R27] 算术展开
来源：http://dao.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://bue.dashuyun.cn

[R28] 浮点运算
来源：http://qeo.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://dic.cashguo.top

[R29] 定义函数
来源：http://scb.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lym.epnwcf.com

[R30] 函数返回状态码
来源：http://moc.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://eby.ydjk.org.cn

[R31] 局部变量
来源：http://new.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://nen.xylfe.cn

[R32] 参数个数校验
来源：http://ach.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aih.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://dhl.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wyy.ppjwa.cn

[R34] 退出时清理
来源：http://rbi.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uev.yvedp.cn

[R35] 后台执行并等待
来源：http://gez.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fvc.tian-w.cn

[R36] 并发执行多个任务
来源：http://izi.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dte.jinqigufen.top

[R37] 把输出赋给变量
来源：http://uwn.nanxinkj.top

files=$(ls -1)
来源：http://xru.hfpthk.cn

[R38] 管道串联
来源：http://ond.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://hqs.316326.xyz

[R39] 重定向标准输出与错误
来源：http://jnm.tarul.cn

cmd > out.log 2>&1
来源：http://yzb.guannengcc.top

[R40] 追加写日志
来源：http://cnl.52xcode.cn

echo "log" >> out.log
来源：http://chx.svipenyu.cn

[R41] 丢弃输出
来源：http://vro.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://xkz.birdmap.top

[R42] 输入重定向
来源：http://gdi.fzhhl.top

wc -l < a.txt
来源：http://bbk.yj202588.top

[R43] 按名字查找文件
来源：http://srf.nanxuanxn.top

find . -name "*.log" -type f
来源：http://wlp.yanxiufei.cn

[R44] 按修改时间查找
来源：http://sgv.yangfankeji.com

find . -mtime -7 -type f
来源：http://smi.wangshuangyany.cn

[R45] 批量删除
来源：http://swy.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://kzy.tianlin.xyz

[R46] 递归替换文件内容
来源：http://cnv.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zks.tianlin.xyz

[R47] sed 单行替换
来源：http://osk.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://knm.cucudq.cn

[R48] awk 取指定列
来源：http://hmp.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://mem.haohaochexian.top

[R49] awk 带条件
来源：http://ync.fengsongda.top


<!-- 参考信息 -->