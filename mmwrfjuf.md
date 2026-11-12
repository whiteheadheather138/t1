代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rsv.iojbl.cn

);
来源：http://yye.fengsongda.top

[Q02] 创建带外键的表
来源：http://wmi.sjlbkw.cn

CREATE TABLE orders (
来源：http://dfv.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gkj.chenlongwang.top

user_id INT NOT NULL,
来源：http://tox.fehbvm.com

amount DECIMAL(10, 2),
来源：http://rft.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://thv.yueranfly.top

);
来源：http://cxr.nwbrower.top

[Q03] 增加列
来源：http://fdv.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://czc.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://dyv.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxy.chenjidiqi.icu

[Q05] 重命名列
来源：http://vwf.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bmu.jqgfzy.top

[Q06] 删除列
来源：http://buu.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://vif.daxiang520.top

[Q07] 删除表
来源：http://nst.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://hly.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://rzn.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://xeg.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://cho.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://var.guowangkeji.top

[Q10] 插入单行
来源：http://gsf.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ohf.tanke756.top

[Q11] 一次插入多行
来源：http://hin.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rna.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://wnh.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://goq.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dkd.c1oappe.top

[Q13] 忽略重复插入
来源：http://jbp.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zji.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://dan.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dvl.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ers.fanxiaobao.xyz

[Q15] 查询全部
来源：http://tar.snrcjt.cn

SELECT * FROM users;
来源：http://nin.jinqigfzy.top

[Q16] 查询指定列
来源：http://jvk.tian-w.cn

SELECT id, name FROM users;
来源：http://egu.jlsjyb.cn

[Q17] 条件查询
来源：http://dga.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nbb.tarul.cn

[Q18] 模糊匹配
来源：http://amf.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zdv.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://gxw.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epy.xziqi.cn

[Q20] IN 列表
来源：http://odw.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dhg.yonumen.top

[Q21] 空值判断
来源：http://yix.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zon.meibo888.top

[Q22] 排序
来源：http://ixy.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cws.sufxvd.cn

[Q23] 分页
来源：http://akl.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pnh.sjlbkw.cn

[Q24] 去重
来源：http://vcm.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://oxv.ivvv.top

[Q25] 只取前 N 条
来源：http://nau.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oli.andypj.xyz

[Q26] 计数
来源：http://vow.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://ctq.pengpengdd.cyou

[Q27] 条件计数
来源：http://moq.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://heh.tian-w.cn

[Q28] 求和与平均
来源：http://esy.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://exs.svipenyu.cn

[Q29] 最大最小值
来源：http://yon.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ttd.xinyue.icu

[Q30] 分组统计
来源：http://xxo.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tef.cdnleiting.top

[Q31] 分组后过滤
来源：http://yuc.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uyr.yueranfly.top

[Q32] 分组拼接字符串
来源：http://gjo.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iqu.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xje.yj20258888.top

[Q33] 多列分组
来源：http://jjy.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ffp.zdqjudy.top

[Q34] 每组取第一条
来源：http://ecp.havefunace.top

SELECT * FROM (
来源：http://scz.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://whk.hfpthk.cn

) t WHERE rn = 1;
来源：http://wxz.jlsjyb.cn

[Q35] 内连接
来源：http://drx.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gmk.chenzaomai.com

[Q36] 左连接
来源：http://sqh.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xck.shanyushiyangtech.top

[Q37] 右连接
来源：http://xii.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ccb.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://wuc.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://whh.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://veh.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ryt.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejc.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kut.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nup.ehwqpu.com

[Q41] 多表连接
来源：http://oaj.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vra.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://lbh.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://qly.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://efg.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://dgp.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sxb.yueranfly.top

[Q43] 标量子查询
来源：http://zdi.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ilq.wangshuangyany.cn

[Q44] IN 子查询
来源：http://ngw.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qtp.birdmap.top

[Q45] EXISTS 判断存在
来源：http://ijf.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nor.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dvv.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lye.snrcjt.cn

[Q47] 与平均值比较
来源：http://lya.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iji.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://htx.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qps.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://vjp.shuidangran.top

[Q49] 更新单行
来源：http://wyi.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bxe.cqqwz.cn

[Q50] 批量更新
来源：http://moe.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uss.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://suh.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yam.guowangkeji.top

[Q52] 删除指定行
来源：http://tgc.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://oon.fktsv.cn

[Q53] 按条件删除
来源：http://dsr.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hum.jlsjyb.cn

[Q54] 清空表
来源：http://keb.sysykeji.top

TRUNCATE TABLE logs;
来源：http://qps.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://qhh.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fao.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://nrt.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nut.chenjidiqi.icu

[Q57] 行号
来源：http://lhk.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wkb.pengpengdd.cyou

[Q58] 累计求和
来源：http://oei.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpk.fengsongda.top

[Q59] 分组内累计
来源：http://raa.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://anq.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://puh.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hhc.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mev.gotoacloud.top

[Q61] 移动平均
来源：http://rsb.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://igr.52xcode.cn

[Q62] 分组占比
来源：http://uib.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://apq.cheryme.top

[Q63] 开启事务
来源：http://wkq.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://clh.xuetiantiany.cn

[Q64] 提交事务
来源：http://mtl.shzxlz.cn

COMMIT;
来源：http://dqb.zhiwuduotai.top

[Q65] 回滚事务
来源：http://vmm.jlsjyb.cn

ROLLBACK;
来源：http://kkr.daxiang520.top

[Q66] 行锁查询
来源：http://jss.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hqd.ivvv.top

[Q67] 设置隔离级别
来源：http://lne.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gog.tarul.cn

[Q68] 保存点
来源：http://ztr.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://eks.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://gqd.yuanzhike.top

[Q69] 查看执行计划
来源：http://zhc.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rdm.xuanzx.com

[Q70] 更新统计信息
来源：http://nke.hammf.cn

ANALYZE TABLE users;
来源：http://ubo.hnqzz.top

[Q71] 查看建表语句
来源：http://njb.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ysh.yonumen.top

[Q72] 查看索引
来源：http://vnr.yueranfly.top

SHOW INDEX FROM users;
来源：http://dxa.hcnkem.com

[Q73] 查看表状态
来源：http://xbi.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fgo.jianghu66.top

[Q74] 强制使用索引
来源：http://zdl.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wpr.yfazqb.com

[Q75] 日期格式化
来源：http://jvc.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sbw.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uvs.xylfe.cn

[Q76] 按天统计
来源：http://lzs.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lnv.hnxiangtu.top

[Q77] 时间加减
来源：http://ggg.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iaa.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://igc.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://caj.vqdsnc.cn

[Q79] 字符串拼接
来源：http://fpx.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cyf.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://hms.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zrd.chenzaomai.com

[Q81] 字符串替换
来源：http://vnv.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xeb.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://clm.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tjk.sufxvd.cn

[Q83] 大小写转换
来源：http://gus.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lpk.cqqwz.cn

[Q84] 去除首尾空格
来源：http://uzi.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://rkk.zycfv.cn

[Q85] 数值取整
来源：http://xnc.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pma.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://dhf.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qun.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://skp.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://leh.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://nts.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://itq.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://una.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://rrv.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ogs.jinqigfzy.top

[Q90] 生成序号列
来源：http://prr.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gfu.yuxming.cn

================================================================================
来源：http://qun.jqgfzy.top

R. Bash 专题
来源：http://kht.havefunace.top

================================================================================
来源：http://byh.uphjek.com

[R01] shebang 与严格模式
来源：http://uty.9152youxi.cn

#!/usr/bin/env bash
来源：http://vyf.havefunace.top

set -euo pipefail
来源：http://zir.gogol.net.cn

[R02] 变量赋值与使用
来源：http://uye.gogol.net.cn

name="Tom"; echo "$name"
来源：http://mre.haohaochexian.top

[R03] 只读变量
来源：http://xud.jqgufenzy.top

readonly PI=3.14
来源：http://qdu.hammf.cn

[R04] 位置参数
来源：http://mss.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cqm.tanke756.top

[R05] 参数默认值
来源：http://zwf.chenjidiqi.icu

name="${1:-default}"
来源：http://hrz.yj20258.top

[R06] 判断命令是否存在
来源：http://hzj.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cge.hcnkem.com

[R07] if 判断文件
来源：http://mhi.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bpe.bbcook.cn

[R08] 数值比较
来源：http://ptk.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jpw.cqqwz.cn

[R09] 字符串比较
来源：http://kck.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://amx.shzxlz.cn

[R10] 正则匹配
来源：http://bhz.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gdr.yfazqb.com

[R11] case 多分支
来源：http://ysn.nanxinkj.top

case "$1" in
来源：http://cfy.quarkkingdee.top

start) echo "启动" ;;
来源：http://epp.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://xlk.tian-w.cn

*)     echo "未知命令" ;;
来源：http://wwv.zhaomingkeji.xyz

esac
来源：http://nyl.aizwys.cn

[R12] for 遍历文件
来源：http://gnm.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://uwq.ivvv.top

[R13] for 计数循环
来源：http://erj.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://oso.tarul.cn

[R14] C 风格 for
来源：http://pdr.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zdq.yonumen.top

[R15] while 逐行读文件
来源：http://bzd.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://agy.hywenlv.cn

[R16] until 等待条件
来源：http://can.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gpp.gotoacloud.top

[R17] 数组定义与取值
来源：http://cuo.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ffe.wangdashe.top

[R18] 遍历数组
来源：http://kpd.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jxb.smart0.xyz

[R19] 数组长度
来源：http://hhr.fengsongda.top

echo "${#arr[@]}"
来源：http://dgj.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://thq.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ioc.chenlongwang.top

[R21] 字符串长度
来源：http://dsy.chenzaomai.com

echo "${#s}"
来源：http://qaj.ydzc1.top

[R22] 截取子串
来源：http://eka.sysykeji.top

echo "${s:0:5}"
来源：http://unk.yongpay.top

[R23] 字符串替换
来源：http://pdl.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dla.wangdashe.top

[R24] 大小写转换
来源：http://jnp.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://vnz.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://xcu.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://iqj.ppjwa.cn

[R26] 命令替换
来源：http://hqw.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://ugz.aibaodan.cn

[R27] 算术展开
来源：http://nqn.cheryme.top

echo $((1 + 2 * 3))
来源：http://nwi.daria6918.cn

[R28] 浮点运算
来源：http://sjk.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://sca.quarkkingdee.top

[R29] 定义函数
来源：http://gcw.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ttd.kuanghao11.cn

[R30] 函数返回状态码
来源：http://kai.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://iap.havefunace.top

[R31] 局部变量
来源：http://oqo.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://lqg.hfpthk.cn

[R32] 参数个数校验
来源：http://pns.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hwa.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://aom.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ind.aibaodan.cn

[R34] 退出时清理
来源：http://sfn.bjfxy.top

trap 'rm -f "$tmp"' EXIT
来源：http://wiq.chenlongwang.top

[R35] 后台执行并等待
来源：http://vxw.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://koz.tian-w.cn

[R36] 并发执行多个任务
来源：http://efc.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hvo.sysykeji.top

[R37] 把输出赋给变量
来源：http://bya.nanxinkj.top

files=$(ls -1)
来源：http://qee.birdmap.top

[R38] 管道串联
来源：http://xyr.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://pzg.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://mbs.ivvv.top

cmd > out.log 2>&1
来源：http://zul.daria6918.cn

[R40] 追加写日志
来源：http://lld.fktsv.cn

echo "log" >> out.log
来源：http://qjb.havefunace.top

[R41] 丢弃输出
来源：http://voz.sysykeji.top

cmd >/dev/null 2>&1
来源：http://vmo.hnxiangtu.top

[R42] 输入重定向
来源：http://axi.pycfn.com

wc -l < a.txt
来源：http://bae.zhongyouzk.top

[R43] 按名字查找文件
来源：http://dvt.yj20258888.top

find . -name "*.log" -type f
来源：http://wgk.vehdjk.com

[R44] 按修改时间查找
来源：http://obe.havefunace.top

find . -mtime -7 -type f
来源：http://lns.jinyuanbaomall.cn

[R45] 批量删除
来源：http://llt.cucudq.cn

find . -name "*.tmp" -delete
来源：http://stv.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://fqo.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbl.tianlin.xyz

[R47] sed 单行替换
来源：http://sgs.yj202588.top


<!-- 参考信息 -->