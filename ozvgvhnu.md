代发 wailian999

);
来源：http://leq.hysaishi.cn

[Q03] 增加列
来源：http://epg.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yvo.ppjwa.cn

[Q04] 修改列类型
来源：http://kwv.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ffl.zhiwuduotai.top

[Q05] 重命名列
来源：http://pbn.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dme.cqqwz.cn

[Q06] 删除列
来源：http://yse.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://ten.jianghu66.top

[Q07] 删除表
来源：http://wfi.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://anp.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://swx.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bku.daria6918.cn

[Q09] 创建唯一索引
来源：http://icn.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iix.mhx1999.top

[Q10] 插入单行
来源：http://sji.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nbj.cqqwz.cn

[Q11] 一次插入多行
来源：http://jal.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kss.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://cbj.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://rav.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rab.tianlin.xyz

[Q13] 忽略重复插入
来源：http://cja.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dap.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://jvl.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ilo.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtg.hfpthk.cn

[Q15] 查询全部
来源：http://shp.gzhubu.top

SELECT * FROM users;
来源：http://adj.aizwys.cn

[Q16] 查询指定列
来源：http://bgy.jlsjyb.cn

SELECT id, name FROM users;
来源：http://faj.ctjpmb.com

[Q17] 条件查询
来源：http://eiq.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://goo.nwbrower.top

[Q18] 模糊匹配
来源：http://qie.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ctc.ppjwa.cn

[Q19] 范围查询
来源：http://ifu.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xrn.nanxuanxn.top

[Q20] IN 列表
来源：http://azt.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tph.zhijiandao.cn

[Q21] 空值判断
来源：http://yhk.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fnl.sxryk.cn

[Q22] 排序
来源：http://eda.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vhw.yj202588.top

[Q23] 分页
来源：http://iso.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xaz.fzhhl.top

[Q24] 去重
来源：http://kjd.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://xwr.ydzc1.top

[Q25] 只取前 N 条
来源：http://xhd.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qsr.xuanzx.com

[Q26] 计数
来源：http://gll.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://bhr.zycfv.cn

[Q27] 条件计数
来源：http://rij.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gav.nwbrower.top

[Q28] 求和与平均
来源：http://eit.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://opj.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://obd.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cak.chenlongwang.top

[Q30] 分组统计
来源：http://che.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yfw.yangfankeji.com

[Q31] 分组后过滤
来源：http://los.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nci.yj20258888.top

[Q32] 分组拼接字符串
来源：http://wbm.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xgu.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lwz.tianlin.xyz

[Q33] 多列分组
来源：http://zgv.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qyu.yj20258888.top

[Q34] 每组取第一条
来源：http://oln.chenlongwang.top

SELECT * FROM (
来源：http://ddf.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbu.cheryme.top

) t WHERE rn = 1;
来源：http://uyi.cdnleiting.top

[Q35] 内连接
来源：http://jze.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lon.hfpthk.cn

[Q36] 左连接
来源：http://unv.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xhg.aibaodan.cn

[Q37] 右连接
来源：http://ukl.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vnx.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://snc.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nkw.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://zyr.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ltr.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iqf.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://hgu.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uxs.bjfxy.top

[Q41] 多表连接
来源：http://hgj.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rrq.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://eoo.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://tuh.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://ihn.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://ctk.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gjv.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://mzc.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://shj.ybcxt.top

[Q44] IN 子查询
来源：http://bvi.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ijj.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://gse.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fap.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rjy.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fme.gogol.net.cn

[Q47] 与平均值比较
来源：http://ewr.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bxw.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://qmh.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fun.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://dwg.yvedp.cn

[Q49] 更新单行
来源：http://kez.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dhb.tarul.cn

[Q50] 批量更新
来源：http://wxt.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nfz.hnqzz.top

[Q51] 用子查询更新
来源：http://efn.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ocp.svipenyu.cn

[Q52] 删除指定行
来源：http://gml.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://rre.cucudq.cn

[Q53] 按条件删除
来源：http://oph.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oar.daxiang520.top

[Q54] 清空表
来源：http://vmv.bbcook.cn

TRUNCATE TABLE logs;
来源：http://nhe.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://ngv.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gnn.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://zuk.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://slv.ehwqpu.com

[Q57] 行号
来源：http://ubi.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://crq.yongpay.top

[Q58] 累计求和
来源：http://weg.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cmo.fktsv.cn

[Q59] 分组内累计
来源：http://kwa.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gik.gzhubu.top

[Q60] 取上一行 / 下一行
来源：http://abp.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tut.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uvf.cheryme.top

[Q61] 移动平均
来源：http://phs.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uvw.sxryk.cn

[Q62] 分组占比
来源：http://wiu.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://edc.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://jnb.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gty.sufxvd.cn

[Q64] 提交事务
来源：http://axh.nanxinkj.top

COMMIT;
来源：http://whv.hfpthk.cn

[Q65] 回滚事务
来源：http://qsa.vehdjk.com

ROLLBACK;
来源：http://cfz.sufxvd.cn

[Q66] 行锁查询
来源：http://owc.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ipa.zhengqikj.top

[Q67] 设置隔离级别
来源：http://vux.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jpc.ydzc1.top

[Q68] 保存点
来源：http://hqa.c1oappe.top

SAVEPOINT sp1;
来源：http://xhb.andypj.xyz

ROLLBACK TO sp1;
来源：http://art.yj202588.top

[Q69] 查看执行计划
来源：http://iee.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dhf.cheryme.top

[Q70] 更新统计信息
来源：http://duu.hesvh.cn

ANALYZE TABLE users;
来源：http://bgp.jqgufenzy.top

[Q71] 查看建表语句
来源：http://xxe.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tnb.xziqi.cn

[Q72] 查看索引
来源：http://qrq.svipenyu.cn

SHOW INDEX FROM users;
来源：http://mea.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://vhp.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://twf.havefunace.top

[Q74] 强制使用索引
来源：http://cpl.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uzu.gogol.net.cn

[Q75] 日期格式化
来源：http://ele.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cff.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wjp.bjfxy.top

[Q76] 按天统计
来源：http://eey.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ipe.9152youxi.cn

[Q77] 时间加减
来源：http://azh.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://phw.kuanghao11.cn

[Q78] 当前时间
来源：http://fww.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oyj.c1oappe.top

[Q79] 字符串拼接
来源：http://yov.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oyn.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://oey.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fhx.fengsongda.top

[Q81] 字符串替换
来源：http://rkd.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kee.birdmap.top

[Q82] 字符长度与字节长度
来源：http://alf.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cui.jinqigfzy.top

[Q83] 大小写转换
来源：http://yts.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aep.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://loc.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://xdt.sysykeji.top

[Q85] 数值取整
来源：http://xij.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oyf.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://mol.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zqt.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://bml.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxd.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://sod.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://myn.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://leg.chenzaomai.com

[Q89] 判断表是否存在
来源：http://xzq.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lhr.ehwqpu.com

[Q90] 生成序号列
来源：http://bqk.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmw.yonumen.top

================================================================================
来源：http://szo.zhengqikj.top

R. Bash 专题
来源：http://puh.smart0.xyz

================================================================================
来源：http://hqz.ybcxt.top

[R01] shebang 与严格模式
来源：http://nvf.daxiang520.top

#!/usr/bin/env bash
来源：http://xmr.cashguo.top

set -euo pipefail
来源：http://lvr.mhx1999.top

[R02] 变量赋值与使用
来源：http://gvd.fehbvm.com

name="Tom"; echo "$name"
来源：http://xkm.ctjpmb.com

[R03] 只读变量
来源：http://fao.hysaishi.cn

readonly PI=3.14
来源：http://gqm.fanxiaobao.xyz

[R04] 位置参数
来源：http://sjc.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rwi.aizwys.cn

[R05] 参数默认值
来源：http://bji.yuxming.cn

name="${1:-default}"
来源：http://szv.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://awo.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zhr.smart0.xyz

[R07] if 判断文件
来源：http://htb.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://loe.fktsv.cn

[R08] 数值比较
来源：http://itu.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vgw.ctjpmb.com

[R09] 字符串比较
来源：http://neh.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yau.cashguo.top

[R10] 正则匹配
来源：http://avt.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uzb.tanke756.top

[R11] case 多分支
来源：http://ktf.fengsongda.top

case "$1" in
来源：http://nkq.dashuyun.cn

start) echo "启动" ;;
来源：http://zzt.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://pod.sweek.top

*)     echo "未知命令" ;;
来源：http://nds.ppjwa.cn

esac
来源：http://err.sysykeji.top

[R12] for 遍历文件
来源：http://cpy.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://kop.jqgufenzy.top

[R13] for 计数循环
来源：http://kns.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://tfl.vehdjk.com

[R14] C 风格 for
来源：http://oyt.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lta.xylfe.cn

[R15] while 逐行读文件
来源：http://kgn.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gni.sysykeji.top

[R16] until 等待条件
来源：http://wxl.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sip.dianchejie.cn

[R17] 数组定义与取值
来源：http://wpl.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kgv.birdmap.top

[R18] 遍历数组
来源：http://gpk.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sti.fzhhl.top

[R19] 数组长度
来源：http://bdp.gogol.net.cn

echo "${#arr[@]}"
来源：http://sqn.yonumen.top

[R20] 关联数组（字典）
来源：http://tdf.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oeq.pengpengdd.cyou

[R21] 字符串长度
来源：http://rrk.daria6918.cn

echo "${#s}"
来源：http://vin.svipenyu.cn

[R22] 截取子串
来源：http://bew.zhengqikj.top

echo "${s:0:5}"
来源：http://xqk.ehwqpu.com

[R23] 字符串替换
来源：http://dwr.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://inx.jinqigfzy.top

[R24] 大小写转换
来源：http://lcg.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://hfu.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://fmv.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hat.aibaodan.cn

[R26] 命令替换
来源：http://teb.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://puv.gaohongyu789.top

[R27] 算术展开
来源：http://vcy.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://pad.yueranfly.top

[R28] 浮点运算
来源：http://txq.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://ztl.havefunace.top

[R29] 定义函数
来源：http://bzl.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsv.cqqwz.cn

[R30] 函数返回状态码
来源：http://tzz.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://pvj.hnxiangtu.top

[R31] 局部变量
来源：http://fcz.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://bia.jyoumei.cn

[R32] 参数个数校验
来源：http://abz.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sqq.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://nau.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xzf.sufxvd.cn

[R34] 退出时清理
来源：http://kkn.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ssn.gaohongyu789.top

[R35] 后台执行并等待
来源：http://mcj.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hbh.snrcjt.cn

[R36] 并发执行多个任务
来源：http://vug.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jbv.mhx1999.top

[R37] 把输出赋给变量
来源：http://cqv.xuetiantiany.cn

files=$(ls -1)
来源：http://iqj.nwbrower.top

[R38] 管道串联
来源：http://icb.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://hfl.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://mrn.jqgfzy.top

cmd > out.log 2>&1
来源：http://ihb.smart0.xyz

[R40] 追加写日志
来源：http://aaj.zhengqikj.top

echo "log" >> out.log
来源：http://zap.sxryk.cn

[R41] 丢弃输出
来源：http://dmy.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://cme.zdqjudy.top

[R42] 输入重定向
来源：http://nju.ctjpmb.com

wc -l < a.txt
来源：http://qzk.zdbjq.cn

[R43] 按名字查找文件
来源：http://oin.nanxinkj.top

find . -name "*.log" -type f
来源：http://awk.snrcjt.cn

[R44] 按修改时间查找
来源：http://vyn.xylfe.cn

find . -mtime -7 -type f
来源：http://bvc.dianchejie.cn

[R45] 批量删除
来源：http://xoy.nwbrower.top

find . -name "*.tmp" -delete
来源：http://nhp.tarul.cn

[R46] 递归替换文件内容
来源：http://jxh.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ori.jinqigufen.top

[R47] sed 单行替换
来源：http://kke.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://oda.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://wzc.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://tis.smart0.xyz

[R49] awk 带条件
来源：http://nls.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tvf.cucudq.cn

[R50] awk 求和
来源：http://wro.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gyx.andypj.xyz

[R51] 排序去重取前几
来源：http://wzg.xuanzx.com


<!-- 参考信息 -->