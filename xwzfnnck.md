代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fbi.cashguo.top

);
来源：http://bzf.xinyue.icu

[Q02] 创建带外键的表
来源：http://nkn.tianlin.xyz

CREATE TABLE orders (
来源：http://awt.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyo.gogol.net.cn

user_id INT NOT NULL,
来源：http://rhj.ivvv.top

amount DECIMAL(10, 2),
来源：http://mix.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dqe.aizwys.cn

);
来源：http://ubv.yongpay.top

[Q03] 增加列
来源：http://imp.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://res.ydzc1.top

[Q04] 修改列类型
来源：http://srj.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mbt.hammf.cn

[Q05] 重命名列
来源：http://iwb.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lno.52xcode.cn

[Q06] 删除列
来源：http://qbc.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ayw.chenjidiqi.icu

[Q07] 删除表
来源：http://yeg.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://fcl.xylfe.cn

[Q08] 创建普通索引
来源：http://bnf.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://shd.gogol.net.cn

[Q09] 创建唯一索引
来源：http://wwq.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://krt.xylfe.cn

[Q10] 插入单行
来源：http://bfc.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sds.316326.xyz

[Q11] 一次插入多行
来源：http://ksa.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://heg.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://wjf.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qxn.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://djg.jianghu66.top

[Q13] 忽略重复插入
来源：http://npw.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nxu.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://lve.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uap.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nrf.yanxiufei.cn

[Q15] 查询全部
来源：http://hly.iojbl.cn

SELECT * FROM users;
来源：http://nep.chenzaomai.com

[Q16] 查询指定列
来源：http://thd.chenlongwang.top

SELECT id, name FROM users;
来源：http://hzl.jlsjyb.cn

[Q17] 条件查询
来源：http://kgj.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hfj.meibo888.top

[Q18] 模糊匹配
来源：http://spc.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jgn.nanxinkj.top

[Q19] 范围查询
来源：http://fur.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfn.fanxiaobao.xyz

[Q20] IN 列表
来源：http://app.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://utz.vqdsnc.cn

[Q21] 空值判断
来源：http://zqb.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xwj.yj20258.top

[Q22] 排序
来源：http://eok.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pfr.cqqwz.cn

[Q23] 分页
来源：http://inx.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wyv.gaohongyu789.top

[Q24] 去重
来源：http://tjb.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://dhm.fzhhl.top

[Q25] 只取前 N 条
来源：http://zhs.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oje.hnqzz.top

[Q26] 计数
来源：http://wgd.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://upw.shangyingyoupin.top

[Q27] 条件计数
来源：http://jca.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kja.quarkkingdee.top

[Q28] 求和与平均
来源：http://gpx.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eqz.gotoacloud.top

[Q29] 最大最小值
来源：http://hpp.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aws.52xcode.cn

[Q30] 分组统计
来源：http://ydb.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://syb.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://jxx.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ltv.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://kbx.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ycr.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tom.hnxiangtu.top

[Q33] 多列分组
来源：http://joc.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wwr.aizwys.cn

[Q34] 每组取第一条
来源：http://ygc.wangshuangyany.cn

SELECT * FROM (
来源：http://ljr.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qfa.meibo888.top

) t WHERE rn = 1;
来源：http://hpo.zhixingplan.top

[Q35] 内连接
来源：http://msf.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://knr.quarkkingdee.top

[Q36] 左连接
来源：http://lkc.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ipy.xziqi.cn

[Q37] 右连接
来源：http://ztm.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wqu.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://blb.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rux.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://kmo.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bcv.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qin.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gkv.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://soq.zhongyouzk.top

[Q41] 多表连接
来源：http://vrz.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://crp.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://mge.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://lih.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://rbh.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://rfd.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://khv.yonumen.top

[Q43] 标量子查询
来源：http://zos.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://edt.chenjidiqi.icu

[Q44] IN 子查询
来源：http://cae.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wph.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://mgz.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wwy.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://phw.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jjm.hnqzz.top

[Q47] 与平均值比较
来源：http://cca.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iaw.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://qij.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zvw.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://vvh.zhengqikj.top

[Q49] 更新单行
来源：http://waw.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uur.tanke756.top

[Q50] 批量更新
来源：http://ngt.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://efk.jqgufenzy.top

[Q51] 用子查询更新
来源：http://rpo.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fau.hfpthk.cn

[Q52] 删除指定行
来源：http://ixn.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://wzw.wangdashe.top

[Q53] 按条件删除
来源：http://onp.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gee.yanxiufei.cn

[Q54] 清空表
来源：http://ujy.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://epk.shuidangran.top

[Q55] 排名（并列占位）
来源：http://uar.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uka.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://icr.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cdd.sjlbkw.cn

[Q57] 行号
来源：http://chz.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sbe.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://bda.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oet.yfazqb.com

[Q59] 分组内累计
来源：http://bik.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sgs.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://fif.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahx.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vth.redwolf501.top

[Q61] 移动平均
来源：http://fon.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qff.shzxlz.cn

[Q62] 分组占比
来源：http://hyu.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jen.sxryk.cn

[Q63] 开启事务
来源：http://wrv.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://twc.shanyushiyangtech.top

[Q64] 提交事务
来源：http://sav.shuidangran.top

COMMIT;
来源：http://vpr.ivvv.top

[Q65] 回滚事务
来源：http://zyv.chenjidiqi.icu

ROLLBACK;
来源：http://amf.tanke756.top

[Q66] 行锁查询
来源：http://ude.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qhd.sxryk.cn

[Q67] 设置隔离级别
来源：http://lbf.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zff.zdqjudy.top

[Q68] 保存点
来源：http://ryh.yueranfly.top

SAVEPOINT sp1;
来源：http://gvl.yangfankeji.com

ROLLBACK TO sp1;
来源：http://nhh.sweek.top

[Q69] 查看执行计划
来源：http://sxv.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jaf.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://tyn.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://bjp.yangfankeji.com

[Q71] 查看建表语句
来源：http://hlm.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gpk.mhx1999.top

[Q72] 查看索引
来源：http://yst.bjfxy.top

SHOW INDEX FROM users;
来源：http://yxe.kuanghao11.cn

[Q73] 查看表状态
来源：http://kvl.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kal.yuanzhike.top

[Q74] 强制使用索引
来源：http://mkx.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hps.yj202588.top

[Q75] 日期格式化
来源：http://lfz.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pey.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wpg.aibaodan.cn

[Q76] 按天统计
来源：http://qjq.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oib.yfazqb.com

[Q77] 时间加减
来源：http://itu.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mke.iojbl.cn

[Q78] 当前时间
来源：http://mwn.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://acm.yuxming.cn

[Q79] 字符串拼接
来源：http://chp.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rfs.9152youxi.cn

[Q80] 字符串截取
来源：http://cxh.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dzh.tanke756.top

[Q81] 字符串替换
来源：http://kuk.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tbi.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://bpn.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fbk.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://guo.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vtm.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://hfu.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://cvr.yfazqb.com

[Q85] 数值取整
来源：http://viw.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://trh.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://dvv.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gxr.vehdjk.com

[Q87] JSON 字段做条件
来源：http://ijs.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzg.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://jnj.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ltj.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rta.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://yma.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dge.svipenyu.cn

[Q90] 生成序号列
来源：http://jmk.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://upy.tian-w.cn

================================================================================
来源：http://qsa.zhengqikj.top

R. Bash 专题
来源：http://wko.bbcook.cn

================================================================================
来源：http://ilq.havefunace.top

[R01] shebang 与严格模式
来源：http://bcc.wangdashe.top

#!/usr/bin/env bash
来源：http://wzs.shangyingyoupin.top

set -euo pipefail
来源：http://yow.jinqigufen.top

[R02] 变量赋值与使用
来源：http://kii.tianlin.xyz

name="Tom"; echo "$name"
来源：http://lrc.ctjpmb.com

[R03] 只读变量
来源：http://awq.hongshengwenyu.top

readonly PI=3.14
来源：http://sft.shzxlz.cn

[R04] 位置参数
来源：http://hkp.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zoy.yangfankeji.com

[R05] 参数默认值
来源：http://cfq.meibo888.top

name="${1:-default}"
来源：http://uel.sysykeji.top

[R06] 判断命令是否存在
来源：http://iwi.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dte.ydzc1.top

[R07] if 判断文件
来源：http://gic.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sft.vqdsnc.cn

[R08] 数值比较
来源：http://vpr.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://map.jinqigufen.top

[R09] 字符串比较
来源：http://qge.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uxc.birdmap.top

[R10] 正则匹配
来源：http://skj.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nxw.jinghuilouyu.cn

[R11] case 多分支
来源：http://foi.ywan-chungtsiang.top

case "$1" in
来源：http://qzc.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://bth.aizwys.cn

stop)  echo "停止" ;;
来源：http://mvl.vehdjk.com

*)     echo "未知命令" ;;
来源：http://qhn.chenzaomai.com

esac
来源：http://fer.vqdsnc.cn

[R12] for 遍历文件
来源：http://dxj.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://eeh.tianlin.xyz

[R13] for 计数循环
来源：http://amv.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://esw.fengsongda.top

[R14] C 风格 for
来源：http://eav.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbc.hywenlv.cn

[R15] while 逐行读文件
来源：http://xce.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vgv.yj202588.top

[R16] until 等待条件
来源：http://yit.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zpx.meibo888.top

[R17] 数组定义与取值
来源：http://mec.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dyb.yanxiufei.cn

[R18] 遍历数组
来源：http://tsx.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ast.fehbvm.com

[R19] 数组长度
来源：http://qqa.zhongyouzk.top

echo "${#arr[@]}"
来源：http://lab.xuanzx.com

[R20] 关联数组（字典）
来源：http://iqb.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lfx.jlsjyb.cn

[R21] 字符串长度
来源：http://ocw.cheryme.top

echo "${#s}"
来源：http://kih.cucudq.cn

[R22] 截取子串
来源：http://suh.andypj.xyz

echo "${s:0:5}"
来源：http://inr.nanxuanxn.top

[R23] 字符串替换
来源：http://iqn.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://phr.vehdjk.com

[R24] 大小写转换
来源：http://wga.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ian.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://oor.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jen.sufxvd.cn

[R26] 命令替换
来源：http://hbf.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://xgg.zhengqikj.top

[R27] 算术展开
来源：http://ujp.yj20258.top

echo $((1 + 2 * 3))
来源：http://mgj.sjlbkw.cn

[R28] 浮点运算
来源：http://aut.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://tsp.gzhubu.top

[R29] 定义函数
来源：http://ipm.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pon.gzhubu.top

[R30] 函数返回状态码
来源：http://may.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://keg.52xcode.cn

[R31] 局部变量
来源：http://dhm.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://nqp.svipenyu.cn

[R32] 参数个数校验
来源：http://yit.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rxx.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://qjk.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uxk.gogol.net.cn

[R34] 退出时清理
来源：http://pgs.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://usr.vehdjk.com

[R35] 后台执行并等待
来源：http://qbl.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mpi.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://osg.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gcq.ivvv.top

[R37] 把输出赋给变量
来源：http://pbd.sufxvd.cn

files=$(ls -1)
来源：http://qyc.sweek.top

[R38] 管道串联
来源：http://okm.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://dfs.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://fbk.jqgufenzy.top

cmd > out.log 2>&1
来源：http://vqk.hcnkem.com

[R40] 追加写日志
来源：http://rwc.daria6918.cn

echo "log" >> out.log
来源：http://jpq.epnwcf.com

[R41] 丢弃输出
来源：http://mgp.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://zdz.cheryme.top

[R42] 输入重定向
来源：http://cmg.gzhubu.top

wc -l < a.txt
来源：http://ozl.52xcode.cn

[R43] 按名字查找文件
来源：http://eew.shzxlz.cn

find . -name "*.log" -type f
来源：http://tgq.yangfankeji.com

[R44] 按修改时间查找
来源：http://mxx.hesvh.cn

find . -mtime -7 -type f
来源：http://tco.sweek.top

[R45] 批量删除
来源：http://bsh.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://kvp.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://gec.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kfb.wangdashe.top

[R47] sed 单行替换
来源：http://pfq.zhijiandao.cn


<!-- 参考信息 -->