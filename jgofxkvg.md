代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://dmq.shanyushiyangtech.top

[Q07] 删除表
来源：http://wez.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://dts.xylfe.cn

[Q08] 创建普通索引
来源：http://fmt.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yye.ctjpmb.com

[Q09] 创建唯一索引
来源：http://bam.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wij.yueranfly.top

[Q10] 插入单行
来源：http://ipj.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://byj.vqdsnc.cn

[Q11] 一次插入多行
来源：http://qae.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bac.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://gwx.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://ovx.hywenlv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://teo.gotoacloud.top

[Q13] 忽略重复插入
来源：http://buv.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xll.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://hxa.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fho.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://veb.fengsongda.top

[Q15] 查询全部
来源：http://adm.zhoulong.xyz

SELECT * FROM users;
来源：http://oft.chenzaomai.com

[Q16] 查询指定列
来源：http://jdy.zhijiandao.cn

SELECT id, name FROM users;
来源：http://unl.hammf.cn

[Q17] 条件查询
来源：http://wym.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udz.pycfn.com

[Q18] 模糊匹配
来源：http://pqi.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gmx.yonumen.top

[Q19] 范围查询
来源：http://yum.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ffv.hnqzz.top

[Q20] IN 列表
来源：http://xkm.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vgo.zdbjq.cn

[Q21] 空值判断
来源：http://snl.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://juw.haohaochexian.top

[Q22] 排序
来源：http://vxk.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ald.zhiwuduotai.top

[Q23] 分页
来源：http://aey.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rhy.52xcode.cn

[Q24] 去重
来源：http://qul.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://exy.chenzaomai.com

[Q25] 只取前 N 条
来源：http://jkd.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xor.nanxinkj.top

[Q26] 计数
来源：http://ndb.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://vxk.smart0.xyz

[Q27] 条件计数
来源：http://ghe.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvb.nanxinkj.top

[Q28] 求和与平均
来源：http://vbw.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gbi.birdmap.top

[Q29] 最大最小值
来源：http://anf.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fqe.nanxuanxn.top

[Q30] 分组统计
来源：http://wxd.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://akn.ctjpmb.com

[Q31] 分组后过滤
来源：http://qvv.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://seb.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://xex.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ccj.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rgd.tanke756.top

[Q33] 多列分组
来源：http://ocb.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://een.zhoulong.xyz

[Q34] 每组取第一条
来源：http://yzb.shuidangran.top

SELECT * FROM (
来源：http://vpq.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lqd.fehbvm.com

) t WHERE rn = 1;
来源：http://ovn.nanxuanxn.top

[Q35] 内连接
来源：http://ilw.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zxn.xylfe.cn

[Q36] 左连接
来源：http://izl.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iuz.smart0.xyz

[Q37] 右连接
来源：http://dng.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ibb.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://xdb.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qay.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://ewb.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uoa.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dmu.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vxq.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wlq.pycfn.com

[Q41] 多表连接
来源：http://osd.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://axt.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://zwz.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://pve.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://gai.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://wns.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yuc.nanxuanxn.top

[Q43] 标量子查询
来源：http://zbd.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vts.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://yte.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://itx.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://xva.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ouy.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://imi.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rzi.sweek.top

[Q47] 与平均值比较
来源：http://cuz.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pyu.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://cqj.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://die.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://vdn.cheryme.top

[Q49] 更新单行
来源：http://gcr.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fhz.havefunace.top

[Q50] 批量更新
来源：http://jzn.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tkk.andypj.xyz

[Q51] 用子查询更新
来源：http://kku.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zpa.smart0.xyz

[Q52] 删除指定行
来源：http://ydc.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://qbg.gotoacloud.top

[Q53] 按条件删除
来源：http://cxw.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxf.jinqigfzy.top

[Q54] 清空表
来源：http://eyu.smart0.xyz

TRUNCATE TABLE logs;
来源：http://waa.yuxming.cn

[Q55] 排名（并列占位）
来源：http://dqa.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yoh.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://msm.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qqi.hysaishi.cn

[Q57] 行号
来源：http://ree.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgg.meibo888.top

[Q58] 累计求和
来源：http://bfj.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://txc.hysaishi.cn

[Q59] 分组内累计
来源：http://xfg.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xvq.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://fto.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oca.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lej.pycfn.com

[Q61] 移动平均
来源：http://yoc.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ncq.xylfe.cn

[Q62] 分组占比
来源：http://gtt.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://etj.yueranfly.top

[Q63] 开启事务
来源：http://blr.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kyp.dianchejie.cn

[Q64] 提交事务
来源：http://tjp.uphjek.com

COMMIT;
来源：http://sei.redwolf501.top

[Q65] 回滚事务
来源：http://hab.hongshengwenyu.top

ROLLBACK;
来源：http://avw.zdqjudy.top

[Q66] 行锁查询
来源：http://cbh.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tyb.316326.xyz

[Q67] 设置隔离级别
来源：http://jlt.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fch.cqqwz.cn

[Q68] 保存点
来源：http://rqx.bjfxy.top

SAVEPOINT sp1;
来源：http://wgc.bjfxy.top

ROLLBACK TO sp1;
来源：http://ncr.sysykeji.top

[Q69] 查看执行计划
来源：http://pky.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bds.fengsongda.top

[Q70] 更新统计信息
来源：http://jiq.jyoumei.cn

ANALYZE TABLE users;
来源：http://zou.zhijiandao.cn

[Q71] 查看建表语句
来源：http://cks.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wev.fengsongda.top

[Q72] 查看索引
来源：http://jym.bjfxy.top

SHOW INDEX FROM users;
来源：http://qbg.yuanzhike.top

[Q73] 查看表状态
来源：http://fsn.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://noi.daxiang520.top

[Q74] 强制使用索引
来源：http://idh.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eqz.yueranfly.top

[Q75] 日期格式化
来源：http://uwb.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rls.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qbo.sjlbkw.cn

[Q76] 按天统计
来源：http://wkw.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tvs.dianchejie.cn

[Q77] 时间加减
来源：http://ill.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qbo.dashuyun.cn

[Q78] 当前时间
来源：http://kah.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cbj.iojbl.cn

[Q79] 字符串拼接
来源：http://mrn.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zon.vehdjk.com

[Q80] 字符串截取
来源：http://tik.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kta.yangfankeji.com

[Q81] 字符串替换
来源：http://nbh.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zkq.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://eff.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nlh.jqgfzy.top

[Q83] 大小写转换
来源：http://lqa.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbe.havefunace.top

[Q84] 去除首尾空格
来源：http://dxd.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://znn.jyoumei.cn

[Q85] 数值取整
来源：http://rxp.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bwf.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://fym.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bmh.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://xeu.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xvn.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://cpa.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tmv.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ytk.bjfxy.top

[Q89] 判断表是否存在
来源：http://ztn.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lnr.jqgufenzy.top

[Q90] 生成序号列
来源：http://uuj.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bqr.gotoacloud.top

================================================================================
来源：http://dzs.jqgfzy.top

R. Bash 专题
来源：http://rih.zhoulong.xyz

================================================================================
来源：http://mfn.0kj1m.cn

[R01] shebang 与严格模式
来源：http://fvq.havefunace.top

#!/usr/bin/env bash
来源：http://xuv.yonumen.top

set -euo pipefail
来源：http://yet.yangfankeji.com

[R02] 变量赋值与使用
来源：http://nuu.tian-w.cn

name="Tom"; echo "$name"
来源：http://mam.iojbl.cn

[R03] 只读变量
来源：http://zia.andypj.xyz

readonly PI=3.14
来源：http://ixv.xziqi.cn

[R04] 位置参数
来源：http://yai.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iel.daxiang520.top

[R05] 参数默认值
来源：http://uei.fzhhl.top

name="${1:-default}"
来源：http://vxy.9152youxi.cn

[R06] 判断命令是否存在
来源：http://zkr.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mjq.ivvv.top

[R07] if 判断文件
来源：http://iog.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cfl.ehwqpu.com

[R08] 数值比较
来源：http://loo.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xds.yueranfly.top

[R09] 字符串比较
来源：http://sro.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qpm.yongpay.top

[R10] 正则匹配
来源：http://hyt.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://brr.chenlongwang.top

[R11] case 多分支
来源：http://rng.cdnleiting.top

case "$1" in
来源：http://vtx.tarul.cn

start) echo "启动" ;;
来源：http://waf.cucudq.cn

stop)  echo "停止" ;;
来源：http://ldf.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://neb.yj20258888.top

esac
来源：http://ixy.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://txy.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://qbk.shuidangran.top

[R13] for 计数循环
来源：http://bcu.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://wvg.feifeiyinyue.top

[R14] C 风格 for
来源：http://ttx.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uwn.cashguo.top

[R15] while 逐行读文件
来源：http://aly.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bcr.sysykeji.top

[R16] until 等待条件
来源：http://tls.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdw.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://ekg.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aiw.aizwys.cn

[R18] 遍历数组
来源：http://ysy.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oxm.tanke756.top

[R19] 数组长度
来源：http://ykc.uphjek.com

echo "${#arr[@]}"
来源：http://fhm.dashuyun.cn

[R20] 关联数组（字典）
来源：http://evf.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mha.nwbrower.top

[R21] 字符串长度
来源：http://mae.nwbrower.top

echo "${#s}"
来源：http://npw.yuanzhike.top

[R22] 截取子串
来源：http://mbq.cashguo.top

echo "${s:0:5}"
来源：http://yfv.daria6918.cn

[R23] 字符串替换
来源：http://nkk.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lmb.hnqzz.top

[R24] 大小写转换
来源：http://ibz.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gks.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://qro.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lyi.yj202588.top

[R26] 命令替换
来源：http://nhf.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://nvq.wangshuangyany.cn

[R27] 算术展开
来源：http://msn.bbcook.cn

echo $((1 + 2 * 3))
来源：http://fxi.pengpengdd.cyou

[R28] 浮点运算
来源：http://wgw.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://sxb.pengpengdd.cyou

[R29] 定义函数
来源：http://xyi.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gvk.chenlongwang.top

[R30] 函数返回状态码
来源：http://mxm.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://fsl.cdnleiting.top

[R31] 局部变量
来源：http://tfq.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://uwa.redwolf501.top

[R32] 参数个数校验
来源：http://shv.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://elh.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://umv.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvy.meibo888.top

[R34] 退出时清理
来源：http://nve.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://ecl.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://gqc.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ziv.tianlin.xyz

[R36] 并发执行多个任务
来源：http://ymx.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xwz.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://pyn.tian-w.cn

files=$(ls -1)
来源：http://iac.shangyingyoupin.top

[R38] 管道串联
来源：http://yzk.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://bgc.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://ymu.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://oxx.jlsjyb.cn

[R40] 追加写日志
来源：http://jdx.shuidangran.top

echo "log" >> out.log
来源：http://uvn.sufxvd.cn

[R41] 丢弃输出
来源：http://ybb.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://ppb.meibo888.top

[R42] 输入重定向
来源：http://eey.jqgufenzy.top

wc -l < a.txt
来源：http://dsn.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://jlf.cqqwz.cn

find . -name "*.log" -type f
来源：http://htk.yuxming.cn

[R44] 按修改时间查找
来源：http://ztz.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://big.zhixingplan.top

[R45] 批量删除
来源：http://gzb.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://mrp.yfazqb.com

[R46] 递归替换文件内容
来源：http://alu.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vdd.daxiang520.top

[R47] sed 单行替换
来源：http://jtk.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://tgn.mhx1999.top

[R48] awk 取指定列
来源：http://qea.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://ehj.yfazqb.com

[R49] awk 带条件
来源：http://vpk.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hjt.bjfxy.top

[R50] awk 求和
来源：http://lsi.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://qrd.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://hiz.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lvd.quarkkingdee.top

[R52] 统计行数
来源：http://grf.aizwys.cn

wc -l a.txt
来源：http://pfk.sweek.top

[R53] 查看文件头与实时尾
来源：http://cun.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tmv.ydjk.org.cn

[R54] 比较两个文件
来源：http://xla.ehwqpu.com

diff a.txt b.txt
来源：http://dli.fehbvm.com

[R55] 压缩与解压
来源：http://iik.zhongyouzk.top


<!-- 参考信息 -->