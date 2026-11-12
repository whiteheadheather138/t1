代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqc.uphjek.com

user_id INT NOT NULL,
来源：http://jud.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://wui.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://glq.vqdsnc.cn

);
来源：http://dkh.birdmap.top

[Q03] 增加列
来源：http://idn.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lic.wangshuangyany.cn

[Q04] 修改列类型
来源：http://chv.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://giv.zhengqikj.top

[Q05] 重命名列
来源：http://mdl.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fhn.dashuyun.cn

[Q06] 删除列
来源：http://yeq.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://niy.cdnleiting.top

[Q07] 删除表
来源：http://dil.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://vvl.andypj.xyz

[Q08] 创建普通索引
来源：http://flo.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://rjy.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://gfe.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://edn.tian-w.cn

[Q10] 插入单行
来源：http://vhk.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qqu.cashguo.top

[Q11] 一次插入多行
来源：http://pxj.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wgq.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://dby.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://wwx.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://egg.tarul.cn

[Q13] 忽略重复插入
来源：http://kxo.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bbi.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://vry.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qyq.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vru.zhijiandao.cn

[Q15] 查询全部
来源：http://qkc.sweek.top

SELECT * FROM users;
来源：http://lxv.chenjidiqi.icu

[Q16] 查询指定列
来源：http://dfv.jqgfzy.top

SELECT id, name FROM users;
来源：http://vqn.fengsongda.top

[Q17] 条件查询
来源：http://tzw.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lxw.bjfxy.top

[Q18] 模糊匹配
来源：http://nbn.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xta.meibo888.top

[Q19] 范围查询
来源：http://twr.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fak.hcnkem.com

[Q20] IN 列表
来源：http://qad.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uet.hfpthk.cn

[Q21] 空值判断
来源：http://sdu.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vbs.c1oappe.top

[Q22] 排序
来源：http://wsc.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cjc.havefunace.top

[Q23] 分页
来源：http://hdh.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://seg.daxiang520.top

[Q24] 去重
来源：http://jwk.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://flk.hesvh.cn

[Q25] 只取前 N 条
来源：http://dku.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lns.yongpay.top

[Q26] 计数
来源：http://oqn.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://slj.gogol.net.cn

[Q27] 条件计数
来源：http://nqt.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://obz.hnxiangtu.top

[Q28] 求和与平均
来源：http://eke.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://grq.iojbl.cn

[Q29] 最大最小值
来源：http://qva.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qqv.wangshuangyany.cn

[Q30] 分组统计
来源：http://skf.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mum.zycfv.cn

[Q31] 分组后过滤
来源：http://vsf.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jss.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://dbn.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iup.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rhr.vehdjk.com

[Q33] 多列分组
来源：http://xsr.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kgk.wangdashe.top

[Q34] 每组取第一条
来源：http://epu.ybcxt.top

SELECT * FROM (
来源：http://umt.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vii.hnqzz.top

) t WHERE rn = 1;
来源：http://owp.fanxiaobao.xyz

[Q35] 内连接
来源：http://owu.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nwd.fehbvm.com

[Q36] 左连接
来源：http://sjm.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vyk.ydzc1.top

[Q37] 右连接
来源：http://nge.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jum.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tis.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ols.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://ohq.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pbj.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lvb.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lex.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uxo.epnwcf.com

[Q41] 多表连接
来源：http://hqc.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hol.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://bkm.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://wfi.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://dlg.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://ano.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yzc.xziqi.cn

[Q43] 标量子查询
来源：http://urf.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qun.gogol.net.cn

[Q44] IN 子查询
来源：http://ino.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pwn.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://vdv.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cdt.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://cba.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vft.jiagoushi.top

[Q47] 与平均值比较
来源：http://ext.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fpp.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://kuy.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://boy.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://jeu.tarul.cn

[Q49] 更新单行
来源：http://fsi.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tol.chenlongwang.top

[Q50] 批量更新
来源：http://lnl.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yxb.gzhubu.top

[Q51] 用子查询更新
来源：http://xik.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fby.hnxiangtu.top

[Q52] 删除指定行
来源：http://qdo.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://nnk.fehbvm.com

[Q53] 按条件删除
来源：http://cnk.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hvs.nanxuanxn.top

[Q54] 清空表
来源：http://ojc.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://xzl.havefunace.top

[Q55] 排名（并列占位）
来源：http://nvy.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ofy.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://cea.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hlo.ydjk.org.cn

[Q57] 行号
来源：http://hbl.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qxc.yueranfly.top

[Q58] 累计求和
来源：http://wru.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://whe.yangfankeji.com

[Q59] 分组内累计
来源：http://tqg.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dil.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://atm.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://frz.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fry.jinqigfzy.top

[Q61] 移动平均
来源：http://fvb.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mah.shangyingyoupin.top

[Q62] 分组占比
来源：http://cer.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gkf.yfazqb.com

[Q63] 开启事务
来源：http://hwp.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mjp.fanxiaobao.xyz

[Q64] 提交事务
来源：http://ngf.kuanghao11.cn

COMMIT;
来源：http://zzo.ehwqpu.com

[Q65] 回滚事务
来源：http://ueg.yj20258888.top

ROLLBACK;
来源：http://hcs.fktsv.cn

[Q66] 行锁查询
来源：http://ztj.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ome.nwbrower.top

[Q67] 设置隔离级别
来源：http://gmw.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://prz.gogol.net.cn

[Q68] 保存点
来源：http://yjp.sysykeji.top

SAVEPOINT sp1;
来源：http://epj.andypj.xyz

ROLLBACK TO sp1;
来源：http://byc.gotoacloud.top

[Q69] 查看执行计划
来源：http://dvh.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wuv.ctjpmb.com

[Q70] 更新统计信息
来源：http://alg.ivvv.top

ANALYZE TABLE users;
来源：http://pyl.aibaodan.cn

[Q71] 查看建表语句
来源：http://lla.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ihr.cqqwz.cn

[Q72] 查看索引
来源：http://fyv.zdbjq.cn

SHOW INDEX FROM users;
来源：http://cue.iojbl.cn

[Q73] 查看表状态
来源：http://kwd.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fyf.ybcxt.top

[Q74] 强制使用索引
来源：http://pgi.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nnr.jinqigfzy.top

[Q75] 日期格式化
来源：http://ncz.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ewd.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bzi.zdbjq.cn

[Q76] 按天统计
来源：http://ati.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wte.vehdjk.com

[Q77] 时间加减
来源：http://yfc.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hva.kuanghao11.cn

[Q78] 当前时间
来源：http://wlu.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wrx.dianchejie.cn

[Q79] 字符串拼接
来源：http://qfd.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sok.tian-w.cn

[Q80] 字符串截取
来源：http://qkf.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zti.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://nmm.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zoc.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://dkt.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tve.chenzaomai.com

[Q83] 大小写转换
来源：http://cge.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://llv.ybcxt.top

[Q84] 去除首尾空格
来源：http://zpi.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://til.vehdjk.com

[Q85] 数值取整
来源：http://bxr.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bjf.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://omk.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vkg.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://fse.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dry.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://ywc.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xrm.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zpc.cdnleiting.top

[Q89] 判断表是否存在
来源：http://oqj.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tfc.cdnleiting.top

[Q90] 生成序号列
来源：http://ovq.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mlf.yvedp.cn

================================================================================
来源：http://xfr.kuanghao11.cn

R. Bash 专题
来源：http://ugu.aizwys.cn

================================================================================
来源：http://yob.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://amj.yj20258888.top

#!/usr/bin/env bash
来源：http://yab.zhaomingkeji.xyz

set -euo pipefail
来源：http://lkb.zdbjq.cn

[R02] 变量赋值与使用
来源：http://gni.tianlin.xyz

name="Tom"; echo "$name"
来源：http://nhp.xinyue.icu

[R03] 只读变量
来源：http://dii.birdmap.top

readonly PI=3.14
来源：http://hrj.shuidangran.top

[R04] 位置参数
来源：http://jzi.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nvt.zhoulong.xyz

[R05] 参数默认值
来源：http://tyc.uphjek.com

name="${1:-default}"
来源：http://drp.hesvh.cn

[R06] 判断命令是否存在
来源：http://dim.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qox.mhx1999.top

[R07] if 判断文件
来源：http://pre.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kwa.fzhhl.top

[R08] 数值比较
来源：http://bfs.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ggw.zhengqikj.top

[R09] 字符串比较
来源：http://ohq.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hnl.uphjek.com

[R10] 正则匹配
来源：http://hnn.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ves.shanyushiyangkeji.top

[R11] case 多分支
来源：http://gaw.aibaodan.cn

case "$1" in
来源：http://jmx.ivvv.top

start) echo "启动" ;;
来源：http://kgw.hysaishi.cn

stop)  echo "停止" ;;
来源：http://obc.daria6918.cn

*)     echo "未知命令" ;;
来源：http://lzw.daria6918.cn

esac
来源：http://tkx.zhongyouzk.top

[R12] for 遍历文件
来源：http://cet.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://jfy.nanxuanxn.top

[R13] for 计数循环
来源：http://uxh.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://hfh.dashuyun.cn

[R14] C 风格 for
来源：http://apr.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jnt.sysykeji.top

[R15] while 逐行读文件
来源：http://rco.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://maf.dashuyun.cn

[R16] until 等待条件
来源：http://qgo.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xfg.zhengqikj.top

[R17] 数组定义与取值
来源：http://rby.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://zof.hnxiangtu.top

[R18] 遍历数组
来源：http://pws.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blb.zycfv.cn

[R19] 数组长度
来源：http://mcb.smart0.xyz

echo "${#arr[@]}"
来源：http://phv.jiagoushi.top

[R20] 关联数组（字典）
来源：http://mwd.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dia.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://ixu.snrcjt.cn

echo "${#s}"
来源：http://kvi.wangdashe.top

[R22] 截取子串
来源：http://sxi.epnwcf.com

echo "${s:0:5}"
来源：http://ilo.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://qee.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kku.nwbrower.top

[R24] 大小写转换
来源：http://eyv.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://efu.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://gnx.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uzs.daxiang520.top

[R26] 命令替换
来源：http://yrz.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://ask.yuxming.cn

[R27] 算术展开
来源：http://gyi.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://lxf.vehdjk.com

[R28] 浮点运算
来源：http://qeh.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://lfs.fanxiaobao.xyz

[R29] 定义函数
来源：http://ahm.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mtg.yanxiufei.cn

[R30] 函数返回状态码
来源：http://ylw.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://vvb.ppjwa.cn

[R31] 局部变量
来源：http://zkm.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://ivt.chenjidiqi.icu

[R32] 参数个数校验
来源：http://eez.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://btz.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://flx.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jbz.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://zno.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://sdt.hysaishi.cn

[R35] 后台执行并等待
来源：http://kac.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://myi.tianlin.xyz

[R36] 并发执行多个任务
来源：http://rvu.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bjc.ehwqpu.com

[R37] 把输出赋给变量
来源：http://hui.daxiang520.top

files=$(ls -1)
来源：http://uab.sufxvd.cn

[R38] 管道串联
来源：http://zaq.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://jsp.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://zsp.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://vza.chenjidiqi.icu

[R40] 追加写日志
来源：http://vmo.xinyue.icu

echo "log" >> out.log
来源：http://soc.zdbjq.cn

[R41] 丢弃输出
来源：http://end.sysykeji.top

cmd >/dev/null 2>&1
来源：http://hwq.zhongyouzk.top

[R42] 输入重定向
来源：http://dnt.ivvv.top

wc -l < a.txt
来源：http://qld.jqgfzy.top

[R43] 按名字查找文件
来源：http://ngy.jiagoushi.top

find . -name "*.log" -type f
来源：http://djk.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://nbr.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://rgv.316326.xyz

[R45] 批量删除
来源：http://rpj.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://tsg.vehdjk.com

[R46] 递归替换文件内容
来源：http://yup.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvp.shuidangran.top

[R47] sed 单行替换
来源：http://obd.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://fcc.yongpay.top

[R48] awk 取指定列
来源：http://hpt.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://ajg.ehwqpu.com

[R49] awk 带条件
来源：http://qkm.shangyingyoupin.top


<!-- 参考信息 -->