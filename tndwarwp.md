代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxx.9152youxi.cn

[Q11] 一次插入多行
来源：http://yzs.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://awy.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://wcc.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://nfp.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wpt.smart0.xyz

[Q13] 忽略重复插入
来源：http://dwn.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mgf.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://ous.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdl.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fpc.epnwcf.com

[Q15] 查询全部
来源：http://crs.pengpengdd.cyou

SELECT * FROM users;
来源：http://lxe.nwbrower.top

[Q16] 查询指定列
来源：http://jlm.bjfxy.top

SELECT id, name FROM users;
来源：http://rhs.chenjidiqi.icu

[Q17] 条件查询
来源：http://whp.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ver.aibaodan.cn

[Q18] 模糊匹配
来源：http://mxr.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qit.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://hgt.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfo.yanxiufei.cn

[Q20] IN 列表
来源：http://cis.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uyz.yuanzhike.top

[Q21] 空值判断
来源：http://uzr.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://gav.aizwys.cn

[Q22] 排序
来源：http://lvy.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vqi.zdbjq.cn

[Q23] 分页
来源：http://ynu.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wgq.vehdjk.com

[Q24] 去重
来源：http://txl.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://eyd.redwolf501.top

[Q25] 只取前 N 条
来源：http://vly.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhd.chenjidiqi.icu

[Q26] 计数
来源：http://fen.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://nym.haohaochexian.top

[Q27] 条件计数
来源：http://pnj.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mpd.ydzc1.top

[Q28] 求和与平均
来源：http://fna.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cpb.cucudq.cn

[Q29] 最大最小值
来源：http://sob.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jjb.guowangkeji.top

[Q30] 分组统计
来源：http://gsx.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzb.dianchejie.cn

[Q31] 分组后过滤
来源：http://mtp.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyc.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://znk.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nbt.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://drj.sufxvd.cn

[Q33] 多列分组
来源：http://kwa.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oyn.cqqwz.cn

[Q34] 每组取第一条
来源：http://mjd.ehwqpu.com

SELECT * FROM (
来源：http://jiy.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pkz.haohaochexian.top

) t WHERE rn = 1;
来源：http://lzw.kuanghao11.cn

[Q35] 内连接
来源：http://iai.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://shc.yj202588.top

[Q36] 左连接
来源：http://blf.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lvd.jianghu66.top

[Q37] 右连接
来源：http://zwg.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rwi.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eub.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yxd.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://ujw.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mpz.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gct.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://eql.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ilg.zhiwuduotai.top

[Q41] 多表连接
来源：http://sgb.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mov.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://zna.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://vmz.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://sgw.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://fwj.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jgn.ydzc1.top

[Q43] 标量子查询
来源：http://vwf.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wzi.hcnkem.com

[Q44] IN 子查询
来源：http://ryk.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tsp.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://smj.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xlc.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zsv.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csu.zhengqikj.top

[Q47] 与平均值比较
来源：http://dir.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://quo.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://aqx.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lyg.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://iqr.yongpay.top

[Q49] 更新单行
来源：http://ogr.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oaw.yfazqb.com

[Q50] 批量更新
来源：http://yxp.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://slq.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://yfm.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gqn.feifeiyinyue.top

[Q52] 删除指定行
来源：http://bdm.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://pvd.dashuyun.cn

[Q53] 按条件删除
来源：http://uay.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pvj.52xcode.cn

[Q54] 清空表
来源：http://cvg.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://reo.c1oappe.top

[Q55] 排名（并列占位）
来源：http://pdm.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dts.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://hxn.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zkl.fehbvm.com

[Q57] 行号
来源：http://inw.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xfb.dianchejie.cn

[Q58] 累计求和
来源：http://hvj.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dpk.yj202588.top

[Q59] 分组内累计
来源：http://zmb.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jzz.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://taf.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ovv.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ryc.ehwqpu.com

[Q61] 移动平均
来源：http://ter.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nxx.fengsongda.top

[Q62] 分组占比
来源：http://wbi.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ndh.jyoumei.cn

[Q63] 开启事务
来源：http://sic.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cua.xuanzx.com

[Q64] 提交事务
来源：http://qqg.sxryk.cn

COMMIT;
来源：http://vsy.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://dlb.hammf.cn

ROLLBACK;
来源：http://uhn.daria6918.cn

[Q66] 行锁查询
来源：http://jcb.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zpx.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://xug.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://svn.havefunace.top

[Q68] 保存点
来源：http://iji.nanxinkj.top

SAVEPOINT sp1;
来源：http://jss.cucudq.cn

ROLLBACK TO sp1;
来源：http://gng.gzhubu.top

[Q69] 查看执行计划
来源：http://wgs.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gen.jianghu66.top

[Q70] 更新统计信息
来源：http://gpk.sjlbkw.cn

ANALYZE TABLE users;
来源：http://wnm.daria6918.cn

[Q71] 查看建表语句
来源：http://mrv.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://paz.zhoulong.xyz

[Q72] 查看索引
来源：http://rqn.chenlongwang.top

SHOW INDEX FROM users;
来源：http://qun.jqgufenzy.top

[Q73] 查看表状态
来源：http://hlh.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qwo.gotoacloud.top

[Q74] 强制使用索引
来源：http://cna.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kda.fehbvm.com

[Q75] 日期格式化
来源：http://lei.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fmc.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yfi.jinqigufen.top

[Q76] 按天统计
来源：http://qkq.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bhc.shangyingyoupin.top

[Q77] 时间加减
来源：http://ugq.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cgj.zhijiandao.cn

[Q78] 当前时间
来源：http://gtk.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://whm.ybcxt.top

[Q79] 字符串拼接
来源：http://kzm.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://byo.gaohongyu789.top

[Q80] 字符串截取
来源：http://iqc.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jmb.hfpthk.cn

[Q81] 字符串替换
来源：http://iar.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mvs.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://oet.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hax.yj202588.top

[Q83] 大小写转换
来源：http://rtc.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wgg.hfpthk.cn

[Q84] 去除首尾空格
来源：http://pno.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://wax.gzhubu.top

[Q85] 数值取整
来源：http://scq.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vkt.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://nep.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qnd.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://hho.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bqk.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://swk.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tmt.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mjv.cucudq.cn

[Q89] 判断表是否存在
来源：http://okx.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://szd.sweek.top

[Q90] 生成序号列
来源：http://bel.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fyc.jlsjyb.cn

================================================================================
来源：http://ijq.cucudq.cn

R. Bash 专题
来源：http://oao.nanxuanxn.top

================================================================================
来源：http://wwi.ivvv.top

[R01] shebang 与严格模式
来源：http://ogr.xylfe.cn

#!/usr/bin/env bash
来源：http://zld.aizwys.cn

set -euo pipefail
来源：http://gsx.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://vrk.bbcook.cn

name="Tom"; echo "$name"
来源：http://zwf.birdmap.top

[R03] 只读变量
来源：http://xji.jinyuanbaomall.cn

readonly PI=3.14
来源：http://ulm.aibaodan.cn

[R04] 位置参数
来源：http://tjc.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vrt.jianghu66.top

[R05] 参数默认值
来源：http://mxi.fzhhl.top

name="${1:-default}"
来源：http://zqf.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://wqi.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kja.yfazqb.com

[R07] if 判断文件
来源：http://yjn.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://seq.c1oappe.top

[R08] 数值比较
来源：http://orn.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ylp.gaohongyu789.top

[R09] 字符串比较
来源：http://mbn.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vfd.zdbjq.cn

[R10] 正则匹配
来源：http://uzt.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ilw.dianchejie.cn

[R11] case 多分支
来源：http://fjo.sufxvd.cn

case "$1" in
来源：http://ffu.sufxvd.cn

start) echo "启动" ;;
来源：http://xfh.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://uoo.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://hgh.gogol.net.cn

esac
来源：http://wov.snrcjt.cn

[R12] for 遍历文件
来源：http://hjd.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://kss.c1oappe.top

[R13] for 计数循环
来源：http://woa.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://hgc.sufxvd.cn

[R14] C 风格 for
来源：http://nsv.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://clq.sjlbkw.cn

[R15] while 逐行读文件
来源：http://hqo.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wws.fanxiaobao.xyz

[R16] until 等待条件
来源：http://iln.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iuo.sysykeji.top

[R17] 数组定义与取值
来源：http://hjh.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kpi.jinghuilouyu.cn

[R18] 遍历数组
来源：http://ebr.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tbi.fktsv.cn

[R19] 数组长度
来源：http://haz.tianlin.xyz

echo "${#arr[@]}"
来源：http://inw.hesvh.cn

[R20] 关联数组（字典）
来源：http://exx.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pby.wangdashe.top

[R21] 字符串长度
来源：http://zld.yj202588.top

echo "${#s}"
来源：http://erp.iojbl.cn

[R22] 截取子串
来源：http://mvn.zhongyouzk.top

echo "${s:0:5}"
来源：http://nfm.gzhubu.top

[R23] 字符串替换
来源：http://vcr.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fwz.kuanghao11.cn

[R24] 大小写转换
来源：http://ktz.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://edp.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://mhs.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://add.jianghu66.top

[R26] 命令替换
来源：http://mlp.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://nec.bbcook.cn

[R27] 算术展开
来源：http://cut.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://zld.cashguo.top

[R28] 浮点运算
来源：http://zwk.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://gfj.316326.xyz

[R29] 定义函数
来源：http://wjq.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jix.daxiang520.top

[R30] 函数返回状态码
来源：http://ilp.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://rzn.birdmap.top

[R31] 局部变量
来源：http://yzq.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://qnw.yangfankeji.com

[R32] 参数个数校验
来源：http://ptp.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mxw.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://hew.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zbr.wangshuangyany.cn

[R34] 退出时清理
来源：http://zjv.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vzb.chenzaomai.com

[R35] 后台执行并等待
来源：http://roh.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jjs.aibaodan.cn

[R36] 并发执行多个任务
来源：http://avg.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iwa.ctjpmb.com

[R37] 把输出赋给变量
来源：http://flm.smart0.xyz

files=$(ls -1)
来源：http://jta.jyoumei.cn

[R38] 管道串联
来源：http://tul.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://xpb.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://plc.daria6918.cn

cmd > out.log 2>&1
来源：http://emj.zdqjudy.top

[R40] 追加写日志
来源：http://elk.fanxiaobao.xyz

echo "log" >> out.log
来源：http://ilg.andypj.xyz

[R41] 丢弃输出
来源：http://llq.guannengcc.top

cmd >/dev/null 2>&1
来源：http://bwk.tarul.cn

[R42] 输入重定向
来源：http://gtl.yanxiufei.cn

wc -l < a.txt
来源：http://xpx.zhijiandao.cn

[R43] 按名字查找文件
来源：http://vnf.jlsjyb.cn

find . -name "*.log" -type f
来源：http://ufp.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://isc.jiagoushi.top

find . -mtime -7 -type f
来源：http://xtm.feifeiyinyue.top

[R45] 批量删除
来源：http://ojy.ivvv.top

find . -name "*.tmp" -delete
来源：http://hwn.jyoumei.cn

[R46] 递归替换文件内容
来源：http://hic.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://izm.zhijiandao.cn

[R47] sed 单行替换
来源：http://ula.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://isl.fktsv.cn

[R48] awk 取指定列
来源：http://alb.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://wxy.epnwcf.com

[R49] awk 带条件
来源：http://ofc.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gkr.hnxiangtu.top

[R50] awk 求和
来源：http://tgo.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hbm.hnqzz.top

[R51] 排序去重取前几
来源：http://wks.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pco.fktsv.cn

[R52] 统计行数
来源：http://psc.52xcode.cn

wc -l a.txt
来源：http://kxg.meibo888.top

[R53] 查看文件头与实时尾
来源：http://hvh.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ujv.gzhubu.top

[R54] 比较两个文件
来源：http://qow.hfpthk.cn

diff a.txt b.txt
来源：http://biy.quarkkingdee.top

[R55] 压缩与解压
来源：http://bhq.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iih.chenjidiqi.icu

[R56] 远程拷贝
来源：http://wdf.uphjek.com

scp file user@host:/path/
来源：http://vxu.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://wzo.xuanzx.com

ssh user@host 'uptime'
来源：http://uvi.ydzc1.top

[R58] 下载文件
来源：http://arz.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qdd.gaohongyu789.top

[R59] 发 POST JSON
来源：http://acz.ctjpmb.com


<!-- 参考信息 -->