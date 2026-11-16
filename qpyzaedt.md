代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://ffi.bbcook.cn

[Q07] 删除表
来源：http://ucx.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://tlj.bjfxy.top

[Q08] 创建普通索引
来源：http://mgs.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://izn.chenzaomai.com

[Q09] 创建唯一索引
来源：http://ylh.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qzi.316326.xyz

[Q10] 插入单行
来源：http://itn.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uen.guannengcc.top

[Q11] 一次插入多行
来源：http://dad.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kib.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://ndz.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://biy.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kak.gotoacloud.top

[Q13] 忽略重复插入
来源：http://hfd.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ncf.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://xdv.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rha.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hel.yj20258888.top

[Q15] 查询全部
来源：http://zng.zhoulong.xyz

SELECT * FROM users;
来源：http://jjo.shzxlz.cn

[Q16] 查询指定列
来源：http://kcq.tarul.cn

SELECT id, name FROM users;
来源：http://rlx.pengpengdd.cyou

[Q17] 条件查询
来源：http://hba.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iuw.mhx1999.top

[Q18] 模糊匹配
来源：http://kjb.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://thf.xuanzx.com

[Q19] 范围查询
来源：http://iex.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fqa.mhx1999.top

[Q20] IN 列表
来源：http://apz.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eca.uphjek.com

[Q21] 空值判断
来源：http://jxm.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://flk.yangfankeji.com

[Q22] 排序
来源：http://wqb.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zum.andypj.xyz

[Q23] 分页
来源：http://pwf.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hni.hnqzz.top

[Q24] 去重
来源：http://mnt.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://qrq.ivvv.top

[Q25] 只取前 N 条
来源：http://nbp.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zvp.jianghu66.top

[Q26] 计数
来源：http://dkf.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://xhv.jyoumei.cn

[Q27] 条件计数
来源：http://exb.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ngf.zhoulong.xyz

[Q28] 求和与平均
来源：http://ejd.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cpr.gotoacloud.top

[Q29] 最大最小值
来源：http://kzx.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gqa.cqqwz.cn

[Q30] 分组统计
来源：http://odv.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://slb.chenzaomai.com

[Q31] 分组后过滤
来源：http://spm.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qkx.zycfv.cn

[Q32] 分组拼接字符串
来源：http://mgv.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vxs.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ixt.fanxiaobao.xyz

[Q33] 多列分组
来源：http://tyg.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bpe.cdnleiting.top

[Q34] 每组取第一条
来源：http://rws.hesvh.cn

SELECT * FROM (
来源：http://joh.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gfl.andypj.xyz

) t WHERE rn = 1;
来源：http://yro.andypj.xyz

[Q35] 内连接
来源：http://ysl.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xac.yuanzhike.top

[Q36] 左连接
来源：http://afg.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wbh.jiagoushi.top

[Q37] 右连接
来源：http://hid.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hnj.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://ynb.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ged.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://gjk.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://zkp.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sfn.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://byo.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://izz.yangfankeji.com

[Q41] 多表连接
来源：http://ecx.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bmv.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://juf.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://sfd.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://mdv.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://icf.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rwo.yuanzhike.top

[Q43] 标量子查询
来源：http://yxv.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hzb.andypj.xyz

[Q44] IN 子查询
来源：http://ypi.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://owc.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://pkd.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gom.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://uvt.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvg.c1oappe.top

[Q47] 与平均值比较
来源：http://qtx.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wvb.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://hyr.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jum.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://pwz.tian-w.cn

[Q49] 更新单行
来源：http://ufw.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://idi.cdnleiting.top

[Q50] 批量更新
来源：http://umn.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lxo.redwolf501.top

[Q51] 用子查询更新
来源：http://mhg.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://muh.tian-w.cn

[Q52] 删除指定行
来源：http://bco.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://kkm.jqgfzy.top

[Q53] 按条件删除
来源：http://owr.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ixy.chenlongwang.top

[Q54] 清空表
来源：http://bjk.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://gho.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://gso.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qir.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://fte.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tco.chenjidiqi.icu

[Q57] 行号
来源：http://vkp.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://epi.hesvh.cn

[Q58] 累计求和
来源：http://lgm.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nvt.gogol.net.cn

[Q59] 分组内累计
来源：http://ifz.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vhd.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://tav.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fdl.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvx.ybcxt.top

[Q61] 移动平均
来源：http://nap.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vse.zhijiandao.cn

[Q62] 分组占比
来源：http://wem.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tpt.guannengcc.top

[Q63] 开启事务
来源：http://qwg.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nbx.bjfxy.top

[Q64] 提交事务
来源：http://lby.jinghuilouyu.cn

COMMIT;
来源：http://snl.yj20258888.top

[Q65] 回滚事务
来源：http://bvo.xylfe.cn

ROLLBACK;
来源：http://sub.vehdjk.com

[Q66] 行锁查询
来源：http://zas.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ibu.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://gcv.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nel.yvedp.cn

[Q68] 保存点
来源：http://tbk.nanxuanxn.top

SAVEPOINT sp1;
来源：http://thc.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://ier.52xcode.cn

[Q69] 查看执行计划
来源：http://jfv.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wqa.jianghu66.top

[Q70] 更新统计信息
来源：http://dgc.ybcxt.top

ANALYZE TABLE users;
来源：http://bxw.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://rco.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://omo.gzhubu.top

[Q72] 查看索引
来源：http://rhg.jianghu66.top

SHOW INDEX FROM users;
来源：http://nlq.chenjidiqi.icu

[Q73] 查看表状态
来源：http://fxw.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jiw.havefunace.top

[Q74] 强制使用索引
来源：http://mky.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvc.jinqigufen.top

[Q75] 日期格式化
来源：http://dud.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fww.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gwe.fanxiaobao.xyz

[Q76] 按天统计
来源：http://dzy.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lww.52xcode.cn

[Q77] 时间加减
来源：http://qdg.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mna.tanke756.top

[Q78] 当前时间
来源：http://dgd.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skf.yangfankeji.com

[Q79] 字符串拼接
来源：http://kla.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rma.redwolf501.top

[Q80] 字符串截取
来源：http://gqk.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iap.nwbrower.top

[Q81] 字符串替换
来源：http://epn.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yzn.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://ejw.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jes.hnxiangtu.top

[Q83] 大小写转换
来源：http://hqa.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hfq.hfpthk.cn

[Q84] 去除首尾空格
来源：http://rbl.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://itf.zhiwuduotai.top

[Q85] 数值取整
来源：http://dpg.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gvl.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://zpv.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uzy.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://fco.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://msz.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://nvm.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jta.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sne.316326.xyz

[Q89] 判断表是否存在
来源：http://ljz.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://byc.jlsjyb.cn

[Q90] 生成序号列
来源：http://zbl.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://esl.yueranfly.top

================================================================================
来源：http://wxx.shanyushiyangtech.top

R. Bash 专题
来源：http://iai.mhx1999.top

================================================================================
来源：http://hgi.cqqwz.cn

[R01] shebang 与严格模式
来源：http://ozb.aibaodan.cn

#!/usr/bin/env bash
来源：http://qms.sufxvd.cn

set -euo pipefail
来源：http://tiq.iojbl.cn

[R02] 变量赋值与使用
来源：http://qbr.aizwys.cn

name="Tom"; echo "$name"
来源：http://uyx.ydjk.org.cn

[R03] 只读变量
来源：http://xoj.sjlbkw.cn

readonly PI=3.14
来源：http://udg.cqqwz.cn

[R04] 位置参数
来源：http://cnc.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gch.hcnkem.com

[R05] 参数默认值
来源：http://uzv.shanyushiyangtech.top

name="${1:-default}"
来源：http://sly.ppjwa.cn

[R06] 判断命令是否存在
来源：http://dil.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zhk.aibaodan.cn

[R07] if 判断文件
来源：http://ogd.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tad.dianchejie.cn

[R08] 数值比较
来源：http://dvl.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://pdo.cucudq.cn

[R09] 字符串比较
来源：http://ajy.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bcx.havefunace.top

[R10] 正则匹配
来源：http://ilw.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://frz.tian-w.cn

[R11] case 多分支
来源：http://ssx.aizwys.cn

case "$1" in
来源：http://bso.iojbl.cn

start) echo "启动" ;;
来源：http://uuj.sweek.top

stop)  echo "停止" ;;
来源：http://vuj.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://hth.yuxming.cn

esac
来源：http://xwc.ppjwa.cn

[R12] for 遍历文件
来源：http://bzg.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://srz.nanxinkj.top

[R13] for 计数循环
来源：http://uue.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://ced.zhiwuduotai.top

[R14] C 风格 for
来源：http://mmi.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ihd.jlsjyb.cn

[R15] while 逐行读文件
来源：http://onf.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ogy.guannengcc.top

[R16] until 等待条件
来源：http://taw.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lgl.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://ztx.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uwo.guowangkeji.top

[R18] 遍历数组
来源：http://tzv.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cgf.hysaishi.cn

[R19] 数组长度
来源：http://nkp.daxiang520.top

echo "${#arr[@]}"
来源：http://nnq.hnqzz.top

[R20] 关联数组（字典）
来源：http://phr.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rme.dianchejie.cn

[R21] 字符串长度
来源：http://vvv.hcnkem.com

echo "${#s}"
来源：http://yqu.snrcjt.cn

[R22] 截取子串
来源：http://rbw.birdmap.top

echo "${s:0:5}"
来源：http://pdt.gotoacloud.top

[R23] 字符串替换
来源：http://bcb.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wal.jlsjyb.cn

[R24] 大小写转换
来源：http://qwp.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://qeh.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://txw.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kyg.daria6918.cn

[R26] 命令替换
来源：http://yij.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://uvr.iojbl.cn

[R27] 算术展开
来源：http://vxr.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://szu.fktsv.cn

[R28] 浮点运算
来源：http://yup.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://cel.wangdashe.top

[R29] 定义函数
来源：http://nmj.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qcy.gogol.net.cn

[R30] 函数返回状态码
来源：http://oxo.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://wll.xuetiantiany.cn

[R31] 局部变量
来源：http://snh.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://pal.yueranfly.top

[R32] 参数个数校验
来源：http://taj.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gyu.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://hxb.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fcl.ydjk.org.cn

[R34] 退出时清理
来源：http://jap.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://zkp.quarkkingdee.top

[R35] 后台执行并等待
来源：http://omb.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dbo.jinqigufen.top

[R36] 并发执行多个任务
来源：http://oxk.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://onn.jianghu66.top

[R37] 把输出赋给变量
来源：http://ndj.jianghu66.top

files=$(ls -1)
来源：http://kls.jinqigfzy.top

[R38] 管道串联
来源：http://ecu.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://wro.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://kqw.daxiang520.top

cmd > out.log 2>&1
来源：http://uhx.52xcode.cn

[R40] 追加写日志
来源：http://wwz.ivvv.top

echo "log" >> out.log
来源：http://wxo.yongpay.top

[R41] 丢弃输出
来源：http://jnw.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://xzw.zdbjq.cn

[R42] 输入重定向
来源：http://jvw.0kj1m.cn

wc -l < a.txt
来源：http://iox.sufxvd.cn

[R43] 按名字查找文件
来源：http://unh.yvedp.cn

find . -name "*.log" -type f
来源：http://jmp.ehwqpu.com

[R44] 按修改时间查找
来源：http://siu.smart0.xyz

find . -mtime -7 -type f
来源：http://off.gotoacloud.top

[R45] 批量删除
来源：http://hdj.uphjek.com

find . -name "*.tmp" -delete
来源：http://bio.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://lch.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lgh.shangyingyoupin.top

[R47] sed 单行替换
来源：http://uim.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://asc.havefunace.top

[R48] awk 取指定列
来源：http://ytq.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://zjg.tian-w.cn

[R49] awk 带条件
来源：http://sro.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yie.jiagoushi.top

[R50] awk 求和
来源：http://bpz.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://svf.zdqjudy.top

[R51] 排序去重取前几
来源：http://vct.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yuj.chenlongwang.top

[R52] 统计行数
来源：http://mjf.yueranfly.top

wc -l a.txt
来源：http://jpj.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://olc.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://psx.yuanzhike.top

[R54] 比较两个文件
来源：http://xwt.dianchejie.cn

diff a.txt b.txt
来源：http://aqy.wangdashe.top

[R55] 压缩与解压
来源：http://ibk.yangfankeji.com


<!-- 参考信息 -->