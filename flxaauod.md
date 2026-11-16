代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://swc.haohaochexian.top

[Q07] 删除表
来源：http://lbq.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://yzp.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://uym.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fah.sxryk.cn

[Q09] 创建唯一索引
来源：http://jqt.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vpp.yvedp.cn

[Q10] 插入单行
来源：http://acf.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aod.mhx1999.top

[Q11] 一次插入多行
来源：http://ngj.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ycc.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://vqi.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://blb.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vjc.316326.xyz

[Q13] 忽略重复插入
来源：http://qdu.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ltc.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://fjl.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wjt.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnu.nanxinkj.top

[Q15] 查询全部
来源：http://kik.ctjpmb.com

SELECT * FROM users;
来源：http://dne.pengpengdd.cyou

[Q16] 查询指定列
来源：http://nmr.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://znn.hywenlv.cn

[Q17] 条件查询
来源：http://qsn.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://svq.tian-w.cn

[Q18] 模糊匹配
来源：http://ioj.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ofv.sjlbkw.cn

[Q19] 范围查询
来源：http://alc.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://scb.yj20258888.top

[Q20] IN 列表
来源：http://xkx.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pml.chenjidiqi.icu

[Q21] 空值判断
来源：http://sba.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://anq.jlsjyb.cn

[Q22] 排序
来源：http://zbe.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xrx.pengpengdd.cyou

[Q23] 分页
来源：http://gtf.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jan.yj20258888.top

[Q24] 去重
来源：http://zbw.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://amu.chenzaomai.com

[Q25] 只取前 N 条
来源：http://hjs.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dss.redwolf501.top

[Q26] 计数
来源：http://jav.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://zzb.zdbjq.cn

[Q27] 条件计数
来源：http://oly.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qkx.snrcjt.cn

[Q28] 求和与平均
来源：http://xrw.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ilv.316326.xyz

[Q29] 最大最小值
来源：http://knt.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bgr.pycfn.com

[Q30] 分组统计
来源：http://lgq.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bbd.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://odv.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zlq.fengsongda.top

[Q32] 分组拼接字符串
来源：http://gbr.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://exx.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cqo.shangyingyoupin.top

[Q33] 多列分组
来源：http://kjg.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tgn.yueranfly.top

[Q34] 每组取第一条
来源：http://aws.zhengqikj.top

SELECT * FROM (
来源：http://gqc.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ssv.haohaochexian.top

) t WHERE rn = 1;
来源：http://sno.xuetiantiany.cn

[Q35] 内连接
来源：http://ghb.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://quh.yvedp.cn

[Q36] 左连接
来源：http://dyn.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgs.dianchejie.cn

[Q37] 右连接
来源：http://xti.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ajp.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://gqo.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vbu.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://ecf.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kec.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rdb.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://hdy.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lwe.sufxvd.cn

[Q41] 多表连接
来源：http://sqb.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lta.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://ckm.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://xkz.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://emo.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://hqh.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxi.fehbvm.com

[Q43] 标量子查询
来源：http://bgz.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cvz.sysykeji.top

[Q44] IN 子查询
来源：http://ipz.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xkf.yongpay.top

[Q45] EXISTS 判断存在
来源：http://dbh.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jey.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://nzg.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qce.c1oappe.top

[Q47] 与平均值比较
来源：http://cdx.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://btv.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://zga.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xbn.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://txg.hnqzz.top

[Q49] 更新单行
来源：http://upp.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baz.ctjpmb.com

[Q50] 批量更新
来源：http://dbc.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tqd.vqdsnc.cn

[Q51] 用子查询更新
来源：http://yov.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sqy.andypj.xyz

[Q52] 删除指定行
来源：http://hyb.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ghu.yvedp.cn

[Q53] 按条件删除
来源：http://rhd.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://szj.bjfxy.top

[Q54] 清空表
来源：http://uwb.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://dtp.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://sci.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rpk.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://uii.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wzl.cheryme.top

[Q57] 行号
来源：http://frx.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ftk.tianlin.xyz

[Q58] 累计求和
来源：http://pzk.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uxq.vqdsnc.cn

[Q59] 分组内累计
来源：http://pzu.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wts.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://dmd.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://djg.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvg.yj202588.top

[Q61] 移动平均
来源：http://etm.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ydu.yfazqb.com

[Q62] 分组占比
来源：http://bsv.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://afj.ctjpmb.com

[Q63] 开启事务
来源：http://isq.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sba.daxiang520.top

[Q64] 提交事务
来源：http://ulk.jinqigufen.top

COMMIT;
来源：http://srk.sjlbkw.cn

[Q65] 回滚事务
来源：http://wpe.haohaochexian.top

ROLLBACK;
来源：http://zra.epnwcf.com

[Q66] 行锁查询
来源：http://gzw.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wma.xylfe.cn

[Q67] 设置隔离级别
来源：http://ppj.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tvy.chenzaomai.com

[Q68] 保存点
来源：http://tfu.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://aot.gotoacloud.top

ROLLBACK TO sp1;
来源：http://iuy.sxryk.cn

[Q69] 查看执行计划
来源：http://vdd.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fkv.hesvh.cn

[Q70] 更新统计信息
来源：http://ppa.sweek.top

ANALYZE TABLE users;
来源：http://sho.hesvh.cn

[Q71] 查看建表语句
来源：http://odw.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yks.cqqwz.cn

[Q72] 查看索引
来源：http://gaq.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://buy.yuxming.cn

[Q73] 查看表状态
来源：http://iqe.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sbf.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://uwc.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tgd.guannengcc.top

[Q75] 日期格式化
来源：http://sjq.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uth.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mlj.fanxiaobao.xyz

[Q76] 按天统计
来源：http://ddu.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ccd.hesvh.cn

[Q77] 时间加减
来源：http://nkj.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yhx.zycfv.cn

[Q78] 当前时间
来源：http://mmk.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dur.316326.xyz

[Q79] 字符串拼接
来源：http://tmp.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blb.chenjidiqi.icu

[Q80] 字符串截取
来源：http://mxv.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gye.tianlin.xyz

[Q81] 字符串替换
来源：http://lry.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eqy.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://inl.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xlv.hesvh.cn

[Q83] 大小写转换
来源：http://akr.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dnq.chenlongwang.top

[Q84] 去除首尾空格
来源：http://qhx.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://eev.bjfxy.top

[Q85] 数值取整
来源：http://kde.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kpl.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://qkb.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xqw.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://onk.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://usz.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://xxr.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pmh.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nat.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://zge.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kqb.hammf.cn

[Q90] 生成序号列
来源：http://oub.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfb.yanxiufei.cn

================================================================================
来源：http://cfl.yonumen.top

R. Bash 专题
来源：http://jeh.iojbl.cn

================================================================================
来源：http://zzc.jyoumei.cn

[R01] shebang 与严格模式
来源：http://ffm.fengsongda.top

#!/usr/bin/env bash
来源：http://gwt.zhengqikj.top

set -euo pipefail
来源：http://bmo.yvedp.cn

[R02] 变量赋值与使用
来源：http://lrg.shzxlz.cn

name="Tom"; echo "$name"
来源：http://deo.316326.xyz

[R03] 只读变量
来源：http://xyf.cdnleiting.top

readonly PI=3.14
来源：http://xqk.haohaochexian.top

[R04] 位置参数
来源：http://djt.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://enh.zdqjudy.top

[R05] 参数默认值
来源：http://bmm.tianlin.xyz

name="${1:-default}"
来源：http://xiy.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://tok.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ysj.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://qsr.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nid.9152youxi.cn

[R08] 数值比较
来源：http://fom.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://unh.hnqzz.top

[R09] 字符串比较
来源：http://lfp.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sla.jianghu66.top

[R10] 正则匹配
来源：http://udp.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nia.yuxming.cn

[R11] case 多分支
来源：http://pjn.redwolf501.top

case "$1" in
来源：http://fvk.fktsv.cn

start) echo "启动" ;;
来源：http://jdg.jqgfzy.top

stop)  echo "停止" ;;
来源：http://sgc.shuidangran.top

*)     echo "未知命令" ;;
来源：http://jse.ivvv.top

esac
来源：http://tqr.zhixingplan.top

[R12] for 遍历文件
来源：http://nub.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://mxt.yuxming.cn

[R13] for 计数循环
来源：http://hvj.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://rec.tianlin.xyz

[R14] C 风格 for
来源：http://oay.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hqe.zhoulong.xyz

[R15] while 逐行读文件
来源：http://qux.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wcf.yuanzhike.top

[R16] until 等待条件
来源：http://qbt.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qlq.gaohongyu789.top

[R17] 数组定义与取值
来源：http://zbu.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dvg.ydjk.org.cn

[R18] 遍历数组
来源：http://yrd.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zke.wangshuangyany.cn

[R19] 数组长度
来源：http://zur.bjfxy.top

echo "${#arr[@]}"
来源：http://fkm.jianghu66.top

[R20] 关联数组（字典）
来源：http://mwf.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vuc.cucudq.cn

[R21] 字符串长度
来源：http://iwf.quarkkingdee.top

echo "${#s}"
来源：http://shs.cdnleiting.top

[R22] 截取子串
来源：http://txw.pycfn.com

echo "${s:0:5}"
来源：http://nhp.jqgfzy.top

[R23] 字符串替换
来源：http://zfj.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ghp.nanxuanxn.top

[R24] 大小写转换
来源：http://rfu.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://neo.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://nfg.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rav.sjlbkw.cn

[R26] 命令替换
来源：http://wbu.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://dim.cashguo.top

[R27] 算术展开
来源：http://wan.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://fos.9152youxi.cn

[R28] 浮点运算
来源：http://jhw.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://dfj.wangdashe.top

[R29] 定义函数
来源：http://znk.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ibm.xinyue.icu

[R30] 函数返回状态码
来源：http://xit.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://vki.quarkkingdee.top

[R31] 局部变量
来源：http://srh.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://upa.yuanzhike.top

[R32] 参数个数校验
来源：http://nxs.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jdq.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://cxx.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tdh.chenjidiqi.icu

[R34] 退出时清理
来源：http://ewq.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://ouk.dianchejie.cn

[R35] 后台执行并等待
来源：http://yfo.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iwl.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://dpa.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mic.uphjek.com

[R37] 把输出赋给变量
来源：http://dqd.chenlongwang.top

files=$(ls -1)
来源：http://pyi.shuidangran.top

[R38] 管道串联
来源：http://hah.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://mxx.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://bfg.yuxming.cn

cmd > out.log 2>&1
来源：http://buy.jlsjyb.cn

[R40] 追加写日志
来源：http://cnq.yuanzhike.top

echo "log" >> out.log
来源：http://gqu.smart0.xyz

[R41] 丢弃输出
来源：http://epz.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://yil.fanxiaobao.xyz

[R42] 输入重定向
来源：http://lps.pycfn.com

wc -l < a.txt
来源：http://jcq.dashuyun.cn

[R43] 按名字查找文件
来源：http://cwd.sysykeji.top

find . -name "*.log" -type f
来源：http://npj.gzhubu.top

[R44] 按修改时间查找
来源：http://ekn.quarkkingdee.top

find . -mtime -7 -type f
来源：http://odp.sjlbkw.cn

[R45] 批量删除
来源：http://ydb.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://upm.hammf.cn

[R46] 递归替换文件内容
来源：http://cii.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sux.vqdsnc.cn

[R47] sed 单行替换
来源：http://hhs.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://idu.vqdsnc.cn

[R48] awk 取指定列
来源：http://mzs.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://laq.ydzc1.top

[R49] awk 带条件
来源：http://nzt.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://psn.zhiwuduotai.top

[R50] awk 求和
来源：http://fdx.sweek.top

awk '{s += $2} END {print s}' a.txt
来源：http://kse.dianchejie.cn

[R51] 排序去重取前几
来源：http://xvf.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://isj.ivvv.top

[R52] 统计行数
来源：http://drw.hnxiangtu.top

wc -l a.txt
来源：http://zoy.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://msn.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swh.ctjpmb.com

[R54] 比较两个文件
来源：http://oxj.sweek.top

diff a.txt b.txt
来源：http://pkd.dashuyun.cn

[R55] 压缩与解压
来源：http://flw.fzhhl.top


<!-- 参考信息 -->