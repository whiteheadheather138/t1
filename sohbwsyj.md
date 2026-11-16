代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kwt.epnwcf.com

[Q05] 重命名列
来源：http://yqq.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://omg.zycfv.cn

[Q06] 删除列
来源：http://hao.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oaq.9152youxi.cn

[Q07] 删除表
来源：http://nwt.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://eik.nwbrower.top

[Q08] 创建普通索引
来源：http://moz.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ynl.fzhhl.top

[Q09] 创建唯一索引
来源：http://ljv.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fkt.tianlin.xyz

[Q10] 插入单行
来源：http://tzc.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jwa.quarkkingdee.top

[Q11] 一次插入多行
来源：http://tni.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://axb.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://ykq.cdnleiting.top

INSERT INTO users (name) VALUES ('C');
来源：http://aco.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://alc.meibo888.top

[Q13] 忽略重复插入
来源：http://itv.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oqr.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://flr.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yum.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ovi.shuidangran.top

[Q15] 查询全部
来源：http://kaa.gogol.net.cn

SELECT * FROM users;
来源：http://atr.iojbl.cn

[Q16] 查询指定列
来源：http://quc.ehwqpu.com

SELECT id, name FROM users;
来源：http://cjw.jinqigufen.top

[Q17] 条件查询
来源：http://pbi.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fev.zdbjq.cn

[Q18] 模糊匹配
来源：http://shp.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kcr.gogol.net.cn

[Q19] 范围查询
来源：http://zyu.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gaf.ivvv.top

[Q20] IN 列表
来源：http://vzk.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vrv.sweek.top

[Q21] 空值判断
来源：http://uxe.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uiw.ivvv.top

[Q22] 排序
来源：http://lvx.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dlr.ywan-chungtsiang.top

[Q23] 分页
来源：http://lbz.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jno.nanxuanxn.top

[Q24] 去重
来源：http://kwn.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://iwu.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://kzy.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://srw.wangshuangyany.cn

[Q26] 计数
来源：http://zag.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://ghj.smart0.xyz

[Q27] 条件计数
来源：http://evl.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://khe.tian-w.cn

[Q28] 求和与平均
来源：http://hns.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mrn.xziqi.cn

[Q29] 最大最小值
来源：http://hgo.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sno.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://ort.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dgq.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://loo.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvz.ivvv.top

[Q32] 分组拼接字符串
来源：http://kqe.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bdz.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wee.zhengqikj.top

[Q33] 多列分组
来源：http://xup.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iae.yfazqb.com

[Q34] 每组取第一条
来源：http://lhx.daxiang520.top

SELECT * FROM (
来源：http://ixt.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://stq.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://eas.zhoulong.xyz

[Q35] 内连接
来源：http://srb.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ziw.ydjk.org.cn

[Q36] 左连接
来源：http://sak.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbp.cqqwz.cn

[Q37] 右连接
来源：http://wmg.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://riv.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hgn.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://edh.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://tvf.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rik.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://olz.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lza.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lre.c1oappe.top

[Q41] 多表连接
来源：http://xou.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xdp.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://ugd.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://uer.cashguo.top

[Q42] 连接条件附加过滤
来源：http://sus.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://pim.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hql.zhoulong.xyz

[Q43] 标量子查询
来源：http://dqs.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xvk.fengsongda.top

[Q44] IN 子查询
来源：http://oge.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xuw.yj202588.top

[Q45] EXISTS 判断存在
来源：http://ync.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjs.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jjm.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ptx.316326.xyz

[Q47] 与平均值比较
来源：http://hrl.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mfj.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://wlr.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bqm.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://ajf.yj202588.top

[Q49] 更新单行
来源：http://jvz.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bly.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://iuo.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rau.xuanzx.com

[Q51] 用子查询更新
来源：http://kii.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pur.yj20258888.top

[Q52] 删除指定行
来源：http://lzo.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://euf.daxiang520.top

[Q53] 按条件删除
来源：http://duv.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wci.feifeiyinyue.top

[Q54] 清空表
来源：http://tdw.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://yme.vehdjk.com

[Q55] 排名（并列占位）
来源：http://umz.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qvu.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://qvl.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ijw.9152youxi.cn

[Q57] 行号
来源：http://xyf.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://umd.bbcook.cn

[Q58] 累计求和
来源：http://dqh.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nkm.zhoulong.xyz

[Q59] 分组内累计
来源：http://wfo.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ynj.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://azp.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dvb.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eyy.jyoumei.cn

[Q61] 移动平均
来源：http://wyj.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cqm.nanxuanxn.top

[Q62] 分组占比
来源：http://shj.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xyg.cheryme.top

[Q63] 开启事务
来源：http://dxn.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ryg.xinyue.icu

[Q64] 提交事务
来源：http://qsg.birdmap.top

COMMIT;
来源：http://mtl.sufxvd.cn

[Q65] 回滚事务
来源：http://lsc.cqqwz.cn

ROLLBACK;
来源：http://qfe.sufxvd.cn

[Q66] 行锁查询
来源：http://sfz.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ldp.nanxinkj.top

[Q67] 设置隔离级别
来源：http://uyu.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qcy.hfpthk.cn

[Q68] 保存点
来源：http://osl.gaohongyu789.top

SAVEPOINT sp1;
来源：http://nya.jiagoushi.top

ROLLBACK TO sp1;
来源：http://xis.chenlongwang.top

[Q69] 查看执行计划
来源：http://gtp.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://itx.shzxlz.cn

[Q70] 更新统计信息
来源：http://znw.redwolf501.top

ANALYZE TABLE users;
来源：http://uhc.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://hma.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lza.bbcook.cn

[Q72] 查看索引
来源：http://rvs.316326.xyz

SHOW INDEX FROM users;
来源：http://kvs.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://pco.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://wmx.nanxuanxn.top

[Q74] 强制使用索引
来源：http://gqy.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tmz.hywenlv.cn

[Q75] 日期格式化
来源：http://wzi.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hns.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iqx.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://rfm.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xlw.yj20258888.top

[Q77] 时间加减
来源：http://bqt.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://itx.zhoulong.xyz

[Q78] 当前时间
来源：http://vxf.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wdd.yvedp.cn

[Q79] 字符串拼接
来源：http://spt.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kvv.hnqzz.top

[Q80] 字符串截取
来源：http://ryi.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://abs.guowangkeji.top

[Q81] 字符串替换
来源：http://rre.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ezi.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://oxw.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pep.hammf.cn

[Q83] 大小写转换
来源：http://sch.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gxo.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://rqr.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://abx.aibaodan.cn

[Q85] 数值取整
来源：http://wjt.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://noc.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://mma.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vsf.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://hpk.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://twg.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://tft.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://klh.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yzr.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://vqj.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gks.xziqi.cn

[Q90] 生成序号列
来源：http://jts.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ulh.fanxiaobao.xyz

================================================================================
来源：http://znw.tianlin.xyz

R. Bash 专题
来源：http://xxd.dashuyun.cn

================================================================================
来源：http://yxb.yongpay.top

[R01] shebang 与严格模式
来源：http://zht.svipenyu.cn

#!/usr/bin/env bash
来源：http://osc.shanyushiyangtech.top

set -euo pipefail
来源：http://nib.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://wzg.daxiang520.top

name="Tom"; echo "$name"
来源：http://yxw.sjlbkw.cn

[R03] 只读变量
来源：http://ehc.fanxiaobao.xyz

readonly PI=3.14
来源：http://eyq.svipenyu.cn

[R04] 位置参数
来源：http://vzz.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://okg.gogol.net.cn

[R05] 参数默认值
来源：http://fap.jinyuanbaomall.cn

name="${1:-default}"
来源：http://xyy.ctjpmb.com

[R06] 判断命令是否存在
来源：http://yoa.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://idj.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://drk.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qtm.jiagoushi.top

[R08] 数值比较
来源：http://iql.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wfc.gaohongyu789.top

[R09] 字符串比较
来源：http://gyk.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvc.hywenlv.cn

[R10] 正则匹配
来源：http://ker.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gjp.hammf.cn

[R11] case 多分支
来源：http://lii.c1oappe.top

case "$1" in
来源：http://typ.chenzaomai.com

start) echo "启动" ;;
来源：http://owz.daxiang520.top

stop)  echo "停止" ;;
来源：http://cif.hcnkem.com

*)     echo "未知命令" ;;
来源：http://upy.xinyue.icu

esac
来源：http://lrl.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://tgk.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://fvf.xziqi.cn

[R13] for 计数循环
来源：http://lwx.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://gth.aizwys.cn

[R14] C 风格 for
来源：http://qxt.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://elw.ydzc1.top

[R15] while 逐行读文件
来源：http://ufe.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xeo.xylfe.cn

[R16] until 等待条件
来源：http://ezn.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rjp.wangdashe.top

[R17] 数组定义与取值
来源：http://oph.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gyf.quarkkingdee.top

[R18] 遍历数组
来源：http://clc.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gho.yanxiufei.cn

[R19] 数组长度
来源：http://lri.0kj1m.cn

echo "${#arr[@]}"
来源：http://voo.mhx1999.top

[R20] 关联数组（字典）
来源：http://lsm.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fmb.xylfe.cn

[R21] 字符串长度
来源：http://hbg.ybcxt.top

echo "${#s}"
来源：http://pul.nwbrower.top

[R22] 截取子串
来源：http://fmd.xylfe.cn

echo "${s:0:5}"
来源：http://hec.nanxuanxn.top

[R23] 字符串替换
来源：http://aje.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gim.nanxinkj.top

[R24] 大小写转换
来源：http://fwi.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://gta.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://xty.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lqh.nwbrower.top

[R26] 命令替换
来源：http://xvp.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://zda.yj20258.top

[R27] 算术展开
来源：http://mgk.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://zcx.yangfankeji.com

[R28] 浮点运算
来源：http://ibx.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://uxe.fzhhl.top

[R29] 定义函数
来源：http://gjr.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://reg.jianghu66.top

[R30] 函数返回状态码
来源：http://utf.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://qnn.hammf.cn

[R31] 局部变量
来源：http://hov.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://kvn.wangdashe.top

[R32] 参数个数校验
来源：http://igy.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://srs.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://nbh.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnm.yj202588.top

[R34] 退出时清理
来源：http://vve.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://pwa.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://ebw.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tvi.wangdashe.top

[R36] 并发执行多个任务
来源：http://iwt.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mlb.shzxlz.cn

[R37] 把输出赋给变量
来源：http://nwz.tarul.cn

files=$(ls -1)
来源：http://xbh.guowangkeji.top

[R38] 管道串联
来源：http://cnf.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://fpc.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://wnr.yueranfly.top

cmd > out.log 2>&1
来源：http://tjl.kuanghao11.cn

[R40] 追加写日志
来源：http://hvb.hesvh.cn

echo "log" >> out.log
来源：http://baa.9152youxi.cn

[R41] 丢弃输出
来源：http://kax.yj202588.top

cmd >/dev/null 2>&1
来源：http://hwu.316326.xyz

[R42] 输入重定向
来源：http://prz.shzxlz.cn

wc -l < a.txt
来源：http://lov.aizwys.cn

[R43] 按名字查找文件
来源：http://uim.c1oappe.top

find . -name "*.log" -type f
来源：http://zvg.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://lsx.fengsongda.top

find . -mtime -7 -type f
来源：http://vrg.cucudq.cn

[R45] 批量删除
来源：http://dxa.sxryk.cn

find . -name "*.tmp" -delete
来源：http://iin.fehbvm.com

[R46] 递归替换文件内容
来源：http://rou.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wjq.jqgufenzy.top

[R47] sed 单行替换
来源：http://ikv.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kbm.zdbjq.cn

[R48] awk 取指定列
来源：http://evn.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://zfk.ydzc1.top

[R49] awk 带条件
来源：http://tmf.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cpq.haohaochexian.top

[R50] awk 求和
来源：http://dkx.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://fjv.xylfe.cn

[R51] 排序去重取前几
来源：http://nhx.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qsi.fktsv.cn

[R52] 统计行数
来源：http://too.c1oappe.top

wc -l a.txt
来源：http://vvo.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://ejs.ybcxt.top


<!-- 参考信息 -->