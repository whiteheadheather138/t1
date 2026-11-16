代发 wailian999

);
来源：http://kcq.yueranfly.top

[Q03] 增加列
来源：http://dyp.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pkn.jianghu66.top

[Q04] 修改列类型
来源：http://ehd.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aep.birdmap.top

[Q05] 重命名列
来源：http://nsq.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mvc.hnqzz.top

[Q06] 删除列
来源：http://rvd.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://mmn.daria6918.cn

[Q07] 删除表
来源：http://svf.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://wpd.gotoacloud.top

[Q08] 创建普通索引
来源：http://jot.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ocx.0kj1m.cn

[Q09] 创建唯一索引
来源：http://qrj.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bno.hongshengwenyu.top

[Q10] 插入单行
来源：http://llj.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fhe.sjlbkw.cn

[Q11] 一次插入多行
来源：http://jxd.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pyu.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://wfq.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bdm.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uti.gzhubu.top

[Q13] 忽略重复插入
来源：http://uyv.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mcs.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://hvn.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://exm.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yun.daxiang520.top

[Q15] 查询全部
来源：http://tns.yj202588.top

SELECT * FROM users;
来源：http://jhf.mhx1999.top

[Q16] 查询指定列
来源：http://yld.gaohongyu789.top

SELECT id, name FROM users;
来源：http://vve.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://hsg.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ffb.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://fpk.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ffg.wangdashe.top

[Q19] 范围查询
来源：http://vyj.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xlb.guowangkeji.top

[Q20] IN 列表
来源：http://jgy.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uwe.vehdjk.com

[Q21] 空值判断
来源：http://jmz.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mky.redwolf501.top

[Q22] 排序
来源：http://vhh.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eij.zhongyouzk.top

[Q23] 分页
来源：http://izh.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aoo.aibaodan.cn

[Q24] 去重
来源：http://gqi.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://bwq.fktsv.cn

[Q25] 只取前 N 条
来源：http://qdq.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hqs.jinghuilouyu.cn

[Q26] 计数
来源：http://uxs.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://vzc.meibo888.top

[Q27] 条件计数
来源：http://ehy.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ytm.yuanzhike.top

[Q28] 求和与平均
来源：http://fpr.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ndt.cucudq.cn

[Q29] 最大最小值
来源：http://klp.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mri.cashguo.top

[Q30] 分组统计
来源：http://vur.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vxc.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://pmu.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpk.birdmap.top

[Q32] 分组拼接字符串
来源：http://unt.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hyr.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qjb.hfpthk.cn

[Q33] 多列分组
来源：http://tpd.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xzv.wangdashe.top

[Q34] 每组取第一条
来源：http://tom.hnxiangtu.top

SELECT * FROM (
来源：http://kuu.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qxx.cheryme.top

) t WHERE rn = 1;
来源：http://hxy.jianghu66.top

[Q35] 内连接
来源：http://asu.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://reh.yvedp.cn

[Q36] 左连接
来源：http://fnr.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbi.yfazqb.com

[Q37] 右连接
来源：http://wcy.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tge.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://sbr.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://stp.yj20258.top

[Q39] 自连接（查上下级）
来源：http://oqz.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kll.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jxn.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dco.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ldv.quarkkingdee.top

[Q41] 多表连接
来源：http://sfn.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lhu.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://hgm.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://ngp.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://xxz.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://gui.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://npc.xylfe.cn

[Q43] 标量子查询
来源：http://kgp.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vbu.zhoulong.xyz

[Q44] IN 子查询
来源：http://hip.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hwy.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://vpm.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://noo.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://wft.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ere.snrcjt.cn

[Q47] 与平均值比较
来源：http://war.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wad.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://olk.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dzf.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://gob.gaohongyu789.top

[Q49] 更新单行
来源：http://sqv.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://upv.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://hsc.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vpl.chenzaomai.com

[Q51] 用子查询更新
来源：http://eht.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lzz.hcnkem.com

[Q52] 删除指定行
来源：http://box.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://ldv.zdqjudy.top

[Q53] 按条件删除
来源：http://zfr.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jex.yj20258888.top

[Q54] 清空表
来源：http://lpx.vehdjk.com

TRUNCATE TABLE logs;
来源：http://rxy.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://ogh.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ofu.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://bnw.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://coe.haohaochexian.top

[Q57] 行号
来源：http://blm.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fkt.zhijiandao.cn

[Q58] 累计求和
来源：http://zcy.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://imf.ydjk.org.cn

[Q59] 分组内累计
来源：http://ddo.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://huf.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://uef.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://osv.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kqf.snrcjt.cn

[Q61] 移动平均
来源：http://ezd.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ezc.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://kzk.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dhd.sxryk.cn

[Q63] 开启事务
来源：http://kqt.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gqh.ybcxt.top

[Q64] 提交事务
来源：http://php.tarul.cn

COMMIT;
来源：http://cqs.hnxiangtu.top

[Q65] 回滚事务
来源：http://dkj.xuetiantiany.cn

ROLLBACK;
来源：http://yie.chenjidiqi.icu

[Q66] 行锁查询
来源：http://aze.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hyr.daxiang520.top

[Q67] 设置隔离级别
来源：http://ulg.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nhx.zhixingplan.top

[Q68] 保存点
来源：http://nns.tanke756.top

SAVEPOINT sp1;
来源：http://ovv.tanke756.top

ROLLBACK TO sp1;
来源：http://ciq.chenlongwang.top

[Q69] 查看执行计划
来源：http://vky.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tve.epnwcf.com

[Q70] 更新统计信息
来源：http://rjg.tarul.cn

ANALYZE TABLE users;
来源：http://abv.pycfn.com

[Q71] 查看建表语句
来源：http://erq.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cct.chenjidiqi.icu

[Q72] 查看索引
来源：http://yqv.iojbl.cn

SHOW INDEX FROM users;
来源：http://qug.cdnleiting.top

[Q73] 查看表状态
来源：http://gjx.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zgb.havefunace.top

[Q74] 强制使用索引
来源：http://gym.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rqt.iojbl.cn

[Q75] 日期格式化
来源：http://vei.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cwi.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kek.pengpengdd.cyou

[Q76] 按天统计
来源：http://igo.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bre.feifeiyinyue.top

[Q77] 时间加减
来源：http://kcu.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://orp.gogol.net.cn

[Q78] 当前时间
来源：http://vwj.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lpn.cqqwz.cn

[Q79] 字符串拼接
来源：http://nec.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zya.sxryk.cn

[Q80] 字符串截取
来源：http://hsn.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yph.nanxuanxn.top

[Q81] 字符串替换
来源：http://slx.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kcn.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://ifi.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zld.feifeiyinyue.top

[Q83] 大小写转换
来源：http://cuq.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://btq.zhixingplan.top

[Q84] 去除首尾空格
来源：http://jeg.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://qlb.bjfxy.top

[Q85] 数值取整
来源：http://crb.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.sweek.top

[Q86] 读取 JSON 字段
来源：http://poi.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://txl.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://taj.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gwg.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://xpo.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nfs.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bjk.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://rte.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mgj.zhixingplan.top

[Q90] 生成序号列
来源：http://iek.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hdd.aibaodan.cn

================================================================================
来源：http://vpu.xylfe.cn

R. Bash 专题
来源：http://ejn.yfazqb.com

================================================================================
来源：http://iwu.xylfe.cn

[R01] shebang 与严格模式
来源：http://akb.yj20258.top

#!/usr/bin/env bash
来源：http://xnn.jqgufenzy.top

set -euo pipefail
来源：http://foo.gogol.net.cn

[R02] 变量赋值与使用
来源：http://uie.meibo888.top

name="Tom"; echo "$name"
来源：http://qdm.pengpengdd.cyou

[R03] 只读变量
来源：http://xgi.chenlongwang.top

readonly PI=3.14
来源：http://qnf.andypj.xyz

[R04] 位置参数
来源：http://xnh.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xgs.nanxinkj.top

[R05] 参数默认值
来源：http://chn.daxiang520.top

name="${1:-default}"
来源：http://kji.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://kfr.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hgi.hesvh.cn

[R07] if 判断文件
来源：http://hjh.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kfs.shzxlz.cn

[R08] 数值比较
来源：http://ngb.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pmx.yangfankeji.com

[R09] 字符串比较
来源：http://kdo.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oyr.yj20258.top

[R10] 正则匹配
来源：http://ger.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ksp.jiagoushi.top

[R11] case 多分支
来源：http://itw.jqgufenzy.top

case "$1" in
来源：http://qzm.bbcook.cn

start) echo "启动" ;;
来源：http://waf.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://fjt.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://vhk.cashguo.top

esac
来源：http://eyy.tanke756.top

[R12] for 遍历文件
来源：http://cts.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://ntc.c1oappe.top

[R13] for 计数循环
来源：http://bai.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://tgg.sweek.top

[R14] C 风格 for
来源：http://owk.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dbu.tanke756.top

[R15] while 逐行读文件
来源：http://rvj.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bpv.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://rts.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdz.fzhhl.top

[R17] 数组定义与取值
来源：http://qlf.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://qcg.c1oappe.top

[R18] 遍历数组
来源：http://hcb.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://glq.c1oappe.top

[R19] 数组长度
来源：http://boz.shzxlz.cn

echo "${#arr[@]}"
来源：http://vnl.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://svr.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gjc.sufxvd.cn

[R21] 字符串长度
来源：http://zch.xuetiantiany.cn

echo "${#s}"
来源：http://cjo.hfpthk.cn

[R22] 截取子串
来源：http://wgw.shzxlz.cn

echo "${s:0:5}"
来源：http://ejk.hongshengwenyu.top

[R23] 字符串替换
来源：http://zgs.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iol.jianghu66.top

[R24] 大小写转换
来源：http://ozm.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://cxr.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://jgo.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xfs.uphjek.com

[R26] 命令替换
来源：http://qqh.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://zgp.wangshuangyany.cn

[R27] 算术展开
来源：http://ibs.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://qxj.zhongyouzk.top

[R28] 浮点运算
来源：http://dvi.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://ihx.tian-w.cn

[R29] 定义函数
来源：http://vce.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cex.aizwys.cn

[R30] 函数返回状态码
来源：http://xvl.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://nrz.epnwcf.com

[R31] 局部变量
来源：http://mbh.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://gzs.yj20258888.top

[R32] 参数个数校验
来源：http://qiz.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eye.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://cqm.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zyz.cqqwz.cn

[R34] 退出时清理
来源：http://rqx.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://aas.ctjpmb.com

[R35] 后台执行并等待
来源：http://vye.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vrk.jianghu66.top

[R36] 并发执行多个任务
来源：http://mwh.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhe.hnqzz.top

[R37] 把输出赋给变量
来源：http://gas.vehdjk.com

files=$(ls -1)
来源：http://ksl.fanxiaobao.xyz

[R38] 管道串联
来源：http://uhk.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://cou.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://eeu.zhoulong.xyz

cmd > out.log 2>&1
来源：http://daz.shuidangran.top

[R40] 追加写日志
来源：http://gdy.tanke756.top

echo "log" >> out.log
来源：http://hqd.cashguo.top

[R41] 丢弃输出
来源：http://igq.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://lyr.birdmap.top

[R42] 输入重定向
来源：http://cue.xuetiantiany.cn

wc -l < a.txt
来源：http://maj.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://ryk.yangfankeji.com

find . -name "*.log" -type f
来源：http://uux.fzhhl.top

[R44] 按修改时间查找
来源：http://rss.nwbrower.top

find . -mtime -7 -type f
来源：http://peh.redwolf501.top

[R45] 批量删除
来源：http://rsm.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://vqx.sufxvd.cn

[R46] 递归替换文件内容
来源：http://qzk.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bob.zdbjq.cn

[R47] sed 单行替换
来源：http://rrm.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://jae.cdnleiting.top

[R48] awk 取指定列
来源：http://sqr.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://tfm.pengpengdd.cyou

[R49] awk 带条件
来源：http://sdl.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fsp.sysykeji.top

[R50] awk 求和
来源：http://tto.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://zaq.yuxming.cn

[R51] 排序去重取前几
来源：http://lmh.epnwcf.com


<!-- 参考信息 -->