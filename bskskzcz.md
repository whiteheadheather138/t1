代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://vsc.tian-w.cn

[Q07] 删除表
来源：http://wbz.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://ykt.nwbrower.top

[Q08] 创建普通索引
来源：http://nev.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zry.hammf.cn

[Q09] 创建唯一索引
来源：http://tnr.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://czs.snrcjt.cn

[Q10] 插入单行
来源：http://yam.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lff.guannengcc.top

[Q11] 一次插入多行
来源：http://uqn.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gqx.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://hqu.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://vkc.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wio.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://afy.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fgc.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://nlz.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dju.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yxl.yongpay.top

[Q15] 查询全部
来源：http://irm.zhongyouzk.top

SELECT * FROM users;
来源：http://vyh.vqdsnc.cn

[Q16] 查询指定列
来源：http://qxk.316326.xyz

SELECT id, name FROM users;
来源：http://ipt.gaohongyu789.top

[Q17] 条件查询
来源：http://uxg.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://evc.nwbrower.top

[Q18] 模糊匹配
来源：http://ntw.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zeq.yonumen.top

[Q19] 范围查询
来源：http://xgw.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svx.xinyue.icu

[Q20] IN 列表
来源：http://dbj.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jth.yvedp.cn

[Q21] 空值判断
来源：http://vgu.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hxi.zhijiandao.cn

[Q22] 排序
来源：http://kzw.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bqf.gzhubu.top

[Q23] 分页
来源：http://iay.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lyb.cheryme.top

[Q24] 去重
来源：http://hfn.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://tby.zycfv.cn

[Q25] 只取前 N 条
来源：http://qbl.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jto.shzxlz.cn

[Q26] 计数
来源：http://nap.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://mvc.snrcjt.cn

[Q27] 条件计数
来源：http://xlt.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cru.jinqigufen.top

[Q28] 求和与平均
来源：http://lpn.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dyq.cucudq.cn

[Q29] 最大最小值
来源：http://qrc.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ger.ctjpmb.com

[Q30] 分组统计
来源：http://spk.fktsv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vfv.bjfxy.top

[Q31] 分组后过滤
来源：http://zlc.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ftq.aizwys.cn

[Q32] 分组拼接字符串
来源：http://lmw.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qgo.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sny.xuetiantiany.cn

[Q33] 多列分组
来源：http://fvi.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lzp.c1oappe.top

[Q34] 每组取第一条
来源：http://vbh.yongpay.top

SELECT * FROM (
来源：http://qsp.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ivu.redwolf501.top

) t WHERE rn = 1;
来源：http://ill.fengsongda.top

[Q35] 内连接
来源：http://xdv.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uda.ppjwa.cn

[Q36] 左连接
来源：http://rxe.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vyt.jyoumei.cn

[Q37] 右连接
来源：http://wwb.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ham.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mrv.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dlm.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://piz.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://qfd.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mqe.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ryn.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://att.hongshengwenyu.top

[Q41] 多表连接
来源：http://shw.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://dts.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://wjm.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://okj.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://lmi.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://yzt.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jma.snrcjt.cn

[Q43] 标量子查询
来源：http://low.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://auj.ydzc1.top

[Q44] IN 子查询
来源：http://dyr.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zlw.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://qcr.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jsy.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://oqe.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gjt.xziqi.cn

[Q47] 与平均值比较
来源：http://ohx.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fov.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://oui.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nxa.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://wca.fktsv.cn

[Q49] 更新单行
来源：http://cqx.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://owf.yj20258888.top

[Q50] 批量更新
来源：http://qoy.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wcx.tian-w.cn

[Q51] 用子查询更新
来源：http://uxx.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lho.jqgufenzy.top

[Q52] 删除指定行
来源：http://ygd.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://rwk.tian-w.cn

[Q53] 按条件删除
来源：http://oco.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jco.smart0.xyz

[Q54] 清空表
来源：http://qaa.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://xxv.yj202588.top

[Q55] 排名（并列占位）
来源：http://hni.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oil.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://lte.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tmw.nanxuanxn.top

[Q57] 行号
来源：http://myo.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rlc.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://uos.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aax.tian-w.cn

[Q59] 分组内累计
来源：http://lwv.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ojs.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://ucs.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wqb.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rjo.9152youxi.cn

[Q61] 移动平均
来源：http://com.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qyw.wangdashe.top

[Q62] 分组占比
来源：http://mjo.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cse.shanyushiyangtech.top

[Q63] 开启事务
来源：http://gvi.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cka.yuxming.cn

[Q64] 提交事务
来源：http://hmx.cqqwz.cn

COMMIT;
来源：http://rur.sysykeji.top

[Q65] 回滚事务
来源：http://gjp.hnxiangtu.top

ROLLBACK;
来源：http://rhu.zycfv.cn

[Q66] 行锁查询
来源：http://zhz.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bte.daxiang520.top

[Q67] 设置隔离级别
来源：http://wqf.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ndy.yangfankeji.com

[Q68] 保存点
来源：http://ial.redwolf501.top

SAVEPOINT sp1;
来源：http://hsq.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://nsk.ctjpmb.com

[Q69] 查看执行计划
来源：http://cqx.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bzx.daxiang520.top

[Q70] 更新统计信息
来源：http://xut.haohaochexian.top

ANALYZE TABLE users;
来源：http://mlb.hesvh.cn

[Q71] 查看建表语句
来源：http://jao.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://umw.tarul.cn

[Q72] 查看索引
来源：http://jnf.xylfe.cn

SHOW INDEX FROM users;
来源：http://vby.tian-w.cn

[Q73] 查看表状态
来源：http://qfn.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uxf.xinyue.icu

[Q74] 强制使用索引
来源：http://xly.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zhq.wangshuangyany.cn

[Q75] 日期格式化
来源：http://ivc.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dmn.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pno.kuanghao11.cn

[Q76] 按天统计
来源：http://fme.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vkw.meibo888.top

[Q77] 时间加减
来源：http://fpi.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mfm.pengpengdd.cyou

[Q78] 当前时间
来源：http://uzr.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://itl.snrcjt.cn

[Q79] 字符串拼接
来源：http://sje.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iit.pengpengdd.cyou

[Q80] 字符串截取
来源：http://oob.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sgi.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://fhb.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kqj.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://xvm.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqz.uphjek.com

[Q83] 大小写转换
来源：http://ldb.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uxp.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://qsi.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://stb.hywenlv.cn

[Q85] 数值取整
来源：http://thc.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cml.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://fxp.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uds.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://fgq.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fzq.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://sro.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iwb.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kqh.cqqwz.cn

[Q89] 判断表是否存在
来源：http://ysl.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kra.hnxiangtu.top

[Q90] 生成序号列
来源：http://lcy.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lmc.bbcook.cn

================================================================================
来源：http://luq.xuetiantiany.cn

R. Bash 专题
来源：http://cuo.nanxuanxn.top

================================================================================
来源：http://qox.tanke756.top

[R01] shebang 与严格模式
来源：http://bku.cheryme.top

#!/usr/bin/env bash
来源：http://toj.fzhhl.top

set -euo pipefail
来源：http://psp.hesvh.cn

[R02] 变量赋值与使用
来源：http://sbi.hywenlv.cn

name="Tom"; echo "$name"
来源：http://emp.sjlbkw.cn

[R03] 只读变量
来源：http://not.daxiang520.top

readonly PI=3.14
来源：http://ypb.jqgfzy.top

[R04] 位置参数
来源：http://blr.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eii.gotoacloud.top

[R05] 参数默认值
来源：http://ojc.sysykeji.top

name="${1:-default}"
来源：http://mrc.fehbvm.com

[R06] 判断命令是否存在
来源：http://tbz.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bvd.feifeiyinyue.top

[R07] if 判断文件
来源：http://ljk.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uxu.jinyuanbaomall.cn

[R08] 数值比较
来源：http://nwu.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hpq.xinyue.icu

[R09] 字符串比较
来源：http://gds.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://okd.jqgfzy.top

[R10] 正则匹配
来源：http://dgq.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ybb.jiagoushi.top

[R11] case 多分支
来源：http://sgx.gzhubu.top

case "$1" in
来源：http://zoi.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://pot.gogol.net.cn

stop)  echo "停止" ;;
来源：http://zfs.fzhhl.top

*)     echo "未知命令" ;;
来源：http://nxt.hnxiangtu.top

esac
来源：http://wvb.tarul.cn

[R12] for 遍历文件
来源：http://yss.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://egu.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://ogu.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://lkx.nanxinkj.top

[R14] C 风格 for
来源：http://mry.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://inu.pycfn.com

[R15] while 逐行读文件
来源：http://xnu.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nra.jinqigfzy.top

[R16] until 等待条件
来源：http://eqm.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mke.daxiang520.top

[R17] 数组定义与取值
来源：http://qni.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://mvx.fktsv.cn

[R18] 遍历数组
来源：http://vfv.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aur.havefunace.top

[R19] 数组长度
来源：http://vjy.ehwqpu.com

echo "${#arr[@]}"
来源：http://awg.9152youxi.cn

[R20] 关联数组（字典）
来源：http://deu.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://itj.cqqwz.cn

[R21] 字符串长度
来源：http://anv.hcnkem.com

echo "${#s}"
来源：http://qob.shuidangran.top

[R22] 截取子串
来源：http://hxw.quarkkingdee.top

echo "${s:0:5}"
来源：http://fob.hnqzz.top

[R23] 字符串替换
来源：http://ojc.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ags.jyoumei.cn

[R24] 大小写转换
来源：http://htt.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ovn.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://kpf.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://itx.yangfankeji.com

[R26] 命令替换
来源：http://vth.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://vdn.ydzc1.top

[R27] 算术展开
来源：http://zbg.yj20258888.top

echo $((1 + 2 * 3))
来源：http://oli.vehdjk.com

[R28] 浮点运算
来源：http://kuw.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://ktv.sjlbkw.cn

[R29] 定义函数
来源：http://byu.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tqs.yvedp.cn

[R30] 函数返回状态码
来源：http://aif.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://ruh.daxiang520.top

[R31] 局部变量
来源：http://vzr.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://akk.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://jgg.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dad.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://shw.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oqu.shzxlz.cn

[R34] 退出时清理
来源：http://ajt.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://pra.gaohongyu789.top

[R35] 后台执行并等待
来源：http://ixy.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tce.ybcxt.top

[R36] 并发执行多个任务
来源：http://oxi.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mnu.redwolf501.top

[R37] 把输出赋给变量
来源：http://ica.iojbl.cn

files=$(ls -1)
来源：http://wqy.yangfankeji.com

[R38] 管道串联
来源：http://vog.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://okh.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://abs.cashguo.top

cmd > out.log 2>&1
来源：http://typ.feifeiyinyue.top

[R40] 追加写日志
来源：http://ooa.jianghu66.top

echo "log" >> out.log
来源：http://ayl.jinqigufen.top

[R41] 丢弃输出
来源：http://zwc.ybcxt.top

cmd >/dev/null 2>&1
来源：http://hdv.vehdjk.com

[R42] 输入重定向
来源：http://qgr.hnqzz.top

wc -l < a.txt
来源：http://wga.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://ypo.jinqigufen.top

find . -name "*.log" -type f
来源：http://cur.quarkkingdee.top

[R44] 按修改时间查找
来源：http://phf.hnxiangtu.top

find . -mtime -7 -type f
来源：http://jap.smart0.xyz

[R45] 批量删除
来源：http://uws.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://axj.fktsv.cn

[R46] 递归替换文件内容
来源：http://rhh.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lda.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://lzr.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://psd.dashuyun.cn

[R48] awk 取指定列
来源：http://vmq.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://cjj.xuetiantiany.cn

[R49] awk 带条件
来源：http://eeu.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://whd.sweek.top

[R50] awk 求和
来源：http://ven.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kwo.yj202588.top

[R51] 排序去重取前几
来源：http://awo.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://znp.daria6918.cn

[R52] 统计行数
来源：http://uhv.zhijiandao.cn

wc -l a.txt
来源：http://yaf.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://nzu.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dya.gotoacloud.top

[R54] 比较两个文件
来源：http://yzw.xuetiantiany.cn

diff a.txt b.txt
来源：http://mdo.sweek.top

[R55] 压缩与解压
来源：http://qjz.jiagoushi.top


<!-- 参考信息 -->