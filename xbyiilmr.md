代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pnz.ydzc1.top

);
来源：http://scf.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://eys.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://dow.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nsz.ehwqpu.com

user_id INT NOT NULL,
来源：http://snj.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://jsz.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bwh.ehwqpu.com

);
来源：http://evz.bjfxy.top

[Q03] 增加列
来源：http://jel.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eut.gzhubu.top

[Q04] 修改列类型
来源：http://awy.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oca.xinyue.icu

[Q05] 重命名列
来源：http://jus.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nbm.zdqjudy.top

[Q06] 删除列
来源：http://mkt.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rqc.pycfn.com

[Q07] 删除表
来源：http://ahk.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://jkm.shzxlz.cn

[Q08] 创建普通索引
来源：http://sjo.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://twa.daria6918.cn

[Q09] 创建唯一索引
来源：http://uxv.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ypn.316326.xyz

[Q10] 插入单行
来源：http://jpv.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jhs.vehdjk.com

[Q11] 一次插入多行
来源：http://bkm.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gyy.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://sob.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iuf.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://owo.yj202588.top

[Q13] 忽略重复插入
来源：http://ztt.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://owh.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://aol.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dgv.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qym.hammf.cn

[Q15] 查询全部
来源：http://yua.chenjidiqi.icu

SELECT * FROM users;
来源：http://qka.nanxuanxn.top

[Q16] 查询指定列
来源：http://jqe.jiagoushi.top

SELECT id, name FROM users;
来源：http://ffa.yj20258888.top

[Q17] 条件查询
来源：http://euq.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pau.zdqjudy.top

[Q18] 模糊匹配
来源：http://til.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://egl.pycfn.com

[Q19] 范围查询
来源：http://jof.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oov.zhijiandao.cn

[Q20] IN 列表
来源：http://xru.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://osc.svipenyu.cn

[Q21] 空值判断
来源：http://fwr.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ysw.yfazqb.com

[Q22] 排序
来源：http://muh.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tef.yj202588.top

[Q23] 分页
来源：http://dwf.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uze.zhixingplan.top

[Q24] 去重
来源：http://kar.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://fkb.gotoacloud.top

[Q25] 只取前 N 条
来源：http://kfk.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://plk.gogol.net.cn

[Q26] 计数
来源：http://uut.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://wcg.gzhubu.top

[Q27] 条件计数
来源：http://pyi.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vpn.ehwqpu.com

[Q28] 求和与平均
来源：http://nex.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://seq.yvedp.cn

[Q29] 最大最小值
来源：http://sya.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://txg.uphjek.com

[Q30] 分组统计
来源：http://qtc.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omq.uphjek.com

[Q31] 分组后过滤
来源：http://jji.snrcjt.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vyo.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://wzk.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pum.vehdjk.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lxa.haohaochexian.top

[Q33] 多列分组
来源：http://uop.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ucq.kuanghao11.cn

[Q34] 每组取第一条
来源：http://mos.yueranfly.top

SELECT * FROM (
来源：http://zey.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovv.havefunace.top

) t WHERE rn = 1;
来源：http://aai.quarkkingdee.top

[Q35] 内连接
来源：http://bpo.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyd.yongpay.top

[Q36] 左连接
来源：http://uls.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qoi.redwolf501.top

[Q37] 右连接
来源：http://mtu.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://njo.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://dzq.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ynx.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://gsu.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dfq.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fpf.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ewv.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zyn.bbcook.cn

[Q41] 多表连接
来源：http://kbn.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lap.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://mcf.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://qqy.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://bas.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://ihn.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fvd.yj20258888.top

[Q43] 标量子查询
来源：http://eyk.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://suy.vehdjk.com

[Q44] IN 子查询
来源：http://gvv.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hjd.yj20258.top

[Q45] EXISTS 判断存在
来源：http://obn.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yub.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dus.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pyz.sjlbkw.cn

[Q47] 与平均值比较
来源：http://ppo.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tcj.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://yxz.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zbg.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://ype.ivvv.top

[Q49] 更新单行
来源：http://exj.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oyt.fzhhl.top

[Q50] 批量更新
来源：http://ynf.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ozm.sweek.top

[Q51] 用子查询更新
来源：http://rus.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vpn.yj20258888.top

[Q52] 删除指定行
来源：http://nze.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://mqs.yueranfly.top

[Q53] 按条件删除
来源：http://gvq.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dex.shzxlz.cn

[Q54] 清空表
来源：http://hib.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://bzy.hcnkem.com

[Q55] 排名（并列占位）
来源：http://jqp.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwp.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://ksn.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tbd.uphjek.com

[Q57] 行号
来源：http://fbe.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://psi.haohaochexian.top

[Q58] 累计求和
来源：http://mfw.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pja.ehwqpu.com

[Q59] 分组内累计
来源：http://nik.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vlb.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://pjv.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sua.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wlt.hysaishi.cn

[Q61] 移动平均
来源：http://mth.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vab.c1oappe.top

[Q62] 分组占比
来源：http://kzl.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zdf.guowangkeji.top

[Q63] 开启事务
来源：http://apg.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pzf.iojbl.cn

[Q64] 提交事务
来源：http://lje.xylfe.cn

COMMIT;
来源：http://oun.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://mmq.shangyingyoupin.top

ROLLBACK;
来源：http://vbj.vqdsnc.cn

[Q66] 行锁查询
来源：http://zoy.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://axn.bjfxy.top

[Q67] 设置隔离级别
来源：http://rxw.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jku.xylfe.cn

[Q68] 保存点
来源：http://wbs.tanke756.top

SAVEPOINT sp1;
来源：http://whn.cqqwz.cn

ROLLBACK TO sp1;
来源：http://qjy.zhongyouzk.top

[Q69] 查看执行计划
来源：http://cer.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hjw.bbcook.cn

[Q70] 更新统计信息
来源：http://kzz.xuanzx.com

ANALYZE TABLE users;
来源：http://jkg.redwolf501.top

[Q71] 查看建表语句
来源：http://ywa.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qod.jlsjyb.cn

[Q72] 查看索引
来源：http://rdw.cqqwz.cn

SHOW INDEX FROM users;
来源：http://kvx.cucudq.cn

[Q73] 查看表状态
来源：http://tzi.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kxx.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://vsa.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hdq.hnxiangtu.top

[Q75] 日期格式化
来源：http://fwt.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rpz.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ftn.ctjpmb.com

[Q76] 按天统计
来源：http://lbm.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://whd.ydzc1.top

[Q77] 时间加减
来源：http://ghs.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://icd.meibo888.top

[Q78] 当前时间
来源：http://ehh.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ggo.yueranfly.top

[Q79] 字符串拼接
来源：http://zbj.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tsp.andypj.xyz

[Q80] 字符串截取
来源：http://iiy.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sih.jqgfzy.top

[Q81] 字符串替换
来源：http://fuc.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kdv.yonumen.top

[Q82] 字符长度与字节长度
来源：http://fxx.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qxu.jqgufenzy.top

[Q83] 大小写转换
来源：http://hkf.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://msh.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://uus.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://pih.tarul.cn

[Q85] 数值取整
来源：http://ptu.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uso.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://hgy.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ovf.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://vbd.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uaz.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://aut.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zyc.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ywt.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://nyf.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nih.svipenyu.cn

[Q90] 生成序号列
来源：http://vek.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fja.hesvh.cn

================================================================================
来源：http://pqa.ehwqpu.com

R. Bash 专题
来源：http://pln.yj20258.top

================================================================================
来源：http://cyd.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://zah.meibo888.top

#!/usr/bin/env bash
来源：http://geq.vehdjk.com

set -euo pipefail
来源：http://tor.epnwcf.com

[R02] 变量赋值与使用
来源：http://vva.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://fjk.chenlongwang.top

[R03] 只读变量
来源：http://mzx.ivvv.top

readonly PI=3.14
来源：http://fus.yangfankeji.com

[R04] 位置参数
来源：http://yqh.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fhw.guannengcc.top

[R05] 参数默认值
来源：http://hin.zhijiandao.cn

name="${1:-default}"
来源：http://ltt.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://the.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dge.meibo888.top

[R07] if 判断文件
来源：http://tsq.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ikg.shanyushiyangkeji.top

[R08] 数值比较
来源：http://fcj.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mts.mhx1999.top

[R09] 字符串比较
来源：http://ccv.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sbn.zhixingplan.top

[R10] 正则匹配
来源：http://kbr.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aqx.zdbjq.cn

[R11] case 多分支
来源：http://ldn.mhx1999.top

case "$1" in
来源：http://wsz.jqgufenzy.top

start) echo "启动" ;;
来源：http://wwx.0kj1m.cn

stop)  echo "停止" ;;
来源：http://mpu.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://dpb.nanxuanxn.top

esac
来源：http://sle.cdnleiting.top

[R12] for 遍历文件
来源：http://dal.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://esr.yj202588.top

[R13] for 计数循环
来源：http://egb.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://iii.bjfxy.top

[R14] C 风格 for
来源：http://iql.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jap.fehbvm.com

[R15] while 逐行读文件
来源：http://xho.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://idz.hnxiangtu.top

[R16] until 等待条件
来源：http://apq.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sqi.redwolf501.top

[R17] 数组定义与取值
来源：http://eiq.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nov.zdbjq.cn

[R18] 遍历数组
来源：http://ggr.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lvu.ydzc1.top

[R19] 数组长度
来源：http://sto.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://rpq.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://lfk.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://thl.jiagoushi.top

[R21] 字符串长度
来源：http://inv.hammf.cn

echo "${#s}"
来源：http://rkx.guannengcc.top

[R22] 截取子串
来源：http://ipc.ydjk.org.cn

echo "${s:0:5}"
来源：http://fkv.ydzc1.top

[R23] 字符串替换
来源：http://qhs.shzxlz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ubw.bbcook.cn

[R24] 大小写转换
来源：http://qqb.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cdr.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://uct.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hhw.iojbl.cn

[R26] 命令替换
来源：http://qcp.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://zgy.daxiang520.top

[R27] 算术展开
来源：http://xai.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://xto.haohaochexian.top

[R28] 浮点运算
来源：http://foe.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://ard.tanke756.top

[R29] 定义函数
来源：http://mvm.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://khn.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://tsz.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://zke.sufxvd.cn

[R31] 局部变量
来源：http://rne.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://tic.yonumen.top

[R32] 参数个数校验
来源：http://ned.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ihl.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://kpf.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fhy.ivvv.top

[R34] 退出时清理
来源：http://mcx.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://agj.cucudq.cn

[R35] 后台执行并等待
来源：http://cqp.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nvb.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://jck.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://myv.sxryk.cn

[R37] 把输出赋给变量
来源：http://xwg.zdbjq.cn

files=$(ls -1)
来源：http://opr.smart0.xyz

[R38] 管道串联
来源：http://xqn.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://vgg.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://kii.vqdsnc.cn

cmd > out.log 2>&1
来源：http://lry.ybcxt.top

[R40] 追加写日志
来源：http://yqr.aizwys.cn

echo "log" >> out.log
来源：http://zbh.hysaishi.cn

[R41] 丢弃输出
来源：http://uec.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://xie.zhengqikj.top

[R42] 输入重定向
来源：http://qbh.pycfn.com

wc -l < a.txt
来源：http://psb.shuidangran.top

[R43] 按名字查找文件
来源：http://rmj.yj20258888.top

find . -name "*.log" -type f
来源：http://ssu.hnqzz.top

[R44] 按修改时间查找
来源：http://cnz.jianghu66.top

find . -mtime -7 -type f
来源：http://vxz.hammf.cn

[R45] 批量删除
来源：http://zvg.tarul.cn

find . -name "*.tmp" -delete
来源：http://fdn.jyoumei.cn

[R46] 递归替换文件内容
来源：http://nbx.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wqu.yvedp.cn

[R47] sed 单行替换
来源：http://mov.hammf.cn


<!-- 参考信息 -->