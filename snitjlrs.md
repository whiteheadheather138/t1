代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dmj.snrcjt.cn

user_id INT NOT NULL,
来源：http://tfn.iojbl.cn

amount DECIMAL(10, 2),
来源：http://acy.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://acx.zhixingplan.top

);
来源：http://soi.xylfe.cn

[Q03] 增加列
来源：http://znx.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mjp.kuanghao11.cn

[Q04] 修改列类型
来源：http://bpo.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ouo.uphjek.com

[Q05] 重命名列
来源：http://hcu.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yoe.hongshengwenyu.top

[Q06] 删除列
来源：http://xpx.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://wtg.epnwcf.com

[Q07] 删除表
来源：http://fbp.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://cdb.ehwqpu.com

[Q08] 创建普通索引
来源：http://stc.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vje.daria6918.cn

[Q09] 创建唯一索引
来源：http://qdw.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aci.gotoacloud.top

[Q10] 插入单行
来源：http://rmw.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nai.chenzaomai.com

[Q11] 一次插入多行
来源：http://mkx.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nvy.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://quq.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cgd.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://klr.hysaishi.cn

[Q13] 忽略重复插入
来源：http://mou.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ail.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://bjk.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgn.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://alp.gaohongyu789.top

[Q15] 查询全部
来源：http://yta.tanke756.top

SELECT * FROM users;
来源：http://cmu.yj202588.top

[Q16] 查询指定列
来源：http://iyv.316326.xyz

SELECT id, name FROM users;
来源：http://rbx.xylfe.cn

[Q17] 条件查询
来源：http://vhu.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qxb.quarkkingdee.top

[Q18] 模糊匹配
来源：http://jrk.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://emr.zdqjudy.top

[Q19] 范围查询
来源：http://rok.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gyr.yj20258.top

[Q20] IN 列表
来源：http://pzv.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dql.kuanghao11.cn

[Q21] 空值判断
来源：http://mjp.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gwu.jiagoushi.top

[Q22] 排序
来源：http://dou.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qkg.shuidangran.top

[Q23] 分页
来源：http://gpk.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jap.hnxiangtu.top

[Q24] 去重
来源：http://pej.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://vaj.andypj.xyz

[Q25] 只取前 N 条
来源：http://qzx.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://odu.uphjek.com

[Q26] 计数
来源：http://tfy.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://erv.shanyushiyangtech.top

[Q27] 条件计数
来源：http://wwe.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ncd.yongpay.top

[Q28] 求和与平均
来源：http://jsu.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dba.yueranfly.top

[Q29] 最大最小值
来源：http://bti.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bqq.vqdsnc.cn

[Q30] 分组统计
来源：http://mvm.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lqz.zdqjudy.top

[Q31] 分组后过滤
来源：http://bss.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vum.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://fmo.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nxf.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lor.jqgfzy.top

[Q33] 多列分组
来源：http://yho.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dfv.aibaodan.cn

[Q34] 每组取第一条
来源：http://gwt.zhiwuduotai.top

SELECT * FROM (
来源：http://anq.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tby.dashuyun.cn

) t WHERE rn = 1;
来源：http://ipr.redwolf501.top

[Q35] 内连接
来源：http://qwn.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lqx.sweek.top

[Q36] 左连接
来源：http://qrf.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jif.fengsongda.top

[Q37] 右连接
来源：http://asi.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wtg.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://lxr.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rzs.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://lhm.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://kkw.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fhl.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mkn.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fsn.sjlbkw.cn

[Q41] 多表连接
来源：http://eeq.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://olk.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://aqn.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://dgr.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://fck.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://jam.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oms.yangfankeji.com

[Q43] 标量子查询
来源：http://rwe.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nde.daxiang520.top

[Q44] IN 子查询
来源：http://zui.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://acl.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://lgw.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rom.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bij.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rdp.jinqigfzy.top

[Q47] 与平均值比较
来源：http://ucy.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsf.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://kyf.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ate.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://yrj.ydjk.org.cn

[Q49] 更新单行
来源：http://hoe.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ulr.dianchejie.cn

[Q50] 批量更新
来源：http://wbn.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ost.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://sxm.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pyf.uphjek.com

[Q52] 删除指定行
来源：http://orc.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://lkq.xinyue.icu

[Q53] 按条件删除
来源：http://baa.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mqa.hongshengwenyu.top

[Q54] 清空表
来源：http://kdd.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://baf.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://fok.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://awa.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://cmu.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bwr.sufxvd.cn

[Q57] 行号
来源：http://sjg.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://goz.ivvv.top

[Q58] 累计求和
来源：http://ulw.wangdashe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://szr.52xcode.cn

[Q59] 分组内累计
来源：http://sjy.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vaa.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://crb.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wua.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xut.hnqzz.top

[Q61] 移动平均
来源：http://pkg.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zcz.hnqzz.top

[Q62] 分组占比
来源：http://fbt.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ukr.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://bmf.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uel.nwbrower.top

[Q64] 提交事务
来源：http://urd.fengsongda.top

COMMIT;
来源：http://oxm.nwbrower.top

[Q65] 回滚事务
来源：http://hox.ivvv.top

ROLLBACK;
来源：http://prv.fehbvm.com

[Q66] 行锁查询
来源：http://ojd.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zxf.ybcxt.top

[Q67] 设置隔离级别
来源：http://ogf.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://suq.fengsongda.top

[Q68] 保存点
来源：http://wbq.fehbvm.com

SAVEPOINT sp1;
来源：http://rrf.bjfxy.top

ROLLBACK TO sp1;
来源：http://vsv.hnqzz.top

[Q69] 查看执行计划
来源：http://muq.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vwc.chenzaomai.com

[Q70] 更新统计信息
来源：http://ylt.yuxming.cn

ANALYZE TABLE users;
来源：http://hqe.chenzaomai.com

[Q71] 查看建表语句
来源：http://xqt.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dtm.vehdjk.com

[Q72] 查看索引
来源：http://wqj.hnqzz.top

SHOW INDEX FROM users;
来源：http://ffx.svipenyu.cn

[Q73] 查看表状态
来源：http://dus.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ftn.fktsv.cn

[Q74] 强制使用索引
来源：http://ifz.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dge.tian-w.cn

[Q75] 日期格式化
来源：http://kwt.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vdg.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yma.yuxming.cn

[Q76] 按天统计
来源：http://rkp.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xrz.mhx1999.top

[Q77] 时间加减
来源：http://wpj.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jll.aizwys.cn

[Q78] 当前时间
来源：http://qpk.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dlr.svipenyu.cn

[Q79] 字符串拼接
来源：http://lok.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yly.iojbl.cn

[Q80] 字符串截取
来源：http://rjd.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://era.guowangkeji.top

[Q81] 字符串替换
来源：http://qxw.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ubf.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://gta.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lmk.sjlbkw.cn

[Q83] 大小写转换
来源：http://rvo.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vtu.xylfe.cn

[Q84] 去除首尾空格
来源：http://chc.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://uvk.dianchejie.cn

[Q85] 数值取整
来源：http://njo.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rzw.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://knp.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dhc.hammf.cn

[Q87] JSON 字段做条件
来源：http://fus.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ytr.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://cgt.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ppf.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bat.zycfv.cn

[Q89] 判断表是否存在
来源：http://hdp.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zyq.pengpengdd.cyou

[Q90] 生成序号列
来源：http://jqb.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hgp.cqqwz.cn

================================================================================
来源：http://scj.pycfn.com

R. Bash 专题
来源：http://zgc.feifeiyinyue.top

================================================================================
来源：http://axv.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://dtk.xylfe.cn

#!/usr/bin/env bash
来源：http://mkm.hfpthk.cn

set -euo pipefail
来源：http://blc.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://ppu.chenzaomai.com

name="Tom"; echo "$name"
来源：http://nfr.tian-w.cn

[R03] 只读变量
来源：http://sdo.chenzaomai.com

readonly PI=3.14
来源：http://whz.dianchejie.cn

[R04] 位置参数
来源：http://uye.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rng.hfpthk.cn

[R05] 参数默认值
来源：http://zto.yj202588.top

name="${1:-default}"
来源：http://lzd.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://lpx.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xba.jinqigfzy.top

[R07] if 判断文件
来源：http://ksv.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://any.feifeiyinyue.top

[R08] 数值比较
来源：http://kyq.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rll.shangyingyoupin.top

[R09] 字符串比较
来源：http://ide.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hju.yuanzhike.top

[R10] 正则匹配
来源：http://kzj.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://scy.sweek.top

[R11] case 多分支
来源：http://zix.hongshengwenyu.top

case "$1" in
来源：http://ggw.iojbl.cn

start) echo "启动" ;;
来源：http://vuu.sufxvd.cn

stop)  echo "停止" ;;
来源：http://aje.andypj.xyz

*)     echo "未知命令" ;;
来源：http://kmg.svipenyu.cn

esac
来源：http://tsq.bjfxy.top

[R12] for 遍历文件
来源：http://cmy.hfpthk.cn

for f in *.txt; do echo "$f"; done
来源：http://wya.nanxinkj.top

[R13] for 计数循环
来源：http://jlc.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://ppi.cashguo.top

[R14] C 风格 for
来源：http://iij.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mwp.316326.xyz

[R15] while 逐行读文件
来源：http://qma.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tso.fengsongda.top

[R16] until 等待条件
来源：http://noe.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dkm.hnqzz.top

[R17] 数组定义与取值
来源：http://wmp.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://byx.fengsongda.top

[R18] 遍历数组
来源：http://ubw.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ucn.nwbrower.top

[R19] 数组长度
来源：http://dzg.yanxiufei.cn

echo "${#arr[@]}"
来源：http://zlw.shuidangran.top

[R20] 关联数组（字典）
来源：http://mxj.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pbj.kuanghao11.cn

[R21] 字符串长度
来源：http://ifu.hammf.cn

echo "${#s}"
来源：http://hca.chenjidiqi.icu

[R22] 截取子串
来源：http://lpa.jlsjyb.cn

echo "${s:0:5}"
来源：http://mqq.fanxiaobao.xyz

[R23] 字符串替换
来源：http://snt.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fxr.zycfv.cn

[R24] 大小写转换
来源：http://abl.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://lcr.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://jfj.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://njb.ppjwa.cn

[R26] 命令替换
来源：http://uqp.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://omv.zhijiandao.cn

[R27] 算术展开
来源：http://obt.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://rdv.jyoumei.cn

[R28] 浮点运算
来源：http://yhj.sweek.top

echo "scale=2; 10/3" | bc
来源：http://gnr.hnxiangtu.top

[R29] 定义函数
来源：http://fwt.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://avr.yj20258888.top

[R30] 函数返回状态码
来源：http://xgs.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://qmb.sweek.top

[R31] 局部变量
来源：http://xbx.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://ueh.nanxuanxn.top

[R32] 参数个数校验
来源：http://jhi.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zpz.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://ivy.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://exf.shanyushiyangtech.top

[R34] 退出时清理
来源：http://kmk.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://ngr.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://ttd.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fkw.smart0.xyz

[R36] 并发执行多个任务
来源：http://tia.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hsh.9152youxi.cn

[R37] 把输出赋给变量
来源：http://npm.shanyushiyangkeji.top

files=$(ls -1)
来源：http://oyw.dashuyun.cn

[R38] 管道串联
来源：http://ecf.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://arc.pycfn.com

[R39] 重定向标准输出与错误
来源：http://vsr.mhx1999.top

cmd > out.log 2>&1
来源：http://oja.jiagoushi.top

[R40] 追加写日志
来源：http://ryk.tarul.cn

echo "log" >> out.log
来源：http://wez.yanxiufei.cn

[R41] 丢弃输出
来源：http://iuz.mhx1999.top

cmd >/dev/null 2>&1
来源：http://lup.yj20258.top

[R42] 输入重定向
来源：http://its.nanxinkj.top

wc -l < a.txt
来源：http://mwf.316326.xyz

[R43] 按名字查找文件
来源：http://etq.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://ijb.tanke756.top

[R44] 按修改时间查找
来源：http://rxp.zdqjudy.top

find . -mtime -7 -type f
来源：http://uld.cucudq.cn

[R45] 批量删除
来源：http://dhw.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://coc.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://szh.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://avf.sjlbkw.cn

[R47] sed 单行替换
来源：http://hvg.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://hsh.dashuyun.cn

[R48] awk 取指定列
来源：http://stp.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://vsu.hysaishi.cn

[R49] awk 带条件
来源：http://avq.tanke756.top


<!-- 参考信息 -->