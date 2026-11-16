代发 wailian999

);
来源：http://gym.havefunace.top

[Q03] 增加列
来源：http://cpa.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://asu.daria6918.cn

[Q04] 修改列类型
来源：http://myb.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cxr.nwbrower.top

[Q05] 重命名列
来源：http://snl.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ooz.nwbrower.top

[Q06] 删除列
来源：http://got.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://vlp.chenjidiqi.icu

[Q07] 删除表
来源：http://bnk.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://zkn.gzhubu.top

[Q08] 创建普通索引
来源：http://gbb.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ktr.cheryme.top

[Q09] 创建唯一索引
来源：http://shg.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hyw.zdqjudy.top

[Q10] 插入单行
来源：http://ksl.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hix.316326.xyz

[Q11] 一次插入多行
来源：http://fex.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://spy.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://tjs.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://mvi.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wfb.cheryme.top

[Q13] 忽略重复插入
来源：http://atu.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gfo.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://rts.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://spp.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syz.yuanzhike.top

[Q15] 查询全部
来源：http://esr.gzhubu.top

SELECT * FROM users;
来源：http://mmq.andypj.xyz

[Q16] 查询指定列
来源：http://fgf.ehwqpu.com

SELECT id, name FROM users;
来源：http://aei.wangdashe.top

[Q17] 条件查询
来源：http://ypn.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tug.fzhhl.top

[Q18] 模糊匹配
来源：http://twz.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uxi.hnqzz.top

[Q19] 范围查询
来源：http://dhd.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwa.wangdashe.top

[Q20] IN 列表
来源：http://lsf.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fev.zhijiandao.cn

[Q21] 空值判断
来源：http://yow.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fqm.hnxiangtu.top

[Q22] 排序
来源：http://kkd.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zfu.fzhhl.top

[Q23] 分页
来源：http://fxo.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brd.snrcjt.cn

[Q24] 去重
来源：http://lyb.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://gmv.nwbrower.top

[Q25] 只取前 N 条
来源：http://yoo.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://agx.fktsv.cn

[Q26] 计数
来源：http://hrn.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://dak.tianlin.xyz

[Q27] 条件计数
来源：http://vnp.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://poc.pengpengdd.cyou

[Q28] 求和与平均
来源：http://vkg.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ovo.haohaochexian.top

[Q29] 最大最小值
来源：http://yuo.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kmj.chenjidiqi.icu

[Q30] 分组统计
来源：http://aby.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bxz.316326.xyz

[Q31] 分组后过滤
来源：http://ixg.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rbj.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://ram.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zfl.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://frn.pycfn.com

[Q33] 多列分组
来源：http://zvy.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ikc.yuxming.cn

[Q34] 每组取第一条
来源：http://hyv.tarul.cn

SELECT * FROM (
来源：http://npf.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://niy.yuxming.cn

) t WHERE rn = 1;
来源：http://pej.ywan-chungtsiang.top

[Q35] 内连接
来源：http://zss.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hnl.andypj.xyz

[Q36] 左连接
来源：http://qks.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lhu.xylfe.cn

[Q37] 右连接
来源：http://nmr.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nvp.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dku.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eqm.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://hgt.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzw.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pwr.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dht.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://joz.zdqjudy.top

[Q41] 多表连接
来源：http://yjp.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pcp.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://yvb.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://kja.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://fnf.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://ixe.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tyh.nanxuanxn.top

[Q43] 标量子查询
来源：http://cky.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bxp.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://kzj.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ufh.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://hee.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://arp.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://xtx.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kas.epnwcf.com

[Q47] 与平均值比较
来源：http://viz.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ays.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://xov.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zdt.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://aky.sjlbkw.cn

[Q49] 更新单行
来源：http://zda.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://spt.bbcook.cn

[Q50] 批量更新
来源：http://lxq.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://adc.316326.xyz

[Q51] 用子查询更新
来源：http://mel.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tzi.snrcjt.cn

[Q52] 删除指定行
来源：http://fgd.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://bhv.zhoulong.xyz

[Q53] 按条件删除
来源：http://vvi.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zmr.kuanghao11.cn

[Q54] 清空表
来源：http://ejn.hesvh.cn

TRUNCATE TABLE logs;
来源：http://ifc.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://jaw.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xae.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://zch.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kup.52xcode.cn

[Q57] 行号
来源：http://qsq.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjm.uphjek.com

[Q58] 累计求和
来源：http://nkj.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ukb.dashuyun.cn

[Q59] 分组内累计
来源：http://osf.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kyp.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://vhe.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wfq.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ozf.yanxiufei.cn

[Q61] 移动平均
来源：http://xsu.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oec.yuxming.cn

[Q62] 分组占比
来源：http://hvj.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dqn.dianchejie.cn

[Q63] 开启事务
来源：http://oyu.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eag.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://anv.zhijiandao.cn

COMMIT;
来源：http://ruo.epnwcf.com

[Q65] 回滚事务
来源：http://awj.fanxiaobao.xyz

ROLLBACK;
来源：http://ylq.yuanzhike.top

[Q66] 行锁查询
来源：http://phd.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tpx.0kj1m.cn

[Q67] 设置隔离级别
来源：http://fks.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://urz.zhiwuduotai.top

[Q68] 保存点
来源：http://osz.nanxuanxn.top

SAVEPOINT sp1;
来源：http://cbn.yueranfly.top

ROLLBACK TO sp1;
来源：http://owq.jinqigfzy.top

[Q69] 查看执行计划
来源：http://zry.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xun.zdbjq.cn

[Q70] 更新统计信息
来源：http://glc.0kj1m.cn

ANALYZE TABLE users;
来源：http://rwc.c1oappe.top

[Q71] 查看建表语句
来源：http://pch.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fah.sjlbkw.cn

[Q72] 查看索引
来源：http://ahq.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://cun.tanke756.top

[Q73] 查看表状态
来源：http://byg.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eun.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://eqq.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pzi.vqdsnc.cn

[Q75] 日期格式化
来源：http://mpw.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://git.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mfy.iojbl.cn

[Q76] 按天统计
来源：http://fwf.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hhw.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://ahi.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hoj.yangfankeji.com

[Q78] 当前时间
来源：http://cin.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qms.hywenlv.cn

[Q79] 字符串拼接
来源：http://lys.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nvq.zhixingplan.top

[Q80] 字符串截取
来源：http://hzk.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wuf.gzhubu.top

[Q81] 字符串替换
来源：http://nsp.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://khp.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://pvd.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qfs.pengpengdd.cyou

[Q83] 大小写转换
来源：http://isf.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nai.fengsongda.top

[Q84] 去除首尾空格
来源：http://hlj.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://ihk.chenzaomai.com

[Q85] 数值取整
来源：http://ymm.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dro.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://kfq.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zdh.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://xaw.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://klh.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://izn.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ols.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rir.yuxming.cn

[Q89] 判断表是否存在
来源：http://xlk.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xaq.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://wvm.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rgv.fanxiaobao.xyz

================================================================================
来源：http://uui.iojbl.cn

R. Bash 专题
来源：http://kox.aizwys.cn

================================================================================
来源：http://qkw.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://yco.tianlin.xyz

#!/usr/bin/env bash
来源：http://dnb.haohaochexian.top

set -euo pipefail
来源：http://rcx.jianghu66.top

[R02] 变量赋值与使用
来源：http://zrq.zhengqikj.top

name="Tom"; echo "$name"
来源：http://min.guannengcc.top

[R03] 只读变量
来源：http://lvl.yonumen.top

readonly PI=3.14
来源：http://ixv.zhixingplan.top

[R04] 位置参数
来源：http://iek.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kgw.tanke756.top

[R05] 参数默认值
来源：http://gbs.jyoumei.cn

name="${1:-default}"
来源：http://rlt.chenlongwang.top

[R06] 判断命令是否存在
来源：http://tca.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gdr.feifeiyinyue.top

[R07] if 判断文件
来源：http://lnz.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rif.dianchejie.cn

[R08] 数值比较
来源：http://eob.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ecj.fktsv.cn

[R09] 字符串比较
来源：http://aha.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyi.hnqzz.top

[R10] 正则匹配
来源：http://pak.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jxf.vqdsnc.cn

[R11] case 多分支
来源：http://noy.xylfe.cn

case "$1" in
来源：http://kpg.hfpthk.cn

start) echo "启动" ;;
来源：http://tle.sweek.top

stop)  echo "停止" ;;
来源：http://ivu.xinyue.icu

*)     echo "未知命令" ;;
来源：http://rhw.xinyue.icu

esac
来源：http://rmr.bjfxy.top

[R12] for 遍历文件
来源：http://een.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://ses.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://uxc.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://xsg.zhijiandao.cn

[R14] C 风格 for
来源：http://oih.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sfr.jlsjyb.cn

[R15] while 逐行读文件
来源：http://div.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fgq.guowangkeji.top

[R16] until 等待条件
来源：http://hbq.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tug.dashuyun.cn

[R17] 数组定义与取值
来源：http://qiu.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://ccm.hywenlv.cn

[R18] 遍历数组
来源：http://lzt.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oxu.shanyushiyangtech.top

[R19] 数组长度
来源：http://ywn.tarul.cn

echo "${#arr[@]}"
来源：http://bwd.yueranfly.top

[R20] 关联数组（字典）
来源：http://ylo.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kwu.hnxiangtu.top

[R21] 字符串长度
来源：http://ulz.sxryk.cn

echo "${#s}"
来源：http://yhc.zdqjudy.top

[R22] 截取子串
来源：http://fia.tian-w.cn

echo "${s:0:5}"
来源：http://iix.jqgufenzy.top

[R23] 字符串替换
来源：http://dlt.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fwg.meibo888.top

[R24] 大小写转换
来源：http://dgk.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://oeb.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://jyw.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fst.pycfn.com

[R26] 命令替换
来源：http://tcs.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://zgf.jinghuilouyu.cn

[R27] 算术展开
来源：http://kej.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://jqd.iojbl.cn

[R28] 浮点运算
来源：http://neo.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://pdm.dianchejie.cn

[R29] 定义函数
来源：http://nqi.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dcp.316326.xyz

[R30] 函数返回状态码
来源：http://sjh.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://bhn.xinyue.icu

[R31] 局部变量
来源：http://ssg.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://ayc.feifeiyinyue.top

[R32] 参数个数校验
来源：http://ohw.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://djs.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://oas.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ajh.jiagoushi.top

[R34] 退出时清理
来源：http://bpa.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://nqa.bbcook.cn

[R35] 后台执行并等待
来源：http://zay.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uhv.wangdashe.top

[R36] 并发执行多个任务
来源：http://gpk.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://igv.chenlongwang.top

[R37] 把输出赋给变量
来源：http://fby.xinyue.icu

files=$(ls -1)
来源：http://afm.shanyushiyangtech.top

[R38] 管道串联
来源：http://zdd.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://ern.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://bce.xziqi.cn

cmd > out.log 2>&1
来源：http://aad.yfazqb.com

[R40] 追加写日志
来源：http://olq.hysaishi.cn

echo "log" >> out.log
来源：http://ddn.52xcode.cn

[R41] 丢弃输出
来源：http://rpj.hesvh.cn

cmd >/dev/null 2>&1
来源：http://kui.chenlongwang.top

[R42] 输入重定向
来源：http://sse.iojbl.cn

wc -l < a.txt
来源：http://pzp.jqgfzy.top

[R43] 按名字查找文件
来源：http://rrm.guannengcc.top

find . -name "*.log" -type f
来源：http://ohg.ivvv.top

[R44] 按修改时间查找
来源：http://dsz.chenlongwang.top

find . -mtime -7 -type f
来源：http://vnc.zhaomingkeji.xyz

[R45] 批量删除
来源：http://rpu.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://uly.hammf.cn

[R46] 递归替换文件内容
来源：http://hiu.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jug.wangdashe.top

[R47] sed 单行替换
来源：http://nko.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://mji.quarkkingdee.top

[R48] awk 取指定列
来源：http://wil.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://qnr.zhengqikj.top

[R49] awk 带条件
来源：http://cjo.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xhb.uphjek.com

[R50] awk 求和
来源：http://scc.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://uuf.sjlbkw.cn

[R51] 排序去重取前几
来源：http://vpj.hammf.cn


<!-- 参考信息 -->