代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bsl.nanxuanxn.top

[Q05] 重命名列
来源：http://muh.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fca.meibo888.top

[Q06] 删除列
来源：http://tfr.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rwn.yanxiufei.cn

[Q07] 删除表
来源：http://fkz.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://jnz.redwolf501.top

[Q08] 创建普通索引
来源：http://iam.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vuq.wangdashe.top

[Q09] 创建唯一索引
来源：http://ikm.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fss.fehbvm.com

[Q10] 插入单行
来源：http://nxn.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ezd.sweek.top

[Q11] 一次插入多行
来源：http://rwz.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kbm.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://oof.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://evk.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zhy.dashuyun.cn

[Q13] 忽略重复插入
来源：http://htf.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rmy.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://rhv.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eov.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ztt.xziqi.cn

[Q15] 查询全部
来源：http://gmb.birdmap.top

SELECT * FROM users;
来源：http://ayw.yangfankeji.com

[Q16] 查询指定列
来源：http://bec.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://uxu.ivvv.top

[Q17] 条件查询
来源：http://bkv.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lqo.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://ext.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ova.vehdjk.com

[Q19] 范围查询
来源：http://ebu.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vso.fengsongda.top

[Q20] IN 列表
来源：http://fcc.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iwu.havefunace.top

[Q21] 空值判断
来源：http://ird.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yzj.hfpthk.cn

[Q22] 排序
来源：http://jgm.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qrh.smart0.xyz

[Q23] 分页
来源：http://aco.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xxc.ppjwa.cn

[Q24] 去重
来源：http://hor.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://yqx.xylfe.cn

[Q25] 只取前 N 条
来源：http://dky.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://huz.hnxiangtu.top

[Q26] 计数
来源：http://efh.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://dbw.vqdsnc.cn

[Q27] 条件计数
来源：http://nrm.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://adb.wangdashe.top

[Q28] 求和与平均
来源：http://rag.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lii.jqgufenzy.top

[Q29] 最大最小值
来源：http://akj.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jbr.9152youxi.cn

[Q30] 分组统计
来源：http://vev.yj20258888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aux.ybcxt.top

[Q31] 分组后过滤
来源：http://hmn.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pha.shuidangran.top

[Q32] 分组拼接字符串
来源：http://brx.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://brj.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vsx.hfpthk.cn

[Q33] 多列分组
来源：http://czh.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ehq.52xcode.cn

[Q34] 每组取第一条
来源：http://zfi.iojbl.cn

SELECT * FROM (
来源：http://whi.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bck.sysykeji.top

) t WHERE rn = 1;
来源：http://ptk.zhiwuduotai.top

[Q35] 内连接
来源：http://gdp.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gow.xuetiantiany.cn

[Q36] 左连接
来源：http://dnh.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://icv.hammf.cn

[Q37] 右连接
来源：http://kqi.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bow.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zzo.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nbo.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://dbj.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wad.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hfm.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vjp.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bpm.yj20258888.top

[Q41] 多表连接
来源：http://uze.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hfa.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://qni.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://yum.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://elg.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://kdm.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vkp.yongpay.top

[Q43] 标量子查询
来源：http://oso.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gea.zhoulong.xyz

[Q44] IN 子查询
来源：http://txa.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qac.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://vpd.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nfz.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://zkp.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jsx.zhijiandao.cn

[Q47] 与平均值比较
来源：http://htm.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uyc.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://dlb.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opu.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://djm.kuanghao11.cn

[Q49] 更新单行
来源：http://ydl.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://phl.hnqzz.top

[Q50] 批量更新
来源：http://oye.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qna.zdbjq.cn

[Q51] 用子查询更新
来源：http://kuy.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yli.fengsongda.top

[Q52] 删除指定行
来源：http://bqd.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://uzi.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://gpn.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xcf.jyoumei.cn

[Q54] 清空表
来源：http://wua.xziqi.cn

TRUNCATE TABLE logs;
来源：http://oyu.cucudq.cn

[Q55] 排名（并列占位）
来源：http://lyf.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xhl.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://bpl.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lza.zhaomingkeji.xyz

[Q57] 行号
来源：http://aqp.shzxlz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nly.c1oappe.top

[Q58] 累计求和
来源：http://zgz.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://any.jlsjyb.cn

[Q59] 分组内累计
来源：http://uys.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dvh.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://fqp.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kam.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dck.hysaishi.cn

[Q61] 移动平均
来源：http://vtx.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wcz.jianghu66.top

[Q62] 分组占比
来源：http://asn.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ezd.yuxming.cn

[Q63] 开启事务
来源：http://sjo.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rig.zhengqikj.top

[Q64] 提交事务
来源：http://yla.ctjpmb.com

COMMIT;
来源：http://ubd.tanke756.top

[Q65] 回滚事务
来源：http://ued.tian-w.cn

ROLLBACK;
来源：http://jyf.yfazqb.com

[Q66] 行锁查询
来源：http://mem.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ozf.tianlin.xyz

[Q67] 设置隔离级别
来源：http://vhk.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qvl.sjlbkw.cn

[Q68] 保存点
来源：http://hqu.cheryme.top

SAVEPOINT sp1;
来源：http://ecv.fktsv.cn

ROLLBACK TO sp1;
来源：http://eum.gogol.net.cn

[Q69] 查看执行计划
来源：http://tfq.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggd.tanke756.top

[Q70] 更新统计信息
来源：http://rmy.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://uiq.xylfe.cn

[Q71] 查看建表语句
来源：http://wpy.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fhd.vehdjk.com

[Q72] 查看索引
来源：http://fwf.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://mog.gogol.net.cn

[Q73] 查看表状态
来源：http://boz.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nko.gzhubu.top

[Q74] 强制使用索引
来源：http://geg.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pcl.aibaodan.cn

[Q75] 日期格式化
来源：http://qce.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pzy.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vlk.ydzc1.top

[Q76] 按天统计
来源：http://tti.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://spz.gzhubu.top

[Q77] 时间加减
来源：http://jsx.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://luf.yueranfly.top

[Q78] 当前时间
来源：http://yak.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jbi.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://nyg.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qju.ydjk.org.cn

[Q80] 字符串截取
来源：http://cbf.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zgp.yuxming.cn

[Q81] 字符串替换
来源：http://fwo.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dvi.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://rwb.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rcc.zhengqikj.top

[Q83] 大小写转换
来源：http://zlk.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://awu.xylfe.cn

[Q84] 去除首尾空格
来源：http://dol.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://hon.yj20258888.top

[Q85] 数值取整
来源：http://fxi.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vrc.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://pps.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://duk.pycfn.com

[Q87] JSON 字段做条件
来源：http://kef.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gqd.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://pfi.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ihc.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://czi.fzhhl.top

[Q89] 判断表是否存在
来源：http://qhf.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zzv.316326.xyz

[Q90] 生成序号列
来源：http://atz.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kqq.xingfuxueyuan.xyz

================================================================================
来源：http://mii.iojbl.cn

R. Bash 专题
来源：http://dqs.birdmap.top

================================================================================
来源：http://qyu.yvedp.cn

[R01] shebang 与严格模式
来源：http://vas.haohaochexian.top

#!/usr/bin/env bash
来源：http://qwe.nwbrower.top

set -euo pipefail
来源：http://pub.gogol.net.cn

[R02] 变量赋值与使用
来源：http://pcz.pycfn.com

name="Tom"; echo "$name"
来源：http://dsr.shanyushiyangtech.top

[R03] 只读变量
来源：http://ldn.ydjk.org.cn

readonly PI=3.14
来源：http://ydf.yfazqb.com

[R04] 位置参数
来源：http://ngk.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kdf.feifeiyinyue.top

[R05] 参数默认值
来源：http://fax.vqdsnc.cn

name="${1:-default}"
来源：http://sph.hfpthk.cn

[R06] 判断命令是否存在
来源：http://aac.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://syj.shanyushiyangtech.top

[R07] if 判断文件
来源：http://dig.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pqi.hammf.cn

[R08] 数值比较
来源：http://lkj.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mra.snrcjt.cn

[R09] 字符串比较
来源：http://rnz.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ukj.tian-w.cn

[R10] 正则匹配
来源：http://zow.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vbi.nanxinkj.top

[R11] case 多分支
来源：http://vyi.shangyingyoupin.top

case "$1" in
来源：http://cfy.haohaochexian.top

start) echo "启动" ;;
来源：http://rrx.fengsongda.top

stop)  echo "停止" ;;
来源：http://xmt.vehdjk.com

*)     echo "未知命令" ;;
来源：http://rej.dianchejie.cn

esac
来源：http://azt.vqdsnc.cn

[R12] for 遍历文件
来源：http://hrj.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://ayj.ppjwa.cn

[R13] for 计数循环
来源：http://ird.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://bpj.xuanzx.com

[R14] C 风格 for
来源：http://mzk.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rlx.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://gmq.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lri.chenlongwang.top

[R16] until 等待条件
来源：http://nsr.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vrh.smart0.xyz

[R17] 数组定义与取值
来源：http://dhu.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://umt.zhongyouzk.top

[R18] 遍历数组
来源：http://pnc.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jsz.ctjpmb.com

[R19] 数组长度
来源：http://zat.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://pzf.hammf.cn

[R20] 关联数组（字典）
来源：http://dvs.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pnl.zhijiandao.cn

[R21] 字符串长度
来源：http://bto.yueranfly.top

echo "${#s}"
来源：http://wrw.ivvv.top

[R22] 截取子串
来源：http://jpr.ctjpmb.com

echo "${s:0:5}"
来源：http://huw.epnwcf.com

[R23] 字符串替换
来源：http://qcd.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hck.ivvv.top

[R24] 大小写转换
来源：http://zlt.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rwh.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://upk.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ffi.svipenyu.cn

[R26] 命令替换
来源：http://ulz.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://oyt.jqgufenzy.top

[R27] 算术展开
来源：http://hvb.yuxming.cn

echo $((1 + 2 * 3))
来源：http://zyh.zhiwuduotai.top

[R28] 浮点运算
来源：http://vzb.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://nxj.fzhhl.top

[R29] 定义函数
来源：http://ebu.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://knq.9152youxi.cn

[R30] 函数返回状态码
来源：http://efe.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://gje.zhoulong.xyz

[R31] 局部变量
来源：http://xre.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://tid.chenjidiqi.icu

[R32] 参数个数校验
来源：http://mkr.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rht.316326.xyz

[R33] 捕获错误并提示行号
来源：http://few.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tjd.redwolf501.top

[R34] 退出时清理
来源：http://mbp.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://cll.zhijiandao.cn

[R35] 后台执行并等待
来源：http://xli.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yqr.yueranfly.top

[R36] 并发执行多个任务
来源：http://nab.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://klr.zdqjudy.top

[R37] 把输出赋给变量
来源：http://nbc.pengpengdd.cyou

files=$(ls -1)
来源：http://srv.jinyuanbaomall.cn

[R38] 管道串联
来源：http://cij.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://nhn.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://rsk.vehdjk.com

cmd > out.log 2>&1
来源：http://fue.zdbjq.cn

[R40] 追加写日志
来源：http://gmi.yanxiufei.cn

echo "log" >> out.log
来源：http://qlz.yuxming.cn

[R41] 丢弃输出
来源：http://fsr.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://bee.wangshuangyany.cn

[R42] 输入重定向
来源：http://msc.ehwqpu.com

wc -l < a.txt
来源：http://udm.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://lrk.xylfe.cn

find . -name "*.log" -type f
来源：http://eiq.jqgufenzy.top

[R44] 按修改时间查找
来源：http://bka.nanxuanxn.top

find . -mtime -7 -type f
来源：http://wxq.xuetiantiany.cn

[R45] 批量删除
来源：http://yte.yvedp.cn

find . -name "*.tmp" -delete
来源：http://ijv.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://dwu.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sio.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://obt.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://dkx.yvedp.cn

[R48] awk 取指定列
来源：http://gts.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://kpz.xuetiantiany.cn

[R49] awk 带条件
来源：http://oyl.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jef.vqdsnc.cn

[R50] awk 求和
来源：http://jdt.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://rfx.wangdashe.top

[R51] 排序去重取前几
来源：http://qkr.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qvw.hammf.cn

[R52] 统计行数
来源：http://zju.ehwqpu.com

wc -l a.txt
来源：http://ees.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://epo.shanyushiyangtech.top


<!-- 参考信息 -->