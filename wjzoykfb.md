代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://pbc.shzxlz.cn

[Q07] 删除表
来源：http://fsr.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://bos.vqdsnc.cn

[Q08] 创建普通索引
来源：http://edf.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tah.guowangkeji.top

[Q09] 创建唯一索引
来源：http://bgi.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hrm.dashuyun.cn

[Q10] 插入单行
来源：http://qjy.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uom.ppjwa.cn

[Q11] 一次插入多行
来源：http://fxd.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://edh.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://elm.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://dwd.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fia.cqqwz.cn

[Q13] 忽略重复插入
来源：http://lqf.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uab.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://rrk.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mcg.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vvt.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://nfr.epnwcf.com

SELECT * FROM users;
来源：http://rxc.yangfankeji.com

[Q16] 查询指定列
来源：http://gjb.zdqjudy.top

SELECT id, name FROM users;
来源：http://yxf.yvedp.cn

[Q17] 条件查询
来源：http://fvf.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jxt.c1oappe.top

[Q18] 模糊匹配
来源：http://azw.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://agr.hysaishi.cn

[Q19] 范围查询
来源：http://imh.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tva.9152youxi.cn

[Q20] IN 列表
来源：http://abv.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://puv.smart0.xyz

[Q21] 空值判断
来源：http://ote.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bcz.aizwys.cn

[Q22] 排序
来源：http://wjj.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xbu.vqdsnc.cn

[Q23] 分页
来源：http://ebv.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axx.yonumen.top

[Q24] 去重
来源：http://xhh.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://ctv.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://cpj.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ntn.cheryme.top

[Q26] 计数
来源：http://tvf.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://vvz.jqgfzy.top

[Q27] 条件计数
来源：http://kka.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sds.c1oappe.top

[Q28] 求和与平均
来源：http://nci.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rjp.jlsjyb.cn

[Q29] 最大最小值
来源：http://epr.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jeg.yonumen.top

[Q30] 分组统计
来源：http://djn.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ixz.xziqi.cn

[Q31] 分组后过滤
来源：http://rld.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jgg.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://vcv.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vnl.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qlm.birdmap.top

[Q33] 多列分组
来源：http://zdf.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ghh.guannengcc.top

[Q34] 每组取第一条
来源：http://yej.chenlongwang.top

SELECT * FROM (
来源：http://cig.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://igl.haohaochexian.top

) t WHERE rn = 1;
来源：http://umo.tian-w.cn

[Q35] 内连接
来源：http://pwy.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bao.yueranfly.top

[Q36] 左连接
来源：http://lef.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zgm.yfazqb.com

[Q37] 右连接
来源：http://ojg.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ghu.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vgz.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ift.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://abf.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dyc.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hfa.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fwc.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hou.yanxiufei.cn

[Q41] 多表连接
来源：http://jbk.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ijt.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://uom.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://wlf.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://xvr.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://gxm.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rxs.sjlbkw.cn

[Q43] 标量子查询
来源：http://gkj.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hmx.hammf.cn

[Q44] IN 子查询
来源：http://scp.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqk.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://ixm.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qks.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://meu.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bjl.haohaochexian.top

[Q47] 与平均值比较
来源：http://xbp.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mkp.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://lqx.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vsx.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://pif.uphjek.com

[Q49] 更新单行
来源：http://aaz.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uhg.yuxming.cn

[Q50] 批量更新
来源：http://nbe.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xav.tanke756.top

[Q51] 用子查询更新
来源：http://hcb.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wvj.yfazqb.com

[Q52] 删除指定行
来源：http://jjf.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://dhr.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://pfj.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tqp.iojbl.cn

[Q54] 清空表
来源：http://chu.tian-w.cn

TRUNCATE TABLE logs;
来源：http://lmd.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://rtz.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dyv.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://vxf.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cxy.ydzc1.top

[Q57] 行号
来源：http://gtm.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zpr.sysykeji.top

[Q58] 累计求和
来源：http://bcg.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://twg.xuetiantiany.cn

[Q59] 分组内累计
来源：http://ifg.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvj.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://uwi.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ssm.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ipr.hesvh.cn

[Q61] 移动平均
来源：http://xod.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ylz.guowangkeji.top

[Q62] 分组占比
来源：http://viw.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://euk.epnwcf.com

[Q63] 开启事务
来源：http://ypt.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ffw.smart0.xyz

[Q64] 提交事务
来源：http://muj.hcnkem.com

COMMIT;
来源：http://mnw.yj20258888.top

[Q65] 回滚事务
来源：http://oiv.bjfxy.top

ROLLBACK;
来源：http://itc.zhijiandao.cn

[Q66] 行锁查询
来源：http://cfo.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eig.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://zgi.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pkf.chenlongwang.top

[Q68] 保存点
来源：http://euc.sxryk.cn

SAVEPOINT sp1;
来源：http://gyn.cheryme.top

ROLLBACK TO sp1;
来源：http://zmv.zhengqikj.top

[Q69] 查看执行计划
来源：http://xia.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qxg.jiagoushi.top

[Q70] 更新统计信息
来源：http://fem.yvedp.cn

ANALYZE TABLE users;
来源：http://nwq.gaohongyu789.top

[Q71] 查看建表语句
来源：http://vtk.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://udv.redwolf501.top

[Q72] 查看索引
来源：http://efd.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://dnv.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://blx.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://syb.yj20258888.top

[Q74] 强制使用索引
来源：http://yli.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sqx.hongshengwenyu.top

[Q75] 日期格式化
来源：http://ydf.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vqa.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cmr.jinqigfzy.top

[Q76] 按天统计
来源：http://vcq.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rhy.fanxiaobao.xyz

[Q77] 时间加减
来源：http://gmi.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fsd.aizwys.cn

[Q78] 当前时间
来源：http://iwt.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ozh.jinqigufen.top

[Q79] 字符串拼接
来源：http://fbb.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://brv.ydzc1.top

[Q80] 字符串截取
来源：http://jpz.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dsq.vqdsnc.cn

[Q81] 字符串替换
来源：http://jjj.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cwf.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://eqh.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://shi.cheryme.top

[Q83] 大小写转换
来源：http://fva.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kci.yfazqb.com

[Q84] 去除首尾空格
来源：http://rxj.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://gda.xziqi.cn

[Q85] 数值取整
来源：http://cqi.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wqx.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://xkj.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://djj.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://kji.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kio.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://rzn.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zax.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kca.sxryk.cn

[Q89] 判断表是否存在
来源：http://atl.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fdm.yongpay.top

[Q90] 生成序号列
来源：http://rna.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vbg.fehbvm.com

================================================================================
来源：http://ouz.yvedp.cn

R. Bash 专题
来源：http://olp.zhongyouzk.top

================================================================================
来源：http://qqe.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://bff.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://ncd.zhiwuduotai.top

set -euo pipefail
来源：http://mlt.chenlongwang.top

[R02] 变量赋值与使用
来源：http://rjy.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://whp.birdmap.top

[R03] 只读变量
来源：http://bmy.jinyuanbaomall.cn

readonly PI=3.14
来源：http://etg.dashuyun.cn

[R04] 位置参数
来源：http://gbe.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dxj.c1oappe.top

[R05] 参数默认值
来源：http://ced.hfpthk.cn

name="${1:-default}"
来源：http://bcw.hcnkem.com

[R06] 判断命令是否存在
来源：http://vom.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tcy.ppjwa.cn

[R07] if 判断文件
来源：http://xyq.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qpq.hnxiangtu.top

[R08] 数值比较
来源：http://evb.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xxb.jqgufenzy.top

[R09] 字符串比较
来源：http://zwg.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mwe.yuxming.cn

[R10] 正则匹配
来源：http://coh.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://itt.yanxiufei.cn

[R11] case 多分支
来源：http://vih.tianlin.xyz

case "$1" in
来源：http://epq.sufxvd.cn

start) echo "启动" ;;
来源：http://ozf.hfpthk.cn

stop)  echo "停止" ;;
来源：http://bqy.pycfn.com

*)     echo "未知命令" ;;
来源：http://vfa.zhoulong.xyz

esac
来源：http://cvo.hcnkem.com

[R12] for 遍历文件
来源：http://avk.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://nhy.cdnleiting.top

[R13] for 计数循环
来源：http://oes.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://med.yvedp.cn

[R14] C 风格 for
来源：http://wzp.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pbh.quarkkingdee.top

[R15] while 逐行读文件
来源：http://jxq.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://anh.feifeiyinyue.top

[R16] until 等待条件
来源：http://bos.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uow.zdqjudy.top

[R17] 数组定义与取值
来源：http://tbu.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://izw.hammf.cn

[R18] 遍历数组
来源：http://wxl.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dfk.zhijiandao.cn

[R19] 数组长度
来源：http://egz.tian-w.cn

echo "${#arr[@]}"
来源：http://bhg.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://ayn.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkz.yanxiufei.cn

[R21] 字符串长度
来源：http://tqh.yuxming.cn

echo "${#s}"
来源：http://jmu.xinyue.icu

[R22] 截取子串
来源：http://qfi.sufxvd.cn

echo "${s:0:5}"
来源：http://gct.fzhhl.top

[R23] 字符串替换
来源：http://qmt.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gqe.nanxuanxn.top

[R24] 大小写转换
来源：http://umv.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://szs.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://cte.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uaq.epnwcf.com

[R26] 命令替换
来源：http://edf.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://siy.tian-w.cn

[R27] 算术展开
来源：http://psc.hesvh.cn

echo $((1 + 2 * 3))
来源：http://czd.jianghu66.top

[R28] 浮点运算
来源：http://agh.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://gjl.vehdjk.com

[R29] 定义函数
来源：http://zxm.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pub.hnxiangtu.top

[R30] 函数返回状态码
来源：http://tlv.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://tpc.nwbrower.top

[R31] 局部变量
来源：http://wxu.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://lyk.ydjk.org.cn

[R32] 参数个数校验
来源：http://scx.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ekx.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://qpe.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kyq.ydjk.org.cn

[R34] 退出时清理
来源：http://acq.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://cbf.birdmap.top

[R35] 后台执行并等待
来源：http://tjp.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ehg.gogol.net.cn

[R36] 并发执行多个任务
来源：http://lkf.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rkm.daxiang520.top

[R37] 把输出赋给变量
来源：http://wvv.tian-w.cn

files=$(ls -1)
来源：http://vac.dianchejie.cn

[R38] 管道串联
来源：http://bfz.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://irb.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://fnv.quarkkingdee.top

cmd > out.log 2>&1
来源：http://qca.xinyue.icu

[R40] 追加写日志
来源：http://bfe.yfazqb.com

echo "log" >> out.log
来源：http://egh.nanxinkj.top

[R41] 丢弃输出
来源：http://uvd.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://kyt.ybcxt.top

[R42] 输入重定向
来源：http://cdy.xuanzx.com

wc -l < a.txt
来源：http://jrm.tanke756.top

[R43] 按名字查找文件
来源：http://ufx.xylfe.cn

find . -name "*.log" -type f
来源：http://qik.tarul.cn

[R44] 按修改时间查找
来源：http://mms.316326.xyz

find . -mtime -7 -type f
来源：http://ddi.shuidangran.top

[R45] 批量删除
来源：http://cjl.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://mwk.yvedp.cn

[R46] 递归替换文件内容
来源：http://gnt.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rjc.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://ytn.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rsh.yuxming.cn

[R48] awk 取指定列
来源：http://tkk.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://jkt.tianlin.xyz

[R49] awk 带条件
来源：http://ofg.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xff.shanyushiyangtech.top

[R50] awk 求和
来源：http://gva.xinyue.icu

awk '{s += $2} END {print s}' a.txt
来源：http://roz.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://zuv.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gpg.zhengqikj.top

[R52] 统计行数
来源：http://tam.fzhhl.top

wc -l a.txt
来源：http://vuy.hammf.cn

[R53] 查看文件头与实时尾
来源：http://zas.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wun.sxryk.cn

[R54] 比较两个文件
来源：http://usx.fktsv.cn

diff a.txt b.txt
来源：http://yfi.gogol.net.cn

[R55] 压缩与解压
来源：http://uct.fktsv.cn


<!-- 参考信息 -->