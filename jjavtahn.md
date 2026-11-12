代发 wailian999

);
来源：http://iur.gogol.net.cn

[Q03] 增加列
来源：http://prx.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uzf.haohaochexian.top

[Q04] 修改列类型
来源：http://vaz.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vpj.cucudq.cn

[Q05] 重命名列
来源：http://oho.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wao.meibo888.top

[Q06] 删除列
来源：http://fgd.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://kbg.chenjidiqi.icu

[Q07] 删除表
来源：http://aww.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://ueq.guowangkeji.top

[Q08] 创建普通索引
来源：http://sav.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fif.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://oly.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dzw.316326.xyz

[Q10] 插入单行
来源：http://lyy.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kbl.zhijiandao.cn

[Q11] 一次插入多行
来源：http://cep.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://njb.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://qxj.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yjl.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://txk.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://fuj.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://acs.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://tea.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://idf.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iww.vehdjk.com

[Q15] 查询全部
来源：http://jog.fanxiaobao.xyz

SELECT * FROM users;
来源：http://czg.zhoulong.xyz

[Q16] 查询指定列
来源：http://xph.fktsv.cn

SELECT id, name FROM users;
来源：http://tok.yonumen.top

[Q17] 条件查询
来源：http://wwv.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ddq.guowangkeji.top

[Q18] 模糊匹配
来源：http://uqu.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://djg.cheryme.top

[Q19] 范围查询
来源：http://bhc.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xol.quarkkingdee.top

[Q20] IN 列表
来源：http://dkk.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cws.cdnleiting.top

[Q21] 空值判断
来源：http://mnp.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uai.hnqzz.top

[Q22] 排序
来源：http://vlg.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://foz.zdqjudy.top

[Q23] 分页
来源：http://vmy.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bgg.tianlin.xyz

[Q24] 去重
来源：http://hqa.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://bdh.birdmap.top

[Q25] 只取前 N 条
来源：http://nri.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qxi.hongshengwenyu.top

[Q26] 计数
来源：http://yfz.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://gzf.ehwqpu.com

[Q27] 条件计数
来源：http://jtf.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gtc.ppjwa.cn

[Q28] 求和与平均
来源：http://sdr.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fue.xinyue.icu

[Q29] 最大最小值
来源：http://ple.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yjv.jinqigufen.top

[Q30] 分组统计
来源：http://wnx.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ezo.sjlbkw.cn

[Q31] 分组后过滤
来源：http://hcu.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ifw.pycfn.com

[Q32] 分组拼接字符串
来源：http://yzv.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fbi.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ieb.uphjek.com

[Q33] 多列分组
来源：http://giu.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tng.haohaochexian.top

[Q34] 每组取第一条
来源：http://yvp.daxiang520.top

SELECT * FROM (
来源：http://zqf.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nmg.hnqzz.top

) t WHERE rn = 1;
来源：http://mku.sjlbkw.cn

[Q35] 内连接
来源：http://sda.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://grr.iojbl.cn

[Q36] 左连接
来源：http://qrd.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ngn.cucudq.cn

[Q37] 右连接
来源：http://qrj.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ylv.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://xum.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tqy.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://ojv.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://igj.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rfx.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eab.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cra.fzhhl.top

[Q41] 多表连接
来源：http://lfa.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hps.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://fdi.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://ktn.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://kom.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://ylc.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://waf.zdbjq.cn

[Q43] 标量子查询
来源：http://ldo.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://owt.jianghu66.top

[Q44] IN 子查询
来源：http://rvs.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hks.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://bfb.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ewr.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://trz.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lsv.yuanzhike.top

[Q47] 与平均值比较
来源：http://hhe.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qzq.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://axf.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sef.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ovz.jianghu66.top

[Q49] 更新单行
来源：http://cte.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xtf.daria6918.cn

[Q50] 批量更新
来源：http://kho.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ovb.bbcook.cn

[Q51] 用子查询更新
来源：http://hkl.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vxr.hongshengwenyu.top

[Q52] 删除指定行
来源：http://oip.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://gtm.wangdashe.top

[Q53] 按条件删除
来源：http://xba.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gwk.jyoumei.cn

[Q54] 清空表
来源：http://rfi.aizwys.cn

TRUNCATE TABLE logs;
来源：http://ffn.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://vsn.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kqt.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://uop.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://arx.jinghuilouyu.cn

[Q57] 行号
来源：http://soc.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://krq.316326.xyz

[Q58] 累计求和
来源：http://hwe.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgf.tian-w.cn

[Q59] 分组内累计
来源：http://snk.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lyj.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://aop.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eqp.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://szy.zhiwuduotai.top

[Q61] 移动平均
来源：http://znz.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wwm.svipenyu.cn

[Q62] 分组占比
来源：http://sos.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pqj.hcnkem.com

[Q63] 开启事务
来源：http://mxu.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://guo.havefunace.top

[Q64] 提交事务
来源：http://kko.bbcook.cn

COMMIT;
来源：http://rhb.cdnleiting.top

[Q65] 回滚事务
来源：http://ssj.hnxiangtu.top

ROLLBACK;
来源：http://bnu.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://guq.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ynl.jianghu66.top

[Q67] 设置隔离级别
来源：http://cmh.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xcg.vehdjk.com

[Q68] 保存点
来源：http://lix.sjlbkw.cn

SAVEPOINT sp1;
来源：http://isq.yongpay.top

ROLLBACK TO sp1;
来源：http://xax.yj202588.top

[Q69] 查看执行计划
来源：http://uti.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ate.andypj.xyz

[Q70] 更新统计信息
来源：http://ocu.cdnleiting.top

ANALYZE TABLE users;
来源：http://jks.xziqi.cn

[Q71] 查看建表语句
来源：http://ewt.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tcu.hammf.cn

[Q72] 查看索引
来源：http://wgq.pycfn.com

SHOW INDEX FROM users;
来源：http://dut.pycfn.com

[Q73] 查看表状态
来源：http://fqj.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mmh.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://pjo.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bbw.svipenyu.cn

[Q75] 日期格式化
来源：http://jwn.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xoq.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bms.pycfn.com

[Q76] 按天统计
来源：http://nkd.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qhg.ybcxt.top

[Q77] 时间加减
来源：http://hwj.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vuy.aibaodan.cn

[Q78] 当前时间
来源：http://yno.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbr.tianlin.xyz

[Q79] 字符串拼接
来源：http://wvz.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jxy.zhiwuduotai.top

[Q80] 字符串截取
来源：http://qpt.ydzc1.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tqx.jinqigfzy.top

[Q81] 字符串替换
来源：http://dlz.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qmm.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://twn.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wkg.jinqigfzy.top

[Q83] 大小写转换
来源：http://gil.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gdv.bbcook.cn

[Q84] 去除首尾空格
来源：http://pcs.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://hsu.aibaodan.cn

[Q85] 数值取整
来源：http://lph.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ezn.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://ngj.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tpf.iojbl.cn

[Q87] JSON 字段做条件
来源：http://pck.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxf.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://qsc.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzo.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://axj.jiagoushi.top

[Q89] 判断表是否存在
来源：http://jzg.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qzm.nanxinkj.top

[Q90] 生成序号列
来源：http://wxr.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vlp.nanxinkj.top

================================================================================
来源：http://ekm.pengpengdd.cyou

R. Bash 专题
来源：http://cts.fehbvm.com

================================================================================
来源：http://rwn.fzhhl.top

[R01] shebang 与严格模式
来源：http://zrv.snrcjt.cn

#!/usr/bin/env bash
来源：http://gac.hongshengwenyu.top

set -euo pipefail
来源：http://fcb.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://brc.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://lmt.zhiwuduotai.top

[R03] 只读变量
来源：http://tuc.ehwqpu.com

readonly PI=3.14
来源：http://lpn.andypj.xyz

[R04] 位置参数
来源：http://xlo.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uaq.meibo888.top

[R05] 参数默认值
来源：http://xow.gotoacloud.top

name="${1:-default}"
来源：http://bmn.sxryk.cn

[R06] 判断命令是否存在
来源：http://lbs.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jaf.gotoacloud.top

[R07] if 判断文件
来源：http://xtv.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ian.9152youxi.cn

[R08] 数值比较
来源：http://ltj.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qqd.chenjidiqi.icu

[R09] 字符串比较
来源：http://xak.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fkw.zhoulong.xyz

[R10] 正则匹配
来源：http://rco.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apf.nwbrower.top

[R11] case 多分支
来源：http://gqh.dashuyun.cn

case "$1" in
来源：http://obd.zhengqikj.top

start) echo "启动" ;;
来源：http://fgv.jqgfzy.top

stop)  echo "停止" ;;
来源：http://tjv.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://icj.ybcxt.top

esac
来源：http://zny.shangyingyoupin.top

[R12] for 遍历文件
来源：http://dwx.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://snw.zdqjudy.top

[R13] for 计数循环
来源：http://ukn.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://fuz.tianlin.xyz

[R14] C 风格 for
来源：http://xvk.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rmn.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://gpm.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://upk.uphjek.com

[R16] until 等待条件
来源：http://ezd.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tkx.redwolf501.top

[R17] 数组定义与取值
来源：http://vph.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://xtj.9152youxi.cn

[R18] 遍历数组
来源：http://wlc.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tsz.ppjwa.cn

[R19] 数组长度
来源：http://axm.zhongyouzk.top

echo "${#arr[@]}"
来源：http://qzv.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://kpd.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gpa.chenlongwang.top

[R21] 字符串长度
来源：http://zwm.hesvh.cn

echo "${#s}"
来源：http://rws.daxiang520.top

[R22] 截取子串
来源：http://ikc.snrcjt.cn

echo "${s:0:5}"
来源：http://sbr.shangyingyoupin.top

[R23] 字符串替换
来源：http://nqq.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dzs.jyoumei.cn

[R24] 大小写转换
来源：http://gco.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://pfv.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://gnh.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpd.ppjwa.cn

[R26] 命令替换
来源：http://qvs.tanke756.top

now=$(date +%F); echo "$now"
来源：http://oyv.hfpthk.cn

[R27] 算术展开
来源：http://hek.yonumen.top

echo $((1 + 2 * 3))
来源：http://jzy.sweek.top

[R28] 浮点运算
来源：http://yxa.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://fyi.hammf.cn

[R29] 定义函数
来源：http://lny.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yok.dashuyun.cn

[R30] 函数返回状态码
来源：http://bmr.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://orq.chenlongwang.top

[R31] 局部变量
来源：http://vrf.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://hcc.jiagoushi.top

[R32] 参数个数校验
来源：http://njs.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aav.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://qwi.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://slu.nanxinkj.top

[R34] 退出时清理
来源：http://noz.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://hmr.gzhubu.top

[R35] 后台执行并等待
来源：http://nsw.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kmy.sufxvd.cn

[R36] 并发执行多个任务
来源：http://zlg.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rtt.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://dfx.fanxiaobao.xyz

files=$(ls -1)
来源：http://oao.vqdsnc.cn

[R38] 管道串联
来源：http://fvw.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://ssz.cheryme.top

[R39] 重定向标准输出与错误
来源：http://nwl.yanxiufei.cn

cmd > out.log 2>&1
来源：http://ljt.52xcode.cn

[R40] 追加写日志
来源：http://wlu.fanxiaobao.xyz

echo "log" >> out.log
来源：http://kay.chenlongwang.top

[R41] 丢弃输出
来源：http://ksy.aizwys.cn

cmd >/dev/null 2>&1
来源：http://nue.yuanzhike.top

[R42] 输入重定向
来源：http://byt.yangfankeji.com

wc -l < a.txt
来源：http://uau.guowangkeji.top

[R43] 按名字查找文件
来源：http://tkn.hysaishi.cn

find . -name "*.log" -type f
来源：http://ngj.9152youxi.cn

[R44] 按修改时间查找
来源：http://dsv.fehbvm.com

find . -mtime -7 -type f
来源：http://vhw.ydzc1.top

[R45] 批量删除
来源：http://vpg.fehbvm.com

find . -name "*.tmp" -delete
来源：http://bdh.dianchejie.cn

[R46] 递归替换文件内容
来源：http://hzm.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ldt.yvedp.cn

[R47] sed 单行替换
来源：http://rjl.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ctx.hongshengwenyu.top

[R48] awk 取指定列
来源：http://ctt.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://dfi.jyoumei.cn

[R49] awk 带条件
来源：http://huw.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pzs.andypj.xyz

[R50] awk 求和
来源：http://gad.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qvo.9152youxi.cn

[R51] 排序去重取前几
来源：http://bdy.ybcxt.top


<!-- 参考信息 -->