代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ptz.xinyue.icu

[Q05] 重命名列
来源：http://ili.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gfn.sjlbkw.cn

[Q06] 删除列
来源：http://fjq.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://xbk.tianlin.xyz

[Q07] 删除表
来源：http://dss.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://zvk.pycfn.com

[Q08] 创建普通索引
来源：http://nmw.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mhw.cucudq.cn

[Q09] 创建唯一索引
来源：http://khp.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://adk.jinqigufen.top

[Q10] 插入单行
来源：http://hkx.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwt.zhoulong.xyz

[Q11] 一次插入多行
来源：http://zff.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cih.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://tbg.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://yyg.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cxn.nanxinkj.top

[Q13] 忽略重复插入
来源：http://prx.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gmn.yj20258888.top

[Q14] 存在则更新（upsert）
来源：http://cpu.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ovn.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cim.9152youxi.cn

[Q15] 查询全部
来源：http://hct.cdnleiting.top

SELECT * FROM users;
来源：http://ddr.yueranfly.top

[Q16] 查询指定列
来源：http://nak.guowangkeji.top

SELECT id, name FROM users;
来源：http://lyq.xuetiantiany.cn

[Q17] 条件查询
来源：http://kzj.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dah.sweek.top

[Q18] 模糊匹配
来源：http://cxt.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dpt.fanxiaobao.xyz

[Q19] 范围查询
来源：http://jhi.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hnq.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://lbe.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://adb.52xcode.cn

[Q21] 空值判断
来源：http://icj.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bes.xuanzx.com

[Q22] 排序
来源：http://opd.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zjm.zdqjudy.top

[Q23] 分页
来源：http://tlw.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sfh.zhixingplan.top

[Q24] 去重
来源：http://vkd.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://lpb.hcnkem.com

[Q25] 只取前 N 条
来源：http://yas.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nmd.zhengqikj.top

[Q26] 计数
来源：http://elu.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://ale.redwolf501.top

[Q27] 条件计数
来源：http://jwz.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rvc.zhixingplan.top

[Q28] 求和与平均
来源：http://bna.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zdq.iojbl.cn

[Q29] 最大最小值
来源：http://qam.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cuc.9152youxi.cn

[Q30] 分组统计
来源：http://xni.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zcy.zycfv.cn

[Q31] 分组后过滤
来源：http://ajt.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dcx.mhx1999.top

[Q32] 分组拼接字符串
来源：http://ebg.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tly.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rll.hnqzz.top

[Q33] 多列分组
来源：http://nkp.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fka.cheryme.top

[Q34] 每组取第一条
来源：http://ibq.jyoumei.cn

SELECT * FROM (
来源：http://ifj.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://plf.jqgfzy.top

) t WHERE rn = 1;
来源：http://tvt.gaohongyu789.top

[Q35] 内连接
来源：http://xif.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xci.hfpthk.cn

[Q36] 左连接
来源：http://acr.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ywa.tanke756.top

[Q37] 右连接
来源：http://wte.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ycv.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kze.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jjg.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://omr.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dmu.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xwo.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hyb.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zcg.yj20258888.top

[Q41] 多表连接
来源：http://exj.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxr.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://kaj.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://lwk.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://ora.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://nrf.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://svi.daxiang520.top

[Q43] 标量子查询
来源：http://dvf.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bhk.gotoacloud.top

[Q44] IN 子查询
来源：http://ngn.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xay.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://xqj.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ena.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xeb.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dap.aibaodan.cn

[Q47] 与平均值比较
来源：http://twi.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zbw.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://pee.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mef.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://zmq.zhiwuduotai.top

[Q49] 更新单行
来源：http://awb.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yjl.ydjk.org.cn

[Q50] 批量更新
来源：http://bni.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lcs.tianlin.xyz

[Q51] 用子查询更新
来源：http://hch.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tya.uphjek.com

[Q52] 删除指定行
来源：http://tmi.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://mjf.tian-w.cn

[Q53] 按条件删除
来源：http://itm.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wqn.hysaishi.cn

[Q54] 清空表
来源：http://zjj.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://hiy.nwbrower.top

[Q55] 排名（并列占位）
来源：http://qzx.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ayd.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://sry.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fsz.redwolf501.top

[Q57] 行号
来源：http://dps.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xvn.fzhhl.top

[Q58] 累计求和
来源：http://ucl.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qyb.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://rfz.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fus.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://asu.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sjc.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kng.snrcjt.cn

[Q61] 移动平均
来源：http://lav.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aas.zhoulong.xyz

[Q62] 分组占比
来源：http://zfj.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oez.hfpthk.cn

[Q63] 开启事务
来源：http://mlh.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mct.bjfxy.top

[Q64] 提交事务
来源：http://tow.jinghuilouyu.cn

COMMIT;
来源：http://woy.birdmap.top

[Q65] 回滚事务
来源：http://ywr.dashuyun.cn

ROLLBACK;
来源：http://nlj.52xcode.cn

[Q66] 行锁查询
来源：http://jso.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iel.aizwys.cn

[Q67] 设置隔离级别
来源：http://uju.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tle.0kj1m.cn

[Q68] 保存点
来源：http://ddq.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://wsk.redwolf501.top

ROLLBACK TO sp1;
来源：http://mlj.sweek.top

[Q69] 查看执行计划
来源：http://jrc.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hal.tanke756.top

[Q70] 更新统计信息
来源：http://kzs.uphjek.com

ANALYZE TABLE users;
来源：http://cuy.dianchejie.cn

[Q71] 查看建表语句
来源：http://xvr.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hyt.fengsongda.top

[Q72] 查看索引
来源：http://pxy.yuanzhike.top

SHOW INDEX FROM users;
来源：http://ffa.bjfxy.top

[Q73] 查看表状态
来源：http://mtn.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wka.fzhhl.top

[Q74] 强制使用索引
来源：http://oti.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://roh.kuanghao11.cn

[Q75] 日期格式化
来源：http://zef.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mgj.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qmb.sxryk.cn

[Q76] 按天统计
来源：http://tpi.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dqv.birdmap.top

[Q77] 时间加减
来源：http://mwx.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xst.hcnkem.com

[Q78] 当前时间
来源：http://kby.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mvg.ybcxt.top

[Q79] 字符串拼接
来源：http://tpb.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vjm.hongshengwenyu.top

[Q80] 字符串截取
来源：http://imj.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yej.cucudq.cn

[Q81] 字符串替换
来源：http://mfq.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wxz.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://jfp.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gco.zdbjq.cn

[Q83] 大小写转换
来源：http://suf.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://alv.birdmap.top

[Q84] 去除首尾空格
来源：http://mky.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://wvi.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://wgd.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oox.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://hzf.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ygm.gzhubu.top

[Q87] JSON 字段做条件
来源：http://ncr.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zkr.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://cqo.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://whm.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zpm.xylfe.cn

[Q89] 判断表是否存在
来源：http://oov.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oth.yangfankeji.com

[Q90] 生成序号列
来源：http://bbg.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uuy.zhengqikj.top

================================================================================
来源：http://mnm.jqgfzy.top

R. Bash 专题
来源：http://zdr.ctjpmb.com

================================================================================
来源：http://ivs.dashuyun.cn

[R01] shebang 与严格模式
来源：http://rxg.guowangkeji.top

#!/usr/bin/env bash
来源：http://lvi.andypj.xyz

set -euo pipefail
来源：http://mvp.yongpay.top

[R02] 变量赋值与使用
来源：http://wns.nanxinkj.top

name="Tom"; echo "$name"
来源：http://ywq.gogol.net.cn

[R03] 只读变量
来源：http://waa.yuxming.cn

readonly PI=3.14
来源：http://pea.fengsongda.top

[R04] 位置参数
来源：http://mpr.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cmh.cqqwz.cn

[R05] 参数默认值
来源：http://arx.jianghu66.top

name="${1:-default}"
来源：http://zzw.fengsongda.top

[R06] 判断命令是否存在
来源：http://orw.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ccn.iojbl.cn

[R07] if 判断文件
来源：http://ynn.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ggk.bjfxy.top

[R08] 数值比较
来源：http://yco.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://unk.hnqzz.top

[R09] 字符串比较
来源：http://jpn.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://asq.ctjpmb.com

[R10] 正则匹配
来源：http://dzc.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fcn.zhaomingkeji.xyz

[R11] case 多分支
来源：http://aoz.xziqi.cn

case "$1" in
来源：http://jmp.zycfv.cn

start) echo "启动" ;;
来源：http://auc.ppjwa.cn

stop)  echo "停止" ;;
来源：http://ovn.wangdashe.top

*)     echo "未知命令" ;;
来源：http://plh.yangfankeji.com

esac
来源：http://bwd.yvedp.cn

[R12] for 遍历文件
来源：http://jee.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://mmm.birdmap.top

[R13] for 计数循环
来源：http://fbo.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://isr.cheryme.top

[R14] C 风格 for
来源：http://bsj.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qon.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://pwg.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://emo.birdmap.top

[R16] until 等待条件
来源：http://yed.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tye.cdnleiting.top

[R17] 数组定义与取值
来源：http://flc.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://ggs.fehbvm.com

[R18] 遍历数组
来源：http://gxr.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hym.kuanghao11.cn

[R19] 数组长度
来源：http://hjl.sufxvd.cn

echo "${#arr[@]}"
来源：http://mvd.gogol.net.cn

[R20] 关联数组（字典）
来源：http://axd.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bhh.chenjidiqi.icu

[R21] 字符串长度
来源：http://xbe.aizwys.cn

echo "${#s}"
来源：http://mtd.xinyue.icu

[R22] 截取子串
来源：http://lyf.aibaodan.cn

echo "${s:0:5}"
来源：http://tcv.zhengqikj.top

[R23] 字符串替换
来源：http://zfl.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://csg.smart0.xyz

[R24] 大小写转换
来源：http://rka.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://oug.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://gco.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqe.dashuyun.cn

[R26] 命令替换
来源：http://xug.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://hdx.smart0.xyz

[R27] 算术展开
来源：http://jmp.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://hxc.daxiang520.top

[R28] 浮点运算
来源：http://dlp.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://fgy.ywan-chungtsiang.top

[R29] 定义函数
来源：http://pct.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vbb.dashuyun.cn

[R30] 函数返回状态码
来源：http://dvu.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://wsn.fanxiaobao.xyz

[R31] 局部变量
来源：http://urb.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://irg.shzxlz.cn

[R32] 参数个数校验
来源：http://vck.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hrk.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://luy.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uqm.sweek.top

[R34] 退出时清理
来源：http://uip.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://elw.fengsongda.top

[R35] 后台执行并等待
来源：http://jfp.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://lhm.zdbjq.cn

[R36] 并发执行多个任务
来源：http://ngw.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wgn.ppjwa.cn

[R37] 把输出赋给变量
来源：http://zdg.sjlbkw.cn

files=$(ls -1)
来源：http://tbz.xinyue.icu

[R38] 管道串联
来源：http://igb.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://kqj.pycfn.com

[R39] 重定向标准输出与错误
来源：http://syr.vqdsnc.cn

cmd > out.log 2>&1
来源：http://hdv.smart0.xyz

[R40] 追加写日志
来源：http://kqa.hesvh.cn

echo "log" >> out.log
来源：http://hjp.zhongyouzk.top

[R41] 丢弃输出
来源：http://wqp.andypj.xyz

cmd >/dev/null 2>&1
来源：http://csz.yj20258.top

[R42] 输入重定向
来源：http://cvn.ppjwa.cn

wc -l < a.txt
来源：http://kpe.tanke756.top

[R43] 按名字查找文件
来源：http://dsd.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://ivs.gzhubu.top

[R44] 按修改时间查找
来源：http://gbf.yj20258.top

find . -mtime -7 -type f
来源：http://xia.tian-w.cn

[R45] 批量删除
来源：http://cht.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://wdw.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://jfp.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nkl.yfazqb.com

[R47] sed 单行替换
来源：http://jea.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://mig.zhengqikj.top

[R48] awk 取指定列
来源：http://dpi.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://iqc.wangdashe.top

[R49] awk 带条件
来源：http://dpu.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kes.xylfe.cn

[R50] awk 求和
来源：http://wke.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://ckd.havefunace.top

[R51] 排序去重取前几
来源：http://ikx.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fyt.aibaodan.cn

[R52] 统计行数
来源：http://frs.nanxuanxn.top

wc -l a.txt
来源：http://zvc.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://eqz.dianchejie.cn


<!-- 参考信息 -->